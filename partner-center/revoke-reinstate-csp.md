---
title: Restabelecer privilégios de administrador para assinaturas do Azure CSP | Partner Center
ms.topic: article
ms.date: 10/15/2019
description: Este documento explica como ajudar os clientes a restabelecer os privilégios de administrador do parceiro
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: High
ms.openlocfilehash: 51f19724751b296789a1d5367d9892b21cab4f09
ms.sourcegitcommit: 646536a113584f1572de851e22a212a6f77e64d7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/01/2019
ms.locfileid: "73433748"
---
# <a name="reinstate-admin-privileges-for-azure-csp-subscriptions"></a>Restabelecer privilégios de administrador para assinaturas do Azure CSP  

**Funções aplicáveis**

- Administração global
- Agente administrador

Na condição de um parceiro CSP, muitas vezes os clientes esperam que você gerencie para eles o uso que eles fazem do Azure e os sistemas deles. Para fazer isso, é necessário ter privilégios de administrador. Alguns privilégios são concedidos quando seu relacionamento de revendedor com o cliente é estabelecido. Outros são concedidos a você pelo cliente.

## <a name="admin-privileges-for-azure-in-csp"></a>Privilégios de administrador para o Azure no CSP 

Há dois níveis de privilégios de administrador para o Azure no CSP. 

**Privilégios de administrador de nível de locatário** (**privilégios de administrador delegado**) – os parceiros CSP obtêm esses privilégios ao estabelecerem o relacionamento de revendedor CSP com os clientes. Isso fornece aos parceiros CSP acesso aos locatários dos clientes deles, o que permite que eles executem funções administrativas, tais como adicionar/gerenciar usuários, redefinir senhas e gerenciar licenças de usuário. 

**Privilégios de administrador de nível de assinatura** – os parceiros CSP obtêm esses privilégios ao criar assinaturas do Azure CSP para os clientes deles. Isso permite acesso completo a essas assinaturas aos parceiros CSP, o que permite que eles provisionem e gerenciem recursos do Azure. 


## <a name="reinstate-csp-partners-admin-privileges"></a>Restabelecer privilégios de administrador dos parceiros CSP

Para restabelecer os privilégios de administrador delegado, você precisa trabalhar com o cliente.
 
 1. Entre no painel do Partner Center e, no menu do Partner Center, selecione **Clientes**.

 2. Selecione o cliente com o qual você está trabalhando e **solicite um relacionamento de revendedor.** Isso gera um link para o cliente que tem direitos de administrador de locatários.

 3. Esse usuário precisa selecionar o link e aprovar a solicitação de relacionamento de revendedor.
 
![relacionamento de revendedor](images/azure/revoke4.png)

## <a name="adding-the-admin-agents-group-as-an-owner-for-the-azure-csp-subscription"></a>Como adicionar o grupo de agentes administrativos como um proprietário para a assinatura do Azure CSP

 O cliente precisará adicionar seu grupo de agentes administrativos como o proprietário da assinatura do Azure CSP.

1. Use o console do PowerShell ou o ISE (ambiente de script integrado) do PowerShell. Verifique se os módulos AzureRM e AzureAD estão instalados. 

2.  Conecte-se ao seu locatário do Azure AD.
Cmdlet do PowerShell: Connect-AzureAD

3.  Obtenha o ObjectId dos grupos de agentes administrativos.
Cmdlet do PowerShell: Get-AzureADGroup`1nn

![grupo de agentes administrativos](images/azure/revoke5.png)

As etapas a seguir são executadas pelo usuário na empresa do seu cliente que tem acesso de proprietário à assinatura do Azure CSP.

4. O usuário com acesso de proprietário à assinatura do Azure CSP entra no Azure Resource Manager usando suas próprias credenciais.

    Cmdlet do PowerShell: Login-AzureRMAccount

5.  Em seguida, ele pode adicionar seu grupo de agentes administrativos como proprietário da assinatura do Azure CSP.

    Cmdlet do PowerShell: New-AzureRMRoleAssignment -ObjectId < ID do objeto que você obteve da etapa 3> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>"

![proprietários de agente administrativo](images/azure/revoke6.png)    

**Para saber mais**

[Gerenciar assinaturas e recursos no âmbito do plano do Azure](azure-plan-manage.md)
