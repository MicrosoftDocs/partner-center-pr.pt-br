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
ms.openlocfilehash: 26768bdf33c03145a893fa445eab6ebf92ca9b1c
ms.sourcegitcommit: efd711b0e65c55f24ce5b9636abd7b5a8cc719fe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "108018180"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="850c1-103">Restabelecer privilégios de administrador para assinaturas de CSP do Azure de um cliente</span><span class="sxs-lookup"><span data-stu-id="850c1-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="850c1-104">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="850c1-104">**Appropriate roles**</span></span>

- <span data-ttu-id="850c1-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="850c1-105">Global admin</span></span>
- <span data-ttu-id="850c1-106">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="850c1-106">Admin agent</span></span>

<span data-ttu-id="850c1-107">Na condição de um parceiro CSP, muitas vezes os clientes esperam que você gerencie para eles o uso que eles fazem do Azure e os sistemas deles.</span><span class="sxs-lookup"><span data-stu-id="850c1-107">As a CSP partner your customers often expect that you will manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="850c1-108">Isso exige que você tenha privilégios de administrador.</span><span class="sxs-lookup"><span data-stu-id="850c1-108">Doing so requires you to have admin privileges.</span></span> <span data-ttu-id="850c1-109">Alguns privilégios são concedidos quando seu relacionamento de revendedor com o cliente é estabelecido.</span><span class="sxs-lookup"><span data-stu-id="850c1-109">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="850c1-110">Outros são concedidos a você pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="850c1-110">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="850c1-111">Privilégios de administrador para o Azure no CSP</span><span class="sxs-lookup"><span data-stu-id="850c1-111">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="850c1-112">Há dois níveis de privilégios de administrador para o Azure no CSP.</span><span class="sxs-lookup"><span data-stu-id="850c1-112">There are two levels of admin privileges for Azure in CSP.</span></span>

<span data-ttu-id="850c1-113">**Privilégios de administrador de nível de locatário** (**privilégios de administrador delegado**) – os parceiros CSP obtêm esses privilégios ao estabelecerem o relacionamento de revendedor CSP com os clientes.</span><span class="sxs-lookup"><span data-stu-id="850c1-113">**Tenant level admin privileges** (**Delegated admin privileges**) -  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="850c1-114">Os privilégios de administrador delegado oferecem aos parceiros CSP acesso aos locatários dos clientes deles, para que eles possam realizar funções administrativas, como adicionar/gerenciar usuários, redefinir senhas e gerenciar licenças de usuário.</span><span class="sxs-lookup"><span data-stu-id="850c1-114">Delegated admin privileges give CSP partners access to their customers' tenants, which allows them to perform administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>

<span data-ttu-id="850c1-115">**Privilégios de administrador de nível de assinatura** – os parceiros CSP obtêm esses privilégios ao criar assinaturas do Azure CSP para os clientes deles.</span><span class="sxs-lookup"><span data-stu-id="850c1-115">**Subscription level admin privileges** - CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="850c1-116">A posse desses privilégios fornece aos parceiros do CSP acesso completo a essas assinaturas, o que lhes permite provisionar e gerenciar recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="850c1-116">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-partners-admin-privileges"></a><span data-ttu-id="850c1-117">Restabelecer privilégios de administrador dos parceiros CSP</span><span class="sxs-lookup"><span data-stu-id="850c1-117">Reinstate CSP partners' admin privileges</span></span>

<span data-ttu-id="850c1-118">O cliente pode recriar a atribuição de função do CSP desde que você forneça a ele a ID de objeto do grupo AdminAgents.</span><span class="sxs-lookup"><span data-stu-id="850c1-118">Your customer can re-create the CSP role assignment as long as you provide the object ID of the AdminAgents group to your customer.</span></span> <span data-ttu-id="850c1-119">Para restabelecer os privilégios de administrador delegado, você precisa trabalhar com o cliente.</span><span class="sxs-lookup"><span data-stu-id="850c1-119">To regain delegated admin privileges, you need to work with your customer.</span></span>

1. <span data-ttu-id="850c1-120">Entre no Painel do Partner Center e, no menu do Partner Center, selecione **Clientes**.</span><span class="sxs-lookup"><span data-stu-id="850c1-120">Sign into the Partner Center dashboard and from the Partner Center menu, select **Customers**.</span></span>

2. <span data-ttu-id="850c1-121">Selecione o cliente com o qual você está trabalhando e **solicite um relacionamento de revendedor.**</span><span class="sxs-lookup"><span data-stu-id="850c1-121">Select the customer you are working with and **request a reseller relationship.**</span></span> <span data-ttu-id="850c1-122">Essa ação gera um link para o cliente que tem direitos de administrador de locatários.</span><span class="sxs-lookup"><span data-stu-id="850c1-122">This action generates a link to the customer who has tenant admin rights.</span></span>

3. <span data-ttu-id="850c1-123">O cliente precisa selecionar o link e aprovar a solicitação de relacionamento do revendedor.</span><span class="sxs-lookup"><span data-stu-id="850c1-123">That customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="Exemplo de email para criar relacionamento com o revendedor":::

4. <span data-ttu-id="850c1-125">Você, o parceiro, precisa se conectar ao locatário do parceiro para obter a ID de objeto do grupo AdminAgents.</span><span class="sxs-lookup"><span data-stu-id="850c1-125">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. <span data-ttu-id="850c1-126">O cliente que tem a função de **proprietário ou administrador de acesso do usuário** e tem permissão para criar a atribuição de função no nível da assinatura, faz o seguinte:</span><span class="sxs-lookup"><span data-stu-id="850c1-126">Your customer who has the role of **owner or user access administrator** and has permission to create role assignment at the subscription level does the following:</span></span>


    1. <span data-ttu-id="850c1-127">Conecta-se ao locatário em que se encontra a assinatura do CSP.</span><span class="sxs-lookup"><span data-stu-id="850c1-127">Connects to the tenant where the CSP subscription exists.</span></span>
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. <span data-ttu-id="850c1-128">Conecta-se à assinatura (aplicável somente se o usuário tiver permissões de atribuição de função em várias assinaturas no locatário).</span><span class="sxs-lookup"><span data-stu-id="850c1-128">Connects to the subscription (only applicable if the user has role assignment permissions over multiple subscriptions in the tenant).</span></span>
   
         <span data-ttu-id="850c1-129">PS C:\WINDOWS\system32> Set-AzContext-SubscriptionId "CSP Subscription ID"</span><span class="sxs-lookup"><span data-stu-id="850c1-129">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"\`</span></span>


    3. <span data-ttu-id="850c1-130">Cria a atribuição de função</span><span class="sxs-lookup"><span data-stu-id="850c1-130">Creates the role assignment</span></span>
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


<span data-ttu-id="850c1-131">Se você quer conceder permissões de função de proprietário no nível do grupo de recursos ou no nível do recurso, e não no escopo da assinatura, use os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="850c1-131">If you want to grant owner role permission at resource group level or resource level instead of subscription scope, the following commands can work:</span></span>


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a><span data-ttu-id="850c1-132">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="850c1-132">Next steps</span></span>

- [<span data-ttu-id="850c1-133">Gerenciar assinaturas e recursos no âmbito do plano do Azure</span><span class="sxs-lookup"><span data-stu-id="850c1-133">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
