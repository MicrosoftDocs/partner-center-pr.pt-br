---
title: Cenários comuns de cobrança para uma única vez e selecione compras recorrentes | Centro de parceiros
ms.topic: article
ms.date: 11/25/2019
description: Confira exemplos de cobrança do Partner Center para uma única vez e selecione compras recorrentes--quando você adquire assinaturas, adicione mais assinaturas, adicione ou remova estações.
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
Keywords: cobrança, pagamentos, compra única, compra recorrente, assinaturas, estações
ms.localizationpriority: medium
ms.openlocfilehash: f330e49fdfea9b93d02a644610f3621916667f86
ms.sourcegitcommit: c793c1b61f50fc0b0a12c95cedd9f57b31703093
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2019
ms.locfileid: "74722513"
---
# <a name="one-time-and-select-recurring-purchase-billing-scenarios"></a>Cenários de cobrança de compra recorrente e selecionados de uso único

**Funções apropriadas**

- Agente administrativo
- Administrador de cobrança
- Agente de suporte técnico
- Agente de vendas

Esses [cenários de cobrança comuns](common-billing-scenarios.md) de exemplo são aplicáveis a [uma única vez e selecionam encargos recorrentes](one-time-and-recurring-billing.md) no Partner Center.

## <a name="purchase-a-subscription-and-add-a-seat-on-the-same-day"></a>Comprar uma assinatura e adicionar um assento no mesmo dia

No Cenário 1, você compra uma assinatura em 11 de junho a um preço unitário de US$ 4. Mais tarde, no mesmo dia, você compra outra assinatura como a anterior pelo mesmo preço.

O arquivo de reconhecimento incluirá o seguinte:

- Cobrança de US$ 4 pelo período de serviço de 10 de junho – 9 de julho.
- Nova cobrança proporcional de US$ -4,00 pelo período de serviço de 11 de junho – 11 de junho. Nesse período, você tinha 1 licença. Cálculo = (preço mensal/total de dias no período de serviço) x dias no período de serviço proporcional x número de licenças = (4/30) x 30 x 1 = 4,00.
- Nova cobrança proporcional de US$ 8,00 pelo período de serviço de 10 de junho – 9 de julho. Nesse período, você tinha 2 licenças. Cálculo = (4/30) x 30 x 2 = 8,00.

|**Data de compra**   |**Início da cobrança** |**Término da cobrança**  |**Preço unitário**  |**Quantidade**  |**Valor** |**Tipo de cobrança** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/06/2019      |10/06/2019   |9/07/2019         |US$ 4                |1                 |US$ 4            |Novo         |
|11/06/2019     | 10/06/2019    |9/07/2019        |US$ 4        |1        | -US$ 4       |addQuantity           |
|11/06/2019     | 10/06/2019    |9/07/2019        |US$ 4        | 2      |US$ 8         |addQuantity           |

## <a name="purchase-a-subscription-and-add-more-subscriptions-later"></a>Comprar uma assinatura e adicionar mais assinaturas mais tarde

No Cenário 2, você compra uma assinatura em 11 de junho com um preço unitário de US$ 4 e, em 12 de junho, você compra outra assinatura do mesmo produto pelo mesmo preço.

O arquivo de reconhecimento incluirá o seguinte:

- Cobrança de US$ 4 pelo período de serviço de 10 de junho – 9 de julho.
- Nova cobrança proporcional de US$ -3,87 pelo período de serviço de 11 de junho – 12 de junho. Nesse período, você tinha 1 licença. Cálculo = (preço mensal/total de dias no período de serviço) x dias no período de serviço proporcional x número de licenças = (4/30) x 29 x 1 = 3,87.
- Nova cobrança proporcional de US$ 7,74 pelo período de serviço de 12 de junho – 9 de julho. Nesse período, você tinha 2 licenças. Cálculo = (4/30) x 29 x 2 = 7,74.

|**Data de compra**   |**Início da cobrança** |**Término da cobrança**  |**Preço unitário**  |**Quantidade**  |**Valor** |**Tipo de cobrança** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/06/2019 (você tem uma licença)     |10/06/2019   |9/07/2019         |US$ 4         |1        |US$ 4            |Novo         |
|12/06/2019     | 10/06/2019    |9/07/2019        |US$ 4        |1        | -US$ 3,87       |addQuantity           |
|12/06/2019     | 10/06/2019    |9/07/2019        |US$ 4        | 2      |US$ 7,74       |addQuantity           |

## <a name="purchase-a-subscription-and-remove-a-seat-on-the-same-day"></a>Comprar uma assinatura e remover um assento no mesmo dia

No Cenário 3, você compra duas assinaturas para o mesmo produto em 11 de junho a um preço unitário de US$ 4. Mais tarde, no mesmo dia, você remove um dos usuários.  

O arquivo de reconhecimento incluirá o seguinte:

- Cobrança de US$ 8 por duas licenças pelo período de serviço de 10 de junho – 9 de julho.
- Nova cobrança proporcional de US$ -8,00 pelo período de serviço de 11 de junho – 11 de junho. Nesse período, você tinha 2 licenças. Cálculo = (preço mensal/total de dias no período de serviço) x dias no período de serviço proporcional x número de licenças = (4/30) x 30 x 2 = 8,00.
- Nova cobrança proporcional de US$ 4,00 pelo período de serviço de 11 de junho – 9 de julho. Nesse período, você tinha 1 licença. Cálculo = (4/30) x 30 x 1 = 4,00.

|**Data de compra**   |**Início da cobrança** |**Término da cobrança**  |**Preço unitário**  |**Quantidade**  |**Valor** |**Tipo de cobrança** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/06/2019      |10/06/2019   |9/07/2019         |US$ 4                |2                 |US$ 8            |Novo         |
|11/06/2019     | 10/06/2019    |9/07/2019        |US$ 4        |2        | -US$ 8       |removeQuantity           |
|11/06/2019     | 10/06/2019    |9/07/2019        |US$ 4        | 1      |US$ 4         |removeQuantity           |

## <a name="purchase-a-subscription-and-remove-seats-later"></a>Comprar uma assinatura e remover estações mais tarde

No Cenário 4, você compra duas assinaturas em 11 de junho pelo preço unitário de US$ 4 e em 12 de junho você remove um dos usuários.

O arquivo de reconhecimento incluirá o seguinte:

- Cobrança de US$ 8 pelo período de serviço de 10 de junho – 9 de julho.
- Nova cobrança proporcional de US$ -7,74 pelo período de serviço de 11 de junho – 12 de junho. Nesse período, você tinha 2 licenças. Cálculo = (preço mensal/total de dias no período de serviço) x dias no período de serviço proporcional x número de licenças = (4/30) x 29 x 2 = 7,74.
- Nova cobrança proporcional de US$ 3,87 pelo período de serviço de 12 de junho – 9 de julho. Nesse período, você tinha 1 licença. Cálculo = (4/30) x 29 x 1 = 3,87.

|**Data de compra**   |**Início da cobrança** |**Término da cobrança**  |**Preço unitário**  |**Quantidade**  |**Valor** |**Tipo de cobrança** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/06/2019 (você tem duas licenças)     |10/06/2019   |9/07/2019         |US$ 4         |2        |US$ 8       |Novo       |
|12/06/2019     | 10/06/2019    |9/07/2019        |US$ 4        |2        | -US$ 7,74       |removeQuantity           |
|12/06/2019 (você tem uma licença)    | 10/06/2019    |9/07/2019   |US$ 4    |1      |US$ 3,87    |removeQuantity |
