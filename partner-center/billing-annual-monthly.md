---
title: Monthly and annual billing differences | Partner Center
ms.topic: article
ms.date: 11/21/2019
Description: Differences between monthly and annual billing cycles in Partner Center.
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
ms.localizationpriority: medium
ms.openlocfilehash: 4d6b316f55a6d2cd84959d60feed666d657893b8
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389764"
---
# <a name="monthly-and-annual-billing-differences"></a>Monthly and annual billing differences

Aplica-se a:

- Partner Center
- Partner Center do Microsoft Cloud for US Government

This topic explains the differences between **monthly billing** and **annual billing** in Partner Center, including benefits and use cases. You have the option to pay for certain Cloud Solution Provider (CSP) subscriptions on a monthly or annual basis.

## <a name="applicability"></a>Aplicabilidade

Most licensed-based subscriptions have the option for either monthly or annual billing option. As assinaturas baseadas em uso só apresentam a opção de cobrança mensal.

Both annual and monthly billing are **per subscription**, ***not* per license**.

### <a name="find-subscription-applicability"></a>Find subscription applicability

You can identify the available billing frequencies for each offer by using column J in the offer matrix. You can find the offer matrix in the **See offers and pricing** section on Partner Center.

### <a name="applicable-partners"></a>Applicable partners

All partners and partner types can choose monthly or annual billing.

### <a name="applicable-markets"></a>Applicable markets

Monthly and annual billing (for applicable offers) are available in all markets where the CSP program is currently available.

## <a name="change-billing-frequency"></a>Change billing frequency

You can switch between monthly and annual billing at any time. You may want to change your billing frequency if your business needs change.

When you change the billing frequency to annual, the annual term is updated to reflect the date you changed the billing frequency. A new renewal date is also established.

### <a name="monthly-to-annual-billing"></a>Monthly to annual billing

Switching from monthly billing to annual billing may be useful if you have numerous subscriptions that are billed monthly. When you switch to annual billing, you can align the subscriptions to a common billing date.

### <a name="annual-to-monthly-billing"></a>Annual to monthly billing

Switching from annual billing to monthly billing may be useful if you want to adjust your billing dates to those of your individual customers.

## <a name="annual-billing"></a>Annual billing

A cobrança anual tem os seguintes benefícios:

- Maior flexibilidade nas opções de pagamento.
- Melhor alinhamento com o faturamento dos seus clientes.
- Impacto reduzido nas flutuações de moeda.
- Custos operacionais de cobrança reduzidos.

### <a name="configure-annual-billing"></a>Configure annual billing

If you're planning to switch to annual billing in Partner Center, be sure to consider how your sales motion will be affected. You should inform your team and update your internal processes as necessary. You should also review changes to your invoice and license-based reconciliation file. 

You will also need to [update your APIs for annual billing](#required-api-changes).

#### <a name="required-api-changes"></a>Required API changes

Para aproveitar a cobrança anual, algumas mudanças são necessárias para suas APIs.

- [Order.BillingCycle property](https://docs.microsoft.com/dotnet/api/microsoft.store.partnercenter.models.orders.order.billingcycle)
- [Create an order](https://docs.microsoft.com/partner-center/develop/create-an-order)

For more information about Partner Center APIs, see all [Partner Center developer resources and documentation](https://docs.microsoft.com/partner-center/develop/).

## <a name="placing-orders"></a>Placing orders

The billing frequency type, including the annual billing option, is assigned to the **Offer** as an attribute. There is not a unique offer specifically for orders with annual billing. Entretanto, você pode renomear uma oferta usando um nome de cliente mais amigável para permitir a diferenciação.

### <a name="select-annual-billing"></a>Select annual billing

When you add a new subscription, you will be prompted to choose the billing frequency. Você pode escolher a opção de cobrança anual nesse ponto. When you select annual billing,all available offers will be displayed.

### <a name="billing-time"></a>Billing time

Você será cobrado na próxima data de cobrança. For example, if your billing date is the 1st of the month and you purchase an annually billed subscription on October 29, 2019, you will be billed on November 1, 2019. Assuming that you make no license changes, you will be billed again on November 1, 2020. If you make a license change you will receive a credit and rebill on your next billing date.

### <a name="annual-renewals"></a>Annual renewals

Your subscription renewal date will be twelve months after the service start date. O período de serviço começa na data em que a assinatura é criada.  For example, a subscription created on January 10, 2019, will be renewed on January 10, 2020.

Você será cobrado na próxima data de cobrança após a data de renovação da assinatura. Por exemplo, se você comprar uma assinatura com cobrança anual em 15 de janeiro de 2018 e se a sua data de cobrança for 20 de janeiro, sua assinatura será renovada em 15 de janeiro de 2019. Você será cobrado pela renovação em 20 de janeiro de 2019.

### <a name="split-subscription-billing-frequency"></a>Split subscription billing frequency

It isn't possible to split a **single subscription** so that one part is billed monthly and the other part is billed annually. The entire subscription must have the same billing frequency (either monthly or annual billing).

For customers with **multiple subscriptions** of the same offer, it may be possible to have different billing frequencies per subscription. Há algumas ofertas restritas a uma assinatura por cliente. Se a oferta não estiver restrita, o cliente poderá ter várias assinaturas da mesma oferta com diferentes frequências de cobrança. Você pode encontrar os detalhes de todos os limites e restrições de oferta na coluna I da matriz de ofertas. You can find the offer matrix in the **See offers and pricing** section on Partner Center.

### <a name="free-subscription-period"></a>Free subscription period

Subscriptions with annual billing frequency do not receive a free period. The twelve-month paid term begins on the purchase date. Isso é diferente de assinaturas com frequência de cobrança mensal que recebem um período gratuito entre a data da compra e a próxima data de cobrança.

### <a name="adding-and-removing-licenses"></a>Adding and removing licenses

Você pode alterar a quantidade de licenças das suas assinaturas a qualquer momento. A adição de outras licenças não afetará a frequência de cobrança.

Você pode adicionar ou remover licenças a qualquer momento.  You will receive a credit and prorated rebill on your next billing date after you change the number of licenses.

If your existing subscription has annual billing, it's not possible to add licenses with monthly billing to that subscription. Assim que você comprar uma assinatura com cobrança anual, todas as licenças adicionais seguirão a mesma frequência de cobrança. Se então você precisar comprar licenças com cobrança mensal, precisará comprar uma nova assinatura.

### <a name="add-on-offers"></a>Add-on offers

A assinatura complementar terá automaticamente a mesma frequência de cobrança da assinatura principal. Annual billing is available for add-on offers. 

### <a name="cancelling-subscriptions"></a>Cancelling subscriptions

A política de cancelamento é a mesma para todas as frequências de cobrança.

For annual billing, if the subscription is cancelled in the first 30 days of the twelve-month paid term you will receive a 100 percent credit on your next billing date. If the subscription is cancelled after 30 days of the twelve-month paid term you will receive a prorated credit on your next billing date.

### <a name="moving-subscriptions-between-partners"></a>Moving subscriptions between partners

Customers can't move subscriptions between from one partner to another. Isso se aplica a assinaturas cobradas mensal e anualmente.

O novo parceiro deve comprar uma nova assinatura em nome do cliente. It's not possible to move subscriptions between partners.

### <a name="reactivating-subscriptions"></a>Reactivating subscriptions

You can reactivate a subscription for up to 90 days after the suspension date. Você receberá uma cobrança proporcional na data de cobrança seguinte. A data de renovação da assinatura permanece a mesma.

## <a name="pricing"></a>Preço

### <a name="offer-pricing"></a>Offer pricing

The offer price at time of purchase is guaranteed for the full billed subscription term (one month for monthly billing, twelve months for annual billing). Quando uma assinatura for renovada, o preço se baseará na lista de preços atual na data de renovação. The new price is guaranteed for the next subscription term.

If an offer price decreases during the billing period, the amount you are billed for doesn't change. The price is set for the full billing period at the time of purchase. This applies to both monthly and annual billing.

### <a name="cancellation-credits"></a>Cancellation credits

Credit for a cancelled license or subscription is calculated as follows:

**Cancellation credit** = ((**monthly price***12)/365) \* **days remaining in the twelve-month term** \* number of licenses cancelled.

## <a name="reconciliation-file"></a>Reconciliation file

### <a name="find-subscriptions-billing-frequency"></a>Find subscription's billing frequency

Review your license-based reconciliation file for information on whether your subscription is billed monthly or annually. This information is in column **AA**.

To find out whether you can change a monthly subscription to annual billing, see [Find subscription applicability](#find-subscription-applicability).

### <a name="reconciliation-file-changes-for-annual-billing"></a>Reconciliation file changes for annual billing

When you purchase or renew a subscription with annual billing, your license-based reconciliation file will change as follows.

A new row on the license-based reconciliation file on the first billing date following the purchase or a new subscription.

Se nenhuma alteração for feita na assinatura, não haverá linhas nos arquivos de reconciliação para o segundo mês até o décimo-segundo do período da assinatura. If a change is made to the subscription during the twelve-month term, a credit and prorated rebill will appear on the next reconciliation file after the change is made.

The next change to the reconciliation file will appear when the subscription is renewed. Isso será exibido na data da primeira cobrança após a renovação.

### <a name="usage-file-changes-for-annual-billing"></a>Usage file changes for annual billing

The following annually billed subscription changes appear in column P of your usage file.

- **Prorate Fees When Purchase**: the initial purchase of an annual subscription.
- **Cycle Instance Prorate**: license changes that result in credit and rebilling.
- **Cancel Fee**: the [cancellation of an annual subscription](#cancellation-of-annual-subscription).

### <a name="cancellation-of-annual-subscription"></a>Cancellation of annual subscription

When an annually billed subscription is cancelled, the reconciliation file will contain one line item for a cancellation credit.

If the cancellation occurs in the first 30 days of the twelve-month term, the subscription will be credited at 100 percent. Se o cancelamento ocorrer após os 30 primeiros dias, a assinatura será creditada de forma proporcional.

### <a name="adding-licenses-to-annual-subscription"></a>Adding licenses to annual subscription

When you add licenses to a subscription, the reconciliation file will contain a credit and prorated rebill. This applies to monthly and annually billed subscriptions.

### <a name="price-lists-for-annual-billing"></a>Price lists for annual billing

Partner Center price lists show the monthly prices. There is no annual price listed. Você pode calcular o preço anual multiplicando o preço mensal por doze.

### <a name="offer-matrix"></a>Offer matrix

Offer IDs in the offer matrix are the same for all billing frequencies. There are no unique IDs for offers that can be billed annually.

## <a name="incentives"></a>Incentivos

### <a name="incentives-calculation"></a>Incentives calculation

Incentives are calculated based on **billed revenue**, ***not* adjusted revenue**. Os pagamentos de incentivos ganhos serão efetuados de acordo com nossa política encontrada em nossos guias de incentivos do CSP.

When an annually billed subscription is sold, that subscription's revenue is recognized for the calculation of incentives based on billed revenue.

### <a name="payout"></a>Pagamento

Currently, all incentive payments are made twice a year. Esses pagamentos são feitos 45 dias após o fim do semestre.

### <a name="rates"></a>Taxas

Partners earn incentives on all eligible transactions, regardless of how a subscription is billed. Incentive earnings are calculated based on the global incentive rate (which is applied to the billed revenue for the period), the local accelerator (for all geographies in which there are local accelerators), and any global campaigns (where applicable).

### <a name="contacts"></a>Contatos

For questions about incentives, contact the appropriate regional incentives support team:

| Region | Endereço de email |
| ------ | ------------- |
| América do Norte | <ocina@microsoft.com> |
|Latin America & Brazil | <ocilatam@microsoft.com> |
| EMEA | <ociemea@microsoft.com> |
| APOAC (excluding Japan) | <ociapgc@microsoft.com> |
| Japão | <ocijp@microsoft.com> |


### <a name="suspension"></a>Suspension

If you suspend an subscription (in Partner Center or through the APIs) within 30 days of purchase, you will receive a 100% credit, regardless of billing frequency.

For annual billing:

1. The partner buys the subscription on January 1st. A charge billing line is created for the service period January 1st to December 31st.
2. The partner suspends the subscription on January 25th. A credit billing line is created for the service period January 1st to December 31st.
3. The reactivates the subscription on January 29th. A charge billing line is created for the service period January 29th to December 31st.

For monthly billing:

1. The partner buys the subscription on January 1st. A charge billing line is created for the service period January 1st to January 31st.
2. The partner suspends the subscription on January 25th. A credit billing line is created for the service period January 1st to January 31st.
3. The partner reactivates the subscription on January 29th. A charge billing line is created for the service period January 29th to January 31st.
