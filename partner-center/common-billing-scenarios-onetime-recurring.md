---
title: Cobrança de compras & recorrentes de uma vez
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Exemplos de cobrança do Partner Center para uma única vez e selecione compras recorrentes-quando você adquire assinaturas, adicione mais assinaturas, adicione ou remova licenças.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a26b6e5299c5186959612e622808161ca0f7f7c2
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148611"
---
# <a name="partner-center-billing-scenarios-for-one-time-and-select-recurring-purchases"></a>Cenários de cobrança do Partner Center para uma única vez e selecione compras recorrentes

**Funções apropriadas**: agente de administração | Administrador de cobrança | Agente de assistência técnica | Agente de vendas

Esses são [cenários de cobrança comuns](common-billing-scenarios.md). 

## <a name="purchase-a-subscription-and-add-a-license-on-the-same-day"></a>Comprar uma assinatura e adicionar uma licença no mesmo dia

No Cenário 1, você compra uma assinatura em 11 de junho a um preço unitário de US$ 4. Mais tarde, no mesmo dia, você compra outra assinatura como a anterior pelo mesmo preço.

O arquivo de reconhecimento incluirá o seguinte:

- Cobrança de US$ 4 pelo período de serviço de 10 de junho – 9 de julho.
- Nova cobrança proporcional de US$ -4,00 pelo período de serviço de 11 de junho – 11 de junho. Esse é o período em que você tinha alguma licença. Cálculo = (preço mensal/total de dias no período de serviço) x dias no período de serviço proporcional x número de licenças = (4/30) x 30 x 1 = 4,00.
- Nova cobrança proporcional de US$ 8,00 pelo período de serviço de 10 de junho – 9 de julho. Esse é o período em que você tinha duas licenças. Cálculo = (4/30) x 30 x 2 = 8,00.

|**Data de compra**   |**Início da cobrança** |**Término da cobrança**  |**Preço unitário**  |**Quantidade**  |**Amount** |**Tipo de preço** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/06/2019      |10/06/2019   |9/07/2019         |US$ 4                |1                 |US$ 4            |Novo         |
|11/06/2019     | 10/06/2019    |9/07/2019        |US$ 4        |1        | -US$ 4       |addQuantity           |
|11/06/2019     | 10/06/2019    |9/07/2019        |US$ 4        | 2      |US$ 8         |addQuantity           |

## <a name="purchase-a-subscription-and-add-more-subscriptions-later"></a>Comprar uma assinatura e adicionar mais assinaturas mais tarde

No Cenário 2, você compra uma assinatura em 11 de junho com um preço unitário de US$ 4 e, em 12 de junho, você compra outra assinatura do mesmo produto pelo mesmo preço.

O arquivo de reconhecimento incluirá o seguinte:

- Cobrança de US$ 4 pelo período de serviço de 10 de junho – 9 de julho.
- Nova cobrança proporcional de US$ -3,87 pelo período de serviço de 11 de junho – 12 de junho. Esse é o período em que você tinha uma licença. Cálculo = (preço mensal/total de dias no período de serviço) x dias no período de serviço proporcional x número de licenças = (4/30) x 29 x 1 = 3,87.
- Nova cobrança proporcional de US$ 7,74 pelo período de serviço de 12 de junho – 9 de julho. Esse é o período em que você tinha duas licenças. Cálculo = (4/30) x 29 x 2 = 7,74.

|**Data de compra**   |**Início da cobrança** |**Término da cobrança**  |**Preço unitário**  |**Quantidade**  |**Amount** |**Tipo de preço** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/06/2019 (você tem uma licença)     |10/06/2019   |9/07/2019         |US$ 4         |1        |US$ 4            |Novo         |
|12/06/2019     | 10/06/2019    |9/07/2019        |US$ 4        |1        | -US$ 3,87       |addQuantity           |
|12/06/2019     | 10/06/2019    |9/07/2019        |US$ 4        | 2      |US$ 7,74       |addQuantity           |

## <a name="purchase-a-subscription-and-remove-a-license-on-the-same-day"></a>Comprar uma assinatura e remover uma licença no mesmo dia

No Cenário 3, você compra duas assinaturas para o mesmo produto em 11 de junho a um preço unitário de US$ 4. Mais tarde, no mesmo dia, você remove uma das licenças.  

O arquivo de reconhecimento incluirá o seguinte:

- Cobrança de US$ 8 por duas licenças pelo período de serviço de 10 de junho – 9 de julho.
- Nova cobrança proporcional de US$ -8,00 pelo período de serviço de 11 de junho – 11 de junho. Esse é o período em que você tinha duas licenças. Cálculo = (preço mensal/total de dias no período de serviço) x dias no período de serviço proporcional x número de licenças = (4/30) x 30 x 2 = 8,00.
- Nova cobrança proporcional de US$ 4,00 pelo período de serviço de 11 de junho – 9 de julho. Esse é o período em que você tinha uma licença. Cálculo = (4/30) x 30 x 1 = 4,00.

|**Data de compra**   |**Início da cobrança** |**Término da cobrança**  |**Preço unitário**  |**Quantidade**  |**Amount** |**Tipo de preço** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/06/2019      |10/06/2019   |9/07/2019         |US$ 4                |2                 |US$ 8            |Novo         |
|11/06/2019     | 10/06/2019    |9/07/2019        |US$ 4        |2        | -US$ 8       |removeQuantity           |
|11/06/2019     | 10/06/2019    |9/07/2019        |US$ 4        | 1      |US$ 4         |removeQuantity           |

## <a name="purchase-a-subscription-and-remove-licenses-later"></a>Comprar uma assinatura e remover licenças mais tarde

No cenário 4, você compra duas assinaturas em 11 de junho a um preço unitário de $4 e em 12 de junho você remove uma das licenças.

O arquivo de reconhecimento incluirá o seguinte:

- Cobrança de US$ 8 pelo período de serviço de 10 de junho – 9 de julho.
- Nova cobrança proporcional de US$ -7,74 pelo período de serviço de 11 de junho – 12 de junho. Esse é o período em que você tinha duas licenças. Cálculo = (preço mensal/total de dias no período de serviço) x dias no período de serviço proporcional x número de licenças = (4/30) x 29 x 2 = 7,74.
- Nova cobrança proporcional de US$ 3,87 pelo período de serviço de 12 de junho – 9 de julho. Esse é o período em que você tinha uma licença. Cálculo = (4/30) x 29 x 1 = 3,87.

|**Data de compra**   |**Início da cobrança** |**Término da cobrança**  |**Preço unitário**  |**Quantidade**  |**Amount** |**Tipo de preço** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019 (você tem duas licenças)     |10/06/2019   |9/07/2019         |US$ 4         |2        |US$ 8       |Novo       |
|12/06/2019     | 10/06/2019    |9/07/2019        |US$ 4        |2        | -US$ 7,74       |removeQuantity           |
|6/12/2019 (você tem uma licença)    | 10/06/2019    |9/07/2019   |US$ 4    |1      |US$ 3,87    |removeQuantity |

## <a name="next-steps"></a>Próximas etapas

- [Cenários de cobrança mensal de exemplo para novas assinaturas, alteração de valores de licença ou suspensão](common-billing-scenarios-monthly.md)