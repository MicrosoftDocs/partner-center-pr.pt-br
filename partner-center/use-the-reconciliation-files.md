---
title: Usar os arquivos de reconciliação | Partner Center
ms.topic: article
ms.date: 10/29/2018
description: Para uma exibição detalhada do item de linha de cada encargo em um ciclo de cobrança, baixe os arquivos de reconciliação do Partner Center.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: KPacquer
ms.author: kenpacq
ms.localizationpriority: medium
ms.openlocfilehash: dac94723d8939f83628dfc8cd0992ab3516fa5a1
ms.sourcegitcommit: 3871c82c1075206a33eae7cd395a5a36edb2d1fc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/08/2019
ms.locfileid: "8995940"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="e7a85-103">Usar os arquivos de reconciliação</span><span class="sxs-lookup"><span data-stu-id="e7a85-103">Use the reconciliation files</span></span>

**<span data-ttu-id="e7a85-104">Aplicável a</span><span class="sxs-lookup"><span data-stu-id="e7a85-104">Applies to</span></span>**

-  <span data-ttu-id="e7a85-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="e7a85-105">Partner Center</span></span>
-  <span data-ttu-id="e7a85-106">Partner Center for Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="e7a85-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="e7a85-107">Para uma exibição detalhada do item de linha de cada encargo em um ciclo de cobrança, baixe os arquivos de reconciliação do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e7a85-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="e7a85-108">Os detalhes incluem encargos por assinaturas de cada cliente e eventos detalhados (como a adição de assentos a uma assinatura no meio do período).</span><span class="sxs-lookup"><span data-stu-id="e7a85-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="e7a85-109">Discriminar por parceiro</span><span class="sxs-lookup"><span data-stu-id="e7a85-109">Itemize by partner</span></span>


<span data-ttu-id="e7a85-110">Os parceiros no modelo indireto podem usar esses campos adicionais nos arquivos de reconciliação baseados em uso e em licença para discriminar por revendedor.</span><span class="sxs-lookup"><span data-stu-id="e7a85-110">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="e7a85-111">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="e7a85-111">MPN ID</span></span></th>
<th><span data-ttu-id="e7a85-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7a85-112">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="e7a85-113">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="e7a85-113">MPN ID</span></span></td>
<td><p><span data-ttu-id="e7a85-114">A ID do Microsoft Partner Network (MPN) do parceiro CSP (direta ou indireta).</span><span class="sxs-lookup"><span data-stu-id="e7a85-114">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e7a85-115">ID do MPN do revendedor</span><span class="sxs-lookup"><span data-stu-id="e7a85-115">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="e7a85-116">Só aparece em arquivos de reconciliação para parceiros no modelo indireto.</span><span class="sxs-lookup"><span data-stu-id="e7a85-116">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="e7a85-117">A ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="e7a85-117">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="e7a85-118">Isso corresponde à ID de revendedor listada para a assinatura específica no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e7a85-118">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="e7a85-119">Para exibir ou atualizar o revendedor, no menu Partner Center, selecione <strong>clientes</strong>e, em seguida, escolha o cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="e7a85-119">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="e7a85-120">No menu do cliente, selecione <strong>Assinaturas</strong>, escolha a assinatura na lista.</span><span class="sxs-lookup"><span data-stu-id="e7a85-120">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="e7a85-121">Selecione <strong>Atualizar</strong> para alterar o <strong>Revendedor (ID do MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="e7a85-121">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="e7a85-122">Se um parceiro CSP vendeu a assinatura diretamente para o cliente, sua ID do MPN estará listada duas vezes, como a ID do MPN e a ID do MPN do revendedor.</span><span class="sxs-lookup"><span data-stu-id="e7a85-122">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="e7a85-123">Se um parceiro CSP tiver um revendedor sem ID do MPN, esse valor será definido como a ID do MPN do parceiro.</span><span class="sxs-lookup"><span data-stu-id="e7a85-123">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="e7a85-124">Se o parceiro CSP remover uma ID de revendedor, esse valor será definido como -1.</span><span class="sxs-lookup"><span data-stu-id="e7a85-124">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="e7a85-125">Campos de arquivos baseado em licença</span><span class="sxs-lookup"><span data-stu-id="e7a85-125">License-based file fields</span></span>


<span data-ttu-id="e7a85-126">Para reconciliar seus encargos com os pedidos de seu cliente, compare o campo Syndication\_Partner\_Subscription\_Number do arquivo de reconciliação com a ID de Assinatura do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e7a85-126">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="e7a85-127">Coluna</span><span class="sxs-lookup"><span data-stu-id="e7a85-127">Column</span></span></strong></td>
<td><strong><span data-ttu-id="e7a85-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7a85-128">Description</span></span></strong></td>
<td><strong><span data-ttu-id="e7a85-129">Valor de exemplo</span><span class="sxs-lookup"><span data-stu-id="e7a85-129">Sample Value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e7a85-130">PartnerId</span><span class="sxs-lookup"><span data-stu-id="e7a85-130">PartnerId</span></span></td>
<td><p><span data-ttu-id="e7a85-131">Identificador exclusivo de uma entidade de cobrança específica, em formato GUID.</span><span class="sxs-lookup"><span data-stu-id="e7a85-131">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="e7a85-132">Não é necessário para reconciliação, mas pode ser uma informação útil.</span><span class="sxs-lookup"><span data-stu-id="e7a85-132">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="e7a85-133">O mesmo em todas as linhas.</span><span class="sxs-lookup"><span data-stu-id="e7a85-133">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="e7a85-134">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="e7a85-134">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e7a85-135">CustomerID</span><span class="sxs-lookup"><span data-stu-id="e7a85-135">CustomerID</span></span></td>
<td><p><span data-ttu-id="e7a85-136">ID exclusiva da Microsoft, no formato GUID, usada para identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="e7a85-136">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="e7a85-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="e7a85-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e7a85-138">OrderID</span><span class="sxs-lookup"><span data-stu-id="e7a85-138">OrderID</span></span></td>
<td><p><span data-ttu-id="e7a85-139">Identificador exclusivo para um pedido na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e7a85-139">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="e7a85-140">Pode ser útil para identificar o pedido ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="e7a85-140">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="e7a85-141">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="e7a85-141">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e7a85-142">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="e7a85-142">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="e7a85-143">Identificador exclusivo de uma assinatura na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e7a85-143">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="e7a85-144">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="e7a85-144">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="e7a85-145">Esse não é o mesmo que o ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="e7a85-145">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="e7a85-146">Consulte Número_Assinatura_Parceiro_Sindicalização.</span><span class="sxs-lookup"><span data-stu-id="e7a85-146">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="e7a85-147">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="e7a85-147">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e7a85-148">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="e7a85-148">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="e7a85-149">Identificador exclusivo para assinaturas.</span><span class="sxs-lookup"><span data-stu-id="e7a85-149">Unique identifier for subscriptions.</span></span> <span data-ttu-id="e7a85-150">Target: Um cliente pode ter várias assinaturas para o mesmo plano, portanto, isso é importante para análise de arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="e7a85-150">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="e7a85-151">Esse campo é mapeado para a ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="e7a85-151">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="e7a85-152">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="e7a85-152">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e7a85-153">OfferID</span><span class="sxs-lookup"><span data-stu-id="e7a85-153">OfferID</span></span></td>
<td><p><span data-ttu-id="e7a85-154">ID exclusivo da oferta.</span><span class="sxs-lookup"><span data-stu-id="e7a85-154">Unique offer ID.</span></span> <span data-ttu-id="e7a85-155">ID padrão da oferta de acordo com a lista de preços.</span><span class="sxs-lookup"><span data-stu-id="e7a85-155">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="e7a85-156"><b>Observação</b>: esse valor não coincide com a ID de oferta da lista de preços.</span><span class="sxs-lookup"><span data-stu-id="e7a85-156"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="e7a85-157">Veja DurableOfferID abaixo.</span><span class="sxs-lookup"><span data-stu-id="e7a85-157">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="e7a85-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="e7a85-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e7a85-159">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="e7a85-159">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="e7a85-160">ID exclusiva da oferta durável, conforme definido na tabela de preços.</span><span class="sxs-lookup"><span data-stu-id="e7a85-160">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="e7a85-161"><b>Observação</b>: esse valor corresponde à ID de oferta da lista de preços.</span><span class="sxs-lookup"><span data-stu-id="e7a85-161"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="e7a85-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="e7a85-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e7a85-163">OfferName</span><span class="sxs-lookup"><span data-stu-id="e7a85-163">OfferName</span></span></td>
<td><p><span data-ttu-id="e7a85-164">O nome da oferta de serviço comprada pelo cliente, conforme definido na tabela de preços.</span><span class="sxs-lookup"><span data-stu-id="e7a85-164">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="e7a85-165">Microsoft Office 365 (plano E3)</span><span class="sxs-lookup"><span data-stu-id="e7a85-165">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e7a85-166">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="e7a85-166">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="e7a85-167">A data de início da assinatura, definida como um dia após o pedido ser enviado.</span><span class="sxs-lookup"><span data-stu-id="e7a85-167">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="e7a85-168">Verificando a data de início da assinatura em conjunto com a data de término, você pode determinar se o cliente está dentro do primeiro ano da assinatura ou se a assinatura foi renovada para o ano seguinte.</span><span class="sxs-lookup"><span data-stu-id="e7a85-168">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="e7a85-169">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="e7a85-169">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="e7a85-170">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="e7a85-170">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e7a85-171">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="e7a85-171">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="e7a85-172">A data do término da assinatura: 12 meses + x dias após a data de início (para se alinhar com a data de cobrança do parceiro) ou 12 meses a partir da data de renovação.</span><span class="sxs-lookup"><span data-stu-id="e7a85-172">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="e7a85-173">Na renovação, os preços são atualizados com a tabela de preços atual.</span><span class="sxs-lookup"><span data-stu-id="e7a85-173">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="e7a85-174">Um comunicado ao cliente pode ser necessário antes da renovação automática.</span><span class="sxs-lookup"><span data-stu-id="e7a85-174">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="e7a85-175">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="e7a85-175">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="e7a85-176">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="e7a85-176">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e7a85-177">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="e7a85-177">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="e7a85-178">Dia de início dos encargos.</span><span class="sxs-lookup"><span data-stu-id="e7a85-178">Start day of the charges.</span></span></p>
<p><span data-ttu-id="e7a85-179">Quando o cliente muda o número de assentos, esse número é usado para calcular os encargos por dia (pro-rata).</span><span class="sxs-lookup"><span data-stu-id="e7a85-179">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="e7a85-180">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="e7a85-180">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="e7a85-181">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="e7a85-181">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e7a85-182">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="e7a85-182">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="e7a85-183">Dia do término dos encargos.</span><span class="sxs-lookup"><span data-stu-id="e7a85-183">End day of the charges.</span></span></p>
<p><span data-ttu-id="e7a85-184">Quando o cliente muda o número de assentos, esse número é usado para calcular os encargos por dia (pro-rata).</span><span class="sxs-lookup"><span data-stu-id="e7a85-184">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="e7a85-185">A hora é sempre o fim do dia, 23:59.</span><span class="sxs-lookup"><span data-stu-id="e7a85-185">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="e7a85-186">28/2/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="e7a85-186">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e7a85-187">ChargeType</span><span class="sxs-lookup"><span data-stu-id="e7a85-187">ChargeType</span></span></td>
<td><p><span data-ttu-id="e7a85-188">O tipo de encargo ou ajuste.</span><span class="sxs-lookup"><span data-stu-id="e7a85-188">The type of charge or adjustment.</span></span> <span data-ttu-id="e7a85-189">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="e7a85-189">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="e7a85-190">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="e7a85-190">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e7a85-191">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="e7a85-191">UnitPrice</span></span></td>
<td><p><span data-ttu-id="e7a85-192">Preço por estação, conforme publicado na lista de preços no momento da compra.</span><span class="sxs-lookup"><span data-stu-id="e7a85-192">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="e7a85-193">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="e7a85-193">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="e7a85-194">6.82</span><span class="sxs-lookup"><span data-stu-id="e7a85-194">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e7a85-195">Quantity</span><span class="sxs-lookup"><span data-stu-id="e7a85-195">Quantity</span></span></td>
<td><p><span data-ttu-id="e7a85-196">Número de assentos.</span><span class="sxs-lookup"><span data-stu-id="e7a85-196">Number of seats.</span></span> <span data-ttu-id="e7a85-197">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="e7a85-197">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="e7a85-198">2</span><span class="sxs-lookup"><span data-stu-id="e7a85-198">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e7a85-199">Quantidade</span><span class="sxs-lookup"><span data-stu-id="e7a85-199">Amount</span></span></td>
<td><p><span data-ttu-id="e7a85-200">Preço total por quantidade.</span><span class="sxs-lookup"><span data-stu-id="e7a85-200">Total of price for quantity.</span></span> <span data-ttu-id="e7a85-201">Útil para verificar se o cálculo do valor coincide com a forma como você calcula isso para seus clientes.</span><span class="sxs-lookup"><span data-stu-id="e7a85-201">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="e7a85-202">13.32</span><span class="sxs-lookup"><span data-stu-id="e7a85-202">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e7a85-203">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="e7a85-203">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="e7a85-204">Valor de desconto aplicado a esses encargos.</span><span class="sxs-lookup"><span data-stu-id="e7a85-204">Amount of discount applied to these charges.</span></span> <span data-ttu-id="e7a85-205">IUR ou novas assinaturas qualificadas para incentivo também conterão um valor de desconto nessa coluna.</span><span class="sxs-lookup"><span data-stu-id="e7a85-205">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="e7a85-206">2.32</span><span class="sxs-lookup"><span data-stu-id="e7a85-206">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e7a85-207">Subtotal</span><span class="sxs-lookup"><span data-stu-id="e7a85-207">Subtotal</span></span></td>
<td><p><span data-ttu-id="e7a85-208">Total sem imposto.</span><span class="sxs-lookup"><span data-stu-id="e7a85-208">Total before tax.</span></span> <span data-ttu-id="e7a85-209">Verifica se seu subtotal corresponde ao total esperado, em caso de desconto.</span><span class="sxs-lookup"><span data-stu-id="e7a85-209">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="e7a85-210">11</span><span class="sxs-lookup"><span data-stu-id="e7a85-210">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e7a85-211">Imposto</span><span class="sxs-lookup"><span data-stu-id="e7a85-211">Tax</span></span></td>
<td><p><span data-ttu-id="e7a85-212">Valor do imposto cobrado, com base em seu mercado & #39; s regras fiscais e em circunstâncias específicas.</span><span class="sxs-lookup"><span data-stu-id="e7a85-212">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="e7a85-213">0</span><span class="sxs-lookup"><span data-stu-id="e7a85-213">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e7a85-214">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="e7a85-214">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="e7a85-215">Total com imposto.</span><span class="sxs-lookup"><span data-stu-id="e7a85-215">Total after tax.</span></span> <span data-ttu-id="e7a85-216">Verifica se o imposto é cobrado na fatura.</span><span class="sxs-lookup"><span data-stu-id="e7a85-216">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="e7a85-217">11</span><span class="sxs-lookup"><span data-stu-id="e7a85-217">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e7a85-218">Moeda</span><span class="sxs-lookup"><span data-stu-id="e7a85-218">Currency</span></span></td>
<td><p><span data-ttu-id="e7a85-219">Tipo de moeda.</span><span class="sxs-lookup"><span data-stu-id="e7a85-219">Currency type.</span></span> <span data-ttu-id="e7a85-220">Cada entidade de cobrança tem somente uma moeda.</span><span class="sxs-lookup"><span data-stu-id="e7a85-220">Each billing entity has only one currency.</span></span> <span data-ttu-id="e7a85-221">Verifique se isso coincide com a primeira fatura e faça o mesmo após grandes atualizações na plataforma de cobrança.</span><span class="sxs-lookup"><span data-stu-id="e7a85-221">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="e7a85-222">Euro</span><span class="sxs-lookup"><span data-stu-id="e7a85-222">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e7a85-223">CustomerName</span><span class="sxs-lookup"><span data-stu-id="e7a85-223">CustomerName</span></span></td>
<td><p><span data-ttu-id="e7a85-224">Cliente & #39; o nome da organização s como informado no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e7a85-224">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="e7a85-225">Isso é muito importante para reconciliar a fatura com as informações de seu sistema.</span><span class="sxs-lookup"><span data-stu-id="e7a85-225">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="e7a85-226">Cliente de teste A</span><span class="sxs-lookup"><span data-stu-id="e7a85-226">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e7a85-227">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="e7a85-227">MPNID</span></span></td>
<td><p><span data-ttu-id="e7a85-228">ID do MPN do parceiro CSP</span><span class="sxs-lookup"><span data-stu-id="e7a85-228">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="e7a85-229">4390934</span><span class="sxs-lookup"><span data-stu-id="e7a85-229">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e7a85-230">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="e7a85-230">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="e7a85-231">ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="e7a85-231">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="e7a85-232">Consulte <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Discriminar por parceiro</a>.</span><span class="sxs-lookup"><span data-stu-id="e7a85-232">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="e7a85-233">4390934</span><span class="sxs-lookup"><span data-stu-id="e7a85-233">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e7a85-234">DomainName</span><span class="sxs-lookup"><span data-stu-id="e7a85-234">DomainName</span></span></td>
<td><p><span data-ttu-id="e7a85-235">Cliente & #39; o nome de domínio s, usado para ajudar a identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="e7a85-235">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="e7a85-236">Isso não deve ser usado para identificar exclusivamente o cliente como o cliente/parceiro pode atualizar o domínio banidos/padrão através do portal do O365.</span><span class="sxs-lookup"><span data-stu-id="e7a85-236">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="e7a85-237">Este campo pode aparecer em branco até o segundo ciclo de cobrança.</span><span class="sxs-lookup"><span data-stu-id="e7a85-237">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="e7a85-238">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="e7a85-238">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e7a85-239">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="e7a85-239">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="e7a85-240">Apelido da Inscrição.</span><span class="sxs-lookup"><span data-stu-id="e7a85-240">Subscription nickname.</span></span> <span data-ttu-id="e7a85-241">Se nenhum apelido for especificado, o Partner Center usa o OfferName.</span><span class="sxs-lookup"><span data-stu-id="e7a85-241">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="e7a85-242">PROJETO ONLINE</span><span class="sxs-lookup"><span data-stu-id="e7a85-242">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e7a85-243">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="e7a85-243">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="e7a85-244">O nome da oferta de serviço comprada pelo cliente, conforme definido na tabela de preços.</span><span class="sxs-lookup"><span data-stu-id="e7a85-244">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="e7a85-245">(Este é um campo idêntico ao nome da oferta).</span><span class="sxs-lookup"><span data-stu-id="e7a85-245">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="e7a85-246">PROJETO ONLINE PREMIUM SEM PROJETO CLIENTE</span><span class="sxs-lookup"><span data-stu-id="e7a85-246">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="e7a85-247">Campos de arquivo baseado em uso</span><span class="sxs-lookup"><span data-stu-id="e7a85-247">Usage-based file fields</span></span>


<span data-ttu-id="e7a85-248">Para reconciliar seus encargos com o uso de seu cliente, compare ResellerID/ResellerName/ResellerBillableAccount do arquivo de reconciliação com o nome do cliente e a ID da assinatura do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e7a85-248">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="e7a85-249">Os campos a seguir explicam quais serviços foram usados e a taxa.</span><span class="sxs-lookup"><span data-stu-id="e7a85-249">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="e7a85-250">Coluna</span><span class="sxs-lookup"><span data-stu-id="e7a85-250">Column</span></span></strong></td>
<td><strong><span data-ttu-id="e7a85-251">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7a85-251">Description</span></span></strong></td>
<td><strong><span data-ttu-id="e7a85-252">Valor de exemplo</span><span class="sxs-lookup"><span data-stu-id="e7a85-252">Sample value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e7a85-253">PartnerID</span><span class="sxs-lookup"><span data-stu-id="e7a85-253">PartnerID</span></span></td>
<td><p><span data-ttu-id="e7a85-254">ID do parceiro, no formato GUID.</span><span class="sxs-lookup"><span data-stu-id="e7a85-254">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="e7a85-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="e7a85-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e7a85-256">PartnerName</span><span class="sxs-lookup"><span data-stu-id="e7a85-256">PartnerName</span></span></td>
<td><p><span data-ttu-id="e7a85-257">Nome do parceiro.</span><span class="sxs-lookup"><span data-stu-id="e7a85-257">Partner Name.</span></span></p></td>
<td><span data-ttu-id="e7a85-258">Acme incorporado</span><span class="sxs-lookup"><span data-stu-id="e7a85-258">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e7a85-259">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="e7a85-259">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="e7a85-260">ID da conta do parceiro.</span><span class="sxs-lookup"><span data-stu-id="e7a85-260">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="e7a85-261">1010578050</span><span class="sxs-lookup"><span data-stu-id="e7a85-261">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e7a85-262">CustomerName</span><span class="sxs-lookup"><span data-stu-id="e7a85-262">CustomerName</span></span></td>
<td><p><span data-ttu-id="e7a85-263">Cliente & #39; o nome da organização s como informado no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e7a85-263">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="e7a85-264">Isso é muito importante para reconciliar a fatura com as informações de seu sistema.</span><span class="sxs-lookup"><span data-stu-id="e7a85-264">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="e7a85-265">Cliente de teste A</span><span class="sxs-lookup"><span data-stu-id="e7a85-265">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e7a85-266">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="e7a85-266">MPNID</span></span></td>
<td><p><span data-ttu-id="e7a85-267">ID do MPN do parceiro CSP.</span><span class="sxs-lookup"><span data-stu-id="e7a85-267">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="e7a85-268">4390934</span><span class="sxs-lookup"><span data-stu-id="e7a85-268">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e7a85-269">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="e7a85-269">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="e7a85-270">ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="e7a85-270">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="e7a85-271">Consulte <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Discriminar por parceiro</a>.</span><span class="sxs-lookup"><span data-stu-id="e7a85-271">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="e7a85-272">4390934</span><span class="sxs-lookup"><span data-stu-id="e7a85-272">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e7a85-273">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="e7a85-273">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="e7a85-274">Número da fatura na qual a transação especificada é exibida.</span><span class="sxs-lookup"><span data-stu-id="e7a85-274">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="e7a85-275">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="e7a85-275">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e7a85-276">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="e7a85-276">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="e7a85-277">Data de início do ciclo de cobrança exceto quando apresentadas as datas de dados de uso latentes anteriormente não cobradas (do ciclo de cobrança anterior).</span><span class="sxs-lookup"><span data-stu-id="e7a85-277">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="e7a85-278">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="e7a85-278">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="e7a85-279">1/2/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="e7a85-279">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e7a85-280">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="e7a85-280">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="e7a85-281">Data de término do ciclo de cobrança exceto quando apresentadas as datas de dados de uso latentes anteriormente não cobradas (do ciclo de cobrança anterior).</span><span class="sxs-lookup"><span data-stu-id="e7a85-281">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="e7a85-282">A hora é sempre o fim do dia, 23:59.</span><span class="sxs-lookup"><span data-stu-id="e7a85-282">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="e7a85-283">28/2/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="e7a85-283">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e7a85-284">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="e7a85-284">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="e7a85-285">Identificador exclusivo de uma assinatura na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e7a85-285">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="e7a85-286">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="e7a85-286">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="e7a85-287">Esse não é o mesmo que a ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="e7a85-287">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="e7a85-288">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="e7a85-288">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e7a85-289">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="e7a85-289">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="e7a85-290">Apelido da oferta do serviço.</span><span class="sxs-lookup"><span data-stu-id="e7a85-290">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="e7a85-291">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="e7a85-291">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e7a85-292">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="e7a85-292">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="e7a85-293">Linha de negócios da oferta do serviço</span><span class="sxs-lookup"><span data-stu-id="e7a85-293">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="e7a85-294">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="e7a85-294">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e7a85-295">OrderID</span><span class="sxs-lookup"><span data-stu-id="e7a85-295">OrderID</span></span></td>
<td><p><span data-ttu-id="e7a85-296">Identificador exclusivo para um pedido na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e7a85-296">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="e7a85-297">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="e7a85-297">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="e7a85-298">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="e7a85-298">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e7a85-299">ServiceName</span><span class="sxs-lookup"><span data-stu-id="e7a85-299">ServiceName</span></span></td>
<td><p><span data-ttu-id="e7a85-300">O nome do serviço do Azure em questão.</span><span class="sxs-lookup"><span data-stu-id="e7a85-300">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="e7a85-301">MÁQUINAS VIRTUAIS</span><span class="sxs-lookup"><span data-stu-id="e7a85-301">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e7a85-302">ServiceType</span><span class="sxs-lookup"><span data-stu-id="e7a85-302">ServiceType</span></span></td>
<td><p><span data-ttu-id="e7a85-303">O tipo específico de serviço do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="e7a85-303">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="e7a85-304">Service Bus – Individual ou pacote</span><span class="sxs-lookup"><span data-stu-id="e7a85-304">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="e7a85-305">Banco de dados SQL Azure – Edição empresa ou Web</span><span class="sxs-lookup"><span data-stu-id="e7a85-305">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e7a85-306">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="e7a85-306">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="e7a85-307">Identificador exclusivo específico de toda a estrutura de serviço de dados e preço.</span><span class="sxs-lookup"><span data-stu-id="e7a85-307">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="e7a85-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="e7a85-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e7a85-309">Nome do recurso</span><span class="sxs-lookup"><span data-stu-id="e7a85-309">Resource Name</span></span></td>
<td><p><span data-ttu-id="e7a85-310">O nome do recurso do Azure.</span><span class="sxs-lookup"><span data-stu-id="e7a85-310">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="e7a85-311">Dados de entrada transferidos (GB)</span><span class="sxs-lookup"><span data-stu-id="e7a85-311">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="e7a85-312">Dados de saída transferidos (GB)</span><span class="sxs-lookup"><span data-stu-id="e7a85-312">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e7a85-313">Região</span><span class="sxs-lookup"><span data-stu-id="e7a85-313">Region</span></span></td>
<td><p><span data-ttu-id="e7a85-314">A região a qual o uso se aplica.</span><span class="sxs-lookup"><span data-stu-id="e7a85-314">The region the usage applies to.</span></span> <span data-ttu-id="e7a85-315">Usado principalmente para atribuir as taxas de transferências de dados, já que as taxas variam de acordo com a região.</span><span class="sxs-lookup"><span data-stu-id="e7a85-315">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="e7a85-316">Pacífico Asiático, Europa, América Latina e América do Norte</span><span class="sxs-lookup"><span data-stu-id="e7a85-316">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e7a85-317">SKU</span><span class="sxs-lookup"><span data-stu-id="e7a85-317">SKU</span></span></td>
<td><p><span data-ttu-id="e7a85-318">Identificador exclusivo MSFT da oferta</span><span class="sxs-lookup"><span data-stu-id="e7a85-318">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="e7a85-319">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="e7a85-319">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="e7a85-320">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="e7a85-320">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="e7a85-321">Uma ID e a quantidade para discriminar as taxas diferentes de um serviço ou recurso em um determinado período de cobrança.</span><span class="sxs-lookup"><span data-stu-id="e7a85-321">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="e7a85-322">Para a classificação em camadas do Azure, pode haver uma taxa para uma determinada quantidade de unidades faturáveis e uma taxa diferente depois disso.</span><span class="sxs-lookup"><span data-stu-id="e7a85-322">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="e7a85-323">1</span><span class="sxs-lookup"><span data-stu-id="e7a85-323">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e7a85-324">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="e7a85-324">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="e7a85-325">A quantidade de serviço consumida (horas, GB etc.) durante o período de relatório.</span><span class="sxs-lookup"><span data-stu-id="e7a85-325">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="e7a85-326">Também inclui qualquer uso não cobrado de períodos de relatório anteriores.</span><span class="sxs-lookup"><span data-stu-id="e7a85-326">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="e7a85-327">11</span><span class="sxs-lookup"><span data-stu-id="e7a85-327">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e7a85-328">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="e7a85-328">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="e7a85-329">Unidades incluídas como parte da oferta.</span><span class="sxs-lookup"><span data-stu-id="e7a85-329">Units included as part of the offer.</span></span> <span data-ttu-id="e7a85-330">Normalmente não está presente no CSP.</span><span class="sxs-lookup"><span data-stu-id="e7a85-330">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="e7a85-331">0</span><span class="sxs-lookup"><span data-stu-id="e7a85-331">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="e7a85-332">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="e7a85-332">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="e7a85-333">Unidades não incluídas como parte da oferta devem ser pagas pelo parceiro.</span><span class="sxs-lookup"><span data-stu-id="e7a85-333">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="e7a85-334">Igual a ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="e7a85-334">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="e7a85-335">11</span><span class="sxs-lookup"><span data-stu-id="e7a85-335">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e7a85-336">ListPrice</span><span class="sxs-lookup"><span data-stu-id="e7a85-336">ListPrice</span></span></td>
<td><p><span data-ttu-id="e7a85-337">Preço da oferta em vigor na data de início da assinatura.</span><span class="sxs-lookup"><span data-stu-id="e7a85-337">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="e7a85-338">U$ 0,0808</span><span class="sxs-lookup"><span data-stu-id="e7a85-338">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e7a85-339">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="e7a85-339">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="e7a85-340">ListPrist vezes OverageQuantity, arredondado para o centavo mais próximo.</span><span class="sxs-lookup"><span data-stu-id="e7a85-340">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="e7a85-341">U$ 0,085</span><span class="sxs-lookup"><span data-stu-id="e7a85-341">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e7a85-342">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="e7a85-342">TaxAmount</span></span></td>
<td><p><span data-ttu-id="e7a85-343">Valor do imposto cobrado, com base em seu mercado & #39; s regras fiscais e em circunstâncias específicas.</span><span class="sxs-lookup"><span data-stu-id="e7a85-343">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="e7a85-344">U$ 0,08</span><span class="sxs-lookup"><span data-stu-id="e7a85-344">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e7a85-345">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="e7a85-345">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="e7a85-346">Total após imposto, quando o imposto é aplicável.</span><span class="sxs-lookup"><span data-stu-id="e7a85-346">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="e7a85-347">U$ 0,93</span><span class="sxs-lookup"><span data-stu-id="e7a85-347">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e7a85-348">Moeda</span><span class="sxs-lookup"><span data-stu-id="e7a85-348">Currency</span></span></td>
<td><p><span data-ttu-id="e7a85-349">Tipo de moeda.</span><span class="sxs-lookup"><span data-stu-id="e7a85-349">Currency type.</span></span> <span data-ttu-id="e7a85-350">Cada entidade de cobrança tem somente uma moeda.</span><span class="sxs-lookup"><span data-stu-id="e7a85-350">Each billing entity has only one currency.</span></span> <span data-ttu-id="e7a85-351">Verifique se isso coincide com a primeira fatura e faça o mesmo após grandes atualizações na plataforma de cobrança.</span><span class="sxs-lookup"><span data-stu-id="e7a85-351">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="e7a85-352">Euro</span><span class="sxs-lookup"><span data-stu-id="e7a85-352">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e7a85-353">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="e7a85-353">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="e7a85-354">Preço por unidade sem imposto.</span><span class="sxs-lookup"><span data-stu-id="e7a85-354">Pretax price per unit.</span></span> <span data-ttu-id="e7a85-355">Igual a PretaxCharges / OverageQuantity, arredondado para o centavo mais próximo.</span><span class="sxs-lookup"><span data-stu-id="e7a85-355">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="e7a85-356">U$ 0,08</span><span class="sxs-lookup"><span data-stu-id="e7a85-356">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e7a85-357">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="e7a85-357">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="e7a85-358">Preço pós-imposto por unidade.</span><span class="sxs-lookup"><span data-stu-id="e7a85-358">Post tax price per unit.</span></span> <span data-ttu-id="e7a85-359">Igual a PostTaxTotal / OverageQuantity, ou PretaxEffectiveRate + taxa de imposto por valor de unidade, arredondado para o centavo mais próximo.</span><span class="sxs-lookup"><span data-stu-id="e7a85-359">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="e7a85-360">U$ 0,08</span><span class="sxs-lookup"><span data-stu-id="e7a85-360">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e7a85-361">ChargeType</span><span class="sxs-lookup"><span data-stu-id="e7a85-361">ChargeType</span></span></td>
<td><p><span data-ttu-id="e7a85-362">O tipo de encargo ou ajuste.</span><span class="sxs-lookup"><span data-stu-id="e7a85-362">The type of charge or adjustment.</span></span> <span data-ttu-id="e7a85-363">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="e7a85-363">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="e7a85-364">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="e7a85-364">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e7a85-365">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="e7a85-365">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="e7a85-366">ID exclusiva da conta na plataforma de cobrança da MSFT.</span><span class="sxs-lookup"><span data-stu-id="e7a85-366">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="e7a85-367">1280018095</span><span class="sxs-lookup"><span data-stu-id="e7a85-367">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e7a85-368">UsageDate</span><span class="sxs-lookup"><span data-stu-id="e7a85-368">UsageDate</span></span></td>
<td><p><span data-ttu-id="e7a85-369">Data da implantação do serviço.</span><span class="sxs-lookup"><span data-stu-id="e7a85-369">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="e7a85-370">1/2/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="e7a85-370">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e7a85-371">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="e7a85-371">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="e7a85-372">Essa coluna identifica a localização de um data center dentro da região para serviços onde isso é aplicável e preenchido.</span><span class="sxs-lookup"><span data-stu-id="e7a85-372">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="e7a85-373">Leste da Ásia, Sudeste da Ásia, Norte da Europa, Europa Ocidental, Centro Norte e Centro Sul dos EUA</span><span class="sxs-lookup"><span data-stu-id="e7a85-373">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e7a85-374">MeteredService</span><span class="sxs-lookup"><span data-stu-id="e7a85-374">MeteredService</span></span></td>
<td><p><span data-ttu-id="e7a85-375">Essa coluna é utilizada para rastrear o serviço do Microsoft Azure individual que não pode ser identificado especificamente na coluna Nome do Serviço.</span><span class="sxs-lookup"><span data-stu-id="e7a85-375">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="e7a85-376">Por exemplo, transferências de dados são relatadas como &quot;Microsoft Azure – Todos os Serviços&quot; na coluna Nome do Serviço.</span><span class="sxs-lookup"><span data-stu-id="e7a85-376">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="e7a85-377">Essa coluna MeteredService indicará ao qual serviço específico o uso pertence.</span><span class="sxs-lookup"><span data-stu-id="e7a85-377">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="e7a85-378">AccessControl, CDN, Computação, Banco de dados, ServiceBus, Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e7a85-378">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e7a85-379">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="e7a85-379">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="e7a85-380">Um subcabeçalho que esclarece ainda mais o serviço Microsoft Azure individual além do nível fornecido pelo campo MeteredService.</span><span class="sxs-lookup"><span data-stu-id="e7a85-380">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="e7a85-381">EXTERNO</span><span class="sxs-lookup"><span data-stu-id="e7a85-381">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e7a85-382">Projeto</span><span class="sxs-lookup"><span data-stu-id="e7a85-382">Project</span></span></td>
<td><p><span data-ttu-id="e7a85-383">Nome definido pelo cliente para a instância do serviço</span><span class="sxs-lookup"><span data-stu-id="e7a85-383">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="e7a85-384">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="e7a85-384">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e7a85-385">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="e7a85-385">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="e7a85-386">O número de conexões ServiceBus que foram provisionados e utilizados em um dia específico.</span><span class="sxs-lookup"><span data-stu-id="e7a85-386">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="e7a85-387">Por exemplo: se você tivesse uma conexão individualmente provisionada durante um mês de 30 dias, a coluna Informação do Serviço 1 lerá "1,000000 conexões/30 dias".</span><span class="sxs-lookup"><span data-stu-id="e7a85-387">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="e7a85-388">Se você tinha um pacote de 25 conexões ServiceBus provisionadas e você utilizou 1 durante o dia, sua declaração de uso diário para esse dia indicaria "25 conexões/30 dias – Usado: 1,000000".</span><span class="sxs-lookup"><span data-stu-id="e7a85-388">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e7a85-389">CustomerID</span><span class="sxs-lookup"><span data-stu-id="e7a85-389">CustomerID</span></span></td>
<td><p><span data-ttu-id="e7a85-390">ID exclusiva da Microsoft, no formato GUID, usada para identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="e7a85-390">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="e7a85-391">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="e7a85-391">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e7a85-392">DomainName</span><span class="sxs-lookup"><span data-stu-id="e7a85-392">DomainName</span></span></td>
<td><p><span data-ttu-id="e7a85-393">Cliente & #39; o nome de domínio s, usado para ajudar a identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="e7a85-393">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="e7a85-394">Este campo pode aparecer em branco até o segundo ciclo de cobrança.</span><span class="sxs-lookup"><span data-stu-id="e7a85-394">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="e7a85-395">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="e7a85-395">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="e7a85-396">Unidade</span><span class="sxs-lookup"><span data-stu-id="e7a85-396">Unit</span></span></td>
<td><p><span data-ttu-id="e7a85-397">A unidade do nome do recurso</span><span class="sxs-lookup"><span data-stu-id="e7a85-397">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="e7a85-398">GB ou HORAS</span><span class="sxs-lookup"><span data-stu-id="e7a85-398">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="onetimefiles"></a><span data-ttu-id="e7a85-399">Campos de arquivo de compra única</span><span class="sxs-lookup"><span data-stu-id="e7a85-399">One-time purchase file fields</span></span>

|**<span data-ttu-id="e7a85-400">Campo</span><span class="sxs-lookup"><span data-stu-id="e7a85-400">Field</span></span>** |**<span data-ttu-id="e7a85-401">Definição</span><span class="sxs-lookup"><span data-stu-id="e7a85-401">Definition</span></span>**|
|:----------------|:-----------------------------|
|<span data-ttu-id="e7a85-402">PartnerId</span><span class="sxs-lookup"><span data-stu-id="e7a85-402">PartnerId</span></span> |<span data-ttu-id="e7a85-403">ID do parceiro, no formato GUID.</span><span class="sxs-lookup"><span data-stu-id="e7a85-403">Partner ID, in GUID format.</span></span> |
|<span data-ttu-id="e7a85-404">CustomerID</span><span class="sxs-lookup"><span data-stu-id="e7a85-404">CustomerId</span></span> |<span data-ttu-id="e7a85-405">ID exclusiva da Microsoft, no formato GUID, usada para identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="e7a85-405">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span> |
|<span data-ttu-id="e7a85-406">CustomerName</span><span class="sxs-lookup"><span data-stu-id="e7a85-406">CustomerName</span></span> |<span data-ttu-id="e7a85-407">Nome da organização do cliente como informado no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e7a85-407">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="e7a85-408">Isso é muito importante para reconciliar a fatura com as informações de seu sistema.</span><span class="sxs-lookup"><span data-stu-id="e7a85-408">This is very important for reconciling the invoice with your system information.</span></span> |
|<span data-ttu-id="e7a85-409">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="e7a85-409">CustomerDomainName</span></span> |<span data-ttu-id="e7a85-410">O nome de domínio do cliente.</span><span class="sxs-lookup"><span data-stu-id="e7a85-410">The customer’s domain name.</span></span> |
|<span data-ttu-id="e7a85-411">CustomerCountry</span><span class="sxs-lookup"><span data-stu-id="e7a85-411">CustomerCountry</span></span> |<span data-ttu-id="e7a85-412">O país em que o cliente está localizado.</span><span class="sxs-lookup"><span data-stu-id="e7a85-412">The country in which the customer is located.</span></span> |
|<span data-ttu-id="e7a85-413">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="e7a85-413">InvoiceNumber</span></span> |<span data-ttu-id="e7a85-414">Número da fatura na qual a transação especificada é exibida.</span><span class="sxs-lookup"><span data-stu-id="e7a85-414">Invoice number where the specified transaction appears.</span></span> |
|<span data-ttu-id="e7a85-415">MpnId</span><span class="sxs-lookup"><span data-stu-id="e7a85-415">MpnId</span></span> |<span data-ttu-id="e7a85-416">ID do MPN do parceiro CSP (direto ou indireto).</span><span class="sxs-lookup"><span data-stu-id="e7a85-416">MPN ID of the CSP partner (direct or indirect).</span></span> |
|<span data-ttu-id="e7a85-417">ID do MPN do revendedor</span><span class="sxs-lookup"><span data-stu-id="e7a85-417">Reseller MPN ID</span></span> |<span data-ttu-id="e7a85-418">Só aparece em arquivos de reconciliação para parceiros no modelo indireto.</span><span class="sxs-lookup"><span data-stu-id="e7a85-418">Only appears on reconciliation files for partners in the indirect model.</span></span> <span data-ttu-id="e7a85-419">A ID do MPN do revendedor de registro da reserva.</span><span class="sxs-lookup"><span data-stu-id="e7a85-419">The MPN ID of the reseller of record for the reservation.</span></span> <span data-ttu-id="e7a85-420">Isso corresponde à ID de revendedor listada para a reserva específica no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e7a85-420">This corresponds to the reseller ID listed for the specific reservation in Partner Center.</span></span> <span data-ttu-id="e7a85-421">Se um parceiro CSP vendeu a reserva diretamente para o cliente, sua ID do MPN estará listada duas vezes, como a ID do MPN e a ID do MPN do revendedor.</span><span class="sxs-lookup"><span data-stu-id="e7a85-421">If a CSP partner sold the reservation directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span> <span data-ttu-id="e7a85-422">Se um parceiro CSP tiver um revendedor sem ID do MPN, esse valor será definido como a ID do MPN do parceiro.</span><span class="sxs-lookup"><span data-stu-id="e7a85-422">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span> <span data-ttu-id="e7a85-423">Se o parceiro CSP remover uma ID de revendedor, esse valor será definido como -1.</span><span class="sxs-lookup"><span data-stu-id="e7a85-423">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span> |
|<span data-ttu-id="e7a85-424">OrderId</span><span class="sxs-lookup"><span data-stu-id="e7a85-424">OrderId</span></span> |<span data-ttu-id="e7a85-425">Identificador exclusivo para um pedido na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e7a85-425">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="e7a85-426">Pode ser útil para identificar a reserva do Azure ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="e7a85-426">May be useful to identify the Azure reservation when contacting support but not for reconciliation.</span></span> |
|<span data-ttu-id="e7a85-427">OrderDate</span><span class="sxs-lookup"><span data-stu-id="e7a85-427">OrderDate</span></span> |<span data-ttu-id="e7a85-428">A data em que o pedido foi feito.</span><span class="sxs-lookup"><span data-stu-id="e7a85-428">The date the order was placed.</span></span> |
|<span data-ttu-id="e7a85-429">ProductId</span><span class="sxs-lookup"><span data-stu-id="e7a85-429">ProductId</span></span> |<span data-ttu-id="e7a85-430">A ID do produto.</span><span class="sxs-lookup"><span data-stu-id="e7a85-430">The ID for the product.</span></span> |
|<span data-ttu-id="e7a85-431">SkuId</span><span class="sxs-lookup"><span data-stu-id="e7a85-431">SkuId</span></span>  |<span data-ttu-id="e7a85-432">A ID de uma SKU em particular.</span><span class="sxs-lookup"><span data-stu-id="e7a85-432">The ID for a particular SKU.</span></span> |
|<span data-ttu-id="e7a85-433">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="e7a85-433">AvailabilityId</span></span> |<span data-ttu-id="e7a85-434">A ID de uma Disponibilidade em particular.</span><span class="sxs-lookup"><span data-stu-id="e7a85-434">The ID for a particular Availability.</span></span> <span data-ttu-id="e7a85-435">"Disponibilidade" refere-se a se uma SKU em particular está disponível ou não para compra para determinado país, moeda, segmento do setor etc.</span><span class="sxs-lookup"><span data-stu-id="e7a85-435">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span> |
|<span data-ttu-id="e7a85-436">SkuName</span><span class="sxs-lookup"><span data-stu-id="e7a85-436">SkuName</span></span>  |<span data-ttu-id="e7a85-437">O título de uma SKU em particular.</span><span class="sxs-lookup"><span data-stu-id="e7a85-437">The title for a particular SKU.</span></span> |
|<span data-ttu-id="e7a85-438">ProductName</span><span class="sxs-lookup"><span data-stu-id="e7a85-438">ProductName</span></span> |<span data-ttu-id="e7a85-439">O nome do produto.</span><span class="sxs-lookup"><span data-stu-id="e7a85-439">The name of the product.</span></span> |
|<span data-ttu-id="e7a85-440">ChargeType</span><span class="sxs-lookup"><span data-stu-id="e7a85-440">ChargeType</span></span> |<span data-ttu-id="e7a85-441">O tipo de encargo ou ajuste.</span><span class="sxs-lookup"><span data-stu-id="e7a85-441">The type of charge or adjustment.</span></span> |
|<span data-ttu-id="e7a85-442">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="e7a85-442">UnitPrice</span></span> |<span data-ttu-id="e7a85-443">Preço por produto pedido.</span><span class="sxs-lookup"><span data-stu-id="e7a85-443">Price per product ordered.</span></span> |
|<span data-ttu-id="e7a85-444">Quantidade</span><span class="sxs-lookup"><span data-stu-id="e7a85-444">Quantity</span></span> |<span data-ttu-id="e7a85-445">Número de produtos pedidos.</span><span class="sxs-lookup"><span data-stu-id="e7a85-445">Number of products ordered.</span></span> |
|<span data-ttu-id="e7a85-446">Subtotal</span><span class="sxs-lookup"><span data-stu-id="e7a85-446">Subtotal</span></span> |<span data-ttu-id="e7a85-447">Total sem imposto.</span><span class="sxs-lookup"><span data-stu-id="e7a85-447">Total before tax.</span></span> <span data-ttu-id="e7a85-448">Verifica se seu subtotal corresponde ao total esperado, em caso de desconto.</span><span class="sxs-lookup"><span data-stu-id="e7a85-448">Checks that your subtotal matches your expected total, in case of a discount.</span></span> |
|<span data-ttu-id="e7a85-449">TaxTotal</span><span class="sxs-lookup"><span data-stu-id="e7a85-449">TaxTotal</span></span> |<span data-ttu-id="e7a85-450">O total de todos os impostos aplicáveis.</span><span class="sxs-lookup"><span data-stu-id="e7a85-450">The total of all applicable taxes.</span></span> |
|<span data-ttu-id="e7a85-451">Total</span><span class="sxs-lookup"><span data-stu-id="e7a85-451">Total</span></span> |<span data-ttu-id="e7a85-452">O valor total desta compra.</span><span class="sxs-lookup"><span data-stu-id="e7a85-452">The total amount of this purchase.</span></span> |
|<span data-ttu-id="e7a85-453">Moeda</span><span class="sxs-lookup"><span data-stu-id="e7a85-453">Currency</span></span> |<span data-ttu-id="e7a85-454">Tipo de moeda.</span><span class="sxs-lookup"><span data-stu-id="e7a85-454">Currency type.</span></span> <span data-ttu-id="e7a85-455">Cada entidade de cobrança tem somente uma moeda.</span><span class="sxs-lookup"><span data-stu-id="e7a85-455">Each billing entity has only one currency.</span></span> <span data-ttu-id="e7a85-456">Verifique se isso coincide com a primeira fatura e faça o mesmo após grandes atualizações na plataforma de cobrança.</span><span class="sxs-lookup"><span data-stu-id="e7a85-456">Check that it matches your first invoice and then after any major billing platform update.</span></span> |
|<span data-ttu-id="e7a85-457">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="e7a85-457">DiscountDetails</span></span> |<span data-ttu-id="e7a85-458">Lista detalhada dos descontos relevantes.</span><span class="sxs-lookup"><span data-stu-id="e7a85-458">Detailed listing of any relevant discounts.</span></span> |



## <a href="" id="charge_types"></a><span data-ttu-id="e7a85-459">Como mapear encargos entre uma fatura e o arquivo de reconciliação</span><span class="sxs-lookup"><span data-stu-id="e7a85-459">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="e7a85-460">Sua fatura fornece um resumo dos encargos, enquanto seu arquivo de reconciliação fornece uma divisão detalhada das transações de item de linha, incluindo os tipos de carga.</span><span class="sxs-lookup"><span data-stu-id="e7a85-460">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="e7a85-461">Para fazer referência cruzada das quantidades de carga entre o arquivo de reconciliação e fatura, você pode usar opções de filtro do Microsoft Excel para filtrar por tipos de cobrança no arquivo de reconciliação para mapear os encargos de fatura em um conjunto de detalhamentos de cobrança no arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="e7a85-461">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="e7a85-462">Os arquivos de reconciliação, tanto os baseados em licença quanto os baseados em uso, mostram apenas encargos e transações relacionadas ao uso (unidades consumidas e encargos relacionados).</span><span class="sxs-lookup"><span data-stu-id="e7a85-462">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="e7a85-463">Créditos únicos, descontos ou reembolsos que aparecem na fatura como "Ajustes" não são mostrados no arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="e7a85-463">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="e7a85-464">A tabela a seguir mostra os mapeamentos entre uma seção da fatura e os tipos de encargo associados que podem aparecer nos arquivos de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="e7a85-464">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><strong><span data-ttu-id="e7a85-465">Descrição do encargo da fatura</span><span class="sxs-lookup"><span data-stu-id="e7a85-465">Invoice charge description</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="e7a85-466">Descrição do encargo do arquivo de reconciliação (coluna ChargeType)</span><span class="sxs-lookup"><span data-stu-id="e7a85-466">Reconciliation file charge description (ChargeType column)</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="e7a85-467">O que é este encargo?</span><span class="sxs-lookup"><span data-stu-id="e7a85-467">What is this charge?</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="e7a85-468">Como é possível mapear esses tipos de encargo na fatura?</span><span class="sxs-lookup"><span data-stu-id="e7a85-468">How do I map these ChargeTypes to the invoice?</span></span></strong></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><strong><span data-ttu-id="e7a85-469">Encargos baseadas em licença</span><span class="sxs-lookup"><span data-stu-id="e7a85-469">License-based charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="e7a85-470">Taxa de ativação</span><span class="sxs-lookup"><span data-stu-id="e7a85-470">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="e7a85-471">O valor cobrado do cliente quando ele usa a assinatura depois de comprá-la.</span><span class="sxs-lookup"><span data-stu-id="e7a85-471">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="e7a85-472">No arquivo baseado em licença, some a coluna <strong>Quantidade</strong></span><span class="sxs-lookup"><span data-stu-id="e7a85-472">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e7a85-473">Taxa de cancelamento</span><span class="sxs-lookup"><span data-stu-id="e7a85-473">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="e7a85-474">Os encargos proporcionais reembolsados para o cliente quando os assentos associados são alterados</span><span class="sxs-lookup"><span data-stu-id="e7a85-474">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e7a85-475">Taxa do ciclo</span><span class="sxs-lookup"><span data-stu-id="e7a85-475">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="e7a85-476">Encargos periódicos de uma assinatura</span><span class="sxs-lookup"><span data-stu-id="e7a85-476">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e7a85-477">Percorrer ocorrência proporcional</span><span class="sxs-lookup"><span data-stu-id="e7a85-477">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="e7a85-478">Os encargos proporcionais cobrados do cliente quando os assentos associados são alterados</span><span class="sxs-lookup"><span data-stu-id="e7a85-478">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e7a85-479">Taxas proporcionais durante o cancelamento</span><span class="sxs-lookup"><span data-stu-id="e7a85-479">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="e7a85-480">Reembolso proporcional para a parte não utilizada do serviço após o cancelamento</span><span class="sxs-lookup"><span data-stu-id="e7a85-480">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e7a85-481">Taxas proporcionais durante a compra</span><span class="sxs-lookup"><span data-stu-id="e7a85-481">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="e7a85-482">O tipo de cobrança de uma assinatura ao usar a cobrança anual</span><span class="sxs-lookup"><span data-stu-id="e7a85-482">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e7a85-483">Taxa de compra</span><span class="sxs-lookup"><span data-stu-id="e7a85-483">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="e7a85-484">O tipo de cobrança de uma assinatura ao usar a cobrança mensal</span><span class="sxs-lookup"><span data-stu-id="e7a85-484">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e7a85-485">Taxa proporcional ao renovar</span><span class="sxs-lookup"><span data-stu-id="e7a85-485">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="e7a85-486">Taxas proporcionais após a renovação da assinatura</span><span class="sxs-lookup"><span data-stu-id="e7a85-486">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="e7a85-487">Taxa de renovação</span><span class="sxs-lookup"><span data-stu-id="e7a85-487">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="e7a85-488">Cobrança para renovação de uma assinatura</span><span class="sxs-lookup"><span data-stu-id="e7a85-488">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e7a85-489">Taxas proporcionais ao ativar</span><span class="sxs-lookup"><span data-stu-id="e7a85-489">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="e7a85-490">Taxas proporcionais da ativação até o final do período de cobrança</span><span class="sxs-lookup"><span data-stu-id="e7a85-490">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong><span data-ttu-id="e7a85-491">Tarifas de uso</span><span class="sxs-lookup"><span data-stu-id="e7a85-491">Usage Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="e7a85-492">Avaliar a taxa de uso ao cancelar</span><span class="sxs-lookup"><span data-stu-id="e7a85-492">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="e7a85-493">Taxa de uso de acesso com o cancelamento para uso não pago durante o período de cobrança atual</span><span class="sxs-lookup"><span data-stu-id="e7a85-493">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="e7a85-494">No arquivo baseado em uso, some a coluna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="e7a85-494">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e7a85-495">Avalie a taxa de uso para o ciclo atual</span><span class="sxs-lookup"><span data-stu-id="e7a85-495">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="e7a85-496">Taxa de uso de acesso para o período atual de cobrança</span><span class="sxs-lookup"><span data-stu-id="e7a85-496">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="e7a85-497">Créditos</span><span class="sxs-lookup"><span data-stu-id="e7a85-497">Credits</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="e7a85-498">Deslocando um item de linha</span><span class="sxs-lookup"><span data-stu-id="e7a85-498">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="e7a85-499">Reembolso parcial ou integral para um item de linha, incluindo os impostos</span><span class="sxs-lookup"><span data-stu-id="e7a85-499">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="e7a85-500">No arquivo baseado em licença, some a coluna <strong>TotalForCustomer</strong></span><span class="sxs-lookup"><span data-stu-id="e7a85-500">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="e7a85-501">No arquivo baseado em uso, some a coluna <strong>PostTaxTotal</strong></span><span class="sxs-lookup"><span data-stu-id="e7a85-501">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><strong><span data-ttu-id="e7a85-502">Descontos baseados em uso</span><span class="sxs-lookup"><span data-stu-id="e7a85-502">Usage-based discounts</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="e7a85-503">Desconto de ativação</span><span class="sxs-lookup"><span data-stu-id="e7a85-503">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="e7a85-504">Desconto aplicado quando a assinatura é ativada</span><span class="sxs-lookup"><span data-stu-id="e7a85-504">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="e7a85-505">No arquivo baseado em uso, some a coluna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="e7a85-505">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e7a85-506">Desconto de ciclo</span><span class="sxs-lookup"><span data-stu-id="e7a85-506">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="e7a85-507">Desconto aplicado em cobranças periódicas</span><span class="sxs-lookup"><span data-stu-id="e7a85-507">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e7a85-508">Desconto de renovação</span><span class="sxs-lookup"><span data-stu-id="e7a85-508">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="e7a85-509">Desconto aplicado quando a assinatura é renovada</span><span class="sxs-lookup"><span data-stu-id="e7a85-509">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e7a85-510">Desconto de cancelamento</span><span class="sxs-lookup"><span data-stu-id="e7a85-510">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="e7a85-511">Encargos aplicados quando descontos são cancelados</span><span class="sxs-lookup"><span data-stu-id="e7a85-511">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><strong><span data-ttu-id="e7a85-512">Descontos baseados em licença</span><span class="sxs-lookup"><span data-stu-id="e7a85-512">License-based discounts</span></span></strong></p>
</td>
<td>
<p><em><span data-ttu-id="e7a85-513">Podem ser aplicados a vários tipos de cobrança</span><span class="sxs-lookup"><span data-stu-id="e7a85-513">May be applied to multiple charge types</span></span></em></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="e7a85-514">No arquivo baseado em licença, some a coluna <strong>TotalOtherDiscount</strong></span><span class="sxs-lookup"><span data-stu-id="e7a85-514">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e7a85-515"><strong>Impostos</strong>&nbsp;ou&nbsp;<strong>IVA</strong></span><span class="sxs-lookup"><span data-stu-id="e7a85-515"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><em><span data-ttu-id="e7a85-516">Podem ser aplicados a vários tipos de cobrança</span><span class="sxs-lookup"><span data-stu-id="e7a85-516">May be applied to multiple charge types</span></span></em></p>
<p><em><span data-ttu-id="e7a85-517">Exceção: &quot;deslocamento de um item de linha&quot; já inclui impostos.</span><span class="sxs-lookup"><span data-stu-id="e7a85-517">Exception: &quot;Offset a line item&quot; already includes taxes.</span></span> <span data-ttu-id="e7a85-518">Consulte créditos, acima.</span><span class="sxs-lookup"><span data-stu-id="e7a85-518">See Credits, above.</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="e7a85-519">Impostos ou impostos sobre valor agregado (IVA)</span><span class="sxs-lookup"><span data-stu-id="e7a85-519">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="e7a85-520">No arquivo baseado em licença, some a coluna <strong>Imposto</strong></span><span class="sxs-lookup"><span data-stu-id="e7a85-520">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="e7a85-521">No arquivo baseado em uso, some a coluna <strong>TaxAmount</strong></span><span class="sxs-lookup"><span data-stu-id="e7a85-521">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
