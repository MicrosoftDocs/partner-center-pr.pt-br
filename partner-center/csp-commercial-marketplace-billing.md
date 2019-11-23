---
title: Billing for commercial marketplace products | Partner Center
ms.topic: article
ms.date: 11/21/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Learn how billing works for ISV SaaS products or subscriptions purchased for customers from the commercial marketplace within Partner Center.
author: MicheleHope
ms.author: v-mihope
keywords: subscriptions, products, purchases, Marketplace, third party, ISV, billing, invoices, reconciliation, recon file
ms.localizationpriority: medium
ms.openlocfilehash: bc4dcca3d8c3d454a17eca676d5fadd1dac202d3
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/22/2019
ms.locfileid: "74384918"
---
# <a name="billing-for-commercial-marketplace-products"></a>Billing for commercial marketplace products

**Aplica-se a**

- Partner Center
- Parceiros no programa CSP

**Appropriate roles**

- Administração global
- Administrador de cobrança

As a partner in the CSP program, you can use Partner Center to purchase license-based SaaS products from ISV publishers in the commercial marketplace. After you do so, you can access a bill for these types of purchases. The billing period starts on the first day of the calendar month and ends on the last day of the calendar month. Invoices are made available on the 8th day of the following month.

You can access invoices from either the Partner Center [dashboard](https://partner.microsoft.com/dashboard/) or by using [Partner Center APIs](https://docs.microsoft.com/partner-center/develop/).

Partners in the CSP program are billed for ISV commercial marketplace solutions purchased for a customer when they purchase those products from either Partner Center or from the Azure portal (using the customer's prior, CSP-purchased Azure tenant).

>[!NOTE]
>If customers use their own Azure AD tenant (not one purchased from a partner in the CSP program), customers can also choose to purchase their own ISV SaaS solution directly from ([Microsoft AppSource](https://appsource.microsoft.com/) or [Azure Marketplace](https://azuremarketplace.microsoft.com/)). If they do so, they will receive their own bill directly from Microsoft. Likewise, if a partner in the CSP program sells an Azure AD tenant to the customer and grants the customer [role-based access](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles) to that tenant (assigning any role to the customer besides **Reader**), that customer can also purchase commercial marketplace offers without prior approval or notification to the CSP partner. In these cases, Microsoft will not directly notify partners in the CSP program about purchases made by their customers. However, Microsoft does offer an optional [Azure Monitor](https://docs.microsoft.com/azure/azure-monitor/platform/alerts-activity-log) mechanism that you can use to set alerts or notifications about activity on an Azure subscription.

## <a name="access-billing-information-for-commercial-marketplace-products"></a>Access billing information for commercial marketplace products

O administrador global ou de cobrança da sua empresa receberá um email quando a fatura estiver pronta para ser exibida. To access the latest invoice and reconciliation file for commercial marketplace product purchases:

1. Entre no [Painel](https://partner.microsoft.com/dashboard/) do Partner Center.

2. No menu do Partner Center, selecione **Cobrança**. 

    You will see two tabs at the top of the Billing page: **Recurring** and **Recurring and one-time purchases**. Each tab lets you access invoice and reconciliation (recon) files for different marketplace products:

    - **Recurring** tab: Shows invoice and reconciliation files for subscriptions related to Office 365, Microsoft 365, Dynamics 365, Azure Active Directory, PowerBI Pro, and Microsoft Azure.

    - **Recurring and one-time purchases** tab: Shows invoice and reconciliation files for Azure plan, Azure reservations, software and commercial marketplace products.
  
3. Select the **Recurring and one-time purchases** tab. If you purchased subscriptions for a customer in a different currency, you will see a tab for each currency. You can do a few things fr:om this page:

    - To see the latest invoice and reconciliation file, select **Invoice** or **Reconciliation file**. (If you wanted to, you can also access the latest invoice and recon file data using [Partner Center APIs](https://docs.microsoft.com/partner-center/develop/).

    - To see earlier invoices and recon files, expand the **Billing history** row below.

    - To check your estimated account balance or bill at any time based on the latest account activity, select a link under the **Estimates** heading.  

    >[!NOTE]
    > When we post your bill on the 8th day of the month, it will include taxes and any other applicable charges and credits. This means the final amount due might differ from what you see during the billing period.

## <a name="more-about-invoices-and-recon-files-for-commercial-marketplace-products"></a>More about invoices and recon files for commercial marketplace products

This section offers more information about invoice and reconciliation files for commercial marketplace SaaS subscriptions purchased for customers from third-party ISV publishers.

When you select **Recurring and one-time purchases** from the **Billing** option in the Partner Center menu, you gain access to invoices and reconciliation files for charges related to both Microsoft (first-party) and ISV (third-party) purchases. These purchases may be associated with:

- SaaS subscriptions (from either Microsoft or ISV publishers)

- Azure plan

- Reservas do Azure

- Other subscription-based software (from either Microsoft or ISV publishers)

Examples of these purchases might include SUSE Linux software (a software subscription) or an Azure ISV SaaS product subscription.

>[!NOTE]
> For more information about how to read invoice and recon files, see also [Billing overview](billing.md).

### <a name="tips-on-reading-your-invoice"></a>Tips on reading your invoice

When you purchase a license-based SaaS product from a third-party ISV publisher, you will only see charges for the license fee on your invoice. This is true even when the ISV's SaaS product uses (or consumes) underlying Azure infrastructure resources. That is because your customer's Azure infrastructure usage charges for an ISV's SaaS product are billed directly to the ISV. (ISVs will see associated Azure consumption charges in their own Azure usage daily-rated invoice reconciliation file.)

Your invoice will contain several pages:

- **Page 1 of the invoice:** Contains a summary overview of the CSP program partner's billing details. This includes a summary of charges for the billing period, an invoice number, payment terms (Net 60 days), and billing payment methods to pay by wire or by check.

- **Page 2 (and any subsequent pages) of the invoice:** Details charges for both first-party Microsoft purchases and third-party ISV (license-based) purchases from the commercial marketplace. You can identify ISV license-based purchases by the **Publisher** line beneath each product name. The associated reconciliation file offers more billing details for specific invoice charges.

- **Final page of the invoice:** If you were charged for license-based marketplace products from an ISV, this final page will display more details about the ISV publisher's name and address.

### <a name="tips-on-reading-your-reconciliation-file"></a>Tips on reading your reconciliation file

The **Recurring and one-time purchases** reconciliation file contains several columns with additional details that map to the charges in your invoice. The **PublisherName** column shows whether the purchase is from Microsoft or a third-party ISV publisher.

Some charges in your reconciliation file may appear with a cost of $0. This may be due to an ISV "free trial" offer (usually 30 or 60 days) or a Bring Your Own License offer.

In the case of free trial ISV offers:

- The free trial period covers the cost of the ISV's license-based SaaS product during that time. You will also not be charged for associated Azure infrastructure use of that SaaS product.  If you are using a usage-based ISV offer, however, the free trial does not include the cost of underlying Azure infrastructure usage. In this case, Azure infrastructure usage charges will appear in a separate Azure reconciliation file.

- When you purchase and deploy an ISV's free trial-eligible product for your customer, the customer is automatically enrolled in the free trial by the ISV publisher. The free trial period ends automatically after the period defined by the ISV publisher. After the period ends, the customer will be charged. This means the reconciliation file may show two rows for a trial-eligible product: One that tracks the trial period and one that tracks the paid offer (which will display a cost of $0 until after the trial period ends). Once the trial ends, the row showing the paid offer will start to show charges. 

For more information about what each column represents, see [Use your reconciliation files](use-the-reconciliation-files.md). See also [Types of billing in Partner Center](billing-different-types.md)

## <a name="next-steps"></a>Próximas etapas

- [Manage commercial marketplace products for customers](csp-commercial-marketplace-manage.md)
- [Learn about support for commercial marketplace products](csp-commercial-marketplace-support.md)
