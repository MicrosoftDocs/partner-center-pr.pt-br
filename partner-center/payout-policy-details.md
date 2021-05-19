---
title: Agendas e processos de pagamento
description: Saiba mais sobre pagamentos e transações, como agendamentos de pagamento e processos de recoupmentação para o marketplace comercial e outras transações.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
author: eunjkim520
ms.author: eunjkim
ms.date: 12/04/2020
ms.openlocfilehash: f2ba8132677eb0a0368021b6d7065f5202589f24
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146945"
---
# <a name="payout-schedules-and-processes"></a>Agendas e processos de pagamento

**Funções apropriadas:** conta de administrador | Administrador global

Este artigo aborda a agenda de pagamento da Microsoft, onde encontrar o status de um pagamento e o processo de não pagamento do cliente.

## <a name="payment-schedules"></a>Agendamentos de pagamento

As seções a seguir descrevem nosso processo de pagamento para **Enterprise Agreement** e **transações de cartão de crédito/fatura.**

### <a name="enterprise-agreement-transactions"></a>Enterprise Agreement transações

Quando um cliente comprar um produto do Microsoft AppSource ou Azure Marketplace usando o Microsoft Enterprise Agreement existente para transações, emitiremos pagamentos no próximo ciclo de pagamento 30 dias após a fatura do cliente. As transações em que um cliente usa um cartão de crédito têm um período de 30 dias antes do pagamento.

Um pagamento geralmente ocorrerá antes que a Microsoft colete o pagamento do cliente. Confira [Processar o não pagamento do](#process-for-customer-non-payment) cliente abaixo para as ações que tomaremos se o cliente não pagar a Microsoft, mas já emitirmos um pagamento.

| Evento | Descrição | Visibilidade do relatório | Tempo* |
| --- | --- | --- | --- |
| Uso ou mês da transação | O cliente usa ou compra um serviço. | [Painel uso](/azure/marketplace/partner-center-portal/usage-dashboard) [ou](/azure/marketplace/partner-center-portal/orders-dashboard) pedido | **Mês 1** |
| A Microsoft calcula o valor da cobrança | Determinar o uso total, total de transações | [Painel uso](/azure/marketplace/partner-center-portal/usage-dashboard) [ou](/azure/marketplace/partner-center-portal/orders-dashboard) pedido | **2º mês** |
| Pagamento postado | Determinar a taxa da Agência e os ganhos de pagamento | Marcado como não processado no histórico de transações na [instrução de pagamento](payout-statement.md) | **Mês 3 (1ª semana)** |
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
| Uso ou mês da transação | O cliente usa ou compra um serviço. | [Painel uso](/azure/marketplace/partner-center-portal/usage-dashboard) [ou](/azure/marketplace/partner-center-portal/orders-dashboard) pedido | **Mês 1** |
| Fatura paga pelo cliente | Determinar o uso total, o valor total da transação e a fatura paga pelo cliente | [Painel uso](/azure/marketplace/partner-center-portal/usage-dashboard) [ou](/azure/marketplace/partner-center-portal/orders-dashboard) pedido | **2º mês** |
| Pagamento postado | Determinar os ganhos de tarifa de agência e pagamento | Marcado como Não Processado no Histórico de Transações na [instrução de pagamento](payout-statement.md) | **2º mês** |
| Período de espera de 30 dias | Garantir a coleta de fundos, possíveis esbarrões e solicitações de reembolso | Marcado como Não Processado no Histórico de Transações na [instrução de pagamento](payout-statement.md) | **Mês 3** |
| Preparar o pagamento | Os ganhos são preparados para pagamento mensal | Marcado como Futuro no Histórico de Transações na [instrução de pagamento](payout-statement.md) | **Mês 4 (1ª semana)** |
| **Pagamento enviado** | **O pagamento é enviado ao Publicador** | **Marcado como enviado no histórico de transações e na seção de pagamentos da [instrução de pagamento](payout-statement.md)** | **Mês 4 (não depois do 15º)** |
|

\* A data de pagamento está no horário padrão do Pacífico (PST).

:::image type="content" source="images/payouts/timeline-credit-card-invoice.png" alt-text="Linha do tempo de pagamentos para clientes de cartão de crédito e fatura.":::

## <a name="process-for-customer-non-payment"></a>Processo de não pagamento de cliente

Em raras ocasiões, a Microsoft não consegue coletar pagamentos de clientes para suas compras do Marketplace comercial. Quando um cliente não paga a Microsoft de acordo com seu agendamento de cobrança, começamos o processo de coleções. Esse processo leva aproximadamente quatro meses e envolve a comunicação persistente da Microsoft. Se o pagamento não for recebido pelo final deste processo, a Microsoft gravará os fundos como não coletáveis.

De acordo com o processo de pagamento articulado aqui, a Microsoft pode já ter pago os fundos para os editores (você) que, por fim, não podem ser coletados. Portanto, temos um processo para reconciliar esses valores. Para garantir que você tenha um aviso de que o pagamento (já recebido) pode ser reconciliado, você será notificado quando um cliente estiver no processo de cobranças e as compras provavelmente serão gravadas.

A Microsoft recuperará todos os pagamentos já pagos usando um dos seguintes métodos: (1) a Microsoft poderá subtrair os valores não pagos de pagamentos futuros; por exemplo, se $1000 em pagamentos forem considerados não colecionáveis e gravados, seus pagamentos futuros serão retidos até que a $1000 seja recuperada ou (2) a Microsoft poderá solicitar um reembolso ou Publicadores de notas fiscais por quaisquer valores não coletados.

O agendamento a seguir é um exemplo:

| Evento | Data aproximada * | Visibilidade do parceiro |
| --- | --- | --- |
| Data de pagamento de exemplo | 10/15/2020 | Marcado como **Enviado no** Histórico de Transações e na seção Pagamentos no Painel de Pagamento |
| <font color="red">Se o cliente não pagar à Microsoft</font> | 12/2/2020 – 12/5/2020 | Nenhuma alteração, a mesma que acima |
| O cliente recebe o primeiro email de pagamento atrasado | 12/6/2020 | Nenhum |
| O cliente recebe emails regulares de crescente urgência | 12/7/2020 – 1/31/2021 | Nenhum |
| É provável que o editor seja notificado sobre a ressarção | 1/7/2021 | Notificação por email enviada ao editor de que seu cliente ainda não enviou o pagamento. ID da transação e valor em dólar estão incluídos. |
| O cliente recebe um aviso de encerramento | 2/1/2021 | Nenhum |
| O processo de coleta termina/os fundos são gravados | 2/15/2021 | Notificação por email enviada ao editor de que os fundos foram gravados. ID da transação e valor em dólar estão incluídos. |
| O pagamento é deduzido | 01/03/2021 | O publicador verá uma transação negativa Partner Center instrução de pagamento |
| Pagamento retido | 3/15/2021 | Pagamentos futuros serão mostrados na instrução pagamento do centro de parceiros. O Publicador não receberá o pagamento até que o saldo não seja mais negativo.  |
|||

\* A data de pagamento está no horário padrão do Pacífico (PST).

## <a name="number-of-days-for-payments-to-reach-a-payout-account"></a>Número de dias para os pagamentos chegarem a uma conta de pagamento

Normalmente, enviamos qualquer pagamento devido em um determinado mês no 15º dia desse mês, mas leva outro tempo para que o pagamento chegue à sua conta. O número de dias depende do método de pagamento que usamos para sua conta, conforme descrito abaixo.

> [!NOTE]
> Os dias mostrados abaixo são aproximados; qualquer pagamento pode levar mais ou menos tempo para alcançar sua conta.

| Método de pagamento     | Número de dias até chegar à conta de pagamento     |
|--------------------|--------------------------------------------|
| PayPal             | 1 dia útil                             |
| ACH/SEPA           | 2 a 3 dias úteis                          |
| Transferência eletrônica      | 7 a 10 dias úteis                         |
|

## <a name="next-steps"></a>Próximas etapas

- [Detalhes do imposto](tax-details-marketplace.md)
