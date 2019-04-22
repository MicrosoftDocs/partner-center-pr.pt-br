---
title: Usar os arquivos de reconciliação | Partner Center
ms.topic: article
ms.date: 10/29/2018
description: Para uma exibição detalhada do item de linha de cada carga, em um ciclo de cobrança, baixe os arquivos de reconciliação do Partner Center.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 0d986ca81e77578ecbb79b909d8f2a8afc4777e4
ms.sourcegitcommit: 7022f1e3d26751e66f90db96bf6d881cb2a694d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/18/2019
ms.locfileid: "59430195"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="30acf-103">Usar os arquivos de reconciliação</span><span class="sxs-lookup"><span data-stu-id="30acf-103">Use the reconciliation files</span></span>

<span data-ttu-id="30acf-104">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="30acf-104">**Applies to**</span></span>

-  <span data-ttu-id="30acf-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="30acf-105">Partner Center</span></span>
-  <span data-ttu-id="30acf-106">Partner Center para Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="30acf-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="30acf-107">Para uma exibição detalhada do item de linha de cada carga, em um ciclo de cobrança, baixe os arquivos de reconciliação do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="30acf-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="30acf-108">Os detalhes incluem encargos por assinaturas de cada cliente e eventos detalhados (como a adição de assentos a uma assinatura no meio do período).</span><span class="sxs-lookup"><span data-stu-id="30acf-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="30acf-109">Problemas de formatação</span><span class="sxs-lookup"><span data-stu-id="30acf-109">Formatting issues</span></span>

<span data-ttu-id="30acf-110">Ocasionalmente, seu arquivo de reconhecimento pode ter problemas de formatação.</span><span class="sxs-lookup"><span data-stu-id="30acf-110">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="30acf-111">(Isso pode acontecer, por exemplo, se a localidade EN-US não for usada.) Siga as etapas abaixo para corrigir esses problemas.</span><span class="sxs-lookup"><span data-stu-id="30acf-111">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="30acf-112">Abra o arquivo. csv no Excel e selecione a primeira coluna.</span><span class="sxs-lookup"><span data-stu-id="30acf-112">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="30acf-113">Na faixa de opções, selecione <strong>dados</strong>e, em seguida, selecione <strong>texto para colunas</strong>.</span><span class="sxs-lookup"><span data-stu-id="30acf-113">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="30acf-114">Na conversão de texto ao Assistente de colunas, selecione <strong>delimitada por tipo de arquivo</strong>e, em seguida, selecione <strong>próxima</strong>.</span><span class="sxs-lookup"><span data-stu-id="30acf-114">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="30acf-115">No campo dos delimitadores, selecione <strong>vírgula</strong>.</span><span class="sxs-lookup"><span data-stu-id="30acf-115">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="30acf-116">Se <strong>guia</strong> é estiver selecionado, você pode deixá-lo.</span><span class="sxs-lookup"><span data-stu-id="30acf-116">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="30acf-117">Selecione <strong>Avançar</strong>.</span><span class="sxs-lookup"><span data-stu-id="30acf-117">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="30acf-118">No campo de formato de dados de coluna, selecione <strong>data: MDY</strong>e, em seguida, selecione <strong>próxima</strong>.</span><span class="sxs-lookup"><span data-stu-id="30acf-118">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="30acf-119">No campo de formato de dados de coluna, selecione <strong>texto</strong> para o valor de todas as colunas e, em seguida, selecione <strong>concluir</strong>.</span><span class="sxs-lookup"><span data-stu-id="30acf-119">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="30acf-120">Discriminar pelo parceiro</span><span class="sxs-lookup"><span data-stu-id="30acf-120">Itemize by partner</span></span>


<span data-ttu-id="30acf-121">Os parceiros no modelo indireto podem usar esses campos adicionais nos arquivos de reconciliação baseados em uso e em licença para discriminar por revendedor.</span><span class="sxs-lookup"><span data-stu-id="30acf-121">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="30acf-122">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="30acf-122">MPN ID</span></span></th>
<th><span data-ttu-id="30acf-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="30acf-123">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="30acf-124">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="30acf-124">MPN ID</span></span></td>
<td><p><span data-ttu-id="30acf-125">A ID do Microsoft Partner Network (MPN) do parceiro CSP (direta ou indireta).</span><span class="sxs-lookup"><span data-stu-id="30acf-125">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="30acf-126">ID do MPN do revendedor</span><span class="sxs-lookup"><span data-stu-id="30acf-126">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="30acf-127">Só aparece em arquivos de reconciliação para parceiros no modelo indireto.</span><span class="sxs-lookup"><span data-stu-id="30acf-127">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="30acf-128">A ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="30acf-128">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="30acf-129">Isso corresponde à ID de revendedor listada para a assinatura específica no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="30acf-129">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="30acf-130">modo de exibição eTo ou atualização revendedor, no menu do Partner Center, selecione <strong>clientes</strong>, em seguida, escolha o cliente da lista.</span><span class="sxs-lookup"><span data-stu-id="30acf-130">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="30acf-131">No menu do cliente, selecione <strong>Assinaturas</strong>, escolha a assinatura na lista.</span><span class="sxs-lookup"><span data-stu-id="30acf-131">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="30acf-132">Selecione <strong>Atualizar</strong> para alterar o <strong>Revendedor (ID do MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="30acf-132">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="30acf-133">Se um parceiro CSP vendeu a assinatura diretamente para o cliente, sua ID do MPN estará listada duas vezes, como a ID do MPN e a ID do MPN do revendedor.</span><span class="sxs-lookup"><span data-stu-id="30acf-133">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="30acf-134">Se um parceiro CSP tiver um revendedor sem ID do MPN, esse valor será definido como a ID do MPN do parceiro.</span><span class="sxs-lookup"><span data-stu-id="30acf-134">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="30acf-135">Se o parceiro CSP remover uma ID de revendedor, esse valor será definido como -1.</span><span class="sxs-lookup"><span data-stu-id="30acf-135">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="30acf-136">Campos de arquivo de licença</span><span class="sxs-lookup"><span data-stu-id="30acf-136">License-based file fields</span></span>


<span data-ttu-id="30acf-137">Para reconciliar seus encargos com os pedidos de seu cliente, compare o campo Syndication\_Partner\_Subscription\_Number do arquivo de reconciliação com a ID de Assinatura do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="30acf-137">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="30acf-138"><strong>Coluna</strong></span><span class="sxs-lookup"><span data-stu-id="30acf-138"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="30acf-139"><strong>Descrição</strong></span><span class="sxs-lookup"><span data-stu-id="30acf-139"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="30acf-140"><strong>Valor de exemplo</strong></span><span class="sxs-lookup"><span data-stu-id="30acf-140"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="30acf-141">PartnerID</span><span class="sxs-lookup"><span data-stu-id="30acf-141">PartnerId</span></span></td>
<td><p><span data-ttu-id="30acf-142">Identificador exclusivo de uma entidade de cobrança específica, em formato GUID.</span><span class="sxs-lookup"><span data-stu-id="30acf-142">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="30acf-143">Não é necessário para reconciliação, mas pode ser uma informação útil.</span><span class="sxs-lookup"><span data-stu-id="30acf-143">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="30acf-144">O mesmo em todas as linhas.</span><span class="sxs-lookup"><span data-stu-id="30acf-144">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="30acf-145">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="30acf-145">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="30acf-146">CustomerID</span><span class="sxs-lookup"><span data-stu-id="30acf-146">CustomerID</span></span></td>
<td><p><span data-ttu-id="30acf-147">ID exclusiva da Microsoft, no formato GUID, usada para identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="30acf-147">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="30acf-148">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="30acf-148">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="30acf-149">OrderID</span><span class="sxs-lookup"><span data-stu-id="30acf-149">OrderID</span></span></td>
<td><p><span data-ttu-id="30acf-150">Identificador exclusivo para um pedido na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="30acf-150">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="30acf-151">Pode ser útil para identificar o pedido ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="30acf-151">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="30acf-152">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="30acf-152">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="30acf-153">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="30acf-153">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="30acf-154">Identificador exclusivo de uma assinatura na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="30acf-154">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="30acf-155">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="30acf-155">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="30acf-156">Esse não é o mesmo que o ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="30acf-156">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="30acf-157">Consulte Número_Assinatura_Parceiro_Sindicalização.</span><span class="sxs-lookup"><span data-stu-id="30acf-157">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="30acf-158">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="30acf-158">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="30acf-159">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="30acf-159">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="30acf-160">Identificador exclusivo para assinaturas.</span><span class="sxs-lookup"><span data-stu-id="30acf-160">Unique identifier for subscriptions.</span></span> <span data-ttu-id="30acf-161">Target: Um cliente pode ter várias assinaturas para o mesmo plano, portanto, isso é importante para análise de arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="30acf-161">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="30acf-162">Esse campo é mapeado para a ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="30acf-162">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="30acf-163">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="30acf-163">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="30acf-164">OfferID</span><span class="sxs-lookup"><span data-stu-id="30acf-164">OfferID</span></span></td>
<td><p><span data-ttu-id="30acf-165">ID exclusivo da oferta.</span><span class="sxs-lookup"><span data-stu-id="30acf-165">Unique offer ID.</span></span> <span data-ttu-id="30acf-166">ID padrão da oferta de acordo com a lista de preços.</span><span class="sxs-lookup"><span data-stu-id="30acf-166">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="30acf-167"><b>Observação</b>: Esse valor não corresponde a ID da oferta da lista de preços.</span><span class="sxs-lookup"><span data-stu-id="30acf-167"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="30acf-168">Veja DurableOfferID abaixo.</span><span class="sxs-lookup"><span data-stu-id="30acf-168">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="30acf-169">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="30acf-169">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="30acf-170">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="30acf-170">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="30acf-171">ID exclusivo da oferta durável, conforme definido na tabela de preços.</span><span class="sxs-lookup"><span data-stu-id="30acf-171">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="30acf-172"><b>Observação</b>: Esse valor corresponde à ID da oferta da lista de preços.</span><span class="sxs-lookup"><span data-stu-id="30acf-172"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="30acf-173">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="30acf-173">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="30acf-174">OfferName</span><span class="sxs-lookup"><span data-stu-id="30acf-174">OfferName</span></span></td>
<td><p><span data-ttu-id="30acf-175">O nome da oferta de serviço comprada pelo cliente, conforme definido na tabela de preços.</span><span class="sxs-lookup"><span data-stu-id="30acf-175">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="30acf-176">Microsoft Office 365 (plano E3)</span><span class="sxs-lookup"><span data-stu-id="30acf-176">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="30acf-177">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="30acf-177">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="30acf-178">A data de início da assinatura, definida como um dia após o pedido ser enviado.</span><span class="sxs-lookup"><span data-stu-id="30acf-178">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="30acf-179">Verificando a data de início da assinatura em conjunto com a data de término, você pode determinar se o cliente está dentro do primeiro ano da assinatura ou se a assinatura foi renovada para o ano seguinte.</span><span class="sxs-lookup"><span data-stu-id="30acf-179">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="30acf-180">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="30acf-180">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="30acf-181">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="30acf-181">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="30acf-182">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="30acf-182">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="30acf-183">A data de término da assinatura: + x dias após a data de início (para alinhar com data de cobrança do parceiro) ou 12 meses a partir da data de renovação de 12 meses.</span><span class="sxs-lookup"><span data-stu-id="30acf-183">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="30acf-184">Na renovação, os preços são atualizados com a tabela de preços atual.</span><span class="sxs-lookup"><span data-stu-id="30acf-184">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="30acf-185">Um comunicado ao cliente pode ser necessário antes da renovação automática.</span><span class="sxs-lookup"><span data-stu-id="30acf-185">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="30acf-186">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="30acf-186">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="30acf-187">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="30acf-187">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="30acf-188">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="30acf-188">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="30acf-189">Dia de início dos encargos.</span><span class="sxs-lookup"><span data-stu-id="30acf-189">Start day of the charges.</span></span></p>
<p><span data-ttu-id="30acf-190">Quando o cliente muda o número de assentos, esse número é usado para calcular os encargos por dia (pro-rata).</span><span class="sxs-lookup"><span data-stu-id="30acf-190">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="30acf-191">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="30acf-191">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="30acf-192">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="30acf-192">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="30acf-193">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="30acf-193">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="30acf-194">Dia do término dos encargos.</span><span class="sxs-lookup"><span data-stu-id="30acf-194">End day of the charges.</span></span></p>
<p><span data-ttu-id="30acf-195">Quando o cliente muda o número de assentos, esse número é usado para calcular os encargos por dia (pro-rata).</span><span class="sxs-lookup"><span data-stu-id="30acf-195">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="30acf-196">A hora é sempre o fim do dia, 23:59.</span><span class="sxs-lookup"><span data-stu-id="30acf-196">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="30acf-197">28/2/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="30acf-197">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="30acf-198">ChargeType</span><span class="sxs-lookup"><span data-stu-id="30acf-198">ChargeType</span></span></td>
<td><p><span data-ttu-id="30acf-199">O tipo de encargo ou ajuste.</span><span class="sxs-lookup"><span data-stu-id="30acf-199">The type of charge or adjustment.</span></span> <span data-ttu-id="30acf-200">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="30acf-200">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="30acf-201">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="30acf-201">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="30acf-202">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="30acf-202">UnitPrice</span></span></td>
<td><p><span data-ttu-id="30acf-203">Preço por estação, conforme publicado na lista de preços no momento da compra.</span><span class="sxs-lookup"><span data-stu-id="30acf-203">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="30acf-204">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="30acf-204">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="30acf-205">6.82</span><span class="sxs-lookup"><span data-stu-id="30acf-205">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="30acf-206">Quantidade</span><span class="sxs-lookup"><span data-stu-id="30acf-206">Quantity</span></span></td>
<td><p><span data-ttu-id="30acf-207">Número de assentos.</span><span class="sxs-lookup"><span data-stu-id="30acf-207">Number of seats.</span></span> <span data-ttu-id="30acf-208">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="30acf-208">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="30acf-209">2</span><span class="sxs-lookup"><span data-stu-id="30acf-209">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="30acf-210">Valor</span><span class="sxs-lookup"><span data-stu-id="30acf-210">Amount</span></span></td>
<td><p><span data-ttu-id="30acf-211">Preço total por quantidade.</span><span class="sxs-lookup"><span data-stu-id="30acf-211">Total of price for quantity.</span></span> <span data-ttu-id="30acf-212">Útil para verificar se o cálculo do valor coincide com a forma como você calcula isso para seus clientes.</span><span class="sxs-lookup"><span data-stu-id="30acf-212">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="30acf-213">13.32</span><span class="sxs-lookup"><span data-stu-id="30acf-213">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="30acf-214">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="30acf-214">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="30acf-215">Valor de desconto aplicado a esses encargos.</span><span class="sxs-lookup"><span data-stu-id="30acf-215">Amount of discount applied to these charges.</span></span> <span data-ttu-id="30acf-216">IUR ou novas assinaturas qualificadas para incentivo também conterão um valor de desconto nessa coluna.</span><span class="sxs-lookup"><span data-stu-id="30acf-216">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="30acf-217">2.32</span><span class="sxs-lookup"><span data-stu-id="30acf-217">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="30acf-218">Subtotal</span><span class="sxs-lookup"><span data-stu-id="30acf-218">Subtotal</span></span></td>
<td><p><span data-ttu-id="30acf-219">Total sem imposto.</span><span class="sxs-lookup"><span data-stu-id="30acf-219">Total before tax.</span></span> <span data-ttu-id="30acf-220">Verifica se seu subtotal corresponde ao total esperado, em caso de desconto.</span><span class="sxs-lookup"><span data-stu-id="30acf-220">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="30acf-221">11</span><span class="sxs-lookup"><span data-stu-id="30acf-221">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="30acf-222">Tax</span><span class="sxs-lookup"><span data-stu-id="30acf-222">Tax</span></span></td>
<td><p><span data-ttu-id="30acf-223">Encargo de valor, com base em seu mercado de imposto&#39;regras de imposto de s e as circunstâncias específicas.</span><span class="sxs-lookup"><span data-stu-id="30acf-223">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="30acf-224">0</span><span class="sxs-lookup"><span data-stu-id="30acf-224">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="30acf-225">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="30acf-225">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="30acf-226">Total com imposto.</span><span class="sxs-lookup"><span data-stu-id="30acf-226">Total after tax.</span></span> <span data-ttu-id="30acf-227">Verifica se o imposto é cobrado na fatura.</span><span class="sxs-lookup"><span data-stu-id="30acf-227">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="30acf-228">11</span><span class="sxs-lookup"><span data-stu-id="30acf-228">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="30acf-229">Currency</span><span class="sxs-lookup"><span data-stu-id="30acf-229">Currency</span></span></td>
<td><p><span data-ttu-id="30acf-230">Tipo de moeda.</span><span class="sxs-lookup"><span data-stu-id="30acf-230">Currency type.</span></span> <span data-ttu-id="30acf-231">Cada entidade de cobrança tem somente uma moeda.</span><span class="sxs-lookup"><span data-stu-id="30acf-231">Each billing entity has only one currency.</span></span> <span data-ttu-id="30acf-232">Verifique se isso coincide com a primeira fatura e faça o mesmo após grandes atualizações na plataforma de cobrança.</span><span class="sxs-lookup"><span data-stu-id="30acf-232">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="30acf-233">EUR</span><span class="sxs-lookup"><span data-stu-id="30acf-233">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="30acf-234">CustomerName</span><span class="sxs-lookup"><span data-stu-id="30acf-234">CustomerName</span></span></td>
<td><p><span data-ttu-id="30acf-235">Cliente&#39;nome da organização s conforme relatado no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="30acf-235">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="30acf-236">Isso é muito importante para reconciliar a fatura com as informações de seu sistema.</span><span class="sxs-lookup"><span data-stu-id="30acf-236">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="30acf-237">Cliente de teste A</span><span class="sxs-lookup"><span data-stu-id="30acf-237">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="30acf-238">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="30acf-238">MPNID</span></span></td>
<td><p><span data-ttu-id="30acf-239">ID do MPN do parceiro CSP</span><span class="sxs-lookup"><span data-stu-id="30acf-239">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="30acf-240">4390934</span><span class="sxs-lookup"><span data-stu-id="30acf-240">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="30acf-241">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="30acf-241">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="30acf-242">ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="30acf-242">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="30acf-243">Consulte <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Discriminar por parceiro</a>.</span><span class="sxs-lookup"><span data-stu-id="30acf-243">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="30acf-244">4390934</span><span class="sxs-lookup"><span data-stu-id="30acf-244">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="30acf-245">DomainName</span><span class="sxs-lookup"><span data-stu-id="30acf-245">DomainName</span></span></td>
<td><p><span data-ttu-id="30acf-246">Cliente&#39;nome de domínio s, usado para ajudar a identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="30acf-246">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="30acf-247">Isso não deve ser usado para identificar exclusivamente o cliente, assim como o cliente/parceiro pode atualizar o domínio intuitivo/padrão por meio do portal do O365.</span><span class="sxs-lookup"><span data-stu-id="30acf-247">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="30acf-248">Este campo pode aparecer em branco até o segundo ciclo de cobrança.</span><span class="sxs-lookup"><span data-stu-id="30acf-248">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="30acf-249">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="30acf-249">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="30acf-250">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="30acf-250">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="30acf-251">Apelido da Inscrição.</span><span class="sxs-lookup"><span data-stu-id="30acf-251">Subscription nickname.</span></span> <span data-ttu-id="30acf-252">Se nenhum apelido for especificado, o Partner Center usa o OfferName.</span><span class="sxs-lookup"><span data-stu-id="30acf-252">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="30acf-253">PROJETO ONLINE</span><span class="sxs-lookup"><span data-stu-id="30acf-253">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="30acf-254">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="30acf-254">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="30acf-255">O nome da oferta de serviço comprada pelo cliente, conforme definido na tabela de preços.</span><span class="sxs-lookup"><span data-stu-id="30acf-255">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="30acf-256">(Este é um campo idêntico ao nome da oferta).</span><span class="sxs-lookup"><span data-stu-id="30acf-256">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="30acf-257">PROJETO ONLINE PREMIUM SEM PROJETO CLIENTE</span><span class="sxs-lookup"><span data-stu-id="30acf-257">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="30acf-258">Campos de arquivo baseada em uso</span><span class="sxs-lookup"><span data-stu-id="30acf-258">Usage-based file fields</span></span>


<span data-ttu-id="30acf-259">Para reconciliar seus encargos com o uso de seu cliente, compare ResellerID/ResellerName/ResellerBillableAccount do arquivo de reconciliação com o nome do cliente e a ID da assinatura do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="30acf-259">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="30acf-260">Os campos a seguir explicam quais serviços foram usados e a taxa.</span><span class="sxs-lookup"><span data-stu-id="30acf-260">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="30acf-261"><strong>Coluna</strong></span><span class="sxs-lookup"><span data-stu-id="30acf-261"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="30acf-262"><strong>Descrição</strong></span><span class="sxs-lookup"><span data-stu-id="30acf-262"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="30acf-263"><strong>Valor de exemplo</strong></span><span class="sxs-lookup"><span data-stu-id="30acf-263"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="30acf-264">PartnerID</span><span class="sxs-lookup"><span data-stu-id="30acf-264">PartnerID</span></span></td>
<td><p><span data-ttu-id="30acf-265">ID do parceiro, no formato GUID.</span><span class="sxs-lookup"><span data-stu-id="30acf-265">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="30acf-266">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="30acf-266">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="30acf-267">PartnerName</span><span class="sxs-lookup"><span data-stu-id="30acf-267">PartnerName</span></span></td>
<td><p><span data-ttu-id="30acf-268">Nome do parceiro.</span><span class="sxs-lookup"><span data-stu-id="30acf-268">Partner Name.</span></span></p></td>
<td><span data-ttu-id="30acf-269">Acme incorporado</span><span class="sxs-lookup"><span data-stu-id="30acf-269">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="30acf-270">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="30acf-270">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="30acf-271">ID da conta do parceiro.</span><span class="sxs-lookup"><span data-stu-id="30acf-271">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="30acf-272">1010578050</span><span class="sxs-lookup"><span data-stu-id="30acf-272">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="30acf-273">CustomerName</span><span class="sxs-lookup"><span data-stu-id="30acf-273">CustomerName</span></span></td>
<td><p><span data-ttu-id="30acf-274">Cliente&#39;nome da organização s conforme relatado no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="30acf-274">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="30acf-275">Isso é muito importante para reconciliar a fatura com as informações de seu sistema.</span><span class="sxs-lookup"><span data-stu-id="30acf-275">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="30acf-276">Cliente de teste A</span><span class="sxs-lookup"><span data-stu-id="30acf-276">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="30acf-277">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="30acf-277">MPNID</span></span></td>
<td><p><span data-ttu-id="30acf-278">ID do MPN do parceiro CSP.</span><span class="sxs-lookup"><span data-stu-id="30acf-278">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="30acf-279">4390934</span><span class="sxs-lookup"><span data-stu-id="30acf-279">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="30acf-280">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="30acf-280">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="30acf-281">ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="30acf-281">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="30acf-282">Consulte <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Discriminar por parceiro</a>.</span><span class="sxs-lookup"><span data-stu-id="30acf-282">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="30acf-283">4390934</span><span class="sxs-lookup"><span data-stu-id="30acf-283">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="30acf-284">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="30acf-284">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="30acf-285">Número da fatura na qual a transação especificada é exibida.</span><span class="sxs-lookup"><span data-stu-id="30acf-285">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="30acf-286">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="30acf-286">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="30acf-287">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="30acf-287">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="30acf-288">Data de início do ciclo de cobrança exceto quando apresentadas as datas de dados de uso latentes anteriormente não cobradas (do ciclo de cobrança anterior).</span><span class="sxs-lookup"><span data-stu-id="30acf-288">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="30acf-289">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="30acf-289">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="30acf-290">1/2/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="30acf-290">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="30acf-291">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="30acf-291">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="30acf-292">Data de término do ciclo de cobrança exceto quando apresentadas as datas de dados de uso latentes anteriormente não cobradas (do ciclo de cobrança anterior).</span><span class="sxs-lookup"><span data-stu-id="30acf-292">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="30acf-293">A hora é sempre o fim do dia, 23:59.</span><span class="sxs-lookup"><span data-stu-id="30acf-293">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="30acf-294">28/2/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="30acf-294">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="30acf-295">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="30acf-295">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="30acf-296">Identificador exclusivo de uma assinatura na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="30acf-296">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="30acf-297">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="30acf-297">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="30acf-298">Esse não é o mesmo que o ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="30acf-298">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="30acf-299">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="30acf-299">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="30acf-300">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="30acf-300">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="30acf-301">Apelido da oferta do serviço.</span><span class="sxs-lookup"><span data-stu-id="30acf-301">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="30acf-302">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="30acf-302">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="30acf-303">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="30acf-303">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="30acf-304">Linha de negócios da oferta do serviço</span><span class="sxs-lookup"><span data-stu-id="30acf-304">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="30acf-305">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="30acf-305">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="30acf-306">OrderID</span><span class="sxs-lookup"><span data-stu-id="30acf-306">OrderID</span></span></td>
<td><p><span data-ttu-id="30acf-307">Identificador exclusivo para um pedido na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="30acf-307">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="30acf-308">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="30acf-308">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="30acf-309">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="30acf-309">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="30acf-310">ServiceName</span><span class="sxs-lookup"><span data-stu-id="30acf-310">ServiceName</span></span></td>
<td><p><span data-ttu-id="30acf-311">O nome do serviço do Azure em questão.</span><span class="sxs-lookup"><span data-stu-id="30acf-311">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="30acf-312">MÁQUINAS VIRTUAIS</span><span class="sxs-lookup"><span data-stu-id="30acf-312">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="30acf-313">ServiceType</span><span class="sxs-lookup"><span data-stu-id="30acf-313">ServiceType</span></span></td>
<td><p><span data-ttu-id="30acf-314">O tipo específico de serviço do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="30acf-314">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="30acf-315">Service Bus – Individual ou pacote</span><span class="sxs-lookup"><span data-stu-id="30acf-315">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="30acf-316">Banco de dados SQL Azure – Edição empresa ou Web</span><span class="sxs-lookup"><span data-stu-id="30acf-316">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="30acf-317">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="30acf-317">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="30acf-318">Identificador exclusivo específico de toda a estrutura de serviço de dados e preço.</span><span class="sxs-lookup"><span data-stu-id="30acf-318">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="30acf-319">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="30acf-319">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="30acf-320">Nome do recurso</span><span class="sxs-lookup"><span data-stu-id="30acf-320">Resource Name</span></span></td>
<td><p><span data-ttu-id="30acf-321">O nome do recurso do Azure.</span><span class="sxs-lookup"><span data-stu-id="30acf-321">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="30acf-322">Dados de entrada transferidos (GB)</span><span class="sxs-lookup"><span data-stu-id="30acf-322">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="30acf-323">Dados de saída transferidos (GB)</span><span class="sxs-lookup"><span data-stu-id="30acf-323">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="30acf-324">Region</span><span class="sxs-lookup"><span data-stu-id="30acf-324">Region</span></span></td>
<td><p><span data-ttu-id="30acf-325">A região a qual o uso se aplica.</span><span class="sxs-lookup"><span data-stu-id="30acf-325">The region the usage applies to.</span></span> <span data-ttu-id="30acf-326">Usado principalmente para atribuir as taxas de transferências de dados, já que as taxas variam de acordo com a região.</span><span class="sxs-lookup"><span data-stu-id="30acf-326">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="30acf-327">Pacífico Asiático, Europa, América Latina e América do Norte</span><span class="sxs-lookup"><span data-stu-id="30acf-327">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="30acf-328">SKU</span><span class="sxs-lookup"><span data-stu-id="30acf-328">SKU</span></span></td>
<td><p><span data-ttu-id="30acf-329">Identificador exclusivo MSFT da oferta</span><span class="sxs-lookup"><span data-stu-id="30acf-329">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="30acf-330">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="30acf-330">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="30acf-331">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="30acf-331">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="30acf-332">Uma ID e a quantidade para discriminar as taxas diferentes de um serviço ou recurso em um determinado período de cobrança.</span><span class="sxs-lookup"><span data-stu-id="30acf-332">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="30acf-333">Para a classificação em camadas do Azure, pode haver uma taxa para uma determinada quantidade de unidades faturáveis e uma taxa diferente depois disso.</span><span class="sxs-lookup"><span data-stu-id="30acf-333">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="30acf-334">1</span><span class="sxs-lookup"><span data-stu-id="30acf-334">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="30acf-335">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="30acf-335">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="30acf-336">A quantidade de serviço consumida (horas, GB etc.) durante o período de relatório.</span><span class="sxs-lookup"><span data-stu-id="30acf-336">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="30acf-337">Também inclui qualquer uso não cobrado de períodos de relatório anteriores.</span><span class="sxs-lookup"><span data-stu-id="30acf-337">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="30acf-338">11</span><span class="sxs-lookup"><span data-stu-id="30acf-338">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="30acf-339">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="30acf-339">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="30acf-340">Unidades incluídas como parte da oferta.</span><span class="sxs-lookup"><span data-stu-id="30acf-340">Units included as part of the offer.</span></span> <span data-ttu-id="30acf-341">Normalmente não está presente no CSP.</span><span class="sxs-lookup"><span data-stu-id="30acf-341">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="30acf-342">0</span><span class="sxs-lookup"><span data-stu-id="30acf-342">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="30acf-343">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="30acf-343">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="30acf-344">Unidades não incluídas como parte da oferta devem ser pagas pelo parceiro.</span><span class="sxs-lookup"><span data-stu-id="30acf-344">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="30acf-345">Igual a ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="30acf-345">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="30acf-346">11</span><span class="sxs-lookup"><span data-stu-id="30acf-346">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="30acf-347">ListPrice</span><span class="sxs-lookup"><span data-stu-id="30acf-347">ListPrice</span></span></td>
<td><p><span data-ttu-id="30acf-348">Preço da oferta em vigor na data de início da assinatura.</span><span class="sxs-lookup"><span data-stu-id="30acf-348">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="30acf-349">U$ 0,0808</span><span class="sxs-lookup"><span data-stu-id="30acf-349">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="30acf-350">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="30acf-350">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="30acf-351">ListPrist vezes OverageQuantity, arredondado para o centavo mais próximo.</span><span class="sxs-lookup"><span data-stu-id="30acf-351">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="30acf-352">U$ 0,085</span><span class="sxs-lookup"><span data-stu-id="30acf-352">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="30acf-353">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="30acf-353">TaxAmount</span></span></td>
<td><p><span data-ttu-id="30acf-354">Encargo de valor, com base em seu mercado de imposto&#39;regras de imposto de s e as circunstâncias específicas.</span><span class="sxs-lookup"><span data-stu-id="30acf-354">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="30acf-355">U$ 0,08</span><span class="sxs-lookup"><span data-stu-id="30acf-355">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="30acf-356">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="30acf-356">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="30acf-357">Total após imposto, quando o imposto é aplicável.</span><span class="sxs-lookup"><span data-stu-id="30acf-357">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="30acf-358">U$ 0,93</span><span class="sxs-lookup"><span data-stu-id="30acf-358">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="30acf-359">Currency</span><span class="sxs-lookup"><span data-stu-id="30acf-359">Currency</span></span></td>
<td><p><span data-ttu-id="30acf-360">Tipo de moeda.</span><span class="sxs-lookup"><span data-stu-id="30acf-360">Currency type.</span></span> <span data-ttu-id="30acf-361">Cada entidade de cobrança tem somente uma moeda.</span><span class="sxs-lookup"><span data-stu-id="30acf-361">Each billing entity has only one currency.</span></span> <span data-ttu-id="30acf-362">Verifique se isso coincide com a primeira fatura e faça o mesmo após grandes atualizações na plataforma de cobrança.</span><span class="sxs-lookup"><span data-stu-id="30acf-362">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="30acf-363">EUR</span><span class="sxs-lookup"><span data-stu-id="30acf-363">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="30acf-364">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="30acf-364">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="30acf-365">Preço por unidade sem imposto.</span><span class="sxs-lookup"><span data-stu-id="30acf-365">Pretax price per unit.</span></span> <span data-ttu-id="30acf-366">Igual a PretaxCharges / OverageQuantity, arredondado para o centavo mais próximo.</span><span class="sxs-lookup"><span data-stu-id="30acf-366">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="30acf-367">U$ 0,08</span><span class="sxs-lookup"><span data-stu-id="30acf-367">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="30acf-368">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="30acf-368">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="30acf-369">Preço pós-imposto por unidade.</span><span class="sxs-lookup"><span data-stu-id="30acf-369">Post tax price per unit.</span></span> <span data-ttu-id="30acf-370">Igual a PostTaxTotal / OverageQuantity, ou PretaxEffectiveRate + taxa de imposto por valor de unidade, arredondado para o centavo mais próximo.</span><span class="sxs-lookup"><span data-stu-id="30acf-370">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="30acf-371">U$ 0,08</span><span class="sxs-lookup"><span data-stu-id="30acf-371">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="30acf-372">ChargeType</span><span class="sxs-lookup"><span data-stu-id="30acf-372">ChargeType</span></span></td>
<td><p><span data-ttu-id="30acf-373">O tipo de encargo ou ajuste.</span><span class="sxs-lookup"><span data-stu-id="30acf-373">The type of charge or adjustment.</span></span> <span data-ttu-id="30acf-374">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="30acf-374">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="30acf-375">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="30acf-375">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="30acf-376">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="30acf-376">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="30acf-377">ID exclusiva da conta na plataforma de cobrança da MSFT.</span><span class="sxs-lookup"><span data-stu-id="30acf-377">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="30acf-378">1280018095</span><span class="sxs-lookup"><span data-stu-id="30acf-378">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="30acf-379">UsageDate</span><span class="sxs-lookup"><span data-stu-id="30acf-379">UsageDate</span></span></td>
<td><p><span data-ttu-id="30acf-380">Data da implantação do serviço.</span><span class="sxs-lookup"><span data-stu-id="30acf-380">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="30acf-381">1/2/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="30acf-381">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="30acf-382">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="30acf-382">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="30acf-383">Essa coluna identifica a localização de um data center dentro da região para serviços onde isso é aplicável e preenchido.</span><span class="sxs-lookup"><span data-stu-id="30acf-383">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="30acf-384">Leste da Ásia, Sudeste da Ásia, Norte da Europa, Europa Ocidental, Centro Norte e Centro Sul dos EUA</span><span class="sxs-lookup"><span data-stu-id="30acf-384">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="30acf-385">MeteredService</span><span class="sxs-lookup"><span data-stu-id="30acf-385">MeteredService</span></span></td>
<td><p><span data-ttu-id="30acf-386">Essa coluna é utilizada para rastrear o serviço do Microsoft Azure individual que não pode ser identificado especificamente na coluna Nome do Serviço.</span><span class="sxs-lookup"><span data-stu-id="30acf-386">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="30acf-387">Por exemplo, transferências de dados são relatadas como &quot;Microsoft Azure – Todos os Serviços&quot; na coluna Nome do Serviço.</span><span class="sxs-lookup"><span data-stu-id="30acf-387">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="30acf-388">Essa coluna MeteredService indicará ao qual serviço específico o uso pertence.</span><span class="sxs-lookup"><span data-stu-id="30acf-388">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="30acf-389">AccessControl, CDN, Computação, Banco de dados, ServiceBus, Armazenamento</span><span class="sxs-lookup"><span data-stu-id="30acf-389">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="30acf-390">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="30acf-390">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="30acf-391">Um subcabeçalho que esclarece ainda mais o serviço Microsoft Azure individual além do nível fornecido pelo campo MeteredService.</span><span class="sxs-lookup"><span data-stu-id="30acf-391">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="30acf-392">EXTERNO</span><span class="sxs-lookup"><span data-stu-id="30acf-392">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="30acf-393">Projeto</span><span class="sxs-lookup"><span data-stu-id="30acf-393">Project</span></span></td>
<td><p><span data-ttu-id="30acf-394">Nome definido pelo cliente para a instância do serviço</span><span class="sxs-lookup"><span data-stu-id="30acf-394">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="30acf-395">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="30acf-395">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="30acf-396">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="30acf-396">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="30acf-397">O número de conexões ServiceBus que foram provisionados e utilizados em um dia específico.</span><span class="sxs-lookup"><span data-stu-id="30acf-397">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="30acf-398">Por exemplo: se você tivesse uma conexão individualmente provisionada durante um mês de 30 dias, a coluna Informação do Serviço 1 lerá "1,000000 conexões/30 dias".</span><span class="sxs-lookup"><span data-stu-id="30acf-398">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="30acf-399">Se você tivesse um pacote de 25 de conexões de barramento de serviço provisionado e você tinha utilizou 1 durante o dia, sua instrução de uso diário para esse dia indicaria "25 conexões / 30 dias – usado: 1.000000”.</span><span class="sxs-lookup"><span data-stu-id="30acf-399">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="30acf-400">CustomerID</span><span class="sxs-lookup"><span data-stu-id="30acf-400">CustomerID</span></span></td>
<td><p><span data-ttu-id="30acf-401">ID exclusiva da Microsoft, no formato GUID, usada para identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="30acf-401">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="30acf-402">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="30acf-402">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="30acf-403">DomainName</span><span class="sxs-lookup"><span data-stu-id="30acf-403">DomainName</span></span></td>
<td><p><span data-ttu-id="30acf-404">Cliente&#39;nome de domínio s, usado para ajudar a identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="30acf-404">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="30acf-405">Este campo pode aparecer em branco até o segundo ciclo de cobrança.</span><span class="sxs-lookup"><span data-stu-id="30acf-405">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="30acf-406">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="30acf-406">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="30acf-407">Unidade</span><span class="sxs-lookup"><span data-stu-id="30acf-407">Unit</span></span></td>
<td><p><span data-ttu-id="30acf-408">A unidade do nome do recurso</span><span class="sxs-lookup"><span data-stu-id="30acf-408">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="30acf-409">GB ou HORAS</span><span class="sxs-lookup"><span data-stu-id="30acf-409">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="30acf-410">Campos de arquivo únicos e recorrentes</span><span class="sxs-lookup"><span data-stu-id="30acf-410">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="30acf-411">Column</span><span class="sxs-lookup"><span data-stu-id="30acf-411">Column</span></span></th>
<th><span data-ttu-id="30acf-412">Descrição</span><span class="sxs-lookup"><span data-stu-id="30acf-412">Description</span></span></th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td><span data-ttu-id="30acf-413">PartnerID</span><span class="sxs-lookup"><span data-stu-id="30acf-413">PartnerId</span></span></td>
<td><p><span data-ttu-id="30acf-414">Identificador exclusivo do locatário Microsoft Azure Active Directory para uma entidade específica de cobrança, no formato GUID.</span><span class="sxs-lookup"><span data-stu-id="30acf-414">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="30acf-415">Não é necessário para reconciliação, mas pode ser uma informação útil.</span><span class="sxs-lookup"><span data-stu-id="30acf-415">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="30acf-416">O mesmo em todas as linhas.</span><span class="sxs-lookup"><span data-stu-id="30acf-416">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="30acf-417">Id do cliente</span><span class="sxs-lookup"><span data-stu-id="30acf-417">Customer Id</span></span></td>
<td><p><span data-ttu-id="30acf-418">Microsoft Azure Active Directory locatário ID exclusiva, no formato GUID, usado para identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="30acf-418">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="30acf-419">Nome do cliente</span><span class="sxs-lookup"><span data-stu-id="30acf-419">Customer Name</span></span></td>
<td><p><span data-ttu-id="30acf-420">Nome da organização do cliente como informado no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="30acf-420">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="30acf-421">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="30acf-421">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="30acf-422">Nome de domínio do cliente, usado para ajudar a identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="30acf-422">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="30acf-423">Isso não deve ser usado para identificar exclusivamente o cliente, assim como o cliente/parceiro pode atualizar o domínio intuitivo/padrão por meio do portal do O365.</span><span class="sxs-lookup"><span data-stu-id="30acf-423">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="30acf-424">Este campo pode aparecer em branco até o segundo ciclo de cobrança.</span><span class="sxs-lookup"><span data-stu-id="30acf-424">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="30acf-425">País do cliente</span><span class="sxs-lookup"><span data-stu-id="30acf-425">Customer Country</span></span></td>
<td><p><span data-ttu-id="30acf-426">O país em que o cliente está localizado.</span><span class="sxs-lookup"><span data-stu-id="30acf-426">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="30acf-427">Número da fatura</span><span class="sxs-lookup"><span data-stu-id="30acf-427">Invoice number</span></span></td>
<td><p><span data-ttu-id="30acf-428">Número da fatura na qual a transação especificada é exibida.</span><span class="sxs-lookup"><span data-stu-id="30acf-428">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="30acf-429">MpnID</span><span class="sxs-lookup"><span data-stu-id="30acf-429">MpnId</span></span></td>
<td><p><span data-ttu-id="30acf-430">ID do MPN do parceiro CSP.</span><span class="sxs-lookup"><span data-stu-id="30acf-430">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="30acf-431">Reseller MpnId</span><span class="sxs-lookup"><span data-stu-id="30acf-431">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="30acf-432">ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="30acf-432">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="30acf-433">ID do Pedido</span><span class="sxs-lookup"><span data-stu-id="30acf-433">Order ID</span></span></td>
<td><p><span data-ttu-id="30acf-434">Identificador exclusivo para um pedido na plataforma de comércio do Microsoft.</span><span class="sxs-lookup"><span data-stu-id="30acf-434">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="30acf-435">Pode ser útil para identificar o pedido ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="30acf-435">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="30acf-436">Data do pedido</span><span class="sxs-lookup"><span data-stu-id="30acf-436">Order date</span></span></td>
<td><p><span data-ttu-id="30acf-437">A data em que o pedido foi feito.</span><span class="sxs-lookup"><span data-stu-id="30acf-437">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="30acf-438">ProductId</span><span class="sxs-lookup"><span data-stu-id="30acf-438">ProductId</span></span></td>
<td><p><span data-ttu-id="30acf-439">A ID do produto.</span><span class="sxs-lookup"><span data-stu-id="30acf-439">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="30acf-440">SkuId</span><span class="sxs-lookup"><span data-stu-id="30acf-440">SkuId</span></span></td>
<td><p><span data-ttu-id="30acf-441">A ID de uma SKU em particular.</span><span class="sxs-lookup"><span data-stu-id="30acf-441">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="30acf-442">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="30acf-442">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="30acf-443">A ID de uma Disponibilidade em particular.</span><span class="sxs-lookup"><span data-stu-id="30acf-443">The ID for a particular Availability.</span></span> <span data-ttu-id="30acf-444">"Disponibilidade" refere-se a se uma SKU em particular está disponível ou não para compra para determinado país, moeda, segmento do setor etc.</span><span class="sxs-lookup"><span data-stu-id="30acf-444">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="30acf-445">Nome do SKU</span><span class="sxs-lookup"><span data-stu-id="30acf-445">SKU Name</span></span></td>
<td><p><span data-ttu-id="30acf-446">O título de uma SKU em particular.</span><span class="sxs-lookup"><span data-stu-id="30acf-446">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="30acf-447">Nome do produto</span><span class="sxs-lookup"><span data-stu-id="30acf-447">Product name</span></span></td>
<td><p><span data-ttu-id="30acf-448">O nome do produto.</span><span class="sxs-lookup"><span data-stu-id="30acf-448">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="30acf-449">PublisherName</span><span class="sxs-lookup"><span data-stu-id="30acf-449">PublisherName</span></span></td>
<td><p><span data-ttu-id="30acf-450">O nome do publicador do produto.</span><span class="sxs-lookup"><span data-stu-id="30acf-450">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="30acf-451">PublisherID</span><span class="sxs-lookup"><span data-stu-id="30acf-451">PublisherID</span></span></td>
<td><p><span data-ttu-id="30acf-452">ID exclusiva para esse publicador.</span><span class="sxs-lookup"><span data-stu-id="30acf-452">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="30acf-453">Descrição da assinatura</span><span class="sxs-lookup"><span data-stu-id="30acf-453">Subscription Description</span></span></td>
<td><p><span data-ttu-id="30acf-454">Nome amigável de uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="30acf-454">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="30acf-455">ID da assinatura</span><span class="sxs-lookup"><span data-stu-id="30acf-455">Subscription ID</span></span></td>
<td><p><span data-ttu-id="30acf-456">Identificador exclusivo para uma assinatura da plataforma de comércio do Microsoft.</span><span class="sxs-lookup"><span data-stu-id="30acf-456">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="30acf-457">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="30acf-457">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="30acf-458">Esse não é o mesmo que o ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="30acf-458">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="30acf-459">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="30acf-459">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="30acf-460">Dia de início dos encargos.</span><span class="sxs-lookup"><span data-stu-id="30acf-460">Start day of the charges.</span></span> <span data-ttu-id="30acf-461">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="30acf-461">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="30acf-462">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="30acf-462">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="30acf-463">Dia do término dos encargos.</span><span class="sxs-lookup"><span data-stu-id="30acf-463">End day of the charges.</span></span> <span data-ttu-id="30acf-464">A hora é sempre o fim do dia, 23:59.</span><span class="sxs-lookup"><span data-stu-id="30acf-464">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="30acf-465">Termo e Billingcycle</span><span class="sxs-lookup"><span data-stu-id="30acf-465">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="30acf-466">A vigência e o ciclo de cobrança para a compra.</span><span class="sxs-lookup"><span data-stu-id="30acf-466">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="30acf-467">Por exemplo, "1 ano, mês."</span><span class="sxs-lookup"><span data-stu-id="30acf-467">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="30acf-468">Tipo de Cobrança</span><span class="sxs-lookup"><span data-stu-id="30acf-468">Charge Type</span></span></td>
<td><p><span data-ttu-id="30acf-469">O tipo de encargo ou ajuste.</span><span class="sxs-lookup"><span data-stu-id="30acf-469">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="30acf-470">Preço unitário</span><span class="sxs-lookup"><span data-stu-id="30acf-470">Unit Price</span></span></td>
<td><p><span data-ttu-id="30acf-471">O preço como publicado no pricelist no momento da compra.</span><span class="sxs-lookup"><span data-stu-id="30acf-471">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="30acf-472">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="30acf-472">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="30acf-473">Preço unitário efetiva</span><span class="sxs-lookup"><span data-stu-id="30acf-473">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="30acf-474">O preço unitário depois de fazer ajustes.</span><span class="sxs-lookup"><span data-stu-id="30acf-474">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="30acf-475">Quantidade</span><span class="sxs-lookup"><span data-stu-id="30acf-475">Quantity</span></span></td>
<td><p><span data-ttu-id="30acf-476">Número de unidades.</span><span class="sxs-lookup"><span data-stu-id="30acf-476">Number of units.</span></span> <span data-ttu-id="30acf-477">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="30acf-477">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="30acf-478">Tipo de unidade</span><span class="sxs-lookup"><span data-stu-id="30acf-478">Unit type</span></span></td>
<td><p><span data-ttu-id="30acf-479">O tipo de unidade que está sendo comprado.</span><span class="sxs-lookup"><span data-stu-id="30acf-479">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="30acf-480">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="30acf-480">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="30acf-481">Obter uma explicação de qualquer desconto aplicável.</span><span class="sxs-lookup"><span data-stu-id="30acf-481">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="30acf-482">Subtotal</span><span class="sxs-lookup"><span data-stu-id="30acf-482">Sub Total</span></span></td>
<td><p><span data-ttu-id="30acf-483">Total sem imposto.</span><span class="sxs-lookup"><span data-stu-id="30acf-483">Total before tax.</span></span> <span data-ttu-id="30acf-484">Verifica se seu subtotal corresponde ao total esperado, em caso de desconto.</span><span class="sxs-lookup"><span data-stu-id="30acf-484">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="30acf-485">Total de impostos</span><span class="sxs-lookup"><span data-stu-id="30acf-485">Tax Total</span></span></td>
<td><p><span data-ttu-id="30acf-486">Valor do imposto cobrado, com base nas regras fiscais do mercado e em circunstâncias específicas.</span><span class="sxs-lookup"><span data-stu-id="30acf-486">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="30acf-487">Total</span><span class="sxs-lookup"><span data-stu-id="30acf-487">Total</span></span></td>
<td><p><span data-ttu-id="30acf-488">Total com imposto.</span><span class="sxs-lookup"><span data-stu-id="30acf-488">Total after tax.</span></span> <span data-ttu-id="30acf-489">Verifica se o imposto é cobrado na fatura.</span><span class="sxs-lookup"><span data-stu-id="30acf-489">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="30acf-490">Currency</span><span class="sxs-lookup"><span data-stu-id="30acf-490">Currency</span></span></td>
<td><p><span data-ttu-id="30acf-491">Tipo de moeda.</span><span class="sxs-lookup"><span data-stu-id="30acf-491">Currency type.</span></span> <span data-ttu-id="30acf-492">Cada entidade de cobrança tem somente uma moeda.</span><span class="sxs-lookup"><span data-stu-id="30acf-492">Each billing entity has only one currency.</span></span> <span data-ttu-id="30acf-493">Verifique se isso coincide com a primeira fatura e faça o mesmo após grandes atualizações na plataforma de cobrança.</span><span class="sxs-lookup"><span data-stu-id="30acf-493">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="30acf-494">AlternateID</span><span class="sxs-lookup"><span data-stu-id="30acf-494">AlternateID</span></span></td>
<td><p><span data-ttu-id="30acf-495">Um identificador alternativo para uma ID de pedido.</span><span class="sxs-lookup"><span data-stu-id="30acf-495">An alternate identifier to an order ID.</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="30acf-496">Campos de arquivo de uso classificada como diária</span><span class="sxs-lookup"><span data-stu-id="30acf-496">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="30acf-497">Column</span><span class="sxs-lookup"><span data-stu-id="30acf-497">Column</span></span></th>
<th><span data-ttu-id="30acf-498">Descrição</span><span class="sxs-lookup"><span data-stu-id="30acf-498">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="30acf-499">PartnerID</span><span class="sxs-lookup"><span data-stu-id="30acf-499">PartnerId</span></span></td>
<td><p><span data-ttu-id="30acf-500">ID do parceiro, no formato GUID.</span><span class="sxs-lookup"><span data-stu-id="30acf-500">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="30acf-501">PartnerName</span><span class="sxs-lookup"><span data-stu-id="30acf-501">PartnerName</span></span></td>
<td><p><span data-ttu-id="30acf-502">Nome do parceiro.</span><span class="sxs-lookup"><span data-stu-id="30acf-502">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="30acf-503">CustomerID</span><span class="sxs-lookup"><span data-stu-id="30acf-503">CustomerId</span></span></td>
<td><p><span data-ttu-id="30acf-504">ID exclusiva da Microsoft, no formato GUID, usada para identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="30acf-504">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="30acf-505">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="30acf-505">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="30acf-506">Nome da organização do cliente como informado no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="30acf-506">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="30acf-507">Isso é muito importante para reconciliar a fatura com as informações de seu sistema.</span><span class="sxs-lookup"><span data-stu-id="30acf-507">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="30acf-508">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="30acf-508">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="30acf-509">O nome de domínio do cliente.</span><span class="sxs-lookup"><span data-stu-id="30acf-509">The customer’s domain name.</span></span> <span data-ttu-id="30acf-510">Não disponível para a atividade atual.</span><span class="sxs-lookup"><span data-stu-id="30acf-510">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="30acf-511">País do cliente</span><span class="sxs-lookup"><span data-stu-id="30acf-511">Customer country</span></span></td>
<td><p><span data-ttu-id="30acf-512">O país em que o cliente está localizado.</span><span class="sxs-lookup"><span data-stu-id="30acf-512">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="30acf-513">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="30acf-513">MPNID</span></span></td>
<td><p><span data-ttu-id="30acf-514">ID do MPN do parceiro CSP.</span><span class="sxs-lookup"><span data-stu-id="30acf-514">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="30acf-515">Revendedor MPNID</span><span class="sxs-lookup"><span data-stu-id="30acf-515">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="30acf-516">ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="30acf-516">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="30acf-517">Não disponível para a atividade atual.</span><span class="sxs-lookup"><span data-stu-id="30acf-517">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="30acf-518">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="30acf-518">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="30acf-519">Número da fatura na qual a transação especificada é exibida.</span><span class="sxs-lookup"><span data-stu-id="30acf-519">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="30acf-520">Não disponível para a atividade atual.</span><span class="sxs-lookup"><span data-stu-id="30acf-520">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="30acf-521">ProductId</span><span class="sxs-lookup"><span data-stu-id="30acf-521">ProductId</span></span></td>
<td><p><span data-ttu-id="30acf-522">A ID do produto.</span><span class="sxs-lookup"><span data-stu-id="30acf-522">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="30acf-523">SkuId</span><span class="sxs-lookup"><span data-stu-id="30acf-523">SkuId</span></span></td>
<td><p><span data-ttu-id="30acf-524">A ID de uma SKU em particular.</span><span class="sxs-lookup"><span data-stu-id="30acf-524">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="30acf-525">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="30acf-525">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="30acf-526">A ID de uma Disponibilidade em particular.</span><span class="sxs-lookup"><span data-stu-id="30acf-526">The ID for a particular Availability.</span></span> <span data-ttu-id="30acf-527">"Disponibilidade" refere-se a se uma SKU em particular está disponível ou não para compra para determinado país, moeda, segmento do setor etc.</span><span class="sxs-lookup"><span data-stu-id="30acf-527">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="30acf-528">Nome do SKU</span><span class="sxs-lookup"><span data-stu-id="30acf-528">SKU Name</span></span></td>
<td><p><span data-ttu-id="30acf-529">O título de uma SKU em particular.</span><span class="sxs-lookup"><span data-stu-id="30acf-529">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="30acf-530">PublisherName</span><span class="sxs-lookup"><span data-stu-id="30acf-530">PublisherName</span></span></td>
<td><p><span data-ttu-id="30acf-531">O nome do publicador.</span><span class="sxs-lookup"><span data-stu-id="30acf-531">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="30acf-532">PublisherID</span><span class="sxs-lookup"><span data-stu-id="30acf-532">PublisherID</span></span></td>
<td><p><span data-ttu-id="30acf-533">A ID do publicador, no formato GUID.</span><span class="sxs-lookup"><span data-stu-id="30acf-533">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="30acf-534">Não disponível para a atividade atual.</span><span class="sxs-lookup"><span data-stu-id="30acf-534">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="30acf-535">Descrição da assinatura</span><span class="sxs-lookup"><span data-stu-id="30acf-535">Subscription Description</span></span></td>
<td><p><span data-ttu-id="30acf-536">O nome da oferta de serviço comprada pelo cliente, conforme definido na tabela de preços.</span><span class="sxs-lookup"><span data-stu-id="30acf-536">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="30acf-537">(Este é um campo idêntico ao nome da oferta).</span><span class="sxs-lookup"><span data-stu-id="30acf-537">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="30acf-538">ID da assinatura</span><span class="sxs-lookup"><span data-stu-id="30acf-538">Subscription ID</span></span></td>
<td><p><span data-ttu-id="30acf-539">Identificador exclusivo de uma assinatura na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="30acf-539">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="30acf-540">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="30acf-540">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="30acf-541">Esse não é o mesmo que o ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="30acf-541">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="30acf-542">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="30acf-542">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="30acf-543">Data de início do ciclo de cobrança exceto quando apresentadas as datas de dados de uso latentes anteriormente não cobradas (do ciclo de cobrança anterior).</span><span class="sxs-lookup"><span data-stu-id="30acf-543">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="30acf-544">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="30acf-544">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="30acf-545">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="30acf-545">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="30acf-546">Data de término do ciclo de cobrança exceto quando apresentadas as datas de dados de uso latentes anteriormente não cobradas (do ciclo de cobrança anterior).</span><span class="sxs-lookup"><span data-stu-id="30acf-546">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="30acf-547">A hora é sempre o fim do dia, 23:59.</span><span class="sxs-lookup"><span data-stu-id="30acf-547">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="30acf-548">Data de uso</span><span class="sxs-lookup"><span data-stu-id="30acf-548">Usage Date</span></span></td>
<td><p><span data-ttu-id="30acf-549">Data de uso do serviço.</span><span class="sxs-lookup"><span data-stu-id="30acf-549">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="30acf-550">Tipo de medidor</span><span class="sxs-lookup"><span data-stu-id="30acf-550">Meter Type</span></span></td>
<td><p><span data-ttu-id="30acf-551">O tipo de medidor.</span><span class="sxs-lookup"><span data-stu-id="30acf-551">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="30acf-552">Categoria do medidor</span><span class="sxs-lookup"><span data-stu-id="30acf-552">Meter Category</span></span></td>
<td><p><span data-ttu-id="30acf-553">O serviço de nível superior para o uso.</span><span class="sxs-lookup"><span data-stu-id="30acf-553">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="30acf-554">Id do medidor</span><span class="sxs-lookup"><span data-stu-id="30acf-554">Meter Id</span></span></td>
<td><p><span data-ttu-id="30acf-555">A ID do medidor que está sendo usado.</span><span class="sxs-lookup"><span data-stu-id="30acf-555">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="30acf-556">Medir subcategoria</span><span class="sxs-lookup"><span data-stu-id="30acf-556">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="30acf-557">O tipo de serviço do Azure que pode afetar a tarifa.</span><span class="sxs-lookup"><span data-stu-id="30acf-557">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="30acf-558">Nome do medidor</span><span class="sxs-lookup"><span data-stu-id="30acf-558">Meter Name</span></span></td>
<td><p><span data-ttu-id="30acf-559">A unidade de medida para o medidor sendo consumido.</span><span class="sxs-lookup"><span data-stu-id="30acf-559">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="30acf-560">Região do medidor</span><span class="sxs-lookup"><span data-stu-id="30acf-560">Meter Region</span></span></td>
<td><p><span data-ttu-id="30acf-561">Essa coluna identifica a localização de um data center dentro da região para serviços onde isso é aplicável e preenchido.</span><span class="sxs-lookup"><span data-stu-id="30acf-561">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="30acf-562">Unidade</span><span class="sxs-lookup"><span data-stu-id="30acf-562">Unit</span></span></td>
<td><p><span data-ttu-id="30acf-563">A unidade do nome do recurso.</span><span class="sxs-lookup"><span data-stu-id="30acf-563">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="30acf-564">Quantidade consumida</span><span class="sxs-lookup"><span data-stu-id="30acf-564">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="30acf-565">A quantidade de serviço consumida (horas, GB etc.) durante o período de relatório.</span><span class="sxs-lookup"><span data-stu-id="30acf-565">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="30acf-566">Também inclui qualquer uso não cobrado de períodos de relatório anteriores.</span><span class="sxs-lookup"><span data-stu-id="30acf-566">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="30acf-567">Local do recurso</span><span class="sxs-lookup"><span data-stu-id="30acf-567">Resource Location</span></span></td>
<td><p><span data-ttu-id="30acf-568">O datacenter em que o medidor está sendo executado.</span><span class="sxs-lookup"><span data-stu-id="30acf-568">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="30acf-569">Serviço consumido</span><span class="sxs-lookup"><span data-stu-id="30acf-569">Consumed Service</span></span></td>
<td><p><span data-ttu-id="30acf-570">O serviço de plataforma do Azure que você usou.</span><span class="sxs-lookup"><span data-stu-id="30acf-570">The Azure platform service that you used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="30acf-571">Grupo de Recursos</span><span class="sxs-lookup"><span data-stu-id="30acf-571">Resource Group</span></span></td>
<td><p><span data-ttu-id="30acf-572">O grupo de recursos no qual o medidor implantado está sendo executado.</span><span class="sxs-lookup"><span data-stu-id="30acf-572">The resource group in which the deployed meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="30acf-573">URI de recurso</span><span class="sxs-lookup"><span data-stu-id="30acf-573">Resource URI</span></span></td>
<td><p><span data-ttu-id="30acf-574">O URI do recurso que está sendo usado.</span><span class="sxs-lookup"><span data-stu-id="30acf-574">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="30acf-575">Tipo de cobrança</span><span class="sxs-lookup"><span data-stu-id="30acf-575">Charge type</span></span></td>
<td><p><span data-ttu-id="30acf-576">O tipo de encargo ou ajuste.</span><span class="sxs-lookup"><span data-stu-id="30acf-576">The type of charge or adjustment.</span></span> <span data-ttu-id="30acf-577">Não disponível para a atividade atual.</span><span class="sxs-lookup"><span data-stu-id="30acf-577">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="30acf-578">Preço unitário</span><span class="sxs-lookup"><span data-stu-id="30acf-578">Unit price</span></span></td>
<td><p><span data-ttu-id="30acf-579">Preço por licença, como publicado no pricelist no momento da compra.</span><span class="sxs-lookup"><span data-stu-id="30acf-579">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="30acf-580">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="30acf-580">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="30acf-581">Quantidade</span><span class="sxs-lookup"><span data-stu-id="30acf-581">Quantity</span></span></td>
<td><p><span data-ttu-id="30acf-582">Número de licenças.</span><span class="sxs-lookup"><span data-stu-id="30acf-582">Number of licenses.</span></span> <span data-ttu-id="30acf-583">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="30acf-583">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="30acf-584">Tipo de unidade</span><span class="sxs-lookup"><span data-stu-id="30acf-584">Unit type</span></span></td>
<td><p><span data-ttu-id="30acf-585">O tipo de unidade, que o medidor é cobrado.</span><span class="sxs-lookup"><span data-stu-id="30acf-585">The type of unit the meter is charged in.</span></span> <span data-ttu-id="30acf-586">Não disponível para a atividade atual.</span><span class="sxs-lookup"><span data-stu-id="30acf-586">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="30acf-587">Imposto de versão anterior de cobrança</span><span class="sxs-lookup"><span data-stu-id="30acf-587">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="30acf-588">Quantidade total antes dos impostos.</span><span class="sxs-lookup"><span data-stu-id="30acf-588">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="30acf-589">Moeda de cobrança</span><span class="sxs-lookup"><span data-stu-id="30acf-589">Billing currency</span></span></td>
<td><p><span data-ttu-id="30acf-590">A moeda na região de geográfica do cliente</span><span class="sxs-lookup"><span data-stu-id="30acf-590">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="30acf-591">Preço total pretax</span><span class="sxs-lookup"><span data-stu-id="30acf-591">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="30acf-592">O preço antes de impostos forem adicionados.</span><span class="sxs-lookup"><span data-stu-id="30acf-592">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="30acf-593">Preços de moeda</span><span class="sxs-lookup"><span data-stu-id="30acf-593">Pricing currency</span></span></td>
<td><p><span data-ttu-id="30acf-594">A moeda no pricelist.</span><span class="sxs-lookup"><span data-stu-id="30acf-594">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="30acf-595">Informações do serviço 1</span><span class="sxs-lookup"><span data-stu-id="30acf-595">Service Info 1</span></span></td>
<td><p><span data-ttu-id="30acf-596">O número de conexões ServiceBus que foram provisionados e utilizados em um dia específico.</span><span class="sxs-lookup"><span data-stu-id="30acf-596">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="30acf-597">Informações do serviço 2</span><span class="sxs-lookup"><span data-stu-id="30acf-597">Service Info 2</span></span></td>
<td><p><span data-ttu-id="30acf-598">Um campo herdado que captura os metadados específicos do serviço opcional.</span><span class="sxs-lookup"><span data-stu-id="30acf-598">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="30acf-599">Marcas</span><span class="sxs-lookup"><span data-stu-id="30acf-599">Tags</span></span></td>
<td><p><span data-ttu-id="30acf-600">Marcas que você atribui ao medidor na ordem para agrupar registros de cobrança.</span><span class="sxs-lookup"><span data-stu-id="30acf-600">Tags you assign to the meter in order to group billing records.</span></span> <span data-ttu-id="30acf-601">Por exemplo, você pode usar marcas para distribuir os custos entre os departamentos que usam o medidor.</span><span class="sxs-lookup"><span data-stu-id="30acf-601">For example, you can use tags to distribute costs by the department that uses the meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="30acf-602">Informações adicionais</span><span class="sxs-lookup"><span data-stu-id="30acf-602">Additional Info</span></span></td>
<td><p><span data-ttu-id="30acf-603">Informações adicionais não são abordadas em outras colunas.</span><span class="sxs-lookup"><span data-stu-id="30acf-603">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="30acf-604">Encargos de mapeamento entre uma nota fiscal e o arquivo de reconciliação</span><span class="sxs-lookup"><span data-stu-id="30acf-604">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="30acf-605">Sua fatura fornece um resumo dos encargos, enquanto seu arquivo de reconciliação fornece uma divisão detalhada das transações de item de linha, incluindo os tipos de carga.</span><span class="sxs-lookup"><span data-stu-id="30acf-605">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="30acf-606">Para fazer referência cruzada das quantidades de carga entre o arquivo de reconciliação e fatura, você pode usar opções de filtro do Microsoft Excel para filtrar por tipos de cobrança no arquivo de reconciliação para mapear os encargos de fatura em um conjunto de detalhamentos de cobrança no arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="30acf-606">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="30acf-607">Os arquivos de reconciliação, tanto os baseados em licença quanto os baseados em uso, mostram apenas encargos e transações relacionadas ao uso (unidades consumidas e encargos relacionados).</span><span class="sxs-lookup"><span data-stu-id="30acf-607">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="30acf-608">Créditos únicos, descontos ou reembolsos que aparecem na fatura como "Ajustes" não são mostrados no arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="30acf-608">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="30acf-609">A tabela a seguir mostra os mapeamentos entre uma seção da fatura e os tipos de encargo associados que podem aparecer nos arquivos de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="30acf-609">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="30acf-610"><strong>Descrição de encargo de fatura</strong></span><span class="sxs-lookup"><span data-stu-id="30acf-610"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="30acf-611"><strong>Descrição de cobrança de arquivo de reconciliação (ChargeType coluna)</strong></span><span class="sxs-lookup"><span data-stu-id="30acf-611"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="30acf-612"><strong>O que é a cobrança?</strong></span><span class="sxs-lookup"><span data-stu-id="30acf-612"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="30acf-613"><strong>Como faço para mapear esses ChargeTypes à fatura?</strong></span><span class="sxs-lookup"><span data-stu-id="30acf-613"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="30acf-614"><strong>Encargos de licença</strong></span><span class="sxs-lookup"><span data-stu-id="30acf-614"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="30acf-615">Taxa de ativação</span><span class="sxs-lookup"><span data-stu-id="30acf-615">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="30acf-616">O valor cobrado do cliente quando ele usa a assinatura depois de comprá-la.</span><span class="sxs-lookup"><span data-stu-id="30acf-616">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="30acf-617">No arquivo baseado em licença, some a coluna <strong>Quantidade</strong></span><span class="sxs-lookup"><span data-stu-id="30acf-617">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="30acf-618">Taxa de cancelamento</span><span class="sxs-lookup"><span data-stu-id="30acf-618">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="30acf-619">Os encargos proporcionais reembolsados para o cliente quando os assentos associados são alterados</span><span class="sxs-lookup"><span data-stu-id="30acf-619">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="30acf-620">Taxa do ciclo</span><span class="sxs-lookup"><span data-stu-id="30acf-620">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="30acf-621">Encargos periódicos de uma assinatura</span><span class="sxs-lookup"><span data-stu-id="30acf-621">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="30acf-622">Proporcional à instância do ciclo</span><span class="sxs-lookup"><span data-stu-id="30acf-622">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="30acf-623">Os encargos proporcionais cobrados do cliente quando os assentos associados são alterados</span><span class="sxs-lookup"><span data-stu-id="30acf-623">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="30acf-624">Taxas proporcionais durante o cancelamento</span><span class="sxs-lookup"><span data-stu-id="30acf-624">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="30acf-625">Reembolso proporcional para a parte não utilizada do serviço após o cancelamento</span><span class="sxs-lookup"><span data-stu-id="30acf-625">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="30acf-626">Taxas proporcionais durante a compra</span><span class="sxs-lookup"><span data-stu-id="30acf-626">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="30acf-627">O tipo de encargo para uma assinatura ao usar cobranças anuais</span><span class="sxs-lookup"><span data-stu-id="30acf-627">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="30acf-628">Valor de compra</span><span class="sxs-lookup"><span data-stu-id="30acf-628">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="30acf-629">O tipo de encargo para uma assinatura ao usar a cobrança mensal</span><span class="sxs-lookup"><span data-stu-id="30acf-629">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="30acf-630">Taxa proporcional ao renovar</span><span class="sxs-lookup"><span data-stu-id="30acf-630">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="30acf-631">Taxas proporcionais após a renovação da assinatura</span><span class="sxs-lookup"><span data-stu-id="30acf-631">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="30acf-632">Taxa de renovação</span><span class="sxs-lookup"><span data-stu-id="30acf-632">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="30acf-633">Cobrança para renovação de uma assinatura</span><span class="sxs-lookup"><span data-stu-id="30acf-633">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="30acf-634">Taxas proporcionais ao ativar</span><span class="sxs-lookup"><span data-stu-id="30acf-634">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="30acf-635">Taxas proporcionais da ativação até o final do período de cobrança</span><span class="sxs-lookup"><span data-stu-id="30acf-635">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><span data-ttu-id="30acf-636"><strong>Encargos de uso</strong></span><span class="sxs-lookup"><span data-stu-id="30acf-636"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="30acf-637">Avaliar a taxa de uso ao cancelar</span><span class="sxs-lookup"><span data-stu-id="30acf-637">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="30acf-638">Taxa de uso de acesso com o cancelamento para uso não pago durante o período de cobrança atual</span><span class="sxs-lookup"><span data-stu-id="30acf-638">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="30acf-639">No arquivo baseado em uso, some a coluna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="30acf-639">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="30acf-640">Avalie a taxa de uso para o ciclo atual</span><span class="sxs-lookup"><span data-stu-id="30acf-640">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="30acf-641">Taxa de uso de acesso para o período atual de cobrança</span><span class="sxs-lookup"><span data-stu-id="30acf-641">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="30acf-642"><strong>Créditos</strong></span><span class="sxs-lookup"><span data-stu-id="30acf-642"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="30acf-643">Deslocando um item de linha</span><span class="sxs-lookup"><span data-stu-id="30acf-643">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="30acf-644">Reembolso parcial ou integral para um item de linha, incluindo os impostos</span><span class="sxs-lookup"><span data-stu-id="30acf-644">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="30acf-645">No arquivo baseado em licença, some a coluna <strong>TotalForCustomer</strong></span><span class="sxs-lookup"><span data-stu-id="30acf-645">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="30acf-646">No arquivo baseado em uso, some a coluna <strong>PostTaxTotal</strong></span><span class="sxs-lookup"><span data-stu-id="30acf-646">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="30acf-647"><strong>Descontos com base no uso</strong></span><span class="sxs-lookup"><span data-stu-id="30acf-647"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="30acf-648">Desconto de ativação</span><span class="sxs-lookup"><span data-stu-id="30acf-648">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="30acf-649">Desconto aplicado quando a assinatura é ativada</span><span class="sxs-lookup"><span data-stu-id="30acf-649">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="30acf-650">No arquivo baseado em uso, some a coluna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="30acf-650">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="30acf-651">Desconto de ciclo</span><span class="sxs-lookup"><span data-stu-id="30acf-651">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="30acf-652">Desconto aplicado em cobranças periódicas</span><span class="sxs-lookup"><span data-stu-id="30acf-652">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="30acf-653">Desconto de renovação</span><span class="sxs-lookup"><span data-stu-id="30acf-653">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="30acf-654">Desconto aplicado quando a assinatura é renovada</span><span class="sxs-lookup"><span data-stu-id="30acf-654">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="30acf-655">Desconto de cancelamento</span><span class="sxs-lookup"><span data-stu-id="30acf-655">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="30acf-656">Encargos aplicados quando descontos são cancelados</span><span class="sxs-lookup"><span data-stu-id="30acf-656">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="30acf-657"><strong>Descontos de licença</strong></span><span class="sxs-lookup"><span data-stu-id="30acf-657"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="30acf-658"><em>Pode ser aplicado a vários tipos de custo</em></span><span class="sxs-lookup"><span data-stu-id="30acf-658"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="30acf-659">No arquivo baseado em licença, some a coluna <strong>TotalOtherDiscount</strong></span><span class="sxs-lookup"><span data-stu-id="30acf-659">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="30acf-660"><strong>Impostos</strong>&nbsp;ou&nbsp;<strong>IVA</strong></span><span class="sxs-lookup"><span data-stu-id="30acf-660"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="30acf-661"><em>Pode ser aplicado a vários tipos de custo</em></span><span class="sxs-lookup"><span data-stu-id="30acf-661"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="30acf-662"><em>Exceção: &quot;Deslocamento de um item de linha&quot; já inclui os impostos. Ver créditos, acima.</em></span><span class="sxs-lookup"><span data-stu-id="30acf-662"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="30acf-663">Impostos ou impostos sobre valor agregado (IVA)</span><span class="sxs-lookup"><span data-stu-id="30acf-663">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="30acf-664">No arquivo baseado em licença, some a coluna <strong>Imposto</strong></span><span class="sxs-lookup"><span data-stu-id="30acf-664">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="30acf-665">No arquivo baseado em uso, some a coluna <strong>TaxAmount</strong></span><span class="sxs-lookup"><span data-stu-id="30acf-665">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
