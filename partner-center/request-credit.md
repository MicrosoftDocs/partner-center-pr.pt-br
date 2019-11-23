---
title: Request an SLA credit from Microsoft | Partner Center
ms.topic: article
ms.date: 11/21/2019
description: Request an SLA credit from Microsoft if they experience a service outage.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.assetid: E7F1F68D-25E5-46C5-9C98-1D0A9FAB7993
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: a3eb79b78b3edb052d85cc7461d9fd50a115eb43
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/22/2019
ms.locfileid: "74384901"
---
# <a name="request-an-sla-credit-from-microsoft"></a>Request an SLA credit from Microsoft 

You're able to request **service-level agreement (SLA) credits** from Microsoft if a service that you're providing for your customers has an outage.

## <a name="sla-credit-calculation"></a>SLA credit calculation

SLA credits from Microsoft are determined based on which service(s) were impacted. For example, if your customer has an Office 365 suite but only experienced a SharePoint outage, the SLA credit is approved only for SharePoint and not the customer's entire plan.

*Credits are pro-rated based on the service affected and the duration of the outage.* To see the types of scenarios that qualify for SLA credits, see the [Online Services Consolidated SLA document](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37). This information applies to services sold through the Cloud Solution Provider program, too.

## <a name="request-an-sla-credit"></a>Request an SLA credit

*The Cloud Solution Provider (CSP) partner must submit the claim and all required information by the end of the calendar month following the month in which the incident occurred.* For example, if the incident occurred on February 15th, Microsoft must receive the claim and all required information by March 31st. End customers and indirect resellers can't submit SLA credit claims; either the indirect provider or direct bill partner must submit claims on their behalf.

### <a name="required-information"></a>Required information

Before you [submit an SLA credit request](#submit-sla-credit-request) to Microsoft, you must gather the following information to include in your support ticket:

- The customer tenant's GUID
- The [outage incident identifier](#outage-incident-identifier)?
- Were the impacted subscriptions purchased through CSP? (*yes* or *no*)

#### <a name="outage-incident-identifier"></a>Outage incident identifier

You can find the identifier for the outage incident on the **Service Health** page in the Microsoft 365 admin center. The **Outage Incident ID** is a number preceded by a two-letter abbreviation that indicates the affected service (for example, *EX25194* for an Exchange Online outage). The follow table describes common service abbreviations:

| Two-letter abbreviation | Microsoft service |
| ----------------------- | ----------------- |
| EX | Exchange Online |
| FO | Exchange Online Protection |
| SB | Skype for Business Online (formerly Lync Online) |
| SO | Assinatura do Office |
| PB | Power BI for Office 365 |
| SP | SharePoint Online |
| YA | Yammer Enterprise |
| MO | Portal error |

### <a name="submit-sla-credit-request"></a>Submit SLA credit request

To submit your SLA credit request to Microsoft through the Partner Center dashboard:

1. Sign in to the Partner Center dashboard.
2. In the left-hand menu, choose **Service requests**, then select **Partner support requests**.
3. On the **Partner request** page, choose **New request**.
4. On the **Start the request** page, find the section **CSP - customers, orders and subscriptions**. In this section, choose **Select an issue type**, then select **Customer services credit requests**.
5. On the **Recommended solutions** page, under **Do you need more help?** , choose **Yes**.
6. On the **Details** page, fill out the **Issue details** section. In the **Details** text box, be sure to enter the [required information](#required-information) that you gathered earlier.
7. Choose **Submit** to send in your SLA credit request.
