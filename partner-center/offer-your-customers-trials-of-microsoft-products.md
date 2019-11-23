---
title: Oferecer avaliações de produtos da Microsoft aos clientes | Partner Center
ms.topic: article
ms.date: 11/21/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Seus clientes podem testar produtos de assinatura da Microsoft durante 30 dias. You can sign up for these trials in the catalog just like many other online services.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: ca774233fa6d5314e57f1ab2eb2a73b6037223e5
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/22/2019
ms.locfileid: "74384837"
---
# <a name="offer-your-customers-trials-of-microsoft-products"></a>Oferecer aos clientes avaliações de produtos da Microsoft

Aplica-se a:

- Partner Center

Uma boa maneira de apresentar novos produtos da Microsoft aos clientes é oferecendo avaliações gratuitas de 30 dias. Você pode se inscrever para as avaliações no catálogo da mesma forma que se inscreve em muitos outros serviços online. Todos os parceiros podem participar.

## <a name="available-trial-offers"></a>Available trial offers

You can find all of your outstanding trial offers on the **Customer** page. This page lists all subscriptions, including free trials and paid subscriptions. (This feature is not currently available in China.)

Each customer is entitled to one free trial for each available offer. Por exemplo, eles podem obter uma avaliação gratuita do Office 365 Business Premium e uma avaliação gratuita do Office 365 E3. However, if the customer already owns the offer, they can't use a free trial for that offer.

### <a name="available-products"></a>Available products

As avaliações gratuitas estão disponíveis para os seguintes produtos:

- Office 365 Business Premium
- Office 365 E3
- Office 365 E5 with PSTN
- Office 365 E5 without PSTN
- Enterprise Mobility & Security E5
- Dynamics 365 Customer Engagement Plan 1
- Dynamics 365 for Financials
- Microsoft 365 Business

Nós fornecemos avaliações gratuitas para esses produtos porque eles são as ofertas de negócios mais abrangentes e populares. É possível que adicionemos outras ofertas de avaliação gratuita no futuro.

Currently, there are **no free trials** for government offers, education offers, or add-on offers.

## <a name="licenses-for-free-trial-offers"></a>Licenses for free trial offers

All free trials provide 25 licenses. You can't change this number during the trial. You can't add or remove seats in the free trial. After the trial is converted to a paid subscription, you can add additional licenses to the subscription.

You should assign trial licenses and seats just as you would for a paid service in Partner Center.

## <a name="sign-customers-up-for-trials"></a>Sign customers up for trials

To sign your customer up for a trial through Partner Center:

1. From **Sell** on the Partner Center, go to **Catalog**. 
2. No catálogo, em **Frequência da cobrança**, clique em **Trial offer**. Isso exibe apenas as avaliações gratuitas e oculta ofertas que não são gratuitas. Avaliações aparecem na guia **Avaliações** no catálogo.
3. Selecione a avaliação gratuita que você deseja oferecer e, em seguida, selecione **enviar**. Todas as avaliações são válidas por um período de 30 dias durante o qual você não será cobrado. Você também pode convertê-la para uma assinatura paga a qualquer momento durante a avaliação.

## <a name="converting-trials-to-paid-subscriptions"></a>Converting trials to paid subscriptions

A free trial is not automatically converted to a paid subscription. After thirty days, a free trial must be converted to a paid subscription or it will [expire](#expiring-offers). Free trials can't be extended.

You'll need to convert the trial into a paid subscription yourself. You can do this [using the Partner Center](#convert-trials-using-partner-center) or [through the Partner Center APIs](#convert-trials-using-apis).

> [!NOTE]
> Customer free trials for the Cloud Solution Provider (CSP) program can't be converted to another program tenant (such as EA, Open or MOSP).

### <a name="convert-trials-using-partner-center"></a>Convert trials using Partner Center

You can convert trials to paid subscriptions using the Partner Center dashboard as follows:

1. Acesse a página de assinatura do cliente e selecione a avaliação gratuita.
2. Selecione **Converter uma assinatura de avaliação em paga**.
3. Insira a quantidade de licenças desejada e a frequência de cobrança e selecione **Aplicar**.
4. A cobrança para a assinatura paga começa na data de conversão, e a inscrição será renovada automaticamente 12 meses a partir da data de conversão. 

### <a name="convert-trials-using-apis"></a>Convert trials using APIs

You may need to alter your APIs to accommodate the conversion of a free trial to a paid subscription. For more information, see the following developer documentation:

- [Converter uma assinatura de avaliação em paga](https://docs.microsoft.com/partner-center/develop/convert-a-trial-subscription-to-paid)
- [Obter uma lista de ofertas de conversão de avaliação](https://docs.microsoft.com/partner-center/develop/get-a-list-of-trial-conversion-offers)

### <a name="expiring-offers"></a>Expiring offers

You will not be notified of expiring offers. You can track upcoming expiration dates using the customer view on Partner Center or by querying the API. É recomendável monitorar essas datas com frequência para que você possa executar as ações de acompanhamento apropriadas quando os clientes tomarem uma decisão.

After a trial has expired, a customer who attempts to log into that trial will see an expiry message. However, the data is stored in line with data retention standards. After you purchase a new subscription with the same service plans, your customer's information can be accessed again from the newly activated subscription.

## <a name="billing"></a>Cobrança

Annual billing and free trials are the same in sovereign clouds and the public cloud. The only difference is the trial SKUs available at the time of launch.

## <a name="billing-for-free-trials"></a>Billing for free trials

Free trials can be used for both monthly and annually billed subscriptions. You can select the billing frequency when you convert the trial to a paid subscription.

The subscription start date is based on the conversion date. Se a avaliação gratuita for convertida em uma oferta paga com cobrança anual, a data de renovação da assinatura será de doze meses a partir da data de conversão. Se a avaliação gratuita for convertida em uma oferta paga com cobrança mensal, a data de renovação da assinatura será 12 meses a partir da data de cobrança após a data de conversão.

### <a name="invoices"></a>Faturas

You won't see free trials listed in your invoice or license-based reconciliation file. Free trials will only appear on your invoice and license-based reconciliation file after you convert a free trial to a paid subscription. The converted subscription will appear in the same way as any new subscription.

### <a name="incentives"></a>Incentivos

Free trials do not have an impact on incentives.

## <a name="support"></a>Suporte

For support on free trials, submit a service request through Partner Center.
