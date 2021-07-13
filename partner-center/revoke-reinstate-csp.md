---
title: Restabelecer privilégios de administrador para o CSP do Azure
ms.topic: how-to
ms.date: 05/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como ajudar os clientes a restabelecer os privilégios de administrador de um parceiro para que ele possa ajudar a gerenciar as assinaturas de CSP (Provedor de Soluções de Nuvem) do Azure de um cliente.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 196b38d30942278beb00096529f5965db7dfb96c
ms.sourcegitcommit: b55f63a029d88c73cd5190bbac2df1b5990e6e44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2021
ms.locfileid: "113510169"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Restabelecer privilégios de administrador para assinaturas de CSP do Azure de um cliente  

**Funções apropriadas**: Administração global | Agente de administração

Na condição de um parceiro CSP (Provedor de Soluções na Nuvem), muitas vezes os clientes esperam que você gerencie para eles o uso que eles fazem do Azure e os sistemas deles. Você precisa ter privilégios de administrador para fazer isso. Alguns privilégios são concedidos quando seu relacionamento de revendedor com o cliente é estabelecido. Outros são concedidos a você pelo cliente.

## <a name="admin-privileges-for-azure-in-csp"></a>Privilégios de administrador para o Azure no CSP

Há dois níveis de privilégios de administrador para o Azure no CSP.

- **Privilégios de administrador de nível de locatário (privilégios de administrador delegado)** : os parceiros CSP obtêm esses privilégios ao estabelecerem o relacionamento de revendedor CSP com os clientes. Os privilégios de administrador delegado fornecem aos parceiros CSP acesso aos locatários dos clientes deles. Esse acesso permite que eles desempenhem funções administrativas, como adicionar/gerenciar usuários, redefinir senhas e gerenciar licenças dos usuários.
- **Privilégios de administrador de nível de assinatura**: os parceiros CSP obtêm esses privilégios ao criar assinaturas do CSP do Azure para os clientes deles. A posse desses privilégios fornece aos parceiros do CSP acesso completo a essas assinaturas, o que lhes permite provisionar e gerenciar recursos do Azure.

## <a name="reinstate-csp-a-partners-admin-privileges"></a>Reaplicar ao CSP os privilégios de administrador de um parceiro

O cliente poderá recriar a atribuição de função do CSP se você fornecer o `object ID` do grupo AdminAgents ao seu cliente. Para restabelecer os privilégios de administrador delegado, você precisa trabalhar com o cliente por meio das etapas a seguir.

1. Entre no painel do Partner Center.

2. No menu do Partner Center, selecione **Clientes**.

3. Selecione o cliente com o qual você está trabalhando e **solicite um relacionamento de revendedor**. Essa ação gera um link para o cliente que tem direitos de administrador de locatários.

4. Seu cliente precisa selecionar o link e aprovar a solicitação de relacionamento do revendedor.

   :::image type="content" source="images/azure/revoke4.png" alt-text="Exemplo de email para criar relacionamento com o revendedor":::.

5. Você, o parceiro, precisa se conectar ao locatário do parceiro para obter a ID de objeto do grupo AdminAgents.
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

6. O cliente precisa executar as etapas a seguir usando o PowerShell ou a CLI do Azure. O cliente precisa ter:

- A função de **proprietário** ou **administrador de acesso do usuário** 
- Permissões para criar atribuições de função no nível da assinatura

   a. Somente para o PowerShell, o cliente precisa atualizar o módulo `Az.Resources`.
   ```powershell
   Update-Module Az.Resources
   ```

   b. O cliente se conecta ao locatário em que a assinatura do CSP existe.
   ```powershell
   Connect-AzAccount -TenantID "<Customer tenant>"
   ```
   ```azurecli
   az login --tenant <Customer tenant>
   ```

   c. O cliente se conecta à assinatura. Isso será aplicável *somente* se o usuário tiver permissões de atribuição de função em várias assinaturas no locatário.

   ```powershell
   Set-AzContext -SubscriptionID <"CSP Subscription ID">
   ```
   ```azurecli
   az account set --subscription <CSP Subscription ID>
   ```

   d. O cliente criará a atribuição de função.
    
   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the Admin Agents group provided by partner>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>"
   ```

Em vez de conceder permissões de proprietário no escopo da assinatura, você pode conceder no nível de recurso ou grupo de recursos. 

- No nível do grupo de recursos

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- No nível do recurso

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "<Resource URI>"
   ```

Se as etapas acima não funcionarem ou se você receber erros ao tentar segui-las, experimente o procedimento "catch-all" a seguir para restabelecer os direitos de administrador para o cliente.

```powershell
Install-Module -Name Az.Resources -Force -Verbose
Import-Module -Name Az.Resources -Verbose -MinimumVersion 4.1.1
Connect-AzAccount -Tenant <customer tenant>
Set-AzContext -SubscriptionId <customer subscriptions>
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup"
```

### <a name="troubleshooting"></a>Solução de problemas

Se o cliente não conseguir concluir a etapa 6 acima, faça com que ele experimente o seguinte comando:

```powershell
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<costumer subscription>" -ObjectType "ForeignGroup" -Debug > newRoleAssignment.log
```

Forneça o arquivo `newRoleAssignment.log` resultante à Microsoft para análise posterior.

Se o procedimento "catch-all" falhar durante o `Import-Module`, experimente as seguintes etapas:
- Se a importação falhar porque o módulo está em uso, reinicie a sessão do PowerShell fechando e reabrindo todas as janelas.
- Verifique a versão do `Az.Resources` com `Get-Module Az.Resources -ListAvailable`.
- Se a versão 4.1.1 não estiver na lista disponível, você precisará usar `Update-Module Az.Resources -Force`.
- Se o erro informar que `Az.Accounts` precisa ser uma versão específica, atualize esse módulo também, substituindo `Az.Resources` por `Az.Accounts`. Em seguida, você precisa reiniciar a sessão do PowerShell.


## <a name="next-steps"></a>Próximas etapas

- [Gerenciar assinaturas e recursos no âmbito do plano do Azure](azure-plan-manage.md)
