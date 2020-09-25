---
title: Perguntas frequentes sobre pagamento para o Marketplace comercial da Microsoft
description: Obtenha respostas para perguntas comuns sobre pagamentos no mercado comercial.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: article
author: keferna
ms.author: keferna
ms.date: 09/11/2020
ms.openlocfilehash: eea01f5c3c7f6e249a00e8b95df93274b87fb43d
ms.sourcegitcommit: a84812b650ec8b6d0513c46c04840e4bbb0c8460
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/25/2020
ms.locfileid: "91335632"
---
# <a name="common-questions-about-commercial-marketplace-payouts"></a>Perguntas comuns sobre pagamentos do Marketplace comercial

Este artigo responde a perguntas frequentes sobre pagamentos no mercado comercial.

## <a name="earnings-incorrect-or-missing"></a>Ganhos incorretos ou ausentes

#### <a name="why-are-my-earnings-missing"></a>Por que meus ganhos estão ausentes?

- A ordem do cliente talvez ainda não esteja qualificada para pagamento. Para pedidos de clientes não empresariais, a Microsoft deve receber o pagamento do cliente antes que a conquista do editor fique qualificada. Para pedidos de clientes empresariais, seus ganhos estarão disponíveis 1-2 dias após a data do pedido de compra. Verifique o status da ordem nos [relatórios de pedidos](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order).
- Os ganhos de transações antes de julho de 2019 não podem ser mostrados no relatório de histórico de transações. Verifique as instruções históricas no [download do pagamento](https://partner.microsoft.com/dashboard/payouts/reports/incentiveexport).
- Verifique o período [do ciclo de pagamento](payment-thresholds-methods-timeframes.md) e entenda quando seus ganhos devem aparecer na instrução pagamento.

#### <a name="why-is-my-earnings-amount-different-than-what-i-expected"></a>Por que o valor dos meus ganhos é diferente do esperado?

- Se o pedido foi parcialmente pago por seu cliente, seu valor de conquista será baseado no valor parcialmente pago após a dedução da taxa e do imposto apropriado.
- Verifique a responsabilidade de remessa de imposto por país. No caso de países em que o imposto é responsável pela Microsoft, a Microsoft coleta e deduz o imposto dos ganhos do Publicador. O valor da transação mostrado na instrução é após o valor do imposto. Consulte [detalhes do imposto](tax-details-marketplace.md).
- As ofertas de SaaS e IaaS têm uma tarifa de agência com desconto em 10% em vez do padrão de 20%, deixando uma taxa de ganhos de 90%. Essa promoção entrará em vigor até 30 de junho de 2021.

**Leitura adicional**: [contrato de editor do Marketplace comercial](https://go.microsoft.com/fwlink/p/?LinkID=699560), [detalhes da política de pagamento](payout-policy-details.md), [limite de pagamento, método e intervalo de tempo](payment-thresholds-methods-timeframes.md), [sendo pago no Marketplace comercial](marketplace-get-paid.md), detalhes do [imposto](tax-details-marketplace.md), [instruções de pagamento](payout-statement.md), [painel de pedidos na análise do Marketplace comercial](/azure/marketplace/partner-center-portal/orders-dashboard)

## <a name="earnings-reconciliation"></a>Reconciliação de ganhos
### <a name="how-do-i-reconcile-payout-statements-to-order-or-usage-reports-in-analytics"></a>Como fazer reconciliar as instruções de pagamento para relatórios de pedidos ou de uso no Analytics?
Use AssetID, orderID e ID de item de linha aparecendo no relatório de histórico de transações de pagamento com ordens analíticas e relatórios de uso. Use este mapeamento:

- Histórico de transações de pagamento. AssetID = ordem. OrderID
- Histórico de transação de pagamento. OrderID & LineItem = Usage. UsageReferenceID [OrderID: LineItemID]

### <a name="how-do-i-know-when-to-expect-payments-for-my-customer-orders"></a>Como fazer saber quando esperar pagamentos para meus pedidos de clientes?
- Primeiro, usando seu AssetID, marque pedidos de clientes em [relatórios de pedidos](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order).
- Verifique o canal de cliente para sua assinatura de cliente no [relatório de clientes](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/customer).
- Para clientes corporativos, os ganhos do editor aparecem na instrução 1-2 dias após a data da ordem de compra.
- Para clientes não empresariais, os ganhos do editor aparecem na instrução 1-2 dias após o pagamento do cliente ser recebido.

**Leitura adicional**: [instruções de pagamento](payout-statement.md), [painel de pedidos na análise do Marketplace comercial](/azure/marketplace/partner-center-portal/orders-dashboard)

## <a name="payout-policies"></a>Políticas de pagamento

#### <a name="how-do-i-find-the-current-agency-fee-and-the-payout-rate"></a>Como fazer encontrar a taxa de agência atual e a taxa de pagamento?

- Verifique o contrato de editor do Marketplace comercial. A taxa de agência padrão é de 20%. As transações qualificadas de revenda de SaaS têm uma taxa com desconto de 10%. Verifique se há anúncios de tarifas da Agência promocional.
- Na sua declaração de pagamento, a taxa de conquista especifica a taxa de pagamento real para uma determinada transação.

#### <a name="when-can-i-expect-a-payment-from-microsoft-once-earnings-appear-on-my-statement"></a>Quando posso esperar um pagamento da Microsoft, uma vez que os ganhos apareçam na minha declaração?
- Quando a sua conquista estiver em status não processado, você poderá verificar a data de vencimento do mês em que seus ganhos serão processados para pagamento. Quando o pagamento for preparado, seu status de conquista será alterado para "processado".  A Microsoft lança pagamentos pelo 15º dia do mês de maturidade.
- Para pedidos pagos por cartão de crédito, a Microsoft tem pagamentos de 30 dias até que a conquista seja amadureceda.

 **Leitura adicional**: [contrato de editor do Marketplace comercial](https://go.microsoft.com/fwlink/p/?LinkID=699560), [detalhes da política de pagamento](payout-policy-details.md), detalhes do [imposto](tax-details-marketplace.md), [limite de pagamento, método e período de tempo](payment-thresholds-methods-timeframes.md)

## <a name="payments-and-adjustments"></a>Pagamentos e ajustes

#### <a name="why-is-my-payment-missing"></a>Por que meu pagamento está ausente?

- Verifique se o status do pagamento e o status do perfil de imposto são mostrados como *válidos* na [página Visão geral](https://partner.microsoft.com/dashboard/commercial-marketplace/overview).
- Talvez você não tenha atendido ao limite mínimo de um pagamento. Os ganhos devem ser pelo menos $50 USD para receber um pagamento.


#### <a name="how-do-i-set-my-account-to-not-receive-payment"></a>Como fazer definir minha conta para não receber o pagamento?
Você pode manter pagamentos no [perfil de pagamento](https://partner.microsoft.com/dashboard/commercial-marketplace/overview); Basta marcar a lista **suspensa**. A Microsoft manterá o pagamento até você até que você libere a espera.

#### <a name="why-do-i-receive-in-a-different-currency-than-the-purchase-currency"></a>Por que recebo em uma moeda diferente da moeda de compra?

A moeda de pagamento é baseada na moeda selecionada no perfil de pagamento. A moeda de compra é baseada na moeda paga pelo cliente.

#### <a name="how-do-i-reconcile-adjustments"></a>Como fazer reconciliar ajustes?

Os ajustes de pagamento são correções de pagamento para acomodar os ajustes de compensação, como problemas do sistema. Na instrução pagamento, ReasonCode especificará o motivo do ajuste. Elas não devem ser reconciliadas diretamente em transações individuais.

**Leitura adicional**: [contrato de editor do Marketplace comercial](https://go.microsoft.com/fwlink/p/?LinkID=699560), [detalhes da política de pagamento](payout-policy-details.md), detalhes do [imposto](tax-details-marketplace.md), [limite de pagamento, método e período de tempo](payment-thresholds-methods-timeframes.md)

## <a name="taxes"></a>Impostos

#### <a name="how-do-we-identify-tax-remit-responsibility-between-microsoft-or-publisher-in-the-payout-statement"></a>Como identificamos a responsabilidade de remessa de impostos entre a Microsoft ou o Publisher na declaração de pagamento?

Em download do histórico de transações, localize a coluna de modelo de imposto. Isso mostra MS Managed ou ISV Managed. Consulte regras de impostos específicas do país e implicações de pagamento em [detalhes do imposto](tax-details-marketplace.md).

#### <a name="how-do-i-download-service-fee-tax-forms"></a>Como fazer baixar os formulários de imposto sobre tarifas de serviço?

Vá para a página **pagamento** do pagamento e, em seguida, a seção **lista de pagamentos** . Um link para o formulário de imposto sobre tarifa de serviço é exibido para um pagamento que tem o imposto sobre tarifa de serviço.

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>Como fazer baixar um formulário de imposto sobre retenção em PDF?

Vá para a página *pagamento* do pagamento e, em seguida, a seção **lista de pagamentos** . Um link para um formulário de imposto retido na fonte é exibido ao lado de um pagamento.

#### <a name="where-do-i-find-year-end-tax-forms"></a>Onde encontro os formulários de imposto de fim de ano?

Acesse a [página de perfil](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage) para exibir seus formulários de imposto de fim de ano.

#### <a name="how-do-i-find-withholding-tax-for-a-transaction"></a>Como fazer localizar a retenção de imposto de uma transação?
A retenção de imposto é aplicável a editores norte-americanos que arquivaram um formulário W-9. A retenção de imposto é calculada em um pagamento mensal.

**Leitura adicional**: [contrato de editor do Marketplace comercial](https://go.microsoft.com/fwlink/p/?LinkID=699560), [detalhes da política de pagamento](payout-policy-details.md)

## <a name="payout-statement-access"></a>Acesso à instrução de pagamento

#### <a name="how-do-i-access-a-payout-statement"></a>Como fazer acessar uma instrução de pagamento?

1. Verifique suas funções. Você deve ter a função *colaborador financeiro* ou *proprietário da conta* para acessar a instrução pagamento.
2. Na barra de navegação superior direita, selecione o ícone de **pagamento** para exibir sua instrução de pagamento. Escolha entre o **histórico de transações**, o **pagamento**e o **Download**.

**Leitura adicional**: [funções de pagamento e permissões](payout-statement.md#roles-and-permissions), [instruções de pagamento](payout-statement.md) 

## <a name="payout-statement-report"></a>Relatório de demonstrativo de pagamento

#### <a name="what-does-each-field-in-the-transaction-download-mean"></a>O que significa cada campo no download da transação?

Consulte as [instruções de pagamento](payout-statement.md) para obter uma lista detalhada dos atributos e seus significados.

#### <a name="what-is-earning-status"></a>O que é o status de conquista?

Isso mostra seus ganhos como não processados, processados ou enviados.

- Não **processado** – os ganhos estão em um período de caução até a data de vencimento.
- **Processado** – os ganhos foram amadurecedos e estão preparados para um pagamento mensal. Os pagamentos são lançados por 15 a cada mês.
- **Enviado** – o pagamento foi liberado com êxito para seu banco com base em seu perfil de pagamento.

#### <a name="how-do-i-download-service-fee-tax-forms"></a>Como fazer baixar os formulários de imposto sobre tarifas de serviço?

Vá para a página **pagamento** do pagamento e, em seguida, a seção **lista de pagamentos** . Um link para o formulário de imposto sobre tarifa de serviço é exibido para um pagamento que tem o imposto sobre tarifa de serviço.

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>Como fazer baixar um formulário de imposto sobre retenção em PDF?

Vá para a página **pagamento** do pagamento e, em seguida, a seção **lista de pagamentos** . Um link para um formulário de imposto retido na fonte é exibido ao lado de um pagamento.

#### <a name="where-do-i-find-year-end-tax-forms"></a>Onde encontro os formulários de imposto de fim de ano?

Acesse a [página de perfil](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage) para exibir seus formulários de imposto de fim de ano.

**Leitura adicional**: [instruções de pagamento](payout-statement.md), [download de histórico de transações](payout-statement.md#transaction-history-download)

## <a name="historical-statements"></a>Demonstrativo do histórico

#### <a name="how-do-i-view-historical-information"></a>Como fazer exibir informações históricas?

A instrução histórica mostrará o instantâneo dos dados de pagamento a partir de outubro de 2019. Infelizmente, as informações de pagamento aqui não são atualizadas. Para receber as informações mais recentes, envie um tíquete de suporte para os dados mais recentes.

**Leitura adicional**: [instruções de pagamento](payout-statement.md), [download de histórico de transações](payout-statement.md#transaction-history-download)

## <a name="payout-export-api"></a>API de exportação de pagamento

#### <a name="how-do-i-download-payout-data"></a>Como fazer baixar dados de pagamento?

Use a [API de pagamento do parceiro](https://apidocs.microsoft.com/services/partnerpayouts).

## <a name="next-steps"></a>Próximas etapas

- [Ser pago no marketplace comercial](marketplace-get-paid.md)
