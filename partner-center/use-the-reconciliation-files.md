---
title: Usar os arquivos de reconciliação | Partner Center
ms.topic: article
ms.date: 10/29/2018
description: Para uma exibição detalhada do item de linha de cada encargo em um ciclo de cobrança, baixe os arquivos de reconciliação do Partner Center.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: KPacquer
ms.author: kenpacq
ms.localizationpriority: medium
ms.openlocfilehash: 4b5fbab84c30743e4d91b32bf4cbd2bb8b950992
ms.sourcegitcommit: b433061dff8f667c81b623c33417fb490d8e3b4a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2018
ms.locfileid: "6022241"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="d870f-103">Usar os arquivos de reconciliação</span><span class="sxs-lookup"><span data-stu-id="d870f-103">Use the reconciliation files</span></span>

**<span data-ttu-id="d870f-104">Aplicável a</span><span class="sxs-lookup"><span data-stu-id="d870f-104">Applies to</span></span>**

-  <span data-ttu-id="d870f-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="d870f-105">Partner Center</span></span>
-  <span data-ttu-id="d870f-106">Partner Center for Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="d870f-106">Partner Center for Microsoft Cloud for US Government</span></span>
-  <span data-ttu-id="d870f-107">Partner Center do Microsoft Cloud Germany</span><span class="sxs-lookup"><span data-stu-id="d870f-107">Partner Center for Microsoft Cloud Germany</span></span>

<span data-ttu-id="d870f-108">Para uma exibição detalhada do item de linha de cada encargo em um ciclo de cobrança, baixe os arquivos de reconciliação do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="d870f-108">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="d870f-109">Os detalhes incluem encargos por assinaturas de cada cliente e eventos detalhados (como a adição de assentos a uma assinatura no meio do período).</span><span class="sxs-lookup"><span data-stu-id="d870f-109">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="d870f-110">Discriminar por parceiro</span><span class="sxs-lookup"><span data-stu-id="d870f-110">Itemize by partner</span></span>


<span data-ttu-id="d870f-111">Os parceiros no modelo indireto podem usar esses campos adicionais nos arquivos de reconciliação baseados em uso e em licença para discriminar por revendedor.</span><span class="sxs-lookup"><span data-stu-id="d870f-111">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="d870f-112">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="d870f-112">MPN ID</span></span></th>
<th><span data-ttu-id="d870f-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="d870f-113">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="d870f-114">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="d870f-114">MPN ID</span></span></td>
<td><p><span data-ttu-id="d870f-115">A ID do Microsoft Partner Network (MPN) do parceiro CSP (direta ou indireta).</span><span class="sxs-lookup"><span data-stu-id="d870f-115">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d870f-116">ID do MPN do revendedor</span><span class="sxs-lookup"><span data-stu-id="d870f-116">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="d870f-117">Só aparece em arquivos de reconciliação para parceiros no modelo indireto.</span><span class="sxs-lookup"><span data-stu-id="d870f-117">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="d870f-118">A ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="d870f-118">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="d870f-119">Isso corresponde à ID de revendedor listada para a assinatura específica no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="d870f-119">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="d870f-120">Para exibir ou atualizar o revendedor, no menu Partner Center, selecione <strong>clientes</strong>e, em seguida, escolha o cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="d870f-120">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="d870f-121">No menu do cliente, selecione <strong>Assinaturas</strong>, escolha a assinatura na lista.</span><span class="sxs-lookup"><span data-stu-id="d870f-121">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="d870f-122">Selecione <strong>Atualizar</strong> para alterar o <strong>Revendedor (ID do MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="d870f-122">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="d870f-123">Se um parceiro CSP vendeu a assinatura diretamente para o cliente, sua ID do MPN estará listada duas vezes, como a ID do MPN e a ID do MPN do revendedor.</span><span class="sxs-lookup"><span data-stu-id="d870f-123">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="d870f-124">Se um parceiro CSP tiver um revendedor sem ID do MPN, esse valor será definido como a ID do MPN do parceiro.</span><span class="sxs-lookup"><span data-stu-id="d870f-124">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="d870f-125">Se o parceiro CSP remover uma ID de revendedor, esse valor será definido como -1.</span><span class="sxs-lookup"><span data-stu-id="d870f-125">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="d870f-126">Campos de arquivos baseado em licença</span><span class="sxs-lookup"><span data-stu-id="d870f-126">License-based file fields</span></span>


<span data-ttu-id="d870f-127">Para reconciliar seus encargos com os pedidos de seu cliente, compare o campo Syndication\_Partner\_Subscription\_Number do arquivo de reconciliação com a ID de Assinatura do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="d870f-127">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="d870f-128">Coluna</span><span class="sxs-lookup"><span data-stu-id="d870f-128">Column</span></span></strong></td>
<td><strong><span data-ttu-id="d870f-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="d870f-129">Description</span></span></strong></td>
<td><strong><span data-ttu-id="d870f-130">Valor de exemplo</span><span class="sxs-lookup"><span data-stu-id="d870f-130">Sample Value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d870f-131">PartnerId</span><span class="sxs-lookup"><span data-stu-id="d870f-131">PartnerId</span></span></td>
<td><p><span data-ttu-id="d870f-132">Identificador exclusivo de uma entidade de cobrança específica, em formato GUID.</span><span class="sxs-lookup"><span data-stu-id="d870f-132">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="d870f-133">Não é necessário para reconciliação, mas pode ser uma informação útil.</span><span class="sxs-lookup"><span data-stu-id="d870f-133">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="d870f-134">O mesmo em todas as linhas.</span><span class="sxs-lookup"><span data-stu-id="d870f-134">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="d870f-135">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="d870f-135">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d870f-136">CustomerID</span><span class="sxs-lookup"><span data-stu-id="d870f-136">CustomerID</span></span></td>
<td><p><span data-ttu-id="d870f-137">ID exclusiva da Microsoft, no formato GUID, usada para identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="d870f-137">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="d870f-138">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="d870f-138">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d870f-139">OrderID</span><span class="sxs-lookup"><span data-stu-id="d870f-139">OrderID</span></span></td>
<td><p><span data-ttu-id="d870f-140">Identificador exclusivo para um pedido na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d870f-140">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="d870f-141">Pode ser útil para identificar o pedido ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="d870f-141">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="d870f-142">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="d870f-142">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d870f-143">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="d870f-143">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="d870f-144">Identificador exclusivo de uma assinatura na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d870f-144">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="d870f-145">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="d870f-145">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="d870f-146">Esse não é o mesmo que o ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="d870f-146">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="d870f-147">Consulte Número_Assinatura_Parceiro_Sindicalização.</span><span class="sxs-lookup"><span data-stu-id="d870f-147">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="d870f-148">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="d870f-148">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d870f-149">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="d870f-149">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="d870f-150">Identificador exclusivo para assinaturas.</span><span class="sxs-lookup"><span data-stu-id="d870f-150">Unique identifier for subscriptions.</span></span> <span data-ttu-id="d870f-151">Target: Um cliente pode ter várias assinaturas para o mesmo plano, portanto, isso é importante para análise de arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="d870f-151">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="d870f-152">Esse campo é mapeado para a ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="d870f-152">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="d870f-153">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="d870f-153">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d870f-154">OfferID</span><span class="sxs-lookup"><span data-stu-id="d870f-154">OfferID</span></span></td>
<td><p><span data-ttu-id="d870f-155">ID exclusivo da oferta.</span><span class="sxs-lookup"><span data-stu-id="d870f-155">Unique offer ID.</span></span> <span data-ttu-id="d870f-156">ID padrão da oferta de acordo com a lista de preços.</span><span class="sxs-lookup"><span data-stu-id="d870f-156">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="d870f-157"><b>Observação</b>: esse valor não coincide com a ID de oferta da lista de preços.</span><span class="sxs-lookup"><span data-stu-id="d870f-157"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="d870f-158">Veja DurableOfferID abaixo.</span><span class="sxs-lookup"><span data-stu-id="d870f-158">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="d870f-159">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="d870f-159">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d870f-160">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="d870f-160">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="d870f-161">ID exclusiva da oferta durável, conforme definido na tabela de preços.</span><span class="sxs-lookup"><span data-stu-id="d870f-161">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="d870f-162"><b>Observação</b>: esse valor corresponde à ID de oferta da lista de preços.</span><span class="sxs-lookup"><span data-stu-id="d870f-162"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="d870f-163">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="d870f-163">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d870f-164">OfferName</span><span class="sxs-lookup"><span data-stu-id="d870f-164">OfferName</span></span></td>
<td><p><span data-ttu-id="d870f-165">O nome da oferta de serviço comprada pelo cliente, conforme definido na tabela de preços.</span><span class="sxs-lookup"><span data-stu-id="d870f-165">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="d870f-166">Microsoft Office 365 (plano E3)</span><span class="sxs-lookup"><span data-stu-id="d870f-166">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d870f-167">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="d870f-167">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="d870f-168">A data de início da assinatura, definida como um dia após o pedido ser enviado.</span><span class="sxs-lookup"><span data-stu-id="d870f-168">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="d870f-169">Verificando a data de início da assinatura em conjunto com a data de término, você pode determinar se o cliente está dentro do primeiro ano da assinatura ou se a assinatura foi renovada para o ano seguinte.</span><span class="sxs-lookup"><span data-stu-id="d870f-169">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="d870f-170">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="d870f-170">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="d870f-171">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="d870f-171">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d870f-172">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="d870f-172">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="d870f-173">A data do término da assinatura: 12 meses + x dias após a data de início (para se alinhar com a data de cobrança do parceiro) ou 12 meses a partir da data de renovação.</span><span class="sxs-lookup"><span data-stu-id="d870f-173">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="d870f-174">Na renovação, os preços são atualizados com a tabela de preços atual.</span><span class="sxs-lookup"><span data-stu-id="d870f-174">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="d870f-175">Um comunicado ao cliente pode ser necessário antes da renovação automática.</span><span class="sxs-lookup"><span data-stu-id="d870f-175">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="d870f-176">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="d870f-176">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="d870f-177">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="d870f-177">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d870f-178">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="d870f-178">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="d870f-179">Dia de início dos encargos.</span><span class="sxs-lookup"><span data-stu-id="d870f-179">Start day of the charges.</span></span></p>
<p><span data-ttu-id="d870f-180">Quando o cliente muda o número de assentos, esse número é usado para calcular os encargos por dia (pro-rata).</span><span class="sxs-lookup"><span data-stu-id="d870f-180">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="d870f-181">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="d870f-181">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="d870f-182">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="d870f-182">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d870f-183">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="d870f-183">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="d870f-184">Dia do término dos encargos.</span><span class="sxs-lookup"><span data-stu-id="d870f-184">End day of the charges.</span></span></p>
<p><span data-ttu-id="d870f-185">Quando o cliente muda o número de assentos, esse número é usado para calcular os encargos por dia (pro-rata).</span><span class="sxs-lookup"><span data-stu-id="d870f-185">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="d870f-186">A hora é sempre o fim do dia, 23:59.</span><span class="sxs-lookup"><span data-stu-id="d870f-186">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="d870f-187">28/2/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="d870f-187">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d870f-188">ChargeType</span><span class="sxs-lookup"><span data-stu-id="d870f-188">ChargeType</span></span></td>
<td><p><span data-ttu-id="d870f-189">O tipo de encargo ou ajuste.</span><span class="sxs-lookup"><span data-stu-id="d870f-189">The type of charge or adjustment.</span></span> <span data-ttu-id="d870f-190">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="d870f-190">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="d870f-191">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="d870f-191">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d870f-192">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="d870f-192">UnitPrice</span></span></td>
<td><p><span data-ttu-id="d870f-193">Preço por estação, conforme publicado na lista de preços no momento da compra.</span><span class="sxs-lookup"><span data-stu-id="d870f-193">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="d870f-194">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="d870f-194">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="d870f-195">6.82</span><span class="sxs-lookup"><span data-stu-id="d870f-195">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d870f-196">Quantity</span><span class="sxs-lookup"><span data-stu-id="d870f-196">Quantity</span></span></td>
<td><p><span data-ttu-id="d870f-197">Número de assentos.</span><span class="sxs-lookup"><span data-stu-id="d870f-197">Number of seats.</span></span> <span data-ttu-id="d870f-198">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="d870f-198">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="d870f-199">2</span><span class="sxs-lookup"><span data-stu-id="d870f-199">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d870f-200">Quantidade</span><span class="sxs-lookup"><span data-stu-id="d870f-200">Amount</span></span></td>
<td><p><span data-ttu-id="d870f-201">Preço total por quantidade.</span><span class="sxs-lookup"><span data-stu-id="d870f-201">Total of price for quantity.</span></span> <span data-ttu-id="d870f-202">Útil para verificar se o cálculo do valor coincide com a forma como você calcula isso para seus clientes.</span><span class="sxs-lookup"><span data-stu-id="d870f-202">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="d870f-203">13.32</span><span class="sxs-lookup"><span data-stu-id="d870f-203">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d870f-204">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="d870f-204">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="d870f-205">Valor de desconto aplicado a esses encargos.</span><span class="sxs-lookup"><span data-stu-id="d870f-205">Amount of discount applied to these charges.</span></span> <span data-ttu-id="d870f-206">IUR ou novas assinaturas qualificadas para incentivo também conterão um valor de desconto nessa coluna.</span><span class="sxs-lookup"><span data-stu-id="d870f-206">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="d870f-207">2.32</span><span class="sxs-lookup"><span data-stu-id="d870f-207">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d870f-208">Subtotal</span><span class="sxs-lookup"><span data-stu-id="d870f-208">Subtotal</span></span></td>
<td><p><span data-ttu-id="d870f-209">Total sem imposto.</span><span class="sxs-lookup"><span data-stu-id="d870f-209">Total before tax.</span></span> <span data-ttu-id="d870f-210">Verifica se seu subtotal corresponde ao total esperado, em caso de desconto.</span><span class="sxs-lookup"><span data-stu-id="d870f-210">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="d870f-211">11</span><span class="sxs-lookup"><span data-stu-id="d870f-211">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d870f-212">Imposto</span><span class="sxs-lookup"><span data-stu-id="d870f-212">Tax</span></span></td>
<td><p><span data-ttu-id="d870f-213">Valor do imposto cobrado, com base nas regras fiscais do mercado e em circunstâncias específicas.</span><span class="sxs-lookup"><span data-stu-id="d870f-213">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="d870f-214">0</span><span class="sxs-lookup"><span data-stu-id="d870f-214">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d870f-215">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="d870f-215">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="d870f-216">Total com imposto.</span><span class="sxs-lookup"><span data-stu-id="d870f-216">Total after tax.</span></span> <span data-ttu-id="d870f-217">Verifica se o imposto é cobrado na fatura.</span><span class="sxs-lookup"><span data-stu-id="d870f-217">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="d870f-218">11</span><span class="sxs-lookup"><span data-stu-id="d870f-218">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d870f-219">Moeda</span><span class="sxs-lookup"><span data-stu-id="d870f-219">Currency</span></span></td>
<td><p><span data-ttu-id="d870f-220">Tipo de moeda.</span><span class="sxs-lookup"><span data-stu-id="d870f-220">Currency type.</span></span> <span data-ttu-id="d870f-221">Cada entidade de cobrança tem somente uma moeda.</span><span class="sxs-lookup"><span data-stu-id="d870f-221">Each billing entity has only one currency.</span></span> <span data-ttu-id="d870f-222">Verifique se isso coincide com a primeira fatura e faça o mesmo após grandes atualizações na plataforma de cobrança.</span><span class="sxs-lookup"><span data-stu-id="d870f-222">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="d870f-223">Euro</span><span class="sxs-lookup"><span data-stu-id="d870f-223">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d870f-224">CustomerName</span><span class="sxs-lookup"><span data-stu-id="d870f-224">CustomerName</span></span></td>
<td><p><span data-ttu-id="d870f-225">Nome da organização do cliente como informado no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="d870f-225">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="d870f-226">Isso é muito importante para reconciliar a fatura com as informações de seu sistema.</span><span class="sxs-lookup"><span data-stu-id="d870f-226">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="d870f-227">Cliente de teste A</span><span class="sxs-lookup"><span data-stu-id="d870f-227">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d870f-228">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="d870f-228">MPNID</span></span></td>
<td><p><span data-ttu-id="d870f-229">ID do MPN do parceiro CSP</span><span class="sxs-lookup"><span data-stu-id="d870f-229">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="d870f-230">4390934</span><span class="sxs-lookup"><span data-stu-id="d870f-230">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d870f-231">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="d870f-231">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="d870f-232">ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="d870f-232">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="d870f-233">Consulte [Discriminar por parceiro](#itemizebypartner).</span><span class="sxs-lookup"><span data-stu-id="d870f-233">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="d870f-234">4390934</span><span class="sxs-lookup"><span data-stu-id="d870f-234">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d870f-235">DomainName</span><span class="sxs-lookup"><span data-stu-id="d870f-235">DomainName</span></span></td>
<td><p><span data-ttu-id="d870f-236">Nome de domínio do cliente, usado para ajudar a identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="d870f-236">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="d870f-237">Isso não deve ser usado para identificar exclusivamente o cliente como o cliente/parceiro pode atualizar o domínio banidos/padrão através do portal do O365.</span><span class="sxs-lookup"><span data-stu-id="d870f-237">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="d870f-238">Este campo pode aparecer em branco até o segundo ciclo de cobrança.</span><span class="sxs-lookup"><span data-stu-id="d870f-238">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="d870f-239">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="d870f-239">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d870f-240">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="d870f-240">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="d870f-241">Apelido da Inscrição.</span><span class="sxs-lookup"><span data-stu-id="d870f-241">Subscription nickname.</span></span> <span data-ttu-id="d870f-242">Se nenhum apelido for especificado, o Partner Center usa o OfferName.</span><span class="sxs-lookup"><span data-stu-id="d870f-242">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="d870f-243">PROJETO ONLINE</span><span class="sxs-lookup"><span data-stu-id="d870f-243">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d870f-244">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="d870f-244">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="d870f-245">O nome da oferta de serviço comprada pelo cliente, conforme definido na tabela de preços.</span><span class="sxs-lookup"><span data-stu-id="d870f-245">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="d870f-246">(Este é um campo idêntico ao nome da oferta).</span><span class="sxs-lookup"><span data-stu-id="d870f-246">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="d870f-247">PROJETO ONLINE PREMIUM SEM PROJETO CLIENTE</span><span class="sxs-lookup"><span data-stu-id="d870f-247">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="d870f-248">Campos de arquivo baseado em uso</span><span class="sxs-lookup"><span data-stu-id="d870f-248">Usage-based file fields</span></span>


<span data-ttu-id="d870f-249">Para reconciliar seus encargos com o uso de seu cliente, compare ResellerID/ResellerName/ResellerBillableAccount do arquivo de reconciliação com o nome do cliente e a ID da assinatura do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="d870f-249">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="d870f-250">Os campos a seguir explicam quais serviços foram usados e a taxa.</span><span class="sxs-lookup"><span data-stu-id="d870f-250">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="d870f-251">Coluna</span><span class="sxs-lookup"><span data-stu-id="d870f-251">Column</span></span></strong></td>
<td><strong><span data-ttu-id="d870f-252">Descrição</span><span class="sxs-lookup"><span data-stu-id="d870f-252">Description</span></span></strong></td>
<td><strong><span data-ttu-id="d870f-253">Valor de exemplo</span><span class="sxs-lookup"><span data-stu-id="d870f-253">Sample value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d870f-254">PartnerID</span><span class="sxs-lookup"><span data-stu-id="d870f-254">PartnerID</span></span></td>
<td><p><span data-ttu-id="d870f-255">ID do parceiro, no formato GUID.</span><span class="sxs-lookup"><span data-stu-id="d870f-255">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="d870f-256">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="d870f-256">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d870f-257">PartnerName</span><span class="sxs-lookup"><span data-stu-id="d870f-257">PartnerName</span></span></td>
<td><p><span data-ttu-id="d870f-258">Nome do parceiro.</span><span class="sxs-lookup"><span data-stu-id="d870f-258">Partner Name.</span></span></p></td>
<td><span data-ttu-id="d870f-259">Acme incorporado</span><span class="sxs-lookup"><span data-stu-id="d870f-259">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d870f-260">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="d870f-260">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="d870f-261">ID da conta do parceiro.</span><span class="sxs-lookup"><span data-stu-id="d870f-261">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="d870f-262">1010578050</span><span class="sxs-lookup"><span data-stu-id="d870f-262">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d870f-263">CustomerName</span><span class="sxs-lookup"><span data-stu-id="d870f-263">CustomerName</span></span></td>
<td><p><span data-ttu-id="d870f-264">Nome da organização do cliente como informado no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="d870f-264">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="d870f-265">Isso é muito importante para reconciliar a fatura com as informações de seu sistema.</span><span class="sxs-lookup"><span data-stu-id="d870f-265">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="d870f-266">Cliente de teste A</span><span class="sxs-lookup"><span data-stu-id="d870f-266">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d870f-267">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="d870f-267">MPNID</span></span></td>
<td><p><span data-ttu-id="d870f-268">ID do MPN do parceiro CSP.</span><span class="sxs-lookup"><span data-stu-id="d870f-268">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="d870f-269">4390934</span><span class="sxs-lookup"><span data-stu-id="d870f-269">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d870f-270">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="d870f-270">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="d870f-271">ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="d870f-271">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="d870f-272">Consulte [Discriminar por parceiro](#itemizebypartner).</span><span class="sxs-lookup"><span data-stu-id="d870f-272">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="d870f-273">4390934</span><span class="sxs-lookup"><span data-stu-id="d870f-273">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d870f-274">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="d870f-274">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="d870f-275">Número da fatura na qual a transação especificada é exibida.</span><span class="sxs-lookup"><span data-stu-id="d870f-275">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="d870f-276">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="d870f-276">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d870f-277">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="d870f-277">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="d870f-278">Data de início do ciclo de cobrança exceto quando apresentadas as datas de dados de uso latentes anteriormente não cobradas (do ciclo de cobrança anterior).</span><span class="sxs-lookup"><span data-stu-id="d870f-278">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="d870f-279">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="d870f-279">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="d870f-280">1/2/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="d870f-280">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d870f-281">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="d870f-281">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="d870f-282">Data de término do ciclo de cobrança exceto quando apresentadas as datas de dados de uso latentes anteriormente não cobradas (do ciclo de cobrança anterior).</span><span class="sxs-lookup"><span data-stu-id="d870f-282">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="d870f-283">A hora é sempre o fim do dia, 23:59.</span><span class="sxs-lookup"><span data-stu-id="d870f-283">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="d870f-284">28/2/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="d870f-284">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d870f-285">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="d870f-285">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="d870f-286">Identificador exclusivo de uma assinatura na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d870f-286">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="d870f-287">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="d870f-287">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="d870f-288">Esse não é o mesmo que a ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="d870f-288">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="d870f-289">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="d870f-289">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d870f-290">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="d870f-290">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="d870f-291">Apelido da oferta do serviço.</span><span class="sxs-lookup"><span data-stu-id="d870f-291">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="d870f-292">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="d870f-292">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d870f-293">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="d870f-293">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="d870f-294">Linha de negócios da oferta do serviço</span><span class="sxs-lookup"><span data-stu-id="d870f-294">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="d870f-295">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="d870f-295">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d870f-296">OrderID</span><span class="sxs-lookup"><span data-stu-id="d870f-296">OrderID</span></span></td>
<td><p><span data-ttu-id="d870f-297">Identificador exclusivo para um pedido na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d870f-297">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="d870f-298">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="d870f-298">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="d870f-299">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="d870f-299">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d870f-300">ServiceName</span><span class="sxs-lookup"><span data-stu-id="d870f-300">ServiceName</span></span></td>
<td><p><span data-ttu-id="d870f-301">O nome do serviço do Azure em questão.</span><span class="sxs-lookup"><span data-stu-id="d870f-301">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="d870f-302">MÁQUINAS VIRTUAIS</span><span class="sxs-lookup"><span data-stu-id="d870f-302">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d870f-303">ServiceType</span><span class="sxs-lookup"><span data-stu-id="d870f-303">ServiceType</span></span></td>
<td><p><span data-ttu-id="d870f-304">O tipo específico de serviço do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="d870f-304">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="d870f-305">Service Bus – Individual ou pacote</span><span class="sxs-lookup"><span data-stu-id="d870f-305">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="d870f-306">Banco de dados SQL Azure – Edição empresa ou Web</span><span class="sxs-lookup"><span data-stu-id="d870f-306">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d870f-307">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="d870f-307">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="d870f-308">Identificador exclusivo específico de toda a estrutura de serviço de dados e preço.</span><span class="sxs-lookup"><span data-stu-id="d870f-308">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="d870f-309">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="d870f-309">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d870f-310">Nome do recurso</span><span class="sxs-lookup"><span data-stu-id="d870f-310">Resource Name</span></span></td>
<td><p><span data-ttu-id="d870f-311">O nome do recurso do Azure.</span><span class="sxs-lookup"><span data-stu-id="d870f-311">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="d870f-312">Dados de entrada transferidos (GB)</span><span class="sxs-lookup"><span data-stu-id="d870f-312">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="d870f-313">Dados de saída transferidos (GB)</span><span class="sxs-lookup"><span data-stu-id="d870f-313">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d870f-314">Região</span><span class="sxs-lookup"><span data-stu-id="d870f-314">Region</span></span></td>
<td><p><span data-ttu-id="d870f-315">A região a qual o uso se aplica.</span><span class="sxs-lookup"><span data-stu-id="d870f-315">The region the usage applies to.</span></span> <span data-ttu-id="d870f-316">Usado principalmente para atribuir as taxas de transferências de dados, já que as taxas variam de acordo com a região.</span><span class="sxs-lookup"><span data-stu-id="d870f-316">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="d870f-317">Pacífico Asiático, Europa, América Latina e América do Norte</span><span class="sxs-lookup"><span data-stu-id="d870f-317">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d870f-318">SKU</span><span class="sxs-lookup"><span data-stu-id="d870f-318">SKU</span></span></td>
<td><p><span data-ttu-id="d870f-319">Identificador exclusivo MSFT da oferta</span><span class="sxs-lookup"><span data-stu-id="d870f-319">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="d870f-320">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="d870f-320">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="d870f-321">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="d870f-321">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="d870f-322">Uma ID e a quantidade para discriminar as taxas diferentes de um serviço ou recurso em um determinado período de cobrança.</span><span class="sxs-lookup"><span data-stu-id="d870f-322">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="d870f-323">Para a classificação em camadas do Azure, pode haver uma taxa para uma determinada quantidade de unidades faturáveis e uma taxa diferente depois disso.</span><span class="sxs-lookup"><span data-stu-id="d870f-323">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="d870f-324">1</span><span class="sxs-lookup"><span data-stu-id="d870f-324">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d870f-325">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="d870f-325">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="d870f-326">A quantidade de serviço consumida (horas, GB etc.) durante o período de relatório.</span><span class="sxs-lookup"><span data-stu-id="d870f-326">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="d870f-327">Também inclui qualquer uso não cobrado de períodos de relatório anteriores.</span><span class="sxs-lookup"><span data-stu-id="d870f-327">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="d870f-328">11</span><span class="sxs-lookup"><span data-stu-id="d870f-328">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d870f-329">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="d870f-329">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="d870f-330">Unidades incluídas como parte da oferta.</span><span class="sxs-lookup"><span data-stu-id="d870f-330">Units included as part of the offer.</span></span> <span data-ttu-id="d870f-331">Normalmente não está presente no CSP.</span><span class="sxs-lookup"><span data-stu-id="d870f-331">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="d870f-332">0</span><span class="sxs-lookup"><span data-stu-id="d870f-332">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="d870f-333">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="d870f-333">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="d870f-334">Unidades não incluídas como parte da oferta devem ser pagas pelo parceiro.</span><span class="sxs-lookup"><span data-stu-id="d870f-334">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="d870f-335">Igual a ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="d870f-335">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="d870f-336">11</span><span class="sxs-lookup"><span data-stu-id="d870f-336">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d870f-337">ListPrice</span><span class="sxs-lookup"><span data-stu-id="d870f-337">ListPrice</span></span></td>
<td><p><span data-ttu-id="d870f-338">Preço da oferta em vigor na data de início da assinatura.</span><span class="sxs-lookup"><span data-stu-id="d870f-338">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="d870f-339">U$ 0,0808</span><span class="sxs-lookup"><span data-stu-id="d870f-339">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d870f-340">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="d870f-340">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="d870f-341">ListPrist vezes OverageQuantity, arredondado para o centavo mais próximo.</span><span class="sxs-lookup"><span data-stu-id="d870f-341">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="d870f-342">U$ 0,085</span><span class="sxs-lookup"><span data-stu-id="d870f-342">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d870f-343">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="d870f-343">TaxAmount</span></span></td>
<td><p><span data-ttu-id="d870f-344">Valor do imposto cobrado, com base nas regras fiscais do mercado e em circunstâncias específicas.</span><span class="sxs-lookup"><span data-stu-id="d870f-344">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="d870f-345">U$ 0,08</span><span class="sxs-lookup"><span data-stu-id="d870f-345">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d870f-346">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="d870f-346">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="d870f-347">Total após imposto, quando o imposto é aplicável.</span><span class="sxs-lookup"><span data-stu-id="d870f-347">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="d870f-348">U$ 0,93</span><span class="sxs-lookup"><span data-stu-id="d870f-348">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d870f-349">Moeda</span><span class="sxs-lookup"><span data-stu-id="d870f-349">Currency</span></span></td>
<td><p><span data-ttu-id="d870f-350">Tipo de moeda.</span><span class="sxs-lookup"><span data-stu-id="d870f-350">Currency type.</span></span> <span data-ttu-id="d870f-351">Cada entidade de cobrança tem somente uma moeda.</span><span class="sxs-lookup"><span data-stu-id="d870f-351">Each billing entity has only one currency.</span></span> <span data-ttu-id="d870f-352">Verifique se isso coincide com a primeira fatura e faça o mesmo após grandes atualizações na plataforma de cobrança.</span><span class="sxs-lookup"><span data-stu-id="d870f-352">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="d870f-353">Euro</span><span class="sxs-lookup"><span data-stu-id="d870f-353">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d870f-354">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="d870f-354">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="d870f-355">Preço por unidade sem imposto.</span><span class="sxs-lookup"><span data-stu-id="d870f-355">Pretax price per unit.</span></span> <span data-ttu-id="d870f-356">Igual a PretaxCharges / OverageQuantity, arredondado para o centavo mais próximo.</span><span class="sxs-lookup"><span data-stu-id="d870f-356">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="d870f-357">U$ 0,08</span><span class="sxs-lookup"><span data-stu-id="d870f-357">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d870f-358">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="d870f-358">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="d870f-359">Preço pós-imposto por unidade.</span><span class="sxs-lookup"><span data-stu-id="d870f-359">Post tax price per unit.</span></span> <span data-ttu-id="d870f-360">Igual a PostTaxTotal / OverageQuantity, ou PretaxEffectiveRate + taxa de imposto por valor de unidade, arredondado para o centavo mais próximo.</span><span class="sxs-lookup"><span data-stu-id="d870f-360">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="d870f-361">U$ 0,08</span><span class="sxs-lookup"><span data-stu-id="d870f-361">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d870f-362">ChargeType</span><span class="sxs-lookup"><span data-stu-id="d870f-362">ChargeType</span></span></td>
<td><p><span data-ttu-id="d870f-363">O tipo de encargo ou ajuste.</span><span class="sxs-lookup"><span data-stu-id="d870f-363">The type of charge or adjustment.</span></span> <span data-ttu-id="d870f-364">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="d870f-364">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="d870f-365">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="d870f-365">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d870f-366">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="d870f-366">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="d870f-367">ID exclusiva da conta na plataforma de cobrança da MSFT.</span><span class="sxs-lookup"><span data-stu-id="d870f-367">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="d870f-368">1280018095</span><span class="sxs-lookup"><span data-stu-id="d870f-368">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d870f-369">UsageDate</span><span class="sxs-lookup"><span data-stu-id="d870f-369">UsageDate</span></span></td>
<td><p><span data-ttu-id="d870f-370">Data da implantação do serviço.</span><span class="sxs-lookup"><span data-stu-id="d870f-370">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="d870f-371">1/2/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="d870f-371">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d870f-372">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="d870f-372">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="d870f-373">Essa coluna identifica a localização de um data center dentro da região para serviços onde isso é aplicável e preenchido.</span><span class="sxs-lookup"><span data-stu-id="d870f-373">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="d870f-374">Leste da Ásia, Sudeste da Ásia, Norte da Europa, Europa Ocidental, Centro Norte e Centro Sul dos EUA</span><span class="sxs-lookup"><span data-stu-id="d870f-374">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d870f-375">MeteredService</span><span class="sxs-lookup"><span data-stu-id="d870f-375">MeteredService</span></span></td>
<td><p><span data-ttu-id="d870f-376">Essa coluna é utilizada para rastrear o serviço do Microsoft Azure individual que não pode ser identificado especificamente na coluna Nome do Serviço.</span><span class="sxs-lookup"><span data-stu-id="d870f-376">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="d870f-377">Por exemplo, transferências de dados são relatadas como &quot;Microsoft Azure – Todos os Serviços&quot; na coluna Nome do Serviço.</span><span class="sxs-lookup"><span data-stu-id="d870f-377">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="d870f-378">Essa coluna MeteredService indicará ao qual serviço específico o uso pertence.</span><span class="sxs-lookup"><span data-stu-id="d870f-378">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="d870f-379">AccessControl, CDN, Computação, Banco de dados, ServiceBus, Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d870f-379">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d870f-380">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="d870f-380">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="d870f-381">Um subcabeçalho que esclarece ainda mais o serviço Microsoft Azure individual além do nível fornecido pelo campo MeteredService.</span><span class="sxs-lookup"><span data-stu-id="d870f-381">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="d870f-382">EXTERNO</span><span class="sxs-lookup"><span data-stu-id="d870f-382">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d870f-383">Projeto</span><span class="sxs-lookup"><span data-stu-id="d870f-383">Project</span></span></td>
<td><p><span data-ttu-id="d870f-384">Nome definido pelo cliente para a instância do serviço</span><span class="sxs-lookup"><span data-stu-id="d870f-384">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="d870f-385">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="d870f-385">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d870f-386">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="d870f-386">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="d870f-387">O número de conexões ServiceBus que foram provisionados e utilizados em um dia específico.</span><span class="sxs-lookup"><span data-stu-id="d870f-387">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="d870f-388">Por exemplo: se você tivesse uma conexão individualmente provisionada durante um mês de 30 dias, a coluna Informação do Serviço 1 lerá "1,000000 conexões/30 dias".</span><span class="sxs-lookup"><span data-stu-id="d870f-388">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="d870f-389">Se você tinha um pacote de 25 conexões ServiceBus provisionadas e você utilizou 1 durante o dia, sua declaração de uso diário para esse dia indicaria "25 conexões/30 dias – Usado: 1,000000".</span><span class="sxs-lookup"><span data-stu-id="d870f-389">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d870f-390">CustomerID</span><span class="sxs-lookup"><span data-stu-id="d870f-390">CustomerID</span></span></td>
<td><p><span data-ttu-id="d870f-391">ID exclusiva da Microsoft, no formato GUID, usada para identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="d870f-391">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="d870f-392">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="d870f-392">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d870f-393">DomainName</span><span class="sxs-lookup"><span data-stu-id="d870f-393">DomainName</span></span></td>
<td><p><span data-ttu-id="d870f-394">Nome de domínio do cliente, usado para ajudar a identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="d870f-394">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="d870f-395">Este campo pode aparecer em branco até o segundo ciclo de cobrança.</span><span class="sxs-lookup"><span data-stu-id="d870f-395">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="d870f-396">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="d870f-396">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="d870f-397">Unidade</span><span class="sxs-lookup"><span data-stu-id="d870f-397">Unit</span></span></td>
<td><p><span data-ttu-id="d870f-398">A unidade do nome do recurso</span><span class="sxs-lookup"><span data-stu-id="d870f-398">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="d870f-399">GB ou HORAS</span><span class="sxs-lookup"><span data-stu-id="d870f-399">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="onetimefiles"></a><span data-ttu-id="d870f-400">Campos de arquivo de compra única</span><span class="sxs-lookup"><span data-stu-id="d870f-400">One-time purchase file fields</span></span>

|**<span data-ttu-id="d870f-401">Campo</span><span class="sxs-lookup"><span data-stu-id="d870f-401">Field</span></span>** |**<span data-ttu-id="d870f-402">Definição</span><span class="sxs-lookup"><span data-stu-id="d870f-402">Definition</span></span>**|
|:----------------|:-----------------------------|
|<span data-ttu-id="d870f-403">PartnerId</span><span class="sxs-lookup"><span data-stu-id="d870f-403">PartnerId</span></span> |<span data-ttu-id="d870f-404">ID do parceiro, no formato GUID.</span><span class="sxs-lookup"><span data-stu-id="d870f-404">Partner ID, in GUID format.</span></span> |
|<span data-ttu-id="d870f-405">CustomerID</span><span class="sxs-lookup"><span data-stu-id="d870f-405">CustomerId</span></span> |<span data-ttu-id="d870f-406">ID exclusiva da Microsoft, no formato GUID, usada para identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="d870f-406">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span> |
|<span data-ttu-id="d870f-407">CustomerName</span><span class="sxs-lookup"><span data-stu-id="d870f-407">CustomerName</span></span> |<span data-ttu-id="d870f-408">Nome da organização do cliente como informado no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="d870f-408">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="d870f-409">Isso é muito importante para reconciliar a fatura com as informações de seu sistema.</span><span class="sxs-lookup"><span data-stu-id="d870f-409">This is very important for reconciling the invoice with your system information.</span></span> |
|<span data-ttu-id="d870f-410">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="d870f-410">CustomerDomainName</span></span> |<span data-ttu-id="d870f-411">O nome de domínio do cliente.</span><span class="sxs-lookup"><span data-stu-id="d870f-411">The customer’s domain name.</span></span> |
|<span data-ttu-id="d870f-412">CustomerCountry</span><span class="sxs-lookup"><span data-stu-id="d870f-412">CustomerCountry</span></span> |<span data-ttu-id="d870f-413">O país em que o cliente está localizado.</span><span class="sxs-lookup"><span data-stu-id="d870f-413">The country in which the customer is located.</span></span> |
|<span data-ttu-id="d870f-414">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="d870f-414">InvoiceNumber</span></span> |<span data-ttu-id="d870f-415">Número da fatura na qual a transação especificada é exibida.</span><span class="sxs-lookup"><span data-stu-id="d870f-415">Invoice number where the specified transaction appears.</span></span> |
|<span data-ttu-id="d870f-416">MpnId</span><span class="sxs-lookup"><span data-stu-id="d870f-416">MpnId</span></span> |<span data-ttu-id="d870f-417">ID do MPN do parceiro CSP (direto ou indireto).</span><span class="sxs-lookup"><span data-stu-id="d870f-417">MPN ID of the CSP partner (direct or indirect).</span></span> |
|<span data-ttu-id="d870f-418">ID do MPN do revendedor</span><span class="sxs-lookup"><span data-stu-id="d870f-418">Reseller MPN ID</span></span> |<span data-ttu-id="d870f-419">Só aparece em arquivos de reconciliação para parceiros no modelo indireto.</span><span class="sxs-lookup"><span data-stu-id="d870f-419">Only appears on reconciliation files for partners in the indirect model.</span></span> <span data-ttu-id="d870f-420">A ID do MPN do revendedor de registro da reserva.</span><span class="sxs-lookup"><span data-stu-id="d870f-420">The MPN ID of the reseller of record for the reservation.</span></span> <span data-ttu-id="d870f-421">Isso corresponde à ID de revendedor listada para a reserva específica no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="d870f-421">This corresponds to the reseller ID listed for the specific reservation in Partner Center.</span></span> <span data-ttu-id="d870f-422">Se um parceiro CSP vendeu a reserva diretamente para o cliente, sua ID do MPN estará listada duas vezes, como a ID do MPN e a ID do MPN do revendedor.</span><span class="sxs-lookup"><span data-stu-id="d870f-422">If a CSP partner sold the reservation directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span> <span data-ttu-id="d870f-423">Se um parceiro CSP tiver um revendedor sem ID do MPN, esse valor será definido como a ID do MPN do parceiro.</span><span class="sxs-lookup"><span data-stu-id="d870f-423">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span> <span data-ttu-id="d870f-424">Se o parceiro CSP remover uma ID de revendedor, esse valor será definido como -1.</span><span class="sxs-lookup"><span data-stu-id="d870f-424">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span> |
|<span data-ttu-id="d870f-425">OrderId</span><span class="sxs-lookup"><span data-stu-id="d870f-425">OrderId</span></span> |<span data-ttu-id="d870f-426">Identificador exclusivo para um pedido na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d870f-426">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="d870f-427">Pode ser útil para identificar a reserva do Azure ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="d870f-427">May be useful to identify the Azure reservation when contacting support but not for reconciliation.</span></span> |
|<span data-ttu-id="d870f-428">OrderDate</span><span class="sxs-lookup"><span data-stu-id="d870f-428">OrderDate</span></span> |<span data-ttu-id="d870f-429">A data em que o pedido foi feito.</span><span class="sxs-lookup"><span data-stu-id="d870f-429">The date the order was placed.</span></span> |
|<span data-ttu-id="d870f-430">ProductId</span><span class="sxs-lookup"><span data-stu-id="d870f-430">ProductId</span></span> |<span data-ttu-id="d870f-431">A ID do produto.</span><span class="sxs-lookup"><span data-stu-id="d870f-431">The ID for the product.</span></span> |
|<span data-ttu-id="d870f-432">SkuId</span><span class="sxs-lookup"><span data-stu-id="d870f-432">SkuId</span></span>  |<span data-ttu-id="d870f-433">A ID de uma SKU em particular.</span><span class="sxs-lookup"><span data-stu-id="d870f-433">The ID for a particular SKU.</span></span> |
|<span data-ttu-id="d870f-434">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="d870f-434">AvailabilityId</span></span> |<span data-ttu-id="d870f-435">A ID de uma Disponibilidade em particular.</span><span class="sxs-lookup"><span data-stu-id="d870f-435">The ID for a particular Availability.</span></span> <span data-ttu-id="d870f-436">"Disponibilidade" refere-se a se uma SKU em particular está disponível ou não para compra para determinado país, moeda, segmento do setor etc.</span><span class="sxs-lookup"><span data-stu-id="d870f-436">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span> |
|<span data-ttu-id="d870f-437">SkuName</span><span class="sxs-lookup"><span data-stu-id="d870f-437">SkuName</span></span>  |<span data-ttu-id="d870f-438">O título de uma SKU em particular.</span><span class="sxs-lookup"><span data-stu-id="d870f-438">The title for a particular SKU.</span></span> |
|<span data-ttu-id="d870f-439">ProductName</span><span class="sxs-lookup"><span data-stu-id="d870f-439">ProductName</span></span> |<span data-ttu-id="d870f-440">O nome do produto.</span><span class="sxs-lookup"><span data-stu-id="d870f-440">The name of the product.</span></span> |
|<span data-ttu-id="d870f-441">ChargeType</span><span class="sxs-lookup"><span data-stu-id="d870f-441">ChargeType</span></span> |<span data-ttu-id="d870f-442">O tipo de encargo ou ajuste.</span><span class="sxs-lookup"><span data-stu-id="d870f-442">The type of charge or adjustment.</span></span> |
|<span data-ttu-id="d870f-443">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="d870f-443">UnitPrice</span></span> |<span data-ttu-id="d870f-444">Preço por produto pedido.</span><span class="sxs-lookup"><span data-stu-id="d870f-444">Price per product ordered.</span></span> |
|<span data-ttu-id="d870f-445">Quantidade</span><span class="sxs-lookup"><span data-stu-id="d870f-445">Quantity</span></span> |<span data-ttu-id="d870f-446">Número de produtos pedidos.</span><span class="sxs-lookup"><span data-stu-id="d870f-446">Number of products ordered.</span></span> |
|<span data-ttu-id="d870f-447">Subtotal</span><span class="sxs-lookup"><span data-stu-id="d870f-447">Subtotal</span></span> |<span data-ttu-id="d870f-448">Total sem imposto.</span><span class="sxs-lookup"><span data-stu-id="d870f-448">Total before tax.</span></span> <span data-ttu-id="d870f-449">Verifica se seu subtotal corresponde ao total esperado, em caso de desconto.</span><span class="sxs-lookup"><span data-stu-id="d870f-449">Checks that your subtotal matches your expected total, in case of a discount.</span></span> |
|<span data-ttu-id="d870f-450">TaxTotal</span><span class="sxs-lookup"><span data-stu-id="d870f-450">TaxTotal</span></span> |<span data-ttu-id="d870f-451">O total de todos os impostos aplicáveis.</span><span class="sxs-lookup"><span data-stu-id="d870f-451">The total of all applicable taxes.</span></span> |
|<span data-ttu-id="d870f-452">Total</span><span class="sxs-lookup"><span data-stu-id="d870f-452">Total</span></span> |<span data-ttu-id="d870f-453">O valor total desta compra.</span><span class="sxs-lookup"><span data-stu-id="d870f-453">The total amount of this purchase.</span></span> |
|<span data-ttu-id="d870f-454">Moeda</span><span class="sxs-lookup"><span data-stu-id="d870f-454">Currency</span></span> |<span data-ttu-id="d870f-455">Tipo de moeda.</span><span class="sxs-lookup"><span data-stu-id="d870f-455">Currency type.</span></span> <span data-ttu-id="d870f-456">Cada entidade de cobrança tem somente uma moeda.</span><span class="sxs-lookup"><span data-stu-id="d870f-456">Each billing entity has only one currency.</span></span> <span data-ttu-id="d870f-457">Verifique se isso coincide com a primeira fatura e faça o mesmo após grandes atualizações na plataforma de cobrança.</span><span class="sxs-lookup"><span data-stu-id="d870f-457">Check that it matches your first invoice and then after any major billing platform update.</span></span> |
|<span data-ttu-id="d870f-458">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="d870f-458">DiscountDetails</span></span> |<span data-ttu-id="d870f-459">Lista detalhada dos descontos relevantes.</span><span class="sxs-lookup"><span data-stu-id="d870f-459">Detailed listing of any relevant discounts.</span></span> |



## <a href="" id="charge_types"></a><span data-ttu-id="d870f-460">Como mapear encargos entre uma fatura e o arquivo de reconciliação</span><span class="sxs-lookup"><span data-stu-id="d870f-460">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="d870f-461">Sua fatura fornece um resumo dos encargos, enquanto seu arquivo de reconciliação fornece uma divisão detalhada das transações de item de linha, incluindo os tipos de carga.</span><span class="sxs-lookup"><span data-stu-id="d870f-461">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="d870f-462">Para fazer referência cruzada das quantidades de carga entre o arquivo de reconciliação e fatura, você pode usar opções de filtro do Microsoft Excel para filtrar por tipos de cobrança no arquivo de reconciliação para mapear os encargos de fatura em um conjunto de detalhamentos de cobrança no arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="d870f-462">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="d870f-463">Os arquivos de reconciliação, tanto os baseados em licença quanto os baseados em uso, mostram apenas encargos e transações relacionadas ao uso (unidades consumidas e encargos relacionados).</span><span class="sxs-lookup"><span data-stu-id="d870f-463">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="d870f-464">Créditos únicos, descontos ou reembolsos que aparecem na fatura como "Ajustes" não são mostrados no arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="d870f-464">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="d870f-465">A tabela a seguir mostra os mapeamentos entre uma seção da fatura e os tipos de encargo associados que podem aparecer nos arquivos de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="d870f-465">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><strong><span data-ttu-id="d870f-466">Descrição do encargo da fatura</span><span class="sxs-lookup"><span data-stu-id="d870f-466">Invoice charge description</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="d870f-467">Descrição do encargo do arquivo de reconciliação (coluna ChargeType)</span><span class="sxs-lookup"><span data-stu-id="d870f-467">Reconciliation file charge description (ChargeType column)</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="d870f-468">O que é este encargo?</span><span class="sxs-lookup"><span data-stu-id="d870f-468">What is this charge?</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="d870f-469">Como é possível mapear esses tipos de encargo na fatura?</span><span class="sxs-lookup"><span data-stu-id="d870f-469">How do I map these ChargeTypes to the invoice?</span></span></strong></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><strong><span data-ttu-id="d870f-470">Encargos baseadas em licença</span><span class="sxs-lookup"><span data-stu-id="d870f-470">License-based charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="d870f-471">Taxa de ativação</span><span class="sxs-lookup"><span data-stu-id="d870f-471">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="d870f-472">O valor cobrado do cliente quando ele usa a assinatura depois de comprá-la.</span><span class="sxs-lookup"><span data-stu-id="d870f-472">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="d870f-473">No arquivo baseado em licença, some a coluna <strong>Quantidade</strong></span><span class="sxs-lookup"><span data-stu-id="d870f-473">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="d870f-474">Taxa de cancelamento</span><span class="sxs-lookup"><span data-stu-id="d870f-474">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="d870f-475">Os encargos proporcionais reembolsados para o cliente quando os assentos associados são alterados</span><span class="sxs-lookup"><span data-stu-id="d870f-475">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="d870f-476">Taxa do ciclo</span><span class="sxs-lookup"><span data-stu-id="d870f-476">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="d870f-477">Encargos periódicos de uma assinatura</span><span class="sxs-lookup"><span data-stu-id="d870f-477">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="d870f-478">Percorrer ocorrência proporcional</span><span class="sxs-lookup"><span data-stu-id="d870f-478">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="d870f-479">Os encargos proporcionais cobrados do cliente quando os assentos associados são alterados</span><span class="sxs-lookup"><span data-stu-id="d870f-479">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="d870f-480">Taxas proporcionais durante o cancelamento</span><span class="sxs-lookup"><span data-stu-id="d870f-480">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="d870f-481">Reembolso proporcional para a parte não utilizada do serviço após o cancelamento</span><span class="sxs-lookup"><span data-stu-id="d870f-481">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="d870f-482">Taxas proporcionais durante a compra</span><span class="sxs-lookup"><span data-stu-id="d870f-482">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="d870f-483">Taxas proporcionais após a compra</span><span class="sxs-lookup"><span data-stu-id="d870f-483">Prorated fees upon purchase</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="d870f-484">Taxa de compra</span><span class="sxs-lookup"><span data-stu-id="d870f-484">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="d870f-485">Encargo inicial de uma assinatura</span><span class="sxs-lookup"><span data-stu-id="d870f-485">Initial charge for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="d870f-486">Taxa proporcional ao renovar</span><span class="sxs-lookup"><span data-stu-id="d870f-486">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="d870f-487">Taxas proporcionais após a renovação da assinatura</span><span class="sxs-lookup"><span data-stu-id="d870f-487">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="d870f-488">Taxa de renovação</span><span class="sxs-lookup"><span data-stu-id="d870f-488">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="d870f-489">Cobrança para renovação de uma assinatura</span><span class="sxs-lookup"><span data-stu-id="d870f-489">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="d870f-490">Taxas proporcionais ao ativar</span><span class="sxs-lookup"><span data-stu-id="d870f-490">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="d870f-491">Taxas proporcionais da ativação até o final do período de cobrança</span><span class="sxs-lookup"><span data-stu-id="d870f-491">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong><span data-ttu-id="d870f-492">Tarifas de uso</span><span class="sxs-lookup"><span data-stu-id="d870f-492">Usage Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="d870f-493">Avaliar a taxa de uso ao cancelar</span><span class="sxs-lookup"><span data-stu-id="d870f-493">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="d870f-494">Taxa de uso de acesso com o cancelamento para uso não pago durante o período de cobrança atual</span><span class="sxs-lookup"><span data-stu-id="d870f-494">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="d870f-495">No arquivo baseado em uso, some a coluna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="d870f-495">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="d870f-496">Avalie a taxa de uso para o ciclo atual</span><span class="sxs-lookup"><span data-stu-id="d870f-496">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="d870f-497">Taxa de uso de acesso para o período atual de cobrança</span><span class="sxs-lookup"><span data-stu-id="d870f-497">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="d870f-498">Créditos</span><span class="sxs-lookup"><span data-stu-id="d870f-498">Credits</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="d870f-499">Deslocando um item de linha</span><span class="sxs-lookup"><span data-stu-id="d870f-499">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="d870f-500">Reembolso parcial ou integral para um item de linha, incluindo os impostos</span><span class="sxs-lookup"><span data-stu-id="d870f-500">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="d870f-501">No arquivo baseado em licença, some a coluna <strong>TotalForCustomer</strong></span><span class="sxs-lookup"><span data-stu-id="d870f-501">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="d870f-502">No arquivo baseado em uso, some a coluna <strong>PostTaxTotal</strong></span><span class="sxs-lookup"><span data-stu-id="d870f-502">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><strong><span data-ttu-id="d870f-503">Descontos baseados em uso</span><span class="sxs-lookup"><span data-stu-id="d870f-503">Usage-based discounts</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="d870f-504">Desconto de ativação</span><span class="sxs-lookup"><span data-stu-id="d870f-504">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="d870f-505">Desconto aplicado quando a assinatura é ativada</span><span class="sxs-lookup"><span data-stu-id="d870f-505">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="d870f-506">No arquivo baseado em uso, some a coluna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="d870f-506">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="d870f-507">Desconto de ciclo</span><span class="sxs-lookup"><span data-stu-id="d870f-507">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="d870f-508">Desconto aplicado em cobranças periódicas</span><span class="sxs-lookup"><span data-stu-id="d870f-508">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="d870f-509">Desconto de renovação</span><span class="sxs-lookup"><span data-stu-id="d870f-509">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="d870f-510">Desconto aplicado quando a assinatura é renovada</span><span class="sxs-lookup"><span data-stu-id="d870f-510">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="d870f-511">Desconto de cancelamento</span><span class="sxs-lookup"><span data-stu-id="d870f-511">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="d870f-512">Encargos aplicados quando descontos são cancelados</span><span class="sxs-lookup"><span data-stu-id="d870f-512">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><strong><span data-ttu-id="d870f-513">Descontos baseados em licença</span><span class="sxs-lookup"><span data-stu-id="d870f-513">License-based discounts</span></span></strong></p>
</td>
<td>
<p><em><span data-ttu-id="d870f-514">Podem ser aplicados a vários tipos de cobrança</span><span class="sxs-lookup"><span data-stu-id="d870f-514">May be applied to multiple charge types</span></span></em></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="d870f-515">No arquivo baseado em licença, some a coluna <strong>TotalOtherDiscount</strong></span><span class="sxs-lookup"><span data-stu-id="d870f-515">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="d870f-516"><strong>Impostos</strong>&nbsp;ou&nbsp;<strong>IVA</strong></span><span class="sxs-lookup"><span data-stu-id="d870f-516"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><em><span data-ttu-id="d870f-517">Podem ser aplicados a vários tipos de cobrança</span><span class="sxs-lookup"><span data-stu-id="d870f-517">May be applied to multiple charge types</span></span></em></p>
<p><em><span data-ttu-id="d870f-518">Exceção: "Deslocamento de um item de linha" já inclui impostos.</span><span class="sxs-lookup"><span data-stu-id="d870f-518">Exception: "Offset a line item" already includes taxes.</span></span> <span data-ttu-id="d870f-519">Consulte créditos, acima.</span><span class="sxs-lookup"><span data-stu-id="d870f-519">See Credits, above.</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="d870f-520">Impostos ou impostos sobre valor agregado (IVA)</span><span class="sxs-lookup"><span data-stu-id="d870f-520">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="d870f-521">No arquivo baseado em licença, some a coluna <strong>Imposto</strong></span><span class="sxs-lookup"><span data-stu-id="d870f-521">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="d870f-522">No arquivo baseado em uso, some a coluna <strong>TaxAmount</strong></span><span class="sxs-lookup"><span data-stu-id="d870f-522">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
