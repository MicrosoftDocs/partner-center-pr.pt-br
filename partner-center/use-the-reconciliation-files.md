---
title: Use your reconciliation files | Partner Center
ms.topic: article
ms.date: 11/21/2019
description: Use your reconciliation files to understand detailed line-item views of Partner Center charges.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 6bb65718159019c9ae47aa384524d9d52043d39b
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/22/2019
ms.locfileid: "74384789"
---
# <a name="use-your-reconciliation-files"></a>Use your reconciliation files

Aplica-se a:

- Partner Center
- Partner Center do Microsoft Cloud for US Government

You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle. Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).

Appropriate roles:

- Administrador de cobrança
- Administração global

For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).

## <a name="understand-reconciliation-file-fields"></a>Understand reconciliation file fields

- [License-based reconciliation file fields](license-based-recon-files.md)
- [Usage-based reconciliation file fields](usage-based-recon-files.md)
- [One-time and recurring reconciliation file fields](one-time-recurring-recon-files.md)
- [Daily-rated usage reconciliation file fields](daily-rated-usage-recon-files.md)

## <a name="understand-charge-types-in-reconciliation-files"></a>Understand charge types in reconciliation files

To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).

## <a name="fix-formatting-issues"></a>Fix formatting issues

Occasionally, a reconciliation file might contain formatting issues. For example, this issue might occur if the en-US locale is not used.

Follow these steps for fix any formatting issues in your reconciliation files:

1. Open the reconciliation file (in .csv format) in Microsoft Excel.
2. Select the first column in the file.
3. Open the **Convert Text to Columns Wizard**. On the ribbon, select **Data**, then select **Text to Columns**.
4. In the wizard, select **Delimited file type**. Then, select **Next**.
5. In the **Delimiters** field, select **Comma**. (If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.
6. In the **Column data format** field, select **Date:MDY**. Then, select **Next**.
7. In the **Column data format** field, select **Text** for all amount columns. Then, select **Finish**.

## <a name="download-reconciliation-files-programmatically"></a>Download reconciliation files programmatically

Reconciliation files can be very large and are sometimes difficult to download. To download reconciliation files programmatically, see [Get invoice line items](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).

## <a name="map-taxes-or-vat"></a>Map taxes or VAT

To map Taxes or value-added tax (VAT) to your invoice:

- Sum the **Tax** column from the license-based file.
- Sum the **TaxAmount** column from the usage-based file.

## <a name="itemize-reconciliation-files-by-partner"></a>Itemize reconciliation files by partner

Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.

| ID do MPN | Descrição |
| ------ | ----------- |
| ID do MPN | The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect). |
| [Reseller MPN ID](#reseller-mpn-id) | The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id). This field corresponds to the reseller ID listed for the specific subscription in Partner Center. Só aparece em arquivos de reconciliação para parceiros no modelo indireto. |

### <a name="reseller-mpn-id"></a>ID do MPN do revendedor

If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.

If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.

If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.

To view or update the **Reseller MPN ID**:

1. Entre no Partner Center.
2. No menu Partner Center, selecione **Clientes**.
3. Escolha o cliente na lista.
4. In the customer menu, select **Subscriptions**.
5. Choose the subscription from the list.
6. Selecione **Atualizar** para alterar o **Revendedor (ID do MPN)** .
