---
title: Cenários comuns de cobrança | Partner Center
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Este tópico explica o que você deve esperar ver em sua fatura depois de adicionar novas assinaturas, ajustar o número de licenças em uma assinatura ou cancelar uma assinatura. As assinaturas baseadas em uso e em licença serão afetadas de forma diferente.
ms.assetid: E4BBD3E7-AFE2-4998-950D-0D27D1178160
author: MaggiePucciEvans
ms.author: evansma
Keywords: cobrança, pagamentos, pedidos, uso, cobrança baseada em licença, data de aniversário, termo, cancelamento, renovação, fórmula de preço, arquivo de reconciliação, arquivo reconhecimento
ms.localizationpriority: medium
ms.openlocfilehash: a4a152719f20c82ff338e6f577ea83fa9eb5e4f6
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "73653662"
---
# <a name="common-billing-scenarios"></a>Cenários comuns de cobrança

**Aplica-se a**

-   Cobrança do programa do provedor de soluções na nuvem

Este tópico explica o que você deve esperar ver em sua fatura depois de adicionar novas assinaturas, ajustar o número de licenças de uma assinatura ou cancelar uma assinatura. As assinaturas baseadas em uso e em licença são afetadas de forma diferente.

## <a name="in-this-section"></a>Nesta seção

-   [Cobrança baseada em uso](#usagebased)

-   [Cobrança baseada em licença](#licensebased)

## <a href="" id="usagebased"></a>Cobrança baseada em uso

As assinaturas baseadas em uso são cobradas mensalmente, em atrasos de pagamento, no dia do aniversário da assinatura. Por exemplo, se a data de aniversário da assinatura for a 15, você será cobrado em 15 de Janeiro para o período de serviço de 15 de dezembro de 14 de Janeiro. Você será cobrado novamente em 15 de fevereiro para o período de serviço de 15 de janeiro de 14 de fevereiro, etc. Os encargos gerados no dia de aniversário da assinatura serão exibidos na nota fiscal e no arquivo de reconciliação a seguir.

Ocasionalmente, você pode observar que alguns encargos de uso estão ausentes de sua fatura ou que o uso de um mês anterior é cobrado na fatura do mês atual. Isso não é um erro; Isso simplesmente significa que o serviço estava com carimbo de data/hora depois que os serviços ocorreram. O uso relatado dentro de 24 horas do final do ciclo de cobrança será exibido na fatura do próximo mês. 

As assinaturas baseadas em uso podem ser suspensas a qualquer momento. 

A Lista de Preços do Azure CSP é publicada mensalmente e pode ser encontrada na página Vender -> Preço e Ofertas do Partner Center. Observe que os preços podem mudar diariamente e se refletem na guia Alterar Histórico da Lista de Preços.

Os encargos de uso se baseiam em preços diários. Se o preço mudar durante o termo de serviço, você verá uma linha de cobrança para cada termo de serviço proporcional e o preço aplicável.

## <a href="" id="licensebased"></a>Cobrança baseada em licença

**Cobrança:** assinaturas baseadas em licença são cobradas antecipadamente no dia de aniversário de assinatura.

**Dia do Aniversário:** o dia do aniversário é o dia do mês em que você comprou a assinatura. Por exemplo, se você tiver comprado a assinatura em 15 de janeiro, o dia do aniversário será o 15º de cada mês.

**termo:** todas as assinaturas baseadas em licença têm um termo pago de 12 meses, que começa na data da compra.

**Cancelamento:** as assinaturas suspensas no mês 1 serão totalmente creditadas. As assinaturas suspensas nos meses 2 a 12 serão creditadas proporcionalmente.

**Renovação:** todas as assinaturas baseadas em licença serão renovadas automaticamente 12 meses após o período pago começar.

## <a href="" id="licensebasedmonthly"></a>Cenários de cobrança mensal

**Cenário 1: nova assinatura**

Sua data de cobrança é no 15º dia de cada mês. Em 13 de janeiro, você compra uma nova assinatura com uma licença por US$4/mês e seleciona a cobrança mensal. Em 15 de janeiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantity |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/01/2018         |12/02/2018    |Taxa do Ciclo   |4,00       |1        |4,00    

Em 15 de fevereiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantity |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/02/2018         |12/03/2018    |Taxa do Ciclo   |4,00       |1        |4,00    

**Cenário 2: alterar a quantidade de licenças**

Sua data de cobrança é no 15º dia de cada mês. Em 13 de janeiro, você compra uma nova assinatura com uma licença por US$4/mês e seleciona a cobrança mensal. Em 15 de janeiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantity |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/01/2018         |12/02/2018    |Taxa do Ciclo   |4,00       |1        |4,00    

Em 1º de fevereiro, você aumentará sua quantidade de licença de uma para duas. Em 15 de fevereiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantity |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 13/01/2018        |12/02/2018    |Proporcional à Instância do Ciclo   |-4,00       |1        |-4,00    
|13/01/2018         |31/01/2018    | Proporcional à Instância do Ciclo   |2,45       |1        |2,45    
|01/02/2018         |12/02/2018    | Proporcional à Instância do Ciclo   |1,55       |2        |3,10    
|13/02/2018         |12/03/2018    | Proporcional à Instância do Ciclo   |4,00       |2        |8,00    

**Fórmulas de preço unitário:**

O preço mensal é 4, 0 e há 31 dias no período de serviço 1/13/2018-2/12/2018. Isso equivale a um preço diário de 0,129 (4/31).

Há 19 dias no período de proporção de 1/13/2018-1/31/2018.

Preço unitário proporcional = 2,451 = 19 x 0,129

Há 12 dias no período de proporção de 2/1/2018-2/12/2018.

Preço unitário proporcional = 1,54 = 12 x 0,129

**Cenário 3: suspender antes de 30 dias**

Sua data de cobrança é no 15º dia de cada mês. Em 13 de janeiro, você compra uma nova assinatura com uma licença por US$4/mês e seleciona a cobrança mensal. Em 15 de janeiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantity |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/01/2018         |12/02/2018    |Taxa do Ciclo   |4,00       |1        |4,00    

Em 1º de fevereiro você suspende uma assinatura. Em 15 de fevereiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantity |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/02/2018|Taxa de cancelamento|-4,00|1|-4,00

**Cenário 4: suspender após 30 dias**

Sua data de cobrança é no 15º dia de cada mês. Em 13 de janeiro, você compra uma nova assinatura com uma licença por US$4/mês e seleciona a cobrança mensal. Em 15 de janeiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantity |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/02/2018|Taxa do Ciclo|4,00|1|4,00

Em 15 de fevereiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantity |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/02/2018|12/03/2018|Taxa do Ciclo|4,00|1|4,00

Em 1º de março, você suspende a assinatura. Em 15 de março, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantity |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
01/03/2018|12/03/2018|Taxa de cancelamento|-1,72|1|-1,72

**Fórmulas de preço unitário:**

O preço mensal é 4, 0 e há 28 dias no período de serviço 2/13/2018-3/12/2018. Isso equivale a um preço diário de 0,143 (4/28).

Preço unitário = dias no termo de serviço x preço diário x número de licenças.

Há 12 dias no período de cancelamento 3/1/2018-3/12/2018. 

Portanto, o preço unitário =-1,716 (12 x 0,143 x (-1)).

## <a name="annual-billing-scenarios"></a>Cenários de Cobrança Anual

**Cenário 1: nova assinatura**

Sua data de cobrança é no 15º dia de cada mês. Em 13 de janeiro, você compra uma nova assinatura com uma licença por US$4/mês e seleciona a cobrança anual. Em 15 de janeiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantity |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Taxas proporcionais na compra|48,00|1|48,00

**Cenário 2: adicionar licença após a data de aniversário da assinatura, mas antes da data de cobrança**

Você compra uma nova assinatura dia 11/02/17 com uma licença por US$ 211,20/ano. O aniversário da sua assinatura é definido como o dia 11 de cada mês. O sistema de cobrança da Microsoft cria as seguintes linhas de cobrança: 

-   $211.20 encargo para o período 2/11/17-2/10/18. 

Em 12/02/17, você compra uma segunda licença. Sua data de cobrança é 14/02/17. Os arquivos de fatura e reconciliação são gerados. O arquivo de reconciliação conterá as seguintes linhas de cobrança: 

|Data de Início da Cobrança  |Data de Término da Cobrança  |Tipo de Cobrança  |Preço unitário |Quantity | Valor |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11/02/2017 |10/02/2018 |Taxas proporcionais na compra |211,20 |1 | 211,20 |

No aniversário da sua assinatura, 11/03/17, o sistema de cobrança da Microsoft cria as seguintes linhas de cobrança para o aumento de licença em 12/02/17: 
-   -$211.20 crédito para o período 2/11/17-2/10/18. 
-   $0.58 cobrança rateada por licença para 1 licença para o período 2/11/17-2/11/17. 
-   $15.62 cobrança rateada por licença para 2 licenças para o período 2/12/17-3/10/2017. 
-   $195 cobrança rateada por licença para 2 licenças para o período 3/11/2017-2/10/2018. 

Em 11/02/17, você compra um assinatura. Em 12/02/17, você adiciona uma licença. Sua data de cobrança é 14/02/17. Em 11/02/18, sua assinatura é renovada.

A próxima data de cobrança é 14/03/17, e os arquivos de fatura e reconciliação são gerados. O arquivo de reconciliação conterá as seguintes linhas de cobrança: 

|Data de Início da Cobrança  |Data de Término da Cobrança  |Tipo de Cobrança  |Preço unitário |Quantity | Valor |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11/02/2017 |10/02/2018 |Proporcional à Instância do Ciclo |-211,20 |1 |-211,20 |
|11/02/2017 |11/02/2017 |Proporcional à Instância do Ciclo |0,58 |1 |0,58 |
|12/02/2017 |10/03/2017 |Proporcional à Instância do Ciclo |15,62 |2 |31,25 |
|11/03/2017 |10/02/2018 |Proporcional à Instância do Ciclo |195,00 |2 |390,00 |

Em 11/02/18, a assinatura será renovada por outro período de 12 meses.


**Cenário 3: alterar a quantidade de licenças**

Sua data de cobrança é no 15º dia de cada mês. Em 13 de janeiro, você compra uma nova assinatura com uma licença por US$4/mês e seleciona a cobrança anual. Em 15 de janeiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantity |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Taxas proporcionais na compra|48,00|1|48,00

Em 1º de fevereiro, você aumentará sua quantidade de licença de uma para duas. Em 15 de fevereiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantity |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  | 
13/01/2018|12/01/2019|Proporcional à Instância do Ciclo|-48,00|1|-48,00
13/01/2018|31/01/2018|Proporcional à Instância do Ciclo|2,47|1|2,47
01/02/2018|12/01/2019|Proporcional à Instância do Ciclo|44,98|2|89,96

**Fórmulas de preço unitário:**

O preço anual é 48,00, que equivale ao preço diário de 0,13 (48,00/365).

Preço unitário = dias no termo de serviço x preço diário x número de licenças.

Há 19 dias no período de serviço 1/13/2018-1/31/2018. 

Portanto, o preço unitário = 2,47 (19 x 0,13 x 1)

Há 346 dias no período de serviço 2/1/2018-1/12/2019. 

Portanto, o preço unitário = 44,98 (346 x 0,13 x 2)

**Cenário 4: suspender antes de 30 dias**

Sua data de cobrança é no 15º dia de cada mês. Em 13 de janeiro, você compra uma nova assinatura com uma licença por US$4/mês e seleciona a cobrança anual. Em 15 de janeiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantity |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Taxas proporcionais na compra|48,00|1|48,00

Em 1º de fevereiro, você suspende sua assinatura. Em 15 de fevereiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantity |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Taxa de cancelamento|-48,00|1|-48,00

**Cenário 5: suspender após 30 dias**

Sua data de cobrança é no 15º dia de cada mês. Em 13 de janeiro, você compra uma nova assinatura com uma licença por US$4/mês e seleciona a cobrança anual. Em 15 de janeiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantity |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Taxas proporcionais na compra|48,00|1|48,00

Em 15 de fevereiro, o arquivo de reconciliação baseado em licenças não conterá nenhuma linha de cobrança para essa assinatura.
Em 1º de março, você suspende sua assinatura. Em 15 de março, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantity |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
01/03/2018|12/01/2019|Taxa de cancelamento|-41,34|1|-41,34

**Fórmulas de preço unitário:**

O preço anual é 48,00, que equivale ao preço diário de 0,13 (48,00/365).

Preço unitário = dias no termo de serviço x preço diário x número de licenças.

Há 318 dias no período de serviço 3/1/2018-1/12/2019. 

Portanto, o preço unitário = 41,34 (318 x 0,13 x 1). Como isso é um crédito, o preço unitário é de -41,34.

**Cenário 6: suspender e reativar**

Sua data de cobrança é no 15º dia de cada mês. Em 13 de janeiro, você compra uma nova assinatura com uma licença por US$4/mês e seleciona a cobrança anual. Em 15 de janeiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantity |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Taxas proporcionais na compra|48,00|1|48,00

Em 1º de fevereiro, você suspende sua assinatura. Em 15 de fevereiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantity |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Taxa de cancelamento|-48,00|1|-48,00

Em 1º de março, você reativa sua assinatura. Em 15 de março, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantity |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
01/03/2018|12/01/2019|Taxas proporcionais na compra|41,34|1|41,34

**Fórmulas de preço unitário:**

O preço anual é 48,00, que equivale ao preço diário de 0,13 (48,00/365).

Preço unitário = dias no termo de serviço x preço diário x número de licenças.

Há 318 dias no período de serviço 3/1/2018-1/12/2019. 

Portanto, o preço unitário = 41,34 (318 x 0,13 x 1).
