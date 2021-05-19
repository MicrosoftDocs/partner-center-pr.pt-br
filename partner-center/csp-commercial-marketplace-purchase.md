---
title: Comprar ofertas do Marketplace comercial
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como os parceiros do programa CSP podem usar o Marketplace do Partner Center para fazer compras de clientes de ofertas de SaaS de ISVs (fornecedores independentes de software).
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3f5cf4895fa4d66c65215989d808a1dd18ef9064
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147846"
---
# <a name="purchase-commercial-marketplace-products-for-your-customers-in-partner-center"></a>Comprar produtos do Marketplace comercial para seus clientes no Partner Center


**Funções apropriadas**: Administração Global | Agente de administração

Como parceiro no programa CSP (provedor de soluções na nuvem), você pode usar o Marketplace comercial para comprar assinaturas para seus clientes para determinados produtos de SaaS (software como serviço) oferecidos por fornecedores independentes de software (ISVs).

Ao oferecer assinaturas SaaS de ISV aos seus clientes, você pode ajudar a diferenciar seus negócios. Você também pode fornecer aos clientes acesso a pacotes de software que atendam às suas necessidades de negócios específicas. Você gerencia licenças e assinaturas para esses produtos SaaS do Marketplace por meio de editores ISV, assim como gerencia licenças e assinaturas de produtos da Microsoft.

Você pode comprar assinaturas SaaS **baseadas em licença** ou assinaturas baseadas em **uso** . Para saber mais sobre a diferença entre a cobrança baseada em licença e com base no uso, consulte [noções básicas de cobrança](billing-basics.md).

## <a name="purchase-license-based-and-metered-saas-subscriptions-in-partner-center"></a>Comprar assinaturas de SaaS limitadas e baseadas em licença no Partner Center

Você adquire assinaturas para produtos SaaS baseados em licença ou limitados oferecidos por editores ISV usando o mesmo processo usado para comprar assinaturas de produtos da Microsoft.

Para comprar uma assinatura de SaaS limitada ou com base em licença no Partner Center, consulte [criar, suspender ou cancelar assinaturas de cliente](create-a-new-subscription.md#create-a-new-subscription).

Você também pode usar [as APIs](/partner-center/develop/) do Partner Center para criar assinaturas do Marketplace comercial para seus clientes. (Para obter mais informações sobre como usar as APIs do Partner Center, consulte [criar uma assinatura para produtos do Marketplace comercial](/partner-center/develop/create-subscription-azure-marketplace-products).)

>[!IMPORTANT]
> Como um parceiro no programa CSP, você pode comprar assinaturas SaaS **limitadas** ou **baseadas em licença** de editores ISV no Partner Center. Isso significa que você pode comprar qualquer oferta de SaaS **limitada** ou **baseada em licença** que o editor ISV tenha disponibilizado para você, incluindo [ofertas exclusivas](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) às quais você tem acesso. Para comprar ou gerenciar outras ofertas do marketplace comercial de ISVs (como ofertas baseadas em uso que envolvem aplicativos do Azure, contêineres ou VMs), você deve ir para o [portal do Azure](https://portal.azure.com/).

## <a name="purchase-usage-based-subscriptions-in-the-azure-portal"></a>Comprar assinaturas baseadas em uso no portal do Azure

Ao contrário das assinaturas SaaS baseadas em licença de editores ISV de terceiros, as assinaturas baseadas em uso primeiro exigem que um cliente tenha uma assinatura do Azure. A cobrança para o marketplace comercial, recursos baseados em uso, fica abaixo da assinatura do Azure do cliente. Depois que o cliente tiver uma assinatura do Azure, um parceiro no programa CSP poderá seguir estas etapas para comprar uma assinatura do marketplace comercial para eles:

1. Entre no painel Partner Center [e](https://partner.microsoft.com/dashboard)selecione **Clientes** no menu à esquerda.

2. Selecione o cliente específico e, em seguida, **selecione Assinaturas.**  

3. Em **Assinaturas baseadas em uso,** selecione **Todos os recursos**. Isso leva você ao portal de Gerenciamento do Azure.

4. No portal de Gerenciamento do Azure, **selecione Criar um recurso** no menu à esquerda.

5. Selecione **Ver tudo** na parte superior da Azure Marketplace lista.

6. Para restringir sua lista, use filtros na parte superior da lista do Marketplace. Por exemplo, você pode selecionar  **Microsoft** ou **Partner** na lista suspenso Publicador para exibir apenas ofertas da Microsoft ou aquelas de um publicador ISV.

7. Escolha uma oferta específica e, em seguida, **selecione Criar**.

## <a name="next-steps"></a>Próximas etapas

- [Gerenciar ofertas do marketplace comercial](csp-commercial-marketplace-purchase.md)