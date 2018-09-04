---
title: Cenários comuns de cobrança | Partner Center
description: Este tópico explica o que você deve esperar ver em sua fatura depois de adicionar novas assinaturas, ajustar o número de licenças em uma assinatura ou cancelar uma assinatura. As assinaturas baseadas em uso e em licença serão afetadas de forma diferente.
ms.assetid: E4BBD3E7-AFE2-4998-950D-0D27D1178160
author: MaggiePucciEvans
Keywords: billing, payments, orders, usage, license-based billing, anniversary date, term, cancellation, renewal, price formula,reconciliation file, recon file
ms.localizationpriority: medium
ms.openlocfilehash: ff329480cec68e45c809016da64f6604c9837bb6
ms.sourcegitcommit: 92629114d5081103bfe555081f69997af4ed56f2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2018
ms.locfileid: "2876586"
---
# <a name="common-billing-scenarios"></a>Cenários comuns de cobrança

**Aplicável a**

-  Partner Center
-  Partner Center for Microsoft Cloud for US Government
-  Partner Center do Microsoft Cloud Alemanha

Este tópico explica o que você deve esperar ver em sua fatura depois de adicionar novas assinaturas, ajustar o número de licenças de uma assinatura ou cancelar uma assinatura. As assinaturas baseadas em uso e em licença são afetadas de forma diferente.

## <a name="in-this-section"></a>Nesta seção

-   [Cobrança baseada em uso](#usagebased)

-   [Cobrança baseada em licença](#licensebased)

## <a href="" id="usagebased"></a>Cobrança baseada em uso

As assinaturas baseadas em uso são cobradas mensalmente, em atrasos de pagamento, no dia do aniversário da assinatura. Por exemplo, se a data de aniversário da assinatura for o dia 15, você será cobrado em 15 de janeiro pelo termo de serviço entre 15 de dezembro e 14 de janeiro. Você será cobrado em 15 de fevereiro pelo termo de serviço entre 15 de janeiro e 14 de fevereiro etc. Os encargos gerados no dia do aniversário da assinatura serão exibidos no arquivo de reconciliação e na fatura a seguir.

As assinaturas baseadas em uso podem ser suspensas a qualquer momento. 

A Lista de Preços do Azure CSP é publicada mensalmente e pode ser encontrada na página Vender -> Preço e Ofertas do Partner Center. Observe que os preços podem mudar diariamente e se refletem na guia Alterar Histórico da Lista de Preços.

Os encargos de uso se baseiam em preços diários. Se o preço mudar durante o termo de serviço, você verá uma linha de cobrança para cada termo de serviço proporcional e o preço aplicável.

## <a href="" id="licensebased"></a>Cobrança baseada em licença

**Cobrança:** assinaturas baseadas em licença são cobradas antecipadamente no dia de aniversário de assinatura.

**Dia do Aniversário:** o dia do aniversário é o dia do mês em que você comprou a assinatura. Por exemplo, se você tiver comprado a assinatura em 15 de janeiro, o dia do aniversário será o 15º de cada mês.

**termo:** todas as assinaturas baseadas em licença têm um termo pago de 12 meses, que começa na data da compra.

**Cancelamento:** as assinaturas suspensas no mês 1 serão totalmente creditadas. As assinaturas suspensas nos meses 2 a 12 serão creditadas proporcionalmente.

**Renovação:** todas as assinaturas baseadas em licença serão renovadas automaticamente 12 meses após o período pago começar.

## <a href="" id="licensebasedmonthly"></a>Cenários de cobrança mensais

**Cenário 1: Nova assinatura**

Sua data de cobrança é no 15º dia de cada mês. Em 13 de janeiro, você compra uma nova assinatura com uma licença por US$4/mês e seleciona a cobrança mensal. Em 15 de janeiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/01/2018         |12/02/2018    |Taxa do Ciclo   |4,00       |1        |4,00    

Em 15 de fevereiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/02/2018         |12/03/2018    |Taxa do Ciclo   |4,00       |1        |4,00    

**Cenário 2: Alterar a quantidade de licenças**

Sua data de cobrança é no 15º dia de cada mês. Em 13 de janeiro, você compra uma nova assinatura com uma licença por US$4/mês e seleciona a cobrança mensal. Em 15 de janeiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/01/2018         |12/02/2018    |Taxa do Ciclo   |4,00       |1        |4,00    

Em 1º de fevereiro, você aumentará sua quantidade de licença de uma para duas. Em 15 de fevereiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 13/01/2018        |12/02/2018    |Proporcional à Instância do Ciclo   |-4,00       |1        |4,00    
|13/01/2018         |31/01/2018    | Proporcional à Instância do Ciclo   |2,45       |1        |2,45    
|01/02/2018         |12/02/2018    | Proporcional à Instância do Ciclo   |1,55       |2        |3,10    
|13/02/2018         |12/03/2018    | Proporcional à Instância do Ciclo   |4,00       |2        |8,00    

**Fórmulas do Preço Unitário:**

O preço mensal é de 4,00 e há 31 dias no termo de serviço: 13/01/2018 a 12/02/2018. Isso equivale a um preço diário de 0,129 (4/31).

Há 19 dias no termo proporcional de 13/01/2018 a 31/01/2018.

Preço unitário proporcional = 2,451 = 19 x 0,129

Há 12 dias no termo proporcional de 01/02/2018 a 12/02/2018.

Preço unitário proporcional = 1,54 = 12 x 0,129

**Cenário 3: Suspender antes de 30 dias**

Sua data de cobrança é no 15º dia de cada mês. Em 13 de janeiro, você compra uma nova assinatura com uma licença por US$4/mês e seleciona a cobrança mensal. Em 15 de janeiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/01/2018         |12/02/2018    |Taxa do Ciclo   |4,00       |1        |4,00    

Em 1º de fevereiro, você suspende a assinatura. Em 15 de fevereiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/02/2018|Taxa de cancelamento|-4,00|1|4,00

**Cenário 4: Suspender depois de 30 dias**

Sua data de cobrança é no 15º dia de cada mês. Em 13 de janeiro, você compra uma nova assinatura com uma licença por US$4/mês e seleciona a cobrança mensal. Em 15 de janeiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/02/2018|Taxa do Ciclo|4,00|1|4,00

Em 15 de fevereiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/02/2018|12/03/2018|Taxa do Ciclo|4,00|1|4,00

Em 1º de março, você suspende a assinatura. Em 15 de março, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
01/03/2018|12/03/2018|Taxa de cancelamento|-1,72|1|-1,72

**Fórmulas do Preço Unitário:**

O preço mensal é de 4,00 e há 28 dias no termo de serviço: 13/02/2018 a 12/03/2018. Isso equivale a um preço diário de 0,143 (4/28).

Preço unitário = dias no termo de serviço x preço diário x número de licenças.

Há 12 dias no termo de cancelamento de 01/03/2018 a 12/03/2018. 

Portanto, o preço unitário =-1,716 (14 x 0,14 x(-1)).

## <a name="annual-billing-scenarios"></a>Cenários de Cobrança Anual

**Cenário 1: Nova assinatura**

Sua data de cobrança é no 15º dia de cada mês. Em 13 de janeiro, você compra uma nova assinatura com uma licença por US$4/mês e seleciona a cobrança anual. Em 15 de janeiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Taxas proporcionais durante a compra|48,00|1|48,00

**Cenário 2: adicionar uma licença após a data de aniversário da assinatura, mas antes da data de cobrança**

Você compra uma nova assinatura dia 11/02/17 com uma licença por US$211,20/ano. O aniversário da sua assinatura é definido como o dia 11 de cada mês. O sistema de cobrança da Microsoft cria as seguintes linhas de cobrança: 

-   Cobrança de US$211,20 pelo período de 11/02/17 a 10/02/18. 

Em 12/02/17, você compra uma segunda licença. Sua data de cobrança é 14/02/17. Os arquivos de fatura e reconciliação são gerados. O arquivo de reconciliação conterá as seguintes linhas de cobrança: 
|Data de Início da Cobrança  |Data de Término da Cobrança  |Tipo de Cobrança  |Preço unitário |Quantidade | Valor |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11/02/2017 |10/02/2018 |Taxas proporcionais na compra |211,20 |1 | 211,20 |
 
No aniversário da sua assinatura, 11/03/17, o sistema de cobrança da Microsoft cria as seguintes linhas de cobrança para o aumento de licença em 12/02/17: 
-   Crédito de -US$211,20 pelo período de 11/02/17 a 10/02/18. 
-   Cobrança proporcional por licença de US$0,58 por 1 licença pelo período de 11/02/17 a 11/02/17. 
-   Cobrança proporcional por licença de US$15,62 por 2 licenças pelo período de 12/02/17 a 10/03/17. 
-   Cobrança proporcional por licença de US$195,00 por 2 licenças pelo período de 11/03/2017 a 10/02/2018. 
 
Em 11/02/17, você compra um assinatura. Em 12/02/17, você adiciona uma licença. Sua data de cobrança é 14/02/17. Em 11/02/18, sua assinatura é renovada.

A próxima data de cobrança é 14/03/17, e os arquivos de fatura e reconciliação são gerados. O arquivo de reconciliação conterá as seguintes linhas de cobrança: 
|Data de Início da Cobrança  |Data de Término da Cobrança  |Tipo de Cobrança  |Preço unitário |Quantidade | Valor |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11/02/2017 |10/02/2018 |Proporcional à instância do ciclo |-211,20 |1 |-211,20 |
|11/02/2017 |11/02/2017 |Proporcional à instância do ciclo |0,58 |1 |0,58 |
|12/02/2017 |10/03/2017 |Proporcional à instância do ciclo |15,62 |2 |31,25 |
|11/03/2017 |10/02/2018 |Proporcional à instância do ciclo |195,00 |2 |390,00 |
 
Em 11/02/18, a assinatura será renovada por outro período de 12 meses.


**Cenário 3: Alterar a quantidade de licença**

Sua data de cobrança é no 15º dia de cada mês. Em 13 de janeiro, você compra uma nova assinatura com uma licença por US$4/mês e seleciona a cobrança anual. Em 15 de janeiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Taxas proporcionais durante a compra|48,00|1|48,00

Em 1º de fevereiro, você aumentará sua quantidade de licença de uma para duas. Em 15 de fevereiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  | 
13/01/2018|12/01/2019|Proporcional à instância do ciclo|-48,00|1|-48,00
13/01/2018|31/01/2018|Proporcional à instância do ciclo|2,47|1|2,47
01/02/2018|12/01/2019|Proporcional à instância do ciclo|44,98|2|89,96

**Fórmulas do Preço Unitário:**

O preço anual é 48,00, que equivale ao preço diário de 0,13 (48,00/365).

Preço unitário = dias no período de serviço x preço diário x número de licenças.

Há dias 19 no período de serviço de 13/01/2018 – 31/01/2018. 

Portanto, o preço unitário = 2,47 (19 x 0,13 x 1)

Há dias 346 no período de serviço de 01/02/2018 – 12/01/2019. 

Portanto, o preço unitário = 44,98 (346 x 0,13 x 2)

**Cenário 4: Suspender antes de 30 dias**

Sua data de cobrança é no 15º dia de cada mês. Em 13 de janeiro, você compra uma nova assinatura com uma licença por US$4/mês e seleciona a cobrança anual. Em 15 de janeiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Taxas proporcionais durante a compra|48,00|1|48,00

Em 1º de fevereiro, você suspende sua assinatura. Em 15 de fevereiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Taxa de cancelamento|-48,00|1|-48,00

**Cenário 5: Suspender depois de 30 dias**

Sua data de cobrança é no 15º dia de cada mês. Em 13 de janeiro, você compra uma nova assinatura com uma licença por US$4/mês e seleciona a cobrança anual. Em 15 de janeiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Taxas proporcionais durante a compra|48,00|1|48,00

Em 15 de fevereiro, o arquivo de reconciliação baseado em licenças não conterá nenhuma linha de cobrança para essa assinatura.
Em 1º de março, você suspende sua assinatura. Em 15 de março, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
01/03/2018|12/01/2019|Taxa de cancelamento|-41,34|1|-41,34

**Fórmulas do Preço Unitário:**

O preço anual é 48,00, que equivale ao preço diário de 0,13 (48,00/365).

Preço unitário = dias no período de serviço x preço diário x número de licenças.

Há dias 318 no período de serviço de 01/03/2018 – 12/01/2019. 

Portanto, o preço unitário = 41,34 (318 x 0,13 x 1). Como isso é um crédito, o preço unitário é de -41,34.

**Cenário 6: Suspender e reativar**

Sua data de cobrança é no 15º dia de cada mês. Em 13 de janeiro, você compra uma nova assinatura com uma licença por US$4/mês e seleciona a cobrança anual. Em 15 de janeiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Taxas proporcionais durante a compra|48,00|1|48,00

Em 1º de fevereiro, você suspende sua assinatura. Em 15 de fevereiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Taxa de cancelamento|-48,00|1|-48,00

Em 1º de março, você reativa sua assinatura. Em 15 de março, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
01/03/2018|12/01/2019|Taxas proporcionais durante a compra|41,34|1|41,34

**Fórmulas do Preço Unitário:**

O preço anual é 48,00, que equivale ao preço diário de 0,13 (48,00/365).

Preço unitário = dias no período de serviço x preço diário x número de licenças.

Há dias 318 no período de serviço de 01/03/2018 – 12/01/2019. 

Portanto, o preço unitário = 41,34 (318 x 0,13 x 1).
