---
title: Visão geral de cobrança | Partner Center
ms.topic: article
ms.date: 10/29/2018
Description: Information on basic billing scenarios and the differences between license-based and usage-based billing
author: labrenne
ms.author: labrenne
keywords: cobrança, pagamentos, pedidos, cancelamento, gerenciamento de pedidos, falta de pagamento, fraude, uso indevido, imposto, isenções fiscais, arquivos de reconciliação, arquivo de reconciliação
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: eebf3573cdb6724497bb7933d7edc08879dc8e5e
ms.sourcegitcommit: 9ea2f05f938ea22251f3719b61f03ccb71d3494f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/03/2019
ms.locfileid: "8990938"
---
# <a name="billing-overview"></a>Visão geral de cobrança

**Aplica-se a**

-  Partner Center
-  Parceiros no programa CSP

Dependendo dos produtos, soluções e serviços que você compra em nome dos seus clientes, você será cobrado por essas compras em uma ou mais das seguintes maneiras:
-   [Cobrança baseada em licença](#licensebasedbilling)

    Ao comprar produtos ou serviços online que exigem licenças, você está cobrado por cada licença que você comprou (não no uso de licença). Você pode optar por ser cobrado uma vez por mês ou uma vez por ano. Se seus negócios mudam, você pode alternar de um para o outro e novamente. 
    
    Para obter mais informações sobre mensal versus a cobrança anual, consulte a cobrança [perguntas Frequentes](https://docs.microsoft.com/en-us/partner-center/faq-about-new-billing-features).

-   [Cobrança baseada em uso](#usagebasedbilling)

    Ao comprar serviços on-line como assinaturas do Azure, você está cobrado por taxas mensal de uso. Cobrança mensal só está disponível para produtos baseados em uso. Serviços baseados em uso, como Azure, são cobrados de acordo com taxas limitadas, com base no consumo.

-   [Cobrança única](#onetimebilling)

    Ao comprar reservas do Azure ou outras assinaturas de software, você paga antecipadamente por um termo previamente configurado. Porque você está pagando antecipadamente, você está cobrado em uma quantia. 
    
Se você optou por ser cobrados mensalmente ou se você comprou produtos baseados em uso são cobrados mensalmente, sua data de cobrança mensal é o dia do mês selecionado quando você criou sua conta do CSP no Partner Center. Depois que você criou com êxito sua conta do CSP, a Microsoft enviará um email de confirmação que inclui sua data de cobrança. Depois de criados, essa data não pode ser alterada. 

## <a name="pricing-and-invoicing"></a>Preços e faturamento
Você pode encontrar listas de preços com um (1) mês de antecedência, pois são atualizadas mensalmente. Os preços baseados em licença são garantidos durante o período da assinatura, geralmente 12 meses a partir da data de compra. Os preços baseados em uso podem ser alterados mensalmente. 

Os preços para assinaturas de software, serviços e produtos são garantidos por meio da duração da assinatura, no entanto, os preços podem mudar quando você renovar.

Você verá os ajustes e créditos em atraso em sua próxima fatura de cobrança após o crédito ou ajuste ser aplicado.

Você pode ver e baixar suas faturas e seus arquivos de reconciliação na página Cobrança no Partner Center. Observe que as faturas mensais estarão disponíveis no Partner Center em até quatro (4) dias da data de cobrança selecionada.

## <a name="payment-terms"></a>Termos de pagamento

Termos de pagamento são net 60 dias. As faturas devem ser pagas pelo fatura data de vencimento (60 dias após a data de cobrança), ou sua conta se tornará inadimplente, que pode afetar sua inscrição no CSP. Você pode retomar a funcionalidade total de suas contas suspensas quando você paga passado quantidade de vencimento.

### <a name="tax"></a>Imposto

Você é sobrecarregados com base em seus detalhes, (não dos seus clientes) como a relação de cobrança é entre você e a Microsoft. Você pode enviar seu ID do contribuinte durante o processo de instalação de conta ou enviando uma solicitação de suporte mais tarde. Você verá as alterações refletidas no seu próximo ciclo de cobrança.

-   Para isenção de imposto sobre vendas e retenção, você deve enviar a documentação do contribuinte por meio de uma solicitação de suporte. Você verá as alterações e reembolsos apropriados em seu próximo ciclo de cobrança.

-   Para isenção de imposto sobre valor agregado (IVA), você deve enviar seu ID de IVA (validado pela Microsoft) por meio de uma solicitação de serviço. Você verá as alterações e reembolsos apropriados em seu próximo ciclo de cobrança.

Você pode encontrar mais detalhes fiscais do escritório fiscal local ou consultor de imposto.

## <a href="" id="licensebasedbilling"></a>Cobrança baseada em licença

Quando você compra um produto baseado em licença em nome do cliente, você pode optar por ser cobrados mensalmente ou anualmente. Se você quiser alterar a frequência de cobrança em um momento posterior, use o procedimento a seguir. 

Alternar de cobrança mensal para cobrança anual é útil se você tiver várias assinaturas que são cobradas mensalmente e você deseja alinhá-los até uma data de cobrança comuns. Alternar de cobrança anual para cobrança mensal é útil em adaptar suas datas de faturamento aos seus clientes individuais. 

Quando você alterar a frequência de cobrança, o termo anual é atualizado para refletir que a data em que você alterou a frequência de cobrança e uma nova data de renovação são estabelecidas. 

Você pode alterar a frequência de cobrança sempre que seus negócios mudam. 

### <a name="billing-rules-for-annual-billing"></a>Regras de cobrança para cobrança anual

-   As assinaturas são anuais com renovação automática.

-   A cobrança é em 12 pagamentos mensais ou um pagamento anual por assinatura anual.

-   Você será cobrado com antecedência pelo próximo período de cobrança pelos serviços baseados em licença, de acordo com o número de licenças no final do período de cobrança anterior.

-   Você é cobrado/creditado em atraso de pagamento por alterações no número de licenças (cálculo proporcional com base em dias de licença). Cálculo proporcional usa a seguinte fórmula: [ROUND((ROUND(Preço unitário * Quantidade/Número de dias no mês proporcional, 2) * Número de dias proporcionais) / Quantidade, 2) * Quantidade]

-   Pagamentos são cobrados para licenças vendidas (não licenças provisionadas).

### <a name="to-change-the-billing-frequency-of-an-online-service"></a>Para alterar a frequência de cobrança de um serviço online

1.  Selecione **os clientes** no menu Partner Center e, em seguida, selecione o cliente com a assinatura que deseja alterar. 

2.  Na página de assinaturas do cliente, selecione a assinatura que deseja alterar. 

3.  Na página de detalhes, sob a **frequência de cobrança**, selecione **mensal** ou **anual**. Você verá uma página de confirmação com informações importantes sobre como alterar a frequência de cobrança, bem como uma lista as assinaturas prestes a ser alterado. 

4.  Selecione **Okey** para fazer a alteração, ou **Cancelar** para desfazer a ele. 

### <a name="adjustmentscreditscancellations"></a>Ajustes/créditos/cancelamentos

A Microsoft não cobrará taxas de término antecipado para cancelamento dos serviços baseados em licença. 

Os créditos de cancelamento para serviços baseados em licença são proporcionais aos dias não utilizados para cancelamentos de ciclo médio (bem como pela diminuição de licenças pela fórmula acima).

## <a href="" id="usagebasedbilling"></a>Cobrança baseada em uso

Alguns produtos e serviços Microsoft usam um modelo de cobrança "pré-pago", na qual você será cobrado somente pelos serviços usados. Por exemplo, o Microsoft Azure usa esse modelo. 

### <a name="billing-rules"></a>Regras de cobrança
-   As assinaturas são mês a mês e renovadas automaticamente com as novas taxas de serviço limitadas. Você está cobrado mensalmente para uso do mês anterior.

-   As taxas de serviço limitadas podem ser alteradas dentro do ciclo de fatura. 

    -   Aumentos de preço: é fornecido um aviso prévio de 30 dias.

    -   Preço diminui: dia de alteração refletido.

    -   As assinaturas existentes usam a taxa em vigor no início do ciclo de cobrança.

    -   Novas assinaturas, quando criado dentro do mesmo ciclo de cobrança, usam a taxa em vigor na data que criá-las. 

### <a name="adjustmentscreditscancellations"></a>Ajustes/créditos/cancelamentos

Você verá pagamentos com ajustes em sua próxima fatura de cobrança mensal.

A Microsoft não cobrará taxas de término antecipado para cancelamento dos serviços baseados em uso. 

Você verá créditos de qualquer tipo, incluindo créditos SLAs, em sua próxima fatura de cobrança mensal.

## <a href="" id="onetimebilling"></a>Cobrança única

Você pode adquirir assinaturas de software e reservas do Azure com antecedência, para termos de um a três anos. Quando você compra antecipadamente, você está cobrado por custo inteiro em uma quantia de um. Esse tipo de cobrança é chamado de cobrança única.

>[!IMPORTANT]
>Se você comprar reservas do Azure e/ou assinaturas de software para um cliente em um local com uma moeda diferente da sua, o padrão de moeda de cobrança é baseado no local do cliente, não em sua localização. Se você tiver clientes em vários locais, você receberá faturas separadas e arquivos de reconciliação para clientes cada moeda precisam ser cobrados, permitindo que você faturas para seus clientes na moeda apropriada. 

### <a name="manage-your-one-time-billing"></a>Gerenciar a cobrança única

**Exibir o status de cobrança, as faturas e os arquivos de reconhecimento atuais**

1.  No Partner Center, selecione **de cobrança** e, em seguida, **uma vez** para exibir o status de cobrança. 

2.  Selecione uma fatura ou um arquivo de reconhecimento para exibir informações mais detalhadas. 

**Exibir o histórico de pedidos de um cliente**

1.  Selecione **os clientes** no menu Partner Center.

2.  Na sua página **Clientes**, localize o cliente cujo histórico de pedidos você deseja exibir e, em seguida, selecione a seta para baixo para expandir o registro do cliente. 

3.  Selecione **Exibir pedidos** para exibir o histórico de pedidos.

**Baixe uma nota de crédito**

Se você precisar solicitar um crédito ou uma nova cobrança, forneceremos uma nota de crédito para cancelar a fatura original. Você pode solicitar uma crédito/nova cobrança pelos seguintes motivos:

-   Correções de ordem de compra ou endereço

-   Fatura gerada e, em seguida, um reembolso de imposto foi aplicado. Você pode solicitar uma crédito/nova cobrança para obter o reembolso de imposto puxado de volta para a fatura original. Isso também é verdadeiro para reembolsos, como você pode solicitar uma crédito/nova cobrança da fatura original e, em seguida, recepção em um reembolso.
