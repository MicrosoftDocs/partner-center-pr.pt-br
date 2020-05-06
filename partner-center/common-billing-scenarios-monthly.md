---
title: Cenários comuns de cobrança mensal | Centro de parceiros
ms.topic: article
ms.date: 11/25/2019
description: Cenários comuns no Partner Center quando você usa a cobrança mensal (como adicionar novas assinaturas, alterar a quantidade de licenças e suspender assinaturas).
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
Keywords: cobrança, pagamentos, pedidos, uso, cobrança mensal, assinaturas, arquivo de reconciliação
ms.localizationpriority: medium
ms.openlocfilehash: e67281a0bf7d5649a68a6a3f3c27c40e3666eb14
ms.sourcegitcommit: faf7b1ac1653497f963b428bbfafcd821378adaa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2020
ms.locfileid: "82798534"
---
# <a name="monthly-billing-scenarios"></a>Cenários de cobrança mensais

**Funções apropriadas**

- Agente administrativo
- Administrador de cobrança
- Agente de suporte técnico
- Agente de vendas

Esses [cenários de cobrança comuns](common-billing-scenarios.md) de exemplo são aplicáveis se você usar a cobrança mensal no Partner Center.

## <a name="new-monthly-subscription"></a>Nova assinatura mensal

Sua data de cobrança é no 15º dia de cada mês. Em 13 de janeiro, você compra uma nova assinatura com uma licença por US$4/mês e seleciona a cobrança mensal. Em 15 de janeiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço Unitário |Quantidade |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/01/2018         |12/02/2018    |Taxa do Ciclo   |4,00       |1        |4,00 |

Em 15 de fevereiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço Unitário |Quantidade |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/02/2018         |12/03/2018    |Taxa do Ciclo   |4,00       |1        |4,00 |

## <a name="change-license-quantity"></a>Alterar quantidade de licenças

Sua data de cobrança é no 15º dia de cada mês. Em 13 de janeiro, você compra uma nova assinatura com uma licença por US$4/mês e seleciona a cobrança mensal. Em 15 de janeiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço Unitário |Quantidade |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/01/2018         |12/02/2018    |Taxa do Ciclo   |4,00       |1        |4,00    |

Em 1º de fevereiro, você aumentará sua quantidade de licença de uma para duas. Em 15 de fevereiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço Unitário |Quantidade |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 13/01/2018        |12/02/2018    |Proporcional à Instância do Ciclo   |-4,00       |1        |-4,00   |
|13/01/2018         |31/01/2018    | Proporcional à Instância do Ciclo   |2.45       |1        |2.45    |
|1/02/2018         |12/02/2018    | Proporcional à Instância do Ciclo   |1.55       |2        |3,10    |
|13/02/2018         |12/03/2018    | Proporcional à Instância do Ciclo   |4,00       |2        |8,00    |

O preço mensal é de 4,00 e há 31 dias no termo de serviço: 13/01/2018 a 12/02/2018. Isso equivale a um preço diário de 0,129 (4/31).

Há 19 dias no termo proporcional de 13/01/2018 a 31/01/2018.

Preço unitário proporcional = 2,451 = 19 x 0,129

Há 12 dias no termo proporcional de 01/02/2018 a 12/02/2018.

Preço unitário proporcional = 1,54 = 12 x 0,129

## <a name="suspend-before-30-days"></a>Suspender antes de 30 dias

Sua data de cobrança é no 15º dia de cada mês. Em 13 de janeiro, você compra uma nova assinatura com uma licença por US$4/mês e seleciona a cobrança mensal. Em 15 de janeiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço Unitário |Quantidade |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/01/2018         |12/02/2018    |Taxa do Ciclo   |4,00       |1        |4,00    |

Em 1º de fevereiro você suspende uma assinatura. Em 15 de fevereiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço Unitário |Quantidade |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/02/2018|Taxa de cancelamento|-4,00|1|-4,00

## <a name="suspend-after-30-days"></a>Suspender após 30 dias

Sua data de cobrança é no 15º dia de cada mês. Em 13 de janeiro, você compra uma nova assinatura com uma licença por US$4/mês e seleciona a cobrança mensal. Em 15 de janeiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço Unitário |Quantidade |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/02/2018|Taxa do Ciclo|4,00|1|4,00

Em 15 de fevereiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço Unitário |Quantidade |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/02/2018|12/03/2018|Taxa do Ciclo|4,00|1|4,00

Em 1º de março, você suspende a assinatura. Em 15 de março, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço Unitário |Quantidade |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
01/03/2018|12/03/2018|Taxa de cancelamento|-1,72|1|-1,72

O preço mensal é de 4,00 e há 28 dias no termo de serviço: 13/02/2018 a 12/03/2018. Isso equivale a um preço diário de 0,143 (4/28).

Preço unitário = dias no termo de serviço x preço diário x número de licenças.

Há 12 dias no termo de cancelamento de 01/03/2018 a 12/03/2018.

Portanto, o preço unitário =-1,716 (12 x 0,143 x (-1)).
