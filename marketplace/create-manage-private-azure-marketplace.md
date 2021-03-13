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
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a>Criar e gerenciar o Azure Marketplace privado no portal do Azure

O Azure Marketplace privado permite que os administradores controlem quais soluções de terceiros seus usuários podem usar. Ele faz isso permitindo que o usuário implante apenas ofertas que são aprovadas pelo administrador e que estão em conformidade com as políticas da sua empresa. Com o Azure Marketplace privado, os usuários podem pesquisar as ofertas em conformidade da loja online para comprar e implantar.

Como um administrador do Marketplace (função atribuída), você começará com um repositório privado desabilitado e vazio, onde poderá adicionar suas ofertas e planos aprovados. Este artigo explica como atribuir a função necessária, criar um armazenamento privado, gerenciar itens, aprovar solicitações de usuário e habilitar o Azure Marketplace privado para seus usuários.

> [!NOTE]
> - O Azure Marketplace privado está em um nível de locatário, portanto, todos os usuários no locatário verão a mesma lista organizada.
> - Todas as soluções da Microsoft (incluindo [distribuições do Linux endossadas](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) são adicionadas automaticamente ao Azure Marketplace privado.

## <a name="assign-the-marketplace-admin-role"></a>Atribuir a função de administrador do Marketplace

O administrador global do locatário deve atribuir a função de **administrador do Marketplace** ao administrador privado do Azure Marketplace que gerenciará o repositório privado.

>[!IMPORTANT]
> O acesso ao gerenciamento privado do Azure Marketplace está disponível somente para administradores de ti com a função de administrador do Marketplace atribuída.

### <a name="prerequisites"></a>Pré-requisitos

Esses pré-requisitos são necessários para que você possa atribuir a função de administrador do Marketplace a um usuário no escopo do locatário:

- Você tem acesso a um usuário **administrador global** .
- O locatário tem pelo menos uma assinatura (pode ser qualquer tipo).
- O usuário administrador global recebe a função **colaborador** ou superior para a assinatura escolhida.

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a>Atribuir a função de administrador do Marketplace com o controle de acesso (IAM)

1. Entre no [portal do Azure](https://portal.azure.com/).
1. Selecione **todos os serviços** e, em seguida, **Marketplace**.
1. Selecione **Marketplace privado** no menu à esquerda.

    [![Mostra a opção de menu particular do Marketplace no lado esquerdo do Marketplace.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)

1. Selecione **controle de acesso (iam)** para atribuir a função de administrador do Marketplace.

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Mostra a tela de controle de acesso I M.":::

1. Selecione **+Adicionar** > **Adicionar atribuição de função**.
1. Em **função**, escolha **administrador do Marketplace**.

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Mostra o menu de atribuição de função.":::

1. Selecione o usuário desejado na lista suspensa e, em seguida, selecione **concluído**.

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

Para obter mais informações sobre os cmdlets contidos no módulo do PowerShell AZ. Portal, consulte [Microsoft Azure PowerShell: cmdlets do painel do portal](/powershell/module/az.portal/).

## <a name="create-private-azure-marketplace"></a>Criar Azure Marketplace privado

1. Entre no [portal do Azure](https://portal.azure.com/).
2. Selecione **todos os serviços** e, em seguida, **Marketplace**.

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Mostra a janela principal do portal do Azure.":::

3. Selecione **Marketplace privado** no menu à esquerda.

4. Selecione **introdução** para criar o Azure Marketplace privado (você só precisa fazer isso uma vez).

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Mostra como selecionar a janela principal ' Introdução à portal do Azure '.":::

    Se o Azure Marketplace privado já existir para esse locatário, o **Manage Marketplace** será selecionado por padrão.

5. Depois de concluído, você terá um Azure Marketplace privado vazio e desabilitado.

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Mostra a tela particular do Azure Marketplace vazia.":::

## <a name="add-items-from-gallery"></a>Adicionar itens da Galeria

Um item é uma combinação de uma oferta e um plano. Você pode pesquisar e adicionar itens na página Gerenciar Marketplace.

1. Selecione **Adicionar itens**.

2. Procure a **Galeria** ou use o campo de pesquisa para localizar o item desejado.

    [![Mostra como procurar a galeria ou usar o campo de pesquisa.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)

3. Como padrão, ao adicionar uma nova oferta, todos os planos atuais serão adicionados à lista aprovada. Para modificar a seleção do plano antes de adicionar os itens selecionados, selecione o menu suspenso no bloco da oferta e atualize os planos necessários.

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Mostra como atualizar os planos necessários.":::

4. Selecione **concluído** na parte inferior esquerda depois de fazer suas seleções.

>[!Note]
> **Adicionar itens** ao Marketplace estará disponível somente para ofertas que não sejam da Microsoft. As soluções da Microsoft (incluindo [distribuições do Linux endossadas](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) serão marcadas como "aprovadas por padrão" e não poderão ser gerenciadas no Marketplace privado.

## <a name="edit-items-plans"></a>Editar planos do item

Você pode editar os planos de um item na página Gerenciar Marketplace.

1. Na coluna **planos** , examine os planos disponíveis no menu suspenso desse item.
2. Marque ou desmarque as caixas de seleção para escolher quais planos disponibilizar para os usuários.

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Mostra como marcar ou desmarcar a caixa de seleção para o item necessário.":::

> [!NOTE]
> Cada oferta precisa de pelo menos um plano selecionado para que a atualização ocorra. Para remover todos os planos relacionados a uma oferta, exclua a oferta inteira (consulte a próxima seção).

## <a name="delete-offers"></a>Excluir ofertas

Na página Gerenciar Marketplace, marque a caixa de seleção ao lado do nome da oferta (consulte a tela acima) e selecione **excluir itens**.

## <a name="enabledisable-private-azure-marketplace"></a>Habilitar/desabilitar o Azure Marketplace privado

Na página Gerenciar o Marketplace, você verá uma dessas faixas, que mostra o estado atual do Azure Marketplace privado:

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Mostra a faixa &quot;desabilitar estado&quot;.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Mostra a faixa ' habilitar estado '.":::

Você pode habilitar ou desabilitar o Azure Marketplace privado, conforme necessário.

- Se desabilitado, selecione **habilitar Marketplace privado** para habilitar.
- Se habilitado, selecione **desabilitar Marketplace privado** para desabilitar.

## <a name="private-azure-marketplace-notification-center"></a>Central de notificações do Azure Marketplace privada

O centro de notificações consiste em três tipos de notificações e permite que o administrador do Marketplace execute ações com base na notificação:

- Solicitações de aprovação de usuários para itens que não estão na lista aprovada (consulte [solicitação para adicionar ofertas ou planos](#request-to-add-offers-or-plans) abaixo).
- Novas notificações de plano para ofertas que já têm um ou mais planos na lista aprovada.
- As notificações do plano foram removidas para itens que estão na lista aprovada, mas foram removidas do Azure marketplace global.

Para acessar o centro de notificações:

1. Selecione **notificações** no menu do lado esquerdo.

    [![Mostra o menu notificações.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)

1. Selecione o menu de reticências para obter mais ações.

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Mostra os resultados do menu mais opções.":::

1. Para solicitações de plano, **Mostrar solicitações** abre o formulário de solicitação de aprovação, onde você pode examinar todas as solicitações de usuário para a oferta específica.
1. Selecione **aprovar** ou **rejeitar**.

    [![Mostra as opções de aprovar e rejeitar.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)

1. Selecione o plano a ser aprovado no menu suspenso.
1. Adicione um comentário e selecione **Enviar**.

## <a name="browsing-private-azure-marketplace"></a>Navegando no Azure Marketplace privado

Quando o Azure Marketplace privado estiver habilitado, os usuários verão quais planos foram aprovados pelo administrador do Marketplace.

- Um aviso de **aprovação** verde indica uma oferta de parceiro (que não é da Microsoft) aprovada.
- Um aviso de **aprovação** azul indica uma oferta da Microsoft (incluindo as [distribuições do Linux endossadas](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) que é aprovada.

Os usuários podem filtrar entre ofertas que são e não são aprovadas:

[![Mostra a opção de filtragem.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>Comprar ou implantar no Azure Marketplace privado

Embora a experiência de página de detalhes do produto seja semelhante ao Azure marketplace global, há três cenários particulares específicos do Azure Marketplace.

- Quando um usuário seleciona um plano aprovado, o botão **criar** é habilitado:

    [![Mostra a faixa de oferta indicando que um plano pode ser criado.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)

- Se uma seleção de plano de produto não aparecer na página de detalhes do produto, mas o administrador tiver aprovado um ou mais planos, uma faixa anotará quais planos são aprovados e o botão **criar** será habilitado:

    [![Mostra a faixa de oferta indicando que um plano pode ser criado e mostrando os planos disponíveis.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)

- Quando um usuário seleciona um plano não aprovado, uma faixa anota o plano como não aprovado e o botão **criar** é desabilitado. O usuário ainda pode solicitar a adição do plano à lista aprovada (consulte a próxima seção).

## <a name="request-to-add-offers-or-plans"></a>Solicitação para adicionar ofertas ou planos

Você pode solicitar a adição de uma oferta pública ou um plano que não esteja atualmente aprovado no Azure Marketplace privado.

1. Selecione **solicitação para adicionar** na faixa para abrir o **formulário de solicitação de acesso**.

    [![Mostra a faixa com o link ' solicitar a adição '.](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)

    [![Mostra o formulário de solicitação de acesso para ofertas ou planos.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)

1. Selecione quais planos adicionar à solicitação (**qualquer plano** informa ao administrador do Marketplace que você não tem uma preferência para um plano em uma oferta).

1. Adicione uma **justificativa** e selecione **solicitação** para enviar sua solicitação.
  
    [![Mostra o formulário de solicitação de acesso para ofertas ou planos com entradas de exemplo.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)

1. Uma indicação para uma solicitação pendente será exibida no formulário de solicitação de acesso com uma opção para **retirar a solicitação**.

    [![Mostra uma lista de planos aprovados ou pendentes com o link retirar solicitação.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)

> [!NOTE]
> Depois de enviado, o formulário de solicitação de aprovação será enviado para o [centro de notificações](#private-azure-marketplace-notification-center) para que o administrador do Marketplace examine a solicitação e execute a ação.

## <a name="frequently-asked-questions-faqs"></a>Perguntas frequentes (FAQs)

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a>Já estou bloqueando o aplicativo de terceiros do Marketplace por meio de Azure Policy. Como isso é diferente?

Atualmente, há duas maneiras de restringir serviços de terceiros no Marketplace:

1. Por meio do portal de EA ou do portal do Azure, desabilite serviços de terceiros ou restrinja a "somente SKUs gratuitas ou BYOL".

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Mostra como restringir os serviços no portal do Azure.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="Mostra como restringir serviços no E um portal.":::

2. Crie uma política do Azure para permitir apenas VMs específicas. Para obter detalhes sobre como impor a política para VMs do Windows, consulte [aplicar políticas a VMs do Windows com Azure Resource Manager](https://docs.microsoft.com/azure/virtual-machines/windows/policy).

O Azure Marketplace privado permite mais flexibilidade na restrição e na concessão de ofertas e planos específicos. Ele informa os usuários finais sobre a disponibilidade para implantação na galeria do Marketplace, mesmo antes de tentar implantar serviços de terceiros. Para permitir a implantação de serviços de terceiros, defina o Azure Marketplace como ativado/habilitado no portal de EA e o portal do Azure.

- O Azure Marketplace privado pode organizar soluções de parceiros não limitadas a máquinas virtuais.
- O Azure Marketplace privado pode ser organizado no nível do plano e também pode definir "plano atual e futuro".
- O Azure Marketplace privado pode informar os usuários finais sobre o que o pode e não pode ser implantado.

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a>Qual é a diferença entre uma oferta privada e o Azure Marketplace privado?

Uma **oferta privada** permite que os editores criem planos que só são visíveis para os clientes de destino. Isso permite que eles compartilhem de maneira privada soluções personalizadas com preços negociados, termos e condições particulares e configurações especializadas. Para obter detalhes, consulte [ofertas privadas no Marketplace comercial](https://docs.microsoft.com/azure/marketplace/private-offers).

O **Azure Marketplace privado** no portal do Azure permite que os administradores aprovem previamente quais soluções de terceiros seus usuários podem implantar. Com um Azure Marketplace privado, os usuários podem aproveitar os benefícios do Azure Marketplace encontrando, comprando e implantando ofertas compatíveis. Para gerenciar ofertas privadas baseadas em assinatura no Marketplace privado, o administrador do Marketplace deve ter, no mínimo, a função de "leitura" na assinatura específica.

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a>Adicionei uma oferta privada ao Azure Marketplace particular, por que ela não aparece na guia Gerenciar Marketplace?

As ofertas privadas baseadas em assinatura são visíveis apenas para as assinaturas listadas nas configurações da oferta privada. Para exibir a oferta privada, verifique se o filtro de assinatura global está mostrando todas as assinaturas.

[![Mostra o filtro particular do Marketplace.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a>Podemos incluir imagens personalizadas no Azure Marketplace privado?

Não. O Azure Marketplace privado permite que qualquer administrador de ti gerencie e acesse soluções de terceiros do Azure marketplace global. Como as imagens personalizadas não estão no Azure marketplace global, o administrador de ti não pode escolher as imagens personalizadas. Se você quiser compartilhar imagens personalizadas, use a [Galeria de imagens compartilhadas](https://docs.microsoft.com/azure/virtual-machines/shared-image-galleries).

1. Guia passo a passo criar uma galeria de imagens compartilhadas (SIG) ([CLI](https://docs.microsoft.com/azure/virtual-machines/shared-images-cli), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/shared-images-powershell)).
2. Criar uma definição de imagem em um SIG. O cliente deve escolher **generalizado** para o campo Estado do sistema operacional. ([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).
3. Traga a imagem gerenciada para a Galeria de imagens compartilhadas ([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-powershell)).
4. As imagens de VM SIG residiriam em uma assinatura. Para torná-lo disponível para outras assinaturas, use um registro de aplicativo ([CLI](https://docs.microsoft.com/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/windows/share-images-across-tenants)).

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a>Por que vejo algumas ofertas **aprovadas por padrão** , embora o editor não seja a Microsoft?

A Microsoft dá suporte à tecnologia Linux e de software livre no Azure. As [distribuições do Linux endossadas](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros) têm suporte no Azure e o preço é integrado em máquinas virtuais. Como o agente Linux do Azure já está pré-instalado no Azure Marketplace, ele é tratado como uma oferta da Microsoft. Como as ofertas da Microsoft são aprovadas por padrão, as distribuições do Linux endossadas não podem ser gerenciadas no Azure Marketplace privado e são aprovadas por padrão.

## <a name="contact-support"></a>Contate o suporte

- Para obter suporte ao Azure Marketplace, visite [o Microsoft Q&A](/answers/products/).
