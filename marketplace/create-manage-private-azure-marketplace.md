---
title: Criar e gerenciar o Azure Marketplace privado no portal do Azure
description: Saiba mais sobre como criar e gerenciar o Azure Marketplace privado (versão prévia) no portal do Azure.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: article
author: keferna
ms.author: keferna
ms.date: 09/18/2020
ms.openlocfilehash: c0a395a7c5bfe926cdc56d7386aaaebb0305fb68
ms.sourcegitcommit: d31c06022624ca2d1db12b3c60ef1d0a3861f763
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/19/2020
ms.locfileid: "91429289"
---
# <a name="create-and-manage-private-azure-marketplace-preview-in-the-azure-portal"></a><span data-ttu-id="76454-103">Criar e gerenciar o Azure Marketplace privado (versão prévia) no portal do Azure</span><span class="sxs-lookup"><span data-stu-id="76454-103">Create and manage Private Azure Marketplace (preview) in the Azure portal</span></span>

<span data-ttu-id="76454-104">O Azure Marketplace privado (versão prévia) permite que os administradores controlem quais soluções de terceiros seus usuários podem usar.</span><span class="sxs-lookup"><span data-stu-id="76454-104">Private Azure Marketplace (preview) lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="76454-105">Ele faz isso permitindo que você implante apenas ofertas que você aprova e que estejam em conformidade com as políticas da sua empresa.</span><span class="sxs-lookup"><span data-stu-id="76454-105">It does this by allowing you to deploy only offers that you approve and that comply with your enterprise's policies.</span></span> <span data-ttu-id="76454-106">Com o Azure Marketplace privado, os usuários podem pesquisar na loja online as ofertas compatíveis para comprar e implantar.</span><span class="sxs-lookup"><span data-stu-id="76454-106">With Private Azure Marketplace, your users can search the online store for compliant offers to purchase and deploy.</span></span> 

<span data-ttu-id="76454-107">Como um administrador do Marketplace (função atribuída), você começará com um repositório privado desabilitado e vazio, onde poderá adicionar suas ofertas e planos aprovados.</span><span class="sxs-lookup"><span data-stu-id="76454-107">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="76454-108">Este artigo explica como criar, gerenciar e habilitar o Azure Marketplace privado para seus usuários.</span><span class="sxs-lookup"><span data-stu-id="76454-108">This article explains how to create, manage, and enable Private Azure Marketplace for your users.</span></span>

<span data-ttu-id="76454-109">Observações:</span><span class="sxs-lookup"><span data-stu-id="76454-109">Notes:</span></span>

- <span data-ttu-id="76454-110">O Azure Marketplace privado está em um nível de locatário, portanto, todos os usuários no locatário verão a mesma lista organizada.</span><span class="sxs-lookup"><span data-stu-id="76454-110">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
- <span data-ttu-id="76454-111">Todas as soluções da Microsoft são adicionadas automaticamente ao Azure Marketplace privado.</span><span class="sxs-lookup"><span data-stu-id="76454-111">All Microsoft solutions are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="76454-112">Atribuir a função de administrador do Marketplace</span><span class="sxs-lookup"><span data-stu-id="76454-112">Assign the Marketplace admin role</span></span>

<span data-ttu-id="76454-113">O administrador global do locatário deve atribuir a função de **administrador do Marketplace** ao administrador privado do Azure Marketplace que gerenciará o repositório privado.</span><span class="sxs-lookup"><span data-stu-id="76454-113">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="76454-114">O acesso ao gerenciamento privado do Azure Marketplace está disponível somente para administradores de ti com a função de administrador do Marketplace atribuída.</span><span class="sxs-lookup"><span data-stu-id="76454-114">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="76454-115">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="76454-115">Prerequisites</span></span>

<span data-ttu-id="76454-116">Você deve atender a esses pré-requisitos antes de poder atribuir a função de administrador do Marketplace a um usuário no escopo do locatário:</span><span class="sxs-lookup"><span data-stu-id="76454-116">You must meet these prerequisites before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="76454-117">Você tem acesso a um usuário **administrador global** .</span><span class="sxs-lookup"><span data-stu-id="76454-117">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="76454-118">O locatário tem pelo menos uma assinatura (pode ser qualquer tipo).</span><span class="sxs-lookup"><span data-stu-id="76454-118">The tenant has at least one Subscription (can be any type).</span></span>
- <span data-ttu-id="76454-119">O usuário administrador global recebe a função **colaborador** ou superior para a assinatura escolhida na etapa 2.</span><span class="sxs-lookup"><span data-stu-id="76454-119">The Global administrator user is assigned the **Contributor** role or higher for the subscription chosen in step 2.</span></span>
- <span data-ttu-id="76454-120">O usuário administrador global tem acesso elevado definido como **Sim** (consulte [Elevate-Access-global-admin](/azure/role-based-access-control/elevate-access-global-admin)).</span><span class="sxs-lookup"><span data-stu-id="76454-120">The Global administrator user has elevated access set to **Yes** (see [elevate-access-global-admin](/azure/role-based-access-control/elevate-access-global-admin)).</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="76454-121">Atribuir a função de administrador do Marketplace com o PowerShell</span><span class="sxs-lookup"><span data-stu-id="76454-121">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="76454-122">Use o seguinte script do PowerShell para atribuir a função de administrador do Marketplace; Ele requer os seguintes parâmetros:</span><span class="sxs-lookup"><span data-stu-id="76454-122">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="76454-123">**Tenantid:** A ID do locatário no escopo (a função de administrador do Marketplace é atribuível no escopo do locatário).</span><span class="sxs-lookup"><span data-stu-id="76454-123">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="76454-124">**SubscriptionId:** Uma assinatura da qual o administrador global tem a função **colaborador** ou mais alta atribuída.</span><span class="sxs-lookup"><span data-stu-id="76454-124">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="76454-125">**GlobalAdminUsername:** O nome de usuário do administrador global.</span><span class="sxs-lookup"><span data-stu-id="76454-125">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="76454-126">**UsernameToAssignRoleFor:** O nome de usuário ao qual a função de administrador do Marketplace será atribuída.</span><span class="sxs-lookup"><span data-stu-id="76454-126">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="76454-127">Para usuários convidados convidados para o locatário, pode levar até 48 horas até que sua conta esteja disponível para atribuir a função de administrador do Marketplace.</span><span class="sxs-lookup"><span data-stu-id="76454-127">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace admin role.</span></span> <span data-ttu-id="76454-128">Para obter mais informações, consulte [Propriedades de um usuário de colaboração B2B Azure Active Directory](/azure/active-directory/b2b/user-properties).</span><span class="sxs-lookup"><span data-stu-id="76454-128">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

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

$MarketPlaceAdminRole = Get-AzRoleDefinition $MarketplaceAdminRoleDefinitionName

if($MarketPlaceAdminRole -eq $null)
{
Write-Error -Message "'$($MarketplaceAdminRoleDefinitionName)' role is not available" -ErrorAction Stop
}
else
{
Write-Output -Message "'$($MarketplaceAdminRoleDefinitionName)' role is available"
}

Write-Output -Message "About to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)..."

$elevatedAccessOnRoot = Get-AzRoleAssignment | where {$_.RoleDefinitionName -eq "User Access Administrator" -and $_.Scope -eq "/" -and $_.SignInName.Trim().ToLower() -eq $GlobalAdminUsername.Trim().ToLower() } | ft -Property SignInName

if($elevatedAccessOnRoot.Count -eq 0)
{
Write-Error -Message "$($GlobalAdminUsername) doesn't have permissions to assign '$($MarketplaceAdminRoleDefinitionName)'. Please verify it has elevated access 'On' in portal, https://docs.microsoft.com/en-us/azure/role-based-access-control/elevate-access-global-admin" -ErrorAction Stop
}
else
{
Write-Output "$GlobalAdminUsername has elevated access on root"
}

New-AzRoleAssignment -SignInName $UsernameToAssignRoleFor -RoleDefinitionName $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace"

}

Assign-MarketplaceAdminRole
```

<span data-ttu-id="76454-129">Para obter mais informações sobre os cmdlets contidos no módulo do PowerShell AZ. Portal, consulte [Microsoft Azure PowerShell: cmdlets do painel do portal](/powershell/module/az.portal/).</span><span class="sxs-lookup"><span data-stu-id="76454-129">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="76454-130">Criar Azure Marketplace privado</span><span class="sxs-lookup"><span data-stu-id="76454-130">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="76454-131">Entre no [portal do Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="76454-131">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="76454-132">Selecione **todos os serviços** e, em seguida, **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="76454-132">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Portal do Azure janela principal.":::

3. <span data-ttu-id="76454-134">Selecione **Marketplace privado** nas opções à esquerda.</span><span class="sxs-lookup"><span data-stu-id="76454-134">Select **Private Marketplace** from the options on the left.</span></span>

    :::image type="content" source="media/private-azure/private-marketplace.png" alt-text="Portal do Azure janela principal.":::

4. <span data-ttu-id="76454-136">Selecione **introdução** para criar o Azure Marketplace privado (você só precisa fazer isso uma vez).</span><span class="sxs-lookup"><span data-stu-id="76454-136">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Portal do Azure janela principal.":::

    <span data-ttu-id="76454-138">Se o Azure Marketplace privado já existir para esse locatário, o **Manage Marketplace** será selecionado por padrão.</span><span class="sxs-lookup"><span data-stu-id="76454-138">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="76454-139">Depois de concluído, você terá um Azure Marketplace privado vazio e desabilitado.</span><span class="sxs-lookup"><span data-stu-id="76454-139">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Portal do Azure janela principal.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="76454-141">Adicionar itens da Galeria</span><span class="sxs-lookup"><span data-stu-id="76454-141">Add items from gallery</span></span>

<span data-ttu-id="76454-142">Um item é uma combinação de uma oferta e um plano.</span><span class="sxs-lookup"><span data-stu-id="76454-142">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="76454-143">Você pode pesquisar e adicionar um item na página Gerenciar Marketplace.</span><span class="sxs-lookup"><span data-stu-id="76454-143">You can search for and add item in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="76454-144">Selecione **Adicionar itens**.</span><span class="sxs-lookup"><span data-stu-id="76454-144">Select **Add items**.</span></span>

2. <span data-ttu-id="76454-145">Procure a **Galeria** ou use o campo de pesquisa para localizar o item desejado.</span><span class="sxs-lookup"><span data-stu-id="76454-145">Browse the **Gallery** or use the search field to find the item you want.</span></span>

    :::image type="content" source="media/private-azure/marketplace-gallery.png" alt-text="Portal do Azure janela principal.":::

3. <span data-ttu-id="76454-147">Como padrão, ao adicionar uma nova oferta, todos os planos atuais serão adicionados à lista de permissões.</span><span class="sxs-lookup"><span data-stu-id="76454-147">As default, when adding a new offer, all current plans will be added to the allowed list.</span></span> <span data-ttu-id="76454-148">Para modificar a seleção do plano antes de adicionar os itens selecionados, selecione o menu suspenso no bloco da oferta e atualize os planos necessários.</span><span class="sxs-lookup"><span data-stu-id="76454-148">To modify the plan selection before adding the selected items, select the drop-down menu in the offer’s tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Portal do Azure janela principal.":::

4. <span data-ttu-id="76454-150">Selecione **concluído** na parte inferior esquerda depois de fazer suas seleções.</span><span class="sxs-lookup"><span data-stu-id="76454-150">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="76454-151">**Adicionar itens** ao Marketplace estará disponível somente para ofertas que não sejam da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="76454-151">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="76454-152">As ofertas da Microsoft são permitidas por padrão.</span><span class="sxs-lookup"><span data-stu-id="76454-152">Microsoft offers are allowed by default.</span></span>

## <a name="edit-item-plans"></a><span data-ttu-id="76454-153">Editar planos de item</span><span class="sxs-lookup"><span data-stu-id="76454-153">Edit item plans</span></span>

<span data-ttu-id="76454-154">Você pode editar os planos de um item na página Gerenciar Marketplace.</span><span class="sxs-lookup"><span data-stu-id="76454-154">You can edit an item's plans in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="76454-155">Na coluna **planos** , examine os planos disponíveis no menu suspenso desse item.</span><span class="sxs-lookup"><span data-stu-id="76454-155">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>
2. <span data-ttu-id="76454-156">Marque ou desmarque as caixas de seleção para escolher quais planos disponibilizar para os usuários.</span><span class="sxs-lookup"><span data-stu-id="76454-156">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Portal do Azure janela principal.":::

> [!NOTE]
> <span data-ttu-id="76454-158">Cada oferta precisa de pelo menos um plano selecionado para que a atualização ocorra.</span><span class="sxs-lookup"><span data-stu-id="76454-158">Each offer needs at least one plan selected in order for the update to occur.</span></span> <span data-ttu-id="76454-159">Para remover todos os planos relacionados a uma oferta, exclua a oferta inteira (consulte a próxima seção).</span><span class="sxs-lookup"><span data-stu-id="76454-159">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="76454-160">Excluir ofertas</span><span class="sxs-lookup"><span data-stu-id="76454-160">Delete offers</span></span>

<span data-ttu-id="76454-161">Na página Gerenciar Marketplace, marque a caixa de seleção ao lado do nome da oferta (consulte a tela acima) e selecione **excluir itens**.</span><span class="sxs-lookup"><span data-stu-id="76454-161">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="76454-162">Habilitar/desabilitar o Azure Marketplace privado</span><span class="sxs-lookup"><span data-stu-id="76454-162">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="76454-163">Na página Gerenciar o Marketplace, você verá uma dessas faixas, que mostra o estado atual do Azure Marketplace privado:</span><span class="sxs-lookup"><span data-stu-id="76454-163">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Portal do Azure janela principal.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Portal do Azure janela principal.":::

<span data-ttu-id="76454-166">Você pode habilitar ou desabilitar o Azure Marketplace privado, conforme necessário.</span><span class="sxs-lookup"><span data-stu-id="76454-166">You can enable or disable Private Azure Marketplace as needed.</span></span>

1. <span data-ttu-id="76454-167">Se desabilitado, selecione **habilitar Marketplace privado** para habilitar.</span><span class="sxs-lookup"><span data-stu-id="76454-167">If disabled, select **Enable Private Marketplace** to enable.</span></span>
2. <span data-ttu-id="76454-168">Se habilitado, selecione **desabilitar Marketplace privado** para desabilitar.</span><span class="sxs-lookup"><span data-stu-id="76454-168">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="76454-169">Navegando no Azure Marketplace privado</span><span class="sxs-lookup"><span data-stu-id="76454-169">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="76454-170">Quando o Azure Marketplace privado estiver habilitado, os usuários verão quais planos o administrador do Marketplace permitiu.</span><span class="sxs-lookup"><span data-stu-id="76454-170">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has allowed.</span></span>

- <span data-ttu-id="76454-171">Um aviso verde **permitido** indica uma oferta de parceiro (não Microsoft) que é permitida.</span><span class="sxs-lookup"><span data-stu-id="76454-171">A green **Allowed** notice indicates a Partner (non-Microsoft) offer that is allowed.</span></span>
- <span data-ttu-id="76454-172">Um aviso azul **permitido** indica uma oferta da Microsoft que é permitida.</span><span class="sxs-lookup"><span data-stu-id="76454-172">A blue **Allowed** notice indicates a Microsoft offer that is allowed.</span></span>

<span data-ttu-id="76454-173">Os usuários podem filtrar entre ofertas que são e não são permitidas:</span><span class="sxs-lookup"><span data-stu-id="76454-173">Users can filter between offers that are and are not allowed:</span></span>

:::image type="content" source="media/private-azure/filter-option.png" alt-text="Portal do Azure janela principal.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="76454-175">Comprar ou implantar no Azure Marketplace privado</span><span class="sxs-lookup"><span data-stu-id="76454-175">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="76454-176">Embora a experiência de página de detalhes do produto seja semelhante ao Azure Marketplace público, há três cenários particulares específicos do Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="76454-176">While the product details page experience is similar to the public Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="76454-177">Quando um usuário seleciona um plano permitido, o botão **criar** é habilitado:</span><span class="sxs-lookup"><span data-stu-id="76454-177">When a user selects an allowed plan, the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled.png" alt-text="Portal do Azure janela principal.":::

- <span data-ttu-id="76454-179">Quando um usuário seleciona um plano não permitido, uma faixa observa que o plano não é permitido e o botão **criar** é desabilitado.</span><span class="sxs-lookup"><span data-stu-id="76454-179">When a user selects a non-allowed plan, a banner notes that the plan is not allowed and the **Create** button is disabled.</span></span>

   :::image type="content" source="media/private-azure/button-create-disabled.png" alt-text="Portal do Azure janela principal.":::

- <span data-ttu-id="76454-181">Se uma seleção de plano de produto não aparecer na página de detalhes do produto, mas o administrador tiver aprovado um ou mais planos, uma faixa anotará quais planos são permitidos e o botão **criar** será habilitado:</span><span class="sxs-lookup"><span data-stu-id="76454-181">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are allowed and the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled-and-plans.png" alt-text="Portal do Azure janela principal.":::

## <a name="contact-support"></a><span data-ttu-id="76454-183">Contate o suporte</span><span class="sxs-lookup"><span data-stu-id="76454-183">Contact support</span></span>

<span data-ttu-id="76454-184">Para obter suporte ao Azure Marketplace, visite [o Microsoft Q&A](/answers/products/).</span><span class="sxs-lookup"><span data-stu-id="76454-184">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span> 
