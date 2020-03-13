---
title: Visão geral de cobrança | Partner Center
ms.topic: article
ms.date: 11/25/2019
description: Saiba mais sobre as informações básicas de cobrança e fatura para o Partner Center.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: LauraBrenner
ms.author: labrenne
keywords: cobrança, pagamentos, pedidos, cancelamento, gerenciamento de pedidos, falta de pagamento, fraude, uso indevido, imposto, isenções de imposto, arquivos de reconciliação, arquivo de reconciliação
ms.localizationpriority: high
ms.custom: seodec18
ms.openlocfilehash: 9ad98091829459612a320135629b6611f36c931a
ms.sourcegitcommit: eb4fc25524cc68c10906ccd3392914e805213ee5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "78340114"
---
# <a name="billing-overview"></a>Visão geral de cobrança

**Aplica-se a**

- Partner Center
- Parceiros no programa CSP (Provedor de Soluções na Nuvem)

**Funções apropriadas**

- Agente administrativo
- Administrador de cobrança
- Administrador global
- Agente de suporte técnico
- Agente de vendas

## <a name="find-your-bill"></a>Encontre sua fatura

Para encontrar sua fatura:

1. [Entre no painel do Partner Center](https://partner.microsoft.com/dashboard/home).

2. No menu à esquerda, escolha **Cobrança**.

3. Na página **Cobrança**, você pode baixar sua conta mais recente ou as listas anteriores na seção **Histórico de cobrança**.

## <a name="bill-your-customers"></a>Cobrar seus clientes

A Microsoft não tem requisitos ou condições sobre como você deve administrar seu sistema de faturas.

Para determinar o uso de um cliente, [confira seus arquivos de reconciliação](#find-your-bill). Você pode usar o nome do cliente e outros campos relevantes para determinar o uso.

Em seguida, você pode adicionar os próprios valores e suas tarifas para serviços e produtos que você fornece. Depois você pode enviar uma única cobrança para todas os encargos devidos por seu cliente.

### <a name="billing-types"></a>Tipos de cobrança

Os tipos de cobrança no Partner Center incluem **cobrança baseada em licença**, **cobrança baseada em uso** e **cobrança única**. Para obter mais informações, confira a explicação completa de [tipos de cobrança no Partner Center](billing-different-types.md).

### <a name="billing-currency"></a>Moeda de cobrança

Você será cobrado por produtos na moeda do país ou da região em que está localizado. Você é cobrado igual, independentemente do local do cliente para quem você vendeu os produtos.

## <a name="invoices"></a>Faturas

Sua fatura é um resumo de todos os encargos do período de cobrança atual. Isso inclui encargos entre o programa, todos os produtos e todos os clientes. Para obter exemplos de cenários de cobrança mensal e anual, confira [cenários comuns de cobrança](common-billing-scenarios.md)

Sua fatura estará disponível dentro de 2 (dois) dias da data de cobrança selecionada no horário UTC. Por exemplo, se você tiver uma data de cobrança igual a 12 de setembro, o processo de geração da fatura será iniciado em 00:00 UTC no dia 13 e será concluído até 00:00 UTC no dia 14. Caso a sua fatura não seja exibida até 23h59 UTC do dia 15, você estará fora do Contrato de Nível de Serviço e deverá registrar uma solicitação de serviço.

Os parceiros no programa CSP (Provedor de Soluções na Nuvem) que optam pela cobrança mensal pagam à Microsoft 60 dias em atraso pelas assinaturas (baseadas em licença e em uso) dos clientes deles.

## <a name="price-lists"></a>Listas de preços

As listas de preços são atualizadas mensalmente. As listas de preços de versão prévia estão disponíveis com 1 (um) mês de antecedência.

Para exibir as listas de preços:

1. [Entre no painel do Partner Center](https://partner.microsoft.com/dashboard/home).
2. No menu à esquerda, escolha **Vender**, em seguida, selecione **Preços e ofertas**.
3. Na página **Preços e ofertas**, você pode ver 6 meses de listas de preços (incluindo o mês atual) e listas de preços de versão prévia (quando aplicável).

Os preços **baseados em licença** são garantidos pelo termo de assinatura, geralmente 12 meses a partir da data de compra. 

Os **preços baseados em uso** podem ser alterados mensalmente.

Os **preços de produtos, serviços e assinaturas de software** são garantidos pela duração da assinatura. No entanto, os preços podem mudar quando você renova.

Você verá **ajustes** e **créditos** em atraso em sua próxima fatura de cobrança após o crédito ou ajuste ser aplicado.

## <a name="payment-terms"></a>Termos de pagamento

Os termos de pagamento são 60 dias corridos. As faturas devem ser pagas até data de vencimento (60 dias após a data de cobrança) ou sua conta estará inadimplente, o que pode afetar seu registro no CSP. 

Você poderá recuperar funcionalidade completa de suas contas suspensas quando pagar o montante devido.

### <a name="taxes-and-vat"></a>Impostos e IVA

Você paga imposto com base em seus detalhes (não dos seus clientes) porque o relacionamento de cobrança se dá entre você e a Microsoft. Você pode enviar seu identificador fiscal durante o processo de configuração da conta ou por meio de uma solicitação de suporte mais tarde. Você verá as alterações refletidas no seu próximo ciclo de cobrança.

Para **isenção de impostos sobre vendas e retenção**, você deve enviar a documentação fiscal por meio de uma solicitação de suporte. Você verá as alterações e reembolsos apropriados em seu próximo ciclo de cobrança.

Para **isenção do IVA (imposto sobre valor agregado)** , você deve enviar sua ID do IVA (validado pela Microsoft) por meio de uma solicitação de serviço. Você verá as alterações e reembolsos apropriados em seu próximo ciclo de cobrança.

Você pode encontrar mais detalhes sobre impostos no escritório fiscal local ou de um consultor fiscal.

### <a name="annual-billing-rules"></a>Regras sobre a cobrança anual

As assinaturas são anuais com renovação automática.

A cobrança é feita em 12 pagamentos mensais ou um anual por assinatura anual.

Você será cobrado com antecedência pelo próximo período de cobrança pelos serviços baseados em licença, de acordo com o número de licenças no final do período de cobrança anterior.

Você é cobrado/creditado em atraso de pagamento por alterações no número de licenças (cálculo proporcional com base em dias de licença). O cálculo proporcional usa a seguinte fórmula:

`[ROUND((ROUND(Unit Price * Quantity / Number of days in pro-rated Month, 2) * Number of pro-rated days) / Quantity, 2) * Quantity]`

Pagamentos são cobrados por licenças vendidas, não licenças provisionadas.

### <a name="change-billing-frequency"></a>Alterar a frequência de cobrança

Para alterar a frequência de cobrança de um serviço online para um cliente:

1. [Entre no painel do Partner Center](https://partner.microsoft.com/dashboard/home).
2. No menu à esquerda, escolha **Clientes**.
3. Selecione o cliente cuja frequência de cobrança de assinatura você deseja alterar.
4. Na página **Assinaturas** do cliente, selecione a assinatura que você deseja alterar.
5. Na página **Detalhes**, em **Frequência de cobrança**, selecione **Mensal** ou **Anual**. Você verá uma página de confirmação com informações importantes sobre como alterar a frequência de cobrança, bem como uma lista das assinaturas a serem alteradas.
6. Escolha **OK** para fazer a alteração (ou **Cancelar** para desfazê-la).

### <a name="adjustmentscreditscancellations"></a>Ajustes/créditos/cancelamentos

A Microsoft não cobra valores de cancelamento antecipado dos serviços baseados em licença.

Os créditos de cancelamento para serviços baseados em licença são proporcionais aos dias não utilizados para cancelamentos de ciclo médio (bem como pela diminuição de licenças de acordo com a fórmula acima).

### <a name="billing-rules"></a>Regras de cobrança

As assinaturas são de mês a mês e renovadas automaticamente de acordo com as novas taxas de serviço limitadas. Você será cobrado a cada mês pelo uso do mês anterior.

As taxas de serviço limitadas podem ser alteradas dentro do ciclo de fatura.

#### <a name="price-changes"></a>Alterações de preço

Para **aumentos de preço**, é fornecido um aviso prévio de 30 dias.

As **diminuições de preço** são refletidas no dia da alteração.

As **assinaturas existentes** usam a taxa em vigor no início do ciclo de cobrança.

**Novas assinaturas**, quando criadas no mesmo ciclo de cobrança, usam a taxa em vigor na data em que você as cria. 

### <a name="adjustmentscreditscancellations"></a>Ajustes/créditos/cancelamentos

Você verá pagamentos com ajustes em sua próxima fatura de cobrança mensal.

A Microsoft não cobra valores de cancelamento antecipado dos serviços baseados no uso. 

Você verá créditos de qualquer tipo, incluindo créditos SLAs, em sua próxima fatura de cobrança mensal.

>[!IMPORTANT]
>Se você comprar reservas e/ou assinaturas de software do Azure para um cliente em um local com uma moeda diferente da sua, a moeda de cobrança padrão será baseada no local do cliente, não no seu. Se você tiver clientes em vários locais, receberá faturas separadas e arquivos de reconciliação para cada moeda em que os clientes precisam ser cobrados, permitindo que você envie faturas para seus clientes na moeda apropriada.

## <a name="manage-one-time-billing"></a>Gerenciar cobrança única

### <a name="billing-status-invoices-and-reconciliation-files"></a>Status da cobrança, faturas e arquivos de reconciliação

Para exibir o status de cobrança, as faturas e os arquivos de reconciliação:

1. [Entre no painel do Partner Center](https://partner.microsoft.com/dashboard/home).
2. No menu à esquerda, escolha **Cobrança** e, em seguida, selecione **Única**.
3. Na página de status da cobrança, selecione uma nota fiscal ou um arquivo de reconciliação para exibir informações mais detalhadas.

### <a name="customer-order-history"></a>Histórico de pedidos do cliente

Para exibir o histórico de pedidos de um cliente:

1. [Entre no painel do Partner Center](https://partner.microsoft.com/dashboard/home).
2. No menu à esquerda, escolha **Clientes**.
3. Na página **Clientes**, localize o cliente cujo histórico de pedidos você deseja exibir. Selecione a seta para baixo para expandir o registro do cliente.
4. Escolha **Exibir pedidos** para exibir o histórico de pedidos do cliente.

### <a name="credit-notes"></a>Notas de crédito

Talvez você precise solicitar um crédito ou uma nova cobrança pelos seguintes motivos:

- Você precisa fazer correções no endereço ou em uma ordem de compra.
- Um reembolso de imposto foi aplicado depois que a fatura foi gerada. Você pode solicitar um crédito ou nova cobrança para fazer o reembolso de imposto retroceder à fatura original. Isso também é válido para reembolsos. Você pode solicitar um crédito ou uma nova cobrança da fatura original e receber um reembolso.

Se você solicitar um crédito ou uma nova cobrança, daremos uma **nota de crédito** para cancelar a nota fiscal original.
