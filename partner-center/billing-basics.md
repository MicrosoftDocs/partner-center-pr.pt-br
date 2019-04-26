---
title: Visão geral de cobrança | Partner Center
ms.topic: article
ms.date: 03/15/2019
Description: Obter informações sobre cenários básicos de cobrança e as diferenças entre a cobrança baseados em uso e licença
author: LauraBrenner
ms.author: labrenne
keywords: cobrança, pagamentos, pedidos, cancelamento, gerenciamento de pedidos, falta de pagamento, fraude, uso indevido, imposto, isenções fiscais, arquivos de reconciliação, arquivo de reconciliação
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: cd1488fbe107363ca924823cdd526005f5a3f21c
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2019
ms.locfileid: "62135386"
---
# <a name="billing-overview"></a>Visão geral de cobrança

**Aplica-se a**

-  Partner Center
-  Parceiros no programa CSP

Dependendo da produtos, soluções e serviços que você compra em nome de seus clientes, você será cobrado por essas compras em uma ou mais das seguintes maneiras:
-   [Cobrança baseada em licença](#licensebasedbilling)

    Quando você compra produtos ou serviços online que exigem licenças, você será cobrado para cada licença que você comprou (não em uso de licença). Você pode optar por ser cobrado uma vez por mês ou uma vez por ano. Se suas necessidades comerciais mudarem, você pode alternar de um para outro e vice-versa. 
    
    Para obter mais informações sobre mensal versus cobranças anuais, consulte a cobrança [perguntas frequentes sobre](https://docs.microsoft.com/en-us/partner-center/faq-about-new-billing-features).

-   [Cobrança com base no uso](#usagebasedbilling)

    Quando você compra online services, como as assinaturas do Azure, você será cobrado por taxas de uso mensal. A cobrança mensal só está disponível para produtos com base no uso. Serviços baseados em uso, como o Azure, são cobrados de acordo com as taxas limitadas, com base no consumo.

-   [Cobrança de uso única](#onetimebilling)

    Quando você comprar reservas do Azure ou outras assinaturas de software, você paga antecipadamente por um período predefinido. Porque você está pagando com antecedência, você será cobrado em uma quantia. 
    
Se você tiver escolhido será cobrado mensalmente, ou se você comprou com base no uso de produtos que são cobrados mensalmente, sua data de cobrança mensal é o dia do mês em que você selecionou quando criou sua conta do CSP no Partner Center. Depois que você criou com êxito sua conta do CSP, a Microsoft enviará um email de confirmação que inclui sua data de cobrança. Depois de criado, essa data não pode ser alterada. 

## <a name="pricing-and-invoicing"></a>Preços e faturamento
Você pode encontrar listas de preços com um (1) mês de antecedência, pois são atualizadas mensalmente. Os preços baseados em licença são garantidos pelo termo de assinatura, geralmente 12 meses a partir da data de compra. Os preços baseados em uso podem ser alterados mensalmente. 

Os preços para produtos, serviços e assinaturas de software são garantidos por meio da duração da assinatura, no entanto, os preços podem ser alteradas quando você renovar.

Você verá os ajustes e créditos em atraso em sua próxima fatura de cobrança após o crédito ou ajuste ser aplicado.

Você pode ver e baixar suas faturas e seus arquivos de reconciliação na página Cobrança no Partner Center. Observe que as faturas mensais estarão disponíveis no Partner Center em até quatro (4) dias da data de cobrança selecionada.

## <a name="payment-terms"></a>Termos de pagamento

Condições de pagamento são net 60 dias. Notas fiscais devem ser pagas pela nota fiscal data de conclusão (60 dias após a data de cobrança) ou sua conta será efetuada, que pode causar impacto em seu registro no CSP. Você pode recuperar a funcionalidade completa de suas contas suspensas quando você paga passado quantidade devida.

### <a name="tax"></a>Tax

Você é sobrecarregados com base em seus detalhes, (não dos seus clientes) como a relação de cobrança é entre você e a Microsoft. Você pode enviar a ID de imposto durante o processo de configuração de conta ou enviando uma solicitação de suporte mais tarde. Você verá as alterações refletidas no seu próximo ciclo de cobrança.

-   Para garantia de imposto e isenção de imposto sobre vendas, você deve enviar a documentação de imposto por meio de uma solicitação de suporte. Você verá as alterações e reembolsos apropriados em seu próximo ciclo de cobrança.

-   Para o valor adicionado isenção de IVA (imposto), você deve enviar sua ID de IVA (validado pela Microsoft) por meio de uma solicitação de serviço. Você verá as alterações e reembolsos apropriados em seu próximo ciclo de cobrança.

É possível encontrar mais detalhes de imposto do seu office imposto local ou um consultor de impostos.

## <a href="" id="licensebasedbilling"></a>Cobrança baseada em licença

Quando você comprar um produto de licença baseada em nome de um cliente, você pode escolher a ser cobrados mensalmente ou anualmente. Se você quiser alterar a frequência de cobrança em um momento posterior, use o procedimento a seguir. 

Alternar de cobrança mensal a ter cobrança anual é útil se você tiver várias assinaturas que são cobradas mensalmente e você desejar para alinhá-los em uma data de cobrança comuns. Alternar de cobrança anual para cobrança mensal é útil em adaptar suas datas de faturamento aos seus clientes individuais. 

Quando você altera a frequência de cobrança, o termo anual é atualizado para refletir que a data em que você alterou a frequência de cobrança e uma nova data de renovação são estabelecidas. 

Você pode alterar a frequência da cobrança sempre que suas necessidades comerciais mudarem. 

### <a name="billing-rules-for-annual-billing"></a>Regras de cobrança para cobrança anual

-   As assinaturas são anuais com renovação automática.

-   A cobrança é feita em 12 pagamentos mensais ou um anual por assinatura anual.

-   Você será cobrado com antecedência pelo próximo período de cobrança pelos serviços baseados em licença, de acordo com o número de licenças no final do período de cobrança anterior.

-   Você é cobrado/creditado em atraso de pagamento por alterações no número de licenças (cálculo proporcional com base em dias de licença). Cálculo proporcional usa a seguinte fórmula: [ROUND((ROUND(Preço unitário * Quantidade/Número de dias no mês proporcional, 2) * Número de dias proporcionais) / Quantidade, 2) * Quantidade]

-   Os pagamentos são cobrados pelo licenças vendidas (não licenças provisionadas).

### <a name="to-change-the-billing-frequency-of-an-online-service"></a>Para alterar a frequência de cobrança de um serviço online

1.  Selecione **clientes** no menu do Partner Center e em seguida, selecione o cliente com a assinatura que você deseja alterar. 

2.  Na página de assinaturas do cliente, selecione a assinatura que você deseja alterar. 

3.  Na página de detalhes, sob **frequência de cobrança**, selecione **mensal** ou **anual**. Você verá uma página de confirmação com informações importantes sobre como alterar a frequência da cobrança, bem como uma lista das inscrições prestes a ser alterado. 

4.  Selecione **Okey** para fazer a alteração, ou **Cancelar** desfazê-lo. 

### <a name="adjustmentscreditscancellations"></a>Ajustes/créditos/cancelamentos

Microsoft não cobra tarifas de término antecipado de cancelamento de serviços baseados em licença. 

Os créditos de cancelamento para serviços baseados em licença são proporcionais aos dias não utilizados para cancelamentos de ciclo médio (bem como pela diminuição de licenças pela fórmula acima).

## <a href="" id="usagebasedbilling"></a>Cobrança com base no uso

Alguns serviços e produtos da Microsoft usam um modelo de cobrança "pré-pago", na qual você será cobrado apenas para os serviços usados. Por exemplo, o Microsoft Azure usa esse modelo. 

### <a name="billing-rules"></a>Regras de cobrança
-   As assinaturas são o mês a mês e renovar automaticamente com as novas taxas de serviço limitado. Você será cobrado mensalmente para uso do mês anterior.

-   As taxas de serviço limitadas podem ser alteradas dentro do ciclo de fatura. 

    -   Aumentos de preço: Aviso de 30 dias é fornecido.

    -   Preço diminui: dia de alteração refletido.

    -   As assinaturas existentes usam a taxa em vigor no início do ciclo de cobrança.

    -   Novas assinaturas, quando criado no mesmo ciclo de cobrança, usam a taxa em vigor na data em que você criá-los. 

### <a name="adjustmentscreditscancellations"></a>Ajustes/créditos/cancelamentos

Você verá pagamentos com ajustes em sua próxima fatura de cobrança mensal.

Microsoft não cobra tarifas de término antecipado de cancelamento de serviços baseados em uso. 

Você verá créditos de qualquer tipo, incluindo créditos SLAs, em sua próxima fatura de cobrança mensal.

## <a href="" id="onetimebilling"></a>Cobrança de uso única

Você pode comprar assinaturas de software e reservas do Azure com antecedência, para termos de um ou três anos. Quando você adquire com antecedência, você será cobrado por todo o custo em uma quantia de um. Esse tipo de cobrança é chamado de cobrança de uso única.

>[!IMPORTANT]
>Se você comprar reservas do Azure e/ou assinaturas de software para um cliente em um local com uma moeda diferente do seu, o padrão de moeda de cobrança se baseia o local do cliente, não sua localização. Se você tiver clientes em vários locais, você recebe faturas separadas e arquivos de reconciliação para cada cliente moeda precisam ser cobrados em, permitindo que você os clientes na moeda apropriada de nota fiscal. 

### <a name="manage-your-one-time-billing"></a>Gerenciar a cobrança única

**Exibir seu status atual de cobrança, faturas e arquivos de reconhecimento**

1.  No Centro de parceiro, selecione **cobrança** e, em seguida **uma vez** para exibir seu status de cobrança. 

2.  Selecione uma fatura ou um arquivo de reconhecimento para exibir informações mais detalhadas. 

**Exibir o histórico de pedidos do cliente**

1.  Selecione **clientes** no menu do Partner Center.

2.  Na sua página **Clientes**, localize o cliente cujo histórico de pedidos você deseja exibir e, em seguida, selecione a seta para baixo para expandir o registro do cliente. 

3.  Selecione **Exibir pedidos** para exibir o histórico de pedidos.

**Baixe uma nota de crédito**

Se você precisar solicitar um crédito ou rebill, daremos uma nota de crédito para cancelar a fatura original. Você pode solicitar um crédito/rebill pelos seguintes motivos:

-   Correções de ordem de compra ou de endereço

-   A fatura foi gerada e então um reembolso de imposto foi aplicado. Você pode solicitar um crédito/nova cobrança para fazer o reembolso de imposto retroceder à fatura original. Isso também é verdadeiro para reembolsos, já que você pode solicitar um crédito/nova cobrança da fatura original e então obter um reembolso.
