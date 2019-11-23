---
title: Invoice files | Partner Center
ms.topic: article
ms.date: 08/26/2019
description: Understand the fields in your invoice file for Partner Center billing.
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
keywords: billing, invoice
ms.localizationpriority: medium
ms.openlocfilehash: 9b3219b5752de59b9dde81343b8bd4e1128037bd
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389834"
---
# <a name="invoice-files"></a>Invoice files

You can use the following tables to understand the fields in Partner Center invoice files.

## <a name="invoice-file-fields"></a>Invoice file fields

The following fields appear on your invoice files.

| Campo | Definição |
| ----- | ---------- |
| EUA FEIN | Your Federal Employer Identification Number (FEIN). This is your United States federal tax identifier number. |
| Número do cliente | Seu número do cliente. |
| Cobrar de | O endereço para onde enviamos sua fatura. You can change your company name and/or address in your Partner Center billing profile. |
| Cobranças baseada em licença | The flat monthly or annual charges for your purchased usage-based licenses, billed in advance of the service. This number is the sum of all charges in the **Subtotal** column (column **T**) in your license-based reconciliation file. |
| Encargos baseados em uso | Your Azure usage. This includes new services or applications enabled and used during the billing period. This number is the sum of all charges in the **PretaxCharges** column (column **Z**) in your usage-based reconciliation file. |
| Descontos | The discount that the customer receives from subscription's normal price. This number is shown as a *flat amount*, not as a price per unit or license. |
| Créditos | Credits or adjustments for changes made to subscriptions (for example, seat increases or decreases). |
| Subtotal | Total antes de impostos e encargos e créditos sem imposto. |
| Tax | The total tax for your current charges, as totaled in the **Details** section beginning on page 2 of your invoice. This number is the sum of all charges in the **TaxAmount** column (column **AA**) in your usage-based reconciliation file, and the **Tax** column (column **U**) in your license-based reconciliation file. |
| Outros créditos | Créditos sem imposto. |
| Total dos encargos atuais | The amount due in your billing currency for the billing period. These charges are due by the payment due date. |
| Instruções de pagamento | Description of how to pay your invoice, based on your region. *Always be sure to include your invoice number when making a payment.* |
| Número da fatura | O número da sua fatura. |
| Período de cobrança | The monthly period leading up to the invoice date. This is the period during which usage-based services are consumed and license-based services are reconciled for any credit adjustments or changes in license count. |
| Data da fatura | The billing date or anniversary date on which your invoice is generated each month. |
| Termos de pagamento | The payment term. Para as compras únicas, sempre será 60 dias. |
| Data do pagamento | The date by which your payment must be received. |
| PO do cliente | Your purchase number order. |
| Atendimento ao cliente | The website address where you can access customer service. |
| Destinatário do serviço | The address where the service is being used. (This is the legal company address associated with company vetting.) |

## <a name="one-time-charges-fields"></a>One-time charges fields

The following fields only apply to **one-time charges** in Partner Center:

| Campo | Definição |
| ----- | ---------- |
| Data | Data da compra. |
| Descrição | Nome do produto. |
| Quantity | The number of products (such as reservations) purchased. |
| Preço unitário | Price per product (such as a reservation). |
| Descontos | Qualquer desconto aplicável. |
| Valor pré-taxado | Subtotal das compras antes dos impostos. |
| Imposto sobre vendas | Valor do imposto. |
| Total | Total amount to be paid. |
