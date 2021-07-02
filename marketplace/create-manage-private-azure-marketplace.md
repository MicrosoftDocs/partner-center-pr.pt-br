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
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a>Criar e gerenciar dados Azure Marketplace privado no portal do Azure

A Azure Marketplace privada permite que os administradores controlem quais soluções de terceiros seus usuários podem usar. Ele faz isso permitindo que o usuário implante apenas ofertas aprovadas pelo administrador e que estão em conformidade com as políticas da sua empresa. Com o private Azure Marketplace, os usuários podem pesquisar ofertas em conformidade na loja online para comprar e implantar.

Como administrador do Marketplace (função atribuída), você começará com um Armazenamento Privado desabilitado e vazio, no qual poderá adicionar suas ofertas e planos aprovados. Este artigo explica como atribuir a função necessária, criar um armazenamento privado, gerenciar itens, aprovar solicitações de usuário e habilitar o Azure Marketplace privado para seus usuários.

> [!NOTE]
> - O Azure Marketplace privado está em um nível de locatário, portanto, todos os usuários no locatário verão a mesma lista de convidados.
> - Todas as soluções da Microsoft (incluindo [Distribuições endossadas](/azure/virtual-machines/linux/endorsed-distros)do Linux ) são adicionadas automaticamente ao Private Azure Marketplace.

## <a name="assign-the-marketplace-admin-role"></a>Atribuir a função de administrador do Marketplace

O locatário Administrador global deve atribuir a função de administrador do **Marketplace** ao administrador Azure Marketplace privado que gerenciará o armazenamento privado.

>[!IMPORTANT]
> O acesso ao gerenciamento Azure Marketplace privado só está disponível para administradores de IT com a função de administrador do Marketplace atribuída.

### <a name="prerequisites"></a>Pré-requisitos

Esses pré-requisitos são necessários antes que você possa atribuir a função administrador do Marketplace a um usuário no escopo do locatário:

- Você tem acesso a um **Administrador global** usuário.
- O locatário tem pelo menos uma assinatura (pode ser qualquer tipo).
- O Administrador global usuário recebe a **função** Colaborador ou superior para a assinatura escolhida.

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a>Atribuir a função de administrador do Marketplace com controle de acesso (IAM)

1. Entre no [portal do Azure](https://portal.azure.com/).

1. Selecione **Todos os serviços** e, em seguida, **Marketplace.**

1. Selecione **Marketplace Privado** no menu à esquerda.

   :::image type="content" source="media/private-azure/private-marketplace.png" lightbox="media/private-azure/private-marketplace-zoom.png" alt-text="Mostra a opção de menu do marketplace privado no lado esquerdo do Marketplace.":::

1. Selecione **Controle de acesso (IAM)** para atribuir a função de administrador do Marketplace.

   :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Mostra a tela controle de acesso I A M.":::

1. Selecione **+Adicionar** > **Adicionar atribuição de função**.

1. Em **Função**, escolha Administrador **do Marketplace.**

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Mostra o menu Atribuição de função.":::

1. Selecione o usuário desejado na lista suspenso e, em seguida, selecione **Feito.**

### <a name="assign-the-marketplace-admin-role-with-powershell"></a>Atribuir a função de administrador do Marketplace com o PowerShell

Use o script do PowerShell a seguir para atribuir a função de Administrador do Marketplace; ele requer os seguintes parâmetros:

- **TenantId:** A ID do locatário no escopo (a função de administrador do Marketplace é atribuível no escopo do locatário).
- **SubscriptionId:** Uma assinatura da qual o administrador global tem **a função Colaborador** ou mais atribuída.
- **GlobalAdminUsername:** O nome de usuário do administrador global.
- **UsernameToAssignRoleFor:** O nome de usuário ao qual a função de administrador do Marketplace será atribuída.

> [!NOTE]
> Para usuários convidados para o locatário, pode levar até 48 horas até que sua conta seja disponibilizada para atribuir a função de Administrador do Marketplace. Para obter mais informações, consulte [Propriedades de um usuário Azure Active Directory colaboração B2B](/azure/active-directory/b2b/user-properties).

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

Para obter mais informações sobre os cmdlets contidos no módulo do PowerShell do Az.Portal, [consulte Microsoft Azure PowerShell: cmdlets do Painel do Portal](/powershell/module/az.portal/).

## <a name="create-private-azure-marketplace"></a>Criar uma conta Azure Marketplace

1. Entre no [portal do Azure](https://portal.azure.com/).
2. Selecione **Todos os serviços** e, em seguida, **Marketplace.**

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Mostra a portal do Azure principal.":::

3. Selecione **Marketplace Privado** no menu à esquerda.

4. Selecione **Introdução** para criar Azure Marketplace privado (você só precisa fazer isso uma vez).

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Mostra como selecionar o &quot;Introdução na janela portal do Azure&quot; principal.":::

    Se o Azure Marketplace privado já existir para esse locatário, **Gerenciar Marketplace** será selecionado por padrão.

5. Depois de concluído, você terá uma conta privada vazia e desabilitada Azure Marketplace.

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Mostra a tela de Azure Marketplace privada vazia.":::

## <a name="add-items-from-gallery"></a>Adicionar itens da galeria

Um item é uma combinação de uma oferta e um plano. Você pode pesquisar e adicionar itens na página Gerenciar Marketplace.

1. Selecione **Adicionar itens**.

2. Navegue **pela Galeria** ou use o campo de pesquisa para encontrar o item que você deseja.

   :::image type="content" source="media/private-azure/marketplace-gallery.png" lightbox="media/private-azure/marketplace-gallery-zoom.png" alt-text="Mostra como procurar na galeria ou usar o campo de pesquisa.":::

3. Por padrão, ao adicionar uma nova oferta, todos os planos atuais serão adicionados à lista aprovada. Para modificar a seleção de plano antes de adicionar os itens selecionados, selecione o menu suspenso no peças da oferta e atualize os planos necessários.

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Mostra como atualizar os planos necessários.":::

4. Selecione **Feito** na parte inferior esquerda depois de fazer suas seleções.

>[!Note]
> **Adicionar itens** ao Marketplace estará disponível apenas para ofertas que não são da Microsoft. As soluções da Microsoft (incluindo [Distribuições endossadas](/azure/virtual-machines/linux/endorsed-distros)do Linux ) serão marcadas como "Aprovadas por padrão" e não poderão ser gerenciadas no Marketplace Privado.

## <a name="edit-items-plans"></a>Editar planos do item

Você pode editar os planos de um item na página Gerenciar Marketplace.

1. Na coluna **Planos,** revise os planos disponíveis no menu suspenso desse item.

2. Marque ou des marque as caixas de seleção para escolher quais planos disponibilizar aos usuários.

   :::image type="content" source="media/private-azure/edit-items.png" alt-text="Mostra como selecionar ou limpar a caixa de seleção do item necessário.":::

   > [!NOTE]
   > Cada oferta precisa de pelo menos um plano selecionado para que a atualização ocorra. Para remover todos os planos relacionados a uma oferta, exclua a oferta inteira (consulte a próxima seção).

## <a name="delete-offers"></a>Excluir ofertas

Na página Gerenciar Marketplace, marque a caixa de seleção ao lado do nome da oferta (veja a tela acima) e **selecione Excluir itens**.

## <a name="enabledisable-private-azure-marketplace"></a>Habilitar/desabilitar a Azure Marketplace

Na página Gerenciar Marketplace, você verá uma dessas faixas, que mostram o estado atual do aplicativo Azure Marketplace:

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Mostra a faixa &quot;Desabilitar estado&quot;.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Mostra a faixa &quot;Habilitar estado&quot;.":::

Você pode habilitar ou desabilitar a Azure Marketplace privada conforme necessário.

- Se desabilitado, selecione **Habilitar Marketplace Privado** para habilitar.
- Se habilitado, selecione **Desabilitar Marketplace Privado** para desabilitar.

## <a name="private-azure-marketplace-notification-center"></a>Central de Azure Marketplace privada

O Centro de Notificações consiste em três tipos de notificações e permite que o administrador do Marketplace tome medidas com base na notificação:

- Solicitações de aprovação de usuários para itens que não estão na lista aprovada (consulte [Solicitação para adicionar ofertas ou planos](#request-to-add-offers-or-plans) abaixo).
- Novas notificações de plano para ofertas que já têm um ou mais planos na lista aprovada.
- Remoção das notificações de plano para itens que estão na lista aprovada, mas que foram removidas do Azure Marketplace.

Para acessar o centro de notificações:

1. Selecione **Notificações no** menu do lado esquerdo.

   :::image type="content" source="media/private-azure/marketplace-notifications-small.png" lightbox="media/private-azure/marketplace-notifications.png" alt-text="Mostra o menu Notificações.":::

1. Selecione o menu de reellipse para obter mais ações.

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Mostra os resultados do menu Mais Opções.":::

1. Para solicitações de plano, **Mostrar solicitações** abre o formulário de solicitação de aprovação, no qual você pode revisar todas as solicitações de usuário para a oferta específica.
1. Selecione **Aprovar** ou **Rejeitar**.

   :::image type="content" source="media/private-azure/notifications-approve-reject-small.png" lightbox="media/private-azure/notifications-approve-reject.png" alt-text="Mostra as opções aprovar e rejeitar.":::

1. Selecione o plano a ser aprovado no menu suspenso.
1. Adicione um comentário e selecione **Enviar**.

## <a name="browsing-private-azure-marketplace"></a>Navegação privada Azure Marketplace

Quando a Azure Marketplace privada estiver habilitada, os usuários verão quais planos o administrador do Marketplace aprovou.

- Um aviso **aprovado** verde indica uma oferta de parceiro (não Microsoft) aprovada.
- Um aviso **azul Aprovado** indica uma oferta da Microsoft (incluindo distribuições [endossada do Linux](/azure/virtual-machines/linux/endorsed-distros)) aprovada.

Os usuários podem filtrar entre ofertas que são e não foram aprovadas:

   :::image type="content" source="media/private-azure/filter-option-small.png" lightbox="media/private-azure/filter-option.png" alt-text="Mostra a opção de filtragem.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>Comprar ou implantar em aplicativos Azure Marketplace

Embora a experiência da página de detalhes do produto seja semelhante à Azure Marketplace global, há três cenários Azure Marketplace específicos.

- Quando um usuário seleciona um plano aprovado, o botão **criar** é habilitado:

   :::image type="content" source="media/private-azure/button-create-enabled-small.png" lightbox="media/private-azure/button-create-enabled.png" alt-text="Mostra a faixa de oferta indicando que um plano pode ser criado.":::

- Se uma seleção de plano de produto não aparecer na página de detalhes do produto, mas o administrador tiver aprovado um ou mais planos, uma faixa anotará quais planos são aprovados e o botão **criar** será habilitado:

   :::image type="content" source="media/private-azure/button-create-enabled-and-plans-small.png" lightbox="media/private-azure/button-create-enabled-and-plans.png" alt-text="Mostra a faixa de oferta indicando que um plano pode ser criado e mostrando os planos disponíveis.":::

- Quando um usuário seleciona um plano não aprovado, uma faixa anota o plano como não aprovado e o botão **criar** é desabilitado. O usuário ainda pode solicitar a adição do plano à lista aprovada (consulte a próxima seção).

## <a name="request-to-add-offers-or-plans"></a>Solicitação para adicionar ofertas ou planos

Você pode solicitar a adição de uma oferta pública ou um plano que não esteja atualmente aprovado no Azure Marketplace privado.

1. Selecione **solicitação para adicionar** na faixa para abrir o **formulário de solicitação de acesso**.

   :::image type="content" source="media/private-azure/request-banner-small.png" lightbox="media/private-azure/request-banner.png" alt-text="Mostra a faixa com o link ' solicitar a adição '.":::

   :::image type="content" source="media/private-azure/access-request-form-small.png" lightbox="media/private-azure/access-request-form.png" alt-text="Mostra o formulário de solicitação de acesso para ofertas ou planos.":::

1. Selecione quais planos adicionar à solicitação (**qualquer plano** informa ao administrador do Marketplace que você não tem uma preferência para um plano em uma oferta).

1. Adicione uma **justificativa** e selecione **solicitação** para enviar sua solicitação.

   :::image type="content" source="media/private-azure/access-request-form-filled-small.png" lightbox="media/private-azure/access-request-form-filled.png" alt-text="Mostra o formulário de solicitação de acesso para ofertas ou planos com entradas de exemplo.":::

1. Uma indicação para uma solicitação pendente será exibida no formulário de solicitação de acesso com uma opção para **retirar a solicitação**.

   :::image type="content" source="media/private-azure/approved-pending-plans-small.png" lightbox="media/private-azure/approved-pending-plans.png" alt-text="Mostra uma lista de planos aprovados ou pendentes com o link retirar solicitação.":::

> [!NOTE]
> Depois de enviado, o formulário de solicitação de aprovação será enviado para o [centro de notificações](#private-azure-marketplace-notification-center) para que o administrador do Marketplace examine a solicitação e execute a ação.

> [!CAUTION]
> A aprovação no Marketplace privado não indica a aquisição de uma solução.

## <a name="frequently-asked-questions-faqs"></a>Perguntas frequentes (FAQs)

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a>Já estou bloqueando o aplicativo de terceiros do Marketplace por meio de Azure Policy. Como isso é diferente?

Atualmente, há duas maneiras de restringir serviços de terceiros no Marketplace:

1. Por meio do portal de EA ou do portal do Azure, desabilite serviços de terceiros ou restrinja a "somente SKUs gratuitas ou BYOL".

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Mostra como restringir os serviços no portal do Azure.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="Mostra como restringir serviços no E um portal.":::

2. Crie uma política do Azure para permitir apenas VMs específicas. para obter detalhes sobre como impor a política para Windows vms, consulte [aplicar políticas para Windows vms com Azure Resource Manager](/azure/virtual-machines/windows/policy).

O Azure Marketplace privado permite mais flexibilidade na restrição e na concessão de ofertas e planos específicos. Ele informa os usuários finais sobre a disponibilidade para implantação na galeria do Marketplace, mesmo antes de tentar implantar serviços de terceiros. Para permitir a implantação de serviços de terceiros, defina o Azure Marketplace como ativado/habilitado no portal de EA e o portal do Azure.

- O Azure Marketplace privado pode organizar soluções de parceiros não limitadas a máquinas virtuais.
- O Azure Marketplace privado pode ser organizado no nível do plano e também pode definir "plano atual e futuro".
- O Azure Marketplace privado pode informar os usuários finais sobre o que o pode e não pode ser implantado.

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a>Qual é a diferença entre uma oferta privada e o Azure Marketplace privado?

Uma **oferta privada** permite que os editores criem planos que só são visíveis para os clientes de destino. Isso permite que eles compartilhem de maneira privada soluções personalizadas com preços negociados, termos e condições particulares e configurações especializadas. Para obter detalhes, consulte [ofertas privadas no Marketplace comercial](/azure/marketplace/private-offers).

O **Azure Marketplace privado** no portal do Azure permite que os administradores aprovem previamente quais soluções de terceiros seus usuários podem implantar. Com um Azure Marketplace privado, os usuários podem aproveitar os benefícios do Azure Marketplace encontrando, comprando e implantando ofertas compatíveis. Para gerenciar ofertas privadas baseadas em assinatura no Marketplace privado, o administrador do Marketplace deve ter, no mínimo, a função de "leitura" na assinatura específica.

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a>Adicionei uma oferta privada ao Azure Marketplace particular, por que ela não aparece na guia Gerenciar Marketplace?

As ofertas privadas baseadas em assinatura são visíveis apenas para as assinaturas listadas nas configurações da oferta privada. Para exibir a oferta privada, verifique se o filtro de assinatura global está mostrando todas as assinaturas.

   :::image type="content" source="media/private-azure/private-marketplace-filter.png" lightbox="media/private-azure/private-marketplace-filter.png" alt-text="Mostra o filtro particular do Marketplace.":::

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a>Podemos incluir imagens personalizadas no Azure Marketplace privado?

Não. O Azure Marketplace privado permite que qualquer administrador de ti gerencie e acesse soluções de terceiros do Azure marketplace global. Como as imagens personalizadas não estão no Azure marketplace global, o administrador de ti não pode escolher as imagens personalizadas. Se você quiser compartilhar imagens personalizadas, use a [Galeria de imagens compartilhadas](/azure/virtual-machines/shared-image-galleries).

1. Guia passo a passo criar uma galeria de imagens compartilhadas (SIG) ([CLI](/azure/virtual-machines/shared-images-cli), [PowerShell](/azure/virtual-machines/shared-images-powershell)).
2. Criar uma definição de imagem em um SIG. O cliente deve escolher **generalizado** para o campo Estado do sistema operacional. ([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).
3. Traga a imagem gerenciada para a Galeria de imagens compartilhadas ([CLI](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).
4. As imagens de VM SIG residiriam em uma assinatura. Para torná-lo disponível para outras assinaturas, use um registro de aplicativo ([CLI](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)).

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a>Por que vejo algumas ofertas **aprovadas por padrão** , embora o editor não seja a Microsoft?

A Microsoft dá suporte à tecnologia Linux e de software livre no Azure. As [distribuições do Linux endossadas](/azure/virtual-machines/linux/endorsed-distros) têm suporte no Azure e o preço é integrado em máquinas virtuais. Como o agente Linux do Azure já está pré-instalado no Azure Marketplace, ele é tratado como uma oferta da Microsoft. Como as ofertas da Microsoft são aprovadas por padrão, as distribuições do Linux endossadas não podem ser gerenciadas no Azure Marketplace privado e são aprovadas por padrão.

## <a name="contact-support"></a>Contate o suporte

- Para obter suporte ao Azure Marketplace, visite [o Microsoft Q&A](/answers/products/).