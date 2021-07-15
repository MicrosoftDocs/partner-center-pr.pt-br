---
title: Tipos de encargo de arquivos de reconciliação
ms.topic: article
ms.date: 06/05/2020
description: Descubra os tipos de encargos (como, baseado em licença, baseado em uso e uma vez), créditos e descontos em Partner Center de reconciliação.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 10438ba30c6eb5ba5b1daef1ad16521f1f8e77c6
ms.sourcegitcommit: 70b8ebbe0d431c7a13529f9eabd1b24f40108a46
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2021
ms.locfileid: "113989767"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a>Entender os diferentes tipos de cobrança em arquivos Partner Center reconciliação

**Aplica-se a**: Partner Center | Partner Center para o Microsoft Cloud for US Government

**Funções apropriadas**: Agente administrativo | Administrador de cobrança | Administrador global

Este artigo descreve os mapeamentos entre uma seção da fatura e os tipos de cobrança associados que podem estar em seu arquivo de reconciliação. Sua fatura fornece um resumo dos encargos. Seu arquivo de reconciliação fornece um detalhamento das transações de item de linha, incluindo tipos de cobrança. Para obter mais informações sobre arquivos de reconciliação, [consulte como usar arquivos de reconciliação](use-the-reconciliation-files.md).

Os [arquivos de reconciliação baseados](usage-based-recon-files.md) em uso e os arquivos de reconciliação baseados em licença mostram apenas transações e encargos relacionados ao uso (unidades consumidas e encargos relacionados). [](license-based-recon-files.md)

> [!NOTE]
> Créditos, descontos ou reembolsos pontuais que aparecem na fatura como Ajustes não são **mostrados** no arquivo de reconciliação.

## <a name="map-charge-types-to-invoice-charges"></a>Mapear tipos de cobrança para encargos de fatura

Para fazer referência cruzada de valores de cobrança entre sua fatura e o arquivo de reconciliação, use as opções de filtro Microsoft Excel. Filtre por tipos de cobrança em seu arquivo de reconciliação para mapear os encargos da fatura para um conjunto de detalhamentos de encargos no arquivo de reconciliação.

## <a name="license-based-charges"></a>Cobranças baseada em licença

Para mapear esses encargos baseados em licença para sua fatura, soma a **coluna Valor** do arquivo baseado em licença.

| Descrição da cobrança (coluna ChargeType no arquivo de reconciliação) | Explicação da cobrança |
| ------------------------------------------------------------- | ------------------ |
| Taxa de ativação | O valor cobrado ao cliente quando ele usa a assinatura após a compra. |
| Taxa de cancelamento | Encargos rateados reembolsados ao cliente quando as licenças associadas são alteradas. |
| Cancelar ocorrência proporcional | Encargos rateados cancelados quando o cliente com assinatura mensal tem a assinatura suspensa e as licenças associadas foram alteradas no mesmo mês. |
| Taxa do Ciclo | Encargos periódicos para uma assinatura. |
| Proporcional à instância do ciclo | Encargos rateados avaliados pelo cliente quando as licenças associadas são alteradas. |
| Taxas proporcionais durante o cancelamento | Reembolso rateado por parte nãoutilizada do serviço após o cancelamento. |
| Taxas de taxa de taxa ao converter fora da oferta atual | Encargos rateados após a conversão da assinatura mensal atual em uma assinatura anual. |
| Taxas de taxa ao converter em uma nova oferta | Encargos rateados depois de converter uma assinatura mensal em uma nova assinatura anual. |
| Taxas proporcionais na compra | O tipo de cobrança de uma assinatura ao usar a cobrança mensal ou anual. |
| Taxa proporcional ao renovar | Valores rateados após a renovação da assinatura. |
| Taxa de renovação | Cobrança para renovação de uma assinatura |
| Taxas proporcionais ao ativar | Valores rateados da ativação até o final do período de cobrança. |

## <a name="one-time-charges"></a>Encargos único

Para mapear esses encargos de uso único para sua fatura, soma a **coluna Valor** do arquivo baseado em licença.

| Descrição da cobrança (coluna ChargeType no arquivo de reconciliação) | Explicação da cobrança |
| ------------------------------------------------------------- | ------------------ |
| novo | Usado quando uma nova compra é criada. |
| renovar | Usado quando uma assinatura é renovada após o final do termo. |
| addQuantity | Usado no reembolso da compra original e na nova quantidade após um aumento. |
| removeQuantity | Usado no reembolso da compra original e na nova quantidade após uma diminuição. |
| cancelImmediate | Usado quando uma assinatura é cancelada. |
| convert | Usado quando uma licença é atualizada. |
| customerCredit | Usado quando créditos (por exemplo, Azure, SLA etc.) são dados em uma transação. |

## <a name="usage-charges"></a>Encargos de uso

Para mapear esses encargos de uso para sua fatura, soma a **coluna PretaxCharges** do arquivo baseado em uso.

| Descrição da cobrança (coluna ChargeType no arquivo de reconciliação) | Explicação da cobrança |
| ------------------------------------------------------------- | ------------------ |
| Avaliar a taxa de uso ao cancelar | Taxa de uso de acesso ao cancelamento para uso não pago durante o período de faturamento atual. |
| Avalie a taxa de uso para o ciclo atual | Taxa de uso de acesso para o período de faturamento atual. |

### <a name="credits"></a>Credits

Para mapear esses créditos para sua fatura:

- Soma o **TotalForCustomer do** arquivo baseado em licença.
- Soma a **coluna PostTaxTotal** do arquivo baseado em uso.

| Descrição da cobrança (coluna ChargeType no arquivo de reconciliação) | Explicação da cobrança |
| ------------------------------------------------------------- | ------------------ |
| Deslocando um item de linha | Reembolso parcial ou total para um item de linha, incluindo impostos. |

### <a name="usage-based-discounts"></a>Descontos baseados em uso

Para mapear esses descontos baseados em uso para sua fatura, soma a **coluna PretaxCharges** do arquivo baseado em uso.

| Descrição da cobrança (coluna ChargeType no arquivo de reconciliação) | Explicação da cobrança |
| ------------------------------------------------------------- | ------------------ |
| Desconto de ativação | Desconto aplicado quando a assinatura é ativada. |
| Desconto de ciclo | Desconto aplicado em encargos periódicos. |
| Desconto de renovação | Desconto aplicado quando a assinatura é renovada. |
| Desconto de cancelamento | Encargos aplicados quando descontos são cancelados. |

### <a name="license-based-discounts"></a>Descontos baseados em licença

Para mapear descontos baseados em licença para sua fatura, soma a **coluna TotalOtherDiscount** do arquivo baseado em licença.

*Descontos baseados em licença podem ser aplicados a vários tipos de cobrança.*
