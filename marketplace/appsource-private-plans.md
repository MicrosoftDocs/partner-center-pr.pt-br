---
title: Planos privados no Microsoft AppSource
description: Configurando planos privados no Microsoft AppSource (Azure Marketplace).
ms.service: marketplace-customer
ms.topic: how-to
author: Guyshu
ms.author: gushuchm
ms.date: 06/08/2021
robots: noindex
ms.openlocfilehash: a392859c1106c747e0e7c696927ef3b25262e411
ms.sourcegitcommit: a576c9606ade59cef7d0b2d5e1584016740d08eb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2021
ms.locfileid: "112008515"
---
# <a name="private-plans-in-microsoft-appsource"></a><span data-ttu-id="65f44-103">Planos privados no Microsoft AppSource</span><span class="sxs-lookup"><span data-stu-id="65f44-103">Private plans in Microsoft AppSource</span></span>

<span data-ttu-id="65f44-104">Os planos privados são como os editores fornecem planos personalizados para clientes específicos.</span><span class="sxs-lookup"><span data-stu-id="65f44-104">Private plans are how publishers provide custom plans to specific customers.</span></span> <span data-ttu-id="65f44-105">Essa opção agora está disponível em Microsoft AppSource.</span><span class="sxs-lookup"><span data-stu-id="65f44-105">This option is now available in Microsoft AppSource.</span></span> <span data-ttu-id="65f44-106">Os planos privados podem ser vendidos em AppSource para ofertas de SaaS (software como serviço) com o Get to-to-Action **agora** .</span><span class="sxs-lookup"><span data-stu-id="65f44-106">Private plans can be sold on AppSource for software as a service (SaaS) offers with the **Get it now** call-to-action.</span></span>

## <a name="ask-your-isv-for-a-private-plan"></a><span data-ttu-id="65f44-107">Pergunte ao seu ISV um plano privado</span><span class="sxs-lookup"><span data-stu-id="65f44-107">Ask your ISV for a private plan</span></span>

<span data-ttu-id="65f44-108">Para que um plano privado esteja disponível para você no AppSource, você precisa entrar em contato com o ISV diretamente e negociar um preço personalizado e especificações técnicas.</span><span class="sxs-lookup"><span data-stu-id="65f44-108">For a private plan to be available to you in AppSource, you need to contact the ISV directly and negotiate a custom price and technical specifications.</span></span> <span data-ttu-id="65f44-109">Depois que os termos do plano privado forem acordados, o ISV criará um plano para você e o atribuirá à ID de locatário da sua organização, que você precisará fornecer.</span><span class="sxs-lookup"><span data-stu-id="65f44-109">Once the terms of the private plan are agreed to, the ISV will create a plan for you and assign it to your organization’s tenant ID, which you’ll need to provide.</span></span>

### <a name="finding-your-tenant-id"></a><span data-ttu-id="65f44-110">Encontrando sua ID de locatário</span><span class="sxs-lookup"><span data-stu-id="65f44-110">Finding your tenant ID</span></span>

1. <span data-ttu-id="65f44-111">Em AppSource, no canto superior direito, selecione o ícone de perfil de conta e, em seguida, **exiba locatário**.</span><span class="sxs-lookup"><span data-stu-id="65f44-111">In AppSource, in the upper right corner, select your account profile icon and then **View tenant**.</span></span>
2. <span data-ttu-id="65f44-112">Copie a ID do locatário e forneça-a para o ISV.</span><span class="sxs-lookup"><span data-stu-id="65f44-112">Copy the tenant ID and provide it to the ISV.</span></span>

    :::image type="content" source="media/private-offers/find-tenant-id.png" alt-text="Mostra como localizar sua ID de locatário.":::

## <a name="find-a-private-plan-in-appsource"></a><span data-ttu-id="65f44-114">Encontre um plano privado no AppSource</span><span class="sxs-lookup"><span data-stu-id="65f44-114">Find a private plan in AppSource</span></span>

<span data-ttu-id="65f44-115">Pode levar até 48 horas após o ISV publicar o novo plano privado antes de vê-lo em AppSource.</span><span class="sxs-lookup"><span data-stu-id="65f44-115">It can take up to 48 hours after the ISV publishes the new private plan before you see it in AppSource.</span></span> <span data-ttu-id="65f44-116">Para localizar planos privados associados à sua ID de locatário, selecione **planos privados** (ícone de cadeado) no canto superior direito de AppSource.</span><span class="sxs-lookup"><span data-stu-id="65f44-116">To find private plans associated with your tenant ID, select **Private plans** (Lock icon) at the upper right of AppSource.</span></span>

:::image type="content" source="media/private-offers/lock-icon.png" alt-text="Mostra o ícone de cadeado (cadeado) na barra de ferramentas superior.":::

<span data-ttu-id="65f44-118">Se você não estiver conectado, uma mensagem solicitará que você faça isso.</span><span class="sxs-lookup"><span data-stu-id="65f44-118">If you are not signed in, a message will prompt you to do so.</span></span> <span data-ttu-id="65f44-119">Em seguida, você pode comprar os planos privados associados à sua ID de locatário na guia **planos + preços** .</span><span class="sxs-lookup"><span data-stu-id="65f44-119">You can then purchase the private plans associated with your tenant ID on the **Plans + pricing** tab.</span></span>

:::image type="content" source="media/private-offers/plan-pricing-tab.png" alt-text="Mostra as ofertas privadas na guia plano e preços.":::

<span data-ttu-id="65f44-121">Se os planos privados não estiverem disponíveis para seu locatário, uma mensagem irá declarar que você não tem nenhum plano ou oferta particular.</span><span class="sxs-lookup"><span data-stu-id="65f44-121">If private plans are not available for your tenant, a message will state that you don’t have any private plans or offers.</span></span>

## <a name="purchase-a-private-plan"></a><span data-ttu-id="65f44-122">Comprar um plano privado</span><span class="sxs-lookup"><span data-stu-id="65f44-122">Purchase a private plan</span></span>

<span data-ttu-id="65f44-123">Um ISV pode incluir um ou mais planos privados em uma oferta.</span><span class="sxs-lookup"><span data-stu-id="65f44-123">An ISV can include one or more private plans within an offer.</span></span> <span data-ttu-id="65f44-124">Cada oferta pode ter planos públicos e privados, mas os planos privados aparecem em uma página de listagem de oferta separada, acessada no ícone de ofertas particulares (cadeado) no canto superior direito da página.</span><span class="sxs-lookup"><span data-stu-id="65f44-124">Each offer can have both public and private plans, but private plans appear under a separate offer listing page accessed from the Private offers icon (padlock) at the upper right of the page.</span></span>

<span data-ttu-id="65f44-125">Os planos privados disponíveis são exibidos na guia **planos + preços** . Os planos privados têm um emblema azul distintivo.</span><span class="sxs-lookup"><span data-stu-id="65f44-125">Available private plans display on the **Plans + pricing** tab. Private plans have a distinctive blue badge.</span></span>

:::image type="content" source="media/private-offers/private-plans-badge.png" alt-text="Mostra o selo da oferta privada azul ao lado das ofertas privadas.":::

<span data-ttu-id="65f44-127">Para comprar um plano selecionado, selecione **obter agora** e siga as etapas fornecidas.</span><span class="sxs-lookup"><span data-stu-id="65f44-127">To purchase a selected plan, select **Get it now** and follow the steps provided.</span></span>

## <a name="next-steps"></a><span data-ttu-id="65f44-128">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="65f44-128">Next steps</span></span>

- [<span data-ttu-id="65f44-129">O que é o Microsoft AppSource?</span><span class="sxs-lookup"><span data-stu-id="65f44-129">What is Microsoft AppSource?</span></span>](appsource-overview.md)
