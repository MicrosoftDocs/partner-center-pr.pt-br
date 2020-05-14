---
title: Usar opções de multicanal no Partner Center
description: Em alguns casos, os clientes talvez queiram contratar você para provisionar e dar suporte a uma assinatura comprada em outro lugar.
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.assetid: C8B58255-2C7D-4338-A5B0-572BC0F54C0D
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: e96b7cb91915c6ccbc6485fde87b1e061a73e2da
ms.sourcegitcommit: 3849d49261f4f652bd7c0537ebe31558af427c5c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "83362694"
---
# <a name="multi-channel-support"></a><span data-ttu-id="1695f-103">Suporte multicanal</span><span class="sxs-lookup"><span data-stu-id="1695f-103">Multi-channel support</span></span>

<span data-ttu-id="1695f-104">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="1695f-104">**Applies to**</span></span>

- <span data-ttu-id="1695f-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="1695f-105">Partner Center</span></span>
- <span data-ttu-id="1695f-106">Partner Center do Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="1695f-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="1695f-107">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="1695f-107">**Appropriate roles**</span></span>

- <span data-ttu-id="1695f-108">Administrador global</span><span class="sxs-lookup"><span data-stu-id="1695f-108">Global admin</span></span>
- <span data-ttu-id="1695f-109">Administrador de usuários</span><span class="sxs-lookup"><span data-stu-id="1695f-109">User admin</span></span>
- <span data-ttu-id="1695f-110">Agente de vendas</span><span class="sxs-lookup"><span data-stu-id="1695f-110">Sales agent</span></span>

<span data-ttu-id="1695f-111">O recurso de vários canais do Partner Center dá suporte a cenários quando um cliente deseja contratar um parceiro para gerenciar e dar suporte a uma assinatura comprada em outro lugar.</span><span class="sxs-lookup"><span data-stu-id="1695f-111">The Partner Center's multi-channel feature supports scenarios when a customer wants to hire a partner to manage and support a subscription they purchased elsewhere.</span></span> <span data-ttu-id="1695f-112">O suporte multi-canal se aplica quando o cliente:</span><span class="sxs-lookup"><span data-stu-id="1695f-112">Multi-channel support applies when the customer:</span></span>

- <span data-ttu-id="1695f-113">Já adquiriu assinaturas diretamente da Microsoft ou por meio dos programas Advisor, Open ou EA.</span><span class="sxs-lookup"><span data-stu-id="1695f-113">Already purchased subscriptions directly from Microsoft or through the Advisor, Open, or EA programs.</span></span>

- <span data-ttu-id="1695f-114">Comprou as assinaturas de um terceiro, que não está no programa Provedor de Soluções na Nuvem ou de um Parceiro de Distribuição da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1695f-114">Purchased the subscriptions from a third party not in the Cloud Solution Provider program or not a Microsoft Syndication Partner.</span></span> <span data-ttu-id="1695f-115">Os clientes não podem alternar assinaturas baseadas em licença existentes para um parceiro diferente no programa do provedor de soluções de nuvem. eles devem aguardar até o fim do período de assinatura ou cancelar antes de mover.</span><span class="sxs-lookup"><span data-stu-id="1695f-115">Customers can't switch existing license-based subscriptions to a different partner in the Cloud Solution Provider program-they must wait until the end of their subscription period or cancel before moving.</span></span>

| | |
|---------|---------|
|<span data-ttu-id="1695f-116">Serviços baseados em licença</span><span class="sxs-lookup"><span data-stu-id="1695f-116">License-based services</span></span>    | <span data-ttu-id="1695f-117">Para dar suporte a contas de vários canais, você deve solicitar permissões do cliente para gerenciar as assinaturas dele.</span><span class="sxs-lookup"><span data-stu-id="1695f-117">To provide support for multi-channel accounts, you must request permissions from the customer to manage their subscriptions.</span></span> <span data-ttu-id="1695f-118">Para obter mais informações, consulte [solicitar uma relação de revendedor com um cliente](request-a-relationship-with-a-customer.md).</span><span class="sxs-lookup"><span data-stu-id="1695f-118">For more information, see [Request a reseller relationship with a customer](request-a-relationship-with-a-customer.md).</span></span>   |
|<span data-ttu-id="1695f-119">Serviços com base em uso</span><span class="sxs-lookup"><span data-stu-id="1695f-119">Usage-based services</span></span>     |  <span data-ttu-id="1695f-120">Para um cliente que já tem uma assinatura do Microsoft Azure de outro canal, como Advisor, Open ou EA, você precisa criar uma nova assinatura do Azure no Partner Center, inserir manualmente os detalhes da assinatura e, em seguida, cancelar os serviços individuais ou a assinatura inteira.</span><span class="sxs-lookup"><span data-stu-id="1695f-120">For a customer who already has a subscription to Microsoft Azure from another channel, such as Advisor, Open, or EA, you'll need to create a new Azure subscription in Partner Center, manually enter the subscription details, and then cancel the individual services or the entire subscription.</span></span> <span data-ttu-id="1695f-121">O Azure CSP pode coexistir com diferentes canais.</span><span class="sxs-lookup"><span data-stu-id="1695f-121">Azure CSP can coexist with different channels.</span></span><br/><br/> <span data-ttu-id="1695f-122">Por exemplo, para um cliente que já tem uma assinatura do Microsoft Azure de outro parceiro, você pode alternar os serviços do Azure para o outro parceiro.</span><span class="sxs-lookup"><span data-stu-id="1695f-122">For a customer who already has a subscription to Microsoft Azure from another partner, for example, you can switch Azure services to the other partner.</span></span>  <span data-ttu-id="1695f-123">Para obter mais informações, consulte [Alternar assinaturas do Azure para um parceiro diferente](switch-azure-subscriptions-to-a-different-partner.md).</span><span class="sxs-lookup"><span data-stu-id="1695f-123">For more information, see [Switch Azure subscriptions to a different partner](switch-azure-subscriptions-to-a-different-partner.md).</span></span> |

> [!IMPORTANT]  
> <span data-ttu-id="1695f-124">Um parceiro CSP não revende serviços online para outro parceiro CSP no momento.</span><span class="sxs-lookup"><span data-stu-id="1695f-124">A CSP partner cannot resell online services to another CSP partner currently.</span></span> <span data-ttu-id="1695f-125">A Microsoft revisa continuamente as políticas e competências de todos os programas.</span><span class="sxs-lookup"><span data-stu-id="1695f-125">Microsoft continuously reviews policies and capabilities of all programs.</span></span> <span data-ttu-id="1695f-126">Todos os comunicados sobre as versões de recursos serão anunciados por meio dos canais de comunicação usuais, incluindo o Partner Center.</span><span class="sxs-lookup"><span data-stu-id="1695f-126">Any announcements about feature releases will be announced through the usual communication channels, including the Partner Center.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1695f-127">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="1695f-127">Next steps</span></span>

[<span data-ttu-id="1695f-128">Trabalhar com outros parceiros</span><span class="sxs-lookup"><span data-stu-id="1695f-128">Work with other partners</span></span>](work-with-other-partners.md)

- <span data-ttu-id="1695f-129">Se você for um revendedor indireto, consulte [parceiro com provedores indiretos](indirect-reseller-tasks-in-partner-center.md).</span><span class="sxs-lookup"><span data-stu-id="1695f-129">If you're an indirect reseller, see [Partner with indirect providers](indirect-reseller-tasks-in-partner-center.md).</span></span>

- <span data-ttu-id="1695f-130">Se você for um provedor indireto, consulte [parceiro com revendedores indiretos](indirect-provider-tasks-in-partner-center.md).</span><span class="sxs-lookup"><span data-stu-id="1695f-130">If you're an indirect provider, see [Partner with indirect resellers](indirect-provider-tasks-in-partner-center.md).</span></span>
