---
title: Agendas de pagamento e detalhes de política-Azure Marketplace
description: Saiba mais sobre os detalhes relacionados às políticas de pagamento do Marketplace comercial, incluindo agendas e revitória.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
author: eunjkim520
ms.author: eunjkim
ms.date: 11/06/2020
ms.openlocfilehash: bd8153ffd368c1f67b27eaeb44d383409bd59e97
ms.sourcegitcommit: 2e880efb02a48afc4f234ec27da34519407f87c6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/02/2020
ms.locfileid: "96513272"
---
# <a name="payout-schedules-and-policy-details"></a>Agendas de pagamento e detalhes da política

Este artigo discute o processo de pagamento da Microsoft, o agendamento de pagamento, onde encontrar o status de um pagamento e o processo de não pagamento do cliente.

## <a name="payment-schedules"></a>Agendamentos de pagamento

As seções a seguir descrevem nosso processo de pagamento para transações de **Enterprise Agreement** e de **cartão de crédito/fatura** .

### <a name="enterprise-agreement-transactions"></a>Transações de Enterprise Agreement

Quando um cliente adquire um produto do Microsoft AppSource ou do Azure Marketplace usando seus Enterprise Agreement da Microsoft existentes para transações, emitiremos pagamentos no próximo ciclo de pagamento de 30 dias após a fatura do cliente. As transações em que um cliente usa um cartão de crédito têm um período de manutenção de 30 dias antes do pagamento.

Muitas vezes, um pagamento ocorrerá antes que A Microsoft colete o pagamento do cliente. Consulte [processar para não pagamento de cliente](#process-for-customer-non-payment) abaixo para as ações que adotamos se o cliente não conseguir pagar a Microsoft, mas já tiver emitido um pagamento.

| Evento | Descrição | Visibilidade de relatórios | Periodic |
| --- | --- | --- | --- |
| Uso ou mês de transação | O cliente usa ou compra um serviço. | Painel de [uso](/azure/marketplace/partner-center-portal/usage-dashboard) ou [ordem](/azure/marketplace/partner-center-portal/orders-dashboard) | **Mês 1** |
| A Microsoft calcula o valor da cobrança | Determinar o uso total, total de transações | Painel de [uso](/azure/marketplace/partner-center-portal/usage-dashboard) ou [ordem](/azure/marketplace/partner-center-portal/orders-dashboard) | **Mês 2** |
| Pagamento Postado | Determinar a taxa da Agência e os ganhos de pagamento | Marcado como não processado no histórico de transações na [instrução de pagamento](payout-statement.md) | **Mês 3 (1ª semana)** |
| Preparar pagamento | Os ganhos são preparados para pagamento mensal | Marcado como futuro no histórico de transações na [instrução de pagamento](payout-statement.md) | **Mês 3 (1ª semana)** |
| **Pagamento enviado** | **O pagamento é enviado ao Publicador** | **Marcado como enviado no histórico de transações e na seção de pagamentos da [instrução de pagamento](payout-statement.md)** | **Mês 3 (não depois do 15º)** |
| Fatura paga pelo cliente | A Microsoft coleta o pagamento do cliente | Nenhuma alteração | **Mês 4 a 12** |
|

\* A data de pagamento está no horário padrão do Pacífico (PST).

:::image type="content" source="images/payouts/timeline-enterprise.png" alt-text="Linha do tempo de pagamentos para clientes do Enterprise Agreement.":::

### <a name="transactions-with-credit-card-or-invoice-checkwire"></a>Transações com cartão de crédito ou fatura (cheque/fio)

Todas as compras com um cartão de crédito ou uma nota fiscal mensal têm um período de manutenção de 30 dias para garantir que os fundos sejam coletados do cliente.

| Evento | Descrição | Visibilidade de relatórios | Periodic |
| --- | --- | --- | --- |
| Uso ou mês de transação | O cliente usa ou compra um serviço. | Painel de [uso](/azure/marketplace/partner-center-portal/usage-dashboard) ou [ordem](/azure/marketplace/partner-center-portal/orders-dashboard) | **Mês 1** |
| Fatura paga pelo cliente | Determinar o uso total, o valor total da transação e o cliente paga fatura | Painel de [uso](/azure/marketplace/partner-center-portal/usage-dashboard) ou [ordem](/azure/marketplace/partner-center-portal/orders-dashboard) | **Mês 2** |
| Pagamento Postado | Determinar a taxa da Agência e os ganhos de pagamento | Marcado como não processado no histórico de transações na [instrução de pagamento](payout-statement.md) | **Mês 2** |
| período de manutenção de 30 dias | Garanta a coleta de fundos, possíveis chargeback e solicitações de reembolso | Marcado como não processado no histórico de transações na [instrução de pagamento](payout-statement.md) | **Mês 3** |
| Preparar pagamento | Os ganhos são preparados para pagamento mensal | Marcado como futuro no histórico de transações na [instrução de pagamento](payout-statement.md) | **Mês 4 (1ª semana)** |
| **Pagamento enviado** | **O pagamento é enviado ao Publicador** | **Marcado como enviado no histórico de transações e na seção de pagamentos da [instrução de pagamento](payout-statement.md)** | **Mês 4 (não depois do 15º)** |
|

\* A data de pagamento está no horário padrão do Pacífico (PST).

:::image type="content" source="images/payouts/timeline-credit-card-invoice.png" alt-text="Linha do tempo de pagamentos para clientes de cartão de crédito e fatura.":::

## <a name="process-for-customer-non-payment"></a>Processo de não pagamento de cliente

Em raras ocasiões, a Microsoft não consegue coletar pagamentos de clientes para suas compras do Marketplace comercial. Quando um cliente não paga a Microsoft de acordo com seu agendamento de cobrança, começamos o processo de coleções. Esse processo leva aproximadamente quatro meses e envolve a comunicação persistente da Microsoft. Se o pagamento não for recebido no final deste processo, a Microsoft gravará os fundos como não coletáveis.

De acordo com o processo de pagamento articulado aqui, a Microsoft pode já ter pago os fundos para os editores (você) que, por fim, não podem ser coletados. Portanto, temos um processo para reconciliar esses valores. Para garantir que você tenha um aviso de que o pagamento (já recebido) pode ser reconciliado, você será notificado quando um cliente estiver no processo de cobranças e as compras provavelmente serão gravadas.

A Microsoft recuperará todos os pagamentos já pagos usando um dos seguintes métodos: (1) a Microsoft poderá subtrair os valores não pagos de pagamentos futuros; por exemplo, se $1000 em pagamentos forem considerados não colecionáveis e gravados, seus pagamentos futuros serão retidos até que a $1000 seja recuperada ou (2) a Microsoft poderá solicitar um reembolso ou Publicadores de notas fiscais por quaisquer valores não coletados.

Veja a seguir um exemplo de agendamento:

| Evento | Data aproximada * | Visibilidade do parceiro |
| --- | --- | --- |
| Data de pagamento de exemplo | 10/15/2020 | Marcado como **enviado** no histórico de transações e na seção de pagamentos no painel de pagamento |
| <font color="red">Se o cliente não pagar a Microsoft</font> | 12/2/2020 – 12/5/2020 | Nenhuma alteração, igual à acima |
| O cliente recebe o primeiro email de pagamento atrasado | 12/6/2020 | Nenhum |
| O cliente recebe emails regulares de maior urgência | 12/7/2020 – 1/31/2021 | Nenhum |
| A gravação notificada do Publicador é provavelmente | 1/7/2021 | Notificação por email enviada ao Publicador de que seu cliente ainda não enviou o pagamento. A ID da transação e o valor de dólar estão incluídos. |
| O cliente recebe aviso de encerramento | 2/1/2021 | Nenhum |
| O processo de coleta termina/fundos são gravados | 2/15/2021 | Notificação por email enviada ao Publicador de que os fundos foram gravados. A ID da transação e o valor de dólar estão incluídos. |
| Pagamento deduzido | 01/03/2021 | O Publicador verá uma transação negativa na instrução pagamento do Partner Center |
| Pagamento retido | 3/15/2021 | Pagamentos futuros serão mostrados na instrução pagamento do centro de parceiros. O Publicador não receberá o pagamento até que o saldo não seja mais negativo.  |
|||

\* A data de pagamento está no horário padrão do Pacífico (PST).

## <a name="number-of-days-for-payments-to-reach-a-payout-account"></a>Número de dias para os pagamentos chegarem a uma conta de pagamento

Normalmente, enviamos qualquer pagamento devido em um determinado mês no 15º dia desse mês, mas leva mais tempo para que o pagamento chegue à sua conta. O número de dias depende do método de pagamento que usamos para sua conta, conforme descrito abaixo.

> [!NOTE]
> Os dias mostrados abaixo são aproximados; qualquer pagamento pode levar um tempo maior ou menor para alcançar sua conta.

| Método de pagamento     | Número de dias até chegar à conta de pagamento     |
|--------------------|--------------------------------------------|
| PayPal             | 1 dia útil                             |
| ACH/SEPA           | 2 a 3 dias úteis                          |
| Transferência eletrônica      | 7 a 10 dias úteis                         |
|

## <a name="next-steps"></a>Próximas etapas

- [Detalhes do imposto](tax-details-marketplace.md)
