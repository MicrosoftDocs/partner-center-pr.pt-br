---
title: Ofertas privadas no Azure Marketplace
description: Saiba mais sobre as ofertas privadas no Azure Marketplace.
ms.service: marketplace-customer
ms.topic: article
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: 72e886a7cfad067b40674f30a9a21810d832994a
ms.sourcegitcommit: 3a2415ab9833d5c574ad76d462f526a131c24f33
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "103412651"
---
# <a name="private-offers-in-azure-marketplace"></a><span data-ttu-id="044ca-103">Ofertas privadas no Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="044ca-103">Private offers in Azure Marketplace</span></span>

<span data-ttu-id="044ca-104">As ofertas privadas são como os editores fornecem planos personalizados para clientes específicos.</span><span class="sxs-lookup"><span data-stu-id="044ca-104">Private offers are how publishers provide custom plans to specific customers.</span></span> <span data-ttu-id="044ca-105">Atualmente, essa opção tem suporte apenas na experiência do Azure Marketplace no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="044ca-105">This option is currently supported only in the Azure Marketplace experience in the Azure portal.</span></span> <span data-ttu-id="044ca-106">As ofertas privadas só estão disponíveis para ofertas pagas que podem ser adquiridas e instaladas diretamente do portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="044ca-106">Private offers are only available for paid offers that can be purchased and directly installed from the Azure portal.</span></span> <span data-ttu-id="044ca-107">O Publisher não pode criar ofertas privadas para serviços de consultoria, qualquer serviço que tenha **contato comigo** como um plano de ação ou qualquer serviço gratuito, independentemente de poder ser instalado ou não no Portal.</span><span class="sxs-lookup"><span data-stu-id="044ca-107">Publisher cannot create private offers for consulting services, any service that has **Contact me** as a call-to-action, or any free service, regardless of whether it can be installed from the portal or not.</span></span>

## <a name="find-private-offers-in-the-azure-portal"></a><span data-ttu-id="044ca-108">Encontre ofertas privadas no portal do Azure</span><span class="sxs-lookup"><span data-stu-id="044ca-108">Find private offers in the Azure portal</span></span>

<span data-ttu-id="044ca-109">Quando um parceiro publica uma oferta privada, ele fica visível somente para usuários qualificados na seção **Marketplace** do portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="044ca-109">When a partner publishes a private offer, it is visible only to eligible users in the **Marketplace** section of the Azure portal.</span></span> <span data-ttu-id="044ca-110">Esses usuários são definidos pela ID de assinatura ou ID de locatário, dependendo do tipo de oferta.</span><span class="sxs-lookup"><span data-stu-id="044ca-110">These users are defined by subscription ID or tenant ID, depending on the offer type.</span></span> <span data-ttu-id="044ca-111">Se você estiver qualificado para ofertas privadas, há duas maneiras de encontrá-las no Portal.</span><span class="sxs-lookup"><span data-stu-id="044ca-111">If you are eligible for  private offers, there are two ways to find them in the portal.</span></span>

> [!NOTE]
> <span data-ttu-id="044ca-112">As ofertas privadas atualmente não são pesquisáveis ou filtráveis (por categoria) no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="044ca-112">Private offers are currently not searchable or filterable (by category) in the Azure portal.</span></span>

<span data-ttu-id="044ca-113">Na portal do Azure, selecione **+ criar um recurso** ou pesquise "Marketplace" para ir para a página do **Marketplace** .</span><span class="sxs-lookup"><span data-stu-id="044ca-113">In the Azure portal, select **+ Create a resource** or search for “marketplace” to go to the **Marketplace** page.</span></span> <span data-ttu-id="044ca-114">Se você estiver qualificado para ofertas privadas, verá a faixa **você tem as ofertas privadas disponíveis** na parte superior da página.</span><span class="sxs-lookup"><span data-stu-id="044ca-114">If you are eligible for private offers, you will see the **You have private offers available** banner on the top of the page.</span></span> <span data-ttu-id="044ca-115">Selecione **Exibir ofertas privadas** para ir para sua página de ofertas particulares.</span><span class="sxs-lookup"><span data-stu-id="044ca-115">Select **View private offers** to go to your private offers page.</span></span>

:::image type="content" source="media/private-offers/private-offers-banner.png" alt-text="A faixa que é exibida quando você tem ofertas privadas disponíveis.":::

<span data-ttu-id="044ca-117">Como alternativa, se você vir a faixa ofertas particulares, também poderá rolar até a parte inferior da página Galeria de produtos e verá um subconjunto de suas ofertas privadas.</span><span class="sxs-lookup"><span data-stu-id="044ca-117">Alternately, if you see the private offers banner, you can also scroll to the bottom of the product gallery page and you will see a subset of your private offers.</span></span> <span data-ttu-id="044ca-118">Selecione o link para **Ver mais** para acessar sua página de ofertas particulares.</span><span class="sxs-lookup"><span data-stu-id="044ca-118">Select the link to **See More** to go to your private offers page.</span></span>

:::image type="content" source="media/private-offers/see-more-link.png" alt-text="Mostra as ofertas privadas na parte inferior da tela, juntamente com o link Ver mais.":::

## <a name="review-private-plans"></a><span data-ttu-id="044ca-120">Examinar planos privados</span><span class="sxs-lookup"><span data-stu-id="044ca-120">Review private plans</span></span>

<span data-ttu-id="044ca-121">Uma oferta privada é, na verdade, um plano privado dentro de uma oferta.</span><span class="sxs-lookup"><span data-stu-id="044ca-121">A private offer is actually a private plan within an offer.</span></span> <span data-ttu-id="044ca-122">Cada oferta pode ter vários planos, públicos e privados, mas os planos privados são mostrados em uma listagem separada dos planos públicos.</span><span class="sxs-lookup"><span data-stu-id="044ca-122">Each offer can have multiple plans, both public and private, but private plans are shown under a separate listing from public plans.</span></span>

<span data-ttu-id="044ca-123">Você pode ver os planos privados disponíveis na guia **planos** , marcados com um selo **particular** distintivo:</span><span class="sxs-lookup"><span data-stu-id="044ca-123">You can see the available private plans under the **Plans** tab, marked with a distinctive **Private** badge:</span></span>

:::image type="content" source="media/private-offers/private-badge.png" alt-text="Uma página de planos marcados como particulares.":::

<span data-ttu-id="044ca-125">Se você tiver mais de uma assinatura, verá todas as ofertas privadas disponíveis para todas as suas assinaturas.</span><span class="sxs-lookup"><span data-stu-id="044ca-125">If you have more than one subscription, you will see all private offers available for all your subscriptions.</span></span> <span data-ttu-id="044ca-126">Ao selecionar **criar**, você será encaminhado para a página de criação de recursos para começar a configurar o recurso.</span><span class="sxs-lookup"><span data-stu-id="044ca-126">When you select **Create**, you are routed to the resource creation page to start configuring your resource.</span></span>

<span data-ttu-id="044ca-127">Se você selecionar **criar** e tiver várias assinaturas, mas nem todas elas forem adicionadas ao plano privado, sua assinatura padrão poderá não ser a assinatura qualificada para esta oferta privada.</span><span class="sxs-lookup"><span data-stu-id="044ca-127">If you select **Create** and have multiple subscriptions, but not all of them are added to the private plan, your default subscription may not be the subscription eligible for this private offer.</span></span> <span data-ttu-id="044ca-128">Nesse caso, selecione a assinatura correta.</span><span class="sxs-lookup"><span data-stu-id="044ca-128">In this case, select the correct subscription.</span></span>

:::image type="content" source="media/private-offers/select-correct-subscription.png" alt-text="O link mostrando que há mais ofertas privadas disponíveis.":::

## <a name="next-steps"></a><span data-ttu-id="044ca-130">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="044ca-130">Next steps</span></span>

- [<span data-ttu-id="044ca-131">O que é o Azure Marketplace?</span><span class="sxs-lookup"><span data-stu-id="044ca-131">What is Azure Marketplace?</span></span>](azure-marketplace-overview.md)
