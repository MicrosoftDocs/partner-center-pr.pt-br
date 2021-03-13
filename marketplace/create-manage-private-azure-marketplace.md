---
title: Criar e gerenciar o Azure Marketplace privado no portal do Azure
description: Saiba mais sobre como criar e gerenciar o Azure Marketplace privado (versão prévia) no portal do Azure. O Azure Marketplace privado (versão prévia) permite que os administradores controlem quais soluções de terceiros seus usuários podem usar.
ms.service: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 02/24/2021
ms.openlocfilehash: dbd67ee1d4e9775d37318ec6389888f03a50b6ec
ms.sourcegitcommit: 3a2415ab9833d5c574ad76d462f526a131c24f33
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "103412702"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a><span data-ttu-id="0a3e4-104">Criar e gerenciar o Azure Marketplace privado no portal do Azure</span><span class="sxs-lookup"><span data-stu-id="0a3e4-104">Create and manage Private Azure Marketplace in the Azure portal</span></span>

<span data-ttu-id="0a3e4-105">O Azure Marketplace privado permite que os administradores controlem quais soluções de terceiros seus usuários podem usar.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-105">Private Azure Marketplace lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="0a3e4-106">Ele faz isso permitindo que o usuário implante apenas ofertas que são aprovadas pelo administrador e que estão em conformidade com as políticas da sua empresa.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-106">It does this by allowing the user to deploy only offers that are approved by the administrator and comply with your enterprise's policies.</span></span> <span data-ttu-id="0a3e4-107">Com o Azure Marketplace privado, os usuários podem pesquisar as ofertas em conformidade da loja online para comprar e implantar.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-107">With Private Azure Marketplace, users can search the online store for compliant offers to purchase and deploy.</span></span>

<span data-ttu-id="0a3e4-108">Como um administrador do Marketplace (função atribuída), você começará com um repositório privado desabilitado e vazio, onde poderá adicionar suas ofertas e planos aprovados.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-108">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="0a3e4-109">Este artigo explica como atribuir a função necessária, criar um armazenamento privado, gerenciar itens, aprovar solicitações de usuário e habilitar o Azure Marketplace privado para seus usuários.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-109">This article explains how to assign the needed role, create a private store, manage items, approve user requests, and enable Private Azure Marketplace for your users.</span></span>

> [!NOTE]
> - <span data-ttu-id="0a3e4-110">O Azure Marketplace privado está em um nível de locatário, portanto, todos os usuários no locatário verão a mesma lista organizada.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-110">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
> - <span data-ttu-id="0a3e4-111">Todas as soluções da Microsoft (incluindo [distribuições do Linux endossadas](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) são adicionadas automaticamente ao Azure Marketplace privado.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-111">All Microsoft solutions (including [Endorsed Linux Distributions](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="0a3e4-112">Atribuir a função de administrador do Marketplace</span><span class="sxs-lookup"><span data-stu-id="0a3e4-112">Assign the Marketplace admin role</span></span>

<span data-ttu-id="0a3e4-113">O administrador global do locatário deve atribuir a função de **administrador do Marketplace** ao administrador privado do Azure Marketplace que gerenciará o repositório privado.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-113">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="0a3e4-114">O acesso ao gerenciamento privado do Azure Marketplace está disponível somente para administradores de ti com a função de administrador do Marketplace atribuída.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-114">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="0a3e4-115">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0a3e4-115">Prerequisites</span></span>

<span data-ttu-id="0a3e4-116">Esses pré-requisitos são necessários para que você possa atribuir a função de administrador do Marketplace a um usuário no escopo do locatário:</span><span class="sxs-lookup"><span data-stu-id="0a3e4-116">These prerequisites are required before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="0a3e4-117">Você tem acesso a um usuário **administrador global** .</span><span class="sxs-lookup"><span data-stu-id="0a3e4-117">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="0a3e4-118">O locatário tem pelo menos uma assinatura (pode ser qualquer tipo).</span><span class="sxs-lookup"><span data-stu-id="0a3e4-118">The tenant has at least one subscription (can be any type).</span></span>
- <span data-ttu-id="0a3e4-119">O usuário administrador global recebe a função **colaborador** ou superior para a assinatura escolhida.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-119">The Global administrator user is assigned the **Contributor** role or higher for the chosen subscription.</span></span>

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a><span data-ttu-id="0a3e4-120">Atribuir a função de administrador do Marketplace com o controle de acesso (IAM)</span><span class="sxs-lookup"><span data-stu-id="0a3e4-120">Assign the Marketplace admin role with access control (IAM)</span></span>

1. <span data-ttu-id="0a3e4-121">Entre no [portal do Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="0a3e4-121">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
1. <span data-ttu-id="0a3e4-122">Selecione **todos os serviços** e, em seguida, **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-122">Select **All services** and then **Marketplace**.</span></span>
1. <span data-ttu-id="0a3e4-123">Selecione **Marketplace privado** no menu à esquerda.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-123">Select **Private Marketplace** from the menu on the left.</span></span>

    <span data-ttu-id="0a3e4-124">[![Mostra a opção de menu particular do Marketplace no lado esquerdo do Marketplace.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="0a3e4-124">[![Shows the private marketplace menu option on the left side of the Marketplace.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)</span></span>

1. <span data-ttu-id="0a3e4-125">Selecione **controle de acesso (iam)** para atribuir a função de administrador do Marketplace.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-125">Select **Access control (IAM)** to assign the Marketplace admin role.</span></span>

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Mostra a tela de controle de acesso I M.":::

1. <span data-ttu-id="0a3e4-127">Selecione **+Adicionar** > **Adicionar atribuição de função**.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-127">Select **+ Add** > **Add role assignment**.</span></span>
1. <span data-ttu-id="0a3e4-128">Em **função**, escolha **administrador do Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-128">Under **Role**, choose **Marketplace Admin**.</span></span>

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Mostra o menu de atribuição de função.":::

1. <span data-ttu-id="0a3e4-130">Selecione o usuário desejado na lista suspensa e, em seguida, selecione **concluído**.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-130">Select the desired user from the dropdown list, then select **Done**.</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="0a3e4-131">Atribuir a função de administrador do Marketplace com o PowerShell</span><span class="sxs-lookup"><span data-stu-id="0a3e4-131">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="0a3e4-132">Use o seguinte script do PowerShell para atribuir a função de administrador do Marketplace; Ele requer os seguintes parâmetros:</span><span class="sxs-lookup"><span data-stu-id="0a3e4-132">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="0a3e4-133">**Tenantid:** A ID do locatário no escopo (a função de administrador do Marketplace é atribuível no escopo do locatário).</span><span class="sxs-lookup"><span data-stu-id="0a3e4-133">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="0a3e4-134">**SubscriptionId:** Uma assinatura da qual o administrador global tem a função **colaborador** ou mais alta atribuída.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-134">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="0a3e4-135">**GlobalAdminUsername:** O nome de usuário do administrador global.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-135">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="0a3e4-136">**UsernameToAssignRoleFor:** O nome de usuário ao qual a função de administrador do Marketplace será atribuída.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-136">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="0a3e4-137">Para usuários convidados convidados para o locatário, pode levar até 48 horas até que sua conta esteja disponível para atribuir a função de administrador do Marketplace.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-137">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace Admin role.</span></span> <span data-ttu-id="0a3e4-138">Para obter mais informações, consulte [Propriedades de um usuário de colaboração B2B Azure Active Directory](/azure/active-directory/b2b/user-properties).</span><span class="sxs-lookup"><span data-stu-id="0a3e4-138">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

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

<span data-ttu-id="0a3e4-139">Para obter mais informações sobre os cmdlets contidos no módulo do PowerShell AZ. Portal, consulte [Microsoft Azure PowerShell: cmdlets do painel do portal](/powershell/module/az.portal/).</span><span class="sxs-lookup"><span data-stu-id="0a3e4-139">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="0a3e4-140">Criar Azure Marketplace privado</span><span class="sxs-lookup"><span data-stu-id="0a3e4-140">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="0a3e4-141">Entre no [portal do Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="0a3e4-141">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="0a3e4-142">Selecione **todos os serviços** e, em seguida, **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-142">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Mostra a janela principal do portal do Azure.":::

3. <span data-ttu-id="0a3e4-144">Selecione **Marketplace privado** no menu à esquerda.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-144">Select **Private Marketplace** from the menu on the left.</span></span>

4. <span data-ttu-id="0a3e4-145">Selecione **introdução** para criar o Azure Marketplace privado (você só precisa fazer isso uma vez).</span><span class="sxs-lookup"><span data-stu-id="0a3e4-145">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Mostra como selecionar a janela principal ' Introdução à portal do Azure '.":::

    <span data-ttu-id="0a3e4-147">Se o Azure Marketplace privado já existir para esse locatário, o **Manage Marketplace** será selecionado por padrão.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-147">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="0a3e4-148">Depois de concluído, você terá um Azure Marketplace privado vazio e desabilitado.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-148">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Mostra a tela particular do Azure Marketplace vazia.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="0a3e4-150">Adicionar itens da Galeria</span><span class="sxs-lookup"><span data-stu-id="0a3e4-150">Add items from gallery</span></span>

<span data-ttu-id="0a3e4-151">Um item é uma combinação de uma oferta e um plano.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-151">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="0a3e4-152">Você pode pesquisar e adicionar itens na página Gerenciar Marketplace.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-152">You can search for and add items on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="0a3e4-153">Selecione **Adicionar itens**.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-153">Select **Add items**.</span></span>

2. <span data-ttu-id="0a3e4-154">Procure a **Galeria** ou use o campo de pesquisa para localizar o item desejado.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-154">Browse the **Gallery** or use the search field to find the item you want.</span></span>

    <span data-ttu-id="0a3e4-155">[![Mostra como procurar a galeria ou usar o campo de pesquisa.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="0a3e4-155">[![Shows how to browse the gallery or use the search field.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)</span></span>

3. <span data-ttu-id="0a3e4-156">Como padrão, ao adicionar uma nova oferta, todos os planos atuais serão adicionados à lista aprovada.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-156">As default, when adding a new offer, all current plans will be added to the approved list.</span></span> <span data-ttu-id="0a3e4-157">Para modificar a seleção do plano antes de adicionar os itens selecionados, selecione o menu suspenso no bloco da oferta e atualize os planos necessários.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-157">To modify the plan selection before adding the selected items, select the drop-down menu in the offer’s tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Mostra como atualizar os planos necessários.":::

4. <span data-ttu-id="0a3e4-159">Selecione **concluído** na parte inferior esquerda depois de fazer suas seleções.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-159">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="0a3e4-160">**Adicionar itens** ao Marketplace estará disponível somente para ofertas que não sejam da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-160">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="0a3e4-161">As soluções da Microsoft (incluindo [distribuições do Linux endossadas](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) serão marcadas como "aprovadas por padrão" e não poderão ser gerenciadas no Marketplace privado.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-161">Microsoft solutions (including [Endorsed Linux Distributions](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) will be tagged as “Approved by default” and cannot be managed in Private Marketplace.</span></span>

## <a name="edit-items-plans"></a><span data-ttu-id="0a3e4-162">Editar planos do item</span><span class="sxs-lookup"><span data-stu-id="0a3e4-162">Edit item's plans</span></span>

<span data-ttu-id="0a3e4-163">Você pode editar os planos de um item na página Gerenciar Marketplace.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-163">You can edit an item's plans on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="0a3e4-164">Na coluna **planos** , examine os planos disponíveis no menu suspenso desse item.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-164">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>
2. <span data-ttu-id="0a3e4-165">Marque ou desmarque as caixas de seleção para escolher quais planos disponibilizar para os usuários.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-165">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Mostra como marcar ou desmarcar a caixa de seleção para o item necessário.":::

> [!NOTE]
> <span data-ttu-id="0a3e4-167">Cada oferta precisa de pelo menos um plano selecionado para que a atualização ocorra.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-167">Each offer needs at least one plan selected for the update to occur.</span></span> <span data-ttu-id="0a3e4-168">Para remover todos os planos relacionados a uma oferta, exclua a oferta inteira (consulte a próxima seção).</span><span class="sxs-lookup"><span data-stu-id="0a3e4-168">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="0a3e4-169">Excluir ofertas</span><span class="sxs-lookup"><span data-stu-id="0a3e4-169">Delete offers</span></span>

<span data-ttu-id="0a3e4-170">Na página Gerenciar Marketplace, marque a caixa de seleção ao lado do nome da oferta (consulte a tela acima) e selecione **excluir itens**.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-170">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="0a3e4-171">Habilitar/desabilitar o Azure Marketplace privado</span><span class="sxs-lookup"><span data-stu-id="0a3e4-171">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="0a3e4-172">Na página Gerenciar o Marketplace, você verá uma dessas faixas, que mostra o estado atual do Azure Marketplace privado:</span><span class="sxs-lookup"><span data-stu-id="0a3e4-172">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Mostra a faixa &quot;desabilitar estado&quot;.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Mostra a faixa ' habilitar estado '.":::

<span data-ttu-id="0a3e4-175">Você pode habilitar ou desabilitar o Azure Marketplace privado, conforme necessário.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-175">You can enable or disable Private Azure Marketplace as needed.</span></span>

- <span data-ttu-id="0a3e4-176">Se desabilitado, selecione **habilitar Marketplace privado** para habilitar.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-176">If disabled, select **Enable Private Marketplace** to enable.</span></span>
- <span data-ttu-id="0a3e4-177">Se habilitado, selecione **desabilitar Marketplace privado** para desabilitar.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-177">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="private-azure-marketplace-notification-center"></a><span data-ttu-id="0a3e4-178">Central de notificações do Azure Marketplace privada</span><span class="sxs-lookup"><span data-stu-id="0a3e4-178">Private Azure Marketplace notification center</span></span>

<span data-ttu-id="0a3e4-179">O centro de notificações consiste em três tipos de notificações e permite que o administrador do Marketplace execute ações com base na notificação:</span><span class="sxs-lookup"><span data-stu-id="0a3e4-179">Notification Center consists of three types of notifications and allows the Marketplace admin to take actions based on the notification:</span></span>

- <span data-ttu-id="0a3e4-180">Solicitações de aprovação de usuários para itens que não estão na lista aprovada (consulte [solicitação para adicionar ofertas ou planos](#request-to-add-offers-or-plans) abaixo).</span><span class="sxs-lookup"><span data-stu-id="0a3e4-180">Approval requests from users for items that are not in the approved list (see [Request to add offers or plans](#request-to-add-offers-or-plans) below).</span></span>
- <span data-ttu-id="0a3e4-181">Novas notificações de plano para ofertas que já têm um ou mais planos na lista aprovada.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-181">New plan notifications for offers that already have one or more plans in the approved list.</span></span>
- <span data-ttu-id="0a3e4-182">As notificações do plano foram removidas para itens que estão na lista aprovada, mas foram removidas do Azure marketplace global.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-182">Removed plan notifications for items that are in the approved list but were removed from the global Azure Marketplace.</span></span>

<span data-ttu-id="0a3e4-183">Para acessar o centro de notificações:</span><span class="sxs-lookup"><span data-stu-id="0a3e4-183">To access the notification center:</span></span>

1. <span data-ttu-id="0a3e4-184">Selecione **notificações** no menu do lado esquerdo.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-184">Select **Notifications** from the left-side menu.</span></span>

    <span data-ttu-id="0a3e4-185">[![Mostra o menu notificações.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="0a3e4-185">[![Shows the Notifications menu.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)</span></span>

1. <span data-ttu-id="0a3e4-186">Selecione o menu de reticências para obter mais ações.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-186">Select the ellipsis menu for more actions.</span></span>

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Mostra os resultados do menu mais opções.":::

1. <span data-ttu-id="0a3e4-188">Para solicitações de plano, **Mostrar solicitações** abre o formulário de solicitação de aprovação, onde você pode examinar todas as solicitações de usuário para a oferta específica.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-188">For plan requests, **Show requests** opens the approval request form where you can review all user requests for the specific offer.</span></span>
1. <span data-ttu-id="0a3e4-189">Selecione **aprovar** ou **rejeitar**.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-189">Select **Approve** or **Reject**.</span></span>

    <span data-ttu-id="0a3e4-190">[![Mostra as opções de aprovar e rejeitar.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="0a3e4-190">[![Shows the approve and reject options.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)</span></span>

1. <span data-ttu-id="0a3e4-191">Selecione o plano a ser aprovado no menu suspenso.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-191">Select the plan to approve from the drop-down menu.</span></span>
1. <span data-ttu-id="0a3e4-192">Adicione um comentário e selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-192">Add a comment and select **Submit**.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="0a3e4-193">Navegando no Azure Marketplace privado</span><span class="sxs-lookup"><span data-stu-id="0a3e4-193">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="0a3e4-194">Quando o Azure Marketplace privado estiver habilitado, os usuários verão quais planos foram aprovados pelo administrador do Marketplace.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-194">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has approved.</span></span>

- <span data-ttu-id="0a3e4-195">Um aviso de **aprovação** verde indica uma oferta de parceiro (que não é da Microsoft) aprovada.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-195">A green **Approved** notice indicates a Partner (non-Microsoft) offer that is approved.</span></span>
- <span data-ttu-id="0a3e4-196">Um aviso de **aprovação** azul indica uma oferta da Microsoft (incluindo as [distribuições do Linux endossadas](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) que é aprovada.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-196">A blue **Approved** notice indicates a Microsoft offer (including [Endorsed Linux distributions](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) that is approved.</span></span>

<span data-ttu-id="0a3e4-197">Os usuários podem filtrar entre ofertas que são e não são aprovadas:</span><span class="sxs-lookup"><span data-stu-id="0a3e4-197">Users can filter between offers that are and are not approved:</span></span>

<span data-ttu-id="0a3e4-198">[![Mostra a opção de filtragem.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="0a3e4-198">[![Shows the filtering option.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)</span></span>

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="0a3e4-199">Comprar ou implantar no Azure Marketplace privado</span><span class="sxs-lookup"><span data-stu-id="0a3e4-199">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="0a3e4-200">Embora a experiência de página de detalhes do produto seja semelhante ao Azure marketplace global, há três cenários particulares específicos do Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-200">While the product details page experience is similar to the global Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="0a3e4-201">Quando um usuário seleciona um plano aprovado, o botão **criar** é habilitado:</span><span class="sxs-lookup"><span data-stu-id="0a3e4-201">When a user selects an approved plan, the **Create** button is enabled:</span></span>

    <span data-ttu-id="0a3e4-202">[![Mostra a faixa de oferta indicando que um plano pode ser criado.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="0a3e4-202">[![Shows the offer banner noting a plan can be created.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)</span></span>

- <span data-ttu-id="0a3e4-203">Se uma seleção de plano de produto não aparecer na página de detalhes do produto, mas o administrador tiver aprovado um ou mais planos, uma faixa anotará quais planos são aprovados e o botão **criar** será habilitado:</span><span class="sxs-lookup"><span data-stu-id="0a3e4-203">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are approved and the **Create** button is enabled:</span></span>

    <span data-ttu-id="0a3e4-204">[![Mostra a faixa de oferta indicando que um plano pode ser criado e mostrando os planos disponíveis.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="0a3e4-204">[![Shows the offer banner noting that a plan can be created and showing available plans.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)</span></span>

- <span data-ttu-id="0a3e4-205">Quando um usuário seleciona um plano não aprovado, uma faixa anota o plano como não aprovado e o botão **criar** é desabilitado.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-205">When a user selects a non-approved plan, a banner notes the plan as not approved and the **Create** button is disabled.</span></span> <span data-ttu-id="0a3e4-206">O usuário ainda pode solicitar a adição do plano à lista aprovada (consulte a próxima seção).</span><span class="sxs-lookup"><span data-stu-id="0a3e4-206">The user can still request to add the plan to the approved list (see next section).</span></span>

## <a name="request-to-add-offers-or-plans"></a><span data-ttu-id="0a3e4-207">Solicitação para adicionar ofertas ou planos</span><span class="sxs-lookup"><span data-stu-id="0a3e4-207">Request to add offers or plans</span></span>

<span data-ttu-id="0a3e4-208">Você pode solicitar a adição de uma oferta pública ou um plano que não esteja atualmente aprovado no Azure Marketplace privado.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-208">You can request to add a public offer or plan that is not currently approved in the Private Azure Marketplace.</span></span>

1. <span data-ttu-id="0a3e4-209">Selecione **solicitação para adicionar** na faixa para abrir o **formulário de solicitação de acesso**.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-209">Select **Request to add** in the banner to open the **Access request form**.</span></span>

    <span data-ttu-id="0a3e4-210">[![Mostra a faixa com o link ' solicitar a adição '.](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="0a3e4-210">[![Shows the banner with the 'Request to add' link.](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)</span></span>

    <span data-ttu-id="0a3e4-211">[![Mostra o formulário de solicitação de acesso para ofertas ou planos.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="0a3e4-211">[![Shows the access request form for offers or plans.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)</span></span>

1. <span data-ttu-id="0a3e4-212">Selecione quais planos adicionar à solicitação (**qualquer plano** informa ao administrador do Marketplace que você não tem uma preferência para um plano em uma oferta).</span><span class="sxs-lookup"><span data-stu-id="0a3e4-212">Select which plans to add to the request (**Any Plan** tells the Marketplace admin that you don't have a preference for a plan within an offer).</span></span>

1. <span data-ttu-id="0a3e4-213">Adicione uma **justificativa** e selecione **solicitação** para enviar sua solicitação.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-213">Add a **Justification** and select **Request** to submit your request.</span></span>
  
    <span data-ttu-id="0a3e4-214">[![Mostra o formulário de solicitação de acesso para ofertas ou planos com entradas de exemplo.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="0a3e4-214">[![Shows the access request form for offers or plans with sample entries.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)</span></span>

1. <span data-ttu-id="0a3e4-215">Uma indicação para uma solicitação pendente será exibida no formulário de solicitação de acesso com uma opção para **retirar a solicitação**.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-215">An indication for a pending request will appear in the Access request form with an option to **Withdraw request**.</span></span>

    <span data-ttu-id="0a3e4-216">[![Mostra uma lista de planos aprovados ou pendentes com o link retirar solicitação.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="0a3e4-216">[![Shows a list of approved or pending plans with Withdraw Request link.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)</span></span>

> [!NOTE]
> <span data-ttu-id="0a3e4-217">Depois de enviado, o formulário de solicitação de aprovação será enviado para o [centro de notificações](#private-azure-marketplace-notification-center) para que o administrador do Marketplace examine a solicitação e execute a ação.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-217">Once submitted, the approval request form will be sent to the [Notification Center](#private-azure-marketplace-notification-center) for the Marketplace admin to review the request and take action.</span></span>

## <a name="frequently-asked-questions-faqs"></a><span data-ttu-id="0a3e4-218">Perguntas frequentes (FAQs)</span><span class="sxs-lookup"><span data-stu-id="0a3e4-218">Frequently Asked Questions (FAQs)</span></span>

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a><span data-ttu-id="0a3e4-219">Já estou bloqueando o aplicativo de terceiros do Marketplace por meio de Azure Policy.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-219">I am already blocking Marketplace third-party application through Azure Policy.</span></span> <span data-ttu-id="0a3e4-220">Como isso é diferente?</span><span class="sxs-lookup"><span data-stu-id="0a3e4-220">How is this different?</span></span>

<span data-ttu-id="0a3e4-221">Atualmente, há duas maneiras de restringir serviços de terceiros no Marketplace:</span><span class="sxs-lookup"><span data-stu-id="0a3e4-221">There are currently two ways to restrict third-party services in Marketplace:</span></span>

1. <span data-ttu-id="0a3e4-222">Por meio do portal de EA ou do portal do Azure, desabilite serviços de terceiros ou restrinja a "somente SKUs gratuitas ou BYOL".</span><span class="sxs-lookup"><span data-stu-id="0a3e4-222">Through EA portal or the Azure portal, disable third-party services or restrict to “Free or BYOL SKUs only”.</span></span>

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Mostra como restringir os serviços no portal do Azure.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="Mostra como restringir serviços no E um portal.":::

2. <span data-ttu-id="0a3e4-225">Crie uma política do Azure para permitir apenas VMs específicas.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-225">Create an Azure policy to only allow specific VMs.</span></span> <span data-ttu-id="0a3e4-226">Para obter detalhes sobre como impor a política para VMs do Windows, consulte [aplicar políticas a VMs do Windows com Azure Resource Manager](https://docs.microsoft.com/azure/virtual-machines/windows/policy).</span><span class="sxs-lookup"><span data-stu-id="0a3e4-226">For details on how to enforce policy to Windows VMs, see [Apply policies to Windows VMs with Azure Resource Manager](https://docs.microsoft.com/azure/virtual-machines/windows/policy).</span></span>

<span data-ttu-id="0a3e4-227">O Azure Marketplace privado permite mais flexibilidade na restrição e na concessão de ofertas e planos específicos.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-227">Private Azure Marketplace allows more flexibility on restricting and allowing specific offers and plans.</span></span> <span data-ttu-id="0a3e4-228">Ele informa os usuários finais sobre a disponibilidade para implantação na galeria do Marketplace, mesmo antes de tentar implantar serviços de terceiros.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-228">It informs end users on the availability for deployment in the marketplace gallery even before they try to deploy third-party services.</span></span> <span data-ttu-id="0a3e4-229">Para permitir a implantação de serviços de terceiros, defina o Azure Marketplace como ativado/habilitado no portal de EA e o portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-229">To allow deployment of third-party services, set Azure Marketplace to On/Enabled in EA Portal and the Azure portal.</span></span>

- <span data-ttu-id="0a3e4-230">O Azure Marketplace privado pode organizar soluções de parceiros não limitadas a máquinas virtuais.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-230">Private Azure Marketplace can curate partner solutions not limited to virtual machines.</span></span>
- <span data-ttu-id="0a3e4-231">O Azure Marketplace privado pode ser organizado no nível do plano e também pode definir "plano atual e futuro".</span><span class="sxs-lookup"><span data-stu-id="0a3e4-231">Private Azure Marketplace can curate at the plan level and can also set “Current and future plan”.</span></span>
- <span data-ttu-id="0a3e4-232">O Azure Marketplace privado pode informar os usuários finais sobre o que o pode e não pode ser implantado.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-232">Private Azure Marketplace can inform the end users up front on what can and cannot be deployed.</span></span>

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a><span data-ttu-id="0a3e4-233">Qual é a diferença entre uma oferta privada e o Azure Marketplace privado?</span><span class="sxs-lookup"><span data-stu-id="0a3e4-233">What's the difference between a Private Offer and Private Azure Marketplace?</span></span>

<span data-ttu-id="0a3e4-234">Uma **oferta privada** permite que os editores criem planos que só são visíveis para os clientes de destino.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-234">A **Private Offer** lets publishers create plans that are only visible to targeted customers.</span></span> <span data-ttu-id="0a3e4-235">Isso permite que eles compartilhem de maneira privada soluções personalizadas com preços negociados, termos e condições particulares e configurações especializadas.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-235">This lets them privately share customized solutions with negotiated pricing, private terms and conditions, and specialized configurations.</span></span> <span data-ttu-id="0a3e4-236">Para obter detalhes, consulte [ofertas privadas no Marketplace comercial](https://docs.microsoft.com/azure/marketplace/private-offers).</span><span class="sxs-lookup"><span data-stu-id="0a3e4-236">For details, see [Private offers in the commercial marketplace](https://docs.microsoft.com/azure/marketplace/private-offers).</span></span>

<span data-ttu-id="0a3e4-237">O **Azure Marketplace privado** no portal do Azure permite que os administradores aprovem previamente quais soluções de terceiros seus usuários podem implantar.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-237">**Private Azure Marketplace** in the Azure portal lets administrators pre-approve which third-party solutions their users can deploy.</span></span> <span data-ttu-id="0a3e4-238">Com um Azure Marketplace privado, os usuários podem aproveitar os benefícios do Azure Marketplace encontrando, comprando e implantando ofertas compatíveis.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-238">With a Private Azure Marketplace, users can enjoy the benefits of Azure Marketplace by finding, buying, and deploying compliant offers.</span></span> <span data-ttu-id="0a3e4-239">Para gerenciar ofertas privadas baseadas em assinatura no Marketplace privado, o administrador do Marketplace deve ter, no mínimo, a função de "leitura" na assinatura específica.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-239">To manage subscription-based Private Offers in Private Marketplace, the Marketplace admin must have a minimum of “read” role on the specific subscription.</span></span>

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a><span data-ttu-id="0a3e4-240">Adicionei uma oferta privada ao Azure Marketplace particular, por que ela não aparece na guia Gerenciar Marketplace?</span><span class="sxs-lookup"><span data-stu-id="0a3e4-240">I added a Private Offer to the Private Azure Marketplace, why is it not showing in the manage marketplace tab?</span></span>

<span data-ttu-id="0a3e4-241">As ofertas privadas baseadas em assinatura são visíveis apenas para as assinaturas listadas nas configurações da oferta privada.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-241">Subscription-based Private Offers are visible only for the listed subscriptions in the Private Offer settings.</span></span> <span data-ttu-id="0a3e4-242">Para exibir a oferta privada, verifique se o filtro de assinatura global está mostrando todas as assinaturas.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-242">To view the Private Offer, ensure the global subscription filter is showing all the subscriptions.</span></span>

<span data-ttu-id="0a3e4-243">[![Mostra o filtro particular do Marketplace.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="0a3e4-243">[![Shows the private marketplace filter.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)</span></span>

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a><span data-ttu-id="0a3e4-244">Podemos incluir imagens personalizadas no Azure Marketplace privado?</span><span class="sxs-lookup"><span data-stu-id="0a3e4-244">Can we include custom images in Private Azure Marketplace?</span></span>

<span data-ttu-id="0a3e4-245">Não.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-245">No.</span></span> <span data-ttu-id="0a3e4-246">O Azure Marketplace privado permite que qualquer administrador de ti gerencie e acesse soluções de terceiros do Azure marketplace global.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-246">Private Azure Marketplace allows any IT administrator to manage and curate third-party solutions from global Azure Marketplace.</span></span> <span data-ttu-id="0a3e4-247">Como as imagens personalizadas não estão no Azure marketplace global, o administrador de ti não pode escolher as imagens personalizadas.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-247">Since custom images are not on global Azure Marketplace, the IT administrator cannot pick and choose your custom images.</span></span> <span data-ttu-id="0a3e4-248">Se você quiser compartilhar imagens personalizadas, use a [Galeria de imagens compartilhadas](https://docs.microsoft.com/azure/virtual-machines/shared-image-galleries).</span><span class="sxs-lookup"><span data-stu-id="0a3e4-248">If you would like to share custom images, use [Shared Image Gallery](https://docs.microsoft.com/azure/virtual-machines/shared-image-galleries).</span></span>

1. <span data-ttu-id="0a3e4-249">Guia passo a passo criar uma galeria de imagens compartilhadas (SIG) ([CLI](https://docs.microsoft.com/azure/virtual-machines/shared-images-cli), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/shared-images-powershell)).</span><span class="sxs-lookup"><span data-stu-id="0a3e4-249">Step-by-step guide Create a Shared Image Gallery (SIG) ([CLI](https://docs.microsoft.com/azure/virtual-machines/shared-images-cli), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/shared-images-powershell)).</span></span>
2. <span data-ttu-id="0a3e4-250">Criar uma definição de imagem em um SIG.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-250">Create an image definition within a SIG.</span></span> <span data-ttu-id="0a3e4-251">O cliente deve escolher **generalizado** para o campo Estado do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-251">Customer should choose **Generalized** for the OS-state field.</span></span> <span data-ttu-id="0a3e4-252">([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span><span class="sxs-lookup"><span data-stu-id="0a3e4-252">([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span></span>
3. <span data-ttu-id="0a3e4-253">Traga a imagem gerenciada para a Galeria de imagens compartilhadas ([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-powershell)).</span><span class="sxs-lookup"><span data-stu-id="0a3e4-253">Bring managed image into the Shared Image Gallery ([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-powershell)).</span></span>
4. <span data-ttu-id="0a3e4-254">As imagens de VM SIG residiriam em uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-254">The SIG VM images would reside in one subscription.</span></span> <span data-ttu-id="0a3e4-255">Para torná-lo disponível para outras assinaturas, use um registro de aplicativo ([CLI](https://docs.microsoft.com/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/windows/share-images-across-tenants)).</span><span class="sxs-lookup"><span data-stu-id="0a3e4-255">To make it available to other subscriptions, use an app registration ([CLI](https://docs.microsoft.com/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/windows/share-images-across-tenants)).</span></span>

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a><span data-ttu-id="0a3e4-256">Por que vejo algumas ofertas **aprovadas por padrão** , embora o editor não seja a Microsoft?</span><span class="sxs-lookup"><span data-stu-id="0a3e4-256">Why do I see some offers **Approved by default** even though the publisher is not Microsoft?</span></span>

<span data-ttu-id="0a3e4-257">A Microsoft dá suporte à tecnologia Linux e de software livre no Azure.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-257">Microsoft supports Linux and open-source technology in Azure.</span></span> <span data-ttu-id="0a3e4-258">As [distribuições do Linux endossadas](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros) têm suporte no Azure e o preço é integrado em máquinas virtuais.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-258">[Endorsed Linux distributions](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros) are supported on Azure and the price is integrated in virtual machines.</span></span> <span data-ttu-id="0a3e4-259">Como o agente Linux do Azure já está pré-instalado no Azure Marketplace, ele é tratado como uma oferta da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-259">Because Azure Linux Agent is already pre-installed on Azure Marketplace, it is treated like a Microsoft offer.</span></span> <span data-ttu-id="0a3e4-260">Como as ofertas da Microsoft são aprovadas por padrão, as distribuições do Linux endossadas não podem ser gerenciadas no Azure Marketplace privado e são aprovadas por padrão.</span><span class="sxs-lookup"><span data-stu-id="0a3e4-260">Since Microsoft offers are approved by default, endorsed Linux distributions cannot be managed in Private Azure Marketplace and are approved by default.</span></span>

## <a name="contact-support"></a><span data-ttu-id="0a3e4-261">Contate o suporte</span><span class="sxs-lookup"><span data-stu-id="0a3e4-261">Contact support</span></span>

- <span data-ttu-id="0a3e4-262">Para obter suporte ao Azure Marketplace, visite [o Microsoft Q&A](/answers/products/).</span><span class="sxs-lookup"><span data-stu-id="0a3e4-262">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span>
