---
title: Restabelecer privilégios de administrador para o CSP do Azure
ms.topic: how-to
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como ajudar os clientes a restabelecer os privilégios de administrador de um parceiro para que ele possa ajudar a gerenciar as assinaturas de CSP do Azure de um cliente.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: f536d975d3c644a7afa29a95a3cb45608f6b2c9f
ms.sourcegitcommit: 89be77c9f35c77463d9558826293202afc6dec56
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/13/2021
ms.locfileid: "107315840"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Restabelecer privilégios de administrador para assinaturas de CSP do Azure de um cliente  

**Funções aplicáveis**

- Administrador global
- Agente administrativo

Na condição de um parceiro CSP, muitas vezes os clientes esperam que você gerencie para eles o uso que eles fazem do Azure e os sistemas deles. Isso exige que você tenha privilégios de administrador. Alguns privilégios são concedidos quando seu relacionamento de revendedor com o cliente é estabelecido. Outros são concedidos a você pelo cliente.

## <a name="admin-privileges-for-azure-in-csp"></a>Privilégios de administrador para o Azure no CSP

Há dois níveis de privilégios de administrador para o Azure no CSP.

**Privilégios de administrador de nível de locatário** (**privilégios de administrador delegado**) – os parceiros CSP obtêm esses privilégios ao estabelecerem o relacionamento de revendedor CSP com os clientes. Os privilégios de administrador delegado fornecem aos parceiros CSP acesso aos locatários dos clientes deles, o que permite que eles executem funções administrativas, tais como adicionar/gerenciar usuários, redefinir senhas e gerenciar licenças de usuário.

**Privilégios de administrador de nível de assinatura** – os parceiros CSP obtêm esses privilégios ao criar assinaturas do Azure CSP para os clientes deles. A posse desses privilégios fornece aos parceiros do CSP acesso completo a essas assinaturas, o que lhes permite provisionar e gerenciar recursos do Azure.

## <a name="reinstate-csp-partners-admin-privileges"></a>Restabelecer privilégios de administrador dos parceiros CSP

O cliente é capaz de recriar a atribuição da função CSP, contanto que você forneça a ele a ID de objeto do grupo AdminAgents. Para restabelecer os privilégios de administrador delegado, você precisa trabalhar com o cliente.

1. Entre no Painel do Partner Center e, no menu do Partner Center, selecione **Clientes**.

2. Selecione o cliente com o qual você está trabalhando e **solicite um relacionamento de revendedor.** Isso gera um link para o cliente que tem direitos de administrador de locatários.

3. O cliente precisa selecionar o link e aprovar a solicitação de relacionamento do revendedor.

   :::image type="content" source="images/azure/revoke4.png" alt-text="Exemplo de email para criar relacionamento com o revendedor":::

4. Você, o parceiro, precisa se conectar ao locatário do parceiro para obter a ID de objeto do grupo AdminAgents.

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. O cliente que tem a função de **proprietário ou administrador de acesso do usuário** e tem permissão para criar a atribuição de função no nível da assinatura, faz o seguinte:


    1. Conecta-se ao locatário em que se encontra a assinatura do CSP.
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. Conecta-se à assinatura (aplicável somente se o usuário tiver permissões de atribuição de função em várias assinaturas no locatário).
   
         PS C:\WINDOWS\system32> Set-AzContext-SubscriptionId "CSP Subscription ID"


    3. Cria a atribuição de função
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


Se o desejo for conceder permissões de função de proprietário no nível do grupo de recursos ou no nível do recurso em vez do escopo da assinatura, os seguintes comandos poderão funcionar:


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a>Próximas etapas

- [Gerenciar assinaturas e recursos no âmbito do plano do Azure](azure-plan-manage.md)
