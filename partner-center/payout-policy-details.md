---
title: Detalhes da política de pagamento-Microsoft Commercial Marketplace
description: Detalhes sobre as políticas de pagamento do Marketplace comercial, incluindo agendas e revitória.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
author: mingshen-ms
ms.author: mingshen
ms.date: 04/24/2020
ms.openlocfilehash: 17fedcf4ef3d474eab679a03eecb221c90342a04
ms.sourcegitcommit: a84812b650ec8b6d0513c46c04840e4bbb0c8460
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/25/2020
ms.locfileid: "91335633"
---
# <a name="payout-policy-details"></a>Detalhes da política de pagamento

Este artigo discute o processo de pagamento da Microsoft, a agenda de pagamento e a política de revitória e onde encontrar o status de um pagamento.

## <a name="where-to-find-upcoming-payouts"></a>Onde encontrar pagamentos futuros

No Partner Center, selecione o ícone de **pagamento** no canto superior direito da tela:

:::image type="content" source="images/payouts/payout-overview.png" alt-text="Ilustra o ícone de pagamento no canto superior direito do portal do Partner Center.":::

> [!TIP]
> Nem todas as funções de conta têm acesso às informações de pagamento. Para obter detalhes, consulte [funções e permissões](payout-statement.md#roles-and-permissions).

## <a name="payment-schedules"></a>Agendamentos de pagamento

As seções a seguir descrevem nosso processo de pagamentos.

### <a name="enterprise-agreement-transactions-after-may-1-2020"></a>Enterprise Agreement transações após 1º de maio de 2020

Fizemos a seguinte atualização para nosso modelo de pagamento de editor do Marketplace comercial:

A partir de 1º de maio de 2020, estamos atualizando nossa política de pagamento relacionada aos produtos adquiridos no Microsoft AppSource ou no Azure Marketplace por clientes com um Enterprise Agreement da Microsoft. Quando um cliente adquire um produto do Azure Marketplace ou AppSource usando seus Enterprise Agreement da Microsoft existentes para transações, após 1º de maio de 2020, começaremos a emitir pagamentos no próximo ciclo de pagamento em 30 dias após a fatura do cliente. As transações em que um cliente usa um cartão de crédito não são alteradas e continuarão a ter um período de manutenção de 30 dias antes do pagamento. Esta tabela mostra detalhes sobre o agendamento de pagamento.

> [!NOTE]
> Consulte [processar para não pagamento de cliente](#process-for-customer-non-payment) abaixo para as ações que executamos se o cliente não conseguir pagar, mas já tiver emitido um pagamento para você.

| Evento  | Data (UTC) | Visibilidade do parceiro: relatório de pagamento do Partner Center  |  Visibilidade do parceiro: análise do Partner Center\* |
| --- | --- | --- | --- |
| Transação ou mês de uso | 8/1/2020 – 8/31/2020 | N/D | **Relatório de uso**: novo consumo mostrado (atualizado a cada quatro horas)<br>**Relatório do pedido**: N/A |
| Final do termo (mês) | 31/8/2020 | N/D | **Relatório de uso**: consumo final do mês mostrado<br>**Relatório do pedido**: N/A |
| Ordem gerada | 9/3/2020 – 9/7/2020 | N/D | **Relatório de uso**: consumo mostrado com OrderID/OrderLineItemID<br>**Relatório de pedidos**: pedidos de clientes mostrados como ativos |
| Calcular pagamento ganhando | 9/4/2020 – 9/10/2020 | Marcado como não **processado** no histórico de transações no painel do pagamento | **Relatório de uso**: consumo mostrado com OrderID/OrderLineItemID<br>**Relatório de pedidos**: pedidos de clientes mostrados como ativos |
| Pagamento mensal | 10/5/2020 | Marcado como **futuro** no histórico de transações no painel de pagamento | **Relatório de uso**: consumo mostrado com OrderID/OrderLineItemID<br>**Relatório de pedidos**: pedidos de clientes mostrados como ativos |
| Data do pagamento\** | 10/15/2020 | Marcado como **enviado** no histórico de transações e na seção de pagamentos do painel de pagamento | **Relatório de uso**: consumo mostrado com OrderID/OrderLineItemID<br>**Relatório de pedidos**: pedidos de clientes mostrados como ativos |
| Fatura de cliente coletada | 12/1/2020 | Marcado como **enviado** no histórico de transações e na seção de pagamentos do painel de pagamento | **Relatório de uso**: consumo mostrado com OrderID/OrderLineItemID<br>**Relatório de pedidos**: pedidos de clientes mostrados como ativos  |
|  |  |  |  |

\* Os relatórios de uso e de pedidos podem ser acessados na seção analisar no Partner Center.</br>\** A data do pagamento está no horário padrão do Pacífico (PST).

### <a name="customers-who-pay-using-credit-card-or-invoice"></a>Clientes que pagam usando cartão de crédito ou fatura

Todas as compras com um cartão de crédito ou uma nota fiscal mensal têm um período de manutenção de 30 dias para garantir que os fundos sejam apagados e não haja estorno ou fraude suspeita.

| Evento  | Data (UTC) | Visibilidade do parceiro: relatório de pagamento do Partner Center  |  Visibilidade do parceiro: análise do Partner Center\*  |
| --- | --- | --- | --- |
| Transação ou mês de uso | 8/1/2019 - 8/31/2019 | N/D | **Relatório de uso**: novo consumo mostrado (atualizado a cada quatro horas)<br>**Relatório do pedido**: N/A |
| Final do termo (mês) | 8/31/2019 | N/D | **Relatório de uso**: consumo final do mês mostrado<br>**Relatório do pedido**: N/A |
| Ordem gerada | 9/3/2019 – 9/7/2019 | N/D | **Relatório de uso**: consumo mostrado com OrderID/OrderLineItemID<br>**Relatório de pedidos**: pedidos de clientes mostrados como ativos |
| Fatura de cliente coletada | 9/7/2019 – 9/10/2019 | N/D | **Relatório de uso**: consumo mostrado com OrderID/OrderLineItemID<br>**Relatório de pedidos**: pedidos de clientes mostrados como ativos |
| Calcular pagamento | 9/8/2019 -9/12/2019 | Marcado como não **processado** no histórico de transações no painel do pagamento | **Relatório de uso**: consumo mostrado com OrderID/OrderLineItemID<br>**Relatório de pedidos**: pedidos de clientes mostrados como ativos |
| Pagamento mensal | 5/11/2019\* | Marcado como **futuro** no histórico de transações no painel de pagamento | **Relatório de uso**: consumo mostrado com OrderID/OrderLineItemID<br>**Relatório de pedidos**: pedidos de clientes mostrados como ativos |
| Data do pagamento\** | 15/11/2019 | Marcado como **enviado** no histórico de transações e na seção de pagamentos no painel de pagamento | **Relatório de uso**: consumo mostrado com OrderID/OrderLineItemID<br>**Relatório de pedidos**: pedidos de clientes mostrados como ativos |
|  |  |  |  |

\* Os relatórios de uso e de pedidos podem ser acessados na seção analisar no Partner Center.</br>\** A data do pagamento está no horário padrão do Pacífico (PST).

### <a name="enterprise-agreement-transactions-prior-to-may-1-2020"></a>Enterprise Agreement transações antes de 1º de maio de 2020

Todas as compras que ocorrem antes dessa data são processadas e pagas de acordo com a agenda abaixo após a Microsoft ter coletado o pagamento dos clientes e processado a taxa do Marketplace.

| Evento  | Data (UTC)  | Visibilidade do parceiro: relatório de pagamento do Partner Center  |  Visibilidade do parceiro: análise do Partner Center\*  |
| --- | --- | --- | --- |
| Transação ou mês de uso | 8/1/2019 – 8/31/2019 | N/D | **Relatório de uso**: novo consumo mostrado (atualizado a cada quatro horas)<br>**Relatório do pedido**: N/A |
| Final do termo (mês) | 8/31/2019 | N/D | **Relatório de uso**: consumo final do mês mostrado<br>**Relatório do pedido**: N/A |
| Ordem gerada | 9/3/2019 – 9/7/2019 | N/D | **Relatório de uso**: consumo mostrado com OrderID/OrderLineItemID<br>**Relatório de pedidos**: pedidos de clientes mostrados como ativos |
| Fatura de cliente coletada | 12/1/2019 | N/D | **Relatório de uso**: consumo mostrado com OrderID/OrderLineItemID<br>**Relatório de pedidos**: pedidos de clientes mostrados como ativos |
| Calcular pagamento | 12/5/2019 – 12/7/2019 | Marcado como não **processado** no histórico de transações no painel do pagamento | **Relatório de uso**: consumo mostrado com OrderID/OrderLineItemID<br>**Relatório de pedidos**: pedidos de clientes mostrados como ativos |
| Pagamento mensal | 1/5/2019 | Marcado como **futuro** no histórico de transações no painel de pagamento | **Relatório de uso**: consumo mostrado com OrderID/OrderLineItemID<br>**Relatório de pedidos**: pedidos de clientes mostrados como ativos |
| Data do pagamento\** | 1/15/2019 | Marcado como **enviado** no histórico de transações e na seção de pagamentos no painel do pagamento | **Relatório de uso**: consumo mostrado com OrderID/OrderLineItemID<br>**Relatório de pedidos**: pedidos de clientes mostrados como ativos |
|  |  |  |  |

\* Os relatórios de uso e de pedidos podem ser acessados na seção analisar no Partner Center.</br>\** A data do pagamento está no horário padrão do Pacífico (PST).

## <a name="process-for-customer-non-payment"></a>Processo de não pagamento de cliente

Em raras ocasiões, a Microsoft não consegue coletar pagamentos de clientes para suas compras do Marketplace comercial. Quando um cliente não paga a Microsoft de acordo com seu agendamento de cobrança, começamos o processo de coleções. Esse processo leva aproximadamente quatro meses e envolve a comunicação persistente da Microsoft. Se o pagamento não for recebido no final deste processo, a Microsoft gravará os fundos como não coletáveis.

De acordo com o processo de pagamento articulado aqui, a Microsoft pode já ter pago os fundos para os editores (você) que, por fim, não podem ser coletados. Portanto, temos um processo para reconciliar esses valores. Para garantir que você tenha um aviso de que o pagamento (já recebido) pode ser reconciliado, você será notificado quando um cliente estiver no processo de cobranças e as compras provavelmente serão gravadas.

A Microsoft recuperará todos os pagamentos já pagos usando um dos seguintes métodos: (1) a Microsoft poderá subtrair os valores não pagos de pagamentos futuros; por exemplo, se $1000 em pagamentos forem considerados não colecionáveis e gravados, seus pagamentos futuros serão retidos até que a $1000 seja recuperada ou (2) a Microsoft poderá solicitar um reembolso ou Publicadores de notas fiscais por quaisquer valores não coletados.

A tabela a seguir mostra um exemplo de agendamento:

| Evento | Data aproximada | Visibilidade do parceiro |
| --- | --- | --- |
| Data de pagamento de exemplo | 10/15/2020 | Marcado como **enviado** no histórico de transações e na seção de pagamentos no painel de pagamento |
| Se o cliente não pagar a Microsoft | 12/2/2020 – 12/5/2020 | Nenhuma alteração, igual à acima |
| O cliente recebe o primeiro email de pagamento atrasado | 12/6/2020 | Nenhum |
| O cliente recebe emails regulares de maior urgência | 12/7/2020 – 1/31/2021 | Nenhum |
| A gravação notificada do Publicador é provavelmente | 1/7/2021 | Notificação por email enviada ao Publicador de que seu cliente ainda não enviou o pagamento. A ID da transação e o valor de dólar estão incluídos. |
| O cliente recebe aviso de encerramento | 2/1/2021 | Nenhum |
| O processo de coleta termina/fundos são gravados | 2/15/2021 | Notificação por email enviada ao Publicador de que os fundos foram gravados. A ID da transação e o valor de dólar estão incluídos. |
| Pagamento deduzido | 3/1/2021 | O Publicador verá uma transação negativa na instrução pagamento do Partner Center |
| Pagamento retido | 3/15/2021 | Pagamentos futuros serão mostrados na instrução pagamento do centro de parceiros. O Publicador não receberá o pagamento até que o saldo não seja mais negativo.  |
|||

## <a name="number-of-days-for-payments-to-reach-a-payout-account"></a>Número de dias para os pagamentos chegarem a uma conta de pagamento

Normalmente, enviamos qualquer pagamento devido em um determinado mês no 15º dia desse mês, mas leva mais tempo para que o pagamento chegue à sua conta. O número de dias depende do método de pagamento que usamos para sua conta, conforme descrito abaixo.

> [!NOTE]
> Os dias mostrados abaixo são aproximados; qualquer pagamento pode levar um tempo maior ou menor para alcançar sua conta.

| Método de pagamento     | Número de dias até chegar à conta de pagamento     |
|--------------------|--------------------------------------------|
| PayPal             | 1 dia útil                             |
| ACH/SEPA           | 2 a 3 dias úteis                          |
| Transferência eletrônica      | 7 a 10 dias úteis                         |

## <a name="next-step"></a>Próxima etapa

- [Detalhes do imposto](tax-details-marketplace.md)
