---
title: Tipos de encargo de arquivo de reconciliação | Centro de parceiros
ms.topic: article
ms.date: 08/26/2019
description: Tipos de encargos (baseados em licença, com base no uso e uma única vez), créditos e descontos em arquivos de reconciliação do Partner Center.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 064ed6dda28f5a8ace64942d55ef2a6327528ff5
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389804"
---
# <a name="understand-charge-types"></a>Entender os tipos de encargo

Aplica-se a:

- Partner Center
- Partner Center do Microsoft Cloud for US Government

Este tópico descreve os mapeamentos entre uma seção de fatura e os tipos de encargos associados que podem estar em seu arquivo de reconciliação. Sua fatura fornece um resumo de encargos. O arquivo de reconciliação fornece uma divisão detalhada das transações de item de linha, incluindo tipos de encargo. Para obter mais informações sobre arquivos de reconciliação, consulte [como usar arquivos de reconciliação](use-the-reconciliation-files.md).

Os [arquivos de reconciliação com base no uso](usage-based-recon-files.md) e os [arquivos de reconciliação baseados em licença](license-based-recon-files.md) mostram apenas transações e encargos relacionados ao uso (unidades consumidas e encargos relacionados).

> [!NOTE]
> Créditos únicos, descontos ou reembolsos que aparecem na fatura como **ajustes** não são mostrados no arquivo de reconciliação.

## <a name="map-charge-types-to-invoice-charges"></a>Mapear tipos de cobrança para encargos de fatura

Para fazer referência cruzada de valores entre a fatura e o arquivo de reconciliação, use as opções de filtro no Microsoft Excel. Filtre por tipos de encargo em seu arquivo de reconciliação para mapear os encargos da fatura para um conjunto de divisões de cobrança no arquivo de reconciliação.

## <a name="license-based-charges"></a>Cobranças baseada em licença

Para mapear esses encargos baseados em licenças para sua fatura, some a coluna de **valor** do arquivo baseado em licença.

| Descrição da cobrança (coluna Chargetype no arquivo de reconciliação) | Explicação da cobrança |
| ------------------------------------------------------------- | ------------------ |
| Taxa de ativação | O valor cobrado para o cliente quando ele usa a assinatura após a compra. |
| Taxa de cancelamento | Encargos rateado reembolsados ao cliente quando as estações associadas são alteradas. |
| Taxa do ciclo | Cobranças periódicas de uma assinatura. |
| Proporcional à instância do ciclo | Encargos rateado avaliados do cliente quando as estações associadas são alteradas. |
| Taxas proporcionais durante o cancelamento | Reembolso rateado para parte não usada do serviço após o cancelamento. |
| Taxas proporcionais na compra | O tipo de encargo para uma assinatura ao usar a cobrança anual. |
| Valor de compra | O tipo de encargo para uma assinatura ao usar a cobrança mensal. |
| Taxa proporcional ao renovar | Taxas rateada após a renovação da assinatura. |
| Taxa de renovação | Cobrança para renovação de uma assinatura |
| Taxas proporcionais ao ativar | > taxas rateada da ativação até o término do período de cobrança. |

## <a name="one-time-charges"></a>Encargos de uso único

Para mapear esses encargos de uma vez para sua fatura, some a coluna de **valor** do arquivo baseado em licença.

| Descrição da cobrança (coluna Chargetype no arquivo de reconciliação) | Explicação da cobrança |
| ------------------------------------------------------------- | ------------------ |
| Novo | Usado quando uma nova compra é criada. |
| addQuantity | Usado tanto no reembolso da compra original quanto na nova quantidade após um aumento. |
| removeQuantity | Usado tanto no reembolso da compra original quanto na nova quantidade após uma diminuição. |
| Cancel | Usado quando uma assinatura é cancelada. |
| Converter | Usado quando uma licença é atualizada, mas o número de estações permanece inalterado. |

## <a name="usage-charges"></a>Tarifas de uso

Para mapear esses encargos de uso para sua fatura, some a coluna **PretaxCharges** do arquivo baseado em uso.

| Descrição da cobrança (coluna Chargetype no arquivo de reconciliação) | Explicação da cobrança |
| ------------------------------------------------------------- | ------------------ |
| Avaliar a taxa de uso ao cancelar | Taxa de uso de acesso no cancelamento para uso não pago durante o período de cobrança atual. |
| Avalie a taxa de uso para o ciclo atual | Taxa de uso de acesso para o período de cobrança atual. |

### <a name="credits"></a>Créditos

Para mapear esses créditos para sua fatura:

- Some o **TotalForCustomer** do arquivo baseado em licença.
- Some a coluna **PostTaxTotal** do arquivo baseado em uso.

| Descrição da cobrança (coluna Chargetype no arquivo de reconciliação) | Explicação da cobrança |
| ------------------------------------------------------------- | ------------------ |
| Deslocando um item de linha | Reembolso parcial ou total para um item de linha, incluindo impostos. |

### <a name="usage-based-discounts"></a>Descontos baseados em uso

Para mapear esses descontos com base no uso para sua fatura, some a coluna **PretaxCharges** do arquivo baseado em uso.

| Descrição da cobrança (coluna Chargetype no arquivo de reconciliação) | Explicação da cobrança |
| ------------------------------------------------------------- | ------------------ |
| Desconto de ativação | Desconto aplicado quando a assinatura é ativada. |
| Desconto de ciclo | Desconto aplicado em encargos periódicos. |
| Desconto de renovação | Desconto aplicado quando a assinatura é renovada. |
| Desconto de cancelamento | Encargos aplicados quando os descontos foram cancelados. |

### <a name="license-based-discounts"></a>Descontos baseados em licença

Para mapear descontos baseados em licença para sua fatura, some a coluna **TotalOtherDiscount** do arquivo baseado em licença.

*Os descontos baseados em licença podem ser aplicados a vários tipos de cobrança.*
