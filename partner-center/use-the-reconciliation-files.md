---
title: Usar os arquivos de reconciliação | Partner Center
ms.topic: article
ms.date: 10/29/2018
description: Para uma exibição detalhada do item de linha de cada encargo em um ciclo de cobrança, baixe os arquivos de reconciliação do Partner Center.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: KPacquer
ms.author: kenpacq
ms.localizationpriority: medium
ms.openlocfilehash: 50af14ab0e8edf6cd4576be6615cd7238b23bd99
ms.sourcegitcommit: 9ea2f05f938ea22251f3719b61f03ccb71d3494f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/03/2019
ms.locfileid: "8990988"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="20e3d-103">Usar os arquivos de reconciliação</span><span class="sxs-lookup"><span data-stu-id="20e3d-103">Use the reconciliation files</span></span>

**<span data-ttu-id="20e3d-104">Aplicável a</span><span class="sxs-lookup"><span data-stu-id="20e3d-104">Applies to</span></span>**

-  <span data-ttu-id="20e3d-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="20e3d-105">Partner Center</span></span>
-  <span data-ttu-id="20e3d-106">Partner Center for Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="20e3d-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="20e3d-107">Para uma exibição detalhada do item de linha de cada encargo em um ciclo de cobrança, baixe os arquivos de reconciliação do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="20e3d-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="20e3d-108">Os detalhes incluem encargos por assinaturas de cada cliente e eventos detalhados (como a adição de assentos a uma assinatura no meio do período).</span><span class="sxs-lookup"><span data-stu-id="20e3d-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="20e3d-109">Discriminar por parceiro</span><span class="sxs-lookup"><span data-stu-id="20e3d-109">Itemize by partner</span></span>


<span data-ttu-id="20e3d-110">Os parceiros no modelo indireto podem usar esses campos adicionais nos arquivos de reconciliação baseados em uso e em licença para discriminar por revendedor.</span><span class="sxs-lookup"><span data-stu-id="20e3d-110">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="20e3d-111">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="20e3d-111">MPN ID</span></span></th>
<th><span data-ttu-id="20e3d-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="20e3d-112">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="20e3d-113">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="20e3d-113">MPN ID</span></span></td>
<td><p><span data-ttu-id="20e3d-114">A ID do Microsoft Partner Network (MPN) do parceiro CSP (direta ou indireta).</span><span class="sxs-lookup"><span data-stu-id="20e3d-114">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e3d-115">ID do MPN do revendedor</span><span class="sxs-lookup"><span data-stu-id="20e3d-115">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="20e3d-116">Só aparece em arquivos de reconciliação para parceiros no modelo indireto.</span><span class="sxs-lookup"><span data-stu-id="20e3d-116">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="20e3d-117">A ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="20e3d-117">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="20e3d-118">Isso corresponde à ID de revendedor listada para a assinatura específica no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="20e3d-118">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="20e3d-119">Para exibir ou atualizar o revendedor, no menu Partner Center, selecione <strong>clientes</strong>e, em seguida, escolha o cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="20e3d-119">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="20e3d-120">No menu do cliente, selecione <strong>Assinaturas</strong>, escolha a assinatura na lista.</span><span class="sxs-lookup"><span data-stu-id="20e3d-120">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="20e3d-121">Selecione <strong>Atualizar</strong> para alterar o <strong>Revendedor (ID do MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="20e3d-121">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="20e3d-122">Se um parceiro CSP vendeu a assinatura diretamente para o cliente, sua ID do MPN estará listada duas vezes, como a ID do MPN e a ID do MPN do revendedor.</span><span class="sxs-lookup"><span data-stu-id="20e3d-122">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="20e3d-123">Se um parceiro CSP tiver um revendedor sem ID do MPN, esse valor será definido como a ID do MPN do parceiro.</span><span class="sxs-lookup"><span data-stu-id="20e3d-123">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="20e3d-124">Se o parceiro CSP remover uma ID de revendedor, esse valor será definido como -1.</span><span class="sxs-lookup"><span data-stu-id="20e3d-124">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="20e3d-125">Campos de arquivos baseado em licença</span><span class="sxs-lookup"><span data-stu-id="20e3d-125">License-based file fields</span></span>


<span data-ttu-id="20e3d-126">Para reconciliar seus encargos com os pedidos de seu cliente, compare o campo Syndication\_Partner\_Subscription\_Number do arquivo de reconciliação com a ID de Assinatura do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="20e3d-126">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="20e3d-127">Coluna</span><span class="sxs-lookup"><span data-stu-id="20e3d-127">Column</span></span></strong></td>
<td><strong><span data-ttu-id="20e3d-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="20e3d-128">Description</span></span></strong></td>
<td><strong><span data-ttu-id="20e3d-129">Valor de exemplo</span><span class="sxs-lookup"><span data-stu-id="20e3d-129">Sample Value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e3d-130">PartnerId</span><span class="sxs-lookup"><span data-stu-id="20e3d-130">PartnerId</span></span></td>
<td><p><span data-ttu-id="20e3d-131">Identificador exclusivo de uma entidade de cobrança específica, em formato GUID.</span><span class="sxs-lookup"><span data-stu-id="20e3d-131">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="20e3d-132">Não é necessário para reconciliação, mas pode ser uma informação útil.</span><span class="sxs-lookup"><span data-stu-id="20e3d-132">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="20e3d-133">O mesmo em todas as linhas.</span><span class="sxs-lookup"><span data-stu-id="20e3d-133">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="20e3d-134">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="20e3d-134">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e3d-135">CustomerID</span><span class="sxs-lookup"><span data-stu-id="20e3d-135">CustomerID</span></span></td>
<td><p><span data-ttu-id="20e3d-136">ID exclusiva da Microsoft, no formato GUID, usada para identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="20e3d-136">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="20e3d-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="20e3d-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e3d-138">OrderID</span><span class="sxs-lookup"><span data-stu-id="20e3d-138">OrderID</span></span></td>
<td><p><span data-ttu-id="20e3d-139">Identificador exclusivo para um pedido na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="20e3d-139">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="20e3d-140">Pode ser útil para identificar o pedido ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="20e3d-140">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="20e3d-141">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="20e3d-141">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e3d-142">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="20e3d-142">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="20e3d-143">Identificador exclusivo de uma assinatura na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="20e3d-143">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="20e3d-144">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="20e3d-144">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="20e3d-145">Esse não é o mesmo que o ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="20e3d-145">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="20e3d-146">Consulte Número_Assinatura_Parceiro_Sindicalização.</span><span class="sxs-lookup"><span data-stu-id="20e3d-146">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="20e3d-147">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="20e3d-147">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e3d-148">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="20e3d-148">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="20e3d-149">Identificador exclusivo para assinaturas.</span><span class="sxs-lookup"><span data-stu-id="20e3d-149">Unique identifier for subscriptions.</span></span> <span data-ttu-id="20e3d-150">Target: Um cliente pode ter várias assinaturas para o mesmo plano, portanto, isso é importante para análise de arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="20e3d-150">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="20e3d-151">Esse campo é mapeado para a ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="20e3d-151">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="20e3d-152">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="20e3d-152">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e3d-153">OfferID</span><span class="sxs-lookup"><span data-stu-id="20e3d-153">OfferID</span></span></td>
<td><p><span data-ttu-id="20e3d-154">ID exclusivo da oferta.</span><span class="sxs-lookup"><span data-stu-id="20e3d-154">Unique offer ID.</span></span> <span data-ttu-id="20e3d-155">ID padrão da oferta de acordo com a lista de preços.</span><span class="sxs-lookup"><span data-stu-id="20e3d-155">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="20e3d-156"><b>Observação</b>: esse valor não coincide com a ID de oferta da lista de preços.</span><span class="sxs-lookup"><span data-stu-id="20e3d-156"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="20e3d-157">Veja DurableOfferID abaixo.</span><span class="sxs-lookup"><span data-stu-id="20e3d-157">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="20e3d-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="20e3d-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e3d-159">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="20e3d-159">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="20e3d-160">ID exclusiva da oferta durável, conforme definido na tabela de preços.</span><span class="sxs-lookup"><span data-stu-id="20e3d-160">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="20e3d-161"><b>Observação</b>: esse valor corresponde à ID de oferta da lista de preços.</span><span class="sxs-lookup"><span data-stu-id="20e3d-161"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="20e3d-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="20e3d-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e3d-163">OfferName</span><span class="sxs-lookup"><span data-stu-id="20e3d-163">OfferName</span></span></td>
<td><p><span data-ttu-id="20e3d-164">O nome da oferta de serviço comprada pelo cliente, conforme definido na tabela de preços.</span><span class="sxs-lookup"><span data-stu-id="20e3d-164">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="20e3d-165">Microsoft Office 365 (plano E3)</span><span class="sxs-lookup"><span data-stu-id="20e3d-165">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e3d-166">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="20e3d-166">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="20e3d-167">A data de início da assinatura, definida como um dia após o pedido ser enviado.</span><span class="sxs-lookup"><span data-stu-id="20e3d-167">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="20e3d-168">Verificando a data de início da assinatura em conjunto com a data de término, você pode determinar se o cliente está dentro do primeiro ano da assinatura ou se a assinatura foi renovada para o ano seguinte.</span><span class="sxs-lookup"><span data-stu-id="20e3d-168">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="20e3d-169">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="20e3d-169">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="20e3d-170">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="20e3d-170">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e3d-171">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="20e3d-171">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="20e3d-172">A data do término da assinatura: 12 meses + x dias após a data de início (para se alinhar com a data de cobrança do parceiro) ou 12 meses a partir da data de renovação.</span><span class="sxs-lookup"><span data-stu-id="20e3d-172">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="20e3d-173">Na renovação, os preços são atualizados com a tabela de preços atual.</span><span class="sxs-lookup"><span data-stu-id="20e3d-173">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="20e3d-174">Um comunicado ao cliente pode ser necessário antes da renovação automática.</span><span class="sxs-lookup"><span data-stu-id="20e3d-174">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="20e3d-175">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="20e3d-175">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="20e3d-176">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="20e3d-176">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e3d-177">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="20e3d-177">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="20e3d-178">Dia de início dos encargos.</span><span class="sxs-lookup"><span data-stu-id="20e3d-178">Start day of the charges.</span></span></p>
<p><span data-ttu-id="20e3d-179">Quando o cliente muda o número de assentos, esse número é usado para calcular os encargos por dia (pro-rata).</span><span class="sxs-lookup"><span data-stu-id="20e3d-179">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="20e3d-180">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="20e3d-180">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="20e3d-181">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="20e3d-181">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e3d-182">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="20e3d-182">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="20e3d-183">Dia do término dos encargos.</span><span class="sxs-lookup"><span data-stu-id="20e3d-183">End day of the charges.</span></span></p>
<p><span data-ttu-id="20e3d-184">Quando o cliente muda o número de assentos, esse número é usado para calcular os encargos por dia (pro-rata).</span><span class="sxs-lookup"><span data-stu-id="20e3d-184">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="20e3d-185">A hora é sempre o fim do dia, 23:59.</span><span class="sxs-lookup"><span data-stu-id="20e3d-185">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="20e3d-186">28/2/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="20e3d-186">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e3d-187">ChargeType</span><span class="sxs-lookup"><span data-stu-id="20e3d-187">ChargeType</span></span></td>
<td><p><span data-ttu-id="20e3d-188">O tipo de encargo ou ajuste.</span><span class="sxs-lookup"><span data-stu-id="20e3d-188">The type of charge or adjustment.</span></span> <span data-ttu-id="20e3d-189">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="20e3d-189">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="20e3d-190">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="20e3d-190">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e3d-191">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="20e3d-191">UnitPrice</span></span></td>
<td><p><span data-ttu-id="20e3d-192">Preço por estação, conforme publicado na lista de preços no momento da compra.</span><span class="sxs-lookup"><span data-stu-id="20e3d-192">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="20e3d-193">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="20e3d-193">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="20e3d-194">6.82</span><span class="sxs-lookup"><span data-stu-id="20e3d-194">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e3d-195">Quantity</span><span class="sxs-lookup"><span data-stu-id="20e3d-195">Quantity</span></span></td>
<td><p><span data-ttu-id="20e3d-196">Número de assentos.</span><span class="sxs-lookup"><span data-stu-id="20e3d-196">Number of seats.</span></span> <span data-ttu-id="20e3d-197">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="20e3d-197">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="20e3d-198">2</span><span class="sxs-lookup"><span data-stu-id="20e3d-198">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e3d-199">Quantidade</span><span class="sxs-lookup"><span data-stu-id="20e3d-199">Amount</span></span></td>
<td><p><span data-ttu-id="20e3d-200">Preço total por quantidade.</span><span class="sxs-lookup"><span data-stu-id="20e3d-200">Total of price for quantity.</span></span> <span data-ttu-id="20e3d-201">Útil para verificar se o cálculo do valor coincide com a forma como você calcula isso para seus clientes.</span><span class="sxs-lookup"><span data-stu-id="20e3d-201">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="20e3d-202">13.32</span><span class="sxs-lookup"><span data-stu-id="20e3d-202">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e3d-203">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="20e3d-203">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="20e3d-204">Valor de desconto aplicado a esses encargos.</span><span class="sxs-lookup"><span data-stu-id="20e3d-204">Amount of discount applied to these charges.</span></span> <span data-ttu-id="20e3d-205">IUR ou novas assinaturas qualificadas para incentivo também conterão um valor de desconto nessa coluna.</span><span class="sxs-lookup"><span data-stu-id="20e3d-205">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="20e3d-206">2.32</span><span class="sxs-lookup"><span data-stu-id="20e3d-206">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e3d-207">Subtotal</span><span class="sxs-lookup"><span data-stu-id="20e3d-207">Subtotal</span></span></td>
<td><p><span data-ttu-id="20e3d-208">Total sem imposto.</span><span class="sxs-lookup"><span data-stu-id="20e3d-208">Total before tax.</span></span> <span data-ttu-id="20e3d-209">Verifica se seu subtotal corresponde ao total esperado, em caso de desconto.</span><span class="sxs-lookup"><span data-stu-id="20e3d-209">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="20e3d-210">11</span><span class="sxs-lookup"><span data-stu-id="20e3d-210">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e3d-211">Imposto</span><span class="sxs-lookup"><span data-stu-id="20e3d-211">Tax</span></span></td>
<td><p><span data-ttu-id="20e3d-212">Valor do imposto cobrado, com base nas regras fiscais do mercado e em circunstâncias específicas.</span><span class="sxs-lookup"><span data-stu-id="20e3d-212">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="20e3d-213">0</span><span class="sxs-lookup"><span data-stu-id="20e3d-213">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e3d-214">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="20e3d-214">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="20e3d-215">Total com imposto.</span><span class="sxs-lookup"><span data-stu-id="20e3d-215">Total after tax.</span></span> <span data-ttu-id="20e3d-216">Verifica se o imposto é cobrado na fatura.</span><span class="sxs-lookup"><span data-stu-id="20e3d-216">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="20e3d-217">11</span><span class="sxs-lookup"><span data-stu-id="20e3d-217">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e3d-218">Moeda</span><span class="sxs-lookup"><span data-stu-id="20e3d-218">Currency</span></span></td>
<td><p><span data-ttu-id="20e3d-219">Tipo de moeda.</span><span class="sxs-lookup"><span data-stu-id="20e3d-219">Currency type.</span></span> <span data-ttu-id="20e3d-220">Cada entidade de cobrança tem somente uma moeda.</span><span class="sxs-lookup"><span data-stu-id="20e3d-220">Each billing entity has only one currency.</span></span> <span data-ttu-id="20e3d-221">Verifique se isso coincide com a primeira fatura e faça o mesmo após grandes atualizações na plataforma de cobrança.</span><span class="sxs-lookup"><span data-stu-id="20e3d-221">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="20e3d-222">Euro</span><span class="sxs-lookup"><span data-stu-id="20e3d-222">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e3d-223">CustomerName</span><span class="sxs-lookup"><span data-stu-id="20e3d-223">CustomerName</span></span></td>
<td><p><span data-ttu-id="20e3d-224">Nome da organização do cliente como informado no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="20e3d-224">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="20e3d-225">Isso é muito importante para reconciliar a fatura com as informações de seu sistema.</span><span class="sxs-lookup"><span data-stu-id="20e3d-225">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="20e3d-226">Cliente de teste A</span><span class="sxs-lookup"><span data-stu-id="20e3d-226">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e3d-227">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="20e3d-227">MPNID</span></span></td>
<td><p><span data-ttu-id="20e3d-228">ID do MPN do parceiro CSP</span><span class="sxs-lookup"><span data-stu-id="20e3d-228">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="20e3d-229">4390934</span><span class="sxs-lookup"><span data-stu-id="20e3d-229">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e3d-230">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="20e3d-230">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="20e3d-231">ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="20e3d-231">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="20e3d-232">Consulte [Discriminar por parceiro](#itemizebypartner).</span><span class="sxs-lookup"><span data-stu-id="20e3d-232">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="20e3d-233">4390934</span><span class="sxs-lookup"><span data-stu-id="20e3d-233">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e3d-234">DomainName</span><span class="sxs-lookup"><span data-stu-id="20e3d-234">DomainName</span></span></td>
<td><p><span data-ttu-id="20e3d-235">Nome de domínio do cliente, usado para ajudar a identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="20e3d-235">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="20e3d-236">Isso não deve ser usado para identificar exclusivamente o cliente como o cliente/parceiro pode atualizar o domínio banidos/padrão através do portal do O365.</span><span class="sxs-lookup"><span data-stu-id="20e3d-236">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="20e3d-237">Este campo pode aparecer em branco até o segundo ciclo de cobrança.</span><span class="sxs-lookup"><span data-stu-id="20e3d-237">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="20e3d-238">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="20e3d-238">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e3d-239">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="20e3d-239">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="20e3d-240">Apelido da Inscrição.</span><span class="sxs-lookup"><span data-stu-id="20e3d-240">Subscription nickname.</span></span> <span data-ttu-id="20e3d-241">Se nenhum apelido for especificado, o Partner Center usa o OfferName.</span><span class="sxs-lookup"><span data-stu-id="20e3d-241">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="20e3d-242">PROJETO ONLINE</span><span class="sxs-lookup"><span data-stu-id="20e3d-242">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e3d-243">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="20e3d-243">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="20e3d-244">O nome da oferta de serviço comprada pelo cliente, conforme definido na tabela de preços.</span><span class="sxs-lookup"><span data-stu-id="20e3d-244">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="20e3d-245">(Este é um campo idêntico ao nome da oferta).</span><span class="sxs-lookup"><span data-stu-id="20e3d-245">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="20e3d-246">PROJETO ONLINE PREMIUM SEM PROJETO CLIENTE</span><span class="sxs-lookup"><span data-stu-id="20e3d-246">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="20e3d-247">Campos de arquivo baseado em uso</span><span class="sxs-lookup"><span data-stu-id="20e3d-247">Usage-based file fields</span></span>


<span data-ttu-id="20e3d-248">Para reconciliar seus encargos com o uso de seu cliente, compare ResellerID/ResellerName/ResellerBillableAccount do arquivo de reconciliação com o nome do cliente e a ID da assinatura do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="20e3d-248">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="20e3d-249">Os campos a seguir explicam quais serviços foram usados e a taxa.</span><span class="sxs-lookup"><span data-stu-id="20e3d-249">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="20e3d-250">Coluna</span><span class="sxs-lookup"><span data-stu-id="20e3d-250">Column</span></span></strong></td>
<td><strong><span data-ttu-id="20e3d-251">Descrição</span><span class="sxs-lookup"><span data-stu-id="20e3d-251">Description</span></span></strong></td>
<td><strong><span data-ttu-id="20e3d-252">Valor de exemplo</span><span class="sxs-lookup"><span data-stu-id="20e3d-252">Sample value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e3d-253">PartnerID</span><span class="sxs-lookup"><span data-stu-id="20e3d-253">PartnerID</span></span></td>
<td><p><span data-ttu-id="20e3d-254">ID do parceiro, no formato GUID.</span><span class="sxs-lookup"><span data-stu-id="20e3d-254">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="20e3d-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="20e3d-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e3d-256">PartnerName</span><span class="sxs-lookup"><span data-stu-id="20e3d-256">PartnerName</span></span></td>
<td><p><span data-ttu-id="20e3d-257">Nome do parceiro.</span><span class="sxs-lookup"><span data-stu-id="20e3d-257">Partner Name.</span></span></p></td>
<td><span data-ttu-id="20e3d-258">Acme incorporado</span><span class="sxs-lookup"><span data-stu-id="20e3d-258">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e3d-259">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="20e3d-259">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="20e3d-260">ID da conta do parceiro.</span><span class="sxs-lookup"><span data-stu-id="20e3d-260">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="20e3d-261">1010578050</span><span class="sxs-lookup"><span data-stu-id="20e3d-261">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e3d-262">CustomerName</span><span class="sxs-lookup"><span data-stu-id="20e3d-262">CustomerName</span></span></td>
<td><p><span data-ttu-id="20e3d-263">Nome da organização do cliente como informado no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="20e3d-263">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="20e3d-264">Isso é muito importante para reconciliar a fatura com as informações de seu sistema.</span><span class="sxs-lookup"><span data-stu-id="20e3d-264">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="20e3d-265">Cliente de teste A</span><span class="sxs-lookup"><span data-stu-id="20e3d-265">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e3d-266">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="20e3d-266">MPNID</span></span></td>
<td><p><span data-ttu-id="20e3d-267">ID do MPN do parceiro CSP.</span><span class="sxs-lookup"><span data-stu-id="20e3d-267">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="20e3d-268">4390934</span><span class="sxs-lookup"><span data-stu-id="20e3d-268">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e3d-269">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="20e3d-269">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="20e3d-270">ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="20e3d-270">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="20e3d-271">Consulte [Discriminar por parceiro](#itemizebypartner).</span><span class="sxs-lookup"><span data-stu-id="20e3d-271">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="20e3d-272">4390934</span><span class="sxs-lookup"><span data-stu-id="20e3d-272">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e3d-273">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="20e3d-273">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="20e3d-274">Número da fatura na qual a transação especificada é exibida.</span><span class="sxs-lookup"><span data-stu-id="20e3d-274">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="20e3d-275">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="20e3d-275">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e3d-276">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="20e3d-276">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="20e3d-277">Data de início do ciclo de cobrança exceto quando apresentadas as datas de dados de uso latentes anteriormente não cobradas (do ciclo de cobrança anterior).</span><span class="sxs-lookup"><span data-stu-id="20e3d-277">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="20e3d-278">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="20e3d-278">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="20e3d-279">1/2/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="20e3d-279">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e3d-280">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="20e3d-280">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="20e3d-281">Data de término do ciclo de cobrança exceto quando apresentadas as datas de dados de uso latentes anteriormente não cobradas (do ciclo de cobrança anterior).</span><span class="sxs-lookup"><span data-stu-id="20e3d-281">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="20e3d-282">A hora é sempre o fim do dia, 23:59.</span><span class="sxs-lookup"><span data-stu-id="20e3d-282">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="20e3d-283">28/2/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="20e3d-283">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e3d-284">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="20e3d-284">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="20e3d-285">Identificador exclusivo de uma assinatura na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="20e3d-285">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="20e3d-286">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="20e3d-286">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="20e3d-287">Esse não é o mesmo que a ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="20e3d-287">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="20e3d-288">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="20e3d-288">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e3d-289">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="20e3d-289">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="20e3d-290">Apelido da oferta do serviço.</span><span class="sxs-lookup"><span data-stu-id="20e3d-290">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="20e3d-291">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="20e3d-291">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e3d-292">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="20e3d-292">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="20e3d-293">Linha de negócios da oferta do serviço</span><span class="sxs-lookup"><span data-stu-id="20e3d-293">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="20e3d-294">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="20e3d-294">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e3d-295">OrderID</span><span class="sxs-lookup"><span data-stu-id="20e3d-295">OrderID</span></span></td>
<td><p><span data-ttu-id="20e3d-296">Identificador exclusivo para um pedido na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="20e3d-296">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="20e3d-297">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="20e3d-297">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="20e3d-298">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="20e3d-298">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e3d-299">ServiceName</span><span class="sxs-lookup"><span data-stu-id="20e3d-299">ServiceName</span></span></td>
<td><p><span data-ttu-id="20e3d-300">O nome do serviço do Azure em questão.</span><span class="sxs-lookup"><span data-stu-id="20e3d-300">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="20e3d-301">MÁQUINAS VIRTUAIS</span><span class="sxs-lookup"><span data-stu-id="20e3d-301">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e3d-302">ServiceType</span><span class="sxs-lookup"><span data-stu-id="20e3d-302">ServiceType</span></span></td>
<td><p><span data-ttu-id="20e3d-303">O tipo específico de serviço do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="20e3d-303">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="20e3d-304">Service Bus – Individual ou pacote</span><span class="sxs-lookup"><span data-stu-id="20e3d-304">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="20e3d-305">Banco de dados SQL Azure – Edição empresa ou Web</span><span class="sxs-lookup"><span data-stu-id="20e3d-305">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e3d-306">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="20e3d-306">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="20e3d-307">Identificador exclusivo específico de toda a estrutura de serviço de dados e preço.</span><span class="sxs-lookup"><span data-stu-id="20e3d-307">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="20e3d-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="20e3d-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e3d-309">Nome do recurso</span><span class="sxs-lookup"><span data-stu-id="20e3d-309">Resource Name</span></span></td>
<td><p><span data-ttu-id="20e3d-310">O nome do recurso do Azure.</span><span class="sxs-lookup"><span data-stu-id="20e3d-310">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="20e3d-311">Dados de entrada transferidos (GB)</span><span class="sxs-lookup"><span data-stu-id="20e3d-311">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="20e3d-312">Dados de saída transferidos (GB)</span><span class="sxs-lookup"><span data-stu-id="20e3d-312">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e3d-313">Região</span><span class="sxs-lookup"><span data-stu-id="20e3d-313">Region</span></span></td>
<td><p><span data-ttu-id="20e3d-314">A região a qual o uso se aplica.</span><span class="sxs-lookup"><span data-stu-id="20e3d-314">The region the usage applies to.</span></span> <span data-ttu-id="20e3d-315">Usado principalmente para atribuir as taxas de transferências de dados, já que as taxas variam de acordo com a região.</span><span class="sxs-lookup"><span data-stu-id="20e3d-315">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="20e3d-316">Pacífico Asiático, Europa, América Latina e América do Norte</span><span class="sxs-lookup"><span data-stu-id="20e3d-316">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e3d-317">SKU</span><span class="sxs-lookup"><span data-stu-id="20e3d-317">SKU</span></span></td>
<td><p><span data-ttu-id="20e3d-318">Identificador exclusivo MSFT da oferta</span><span class="sxs-lookup"><span data-stu-id="20e3d-318">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="20e3d-319">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="20e3d-319">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="20e3d-320">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="20e3d-320">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="20e3d-321">Uma ID e a quantidade para discriminar as taxas diferentes de um serviço ou recurso em um determinado período de cobrança.</span><span class="sxs-lookup"><span data-stu-id="20e3d-321">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="20e3d-322">Para a classificação em camadas do Azure, pode haver uma taxa para uma determinada quantidade de unidades faturáveis e uma taxa diferente depois disso.</span><span class="sxs-lookup"><span data-stu-id="20e3d-322">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="20e3d-323">1</span><span class="sxs-lookup"><span data-stu-id="20e3d-323">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e3d-324">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="20e3d-324">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="20e3d-325">A quantidade de serviço consumida (horas, GB etc.) durante o período de relatório.</span><span class="sxs-lookup"><span data-stu-id="20e3d-325">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="20e3d-326">Também inclui qualquer uso não cobrado de períodos de relatório anteriores.</span><span class="sxs-lookup"><span data-stu-id="20e3d-326">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="20e3d-327">11</span><span class="sxs-lookup"><span data-stu-id="20e3d-327">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e3d-328">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="20e3d-328">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="20e3d-329">Unidades incluídas como parte da oferta.</span><span class="sxs-lookup"><span data-stu-id="20e3d-329">Units included as part of the offer.</span></span> <span data-ttu-id="20e3d-330">Normalmente não está presente no CSP.</span><span class="sxs-lookup"><span data-stu-id="20e3d-330">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="20e3d-331">0</span><span class="sxs-lookup"><span data-stu-id="20e3d-331">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="20e3d-332">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="20e3d-332">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="20e3d-333">Unidades não incluídas como parte da oferta devem ser pagas pelo parceiro.</span><span class="sxs-lookup"><span data-stu-id="20e3d-333">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="20e3d-334">Igual a ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="20e3d-334">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="20e3d-335">11</span><span class="sxs-lookup"><span data-stu-id="20e3d-335">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e3d-336">ListPrice</span><span class="sxs-lookup"><span data-stu-id="20e3d-336">ListPrice</span></span></td>
<td><p><span data-ttu-id="20e3d-337">Preço da oferta em vigor na data de início da assinatura.</span><span class="sxs-lookup"><span data-stu-id="20e3d-337">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="20e3d-338">U$ 0,0808</span><span class="sxs-lookup"><span data-stu-id="20e3d-338">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e3d-339">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="20e3d-339">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="20e3d-340">ListPrist vezes OverageQuantity, arredondado para o centavo mais próximo.</span><span class="sxs-lookup"><span data-stu-id="20e3d-340">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="20e3d-341">U$ 0,085</span><span class="sxs-lookup"><span data-stu-id="20e3d-341">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e3d-342">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="20e3d-342">TaxAmount</span></span></td>
<td><p><span data-ttu-id="20e3d-343">Valor do imposto cobrado, com base nas regras fiscais do mercado e em circunstâncias específicas.</span><span class="sxs-lookup"><span data-stu-id="20e3d-343">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="20e3d-344">U$ 0,08</span><span class="sxs-lookup"><span data-stu-id="20e3d-344">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e3d-345">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="20e3d-345">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="20e3d-346">Total após imposto, quando o imposto é aplicável.</span><span class="sxs-lookup"><span data-stu-id="20e3d-346">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="20e3d-347">U$ 0,93</span><span class="sxs-lookup"><span data-stu-id="20e3d-347">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e3d-348">Moeda</span><span class="sxs-lookup"><span data-stu-id="20e3d-348">Currency</span></span></td>
<td><p><span data-ttu-id="20e3d-349">Tipo de moeda.</span><span class="sxs-lookup"><span data-stu-id="20e3d-349">Currency type.</span></span> <span data-ttu-id="20e3d-350">Cada entidade de cobrança tem somente uma moeda.</span><span class="sxs-lookup"><span data-stu-id="20e3d-350">Each billing entity has only one currency.</span></span> <span data-ttu-id="20e3d-351">Verifique se isso coincide com a primeira fatura e faça o mesmo após grandes atualizações na plataforma de cobrança.</span><span class="sxs-lookup"><span data-stu-id="20e3d-351">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="20e3d-352">Euro</span><span class="sxs-lookup"><span data-stu-id="20e3d-352">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e3d-353">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="20e3d-353">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="20e3d-354">Preço por unidade sem imposto.</span><span class="sxs-lookup"><span data-stu-id="20e3d-354">Pretax price per unit.</span></span> <span data-ttu-id="20e3d-355">Igual a PretaxCharges / OverageQuantity, arredondado para o centavo mais próximo.</span><span class="sxs-lookup"><span data-stu-id="20e3d-355">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="20e3d-356">U$ 0,08</span><span class="sxs-lookup"><span data-stu-id="20e3d-356">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e3d-357">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="20e3d-357">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="20e3d-358">Preço pós-imposto por unidade.</span><span class="sxs-lookup"><span data-stu-id="20e3d-358">Post tax price per unit.</span></span> <span data-ttu-id="20e3d-359">Igual a PostTaxTotal / OverageQuantity, ou PretaxEffectiveRate + taxa de imposto por valor de unidade, arredondado para o centavo mais próximo.</span><span class="sxs-lookup"><span data-stu-id="20e3d-359">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="20e3d-360">U$ 0,08</span><span class="sxs-lookup"><span data-stu-id="20e3d-360">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e3d-361">ChargeType</span><span class="sxs-lookup"><span data-stu-id="20e3d-361">ChargeType</span></span></td>
<td><p><span data-ttu-id="20e3d-362">O tipo de encargo ou ajuste.</span><span class="sxs-lookup"><span data-stu-id="20e3d-362">The type of charge or adjustment.</span></span> <span data-ttu-id="20e3d-363">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="20e3d-363">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="20e3d-364">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="20e3d-364">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e3d-365">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="20e3d-365">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="20e3d-366">ID exclusiva da conta na plataforma de cobrança da MSFT.</span><span class="sxs-lookup"><span data-stu-id="20e3d-366">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="20e3d-367">1280018095</span><span class="sxs-lookup"><span data-stu-id="20e3d-367">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e3d-368">UsageDate</span><span class="sxs-lookup"><span data-stu-id="20e3d-368">UsageDate</span></span></td>
<td><p><span data-ttu-id="20e3d-369">Data da implantação do serviço.</span><span class="sxs-lookup"><span data-stu-id="20e3d-369">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="20e3d-370">1/2/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="20e3d-370">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e3d-371">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="20e3d-371">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="20e3d-372">Essa coluna identifica a localização de um data center dentro da região para serviços onde isso é aplicável e preenchido.</span><span class="sxs-lookup"><span data-stu-id="20e3d-372">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="20e3d-373">Leste da Ásia, Sudeste da Ásia, Norte da Europa, Europa Ocidental, Centro Norte e Centro Sul dos EUA</span><span class="sxs-lookup"><span data-stu-id="20e3d-373">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e3d-374">MeteredService</span><span class="sxs-lookup"><span data-stu-id="20e3d-374">MeteredService</span></span></td>
<td><p><span data-ttu-id="20e3d-375">Essa coluna é utilizada para rastrear o serviço do Microsoft Azure individual que não pode ser identificado especificamente na coluna Nome do Serviço.</span><span class="sxs-lookup"><span data-stu-id="20e3d-375">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="20e3d-376">Por exemplo, transferências de dados são relatadas como &quot;Microsoft Azure – Todos os Serviços&quot; na coluna Nome do Serviço.</span><span class="sxs-lookup"><span data-stu-id="20e3d-376">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="20e3d-377">Essa coluna MeteredService indicará ao qual serviço específico o uso pertence.</span><span class="sxs-lookup"><span data-stu-id="20e3d-377">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="20e3d-378">AccessControl, CDN, Computação, Banco de dados, ServiceBus, Armazenamento</span><span class="sxs-lookup"><span data-stu-id="20e3d-378">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e3d-379">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="20e3d-379">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="20e3d-380">Um subcabeçalho que esclarece ainda mais o serviço Microsoft Azure individual além do nível fornecido pelo campo MeteredService.</span><span class="sxs-lookup"><span data-stu-id="20e3d-380">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="20e3d-381">EXTERNO</span><span class="sxs-lookup"><span data-stu-id="20e3d-381">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e3d-382">Projeto</span><span class="sxs-lookup"><span data-stu-id="20e3d-382">Project</span></span></td>
<td><p><span data-ttu-id="20e3d-383">Nome definido pelo cliente para a instância do serviço</span><span class="sxs-lookup"><span data-stu-id="20e3d-383">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="20e3d-384">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="20e3d-384">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e3d-385">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="20e3d-385">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="20e3d-386">O número de conexões ServiceBus que foram provisionados e utilizados em um dia específico.</span><span class="sxs-lookup"><span data-stu-id="20e3d-386">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="20e3d-387">Por exemplo: se você tivesse uma conexão individualmente provisionada durante um mês de 30 dias, a coluna Informação do Serviço 1 lerá "1,000000 conexões/30 dias".</span><span class="sxs-lookup"><span data-stu-id="20e3d-387">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="20e3d-388">Se você tinha um pacote de 25 conexões ServiceBus provisionadas e você utilizou 1 durante o dia, sua declaração de uso diário para esse dia indicaria "25 conexões/30 dias – Usado: 1,000000".</span><span class="sxs-lookup"><span data-stu-id="20e3d-388">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e3d-389">CustomerID</span><span class="sxs-lookup"><span data-stu-id="20e3d-389">CustomerID</span></span></td>
<td><p><span data-ttu-id="20e3d-390">ID exclusiva da Microsoft, no formato GUID, usada para identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="20e3d-390">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="20e3d-391">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="20e3d-391">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e3d-392">DomainName</span><span class="sxs-lookup"><span data-stu-id="20e3d-392">DomainName</span></span></td>
<td><p><span data-ttu-id="20e3d-393">Nome de domínio do cliente, usado para ajudar a identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="20e3d-393">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="20e3d-394">Este campo pode aparecer em branco até o segundo ciclo de cobrança.</span><span class="sxs-lookup"><span data-stu-id="20e3d-394">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="20e3d-395">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="20e3d-395">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="20e3d-396">Unidade</span><span class="sxs-lookup"><span data-stu-id="20e3d-396">Unit</span></span></td>
<td><p><span data-ttu-id="20e3d-397">A unidade do nome do recurso</span><span class="sxs-lookup"><span data-stu-id="20e3d-397">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="20e3d-398">GB ou HORAS</span><span class="sxs-lookup"><span data-stu-id="20e3d-398">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="onetimefiles"></a><span data-ttu-id="20e3d-399">Campos de arquivo de compra única</span><span class="sxs-lookup"><span data-stu-id="20e3d-399">One-time purchase file fields</span></span>

|**<span data-ttu-id="20e3d-400">Campo</span><span class="sxs-lookup"><span data-stu-id="20e3d-400">Field</span></span>** |**<span data-ttu-id="20e3d-401">Definição</span><span class="sxs-lookup"><span data-stu-id="20e3d-401">Definition</span></span>**|
|:----------------|:-----------------------------|
|<span data-ttu-id="20e3d-402">PartnerId</span><span class="sxs-lookup"><span data-stu-id="20e3d-402">PartnerId</span></span> |<span data-ttu-id="20e3d-403">ID do parceiro, no formato GUID.</span><span class="sxs-lookup"><span data-stu-id="20e3d-403">Partner ID, in GUID format.</span></span> |
|<span data-ttu-id="20e3d-404">CustomerID</span><span class="sxs-lookup"><span data-stu-id="20e3d-404">CustomerId</span></span> |<span data-ttu-id="20e3d-405">ID exclusiva da Microsoft, no formato GUID, usada para identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="20e3d-405">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span> |
|<span data-ttu-id="20e3d-406">CustomerName</span><span class="sxs-lookup"><span data-stu-id="20e3d-406">CustomerName</span></span> |<span data-ttu-id="20e3d-407">Nome da organização do cliente como informado no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="20e3d-407">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="20e3d-408">Isso é muito importante para reconciliar a fatura com as informações de seu sistema.</span><span class="sxs-lookup"><span data-stu-id="20e3d-408">This is very important for reconciling the invoice with your system information.</span></span> |
|<span data-ttu-id="20e3d-409">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="20e3d-409">CustomerDomainName</span></span> |<span data-ttu-id="20e3d-410">O nome de domínio do cliente.</span><span class="sxs-lookup"><span data-stu-id="20e3d-410">The customer’s domain name.</span></span> |
|<span data-ttu-id="20e3d-411">CustomerCountry</span><span class="sxs-lookup"><span data-stu-id="20e3d-411">CustomerCountry</span></span> |<span data-ttu-id="20e3d-412">O país em que o cliente está localizado.</span><span class="sxs-lookup"><span data-stu-id="20e3d-412">The country in which the customer is located.</span></span> |
|<span data-ttu-id="20e3d-413">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="20e3d-413">InvoiceNumber</span></span> |<span data-ttu-id="20e3d-414">Número da fatura na qual a transação especificada é exibida.</span><span class="sxs-lookup"><span data-stu-id="20e3d-414">Invoice number where the specified transaction appears.</span></span> |
|<span data-ttu-id="20e3d-415">MpnId</span><span class="sxs-lookup"><span data-stu-id="20e3d-415">MpnId</span></span> |<span data-ttu-id="20e3d-416">ID do MPN do parceiro CSP (direto ou indireto).</span><span class="sxs-lookup"><span data-stu-id="20e3d-416">MPN ID of the CSP partner (direct or indirect).</span></span> |
|<span data-ttu-id="20e3d-417">ID do MPN do revendedor</span><span class="sxs-lookup"><span data-stu-id="20e3d-417">Reseller MPN ID</span></span> |<span data-ttu-id="20e3d-418">Só aparece em arquivos de reconciliação para parceiros no modelo indireto.</span><span class="sxs-lookup"><span data-stu-id="20e3d-418">Only appears on reconciliation files for partners in the indirect model.</span></span> <span data-ttu-id="20e3d-419">A ID do MPN do revendedor de registro da reserva.</span><span class="sxs-lookup"><span data-stu-id="20e3d-419">The MPN ID of the reseller of record for the reservation.</span></span> <span data-ttu-id="20e3d-420">Isso corresponde à ID de revendedor listada para a reserva específica no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="20e3d-420">This corresponds to the reseller ID listed for the specific reservation in Partner Center.</span></span> <span data-ttu-id="20e3d-421">Se um parceiro CSP vendeu a reserva diretamente para o cliente, sua ID do MPN estará listada duas vezes, como a ID do MPN e a ID do MPN do revendedor.</span><span class="sxs-lookup"><span data-stu-id="20e3d-421">If a CSP partner sold the reservation directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span> <span data-ttu-id="20e3d-422">Se um parceiro CSP tiver um revendedor sem ID do MPN, esse valor será definido como a ID do MPN do parceiro.</span><span class="sxs-lookup"><span data-stu-id="20e3d-422">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span> <span data-ttu-id="20e3d-423">Se o parceiro CSP remover uma ID de revendedor, esse valor será definido como -1.</span><span class="sxs-lookup"><span data-stu-id="20e3d-423">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span> |
|<span data-ttu-id="20e3d-424">OrderId</span><span class="sxs-lookup"><span data-stu-id="20e3d-424">OrderId</span></span> |<span data-ttu-id="20e3d-425">Identificador exclusivo para um pedido na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="20e3d-425">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="20e3d-426">Pode ser útil para identificar a reserva do Azure ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="20e3d-426">May be useful to identify the Azure reservation when contacting support but not for reconciliation.</span></span> |
|<span data-ttu-id="20e3d-427">OrderDate</span><span class="sxs-lookup"><span data-stu-id="20e3d-427">OrderDate</span></span> |<span data-ttu-id="20e3d-428">A data em que o pedido foi feito.</span><span class="sxs-lookup"><span data-stu-id="20e3d-428">The date the order was placed.</span></span> |
|<span data-ttu-id="20e3d-429">ProductId</span><span class="sxs-lookup"><span data-stu-id="20e3d-429">ProductId</span></span> |<span data-ttu-id="20e3d-430">A ID do produto.</span><span class="sxs-lookup"><span data-stu-id="20e3d-430">The ID for the product.</span></span> |
|<span data-ttu-id="20e3d-431">SkuId</span><span class="sxs-lookup"><span data-stu-id="20e3d-431">SkuId</span></span>  |<span data-ttu-id="20e3d-432">A ID de uma SKU em particular.</span><span class="sxs-lookup"><span data-stu-id="20e3d-432">The ID for a particular SKU.</span></span> |
|<span data-ttu-id="20e3d-433">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="20e3d-433">AvailabilityId</span></span> |<span data-ttu-id="20e3d-434">A ID de uma Disponibilidade em particular.</span><span class="sxs-lookup"><span data-stu-id="20e3d-434">The ID for a particular Availability.</span></span> <span data-ttu-id="20e3d-435">"Disponibilidade" refere-se a se uma SKU em particular está disponível ou não para compra para determinado país, moeda, segmento do setor etc.</span><span class="sxs-lookup"><span data-stu-id="20e3d-435">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span> |
|<span data-ttu-id="20e3d-436">SkuName</span><span class="sxs-lookup"><span data-stu-id="20e3d-436">SkuName</span></span>  |<span data-ttu-id="20e3d-437">O título de uma SKU em particular.</span><span class="sxs-lookup"><span data-stu-id="20e3d-437">The title for a particular SKU.</span></span> |
|<span data-ttu-id="20e3d-438">ProductName</span><span class="sxs-lookup"><span data-stu-id="20e3d-438">ProductName</span></span> |<span data-ttu-id="20e3d-439">O nome do produto.</span><span class="sxs-lookup"><span data-stu-id="20e3d-439">The name of the product.</span></span> |
|<span data-ttu-id="20e3d-440">ChargeType</span><span class="sxs-lookup"><span data-stu-id="20e3d-440">ChargeType</span></span> |<span data-ttu-id="20e3d-441">O tipo de encargo ou ajuste.</span><span class="sxs-lookup"><span data-stu-id="20e3d-441">The type of charge or adjustment.</span></span> |
|<span data-ttu-id="20e3d-442">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="20e3d-442">UnitPrice</span></span> |<span data-ttu-id="20e3d-443">Preço por produto pedido.</span><span class="sxs-lookup"><span data-stu-id="20e3d-443">Price per product ordered.</span></span> |
|<span data-ttu-id="20e3d-444">Quantidade</span><span class="sxs-lookup"><span data-stu-id="20e3d-444">Quantity</span></span> |<span data-ttu-id="20e3d-445">Número de produtos pedidos.</span><span class="sxs-lookup"><span data-stu-id="20e3d-445">Number of products ordered.</span></span> |
|<span data-ttu-id="20e3d-446">Subtotal</span><span class="sxs-lookup"><span data-stu-id="20e3d-446">Subtotal</span></span> |<span data-ttu-id="20e3d-447">Total sem imposto.</span><span class="sxs-lookup"><span data-stu-id="20e3d-447">Total before tax.</span></span> <span data-ttu-id="20e3d-448">Verifica se seu subtotal corresponde ao total esperado, em caso de desconto.</span><span class="sxs-lookup"><span data-stu-id="20e3d-448">Checks that your subtotal matches your expected total, in case of a discount.</span></span> |
|<span data-ttu-id="20e3d-449">TaxTotal</span><span class="sxs-lookup"><span data-stu-id="20e3d-449">TaxTotal</span></span> |<span data-ttu-id="20e3d-450">O total de todos os impostos aplicáveis.</span><span class="sxs-lookup"><span data-stu-id="20e3d-450">The total of all applicable taxes.</span></span> |
|<span data-ttu-id="20e3d-451">Total</span><span class="sxs-lookup"><span data-stu-id="20e3d-451">Total</span></span> |<span data-ttu-id="20e3d-452">O valor total desta compra.</span><span class="sxs-lookup"><span data-stu-id="20e3d-452">The total amount of this purchase.</span></span> |
|<span data-ttu-id="20e3d-453">Moeda</span><span class="sxs-lookup"><span data-stu-id="20e3d-453">Currency</span></span> |<span data-ttu-id="20e3d-454">Tipo de moeda.</span><span class="sxs-lookup"><span data-stu-id="20e3d-454">Currency type.</span></span> <span data-ttu-id="20e3d-455">Cada entidade de cobrança tem somente uma moeda.</span><span class="sxs-lookup"><span data-stu-id="20e3d-455">Each billing entity has only one currency.</span></span> <span data-ttu-id="20e3d-456">Verifique se isso coincide com a primeira fatura e faça o mesmo após grandes atualizações na plataforma de cobrança.</span><span class="sxs-lookup"><span data-stu-id="20e3d-456">Check that it matches your first invoice and then after any major billing platform update.</span></span> |
|<span data-ttu-id="20e3d-457">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="20e3d-457">DiscountDetails</span></span> |<span data-ttu-id="20e3d-458">Lista detalhada dos descontos relevantes.</span><span class="sxs-lookup"><span data-stu-id="20e3d-458">Detailed listing of any relevant discounts.</span></span> |



## <a href="" id="charge_types"></a><span data-ttu-id="20e3d-459">Como mapear encargos entre uma fatura e o arquivo de reconciliação</span><span class="sxs-lookup"><span data-stu-id="20e3d-459">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="20e3d-460">Sua fatura fornece um resumo dos encargos, enquanto seu arquivo de reconciliação fornece uma divisão detalhada das transações de item de linha, incluindo os tipos de carga.</span><span class="sxs-lookup"><span data-stu-id="20e3d-460">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="20e3d-461">Para fazer referência cruzada das quantidades de carga entre o arquivo de reconciliação e fatura, você pode usar opções de filtro do Microsoft Excel para filtrar por tipos de cobrança no arquivo de reconciliação para mapear os encargos de fatura em um conjunto de detalhamentos de cobrança no arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="20e3d-461">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="20e3d-462">Os arquivos de reconciliação, tanto os baseados em licença quanto os baseados em uso, mostram apenas encargos e transações relacionadas ao uso (unidades consumidas e encargos relacionados).</span><span class="sxs-lookup"><span data-stu-id="20e3d-462">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="20e3d-463">Créditos únicos, descontos ou reembolsos que aparecem na fatura como "Ajustes" não são mostrados no arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="20e3d-463">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="20e3d-464">A tabela a seguir mostra os mapeamentos entre uma seção da fatura e os tipos de encargo associados que podem aparecer nos arquivos de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="20e3d-464">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><strong><span data-ttu-id="20e3d-465">Descrição do encargo da fatura</span><span class="sxs-lookup"><span data-stu-id="20e3d-465">Invoice charge description</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="20e3d-466">Descrição do encargo do arquivo de reconciliação (coluna ChargeType)</span><span class="sxs-lookup"><span data-stu-id="20e3d-466">Reconciliation file charge description (ChargeType column)</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="20e3d-467">O que é este encargo?</span><span class="sxs-lookup"><span data-stu-id="20e3d-467">What is this charge?</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="20e3d-468">Como é possível mapear esses tipos de encargo na fatura?</span><span class="sxs-lookup"><span data-stu-id="20e3d-468">How do I map these ChargeTypes to the invoice?</span></span></strong></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><strong><span data-ttu-id="20e3d-469">Encargos baseadas em licença</span><span class="sxs-lookup"><span data-stu-id="20e3d-469">License-based charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="20e3d-470">Taxa de ativação</span><span class="sxs-lookup"><span data-stu-id="20e3d-470">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e3d-471">O valor cobrado do cliente quando ele usa a assinatura depois de comprá-la.</span><span class="sxs-lookup"><span data-stu-id="20e3d-471">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="20e3d-472">No arquivo baseado em licença, some a coluna <strong>Quantidade</strong></span><span class="sxs-lookup"><span data-stu-id="20e3d-472">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20e3d-473">Taxa de cancelamento</span><span class="sxs-lookup"><span data-stu-id="20e3d-473">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e3d-474">Os encargos proporcionais reembolsados para o cliente quando os assentos associados são alterados</span><span class="sxs-lookup"><span data-stu-id="20e3d-474">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20e3d-475">Taxa do ciclo</span><span class="sxs-lookup"><span data-stu-id="20e3d-475">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e3d-476">Encargos periódicos de uma assinatura</span><span class="sxs-lookup"><span data-stu-id="20e3d-476">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20e3d-477">Percorrer ocorrência proporcional</span><span class="sxs-lookup"><span data-stu-id="20e3d-477">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e3d-478">Os encargos proporcionais cobrados do cliente quando os assentos associados são alterados</span><span class="sxs-lookup"><span data-stu-id="20e3d-478">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20e3d-479">Taxas proporcionais durante o cancelamento</span><span class="sxs-lookup"><span data-stu-id="20e3d-479">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e3d-480">Reembolso proporcional para a parte não utilizada do serviço após o cancelamento</span><span class="sxs-lookup"><span data-stu-id="20e3d-480">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20e3d-481">Taxas proporcionais durante a compra</span><span class="sxs-lookup"><span data-stu-id="20e3d-481">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e3d-482">O tipo de cobrança de uma assinatura ao usar a cobrança anual</span><span class="sxs-lookup"><span data-stu-id="20e3d-482">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20e3d-483">Taxa de compra</span><span class="sxs-lookup"><span data-stu-id="20e3d-483">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e3d-484">O tipo de cobrança de uma assinatura ao usar a cobrança mensal</span><span class="sxs-lookup"><span data-stu-id="20e3d-484">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20e3d-485">Taxa proporcional ao renovar</span><span class="sxs-lookup"><span data-stu-id="20e3d-485">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e3d-486">Taxas proporcionais após a renovação da assinatura</span><span class="sxs-lookup"><span data-stu-id="20e3d-486">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="20e3d-487">Taxa de renovação</span><span class="sxs-lookup"><span data-stu-id="20e3d-487">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e3d-488">Cobrança para renovação de uma assinatura</span><span class="sxs-lookup"><span data-stu-id="20e3d-488">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20e3d-489">Taxas proporcionais ao ativar</span><span class="sxs-lookup"><span data-stu-id="20e3d-489">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e3d-490">Taxas proporcionais da ativação até o final do período de cobrança</span><span class="sxs-lookup"><span data-stu-id="20e3d-490">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong><span data-ttu-id="20e3d-491">Tarifas de uso</span><span class="sxs-lookup"><span data-stu-id="20e3d-491">Usage Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="20e3d-492">Avaliar a taxa de uso ao cancelar</span><span class="sxs-lookup"><span data-stu-id="20e3d-492">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e3d-493">Taxa de uso de acesso com o cancelamento para uso não pago durante o período de cobrança atual</span><span class="sxs-lookup"><span data-stu-id="20e3d-493">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="20e3d-494">No arquivo baseado em uso, some a coluna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="20e3d-494">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20e3d-495">Avalie a taxa de uso para o ciclo atual</span><span class="sxs-lookup"><span data-stu-id="20e3d-495">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e3d-496">Taxa de uso de acesso para o período atual de cobrança</span><span class="sxs-lookup"><span data-stu-id="20e3d-496">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="20e3d-497">Créditos</span><span class="sxs-lookup"><span data-stu-id="20e3d-497">Credits</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="20e3d-498">Deslocando um item de linha</span><span class="sxs-lookup"><span data-stu-id="20e3d-498">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e3d-499">Reembolso parcial ou integral para um item de linha, incluindo os impostos</span><span class="sxs-lookup"><span data-stu-id="20e3d-499">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e3d-500">No arquivo baseado em licença, some a coluna <strong>TotalForCustomer</strong></span><span class="sxs-lookup"><span data-stu-id="20e3d-500">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="20e3d-501">No arquivo baseado em uso, some a coluna <strong>PostTaxTotal</strong></span><span class="sxs-lookup"><span data-stu-id="20e3d-501">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><strong><span data-ttu-id="20e3d-502">Descontos baseados em uso</span><span class="sxs-lookup"><span data-stu-id="20e3d-502">Usage-based discounts</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="20e3d-503">Desconto de ativação</span><span class="sxs-lookup"><span data-stu-id="20e3d-503">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e3d-504">Desconto aplicado quando a assinatura é ativada</span><span class="sxs-lookup"><span data-stu-id="20e3d-504">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="20e3d-505">No arquivo baseado em uso, some a coluna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="20e3d-505">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20e3d-506">Desconto de ciclo</span><span class="sxs-lookup"><span data-stu-id="20e3d-506">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e3d-507">Desconto aplicado em cobranças periódicas</span><span class="sxs-lookup"><span data-stu-id="20e3d-507">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20e3d-508">Desconto de renovação</span><span class="sxs-lookup"><span data-stu-id="20e3d-508">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e3d-509">Desconto aplicado quando a assinatura é renovada</span><span class="sxs-lookup"><span data-stu-id="20e3d-509">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20e3d-510">Desconto de cancelamento</span><span class="sxs-lookup"><span data-stu-id="20e3d-510">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e3d-511">Encargos aplicados quando descontos são cancelados</span><span class="sxs-lookup"><span data-stu-id="20e3d-511">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><strong><span data-ttu-id="20e3d-512">Descontos baseados em licença</span><span class="sxs-lookup"><span data-stu-id="20e3d-512">License-based discounts</span></span></strong></p>
</td>
<td>
<p><em><span data-ttu-id="20e3d-513">Podem ser aplicados a vários tipos de cobrança</span><span class="sxs-lookup"><span data-stu-id="20e3d-513">May be applied to multiple charge types</span></span></em></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="20e3d-514">No arquivo baseado em licença, some a coluna <strong>TotalOtherDiscount</strong></span><span class="sxs-lookup"><span data-stu-id="20e3d-514">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20e3d-515"><strong>Impostos</strong>&nbsp;ou&nbsp;<strong>IVA</strong></span><span class="sxs-lookup"><span data-stu-id="20e3d-515"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><em><span data-ttu-id="20e3d-516">Podem ser aplicados a vários tipos de cobrança</span><span class="sxs-lookup"><span data-stu-id="20e3d-516">May be applied to multiple charge types</span></span></em></p>
<p><em><span data-ttu-id="20e3d-517">Exceção: "Deslocamento de um item de linha" já inclui impostos.</span><span class="sxs-lookup"><span data-stu-id="20e3d-517">Exception: "Offset a line item" already includes taxes.</span></span> <span data-ttu-id="20e3d-518">Consulte créditos, acima.</span><span class="sxs-lookup"><span data-stu-id="20e3d-518">See Credits, above.</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="20e3d-519">Impostos ou impostos sobre valor agregado (IVA)</span><span class="sxs-lookup"><span data-stu-id="20e3d-519">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e3d-520">No arquivo baseado em licença, some a coluna <strong>Imposto</strong></span><span class="sxs-lookup"><span data-stu-id="20e3d-520">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="20e3d-521">No arquivo baseado em uso, some a coluna <strong>TaxAmount</strong></span><span class="sxs-lookup"><span data-stu-id="20e3d-521">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
