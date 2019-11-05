---
title: Lista de preços do plano do Azure | Partner Center
ms.topic: article
ms.date: 11/01/2019
description: Como ver a lista de preços para assinaturas no plano do Azure
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: high
ms.openlocfilehash: 53e5327b505de1c1860e44b477aca21b5aef2d2b
ms.sourcegitcommit: 646536a113584f1572de851e22a212a6f77e64d7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/01/2019
ms.locfileid: "73428544"
---
# <a name="price-list-for-the-new-commerce-experience-in-csp-for-azure"></a>Lista de preços da nova experiência de comércio no CSP para Azure 

A lista de preços da nova experiência de comércio do Azure no CSP é publicada no Partner Center. A lista de preços é entregue dinamicamente em um arquivo preciso em tempo real e os preços são mostrados apenas em USD. No entanto, a cobrança é feita na moeda compatível, aplicável à moeda local do cliente. Para obter mais informações sobre a cobrança na moeda local do cliente, leia [Plano do Azure – cobrança](azure-plan-billing.md).

## <a name="see-pricing-for-subscriptions-under-the-azure-plan-pricing"></a>Confira os preços das assinaturas nos preços do plano do Azure

1. No menu do Partner Center, à esquerda, selecione **Vender** e, em seguida, selecione **Marketplace**.

2. Ao lado de **Tipo de exportação**, selecione **Preço de consumo do plano do Azure**.

3. Ao lado de **Preço para a data**, selecione a data desejada – por exemplo, **Atual**. Observação: você também pode selecionar **Taxas de câmbio** para exportar as taxas de câmbio atuais.

![Preços do Azure 2](images/azure/pricelist2.jpg)

4. Em **Marketplace**, selecione o **Tipo** e a **Categoria** do produto ou pesquise por um produto. Os produtos disponíveis com base na sua pesquisa são exibidos.

![pricing](images/azure/Azurepricelist1.jpg)

5. Em seguida, selecione **Exportar lista de preços do plano do Azure** para baixar os preços do plano do Azure referentes ao(s) produto(s) selecionado(s).


![exportar lista de preços](images/azure/pricelist1.png)



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
|Mercado|O mercado em que os preços são praticados|
|Currency|A moeda dos preços|
|UnitPrice|Preço por unidade|
|PricingTierRangeMin|Para preços em níveis, aplica-se o preço mínimo|
|PricingTierRangeMax|Para preços em níveis, aplica-se o preço máximo|
|EffectiveStartDate|Data de início dos preços|
|EffectiveEndDate|Data de término dos preços|
|MeterIds|ID do medidor da SKU do produto|
|MeterType|Tipo de Medidor|
|Marcas|Propriedades do item, para os preços do plano do Azure será Azure ou Azure e Reservas (para reservas, especificamente)|

Para obter [informações detalhadas sobre a lista de preços](https://partner.microsoft.com/commerce/sales?type=Any&category=Any)  
