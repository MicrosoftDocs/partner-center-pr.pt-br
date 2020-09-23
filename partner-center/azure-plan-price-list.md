---
title: Lista de preços do plano do Azure para parceiros CSP
ms.topic: how-to
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como os parceiros do programa CSP podem usar o Partner Center para consultar a lista de preços para assinaturas no plano do Azure.
author: brentserbus
ms.author: brserbus
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 57e976f2968f0bd6b13f36eb04be9f68577d1389
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000320"
---
# <a name="price-list-for-the-new-commerce-experience-in-csp-for-azure"></a>Lista de preços da nova experiência de comércio no CSP para Azure

**Funções apropriadas**

- Agente administrativo
- Administrador de cobrança
- Administrador global
- Agente de suporte técnico
- Agente de vendas
- Administrador de gerenciamento de usuário

A lista de preços da nova experiência de comércio do Azure no CSP é publicada no Partner Center. A lista de preços é entregue dinamicamente em um arquivo preciso em tempo real e os preços são mostrados apenas em USD. No entanto, a cobrança é feita na moeda compatível, aplicável à moeda local do cliente. Para obter mais informações sobre a cobrança na moeda local do cliente, leia [Plano do Azure – cobrança](azure-plan-billing.md).

## <a name="see-pricing-for-subscriptions-under-the-azure-plan-pricing"></a>Confira os preços das assinaturas nos preços do plano do Azure

1. No menu do Partner Center, à esquerda, selecione **Vender** e, em seguida, selecione **Marketplace**.

2. Em preços do plano do Azure, selecione o país para o qual você deseja obter preços.

3. Ao lado de **Tipo de exportação**, selecione **Preço de consumo do plano do Azure**, **Preços de reservas do plano do Azure** ou **Taxas de câmbio**. 

>[!NOTE] 
>As **Taxas de câmbio** não são específicas do país.

4. Ao lado de **Preço para a data**, selecione a data desejada – por exemplo, **Atual**.

   :::image type="content" source="images/azure/pricingnew.png" alt-text="específico do país":::

>[!NOTE] 
>Você pode exportar duas listas de preços diferentes: Preços do plano do Azure e Preços de terceiros do Marketplace.

## <a name="azure-price-list-specifics"></a>Especificações da lista de preços do Azure

- Os preços do plano do Azure estarão disponíveis na página do Marketplace, no Partner Center, em **Vender**.

- As exportações estarão disponíveis para os serviços de consumo do plano do Azure, as reservas do Azure e as taxas de câmbio.

- As opções de exportação incluem:

  - **Preços de hoje**: inclui todos os medidores e preços do 1º dia do mês até a data atual do mês atual. Isso inclui preços novos, alterados ou removidos. Todos os preços terão datas de início e término de vigência para explicar se são novos ou removidos.

  - **Preços do mês anterior**: os downloads de cada tipo de recurso serão feitos por mês. Para arquivos de preço, isso incluirá todos os medidores disponíveis durante aquele mês. Se um novo medidor aparecer no meio do mês, será exibido como um medidor com uma data de início de vigência que reflete sua disponibilidade. Semelhante aos preços descontinuados, mostrados com uma data de término de vigência que indica quando não estão mais disponíveis.

  - **Taxas de câmbio**: as taxas de câmbio estarão disponíveis para download no dia anterior ao 1º dia do mês, às 18:00 PST. Por exemplo, se você quiser as taxas de novembro, baixe as taxas no dia 31 de outubro. As taxas de câmbio do mês anterior também estarão disponíveis.

- Os preços das listas de preços são diretos. Alguns parceiros podem estar qualificados para receber o crédito ganho pelo parceiro. Para obter informações sobre como o crédito ganho pelo parceiro é calculado, leia [Como o crédito ganho pelo parceiro é calculado e pago](partner-earned-credit-explanation.md).

- **Serviços qualificados**: O crédito ganho pelo parceiro é aplicável aos serviços listados nos **preços de consumo do plano do Azure**, que os parceiros podem exportar da página de [preços do plano do Azure](https://partner.microsoft.com/commerce/sales). Observe que há exceções que incluem, mas não se limitam a, produtos de terceiros identificados como "De Terceiros" na coluna Marcas da lista de preços de consumo do plano do Azure, reservas do plano do Azure.

## <a name="price-list-data"></a>Dados da lista de preços

|**Campo**   |**Descrição**   |
|--------------------------|:---------------------------|
|ProductTitle  |Título ou nome do produto|
|ProductID   |ID do produto|
|SKuId|ID da SKU|
|SkuTitle|Título ou nome da SKU|
|Editor|A primeira parte será sempre a Microsoft|
|SkuDescription|Descrição da SKU|
|UnitOfMeasure|As unidades que serão cobradas ou faturadas|
|TermDuration|Para produtos baseados em prazos, é a duração do prazo, aplicável às reservas|
|Market|O mercado em que os preços são praticados|
|Currency|A moeda dos preços|
|UnitPrice|Preço por unidade|
|PricingTierRangeMin|Para preços em níveis, aplica-se o preço mínimo|
|PricingTierRangeMax|Para preços em níveis, aplica-se o preço máximo|
|EffectiveStartDate|Data de início dos preços|
|EffectiveEndDate|Data de término dos preços|
|MeterIds|ID do medidor da SKU do produto|
|MeterType|Tipo de Medidor|
|Marcas|Propriedades do item, para os preços do plano do Azure será Azure ou Azure e Reservas (para reservas, especificamente)|

As listas de preços de plano do Azure podem ser exportadas da [página Preços e ofertas](https://partner.microsoft.com/dashboard/sell/pricingandoffers) no Partner Center.

## <a name="tiered-pricing"></a>Preços em camadas

Alguns serviços de consumo do plano do Azure são compatíveis com preços em camadas. Os parceiros podem encontrar esses produtos e SKUs na lista de preços do plano do Azure. Os itens que têm valores nas colunas de intervalo de tipo de preço permitem que os parceiros compreendam o preço com base no uso. No exemplo abaixo, usando dados de amostra, temos um SKU de produto com três tipos de preço.

|**ProductId**   |**SkuId**   |**UnitPrice**   |**PricingTierRangeMin**   |**PricingTierRangeMax**   |
|:---------------|:-----------|:---------------|:-------------------------|:-------------------------|
|DDD123456ABC|01AB|0,50|100001|9223372036854780000|
|DDD123456ABC|01AB|0,80|101|100000|
|DDD123456ABC|01AB|1|1|100|

Neste exemplo, se 101 unidades forem usadas, a cobrança será 100,80. As primeiras 100 unidades são consideradas unitárias e a próxima unidade é cobrada a 0,80.

## <a name="pricing-api-for-azure-plan"></a>API de preço do plano do Azure

Você pode usar a [API de preço](/partner/develop/pricing) para recuperar o preço do plano do Azure para consumo e reservas de forma programática. Você também pode recuperar taxas de câmbio de moeda estrangeira.

A API de preço está em um ponto de extremidade diferente daquele das outras APIs do Partner Center. As informações de preço incluem preços de medidores em USD para recursos do plano do Azure e preços de reservas aplicados às assinaturas do plano do Azure.

Essa API também permite que os parceiros recuperem taxas de câmbio mensais porque o preço do plano do Azure está apenas em USD. Você pode usar as APIs para recuperar o preço e as taxas de câmbio de moeda estrangeira do mês atual ou dos meses anteriores.

>[!NOTE]
> A API de preço é específica para os preços do plano do Azure. Você ainda deve usar a API RateCard existente e as listas de preços publicadas na página "Preços e ofertas" do Partner Center para recursos do Azure ou reservas implantados em assinaturas de planos que não são do Azure. A API de preços do plano do Azure não é compatível com preços baseados em software, marketplace ou licença, como no Microsoft 365 ou no Dynamics 365.

Para obter mais informações sobre as APIs de preço do plano do Azure e da taxa de câmbio de moeda estrangeira, confira a [documentação completa da API de preços](/partner/develop/pricing).