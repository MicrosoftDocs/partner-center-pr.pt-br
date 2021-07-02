---
title: Criar e gerenciar dados Azure Marketplace privado no portal do Azure
description: Saiba mais sobre como criar e gerenciar Azure Marketplace privado (versão prévia) no portal do Azure. A Azure Marketplace privada (versão prévia) permite que os administradores controlem quais soluções de terceiros seus usuários podem usar.
ms.service: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 02/24/2021
ms.openlocfilehash: 8a3ffbe5b57c49004518341d27c785dcd1b9ce87
ms.sourcegitcommit: c4601069340445135b551fa96bee6d9923d8aa97
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2021
ms.locfileid: "113173686"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a><span data-ttu-id="0bb48-104">Criar e gerenciar dados Azure Marketplace privado no portal do Azure</span><span class="sxs-lookup"><span data-stu-id="0bb48-104">Create and manage Private Azure Marketplace in the Azure portal</span></span>

<span data-ttu-id="0bb48-105">A Azure Marketplace privada permite que os administradores controlem quais soluções de terceiros seus usuários podem usar.</span><span class="sxs-lookup"><span data-stu-id="0bb48-105">Private Azure Marketplace lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="0bb48-106">Ele faz isso permitindo que o usuário implante apenas ofertas aprovadas pelo administrador e que estão em conformidade com as políticas da sua empresa.</span><span class="sxs-lookup"><span data-stu-id="0bb48-106">It does this by allowing the user to deploy only offers that are approved by the administrator and comply with your enterprise's policies.</span></span> <span data-ttu-id="0bb48-107">Com o private Azure Marketplace, os usuários podem pesquisar ofertas em conformidade na loja online para comprar e implantar.</span><span class="sxs-lookup"><span data-stu-id="0bb48-107">With Private Azure Marketplace, users can search the online store for compliant offers to purchase and deploy.</span></span>

<span data-ttu-id="0bb48-108">Como administrador do Marketplace (função atribuída), você começará com um Armazenamento Privado desabilitado e vazio, no qual poderá adicionar suas ofertas e planos aprovados.</span><span class="sxs-lookup"><span data-stu-id="0bb48-108">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="0bb48-109">Este artigo explica como atribuir a função necessária, criar um armazenamento privado, gerenciar itens, aprovar solicitações de usuário e habilitar o Azure Marketplace privado para seus usuários.</span><span class="sxs-lookup"><span data-stu-id="0bb48-109">This article explains how to assign the needed role, create a private store, manage items, approve user requests, and enable Private Azure Marketplace for your users.</span></span>

> [!NOTE]
> - <span data-ttu-id="0bb48-110">O Azure Marketplace privado está em um nível de locatário, portanto, todos os usuários no locatário verão a mesma lista de convidados.</span><span class="sxs-lookup"><span data-stu-id="0bb48-110">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
> - <span data-ttu-id="0bb48-111">Todas as soluções da Microsoft (incluindo [Distribuições endossadas](/azure/virtual-machines/linux/endorsed-distros)do Linux ) são adicionadas automaticamente ao Private Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="0bb48-111">All Microsoft solutions (including [Endorsed Linux Distributions](/azure/virtual-machines/linux/endorsed-distros)) are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="0bb48-112">Atribuir a função de administrador do Marketplace</span><span class="sxs-lookup"><span data-stu-id="0bb48-112">Assign the Marketplace admin role</span></span>

<span data-ttu-id="0bb48-113">O locatário Administrador global deve atribuir a função de administrador do **Marketplace** ao administrador Azure Marketplace privado que gerenciará o armazenamento privado.</span><span class="sxs-lookup"><span data-stu-id="0bb48-113">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="0bb48-114">O acesso ao gerenciamento Azure Marketplace privado só está disponível para administradores de IT com a função de administrador do Marketplace atribuída.</span><span class="sxs-lookup"><span data-stu-id="0bb48-114">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="0bb48-115">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0bb48-115">Prerequisites</span></span>

<span data-ttu-id="0bb48-116">Esses pré-requisitos são necessários antes que você possa atribuir a função administrador do Marketplace a um usuário no escopo do locatário:</span><span class="sxs-lookup"><span data-stu-id="0bb48-116">These prerequisites are required before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="0bb48-117">Você tem acesso a um **Administrador global** usuário.</span><span class="sxs-lookup"><span data-stu-id="0bb48-117">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="0bb48-118">O locatário tem pelo menos uma assinatura (pode ser qualquer tipo).</span><span class="sxs-lookup"><span data-stu-id="0bb48-118">The tenant has at least one subscription (can be any type).</span></span>
- <span data-ttu-id="0bb48-119">O Administrador global usuário recebe a **função** Colaborador ou superior para a assinatura escolhida.</span><span class="sxs-lookup"><span data-stu-id="0bb48-119">The Global administrator user is assigned the **Contributor** role or higher for the chosen subscription.</span></span>

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a><span data-ttu-id="0bb48-120">Atribuir a função de administrador do Marketplace com controle de acesso (IAM)</span><span class="sxs-lookup"><span data-stu-id="0bb48-120">Assign the Marketplace admin role with access control (IAM)</span></span>

1. <span data-ttu-id="0bb48-121">Entre no [portal do Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="0bb48-121">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

1. <span data-ttu-id="0bb48-122">Selecione **Todos os serviços** e, em seguida, **Marketplace.**</span><span class="sxs-lookup"><span data-stu-id="0bb48-122">Select **All services** and then **Marketplace**.</span></span>

1. <span data-ttu-id="0bb48-123">Selecione **Marketplace Privado** no menu à esquerda.</span><span class="sxs-lookup"><span data-stu-id="0bb48-123">Select **Private Marketplace** from the menu on the left.</span></span>

   :::image type="content" source="media/private-azure/private-marketplace.png" lightbox="media/private-azure/private-marketplace-zoom.png" alt-text="Mostra a opção de menu do marketplace privado no lado esquerdo do Marketplace.":::

1. <span data-ttu-id="0bb48-125">Selecione **Controle de acesso (IAM)** para atribuir a função de administrador do Marketplace.</span><span class="sxs-lookup"><span data-stu-id="0bb48-125">Select **Access control (IAM)** to assign the Marketplace admin role.</span></span>

   :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Mostra a tela controle de acesso I A M.":::

1. <span data-ttu-id="0bb48-127">Selecione **+Adicionar** > **Adicionar atribuição de função**.</span><span class="sxs-lookup"><span data-stu-id="0bb48-127">Select **+ Add** > **Add role assignment**.</span></span>

1. <span data-ttu-id="0bb48-128">Em **Função**, escolha Administrador **do Marketplace.**</span><span class="sxs-lookup"><span data-stu-id="0bb48-128">Under **Role**, choose **Marketplace Admin**.</span></span>

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Mostra o menu Atribuição de função.":::

1. <span data-ttu-id="0bb48-130">Selecione o usuário desejado na lista suspenso e, em seguida, selecione **Feito.**</span><span class="sxs-lookup"><span data-stu-id="0bb48-130">Select the desired user from the dropdown list, then select **Done**.</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="0bb48-131">Atribuir a função de administrador do Marketplace com o PowerShell</span><span class="sxs-lookup"><span data-stu-id="0bb48-131">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="0bb48-132">Use o script do PowerShell a seguir para atribuir a função de Administrador do Marketplace; ele requer os seguintes parâmetros:</span><span class="sxs-lookup"><span data-stu-id="0bb48-132">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="0bb48-133">**TenantId:** A ID do locatário no escopo (a função de administrador do Marketplace é atribuível no escopo do locatário).</span><span class="sxs-lookup"><span data-stu-id="0bb48-133">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="0bb48-134">**SubscriptionId:** Uma assinatura da qual o administrador global tem **a função Colaborador** ou mais atribuída.</span><span class="sxs-lookup"><span data-stu-id="0bb48-134">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="0bb48-135">**GlobalAdminUsername:** O nome de usuário do administrador global.</span><span class="sxs-lookup"><span data-stu-id="0bb48-135">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="0bb48-136">**UsernameToAssignRoleFor:** O nome de usuário ao qual a função de administrador do Marketplace será atribuída.</span><span class="sxs-lookup"><span data-stu-id="0bb48-136">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="0bb48-137">Para usuários convidados para o locatário, pode levar até 48 horas até que sua conta seja disponibilizada para atribuir a função de Administrador do Marketplace.</span><span class="sxs-lookup"><span data-stu-id="0bb48-137">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace Admin role.</span></span> <span data-ttu-id="0bb48-138">Para obter mais informações, consulte [Propriedades de um usuário Azure Active Directory colaboração B2B](/azure/active-directory/b2b/user-properties).</span><span class="sxs-lookup"><span data-stu-id="0bb48-138">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

```PowerShell
function Assign-MarketplaceAdminRole { 
[CmdletBinding()] 
param( 
[Parameter(Mandatory)] 
[string]$TenantId, 
 
[Parameter(Mandatory)] 
[string]$SubscriptionId, 

 

[Parameter(Mandatory)] 
[string]$GlobalAdminUsername, 

 

[Parameter(Mandatory)] 
[string]$UsernameToAssignRoleFor 
) 

$MarketplaceAdminRoleDefinitionName = "Marketplace Admin" 

 

Write-Output "TenantId = $TenantId" 
Write-Output "SubscriptionId = $SubscriptionId" 
Write-Output "GlobalAdminUsername = $GlobalAdminUsername" 
Write-Output "UsernameToAssignRoleFor = $UsernameToAssignRoleFor" 

 

Write-Output "$($GlobalAdminUsername) is about to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)" 

 

$profile = Connect-AzAccount -Tenant $TenantId -SubscriptionId $SubscriptionId

 

 
if($profile -eq $null) 
{ 
Write-Error -Message "Failed to connect to tenant and/or subscription" -ErrorAction Stop 
} 
elseif($profile.Context.Account.Id -ne $GlobalAdminUsername) 
{ 
Write-Error "Connected with $($profile.Context.Account.Id) instead of with the global admin that was specified in the script parameters, which is $($GlobalAdminUsername)" 
} 
else 
{ 
Write-Output "$($GlobalAdminUsername) was connected successfully to Tenant=$($profile.Context.Tenant), Subscription=$($profile.Context.Subscription), AccountId=$($profile.Context.Account.Id), Environment=$($profile.Context.Environment)" 
} 

 

$MarketPlaceAdminRole = Get-AzRoleDefinition $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace"

 

if($MarketPlaceAdminRole -eq $null) 
{ 
Write-Error -Message "'$($MarketplaceAdminRoleDefinitionName)' role is not available" -ErrorAction Stop 
} 
else 
{ 
Write-Output -Message "'$($MarketplaceAdminRoleDefinitionName)' role is available" 
} 

 

Write-Output -Message "About to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)..." 

New-AzRoleAssignment -SignInName $UsernameToAssignRoleFor -RoleDefinitionName $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace" 

} 

Assign-MarketplaceAdminRole 
```

<span data-ttu-id="0bb48-139">Para obter mais informações sobre os cmdlets contidos no módulo do PowerShell do Az.Portal, [consulte Microsoft Azure PowerShell: cmdlets do Painel do Portal](/powershell/module/az.portal/).</span><span class="sxs-lookup"><span data-stu-id="0bb48-139">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="0bb48-140">Criar uma conta Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="0bb48-140">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="0bb48-141">Entre no [portal do Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="0bb48-141">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="0bb48-142">Selecione **Todos os serviços** e, em seguida, **Marketplace.**</span><span class="sxs-lookup"><span data-stu-id="0bb48-142">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Mostra a portal do Azure principal.":::

3. <span data-ttu-id="0bb48-144">Selecione **Marketplace Privado** no menu à esquerda.</span><span class="sxs-lookup"><span data-stu-id="0bb48-144">Select **Private Marketplace** from the menu on the left.</span></span>

4. <span data-ttu-id="0bb48-145">Selecione **Introdução** para criar Azure Marketplace privado (você só precisa fazer isso uma vez).</span><span class="sxs-lookup"><span data-stu-id="0bb48-145">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Mostra como selecionar o &quot;Introdução na janela portal do Azure&quot; principal.":::

    <span data-ttu-id="0bb48-147">Se o Azure Marketplace privado já existir para esse locatário, **Gerenciar Marketplace** será selecionado por padrão.</span><span class="sxs-lookup"><span data-stu-id="0bb48-147">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="0bb48-148">Depois de concluído, você terá uma conta privada vazia e desabilitada Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="0bb48-148">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Mostra a tela de Azure Marketplace privada vazia.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="0bb48-150">Adicionar itens da galeria</span><span class="sxs-lookup"><span data-stu-id="0bb48-150">Add items from gallery</span></span>

<span data-ttu-id="0bb48-151">Um item é uma combinação de uma oferta e um plano.</span><span class="sxs-lookup"><span data-stu-id="0bb48-151">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="0bb48-152">Você pode pesquisar e adicionar itens na página Gerenciar Marketplace.</span><span class="sxs-lookup"><span data-stu-id="0bb48-152">You can search for and add items on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="0bb48-153">Selecione **Adicionar itens**.</span><span class="sxs-lookup"><span data-stu-id="0bb48-153">Select **Add items**.</span></span>

2. <span data-ttu-id="0bb48-154">Navegue **pela Galeria** ou use o campo de pesquisa para encontrar o item que você deseja.</span><span class="sxs-lookup"><span data-stu-id="0bb48-154">Browse the **Gallery** or use the search field to find the item you want.</span></span>

   :::image type="content" source="media/private-azure/marketplace-gallery.png" lightbox="media/private-azure/marketplace-gallery-zoom.png" alt-text="Mostra como procurar na galeria ou usar o campo de pesquisa.":::

3. <span data-ttu-id="0bb48-156">Por padrão, ao adicionar uma nova oferta, todos os planos atuais serão adicionados à lista aprovada.</span><span class="sxs-lookup"><span data-stu-id="0bb48-156">As default, when adding a new offer, all current plans will be added to the approved list.</span></span> <span data-ttu-id="0bb48-157">Para modificar a seleção de plano antes de adicionar os itens selecionados, selecione o menu suspenso no peças da oferta e atualize os planos necessários.</span><span class="sxs-lookup"><span data-stu-id="0bb48-157">To modify the plan selection before adding the selected items, select the drop-down menu in the offer's tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Mostra como atualizar os planos necessários.":::

4. <span data-ttu-id="0bb48-159">Selecione **Feito** na parte inferior esquerda depois de fazer suas seleções.</span><span class="sxs-lookup"><span data-stu-id="0bb48-159">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="0bb48-160">**Adicionar itens** ao Marketplace estará disponível apenas para ofertas que não são da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0bb48-160">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="0bb48-161">As soluções da Microsoft (incluindo [Distribuições endossadas](/azure/virtual-machines/linux/endorsed-distros)do Linux ) serão marcadas como "Aprovadas por padrão" e não poderão ser gerenciadas no Marketplace Privado.</span><span class="sxs-lookup"><span data-stu-id="0bb48-161">Microsoft solutions (including [Endorsed Linux Distributions](/azure/virtual-machines/linux/endorsed-distros)) will be tagged as "Approved by default" and cannot be managed in Private Marketplace.</span></span>

## <a name="edit-items-plans"></a><span data-ttu-id="0bb48-162">Editar planos do item</span><span class="sxs-lookup"><span data-stu-id="0bb48-162">Edit item's plans</span></span>

<span data-ttu-id="0bb48-163">Você pode editar os planos de um item na página Gerenciar Marketplace.</span><span class="sxs-lookup"><span data-stu-id="0bb48-163">You can edit an item's plans on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="0bb48-164">Na coluna **Planos,** revise os planos disponíveis no menu suspenso desse item.</span><span class="sxs-lookup"><span data-stu-id="0bb48-164">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>

2. <span data-ttu-id="0bb48-165">Marque ou des marque as caixas de seleção para escolher quais planos disponibilizar aos usuários.</span><span class="sxs-lookup"><span data-stu-id="0bb48-165">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

   :::image type="content" source="media/private-azure/edit-items.png" alt-text="Mostra como selecionar ou limpar a caixa de seleção do item necessário.":::

   > [!NOTE]
   > <span data-ttu-id="0bb48-167">Cada oferta precisa de pelo menos um plano selecionado para que a atualização ocorra.</span><span class="sxs-lookup"><span data-stu-id="0bb48-167">Each offer needs at least one plan selected for the update to occur.</span></span> <span data-ttu-id="0bb48-168">Para remover todos os planos relacionados a uma oferta, exclua a oferta inteira (consulte a próxima seção).</span><span class="sxs-lookup"><span data-stu-id="0bb48-168">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="0bb48-169">Excluir ofertas</span><span class="sxs-lookup"><span data-stu-id="0bb48-169">Delete offers</span></span>

<span data-ttu-id="0bb48-170">Na página Gerenciar Marketplace, marque a caixa de seleção ao lado do nome da oferta (veja a tela acima) e **selecione Excluir itens**.</span><span class="sxs-lookup"><span data-stu-id="0bb48-170">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="0bb48-171">Habilitar/desabilitar a Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="0bb48-171">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="0bb48-172">Na página Gerenciar Marketplace, você verá uma dessas faixas, que mostram o estado atual do aplicativo Azure Marketplace:</span><span class="sxs-lookup"><span data-stu-id="0bb48-172">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Mostra a faixa &quot;Desabilitar estado&quot;.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Mostra a faixa &quot;Habilitar estado&quot;.":::

<span data-ttu-id="0bb48-175">Você pode habilitar ou desabilitar a Azure Marketplace privada conforme necessário.</span><span class="sxs-lookup"><span data-stu-id="0bb48-175">You can enable or disable Private Azure Marketplace as needed.</span></span>

- <span data-ttu-id="0bb48-176">Se desabilitado, selecione **Habilitar Marketplace Privado** para habilitar.</span><span class="sxs-lookup"><span data-stu-id="0bb48-176">If disabled, select **Enable Private Marketplace** to enable.</span></span>
- <span data-ttu-id="0bb48-177">Se habilitado, selecione **Desabilitar Marketplace Privado** para desabilitar.</span><span class="sxs-lookup"><span data-stu-id="0bb48-177">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="private-azure-marketplace-notification-center"></a><span data-ttu-id="0bb48-178">Central de Azure Marketplace privada</span><span class="sxs-lookup"><span data-stu-id="0bb48-178">Private Azure Marketplace notification center</span></span>

<span data-ttu-id="0bb48-179">O Centro de Notificações consiste em três tipos de notificações e permite que o administrador do Marketplace tome medidas com base na notificação:</span><span class="sxs-lookup"><span data-stu-id="0bb48-179">Notification Center consists of three types of notifications and allows the Marketplace admin to take actions based on the notification:</span></span>

- <span data-ttu-id="0bb48-180">Solicitações de aprovação de usuários para itens que não estão na lista aprovada (consulte [Solicitação para adicionar ofertas ou planos](#request-to-add-offers-or-plans) abaixo).</span><span class="sxs-lookup"><span data-stu-id="0bb48-180">Approval requests from users for items that are not in the approved list (see [Request to add offers or plans](#request-to-add-offers-or-plans) below).</span></span>
- <span data-ttu-id="0bb48-181">Novas notificações de plano para ofertas que já têm um ou mais planos na lista aprovada.</span><span class="sxs-lookup"><span data-stu-id="0bb48-181">New plan notifications for offers that already have one or more plans in the approved list.</span></span>
- <span data-ttu-id="0bb48-182">Remoção das notificações de plano para itens que estão na lista aprovada, mas que foram removidas do Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="0bb48-182">Removed plan notifications for items that are in the approved list but were removed from the global Azure Marketplace.</span></span>

<span data-ttu-id="0bb48-183">Para acessar o centro de notificações:</span><span class="sxs-lookup"><span data-stu-id="0bb48-183">To access the notification center:</span></span>

1. <span data-ttu-id="0bb48-184">Selecione **Notificações no** menu do lado esquerdo.</span><span class="sxs-lookup"><span data-stu-id="0bb48-184">Select **Notifications** from the left-side menu.</span></span>

   :::image type="content" source="media/private-azure/marketplace-notifications-small.png" lightbox="media/private-azure/marketplace-notifications.png" alt-text="Mostra o menu Notificações.":::

1. <span data-ttu-id="0bb48-186">Selecione o menu de reellipse para obter mais ações.</span><span class="sxs-lookup"><span data-stu-id="0bb48-186">Select the ellipsis menu for more actions.</span></span>

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Mostra os resultados do menu Mais Opções.":::

1. <span data-ttu-id="0bb48-188">Para solicitações de plano, **Mostrar solicitações** abre o formulário de solicitação de aprovação, no qual você pode revisar todas as solicitações de usuário para a oferta específica.</span><span class="sxs-lookup"><span data-stu-id="0bb48-188">For plan requests, **Show requests** opens the approval request form where you can review all user requests for the specific offer.</span></span>
1. <span data-ttu-id="0bb48-189">Selecione **Aprovar** ou **Rejeitar**.</span><span class="sxs-lookup"><span data-stu-id="0bb48-189">Select **Approve** or **Reject**.</span></span>

   :::image type="content" source="media/private-azure/notifications-approve-reject-small.png" lightbox="media/private-azure/notifications-approve-reject.png" alt-text="Mostra as opções aprovar e rejeitar.":::

1. <span data-ttu-id="0bb48-191">Selecione o plano a ser aprovado no menu suspenso.</span><span class="sxs-lookup"><span data-stu-id="0bb48-191">Select the plan to approve from the drop-down menu.</span></span>
1. <span data-ttu-id="0bb48-192">Adicione um comentário e selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="0bb48-192">Add a comment and select **Submit**.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="0bb48-193">Navegação privada Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="0bb48-193">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="0bb48-194">Quando a Azure Marketplace privada estiver habilitada, os usuários verão quais planos o administrador do Marketplace aprovou.</span><span class="sxs-lookup"><span data-stu-id="0bb48-194">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has approved.</span></span>

- <span data-ttu-id="0bb48-195">Um aviso **aprovado** verde indica uma oferta de parceiro (não Microsoft) aprovada.</span><span class="sxs-lookup"><span data-stu-id="0bb48-195">A green **Approved** notice indicates a Partner (non-Microsoft) offer that is approved.</span></span>
- <span data-ttu-id="0bb48-196">Um aviso **azul Aprovado** indica uma oferta da Microsoft (incluindo distribuições [endossada do Linux](/azure/virtual-machines/linux/endorsed-distros)) aprovada.</span><span class="sxs-lookup"><span data-stu-id="0bb48-196">A blue **Approved** notice indicates a Microsoft offer (including [Endorsed Linux distributions](/azure/virtual-machines/linux/endorsed-distros)) that is approved.</span></span>

<span data-ttu-id="0bb48-197">Os usuários podem filtrar entre ofertas que são e não foram aprovadas:</span><span class="sxs-lookup"><span data-stu-id="0bb48-197">Users can filter between offers that are and are not approved:</span></span>

   :::image type="content" source="media/private-azure/filter-option-small.png" lightbox="media/private-azure/filter-option.png" alt-text="Mostra a opção de filtragem.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="0bb48-199">Comprar ou implantar em aplicativos Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="0bb48-199">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="0bb48-200">Embora a experiência da página de detalhes do produto seja semelhante à Azure Marketplace global, há três cenários Azure Marketplace específicos.</span><span class="sxs-lookup"><span data-stu-id="0bb48-200">While the product details page experience is similar to the global Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="0bb48-201">Quando um usuário seleciona um plano aprovado, o botão **criar** é habilitado:</span><span class="sxs-lookup"><span data-stu-id="0bb48-201">When a user selects an approved plan, the **Create** button is enabled:</span></span>

   :::image type="content" source="media/private-azure/button-create-enabled-small.png" lightbox="media/private-azure/button-create-enabled.png" alt-text="Mostra a faixa de oferta indicando que um plano pode ser criado.":::

- <span data-ttu-id="0bb48-203">Se uma seleção de plano de produto não aparecer na página de detalhes do produto, mas o administrador tiver aprovado um ou mais planos, uma faixa anotará quais planos são aprovados e o botão **criar** será habilitado:</span><span class="sxs-lookup"><span data-stu-id="0bb48-203">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are approved and the **Create** button is enabled:</span></span>

   :::image type="content" source="media/private-azure/button-create-enabled-and-plans-small.png" lightbox="media/private-azure/button-create-enabled-and-plans.png" alt-text="Mostra a faixa de oferta indicando que um plano pode ser criado e mostrando os planos disponíveis.":::

- <span data-ttu-id="0bb48-205">Quando um usuário seleciona um plano não aprovado, uma faixa anota o plano como não aprovado e o botão **criar** é desabilitado.</span><span class="sxs-lookup"><span data-stu-id="0bb48-205">When a user selects a non-approved plan, a banner notes the plan as not approved and the **Create** button is disabled.</span></span> <span data-ttu-id="0bb48-206">O usuário ainda pode solicitar a adição do plano à lista aprovada (consulte a próxima seção).</span><span class="sxs-lookup"><span data-stu-id="0bb48-206">The user can still request to add the plan to the approved list (see next section).</span></span>

## <a name="request-to-add-offers-or-plans"></a><span data-ttu-id="0bb48-207">Solicitação para adicionar ofertas ou planos</span><span class="sxs-lookup"><span data-stu-id="0bb48-207">Request to add offers or plans</span></span>

<span data-ttu-id="0bb48-208">Você pode solicitar a adição de uma oferta pública ou um plano que não esteja atualmente aprovado no Azure Marketplace privado.</span><span class="sxs-lookup"><span data-stu-id="0bb48-208">You can request to add a public offer or plan that is not currently approved in the Private Azure Marketplace.</span></span>

1. <span data-ttu-id="0bb48-209">Selecione **solicitação para adicionar** na faixa para abrir o **formulário de solicitação de acesso**.</span><span class="sxs-lookup"><span data-stu-id="0bb48-209">Select **Request to add** in the banner to open the **Access request form**.</span></span>

   :::image type="content" source="media/private-azure/request-banner-small.png" lightbox="media/private-azure/request-banner.png" alt-text="Mostra a faixa com o link ' solicitar a adição '.":::

   :::image type="content" source="media/private-azure/access-request-form-small.png" lightbox="media/private-azure/access-request-form.png" alt-text="Mostra o formulário de solicitação de acesso para ofertas ou planos.":::

1. <span data-ttu-id="0bb48-212">Selecione quais planos adicionar à solicitação (**qualquer plano** informa ao administrador do Marketplace que você não tem uma preferência para um plano em uma oferta).</span><span class="sxs-lookup"><span data-stu-id="0bb48-212">Select which plans to add to the request (**Any Plan** tells the Marketplace admin that you don't have a preference for a plan within an offer).</span></span>

1. <span data-ttu-id="0bb48-213">Adicione uma **justificativa** e selecione **solicitação** para enviar sua solicitação.</span><span class="sxs-lookup"><span data-stu-id="0bb48-213">Add a **Justification** and select **Request** to submit your request.</span></span>

   :::image type="content" source="media/private-azure/access-request-form-filled-small.png" lightbox="media/private-azure/access-request-form-filled.png" alt-text="Mostra o formulário de solicitação de acesso para ofertas ou planos com entradas de exemplo.":::

1. <span data-ttu-id="0bb48-215">Uma indicação para uma solicitação pendente será exibida no formulário de solicitação de acesso com uma opção para **retirar a solicitação**.</span><span class="sxs-lookup"><span data-stu-id="0bb48-215">An indication for a pending request will appear in the Access request form with an option to **Withdraw request**.</span></span>

   :::image type="content" source="media/private-azure/approved-pending-plans-small.png" lightbox="media/private-azure/approved-pending-plans.png" alt-text="Mostra uma lista de planos aprovados ou pendentes com o link retirar solicitação.":::

> [!NOTE]
> <span data-ttu-id="0bb48-217">Depois de enviado, o formulário de solicitação de aprovação será enviado para o [centro de notificações](#private-azure-marketplace-notification-center) para que o administrador do Marketplace examine a solicitação e execute a ação.</span><span class="sxs-lookup"><span data-stu-id="0bb48-217">Once submitted, the approval request form will be sent to the [Notification Center](#private-azure-marketplace-notification-center) for the Marketplace admin to review the request and take action.</span></span>

> [!CAUTION]
> <span data-ttu-id="0bb48-218">A aprovação no Marketplace privado não indica a aquisição de uma solução.</span><span class="sxs-lookup"><span data-stu-id="0bb48-218">Approval into Private Marketplace does not indicate procurement of a solution.</span></span>

## <a name="frequently-asked-questions-faqs"></a><span data-ttu-id="0bb48-219">Perguntas frequentes (FAQs)</span><span class="sxs-lookup"><span data-stu-id="0bb48-219">Frequently Asked Questions (FAQs)</span></span>

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a><span data-ttu-id="0bb48-220">Já estou bloqueando o aplicativo de terceiros do Marketplace por meio de Azure Policy.</span><span class="sxs-lookup"><span data-stu-id="0bb48-220">I am already blocking Marketplace third-party application through Azure Policy.</span></span> <span data-ttu-id="0bb48-221">Como isso é diferente?</span><span class="sxs-lookup"><span data-stu-id="0bb48-221">How is this different?</span></span>

<span data-ttu-id="0bb48-222">Atualmente, há duas maneiras de restringir serviços de terceiros no Marketplace:</span><span class="sxs-lookup"><span data-stu-id="0bb48-222">There are currently two ways to restrict third-party services in Marketplace:</span></span>

1. <span data-ttu-id="0bb48-223">Por meio do portal de EA ou do portal do Azure, desabilite serviços de terceiros ou restrinja a "somente SKUs gratuitas ou BYOL".</span><span class="sxs-lookup"><span data-stu-id="0bb48-223">Through EA portal or the Azure portal, disable third-party services or restrict to "Free or BYOL SKUs only".</span></span>

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Mostra como restringir os serviços no portal do Azure.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="Mostra como restringir serviços no E um portal.":::

2. <span data-ttu-id="0bb48-226">Crie uma política do Azure para permitir apenas VMs específicas.</span><span class="sxs-lookup"><span data-stu-id="0bb48-226">Create an Azure policy to only allow specific VMs.</span></span> <span data-ttu-id="0bb48-227">para obter detalhes sobre como impor a política para Windows vms, consulte [aplicar políticas para Windows vms com Azure Resource Manager](/azure/virtual-machines/windows/policy).</span><span class="sxs-lookup"><span data-stu-id="0bb48-227">For details on how to enforce policy to Windows VMs, see [Apply policies to Windows VMs with Azure Resource Manager](/azure/virtual-machines/windows/policy).</span></span>

<span data-ttu-id="0bb48-228">O Azure Marketplace privado permite mais flexibilidade na restrição e na concessão de ofertas e planos específicos.</span><span class="sxs-lookup"><span data-stu-id="0bb48-228">Private Azure Marketplace allows more flexibility on restricting and allowing specific offers and plans.</span></span> <span data-ttu-id="0bb48-229">Ele informa os usuários finais sobre a disponibilidade para implantação na galeria do Marketplace, mesmo antes de tentar implantar serviços de terceiros.</span><span class="sxs-lookup"><span data-stu-id="0bb48-229">It informs end users on the availability for deployment in the marketplace gallery even before they try to deploy third-party services.</span></span> <span data-ttu-id="0bb48-230">Para permitir a implantação de serviços de terceiros, defina o Azure Marketplace como ativado/habilitado no portal de EA e o portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="0bb48-230">To allow deployment of third-party services, set Azure Marketplace to On/Enabled in EA Portal and the Azure portal.</span></span>

- <span data-ttu-id="0bb48-231">O Azure Marketplace privado pode organizar soluções de parceiros não limitadas a máquinas virtuais.</span><span class="sxs-lookup"><span data-stu-id="0bb48-231">Private Azure Marketplace can curate partner solutions not limited to virtual machines.</span></span>
- <span data-ttu-id="0bb48-232">O Azure Marketplace privado pode ser organizado no nível do plano e também pode definir "plano atual e futuro".</span><span class="sxs-lookup"><span data-stu-id="0bb48-232">Private Azure Marketplace can curate at the plan level and can also set "Current and future plan".</span></span>
- <span data-ttu-id="0bb48-233">O Azure Marketplace privado pode informar os usuários finais sobre o que o pode e não pode ser implantado.</span><span class="sxs-lookup"><span data-stu-id="0bb48-233">Private Azure Marketplace can inform the end users up front on what can and cannot be deployed.</span></span>

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a><span data-ttu-id="0bb48-234">Qual é a diferença entre uma oferta privada e o Azure Marketplace privado?</span><span class="sxs-lookup"><span data-stu-id="0bb48-234">What's the difference between a Private Offer and Private Azure Marketplace?</span></span>

<span data-ttu-id="0bb48-235">Uma **oferta privada** permite que os editores criem planos que só são visíveis para os clientes de destino.</span><span class="sxs-lookup"><span data-stu-id="0bb48-235">A **Private Offer** lets publishers create plans that are only visible to targeted customers.</span></span> <span data-ttu-id="0bb48-236">Isso permite que eles compartilhem de maneira privada soluções personalizadas com preços negociados, termos e condições particulares e configurações especializadas.</span><span class="sxs-lookup"><span data-stu-id="0bb48-236">This lets them privately share customized solutions with negotiated pricing, private terms and conditions, and specialized configurations.</span></span> <span data-ttu-id="0bb48-237">Para obter detalhes, consulte [ofertas privadas no Marketplace comercial](/azure/marketplace/private-offers).</span><span class="sxs-lookup"><span data-stu-id="0bb48-237">For details, see [Private offers in the commercial marketplace](/azure/marketplace/private-offers).</span></span>

<span data-ttu-id="0bb48-238">O **Azure Marketplace privado** no portal do Azure permite que os administradores aprovem previamente quais soluções de terceiros seus usuários podem implantar.</span><span class="sxs-lookup"><span data-stu-id="0bb48-238">**Private Azure Marketplace** in the Azure portal lets administrators pre-approve which third-party solutions their users can deploy.</span></span> <span data-ttu-id="0bb48-239">Com um Azure Marketplace privado, os usuários podem aproveitar os benefícios do Azure Marketplace encontrando, comprando e implantando ofertas compatíveis.</span><span class="sxs-lookup"><span data-stu-id="0bb48-239">With a Private Azure Marketplace, users can enjoy the benefits of Azure Marketplace by finding, buying, and deploying compliant offers.</span></span> <span data-ttu-id="0bb48-240">Para gerenciar ofertas privadas baseadas em assinatura no Marketplace privado, o administrador do Marketplace deve ter, no mínimo, a função de "leitura" na assinatura específica.</span><span class="sxs-lookup"><span data-stu-id="0bb48-240">To manage subscription-based Private Offers in Private Marketplace, the Marketplace admin must have a minimum of "read" role on the specific subscription.</span></span>

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a><span data-ttu-id="0bb48-241">Adicionei uma oferta privada ao Azure Marketplace particular, por que ela não aparece na guia Gerenciar Marketplace?</span><span class="sxs-lookup"><span data-stu-id="0bb48-241">I added a Private Offer to the Private Azure Marketplace, why is it not showing in the manage marketplace tab?</span></span>

<span data-ttu-id="0bb48-242">As ofertas privadas baseadas em assinatura são visíveis apenas para as assinaturas listadas nas configurações da oferta privada.</span><span class="sxs-lookup"><span data-stu-id="0bb48-242">Subscription-based Private Offers are visible only for the listed subscriptions in the Private Offer settings.</span></span> <span data-ttu-id="0bb48-243">Para exibir a oferta privada, verifique se o filtro de assinatura global está mostrando todas as assinaturas.</span><span class="sxs-lookup"><span data-stu-id="0bb48-243">To view the Private Offer, ensure the global subscription filter is showing all the subscriptions.</span></span>

   :::image type="content" source="media/private-azure/private-marketplace-filter.png" lightbox="media/private-azure/private-marketplace-filter.png" alt-text="Mostra o filtro particular do Marketplace.":::

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a><span data-ttu-id="0bb48-245">Podemos incluir imagens personalizadas no Azure Marketplace privado?</span><span class="sxs-lookup"><span data-stu-id="0bb48-245">Can we include custom images in Private Azure Marketplace?</span></span>

<span data-ttu-id="0bb48-246">Não.</span><span class="sxs-lookup"><span data-stu-id="0bb48-246">No.</span></span> <span data-ttu-id="0bb48-247">O Azure Marketplace privado permite que qualquer administrador de ti gerencie e acesse soluções de terceiros do Azure marketplace global.</span><span class="sxs-lookup"><span data-stu-id="0bb48-247">Private Azure Marketplace allows any IT administrator to manage and curate third-party solutions from global Azure Marketplace.</span></span> <span data-ttu-id="0bb48-248">Como as imagens personalizadas não estão no Azure marketplace global, o administrador de ti não pode escolher as imagens personalizadas.</span><span class="sxs-lookup"><span data-stu-id="0bb48-248">Since custom images are not on global Azure Marketplace, the IT administrator cannot pick and choose your custom images.</span></span> <span data-ttu-id="0bb48-249">Se você quiser compartilhar imagens personalizadas, use a [Galeria de imagens compartilhadas](/azure/virtual-machines/shared-image-galleries).</span><span class="sxs-lookup"><span data-stu-id="0bb48-249">If you would like to share custom images, use [Shared Image Gallery](/azure/virtual-machines/shared-image-galleries).</span></span>

1. <span data-ttu-id="0bb48-250">Guia passo a passo criar uma galeria de imagens compartilhadas (SIG) ([CLI](/azure/virtual-machines/shared-images-cli), [PowerShell](/azure/virtual-machines/shared-images-powershell)).</span><span class="sxs-lookup"><span data-stu-id="0bb48-250">Step-by-step guide Create a Shared Image Gallery (SIG) ([CLI](/azure/virtual-machines/shared-images-cli), [PowerShell](/azure/virtual-machines/shared-images-powershell)).</span></span>
2. <span data-ttu-id="0bb48-251">Criar uma definição de imagem em um SIG.</span><span class="sxs-lookup"><span data-stu-id="0bb48-251">Create an image definition within a SIG.</span></span> <span data-ttu-id="0bb48-252">O cliente deve escolher **generalizado** para o campo Estado do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="0bb48-252">Customer should choose **Generalized** for the OS-state field.</span></span> <span data-ttu-id="0bb48-253">([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span><span class="sxs-lookup"><span data-stu-id="0bb48-253">([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span></span>
3. <span data-ttu-id="0bb48-254">Traga a imagem gerenciada para a Galeria de imagens compartilhadas ([CLI](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).</span><span class="sxs-lookup"><span data-stu-id="0bb48-254">Bring managed image into the Shared Image Gallery ([CLI](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).</span></span>
4. <span data-ttu-id="0bb48-255">As imagens de VM SIG residiriam em uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="0bb48-255">The SIG VM images would reside in one subscription.</span></span> <span data-ttu-id="0bb48-256">Para torná-lo disponível para outras assinaturas, use um registro de aplicativo ([CLI](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)).</span><span class="sxs-lookup"><span data-stu-id="0bb48-256">To make it available to other subscriptions, use an app registration ([CLI](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)).</span></span>

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a><span data-ttu-id="0bb48-257">Por que vejo algumas ofertas **aprovadas por padrão** , embora o editor não seja a Microsoft?</span><span class="sxs-lookup"><span data-stu-id="0bb48-257">Why do I see some offers **Approved by default** even though the publisher is not Microsoft?</span></span>

<span data-ttu-id="0bb48-258">A Microsoft dá suporte à tecnologia Linux e de software livre no Azure.</span><span class="sxs-lookup"><span data-stu-id="0bb48-258">Microsoft supports Linux and open-source technology in Azure.</span></span> <span data-ttu-id="0bb48-259">As [distribuições do Linux endossadas](/azure/virtual-machines/linux/endorsed-distros) têm suporte no Azure e o preço é integrado em máquinas virtuais.</span><span class="sxs-lookup"><span data-stu-id="0bb48-259">[Endorsed Linux distributions](/azure/virtual-machines/linux/endorsed-distros) are supported on Azure and the price is integrated in virtual machines.</span></span> <span data-ttu-id="0bb48-260">Como o agente Linux do Azure já está pré-instalado no Azure Marketplace, ele é tratado como uma oferta da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0bb48-260">Because Azure Linux Agent is already pre-installed on Azure Marketplace, it is treated like a Microsoft offer.</span></span> <span data-ttu-id="0bb48-261">Como as ofertas da Microsoft são aprovadas por padrão, as distribuições do Linux endossadas não podem ser gerenciadas no Azure Marketplace privado e são aprovadas por padrão.</span><span class="sxs-lookup"><span data-stu-id="0bb48-261">Since Microsoft offers are approved by default, endorsed Linux distributions cannot be managed in Private Azure Marketplace and are approved by default.</span></span>

## <a name="contact-support"></a><span data-ttu-id="0bb48-262">Contate o suporte</span><span class="sxs-lookup"><span data-stu-id="0bb48-262">Contact support</span></span>

- <span data-ttu-id="0bb48-263">Para obter suporte ao Azure Marketplace, visite [o Microsoft Q&A](/answers/products/).</span><span class="sxs-lookup"><span data-stu-id="0bb48-263">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span>