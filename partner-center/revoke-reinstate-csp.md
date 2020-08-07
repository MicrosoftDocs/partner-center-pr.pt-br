---
title: Restabelecer privilégios de administrador para o CSP do Azure
ms.topic: article
ms.date: 07/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como ajudar os clientes a restabelecer os privilégios de administrador de um parceiro para que ele possa ajudar a gerenciar as assinaturas de CSP do Azure de um cliente.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 2c98ddf67567935a17e33546ce41de723b3be134
ms.sourcegitcommit: d7e620f826cd6570113384c3db34bd96e2f0359b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2020
ms.locfileid: "87412422"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Restabelecer privilégios de administrador para assinaturas de CSP do Azure de um cliente  

**Funções aplicáveis**

- Administrador global
- Agente administrativo

Na condição de um parceiro CSP, muitas vezes os clientes esperam que você gerencie para eles o uso que eles fazem do Azure e os sistemas deles. Isso exige que você tenha privilégios de administrador. Alguns privilégios são concedidos quando seu relacionamento de revendedor com o cliente é estabelecido. Outros são concedidos a você pelo cliente.

## <a name="admin-privileges-for-azure-in-csp"></a>Privilégios de administrador para o Azure no CSP

Há dois níveis de privilégios de administrador para o Azure no CSP.

**Privilégios de administrador de nível de locatário** (**privilégios de administrador delegado**) – os parceiros CSP obtêm esses privilégios ao estabelecerem o relacionamento de revendedor CSP com os clientes. Isso fornece aos parceiros CSP acesso aos locatários dos clientes deles, o que permite que eles executem funções administrativas, tais como adicionar/gerenciar usuários, redefinir senhas e gerenciar licenças de usuário.

**Privilégios de administrador de nível de assinatura** – os parceiros CSP obtêm esses privilégios ao criar assinaturas do Azure CSP para os clientes deles. A posse desses privilégios fornece aos parceiros do CSP acesso completo a essas assinaturas, o que lhes permite provisionar e gerenciar recursos do Azure.

## <a name="reinstate-csp-partners-admin-privileges"></a>Restabelecer privilégios de administrador dos parceiros CSP

Para restabelecer os privilégios de administrador delegado, você precisa trabalhar com o cliente.

1. Entre no painel do Partner Center e, no menu do Partner Center, selecione **Clientes**.

2. Selecione o cliente com o qual você está trabalhando e **solicite um relacionamento de revendedor.** Isso gera um link para o cliente que tem direitos de administrador de locatários.

3. Esse usuário precisa selecionar o link e aprovar a solicitação de relacionamento de revendedor.

   :::image type="content" source="images/azure/revoke4.png" alt-text="relacionamento de revendedor":::

## <a name="adding-the-admin-agents-group-as-an-owner-for-the-azure-csp-subscription"></a>Como adicionar o grupo de agentes administrativos como um proprietário para a assinatura do Azure CSP

O cliente precisará adicionar seu grupo de agentes administrativos como o proprietário da assinatura do Azure CSP.

1. Use o console do PowerShell ou o ISE (ambiente de script integrado) do PowerShell. Verifique se os módulos AzureAD estão instalados.

2. Conecte-se ao seu locatário do Azure AD.

   ```powershell
   Connect-AzureAD
   ```

3. Obtenha o ObjectId dos grupos de agentes administrativos.

   ```powershell
   Get-AzureADGroup
   ```
   As etapas a seguir são executadas pelo usuário na empresa do seu cliente que tem acesso de proprietário à assinatura do Azure CSP.

4. O usuário com acesso de proprietário à assinatura do CSP do Azure entra no Azure usando as próprias credenciais.

   ```powershell
   Connect-AzAccount
   ```

5. Em seguida, ele pode adicionar seu grupo de agentes administrativos como proprietário da assinatura do Azure CSP.

    ```powershell
    New-AzureRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>"
    ```

## <a name="next-steps"></a>Próximas etapas

[Gerenciar assinaturas e recursos no âmbito do plano do Azure](azure-plan-manage.md)
