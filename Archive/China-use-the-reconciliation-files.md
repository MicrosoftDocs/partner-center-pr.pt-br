---
title: Use os arquivos de reconciliação (operado pela 21Vianet do Partner Center)
ms.topic: article
ms.date: 10/29/2018
description: Para obter uma exibição detalhada em itens de linha de cada encargo em um ciclo de cobrança, baixe os arquivos de reconciliação do painel do Partner Center.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: KPacquer
ms.author: kenpacq
ms.openlocfilehash: 30e3b7a7933678c4af079bb86aa1439559387f2b
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2019
ms.locfileid: "62132076"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="c8267-103">Usar os arquivos de reconciliação</span><span class="sxs-lookup"><span data-stu-id="c8267-103">Use the reconciliation files</span></span>

<span data-ttu-id="c8267-104">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="c8267-104">**Applies to**</span></span>

-   <span data-ttu-id="c8267-105">Partner Center operado pela 21Vianet</span><span class="sxs-lookup"><span data-stu-id="c8267-105">Partner Center operated by 21Vianet</span></span>


<span data-ttu-id="c8267-106">Para obter uma exibição detalhada em itens de linha de cada encargo em um ciclo de cobrança, baixe os arquivos de reconciliação do painel do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="c8267-106">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from the Partner Center dashboard.</span></span> <span data-ttu-id="c8267-107">Os detalhes incluem encargos por assinaturas de cada cliente e eventos detalhados (como a adição de assentos a uma assinatura no meio do período).</span><span class="sxs-lookup"><span data-stu-id="c8267-107">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="c8267-108">Discriminar pelo parceiro</span><span class="sxs-lookup"><span data-stu-id="c8267-108">Itemize by partner</span></span>


<span data-ttu-id="c8267-109">Os parceiros no modelo indireto podem usar esses campos adicionais nos arquivos de reconciliação baseados em uso e em licença para discriminar por revendedor.</span><span class="sxs-lookup"><span data-stu-id="c8267-109">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="c8267-110">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="c8267-110">MPN ID</span></span></th>
<th><span data-ttu-id="c8267-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8267-111">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="c8267-112">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="c8267-112">MPN ID</span></span></td>
<td><p><span data-ttu-id="c8267-113">A ID do Microsoft Partner Network (MPN) do parceiro CSP (direta ou indireta).</span><span class="sxs-lookup"><span data-stu-id="c8267-113">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c8267-114">ID do MPN do revendedor</span><span class="sxs-lookup"><span data-stu-id="c8267-114">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="c8267-115">Só aparece em arquivos de reconciliação para parceiros no modelo indireto.</span><span class="sxs-lookup"><span data-stu-id="c8267-115">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="c8267-116">A ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="c8267-116">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="c8267-117">Isso corresponde à ID de revendedor listada para a assinatura específica no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="c8267-117">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="c8267-118">Para exibir ou atualizar o revendedor, no menu Partner Center, selecione <strong>Clientes</strong>, em seguida, escolha o cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="c8267-118">eTo view or update the reseller, in the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="c8267-119">No menu do cliente, selecione <strong>Assinaturas</strong>, escolha a assinatura na lista.</span><span class="sxs-lookup"><span data-stu-id="c8267-119">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="c8267-120">Selecione <strong>Atualizar</strong> para alterar o <strong>Revendedor (ID do MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="c8267-120">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="c8267-121">Se um parceiro CSP vendeu a assinatura diretamente para o cliente, sua ID do MPN estará listada duas vezes, como a ID do MPN e a ID do MPN do revendedor.</span><span class="sxs-lookup"><span data-stu-id="c8267-121">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="c8267-122">Se um parceiro CSP tiver um revendedor sem ID do MPN, esse valor será definido como a ID do MPN do parceiro.</span><span class="sxs-lookup"><span data-stu-id="c8267-122">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="c8267-123">Se o parceiro CSP remover uma ID de revendedor, esse valor será definido como -1.</span><span class="sxs-lookup"><span data-stu-id="c8267-123">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="c8267-124">Campos de arquivo de licença</span><span class="sxs-lookup"><span data-stu-id="c8267-124">License-based file fields</span></span>


<span data-ttu-id="c8267-125">Para reconciliar seus encargos com os pedidos de seu cliente, compare o campo Syndication\_Partner\_Subscription\_Number do arquivo de reconciliação com a ID de Assinatura do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="c8267-125">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="c8267-126"><strong>Coluna</strong></span><span class="sxs-lookup"><span data-stu-id="c8267-126"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="c8267-127"><strong>Descrição</strong></span><span class="sxs-lookup"><span data-stu-id="c8267-127"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="c8267-128"><strong>Valor de exemplo</strong></span><span class="sxs-lookup"><span data-stu-id="c8267-128"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c8267-129">PartnerID</span><span class="sxs-lookup"><span data-stu-id="c8267-129">PartnerId</span></span></td>
<td><p><span data-ttu-id="c8267-130">Identificador exclusivo de uma entidade de cobrança específica, em formato GUID.</span><span class="sxs-lookup"><span data-stu-id="c8267-130">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="c8267-131">Não é necessário para reconciliação, mas pode ser uma informação útil.</span><span class="sxs-lookup"><span data-stu-id="c8267-131">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="c8267-132">O mesmo em todas as linhas.</span><span class="sxs-lookup"><span data-stu-id="c8267-132">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="c8267-133">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="c8267-133">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c8267-134">CustomerID</span><span class="sxs-lookup"><span data-stu-id="c8267-134">CustomerID</span></span></td>
<td><p><span data-ttu-id="c8267-135">ID exclusiva da Microsoft, no formato GUID, usada para identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="c8267-135">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="c8267-136">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="c8267-136">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c8267-137">OrderID</span><span class="sxs-lookup"><span data-stu-id="c8267-137">OrderID</span></span></td>
<td><p><span data-ttu-id="c8267-138">Identificador exclusivo para um pedido na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c8267-138">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="c8267-139">Pode ser útil para identificar o pedido ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="c8267-139">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="c8267-140">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="c8267-140">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c8267-141">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="c8267-141">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="c8267-142">Identificador exclusivo de uma assinatura na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c8267-142">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="c8267-143">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="c8267-143">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="c8267-144">Esse não é o mesmo que o ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="c8267-144">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="c8267-145">Consulte Número_Assinatura_Parceiro_Sindicalização.</span><span class="sxs-lookup"><span data-stu-id="c8267-145">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="c8267-146">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="c8267-146">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c8267-147">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="c8267-147">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="c8267-148">Identificador exclusivo para assinaturas.</span><span class="sxs-lookup"><span data-stu-id="c8267-148">Unique identifier for subscriptions.</span></span> <span data-ttu-id="c8267-149">Target: Um cliente pode ter várias assinaturas para o mesmo plano, portanto, isso é importante para análise de arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="c8267-149">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="c8267-150">Esse campo é mapeado para a ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="c8267-150">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="c8267-151">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="c8267-151">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c8267-152">OfferID</span><span class="sxs-lookup"><span data-stu-id="c8267-152">OfferID</span></span></td>
<td><p><span data-ttu-id="c8267-153">ID exclusivo da oferta.</span><span class="sxs-lookup"><span data-stu-id="c8267-153">Unique offer ID.</span></span> <span data-ttu-id="c8267-154">ID padrão da oferta de acordo com a lista de preços.</span><span class="sxs-lookup"><span data-stu-id="c8267-154">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="c8267-155"><b>Observação</b>: Esse valor não corresponde a ID da oferta da lista de preços.</span><span class="sxs-lookup"><span data-stu-id="c8267-155"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="c8267-156">Veja DurableOfferID abaixo.</span><span class="sxs-lookup"><span data-stu-id="c8267-156">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="c8267-157">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="c8267-157">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c8267-158">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="c8267-158">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="c8267-159">ID exclusivo da oferta durável, conforme definido na tabela de preços.</span><span class="sxs-lookup"><span data-stu-id="c8267-159">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="c8267-160"><b>Observação</b>: Esse valor corresponde à ID da oferta da lista de preços.</span><span class="sxs-lookup"><span data-stu-id="c8267-160"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="c8267-161">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="c8267-161">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c8267-162">OfferName</span><span class="sxs-lookup"><span data-stu-id="c8267-162">OfferName</span></span></td>
<td><p><span data-ttu-id="c8267-163">O nome da oferta de serviço comprada pelo cliente, conforme definido na tabela de preços.</span><span class="sxs-lookup"><span data-stu-id="c8267-163">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="c8267-164">Microsoft Office 365 (plano E3)</span><span class="sxs-lookup"><span data-stu-id="c8267-164">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c8267-165">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="c8267-165">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="c8267-166">A data de início da assinatura, definida como um dia após o pedido ser enviado.</span><span class="sxs-lookup"><span data-stu-id="c8267-166">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="c8267-167">Verificando a data de início da assinatura em conjunto com a data de término, você pode determinar se o cliente está dentro do primeiro ano da assinatura ou se a assinatura foi renovada para o ano seguinte.</span><span class="sxs-lookup"><span data-stu-id="c8267-167">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="c8267-168">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="c8267-168">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="c8267-169">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="c8267-169">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c8267-170">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="c8267-170">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="c8267-171">A data de término da assinatura: + x dias após a data de início (para alinhar com data de cobrança do parceiro) ou 12 meses a partir da data de renovação de 12 meses.</span><span class="sxs-lookup"><span data-stu-id="c8267-171">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="c8267-172">Na renovação, os preços são atualizados com a tabela de preços atual.</span><span class="sxs-lookup"><span data-stu-id="c8267-172">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="c8267-173">Um comunicado ao cliente pode ser necessário antes da renovação automática.</span><span class="sxs-lookup"><span data-stu-id="c8267-173">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="c8267-174">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="c8267-174">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="c8267-175">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="c8267-175">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c8267-176">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="c8267-176">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="c8267-177">Dia de início dos encargos.</span><span class="sxs-lookup"><span data-stu-id="c8267-177">Start day of the charges.</span></span></p>
<p><span data-ttu-id="c8267-178">Quando o cliente muda o número de assentos, esse número é usado para calcular os encargos por dia (pro-rata).</span><span class="sxs-lookup"><span data-stu-id="c8267-178">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="c8267-179">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="c8267-179">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="c8267-180">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="c8267-180">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c8267-181">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="c8267-181">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="c8267-182">Dia do término dos encargos.</span><span class="sxs-lookup"><span data-stu-id="c8267-182">End day of the charges.</span></span></p>
<p><span data-ttu-id="c8267-183">Quando o cliente muda o número de assentos, esse número é usado para calcular os encargos por dia (pro-rata).</span><span class="sxs-lookup"><span data-stu-id="c8267-183">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="c8267-184">A hora é sempre o fim do dia, 23:59.</span><span class="sxs-lookup"><span data-stu-id="c8267-184">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="c8267-185">28/2/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="c8267-185">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c8267-186">ChargeType</span><span class="sxs-lookup"><span data-stu-id="c8267-186">ChargeType</span></span></td>
<td><p><span data-ttu-id="c8267-187">O tipo de encargo ou ajuste.</span><span class="sxs-lookup"><span data-stu-id="c8267-187">The type of charge or adjustment.</span></span> <span data-ttu-id="c8267-188">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="c8267-188">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="c8267-189">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="c8267-189">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c8267-190">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="c8267-190">UnitPrice</span></span></td>
<td><p><span data-ttu-id="c8267-191">Preço por assento.</span><span class="sxs-lookup"><span data-stu-id="c8267-191">Price per seat.</span></span> <span data-ttu-id="c8267-192">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="c8267-192">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="c8267-193">6.82</span><span class="sxs-lookup"><span data-stu-id="c8267-193">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c8267-194">Quantidade</span><span class="sxs-lookup"><span data-stu-id="c8267-194">Quantity</span></span></td>
<td><p><span data-ttu-id="c8267-195">Número de assentos.</span><span class="sxs-lookup"><span data-stu-id="c8267-195">Number of seats.</span></span> <span data-ttu-id="c8267-196">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="c8267-196">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="c8267-197">2</span><span class="sxs-lookup"><span data-stu-id="c8267-197">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c8267-198">Valor</span><span class="sxs-lookup"><span data-stu-id="c8267-198">Amount</span></span></td>
<td><p><span data-ttu-id="c8267-199">Preço total por quantidade.</span><span class="sxs-lookup"><span data-stu-id="c8267-199">Total of price for quantity.</span></span> <span data-ttu-id="c8267-200">Útil para verificar se o cálculo do valor coincide com a forma como você calcula isso para seus clientes.</span><span class="sxs-lookup"><span data-stu-id="c8267-200">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="c8267-201">13.32</span><span class="sxs-lookup"><span data-stu-id="c8267-201">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c8267-202">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="c8267-202">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="c8267-203">Valor de desconto aplicado a esses encargos.</span><span class="sxs-lookup"><span data-stu-id="c8267-203">Amount of discount applied to these charges.</span></span> <span data-ttu-id="c8267-204">IUR ou novas assinaturas qualificadas para incentivo também conterão um valor de desconto nessa coluna.</span><span class="sxs-lookup"><span data-stu-id="c8267-204">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="c8267-205">2.32</span><span class="sxs-lookup"><span data-stu-id="c8267-205">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c8267-206">Subtotal</span><span class="sxs-lookup"><span data-stu-id="c8267-206">Subtotal</span></span></td>
<td><p><span data-ttu-id="c8267-207">Total sem imposto.</span><span class="sxs-lookup"><span data-stu-id="c8267-207">Total before tax.</span></span> <span data-ttu-id="c8267-208">Verifica se seu subtotal corresponde ao total esperado, em caso de desconto.</span><span class="sxs-lookup"><span data-stu-id="c8267-208">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="c8267-209">11</span><span class="sxs-lookup"><span data-stu-id="c8267-209">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c8267-210">Tax</span><span class="sxs-lookup"><span data-stu-id="c8267-210">Tax</span></span></td>
<td><p><span data-ttu-id="c8267-211">Valor do imposto cobrado, com base nas regras fiscais do mercado e em circunstâncias específicas.</span><span class="sxs-lookup"><span data-stu-id="c8267-211">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="c8267-212">0</span><span class="sxs-lookup"><span data-stu-id="c8267-212">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c8267-213">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="c8267-213">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="c8267-214">Total com imposto.</span><span class="sxs-lookup"><span data-stu-id="c8267-214">Total after tax.</span></span> <span data-ttu-id="c8267-215">Verifica se o imposto é cobrado na fatura.</span><span class="sxs-lookup"><span data-stu-id="c8267-215">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="c8267-216">11</span><span class="sxs-lookup"><span data-stu-id="c8267-216">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c8267-217">Currency</span><span class="sxs-lookup"><span data-stu-id="c8267-217">Currency</span></span></td>
<td><p><span data-ttu-id="c8267-218">Tipo de moeda.</span><span class="sxs-lookup"><span data-stu-id="c8267-218">Currency type.</span></span> <span data-ttu-id="c8267-219">Cada entidade de cobrança tem somente uma moeda.</span><span class="sxs-lookup"><span data-stu-id="c8267-219">Each billing entity has only one currency.</span></span> <span data-ttu-id="c8267-220">Verifique se isso coincide com a primeira fatura e faça o mesmo após grandes atualizações na plataforma de cobrança.</span><span class="sxs-lookup"><span data-stu-id="c8267-220">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="c8267-221">CNY</span><span class="sxs-lookup"><span data-stu-id="c8267-221">CNY</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c8267-222">CustomerName</span><span class="sxs-lookup"><span data-stu-id="c8267-222">CustomerName</span></span></td>
<td><p><span data-ttu-id="c8267-223">Nome da organização do cliente como informado no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="c8267-223">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="c8267-224">Isso é muito importante para reconciliar a fatura com as informações de seu sistema.</span><span class="sxs-lookup"><span data-stu-id="c8267-224">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="c8267-225">Cliente de teste A</span><span class="sxs-lookup"><span data-stu-id="c8267-225">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c8267-226">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="c8267-226">MPNID</span></span></td>
<td><p><span data-ttu-id="c8267-227">ID do MPN do parceiro CSP</span><span class="sxs-lookup"><span data-stu-id="c8267-227">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="c8267-228">4390934</span><span class="sxs-lookup"><span data-stu-id="c8267-228">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c8267-229">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="c8267-229">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="c8267-230">ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="c8267-230">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="c8267-231">Consulte [Discriminar por parceiro](#itemizebypartner).</span><span class="sxs-lookup"><span data-stu-id="c8267-231">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="c8267-232">4390934</span><span class="sxs-lookup"><span data-stu-id="c8267-232">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c8267-233">DomainName</span><span class="sxs-lookup"><span data-stu-id="c8267-233">DomainName</span></span></td>
<td><p><span data-ttu-id="c8267-234">Nome de domínio do cliente, usado para ajudar a identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="c8267-234">Customer's domain name, used to help identify the customer.</span></span></p></td>
<td><span data-ttu-id="c8267-235">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="c8267-235">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c8267-236">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="c8267-236">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="c8267-237">Apelido da Inscrição.</span><span class="sxs-lookup"><span data-stu-id="c8267-237">Subscription nickname.</span></span> <span data-ttu-id="c8267-238">Se nenhum apelido for especificado, o Partner Center usa o OfferName.</span><span class="sxs-lookup"><span data-stu-id="c8267-238">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="c8267-239">PROJETO ONLINE</span><span class="sxs-lookup"><span data-stu-id="c8267-239">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c8267-240">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="c8267-240">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="c8267-241">O nome da oferta de serviço comprada pelo cliente, conforme definido na tabela de preços.</span><span class="sxs-lookup"><span data-stu-id="c8267-241">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="c8267-242">(Este é um campo idêntico ao nome da oferta).</span><span class="sxs-lookup"><span data-stu-id="c8267-242">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="c8267-243">PROJETO ONLINE PREMIUM SEM PROJETO CLIENTE</span><span class="sxs-lookup"><span data-stu-id="c8267-243">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="c8267-244">Campos de arquivo baseada em uso</span><span class="sxs-lookup"><span data-stu-id="c8267-244">Usage-based file fields</span></span>


<span data-ttu-id="c8267-245">Para reconciliar seus encargos com o uso de seu cliente, compare ResellerID/ResellerName/ResellerBillableAccount do arquivo de reconciliação com o nome do cliente e a ID da assinatura do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="c8267-245">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="c8267-246">Os campos a seguir explicam quais serviços foram usados e a taxa.</span><span class="sxs-lookup"><span data-stu-id="c8267-246">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="c8267-247"><strong>Coluna</strong></span><span class="sxs-lookup"><span data-stu-id="c8267-247"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="c8267-248"><strong>Descrição</strong></span><span class="sxs-lookup"><span data-stu-id="c8267-248"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="c8267-249"><strong>Valor de exemplo</strong></span><span class="sxs-lookup"><span data-stu-id="c8267-249"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c8267-250">PartnerID</span><span class="sxs-lookup"><span data-stu-id="c8267-250">PartnerID</span></span></td>
<td><p><span data-ttu-id="c8267-251">ID do parceiro, no formato GUID.</span><span class="sxs-lookup"><span data-stu-id="c8267-251">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="c8267-252">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="c8267-252">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c8267-253">PartnerName</span><span class="sxs-lookup"><span data-stu-id="c8267-253">PartnerName</span></span></td>
<td><p><span data-ttu-id="c8267-254">Nome do parceiro.</span><span class="sxs-lookup"><span data-stu-id="c8267-254">Partner Name.</span></span></p></td>
<td><span data-ttu-id="c8267-255">Acme incorporado</span><span class="sxs-lookup"><span data-stu-id="c8267-255">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c8267-256">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="c8267-256">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="c8267-257">ID da conta do parceiro.</span><span class="sxs-lookup"><span data-stu-id="c8267-257">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="c8267-258">1010578050</span><span class="sxs-lookup"><span data-stu-id="c8267-258">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c8267-259">CustomerName</span><span class="sxs-lookup"><span data-stu-id="c8267-259">CustomerName</span></span></td>
<td><p><span data-ttu-id="c8267-260">Nome da organização do cliente como informado no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="c8267-260">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="c8267-261">Isso é muito importante para reconciliar a fatura com as informações de seu sistema.</span><span class="sxs-lookup"><span data-stu-id="c8267-261">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="c8267-262">Cliente de teste A</span><span class="sxs-lookup"><span data-stu-id="c8267-262">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c8267-263">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="c8267-263">MPNID</span></span></td>
<td><p><span data-ttu-id="c8267-264">ID do MPN do parceiro CSP.</span><span class="sxs-lookup"><span data-stu-id="c8267-264">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="c8267-265">4390934</span><span class="sxs-lookup"><span data-stu-id="c8267-265">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c8267-266">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="c8267-266">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="c8267-267">ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="c8267-267">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="c8267-268">Consulte [Discriminar por parceiro](#itemizebypartner).</span><span class="sxs-lookup"><span data-stu-id="c8267-268">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="c8267-269">4390934</span><span class="sxs-lookup"><span data-stu-id="c8267-269">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c8267-270">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="c8267-270">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="c8267-271">Número da fatura na qual a transação especificada é exibida.</span><span class="sxs-lookup"><span data-stu-id="c8267-271">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="c8267-272">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="c8267-272">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c8267-273">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="c8267-273">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="c8267-274">Data de início do ciclo de cobrança exceto quando apresentadas as datas de dados de uso latentes anteriormente não cobradas (do ciclo de cobrança anterior).</span><span class="sxs-lookup"><span data-stu-id="c8267-274">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="c8267-275">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="c8267-275">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="c8267-276">1/2/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="c8267-276">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c8267-277">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="c8267-277">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="c8267-278">Data de término do ciclo de cobrança exceto quando apresentadas as datas de dados de uso latentes anteriormente não cobradas (do ciclo de cobrança anterior).</span><span class="sxs-lookup"><span data-stu-id="c8267-278">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="c8267-279">A hora é sempre o fim do dia, 23:59.</span><span class="sxs-lookup"><span data-stu-id="c8267-279">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="c8267-280">28/2/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="c8267-280">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c8267-281">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="c8267-281">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="c8267-282">Identificador exclusivo de uma assinatura na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c8267-282">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="c8267-283">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="c8267-283">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="c8267-284">Esse não é o mesmo que o ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="c8267-284">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="c8267-285">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="c8267-285">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c8267-286">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="c8267-286">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="c8267-287">Apelido da oferta do serviço.</span><span class="sxs-lookup"><span data-stu-id="c8267-287">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="c8267-288">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="c8267-288">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c8267-289">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="c8267-289">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="c8267-290">Linha de negócios da oferta do serviço</span><span class="sxs-lookup"><span data-stu-id="c8267-290">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="c8267-291">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="c8267-291">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c8267-292">OrderID</span><span class="sxs-lookup"><span data-stu-id="c8267-292">OrderID</span></span></td>
<td><p><span data-ttu-id="c8267-293">Identificador exclusivo para um pedido na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c8267-293">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="c8267-294">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="c8267-294">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="c8267-295">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="c8267-295">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c8267-296">ServiceName</span><span class="sxs-lookup"><span data-stu-id="c8267-296">ServiceName</span></span></td>
<td><p><span data-ttu-id="c8267-297">O nome do serviço do Azure em questão.</span><span class="sxs-lookup"><span data-stu-id="c8267-297">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="c8267-298">MÁQUINAS VIRTUAIS</span><span class="sxs-lookup"><span data-stu-id="c8267-298">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c8267-299">ServiceType</span><span class="sxs-lookup"><span data-stu-id="c8267-299">ServiceType</span></span></td>
<td><p><span data-ttu-id="c8267-300">O tipo específico de serviço do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="c8267-300">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="c8267-301">Service Bus – Individual ou pacote</span><span class="sxs-lookup"><span data-stu-id="c8267-301">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="c8267-302">Banco de dados SQL Azure – Edição empresa ou Web</span><span class="sxs-lookup"><span data-stu-id="c8267-302">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c8267-303">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="c8267-303">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="c8267-304">Identificador exclusivo específico de toda a estrutura de serviço de dados e preço.</span><span class="sxs-lookup"><span data-stu-id="c8267-304">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="c8267-305">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="c8267-305">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c8267-306">Nome do recurso</span><span class="sxs-lookup"><span data-stu-id="c8267-306">Resource Name</span></span></td>
<td><p><span data-ttu-id="c8267-307">O nome do recurso do Azure.</span><span class="sxs-lookup"><span data-stu-id="c8267-307">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="c8267-308">Dados de entrada transferidos (GB)</span><span class="sxs-lookup"><span data-stu-id="c8267-308">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="c8267-309">Dados de saída transferidos (GB)</span><span class="sxs-lookup"><span data-stu-id="c8267-309">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c8267-310">Region</span><span class="sxs-lookup"><span data-stu-id="c8267-310">Region</span></span></td>
<td><p><span data-ttu-id="c8267-311">A região a qual o uso se aplica.</span><span class="sxs-lookup"><span data-stu-id="c8267-311">The region the usage applies to.</span></span> <span data-ttu-id="c8267-312">Usado principalmente para atribuir as taxas de transferências de dados, já que as taxas variam de acordo com a região.</span><span class="sxs-lookup"><span data-stu-id="c8267-312">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="c8267-313">Pacífico Asiático, Europa, América Latina e América do Norte</span><span class="sxs-lookup"><span data-stu-id="c8267-313">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c8267-314">SKU</span><span class="sxs-lookup"><span data-stu-id="c8267-314">SKU</span></span></td>
<td><p><span data-ttu-id="c8267-315">Identificador exclusivo MSFT da oferta</span><span class="sxs-lookup"><span data-stu-id="c8267-315">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="c8267-316">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="c8267-316">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="c8267-317">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="c8267-317">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="c8267-318">Uma ID e a quantidade para discriminar as taxas diferentes de um serviço ou recurso em um determinado período de cobrança.</span><span class="sxs-lookup"><span data-stu-id="c8267-318">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="c8267-319">Para a classificação em camadas do Azure, pode haver uma taxa para uma determinada quantidade de unidades faturáveis e uma taxa diferente depois disso.</span><span class="sxs-lookup"><span data-stu-id="c8267-319">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="c8267-320">1</span><span class="sxs-lookup"><span data-stu-id="c8267-320">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c8267-321">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="c8267-321">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="c8267-322">A quantidade de serviço consumida (horas, GB etc.) durante o período de relatório.</span><span class="sxs-lookup"><span data-stu-id="c8267-322">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="c8267-323">Também inclui qualquer uso não cobrado de períodos de relatório anteriores.</span><span class="sxs-lookup"><span data-stu-id="c8267-323">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="c8267-324">11</span><span class="sxs-lookup"><span data-stu-id="c8267-324">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c8267-325">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="c8267-325">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="c8267-326">Unidades incluídas como parte da oferta.</span><span class="sxs-lookup"><span data-stu-id="c8267-326">Units included as part of the offer.</span></span> <span data-ttu-id="c8267-327">Normalmente não está presente no CSP.</span><span class="sxs-lookup"><span data-stu-id="c8267-327">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="c8267-328">0</span><span class="sxs-lookup"><span data-stu-id="c8267-328">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="c8267-329">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="c8267-329">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="c8267-330">Unidades não incluídas como parte da oferta devem ser pagas pelo parceiro.</span><span class="sxs-lookup"><span data-stu-id="c8267-330">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="c8267-331">Igual a ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="c8267-331">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="c8267-332">11</span><span class="sxs-lookup"><span data-stu-id="c8267-332">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c8267-333">ListPrice</span><span class="sxs-lookup"><span data-stu-id="c8267-333">ListPrice</span></span></td>
<td><p><span data-ttu-id="c8267-334">Preço da oferta em vigor na data de início da assinatura.</span><span class="sxs-lookup"><span data-stu-id="c8267-334">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="c8267-335">U$ 0,0808</span><span class="sxs-lookup"><span data-stu-id="c8267-335">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c8267-336">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="c8267-336">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="c8267-337">ListPrist vezes OverageQuantity, arredondado para o centavo mais próximo.</span><span class="sxs-lookup"><span data-stu-id="c8267-337">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="c8267-338">U$ 0,085</span><span class="sxs-lookup"><span data-stu-id="c8267-338">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c8267-339">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="c8267-339">TaxAmount</span></span></td>
<td><p><span data-ttu-id="c8267-340">Valor do imposto cobrado, com base nas regras fiscais do mercado e em circunstâncias específicas.</span><span class="sxs-lookup"><span data-stu-id="c8267-340">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="c8267-341">U$ 0,08</span><span class="sxs-lookup"><span data-stu-id="c8267-341">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c8267-342">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="c8267-342">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="c8267-343">Total após imposto, quando o imposto é aplicável.</span><span class="sxs-lookup"><span data-stu-id="c8267-343">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="c8267-344">U$ 0,93</span><span class="sxs-lookup"><span data-stu-id="c8267-344">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c8267-345">Currency</span><span class="sxs-lookup"><span data-stu-id="c8267-345">Currency</span></span></td>
<td><p><span data-ttu-id="c8267-346">Tipo de moeda.</span><span class="sxs-lookup"><span data-stu-id="c8267-346">Currency type.</span></span> <span data-ttu-id="c8267-347">Cada entidade de cobrança tem somente uma moeda.</span><span class="sxs-lookup"><span data-stu-id="c8267-347">Each billing entity has only one currency.</span></span> <span data-ttu-id="c8267-348">Verifique se isso coincide com a primeira fatura e faça o mesmo após grandes atualizações na plataforma de cobrança.</span><span class="sxs-lookup"><span data-stu-id="c8267-348">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="c8267-349">CNY</span><span class="sxs-lookup"><span data-stu-id="c8267-349">CNY</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c8267-350">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="c8267-350">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="c8267-351">Preço por unidade sem imposto.</span><span class="sxs-lookup"><span data-stu-id="c8267-351">Pretax price per unit.</span></span> <span data-ttu-id="c8267-352">Igual a PretaxCharges / OverageQuantity, arredondado para o centavo mais próximo.</span><span class="sxs-lookup"><span data-stu-id="c8267-352">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="c8267-353">U$ 0,08</span><span class="sxs-lookup"><span data-stu-id="c8267-353">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c8267-354">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="c8267-354">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="c8267-355">Preço pós-imposto por unidade.</span><span class="sxs-lookup"><span data-stu-id="c8267-355">Post tax price per unit.</span></span> <span data-ttu-id="c8267-356">Igual a PostTaxTotal / OverageQuantity, ou PretaxEffectiveRate + taxa de imposto por valor de unidade, arredondado para o centavo mais próximo.</span><span class="sxs-lookup"><span data-stu-id="c8267-356">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="c8267-357">U$ 0,08</span><span class="sxs-lookup"><span data-stu-id="c8267-357">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c8267-358">ChargeType</span><span class="sxs-lookup"><span data-stu-id="c8267-358">ChargeType</span></span></td>
<td><p><span data-ttu-id="c8267-359">O tipo de encargo ou ajuste.</span><span class="sxs-lookup"><span data-stu-id="c8267-359">The type of charge or adjustment.</span></span> <span data-ttu-id="c8267-360">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="c8267-360">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="c8267-361">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="c8267-361">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c8267-362">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="c8267-362">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="c8267-363">ID exclusiva da conta na plataforma de cobrança da MSFT.</span><span class="sxs-lookup"><span data-stu-id="c8267-363">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="c8267-364">1280018095</span><span class="sxs-lookup"><span data-stu-id="c8267-364">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c8267-365">UsageDate</span><span class="sxs-lookup"><span data-stu-id="c8267-365">UsageDate</span></span></td>
<td><p><span data-ttu-id="c8267-366">Data da implantação do serviço.</span><span class="sxs-lookup"><span data-stu-id="c8267-366">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="c8267-367">1/2/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="c8267-367">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c8267-368">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="c8267-368">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="c8267-369">Essa coluna identifica a localização de um data center dentro da região para serviços onde isso é aplicável e preenchido.</span><span class="sxs-lookup"><span data-stu-id="c8267-369">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="c8267-370">Leste da Ásia, Sudeste da Ásia, Norte da Europa, Europa Ocidental, Centro Norte e Centro Sul dos EUA</span><span class="sxs-lookup"><span data-stu-id="c8267-370">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c8267-371">MeteredService</span><span class="sxs-lookup"><span data-stu-id="c8267-371">MeteredService</span></span></td>
<td><p><span data-ttu-id="c8267-372">Essa coluna é utilizada para rastrear o serviço do Microsoft Azure individual que não pode ser identificado especificamente na coluna Nome do Serviço.</span><span class="sxs-lookup"><span data-stu-id="c8267-372">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="c8267-373">Por exemplo, transferências de dados são relatadas como &quot;Microsoft Azure – Todos os Serviços&quot; na coluna Nome do Serviço.</span><span class="sxs-lookup"><span data-stu-id="c8267-373">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="c8267-374">Essa coluna MeteredService indicará ao qual serviço específico o uso pertence.</span><span class="sxs-lookup"><span data-stu-id="c8267-374">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="c8267-375">AccessControl, CDN, Computação, Banco de dados, ServiceBus, Armazenamento</span><span class="sxs-lookup"><span data-stu-id="c8267-375">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c8267-376">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="c8267-376">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="c8267-377">Um subcabeçalho que esclarece ainda mais o serviço Microsoft Azure individual além do nível fornecido pelo campo MeteredService.</span><span class="sxs-lookup"><span data-stu-id="c8267-377">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="c8267-378">EXTERNO</span><span class="sxs-lookup"><span data-stu-id="c8267-378">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c8267-379">Projeto</span><span class="sxs-lookup"><span data-stu-id="c8267-379">Project</span></span></td>
<td><p><span data-ttu-id="c8267-380">Nome definido pelo cliente para a instância do serviço</span><span class="sxs-lookup"><span data-stu-id="c8267-380">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="c8267-381">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="c8267-381">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c8267-382">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="c8267-382">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="c8267-383">O número de conexões ServiceBus que foram provisionados e utilizados em um dia específico.</span><span class="sxs-lookup"><span data-stu-id="c8267-383">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="c8267-384">Por exemplo: se você tivesse uma conexão individualmente provisionada durante um mês de 30 dias, a coluna Informação do Serviço 1 lerá "1,000000 conexões/30 dias".</span><span class="sxs-lookup"><span data-stu-id="c8267-384">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="c8267-385">Se você tivesse um pacote de 25 de conexões de barramento de serviço provisionado e você tinha utilizou 1 durante o dia, sua instrução de uso diário para esse dia indicaria "25 conexões / 30 dias – usado: 1.000000”.</span><span class="sxs-lookup"><span data-stu-id="c8267-385">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c8267-386">CustomerID</span><span class="sxs-lookup"><span data-stu-id="c8267-386">CustomerID</span></span></td>
<td><p><span data-ttu-id="c8267-387">ID exclusiva da Microsoft, no formato GUID, usada para identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="c8267-387">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="c8267-388">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="c8267-388">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c8267-389">DomainName</span><span class="sxs-lookup"><span data-stu-id="c8267-389">DomainName</span></span></td>
<td><p><span data-ttu-id="c8267-390">Nome de domínio do cliente, usado para ajudar a identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="c8267-390">Customer's domain name, used to help identify the customer.</span></span></p></td>
<td><span data-ttu-id="c8267-391">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="c8267-391">example.onmicrosoft.com</span></span></td></tr>
</tbody>
</table>



## <a href="" id="charge_types"></a><span data-ttu-id="c8267-392">Encargos de mapeamento entre uma nota fiscal e o arquivo de reconciliação</span><span class="sxs-lookup"><span data-stu-id="c8267-392">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="c8267-393">Sua fatura fornece um resumo dos encargos, enquanto seu arquivo de reconciliação fornece uma divisão detalhada das transações de item de linha, incluindo os tipos de carga.</span><span class="sxs-lookup"><span data-stu-id="c8267-393">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="c8267-394">Para fazer referência cruzada das quantidades de carga entre o arquivo de reconciliação e fatura, você pode usar opções de filtro do Microsoft Excel para filtrar por tipos de cobrança no arquivo de reconciliação para mapear os encargos de fatura em um conjunto de detalhamentos de cobrança no arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="c8267-394">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="c8267-395">A tabela a seguir mostra os mapeamentos entre uma seção da fatura e os tipos de encargo associados que podem aparecer nos arquivos de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="c8267-395">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="c8267-396"><strong>Descrição de encargo de fatura</strong></span><span class="sxs-lookup"><span data-stu-id="c8267-396"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="c8267-397"><strong>Descrição de cobrança de arquivo de reconciliação (ChargeType coluna)</strong></span><span class="sxs-lookup"><span data-stu-id="c8267-397"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="c8267-398"><strong>O que é a cobrança?</strong></span><span class="sxs-lookup"><span data-stu-id="c8267-398"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="c8267-399"><strong>Como faço para mapear esses ChargeTypes à fatura?</strong></span><span class="sxs-lookup"><span data-stu-id="c8267-399"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="8">
<p><span data-ttu-id="c8267-400"><strong>Encargos recorrentes</strong></span><span class="sxs-lookup"><span data-stu-id="c8267-400"><strong>Recurring Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="c8267-401">Cancelar ocorrência proporcional</span><span class="sxs-lookup"><span data-stu-id="c8267-401">Cancel instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="c8267-402">Os encargos proporcionais reembolsados para o cliente quando os assentos associados são alterados</span><span class="sxs-lookup"><span data-stu-id="c8267-402">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
<td rowspan="8">
<p><span data-ttu-id="c8267-403">No arquivo baseado em licença, some a coluna <strong>Quantidade</strong></span><span class="sxs-lookup"><span data-stu-id="c8267-403">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="c8267-404">Taxa do ciclo</span><span class="sxs-lookup"><span data-stu-id="c8267-404">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="c8267-405">Encargos periódicos de uma assinatura</span><span class="sxs-lookup"><span data-stu-id="c8267-405">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="c8267-406">Proporcional à instância do ciclo</span><span class="sxs-lookup"><span data-stu-id="c8267-406">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="c8267-407">Os encargos proporcionais cobrados do cliente quando os assentos associados são alterados</span><span class="sxs-lookup"><span data-stu-id="c8267-407">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="c8267-408">Taxas proporcionais durante o cancelamento</span><span class="sxs-lookup"><span data-stu-id="c8267-408">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="c8267-409">Reembolso proporcional para a parte não utilizada do serviço após o cancelamento</span><span class="sxs-lookup"><span data-stu-id="c8267-409">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="c8267-410">Taxas proporcionais durante a compra</span><span class="sxs-lookup"><span data-stu-id="c8267-410">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="c8267-411">Taxas proporcionais após a compra</span><span class="sxs-lookup"><span data-stu-id="c8267-411">Prorated fees upon purchase</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="c8267-412">Valor de compra</span><span class="sxs-lookup"><span data-stu-id="c8267-412">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="c8267-413">Encargo inicial de uma assinatura</span><span class="sxs-lookup"><span data-stu-id="c8267-413">Initial charge for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="c8267-414">Taxa proporcional ao renovar</span><span class="sxs-lookup"><span data-stu-id="c8267-414">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="c8267-415">Taxas proporcionais após a renovação da assinatura</span><span class="sxs-lookup"><span data-stu-id="c8267-415">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="c8267-416">Taxa de renovação</span><span class="sxs-lookup"><span data-stu-id="c8267-416">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="c8267-417">Cobrança para renovação de uma assinatura</span><span class="sxs-lookup"><span data-stu-id="c8267-417">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="c8267-418"><strong>Outros produtos e serviços</strong></span><span class="sxs-lookup"><span data-stu-id="c8267-418"><strong>Other Products and Services</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="c8267-419">Taxas proporcionais ao ativar</span><span class="sxs-lookup"><span data-stu-id="c8267-419">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="c8267-420">Taxas proporcionais da ativação até o final do período de cobrança</span><span class="sxs-lookup"><span data-stu-id="c8267-420">Prorated fees from activation until end of billing period</span></span></p>
</td>
<td>
<p><span data-ttu-id="c8267-421">No arquivo baseado em licença, some a coluna <strong>Quantidade</strong></span><span class="sxs-lookup"><span data-stu-id="c8267-421">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><span data-ttu-id="c8267-422"><strong>Encargos de uso</strong></span><span class="sxs-lookup"><span data-stu-id="c8267-422"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="c8267-423">Avaliar a taxa de uso ao cancelar</span><span class="sxs-lookup"><span data-stu-id="c8267-423">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="c8267-424">Taxa de uso de acesso com o cancelamento para uso não pago durante o período de cobrança atual</span><span class="sxs-lookup"><span data-stu-id="c8267-424">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="c8267-425">No arquivo baseado em uso, some a coluna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="c8267-425">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="c8267-426">Avalie a taxa de uso para o ciclo atual</span><span class="sxs-lookup"><span data-stu-id="c8267-426">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="c8267-427">Taxa de uso de acesso para o período atual de cobrança</span><span class="sxs-lookup"><span data-stu-id="c8267-427">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="c8267-428"><strong>Créditos &amp; ajustes</strong></span><span class="sxs-lookup"><span data-stu-id="c8267-428"><strong>Credits &amp; Adjustments</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="c8267-429">Deslocando um item de linha</span><span class="sxs-lookup"><span data-stu-id="c8267-429">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="c8267-430">Reembolso parcial ou integral para um item de linha, incluindo os impostos</span><span class="sxs-lookup"><span data-stu-id="c8267-430">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="c8267-431">No arquivo baseado em licença, some a coluna <strong>TotalForCustomer</strong></span><span class="sxs-lookup"><span data-stu-id="c8267-431">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="c8267-432">No arquivo baseado em uso, some a coluna <strong>PostTaxTotal</strong></span><span class="sxs-lookup"><span data-stu-id="c8267-432">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>


<tr>
<td rowspan="4">
<p><span data-ttu-id="c8267-433"><strong>Outros descontos.</strong></span><span class="sxs-lookup"><span data-stu-id="c8267-433"><strong>Other Discounts</strong></span></span></br><span data-ttu-id="c8267-434">
<em>(com base em uso)</em></span><span class="sxs-lookup"><span data-stu-id="c8267-434">
<em>(usage-based)</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="c8267-435">Desconto de ativação</span><span class="sxs-lookup"><span data-stu-id="c8267-435">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="c8267-436">Desconto aplicado quando a assinatura é ativada</span><span class="sxs-lookup"><span data-stu-id="c8267-436">Discount applied when subscription activated</span></span></p>
</td>
<td rowspan="4">
<p><span data-ttu-id="c8267-437">No arquivo baseado em uso, some a coluna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="c8267-437">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="c8267-438">Desconto de ciclo</span><span class="sxs-lookup"><span data-stu-id="c8267-438">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="c8267-439">Desconto aplicado em cobranças periódicas</span><span class="sxs-lookup"><span data-stu-id="c8267-439">Discount applied on periodic charges</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="c8267-440">Desconto de renovação</span><span class="sxs-lookup"><span data-stu-id="c8267-440">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="c8267-441">Desconto aplicado quando a assinatura é renovada</span><span class="sxs-lookup"><span data-stu-id="c8267-441">Discount applied when subscription renewed</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="c8267-442">Desconto de cancelamento</span><span class="sxs-lookup"><span data-stu-id="c8267-442">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="c8267-443">Encargos aplicados quando descontos são cancelados</span><span class="sxs-lookup"><span data-stu-id="c8267-443">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="c8267-444"><strong>Outros descontos.</strong></span><span class="sxs-lookup"><span data-stu-id="c8267-444"><strong>Other Discounts</strong></span></span></br><span data-ttu-id="c8267-445">
<em>(baseados em licença)</em></span><span class="sxs-lookup"><span data-stu-id="c8267-445">
<em>(license-based)</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="c8267-446"><em>Pode ser aplicado a vários tipos de custo</em></span><span class="sxs-lookup"><span data-stu-id="c8267-446"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p>&nbsp;</p>
</td>
<td>
<p><span data-ttu-id="c8267-447">No arquivo baseado em licença, some a coluna <strong>TotalOtherDiscount</strong></span><span class="sxs-lookup"><span data-stu-id="c8267-447">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="c8267-448"><strong>Impostos</strong>&nbsp;ou&nbsp;<strong>IVA</strong></span><span class="sxs-lookup"><span data-stu-id="c8267-448"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="c8267-449"><em>Pode ser aplicado a vários tipos de custo</em></span><span class="sxs-lookup"><span data-stu-id="c8267-449"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="c8267-450"><em>Exceção: Já "Um item de linha de deslocamento" inclui os impostos. Ver créditos &amp; ajustes, acima.</em></span><span class="sxs-lookup"><span data-stu-id="c8267-450"><em>Exception: "Offset a line item" already includes taxes. See Credits &amp; Adjustments, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="c8267-451">Impostos ou impostos sobre valor agregado (IVA)</span><span class="sxs-lookup"><span data-stu-id="c8267-451">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="c8267-452">No arquivo baseado em licença, some a coluna <strong>Imposto</strong></span><span class="sxs-lookup"><span data-stu-id="c8267-452">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="c8267-453">No arquivo baseado em uso, some a coluna <strong>TaxAmount</strong></span><span class="sxs-lookup"><span data-stu-id="c8267-453">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
