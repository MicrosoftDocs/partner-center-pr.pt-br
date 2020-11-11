---
title: Criar e gerenciar o Azure Marketplace privado no portal do Azure
description: Saiba mais sobre como criar e gerenciar o Azure Marketplace privado (versão prévia) no portal do Azure.
ms.prod: marketplace-customer
ms.topic: article
author: msjogarrig
ms.author: jogarrig
ms.date: 09/18/2020
ms.openlocfilehash: 1333bb2c8830cec83d7b7f05890af818d5c0ce5b
ms.sourcegitcommit: 95a5afdf68d88b6be848729830dcd114e3fb0c0f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/11/2020
ms.locfileid: "94487696"
---
# <a name="create-and-manage-private-azure-marketplace-preview-in-the-azure-portal"></a>Criar e gerenciar o Azure Marketplace privado (versão prévia) no portal do Azure

O Azure Marketplace privado (versão prévia) permite que os administradores controlem quais soluções de terceiros seus usuários podem usar. Ele faz isso permitindo que você implante apenas ofertas que você aprova e que estejam em conformidade com as políticas da sua empresa. Com o Azure Marketplace privado, os usuários podem pesquisar na loja online as ofertas compatíveis para comprar e implantar. 

Como um administrador do Marketplace (função atribuída), você começará com um repositório privado desabilitado e vazio, onde poderá adicionar suas ofertas e planos aprovados. Este artigo explica como criar, gerenciar e habilitar o Azure Marketplace privado para seus usuários.

Observações:

- O Azure Marketplace privado está em um nível de locatário, portanto, todos os usuários no locatário verão a mesma lista organizada.
- Todas as soluções da Microsoft são adicionadas automaticamente ao Azure Marketplace privado.

## <a name="assign-the-marketplace-admin-role"></a>Atribuir a função de administrador do Marketplace

O administrador global do locatário deve atribuir a função de **administrador do Marketplace** ao administrador privado do Azure Marketplace que gerenciará o repositório privado.

>[!IMPORTANT]
> O acesso ao gerenciamento privado do Azure Marketplace está disponível somente para administradores de ti com a função de administrador do Marketplace atribuída.

### <a name="prerequisites"></a>Pré-requisitos

Você deve atender a esses pré-requisitos antes de poder atribuir a função de administrador do Marketplace a um usuário no escopo do locatário:

- Você tem acesso a um usuário **administrador global** .
- O locatário tem pelo menos uma assinatura (pode ser qualquer tipo).
- O usuário administrador global recebe a função **colaborador** ou superior para a assinatura escolhida na etapa 2.
- O usuário administrador global tem acesso elevado definido como **Sim** (consulte [Elevate-Access-global-admin](/azure/role-based-access-control/elevate-access-global-admin)).

### <a name="assign-the-marketplace-admin-role-with-powershell"></a>Atribuir a função de administrador do Marketplace com o PowerShell

Use o seguinte script do PowerShell para atribuir a função de administrador do Marketplace; Ele requer os seguintes parâmetros:

- **Tenantid:** A ID do locatário no escopo (a função de administrador do Marketplace é atribuível no escopo do locatário).
- **SubscriptionId:** Uma assinatura da qual o administrador global tem a função **colaborador** ou mais alta atribuída.
- **GlobalAdminUsername:** O nome de usuário do administrador global.
- **UsernameToAssignRoleFor:** O nome de usuário ao qual a função de administrador do Marketplace será atribuída.

> [!NOTE]
> Para usuários convidados convidados para o locatário, pode levar até 48 horas até que sua conta esteja disponível para atribuir a função de administrador do Marketplace. Para obter mais informações, consulte [Propriedades de um usuário de colaboração B2B Azure Active Directory](/azure/active-directory/b2b/user-properties).

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

Para obter mais informações sobre os cmdlets contidos no módulo do PowerShell AZ. Portal, consulte [Microsoft Azure PowerShell: cmdlets do painel do portal](/powershell/module/az.portal/).

## <a name="create-private-azure-marketplace"></a>Criar Azure Marketplace privado

1. Entre no [portal do Azure](https://portal.azure.com/).
2. Selecione **todos os serviços** e, em seguida, **Marketplace**.

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Portal do Azure janela principal.":::

3. Selecione **Marketplace privado** nas opções à esquerda.

    :::image type="content" source="media/private-azure/private-marketplace.png" alt-text="Selecionando o Marketplace privado na janela principal do portal do Azure.":::

4. Selecione **introdução** para criar o Azure Marketplace privado (você só precisa fazer isso uma vez).

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Selecionando introdução na janela principal do portal do Azure.":::

    Se o Azure Marketplace privado já existir para esse locatário, o **Manage Marketplace** será selecionado por padrão.

5. Depois de concluído, você terá um Azure Marketplace privado vazio e desabilitado.

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="A tela particular do Azure Marketplace vazia.":::

## <a name="add-items-from-gallery"></a>Adicionar itens da Galeria

Um item é uma combinação de uma oferta e um plano. Você pode pesquisar e adicionar um item na página Gerenciar Marketplace.

1. Selecione **Adicionar itens**.

2. Procure a **Galeria** ou use o campo de pesquisa para localizar o item desejado.

    :::image type="content" source="media/private-azure/marketplace-gallery.png" alt-text="Navegação na galeria ou usando o campo de pesquisa.":::

3. Como padrão, ao adicionar uma nova oferta, todos os planos atuais serão adicionados à lista de permissões. Para modificar a seleção do plano antes de adicionar os itens selecionados, selecione o menu suspenso no bloco da oferta e atualize os planos necessários.

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Atualize os planos necessários.":::

4. Selecione **concluído** na parte inferior esquerda depois de fazer suas seleções.

>[!Note]
> **Adicionar itens** ao Marketplace estará disponível somente para ofertas que não sejam da Microsoft. As ofertas da Microsoft são permitidas por padrão.

## <a name="edit-item-plans"></a>Editar planos de item

Você pode editar os planos de um item na página Gerenciar Marketplace.

1. Na coluna **planos** , examine os planos disponíveis no menu suspenso desse item.
2. Marque ou desmarque as caixas de seleção para escolher quais planos disponibilizar para os usuários.

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Marcar ou desmarcar a caixa de seleção para o item necessário.":::

> [!NOTE]
> Cada oferta precisa de pelo menos um plano selecionado para que a atualização ocorra. Para remover todos os planos relacionados a uma oferta, exclua a oferta inteira (consulte a próxima seção).

## <a name="delete-offers"></a>Excluir ofertas

Na página Gerenciar Marketplace, marque a caixa de seleção ao lado do nome da oferta (consulte a tela acima) e selecione **excluir itens**.

## <a name="enabledisable-private-azure-marketplace"></a>Habilitar/desabilitar o Azure Marketplace privado

Na página Gerenciar o Marketplace, você verá uma dessas faixas, que mostra o estado atual do Azure Marketplace privado:

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Desabilitar faixa de estado":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Habilitar faixa de estado":::

Você pode habilitar ou desabilitar o Azure Marketplace privado, conforme necessário.

1. Se desabilitado, selecione **habilitar Marketplace privado** para habilitar.
2. Se habilitado, selecione **desabilitar Marketplace privado** para desabilitar.

## <a name="browsing-private-azure-marketplace"></a>Navegando no Azure Marketplace privado

Quando o Azure Marketplace privado estiver habilitado, os usuários verão quais planos o administrador do Marketplace permitiu.

- Um aviso verde **permitido** indica uma oferta de parceiro (não Microsoft) que é permitida.
- Um aviso azul **permitido** indica uma oferta da Microsoft que é permitida.

Os usuários podem filtrar entre ofertas que são e não são permitidas:

:::image type="content" source="media/private-azure/filter-option.png" alt-text="Opção de filtragem.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>Comprar ou implantar no Azure Marketplace privado

Embora a experiência de página de detalhes do produto seja semelhante ao Azure Marketplace público, há três cenários particulares específicos do Azure Marketplace.

- Quando um usuário seleciona um plano permitido, o botão **criar** é habilitado:

    :::image type="content" source="media/private-azure/button-create-enabled.png" alt-text="Faixa de oferta observando um plano pode ser criado.":::

- Quando um usuário seleciona um plano não permitido, uma faixa observa que o plano não é permitido e o botão **criar** é desabilitado.

   :::image type="content" source="media/private-azure/button-create-disabled.png" alt-text="Faixa de oferta observando um plano não pode ser criado.":::

- Se uma seleção de plano de produto não aparecer na página de detalhes do produto, mas o administrador tiver aprovado um ou mais planos, uma faixa anotará quais planos são permitidos e o botão **criar** será habilitado:

    :::image type="content" source="media/private-azure/button-create-enabled-and-plans.png" alt-text="Faixa de oferta observando que um plano pode ser criado e mostrando os planos disponíveis.":::

## <a name="contact-support"></a>Contate o suporte

Para obter suporte ao Azure Marketplace, visite [o Microsoft Q&A](/answers/products/). 
