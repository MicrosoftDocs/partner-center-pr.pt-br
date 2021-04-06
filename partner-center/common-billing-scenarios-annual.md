---
title: Cobrança anual – cenários comuns
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Cobrança anual do Partner Center-quando você adiciona novas assinaturas, adicione licenças antes da data de cobrança, altere a quantidade de licenças ou suspenda/reative as assinaturas.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7494fd7cc003d1179c0ed959b21e1be2cbcc3255
ms.sourcegitcommit: 3d7d5064c5e021079ed7e6f93f03869cbf425a32
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/06/2021
ms.locfileid: "106502473"
---
# <a name="common-annual-billing-scenarios-in-partner-center"></a>Cenários comuns de cobrança anual no Partner Center

**Funções apropriadas**

- Agente administrativo
- Administrador de cobrança
- Agente de suporte técnico
- Agente de vendas

Esses [cenários de cobrança comuns](common-billing-scenarios.md) de exemplo são aplicáveis se você usar a cobrança anual no Partner Center.

## <a name="new-annual-subscription"></a>Nova assinatura anual

Sua data de cobrança é no 15º dia de cada mês. Em 13 de Janeiro, você compra uma nova assinatura com uma licença para US $4/mês e seleciona cobrança anual. O arquivo de reconciliação com base em licença de 15 de janeiro conterá a seguinte linha de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço Unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Taxas proporcionais na compra|48,00|1|48,00

## <a name="add-license-after-subscription-anniversary-date-but-before-billing-date"></a>Adicionar licença após a data de aniversário da assinatura, mas antes da data de cobrança

Você compra uma nova assinatura dia 11/02/17 com uma licença por US$ 211,20/ano. O aniversário da sua assinatura é definido como o dia 11 de cada mês. O sistema de cobrança da Microsoft cria as seguintes linhas de cobrança:

- Cobrança de US$ 211,20 pelo período de 11/02/17 a 10/02/18.

Em 2/12/17, você adquire uma segunda licença. Sua data de cobrança é 14/02/17. Os arquivos de fatura e reconciliação são gerados. O arquivo de reconciliação conterá as seguintes linhas de cobrança:

|Data de Início da Cobrança  |Data de Término da Cobrança  |Tipo de Cobrança  |Preço Unitário |Quantidade | Valor |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11/02/2017 |10/02/2018 |Taxas proporcionais na compra |211,20 |1 | 211,20 |

No aniversário da sua assinatura, 11/03/17, o sistema de cobrança da Microsoft cria as seguintes linhas de cobrança para o aumento de licença em 12/02/17:

- $211.20 crédito pelo período 2/11/17 – 2/10/18.
- $0.58 cobrança rateada por licença para uma licença para o período 2/11/17 – 2/11/17.
- $15.62 cobrança rateada por licença para duas licenças para o período 2/12/17 – 3/10/2017.
- $195 cobrança rateada por licença para duas licenças para o período 3/11/2017 – 2/10/2018.

Em 2/11/17, você adquire uma assinatura. Em 2/12/17, você adiciona uma licença. Sua data de cobrança é 14/02/17. Em 11/02/18, sua assinatura é renovada.

A próxima data de cobrança é 3/14/17 e uma nota fiscal e um arquivo de reconciliação são gerados. O arquivo de reconciliação conterá as seguintes linhas de cobrança:

|Data de Início da Cobrança  |Data de Término da Cobrança  |Tipo de Cobrança  |Preço Unitário |Quantidade | Valor |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11/02/2017 |10/02/2018 |Proporcional à Instância do Ciclo |-211,20 |1 |-211,20 |
|11/02/2017 |11/02/2017 |Proporcional à Instância do Ciclo |0,58 |1 |0,58 |
|12/02/2017 |10/03/2017 |Proporcional à Instância do Ciclo |15,62 |2 |31,25 |
|11/03/2017 |10/02/2018 |Proporcional à Instância do Ciclo |195,00 |2 |390,00 |

Em 11/02/18, a assinatura será renovada por outro período de 12 meses.

## <a name="change-license-quantity"></a>Alterar a quantidade de licenças

Sua data de cobrança é no 15º dia de cada mês. Em 13 de Janeiro, você compra uma nova assinatura com uma licença para US $4/mês e seleciona cobrança anual. O arquivo de reconciliação com base em licença de 15 de janeiro conterá a seguinte linha de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço Unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Taxas proporcionais na compra|48,00|1|48,00

Em 1º de fevereiro, você aumenta a quantidade de licenças de um para dois. O arquivo de reconciliação com base em licença de 15 de fevereiro conterá as seguintes linhas de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço Unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Proporcional à Instância do Ciclo|-48,00|1|-48,00
13/01/2018|31/01/2018|Proporcional à Instância do Ciclo|2.47|1|2.47
1/02/2018|12/01/2019|Proporcional à Instância do Ciclo|44,98|2|89,96

O preço anual é 48,00, que equivale ao preço diário de 0,13 (48,00/365).

Preço unitário = dias no termo de serviço x preço diário x número de licenças.

Há dias 19 no período de serviço de 13/01/2018 – 31/01/2018.

Portanto, o preço unitário = 2,47 (19 x 0,13 x 1)

Há dias 346 no período de serviço de 01/02/2018 – 12/01/2019.

Portanto, o preço unitário = 44,98 (346 x 0,13 x 2)

## <a name="suspend-before-30-days"></a>Suspender antes de 30 dias

Sua data de cobrança é no 15º dia de cada mês. Em 13 de Janeiro, você compra uma nova assinatura com uma licença para US $4/mês e seleciona cobrança anual. O arquivo de reconciliação com base em licença de 15 de janeiro conterá a seguinte linha de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço Unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Taxas proporcionais na compra|48,00|1|48,00

Em 1º de fevereiro, você suspende sua assinatura. O arquivo de reconciliação com base em licença de 15 de fevereiro conterá a seguinte linha de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço Unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Taxa de cancelamento|-48,00|1|-48,00

## <a name="suspend-after-30-days"></a>Suspender após 30 dias

Sua data de cobrança é no 15º dia de cada mês. Em 13 de Janeiro, você compra uma nova assinatura com uma licença para US $4/mês e seleciona cobrança anual. O arquivo de reconciliação com base em licença de 15 de janeiro conterá a seguinte linha de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço Unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Taxas proporcionais na compra|48,00|1|48,00

O arquivo de reconciliação com base em licença de 15 de fevereiro não conterá nenhuma linha de cobrança para essa assinatura.
Em 1º de março, você suspende sua assinatura. O arquivo de reconciliação com base em licença de 15 de março conterá a seguinte linha de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço Unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
01/03/2018|12/01/2019|Taxa de cancelamento|-41,34|1|-41,34

O preço anual é 48,00, que equivale ao preço diário de 0,13 (48,00/365).

Preço unitário = dias no termo de serviço x preço diário x número de licenças.

Há dias 318 no período de serviço de 01/03/2018 – 12/01/2019.

Portanto, o preço unitário = 41,34 (318 x 0,13 x 1). Como isso é um crédito, o preço unitário é de -41,34.

## <a name="suspend-and-reactivate"></a>Suspender e reativar

Sua data de cobrança é no 15º dia de cada mês. Em 13 de Janeiro, você compra uma nova assinatura com uma licença para US $4/mês e seleciona cobrança anual. O arquivo de reconciliação com base em licença de 15 de janeiro conterá a seguinte linha de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço Unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Taxas proporcionais na compra|48,00|1|48,00

Em 1º de fevereiro, você suspende sua assinatura. O arquivo de reconciliação com base em licença de 15 de fevereiro conterá a seguinte linha de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço Unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Taxa de cancelamento|-48,00|1|-48,00

Em 1º de março, você reativa sua assinatura. O arquivo de reconciliação com base em licença de 15 de março conterá a seguinte linha de cobrança:

|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço Unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
01/03/2018|12/01/2019|Taxas proporcionais na compra|41,34|1|41,34

O preço anual é 48,00, que equivale ao preço diário de 0,13 (48,00/365).

Preço unitário = dias no termo de serviço x preço diário x número de licenças.

Há dias 318 no período de serviço de 01/03/2018 – 12/01/2019.

Portanto, o preço unitário = 41,34 (318 x 0,13 x 1).
