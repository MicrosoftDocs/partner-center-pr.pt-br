---
title: Cenários comuns de cobrança mensal
ms.topic: article
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Cenários comuns no Partner Center quando você usa a cobrança mensal – inclui adicionar novas assinaturas, alterar a quantidade de licenças e suspender assinaturas.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4fe5c33fe549604f25500dd333d187e6b70ad73e
ms.sourcegitcommit: 3d7d5064c5e021079ed7e6f93f03869cbf425a32
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/06/2021
ms.locfileid: "106502507"
---
# <a name="sample-monthly-billing-scenarios-for-new-subscriptions-changing-license-amounts-or-suspensions"></a>Cenários de cobrança mensal de exemplo para novas assinaturas, alteração de valores de licença ou suspensão

**Funções apropriadas**

- Agente administrativo
- Administrador de cobrança
- Agente de suporte técnico
- Agente de vendas

Esses [cenários de cobrança comuns](common-billing-scenarios.md) de exemplo são aplicáveis se você usar a cobrança mensal no Partner Center.

## <a name="new-monthly-subscription"></a>Nova assinatura mensal

Sua data de cobrança é no 15º dia de cada mês. Em 13 de Janeiro, você compra uma nova assinatura com uma licença para US $4/mês e seleciona cobrança mensal. O arquivo de reconciliação com base em licença de 15 de janeiro conterá as seguintes linhas de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço Unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/01/2018         |12/02/2018    |Taxa do Ciclo   |4,00       |1        |4,00 |

O arquivo de reconciliação com base em licença de 15 de fevereiro conterá a seguinte linha de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço Unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/02/2018         |12/03/2018    |Taxa do Ciclo   |4,00       |1        |4,00 |

## <a name="change-license-quantity"></a>Alterar a quantidade de licenças

Sua data de cobrança é no 15º dia de cada mês. Em 13 de Janeiro, você compra uma nova assinatura com uma licença para US $4/mês e seleciona cobrança mensal. O arquivo de reconciliação com base em licença de 15 de janeiro conterá as seguintes linhas de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço Unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/01/2018         |12/02/2018    |Taxa do Ciclo   |4,00       |1        |4,00    |

Em 1º de fevereiro, você aumenta a quantidade de licenças de um para dois. O arquivo de reconciliação com base em licença de 15 de fevereiro conterá as seguintes linhas de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço Unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 13/01/2018        |12/02/2018    |Proporcional à Instância do Ciclo   |-4,00       |1        |-4,00   |
|13/01/2018         |31/01/2018    | Proporcional à Instância do Ciclo   |2.45       |1        |2.45    |
|1/02/2018         |12/02/2018    | Proporcional à Instância do Ciclo   |1.55       |2        |3.10    |
|13/02/2018         |12/03/2018    | Proporcional à Instância do Ciclo   |4,00       |2        |8,00    |

O preço mensal é de 4,00 e há 31 dias no termo de serviço: 13/01/2018 a 12/02/2018. Isso equivale a um preço diário de 0,129 (4/31).

Há 19 dias no termo proporcional de 13/01/2018 a 31/01/2018.

Preço unitário proporcional = 2,451 = 19 x 0,129

Há 12 dias no termo proporcional de 01/02/2018 a 12/02/2018.

Preço unitário proporcional = 1,54 = 12 x 0,129

## <a name="suspend-before-30-days"></a>Suspender antes de 30 dias

Sua data de cobrança é no 15º dia de cada mês. Em 13 de Janeiro, você compra uma nova assinatura com uma licença para US $4/mês e seleciona cobrança mensal. O arquivo de reconciliação com base em licença de 15 de janeiro conterá as seguintes linhas de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço Unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/01/2018         |12/02/2018    |Taxa do Ciclo   |4,00       |1        |4,00    |

Em 1º de fevereiro, você suspende uma assinatura. O arquivo de reconciliação com base em licença de 15 de fevereiro conterá a seguinte linha de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço Unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/02/2018|Taxa de cancelamento|-4,00|1|-4,00

## <a name="suspend-after-30-days"></a>Suspender após 30 dias

Sua data de cobrança é no 15º dia de cada mês. Em 13 de Janeiro, você compra uma nova assinatura com uma licença para US $4/mês e seleciona cobrança mensal. O arquivo de reconciliação com base em licença de 15 de janeiro conterá as seguintes linhas de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço Unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/02/2018|Taxa do Ciclo|4,00|1|4,00

O arquivo de reconciliação com base em licença de 15 de fevereiro conterá a seguinte linha de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço Unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/02/2018|12/03/2018|Taxa do Ciclo|4,00|1|4,00

Em 1º de março, você suspendeu a assinatura. O arquivo de reconciliação com base em licença de 15 de março conterá a seguinte linha de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço Unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
01/03/2018|12/03/2018|Taxa de cancelamento|-1,72|1|-1,72

O preço mensal é de 4,00 e há 28 dias no termo de serviço: 13/02/2018 a 12/03/2018. Isso equivale a um preço diário de 0,143 (4/28).

Preço unitário = dias no termo de serviço x preço diário x número de licenças.

Há 12 dias no termo de cancelamento de 01/03/2018 a 12/03/2018.

Portanto, o preço unitário =-1,716 (12 x 0,143 x (-1)).

## <a name="next-steps"></a>Próximas etapas

- [Cenários de cobrança para uma única vez e selecione compras recorrentes](common-billing-scenarios-onetime-recurring.md)