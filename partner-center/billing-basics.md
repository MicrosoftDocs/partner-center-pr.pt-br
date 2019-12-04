---
title: Visão geral da cobrança | Centro de parceiros
ms.topic: article
ms.date: 11/25/2019
description: Saiba mais sobre as informações básicas de cobrança e fatura para o Partner Center.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: LauraBrenner
ms.author: labrenne
keywords: cobrança, pagamentos, pedidos, cancelamento, gerenciamento de pedidos, falta de pagamento, fraude, uso indevido, imposto, isenções de imposto, arquivos de reconciliação, arquivo de reconciliação
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: e77d641b1b75c5d462871aa61c3f67bc6d6dd13e
ms.sourcegitcommit: c793c1b61f50fc0b0a12c95cedd9f57b31703093
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2019
ms.locfileid: "74722465"
---
# <a name="billing-overview"></a>Visão geral da cobrança

**Aplica-se a**

- Partner Center
- Parceiros no programa CSP (provedor de soluções na nuvem)

**Funções apropriadas**

- Agente administrativo
- Administrador de cobrança
- Administração global
- Agente de suporte técnico
- Agente de vendas

## <a name="find-your-bill"></a>Encontre sua fatura

Para encontrar sua fatura:

1. [Entre no painel do Partner Center](https://partner.microsoft.com/dashboard/home).

2. No menu à esquerda, escolha **cobrança**.

3. Na página de **cobrança** , você pode baixar sua última conta ou baixar as cobranças anteriores na seção **histórico de cobrança** .

## <a name="bill-your-customers"></a>Cobrar seus clientes

A Microsoft não tem requisitos ou condições sobre como você lida com seu próprio faturamento.

Para determinar o uso de um cliente, [consulte seus arquivos de reconciliação](#find-your-bill). Você pode usar o nome do cliente e outros campos relevantes para determinar o uso.

Em seguida, você pode adicionar suas próprias tarifas e cobranças para serviços e produtos que você fornecer. Em seguida, você pode enviar uma única cobrança para todos os encargos para o cliente.

### <a name="billing-types"></a>Tipos de cobrança

Os tipos de cobrança no Partner Center incluem **a cobrança baseada em licença**, **a cobrança baseada no uso**e o **billign único**. Para obter mais informações, consulte a explicação completa de [tipos de cobrança no Partner Center](billing-different-types.md).

### <a name="billing-currency"></a>Moeda de cobrança

Você será cobrado por produtos na moeda do país ou da região em que está localizado. Você é cobrado da mesma, independentemente do local do cliente para quem você vendeu os produtos.

## <a name="invoices"></a>Faturas

Sua fatura é um resumo de todos os encargos para o período de cobrança atual. Isso inclui cobranças entre o programa, todos os produtos e todos os clientes. Para obter exemplos de cenários de cobrança mensal e anual, consulte [cenários comuns de cobrança](common-billing-scenarios.md)

Sua fatura está disponível dentro de dois (2) dias da data de cobrança selecionada em hora UTC. Por exemplo, se você tiver uma data de cobrança igual a 12 de setembro, o processo de geração da fatura será iniciado em 00:00 UTC no dia 13 e será concluído até 00:00 UTC no dia 14. Se você não vir sua fatura por 11:59PM UTC no dia 15, você está fora de seu Contrato de Nível de Serviço e deve arquivar uma solicitação de serviço.

Parceiros no programa CSP (provedor de soluções na nuvem) que optam por ser cobrado mensalmente pagam a Microsoft 60 dias em pelos débitos anteriores para as assinaturas de seus clientes (baseadas em licença e de uso).

## <a name="price-lists"></a>Listas de preços

As listas de preços são atualizadas mensalmente. As listas de preços de visualização estão disponíveis um (1) mês com antecedência.

Para exibir listas de preços:

1. [Entre no painel do Partner Center](https://partner.microsoft.com/dashboard/home).
2. No menu à esquerda, escolha **vender**e, em seguida, selecione **preços e ofertas**.
3. Na página **preços e ofertas** , você pode ver 6 meses de listas de preços (incluindo o mês atual) e listas de preços de visualização (quando aplicável).

Os preços **baseados em licença** são garantidos para o termo da assinatura, geralmente 12 meses a partir da data de compra. 

Os **preços com base no uso** podem ser alterados mensalmente.

Os **preços de produtos, serviços e assinaturas de software** são garantidos por meio da duração da assinatura. No entanto, os preços podem mudar quando você renova.

Você verá os **ajustes** e **créditos** em pelos débitos anteriores em sua próxima fatura de cobrança depois que o crédito ou o ajuste for aplicado.

## <a name="payment-terms"></a>Termos de pagamento

Os termos de pagamento são líquidos 60 dias. As notas fiscais devem ser pagas pela data de vencimento da nota fiscal (60 dias após a data de cobrança) ou sua conta será inadimplente, o que pode afetar seu registro no CSP. 

Você pode obter a funcionalidade completa de suas contas suspensas ao pagar o valor vencido.

### <a name="taxes-and-vat"></a>Impostos e IVA

Você é cobrado com base nos detalhes (não nos detalhes dos seus clientes), pois a relação de cobrança é entre a Microsoft e você. Você pode enviar seu identificador de imposto durante o processo de configuração da conta ou por meio de uma solicitação de suporte mais tarde. Você verá as alterações refletidas no seu próximo ciclo de cobrança.

Para a **isenção de imposto sobre vendas e retenção**, você deve enviar a documentação do imposto por meio de uma solicitação de suporte. Você verá as alterações e reembolsos apropriados em seu próximo ciclo de cobrança.

Para **isenção de imposto de valor agregado (IVA)** , você deve enviar sua ID de IVA (validada pela Microsoft) por meio de uma solicitação de serviço. Você verá as alterações e reembolsos apropriados em seu próximo ciclo de cobrança.

Você pode encontrar detalhes mais detalhados de seu escritório fiscal ou consultor fiscal local.

### <a name="annual-billing-rules"></a>Regras de cobrança anual

As assinaturas são anuais com renovação automática.

A cobrança é feita em 12 pagamentos mensais ou um anual por assinatura anual.

Você será cobrado com antecedência pelo próximo período de cobrança pelos serviços baseados em licença, de acordo com o número de licenças no final do período de cobrança anterior.

Você é cobrado/creditado em atraso de pagamento por alterações no número de licenças (cálculo proporcional com base em dias de licença). O cálculo pro-favorável usa a seguinte fórmula:

`[ROUND((ROUND(Unit Price * Quantity / Number of days in pro-rated Month, 2) * Number of pro-rated days) / Quantity, 2) * Quantity]`

Os pagamentos são cobrados por licenças vendidas, não licenças provisionadas.

### <a name="change-billing-frequency"></a>Alterar frequência de cobrança

Para alterar a frequência de cobrança de um serviço online para um cliente:

1. [Entre no painel do Partner Center](https://partner.microsoft.com/dashboard/home).
2. No menu à esquerda, escolha **clientes**.
3. Selecione o cliente cuja frequência de cobrança de assinatura você deseja alterar.
4. Na página **assinaturas** do cliente, selecione a assinatura que você deseja alterar.
5. Na página **detalhes** , em **frequência de cobrança**, selecione **mensal** ou **anual**. Você verá uma página de confirmação com informações importantes sobre como alterar a frequência de cobrança, bem como uma lista das assinaturas a serem alteradas.
6. Escolha **OK** para fazer a alteração (ou em **Cancelar** para desfazê-la).

### <a name="adjustmentscreditscancellations"></a>Ajustes/créditos/cancelamentos

A Microsoft não cobra as tarifas de rescisão antecipadas para o cancelamento de serviços baseados em licença.

Os créditos de cancelamento de serviços baseados em licenciados são avaliados por pro para dias não utilizados para cancelamentos de ciclo médio (bem como as diminuições de licença de acordo com a fórmula acima).

### <a name="billing-rules"></a>Regras de cobrança

As assinaturas são de mês a mês e são renovadas automaticamente às novas tarifas de serviço limitadas. Você será cobrado a cada mês pelo uso do mês anterior.

As taxas de serviço limitadas podem ser alteradas dentro do ciclo de fatura.

#### <a name="price-changes"></a>Alterações de preço

Para **aumentos de preço**, o aviso de 30 dias é fornecido.

As **diminuições de preço** são refletidas no dia da alteração.

As **assinaturas existentes** usam a taxa em vigor no início do ciclo de cobrança.

**Novas assinaturas**, quando criadas no mesmo ciclo de cobrança, usam a taxa em vigor na data em que você as cria. 

### <a name="adjustmentscreditscancellations"></a>Ajustes/créditos/cancelamentos

Você verá pagamentos com ajustes em sua próxima fatura de cobrança mensal.

A Microsoft não cobra as tarifas de rescisão antecipadas para o cancelamento de serviços baseados em uso. 

Você verá créditos de qualquer tipo, incluindo créditos SLAs, em sua próxima fatura de cobrança mensal.

>[!IMPORTANT]
>Se você comprar reservas do Azure e/ou assinaturas de software para um cliente em um local com uma moeda diferente da sua, a moeda de cobrança padrão será baseada no local do cliente, não no local. Se você tiver clientes em vários locais, receberá faturas e arquivos de reconciliação separados para cada moeda que os clientes precisam ser cobrados, permitindo que você faça faturas de seus clientes na moeda apropriada.

## <a name="manage-one-time-billing"></a>Gerenciar cobrança única

### <a name="billing-status-invoices-and-reconciliation-files"></a>Status de cobrança, faturas e arquivos de reconciliação

Para exibir seu status de cobrança atual, faturas e arquivos de reconciliação:

1. [Entre no painel do Partner Center](https://partner.microsoft.com/dashboard/home).
2. No menu à esquerda, escolha **cobrança**e, em seguida, selecione **uma vez**.
3. Na página status da cobrança, selecione uma nota fiscal ou um arquivo de reconciliação para exibir informações mais detalhadas.

### <a name="customer-order-history"></a>Histórico de pedidos de clientes

Para exibir o histórico de pedidos de um cliente:

1. [Entre no painel do Partner Center](https://partner.microsoft.com/dashboard/home).
2. No menu à esquerda, escolha **clientes**.
3. Na página **clientes** , localize o cliente cujo histórico de pedidos você deseja exibir. Selecione a seta para baixo para expandir o registro do cliente.
4. Escolha **Exibir pedidos** para exibir o histórico do pedido do cliente.

### <a name="credit-notes"></a>Notas de crédito

Talvez seja necessário solicitar um crédito ou faturar pelos seguintes motivos:

- Você precisa fazer correções de endereço ou de ordem de compra.
- Um reembolso de imposto foi aplicado depois que a nota fiscal foi gerada. Você pode solicitar um crédito ou uma fatura para obter o reembolso de imposto retirado da fatura original. O mesmo também é verdadeiro para reembolsos. Você pode solicitar um crédito ou uma fatura da fatura original e, em seguida, receber um reembolso.

Se você solicitar um crédito ou uma fatura, daremos uma nota de **crédito** para cancelar a fatura original.
