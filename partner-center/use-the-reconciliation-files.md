---
title: Use the reconciliation files | Partner Center
description: For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from the Partner Center dashboard.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: KPacquer
ms.openlocfilehash: de93fce5e689093f8e244b3812f682ef48bd47ea
ms.sourcegitcommit: 493122887ab9a5524590be12f5e1fedf4a004682
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/28/2017
---
# <a name="use-the-reconciliation-files"></a>Use the reconciliation files

**Applies to**

-  Partner Center
-  Partner Center for Microsoft Cloud for US Government
-  Partner Center for Microsoft Cloud Germany

For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from the Partner Center dashboard. The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).

## <a href="" id="itemizebypartner"></a>Itemize by partner


Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>MPN ID</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>MPN ID</td>
<td><p>The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</p></td>
</tr>
<tr class="even">
<td>Reseller MPN ID</td>
<td><p>Only appears on reconciliation files for partners in the indirect model.</p>
<p>The MPN ID of the reseller of record for the subscription. This corresponds to the reseller ID listed for the specific subscription in Partner Center.</p>
<p>eTo view or update the reseller, in the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list. In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list. Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</p>
<p>If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</p>
<p>If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</p>
<p>If the CSP partner removes a reseller ID, this value will be set to -1.</p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> License-based file fields


To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>Column</strong></td>
<td><strong>Description</strong></td>
<td><strong>Sample Value</strong></td>
</tr>
<tr class="even">
<td>PartnerId</td>
<td><p>Unique identifier for a specific billing entity, in GUID format. Not required for reconciliation, however may be useful information. Same in all rows.</p></td>
<td>8ddd03642-test-test-test-46b58d356b4e</td>
</tr>
<tr class="odd">
<td>CustomerID</td>
<td><p>Unique Microsoft ID, in GUID format, used to identify the customer.</p></td>
<td>12ABCD34-001A-BCD2-987C-3210ABCD5678</td>
</tr>
<tr class="even">
<td>OrderID</td>
<td><p>Unique identifier for an order in the Microsoft billing platform. May be useful to identify the order when contacting support but not for reconciliation.</p></td>
<td>566890604832738111</td>
</tr>
<tr class="odd">
<td>SubscriptionID</td>
<td><p>Unique identifier for a subscription in the Microsoft billing platform. May be useful to identify the subscription when contacting support but not for reconciliation.</p>
<p>This is not the same as the Subscription ID on the Partner Admin Console. Please see Syndication_Partner_Subscription_Number.</p></td>
<td>usCBMgAAAAAAAAIA</td>
</tr>
<tr class="even">
<td>SyndicationPartnerSubscriptionNumber</td>
<td><p>Unique identifier for subscriptions. A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</p>
<p>This field maps to the Subscription ID in the Partner Admin Console.</p></td>
<td>fb977ab5-test-test-test-24c8d9591708</td>
</tr>
<tr class="odd">
<td>OfferID</td>
<td><p>Unique offer ID. Standard offer ID as per price list.</p>
<p><b>Note</b>: This value does not match Offer ID from the price list. See DurableOfferID below.</p></td>
<td>FE616D64-E9A8-40EF-843F-152E9BBEF3D1</td>
</tr>
<tr class="even">
<td>DurableOfferID</td>
<td><p>Unique durable offer ID, as defined in the price list.</p>
<p><b>Note</b>: This value matches the Offer ID from the price list.</p></td>
<td>1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</td>
</tr>
<tr class="odd">
<td>OfferName</td>
<td><p>The name of the service offering purchased by the customer, as defined in the price list.</p></td>
<td>Microsoft Office 365 (Plan E3)</td>
</tr>
<tr class="even">
<td>SubscriptionStartDate</td>
<td><p>The subscription start date, set to the day after the order is submitted. By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</p>
<p>The time is always the beginning of the day, 0:00.</p></td>
<td>2/1/2015 0:00</td>
</tr>
<tr class="odd">
<td>SubscriptionEndDate</td>
<td><p>The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</p>
<p>At renewal, prices are updated to the current price list. Customer communication may be required in advance of automated renewal.</p>
<p>The time is always the beginning of the day, 0:00.</p></td>
<td>2/1/2015 0:00</td>
</tr>
<tr class="even">
<td>ChargeStartDate</td>
<td><p>Start day of the charges.</p>
<p>When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</p>
<p>The time is always the beginning of the day, 0:00.</p></td>
<td>2/1/2015 0:00</td>
</tr>
<tr class="odd">
<td>ChargeEndDate</td>
<td><p>End day of the charges.</p>
<p>When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</p>
<p>The time is always the end of the day, 23:59.</p></td>
<td>2/28/2015 23:59</td>
</tr>
<tr class="even">
<td>ChargeType</td>
<td><p>The type of charge or adjustment. See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></p></td>
<td><p>See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></p></td>
</tr>
<tr class="odd">
<td>UnitPrice</td>
<td><p>Price per seat. Ensure this matches the information stored in your billing system during reconciliation.</p></td>
<td>6.82</td>
</tr>
<tr class="even">
<td>Quantity</td>
<td><p>Number of seats. Ensure this matches the information stored in your billing system during reconciliation.</p></td>
<td>2</td>
</tr>
<tr class="odd">
<td>Amount</td>
<td><p>Total of price for quantity. Useful to check that the amount calculation matches how you calculate this for your customers.</p></td>
<td>13.32</td>
</tr>
<tr class="even">
<td>TotalOtherDiscount</td>
<td><p>Amount of discount applied to these charges. IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</p></td>
<td>2.32</td>
</tr>
<tr class="odd">
<td>Subtotal</td>
<td><p>Total before tax. Checks that your subtotal matches your expected total, in case of a discount.</p></td>
<td>11</td>
</tr>
<tr class="even">
<td>Tax</td>
<td><p>Tax amount charge, based on your market's tax rules and specific circumstances.</p></td>
<td>0</td>
</tr>
<tr class="odd">
<td>TotalForCustomer</td>
<td><p>Total after tax. Checks if you are charged tax in the invoice.</p></td>
<td>11</td>
</tr>
<tr class="even">
<td>Currency</td>
<td><p>Currency type. Each billing entity has only one currency. Check that it matches your first invoice and then after any major billing platform update.</p></td>
<td>EUR</td>
</tr>
<tr class="odd">
<td>CustomerName</td>
<td><p>Customer's organization name as reported in Partner Center. This is very important for reconciling the invoice with your system information.</p></td>
<td>Test Customer A</td>
</tr>
<tr class="even">
<td>MPNID</td>
<td><p>MPN ID of the CSP partner</p></td>
<td>4390934</td>
</tr>
<tr class="odd">
<td>ResellerMPNID</td>
<td><p>MPN ID of the reseller of record for the subscription. See [Itemize by partner](#itemizebypartner).</p></td>
<td>4390934</td>
</tr>
<tr class="even">
<td>DomainName</td>
<td><p>Customer's domain name, used to help identify the customer.</p></td>
<td>example.onmicrosoft.com</td>
</tr>
<tr class="odd">
<td>SubscriptionName</td>
<td><p>Subscription nickname. If no nickname is specified, Partner Center uses the OfferName.</p></td>
<td>PROJECT ONLINE</td>
</tr>
<tr class="even">
<td>SubscriptionDescription</td>
<td><p>The name of the service offering purchased by the customer, as defined in the price list. (This is an identical field to Offer name).</p></td>
<td>PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a>Usage-based file fields


To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.

The following fields explain which services were used and the rate.

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>Column</strong></td>
<td><strong>Description</strong></td>
<td><strong>Sample value</strong></td>
</tr>
<tr class="even">
<td>PartnerID</td>
<td><p>Partner ID, in GUID format.</p></td>
<td>DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</td>
</tr>
<tr class="odd">
<td>PartnerName</td>
<td><p>Partner Name.</p></td>
<td>Acme Incorporated</td>
</tr>
<tr class="even">
<td>PartnerBillableAccountID</td>
<td><p>Partner Account ID.</p></td>
<td>1010578050</td>
</tr>
<tr class="odd">
<td>CustomerName</td>
<td><p>Customer's organization name as reported in Partner Center. This is very important for reconciling the invoice with your system information.</p></td>
<td>Test Customer A</td>
</tr>
<tr class="even">
<td>MPNID</td>
<td><p>MPN ID of the CSP partner.</p></td>
<td>4390934</td>
</tr>
<tr class="odd">
<td>ResellerMPNID</td>
<td><p>MPN ID of the reseller of record for the subscription. See [Itemize by partner](#itemizebypartner).</p></td>
<td>4390934</td>
</tr>
<tr class="even">
<td>InvoiceNumber</td>
<td><p>Invoice number where the specified transaction appears.</p></td>
<td>D020001IVK</td>
</tr>
<tr class="odd">
<td>ChargeStartDate</td>
<td><p>Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</p>
<p>The time is always the beginning of the day, 0:00.</p></td>
<td>2/1/2014 0:00</td>
</tr>
<tr class="even">
<td>ChargeEndDate</td>
<td><p>End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</p>
<p>The time is always the end of the day, 23:59.</p></td>
<td>2/28/2014 23:59</td>
</tr>
<tr class="odd">
<td>SubscriptionID</td>
<td><p>Unique identifier for a subscription in the Microsoft billing platform. May be useful to identify the subscription when contacting support but not for reconciliation.</p>
<p>This is not the same as the Subscription ID on the Partner Admin Console.</p></td>
<td>usCBMgAAAAAAAAIA</td>
</tr>
<tr class="even">
<td>SubscriptionName</td>
<td><p>Nickname of the service offering.</p></td>
<td>Microsoft Azure</td>
</tr>
<tr class="odd">
<td>SubscriptionDescription</td>
<td><p>Line of business of the service offering</p></td>
<td>Microsoft Azure</td>
</tr>
<tr class="even">
<td>OrderID</td>
<td><p>Unique identifier for an order in the Microsoft billing platform. May be useful to identify the subscription when contacting support but not for reconciliation.</p></td>
<td>566890604832738111</td>
</tr>
<tr class="odd">
<td>ServiceName</td>
<td><p>The name of the Azure service in question.</p></td>
<td>VIRTUAL MACHINES</td>
</tr>
<tr class="even">
<td>ServiceType</td>
<td><p>The specific type of Windows Azure service.</p></td>
<td><ul>
<li>Service Bus – Individual or Pack</li>
<li>SQL Azure database – Business or Web Edition</li>
</ul></td>
</tr>
<tr class="odd">
<td>ResourceGUID</td>
<td><p>Specific unique identifier for all the service data and pricing structure.</p></td>
<td>DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</td>
</tr>
<tr class="even">
<td>Resource Name</td>
<td><p>The name of the Azure resource.</p></td>
<td><ul>
<li>Data Transfer In (GB)</li>
<li>Data Transfer Out (GB)</li>
</ul></td>
</tr>
<tr class="odd">
<td>Region</td>
<td><p>The region the usage applies to. Primarily used to assign rates to data transfers, as rates vary by region.</p></td>
<td>Asia Pacific, Europe, Latin America, North America</td>
</tr>
<tr class="even">
<td>SKU</td>
<td><p>MSFT unique identifier for offer</p></td>
<td>7UD-00001</td>
</tr>
<tr class="odd">
<td><p>DetailLineItemId</p></td>
<td><p>An ID and quantity for itemizing the different rates for a service or resource in a given billing period. For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</p></td>
<td>1</td>
</tr>
<tr class="even">
<td>ConsumedQuantity</td>
<td><p>The amount of service consumed (hours, GB, etc.) during the reporting period.</p>
<p>Also includes any unbilled usage from previous reporting periods.</p></td>
<td>11</td>
</tr>
<tr class="odd">
<td>IncludedQuantity</td>
<td><p>Units included as part of the offer. Not typically present in CSP.</p></td>
<td>0</td>
</tr>
<tr class="even">
<td><p>OverageQuantity</p></td>
<td><p>Units not included as part of the offer, that must be paid for by the partner.</p>
<p>Equal to the ConsumedQuantity - IncludedQuantity.</p></td>
<td>11</td>
</tr>
<tr class="odd">
<td>ListPrice</td>
<td><p>Offer price in effect at subscription start date.</p></td>
<td>$0.0808</td>
</tr>
<tr class="even">
<td>PretaxCharges</td>
<td><p>ListPrist times OverageQuantity, rounded to the nearest cent.</p></td>
<td>$0.085</td>
</tr>
<tr class="odd">
<td>TaxAmount</td>
<td><p>Tax amount charge, based on your market's tax rules and specific circumstances.</p></td>
<td>$0.08</td>
</tr>
<tr class="even">
<td>PostTaxTotal</td>
<td><p>Total after tax, when tax is applicable.</p></td>
<td>$0.93</td>
</tr>
<tr class="odd">
<td>Currency</td>
<td><p>Currency type. Each billing entity has only one currency. Check that it matches your first invoice and then after any major billing platform update.</p></td>
<td>EUR</td>
</tr>
<tr class="even">
<td>PretaxEffectiveRate</td>
<td><p>Pretax price per unit. Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</p></td>
<td>$0.08</td>
</tr>
<tr class="odd">
<td>PostTaxEffectiveRate</td>
<td><p>Post tax price per unit. Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</p></td>
<td>$0.08</td>
</tr>
<tr class="even">
<td>ChargeType</td>
<td><p>The type of charge or adjustment. See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></p></td>
<td><p>See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></p></td>
</tr>
<tr class="odd">
<td>CustomerBillableAccount</td>
<td><p>Unique account ID in the MSFT billing platform.</p></td>
<td>1280018095</td>
</tr>
<tr class="even">
<td>UsageDate</td>
<td><p>Date of service deployment.</p></td>
<td>2/1/2014 0:00</td>
</tr>
<tr class="odd">
<td>MeteredRegion</td>
<td><p>This column identifies the location of a data center within the region for services where this is applicable and populated.</p></td>
<td>East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</td>
</tr>
<tr class="even">
<td>MeteredService</td>
<td><p>This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column. For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column. This MeteredService column will indicate to which specific service the usage pertains.</p></td>
<td>AccessControl, CDN, Compute, Database, ServiceBus, Storage</td>
</tr>
<tr class="odd">
<td>MeteredServiceType</td>
<td><p>A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</p></td>
<td>EXTERNAL</td>
</tr>
<tr class="even">
<td>Project</td>
<td><p>Customer-defined name for their service instance</p></td>
<td>ORDDC52E52FDEF405786F0642DD0108BE4</td>
</tr>
<tr class="odd">
<td>ServiceInfo</td>
<td><p>The number of ServiceBus connections that were provisioned and utilized on a given day.</p></td>
<td>For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”. If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</td>
</tr>
<tr class="even">
<td>CustomerID</td>
<td><p>Unique Microsoft ID, in GUID format, used to identify the customer.</p></td>
<td>ORDDC52E52FDEF405786F0642DD0108BE4</td>
</tr>
<tr class="odd">
<td>DomainName</td>
<td><p>Customer's domain name, used to help identify the customer.</p></td>
<td>example.onmicrosoft.com</td></tr>
</tbody>
</table>



## <a href="" id="charge_types"></a>Mapping charges between an invoice and the reconciliation file

Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.

To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.

The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files. 

<table>
<tbody>
<tr>
<td>
<p><strong>Invoice charge description</strong></p>
</td>
<td>
<p><strong>Reconciliation file charge description (ChargeType column)</strong></p>
</td>
<td>
<p><strong>What is this charge?</strong></p>
</td>
<td>
<p><strong>How do I map these ChargeTypes to the invoice?</strong></p>
</td>
</tr>
<tr>
<td rowspan="8">
<p><strong>Recurring Charges</strong></p>
</td>
<td>
<p>Cancel instance prorate</p>
</td>
<td>
<p>Prorated charges refunded to the customer when associated seats are changed</p>
</td>
<td rowspan="8">
<p>From license-based file, sum the <strong>Amount</strong> column</p>
</td>
</tr>
<tr>
<td>
<p>Cycle fee</p>
</td>
<td>
<p>Periodic charges for a subscription</p>
</td>
</tr>
<tr>
<td>
<p>Cycle instance prorate</p>
</td>
<td>
<p>Prorated charges assessed from the customer when associated seats are changed</p>
</td>
</tr>
<tr>
<td>
<p>Prorate fees when cancel</p>
</td>
<td>
<p>Prorated refund for unused portion of service upon cancellation</p>
</td>
</tr>
<tr>
<td>
<p>Prorate fees when purchase</p>
</td>
<td>
<p>Prorated fees upon purchase</p>
</td>
</tr>
<tr>
<td>
<p>Purchase fee</p>
</td>
<td>
<p>Initial charge for a subscription</p>
</td>
</tr>
<tr>
<td>
<p>Prorate fee when renew</p>
</td>
<td>
<p>Prorated fees upon subscription renewal</p>
</td>
</tr>
<tr>
<td>
<p>Renew fee</p>
</td>
<td>
<p>Charge for renewing a subscription</p>
</td>
</tr>
<tr>
<td>
<p><strong>Other Products and Services</strong></p>
</td>
<td>
<p>Prorate fees when activate</p>
</td>
<td>
<p>Prorated fees from activation until end of billing period</p>
</td>
<td>
<p>From license-based file, sum the <strong>Amount</strong> column</p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong>Usage Charges</strong></p>
</td>
<td>
<p>Assess usage fee when cancel</p>
</td>
<td>
<p>Access usage fee upon cancellation for unpaid usage during the current billing period</p>
</td>
<td rowspan="2">
<p>From usage-based file, sum the <strong>PretaxCharges</strong> column</p>
</td>
</tr>
<tr>
<td>
<p>Assess usage fee for current cycle</p>
</td>
<td>
<p>Access usage fee for the current billing period</p>
</td>
</tr>
<tr>
<td>
<p><strong>Credits &amp; Adjustments</strong></p>
</td>
<td>
<p>Offset a line item</p>
</td>
<td>
<p>Partial or whole refund to a line item, including taxes</p>
</td>
<td>
<p>From license-based file, sum the <strong>TotalForCustomer</strong> column</p>
<p>From usage-based file, sum the <strong>PostTaxTotal</strong> column</p>
</td>
</tr>


<tr>
<td rowspan="4">
<p><strong>Other Discounts</strong></br>
<em>(usage-based)</em></p>
</td>
<td>
<p>Activation discount</p>
</td>
<td>
<p>Discount applied when subscription activated</p>
</td>
<td rowspan="4">
<p>From usage-based file, sum the <strong>PretaxCharges</strong> column</p>
</td>
</tr>
<tr>
<td>
<p>Cycle discount</p>
</td>
<td>
<p>Discount applied on periodic charges</p>
</td>
</tr><tr>
<td>
<p>Renew discount</p>
</td>
<td>
<p>Discount applied when subscription renewed</p>
</td>
</tr><tr>
<td>
<p>Cancel discount</p>
</td>
<td>
<p>Charges applied when discounts cancelled</p>
</td>
</tr>
<tr>
<td>
<p><strong>Other Discounts</strong></br>
<em>(license-based)</em></p>
</td>
<td>
<p><em>May be applied to multiple charge types</em></p>
</td>
<td>
<p>&nbsp;</p>
</td>
<td>
<p>From license-based file, sum the <strong>TotalOtherDiscount</strong> column</p>
</td>
</tr>
<tr>
<td>
<p><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></p>
</td>
<td>
<p><em>May be applied to multiple charge types</em></p>
<p><em>Exception: "Offset a line item" already includes taxes. See Credits &amp; Adjustments, above.</em></p>
</td>
<td>
<p>Taxes or value-added taxes (VAT)</p>
</td>
<td>
<p>From license-based file, sum the <strong>Tax</strong> column</p>
<p>From usage-based file, sum the <strong>TaxAmount</strong> column</p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
