---
title: Reconciliation file charge types | Partner Center
ms.topic: article
ms.date: 08/26/2019
description: Types of charges (license-based, usage-based and one-time), credits and discounts on Partner Center reconciliation files.
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
# <a name="understand-charge-types"></a>Understand charge types

Aplica-se a:

- Partner Center
- Partner Center do Microsoft Cloud for US Government

This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file. Your invoice provides a summary of charges. Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types. For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).

Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).

> [!NOTE]
> One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.

## <a name="map-charge-types-to-invoice-charges"></a>Map charge types to invoice charges

To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel. Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.

## <a name="license-based-charges"></a>Cobranças baseada em licença

To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.

| Charge description (ChargeType column in reconciliation file) | Charge explanation |
| ------------------------------------------------------------- | ------------------ |
| Taxa de ativação | The amount charged to the customer when they use the subscription after purchase. |
| Taxa de cancelamento | Prorated charges refunded to the customer when associated seats are changed. |
| Taxa do Ciclo | Periodic charges for a subscription. |
| Proporcional à instância do ciclo | Prorated charges assessed from the customer when associated seats are changed. |
| Taxas proporcionais durante o cancelamento | Prorated refund for unused portion of service upon cancellation. |
| Taxas proporcionais na compra | The charge type for a subscription when using annual billing. |
| Valor de compra | The charge type for a subscription when using monthly billing. |
| Taxa proporcional ao renovar | Prorated fees upon subscription renewal. |
| Taxa de renovação | Cobrança para renovação de uma assinatura |
| Taxas proporcionais ao ativar | >Prorated fees from activation until end of billing period. |

## <a name="one-time-charges"></a>One-time charges

To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.

| Charge description (ChargeType column in reconciliation file) | Charge explanation |
| ------------------------------------------------------------- | ------------------ |
| Novo | Used when a new purchase is created. |
| addQuantity | Used in both the refund of the original purchase and the new quantity after an increase. |
| removeQuantity | Used in both the refund of the original purchase and the new quantity after a decrease. |
| Cancelar | Used when a subscription is cancelled. |
| Converter | Used when a license is upgraded but the number of seats remains unchanged. |

## <a name="usage-charges"></a>Tarifas de uso

To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.

| Charge description (ChargeType column in reconciliation file) | Charge explanation |
| ------------------------------------------------------------- | ------------------ |
| Avaliar a taxa de uso ao cancelar | Access usage fee upon cancellation for unpaid usage during the current billing period. |
| Avalie a taxa de uso para o ciclo atual | Access usage fee for the current billing period. |

### <a name="credits"></a>Créditos

To map these credits to your invoice:

- Sum the **TotalForCustomer** from the license-based file.
- Sum the **PostTaxTotal** column from the usage-based file.

| Charge description (ChargeType column in reconciliation file) | Charge explanation |
| ------------------------------------------------------------- | ------------------ |
| Deslocando um item de linha | Partial or whole refund to a line item, including taxes. |

### <a name="usage-based-discounts"></a>Descontos baseados em uso

To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.

| Charge description (ChargeType column in reconciliation file) | Charge explanation |
| ------------------------------------------------------------- | ------------------ |
| Desconto de ativação | Discount applied when subscription activated. |
| Desconto de ciclo | Discount applied on periodic charges. |
| Desconto de renovação | Discount applied when subscription renewed. |
| Desconto de cancelamento | Charges applied when discounts cancelled. |

### <a name="license-based-discounts"></a>Descontos baseados em licença

To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.

*License-based discounts may be applied to multiple charge types.*
