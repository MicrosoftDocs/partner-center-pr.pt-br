---
title: Usar os arquivos de reconciliação | Partner Center
description: Para obter uma exibição detalhada em itens de linha de cada encargo em um ciclo de cobrança, baixe os arquivos de reconciliação do painel do Partner Center.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: KPacquer
ms.openlocfilehash: 51716e8abedf83237050cb51bc76e54a954cd28b
ms.sourcegitcommit: ec00affdfc79c1346cf8df482ce39dae98e20772
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/28/2018
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="e589e-103">Usar os arquivos de reconciliação</span><span class="sxs-lookup"><span data-stu-id="e589e-103">Use the reconciliation files</span></span>

**<span data-ttu-id="e589e-104">Aplicável a</span><span class="sxs-lookup"><span data-stu-id="e589e-104">Applies to</span></span>**

-  <span data-ttu-id="e589e-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="e589e-105">Partner Center</span></span>
-  <span data-ttu-id="e589e-106">Partner Center for Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="e589e-106">Partner Center for Microsoft Cloud for US Government</span></span>
-  <span data-ttu-id="e589e-107">Partner Center for Microsoft Cloud Germany</span><span class="sxs-lookup"><span data-stu-id="e589e-107">Partner Center for Microsoft Cloud Germany</span></span>

<span data-ttu-id="e589e-108">Para obter uma exibição detalhada em itens de linha de cada encargo em um ciclo de cobrança, baixe os arquivos de reconciliação do painel do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e589e-108">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from the Partner Center dashboard.</span></span> <span data-ttu-id="e589e-109">Os detalhes incluem encargos por assinaturas de cada cliente e eventos detalhados (como a adição de assentos a uma assinatura no meio do período).</span><span class="sxs-lookup"><span data-stu-id="e589e-109">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="e589e-110">Discriminar por parceiro</span><span class="sxs-lookup"><span data-stu-id="e589e-110">Itemize by partner</span></span>


<span data-ttu-id="e589e-111">Os parceiros no modelo indireto podem usar esses campos adicionais nos arquivos de reconciliação baseados em uso e em licença para discriminar por revendedor.</span><span class="sxs-lookup"><span data-stu-id="e589e-111">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="e589e-112">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="e589e-112">MPN ID</span></span></th>
<th><span data-ttu-id="e589e-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="e589e-113">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="e589e-114">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="e589e-114">MPN ID</span></span></td>
<td><p><span data-ttu-id="e589e-115">A ID do Microsoft Partner Network (MPN) do parceiro CSP (direta ou indireta).</span><span class="sxs-lookup"><span data-stu-id="e589e-115">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e589e-116">ID do MPN do revendedor</span><span class="sxs-lookup"><span data-stu-id="e589e-116">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="e589e-117">Só aparece em arquivos de reconciliação para parceiros no modelo indireto.</span><span class="sxs-lookup"><span data-stu-id="e589e-117">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="e589e-118">A ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="e589e-118">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="e589e-119">Isso corresponde à ID de revendedor listada para a assinatura específica no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e589e-119">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="e589e-120">Para exibir ou atualizar o revendedor, no menu Partner Center, selecione <strong>Clientes</strong>, em seguida, escolha o cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="e589e-120">eTo view or update the reseller, in the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="e589e-121">No menu do cliente, selecione <strong>Assinaturas</strong>, escolha a assinatura na lista.</span><span class="sxs-lookup"><span data-stu-id="e589e-121">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="e589e-122">Selecione <strong>Atualizar</strong> para alterar o <strong>Revendedor (ID do MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="e589e-122">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="e589e-123">Se um parceiro CSP vendeu a assinatura diretamente para o cliente, sua ID do MPN estará listada duas vezes, como a ID do MPN e a ID do MPN do revendedor.</span><span class="sxs-lookup"><span data-stu-id="e589e-123">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="e589e-124">Se um parceiro CSP tiver um revendedor sem ID do MPN, esse valor será definido como a ID do MPN do parceiro.</span><span class="sxs-lookup"><span data-stu-id="e589e-124">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="e589e-125">Se o parceiro CSP remover uma ID de revendedor, esse valor será definido como -1.</span><span class="sxs-lookup"><span data-stu-id="e589e-125">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="e589e-126">Campos de arquivos baseado em licença</span><span class="sxs-lookup"><span data-stu-id="e589e-126">License-based file fields</span></span>


<span data-ttu-id="e589e-127">Para reconciliar seus encargos com os pedidos de seu cliente, compare o campo Syndication\_Partner\_Subscription\_Number do arquivo de reconciliação com a ID de Assinatura do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e589e-127">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="e589e-128">Coluna</span><span class="sxs-lookup"><span data-stu-id="e589e-128">Column</span></span></strong></td>
<td><strong><span data-ttu-id="e589e-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="e589e-129">Description</span></span></strong></td>
<td><strong><span data-ttu-id="e589e-130">Valor de exemplo</span><span class="sxs-lookup"><span data-stu-id="e589e-130">Sample Value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e589e-131">PartnerId</span><span class="sxs-lookup"><span data-stu-id="e589e-131">PartnerId</span></span></td>
<td><p><span data-ttu-id="e589e-132">Identificador exclusivo de uma entidade de cobrança específica, em formato GUID.</span><span class="sxs-lookup"><span data-stu-id="e589e-132">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="e589e-133">Não é necessário para reconciliação, mas pode ser uma informação útil.</span><span class="sxs-lookup"><span data-stu-id="e589e-133">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="e589e-134">O mesmo em todas as linhas.</span><span class="sxs-lookup"><span data-stu-id="e589e-134">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="e589e-135">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="e589e-135">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e589e-136">CustomerID</span><span class="sxs-lookup"><span data-stu-id="e589e-136">CustomerID</span></span></td>
<td><p><span data-ttu-id="e589e-137">ID exclusiva da Microsoft, no formato GUID, usada para identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="e589e-137">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="e589e-138">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="e589e-138">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e589e-139">OrderID</span><span class="sxs-lookup"><span data-stu-id="e589e-139">OrderID</span></span></td>
<td><p><span data-ttu-id="e589e-140">Identificador exclusivo para um pedido na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e589e-140">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="e589e-141">Pode ser útil para identificar o pedido ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="e589e-141">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="e589e-142">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="e589e-142">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e589e-143">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="e589e-143">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="e589e-144">Identificador exclusivo de uma assinatura na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e589e-144">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="e589e-145">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="e589e-145">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="e589e-146">Esse não é o mesmo que o ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="e589e-146">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="e589e-147">Consulte Número_Assinatura_Parceiro_Sindicalização.</span><span class="sxs-lookup"><span data-stu-id="e589e-147">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="e589e-148">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="e589e-148">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e589e-149">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="e589e-149">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="e589e-150">Identificador exclusivo para assinaturas.</span><span class="sxs-lookup"><span data-stu-id="e589e-150">Unique identifier for subscriptions.</span></span> <span data-ttu-id="e589e-151">Target: Um cliente pode ter várias assinaturas para o mesmo plano, portanto, isso é importante para análise de arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="e589e-151">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="e589e-152">Esse campo é mapeado para a ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="e589e-152">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="e589e-153">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="e589e-153">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e589e-154">OfferID</span><span class="sxs-lookup"><span data-stu-id="e589e-154">OfferID</span></span></td>
<td><p><span data-ttu-id="e589e-155">ID exclusivo da oferta.</span><span class="sxs-lookup"><span data-stu-id="e589e-155">Unique offer ID.</span></span> <span data-ttu-id="e589e-156">ID padrão da oferta de acordo com a lista de preços.</span><span class="sxs-lookup"><span data-stu-id="e589e-156">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="e589e-157"><b>Observação</b>: esse valor não coincide com a ID de oferta da lista de preços.</span><span class="sxs-lookup"><span data-stu-id="e589e-157"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="e589e-158">Veja DurableOfferID abaixo.</span><span class="sxs-lookup"><span data-stu-id="e589e-158">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="e589e-159">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="e589e-159">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e589e-160">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="e589e-160">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="e589e-161">ID exclusiva da oferta durável, conforme definido na tabela de preços.</span><span class="sxs-lookup"><span data-stu-id="e589e-161">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="e589e-162"><b>Observação</b>: esse valor corresponde à ID de oferta da lista de preços.</span><span class="sxs-lookup"><span data-stu-id="e589e-162"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="e589e-163">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="e589e-163">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e589e-164">OfferName</span><span class="sxs-lookup"><span data-stu-id="e589e-164">OfferName</span></span></td>
<td><p><span data-ttu-id="e589e-165">O nome da oferta de serviço comprada pelo cliente, conforme definido na tabela de preços.</span><span class="sxs-lookup"><span data-stu-id="e589e-165">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="e589e-166">Microsoft Office 365 (plano E3)</span><span class="sxs-lookup"><span data-stu-id="e589e-166">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e589e-167">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="e589e-167">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="e589e-168">A data de início da assinatura, definida como um dia após o pedido ser enviado.</span><span class="sxs-lookup"><span data-stu-id="e589e-168">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="e589e-169">Verificando a data de início da assinatura em conjunto com a data de término, você pode determinar se o cliente está dentro do primeiro ano da assinatura ou se a assinatura foi renovada para o ano seguinte.</span><span class="sxs-lookup"><span data-stu-id="e589e-169">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="e589e-170">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="e589e-170">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="e589e-171">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="e589e-171">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e589e-172">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="e589e-172">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="e589e-173">A data do término da assinatura: 12 meses + x dias após a data de início (para se alinhar com a data de cobrança do parceiro) ou 12 meses a partir da data de renovação.</span><span class="sxs-lookup"><span data-stu-id="e589e-173">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="e589e-174">Na renovação, os preços são atualizados com a tabela de preços atual.</span><span class="sxs-lookup"><span data-stu-id="e589e-174">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="e589e-175">Um comunicado ao cliente pode ser necessário antes da renovação automática.</span><span class="sxs-lookup"><span data-stu-id="e589e-175">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="e589e-176">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="e589e-176">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="e589e-177">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="e589e-177">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e589e-178">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="e589e-178">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="e589e-179">Dia de início dos encargos.</span><span class="sxs-lookup"><span data-stu-id="e589e-179">Start day of the charges.</span></span></p>
<p><span data-ttu-id="e589e-180">Quando o cliente muda o número de assentos, esse número é usado para calcular os encargos por dia (pro-rata).</span><span class="sxs-lookup"><span data-stu-id="e589e-180">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="e589e-181">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="e589e-181">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="e589e-182">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="e589e-182">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e589e-183">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="e589e-183">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="e589e-184">Dia do término dos encargos.</span><span class="sxs-lookup"><span data-stu-id="e589e-184">End day of the charges.</span></span></p>
<p><span data-ttu-id="e589e-185">Quando o cliente muda o número de assentos, esse número é usado para calcular os encargos por dia (pro-rata).</span><span class="sxs-lookup"><span data-stu-id="e589e-185">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="e589e-186">A hora é sempre o fim do dia, 23:59.</span><span class="sxs-lookup"><span data-stu-id="e589e-186">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="e589e-187">28/2/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="e589e-187">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e589e-188">ChargeType</span><span class="sxs-lookup"><span data-stu-id="e589e-188">ChargeType</span></span></td>
<td><p><span data-ttu-id="e589e-189">O tipo de encargo ou ajuste.</span><span class="sxs-lookup"><span data-stu-id="e589e-189">The type of charge or adjustment.</span></span> <span data-ttu-id="e589e-190">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="e589e-190">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="e589e-191">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="e589e-191">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e589e-192">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="e589e-192">UnitPrice</span></span></td>
<td><p><span data-ttu-id="e589e-193">Preço por estação, conforme publicado na lista de preços no momento da compra.</span><span class="sxs-lookup"><span data-stu-id="e589e-193">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="e589e-194">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="e589e-194">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="e589e-195">6.82</span><span class="sxs-lookup"><span data-stu-id="e589e-195">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e589e-196">Quantity</span><span class="sxs-lookup"><span data-stu-id="e589e-196">Quantity</span></span></td>
<td><p><span data-ttu-id="e589e-197">Número de assentos.</span><span class="sxs-lookup"><span data-stu-id="e589e-197">Number of seats.</span></span> <span data-ttu-id="e589e-198">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="e589e-198">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="e589e-199">2</span><span class="sxs-lookup"><span data-stu-id="e589e-199">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e589e-200">Quantidade</span><span class="sxs-lookup"><span data-stu-id="e589e-200">Amount</span></span></td>
<td><p><span data-ttu-id="e589e-201">Preço total por quantidade.</span><span class="sxs-lookup"><span data-stu-id="e589e-201">Total of price for quantity.</span></span> <span data-ttu-id="e589e-202">Útil para verificar se o cálculo do valor coincide com a forma como você calcula isso para seus clientes.</span><span class="sxs-lookup"><span data-stu-id="e589e-202">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="e589e-203">13.32</span><span class="sxs-lookup"><span data-stu-id="e589e-203">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e589e-204">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="e589e-204">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="e589e-205">Valor de desconto aplicado a esses encargos.</span><span class="sxs-lookup"><span data-stu-id="e589e-205">Amount of discount applied to these charges.</span></span> <span data-ttu-id="e589e-206">IUR ou novas assinaturas qualificadas para incentivo também conterão um valor de desconto nessa coluna.</span><span class="sxs-lookup"><span data-stu-id="e589e-206">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="e589e-207">2.32</span><span class="sxs-lookup"><span data-stu-id="e589e-207">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e589e-208">Subtotal</span><span class="sxs-lookup"><span data-stu-id="e589e-208">Subtotal</span></span></td>
<td><p><span data-ttu-id="e589e-209">Total sem imposto.</span><span class="sxs-lookup"><span data-stu-id="e589e-209">Total before tax.</span></span> <span data-ttu-id="e589e-210">Verifica se seu subtotal corresponde ao total esperado, em caso de desconto.</span><span class="sxs-lookup"><span data-stu-id="e589e-210">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="e589e-211">11</span><span class="sxs-lookup"><span data-stu-id="e589e-211">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e589e-212">Imposto</span><span class="sxs-lookup"><span data-stu-id="e589e-212">Tax</span></span></td>
<td><p><span data-ttu-id="e589e-213">Valor do imposto cobrado, com base nas regras fiscais do mercado e em circunstâncias específicas.</span><span class="sxs-lookup"><span data-stu-id="e589e-213">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="e589e-214">0</span><span class="sxs-lookup"><span data-stu-id="e589e-214">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e589e-215">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="e589e-215">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="e589e-216">Total com imposto.</span><span class="sxs-lookup"><span data-stu-id="e589e-216">Total after tax.</span></span> <span data-ttu-id="e589e-217">Verifica se o imposto é cobrado na fatura.</span><span class="sxs-lookup"><span data-stu-id="e589e-217">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="e589e-218">11</span><span class="sxs-lookup"><span data-stu-id="e589e-218">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e589e-219">Moeda</span><span class="sxs-lookup"><span data-stu-id="e589e-219">Currency</span></span></td>
<td><p><span data-ttu-id="e589e-220">Tipo de moeda.</span><span class="sxs-lookup"><span data-stu-id="e589e-220">Currency type.</span></span> <span data-ttu-id="e589e-221">Cada entidade de cobrança tem somente uma moeda.</span><span class="sxs-lookup"><span data-stu-id="e589e-221">Each billing entity has only one currency.</span></span> <span data-ttu-id="e589e-222">Verifique se isso coincide com a primeira fatura e faça o mesmo após grandes atualizações na plataforma de cobrança.</span><span class="sxs-lookup"><span data-stu-id="e589e-222">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="e589e-223">Euro</span><span class="sxs-lookup"><span data-stu-id="e589e-223">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e589e-224">CustomerName</span><span class="sxs-lookup"><span data-stu-id="e589e-224">CustomerName</span></span></td>
<td><p><span data-ttu-id="e589e-225">Nome da organização do cliente como informado no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e589e-225">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="e589e-226">Isso é muito importante para reconciliar a fatura com as informações de seu sistema.</span><span class="sxs-lookup"><span data-stu-id="e589e-226">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="e589e-227">Cliente de teste A</span><span class="sxs-lookup"><span data-stu-id="e589e-227">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e589e-228">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="e589e-228">MPNID</span></span></td>
<td><p><span data-ttu-id="e589e-229">ID do MPN do parceiro CSP</span><span class="sxs-lookup"><span data-stu-id="e589e-229">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="e589e-230">4390934</span><span class="sxs-lookup"><span data-stu-id="e589e-230">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e589e-231">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="e589e-231">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="e589e-232">ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="e589e-232">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="e589e-233">Consulte [Discriminar por parceiro](#itemizebypartner).</span><span class="sxs-lookup"><span data-stu-id="e589e-233">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="e589e-234">4390934</span><span class="sxs-lookup"><span data-stu-id="e589e-234">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e589e-235">DomainName</span><span class="sxs-lookup"><span data-stu-id="e589e-235">DomainName</span></span></td>
<td><p><span data-ttu-id="e589e-236">Nome de domínio do cliente, usado para ajudar a identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="e589e-236">Customer's domain name, used to help identify the customer.</span></span></p></td>
<td><span data-ttu-id="e589e-237">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="e589e-237">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e589e-238">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="e589e-238">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="e589e-239">Apelido da Inscrição.</span><span class="sxs-lookup"><span data-stu-id="e589e-239">Subscription nickname.</span></span> <span data-ttu-id="e589e-240">Se nenhum apelido for especificado, o Partner Center usa o OfferName.</span><span class="sxs-lookup"><span data-stu-id="e589e-240">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="e589e-241">PROJETO ONLINE</span><span class="sxs-lookup"><span data-stu-id="e589e-241">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e589e-242">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="e589e-242">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="e589e-243">O nome da oferta de serviço comprada pelo cliente, conforme definido na tabela de preços.</span><span class="sxs-lookup"><span data-stu-id="e589e-243">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="e589e-244">(Este é um campo idêntico ao nome da oferta).</span><span class="sxs-lookup"><span data-stu-id="e589e-244">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="e589e-245">PROJETO ONLINE PREMIUM SEM PROJETO CLIENTE</span><span class="sxs-lookup"><span data-stu-id="e589e-245">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="e589e-246">Campos de arquivo baseado em uso</span><span class="sxs-lookup"><span data-stu-id="e589e-246">Usage-based file fields</span></span>


<span data-ttu-id="e589e-247">Para reconciliar seus encargos com o uso de seu cliente, compare ResellerID/ResellerName/ResellerBillableAccount do arquivo de reconciliação com o nome do cliente e a ID da assinatura do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e589e-247">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="e589e-248">Os campos a seguir explicam quais serviços foram usados e a taxa.</span><span class="sxs-lookup"><span data-stu-id="e589e-248">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="e589e-249">Coluna</span><span class="sxs-lookup"><span data-stu-id="e589e-249">Column</span></span></strong></td>
<td><strong><span data-ttu-id="e589e-250">Descrição</span><span class="sxs-lookup"><span data-stu-id="e589e-250">Description</span></span></strong></td>
<td><strong><span data-ttu-id="e589e-251">Valor de exemplo</span><span class="sxs-lookup"><span data-stu-id="e589e-251">Sample value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e589e-252">PartnerID</span><span class="sxs-lookup"><span data-stu-id="e589e-252">PartnerID</span></span></td>
<td><p><span data-ttu-id="e589e-253">ID do parceiro, no formato GUID.</span><span class="sxs-lookup"><span data-stu-id="e589e-253">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="e589e-254">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="e589e-254">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e589e-255">PartnerName</span><span class="sxs-lookup"><span data-stu-id="e589e-255">PartnerName</span></span></td>
<td><p><span data-ttu-id="e589e-256">Nome do parceiro.</span><span class="sxs-lookup"><span data-stu-id="e589e-256">Partner Name.</span></span></p></td>
<td><span data-ttu-id="e589e-257">Acme incorporado</span><span class="sxs-lookup"><span data-stu-id="e589e-257">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e589e-258">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="e589e-258">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="e589e-259">ID da conta do parceiro.</span><span class="sxs-lookup"><span data-stu-id="e589e-259">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="e589e-260">1010578050</span><span class="sxs-lookup"><span data-stu-id="e589e-260">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e589e-261">CustomerName</span><span class="sxs-lookup"><span data-stu-id="e589e-261">CustomerName</span></span></td>
<td><p><span data-ttu-id="e589e-262">Nome da organização do cliente como informado no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e589e-262">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="e589e-263">Isso é muito importante para reconciliar a fatura com as informações de seu sistema.</span><span class="sxs-lookup"><span data-stu-id="e589e-263">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="e589e-264">Cliente de teste A</span><span class="sxs-lookup"><span data-stu-id="e589e-264">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e589e-265">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="e589e-265">MPNID</span></span></td>
<td><p><span data-ttu-id="e589e-266">ID do MPN do parceiro CSP.</span><span class="sxs-lookup"><span data-stu-id="e589e-266">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="e589e-267">4390934</span><span class="sxs-lookup"><span data-stu-id="e589e-267">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e589e-268">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="e589e-268">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="e589e-269">ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="e589e-269">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="e589e-270">Consulte [Discriminar por parceiro](#itemizebypartner).</span><span class="sxs-lookup"><span data-stu-id="e589e-270">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="e589e-271">4390934</span><span class="sxs-lookup"><span data-stu-id="e589e-271">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e589e-272">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="e589e-272">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="e589e-273">Número da fatura na qual a transação especificada é exibida.</span><span class="sxs-lookup"><span data-stu-id="e589e-273">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="e589e-274">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="e589e-274">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e589e-275">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="e589e-275">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="e589e-276">Data de início do ciclo de cobrança exceto quando apresentadas as datas de dados de uso latentes anteriormente não cobradas (do ciclo de cobrança anterior).</span><span class="sxs-lookup"><span data-stu-id="e589e-276">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="e589e-277">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="e589e-277">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="e589e-278">1/2/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="e589e-278">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e589e-279">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="e589e-279">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="e589e-280">Data de término do ciclo de cobrança exceto quando apresentadas as datas de dados de uso latentes anteriormente não cobradas (do ciclo de cobrança anterior).</span><span class="sxs-lookup"><span data-stu-id="e589e-280">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="e589e-281">A hora é sempre o fim do dia, 23:59.</span><span class="sxs-lookup"><span data-stu-id="e589e-281">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="e589e-282">28/2/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="e589e-282">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e589e-283">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="e589e-283">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="e589e-284">Identificador exclusivo de uma assinatura na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e589e-284">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="e589e-285">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="e589e-285">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="e589e-286">Esse não é o mesmo que a ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="e589e-286">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="e589e-287">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="e589e-287">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e589e-288">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="e589e-288">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="e589e-289">Apelido da oferta do serviço.</span><span class="sxs-lookup"><span data-stu-id="e589e-289">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="e589e-290">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="e589e-290">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e589e-291">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="e589e-291">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="e589e-292">Linha de negócios da oferta do serviço</span><span class="sxs-lookup"><span data-stu-id="e589e-292">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="e589e-293">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="e589e-293">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e589e-294">OrderID</span><span class="sxs-lookup"><span data-stu-id="e589e-294">OrderID</span></span></td>
<td><p><span data-ttu-id="e589e-295">Identificador exclusivo para um pedido na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e589e-295">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="e589e-296">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="e589e-296">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="e589e-297">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="e589e-297">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e589e-298">ServiceName</span><span class="sxs-lookup"><span data-stu-id="e589e-298">ServiceName</span></span></td>
<td><p><span data-ttu-id="e589e-299">O nome do serviço do Azure em questão.</span><span class="sxs-lookup"><span data-stu-id="e589e-299">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="e589e-300">MÁQUINAS VIRTUAIS</span><span class="sxs-lookup"><span data-stu-id="e589e-300">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e589e-301">ServiceType</span><span class="sxs-lookup"><span data-stu-id="e589e-301">ServiceType</span></span></td>
<td><p><span data-ttu-id="e589e-302">O tipo específico de serviço do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="e589e-302">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="e589e-303">Service Bus – Individual ou pacote</span><span class="sxs-lookup"><span data-stu-id="e589e-303">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="e589e-304">Banco de dados SQL Azure – Edição empresa ou Web</span><span class="sxs-lookup"><span data-stu-id="e589e-304">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e589e-305">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="e589e-305">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="e589e-306">Identificador exclusivo específico de toda a estrutura de serviço de dados e preço.</span><span class="sxs-lookup"><span data-stu-id="e589e-306">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="e589e-307">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="e589e-307">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e589e-308">Nome do recurso</span><span class="sxs-lookup"><span data-stu-id="e589e-308">Resource Name</span></span></td>
<td><p><span data-ttu-id="e589e-309">O nome do recurso do Azure.</span><span class="sxs-lookup"><span data-stu-id="e589e-309">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="e589e-310">Dados de entrada transferidos (GB)</span><span class="sxs-lookup"><span data-stu-id="e589e-310">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="e589e-311">Dados de saída transferidos (GB)</span><span class="sxs-lookup"><span data-stu-id="e589e-311">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e589e-312">Região</span><span class="sxs-lookup"><span data-stu-id="e589e-312">Region</span></span></td>
<td><p><span data-ttu-id="e589e-313">A região a qual o uso se aplica.</span><span class="sxs-lookup"><span data-stu-id="e589e-313">The region the usage applies to.</span></span> <span data-ttu-id="e589e-314">Usado principalmente para atribuir as taxas de transferências de dados, já que as taxas variam de acordo com a região.</span><span class="sxs-lookup"><span data-stu-id="e589e-314">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="e589e-315">Pacífico Asiático, Europa, América Latina e América do Norte</span><span class="sxs-lookup"><span data-stu-id="e589e-315">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e589e-316">SKU</span><span class="sxs-lookup"><span data-stu-id="e589e-316">SKU</span></span></td>
<td><p><span data-ttu-id="e589e-317">Identificador exclusivo MSFT da oferta</span><span class="sxs-lookup"><span data-stu-id="e589e-317">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="e589e-318">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="e589e-318">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="e589e-319">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="e589e-319">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="e589e-320">Uma ID e a quantidade para discriminar as taxas diferentes de um serviço ou recurso em um determinado período de cobrança.</span><span class="sxs-lookup"><span data-stu-id="e589e-320">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="e589e-321">Para a classificação em camadas do Azure, pode haver uma taxa para uma determinada quantidade de unidades faturáveis e uma taxa diferente depois disso.</span><span class="sxs-lookup"><span data-stu-id="e589e-321">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="e589e-322">1</span><span class="sxs-lookup"><span data-stu-id="e589e-322">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e589e-323">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="e589e-323">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="e589e-324">A quantidade de serviço consumida (horas, GB etc.) durante o período de relatório.</span><span class="sxs-lookup"><span data-stu-id="e589e-324">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="e589e-325">Também inclui qualquer uso não cobrado de períodos de relatório anteriores.</span><span class="sxs-lookup"><span data-stu-id="e589e-325">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="e589e-326">11</span><span class="sxs-lookup"><span data-stu-id="e589e-326">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e589e-327">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="e589e-327">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="e589e-328">Unidades incluídas como parte da oferta.</span><span class="sxs-lookup"><span data-stu-id="e589e-328">Units included as part of the offer.</span></span> <span data-ttu-id="e589e-329">Normalmente não está presente no CSP.</span><span class="sxs-lookup"><span data-stu-id="e589e-329">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="e589e-330">0</span><span class="sxs-lookup"><span data-stu-id="e589e-330">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="e589e-331">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="e589e-331">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="e589e-332">Unidades não incluídas como parte da oferta devem ser pagas pelo parceiro.</span><span class="sxs-lookup"><span data-stu-id="e589e-332">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="e589e-333">Igual a ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="e589e-333">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="e589e-334">11</span><span class="sxs-lookup"><span data-stu-id="e589e-334">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e589e-335">ListPrice</span><span class="sxs-lookup"><span data-stu-id="e589e-335">ListPrice</span></span></td>
<td><p><span data-ttu-id="e589e-336">Preço da oferta em vigor na data de início da assinatura.</span><span class="sxs-lookup"><span data-stu-id="e589e-336">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="e589e-337">U$ 0,0808</span><span class="sxs-lookup"><span data-stu-id="e589e-337">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e589e-338">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="e589e-338">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="e589e-339">ListPrist vezes OverageQuantity, arredondado para o centavo mais próximo.</span><span class="sxs-lookup"><span data-stu-id="e589e-339">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="e589e-340">U$ 0,085</span><span class="sxs-lookup"><span data-stu-id="e589e-340">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e589e-341">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="e589e-341">TaxAmount</span></span></td>
<td><p><span data-ttu-id="e589e-342">Valor do imposto cobrado, com base nas regras fiscais do mercado e em circunstâncias específicas.</span><span class="sxs-lookup"><span data-stu-id="e589e-342">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="e589e-343">U$ 0,08</span><span class="sxs-lookup"><span data-stu-id="e589e-343">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e589e-344">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="e589e-344">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="e589e-345">Total após imposto, quando o imposto é aplicável.</span><span class="sxs-lookup"><span data-stu-id="e589e-345">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="e589e-346">U$ 0,93</span><span class="sxs-lookup"><span data-stu-id="e589e-346">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e589e-347">Moeda</span><span class="sxs-lookup"><span data-stu-id="e589e-347">Currency</span></span></td>
<td><p><span data-ttu-id="e589e-348">Tipo de moeda.</span><span class="sxs-lookup"><span data-stu-id="e589e-348">Currency type.</span></span> <span data-ttu-id="e589e-349">Cada entidade de cobrança tem somente uma moeda.</span><span class="sxs-lookup"><span data-stu-id="e589e-349">Each billing entity has only one currency.</span></span> <span data-ttu-id="e589e-350">Verifique se isso coincide com a primeira fatura e faça o mesmo após grandes atualizações na plataforma de cobrança.</span><span class="sxs-lookup"><span data-stu-id="e589e-350">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="e589e-351">Euro</span><span class="sxs-lookup"><span data-stu-id="e589e-351">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e589e-352">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="e589e-352">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="e589e-353">Preço por unidade sem imposto.</span><span class="sxs-lookup"><span data-stu-id="e589e-353">Pretax price per unit.</span></span> <span data-ttu-id="e589e-354">Igual a PretaxCharges / OverageQuantity, arredondado para o centavo mais próximo.</span><span class="sxs-lookup"><span data-stu-id="e589e-354">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="e589e-355">U$ 0,08</span><span class="sxs-lookup"><span data-stu-id="e589e-355">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e589e-356">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="e589e-356">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="e589e-357">Preço pós-imposto por unidade.</span><span class="sxs-lookup"><span data-stu-id="e589e-357">Post tax price per unit.</span></span> <span data-ttu-id="e589e-358">Igual a PostTaxTotal / OverageQuantity, ou PretaxEffectiveRate + taxa de imposto por valor de unidade, arredondado para o centavo mais próximo.</span><span class="sxs-lookup"><span data-stu-id="e589e-358">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="e589e-359">U$ 0,08</span><span class="sxs-lookup"><span data-stu-id="e589e-359">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e589e-360">ChargeType</span><span class="sxs-lookup"><span data-stu-id="e589e-360">ChargeType</span></span></td>
<td><p><span data-ttu-id="e589e-361">O tipo de encargo ou ajuste.</span><span class="sxs-lookup"><span data-stu-id="e589e-361">The type of charge or adjustment.</span></span> <span data-ttu-id="e589e-362">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="e589e-362">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="e589e-363">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="e589e-363">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e589e-364">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="e589e-364">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="e589e-365">ID exclusiva da conta na plataforma de cobrança da MSFT.</span><span class="sxs-lookup"><span data-stu-id="e589e-365">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="e589e-366">1280018095</span><span class="sxs-lookup"><span data-stu-id="e589e-366">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e589e-367">UsageDate</span><span class="sxs-lookup"><span data-stu-id="e589e-367">UsageDate</span></span></td>
<td><p><span data-ttu-id="e589e-368">Data da implantação do serviço.</span><span class="sxs-lookup"><span data-stu-id="e589e-368">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="e589e-369">1/2/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="e589e-369">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e589e-370">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="e589e-370">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="e589e-371">Essa coluna identifica a localização de um data center dentro da região para serviços onde isso é aplicável e preenchido.</span><span class="sxs-lookup"><span data-stu-id="e589e-371">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="e589e-372">Leste da Ásia, Sudeste da Ásia, Norte da Europa, Europa Ocidental, Centro Norte e Centro Sul dos EUA</span><span class="sxs-lookup"><span data-stu-id="e589e-372">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e589e-373">MeteredService</span><span class="sxs-lookup"><span data-stu-id="e589e-373">MeteredService</span></span></td>
<td><p><span data-ttu-id="e589e-374">Essa coluna é utilizada para rastrear o serviço do Microsoft Azure individual que não pode ser identificado especificamente na coluna Nome do Serviço.</span><span class="sxs-lookup"><span data-stu-id="e589e-374">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="e589e-375">Por exemplo, transferências de dados são relatadas como &quot;Microsoft Azure – Todos os Serviços&quot; na coluna Nome do Serviço.</span><span class="sxs-lookup"><span data-stu-id="e589e-375">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="e589e-376">Essa coluna MeteredService indicará ao qual serviço específico o uso pertence.</span><span class="sxs-lookup"><span data-stu-id="e589e-376">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="e589e-377">AccessControl, CDN, Computação, Banco de dados, ServiceBus, Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e589e-377">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e589e-378">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="e589e-378">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="e589e-379">Um subcabeçalho que esclarece ainda mais o serviço Microsoft Azure individual além do nível fornecido pelo campo MeteredService.</span><span class="sxs-lookup"><span data-stu-id="e589e-379">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="e589e-380">EXTERNO</span><span class="sxs-lookup"><span data-stu-id="e589e-380">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e589e-381">Projeto</span><span class="sxs-lookup"><span data-stu-id="e589e-381">Project</span></span></td>
<td><p><span data-ttu-id="e589e-382">Nome definido pelo cliente para a instância do serviço</span><span class="sxs-lookup"><span data-stu-id="e589e-382">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="e589e-383">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="e589e-383">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e589e-384">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="e589e-384">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="e589e-385">O número de conexões ServiceBus que foram provisionados e utilizados em um dia específico.</span><span class="sxs-lookup"><span data-stu-id="e589e-385">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="e589e-386">Por exemplo: se você tivesse uma conexão individualmente provisionada durante um mês de 30 dias, a coluna Informação do Serviço 1 lerá "1,000000 conexões/30 dias".</span><span class="sxs-lookup"><span data-stu-id="e589e-386">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="e589e-387">Se você tinha um pacote de 25 conexões ServiceBus provisionadas e você utilizou 1 durante o dia, sua declaração de uso diário para esse dia indicaria "25 conexões/30 dias – Usado: 1,000000".</span><span class="sxs-lookup"><span data-stu-id="e589e-387">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e589e-388">CustomerID</span><span class="sxs-lookup"><span data-stu-id="e589e-388">CustomerID</span></span></td>
<td><p><span data-ttu-id="e589e-389">ID exclusiva da Microsoft, no formato GUID, usada para identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="e589e-389">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="e589e-390">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="e589e-390">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e589e-391">DomainName</span><span class="sxs-lookup"><span data-stu-id="e589e-391">DomainName</span></span></td>
<td><p><span data-ttu-id="e589e-392">Nome de domínio do cliente, usado para ajudar a identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="e589e-392">Customer's domain name, used to help identify the customer.</span></span></p></td>
<td><span data-ttu-id="e589e-393">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="e589e-393">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="e589e-394">Unidade</span><span class="sxs-lookup"><span data-stu-id="e589e-394">Unit</span></span></td>
<td><p><span data-ttu-id="e589e-395">A unidade do nome do recurso</span><span class="sxs-lookup"><span data-stu-id="e589e-395">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="e589e-396">GB ou HORAS</span><span class="sxs-lookup"><span data-stu-id="e589e-396">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>



## <a href="" id="charge_types"></a><span data-ttu-id="e589e-397">Mapeando encargos entre uma fatura e o arquivo de reconciliação</span><span class="sxs-lookup"><span data-stu-id="e589e-397">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="e589e-398">Sua fatura fornece um resumo dos encargos, enquanto seu arquivo de reconciliação fornece uma divisão detalhada das transações de item de linha, incluindo os tipos de carga.</span><span class="sxs-lookup"><span data-stu-id="e589e-398">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="e589e-399">Para fazer referência cruzada das quantidades de carga entre o arquivo de reconciliação e fatura, você pode usar opções de filtro do Microsoft Excel para filtrar por tipos de cobrança no arquivo de reconciliação para mapear os encargos de fatura em um conjunto de detalhamentos de cobrança no arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="e589e-399">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="e589e-400">Os arquivos de reconciliação, tanto os baseados em licença quanto os baseados em uso, mostram apenas encargos e transações relacionadas ao uso (unidades consumidas e encargos relacionados).</span><span class="sxs-lookup"><span data-stu-id="e589e-400">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="e589e-401">Créditos únicos, descontos ou reembolsos que aparecem na fatura como "Ajustes" não são mostrados no arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="e589e-401">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="e589e-402">A tabela a seguir mostra os mapeamentos entre uma seção da fatura e os tipos de encargo associados que podem aparecer nos arquivos de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="e589e-402">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><strong><span data-ttu-id="e589e-403">Descrição do encargo da fatura</span><span class="sxs-lookup"><span data-stu-id="e589e-403">Invoice charge description</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="e589e-404">Descrição do encargo do arquivo de reconciliação (coluna ChargeType)</span><span class="sxs-lookup"><span data-stu-id="e589e-404">Reconciliation file charge description (ChargeType column)</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="e589e-405">O que é este encargo?</span><span class="sxs-lookup"><span data-stu-id="e589e-405">What is this charge?</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="e589e-406">Como é possível mapear esses tipos de encargo na fatura?</span><span class="sxs-lookup"><span data-stu-id="e589e-406">How do I map these ChargeTypes to the invoice?</span></span></strong></p>
</td>
</tr>
<tr>
<td rowspan="8">
<p><strong><span data-ttu-id="e589e-407">Encargos recorrentes</span><span class="sxs-lookup"><span data-stu-id="e589e-407">Recurring Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="e589e-408">Taxa de ativação</span><span class="sxs-lookup"><span data-stu-id="e589e-408">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="e589e-409">O valor cobrado do cliente quando ele usa a assinatura depois de comprá-la.</span><span class="sxs-lookup"><span data-stu-id="e589e-409">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="8">
<p><span data-ttu-id="e589e-410">No arquivo baseado em licença, some a coluna <strong>Quantidade</strong></span><span class="sxs-lookup"><span data-stu-id="e589e-410">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e589e-411">Taxa de cancelamento</span><span class="sxs-lookup"><span data-stu-id="e589e-411">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="e589e-412">Os encargos proporcionais reembolsados para o cliente quando os assentos associados são alterados</span><span class="sxs-lookup"><span data-stu-id="e589e-412">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e589e-413">Taxa do ciclo</span><span class="sxs-lookup"><span data-stu-id="e589e-413">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="e589e-414">Encargos periódicos de uma assinatura</span><span class="sxs-lookup"><span data-stu-id="e589e-414">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e589e-415">Percorrer ocorrência proporcional</span><span class="sxs-lookup"><span data-stu-id="e589e-415">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="e589e-416">Os encargos proporcionais cobrados do cliente quando os assentos associados são alterados</span><span class="sxs-lookup"><span data-stu-id="e589e-416">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e589e-417">Taxas proporcionais durante o cancelamento</span><span class="sxs-lookup"><span data-stu-id="e589e-417">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="e589e-418">Reembolso proporcional para a parte não utilizada do serviço após o cancelamento</span><span class="sxs-lookup"><span data-stu-id="e589e-418">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e589e-419">Taxas proporcionais durante a compra</span><span class="sxs-lookup"><span data-stu-id="e589e-419">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="e589e-420">Taxas proporcionais após a compra</span><span class="sxs-lookup"><span data-stu-id="e589e-420">Prorated fees upon purchase</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e589e-421">Taxa de compra</span><span class="sxs-lookup"><span data-stu-id="e589e-421">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="e589e-422">Encargo inicial de uma assinatura</span><span class="sxs-lookup"><span data-stu-id="e589e-422">Initial charge for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e589e-423">Taxa proporcional ao renovar</span><span class="sxs-lookup"><span data-stu-id="e589e-423">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="e589e-424">Taxas proporcionais após a renovação da assinatura</span><span class="sxs-lookup"><span data-stu-id="e589e-424">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e589e-425">Taxa de renovação</span><span class="sxs-lookup"><span data-stu-id="e589e-425">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="e589e-426">Cobrança para renovação de uma assinatura</span><span class="sxs-lookup"><span data-stu-id="e589e-426">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="e589e-427">Outros produtos e serviços</span><span class="sxs-lookup"><span data-stu-id="e589e-427">Other Products and Services</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="e589e-428">Taxas proporcionais ao ativar</span><span class="sxs-lookup"><span data-stu-id="e589e-428">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="e589e-429">Taxas proporcionais da ativação até o final do período de cobrança</span><span class="sxs-lookup"><span data-stu-id="e589e-429">Prorated fees from activation until end of billing period</span></span></p>
</td>
<td>
<p><span data-ttu-id="e589e-430">No arquivo baseado em licença, some a coluna <strong>Quantidade</strong></span><span class="sxs-lookup"><span data-stu-id="e589e-430">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong><span data-ttu-id="e589e-431">Tarifas de uso</span><span class="sxs-lookup"><span data-stu-id="e589e-431">Usage Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="e589e-432">Avaliar a taxa de uso ao cancelar</span><span class="sxs-lookup"><span data-stu-id="e589e-432">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="e589e-433">Taxa de uso de acesso com o cancelamento para uso não pago durante o período de cobrança atual</span><span class="sxs-lookup"><span data-stu-id="e589e-433">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="e589e-434">No arquivo baseado em uso, some a coluna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="e589e-434">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e589e-435">Avalie a taxa de uso para o ciclo atual</span><span class="sxs-lookup"><span data-stu-id="e589e-435">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="e589e-436">Taxa de uso de acesso para o período atual de cobrança</span><span class="sxs-lookup"><span data-stu-id="e589e-436">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="e589e-437">Créditos &amp; Ajustes</span><span class="sxs-lookup"><span data-stu-id="e589e-437">Credits &amp; Adjustments</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="e589e-438">Deslocando um item de linha</span><span class="sxs-lookup"><span data-stu-id="e589e-438">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="e589e-439">Reembolso parcial ou integral para um item de linha, incluindo os impostos</span><span class="sxs-lookup"><span data-stu-id="e589e-439">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="e589e-440">No arquivo baseado em licença, some a coluna <strong>TotalForCustomer</strong></span><span class="sxs-lookup"><span data-stu-id="e589e-440">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="e589e-441">No arquivo baseado em uso, some a coluna <strong>PostTaxTotal</strong></span><span class="sxs-lookup"><span data-stu-id="e589e-441">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>


<tr>
<td rowspan="4">
<p><strong><span data-ttu-id="e589e-442">Outros descontos</span><span class="sxs-lookup"><span data-stu-id="e589e-442">Other Discounts</span></span></strong></br>
<em><span data-ttu-id="e589e-443">(com base em uso)</span><span class="sxs-lookup"><span data-stu-id="e589e-443">(usage-based)</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="e589e-444">Desconto de ativação</span><span class="sxs-lookup"><span data-stu-id="e589e-444">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="e589e-445">Desconto aplicado quando a assinatura é ativada</span><span class="sxs-lookup"><span data-stu-id="e589e-445">Discount applied when subscription activated</span></span></p>
</td>
<td rowspan="4">
<p><span data-ttu-id="e589e-446">No arquivo baseado em uso, some a coluna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="e589e-446">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e589e-447">Desconto de ciclo</span><span class="sxs-lookup"><span data-stu-id="e589e-447">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="e589e-448">Desconto aplicado em cobranças periódicas</span><span class="sxs-lookup"><span data-stu-id="e589e-448">Discount applied on periodic charges</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="e589e-449">Desconto de renovação</span><span class="sxs-lookup"><span data-stu-id="e589e-449">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="e589e-450">Desconto aplicado quando a assinatura é renovada</span><span class="sxs-lookup"><span data-stu-id="e589e-450">Discount applied when subscription renewed</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="e589e-451">Desconto de cancelamento</span><span class="sxs-lookup"><span data-stu-id="e589e-451">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="e589e-452">Encargos aplicados quando descontos são cancelados</span><span class="sxs-lookup"><span data-stu-id="e589e-452">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="e589e-453">Outros descontos</span><span class="sxs-lookup"><span data-stu-id="e589e-453">Other Discounts</span></span></strong></br>
<em><span data-ttu-id="e589e-454">(com base em licença)</span><span class="sxs-lookup"><span data-stu-id="e589e-454">(license-based)</span></span></em></p>
</td>
<td>
<p><em><span data-ttu-id="e589e-455">Podem ser aplicados a vários tipos de cobrança</span><span class="sxs-lookup"><span data-stu-id="e589e-455">May be applied to multiple charge types</span></span></em></p>
</td>
<td>
<p>&nbsp;</p>
</td>
<td>
<p><span data-ttu-id="e589e-456">No arquivo baseado em licença, some a coluna <strong>TotalOtherDiscount</strong></span><span class="sxs-lookup"><span data-stu-id="e589e-456">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e589e-457"><strong>Impostos</strong>&nbsp;ou&nbsp;<strong>IVA</strong></span><span class="sxs-lookup"><span data-stu-id="e589e-457"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><em><span data-ttu-id="e589e-458">Podem ser aplicados a vários tipos de cobrança</span><span class="sxs-lookup"><span data-stu-id="e589e-458">May be applied to multiple charge types</span></span></em></p>
<p><em><span data-ttu-id="e589e-459">Exceção: "Deslocamento de um item de linha" já inclui impostos.</span><span class="sxs-lookup"><span data-stu-id="e589e-459">Exception: "Offset a line item" already includes taxes.</span></span> <span data-ttu-id="e589e-460">Consulte Créditos &amp;Ajustes, acima.</span><span class="sxs-lookup"><span data-stu-id="e589e-460">See Credits &amp; Adjustments, above.</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="e589e-461">Impostos ou impostos sobre valor agregado (IVA)</span><span class="sxs-lookup"><span data-stu-id="e589e-461">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="e589e-462">No arquivo baseado em licença, some a coluna <strong>Imposto</strong></span><span class="sxs-lookup"><span data-stu-id="e589e-462">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="e589e-463">No arquivo baseado em uso, some a coluna <strong>TaxAmount</strong></span><span class="sxs-lookup"><span data-stu-id="e589e-463">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
