---
title: Usar os arquivos de reconciliação | Partner Center
ms.topic: article
ms.date: 03/15/2019
description: Para uma exibição detalhada do item de linha de cada carga, em um ciclo de cobrança, baixe os arquivos de reconciliação do Partner Center.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: fca9897720412a77ac39c86ba31db411c58c2cb0
ms.sourcegitcommit: 1f9078d422af5f8514d79a6ab9c3444500abfe27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2019
ms.locfileid: "67343463"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="4d22b-103">Usar os arquivos de reconciliação</span><span class="sxs-lookup"><span data-stu-id="4d22b-103">Use the reconciliation files</span></span>

<span data-ttu-id="4d22b-104">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="4d22b-104">**Applies to**</span></span>

-  <span data-ttu-id="4d22b-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="4d22b-105">Partner Center</span></span>
-  <span data-ttu-id="4d22b-106">Partner Center para Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="4d22b-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="4d22b-107">Para uma exibição detalhada do item de linha de cada carga, em um ciclo de cobrança, baixe os arquivos de reconciliação do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="4d22b-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="4d22b-108">Os detalhes incluem encargos por assinaturas de cada cliente e eventos detalhados (como a adição de assentos a uma assinatura no meio do período).</span><span class="sxs-lookup"><span data-stu-id="4d22b-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="4d22b-109">Problemas de formatação</span><span class="sxs-lookup"><span data-stu-id="4d22b-109">Formatting issues</span></span>

<span data-ttu-id="4d22b-110">Ocasionalmente, seu arquivo de reconhecimento pode ter problemas de formatação.</span><span class="sxs-lookup"><span data-stu-id="4d22b-110">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="4d22b-111">(Isso pode acontecer, por exemplo, se a localidade EN-US não for usada.) Siga as etapas abaixo para corrigir esses problemas.</span><span class="sxs-lookup"><span data-stu-id="4d22b-111">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="4d22b-112">Abra o arquivo. csv no Excel e selecione a primeira coluna.</span><span class="sxs-lookup"><span data-stu-id="4d22b-112">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="4d22b-113">Na faixa de opções, selecione <strong>dados</strong>e, em seguida, selecione <strong>texto para colunas</strong>.</span><span class="sxs-lookup"><span data-stu-id="4d22b-113">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="4d22b-114">Na conversão de texto ao Assistente de colunas, selecione <strong>delimitada por tipo de arquivo</strong>e, em seguida, selecione <strong>próxima</strong>.</span><span class="sxs-lookup"><span data-stu-id="4d22b-114">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="4d22b-115">No campo dos delimitadores, selecione <strong>vírgula</strong>.</span><span class="sxs-lookup"><span data-stu-id="4d22b-115">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="4d22b-116">Se <strong>guia</strong> é estiver selecionado, você pode deixá-lo.</span><span class="sxs-lookup"><span data-stu-id="4d22b-116">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="4d22b-117">Selecione <strong>Avançar</strong>.</span><span class="sxs-lookup"><span data-stu-id="4d22b-117">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="4d22b-118">No campo de formato de dados de coluna, selecione <strong>data: MDY</strong>e, em seguida, selecione <strong>próxima</strong>.</span><span class="sxs-lookup"><span data-stu-id="4d22b-118">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="4d22b-119">No campo de formato de dados de coluna, selecione <strong>texto</strong> para o valor de todas as colunas e, em seguida, selecione <strong>concluir</strong>.</span><span class="sxs-lookup"><span data-stu-id="4d22b-119">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a name="downloading-a-large-recon-file"></a><span data-ttu-id="4d22b-120">Baixar um arquivo grande de reconhecimento</span><span class="sxs-lookup"><span data-stu-id="4d22b-120">Downloading a large recon file</span></span>

<span data-ttu-id="4d22b-121">Arquivos de reconhecimento podem ficar muito grandes e, às vezes, são difíceis de fazer o download.</span><span class="sxs-lookup"><span data-stu-id="4d22b-121">Recon files can grow very large and are sometimes difficult to download.</span></span> <span data-ttu-id="4d22b-122">Para um script do PowerShell ajudar a fazer o download de arquivos grandes de recon, consulte [itens de linha de nota fiscal Get](https://docs.microsoft.com/en-us/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="4d22b-122">For a PowerShell script to help download large recon files, see [Get invoice line items](https://docs.microsoft.com/en-us/partner-center/develop/get-invoiceline-items).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="4d22b-123">Discriminar pelo parceiro</span><span class="sxs-lookup"><span data-stu-id="4d22b-123">Itemize by partner</span></span>


<span data-ttu-id="4d22b-124">Os parceiros no modelo indireto podem usar esses campos adicionais nos arquivos de reconciliação baseados em uso e em licença para discriminar por revendedor.</span><span class="sxs-lookup"><span data-stu-id="4d22b-124">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="4d22b-125">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="4d22b-125">MPN ID</span></span></th>
<th><span data-ttu-id="4d22b-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d22b-126">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="4d22b-127">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="4d22b-127">MPN ID</span></span></td>
<td><p><span data-ttu-id="4d22b-128">A ID do Microsoft Partner Network (MPN) do parceiro CSP (direta ou indireta).</span><span class="sxs-lookup"><span data-stu-id="4d22b-128">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4d22b-129">ID do MPN do revendedor</span><span class="sxs-lookup"><span data-stu-id="4d22b-129">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="4d22b-130">Só aparece em arquivos de reconciliação para parceiros no modelo indireto.</span><span class="sxs-lookup"><span data-stu-id="4d22b-130">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="4d22b-131">A ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="4d22b-131">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="4d22b-132">Isso corresponde à ID de revendedor listada para a assinatura específica no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="4d22b-132">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="4d22b-133">modo de exibição eTo ou atualização revendedor, no menu do Partner Center, selecione <strong>clientes</strong>, em seguida, escolha o cliente da lista.</span><span class="sxs-lookup"><span data-stu-id="4d22b-133">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="4d22b-134">No menu do cliente, selecione <strong>Assinaturas</strong>, escolha a assinatura na lista.</span><span class="sxs-lookup"><span data-stu-id="4d22b-134">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="4d22b-135">Selecione <strong>Atualizar</strong> para alterar o <strong>Revendedor (ID do MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="4d22b-135">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="4d22b-136">Se um parceiro CSP vendeu a assinatura diretamente para o cliente, sua ID do MPN estará listada duas vezes, como a ID do MPN e a ID do MPN do revendedor.</span><span class="sxs-lookup"><span data-stu-id="4d22b-136">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="4d22b-137">Se um parceiro CSP tiver um revendedor sem ID do MPN, esse valor será definido como a ID do MPN do parceiro.</span><span class="sxs-lookup"><span data-stu-id="4d22b-137">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="4d22b-138">Se o parceiro CSP remover uma ID de revendedor, esse valor será definido como -1.</span><span class="sxs-lookup"><span data-stu-id="4d22b-138">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="4d22b-139">Campos de arquivo de licença</span><span class="sxs-lookup"><span data-stu-id="4d22b-139">License-based file fields</span></span>


<span data-ttu-id="4d22b-140">Para reconciliar seus encargos com os pedidos de seu cliente, compare o campo Syndication\_Partner\_Subscription\_Number do arquivo de reconciliação com a ID de Assinatura do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="4d22b-140">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="4d22b-141"><strong>Coluna</strong></span><span class="sxs-lookup"><span data-stu-id="4d22b-141"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="4d22b-142"><strong>Descrição</strong></span><span class="sxs-lookup"><span data-stu-id="4d22b-142"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="4d22b-143"><strong>Valor de exemplo</strong></span><span class="sxs-lookup"><span data-stu-id="4d22b-143"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4d22b-144">PartnerID</span><span class="sxs-lookup"><span data-stu-id="4d22b-144">PartnerId</span></span></td>
<td><p><span data-ttu-id="4d22b-145">Identificador exclusivo de uma entidade de cobrança específica, em formato GUID.</span><span class="sxs-lookup"><span data-stu-id="4d22b-145">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="4d22b-146">Não é necessário para reconciliação, mas pode ser uma informação útil.</span><span class="sxs-lookup"><span data-stu-id="4d22b-146">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="4d22b-147">O mesmo em todas as linhas.</span><span class="sxs-lookup"><span data-stu-id="4d22b-147">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="4d22b-148">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="4d22b-148">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4d22b-149">CustomerID</span><span class="sxs-lookup"><span data-stu-id="4d22b-149">CustomerID</span></span></td>
<td><p><span data-ttu-id="4d22b-150">ID exclusiva da Microsoft, no formato GUID, usada para identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="4d22b-150">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="4d22b-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="4d22b-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4d22b-152">OrderID</span><span class="sxs-lookup"><span data-stu-id="4d22b-152">OrderID</span></span></td>
<td><p><span data-ttu-id="4d22b-153">Identificador exclusivo para um pedido na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="4d22b-153">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="4d22b-154">Pode ser útil para identificar o pedido ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="4d22b-154">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="4d22b-155">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="4d22b-155">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4d22b-156">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="4d22b-156">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="4d22b-157">Identificador exclusivo de uma assinatura na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="4d22b-157">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="4d22b-158">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="4d22b-158">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="4d22b-159">Esse não é o mesmo que o ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="4d22b-159">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="4d22b-160">Consulte Número_Assinatura_Parceiro_Sindicalização.</span><span class="sxs-lookup"><span data-stu-id="4d22b-160">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="4d22b-161">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="4d22b-161">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4d22b-162">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="4d22b-162">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="4d22b-163">Identificador exclusivo para assinaturas.</span><span class="sxs-lookup"><span data-stu-id="4d22b-163">Unique identifier for subscriptions.</span></span> <span data-ttu-id="4d22b-164">Target: Um cliente pode ter várias assinaturas para o mesmo plano, portanto, isso é importante para análise de arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="4d22b-164">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="4d22b-165">Esse campo é mapeado para a ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="4d22b-165">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="4d22b-166">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="4d22b-166">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4d22b-167">OfferID</span><span class="sxs-lookup"><span data-stu-id="4d22b-167">OfferID</span></span></td>
<td><p><span data-ttu-id="4d22b-168">ID exclusivo da oferta.</span><span class="sxs-lookup"><span data-stu-id="4d22b-168">Unique offer ID.</span></span> <span data-ttu-id="4d22b-169">ID padrão da oferta de acordo com a lista de preços.</span><span class="sxs-lookup"><span data-stu-id="4d22b-169">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="4d22b-170"><b>Observação</b>: Esse valor não corresponde a ID da oferta da lista de preços.</span><span class="sxs-lookup"><span data-stu-id="4d22b-170"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="4d22b-171">Veja DurableOfferID abaixo.</span><span class="sxs-lookup"><span data-stu-id="4d22b-171">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="4d22b-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="4d22b-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4d22b-173">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="4d22b-173">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="4d22b-174">ID exclusivo da oferta durável, conforme definido na tabela de preços.</span><span class="sxs-lookup"><span data-stu-id="4d22b-174">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="4d22b-175"><b>Observação</b>: Esse valor corresponde à ID da oferta da lista de preços.</span><span class="sxs-lookup"><span data-stu-id="4d22b-175"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="4d22b-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="4d22b-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4d22b-177">OfferName</span><span class="sxs-lookup"><span data-stu-id="4d22b-177">OfferName</span></span></td>
<td><p><span data-ttu-id="4d22b-178">O nome da oferta de serviço comprada pelo cliente, conforme definido na tabela de preços.</span><span class="sxs-lookup"><span data-stu-id="4d22b-178">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="4d22b-179">Microsoft Office 365 (plano E3)</span><span class="sxs-lookup"><span data-stu-id="4d22b-179">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4d22b-180">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="4d22b-180">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="4d22b-181">A data de início da assinatura, definida como um dia após o pedido ser enviado.</span><span class="sxs-lookup"><span data-stu-id="4d22b-181">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="4d22b-182">Verificando a data de início da assinatura em conjunto com a data de término, você pode determinar se o cliente está dentro do primeiro ano da assinatura ou se a assinatura foi renovada para o ano seguinte.</span><span class="sxs-lookup"><span data-stu-id="4d22b-182">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="4d22b-183">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="4d22b-183">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="4d22b-184">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="4d22b-184">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4d22b-185">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="4d22b-185">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="4d22b-186">A data de término da assinatura: + x dias após a data de início (para alinhar com data de cobrança do parceiro) ou 12 meses a partir da data de renovação de 12 meses.</span><span class="sxs-lookup"><span data-stu-id="4d22b-186">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="4d22b-187">Na renovação, os preços são atualizados com a tabela de preços atual.</span><span class="sxs-lookup"><span data-stu-id="4d22b-187">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="4d22b-188">Um comunicado ao cliente pode ser necessário antes da renovação automática.</span><span class="sxs-lookup"><span data-stu-id="4d22b-188">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="4d22b-189">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="4d22b-189">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="4d22b-190">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="4d22b-190">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4d22b-191">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="4d22b-191">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="4d22b-192">Dia de início dos encargos.</span><span class="sxs-lookup"><span data-stu-id="4d22b-192">Start day of the charges.</span></span></p>
<p><span data-ttu-id="4d22b-193">Quando o cliente muda o número de assentos, esse número é usado para calcular os encargos por dia (pro-rata).</span><span class="sxs-lookup"><span data-stu-id="4d22b-193">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="4d22b-194">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="4d22b-194">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="4d22b-195">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="4d22b-195">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4d22b-196">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="4d22b-196">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="4d22b-197">Dia do término dos encargos.</span><span class="sxs-lookup"><span data-stu-id="4d22b-197">End day of the charges.</span></span></p>
<p><span data-ttu-id="4d22b-198">Quando o cliente muda o número de assentos, esse número é usado para calcular os encargos por dia (pro-rata).</span><span class="sxs-lookup"><span data-stu-id="4d22b-198">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="4d22b-199">A hora é sempre o fim do dia, 23:59.</span><span class="sxs-lookup"><span data-stu-id="4d22b-199">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="4d22b-200">28/2/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="4d22b-200">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4d22b-201">ChargeType</span><span class="sxs-lookup"><span data-stu-id="4d22b-201">ChargeType</span></span></td>
<td><p><span data-ttu-id="4d22b-202">O tipo de encargo ou ajuste.</span><span class="sxs-lookup"><span data-stu-id="4d22b-202">The type of charge or adjustment.</span></span> <span data-ttu-id="4d22b-203">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="4d22b-203">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="4d22b-204">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="4d22b-204">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4d22b-205">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="4d22b-205">UnitPrice</span></span></td>
<td><p><span data-ttu-id="4d22b-206">Preço por estação, conforme publicado na lista de preços no momento da compra.</span><span class="sxs-lookup"><span data-stu-id="4d22b-206">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="4d22b-207">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="4d22b-207">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="4d22b-208">6.82</span><span class="sxs-lookup"><span data-stu-id="4d22b-208">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4d22b-209">Quantidade</span><span class="sxs-lookup"><span data-stu-id="4d22b-209">Quantity</span></span></td>
<td><p><span data-ttu-id="4d22b-210">Número de assentos.</span><span class="sxs-lookup"><span data-stu-id="4d22b-210">Number of seats.</span></span> <span data-ttu-id="4d22b-211">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="4d22b-211">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="4d22b-212">2</span><span class="sxs-lookup"><span data-stu-id="4d22b-212">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4d22b-213">Valor</span><span class="sxs-lookup"><span data-stu-id="4d22b-213">Amount</span></span></td>
<td><p><span data-ttu-id="4d22b-214">Preço total por quantidade.</span><span class="sxs-lookup"><span data-stu-id="4d22b-214">Total of price for quantity.</span></span> <span data-ttu-id="4d22b-215">Útil para verificar se o cálculo do valor coincide com a forma como você calcula isso para seus clientes.</span><span class="sxs-lookup"><span data-stu-id="4d22b-215">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="4d22b-216">13.32</span><span class="sxs-lookup"><span data-stu-id="4d22b-216">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4d22b-217">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="4d22b-217">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="4d22b-218">Valor de desconto aplicado a esses encargos.</span><span class="sxs-lookup"><span data-stu-id="4d22b-218">Amount of discount applied to these charges.</span></span> <span data-ttu-id="4d22b-219">IUR ou novas assinaturas qualificadas para incentivo também conterão um valor de desconto nessa coluna.</span><span class="sxs-lookup"><span data-stu-id="4d22b-219">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="4d22b-220">2.32</span><span class="sxs-lookup"><span data-stu-id="4d22b-220">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4d22b-221">Subtotal</span><span class="sxs-lookup"><span data-stu-id="4d22b-221">Subtotal</span></span></td>
<td><p><span data-ttu-id="4d22b-222">Total sem imposto.</span><span class="sxs-lookup"><span data-stu-id="4d22b-222">Total before tax.</span></span> <span data-ttu-id="4d22b-223">Verifica se seu subtotal corresponde ao total esperado, em caso de desconto.</span><span class="sxs-lookup"><span data-stu-id="4d22b-223">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="4d22b-224">11</span><span class="sxs-lookup"><span data-stu-id="4d22b-224">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4d22b-225">Tax</span><span class="sxs-lookup"><span data-stu-id="4d22b-225">Tax</span></span></td>
<td><p><span data-ttu-id="4d22b-226">Encargo de valor, com base em seu mercado de imposto&#39;regras de imposto de s e as circunstâncias específicas.</span><span class="sxs-lookup"><span data-stu-id="4d22b-226">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="4d22b-227">0</span><span class="sxs-lookup"><span data-stu-id="4d22b-227">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4d22b-228">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="4d22b-228">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="4d22b-229">Total com imposto.</span><span class="sxs-lookup"><span data-stu-id="4d22b-229">Total after tax.</span></span> <span data-ttu-id="4d22b-230">Verifica se o imposto é cobrado na fatura.</span><span class="sxs-lookup"><span data-stu-id="4d22b-230">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="4d22b-231">11</span><span class="sxs-lookup"><span data-stu-id="4d22b-231">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4d22b-232">Currency</span><span class="sxs-lookup"><span data-stu-id="4d22b-232">Currency</span></span></td>
<td><p><span data-ttu-id="4d22b-233">Tipo de moeda.</span><span class="sxs-lookup"><span data-stu-id="4d22b-233">Currency type.</span></span> <span data-ttu-id="4d22b-234">Cada entidade de cobrança tem somente uma moeda.</span><span class="sxs-lookup"><span data-stu-id="4d22b-234">Each billing entity has only one currency.</span></span> <span data-ttu-id="4d22b-235">Verifique se isso coincide com a primeira fatura e faça o mesmo após grandes atualizações na plataforma de cobrança.</span><span class="sxs-lookup"><span data-stu-id="4d22b-235">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="4d22b-236">EUR</span><span class="sxs-lookup"><span data-stu-id="4d22b-236">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4d22b-237">CustomerName</span><span class="sxs-lookup"><span data-stu-id="4d22b-237">CustomerName</span></span></td>
<td><p><span data-ttu-id="4d22b-238">Cliente&#39;nome da organização s conforme relatado no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="4d22b-238">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="4d22b-239">Isso é muito importante para reconciliar a fatura com as informações de seu sistema.</span><span class="sxs-lookup"><span data-stu-id="4d22b-239">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="4d22b-240">Cliente de teste A</span><span class="sxs-lookup"><span data-stu-id="4d22b-240">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4d22b-241">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="4d22b-241">MPNID</span></span></td>
<td><p><span data-ttu-id="4d22b-242">ID do MPN do parceiro CSP</span><span class="sxs-lookup"><span data-stu-id="4d22b-242">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="4d22b-243">4390934</span><span class="sxs-lookup"><span data-stu-id="4d22b-243">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4d22b-244">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="4d22b-244">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="4d22b-245">ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="4d22b-245">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="4d22b-246">Consulte <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Discriminar por parceiro</a>.</span><span class="sxs-lookup"><span data-stu-id="4d22b-246">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="4d22b-247">4390934</span><span class="sxs-lookup"><span data-stu-id="4d22b-247">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4d22b-248">DomainName</span><span class="sxs-lookup"><span data-stu-id="4d22b-248">DomainName</span></span></td>
<td><p><span data-ttu-id="4d22b-249">Cliente&#39;nome de domínio s, usado para ajudar a identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="4d22b-249">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="4d22b-250">Isso não deve ser usado para identificar exclusivamente o cliente, assim como o cliente/parceiro pode atualizar o domínio intuitivo/padrão por meio do portal do O365.</span><span class="sxs-lookup"><span data-stu-id="4d22b-250">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="4d22b-251">Este campo pode aparecer em branco até o segundo ciclo de cobrança.</span><span class="sxs-lookup"><span data-stu-id="4d22b-251">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="4d22b-252">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="4d22b-252">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4d22b-253">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="4d22b-253">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="4d22b-254">Apelido da Inscrição.</span><span class="sxs-lookup"><span data-stu-id="4d22b-254">Subscription nickname.</span></span> <span data-ttu-id="4d22b-255">Se nenhum apelido for especificado, o Partner Center usa o OfferName.</span><span class="sxs-lookup"><span data-stu-id="4d22b-255">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="4d22b-256">PROJETO ONLINE</span><span class="sxs-lookup"><span data-stu-id="4d22b-256">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4d22b-257">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="4d22b-257">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="4d22b-258">O nome da oferta de serviço comprada pelo cliente, conforme definido na tabela de preços.</span><span class="sxs-lookup"><span data-stu-id="4d22b-258">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="4d22b-259">(Este é um campo idêntico ao nome da oferta).</span><span class="sxs-lookup"><span data-stu-id="4d22b-259">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="4d22b-260">PROJETO ONLINE PREMIUM SEM PROJETO CLIENTE</span><span class="sxs-lookup"><span data-stu-id="4d22b-260">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="4d22b-261">Campos de arquivo baseada em uso</span><span class="sxs-lookup"><span data-stu-id="4d22b-261">Usage-based file fields</span></span>


<span data-ttu-id="4d22b-262">Para reconciliar seus encargos com o uso de seu cliente, compare ResellerID/ResellerName/ResellerBillableAccount do arquivo de reconciliação com o nome do cliente e a ID da assinatura do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="4d22b-262">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="4d22b-263">Os campos a seguir explicam quais serviços foram usados e a taxa.</span><span class="sxs-lookup"><span data-stu-id="4d22b-263">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="4d22b-264"><strong>Coluna</strong></span><span class="sxs-lookup"><span data-stu-id="4d22b-264"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="4d22b-265"><strong>Descrição</strong></span><span class="sxs-lookup"><span data-stu-id="4d22b-265"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="4d22b-266"><strong>Valor de exemplo</strong></span><span class="sxs-lookup"><span data-stu-id="4d22b-266"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4d22b-267">PartnerID</span><span class="sxs-lookup"><span data-stu-id="4d22b-267">PartnerID</span></span></td>
<td><p><span data-ttu-id="4d22b-268">ID do parceiro, no formato GUID.</span><span class="sxs-lookup"><span data-stu-id="4d22b-268">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="4d22b-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="4d22b-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4d22b-270">PartnerName</span><span class="sxs-lookup"><span data-stu-id="4d22b-270">PartnerName</span></span></td>
<td><p><span data-ttu-id="4d22b-271">Nome do parceiro.</span><span class="sxs-lookup"><span data-stu-id="4d22b-271">Partner Name.</span></span></p></td>
<td><span data-ttu-id="4d22b-272">Acme incorporado</span><span class="sxs-lookup"><span data-stu-id="4d22b-272">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4d22b-273">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="4d22b-273">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="4d22b-274">ID da conta do parceiro.</span><span class="sxs-lookup"><span data-stu-id="4d22b-274">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="4d22b-275">1010578050</span><span class="sxs-lookup"><span data-stu-id="4d22b-275">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4d22b-276">CustomerName</span><span class="sxs-lookup"><span data-stu-id="4d22b-276">CustomerName</span></span></td>
<td><p><span data-ttu-id="4d22b-277">Cliente&#39;nome da organização s conforme relatado no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="4d22b-277">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="4d22b-278">Isso é muito importante para reconciliar a fatura com as informações de seu sistema.</span><span class="sxs-lookup"><span data-stu-id="4d22b-278">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="4d22b-279">Cliente de teste A</span><span class="sxs-lookup"><span data-stu-id="4d22b-279">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4d22b-280">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="4d22b-280">MPNID</span></span></td>
<td><p><span data-ttu-id="4d22b-281">ID do MPN do parceiro CSP.</span><span class="sxs-lookup"><span data-stu-id="4d22b-281">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="4d22b-282">4390934</span><span class="sxs-lookup"><span data-stu-id="4d22b-282">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4d22b-283">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="4d22b-283">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="4d22b-284">ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="4d22b-284">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="4d22b-285">Consulte <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Discriminar por parceiro</a>.</span><span class="sxs-lookup"><span data-stu-id="4d22b-285">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="4d22b-286">4390934</span><span class="sxs-lookup"><span data-stu-id="4d22b-286">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4d22b-287">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="4d22b-287">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="4d22b-288">Número da fatura na qual a transação especificada é exibida.</span><span class="sxs-lookup"><span data-stu-id="4d22b-288">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="4d22b-289">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="4d22b-289">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4d22b-290">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="4d22b-290">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="4d22b-291">Data de início do ciclo de cobrança exceto quando apresentadas as datas de dados de uso latentes anteriormente não cobradas (do ciclo de cobrança anterior).</span><span class="sxs-lookup"><span data-stu-id="4d22b-291">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="4d22b-292">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="4d22b-292">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="4d22b-293">1/2/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="4d22b-293">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4d22b-294">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="4d22b-294">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="4d22b-295">Data de término do ciclo de cobrança exceto quando apresentadas as datas de dados de uso latentes anteriormente não cobradas (do ciclo de cobrança anterior).</span><span class="sxs-lookup"><span data-stu-id="4d22b-295">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="4d22b-296">A hora é sempre o fim do dia, 23:59.</span><span class="sxs-lookup"><span data-stu-id="4d22b-296">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="4d22b-297">28/2/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="4d22b-297">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4d22b-298">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="4d22b-298">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="4d22b-299">Identificador exclusivo de uma assinatura na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="4d22b-299">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="4d22b-300">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="4d22b-300">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="4d22b-301">Esse não é o mesmo que o ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="4d22b-301">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="4d22b-302">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="4d22b-302">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4d22b-303">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="4d22b-303">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="4d22b-304">Apelido da oferta do serviço.</span><span class="sxs-lookup"><span data-stu-id="4d22b-304">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="4d22b-305">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="4d22b-305">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4d22b-306">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="4d22b-306">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="4d22b-307">Linha de negócios da oferta do serviço</span><span class="sxs-lookup"><span data-stu-id="4d22b-307">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="4d22b-308">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="4d22b-308">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4d22b-309">OrderID</span><span class="sxs-lookup"><span data-stu-id="4d22b-309">OrderID</span></span></td>
<td><p><span data-ttu-id="4d22b-310">Identificador exclusivo para um pedido na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="4d22b-310">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="4d22b-311">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="4d22b-311">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="4d22b-312">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="4d22b-312">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4d22b-313">ServiceName</span><span class="sxs-lookup"><span data-stu-id="4d22b-313">ServiceName</span></span></td>
<td><p><span data-ttu-id="4d22b-314">O nome do serviço do Azure em questão.</span><span class="sxs-lookup"><span data-stu-id="4d22b-314">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="4d22b-315">MÁQUINAS VIRTUAIS</span><span class="sxs-lookup"><span data-stu-id="4d22b-315">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4d22b-316">ServiceType</span><span class="sxs-lookup"><span data-stu-id="4d22b-316">ServiceType</span></span></td>
<td><p><span data-ttu-id="4d22b-317">O tipo específico de serviço do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="4d22b-317">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="4d22b-318">Service Bus – Individual ou pacote</span><span class="sxs-lookup"><span data-stu-id="4d22b-318">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="4d22b-319">Banco de dados SQL Azure – Edição empresa ou Web</span><span class="sxs-lookup"><span data-stu-id="4d22b-319">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4d22b-320">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="4d22b-320">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="4d22b-321">Identificador exclusivo específico de toda a estrutura de serviço de dados e preço.</span><span class="sxs-lookup"><span data-stu-id="4d22b-321">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="4d22b-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="4d22b-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4d22b-323">Nome do recurso</span><span class="sxs-lookup"><span data-stu-id="4d22b-323">Resource Name</span></span></td>
<td><p><span data-ttu-id="4d22b-324">O nome do recurso do Azure.</span><span class="sxs-lookup"><span data-stu-id="4d22b-324">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="4d22b-325">Dados de entrada transferidos (GB)</span><span class="sxs-lookup"><span data-stu-id="4d22b-325">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="4d22b-326">Dados de saída transferidos (GB)</span><span class="sxs-lookup"><span data-stu-id="4d22b-326">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4d22b-327">Region</span><span class="sxs-lookup"><span data-stu-id="4d22b-327">Region</span></span></td>
<td><p><span data-ttu-id="4d22b-328">A região a qual o uso se aplica.</span><span class="sxs-lookup"><span data-stu-id="4d22b-328">The region the usage applies to.</span></span> <span data-ttu-id="4d22b-329">Usado principalmente para atribuir as taxas de transferências de dados, já que as taxas variam de acordo com a região.</span><span class="sxs-lookup"><span data-stu-id="4d22b-329">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="4d22b-330">Pacífico Asiático, Europa, América Latina e América do Norte</span><span class="sxs-lookup"><span data-stu-id="4d22b-330">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4d22b-331">SKU</span><span class="sxs-lookup"><span data-stu-id="4d22b-331">SKU</span></span></td>
<td><p><span data-ttu-id="4d22b-332">Identificador exclusivo MSFT da oferta</span><span class="sxs-lookup"><span data-stu-id="4d22b-332">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="4d22b-333">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="4d22b-333">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="4d22b-334">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="4d22b-334">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="4d22b-335">Uma ID e a quantidade para discriminar as taxas diferentes de um serviço ou recurso em um determinado período de cobrança.</span><span class="sxs-lookup"><span data-stu-id="4d22b-335">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="4d22b-336">Para a classificação em camadas do Azure, pode haver uma taxa para uma determinada quantidade de unidades faturáveis e uma taxa diferente depois disso.</span><span class="sxs-lookup"><span data-stu-id="4d22b-336">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="4d22b-337">1</span><span class="sxs-lookup"><span data-stu-id="4d22b-337">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4d22b-338">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="4d22b-338">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="4d22b-339">A quantidade de serviço consumida (horas, GB etc.) durante o período de relatório.</span><span class="sxs-lookup"><span data-stu-id="4d22b-339">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="4d22b-340">Também inclui qualquer uso não cobrado de períodos de relatório anteriores.</span><span class="sxs-lookup"><span data-stu-id="4d22b-340">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="4d22b-341">11</span><span class="sxs-lookup"><span data-stu-id="4d22b-341">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4d22b-342">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="4d22b-342">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="4d22b-343">Unidades incluídas como parte da oferta.</span><span class="sxs-lookup"><span data-stu-id="4d22b-343">Units included as part of the offer.</span></span> <span data-ttu-id="4d22b-344">Normalmente não está presente no CSP.</span><span class="sxs-lookup"><span data-stu-id="4d22b-344">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="4d22b-345">0</span><span class="sxs-lookup"><span data-stu-id="4d22b-345">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="4d22b-346">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="4d22b-346">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="4d22b-347">Unidades não incluídas como parte da oferta devem ser pagas pelo parceiro.</span><span class="sxs-lookup"><span data-stu-id="4d22b-347">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="4d22b-348">Igual a ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="4d22b-348">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="4d22b-349">11</span><span class="sxs-lookup"><span data-stu-id="4d22b-349">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4d22b-350">ListPrice</span><span class="sxs-lookup"><span data-stu-id="4d22b-350">ListPrice</span></span></td>
<td><p><span data-ttu-id="4d22b-351">Preço da oferta em vigor na data de início da assinatura.</span><span class="sxs-lookup"><span data-stu-id="4d22b-351">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="4d22b-352">U$ 0,0808</span><span class="sxs-lookup"><span data-stu-id="4d22b-352">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4d22b-353">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="4d22b-353">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="4d22b-354">ListPrist vezes OverageQuantity, arredondado para o centavo mais próximo.</span><span class="sxs-lookup"><span data-stu-id="4d22b-354">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="4d22b-355">U$ 0,085</span><span class="sxs-lookup"><span data-stu-id="4d22b-355">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4d22b-356">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="4d22b-356">TaxAmount</span></span></td>
<td><p><span data-ttu-id="4d22b-357">Encargo de valor, com base em seu mercado de imposto&#39;regras de imposto de s e as circunstâncias específicas.</span><span class="sxs-lookup"><span data-stu-id="4d22b-357">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="4d22b-358">U$ 0,08</span><span class="sxs-lookup"><span data-stu-id="4d22b-358">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4d22b-359">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="4d22b-359">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="4d22b-360">Total após imposto, quando o imposto é aplicável.</span><span class="sxs-lookup"><span data-stu-id="4d22b-360">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="4d22b-361">U$ 0,93</span><span class="sxs-lookup"><span data-stu-id="4d22b-361">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4d22b-362">Currency</span><span class="sxs-lookup"><span data-stu-id="4d22b-362">Currency</span></span></td>
<td><p><span data-ttu-id="4d22b-363">Tipo de moeda.</span><span class="sxs-lookup"><span data-stu-id="4d22b-363">Currency type.</span></span> <span data-ttu-id="4d22b-364">Cada entidade de cobrança tem somente uma moeda.</span><span class="sxs-lookup"><span data-stu-id="4d22b-364">Each billing entity has only one currency.</span></span> <span data-ttu-id="4d22b-365">Verifique se isso coincide com a primeira fatura e faça o mesmo após grandes atualizações na plataforma de cobrança.</span><span class="sxs-lookup"><span data-stu-id="4d22b-365">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="4d22b-366">EUR</span><span class="sxs-lookup"><span data-stu-id="4d22b-366">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4d22b-367">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="4d22b-367">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="4d22b-368">Preço por unidade sem imposto.</span><span class="sxs-lookup"><span data-stu-id="4d22b-368">Pretax price per unit.</span></span> <span data-ttu-id="4d22b-369">Igual a PretaxCharges / OverageQuantity, arredondado para o centavo mais próximo.</span><span class="sxs-lookup"><span data-stu-id="4d22b-369">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="4d22b-370">U$ 0,08</span><span class="sxs-lookup"><span data-stu-id="4d22b-370">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4d22b-371">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="4d22b-371">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="4d22b-372">Preço pós-imposto por unidade.</span><span class="sxs-lookup"><span data-stu-id="4d22b-372">Post tax price per unit.</span></span> <span data-ttu-id="4d22b-373">Igual a PostTaxTotal / OverageQuantity, ou PretaxEffectiveRate + taxa de imposto por valor de unidade, arredondado para o centavo mais próximo.</span><span class="sxs-lookup"><span data-stu-id="4d22b-373">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="4d22b-374">U$ 0,08</span><span class="sxs-lookup"><span data-stu-id="4d22b-374">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4d22b-375">ChargeType</span><span class="sxs-lookup"><span data-stu-id="4d22b-375">ChargeType</span></span></td>
<td><p><span data-ttu-id="4d22b-376">O tipo de encargo ou ajuste.</span><span class="sxs-lookup"><span data-stu-id="4d22b-376">The type of charge or adjustment.</span></span> <span data-ttu-id="4d22b-377">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="4d22b-377">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="4d22b-378">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="4d22b-378">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4d22b-379">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="4d22b-379">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="4d22b-380">ID exclusiva da conta na plataforma de cobrança da MSFT.</span><span class="sxs-lookup"><span data-stu-id="4d22b-380">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="4d22b-381">1280018095</span><span class="sxs-lookup"><span data-stu-id="4d22b-381">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4d22b-382">UsageDate</span><span class="sxs-lookup"><span data-stu-id="4d22b-382">UsageDate</span></span></td>
<td><p><span data-ttu-id="4d22b-383">Data da implantação do serviço.</span><span class="sxs-lookup"><span data-stu-id="4d22b-383">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="4d22b-384">1/2/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="4d22b-384">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4d22b-385">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="4d22b-385">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="4d22b-386">Essa coluna identifica a localização de um data center dentro da região para serviços onde isso é aplicável e preenchido.</span><span class="sxs-lookup"><span data-stu-id="4d22b-386">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="4d22b-387">Leste da Ásia, Sudeste da Ásia, Norte da Europa, Europa Ocidental, Centro Norte e Centro Sul dos EUA</span><span class="sxs-lookup"><span data-stu-id="4d22b-387">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4d22b-388">MeteredService</span><span class="sxs-lookup"><span data-stu-id="4d22b-388">MeteredService</span></span></td>
<td><p><span data-ttu-id="4d22b-389">Essa coluna é utilizada para rastrear o serviço do Microsoft Azure individual que não pode ser identificado especificamente na coluna Nome do Serviço.</span><span class="sxs-lookup"><span data-stu-id="4d22b-389">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="4d22b-390">Por exemplo, transferências de dados são relatadas como &quot;Microsoft Azure – Todos os Serviços&quot; na coluna Nome do Serviço.</span><span class="sxs-lookup"><span data-stu-id="4d22b-390">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="4d22b-391">Essa coluna MeteredService indicará ao qual serviço específico o uso pertence.</span><span class="sxs-lookup"><span data-stu-id="4d22b-391">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="4d22b-392">AccessControl, CDN, Computação, Banco de dados, ServiceBus, Armazenamento</span><span class="sxs-lookup"><span data-stu-id="4d22b-392">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4d22b-393">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="4d22b-393">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="4d22b-394">Um subcabeçalho que esclarece ainda mais o serviço Microsoft Azure individual além do nível fornecido pelo campo MeteredService.</span><span class="sxs-lookup"><span data-stu-id="4d22b-394">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="4d22b-395">EXTERNO</span><span class="sxs-lookup"><span data-stu-id="4d22b-395">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4d22b-396">Projeto</span><span class="sxs-lookup"><span data-stu-id="4d22b-396">Project</span></span></td>
<td><p><span data-ttu-id="4d22b-397">Nome definido pelo cliente para a instância do serviço</span><span class="sxs-lookup"><span data-stu-id="4d22b-397">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="4d22b-398">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="4d22b-398">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4d22b-399">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="4d22b-399">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="4d22b-400">O número de conexões ServiceBus que foram provisionados e utilizados em um dia específico.</span><span class="sxs-lookup"><span data-stu-id="4d22b-400">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="4d22b-401">Por exemplo: se você tivesse uma conexão individualmente provisionada durante um mês de 30 dias, a coluna Informação do Serviço 1 lerá "1,000000 conexões/30 dias".</span><span class="sxs-lookup"><span data-stu-id="4d22b-401">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="4d22b-402">Se você tivesse um pacote de 25 de conexões de barramento de serviço provisionado e você tinha utilizou 1 durante o dia, sua instrução de uso diário para esse dia indicaria "25 conexões / 30 dias – usado: 1.000000”.</span><span class="sxs-lookup"><span data-stu-id="4d22b-402">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4d22b-403">CustomerID</span><span class="sxs-lookup"><span data-stu-id="4d22b-403">CustomerID</span></span></td>
<td><p><span data-ttu-id="4d22b-404">ID exclusiva da Microsoft, no formato GUID, usada para identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="4d22b-404">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="4d22b-405">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="4d22b-405">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4d22b-406">DomainName</span><span class="sxs-lookup"><span data-stu-id="4d22b-406">DomainName</span></span></td>
<td><p><span data-ttu-id="4d22b-407">Cliente&#39;nome de domínio s, usado para ajudar a identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="4d22b-407">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="4d22b-408">Este campo pode aparecer em branco até o segundo ciclo de cobrança.</span><span class="sxs-lookup"><span data-stu-id="4d22b-408">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="4d22b-409">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="4d22b-409">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="4d22b-410">Unidade</span><span class="sxs-lookup"><span data-stu-id="4d22b-410">Unit</span></span></td>
<td><p><span data-ttu-id="4d22b-411">A unidade do nome do recurso</span><span class="sxs-lookup"><span data-stu-id="4d22b-411">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="4d22b-412">GB ou HORAS</span><span class="sxs-lookup"><span data-stu-id="4d22b-412">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="4d22b-413">Campos de arquivo únicos e recorrentes</span><span class="sxs-lookup"><span data-stu-id="4d22b-413">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="4d22b-414">Column</span><span class="sxs-lookup"><span data-stu-id="4d22b-414">Column</span></span></th>
<th><span data-ttu-id="4d22b-415">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d22b-415">Description</span></span></th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td><span data-ttu-id="4d22b-416">PartnerID</span><span class="sxs-lookup"><span data-stu-id="4d22b-416">PartnerId</span></span></td>
<td><p><span data-ttu-id="4d22b-417">Identificador exclusivo do locatário Microsoft Azure Active Directory para uma entidade específica de cobrança, no formato GUID.</span><span class="sxs-lookup"><span data-stu-id="4d22b-417">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="4d22b-418">Não é necessário para reconciliação, mas pode ser uma informação útil.</span><span class="sxs-lookup"><span data-stu-id="4d22b-418">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="4d22b-419">O mesmo em todas as linhas.</span><span class="sxs-lookup"><span data-stu-id="4d22b-419">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4d22b-420">Id do cliente</span><span class="sxs-lookup"><span data-stu-id="4d22b-420">Customer Id</span></span></td>
<td><p><span data-ttu-id="4d22b-421">Microsoft Azure Active Directory locatário ID exclusiva, no formato GUID, usado para identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="4d22b-421">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4d22b-422">Nome do cliente</span><span class="sxs-lookup"><span data-stu-id="4d22b-422">Customer Name</span></span></td>
<td><p><span data-ttu-id="4d22b-423">Nome da organização do cliente como informado no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="4d22b-423">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4d22b-424">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="4d22b-424">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="4d22b-425">Nome de domínio do cliente, usado para ajudar a identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="4d22b-425">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="4d22b-426">Isso não deve ser usado para identificar exclusivamente o cliente, assim como o cliente/parceiro pode atualizar o domínio intuitivo/padrão por meio do portal do O365.</span><span class="sxs-lookup"><span data-stu-id="4d22b-426">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="4d22b-427">Este campo pode aparecer em branco até o segundo ciclo de cobrança.</span><span class="sxs-lookup"><span data-stu-id="4d22b-427">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4d22b-428">País do cliente</span><span class="sxs-lookup"><span data-stu-id="4d22b-428">Customer Country</span></span></td>
<td><p><span data-ttu-id="4d22b-429">O país em que o cliente está localizado.</span><span class="sxs-lookup"><span data-stu-id="4d22b-429">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4d22b-430">Número da fatura</span><span class="sxs-lookup"><span data-stu-id="4d22b-430">Invoice number</span></span></td>
<td><p><span data-ttu-id="4d22b-431">Número da fatura na qual a transação especificada é exibida.</span><span class="sxs-lookup"><span data-stu-id="4d22b-431">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4d22b-432">MpnID</span><span class="sxs-lookup"><span data-stu-id="4d22b-432">MpnId</span></span></td>
<td><p><span data-ttu-id="4d22b-433">ID do MPN do parceiro CSP.</span><span class="sxs-lookup"><span data-stu-id="4d22b-433">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4d22b-434">Reseller MpnId</span><span class="sxs-lookup"><span data-stu-id="4d22b-434">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="4d22b-435">ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="4d22b-435">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4d22b-436">ID do Pedido</span><span class="sxs-lookup"><span data-stu-id="4d22b-436">Order ID</span></span></td>
<td><p><span data-ttu-id="4d22b-437">Identificador exclusivo para um pedido na plataforma de comércio do Microsoft.</span><span class="sxs-lookup"><span data-stu-id="4d22b-437">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="4d22b-438">Pode ser útil para identificar o pedido ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="4d22b-438">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4d22b-439">Data do pedido</span><span class="sxs-lookup"><span data-stu-id="4d22b-439">Order date</span></span></td>
<td><p><span data-ttu-id="4d22b-440">A data em que o pedido foi feito.</span><span class="sxs-lookup"><span data-stu-id="4d22b-440">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4d22b-441">ProductId</span><span class="sxs-lookup"><span data-stu-id="4d22b-441">ProductId</span></span></td>
<td><p><span data-ttu-id="4d22b-442">A ID do produto.</span><span class="sxs-lookup"><span data-stu-id="4d22b-442">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4d22b-443">SkuId</span><span class="sxs-lookup"><span data-stu-id="4d22b-443">SkuId</span></span></td>
<td><p><span data-ttu-id="4d22b-444">A ID de uma SKU em particular.</span><span class="sxs-lookup"><span data-stu-id="4d22b-444">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4d22b-445">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="4d22b-445">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="4d22b-446">A ID de uma Disponibilidade em particular.</span><span class="sxs-lookup"><span data-stu-id="4d22b-446">The ID for a particular Availability.</span></span> <span data-ttu-id="4d22b-447">"Disponibilidade" refere-se a se uma SKU em particular está disponível ou não para compra para determinado país, moeda, segmento do setor etc.</span><span class="sxs-lookup"><span data-stu-id="4d22b-447">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4d22b-448">Nome do SKU</span><span class="sxs-lookup"><span data-stu-id="4d22b-448">SKU Name</span></span></td>
<td><p><span data-ttu-id="4d22b-449">O título de uma SKU em particular.</span><span class="sxs-lookup"><span data-stu-id="4d22b-449">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4d22b-450">Nome do produto</span><span class="sxs-lookup"><span data-stu-id="4d22b-450">Product name</span></span></td>
<td><p><span data-ttu-id="4d22b-451">O nome do produto.</span><span class="sxs-lookup"><span data-stu-id="4d22b-451">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4d22b-452">PublisherName</span><span class="sxs-lookup"><span data-stu-id="4d22b-452">PublisherName</span></span></td>
<td><p><span data-ttu-id="4d22b-453">O nome do publicador do produto.</span><span class="sxs-lookup"><span data-stu-id="4d22b-453">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4d22b-454">PublisherID</span><span class="sxs-lookup"><span data-stu-id="4d22b-454">PublisherID</span></span></td>
<td><p><span data-ttu-id="4d22b-455">ID exclusiva para esse publicador.</span><span class="sxs-lookup"><span data-stu-id="4d22b-455">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4d22b-456">Descrição da assinatura</span><span class="sxs-lookup"><span data-stu-id="4d22b-456">Subscription Description</span></span></td>
<td><p><span data-ttu-id="4d22b-457">Nome amigável de uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="4d22b-457">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4d22b-458">ID da assinatura</span><span class="sxs-lookup"><span data-stu-id="4d22b-458">Subscription ID</span></span></td>
<td><p><span data-ttu-id="4d22b-459">Identificador exclusivo para uma assinatura da plataforma de comércio do Microsoft.</span><span class="sxs-lookup"><span data-stu-id="4d22b-459">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="4d22b-460">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="4d22b-460">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="4d22b-461">Esse não é o mesmo que o ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="4d22b-461">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4d22b-462">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="4d22b-462">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="4d22b-463">Dia de início dos encargos.</span><span class="sxs-lookup"><span data-stu-id="4d22b-463">Start day of the charges.</span></span> <span data-ttu-id="4d22b-464">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="4d22b-464">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4d22b-465">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="4d22b-465">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="4d22b-466">Dia do término dos encargos.</span><span class="sxs-lookup"><span data-stu-id="4d22b-466">End day of the charges.</span></span> <span data-ttu-id="4d22b-467">A hora é sempre o fim do dia, 23:59.</span><span class="sxs-lookup"><span data-stu-id="4d22b-467">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4d22b-468">Termo e Billingcycle</span><span class="sxs-lookup"><span data-stu-id="4d22b-468">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="4d22b-469">A vigência e o ciclo de cobrança para a compra.</span><span class="sxs-lookup"><span data-stu-id="4d22b-469">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="4d22b-470">Por exemplo, "1 ano, mês."</span><span class="sxs-lookup"><span data-stu-id="4d22b-470">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4d22b-471">Tipo de Cobrança</span><span class="sxs-lookup"><span data-stu-id="4d22b-471">Charge Type</span></span></td>
<td><p><span data-ttu-id="4d22b-472">O tipo de encargo ou ajuste.</span><span class="sxs-lookup"><span data-stu-id="4d22b-472">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4d22b-473">Preço unitário</span><span class="sxs-lookup"><span data-stu-id="4d22b-473">Unit Price</span></span></td>
<td><p><span data-ttu-id="4d22b-474">O preço como publicado no pricelist no momento da compra.</span><span class="sxs-lookup"><span data-stu-id="4d22b-474">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="4d22b-475">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="4d22b-475">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4d22b-476">Preço unitário efetiva</span><span class="sxs-lookup"><span data-stu-id="4d22b-476">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="4d22b-477">O preço unitário depois de fazer ajustes.</span><span class="sxs-lookup"><span data-stu-id="4d22b-477">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4d22b-478">Quantidade</span><span class="sxs-lookup"><span data-stu-id="4d22b-478">Quantity</span></span></td>
<td><p><span data-ttu-id="4d22b-479">Número de unidades.</span><span class="sxs-lookup"><span data-stu-id="4d22b-479">Number of units.</span></span> <span data-ttu-id="4d22b-480">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="4d22b-480">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4d22b-481">Tipo de unidade</span><span class="sxs-lookup"><span data-stu-id="4d22b-481">Unit type</span></span></td>
<td><p><span data-ttu-id="4d22b-482">O tipo de unidade que está sendo comprado.</span><span class="sxs-lookup"><span data-stu-id="4d22b-482">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4d22b-483">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="4d22b-483">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="4d22b-484">Obter uma explicação de qualquer desconto aplicável.</span><span class="sxs-lookup"><span data-stu-id="4d22b-484">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4d22b-485">Subtotal</span><span class="sxs-lookup"><span data-stu-id="4d22b-485">Sub Total</span></span></td>
<td><p><span data-ttu-id="4d22b-486">Total sem imposto.</span><span class="sxs-lookup"><span data-stu-id="4d22b-486">Total before tax.</span></span> <span data-ttu-id="4d22b-487">Verifica se seu subtotal corresponde ao total esperado, em caso de desconto.</span><span class="sxs-lookup"><span data-stu-id="4d22b-487">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4d22b-488">Total de impostos</span><span class="sxs-lookup"><span data-stu-id="4d22b-488">Tax Total</span></span></td>
<td><p><span data-ttu-id="4d22b-489">Valor do imposto cobrado, com base nas regras fiscais do mercado e em circunstâncias específicas.</span><span class="sxs-lookup"><span data-stu-id="4d22b-489">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4d22b-490">Total</span><span class="sxs-lookup"><span data-stu-id="4d22b-490">Total</span></span></td>
<td><p><span data-ttu-id="4d22b-491">Total com imposto.</span><span class="sxs-lookup"><span data-stu-id="4d22b-491">Total after tax.</span></span> <span data-ttu-id="4d22b-492">Verifica se o imposto é cobrado na fatura.</span><span class="sxs-lookup"><span data-stu-id="4d22b-492">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4d22b-493">Currency</span><span class="sxs-lookup"><span data-stu-id="4d22b-493">Currency</span></span></td>
<td><p><span data-ttu-id="4d22b-494">Tipo de moeda.</span><span class="sxs-lookup"><span data-stu-id="4d22b-494">Currency type.</span></span> <span data-ttu-id="4d22b-495">Cada entidade de cobrança tem somente uma moeda.</span><span class="sxs-lookup"><span data-stu-id="4d22b-495">Each billing entity has only one currency.</span></span> <span data-ttu-id="4d22b-496">Verifique se isso coincide com a primeira fatura e faça o mesmo após grandes atualizações na plataforma de cobrança.</span><span class="sxs-lookup"><span data-stu-id="4d22b-496">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4d22b-497">AlternateID</span><span class="sxs-lookup"><span data-stu-id="4d22b-497">AlternateID</span></span></td>
<td><p><span data-ttu-id="4d22b-498">Um identificador alternativo para uma ID de pedido.</span><span class="sxs-lookup"><span data-stu-id="4d22b-498">An alternate identifier to an order ID.</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="4d22b-499">Campos de arquivo de uso classificada como diária</span><span class="sxs-lookup"><span data-stu-id="4d22b-499">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="4d22b-500">Column</span><span class="sxs-lookup"><span data-stu-id="4d22b-500">Column</span></span></th>
<th><span data-ttu-id="4d22b-501">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d22b-501">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="4d22b-502">PartnerID</span><span class="sxs-lookup"><span data-stu-id="4d22b-502">PartnerId</span></span></td>
<td><p><span data-ttu-id="4d22b-503">ID do parceiro, no formato GUID.</span><span class="sxs-lookup"><span data-stu-id="4d22b-503">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4d22b-504">PartnerName</span><span class="sxs-lookup"><span data-stu-id="4d22b-504">PartnerName</span></span></td>
<td><p><span data-ttu-id="4d22b-505">Nome do parceiro.</span><span class="sxs-lookup"><span data-stu-id="4d22b-505">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4d22b-506">CustomerID</span><span class="sxs-lookup"><span data-stu-id="4d22b-506">CustomerId</span></span></td>
<td><p><span data-ttu-id="4d22b-507">ID exclusiva da Microsoft, no formato GUID, usada para identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="4d22b-507">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4d22b-508">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="4d22b-508">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="4d22b-509">Nome da organização do cliente como informado no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="4d22b-509">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="4d22b-510">Isso é muito importante para reconciliar a fatura com as informações de seu sistema.</span><span class="sxs-lookup"><span data-stu-id="4d22b-510">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4d22b-511">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="4d22b-511">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="4d22b-512">O nome de domínio do cliente.</span><span class="sxs-lookup"><span data-stu-id="4d22b-512">The customer’s domain name.</span></span> <span data-ttu-id="4d22b-513">Não disponível para a atividade atual.</span><span class="sxs-lookup"><span data-stu-id="4d22b-513">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4d22b-514">País do cliente</span><span class="sxs-lookup"><span data-stu-id="4d22b-514">Customer country</span></span></td>
<td><p><span data-ttu-id="4d22b-515">O país em que o cliente está localizado.</span><span class="sxs-lookup"><span data-stu-id="4d22b-515">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4d22b-516">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="4d22b-516">MPNID</span></span></td>
<td><p><span data-ttu-id="4d22b-517">ID do MPN do parceiro CSP.</span><span class="sxs-lookup"><span data-stu-id="4d22b-517">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4d22b-518">Revendedor MPNID</span><span class="sxs-lookup"><span data-stu-id="4d22b-518">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="4d22b-519">ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="4d22b-519">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="4d22b-520">Não disponível para a atividade atual.</span><span class="sxs-lookup"><span data-stu-id="4d22b-520">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4d22b-521">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="4d22b-521">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="4d22b-522">Número da fatura na qual a transação especificada é exibida.</span><span class="sxs-lookup"><span data-stu-id="4d22b-522">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="4d22b-523">Não disponível para a atividade atual.</span><span class="sxs-lookup"><span data-stu-id="4d22b-523">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4d22b-524">ProductId</span><span class="sxs-lookup"><span data-stu-id="4d22b-524">ProductId</span></span></td>
<td><p><span data-ttu-id="4d22b-525">A ID do produto.</span><span class="sxs-lookup"><span data-stu-id="4d22b-525">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4d22b-526">SkuId</span><span class="sxs-lookup"><span data-stu-id="4d22b-526">SkuId</span></span></td>
<td><p><span data-ttu-id="4d22b-527">A ID de uma SKU em particular.</span><span class="sxs-lookup"><span data-stu-id="4d22b-527">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4d22b-528">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="4d22b-528">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="4d22b-529">A ID de uma Disponibilidade em particular.</span><span class="sxs-lookup"><span data-stu-id="4d22b-529">The ID for a particular Availability.</span></span> <span data-ttu-id="4d22b-530">"Disponibilidade" refere-se a se uma SKU em particular está disponível ou não para compra para determinado país, moeda, segmento do setor etc.</span><span class="sxs-lookup"><span data-stu-id="4d22b-530">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4d22b-531">Nome do SKU</span><span class="sxs-lookup"><span data-stu-id="4d22b-531">SKU Name</span></span></td>
<td><p><span data-ttu-id="4d22b-532">O título de uma SKU em particular.</span><span class="sxs-lookup"><span data-stu-id="4d22b-532">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4d22b-533">PublisherName</span><span class="sxs-lookup"><span data-stu-id="4d22b-533">PublisherName</span></span></td>
<td><p><span data-ttu-id="4d22b-534">O nome do publicador.</span><span class="sxs-lookup"><span data-stu-id="4d22b-534">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4d22b-535">PublisherID</span><span class="sxs-lookup"><span data-stu-id="4d22b-535">PublisherID</span></span></td>
<td><p><span data-ttu-id="4d22b-536">A ID do publicador, no formato GUID.</span><span class="sxs-lookup"><span data-stu-id="4d22b-536">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="4d22b-537">Não disponível para a atividade atual.</span><span class="sxs-lookup"><span data-stu-id="4d22b-537">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="4d22b-538">Descrição da assinatura</span><span class="sxs-lookup"><span data-stu-id="4d22b-538">Subscription Description</span></span></td>
<td><p><span data-ttu-id="4d22b-539">O nome da oferta de serviço comprada pelo cliente, conforme definido na tabela de preços.</span><span class="sxs-lookup"><span data-stu-id="4d22b-539">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="4d22b-540">(Este é um campo idêntico ao nome da oferta).</span><span class="sxs-lookup"><span data-stu-id="4d22b-540">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4d22b-541">ID da assinatura</span><span class="sxs-lookup"><span data-stu-id="4d22b-541">Subscription ID</span></span></td>
<td><p><span data-ttu-id="4d22b-542">Identificador exclusivo de uma assinatura na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="4d22b-542">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="4d22b-543">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="4d22b-543">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="4d22b-544">Esse não é o mesmo que o ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="4d22b-544">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4d22b-545">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="4d22b-545">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="4d22b-546">Data de início do ciclo de cobrança exceto quando apresentadas as datas de dados de uso latentes anteriormente não cobradas (do ciclo de cobrança anterior).</span><span class="sxs-lookup"><span data-stu-id="4d22b-546">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="4d22b-547">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="4d22b-547">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4d22b-548">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="4d22b-548">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="4d22b-549">Data de término do ciclo de cobrança exceto quando apresentadas as datas de dados de uso latentes anteriormente não cobradas (do ciclo de cobrança anterior).</span><span class="sxs-lookup"><span data-stu-id="4d22b-549">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="4d22b-550">A hora é sempre o fim do dia, 23:59.</span><span class="sxs-lookup"><span data-stu-id="4d22b-550">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4d22b-551">Data de uso</span><span class="sxs-lookup"><span data-stu-id="4d22b-551">Usage Date</span></span></td>
<td><p><span data-ttu-id="4d22b-552">Data de uso do serviço.</span><span class="sxs-lookup"><span data-stu-id="4d22b-552">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4d22b-553">Tipo de medidor</span><span class="sxs-lookup"><span data-stu-id="4d22b-553">Meter Type</span></span></td>
<td><p><span data-ttu-id="4d22b-554">O tipo de medidor.</span><span class="sxs-lookup"><span data-stu-id="4d22b-554">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4d22b-555">Categoria do medidor</span><span class="sxs-lookup"><span data-stu-id="4d22b-555">Meter Category</span></span></td>
<td><p><span data-ttu-id="4d22b-556">O serviço de nível superior para o uso.</span><span class="sxs-lookup"><span data-stu-id="4d22b-556">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4d22b-557">Id do medidor</span><span class="sxs-lookup"><span data-stu-id="4d22b-557">Meter Id</span></span></td>
<td><p><span data-ttu-id="4d22b-558">A ID do medidor que está sendo usado.</span><span class="sxs-lookup"><span data-stu-id="4d22b-558">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4d22b-559">Medir subcategoria</span><span class="sxs-lookup"><span data-stu-id="4d22b-559">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="4d22b-560">O tipo de serviço do Azure que pode afetar a tarifa.</span><span class="sxs-lookup"><span data-stu-id="4d22b-560">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4d22b-561">Nome do medidor</span><span class="sxs-lookup"><span data-stu-id="4d22b-561">Meter Name</span></span></td>
<td><p><span data-ttu-id="4d22b-562">A unidade de medida para o medidor sendo consumido.</span><span class="sxs-lookup"><span data-stu-id="4d22b-562">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4d22b-563">Região do medidor</span><span class="sxs-lookup"><span data-stu-id="4d22b-563">Meter Region</span></span></td>
<td><p><span data-ttu-id="4d22b-564">Essa coluna identifica a localização de um data center dentro da região para serviços onde isso é aplicável e preenchido.</span><span class="sxs-lookup"><span data-stu-id="4d22b-564">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4d22b-565">Unidade</span><span class="sxs-lookup"><span data-stu-id="4d22b-565">Unit</span></span></td>
<td><p><span data-ttu-id="4d22b-566">A unidade do nome do recurso.</span><span class="sxs-lookup"><span data-stu-id="4d22b-566">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4d22b-567">Quantidade consumida</span><span class="sxs-lookup"><span data-stu-id="4d22b-567">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="4d22b-568">A quantidade de serviço consumida (horas, GB etc.) durante o período de relatório.</span><span class="sxs-lookup"><span data-stu-id="4d22b-568">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="4d22b-569">Também inclui qualquer uso não cobrado de períodos de relatório anteriores.</span><span class="sxs-lookup"><span data-stu-id="4d22b-569">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4d22b-570">Local do recurso</span><span class="sxs-lookup"><span data-stu-id="4d22b-570">Resource Location</span></span></td>
<td><p><span data-ttu-id="4d22b-571">O datacenter em que o medidor está sendo executado.</span><span class="sxs-lookup"><span data-stu-id="4d22b-571">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4d22b-572">Serviço consumido</span><span class="sxs-lookup"><span data-stu-id="4d22b-572">Consumed Service</span></span></td>
<td><p><span data-ttu-id="4d22b-573">O serviço de plataforma do Azure que você usou.</span><span class="sxs-lookup"><span data-stu-id="4d22b-573">The Azure platform service that you used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4d22b-574">Grupo de Recursos</span><span class="sxs-lookup"><span data-stu-id="4d22b-574">Resource Group</span></span></td>
<td><p><span data-ttu-id="4d22b-575">O grupo de recursos no qual o medidor implantado está sendo executado.</span><span class="sxs-lookup"><span data-stu-id="4d22b-575">The resource group in which the deployed meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4d22b-576">URI de recurso</span><span class="sxs-lookup"><span data-stu-id="4d22b-576">Resource URI</span></span></td>
<td><p><span data-ttu-id="4d22b-577">O URI do recurso que está sendo usado.</span><span class="sxs-lookup"><span data-stu-id="4d22b-577">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4d22b-578">Tipo de cobrança</span><span class="sxs-lookup"><span data-stu-id="4d22b-578">Charge type</span></span></td>
<td><p><span data-ttu-id="4d22b-579">O tipo de encargo ou ajuste.</span><span class="sxs-lookup"><span data-stu-id="4d22b-579">The type of charge or adjustment.</span></span> <span data-ttu-id="4d22b-580">Não disponível para a atividade atual.</span><span class="sxs-lookup"><span data-stu-id="4d22b-580">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4d22b-581">Preço unitário</span><span class="sxs-lookup"><span data-stu-id="4d22b-581">Unit price</span></span></td>
<td><p><span data-ttu-id="4d22b-582">Preço por licença, como publicado no pricelist no momento da compra.</span><span class="sxs-lookup"><span data-stu-id="4d22b-582">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="4d22b-583">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="4d22b-583">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4d22b-584">Quantidade</span><span class="sxs-lookup"><span data-stu-id="4d22b-584">Quantity</span></span></td>
<td><p><span data-ttu-id="4d22b-585">Número de licenças.</span><span class="sxs-lookup"><span data-stu-id="4d22b-585">Number of licenses.</span></span> <span data-ttu-id="4d22b-586">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="4d22b-586">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4d22b-587">Tipo de unidade</span><span class="sxs-lookup"><span data-stu-id="4d22b-587">Unit type</span></span></td>
<td><p><span data-ttu-id="4d22b-588">O tipo de unidade, que o medidor é cobrado.</span><span class="sxs-lookup"><span data-stu-id="4d22b-588">The type of unit the meter is charged in.</span></span> <span data-ttu-id="4d22b-589">Não disponível para a atividade atual.</span><span class="sxs-lookup"><span data-stu-id="4d22b-589">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4d22b-590">Imposto de versão anterior de cobrança</span><span class="sxs-lookup"><span data-stu-id="4d22b-590">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="4d22b-591">Quantidade total antes dos impostos.</span><span class="sxs-lookup"><span data-stu-id="4d22b-591">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4d22b-592">Moeda de cobrança</span><span class="sxs-lookup"><span data-stu-id="4d22b-592">Billing currency</span></span></td>
<td><p><span data-ttu-id="4d22b-593">A moeda na região de geográfica do cliente</span><span class="sxs-lookup"><span data-stu-id="4d22b-593">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4d22b-594">Preço total pretax</span><span class="sxs-lookup"><span data-stu-id="4d22b-594">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="4d22b-595">O preço antes de impostos forem adicionados.</span><span class="sxs-lookup"><span data-stu-id="4d22b-595">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4d22b-596">Preços de moeda</span><span class="sxs-lookup"><span data-stu-id="4d22b-596">Pricing currency</span></span></td>
<td><p><span data-ttu-id="4d22b-597">A moeda no pricelist.</span><span class="sxs-lookup"><span data-stu-id="4d22b-597">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4d22b-598">Informações do serviço 1</span><span class="sxs-lookup"><span data-stu-id="4d22b-598">Service Info 1</span></span></td>
<td><p><span data-ttu-id="4d22b-599">O número de conexões ServiceBus que foram provisionados e utilizados em um dia específico.</span><span class="sxs-lookup"><span data-stu-id="4d22b-599">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4d22b-600">Informações do serviço 2</span><span class="sxs-lookup"><span data-stu-id="4d22b-600">Service Info 2</span></span></td>
<td><p><span data-ttu-id="4d22b-601">Um campo herdado que captura os metadados específicos do serviço opcional.</span><span class="sxs-lookup"><span data-stu-id="4d22b-601">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="4d22b-602">tags</span><span class="sxs-lookup"><span data-stu-id="4d22b-602">Tags</span></span></td>
<td><p><span data-ttu-id="4d22b-603">Marcas que você atribui ao medidor na ordem para agrupar registros de cobrança.</span><span class="sxs-lookup"><span data-stu-id="4d22b-603">Tags you assign to the meter in order to group billing records.</span></span> <span data-ttu-id="4d22b-604">Por exemplo, você pode usar marcas para distribuir os custos entre os departamentos que usam o medidor.</span><span class="sxs-lookup"><span data-stu-id="4d22b-604">For example, you can use tags to distribute costs by the department that uses the meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="4d22b-605">Informações adicionais</span><span class="sxs-lookup"><span data-stu-id="4d22b-605">Additional Info</span></span></td>
<td><p><span data-ttu-id="4d22b-606">Informações adicionais não são abordadas em outras colunas.</span><span class="sxs-lookup"><span data-stu-id="4d22b-606">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="4d22b-607">Encargos de mapeamento entre uma nota fiscal e o arquivo de reconciliação</span><span class="sxs-lookup"><span data-stu-id="4d22b-607">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="4d22b-608">Sua fatura fornece um resumo dos encargos, enquanto seu arquivo de reconciliação fornece uma divisão detalhada das transações de item de linha, incluindo os tipos de carga.</span><span class="sxs-lookup"><span data-stu-id="4d22b-608">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="4d22b-609">Para fazer referência cruzada das quantidades de carga entre o arquivo de reconciliação e fatura, você pode usar opções de filtro do Microsoft Excel para filtrar por tipos de cobrança no arquivo de reconciliação para mapear os encargos de fatura em um conjunto de detalhamentos de cobrança no arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="4d22b-609">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="4d22b-610">Os arquivos de reconciliação, tanto os baseados em licença quanto os baseados em uso, mostram apenas encargos e transações relacionadas ao uso (unidades consumidas e encargos relacionados).</span><span class="sxs-lookup"><span data-stu-id="4d22b-610">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="4d22b-611">Créditos únicos, descontos ou reembolsos que aparecem na fatura como "Ajustes" não são mostrados no arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="4d22b-611">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="4d22b-612">A tabela a seguir mostra os mapeamentos entre uma seção da fatura e os tipos de encargo associados que podem aparecer nos arquivos de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="4d22b-612">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="4d22b-613"><strong>Descrição de encargo de fatura</strong></span><span class="sxs-lookup"><span data-stu-id="4d22b-613"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="4d22b-614"><strong>Descrição de cobrança de arquivo de reconciliação (ChargeType coluna)</strong></span><span class="sxs-lookup"><span data-stu-id="4d22b-614"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="4d22b-615"><strong>O que é a cobrança?</strong></span><span class="sxs-lookup"><span data-stu-id="4d22b-615"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="4d22b-616"><strong>Como faço para mapear esses ChargeTypes à fatura?</strong></span><span class="sxs-lookup"><span data-stu-id="4d22b-616"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="4d22b-617"><strong>Encargos de licença</strong></span><span class="sxs-lookup"><span data-stu-id="4d22b-617"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="4d22b-618">Taxa de ativação</span><span class="sxs-lookup"><span data-stu-id="4d22b-618">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="4d22b-619">O valor cobrado do cliente quando ele usa a assinatura depois de comprá-la.</span><span class="sxs-lookup"><span data-stu-id="4d22b-619">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="4d22b-620">No arquivo baseado em licença, some a coluna <strong>Quantidade</strong></span><span class="sxs-lookup"><span data-stu-id="4d22b-620">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="4d22b-621">Taxa de cancelamento</span><span class="sxs-lookup"><span data-stu-id="4d22b-621">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="4d22b-622">Os encargos proporcionais reembolsados para o cliente quando os assentos associados são alterados</span><span class="sxs-lookup"><span data-stu-id="4d22b-622">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="4d22b-623">Taxa do ciclo</span><span class="sxs-lookup"><span data-stu-id="4d22b-623">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="4d22b-624">Encargos periódicos de uma assinatura</span><span class="sxs-lookup"><span data-stu-id="4d22b-624">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="4d22b-625">Proporcional à instância do ciclo</span><span class="sxs-lookup"><span data-stu-id="4d22b-625">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="4d22b-626">Os encargos proporcionais cobrados do cliente quando os assentos associados são alterados</span><span class="sxs-lookup"><span data-stu-id="4d22b-626">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="4d22b-627">Taxas proporcionais durante o cancelamento</span><span class="sxs-lookup"><span data-stu-id="4d22b-627">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="4d22b-628">Reembolso proporcional para a parte não utilizada do serviço após o cancelamento</span><span class="sxs-lookup"><span data-stu-id="4d22b-628">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="4d22b-629">Taxas proporcionais durante a compra</span><span class="sxs-lookup"><span data-stu-id="4d22b-629">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="4d22b-630">O tipo de encargo para uma assinatura ao usar cobranças anuais</span><span class="sxs-lookup"><span data-stu-id="4d22b-630">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="4d22b-631">Valor de compra</span><span class="sxs-lookup"><span data-stu-id="4d22b-631">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="4d22b-632">O tipo de encargo para uma assinatura ao usar a cobrança mensal</span><span class="sxs-lookup"><span data-stu-id="4d22b-632">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="4d22b-633">Taxa proporcional ao renovar</span><span class="sxs-lookup"><span data-stu-id="4d22b-633">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="4d22b-634">Taxas proporcionais após a renovação da assinatura</span><span class="sxs-lookup"><span data-stu-id="4d22b-634">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="4d22b-635">Taxa de renovação</span><span class="sxs-lookup"><span data-stu-id="4d22b-635">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="4d22b-636">Cobrança para renovação de uma assinatura</span><span class="sxs-lookup"><span data-stu-id="4d22b-636">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="4d22b-637">Taxas proporcionais ao ativar</span><span class="sxs-lookup"><span data-stu-id="4d22b-637">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="4d22b-638">Taxas proporcionais da ativação até o final do período de cobrança</span><span class="sxs-lookup"><span data-stu-id="4d22b-638">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>



<tr>
<td rowspan="5">
<p><span data-ttu-id="4d22b-639"><strong>Encargos de uso únicos</strong></span><span class="sxs-lookup"><span data-stu-id="4d22b-639"><strong>One-time Charges</strong></span></span></p>

</td>
<td>
<p><span data-ttu-id="4d22b-640">Novo</span><span class="sxs-lookup"><span data-stu-id="4d22b-640">New</span></span></p>
</td>
<td>
<p><span data-ttu-id="4d22b-641">Usado quando uma nova compra é criada</span><span class="sxs-lookup"><span data-stu-id="4d22b-641">Used when a new purchase is created</span></span></p>
</td>

<p></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="4d22b-642">addQuantity</span><span class="sxs-lookup"><span data-stu-id="4d22b-642">addQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="4d22b-643">Usado em ambos os o reembolso na compra original e a nova quantidade depois aumento</span><span class="sxs-lookup"><span data-stu-id="4d22b-643">Used in both the refund of the original purchase and the new quantity after increase</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="4d22b-644">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="4d22b-644">removeQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="4d22b-645">Usado em ambos os o reembolso na compra original e a nova quantidade após a redução</span><span class="sxs-lookup"><span data-stu-id="4d22b-645">Used in both the refund of the original purchase and the new quantity after decrease</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="4d22b-646">Cancel</span><span class="sxs-lookup"><span data-stu-id="4d22b-646">Cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="4d22b-647">Usado quando uma assinatura é cancelada</span><span class="sxs-lookup"><span data-stu-id="4d22b-647">Used when a subscription is cancelled</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="4d22b-648">Converter</span><span class="sxs-lookup"><span data-stu-id="4d22b-648">Convert</span></span></p>
</td>
<td>
<p><span data-ttu-id="4d22b-649">Usado quando uma licença é atualizada, mas o número de estações permanece inalterado</span><span class="sxs-lookup"><span data-stu-id="4d22b-649">Used when a license is upgraded but the number of seats remains unchanged</span></span></p>
</td>
</tr>

<tr>
<td rowspan="2">
<p><span data-ttu-id="4d22b-650"><strong>Encargos de uso</strong></span><span class="sxs-lookup"><span data-stu-id="4d22b-650"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="4d22b-651">Avaliar a taxa de uso ao cancelar</span><span class="sxs-lookup"><span data-stu-id="4d22b-651">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="4d22b-652">Taxa de uso de acesso com o cancelamento para uso não pago durante o período de cobrança atual</span><span class="sxs-lookup"><span data-stu-id="4d22b-652">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="4d22b-653">No arquivo baseado em uso, some a coluna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="4d22b-653">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="4d22b-654">Avalie a taxa de uso para o ciclo atual</span><span class="sxs-lookup"><span data-stu-id="4d22b-654">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="4d22b-655">Taxa de uso de acesso para o período atual de cobrança</span><span class="sxs-lookup"><span data-stu-id="4d22b-655">Access usage fee for the current billing period</span></span></p>
</td>
</tr>

<tr>
<td>
<p><span data-ttu-id="4d22b-656"><strong>Créditos</strong></span><span class="sxs-lookup"><span data-stu-id="4d22b-656"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="4d22b-657">Deslocando um item de linha</span><span class="sxs-lookup"><span data-stu-id="4d22b-657">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="4d22b-658">Reembolso parcial ou integral para um item de linha, incluindo os impostos</span><span class="sxs-lookup"><span data-stu-id="4d22b-658">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="4d22b-659">No arquivo baseado em licença, some a coluna <strong>TotalForCustomer</strong></span><span class="sxs-lookup"><span data-stu-id="4d22b-659">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="4d22b-660">No arquivo baseado em uso, some a coluna <strong>PostTaxTotal</strong></span><span class="sxs-lookup"><span data-stu-id="4d22b-660">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="4d22b-661"><strong>Descontos com base no uso</strong></span><span class="sxs-lookup"><span data-stu-id="4d22b-661"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="4d22b-662">Desconto de ativação</span><span class="sxs-lookup"><span data-stu-id="4d22b-662">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="4d22b-663">Desconto aplicado quando a assinatura é ativada</span><span class="sxs-lookup"><span data-stu-id="4d22b-663">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="4d22b-664">No arquivo baseado em uso, some a coluna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="4d22b-664">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="4d22b-665">Desconto de ciclo</span><span class="sxs-lookup"><span data-stu-id="4d22b-665">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="4d22b-666">Desconto aplicado em cobranças periódicas</span><span class="sxs-lookup"><span data-stu-id="4d22b-666">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="4d22b-667">Desconto de renovação</span><span class="sxs-lookup"><span data-stu-id="4d22b-667">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="4d22b-668">Desconto aplicado quando a assinatura é renovada</span><span class="sxs-lookup"><span data-stu-id="4d22b-668">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="4d22b-669">Desconto de cancelamento</span><span class="sxs-lookup"><span data-stu-id="4d22b-669">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="4d22b-670">Encargos aplicados quando descontos são cancelados</span><span class="sxs-lookup"><span data-stu-id="4d22b-670">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="4d22b-671"><strong>Descontos de licença</strong></span><span class="sxs-lookup"><span data-stu-id="4d22b-671"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="4d22b-672"><em>Pode ser aplicado a vários tipos de custo</em></span><span class="sxs-lookup"><span data-stu-id="4d22b-672"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="4d22b-673">No arquivo baseado em licença, some a coluna <strong>TotalOtherDiscount</strong></span><span class="sxs-lookup"><span data-stu-id="4d22b-673">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="4d22b-674"><strong>Impostos</strong>&nbsp;ou&nbsp;<strong>IVA</strong></span><span class="sxs-lookup"><span data-stu-id="4d22b-674"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="4d22b-675"><em>Pode ser aplicado a vários tipos de custo</em></span><span class="sxs-lookup"><span data-stu-id="4d22b-675"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="4d22b-676"><em>Exceção: &quot;Deslocamento de um item de linha&quot; já inclui os impostos. Ver créditos, acima.</em></span><span class="sxs-lookup"><span data-stu-id="4d22b-676"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="4d22b-677">Impostos ou impostos sobre valor agregado (IVA)</span><span class="sxs-lookup"><span data-stu-id="4d22b-677">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="4d22b-678">No arquivo baseado em licença, some a coluna <strong>Imposto</strong></span><span class="sxs-lookup"><span data-stu-id="4d22b-678">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="4d22b-679">No arquivo baseado em uso, some a coluna <strong>TaxAmount</strong></span><span class="sxs-lookup"><span data-stu-id="4d22b-679">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
