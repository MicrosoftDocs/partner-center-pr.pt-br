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
ms.openlocfilehash: 841308d535d4071ee0a8eabf3e70325edea5777c
ms.sourcegitcommit: a78dd3c532860d01867d116bfb4e2c88b84bcd25
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/08/2021
ms.locfileid: "97979708"
---
# <a name="purchase-commercial-marketplace-products-for-your-customers-in-partner-center"></a>Comprar produtos do Marketplace comercial para seus clientes no Partner Center


**Funções apropriadas**

- Administrador global
- Agente administrativo

Como parceiro no programa CSP (provedor de soluções na nuvem), você pode usar o Marketplace comercial para comprar assinaturas para seus clientes para determinados produtos de SaaS (software como serviço) oferecidos por fornecedores independentes de software (ISVs).

Ao oferecer assinaturas SaaS de ISV aos seus clientes, você pode ajudar a diferenciar seus negócios. Você também pode fornecer aos clientes acesso a pacotes de software que atendam às suas necessidades de negócios específicas. Você gerencia licenças e assinaturas para esses produtos SaaS do Marketplace por meio de editores ISV, assim como gerencia licenças e assinaturas de produtos da Microsoft.

Você pode comprar assinaturas SaaS **baseadas em licença** ou assinaturas baseadas em **uso** . Para saber mais sobre a diferença entre a cobrança baseada em licença e com base no uso, consulte [noções básicas de cobrança](billing-basics.md).

## <a name="purchase-license-based-and-metered-saas-subscriptions-in-partner-center"></a>Comprar assinaturas de SaaS limitadas e baseadas em licença no Partner Center

Você adquire assinaturas para produtos SaaS baseados em licença ou limitados oferecidos por editores ISV usando o mesmo processo usado para comprar assinaturas de produtos da Microsoft.

Para comprar uma assinatura de SaaS limitada ou com base em licença no Partner Center, consulte [criar, suspender ou cancelar assinaturas de cliente](create-a-new-subscription.md#create-a-new-subscription).

Você também pode usar [as APIs](/partner-center/develop/) do Partner Center para criar assinaturas do Marketplace comercial para seus clientes. (Para obter mais informações sobre como usar as APIs do Partner Center, consulte [criar uma assinatura para produtos do Marketplace comercial](/partner-center/develop/create-subscription-azure-marketplace-products).)

>[!IMPORTANT]
> Como um parceiro no programa CSP, você pode comprar assinaturas SaaS **limitadas** ou **baseadas em licença** de editores ISV no Partner Center. Isso significa que você pode comprar qualquer oferta de SaaS **limitada** ou **baseada em licença** que o editor ISV tenha disponibilizado para você, incluindo [ofertas exclusivas](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) às quais você tem acesso. Para comprar ou gerenciar outras ofertas de Marketplace comercial de ISVs (como ofertas baseadas em uso que envolvem aplicativos, contêineres ou VMs do Azure), você deve ir para a [portal do Azure](https://portal.azure.com/).

## <a name="purchase-usage-based-subscriptions-in-the-azure-portal"></a>Comprar assinaturas baseadas no uso no portal do Azure

Ao contrário das assinaturas SaaS baseadas em licença de editores de ISVs de terceiros, as assinaturas baseadas em uso primeiro exigem que um cliente tenha uma assinatura do Azure. Cobrança para o Marketplace comercial, os recursos baseados em uso se enquadram na assinatura do Azure do cliente. Depois que o cliente tiver uma assinatura do Azure, um parceiro no programa CSP poderá seguir estas etapas para comprar uma assinatura do Marketplace comercial para elas:

1. Entre no [painel](https://partner.microsoft.com/dashboard)do Partner Center e selecione **clientes** no menu à esquerda.

2. Selecione o cliente específico e, em seguida, selecione **assinaturas**.  

3. Em **assinaturas baseadas em uso**, selecione **todos os recursos**. Isso leva você para o portal de gerenciamento do Azure.

4. No portal de gerenciamento do Azure, selecione **criar um recurso** no menu à esquerda.

5. Selecione **ver tudo** na parte superior da lista do Azure Marketplace.

6. Para restringir sua lista, use filtros na parte superior da lista do Marketplace. Por exemplo, você pode selecionar **Microsoft** ou **Partner** na lista suspensa **Publicador** para exibir apenas ofertas da Microsoft ou de um editor ISV.

7. Escolha uma oferta específica e, em seguida, selecione **criar**.

## <a name="next-steps"></a>Próximas etapas

- [Gerenciar ofertas do Marketplace comercial](csp-commercial-marketplace-purchase.md)