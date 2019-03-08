---
title: Usar os arquivos de reconciliação | Partner Center
ms.topic: article
ms.date: 10/29/2018
description: Para uma exibição detalhada do item de linha de cada carga, em um ciclo de cobrança, baixe os arquivos de reconciliação do Partner Center.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 5ce9b7cd9ead08b7709c68a0e967d64e9f2a32bd
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2019
ms.locfileid: "57585129"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="4f116-103">Usar os arquivos de reconciliação</span><span class="sxs-lookup"><span data-stu-id="4f116-103">Use the reconciliation files</span></span>

<span data-ttu-id="4f116-104">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="4f116-104">**Applies to**</span></span>

-  <span data-ttu-id="4f116-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="4f116-105">Partner Center</span></span>
-  <span data-ttu-id="4f116-106">Partner Center para Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="4f116-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="4f116-107">Para uma exibição detalhada do item de linha de cada carga, em um ciclo de cobrança, baixe os arquivos de reconciliação do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="4f116-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="4f116-108">Os detalhes incluem encargos por assinaturas de cada cliente e eventos detalhados (como a adição de assentos a uma assinatura no meio do período).</span><span class="sxs-lookup"><span data-stu-id="4f116-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="4f116-109">Discriminar pelo parceiro</span><span class="sxs-lookup"><span data-stu-id="4f116-109">Itemize by partner</span></span>


<span data-ttu-id="4f116-110">Os parceiros no modelo indireto podem usar esses campos adicionais nos arquivos de reconciliação baseados em uso e em licença para discriminar por revendedor.</span><span class="sxs-lookup"><span data-stu-id="4f116-110">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="4f116-111">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="4f116-111">MPN ID</span></span></th>
<th><span data-ttu-id="4f116-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f116-112">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="4f116-113">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="4f116-113">MPN ID</span></span></td>
<td><p><span data-ttu-id="4f116-114">A ID do Microsoft Partner Network (MPN) do parceiro CSP (direta ou indireta).</span><span class="sxs-lookup"><span data-stu-id="4f116-114">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4f116-115">ID do MPN do revendedor</span><span class="sxs-lookup"><span data-stu-id="4f116-115">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="4f116-116">Só aparece em arquivos de reconciliação para parceiros no modelo indireto.</span><span class="sxs-lookup"><span data-stu-id="4f116-116">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="4f116-117">A ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="4f116-117">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="4f116-118">Isso corresponde à ID de revendedor listada para a assinatura específica no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="4f116-118">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="4f116-119">modo de exibição eTo ou atualização revendedor, no menu do Partner Center, selecione <strong>clientes</strong>, em seguida, escolha o cliente da lista.</span><span class="sxs-lookup"><span data-stu-id="4f116-119">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="4f116-120">No menu do cliente, selecione <strong>Assinaturas</strong>, escolha a assinatura na lista.</span><span class="sxs-lookup"><span data-stu-id="4f116-120">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="4f116-121">Selecione <strong>Atualizar</strong> para alterar o <strong>Revendedor (ID do MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="4f116-121">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="4f116-122">Se um parceiro CSP vendeu a assinatura diretamente para o cliente, sua ID do MPN estará listada duas vezes, como a ID do MPN e a ID do MPN do revendedor.</span><span class="sxs-lookup"><span data-stu-id="4f116-122">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="4f116-123">Se um parceiro CSP tiver um revendedor sem ID do MPN, esse valor será definido como a ID do MPN do parceiro.</span><span class="sxs-lookup"><span data-stu-id="4f116-123">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="4f116-124">Se o parceiro CSP remover uma ID de revendedor, esse valor será definido como -1.</span><span class="sxs-lookup"><span data-stu-id="4f116-124">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="4f116-125">Campos de arquivo de licença</span><span class="sxs-lookup"><span data-stu-id="4f116-125">License-based file fields</span></span>


<span data-ttu-id="4f116-126">Para reconciliar seus encargos com os pedidos de seu cliente, compare o campo Syndication\_Partner\_Subscription\_Number do arquivo de reconciliação com a ID de Assinatura do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="4f116-126">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="4f116-127"><strong>Coluna</strong></span><span class="sxs-lookup"><span data-stu-id="4f116-127"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="4f116-128"><strong>Descrição</strong></span><span class="sxs-lookup"><span data-stu-id="4f116-128"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="4f116-129"><strong>Valor de exemplo</strong></span><span class="sxs-lookup"><span data-stu-id="4f116-129"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4f116-130">PartnerID</span><span class="sxs-lookup"><span data-stu-id="4f116-130">PartnerId</span></span></td>
<td><p><span data-ttu-id="4f116-131">Identificador exclusivo de uma entidade de cobrança específica, em formato GUID.</span><span class="sxs-lookup"><span data-stu-id="4f116-131">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="4f116-132">Não é necessário para reconciliação, mas pode ser uma informação útil.</span><span class="sxs-lookup"><span data-stu-id="4f116-132">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="4f116-133">O mesmo em todas as linhas.</span><span class="sxs-lookup"><span data-stu-id="4f116-133">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="4f116-134">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="4f116-134">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4f116-135">CustomerID</span><span class="sxs-lookup"><span data-stu-id="4f116-135">CustomerID</span></span></td>
<td><p><span data-ttu-id="4f116-136">ID exclusiva da Microsoft, no formato GUID, usada para identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="4f116-136">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="4f116-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="4f116-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4f116-138">OrderID</span><span class="sxs-lookup"><span data-stu-id="4f116-138">OrderID</span></span></td>
<td><p><span data-ttu-id="4f116-139">Identificador exclusivo para um pedido na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="4f116-139">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="4f116-140">Pode ser útil para identificar o pedido ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="4f116-140">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="4f116-141">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="4f116-141">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4f116-142">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="4f116-142">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="4f116-143">Identificador exclusivo de uma assinatura na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="4f116-143">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="4f116-144">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="4f116-144">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="4f116-145">Esse não é o mesmo que o ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="4f116-145">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="4f116-146">Consulte Número_Assinatura_Parceiro_Sindicalização.</span><span class="sxs-lookup"><span data-stu-id="4f116-146">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="4f116-147">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="4f116-147">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4f116-148">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="4f116-148">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="4f116-149">Identificador exclusivo para assinaturas.</span><span class="sxs-lookup"><span data-stu-id="4f116-149">Unique identifier for subscriptions.</span></span> <span data-ttu-id="4f116-150">Target: Um cliente pode ter várias assinaturas para o mesmo plano, portanto, isso é importante para análise de arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="4f116-150">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="4f116-151">Esse campo é mapeado para a ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="4f116-151">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="4f116-152">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="4f116-152">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4f116-153">OfferID</span><span class="sxs-lookup"><span data-stu-id="4f116-153">OfferID</span></span></td>
<td><p><span data-ttu-id="4f116-154">ID exclusivo da oferta.</span><span class="sxs-lookup"><span data-stu-id="4f116-154">Unique offer ID.</span></span> <span data-ttu-id="4f116-155">ID padrão da oferta de acordo com a lista de preços.</span><span class="sxs-lookup"><span data-stu-id="4f116-155">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="4f116-156"><b>Observação</b>: Esse valor não corresponde a ID da oferta da lista de preços.</span><span class="sxs-lookup"><span data-stu-id="4f116-156"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="4f116-157">Veja DurableOfferID abaixo.</span><span class="sxs-lookup"><span data-stu-id="4f116-157">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="4f116-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="4f116-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4f116-159">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="4f116-159">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="4f116-160">ID exclusivo da oferta durável, conforme definido na tabela de preços.</span><span class="sxs-lookup"><span data-stu-id="4f116-160">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="4f116-161"><b>Observação</b>: Esse valor corresponde à ID da oferta da lista de preços.</span><span class="sxs-lookup"><span data-stu-id="4f116-161"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="4f116-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="4f116-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4f116-163">OfferName</span><span class="sxs-lookup"><span data-stu-id="4f116-163">OfferName</span></span></td>
<td><p><span data-ttu-id="4f116-164">O nome da oferta de serviço comprada pelo cliente, conforme definido na tabela de preços.</span><span class="sxs-lookup"><span data-stu-id="4f116-164">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="4f116-165">Microsoft Office 365 (plano E3)</span><span class="sxs-lookup"><span data-stu-id="4f116-165">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4f116-166">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="4f116-166">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="4f116-167">A data de início da assinatura, definida como um dia após o pedido ser enviado.</span><span class="sxs-lookup"><span data-stu-id="4f116-167">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="4f116-168">Verificando a data de início da assinatura em conjunto com a data de término, você pode determinar se o cliente está dentro do primeiro ano da assinatura ou se a assinatura foi renovada para o ano seguinte.</span><span class="sxs-lookup"><span data-stu-id="4f116-168">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="4f116-169">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="4f116-169">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="4f116-170">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="4f116-170">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4f116-171">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="4f116-171">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="4f116-172">A data de término da assinatura: + x dias após a data de início (para alinhar com data de cobrança do parceiro) ou 12 meses a partir da data de renovação de 12 meses.</span><span class="sxs-lookup"><span data-stu-id="4f116-172">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="4f116-173">Na renovação, os preços são atualizados com a tabela de preços atual.</span><span class="sxs-lookup"><span data-stu-id="4f116-173">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="4f116-174">Um comunicado ao cliente pode ser necessário antes da renovação automática.</span><span class="sxs-lookup"><span data-stu-id="4f116-174">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="4f116-175">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="4f116-175">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="4f116-176">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="4f116-176">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4f116-177">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="4f116-177">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="4f116-178">Dia de início dos encargos.</span><span class="sxs-lookup"><span data-stu-id="4f116-178">Start day of the charges.</span></span></p>
<p><span data-ttu-id="4f116-179">Quando o cliente muda o número de assentos, esse número é usado para calcular os encargos por dia (pro-rata).</span><span class="sxs-lookup"><span data-stu-id="4f116-179">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="4f116-180">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="4f116-180">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="4f116-181">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="4f116-181">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4f116-182">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="4f116-182">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="4f116-183">Dia do término dos encargos.</span><span class="sxs-lookup"><span data-stu-id="4f116-183">End day of the charges.</span></span></p>
<p><span data-ttu-id="4f116-184">Quando o cliente muda o número de assentos, esse número é usado para calcular os encargos por dia (pro-rata).</span><span class="sxs-lookup"><span data-stu-id="4f116-184">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="4f116-185">A hora é sempre o fim do dia, 23:59.</span><span class="sxs-lookup"><span data-stu-id="4f116-185">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="4f116-186">28/2/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="4f116-186">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4f116-187">ChargeType</span><span class="sxs-lookup"><span data-stu-id="4f116-187">ChargeType</span></span></td>
<td><p><span data-ttu-id="4f116-188">O tipo de encargo ou ajuste.</span><span class="sxs-lookup"><span data-stu-id="4f116-188">The type of charge or adjustment.</span></span> <span data-ttu-id="4f116-189">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="4f116-189">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="4f116-190">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="4f116-190">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4f116-191">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="4f116-191">UnitPrice</span></span></td>
<td><p><span data-ttu-id="4f116-192">Preço por estação, conforme publicado na lista de preços no momento da compra.</span><span class="sxs-lookup"><span data-stu-id="4f116-192">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="4f116-193">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="4f116-193">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="4f116-194">6.82</span><span class="sxs-lookup"><span data-stu-id="4f116-194">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4f116-195">Quantidade</span><span class="sxs-lookup"><span data-stu-id="4f116-195">Quantity</span></span></td>
<td><p><span data-ttu-id="4f116-196">Número de assentos.</span><span class="sxs-lookup"><span data-stu-id="4f116-196">Number of seats.</span></span> <span data-ttu-id="4f116-197">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="4f116-197">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="4f116-198">2</span><span class="sxs-lookup"><span data-stu-id="4f116-198">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4f116-199">Valor</span><span class="sxs-lookup"><span data-stu-id="4f116-199">Amount</span></span></td>
<td><p><span data-ttu-id="4f116-200">Preço total por quantidade.</span><span class="sxs-lookup"><span data-stu-id="4f116-200">Total of price for quantity.</span></span> <span data-ttu-id="4f116-201">Útil para verificar se o cálculo do valor coincide com a forma como você calcula isso para seus clientes.</span><span class="sxs-lookup"><span data-stu-id="4f116-201">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="4f116-202">13.32</span><span class="sxs-lookup"><span data-stu-id="4f116-202">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4f116-203">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="4f116-203">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="4f116-204">Valor de desconto aplicado a esses encargos.</span><span class="sxs-lookup"><span data-stu-id="4f116-204">Amount of discount applied to these charges.</span></span> <span data-ttu-id="4f116-205">IUR ou novas assinaturas qualificadas para incentivo também conterão um valor de desconto nessa coluna.</span><span class="sxs-lookup"><span data-stu-id="4f116-205">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="4f116-206">2.32</span><span class="sxs-lookup"><span data-stu-id="4f116-206">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4f116-207">Subtotal</span><span class="sxs-lookup"><span data-stu-id="4f116-207">Subtotal</span></span></td>
<td><p><span data-ttu-id="4f116-208">Total sem imposto.</span><span class="sxs-lookup"><span data-stu-id="4f116-208">Total before tax.</span></span> <span data-ttu-id="4f116-209">Verifica se seu subtotal corresponde ao total esperado, em caso de desconto.</span><span class="sxs-lookup"><span data-stu-id="4f116-209">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="4f116-210">11</span><span class="sxs-lookup"><span data-stu-id="4f116-210">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4f116-211">Tax</span><span class="sxs-lookup"><span data-stu-id="4f116-211">Tax</span></span></td>
<td><p><span data-ttu-id="4f116-212">Encargo de valor, com base em seu mercado de imposto&#39;regras de imposto de s e as circunstâncias específicas.</span><span class="sxs-lookup"><span data-stu-id="4f116-212">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="4f116-213">0</span><span class="sxs-lookup"><span data-stu-id="4f116-213">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4f116-214">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="4f116-214">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="4f116-215">Total com imposto.</span><span class="sxs-lookup"><span data-stu-id="4f116-215">Total after tax.</span></span> <span data-ttu-id="4f116-216">Verifica se o imposto é cobrado na fatura.</span><span class="sxs-lookup"><span data-stu-id="4f116-216">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="4f116-217">11</span><span class="sxs-lookup"><span data-stu-id="4f116-217">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4f116-218">Currency</span><span class="sxs-lookup"><span data-stu-id="4f116-218">Currency</span></span></td>
<td><p><span data-ttu-id="4f116-219">Tipo de moeda.</span><span class="sxs-lookup"><span data-stu-id="4f116-219">Currency type.</span></span> <span data-ttu-id="4f116-220">Cada entidade de cobrança tem somente uma moeda.</span><span class="sxs-lookup"><span data-stu-id="4f116-220">Each billing entity has only one currency.</span></span> <span data-ttu-id="4f116-221">Verifique se isso coincide com a primeira fatura e faça o mesmo após grandes atualizações na plataforma de cobrança.</span><span class="sxs-lookup"><span data-stu-id="4f116-221">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="4f116-222">EUR</span><span class="sxs-lookup"><span data-stu-id="4f116-222">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4f116-223">CustomerName</span><span class="sxs-lookup"><span data-stu-id="4f116-223">CustomerName</span></span></td>
<td><p><span data-ttu-id="4f116-224">Cliente&#39;nome da organização s conforme relatado no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="4f116-224">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="4f116-225">Isso é muito importante para reconciliar a fatura com as informações de seu sistema.</span><span class="sxs-lookup"><span data-stu-id="4f116-225">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="4f116-226">Cliente de teste A</span><span class="sxs-lookup"><span data-stu-id="4f116-226">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4f116-227">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="4f116-227">MPNID</span></span></td>
<td><p><span data-ttu-id="4f116-228">ID do MPN do parceiro CSP</span><span class="sxs-lookup"><span data-stu-id="4f116-228">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="4f116-229">4390934</span><span class="sxs-lookup"><span data-stu-id="4f116-229">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4f116-230">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="4f116-230">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="4f116-231">ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="4f116-231">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="4f116-232">Consulte <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Discriminar por parceiro</a>.</span><span class="sxs-lookup"><span data-stu-id="4f116-232">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="4f116-233">4390934</span><span class="sxs-lookup"><span data-stu-id="4f116-233">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4f116-234">DomainName</span><span class="sxs-lookup"><span data-stu-id="4f116-234">DomainName</span></span></td>
<td><p><span data-ttu-id="4f116-235">Cliente&#39;nome de domínio s, usado para ajudar a identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="4f116-235">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="4f116-236">Isso não deve ser usado para identificar exclusivamente o cliente, assim como o cliente/parceiro pode atualizar o domínio intuitivo/padrão por meio do portal do O365.</span><span class="sxs-lookup"><span data-stu-id="4f116-236">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="4f116-237">Este campo pode aparecer em branco até o segundo ciclo de cobrança.</span><span class="sxs-lookup"><span data-stu-id="4f116-237">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="4f116-238">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="4f116-238">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4f116-239">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="4f116-239">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="4f116-240">Apelido da Inscrição.</span><span class="sxs-lookup"><span data-stu-id="4f116-240">Subscription nickname.</span></span> <span data-ttu-id="4f116-241">Se nenhum apelido for especificado, o Partner Center usa o OfferName.</span><span class="sxs-lookup"><span data-stu-id="4f116-241">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="4f116-242">PROJETO ONLINE</span><span class="sxs-lookup"><span data-stu-id="4f116-242">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4f116-243">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="4f116-243">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="4f116-244">O nome da oferta de serviço comprada pelo cliente, conforme definido na tabela de preços.</span><span class="sxs-lookup"><span data-stu-id="4f116-244">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="4f116-245">(Este é um campo idêntico ao nome da oferta).</span><span class="sxs-lookup"><span data-stu-id="4f116-245">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="4f116-246">PROJETO ONLINE PREMIUM SEM PROJETO CLIENTE</span><span class="sxs-lookup"><span data-stu-id="4f116-246">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="4f116-247">Campos de arquivo baseada em uso</span><span class="sxs-lookup"><span data-stu-id="4f116-247">Usage-based file fields</span></span>


<span data-ttu-id="4f116-248">Para reconciliar seus encargos com o uso de seu cliente, compare ResellerID/ResellerName/ResellerBillableAccount do arquivo de reconciliação com o nome do cliente e a ID da assinatura do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="4f116-248">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="4f116-249">Os campos a seguir explicam quais serviços foram usados e a taxa.</span><span class="sxs-lookup"><span data-stu-id="4f116-249">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="4f116-250"><strong>Coluna</strong></span><span class="sxs-lookup"><span data-stu-id="4f116-250"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="4f116-251"><strong>Descrição</strong></span><span class="sxs-lookup"><span data-stu-id="4f116-251"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="4f116-252"><strong>Valor de exemplo</strong></span><span class="sxs-lookup"><span data-stu-id="4f116-252"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4f116-253">PartnerID</span><span class="sxs-lookup"><span data-stu-id="4f116-253">PartnerID</span></span></td>
<td><p><span data-ttu-id="4f116-254">ID do parceiro, no formato GUID.</span><span class="sxs-lookup"><span data-stu-id="4f116-254">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="4f116-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="4f116-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4f116-256">PartnerName</span><span class="sxs-lookup"><span data-stu-id="4f116-256">PartnerName</span></span></td>
<td><p><span data-ttu-id="4f116-257">Nome do parceiro.</span><span class="sxs-lookup"><span data-stu-id="4f116-257">Partner Name.</span></span></p></td>
<td><span data-ttu-id="4f116-258">Acme incorporado</span><span class="sxs-lookup"><span data-stu-id="4f116-258">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4f116-259">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="4f116-259">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="4f116-260">ID da conta do parceiro.</span><span class="sxs-lookup"><span data-stu-id="4f116-260">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="4f116-261">1010578050</span><span class="sxs-lookup"><span data-stu-id="4f116-261">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4f116-262">CustomerName</span><span class="sxs-lookup"><span data-stu-id="4f116-262">CustomerName</span></span></td>
<td><p><span data-ttu-id="4f116-263">Cliente&#39;nome da organização s conforme relatado no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="4f116-263">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="4f116-264">Isso é muito importante para reconciliar a fatura com as informações de seu sistema.</span><span class="sxs-lookup"><span data-stu-id="4f116-264">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="4f116-265">Cliente de teste A</span><span class="sxs-lookup"><span data-stu-id="4f116-265">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4f116-266">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="4f116-266">MPNID</span></span></td>
<td><p><span data-ttu-id="4f116-267">ID do MPN do parceiro CSP.</span><span class="sxs-lookup"><span data-stu-id="4f116-267">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="4f116-268">4390934</span><span class="sxs-lookup"><span data-stu-id="4f116-268">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4f116-269">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="4f116-269">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="4f116-270">ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="4f116-270">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="4f116-271">Consulte <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Discriminar por parceiro</a>.</span><span class="sxs-lookup"><span data-stu-id="4f116-271">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="4f116-272">4390934</span><span class="sxs-lookup"><span data-stu-id="4f116-272">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4f116-273">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="4f116-273">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="4f116-274">Número da fatura na qual a transação especificada é exibida.</span><span class="sxs-lookup"><span data-stu-id="4f116-274">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="4f116-275">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="4f116-275">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4f116-276">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="4f116-276">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="4f116-277">Data de início do ciclo de cobrança exceto quando apresentadas as datas de dados de uso latentes anteriormente não cobradas (do ciclo de cobrança anterior).</span><span class="sxs-lookup"><span data-stu-id="4f116-277">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="4f116-278">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="4f116-278">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="4f116-279">1/2/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="4f116-279">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4f116-280">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="4f116-280">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="4f116-281">Data de término do ciclo de cobrança exceto quando apresentadas as datas de dados de uso latentes anteriormente não cobradas (do ciclo de cobrança anterior).</span><span class="sxs-lookup"><span data-stu-id="4f116-281">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="4f116-282">A hora é sempre o fim do dia, 23:59.</span><span class="sxs-lookup"><span data-stu-id="4f116-282">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="4f116-283">28/2/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="4f116-283">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4f116-284">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="4f116-284">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="4f116-285">Identificador exclusivo de uma assinatura na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="4f116-285">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="4f116-286">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="4f116-286">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="4f116-287">Esse não é o mesmo que o ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="4f116-287">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="4f116-288">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="4f116-288">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4f116-289">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="4f116-289">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="4f116-290">Apelido da oferta do serviço.</span><span class="sxs-lookup"><span data-stu-id="4f116-290">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="4f116-291">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="4f116-291">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4f116-292">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="4f116-292">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="4f116-293">Linha de negócios da oferta do serviço</span><span class="sxs-lookup"><span data-stu-id="4f116-293">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="4f116-294">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="4f116-294">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4f116-295">OrderID</span><span class="sxs-lookup"><span data-stu-id="4f116-295">OrderID</span></span></td>
<td><p><span data-ttu-id="4f116-296">Identificador exclusivo para um pedido na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="4f116-296">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="4f116-297">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="4f116-297">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="4f116-298">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="4f116-298">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4f116-299">ServiceName</span><span class="sxs-lookup"><span data-stu-id="4f116-299">ServiceName</span></span></td>
<td><p><span data-ttu-id="4f116-300">O nome do serviço do Azure em questão.</span><span class="sxs-lookup"><span data-stu-id="4f116-300">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="4f116-301">MÁQUINAS VIRTUAIS</span><span class="sxs-lookup"><span data-stu-id="4f116-301">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4f116-302">ServiceType</span><span class="sxs-lookup"><span data-stu-id="4f116-302">ServiceType</span></span></td>
<td><p><span data-ttu-id="4f116-303">O tipo específico de serviço do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="4f116-303">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="4f116-304">Service Bus – Individual ou pacote</span><span class="sxs-lookup"><span data-stu-id="4f116-304">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="4f116-305">Banco de dados SQL Azure – Edição empresa ou Web</span><span class="sxs-lookup"><span data-stu-id="4f116-305">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4f116-306">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="4f116-306">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="4f116-307">Identificador exclusivo específico de toda a estrutura de serviço de dados e preço.</span><span class="sxs-lookup"><span data-stu-id="4f116-307">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="4f116-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="4f116-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4f116-309">Nome do recurso</span><span class="sxs-lookup"><span data-stu-id="4f116-309">Resource Name</span></span></td>
<td><p><span data-ttu-id="4f116-310">O nome do recurso do Azure.</span><span class="sxs-lookup"><span data-stu-id="4f116-310">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="4f116-311">Dados de entrada transferidos (GB)</span><span class="sxs-lookup"><span data-stu-id="4f116-311">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="4f116-312">Dados de saída transferidos (GB)</span><span class="sxs-lookup"><span data-stu-id="4f116-312">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4f116-313">Region</span><span class="sxs-lookup"><span data-stu-id="4f116-313">Region</span></span></td>
<td><p><span data-ttu-id="4f116-314">A região a qual o uso se aplica.</span><span class="sxs-lookup"><span data-stu-id="4f116-314">The region the usage applies to.</span></span> <span data-ttu-id="4f116-315">Usado principalmente para atribuir as taxas de transferências de dados, já que as taxas variam de acordo com a região.</span><span class="sxs-lookup"><span data-stu-id="4f116-315">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="4f116-316">Pacífico Asiático, Europa, América Latina e América do Norte</span><span class="sxs-lookup"><span data-stu-id="4f116-316">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4f116-317">SKU</span><span class="sxs-lookup"><span data-stu-id="4f116-317">SKU</span></span></td>
<td><p><span data-ttu-id="4f116-318">Identificador exclusivo MSFT da oferta</span><span class="sxs-lookup"><span data-stu-id="4f116-318">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="4f116-319">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="4f116-319">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="4f116-320">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="4f116-320">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="4f116-321">Uma ID e a quantidade para discriminar as taxas diferentes de um serviço ou recurso em um determinado período de cobrança.</span><span class="sxs-lookup"><span data-stu-id="4f116-321">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="4f116-322">Para a classificação em camadas do Azure, pode haver uma taxa para uma determinada quantidade de unidades faturáveis e uma taxa diferente depois disso.</span><span class="sxs-lookup"><span data-stu-id="4f116-322">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="4f116-323">1</span><span class="sxs-lookup"><span data-stu-id="4f116-323">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4f116-324">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="4f116-324">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="4f116-325">A quantidade de serviço consumida (horas, GB etc.) durante o período de relatório.</span><span class="sxs-lookup"><span data-stu-id="4f116-325">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="4f116-326">Também inclui qualquer uso não cobrado de períodos de relatório anteriores.</span><span class="sxs-lookup"><span data-stu-id="4f116-326">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="4f116-327">11</span><span class="sxs-lookup"><span data-stu-id="4f116-327">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4f116-328">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="4f116-328">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="4f116-329">Unidades incluídas como parte da oferta.</span><span class="sxs-lookup"><span data-stu-id="4f116-329">Units included as part of the offer.</span></span> <span data-ttu-id="4f116-330">Normalmente não está presente no CSP.</span><span class="sxs-lookup"><span data-stu-id="4f116-330">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="4f116-331">0</span><span class="sxs-lookup"><span data-stu-id="4f116-331">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="4f116-332">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="4f116-332">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="4f116-333">Unidades não incluídas como parte da oferta devem ser pagas pelo parceiro.</span><span class="sxs-lookup"><span data-stu-id="4f116-333">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="4f116-334">Igual a ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="4f116-334">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="4f116-335">11</span><span class="sxs-lookup"><span data-stu-id="4f116-335">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4f116-336">ListPrice</span><span class="sxs-lookup"><span data-stu-id="4f116-336">ListPrice</span></span></td>
<td><p><span data-ttu-id="4f116-337">Preço da oferta em vigor na data de início da assinatura.</span><span class="sxs-lookup"><span data-stu-id="4f116-337">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="4f116-338">U$ 0,0808</span><span class="sxs-lookup"><span data-stu-id="4f116-338">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4f116-339">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="4f116-339">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="4f116-340">ListPrist vezes OverageQuantity, arredondado para o centavo mais próximo.</span><span class="sxs-lookup"><span data-stu-id="4f116-340">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="4f116-341">U$ 0,085</span><span class="sxs-lookup"><span data-stu-id="4f116-341">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4f116-342">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="4f116-342">TaxAmount</span></span></td>
<td><p><span data-ttu-id="4f116-343">Encargo de valor, com base em seu mercado de imposto&#39;regras de imposto de s e as circunstâncias específicas.</span><span class="sxs-lookup"><span data-stu-id="4f116-343">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="4f116-344">U$ 0,08</span><span class="sxs-lookup"><span data-stu-id="4f116-344">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4f116-345">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="4f116-345">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="4f116-346">Total após imposto, quando o imposto é aplicável.</span><span class="sxs-lookup"><span data-stu-id="4f116-346">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="4f116-347">U$ 0,93</span><span class="sxs-lookup"><span data-stu-id="4f116-347">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4f116-348">Currency</span><span class="sxs-lookup"><span data-stu-id="4f116-348">Currency</span></span></td>
<td><p><span data-ttu-id="4f116-349">Tipo de moeda.</span><span class="sxs-lookup"><span data-stu-id="4f116-349">Currency type.</span></span> <span data-ttu-id="4f116-350">Cada entidade de cobrança tem somente uma moeda.</span><span class="sxs-lookup"><span data-stu-id="4f116-350">Each billing entity has only one currency.</span></span> <span data-ttu-id="4f116-351">Verifique se isso coincide com a primeira fatura e faça o mesmo após grandes atualizações na plataforma de cobrança.</span><span class="sxs-lookup"><span data-stu-id="4f116-351">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="4f116-352">EUR</span><span class="sxs-lookup"><span data-stu-id="4f116-352">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4f116-353">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="4f116-353">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="4f116-354">Preço por unidade sem imposto.</span><span class="sxs-lookup"><span data-stu-id="4f116-354">Pretax price per unit.</span></span> <span data-ttu-id="4f116-355">Igual a PretaxCharges / OverageQuantity, arredondado para o centavo mais próximo.</span><span class="sxs-lookup"><span data-stu-id="4f116-355">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="4f116-356">U$ 0,08</span><span class="sxs-lookup"><span data-stu-id="4f116-356">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4f116-357">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="4f116-357">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="4f116-358">Preço pós-imposto por unidade.</span><span class="sxs-lookup"><span data-stu-id="4f116-358">Post tax price per unit.</span></span> <span data-ttu-id="4f116-359">Igual a PostTaxTotal / OverageQuantity, ou PretaxEffectiveRate + taxa de imposto por valor de unidade, arredondado para o centavo mais próximo.</span><span class="sxs-lookup"><span data-stu-id="4f116-359">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="4f116-360">U$ 0,08</span><span class="sxs-lookup"><span data-stu-id="4f116-360">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4f116-361">ChargeType</span><span class="sxs-lookup"><span data-stu-id="4f116-361">ChargeType</span></span></td>
<td><p><span data-ttu-id="4f116-362">O tipo de encargo ou ajuste.</span><span class="sxs-lookup"><span data-stu-id="4f116-362">The type of charge or adjustment.</span></span> <span data-ttu-id="4f116-363">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="4f116-363">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="4f116-364">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="4f116-364">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4f116-365">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="4f116-365">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="4f116-366">ID exclusiva da conta na plataforma de cobrança da MSFT.</span><span class="sxs-lookup"><span data-stu-id="4f116-366">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="4f116-367">1280018095</span><span class="sxs-lookup"><span data-stu-id="4f116-367">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4f116-368">UsageDate</span><span class="sxs-lookup"><span data-stu-id="4f116-368">UsageDate</span></span></td>
<td><p><span data-ttu-id="4f116-369">Data da implantação do serviço.</span><span class="sxs-lookup"><span data-stu-id="4f116-369">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="4f116-370">1/2/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="4f116-370">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4f116-371">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="4f116-371">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="4f116-372">Essa coluna identifica a localização de um data center dentro da região para serviços onde isso é aplicável e preenchido.</span><span class="sxs-lookup"><span data-stu-id="4f116-372">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="4f116-373">Leste da Ásia, Sudeste da Ásia, Norte da Europa, Europa Ocidental, Centro Norte e Centro Sul dos EUA</span><span class="sxs-lookup"><span data-stu-id="4f116-373">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4f116-374">MeteredService</span><span class="sxs-lookup"><span data-stu-id="4f116-374">MeteredService</span></span></td>
<td><p><span data-ttu-id="4f116-375">Essa coluna é utilizada para rastrear o serviço do Microsoft Azure individual que não pode ser identificado especificamente na coluna Nome do Serviço.</span><span class="sxs-lookup"><span data-stu-id="4f116-375">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="4f116-376">Por exemplo, transferências de dados são relatadas como &quot;Microsoft Azure – Todos os Serviços&quot; na coluna Nome do Serviço.</span><span class="sxs-lookup"><span data-stu-id="4f116-376">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="4f116-377">Essa coluna MeteredService indicará ao qual serviço específico o uso pertence.</span><span class="sxs-lookup"><span data-stu-id="4f116-377">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="4f116-378">AccessControl, CDN, Computação, Banco de dados, ServiceBus, Armazenamento</span><span class="sxs-lookup"><span data-stu-id="4f116-378">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4f116-379">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="4f116-379">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="4f116-380">Um subcabeçalho que esclarece ainda mais o serviço Microsoft Azure individual além do nível fornecido pelo campo MeteredService.</span><span class="sxs-lookup"><span data-stu-id="4f116-380">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="4f116-381">EXTERNO</span><span class="sxs-lookup"><span data-stu-id="4f116-381">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4f116-382">Projeto</span><span class="sxs-lookup"><span data-stu-id="4f116-382">Project</span></span></td>
<td><p><span data-ttu-id="4f116-383">Nome definido pelo cliente para a instância do serviço</span><span class="sxs-lookup"><span data-stu-id="4f116-383">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="4f116-384">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="4f116-384">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4f116-385">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="4f116-385">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="4f116-386">O número de conexões ServiceBus que foram provisionados e utilizados em um dia específico.</span><span class="sxs-lookup"><span data-stu-id="4f116-386">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="4f116-387">Por exemplo: se você tivesse uma conexão individualmente provisionada durante um mês de 30 dias, a coluna Informação do Serviço 1 lerá "1,000000 conexões/30 dias".</span><span class="sxs-lookup"><span data-stu-id="4f116-387">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="4f116-388">Se você tivesse um pacote de 25 de conexões de barramento de serviço provisionado e você tinha utilizou 1 durante o dia, sua instrução de uso diário para esse dia indicaria "25 conexões / 30 dias – usado: 1.000000”.</span><span class="sxs-lookup"><span data-stu-id="4f116-388">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4f116-389">CustomerID</span><span class="sxs-lookup"><span data-stu-id="4f116-389">CustomerID</span></span></td>
<td><p><span data-ttu-id="4f116-390">ID exclusiva da Microsoft, no formato GUID, usada para identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="4f116-390">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="4f116-391">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="4f116-391">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4f116-392">DomainName</span><span class="sxs-lookup"><span data-stu-id="4f116-392">DomainName</span></span></td>
<td><p><span data-ttu-id="4f116-393">Cliente&#39;nome de domínio s, usado para ajudar a identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="4f116-393">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="4f116-394">Este campo pode aparecer em branco até o segundo ciclo de cobrança.</span><span class="sxs-lookup"><span data-stu-id="4f116-394">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="4f116-395">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="4f116-395">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="4f116-396">Unidade</span><span class="sxs-lookup"><span data-stu-id="4f116-396">Unit</span></span></td>
<td><p><span data-ttu-id="4f116-397">A unidade do nome do recurso</span><span class="sxs-lookup"><span data-stu-id="4f116-397">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="4f116-398">GB ou HORAS</span><span class="sxs-lookup"><span data-stu-id="4f116-398">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="4f116-399">Campos de arquivo únicos e recorrentes</span><span class="sxs-lookup"><span data-stu-id="4f116-399">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="4f116-400">Column</span><span class="sxs-lookup"><span data-stu-id="4f116-400">Column</span></span></th>
<th><span data-ttu-id="4f116-401">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f116-401">Description</span></span></th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td><span data-ttu-id="4f116-402">PartnerID</span><span class="sxs-lookup"><span data-stu-id="4f116-402">PartnerId</span></span></td>
<td><p><span data-ttu-id="4f116-403">Identificador exclusivo do locatário Microsoft Azure Active Directory para uma entidade específica de cobrança, no formato GUID.</span><span class="sxs-lookup"><span data-stu-id="4f116-403">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="4f116-404">Não é necessário para reconciliação, mas pode ser uma informação útil.</span><span class="sxs-lookup"><span data-stu-id="4f116-404">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="4f116-405">O mesmo em todas as linhas.</span><span class="sxs-lookup"><span data-stu-id="4f116-405">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4f116-406">Id do cliente</span><span class="sxs-lookup"><span data-stu-id="4f116-406">Customer Id</span></span></td>
<td><p><span data-ttu-id="4f116-407">Microsoft Azure Active Directory locatário ID exclusiva, no formato GUID, usado para identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="4f116-407">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4f116-408">Nome do cliente</span><span class="sxs-lookup"><span data-stu-id="4f116-408">Customer Name</span></span></td>
<td><p><span data-ttu-id="4f116-409">Nome da organização do cliente como informado no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="4f116-409">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4f116-410">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="4f116-410">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="4f116-411">Nome de domínio do cliente, usado para ajudar a identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="4f116-411">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="4f116-412">Isso não deve ser usado para identificar exclusivamente o cliente, assim como o cliente/parceiro pode atualizar o domínio intuitivo/padrão por meio do portal do O365.</span><span class="sxs-lookup"><span data-stu-id="4f116-412">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="4f116-413">Este campo pode aparecer em branco até o segundo ciclo de cobrança.</span><span class="sxs-lookup"><span data-stu-id="4f116-413">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4f116-414">País do cliente</span><span class="sxs-lookup"><span data-stu-id="4f116-414">Customer Country</span></span></td>
<td><p><span data-ttu-id="4f116-415">O país em que o cliente está localizado.</span><span class="sxs-lookup"><span data-stu-id="4f116-415">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4f116-416">Número da fatura</span><span class="sxs-lookup"><span data-stu-id="4f116-416">Invoice number</span></span></td>
<td><p><span data-ttu-id="4f116-417">Número da fatura na qual a transação especificada é exibida.</span><span class="sxs-lookup"><span data-stu-id="4f116-417">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4f116-418">MpnID</span><span class="sxs-lookup"><span data-stu-id="4f116-418">MpnId</span></span></td>
<td><p><span data-ttu-id="4f116-419">ID do MPN do parceiro CSP.</span><span class="sxs-lookup"><span data-stu-id="4f116-419">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4f116-420">Reseller MpnId</span><span class="sxs-lookup"><span data-stu-id="4f116-420">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="4f116-421">ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="4f116-421">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4f116-422">ID do Pedido</span><span class="sxs-lookup"><span data-stu-id="4f116-422">Order ID</span></span></td>
<td><p><span data-ttu-id="4f116-423">Identificador exclusivo para um pedido na plataforma de comércio do Microsoft.</span><span class="sxs-lookup"><span data-stu-id="4f116-423">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="4f116-424">Pode ser útil para identificar o pedido ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="4f116-424">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4f116-425">Data do pedido</span><span class="sxs-lookup"><span data-stu-id="4f116-425">Order date</span></span></td>
<td><p><span data-ttu-id="4f116-426">A data em que o pedido foi feito.</span><span class="sxs-lookup"><span data-stu-id="4f116-426">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4f116-427">ProductId</span><span class="sxs-lookup"><span data-stu-id="4f116-427">ProductId</span></span></td>
<td><p><span data-ttu-id="4f116-428">A ID do produto.</span><span class="sxs-lookup"><span data-stu-id="4f116-428">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4f116-429">SkuId</span><span class="sxs-lookup"><span data-stu-id="4f116-429">SkuId</span></span></td>
<td><p><span data-ttu-id="4f116-430">A ID de uma SKU em particular.</span><span class="sxs-lookup"><span data-stu-id="4f116-430">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4f116-431">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="4f116-431">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="4f116-432">A ID de uma Disponibilidade em particular.</span><span class="sxs-lookup"><span data-stu-id="4f116-432">The ID for a particular Availability.</span></span> <span data-ttu-id="4f116-433">"Disponibilidade" refere-se a se uma SKU em particular está disponível ou não para compra para determinado país, moeda, segmento do setor etc.</span><span class="sxs-lookup"><span data-stu-id="4f116-433">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4f116-434">Nome do SKU</span><span class="sxs-lookup"><span data-stu-id="4f116-434">SKU Name</span></span></td>
<td><p><span data-ttu-id="4f116-435">O título de uma SKU em particular.</span><span class="sxs-lookup"><span data-stu-id="4f116-435">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4f116-436">Nome do produto</span><span class="sxs-lookup"><span data-stu-id="4f116-436">Product name</span></span></td>
<td><p><span data-ttu-id="4f116-437">O nome do produto.</span><span class="sxs-lookup"><span data-stu-id="4f116-437">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4f116-438">PublisherName</span><span class="sxs-lookup"><span data-stu-id="4f116-438">PublisherName</span></span></td>
<td><p><span data-ttu-id="4f116-439">O nome do publicador do produto.</span><span class="sxs-lookup"><span data-stu-id="4f116-439">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4f116-440">PublisherID</span><span class="sxs-lookup"><span data-stu-id="4f116-440">PublisherID</span></span></td>
<td><p><span data-ttu-id="4f116-441">ID exclusiva para esse publicador.</span><span class="sxs-lookup"><span data-stu-id="4f116-441">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4f116-442">Descrição da assinatura</span><span class="sxs-lookup"><span data-stu-id="4f116-442">Subscription Description</span></span></td>
<td><p><span data-ttu-id="4f116-443">Nome amigável de uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="4f116-443">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4f116-444">ID da assinatura</span><span class="sxs-lookup"><span data-stu-id="4f116-444">Subscription ID</span></span></td>
<td><p><span data-ttu-id="4f116-445">Identificador exclusivo para uma assinatura da plataforma de comércio do Microsoft.</span><span class="sxs-lookup"><span data-stu-id="4f116-445">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="4f116-446">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="4f116-446">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="4f116-447">Esse não é o mesmo que o ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="4f116-447">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4f116-448">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="4f116-448">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="4f116-449">Dia de início dos encargos.</span><span class="sxs-lookup"><span data-stu-id="4f116-449">Start day of the charges.</span></span> <span data-ttu-id="4f116-450">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="4f116-450">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4f116-451">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="4f116-451">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="4f116-452">Dia do término dos encargos.</span><span class="sxs-lookup"><span data-stu-id="4f116-452">End day of the charges.</span></span> <span data-ttu-id="4f116-453">A hora é sempre o fim do dia, 23:59.</span><span class="sxs-lookup"><span data-stu-id="4f116-453">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4f116-454">Termo e Billingcycle</span><span class="sxs-lookup"><span data-stu-id="4f116-454">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="4f116-455">A vigência e o ciclo de cobrança para a compra.</span><span class="sxs-lookup"><span data-stu-id="4f116-455">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="4f116-456">Por exemplo, "1 ano, mês."</span><span class="sxs-lookup"><span data-stu-id="4f116-456">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4f116-457">Tipo de Cobrança</span><span class="sxs-lookup"><span data-stu-id="4f116-457">Charge Type</span></span></td>
<td><p><span data-ttu-id="4f116-458">O tipo de encargo ou ajuste.</span><span class="sxs-lookup"><span data-stu-id="4f116-458">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4f116-459">Preço unitário</span><span class="sxs-lookup"><span data-stu-id="4f116-459">Unit Price</span></span></td>
<td><p><span data-ttu-id="4f116-460">O preço como publicado no pricelist no momento da compra.</span><span class="sxs-lookup"><span data-stu-id="4f116-460">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="4f116-461">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="4f116-461">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4f116-462">Preço unitário efetiva</span><span class="sxs-lookup"><span data-stu-id="4f116-462">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="4f116-463">O preço unitário depois de fazer ajustes.</span><span class="sxs-lookup"><span data-stu-id="4f116-463">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4f116-464">Quantidade</span><span class="sxs-lookup"><span data-stu-id="4f116-464">Quantity</span></span></td>
<td><p><span data-ttu-id="4f116-465">Número de unidades.</span><span class="sxs-lookup"><span data-stu-id="4f116-465">Number of units.</span></span> <span data-ttu-id="4f116-466">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="4f116-466">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4f116-467">Tipo de unidade</span><span class="sxs-lookup"><span data-stu-id="4f116-467">Unit type</span></span></td>
<td><p><span data-ttu-id="4f116-468">O tipo de unidade que está sendo comprado.</span><span class="sxs-lookup"><span data-stu-id="4f116-468">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4f116-469">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="4f116-469">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="4f116-470">Obter uma explicação de qualquer desconto aplicável.</span><span class="sxs-lookup"><span data-stu-id="4f116-470">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4f116-471">Subtotal</span><span class="sxs-lookup"><span data-stu-id="4f116-471">Sub Total</span></span></td>
<td><p><span data-ttu-id="4f116-472">Total sem imposto.</span><span class="sxs-lookup"><span data-stu-id="4f116-472">Total before tax.</span></span> <span data-ttu-id="4f116-473">Verifica se seu subtotal corresponde ao total esperado, em caso de desconto.</span><span class="sxs-lookup"><span data-stu-id="4f116-473">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4f116-474">Total de impostos</span><span class="sxs-lookup"><span data-stu-id="4f116-474">Tax Total</span></span></td>
<td><p><span data-ttu-id="4f116-475">Valor do imposto cobrado, com base nas regras fiscais do mercado e em circunstâncias específicas.</span><span class="sxs-lookup"><span data-stu-id="4f116-475">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4f116-476">Total</span><span class="sxs-lookup"><span data-stu-id="4f116-476">Total</span></span></td>
<td><p><span data-ttu-id="4f116-477">Total com imposto.</span><span class="sxs-lookup"><span data-stu-id="4f116-477">Total after tax.</span></span> <span data-ttu-id="4f116-478">Verifica se o imposto é cobrado na fatura.</span><span class="sxs-lookup"><span data-stu-id="4f116-478">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4f116-479">Currency</span><span class="sxs-lookup"><span data-stu-id="4f116-479">Currency</span></span></td>
<td><p><span data-ttu-id="4f116-480">Tipo de moeda.</span><span class="sxs-lookup"><span data-stu-id="4f116-480">Currency type.</span></span> <span data-ttu-id="4f116-481">Cada entidade de cobrança tem somente uma moeda.</span><span class="sxs-lookup"><span data-stu-id="4f116-481">Each billing entity has only one currency.</span></span> <span data-ttu-id="4f116-482">Verifique se isso coincide com a primeira fatura e faça o mesmo após grandes atualizações na plataforma de cobrança.</span><span class="sxs-lookup"><span data-stu-id="4f116-482">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4f116-483">AlternateID</span><span class="sxs-lookup"><span data-stu-id="4f116-483">AlternateID</span></span></td>
<td><p><span data-ttu-id="4f116-484">Um identificador alternativo para uma ID.</span><span class="sxs-lookup"><span data-stu-id="4f116-484">An alternate identifier to an ID.</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="4f116-485">Campos de arquivo de uso classificada como diária</span><span class="sxs-lookup"><span data-stu-id="4f116-485">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="4f116-486">Column</span><span class="sxs-lookup"><span data-stu-id="4f116-486">Column</span></span></th>
<th><span data-ttu-id="4f116-487">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f116-487">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="4f116-488">PartnerID</span><span class="sxs-lookup"><span data-stu-id="4f116-488">PartnerId</span></span></td>
<td><p><span data-ttu-id="4f116-489">ID do parceiro, no formato GUID.</span><span class="sxs-lookup"><span data-stu-id="4f116-489">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4f116-490">PartnerName</span><span class="sxs-lookup"><span data-stu-id="4f116-490">PartnerName</span></span></td>
<td><p><span data-ttu-id="4f116-491">Nome do parceiro.</span><span class="sxs-lookup"><span data-stu-id="4f116-491">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4f116-492">CustomerID</span><span class="sxs-lookup"><span data-stu-id="4f116-492">CustomerId</span></span></td>
<td><p><span data-ttu-id="4f116-493">ID exclusiva da Microsoft, no formato GUID, usada para identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="4f116-493">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4f116-494">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="4f116-494">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="4f116-495">Nome da organização do cliente como informado no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="4f116-495">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="4f116-496">Isso é muito importante para reconciliar a fatura com as informações de seu sistema.</span><span class="sxs-lookup"><span data-stu-id="4f116-496">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4f116-497">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="4f116-497">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="4f116-498">O nome de domínio do cliente.</span><span class="sxs-lookup"><span data-stu-id="4f116-498">The customer’s domain name.</span></span> <span data-ttu-id="4f116-499">Não disponível para a atividade atual.</span><span class="sxs-lookup"><span data-stu-id="4f116-499">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4f116-500">País do cliente</span><span class="sxs-lookup"><span data-stu-id="4f116-500">Customer country</span></span></td>
<td><p><span data-ttu-id="4f116-501">O país em que o cliente está localizado.</span><span class="sxs-lookup"><span data-stu-id="4f116-501">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4f116-502">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="4f116-502">MPNID</span></span></td>
<td><p><span data-ttu-id="4f116-503">ID do MPN do parceiro CSP.</span><span class="sxs-lookup"><span data-stu-id="4f116-503">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4f116-504">Revendedor MPNID</span><span class="sxs-lookup"><span data-stu-id="4f116-504">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="4f116-505">ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="4f116-505">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="4f116-506">Não disponível para a atividade atual.</span><span class="sxs-lookup"><span data-stu-id="4f116-506">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4f116-507">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="4f116-507">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="4f116-508">Número da fatura na qual a transação especificada é exibida.</span><span class="sxs-lookup"><span data-stu-id="4f116-508">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="4f116-509">Não disponível para a atividade atual.</span><span class="sxs-lookup"><span data-stu-id="4f116-509">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4f116-510">ProductId</span><span class="sxs-lookup"><span data-stu-id="4f116-510">ProductId</span></span></td>
<td><p><span data-ttu-id="4f116-511">A ID do produto.</span><span class="sxs-lookup"><span data-stu-id="4f116-511">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4f116-512">SkuId</span><span class="sxs-lookup"><span data-stu-id="4f116-512">SkuId</span></span></td>
<td><p><span data-ttu-id="4f116-513">A ID de uma SKU em particular.</span><span class="sxs-lookup"><span data-stu-id="4f116-513">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4f116-514">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="4f116-514">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="4f116-515">A ID de uma Disponibilidade em particular.</span><span class="sxs-lookup"><span data-stu-id="4f116-515">The ID for a particular Availability.</span></span> <span data-ttu-id="4f116-516">"Disponibilidade" refere-se a se uma SKU em particular está disponível ou não para compra para determinado país, moeda, segmento do setor etc.</span><span class="sxs-lookup"><span data-stu-id="4f116-516">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4f116-517">Nome do SKU</span><span class="sxs-lookup"><span data-stu-id="4f116-517">SKU Name</span></span></td>
<td><p><span data-ttu-id="4f116-518">O título de uma SKU em particular.</span><span class="sxs-lookup"><span data-stu-id="4f116-518">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4f116-519">PublisherName</span><span class="sxs-lookup"><span data-stu-id="4f116-519">PublisherName</span></span></td>
<td><p><span data-ttu-id="4f116-520">O nome do publicador.</span><span class="sxs-lookup"><span data-stu-id="4f116-520">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4f116-521">PublisherID</span><span class="sxs-lookup"><span data-stu-id="4f116-521">PublisherID</span></span></td>
<td><p><span data-ttu-id="4f116-522">A ID do publicador, no formato GUID.</span><span class="sxs-lookup"><span data-stu-id="4f116-522">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="4f116-523">Não disponível para a atividade atual.</span><span class="sxs-lookup"><span data-stu-id="4f116-523">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="4f116-524">Descrição da assinatura</span><span class="sxs-lookup"><span data-stu-id="4f116-524">Subscription Description</span></span></td>
<td><p><span data-ttu-id="4f116-525">O nome da oferta de serviço comprada pelo cliente, conforme definido na tabela de preços.</span><span class="sxs-lookup"><span data-stu-id="4f116-525">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="4f116-526">(Este é um campo idêntico ao nome da oferta).</span><span class="sxs-lookup"><span data-stu-id="4f116-526">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4f116-527">ID da assinatura</span><span class="sxs-lookup"><span data-stu-id="4f116-527">Subscription ID</span></span></td>
<td><p><span data-ttu-id="4f116-528">Identificador exclusivo de uma assinatura na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="4f116-528">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="4f116-529">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="4f116-529">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="4f116-530">Esse não é o mesmo que o ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="4f116-530">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4f116-531">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="4f116-531">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="4f116-532">Data de início do ciclo de cobrança exceto quando apresentadas as datas de dados de uso latentes anteriormente não cobradas (do ciclo de cobrança anterior).</span><span class="sxs-lookup"><span data-stu-id="4f116-532">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="4f116-533">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="4f116-533">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4f116-534">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="4f116-534">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="4f116-535">Data de término do ciclo de cobrança exceto quando apresentadas as datas de dados de uso latentes anteriormente não cobradas (do ciclo de cobrança anterior).</span><span class="sxs-lookup"><span data-stu-id="4f116-535">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="4f116-536">A hora é sempre o fim do dia, 23:59.</span><span class="sxs-lookup"><span data-stu-id="4f116-536">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4f116-537">Data de uso</span><span class="sxs-lookup"><span data-stu-id="4f116-537">Usage Date</span></span></td>
<td><p><span data-ttu-id="4f116-538">Data de uso do serviço.</span><span class="sxs-lookup"><span data-stu-id="4f116-538">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4f116-539">Tipo de medidor</span><span class="sxs-lookup"><span data-stu-id="4f116-539">Meter Type</span></span></td>
<td><p><span data-ttu-id="4f116-540">O tipo de medidor.</span><span class="sxs-lookup"><span data-stu-id="4f116-540">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4f116-541">Categoria do medidor</span><span class="sxs-lookup"><span data-stu-id="4f116-541">Meter Category</span></span></td>
<td><p><span data-ttu-id="4f116-542">O serviço de nível superior para o uso.</span><span class="sxs-lookup"><span data-stu-id="4f116-542">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4f116-543">Id do medidor</span><span class="sxs-lookup"><span data-stu-id="4f116-543">Meter Id</span></span></td>
<td><p><span data-ttu-id="4f116-544">A ID do medidor que está sendo usado.</span><span class="sxs-lookup"><span data-stu-id="4f116-544">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4f116-545">Medir subcategoria</span><span class="sxs-lookup"><span data-stu-id="4f116-545">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="4f116-546">O tipo de serviço do Azure que pode afetar a tarifa.</span><span class="sxs-lookup"><span data-stu-id="4f116-546">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4f116-547">Nome do medidor</span><span class="sxs-lookup"><span data-stu-id="4f116-547">Meter Name</span></span></td>
<td><p><span data-ttu-id="4f116-548">A unidade de medida para o medidor sendo consumido.</span><span class="sxs-lookup"><span data-stu-id="4f116-548">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4f116-549">Região do medidor</span><span class="sxs-lookup"><span data-stu-id="4f116-549">Meter Region</span></span></td>
<td><p><span data-ttu-id="4f116-550">Essa coluna identifica a localização de um data center dentro da região para serviços onde isso é aplicável e preenchido.</span><span class="sxs-lookup"><span data-stu-id="4f116-550">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4f116-551">Unidade</span><span class="sxs-lookup"><span data-stu-id="4f116-551">Unit</span></span></td>
<td><p><span data-ttu-id="4f116-552">A unidade do nome do recurso.</span><span class="sxs-lookup"><span data-stu-id="4f116-552">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4f116-553">Quantidade consumida</span><span class="sxs-lookup"><span data-stu-id="4f116-553">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="4f116-554">A quantidade de serviço consumida (horas, GB etc.) durante o período de relatório.</span><span class="sxs-lookup"><span data-stu-id="4f116-554">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="4f116-555">Também inclui qualquer uso não cobrado de períodos de relatório anteriores.</span><span class="sxs-lookup"><span data-stu-id="4f116-555">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4f116-556">Local do recurso</span><span class="sxs-lookup"><span data-stu-id="4f116-556">Resource Location</span></span></td>
<td><p><span data-ttu-id="4f116-557">O datacenter em que o medidor está sendo executado.</span><span class="sxs-lookup"><span data-stu-id="4f116-557">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4f116-558">Serviço consumido</span><span class="sxs-lookup"><span data-stu-id="4f116-558">Consumed Service</span></span></td>
<td><p><span data-ttu-id="4f116-559">O serviço de plataforma do Azure que você usou.</span><span class="sxs-lookup"><span data-stu-id="4f116-559">The Azure platform service that you used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4f116-560">Grupo de Recursos</span><span class="sxs-lookup"><span data-stu-id="4f116-560">Resource Group</span></span></td>
<td><p><span data-ttu-id="4f116-561">O grupo de recursos no qual o medidor implantado está sendo executado.</span><span class="sxs-lookup"><span data-stu-id="4f116-561">The resource group in which the deployed meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4f116-562">URI de recurso</span><span class="sxs-lookup"><span data-stu-id="4f116-562">Resource URI</span></span></td>
<td><p><span data-ttu-id="4f116-563">O URI do recurso que está sendo usado.</span><span class="sxs-lookup"><span data-stu-id="4f116-563">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4f116-564">Tipo de cobrança</span><span class="sxs-lookup"><span data-stu-id="4f116-564">Charge type</span></span></td>
<td><p><span data-ttu-id="4f116-565">O tipo de encargo ou ajuste.</span><span class="sxs-lookup"><span data-stu-id="4f116-565">The type of charge or adjustment.</span></span> <span data-ttu-id="4f116-566">Não disponível para a atividade atual.</span><span class="sxs-lookup"><span data-stu-id="4f116-566">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4f116-567">Preço unitário</span><span class="sxs-lookup"><span data-stu-id="4f116-567">Unit price</span></span></td>
<td><p><span data-ttu-id="4f116-568">Preço por licença, como publicado no pricelist no momento da compra.</span><span class="sxs-lookup"><span data-stu-id="4f116-568">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="4f116-569">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="4f116-569">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4f116-570">Quantidade</span><span class="sxs-lookup"><span data-stu-id="4f116-570">Quantity</span></span></td>
<td><p><span data-ttu-id="4f116-571">Número de licenças.</span><span class="sxs-lookup"><span data-stu-id="4f116-571">Number of licenses.</span></span> <span data-ttu-id="4f116-572">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="4f116-572">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4f116-573">Tipo de unidade</span><span class="sxs-lookup"><span data-stu-id="4f116-573">Unit type</span></span></td>
<td><p><span data-ttu-id="4f116-574">O tipo de unidade, que o medidor é cobrado.</span><span class="sxs-lookup"><span data-stu-id="4f116-574">The type of unit the meter is charged in.</span></span> <span data-ttu-id="4f116-575">Não disponível para a atividade atual.</span><span class="sxs-lookup"><span data-stu-id="4f116-575">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4f116-576">Imposto de versão anterior de cobrança</span><span class="sxs-lookup"><span data-stu-id="4f116-576">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="4f116-577">Quantidade total antes dos impostos.</span><span class="sxs-lookup"><span data-stu-id="4f116-577">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4f116-578">Moeda de cobrança</span><span class="sxs-lookup"><span data-stu-id="4f116-578">Billing currency</span></span></td>
<td><p><span data-ttu-id="4f116-579">A moeda na região de geográfica do cliente</span><span class="sxs-lookup"><span data-stu-id="4f116-579">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4f116-580">Preço total pretax</span><span class="sxs-lookup"><span data-stu-id="4f116-580">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="4f116-581">O preço antes de impostos forem adicionados.</span><span class="sxs-lookup"><span data-stu-id="4f116-581">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4f116-582">Preços de moeda</span><span class="sxs-lookup"><span data-stu-id="4f116-582">Pricing currency</span></span></td>
<td><p><span data-ttu-id="4f116-583">A moeda no pricelist.</span><span class="sxs-lookup"><span data-stu-id="4f116-583">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4f116-584">Informações do serviço 1</span><span class="sxs-lookup"><span data-stu-id="4f116-584">Service Info 1</span></span></td>
<td><p><span data-ttu-id="4f116-585">O número de conexões ServiceBus que foram provisionados e utilizados em um dia específico.</span><span class="sxs-lookup"><span data-stu-id="4f116-585">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4f116-586">Informações do serviço 2</span><span class="sxs-lookup"><span data-stu-id="4f116-586">Service Info 2</span></span></td>
<td><p><span data-ttu-id="4f116-587">Um campo herdado que captura os metadados específicos do serviço opcional.</span><span class="sxs-lookup"><span data-stu-id="4f116-587">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4f116-588">Marcas</span><span class="sxs-lookup"><span data-stu-id="4f116-588">Tags</span></span></td>
<td><p><span data-ttu-id="4f116-589">Marcas que você atribui ao medidor na ordem para agrupar registros de cobrança.</span><span class="sxs-lookup"><span data-stu-id="4f116-589">Tags you assign to the meter in order to group billing records.</span></span> <span data-ttu-id="4f116-590">Por exemplo, você pode usar marcas para distribuir os custos entre os departamentos que usam o medidor.</span><span class="sxs-lookup"><span data-stu-id="4f116-590">For example, you can use tags to distribute costs by the department that uses the meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4f116-591">Informações adicionais</span><span class="sxs-lookup"><span data-stu-id="4f116-591">Additional Info</span></span></td>
<td><p><span data-ttu-id="4f116-592">Informações adicionais não são abordadas em outras colunas.</span><span class="sxs-lookup"><span data-stu-id="4f116-592">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="4f116-593">Encargos de mapeamento entre uma nota fiscal e o arquivo de reconciliação</span><span class="sxs-lookup"><span data-stu-id="4f116-593">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="4f116-594">Sua fatura fornece um resumo dos encargos, enquanto seu arquivo de reconciliação fornece uma divisão detalhada das transações de item de linha, incluindo os tipos de carga.</span><span class="sxs-lookup"><span data-stu-id="4f116-594">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="4f116-595">Para fazer referência cruzada das quantidades de carga entre o arquivo de reconciliação e fatura, você pode usar opções de filtro do Microsoft Excel para filtrar por tipos de cobrança no arquivo de reconciliação para mapear os encargos de fatura em um conjunto de detalhamentos de cobrança no arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="4f116-595">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="4f116-596">Os arquivos de reconciliação, tanto os baseados em licença quanto os baseados em uso, mostram apenas encargos e transações relacionadas ao uso (unidades consumidas e encargos relacionados).</span><span class="sxs-lookup"><span data-stu-id="4f116-596">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="4f116-597">Créditos únicos, descontos ou reembolsos que aparecem na fatura como "Ajustes" não são mostrados no arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="4f116-597">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="4f116-598">A tabela a seguir mostra os mapeamentos entre uma seção da fatura e os tipos de encargo associados que podem aparecer nos arquivos de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="4f116-598">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="4f116-599"><strong>Descrição de encargo de fatura</strong></span><span class="sxs-lookup"><span data-stu-id="4f116-599"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="4f116-600"><strong>Descrição de cobrança de arquivo de reconciliação (ChargeType coluna)</strong></span><span class="sxs-lookup"><span data-stu-id="4f116-600"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="4f116-601"><strong>O que é a cobrança?</strong></span><span class="sxs-lookup"><span data-stu-id="4f116-601"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="4f116-602"><strong>Como faço para mapear esses ChargeTypes à fatura?</strong></span><span class="sxs-lookup"><span data-stu-id="4f116-602"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="4f116-603"><strong>Encargos de licença</strong></span><span class="sxs-lookup"><span data-stu-id="4f116-603"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="4f116-604">Taxa de ativação</span><span class="sxs-lookup"><span data-stu-id="4f116-604">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="4f116-605">O valor cobrado do cliente quando ele usa a assinatura depois de comprá-la.</span><span class="sxs-lookup"><span data-stu-id="4f116-605">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="4f116-606">No arquivo baseado em licença, some a coluna <strong>Quantidade</strong></span><span class="sxs-lookup"><span data-stu-id="4f116-606">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="4f116-607">Taxa de cancelamento</span><span class="sxs-lookup"><span data-stu-id="4f116-607">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="4f116-608">Os encargos proporcionais reembolsados para o cliente quando os assentos associados são alterados</span><span class="sxs-lookup"><span data-stu-id="4f116-608">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="4f116-609">Taxa do ciclo</span><span class="sxs-lookup"><span data-stu-id="4f116-609">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="4f116-610">Encargos periódicos de uma assinatura</span><span class="sxs-lookup"><span data-stu-id="4f116-610">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="4f116-611">Proporcional à instância do ciclo</span><span class="sxs-lookup"><span data-stu-id="4f116-611">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="4f116-612">Os encargos proporcionais cobrados do cliente quando os assentos associados são alterados</span><span class="sxs-lookup"><span data-stu-id="4f116-612">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="4f116-613">Taxas proporcionais durante o cancelamento</span><span class="sxs-lookup"><span data-stu-id="4f116-613">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="4f116-614">Reembolso proporcional para a parte não utilizada do serviço após o cancelamento</span><span class="sxs-lookup"><span data-stu-id="4f116-614">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="4f116-615">Taxas proporcionais durante a compra</span><span class="sxs-lookup"><span data-stu-id="4f116-615">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="4f116-616">O tipo de encargo para uma assinatura ao usar cobranças anuais</span><span class="sxs-lookup"><span data-stu-id="4f116-616">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="4f116-617">Valor de compra</span><span class="sxs-lookup"><span data-stu-id="4f116-617">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="4f116-618">O tipo de encargo para uma assinatura ao usar a cobrança mensal</span><span class="sxs-lookup"><span data-stu-id="4f116-618">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="4f116-619">Taxa proporcional ao renovar</span><span class="sxs-lookup"><span data-stu-id="4f116-619">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="4f116-620">Taxas proporcionais após a renovação da assinatura</span><span class="sxs-lookup"><span data-stu-id="4f116-620">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="4f116-621">Taxa de renovação</span><span class="sxs-lookup"><span data-stu-id="4f116-621">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="4f116-622">Cobrança para renovação de uma assinatura</span><span class="sxs-lookup"><span data-stu-id="4f116-622">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="4f116-623">Taxas proporcionais ao ativar</span><span class="sxs-lookup"><span data-stu-id="4f116-623">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="4f116-624">Taxas proporcionais da ativação até o final do período de cobrança</span><span class="sxs-lookup"><span data-stu-id="4f116-624">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><span data-ttu-id="4f116-625"><strong>Encargos de uso</strong></span><span class="sxs-lookup"><span data-stu-id="4f116-625"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="4f116-626">Avaliar a taxa de uso ao cancelar</span><span class="sxs-lookup"><span data-stu-id="4f116-626">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="4f116-627">Taxa de uso de acesso com o cancelamento para uso não pago durante o período de cobrança atual</span><span class="sxs-lookup"><span data-stu-id="4f116-627">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="4f116-628">No arquivo baseado em uso, some a coluna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="4f116-628">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="4f116-629">Avalie a taxa de uso para o ciclo atual</span><span class="sxs-lookup"><span data-stu-id="4f116-629">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="4f116-630">Taxa de uso de acesso para o período atual de cobrança</span><span class="sxs-lookup"><span data-stu-id="4f116-630">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="4f116-631"><strong>Créditos</strong></span><span class="sxs-lookup"><span data-stu-id="4f116-631"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="4f116-632">Deslocando um item de linha</span><span class="sxs-lookup"><span data-stu-id="4f116-632">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="4f116-633">Reembolso parcial ou integral para um item de linha, incluindo os impostos</span><span class="sxs-lookup"><span data-stu-id="4f116-633">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="4f116-634">No arquivo baseado em licença, some a coluna <strong>TotalForCustomer</strong></span><span class="sxs-lookup"><span data-stu-id="4f116-634">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="4f116-635">No arquivo baseado em uso, some a coluna <strong>PostTaxTotal</strong></span><span class="sxs-lookup"><span data-stu-id="4f116-635">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="4f116-636"><strong>Descontos com base no uso</strong></span><span class="sxs-lookup"><span data-stu-id="4f116-636"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="4f116-637">Desconto de ativação</span><span class="sxs-lookup"><span data-stu-id="4f116-637">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="4f116-638">Desconto aplicado quando a assinatura é ativada</span><span class="sxs-lookup"><span data-stu-id="4f116-638">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="4f116-639">No arquivo baseado em uso, some a coluna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="4f116-639">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="4f116-640">Desconto de ciclo</span><span class="sxs-lookup"><span data-stu-id="4f116-640">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="4f116-641">Desconto aplicado em cobranças periódicas</span><span class="sxs-lookup"><span data-stu-id="4f116-641">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="4f116-642">Desconto de renovação</span><span class="sxs-lookup"><span data-stu-id="4f116-642">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="4f116-643">Desconto aplicado quando a assinatura é renovada</span><span class="sxs-lookup"><span data-stu-id="4f116-643">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="4f116-644">Desconto de cancelamento</span><span class="sxs-lookup"><span data-stu-id="4f116-644">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="4f116-645">Encargos aplicados quando descontos são cancelados</span><span class="sxs-lookup"><span data-stu-id="4f116-645">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="4f116-646"><strong>Descontos de licença</strong></span><span class="sxs-lookup"><span data-stu-id="4f116-646"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="4f116-647"><em>Pode ser aplicado a vários tipos de custo</em></span><span class="sxs-lookup"><span data-stu-id="4f116-647"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="4f116-648">No arquivo baseado em licença, some a coluna <strong>TotalOtherDiscount</strong></span><span class="sxs-lookup"><span data-stu-id="4f116-648">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="4f116-649"><strong>Impostos</strong>&nbsp;ou&nbsp;<strong>IVA</strong></span><span class="sxs-lookup"><span data-stu-id="4f116-649"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="4f116-650"><em>Pode ser aplicado a vários tipos de custo</em></span><span class="sxs-lookup"><span data-stu-id="4f116-650"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="4f116-651"><em>Exceção: &quot;Deslocamento de um item de linha&quot; já inclui os impostos. Ver créditos, acima.</em></span><span class="sxs-lookup"><span data-stu-id="4f116-651"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="4f116-652">Impostos ou impostos sobre valor agregado (IVA)</span><span class="sxs-lookup"><span data-stu-id="4f116-652">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="4f116-653">No arquivo baseado em licença, some a coluna <strong>Imposto</strong></span><span class="sxs-lookup"><span data-stu-id="4f116-653">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="4f116-654">No arquivo baseado em uso, some a coluna <strong>TaxAmount</strong></span><span class="sxs-lookup"><span data-stu-id="4f116-654">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
