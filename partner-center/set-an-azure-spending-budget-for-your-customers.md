---
title: Definir um orçamento de gastos do Azure para seus clientes | Partner Center
ms.topic: article
ms.date: 11/21/2019
description: Set a monthly budget per customer in Partner Center.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.assetid: DDE80361-D04E-432C-BC15-D735D2AE954F
author: MaggiePucciEvans
ms.author: evansma
ms.localizationpriority: medium
ms.openlocfilehash: 05212746e1ccbcc5081c68ca97ced6a99e20bb8c
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/22/2019
ms.locfileid: "74384897"
---
# <a name="set-an-azure-spending-budget-for-your-customers"></a>Definir um orçamento de gastos do Azure para seus clientes

Aplica-se a:

- Partner Center
- Partner Center do Microsoft Cloud for US Government

You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center. This helps your customers manage their Azure spending. This option allows you to compare your customers' Azure spending to the budget during the month. It also helps your customers budget their Azure spending so their monthly bill isn't higher than they anticipate.


> [!NOTE]  
> This feature is not available in sandbox or Test in Production (TIP) accounts.

After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways. These options may help you spot misconfigured services or unusual trends that might suggest fraud. You can then work with your customer(s) to identify the root cause and manage costs. If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.

- [Check current Azure spending](#check-current-azure-spending)
- [Turn on email notifications for when a customer's spending is nearing their budget limit](#notifications-for-budget-limits)
- [View itemized costs by service for usage-based subscriptions](#itemized-costs-by-service)

You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.

## <a name="azure-spending-data"></a>Azure spending data

The Azure spending data is an *estimate* and *actual billing amounts may vary*. The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.

The spending data is *refreshed once per day*. Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.

## <a name="set-azure-spending-budget"></a>Set Azure spending budget

You can *set a monthly Azure spending budget* for multiple customers in Partner Center:

1. Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).
2. In the left-hand menu under **CSP**, choose **Azure spending**.
3. On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.
4. Enter a value for **Monthly budget**.
5. Choose **Apply** to save your changes.

You can also *set a budget for an individual customer* in their subscription settings:

1. Sign in to the Partner Center dashboard.
2. In the left-hand menu under **CSP**, choose **Customers**.
3. On the **Customers** page, select the customer's **Company name**.
4. On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.
5. Enter a value for the budget.
6. Choose **Apply** to save your changes.

## <a name="remove-azure-spending-budget"></a>Remove Azure spending budget

You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:

1. Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).
2. In the left-hand menu under **CSP**, choose **Azure spending**.
3. On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.
4. Choose **Remove budget**.

## <a name="check-current-azure-spending"></a>Check current Azure spending

You can *track your customers' current Azure spending and monthly budgets* at any time:

1. Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).
2. In the left-hand menu under **CSP**, choose **Azure spending**.
3. On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.

## <a name="notifications-for-budget-limits"></a>Notifications for budget limits

You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit. When you turn on this option, you will be notified when customers use 80% or more of their monthly budget. This option helps you can keep an eye on your Azure bill. To configure email notifications:

1. Entre no Partner Center.
2. In the left-hand menu under **CSP**, choose **Azure spending**.
3. On the **Azure spending** page, under **Email notifications**, toggle the **Get emails** setting to **On**.
4. Choose **Change email address** to see the email address for notifications.
5. If the email address *isn't correct*, enter the correct email address and choose **Update**. If the email address *is correct*, choose **Cancel**.

## <a name="itemized-costs-by-service"></a>Itemized costs by service

You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:

1. Entre no Partner Center.
2. In the left-hand menu under **CSP**, choose **Customers**.
3. On the **Customers** page, select the customer's **Company name**.
4. On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.
5. On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.
