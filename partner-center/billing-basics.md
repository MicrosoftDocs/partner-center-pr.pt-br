---
title: Visão geral da cobrança | Centro de parceiros
ms.topic: article
ms.date: 03/15/2019
Description: Informações sobre cenários de cobrança básicos e as diferenças entre a cobrança baseada em licença e em uso
author: LauraBrenner
ms.author: labrenne
keywords: cobrança, pagamentos, pedidos, cancelamento, gerenciamento de pedidos, falta de pagamento, fraude, uso indevido, imposto, isenções fiscais, arquivos de reconciliação, arquivo de reconciliação
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: e13f3d24e649cf17daa1e3218c3376c8fc6e4faa
ms.sourcegitcommit: bae29ab191c72e15259d99c40c69a9e7c3f2b502
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/06/2019
ms.locfileid: "68820369"
---
# <a name="billing-overview"></a>Visão geral da cobrança

**Aplica-se a**

-  Partner Center
-  Parceiros no programa CSP

Dependendo dos produtos, das soluções e dos serviços que você comprar em nome dos seus clientes, você será cobrado por essas compras de uma ou mais das seguintes maneiras:
-   [Cobrança baseada em licença](#licensebasedbilling)

    Ao comprar produtos ou serviços online que exigem licenças, você será cobrado por cada licença que comprou (não no uso da licença). Você pode escolher se deseja ser cobrado uma vez por mês ou uma vez por ano. Se suas necessidades de negócios mudarem, você poderá alternar de uma para a outra e voltar. 
    
    Para obter mais informações sobre a cobrança mensal versus anual, consulte as [perguntas frequentes](https://docs.microsoft.com/partner-center/faq-about-new-billing-features)sobre cobrança.

-   [Cobrança baseada em uso](#usagebasedbilling)

    Ao comprar serviços online como assinaturas do Azure, você será cobrado por taxas de uso mensais. Somente a cobrança mensal está disponível para produtos baseados em uso. Os serviços baseados em uso, como o Azure, são cobrados de acordo com as tarifas limitadas, com base no consumo.

-   [Cobrança de uso único](#onetimebilling)

    Ao comprar reservas do Azure ou outras assinaturas de software, você paga com antecedência por um termo predefinido. Como você está pagando com antecedência, você será cobrado em uma soma total. 
    
Se você optou por ser cobrado mensalmente ou se comprou produtos com base no uso que são cobrados mensalmente, sua data de cobrança mensal é o dia do mês que você selecionou quando criou sua conta do CSP no Partner Center. Depois de criar com êxito sua conta do CSP, a Microsoft enviará um email de confirmação que inclui a data de cobrança. Depois de criada, essa data não pode ser alterada. 

## <a name="pricing-and-invoicing"></a>Preços e faturamento
Você pode encontrar listas de preços com um (1) mês de antecedência, pois são atualizadas mensalmente. Os preços baseados em licença são garantidos pelo termo de assinatura, geralmente 12 meses a partir da data de compra. Os preços baseados em uso podem ser alterados mensalmente. 

Os preços de produtos, serviços e assinaturas de software são garantidos por meio da duração da assinatura, no entanto, os preços podem mudar quando você renova.

Você verá os ajustes e créditos em atraso em sua próxima fatura de cobrança após o crédito ou ajuste ser aplicado.

Você pode ver e baixar suas faturas e seus arquivos de reconciliação na página Cobrança no Partner Center. Observe que as faturas mensais estarão disponíveis no Partner Center em até quatro (4) dias da data de cobrança selecionada.

## <a name="payment-terms"></a>Termos de pagamento

Os termos de pagamento são líquidos 60 dias. As notas fiscais devem ser pagas pela data de vencimento da nota fiscal (60 dias após a data de cobrança) ou sua conta será inadimplente, o que pode afetar seu registro no CSP. Você pode obter a funcionalidade completa de suas contas suspensas ao pagar o valor vencido.

### <a name="tax"></a>Tax

Você é cobrado com base nos seus detalhes (não em seus clientes), pois a relação de cobrança é entre a Microsoft e você. Você pode enviar sua ID de imposto durante o processo de configuração da conta ou enviando uma solicitação de suporte mais tarde. Você verá as alterações refletidas no seu próximo ciclo de cobrança.

-   Para a isenção de imposto sobre vendas e retenção, você deve enviar a documentação do imposto por meio de uma solicitação de suporte. Você verá as alterações e reembolsos apropriados em seu próximo ciclo de cobrança.

-   Para isenção de IVA (imposto sobre valor agregado), você deve enviar sua ID de IVA (validada pela Microsoft) por meio de uma solicitação de serviço. Você verá as alterações e reembolsos apropriados em seu próximo ciclo de cobrança.

Você pode encontrar detalhes mais detalhados de seu escritório fiscal ou consultor fiscal local.

## <a href="" id="licensebasedbilling"></a>Cobrança baseada em licença

Ao comprar um produto baseado em licença em nome de um cliente, você pode optar por ser cobrado mensal ou anualmente. Se você quiser alterar sua frequência de cobrança posteriormente, use o procedimento abaixo. 

Mudar de cobrança mensal para cobrança anual é útil se você tiver várias assinaturas que são cobradas mensalmente e quiser alinhá-las a uma data de cobrança comum. A mudança de cobrança anual para cobrança mensal é útil para adaptar suas datas de cobrança para as de seus clientes individuais. 

Quando você altera a frequência de cobrança, o termo anual é atualizado para refletir a data em que você alterou a frequência de cobrança e uma nova data de renovação é estabelecida. 

Você pode alterar a frequência de cobrança sempre que sua empresa precisar mudar. 

### <a name="billing-rules-for-annual-billing"></a>Regras de cobrança para cobrança anual

-   As assinaturas são anuais com renovação automática.

-   A cobrança é feita em 12 pagamentos mensais ou um anual por assinatura anual.

-   Você será cobrado com antecedência pelo próximo período de cobrança pelos serviços baseados em licença, de acordo com o número de licenças no final do período de cobrança anterior.

-   Você é cobrado/creditado em atraso de pagamento por alterações no número de licenças (cálculo proporcional com base em dias de licença). Cálculo proporcional usa a seguinte fórmula: [ROUND((ROUND(Preço unitário * Quantidade/Número de dias no mês proporcional, 2) * Número de dias proporcionais) / Quantidade, 2) * Quantidade]

-   Os pagamentos são cobrados por licenças vendidas (não licenças provisionadas).

### <a name="to-change-the-billing-frequency-of-an-online-service"></a>Para alterar a frequência de cobrança de um serviço online

1.  Selecione **clientes** no menu do centro de parceiros e, em seguida, selecione o cliente com a assinatura que você deseja alterar. 

2.  Na página assinaturas do cliente, selecione a assinatura que você deseja alterar. 

3.  Na página detalhes, em **frequência de cobrança**, selecione **mensal** ou **anual**. Você verá uma página de confirmação com informações importantes sobre como alterar a frequência de cobrança, bem como uma lista das assinaturas a serem alteradas. 

4.  Selecione **OK** para fazer a alteração ou em **Cancelar** para desfazê-la. 

### <a name="adjustmentscreditscancellations"></a>Ajustes/créditos/cancelamentos

A Microsoft não cobra as tarifas de rescisão antecipadas para o cancelamento de serviços baseados em licença. 

Os créditos de cancelamento para serviços baseados em licença são proporcionais aos dias não utilizados para cancelamentos de ciclo médio (bem como pela diminuição de licenças pela fórmula acima).

## <a href="" id="usagebasedbilling"></a>Cobrança baseada em uso

Alguns produtos e serviços da Microsoft usam um modelo de cobrança "pré-pago", no qual você será cobrado somente pelos serviços usados. Por exemplo, Microsoft Azure usa esse modelo. 

### <a name="billing-rules"></a>Regras de cobrança
-   As assinaturas são de mês a mês e são renovadas automaticamente às novas tarifas de serviço limitadas. Você será cobrado a cada mês pelo uso do mês anterior.

-   As taxas de serviço limitadas podem ser alteradas dentro do ciclo de fatura. 

    -   Aumentos de preço: o aviso de 30 dias é fornecido.

    -   Preço diminui: dia de alteração refletido.

    -   As assinaturas existentes usam a taxa em vigor no início do ciclo de cobrança.

    -   Novas assinaturas, quando criadas no mesmo ciclo de cobrança, usam a taxa em vigor na data em que você as cria. 

### <a name="adjustmentscreditscancellations"></a>Ajustes/créditos/cancelamentos

Você verá pagamentos com ajustes em sua próxima fatura de cobrança mensal.

A Microsoft não cobra as tarifas de rescisão antecipadas para o cancelamento de serviços baseados em uso. 

Você verá créditos de qualquer tipo, incluindo créditos SLAs, em sua próxima fatura de cobrança mensal.

## <a href="" id="onetimebilling"></a>Cobrança de uso único

Você pode adquirir assinaturas de software e reservas do Azure com antecedência, para termos de um ou três anos. Ao comprar antecipadamente, você será cobrado pelo custo total em uma soma única. Esse tipo de cobrança é chamado de cobrança única.

>[!IMPORTANT]
>Se você comprar reservas do Azure e/ou assinaturas de software para um cliente em um local com uma moeda diferente da sua, a moeda de cobrança padrão será baseada no local do cliente, não no local. Se você tiver clientes em vários locais, receberá faturas e arquivos de reconciliação separados para cada moeda que os clientes precisam ser cobrados, permitindo que você faça faturas de seus clientes na moeda apropriada. 

### <a name="manage-your-one-time-billing"></a>Gerenciar a cobrança única

**Exibir seu status de cobrança atual, faturas e arquivos reconhecimento**

1.  No Partner Center, selecione **cobrança** e, em seguida, **uma vez** para exibir o status de cobrança. 

2.  Selecione uma fatura ou um arquivo de reconhecimento para exibir informações mais detalhadas. 

**Exibir o histórico de pedidos de um cliente**

1.  Selecione **clientes** no menu do centro de parceiros.

2.  Na sua página **Clientes**, localize o cliente cujo histórico de pedidos você deseja exibir e, em seguida, selecione a seta para baixo para expandir o registro do cliente. 

3.  Selecione **Exibir pedidos** para exibir o histórico de pedidos.

**Baixar uma nota de crédito**

Se você precisar solicitar um crédito ou uma fatura, daremos uma nota de crédito para cancelar a fatura original. Você pode solicitar um crédito/fatura pelos seguintes motivos:

-   Correções de ordem de compra ou de endereço

-   A fatura foi gerada e então um reembolso de imposto foi aplicado. Você pode solicitar um crédito/nova cobrança para fazer o reembolso de imposto retroceder à fatura original. Isso também é verdadeiro para reembolsos, já que você pode solicitar um crédito/nova cobrança da fatura original e então obter um reembolso.
