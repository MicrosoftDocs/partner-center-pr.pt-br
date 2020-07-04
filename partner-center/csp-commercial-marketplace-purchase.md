---
title: Comprar ofertas do Marketplace comercial
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como os parceiros do programa CSP podem usar o Marketplace do Partner Center para fazer compras de clientes de ofertas de SaaS de ISVs (fornecedores independentes de software).
author: rbars
ms.author: rbars
keywords: assinaturas, Marketplace, Marketplace comercial, terceiros, ISV, ofertas de SaaS, programa de provedor de soluções na nuvem, comprar uma oferta, comprar uma assinatura
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0450acd0cfe6586e26baf55c128e64c88f680ba9
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/03/2020
ms.locfileid: "85947699"
---
# <a name="purchase-commercial-marketplace-products-for-your-customers-in-partner-center"></a>Comprar produtos do Marketplace comercial para seus clientes no Partner Center

**Aplica-se a**

- Partner Center
- Parceiros no programa CSP

**Funções apropriadas**

- Administrador global
- Agente administrativo

Como parceiro no programa CSP (provedor de soluções na nuvem), você pode usar o Marketplace comercial para comprar assinaturas para seus clientes para determinados produtos de SaaS (software como serviço) oferecidos por fornecedores independentes de software (ISVs). 

Ao oferecer assinaturas SaaS de ISV aos seus clientes, você pode ajudar a diferenciar seus negócios. Você também pode fornecer aos clientes acesso a pacotes de software que atendam às suas necessidades de negócios específicas. Você gerencia licenças e assinaturas para esses produtos SaaS do Marketplace por meio de editores ISV, assim como gerencia licenças e assinaturas de produtos da Microsoft.

Você pode comprar assinaturas SaaS **baseadas em licença** ou assinaturas baseadas em **uso** . Para saber mais sobre a diferença entre a cobrança baseada em licença e com base no uso, consulte [noções básicas de cobrança](billing-basics.md).

## <a name="purchase-license-based-saas-subscriptions-in-partner-center"></a>Comprar assinaturas SaaS baseadas em licença no Partner Center

Você adquire assinaturas para produtos SaaS baseados em licença oferecidos por editores ISV usando o mesmo processo usado para comprar assinaturas de produtos da Microsoft.

Para comprar uma assinatura SaaS baseada em licença no Partner Center, consulte [criar, suspender ou cancelar assinaturas de cliente](create-a-new-subscription.md#create-a-new-subscription).

Você também pode usar [as APIs](https://docs.microsoft.com/partner-center/develop/) do Partner Center para criar assinaturas do Marketplace comercial para seus clientes. (Para obter mais informações sobre como usar as APIs do Partner Center, consulte [criar uma assinatura para produtos do Marketplace comercial](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products).)

>[!IMPORTANT]
> Como um parceiro no programa CSP, você só pode comprar assinaturas SaaS **baseadas em licença** de editores ISV no Partner Center. Isso significa que você pode comprar qualquer oferta de SaaS **baseada em licença** que o editor ISV disponibilizou para você, incluindo [ofertas exclusivas](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) às quais você tem acesso. Para comprar ou gerenciar outras ofertas de Marketplace comercial de ISVs (como ofertas baseadas em **uso**, limitada ou de consumo que envolvem aplicativos, contêineres ou VMS do Azure), você deve ir para a [portal do Azure](https://portal.azure.com/). Para obter mais informações, consulte o tópico a seguir.

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