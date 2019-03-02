---
title: Usar os arquivos de reconciliação | Partner Center
ms.topic: article
ms.date: 10/29/2018
description: Para uma exibição detalhada do item de linha de cada encargo em um ciclo de cobrança, baixe os arquivos de reconciliação do Partner Center.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: labrenne
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 081afc547a0ff86010e06fcb5224a615a0075e34
ms.sourcegitcommit: 8bfd1358a0ef86e46bee2a1097d86de3c9e969e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/02/2019
ms.locfileid: "9122273"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="03d1a-103">Usar os arquivos de reconciliação</span><span class="sxs-lookup"><span data-stu-id="03d1a-103">Use the reconciliation files</span></span>

**<span data-ttu-id="03d1a-104">Aplicável a</span><span class="sxs-lookup"><span data-stu-id="03d1a-104">Applies to</span></span>**

-  <span data-ttu-id="03d1a-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="03d1a-105">Partner Center</span></span>
-  <span data-ttu-id="03d1a-106">Partner Center for Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="03d1a-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="03d1a-107">Para uma exibição detalhada do item de linha de cada encargo em um ciclo de cobrança, baixe os arquivos de reconciliação do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="03d1a-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="03d1a-108">Os detalhes incluem encargos por assinaturas de cada cliente e eventos detalhados (como a adição de assentos a uma assinatura no meio do período).</span><span class="sxs-lookup"><span data-stu-id="03d1a-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="03d1a-109">Discriminar por parceiro</span><span class="sxs-lookup"><span data-stu-id="03d1a-109">Itemize by partner</span></span>


<span data-ttu-id="03d1a-110">Os parceiros no modelo indireto podem usar esses campos adicionais nos arquivos de reconciliação baseados em uso e em licença para discriminar por revendedor.</span><span class="sxs-lookup"><span data-stu-id="03d1a-110">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="03d1a-111">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="03d1a-111">MPN ID</span></span></th>
<th><span data-ttu-id="03d1a-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="03d1a-112">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="03d1a-113">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="03d1a-113">MPN ID</span></span></td>
<td><p><span data-ttu-id="03d1a-114">A ID do Microsoft Partner Network (MPN) do parceiro CSP (direta ou indireta).</span><span class="sxs-lookup"><span data-stu-id="03d1a-114">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="03d1a-115">ID do MPN do revendedor</span><span class="sxs-lookup"><span data-stu-id="03d1a-115">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="03d1a-116">Só aparece em arquivos de reconciliação para parceiros no modelo indireto.</span><span class="sxs-lookup"><span data-stu-id="03d1a-116">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="03d1a-117">A ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="03d1a-117">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="03d1a-118">Isso corresponde à ID de revendedor listada para a assinatura específica no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="03d1a-118">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="03d1a-119">Para exibir ou atualizar o revendedor, no menu Partner Center, selecione <strong>clientes</strong>e, em seguida, escolha o cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="03d1a-119">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="03d1a-120">No menu do cliente, selecione <strong>Assinaturas</strong>, escolha a assinatura na lista.</span><span class="sxs-lookup"><span data-stu-id="03d1a-120">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="03d1a-121">Selecione <strong>Atualizar</strong> para alterar o <strong>Revendedor (ID do MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="03d1a-121">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="03d1a-122">Se um parceiro CSP vendeu a assinatura diretamente para o cliente, sua ID do MPN estará listada duas vezes, como a ID do MPN e a ID do MPN do revendedor.</span><span class="sxs-lookup"><span data-stu-id="03d1a-122">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="03d1a-123">Se um parceiro CSP tiver um revendedor sem ID do MPN, esse valor será definido como a ID do MPN do parceiro.</span><span class="sxs-lookup"><span data-stu-id="03d1a-123">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="03d1a-124">Se o parceiro CSP remover uma ID de revendedor, esse valor será definido como -1.</span><span class="sxs-lookup"><span data-stu-id="03d1a-124">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="03d1a-125">Campos de arquivos baseado em licença</span><span class="sxs-lookup"><span data-stu-id="03d1a-125">License-based file fields</span></span>


<span data-ttu-id="03d1a-126">Para reconciliar seus encargos com os pedidos de seu cliente, compare o campo Syndication\_Partner\_Subscription\_Number do arquivo de reconciliação com a ID de Assinatura do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="03d1a-126">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="03d1a-127">Coluna</span><span class="sxs-lookup"><span data-stu-id="03d1a-127">Column</span></span></strong></td>
<td><strong><span data-ttu-id="03d1a-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="03d1a-128">Description</span></span></strong></td>
<td><strong><span data-ttu-id="03d1a-129">Valor de exemplo</span><span class="sxs-lookup"><span data-stu-id="03d1a-129">Sample Value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="03d1a-130">PartnerId</span><span class="sxs-lookup"><span data-stu-id="03d1a-130">PartnerId</span></span></td>
<td><p><span data-ttu-id="03d1a-131">Identificador exclusivo de uma entidade de cobrança específica, em formato GUID.</span><span class="sxs-lookup"><span data-stu-id="03d1a-131">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="03d1a-132">Não é necessário para reconciliação, mas pode ser uma informação útil.</span><span class="sxs-lookup"><span data-stu-id="03d1a-132">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="03d1a-133">O mesmo em todas as linhas.</span><span class="sxs-lookup"><span data-stu-id="03d1a-133">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="03d1a-134">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="03d1a-134">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="03d1a-135">CustomerID</span><span class="sxs-lookup"><span data-stu-id="03d1a-135">CustomerID</span></span></td>
<td><p><span data-ttu-id="03d1a-136">ID exclusiva da Microsoft, no formato GUID, usada para identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="03d1a-136">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="03d1a-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="03d1a-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="03d1a-138">OrderID</span><span class="sxs-lookup"><span data-stu-id="03d1a-138">OrderID</span></span></td>
<td><p><span data-ttu-id="03d1a-139">Identificador exclusivo para um pedido na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="03d1a-139">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="03d1a-140">Pode ser útil para identificar o pedido ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="03d1a-140">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="03d1a-141">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="03d1a-141">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="03d1a-142">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="03d1a-142">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="03d1a-143">Identificador exclusivo de uma assinatura na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="03d1a-143">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="03d1a-144">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="03d1a-144">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="03d1a-145">Esse não é o mesmo que o ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="03d1a-145">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="03d1a-146">Consulte Número_Assinatura_Parceiro_Sindicalização.</span><span class="sxs-lookup"><span data-stu-id="03d1a-146">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="03d1a-147">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="03d1a-147">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="03d1a-148">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="03d1a-148">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="03d1a-149">Identificador exclusivo para assinaturas.</span><span class="sxs-lookup"><span data-stu-id="03d1a-149">Unique identifier for subscriptions.</span></span> <span data-ttu-id="03d1a-150">Target: Um cliente pode ter várias assinaturas para o mesmo plano, portanto, isso é importante para análise de arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="03d1a-150">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="03d1a-151">Esse campo é mapeado para a ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="03d1a-151">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="03d1a-152">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="03d1a-152">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="03d1a-153">OfferID</span><span class="sxs-lookup"><span data-stu-id="03d1a-153">OfferID</span></span></td>
<td><p><span data-ttu-id="03d1a-154">ID exclusivo da oferta.</span><span class="sxs-lookup"><span data-stu-id="03d1a-154">Unique offer ID.</span></span> <span data-ttu-id="03d1a-155">ID padrão da oferta de acordo com a lista de preços.</span><span class="sxs-lookup"><span data-stu-id="03d1a-155">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="03d1a-156"><b>Observação</b>: esse valor não coincide com a ID de oferta da lista de preços.</span><span class="sxs-lookup"><span data-stu-id="03d1a-156"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="03d1a-157">Veja DurableOfferID abaixo.</span><span class="sxs-lookup"><span data-stu-id="03d1a-157">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="03d1a-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="03d1a-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="03d1a-159">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="03d1a-159">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="03d1a-160">ID exclusiva da oferta durável, conforme definido na tabela de preços.</span><span class="sxs-lookup"><span data-stu-id="03d1a-160">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="03d1a-161"><b>Observação</b>: esse valor corresponde à ID de oferta da lista de preços.</span><span class="sxs-lookup"><span data-stu-id="03d1a-161"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="03d1a-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="03d1a-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="03d1a-163">OfferName</span><span class="sxs-lookup"><span data-stu-id="03d1a-163">OfferName</span></span></td>
<td><p><span data-ttu-id="03d1a-164">O nome da oferta de serviço comprada pelo cliente, conforme definido na tabela de preços.</span><span class="sxs-lookup"><span data-stu-id="03d1a-164">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="03d1a-165">Microsoft Office 365 (plano E3)</span><span class="sxs-lookup"><span data-stu-id="03d1a-165">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="03d1a-166">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="03d1a-166">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="03d1a-167">A data de início da assinatura, definida como um dia após o pedido ser enviado.</span><span class="sxs-lookup"><span data-stu-id="03d1a-167">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="03d1a-168">Verificando a data de início da assinatura em conjunto com a data de término, você pode determinar se o cliente está dentro do primeiro ano da assinatura ou se a assinatura foi renovada para o ano seguinte.</span><span class="sxs-lookup"><span data-stu-id="03d1a-168">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="03d1a-169">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="03d1a-169">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="03d1a-170">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="03d1a-170">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="03d1a-171">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="03d1a-171">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="03d1a-172">A data do término da assinatura: 12 meses + x dias após a data de início (para se alinhar com a data de cobrança do parceiro) ou 12 meses a partir da data de renovação.</span><span class="sxs-lookup"><span data-stu-id="03d1a-172">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="03d1a-173">Na renovação, os preços são atualizados com a tabela de preços atual.</span><span class="sxs-lookup"><span data-stu-id="03d1a-173">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="03d1a-174">Um comunicado ao cliente pode ser necessário antes da renovação automática.</span><span class="sxs-lookup"><span data-stu-id="03d1a-174">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="03d1a-175">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="03d1a-175">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="03d1a-176">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="03d1a-176">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="03d1a-177">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="03d1a-177">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="03d1a-178">Dia de início dos encargos.</span><span class="sxs-lookup"><span data-stu-id="03d1a-178">Start day of the charges.</span></span></p>
<p><span data-ttu-id="03d1a-179">Quando o cliente muda o número de assentos, esse número é usado para calcular os encargos por dia (pro-rata).</span><span class="sxs-lookup"><span data-stu-id="03d1a-179">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="03d1a-180">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="03d1a-180">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="03d1a-181">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="03d1a-181">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="03d1a-182">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="03d1a-182">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="03d1a-183">Dia do término dos encargos.</span><span class="sxs-lookup"><span data-stu-id="03d1a-183">End day of the charges.</span></span></p>
<p><span data-ttu-id="03d1a-184">Quando o cliente muda o número de assentos, esse número é usado para calcular os encargos por dia (pro-rata).</span><span class="sxs-lookup"><span data-stu-id="03d1a-184">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="03d1a-185">A hora é sempre o fim do dia, 23:59.</span><span class="sxs-lookup"><span data-stu-id="03d1a-185">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="03d1a-186">28/2/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="03d1a-186">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="03d1a-187">ChargeType</span><span class="sxs-lookup"><span data-stu-id="03d1a-187">ChargeType</span></span></td>
<td><p><span data-ttu-id="03d1a-188">O tipo de encargo ou ajuste.</span><span class="sxs-lookup"><span data-stu-id="03d1a-188">The type of charge or adjustment.</span></span> <span data-ttu-id="03d1a-189">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="03d1a-189">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="03d1a-190">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="03d1a-190">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="03d1a-191">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="03d1a-191">UnitPrice</span></span></td>
<td><p><span data-ttu-id="03d1a-192">Preço por estação, conforme publicado na lista de preços no momento da compra.</span><span class="sxs-lookup"><span data-stu-id="03d1a-192">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="03d1a-193">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="03d1a-193">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="03d1a-194">6.82</span><span class="sxs-lookup"><span data-stu-id="03d1a-194">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="03d1a-195">Quantity</span><span class="sxs-lookup"><span data-stu-id="03d1a-195">Quantity</span></span></td>
<td><p><span data-ttu-id="03d1a-196">Número de assentos.</span><span class="sxs-lookup"><span data-stu-id="03d1a-196">Number of seats.</span></span> <span data-ttu-id="03d1a-197">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="03d1a-197">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="03d1a-198">2</span><span class="sxs-lookup"><span data-stu-id="03d1a-198">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="03d1a-199">Quantidade</span><span class="sxs-lookup"><span data-stu-id="03d1a-199">Amount</span></span></td>
<td><p><span data-ttu-id="03d1a-200">Preço total por quantidade.</span><span class="sxs-lookup"><span data-stu-id="03d1a-200">Total of price for quantity.</span></span> <span data-ttu-id="03d1a-201">Útil para verificar se o cálculo do valor coincide com a forma como você calcula isso para seus clientes.</span><span class="sxs-lookup"><span data-stu-id="03d1a-201">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="03d1a-202">13.32</span><span class="sxs-lookup"><span data-stu-id="03d1a-202">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="03d1a-203">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="03d1a-203">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="03d1a-204">Valor de desconto aplicado a esses encargos.</span><span class="sxs-lookup"><span data-stu-id="03d1a-204">Amount of discount applied to these charges.</span></span> <span data-ttu-id="03d1a-205">IUR ou novas assinaturas qualificadas para incentivo também conterão um valor de desconto nessa coluna.</span><span class="sxs-lookup"><span data-stu-id="03d1a-205">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="03d1a-206">2.32</span><span class="sxs-lookup"><span data-stu-id="03d1a-206">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="03d1a-207">Subtotal</span><span class="sxs-lookup"><span data-stu-id="03d1a-207">Subtotal</span></span></td>
<td><p><span data-ttu-id="03d1a-208">Total sem imposto.</span><span class="sxs-lookup"><span data-stu-id="03d1a-208">Total before tax.</span></span> <span data-ttu-id="03d1a-209">Verifica se seu subtotal corresponde ao total esperado, em caso de desconto.</span><span class="sxs-lookup"><span data-stu-id="03d1a-209">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="03d1a-210">11</span><span class="sxs-lookup"><span data-stu-id="03d1a-210">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="03d1a-211">Imposto</span><span class="sxs-lookup"><span data-stu-id="03d1a-211">Tax</span></span></td>
<td><p><span data-ttu-id="03d1a-212">Valor do imposto cobrado, com base no seu market& #39; s regras de fiscais e em circunstâncias específicas.</span><span class="sxs-lookup"><span data-stu-id="03d1a-212">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="03d1a-213">0</span><span class="sxs-lookup"><span data-stu-id="03d1a-213">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="03d1a-214">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="03d1a-214">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="03d1a-215">Total com imposto.</span><span class="sxs-lookup"><span data-stu-id="03d1a-215">Total after tax.</span></span> <span data-ttu-id="03d1a-216">Verifica se o imposto é cobrado na fatura.</span><span class="sxs-lookup"><span data-stu-id="03d1a-216">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="03d1a-217">11</span><span class="sxs-lookup"><span data-stu-id="03d1a-217">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="03d1a-218">Moeda</span><span class="sxs-lookup"><span data-stu-id="03d1a-218">Currency</span></span></td>
<td><p><span data-ttu-id="03d1a-219">Tipo de moeda.</span><span class="sxs-lookup"><span data-stu-id="03d1a-219">Currency type.</span></span> <span data-ttu-id="03d1a-220">Cada entidade de cobrança tem somente uma moeda.</span><span class="sxs-lookup"><span data-stu-id="03d1a-220">Each billing entity has only one currency.</span></span> <span data-ttu-id="03d1a-221">Verifique se isso coincide com a primeira fatura e faça o mesmo após grandes atualizações na plataforma de cobrança.</span><span class="sxs-lookup"><span data-stu-id="03d1a-221">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="03d1a-222">Euro</span><span class="sxs-lookup"><span data-stu-id="03d1a-222">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="03d1a-223">CustomerName</span><span class="sxs-lookup"><span data-stu-id="03d1a-223">CustomerName</span></span></td>
<td><p><span data-ttu-id="03d1a-224">Customer& #39; o nome da organização s como informado no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="03d1a-224">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="03d1a-225">Isso é muito importante para reconciliar a fatura com as informações de seu sistema.</span><span class="sxs-lookup"><span data-stu-id="03d1a-225">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="03d1a-226">Cliente de teste A</span><span class="sxs-lookup"><span data-stu-id="03d1a-226">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="03d1a-227">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="03d1a-227">MPNID</span></span></td>
<td><p><span data-ttu-id="03d1a-228">ID do MPN do parceiro CSP</span><span class="sxs-lookup"><span data-stu-id="03d1a-228">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="03d1a-229">4390934</span><span class="sxs-lookup"><span data-stu-id="03d1a-229">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="03d1a-230">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="03d1a-230">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="03d1a-231">ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="03d1a-231">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="03d1a-232">Consulte <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Discriminar por parceiro</a>.</span><span class="sxs-lookup"><span data-stu-id="03d1a-232">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="03d1a-233">4390934</span><span class="sxs-lookup"><span data-stu-id="03d1a-233">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="03d1a-234">DomainName</span><span class="sxs-lookup"><span data-stu-id="03d1a-234">DomainName</span></span></td>
<td><p><span data-ttu-id="03d1a-235">Customer& #39; o nome de domínio s, usado para ajudar a identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="03d1a-235">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="03d1a-236">Isso não deve ser usado para identificar exclusivamente o cliente como o cliente/parceiro pode atualizar o domínio banidos/padrão através do portal do O365.</span><span class="sxs-lookup"><span data-stu-id="03d1a-236">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="03d1a-237">Este campo pode aparecer em branco até o segundo ciclo de cobrança.</span><span class="sxs-lookup"><span data-stu-id="03d1a-237">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="03d1a-238">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="03d1a-238">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="03d1a-239">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="03d1a-239">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="03d1a-240">Apelido da Inscrição.</span><span class="sxs-lookup"><span data-stu-id="03d1a-240">Subscription nickname.</span></span> <span data-ttu-id="03d1a-241">Se nenhum apelido for especificado, o Partner Center usa o OfferName.</span><span class="sxs-lookup"><span data-stu-id="03d1a-241">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="03d1a-242">PROJETO ONLINE</span><span class="sxs-lookup"><span data-stu-id="03d1a-242">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="03d1a-243">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="03d1a-243">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="03d1a-244">O nome da oferta de serviço comprada pelo cliente, conforme definido na tabela de preços.</span><span class="sxs-lookup"><span data-stu-id="03d1a-244">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="03d1a-245">(Este é um campo idêntico ao nome da oferta).</span><span class="sxs-lookup"><span data-stu-id="03d1a-245">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="03d1a-246">PROJETO ONLINE PREMIUM SEM PROJETO CLIENTE</span><span class="sxs-lookup"><span data-stu-id="03d1a-246">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="03d1a-247">Campos de arquivo baseado em uso</span><span class="sxs-lookup"><span data-stu-id="03d1a-247">Usage-based file fields</span></span>


<span data-ttu-id="03d1a-248">Para reconciliar seus encargos com o uso de seu cliente, compare ResellerID/ResellerName/ResellerBillableAccount do arquivo de reconciliação com o nome do cliente e a ID da assinatura do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="03d1a-248">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="03d1a-249">Os campos a seguir explicam quais serviços foram usados e a taxa.</span><span class="sxs-lookup"><span data-stu-id="03d1a-249">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="03d1a-250">Coluna</span><span class="sxs-lookup"><span data-stu-id="03d1a-250">Column</span></span></strong></td>
<td><strong><span data-ttu-id="03d1a-251">Descrição</span><span class="sxs-lookup"><span data-stu-id="03d1a-251">Description</span></span></strong></td>
<td><strong><span data-ttu-id="03d1a-252">Valor de exemplo</span><span class="sxs-lookup"><span data-stu-id="03d1a-252">Sample value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="03d1a-253">PartnerID</span><span class="sxs-lookup"><span data-stu-id="03d1a-253">PartnerID</span></span></td>
<td><p><span data-ttu-id="03d1a-254">ID do parceiro, no formato GUID.</span><span class="sxs-lookup"><span data-stu-id="03d1a-254">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="03d1a-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="03d1a-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="03d1a-256">PartnerName</span><span class="sxs-lookup"><span data-stu-id="03d1a-256">PartnerName</span></span></td>
<td><p><span data-ttu-id="03d1a-257">Nome do parceiro.</span><span class="sxs-lookup"><span data-stu-id="03d1a-257">Partner Name.</span></span></p></td>
<td><span data-ttu-id="03d1a-258">Acme incorporado</span><span class="sxs-lookup"><span data-stu-id="03d1a-258">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="03d1a-259">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="03d1a-259">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="03d1a-260">ID da conta do parceiro.</span><span class="sxs-lookup"><span data-stu-id="03d1a-260">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="03d1a-261">1010578050</span><span class="sxs-lookup"><span data-stu-id="03d1a-261">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="03d1a-262">CustomerName</span><span class="sxs-lookup"><span data-stu-id="03d1a-262">CustomerName</span></span></td>
<td><p><span data-ttu-id="03d1a-263">Customer& #39; o nome da organização s como informado no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="03d1a-263">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="03d1a-264">Isso é muito importante para reconciliar a fatura com as informações de seu sistema.</span><span class="sxs-lookup"><span data-stu-id="03d1a-264">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="03d1a-265">Cliente de teste A</span><span class="sxs-lookup"><span data-stu-id="03d1a-265">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="03d1a-266">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="03d1a-266">MPNID</span></span></td>
<td><p><span data-ttu-id="03d1a-267">ID do MPN do parceiro CSP.</span><span class="sxs-lookup"><span data-stu-id="03d1a-267">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="03d1a-268">4390934</span><span class="sxs-lookup"><span data-stu-id="03d1a-268">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="03d1a-269">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="03d1a-269">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="03d1a-270">ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="03d1a-270">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="03d1a-271">Consulte <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Discriminar por parceiro</a>.</span><span class="sxs-lookup"><span data-stu-id="03d1a-271">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="03d1a-272">4390934</span><span class="sxs-lookup"><span data-stu-id="03d1a-272">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="03d1a-273">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="03d1a-273">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="03d1a-274">Número da fatura na qual a transação especificada é exibida.</span><span class="sxs-lookup"><span data-stu-id="03d1a-274">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="03d1a-275">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="03d1a-275">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="03d1a-276">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="03d1a-276">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="03d1a-277">Data de início do ciclo de cobrança exceto quando apresentadas as datas de dados de uso latentes anteriormente não cobradas (do ciclo de cobrança anterior).</span><span class="sxs-lookup"><span data-stu-id="03d1a-277">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="03d1a-278">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="03d1a-278">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="03d1a-279">1/2/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="03d1a-279">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="03d1a-280">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="03d1a-280">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="03d1a-281">Data de término do ciclo de cobrança exceto quando apresentadas as datas de dados de uso latentes anteriormente não cobradas (do ciclo de cobrança anterior).</span><span class="sxs-lookup"><span data-stu-id="03d1a-281">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="03d1a-282">A hora é sempre o fim do dia, 23:59.</span><span class="sxs-lookup"><span data-stu-id="03d1a-282">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="03d1a-283">28/2/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="03d1a-283">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="03d1a-284">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="03d1a-284">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="03d1a-285">Identificador exclusivo de uma assinatura na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="03d1a-285">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="03d1a-286">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="03d1a-286">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="03d1a-287">Esse não é o mesmo que a ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="03d1a-287">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="03d1a-288">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="03d1a-288">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="03d1a-289">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="03d1a-289">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="03d1a-290">Apelido da oferta do serviço.</span><span class="sxs-lookup"><span data-stu-id="03d1a-290">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="03d1a-291">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="03d1a-291">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="03d1a-292">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="03d1a-292">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="03d1a-293">Linha de negócios da oferta do serviço</span><span class="sxs-lookup"><span data-stu-id="03d1a-293">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="03d1a-294">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="03d1a-294">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="03d1a-295">OrderID</span><span class="sxs-lookup"><span data-stu-id="03d1a-295">OrderID</span></span></td>
<td><p><span data-ttu-id="03d1a-296">Identificador exclusivo para um pedido na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="03d1a-296">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="03d1a-297">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="03d1a-297">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="03d1a-298">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="03d1a-298">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="03d1a-299">ServiceName</span><span class="sxs-lookup"><span data-stu-id="03d1a-299">ServiceName</span></span></td>
<td><p><span data-ttu-id="03d1a-300">O nome do serviço do Azure em questão.</span><span class="sxs-lookup"><span data-stu-id="03d1a-300">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="03d1a-301">MÁQUINAS VIRTUAIS</span><span class="sxs-lookup"><span data-stu-id="03d1a-301">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="03d1a-302">ServiceType</span><span class="sxs-lookup"><span data-stu-id="03d1a-302">ServiceType</span></span></td>
<td><p><span data-ttu-id="03d1a-303">O tipo específico de serviço do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="03d1a-303">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="03d1a-304">Service Bus – Individual ou pacote</span><span class="sxs-lookup"><span data-stu-id="03d1a-304">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="03d1a-305">Banco de dados SQL Azure – Edição empresa ou Web</span><span class="sxs-lookup"><span data-stu-id="03d1a-305">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="03d1a-306">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="03d1a-306">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="03d1a-307">Identificador exclusivo específico de toda a estrutura de serviço de dados e preço.</span><span class="sxs-lookup"><span data-stu-id="03d1a-307">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="03d1a-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="03d1a-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="03d1a-309">Nome do recurso</span><span class="sxs-lookup"><span data-stu-id="03d1a-309">Resource Name</span></span></td>
<td><p><span data-ttu-id="03d1a-310">O nome do recurso do Azure.</span><span class="sxs-lookup"><span data-stu-id="03d1a-310">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="03d1a-311">Dados de entrada transferidos (GB)</span><span class="sxs-lookup"><span data-stu-id="03d1a-311">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="03d1a-312">Dados de saída transferidos (GB)</span><span class="sxs-lookup"><span data-stu-id="03d1a-312">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="03d1a-313">Região</span><span class="sxs-lookup"><span data-stu-id="03d1a-313">Region</span></span></td>
<td><p><span data-ttu-id="03d1a-314">A região a qual o uso se aplica.</span><span class="sxs-lookup"><span data-stu-id="03d1a-314">The region the usage applies to.</span></span> <span data-ttu-id="03d1a-315">Usado principalmente para atribuir as taxas de transferências de dados, já que as taxas variam de acordo com a região.</span><span class="sxs-lookup"><span data-stu-id="03d1a-315">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="03d1a-316">Pacífico Asiático, Europa, América Latina e América do Norte</span><span class="sxs-lookup"><span data-stu-id="03d1a-316">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="03d1a-317">SKU</span><span class="sxs-lookup"><span data-stu-id="03d1a-317">SKU</span></span></td>
<td><p><span data-ttu-id="03d1a-318">Identificador exclusivo MSFT da oferta</span><span class="sxs-lookup"><span data-stu-id="03d1a-318">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="03d1a-319">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="03d1a-319">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="03d1a-320">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="03d1a-320">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="03d1a-321">Uma ID e a quantidade para discriminar as taxas diferentes de um serviço ou recurso em um determinado período de cobrança.</span><span class="sxs-lookup"><span data-stu-id="03d1a-321">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="03d1a-322">Para a classificação em camadas do Azure, pode haver uma taxa para uma determinada quantidade de unidades faturáveis e uma taxa diferente depois disso.</span><span class="sxs-lookup"><span data-stu-id="03d1a-322">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="03d1a-323">1</span><span class="sxs-lookup"><span data-stu-id="03d1a-323">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="03d1a-324">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="03d1a-324">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="03d1a-325">A quantidade de serviço consumida (horas, GB etc.) durante o período de relatório.</span><span class="sxs-lookup"><span data-stu-id="03d1a-325">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="03d1a-326">Também inclui qualquer uso não cobrado de períodos de relatório anteriores.</span><span class="sxs-lookup"><span data-stu-id="03d1a-326">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="03d1a-327">11</span><span class="sxs-lookup"><span data-stu-id="03d1a-327">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="03d1a-328">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="03d1a-328">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="03d1a-329">Unidades incluídas como parte da oferta.</span><span class="sxs-lookup"><span data-stu-id="03d1a-329">Units included as part of the offer.</span></span> <span data-ttu-id="03d1a-330">Normalmente não está presente no CSP.</span><span class="sxs-lookup"><span data-stu-id="03d1a-330">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="03d1a-331">0</span><span class="sxs-lookup"><span data-stu-id="03d1a-331">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="03d1a-332">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="03d1a-332">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="03d1a-333">Unidades não incluídas como parte da oferta devem ser pagas pelo parceiro.</span><span class="sxs-lookup"><span data-stu-id="03d1a-333">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="03d1a-334">Igual a ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="03d1a-334">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="03d1a-335">11</span><span class="sxs-lookup"><span data-stu-id="03d1a-335">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="03d1a-336">ListPrice</span><span class="sxs-lookup"><span data-stu-id="03d1a-336">ListPrice</span></span></td>
<td><p><span data-ttu-id="03d1a-337">Preço da oferta em vigor na data de início da assinatura.</span><span class="sxs-lookup"><span data-stu-id="03d1a-337">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="03d1a-338">U$ 0,0808</span><span class="sxs-lookup"><span data-stu-id="03d1a-338">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="03d1a-339">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="03d1a-339">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="03d1a-340">ListPrist vezes OverageQuantity, arredondado para o centavo mais próximo.</span><span class="sxs-lookup"><span data-stu-id="03d1a-340">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="03d1a-341">U$ 0,085</span><span class="sxs-lookup"><span data-stu-id="03d1a-341">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="03d1a-342">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="03d1a-342">TaxAmount</span></span></td>
<td><p><span data-ttu-id="03d1a-343">Valor do imposto cobrado, com base no seu market& #39; s regras de fiscais e em circunstâncias específicas.</span><span class="sxs-lookup"><span data-stu-id="03d1a-343">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="03d1a-344">U$ 0,08</span><span class="sxs-lookup"><span data-stu-id="03d1a-344">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="03d1a-345">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="03d1a-345">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="03d1a-346">Total após imposto, quando o imposto é aplicável.</span><span class="sxs-lookup"><span data-stu-id="03d1a-346">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="03d1a-347">U$ 0,93</span><span class="sxs-lookup"><span data-stu-id="03d1a-347">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="03d1a-348">Moeda</span><span class="sxs-lookup"><span data-stu-id="03d1a-348">Currency</span></span></td>
<td><p><span data-ttu-id="03d1a-349">Tipo de moeda.</span><span class="sxs-lookup"><span data-stu-id="03d1a-349">Currency type.</span></span> <span data-ttu-id="03d1a-350">Cada entidade de cobrança tem somente uma moeda.</span><span class="sxs-lookup"><span data-stu-id="03d1a-350">Each billing entity has only one currency.</span></span> <span data-ttu-id="03d1a-351">Verifique se isso coincide com a primeira fatura e faça o mesmo após grandes atualizações na plataforma de cobrança.</span><span class="sxs-lookup"><span data-stu-id="03d1a-351">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="03d1a-352">Euro</span><span class="sxs-lookup"><span data-stu-id="03d1a-352">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="03d1a-353">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="03d1a-353">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="03d1a-354">Preço por unidade sem imposto.</span><span class="sxs-lookup"><span data-stu-id="03d1a-354">Pretax price per unit.</span></span> <span data-ttu-id="03d1a-355">Igual a PretaxCharges / OverageQuantity, arredondado para o centavo mais próximo.</span><span class="sxs-lookup"><span data-stu-id="03d1a-355">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="03d1a-356">U$ 0,08</span><span class="sxs-lookup"><span data-stu-id="03d1a-356">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="03d1a-357">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="03d1a-357">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="03d1a-358">Preço pós-imposto por unidade.</span><span class="sxs-lookup"><span data-stu-id="03d1a-358">Post tax price per unit.</span></span> <span data-ttu-id="03d1a-359">Igual a PostTaxTotal / OverageQuantity, ou PretaxEffectiveRate + taxa de imposto por valor de unidade, arredondado para o centavo mais próximo.</span><span class="sxs-lookup"><span data-stu-id="03d1a-359">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="03d1a-360">U$ 0,08</span><span class="sxs-lookup"><span data-stu-id="03d1a-360">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="03d1a-361">ChargeType</span><span class="sxs-lookup"><span data-stu-id="03d1a-361">ChargeType</span></span></td>
<td><p><span data-ttu-id="03d1a-362">O tipo de encargo ou ajuste.</span><span class="sxs-lookup"><span data-stu-id="03d1a-362">The type of charge or adjustment.</span></span> <span data-ttu-id="03d1a-363">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="03d1a-363">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="03d1a-364">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="03d1a-364">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="03d1a-365">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="03d1a-365">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="03d1a-366">ID exclusiva da conta na plataforma de cobrança da MSFT.</span><span class="sxs-lookup"><span data-stu-id="03d1a-366">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="03d1a-367">1280018095</span><span class="sxs-lookup"><span data-stu-id="03d1a-367">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="03d1a-368">UsageDate</span><span class="sxs-lookup"><span data-stu-id="03d1a-368">UsageDate</span></span></td>
<td><p><span data-ttu-id="03d1a-369">Data da implantação do serviço.</span><span class="sxs-lookup"><span data-stu-id="03d1a-369">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="03d1a-370">1/2/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="03d1a-370">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="03d1a-371">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="03d1a-371">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="03d1a-372">Essa coluna identifica a localização de um data center dentro da região para serviços onde isso é aplicável e preenchido.</span><span class="sxs-lookup"><span data-stu-id="03d1a-372">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="03d1a-373">Leste da Ásia, Sudeste da Ásia, Norte da Europa, Europa Ocidental, Centro Norte e Centro Sul dos EUA</span><span class="sxs-lookup"><span data-stu-id="03d1a-373">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="03d1a-374">MeteredService</span><span class="sxs-lookup"><span data-stu-id="03d1a-374">MeteredService</span></span></td>
<td><p><span data-ttu-id="03d1a-375">Essa coluna é utilizada para rastrear o serviço do Microsoft Azure individual que não pode ser identificado especificamente na coluna Nome do Serviço.</span><span class="sxs-lookup"><span data-stu-id="03d1a-375">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="03d1a-376">Por exemplo, transferências de dados são relatadas como &quot;Microsoft Azure – Todos os Serviços&quot; na coluna Nome do Serviço.</span><span class="sxs-lookup"><span data-stu-id="03d1a-376">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="03d1a-377">Essa coluna MeteredService indicará ao qual serviço específico o uso pertence.</span><span class="sxs-lookup"><span data-stu-id="03d1a-377">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="03d1a-378">AccessControl, CDN, Computação, Banco de dados, ServiceBus, Armazenamento</span><span class="sxs-lookup"><span data-stu-id="03d1a-378">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="03d1a-379">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="03d1a-379">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="03d1a-380">Um subcabeçalho que esclarece ainda mais o serviço Microsoft Azure individual além do nível fornecido pelo campo MeteredService.</span><span class="sxs-lookup"><span data-stu-id="03d1a-380">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="03d1a-381">EXTERNO</span><span class="sxs-lookup"><span data-stu-id="03d1a-381">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="03d1a-382">Projeto</span><span class="sxs-lookup"><span data-stu-id="03d1a-382">Project</span></span></td>
<td><p><span data-ttu-id="03d1a-383">Nome definido pelo cliente para a instância do serviço</span><span class="sxs-lookup"><span data-stu-id="03d1a-383">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="03d1a-384">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="03d1a-384">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="03d1a-385">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="03d1a-385">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="03d1a-386">O número de conexões ServiceBus que foram provisionados e utilizados em um dia específico.</span><span class="sxs-lookup"><span data-stu-id="03d1a-386">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="03d1a-387">Por exemplo: se você tivesse uma conexão individualmente provisionada durante um mês de 30 dias, a coluna Informação do Serviço 1 lerá "1,000000 conexões/30 dias".</span><span class="sxs-lookup"><span data-stu-id="03d1a-387">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="03d1a-388">Se você tinha um pacote de 25 conexões ServiceBus provisionadas e você utilizou 1 durante o dia, sua declaração de uso diário para esse dia indicaria "25 conexões/30 dias – Usado: 1,000000".</span><span class="sxs-lookup"><span data-stu-id="03d1a-388">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="03d1a-389">CustomerID</span><span class="sxs-lookup"><span data-stu-id="03d1a-389">CustomerID</span></span></td>
<td><p><span data-ttu-id="03d1a-390">ID exclusiva da Microsoft, no formato GUID, usada para identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="03d1a-390">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="03d1a-391">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="03d1a-391">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="03d1a-392">DomainName</span><span class="sxs-lookup"><span data-stu-id="03d1a-392">DomainName</span></span></td>
<td><p><span data-ttu-id="03d1a-393">Customer& #39; o nome de domínio s, usado para ajudar a identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="03d1a-393">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="03d1a-394">Este campo pode aparecer em branco até o segundo ciclo de cobrança.</span><span class="sxs-lookup"><span data-stu-id="03d1a-394">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="03d1a-395">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="03d1a-395">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="03d1a-396">Unidade</span><span class="sxs-lookup"><span data-stu-id="03d1a-396">Unit</span></span></td>
<td><p><span data-ttu-id="03d1a-397">A unidade do nome do recurso</span><span class="sxs-lookup"><span data-stu-id="03d1a-397">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="03d1a-398">GB ou HORAS</span><span class="sxs-lookup"><span data-stu-id="03d1a-398">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="03d1a-399">Campos de arquivo únicas e recorrentes</span><span class="sxs-lookup"><span data-stu-id="03d1a-399">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="03d1a-400">Coluna</span><span class="sxs-lookup"><span data-stu-id="03d1a-400">Column</span></span></th>
<th><span data-ttu-id="03d1a-401">Descrição</span><span class="sxs-lookup"><span data-stu-id="03d1a-401">Description</span></span></th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td><span data-ttu-id="03d1a-402">PartnerId</span><span class="sxs-lookup"><span data-stu-id="03d1a-402">PartnerId</span></span></td>
<td><p><span data-ttu-id="03d1a-403">Identificador exclusivo de locatário Microsoft Azure Active Directory para uma entidade de cobrança específica, no formato GUID.</span><span class="sxs-lookup"><span data-stu-id="03d1a-403">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="03d1a-404">Não é necessário para reconciliação, mas pode ser uma informação útil.</span><span class="sxs-lookup"><span data-stu-id="03d1a-404">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="03d1a-405">O mesmo em todas as linhas.</span><span class="sxs-lookup"><span data-stu-id="03d1a-405">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="03d1a-406">Id do cliente</span><span class="sxs-lookup"><span data-stu-id="03d1a-406">Customer Id</span></span></td>
<td><p><span data-ttu-id="03d1a-407">Microsoft Azure Active Directory locatário ID exclusiva, no formato GUID, usada para identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="03d1a-407">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="03d1a-408">Nome do cliente</span><span class="sxs-lookup"><span data-stu-id="03d1a-408">Customer Name</span></span></td>
<td><p><span data-ttu-id="03d1a-409">Nome da organização do cliente como informado no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="03d1a-409">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="03d1a-410">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="03d1a-410">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="03d1a-411">Nome de domínio do cliente, usado para ajudar a identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="03d1a-411">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="03d1a-412">Isso não deve ser usado para identificar exclusivamente o cliente como o cliente/parceiro pode atualizar o domínio banidos/padrão através do portal do O365.</span><span class="sxs-lookup"><span data-stu-id="03d1a-412">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="03d1a-413">Este campo pode aparecer em branco até o segundo ciclo de cobrança.</span><span class="sxs-lookup"><span data-stu-id="03d1a-413">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="03d1a-414">País do cliente</span><span class="sxs-lookup"><span data-stu-id="03d1a-414">Customer Country</span></span></td>
<td><p><span data-ttu-id="03d1a-415">O país em que o cliente está localizado.</span><span class="sxs-lookup"><span data-stu-id="03d1a-415">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="03d1a-416">Número da fatura</span><span class="sxs-lookup"><span data-stu-id="03d1a-416">Invoice number</span></span></td>
<td><p><span data-ttu-id="03d1a-417">Número da fatura na qual a transação especificada é exibida.</span><span class="sxs-lookup"><span data-stu-id="03d1a-417">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="03d1a-418">MpnId</span><span class="sxs-lookup"><span data-stu-id="03d1a-418">MpnId</span></span></td>
<td><p><span data-ttu-id="03d1a-419">ID do MPN do parceiro CSP.</span><span class="sxs-lookup"><span data-stu-id="03d1a-419">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="03d1a-420">ID do MPN do revendedor</span><span class="sxs-lookup"><span data-stu-id="03d1a-420">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="03d1a-421">ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="03d1a-421">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="03d1a-422">ID do Pedido</span><span class="sxs-lookup"><span data-stu-id="03d1a-422">Order ID</span></span></td>
<td><p><span data-ttu-id="03d1a-423">Identificador exclusivo para um pedido na plataforma de comércio da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="03d1a-423">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="03d1a-424">Pode ser útil para identificar o pedido ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="03d1a-424">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="03d1a-425">Data do pedido</span><span class="sxs-lookup"><span data-stu-id="03d1a-425">Order date</span></span></td>
<td><p><span data-ttu-id="03d1a-426">A data em que o pedido foi feito.</span><span class="sxs-lookup"><span data-stu-id="03d1a-426">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="03d1a-427">ProductId</span><span class="sxs-lookup"><span data-stu-id="03d1a-427">ProductId</span></span></td>
<td><p><span data-ttu-id="03d1a-428">A ID do produto.</span><span class="sxs-lookup"><span data-stu-id="03d1a-428">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="03d1a-429">SkuId</span><span class="sxs-lookup"><span data-stu-id="03d1a-429">SkuId</span></span></td>
<td><p><span data-ttu-id="03d1a-430">A ID de uma SKU em particular.</span><span class="sxs-lookup"><span data-stu-id="03d1a-430">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="03d1a-431">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="03d1a-431">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="03d1a-432">A ID de uma Disponibilidade em particular.</span><span class="sxs-lookup"><span data-stu-id="03d1a-432">The ID for a particular Availability.</span></span> <span data-ttu-id="03d1a-433">"Disponibilidade" refere-se a se uma SKU em particular está disponível ou não para compra para determinado país, moeda, segmento do setor etc.</span><span class="sxs-lookup"><span data-stu-id="03d1a-433">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="03d1a-434">Nome SKU</span><span class="sxs-lookup"><span data-stu-id="03d1a-434">SKU Name</span></span></td>
<td><p><span data-ttu-id="03d1a-435">O título de uma SKU em particular.</span><span class="sxs-lookup"><span data-stu-id="03d1a-435">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="03d1a-436">Nome do produto</span><span class="sxs-lookup"><span data-stu-id="03d1a-436">Product name</span></span></td>
<td><p><span data-ttu-id="03d1a-437">O nome do produto.</span><span class="sxs-lookup"><span data-stu-id="03d1a-437">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="03d1a-438">PublisherName</span><span class="sxs-lookup"><span data-stu-id="03d1a-438">PublisherName</span></span></td>
<td><p><span data-ttu-id="03d1a-439">O nome do fornecedor do produto.</span><span class="sxs-lookup"><span data-stu-id="03d1a-439">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="03d1a-440">PublisherID</span><span class="sxs-lookup"><span data-stu-id="03d1a-440">PublisherID</span></span></td>
<td><p><span data-ttu-id="03d1a-441">ID exclusiva para esse fornecedor.</span><span class="sxs-lookup"><span data-stu-id="03d1a-441">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="03d1a-442">Descrição de assinatura</span><span class="sxs-lookup"><span data-stu-id="03d1a-442">Subscription Description</span></span></td>
<td><p><span data-ttu-id="03d1a-443">Nome amigável de uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="03d1a-443">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="03d1a-444">ID da assinatura</span><span class="sxs-lookup"><span data-stu-id="03d1a-444">Subscription ID</span></span></td>
<td><p><span data-ttu-id="03d1a-445">Identificador exclusivo de uma assinatura na plataforma de comércio da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="03d1a-445">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="03d1a-446">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="03d1a-446">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="03d1a-447">Esse não é o mesmo que a ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="03d1a-447">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="03d1a-448">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="03d1a-448">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="03d1a-449">Dia de início dos encargos.</span><span class="sxs-lookup"><span data-stu-id="03d1a-449">Start day of the charges.</span></span> <span data-ttu-id="03d1a-450">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="03d1a-450">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="03d1a-451">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="03d1a-451">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="03d1a-452">Dia do término dos encargos.</span><span class="sxs-lookup"><span data-stu-id="03d1a-452">End day of the charges.</span></span> <span data-ttu-id="03d1a-453">A hora é sempre o fim do dia, 23:59.</span><span class="sxs-lookup"><span data-stu-id="03d1a-453">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="03d1a-454">Termo e Billingcycle</span><span class="sxs-lookup"><span data-stu-id="03d1a-454">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="03d1a-455">O comprimento do termo e o ciclo de cobrança da compra.</span><span class="sxs-lookup"><span data-stu-id="03d1a-455">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="03d1a-456">Por exemplo, "1 ano, mensalmente."</span><span class="sxs-lookup"><span data-stu-id="03d1a-456">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="03d1a-457">Tipo de Cobrança</span><span class="sxs-lookup"><span data-stu-id="03d1a-457">Charge Type</span></span></td>
<td><p><span data-ttu-id="03d1a-458">O tipo de encargo ou ajuste.</span><span class="sxs-lookup"><span data-stu-id="03d1a-458">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="03d1a-459">Preço unitário</span><span class="sxs-lookup"><span data-stu-id="03d1a-459">Unit Price</span></span></td>
<td><p><span data-ttu-id="03d1a-460">O preço conforme publicado na lista de preços no momento da compra.</span><span class="sxs-lookup"><span data-stu-id="03d1a-460">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="03d1a-461">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="03d1a-461">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="03d1a-462">Preço unitário efetivos</span><span class="sxs-lookup"><span data-stu-id="03d1a-462">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="03d1a-463">O preço unitário após ajustes terem sido feitas.</span><span class="sxs-lookup"><span data-stu-id="03d1a-463">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="03d1a-464">Quantidade</span><span class="sxs-lookup"><span data-stu-id="03d1a-464">Quantity</span></span></td>
<td><p><span data-ttu-id="03d1a-465">Número de unidades.</span><span class="sxs-lookup"><span data-stu-id="03d1a-465">Number of units.</span></span> <span data-ttu-id="03d1a-466">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="03d1a-466">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="03d1a-467">Tipo de unidade</span><span class="sxs-lookup"><span data-stu-id="03d1a-467">Unit type</span></span></td>
<td><p><span data-ttu-id="03d1a-468">O tipo de unidade que está sendo comprado.</span><span class="sxs-lookup"><span data-stu-id="03d1a-468">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="03d1a-469">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="03d1a-469">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="03d1a-470">Uma explicação sobre qualquer desconto aplicável.</span><span class="sxs-lookup"><span data-stu-id="03d1a-470">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="03d1a-471">Subtotal</span><span class="sxs-lookup"><span data-stu-id="03d1a-471">Sub Total</span></span></td>
<td><p><span data-ttu-id="03d1a-472">Total sem imposto.</span><span class="sxs-lookup"><span data-stu-id="03d1a-472">Total before tax.</span></span> <span data-ttu-id="03d1a-473">Verifica se seu subtotal corresponde ao total esperado, em caso de desconto.</span><span class="sxs-lookup"><span data-stu-id="03d1a-473">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="03d1a-474">Total do imposto</span><span class="sxs-lookup"><span data-stu-id="03d1a-474">Tax Total</span></span></td>
<td><p><span data-ttu-id="03d1a-475">Valor do imposto cobrado, com base nas regras fiscais do mercado e em circunstâncias específicas.</span><span class="sxs-lookup"><span data-stu-id="03d1a-475">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="03d1a-476">Total</span><span class="sxs-lookup"><span data-stu-id="03d1a-476">Total</span></span></td>
<td><p><span data-ttu-id="03d1a-477">Total com imposto.</span><span class="sxs-lookup"><span data-stu-id="03d1a-477">Total after tax.</span></span> <span data-ttu-id="03d1a-478">Verifica se o imposto é cobrado na fatura.</span><span class="sxs-lookup"><span data-stu-id="03d1a-478">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="03d1a-479">Moeda</span><span class="sxs-lookup"><span data-stu-id="03d1a-479">Currency</span></span></td>
<td><p><span data-ttu-id="03d1a-480">Tipo de moeda.</span><span class="sxs-lookup"><span data-stu-id="03d1a-480">Currency type.</span></span> <span data-ttu-id="03d1a-481">Cada entidade de cobrança tem somente uma moeda.</span><span class="sxs-lookup"><span data-stu-id="03d1a-481">Each billing entity has only one currency.</span></span> <span data-ttu-id="03d1a-482">Verifique se isso coincide com a primeira fatura e faça o mesmo após grandes atualizações na plataforma de cobrança.</span><span class="sxs-lookup"><span data-stu-id="03d1a-482">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="03d1a-483">AlternateID</span><span class="sxs-lookup"><span data-stu-id="03d1a-483">AlternateID</span></span></td>
<td><p><span data-ttu-id="03d1a-484">Um identificador alternativo para uma ID.</span><span class="sxs-lookup"><span data-stu-id="03d1a-484">An alternate identifier to an ID.</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="03d1a-485">Campos de arquivo de uso proporcional diariamente</span><span class="sxs-lookup"><span data-stu-id="03d1a-485">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="03d1a-486">Coluna</span><span class="sxs-lookup"><span data-stu-id="03d1a-486">Column</span></span></th>
<th><span data-ttu-id="03d1a-487">Descrição</span><span class="sxs-lookup"><span data-stu-id="03d1a-487">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="03d1a-488">PartnerId</span><span class="sxs-lookup"><span data-stu-id="03d1a-488">PartnerId</span></span></td>
<td><p><span data-ttu-id="03d1a-489">ID do parceiro, no formato GUID.</span><span class="sxs-lookup"><span data-stu-id="03d1a-489">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="03d1a-490">PartnerName</span><span class="sxs-lookup"><span data-stu-id="03d1a-490">PartnerName</span></span></td>
<td><p><span data-ttu-id="03d1a-491">Nome do parceiro.</span><span class="sxs-lookup"><span data-stu-id="03d1a-491">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="03d1a-492">CustomerID</span><span class="sxs-lookup"><span data-stu-id="03d1a-492">CustomerId</span></span></td>
<td><p><span data-ttu-id="03d1a-493">ID exclusiva da Microsoft, no formato GUID, usada para identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="03d1a-493">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="03d1a-494">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="03d1a-494">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="03d1a-495">Nome da organização do cliente como informado no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="03d1a-495">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="03d1a-496">Isso é muito importante para reconciliar a fatura com as informações de seu sistema.</span><span class="sxs-lookup"><span data-stu-id="03d1a-496">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="03d1a-497">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="03d1a-497">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="03d1a-498">O nome de domínio do cliente.</span><span class="sxs-lookup"><span data-stu-id="03d1a-498">The customer’s domain name.</span></span> <span data-ttu-id="03d1a-499">Não está disponível para a atividade atual.</span><span class="sxs-lookup"><span data-stu-id="03d1a-499">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="03d1a-500">País do cliente</span><span class="sxs-lookup"><span data-stu-id="03d1a-500">Customer country</span></span></td>
<td><p><span data-ttu-id="03d1a-501">O país em que o cliente está localizado.</span><span class="sxs-lookup"><span data-stu-id="03d1a-501">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="03d1a-502">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="03d1a-502">MPNID</span></span></td>
<td><p><span data-ttu-id="03d1a-503">ID do MPN do parceiro CSP.</span><span class="sxs-lookup"><span data-stu-id="03d1a-503">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="03d1a-504">ID do MPN do revendedor</span><span class="sxs-lookup"><span data-stu-id="03d1a-504">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="03d1a-505">ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="03d1a-505">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="03d1a-506">Não está disponível para a atividade atual.</span><span class="sxs-lookup"><span data-stu-id="03d1a-506">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="03d1a-507">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="03d1a-507">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="03d1a-508">Número da fatura na qual a transação especificada é exibida.</span><span class="sxs-lookup"><span data-stu-id="03d1a-508">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="03d1a-509">Não está disponível para a atividade atual.</span><span class="sxs-lookup"><span data-stu-id="03d1a-509">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="03d1a-510">ProductId</span><span class="sxs-lookup"><span data-stu-id="03d1a-510">ProductId</span></span></td>
<td><p><span data-ttu-id="03d1a-511">A ID do produto.</span><span class="sxs-lookup"><span data-stu-id="03d1a-511">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="03d1a-512">SkuId</span><span class="sxs-lookup"><span data-stu-id="03d1a-512">SkuId</span></span></td>
<td><p><span data-ttu-id="03d1a-513">A ID de uma SKU em particular.</span><span class="sxs-lookup"><span data-stu-id="03d1a-513">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="03d1a-514">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="03d1a-514">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="03d1a-515">A ID de uma Disponibilidade em particular.</span><span class="sxs-lookup"><span data-stu-id="03d1a-515">The ID for a particular Availability.</span></span> <span data-ttu-id="03d1a-516">"Disponibilidade" refere-se a se uma SKU em particular está disponível ou não para compra para determinado país, moeda, segmento do setor etc.</span><span class="sxs-lookup"><span data-stu-id="03d1a-516">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="03d1a-517">Nome SKU</span><span class="sxs-lookup"><span data-stu-id="03d1a-517">SKU Name</span></span></td>
<td><p><span data-ttu-id="03d1a-518">O título de uma SKU em particular.</span><span class="sxs-lookup"><span data-stu-id="03d1a-518">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="03d1a-519">PublisherName</span><span class="sxs-lookup"><span data-stu-id="03d1a-519">PublisherName</span></span></td>
<td><p><span data-ttu-id="03d1a-520">O nome do Editor.</span><span class="sxs-lookup"><span data-stu-id="03d1a-520">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="03d1a-521">PublisherID</span><span class="sxs-lookup"><span data-stu-id="03d1a-521">PublisherID</span></span></td>
<td><p><span data-ttu-id="03d1a-522">A ID do fornecedor, no formato GUID.</span><span class="sxs-lookup"><span data-stu-id="03d1a-522">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="03d1a-523">Não está disponível para a atividade atual.</span><span class="sxs-lookup"><span data-stu-id="03d1a-523">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="03d1a-524">Descrição de assinatura</span><span class="sxs-lookup"><span data-stu-id="03d1a-524">Subscription Description</span></span></td>
<td><p><span data-ttu-id="03d1a-525">O nome da oferta de serviço comprada pelo cliente, conforme definido na tabela de preços.</span><span class="sxs-lookup"><span data-stu-id="03d1a-525">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="03d1a-526">(Este é um campo idêntico ao nome da oferta).</span><span class="sxs-lookup"><span data-stu-id="03d1a-526">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="03d1a-527">ID da assinatura</span><span class="sxs-lookup"><span data-stu-id="03d1a-527">Subscription ID</span></span></td>
<td><p><span data-ttu-id="03d1a-528">Identificador exclusivo de uma assinatura na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="03d1a-528">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="03d1a-529">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="03d1a-529">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="03d1a-530">Esse não é o mesmo que a ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="03d1a-530">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="03d1a-531">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="03d1a-531">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="03d1a-532">Data de início do ciclo de cobrança exceto quando apresentadas as datas de dados de uso latentes anteriormente não cobradas (do ciclo de cobrança anterior).</span><span class="sxs-lookup"><span data-stu-id="03d1a-532">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="03d1a-533">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="03d1a-533">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="03d1a-534">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="03d1a-534">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="03d1a-535">Data de término do ciclo de cobrança exceto quando apresentadas as datas de dados de uso latentes anteriormente não cobradas (do ciclo de cobrança anterior).</span><span class="sxs-lookup"><span data-stu-id="03d1a-535">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="03d1a-536">A hora é sempre o fim do dia, 23:59.</span><span class="sxs-lookup"><span data-stu-id="03d1a-536">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="03d1a-537">Data de uso</span><span class="sxs-lookup"><span data-stu-id="03d1a-537">Usage Date</span></span></td>
<td><p><span data-ttu-id="03d1a-538">Data de uso do serviço.</span><span class="sxs-lookup"><span data-stu-id="03d1a-538">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="03d1a-539">Tipo de medidor</span><span class="sxs-lookup"><span data-stu-id="03d1a-539">Meter Type</span></span></td>
<td><p><span data-ttu-id="03d1a-540">O tipo de medidor.</span><span class="sxs-lookup"><span data-stu-id="03d1a-540">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="03d1a-541">Categoria de medidor</span><span class="sxs-lookup"><span data-stu-id="03d1a-541">Meter Category</span></span></td>
<td><p><span data-ttu-id="03d1a-542">O serviço de nível superior para o uso.</span><span class="sxs-lookup"><span data-stu-id="03d1a-542">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="03d1a-543">Id de medidor</span><span class="sxs-lookup"><span data-stu-id="03d1a-543">Meter Id</span></span></td>
<td><p><span data-ttu-id="03d1a-544">A ID para o medidor que está sendo usada.</span><span class="sxs-lookup"><span data-stu-id="03d1a-544">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="03d1a-545">Medidor subcategoria</span><span class="sxs-lookup"><span data-stu-id="03d1a-545">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="03d1a-546">O tipo de serviço do Azure que pode afetar a taxa.</span><span class="sxs-lookup"><span data-stu-id="03d1a-546">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="03d1a-547">Nome do medidor</span><span class="sxs-lookup"><span data-stu-id="03d1a-547">Meter Name</span></span></td>
<td><p><span data-ttu-id="03d1a-548">A unidade de medida para o medidor que está sendo consumido.</span><span class="sxs-lookup"><span data-stu-id="03d1a-548">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="03d1a-549">Região medidor</span><span class="sxs-lookup"><span data-stu-id="03d1a-549">Meter Region</span></span></td>
<td><p><span data-ttu-id="03d1a-550">Essa coluna identifica a localização de um data center dentro da região para serviços onde isso é aplicável e preenchido.</span><span class="sxs-lookup"><span data-stu-id="03d1a-550">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="03d1a-551">Unidade</span><span class="sxs-lookup"><span data-stu-id="03d1a-551">Unit</span></span></td>
<td><p><span data-ttu-id="03d1a-552">A unidade do nome do recurso.</span><span class="sxs-lookup"><span data-stu-id="03d1a-552">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="03d1a-553">Quantidade consumida</span><span class="sxs-lookup"><span data-stu-id="03d1a-553">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="03d1a-554">A quantidade de serviço consumida (horas, GB etc.) durante o período de relatório.</span><span class="sxs-lookup"><span data-stu-id="03d1a-554">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="03d1a-555">Também inclui qualquer uso não cobrado de períodos de relatório anteriores.</span><span class="sxs-lookup"><span data-stu-id="03d1a-555">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="03d1a-556">Localização do recurso</span><span class="sxs-lookup"><span data-stu-id="03d1a-556">Resource Location</span></span></td>
<td><p><span data-ttu-id="03d1a-557">O datacenter em que o medidor está em execução.</span><span class="sxs-lookup"><span data-stu-id="03d1a-557">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="03d1a-558">Serviço consumido</span><span class="sxs-lookup"><span data-stu-id="03d1a-558">Consumed Service</span></span></td>
<td><p><span data-ttu-id="03d1a-559">O serviço de plataforma Windows Azure que você usou.</span><span class="sxs-lookup"><span data-stu-id="03d1a-559">The Azure platform service that you used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="03d1a-560">Grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="03d1a-560">Resource Group</span></span></td>
<td><p><span data-ttu-id="03d1a-561">O grupo de recursos no qual o medidor implantado está em execução.</span><span class="sxs-lookup"><span data-stu-id="03d1a-561">The resource group in which the deployed meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="03d1a-562">URI do recurso</span><span class="sxs-lookup"><span data-stu-id="03d1a-562">Resource URI</span></span></td>
<td><p><span data-ttu-id="03d1a-563">O URI do recurso que está sendo usado.</span><span class="sxs-lookup"><span data-stu-id="03d1a-563">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="03d1a-564">Tipo de cobrança</span><span class="sxs-lookup"><span data-stu-id="03d1a-564">Charge type</span></span></td>
<td><p><span data-ttu-id="03d1a-565">O tipo de encargo ou ajuste.</span><span class="sxs-lookup"><span data-stu-id="03d1a-565">The type of charge or adjustment.</span></span> <span data-ttu-id="03d1a-566">Não está disponível para a atividade atual.</span><span class="sxs-lookup"><span data-stu-id="03d1a-566">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="03d1a-567">Preço unitário</span><span class="sxs-lookup"><span data-stu-id="03d1a-567">Unit price</span></span></td>
<td><p><span data-ttu-id="03d1a-568">Preço por licença, conforme publicado na lista de preços no momento da compra.</span><span class="sxs-lookup"><span data-stu-id="03d1a-568">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="03d1a-569">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="03d1a-569">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="03d1a-570">Quantidade</span><span class="sxs-lookup"><span data-stu-id="03d1a-570">Quantity</span></span></td>
<td><p><span data-ttu-id="03d1a-571">Número de licenças.</span><span class="sxs-lookup"><span data-stu-id="03d1a-571">Number of licenses.</span></span> <span data-ttu-id="03d1a-572">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="03d1a-572">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="03d1a-573">Tipo de unidade</span><span class="sxs-lookup"><span data-stu-id="03d1a-573">Unit type</span></span></td>
<td><p><span data-ttu-id="03d1a-574">O tipo de unidade o medidor é cobrado.</span><span class="sxs-lookup"><span data-stu-id="03d1a-574">The type of unit the meter is charged in.</span></span> <span data-ttu-id="03d1a-575">Não está disponível para a atividade atual.</span><span class="sxs-lookup"><span data-stu-id="03d1a-575">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="03d1a-576">Cobrança pré imposto</span><span class="sxs-lookup"><span data-stu-id="03d1a-576">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="03d1a-577">Valor total antes dos impostos.</span><span class="sxs-lookup"><span data-stu-id="03d1a-577">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="03d1a-578">Moeda de cobrança</span><span class="sxs-lookup"><span data-stu-id="03d1a-578">Billing currency</span></span></td>
<td><p><span data-ttu-id="03d1a-579">A moeda na região geográfica do cliente</span><span class="sxs-lookup"><span data-stu-id="03d1a-579">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="03d1a-580">Preço total sem imposto</span><span class="sxs-lookup"><span data-stu-id="03d1a-580">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="03d1a-581">Os preços antes dos impostos são adicionados.</span><span class="sxs-lookup"><span data-stu-id="03d1a-581">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="03d1a-582">Moeda de preço</span><span class="sxs-lookup"><span data-stu-id="03d1a-582">Pricing currency</span></span></td>
<td><p><span data-ttu-id="03d1a-583">A moeda na lista de preços.</span><span class="sxs-lookup"><span data-stu-id="03d1a-583">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="03d1a-584">Informações do serviço 1</span><span class="sxs-lookup"><span data-stu-id="03d1a-584">Service Info 1</span></span></td>
<td><p><span data-ttu-id="03d1a-585">O número de conexões ServiceBus que foram provisionados e utilizados em um dia específico.</span><span class="sxs-lookup"><span data-stu-id="03d1a-585">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="03d1a-586">Informações do serviço 2</span><span class="sxs-lookup"><span data-stu-id="03d1a-586">Service Info 2</span></span></td>
<td><p><span data-ttu-id="03d1a-587">Um campo herdado que captura opcional metadados específicos ao serviço.</span><span class="sxs-lookup"><span data-stu-id="03d1a-587">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="03d1a-588">Marcas</span><span class="sxs-lookup"><span data-stu-id="03d1a-588">Tags</span></span></td>
<td><p><span data-ttu-id="03d1a-589">Marcas de que atribuir ao medidor na ordem para agrupar registros de cobrança.</span><span class="sxs-lookup"><span data-stu-id="03d1a-589">Tags you assign to the meter in order to group billing records.</span></span> <span data-ttu-id="03d1a-590">Por exemplo, você pode usar marcas para distribuir custos pelo departamento de que usa o medidor.</span><span class="sxs-lookup"><span data-stu-id="03d1a-590">For example, you can use tags to distribute costs by the department that uses the meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="03d1a-591">Informações adicionais</span><span class="sxs-lookup"><span data-stu-id="03d1a-591">Additional Info</span></span></td>
<td><p><span data-ttu-id="03d1a-592">Informações adicionais não são abordadas em outras colunas.</span><span class="sxs-lookup"><span data-stu-id="03d1a-592">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="03d1a-593">Como mapear encargos entre uma fatura e o arquivo de reconciliação</span><span class="sxs-lookup"><span data-stu-id="03d1a-593">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="03d1a-594">Sua fatura fornece um resumo dos encargos, enquanto seu arquivo de reconciliação fornece uma divisão detalhada das transações de item de linha, incluindo os tipos de carga.</span><span class="sxs-lookup"><span data-stu-id="03d1a-594">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="03d1a-595">Para fazer referência cruzada das quantidades de carga entre o arquivo de reconciliação e fatura, você pode usar opções de filtro do Microsoft Excel para filtrar por tipos de cobrança no arquivo de reconciliação para mapear os encargos de fatura em um conjunto de detalhamentos de cobrança no arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="03d1a-595">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="03d1a-596">Os arquivos de reconciliação, tanto os baseados em licença quanto os baseados em uso, mostram apenas encargos e transações relacionadas ao uso (unidades consumidas e encargos relacionados).</span><span class="sxs-lookup"><span data-stu-id="03d1a-596">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="03d1a-597">Créditos únicos, descontos ou reembolsos que aparecem na fatura como "Ajustes" não são mostrados no arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="03d1a-597">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="03d1a-598">A tabela a seguir mostra os mapeamentos entre uma seção da fatura e os tipos de encargo associados que podem aparecer nos arquivos de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="03d1a-598">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><strong><span data-ttu-id="03d1a-599">Descrição do encargo da fatura</span><span class="sxs-lookup"><span data-stu-id="03d1a-599">Invoice charge description</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="03d1a-600">Descrição do encargo do arquivo de reconciliação (coluna ChargeType)</span><span class="sxs-lookup"><span data-stu-id="03d1a-600">Reconciliation file charge description (ChargeType column)</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="03d1a-601">O que é este encargo?</span><span class="sxs-lookup"><span data-stu-id="03d1a-601">What is this charge?</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="03d1a-602">Como é possível mapear esses tipos de encargo na fatura?</span><span class="sxs-lookup"><span data-stu-id="03d1a-602">How do I map these ChargeTypes to the invoice?</span></span></strong></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><strong><span data-ttu-id="03d1a-603">Encargos baseadas em licença</span><span class="sxs-lookup"><span data-stu-id="03d1a-603">License-based charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="03d1a-604">Taxa de ativação</span><span class="sxs-lookup"><span data-stu-id="03d1a-604">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="03d1a-605">O valor cobrado do cliente quando ele usa a assinatura depois de comprá-la.</span><span class="sxs-lookup"><span data-stu-id="03d1a-605">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="03d1a-606">No arquivo baseado em licença, some a coluna <strong>Quantidade</strong></span><span class="sxs-lookup"><span data-stu-id="03d1a-606">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="03d1a-607">Taxa de cancelamento</span><span class="sxs-lookup"><span data-stu-id="03d1a-607">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="03d1a-608">Os encargos proporcionais reembolsados para o cliente quando os assentos associados são alterados</span><span class="sxs-lookup"><span data-stu-id="03d1a-608">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="03d1a-609">Taxa do ciclo</span><span class="sxs-lookup"><span data-stu-id="03d1a-609">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="03d1a-610">Encargos periódicos de uma assinatura</span><span class="sxs-lookup"><span data-stu-id="03d1a-610">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="03d1a-611">Percorrer ocorrência proporcional</span><span class="sxs-lookup"><span data-stu-id="03d1a-611">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="03d1a-612">Os encargos proporcionais cobrados do cliente quando os assentos associados são alterados</span><span class="sxs-lookup"><span data-stu-id="03d1a-612">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="03d1a-613">Taxas proporcionais durante o cancelamento</span><span class="sxs-lookup"><span data-stu-id="03d1a-613">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="03d1a-614">Reembolso proporcional para a parte não utilizada do serviço após o cancelamento</span><span class="sxs-lookup"><span data-stu-id="03d1a-614">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="03d1a-615">Taxas proporcionais durante a compra</span><span class="sxs-lookup"><span data-stu-id="03d1a-615">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="03d1a-616">O tipo de cobrança de uma assinatura ao usar a cobrança anual</span><span class="sxs-lookup"><span data-stu-id="03d1a-616">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="03d1a-617">Taxa de compra</span><span class="sxs-lookup"><span data-stu-id="03d1a-617">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="03d1a-618">O tipo de cobrança de uma assinatura ao usar a cobrança mensal</span><span class="sxs-lookup"><span data-stu-id="03d1a-618">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="03d1a-619">Taxa proporcional ao renovar</span><span class="sxs-lookup"><span data-stu-id="03d1a-619">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="03d1a-620">Taxas proporcionais após a renovação da assinatura</span><span class="sxs-lookup"><span data-stu-id="03d1a-620">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="03d1a-621">Taxa de renovação</span><span class="sxs-lookup"><span data-stu-id="03d1a-621">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="03d1a-622">Cobrança para renovação de uma assinatura</span><span class="sxs-lookup"><span data-stu-id="03d1a-622">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="03d1a-623">Taxas proporcionais ao ativar</span><span class="sxs-lookup"><span data-stu-id="03d1a-623">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="03d1a-624">Taxas proporcionais da ativação até o final do período de cobrança</span><span class="sxs-lookup"><span data-stu-id="03d1a-624">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong><span data-ttu-id="03d1a-625">Tarifas de uso</span><span class="sxs-lookup"><span data-stu-id="03d1a-625">Usage Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="03d1a-626">Avaliar a taxa de uso ao cancelar</span><span class="sxs-lookup"><span data-stu-id="03d1a-626">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="03d1a-627">Taxa de uso de acesso com o cancelamento para uso não pago durante o período de cobrança atual</span><span class="sxs-lookup"><span data-stu-id="03d1a-627">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="03d1a-628">No arquivo baseado em uso, some a coluna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="03d1a-628">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="03d1a-629">Avalie a taxa de uso para o ciclo atual</span><span class="sxs-lookup"><span data-stu-id="03d1a-629">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="03d1a-630">Taxa de uso de acesso para o período atual de cobrança</span><span class="sxs-lookup"><span data-stu-id="03d1a-630">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="03d1a-631">Créditos</span><span class="sxs-lookup"><span data-stu-id="03d1a-631">Credits</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="03d1a-632">Deslocando um item de linha</span><span class="sxs-lookup"><span data-stu-id="03d1a-632">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="03d1a-633">Reembolso parcial ou integral para um item de linha, incluindo os impostos</span><span class="sxs-lookup"><span data-stu-id="03d1a-633">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="03d1a-634">No arquivo baseado em licença, some a coluna <strong>TotalForCustomer</strong></span><span class="sxs-lookup"><span data-stu-id="03d1a-634">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="03d1a-635">No arquivo baseado em uso, some a coluna <strong>PostTaxTotal</strong></span><span class="sxs-lookup"><span data-stu-id="03d1a-635">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><strong><span data-ttu-id="03d1a-636">Descontos baseados em uso</span><span class="sxs-lookup"><span data-stu-id="03d1a-636">Usage-based discounts</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="03d1a-637">Desconto de ativação</span><span class="sxs-lookup"><span data-stu-id="03d1a-637">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="03d1a-638">Desconto aplicado quando a assinatura é ativada</span><span class="sxs-lookup"><span data-stu-id="03d1a-638">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="03d1a-639">No arquivo baseado em uso, some a coluna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="03d1a-639">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="03d1a-640">Desconto de ciclo</span><span class="sxs-lookup"><span data-stu-id="03d1a-640">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="03d1a-641">Desconto aplicado em cobranças periódicas</span><span class="sxs-lookup"><span data-stu-id="03d1a-641">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="03d1a-642">Desconto de renovação</span><span class="sxs-lookup"><span data-stu-id="03d1a-642">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="03d1a-643">Desconto aplicado quando a assinatura é renovada</span><span class="sxs-lookup"><span data-stu-id="03d1a-643">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="03d1a-644">Desconto de cancelamento</span><span class="sxs-lookup"><span data-stu-id="03d1a-644">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="03d1a-645">Encargos aplicados quando descontos são cancelados</span><span class="sxs-lookup"><span data-stu-id="03d1a-645">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><strong><span data-ttu-id="03d1a-646">Descontos baseados em licença</span><span class="sxs-lookup"><span data-stu-id="03d1a-646">License-based discounts</span></span></strong></p>
</td>
<td>
<p><em><span data-ttu-id="03d1a-647">Podem ser aplicados a vários tipos de cobrança</span><span class="sxs-lookup"><span data-stu-id="03d1a-647">May be applied to multiple charge types</span></span></em></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="03d1a-648">No arquivo baseado em licença, some a coluna <strong>TotalOtherDiscount</strong></span><span class="sxs-lookup"><span data-stu-id="03d1a-648">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="03d1a-649"><strong>Impostos</strong>&nbsp;ou&nbsp;<strong>IVA</strong></span><span class="sxs-lookup"><span data-stu-id="03d1a-649"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><em><span data-ttu-id="03d1a-650">Podem ser aplicados a vários tipos de cobrança</span><span class="sxs-lookup"><span data-stu-id="03d1a-650">May be applied to multiple charge types</span></span></em></p>
<p><em><span data-ttu-id="03d1a-651">Exceção: &quot;deslocamento de um item de linha&quot; já inclui impostos.</span><span class="sxs-lookup"><span data-stu-id="03d1a-651">Exception: &quot;Offset a line item&quot; already includes taxes.</span></span> <span data-ttu-id="03d1a-652">Consulte créditos, acima.</span><span class="sxs-lookup"><span data-stu-id="03d1a-652">See Credits, above.</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="03d1a-653">Impostos ou impostos sobre valor agregado (IVA)</span><span class="sxs-lookup"><span data-stu-id="03d1a-653">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="03d1a-654">No arquivo baseado em licença, some a coluna <strong>Imposto</strong></span><span class="sxs-lookup"><span data-stu-id="03d1a-654">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="03d1a-655">No arquivo baseado em uso, some a coluna <strong>TaxAmount</strong></span><span class="sxs-lookup"><span data-stu-id="03d1a-655">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
