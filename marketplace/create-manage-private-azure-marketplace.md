---
title: Criar e gerenciar o Azure Marketplace privado no portal do Azure
description: Saiba mais sobre como criar e gerenciar o Azure Marketplace privado (versão prévia) no portal do Azure. O Azure Marketplace privado (versão prévia) permite que os administradores controlem quais soluções de terceiros seus usuários podem usar.
ms.prod: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 09/18/2020
ms.openlocfilehash: 2459e7841c2c33227ad38f9d6fa1fc139fc0326e
ms.sourcegitcommit: 7beb7327472dc1b0c07c101d121196fb2830bbf8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "96439260"
---
# <a name="create-and-manage-private-azure-marketplace-preview-in-the-azure-portal"></a><span data-ttu-id="1e68d-104">Criar e gerenciar o Azure Marketplace privado (versão prévia) no portal do Azure</span><span class="sxs-lookup"><span data-stu-id="1e68d-104">Create and manage Private Azure Marketplace (preview) in the Azure portal</span></span>

<span data-ttu-id="1e68d-105">O Azure Marketplace privado (versão prévia) permite que os administradores controlem quais soluções de terceiros seus usuários podem usar.</span><span class="sxs-lookup"><span data-stu-id="1e68d-105">Private Azure Marketplace (preview) lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="1e68d-106">Ele faz isso permitindo que você implante apenas ofertas que você aprova e que estejam em conformidade com as políticas da sua empresa.</span><span class="sxs-lookup"><span data-stu-id="1e68d-106">It does this by allowing you to deploy only offers that you approve and that comply with your enterprise's policies.</span></span> <span data-ttu-id="1e68d-107">Com o Azure Marketplace privado, os usuários podem pesquisar na loja online as ofertas compatíveis para comprar e implantar.</span><span class="sxs-lookup"><span data-stu-id="1e68d-107">With Private Azure Marketplace, your users can search the online store for compliant offers to purchase and deploy.</span></span> 

<span data-ttu-id="1e68d-108">Como um administrador do Marketplace (função atribuída), você começará com um repositório privado desabilitado e vazio, onde poderá adicionar suas ofertas e planos aprovados.</span><span class="sxs-lookup"><span data-stu-id="1e68d-108">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="1e68d-109">Este artigo explica como criar, gerenciar e habilitar o Azure Marketplace privado para seus usuários.</span><span class="sxs-lookup"><span data-stu-id="1e68d-109">This article explains how to create, manage, and enable Private Azure Marketplace for your users.</span></span>

<span data-ttu-id="1e68d-110">Observações:</span><span class="sxs-lookup"><span data-stu-id="1e68d-110">Notes:</span></span>

- <span data-ttu-id="1e68d-111">O Azure Marketplace privado está em um nível de locatário, portanto, todos os usuários no locatário verão a mesma lista organizada.</span><span class="sxs-lookup"><span data-stu-id="1e68d-111">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
- <span data-ttu-id="1e68d-112">Todas as soluções da Microsoft são adicionadas automaticamente ao Azure Marketplace privado.</span><span class="sxs-lookup"><span data-stu-id="1e68d-112">All Microsoft solutions are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="1e68d-113">Atribuir a função de administrador do Marketplace</span><span class="sxs-lookup"><span data-stu-id="1e68d-113">Assign the Marketplace admin role</span></span>

<span data-ttu-id="1e68d-114">O administrador global do locatário deve atribuir a função de **administrador do Marketplace** ao administrador privado do Azure Marketplace que gerenciará o repositório privado.</span><span class="sxs-lookup"><span data-stu-id="1e68d-114">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="1e68d-115">O acesso ao gerenciamento privado do Azure Marketplace está disponível somente para administradores de ti com a função de administrador do Marketplace atribuída.</span><span class="sxs-lookup"><span data-stu-id="1e68d-115">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="1e68d-116">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1e68d-116">Prerequisites</span></span>

<span data-ttu-id="1e68d-117">Você deve atender a esses pré-requisitos antes de poder atribuir a função de administrador do Marketplace a um usuário no escopo do locatário:</span><span class="sxs-lookup"><span data-stu-id="1e68d-117">You must meet these prerequisites before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="1e68d-118">Você tem acesso a um usuário **administrador global** .</span><span class="sxs-lookup"><span data-stu-id="1e68d-118">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="1e68d-119">O locatário tem pelo menos uma assinatura (pode ser qualquer tipo).</span><span class="sxs-lookup"><span data-stu-id="1e68d-119">The tenant has at least one subscription (can be any type).</span></span>
- <span data-ttu-id="1e68d-120">O usuário administrador global recebe a função **colaborador** ou superior para a assinatura escolhida.</span><span class="sxs-lookup"><span data-stu-id="1e68d-120">The Global administrator user is assigned the **Contributor** role or higher for the chosen subscription.</span></span>
- <span data-ttu-id="1e68d-121">O usuário administrador global tem acesso elevado definido como **Sim** (consulte [elevar o acesso para gerenciar todas as assinaturas e grupos de gerenciamento do Azure](/azure/role-based-access-control/elevate-access-global-admin)).</span><span class="sxs-lookup"><span data-stu-id="1e68d-121">The Global administrator user has elevated access set to **Yes** (see [Elevate access to manage all Azure subscriptions and management groups](/azure/role-based-access-control/elevate-access-global-admin)).</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="1e68d-122">Atribuir a função de administrador do Marketplace com o PowerShell</span><span class="sxs-lookup"><span data-stu-id="1e68d-122">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="1e68d-123">Use o seguinte script do PowerShell para atribuir a função de administrador do Marketplace; Ele requer os seguintes parâmetros:</span><span class="sxs-lookup"><span data-stu-id="1e68d-123">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="1e68d-124">**Tenantid:** A ID do locatário no escopo (a função de administrador do Marketplace é atribuível no escopo do locatário).</span><span class="sxs-lookup"><span data-stu-id="1e68d-124">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="1e68d-125">**SubscriptionId:** Uma assinatura da qual o administrador global tem a função **colaborador** ou mais alta atribuída.</span><span class="sxs-lookup"><span data-stu-id="1e68d-125">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="1e68d-126">**GlobalAdminUsername:** O nome de usuário do administrador global.</span><span class="sxs-lookup"><span data-stu-id="1e68d-126">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="1e68d-127">**UsernameToAssignRoleFor:** O nome de usuário ao qual a função de administrador do Marketplace será atribuída.</span><span class="sxs-lookup"><span data-stu-id="1e68d-127">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="1e68d-128">Para usuários convidados convidados para o locatário, pode levar até 48 horas até que sua conta esteja disponível para atribuir a função de administrador do Marketplace.</span><span class="sxs-lookup"><span data-stu-id="1e68d-128">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace admin role.</span></span> <span data-ttu-id="1e68d-129">Para obter mais informações, consulte [Propriedades de um usuário de colaboração B2B Azure Active Directory](/azure/active-directory/b2b/user-properties).</span><span class="sxs-lookup"><span data-stu-id="1e68d-129">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

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

<span data-ttu-id="1e68d-130">Para obter mais informações sobre os cmdlets contidos no módulo do PowerShell AZ. Portal, consulte [Microsoft Azure PowerShell: cmdlets do painel do portal](/powershell/module/az.portal/).</span><span class="sxs-lookup"><span data-stu-id="1e68d-130">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="1e68d-131">Criar Azure Marketplace privado</span><span class="sxs-lookup"><span data-stu-id="1e68d-131">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="1e68d-132">Entre no [portal do Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="1e68d-132">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="1e68d-133">Selecione **todos os serviços** e, em seguida, **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="1e68d-133">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Portal do Azure janela principal.":::

3. <span data-ttu-id="1e68d-135">Selecione **Marketplace privado** nas opções à esquerda.</span><span class="sxs-lookup"><span data-stu-id="1e68d-135">Select **Private Marketplace** from the options on the left.</span></span>

    :::image type="content" source="media/private-azure/private-marketplace.png" alt-text="Selecionando o Marketplace privado na janela principal do portal do Azure.":::

4. <span data-ttu-id="1e68d-137">Selecione **introdução** para criar o Azure Marketplace privado (você só precisa fazer isso uma vez).</span><span class="sxs-lookup"><span data-stu-id="1e68d-137">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Selecionando introdução na janela principal do portal do Azure.":::

    <span data-ttu-id="1e68d-139">Se o Azure Marketplace privado já existir para esse locatário, o **Manage Marketplace** será selecionado por padrão.</span><span class="sxs-lookup"><span data-stu-id="1e68d-139">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="1e68d-140">Depois de concluído, você terá um Azure Marketplace privado vazio e desabilitado.</span><span class="sxs-lookup"><span data-stu-id="1e68d-140">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="A tela particular do Azure Marketplace vazia.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="1e68d-142">Adicionar itens da Galeria</span><span class="sxs-lookup"><span data-stu-id="1e68d-142">Add items from gallery</span></span>

<span data-ttu-id="1e68d-143">Um item é uma combinação de uma oferta e um plano.</span><span class="sxs-lookup"><span data-stu-id="1e68d-143">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="1e68d-144">Você pode pesquisar e adicionar um item na página Gerenciar Marketplace.</span><span class="sxs-lookup"><span data-stu-id="1e68d-144">You can search for and add item in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="1e68d-145">Selecione **Adicionar itens**.</span><span class="sxs-lookup"><span data-stu-id="1e68d-145">Select **Add items**.</span></span>

2. <span data-ttu-id="1e68d-146">Procure a **Galeria** ou use o campo de pesquisa para localizar o item desejado.</span><span class="sxs-lookup"><span data-stu-id="1e68d-146">Browse the **Gallery** or use the search field to find the item you want.</span></span>

    :::image type="content" source="media/private-azure/marketplace-gallery.png" alt-text="Navegação na galeria ou usando o campo de pesquisa.":::

3. <span data-ttu-id="1e68d-148">Como padrão, ao adicionar uma nova oferta, todos os planos atuais serão adicionados à lista de permissões.</span><span class="sxs-lookup"><span data-stu-id="1e68d-148">As default, when adding a new offer, all current plans will be added to the allowed list.</span></span> <span data-ttu-id="1e68d-149">Para modificar a seleção do plano antes de adicionar os itens selecionados, selecione o menu suspenso no bloco da oferta e atualize os planos necessários.</span><span class="sxs-lookup"><span data-stu-id="1e68d-149">To modify the plan selection before adding the selected items, select the drop-down menu in the offer’s tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Atualize os planos necessários.":::

4. <span data-ttu-id="1e68d-151">Selecione **concluído** na parte inferior esquerda depois de fazer suas seleções.</span><span class="sxs-lookup"><span data-stu-id="1e68d-151">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="1e68d-152">**Adicionar itens** ao Marketplace estará disponível somente para ofertas que não sejam da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1e68d-152">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="1e68d-153">As ofertas da Microsoft são permitidas por padrão.</span><span class="sxs-lookup"><span data-stu-id="1e68d-153">Microsoft offers are allowed by default.</span></span>

## <a name="edit-item-plans"></a><span data-ttu-id="1e68d-154">Editar planos de item</span><span class="sxs-lookup"><span data-stu-id="1e68d-154">Edit item plans</span></span>

<span data-ttu-id="1e68d-155">Você pode editar os planos de um item na página Gerenciar Marketplace.</span><span class="sxs-lookup"><span data-stu-id="1e68d-155">You can edit an item's plans in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="1e68d-156">Na coluna **planos** , examine os planos disponíveis no menu suspenso desse item.</span><span class="sxs-lookup"><span data-stu-id="1e68d-156">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>
2. <span data-ttu-id="1e68d-157">Marque ou desmarque as caixas de seleção para escolher quais planos disponibilizar para os usuários.</span><span class="sxs-lookup"><span data-stu-id="1e68d-157">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Marcar ou desmarcar a caixa de seleção para o item necessário.":::

> [!NOTE]
> <span data-ttu-id="1e68d-159">Cada oferta precisa de pelo menos um plano selecionado para que a atualização ocorra.</span><span class="sxs-lookup"><span data-stu-id="1e68d-159">Each offer needs at least one plan selected in order for the update to occur.</span></span> <span data-ttu-id="1e68d-160">Para remover todos os planos relacionados a uma oferta, exclua a oferta inteira (consulte a próxima seção).</span><span class="sxs-lookup"><span data-stu-id="1e68d-160">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="1e68d-161">Excluir ofertas</span><span class="sxs-lookup"><span data-stu-id="1e68d-161">Delete offers</span></span>

<span data-ttu-id="1e68d-162">Na página Gerenciar Marketplace, marque a caixa de seleção ao lado do nome da oferta (consulte a tela acima) e selecione **excluir itens**.</span><span class="sxs-lookup"><span data-stu-id="1e68d-162">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="1e68d-163">Habilitar/desabilitar o Azure Marketplace privado</span><span class="sxs-lookup"><span data-stu-id="1e68d-163">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="1e68d-164">Na página Gerenciar o Marketplace, você verá uma dessas faixas, que mostra o estado atual do Azure Marketplace privado:</span><span class="sxs-lookup"><span data-stu-id="1e68d-164">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Desabilitar faixa de estado":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Habilitar faixa de estado":::

<span data-ttu-id="1e68d-167">Você pode habilitar ou desabilitar o Azure Marketplace privado, conforme necessário.</span><span class="sxs-lookup"><span data-stu-id="1e68d-167">You can enable or disable Private Azure Marketplace as needed.</span></span>

1. <span data-ttu-id="1e68d-168">Se desabilitado, selecione **habilitar Marketplace privado** para habilitar.</span><span class="sxs-lookup"><span data-stu-id="1e68d-168">If disabled, select **Enable Private Marketplace** to enable.</span></span>
2. <span data-ttu-id="1e68d-169">Se habilitado, selecione **desabilitar Marketplace privado** para desabilitar.</span><span class="sxs-lookup"><span data-stu-id="1e68d-169">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="1e68d-170">Navegando no Azure Marketplace privado</span><span class="sxs-lookup"><span data-stu-id="1e68d-170">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="1e68d-171">Quando o Azure Marketplace privado estiver habilitado, os usuários verão quais planos o administrador do Marketplace permitiu.</span><span class="sxs-lookup"><span data-stu-id="1e68d-171">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has allowed.</span></span>

- <span data-ttu-id="1e68d-172">Um aviso verde **permitido** indica uma oferta de parceiro (não Microsoft) que é permitida.</span><span class="sxs-lookup"><span data-stu-id="1e68d-172">A green **Allowed** notice indicates a Partner (non-Microsoft) offer that is allowed.</span></span>
- <span data-ttu-id="1e68d-173">Um aviso azul **permitido** indica uma oferta da Microsoft que é permitida.</span><span class="sxs-lookup"><span data-stu-id="1e68d-173">A blue **Allowed** notice indicates a Microsoft offer that is allowed.</span></span>

<span data-ttu-id="1e68d-174">Os usuários podem filtrar entre ofertas que são e não são permitidas:</span><span class="sxs-lookup"><span data-stu-id="1e68d-174">Users can filter between offers that are and are not allowed:</span></span>

:::image type="content" source="media/private-azure/filter-option.png" alt-text="Opção de filtragem.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="1e68d-176">Comprar ou implantar no Azure Marketplace privado</span><span class="sxs-lookup"><span data-stu-id="1e68d-176">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="1e68d-177">Embora a experiência de página de detalhes do produto seja semelhante ao Azure Marketplace público, há três cenários particulares específicos do Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="1e68d-177">While the product details page experience is similar to the public Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="1e68d-178">Quando um usuário seleciona um plano permitido, o botão **criar** é habilitado:</span><span class="sxs-lookup"><span data-stu-id="1e68d-178">When a user selects an allowed plan, the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled.png" alt-text="Faixa de oferta observando um plano pode ser criado.":::

- <span data-ttu-id="1e68d-180">Quando um usuário seleciona um plano não permitido, uma faixa observa que o plano não é permitido e o botão **criar** é desabilitado.</span><span class="sxs-lookup"><span data-stu-id="1e68d-180">When a user selects a non-allowed plan, a banner notes that the plan is not allowed and the **Create** button is disabled.</span></span>

   :::image type="content" source="media/private-azure/button-create-disabled.png" alt-text="Faixa de oferta observando um plano não pode ser criado.":::

- <span data-ttu-id="1e68d-182">Se uma seleção de plano de produto não aparecer na página de detalhes do produto, mas o administrador tiver aprovado um ou mais planos, uma faixa anotará quais planos são permitidos e o botão **criar** será habilitado:</span><span class="sxs-lookup"><span data-stu-id="1e68d-182">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are allowed and the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled-and-plans.png" alt-text="Faixa de oferta observando que um plano pode ser criado e mostrando os planos disponíveis.":::

## <a name="contact-support"></a><span data-ttu-id="1e68d-184">Contate o suporte</span><span class="sxs-lookup"><span data-stu-id="1e68d-184">Contact support</span></span>

<span data-ttu-id="1e68d-185">Para obter suporte ao Azure Marketplace, visite [o Microsoft Q&A](/answers/products/).</span><span class="sxs-lookup"><span data-stu-id="1e68d-185">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span> 
