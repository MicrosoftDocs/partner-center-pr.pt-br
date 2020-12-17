---
title: Restabelecer privilégios de administrador para o CSP do Azure
ms.topic: how-to
ms.date: 07/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como ajudar os clientes a restabelecer os privilégios de administrador de um parceiro para que ele possa ajudar a gerenciar as assinaturas de CSP do Azure de um cliente.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 13fdeb01ecd73dc1a63d174a4ad5cb8e1bdc813a
ms.sourcegitcommit: 455894365fa488368f7572ac72312e84a267ef5e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2020
ms.locfileid: "97011495"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="82274-103">Restabelecer privilégios de administrador para assinaturas de CSP do Azure de um cliente</span><span class="sxs-lookup"><span data-stu-id="82274-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="82274-104">**Funções aplicáveis**</span><span class="sxs-lookup"><span data-stu-id="82274-104">**Applicable roles**</span></span>

- <span data-ttu-id="82274-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="82274-105">Global admin</span></span>
- <span data-ttu-id="82274-106">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="82274-106">Admin agent</span></span>

<span data-ttu-id="82274-107">Na condição de um parceiro CSP, muitas vezes os clientes esperam que você gerencie para eles o uso que eles fazem do Azure e os sistemas deles.</span><span class="sxs-lookup"><span data-stu-id="82274-107">As a CSP partner your customers often expect that you will manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="82274-108">Isso exige que você tenha privilégios de administrador.</span><span class="sxs-lookup"><span data-stu-id="82274-108">Doing so requires you to have admin privileges.</span></span> <span data-ttu-id="82274-109">Alguns privilégios são concedidos quando seu relacionamento de revendedor com o cliente é estabelecido.</span><span class="sxs-lookup"><span data-stu-id="82274-109">Some privileges are granted these when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="82274-110">Outros são concedidos a você pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="82274-110">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="82274-111">Privilégios de administrador para o Azure no CSP</span><span class="sxs-lookup"><span data-stu-id="82274-111">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="82274-112">Há dois níveis de privilégios de administrador para o Azure no CSP.</span><span class="sxs-lookup"><span data-stu-id="82274-112">There are two levels of admin privileges for Azure in CSP.</span></span>

<span data-ttu-id="82274-113">**Privilégios de administrador de nível de locatário** (**privilégios de administrador delegado**) – os parceiros CSP obtêm esses privilégios ao estabelecerem o relacionamento de revendedor CSP com os clientes.</span><span class="sxs-lookup"><span data-stu-id="82274-113">**Tenant level admin privileges** (**Delegated admin privileges**) -  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="82274-114">Isso fornece aos parceiros CSP acesso aos locatários dos clientes deles, o que permite que eles executem funções administrativas, tais como adicionar/gerenciar usuários, redefinir senhas e gerenciar licenças de usuário.</span><span class="sxs-lookup"><span data-stu-id="82274-114">This gives CSP partners access to their customers' tenants, which allows them to perform administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>

<span data-ttu-id="82274-115">**Privilégios de administrador de nível de assinatura** – os parceiros CSP obtêm esses privilégios ao criar assinaturas do Azure CSP para os clientes deles.</span><span class="sxs-lookup"><span data-stu-id="82274-115">**Subscription level admin privileges** - CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="82274-116">A posse desses privilégios fornece aos parceiros do CSP acesso completo a essas assinaturas, o que lhes permite provisionar e gerenciar recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="82274-116">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-partners-admin-privileges"></a><span data-ttu-id="82274-117">Restabelecer privilégios de administrador dos parceiros CSP</span><span class="sxs-lookup"><span data-stu-id="82274-117">Reinstate CSP partners' admin privileges</span></span>

<span data-ttu-id="82274-118">Para restabelecer os privilégios de administrador delegado, você precisa trabalhar com o cliente.</span><span class="sxs-lookup"><span data-stu-id="82274-118">To regain delegated admin privileges, you need to work with your customer.</span></span>

1. <span data-ttu-id="82274-119">Entre no painel do Partner Center e, no menu do Partner Center, selecione **Clientes**.</span><span class="sxs-lookup"><span data-stu-id="82274-119">Sign in to Partner Center dashboard and from the Partner Center menu, select **Customers**.</span></span>

2. <span data-ttu-id="82274-120">Selecione o cliente com o qual você está trabalhando e **solicite um relacionamento de revendedor.**</span><span class="sxs-lookup"><span data-stu-id="82274-120">Select the customer you are working with and **request a reseller relationship.**</span></span> <span data-ttu-id="82274-121">Isso gera um link para o cliente que tem direitos de administrador de locatários.</span><span class="sxs-lookup"><span data-stu-id="82274-121">This generates a link to the customer who has tenant admin rights.</span></span>

3. <span data-ttu-id="82274-122">Esse usuário precisa selecionar o link e aprovar a solicitação de relacionamento de revendedor.</span><span class="sxs-lookup"><span data-stu-id="82274-122">That user needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="relacionamento de revendedor":::

## <a name="adding-the-admin-agents-group-as-an-owner-for-the-azure-csp-subscription"></a><span data-ttu-id="82274-124">Como adicionar o grupo de agentes administrativos como um proprietário para a assinatura do Azure CSP</span><span class="sxs-lookup"><span data-stu-id="82274-124">Adding the admin agents group as an owner for the Azure CSP subscription</span></span>

<span data-ttu-id="82274-125">O cliente precisará adicionar o grupo de agente de administração como proprietário de uma assinatura do CSP do Azure, de um Grupo de Recursos ou de um recurso.</span><span class="sxs-lookup"><span data-stu-id="82274-125">Your customer will need to add your admin agent group as the owner of a Azure CSP subscription, a Resource group or a resource.</span></span> 

1. <span data-ttu-id="82274-126">Use o console do PowerShell ou o ISE (ambiente de script integrado) do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="82274-126">Use either PowerShell Console or PowerShell Integrated Scripting Environment(ISE).</span></span> <span data-ttu-id="82274-127">Verifique se os módulos AzureAD estão instalados.</span><span class="sxs-lookup"><span data-stu-id="82274-127">Ensure that AzureAD modules are installed.</span></span>

2. <span data-ttu-id="82274-128">Conecte-se ao seu locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="82274-128">Connect to your Azure AD Tenant.</span></span>

   ```powershell
   Connect-AzureAD
   ```

3. <span data-ttu-id="82274-129">Obtenha o ObjectId dos grupos de agentes administrativos.</span><span class="sxs-lookup"><span data-stu-id="82274-129">Get ObjectId of the Admin Agents groups.</span></span>

   ```powershell
   Get-AzureADGroup
   ```
   <span data-ttu-id="82274-130">As etapas a seguir são executadas pelo usuário na empresa do seu cliente que tem acesso de proprietário à assinatura do Azure CSP.</span><span class="sxs-lookup"><span data-stu-id="82274-130">The following steps are performed by the user in your customer's company who has owner access to the Azure CSP subscription.</span></span>

4. <span data-ttu-id="82274-131">O usuário com acesso de proprietário à assinatura do CSP do Azure entra no Azure usando as próprias credenciais.</span><span class="sxs-lookup"><span data-stu-id="82274-131">The user with owner access to the Azure CSP subscription, signs into Azure using her credentials.</span></span>

   ```powershell
   Connect-AzureRmAccount
   ```

5. <span data-ttu-id="82274-132">Em seguida, ela pode adicionar seu grupo de agente de administração como proprietário à assinatura do CSP do Azure, ao grupo de recursos ou ao recurso aplicando um URI de recurso apropriado no parâmetro de escopo.</span><span class="sxs-lookup"><span data-stu-id="82274-132">She can then add your admin agent group as owner to the CSP Azure subscription, Resource group or Resource by applying a proper Resource Uri in Scope parameter.</span></span> 

    ```powershell
    # Grant owner role at subscription level
    New-AzureRmRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>"

    # Grant owner role at resource group level
    New-AzureRmRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>/resourceGroups/<Resource group name>"

    # Grant owner role at resource level
    New-AzureRmRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "<Resource Uri>"
    ```

## <a name="next-steps"></a><span data-ttu-id="82274-133">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="82274-133">Next steps</span></span>

[<span data-ttu-id="82274-134">Gerenciar assinaturas e recursos no âmbito do plano do Azure</span><span class="sxs-lookup"><span data-stu-id="82274-134">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
