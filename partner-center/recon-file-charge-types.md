---
title: Tipos de encargo de arquivo de reconciliação
ms.topic: article
ms.date: 06/05/2020
description: Descubra os tipos de encargos (como, baseado em licença, com base no uso e em uma única vez), créditos e descontos em arquivos de reconciliação do Partner Center.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7a5c227748ba24001288ecbec0a5487d38033897
ms.sourcegitcommit: 7abdd277c0eea51237c97cbb163a4943fd740356
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2020
ms.locfileid: "84467506"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a>Entender os diferentes tipos de encargo em arquivos de reconciliação do Partner Center

**Aplica-se a**

- Partner Center
- Partner Center do Microsoft Cloud for US Government

**Funções apropriadas**

- Agente administrativo
- Administrador de cobrança
- Administrador global

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
| Cancelar ocorrência proporcional | Encargos rateado cancelados quando o cliente com a assinatura mensal tem assinatura suspensa e estações associadas foram alteradas no mesmo mês. |
| Taxa do Ciclo | Cobranças periódicas de uma assinatura. |
| Proporcional à instância do ciclo | Encargos rateado avaliados do cliente quando as estações associadas são alteradas. |
| Taxas proporcionais durante o cancelamento | Reembolso rateado para parte não usada do serviço após o cancelamento. |
| Taxa de taxas ao converter da oferta atual | Encargos rateado após a conversão da assinatura mensal atual em uma assinatura anual. |
| Taxas de taxa ao converter em uma nova oferta | Encargos rateado após a conversão de uma assinatura mensal em uma nova assinatura anual. |
| Taxas proporcionais na compra | O tipo de encargo para uma assinatura ao usar a cobrança anual. |
| Valor de compra | O tipo de encargo para uma assinatura ao usar a cobrança mensal. |
| Taxa proporcional ao renovar | Taxas rateada após a renovação da assinatura. |
| Taxa de renovação | Cobrança para renovação de uma assinatura |
| Taxas proporcionais ao ativar | Taxas rateada da ativação até o término do período de cobrança. |

## <a name="one-time-charges"></a>Encargos de uso único

Para mapear esses encargos de uma vez para sua fatura, some a coluna de **valor** do arquivo baseado em licença.

| Descrição da cobrança (coluna Chargetype no arquivo de reconciliação) | Explicação da cobrança |
| ------------------------------------------------------------- | ------------------ |
| Novo | Usado quando uma nova compra é criada. |
| addQuantity | Usado tanto no reembolso da compra original quanto na nova quantidade após um aumento. |
| removeQuantity | Usado tanto no reembolso da compra original quanto na nova quantidade após uma diminuição. |
| Cancelar | Usado quando uma assinatura é cancelada. |
| Converter | Usado quando uma licença é atualizada, mas o número de estações permanece inalterado. |

## <a name="usage-charges"></a>Encargos de uso

Para mapear esses encargos de uso para sua fatura, some a coluna **PretaxCharges** do arquivo baseado em uso.

| Descrição da cobrança (coluna Chargetype no arquivo de reconciliação) | Explicação da cobrança |
| ------------------------------------------------------------- | ------------------ |
| Avaliar a taxa de uso ao cancelar | Taxa de uso de acesso ao cancelamento para uso não pago durante o período de faturamento atual. |
| Avalie a taxa de uso para o ciclo atual | Taxa de uso de acesso para o período de faturamento atual. |

### <a name="credits"></a>Credits

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
| Desconto de cancelamento | Encargos aplicados quando descontos são cancelados. |

### <a name="license-based-discounts"></a>Descontos baseados em licença

Para mapear descontos baseados em licença para sua fatura, some a coluna **TotalOtherDiscount** do arquivo baseado em licença.

*Os descontos baseados em licença podem ser aplicados a vários tipos de cobrança.*
