---
title: Usar os arquivos de reconciliação | Partner Center
ms.topic: article
ms.date: 07/08/2019
description: Para obter uma exibição detalhada de item de linha de cada encargo em um ciclo de cobrança, baixe os arquivos de reconciliação do Partner Center.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: fda8724b389913e49e01d64941622cf366516bf6
ms.sourcegitcommit: 9156f3a7711fae5e0f9a2c5f29e74e8791836c8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/11/2019
ms.locfileid: "67818974"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="b1204-103">Usar os arquivos de reconciliação</span><span class="sxs-lookup"><span data-stu-id="b1204-103">Use the reconciliation files</span></span>

<span data-ttu-id="b1204-104">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="b1204-104">**Applies to**</span></span>

-  <span data-ttu-id="b1204-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="b1204-105">Partner Center</span></span>
-  <span data-ttu-id="b1204-106">Partner Center para Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="b1204-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="b1204-107">Para obter uma exibição detalhada de item de linha de cada encargo em um ciclo de cobrança, baixe os arquivos de reconciliação do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="b1204-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="b1204-108">Os detalhes incluem encargos por assinaturas de cada cliente e eventos detalhados (como a adição de assentos a uma assinatura no meio do período).</span><span class="sxs-lookup"><span data-stu-id="b1204-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="b1204-109">Problemas de formatação</span><span class="sxs-lookup"><span data-stu-id="b1204-109">Formatting issues</span></span>

<span data-ttu-id="b1204-110">Ocasionalmente, seu arquivo reconhecimento pode ter problemas de formatação.</span><span class="sxs-lookup"><span data-stu-id="b1204-110">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="b1204-111">(Isso pode acontecer, por exemplo, se a localidade EN-US não for usada.) Siga as etapas abaixo para corrigir esses problemas.</span><span class="sxs-lookup"><span data-stu-id="b1204-111">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="b1204-112">Abra o arquivo. csv no Excel e selecione a primeira coluna.</span><span class="sxs-lookup"><span data-stu-id="b1204-112">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="b1204-113">Na faixa de opções, selecione <strong>dados</strong>e, em seguida, selecione <strong>texto para colunas</strong>.</span><span class="sxs-lookup"><span data-stu-id="b1204-113">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="b1204-114">No assistente converter texto em colunas, selecione <strong>tipo de arquivo delimitado</strong>e, em seguida, selecione <strong>Avançar</strong>.</span><span class="sxs-lookup"><span data-stu-id="b1204-114">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="b1204-115">No campo delimitadores, selecione <strong>vírgula</strong>.</span><span class="sxs-lookup"><span data-stu-id="b1204-115">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="b1204-116">Se a <strong>guia</strong> já estiver selecionada, você poderá deixá-la.</span><span class="sxs-lookup"><span data-stu-id="b1204-116">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="b1204-117">Selecione <strong>Avançar</strong>.</span><span class="sxs-lookup"><span data-stu-id="b1204-117">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="b1204-118">No campo formato de dados da coluna, <strong>selecione Data: MDY</strong>e, em seguida, selecione <strong>Avançar</strong>.</span><span class="sxs-lookup"><span data-stu-id="b1204-118">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="b1204-119">No campo formato de dados da coluna, selecione <strong>texto</strong> para todas as colunas de valor e, em seguida, selecione <strong>concluir</strong>.</span><span class="sxs-lookup"><span data-stu-id="b1204-119">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a name="downloading-a-large-recon-file"></a><span data-ttu-id="b1204-120">Baixando um arquivo reconhecimento grande</span><span class="sxs-lookup"><span data-stu-id="b1204-120">Downloading a large recon file</span></span>

<span data-ttu-id="b1204-121">Os arquivos reconhecimento podem crescer muito e, às vezes, são difíceis de baixar.</span><span class="sxs-lookup"><span data-stu-id="b1204-121">Recon files can grow very large and are sometimes difficult to download.</span></span> <span data-ttu-id="b1204-122">Para obter um script do PowerShell para ajudar a baixar arquivos grandes do reconhecimento, consulte [obter itens de linha da fatura](https://docs.microsoft.com/en-us/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="b1204-122">For a PowerShell script to help download large recon files, see [Get invoice line items](https://docs.microsoft.com/en-us/partner-center/develop/get-invoiceline-items).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="b1204-123">Discriminar por parceiro</span><span class="sxs-lookup"><span data-stu-id="b1204-123">Itemize by partner</span></span>


<span data-ttu-id="b1204-124">Os parceiros no modelo indireto podem usar esses campos adicionais nos arquivos de reconciliação baseados em uso e em licença para discriminar por revendedor.</span><span class="sxs-lookup"><span data-stu-id="b1204-124">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="b1204-125">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="b1204-125">MPN ID</span></span></th>
<th><span data-ttu-id="b1204-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1204-126">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="b1204-127">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="b1204-127">MPN ID</span></span></td>
<td><p><span data-ttu-id="b1204-128">A ID do Microsoft Partner Network (MPN) do parceiro CSP (direta ou indireta).</span><span class="sxs-lookup"><span data-stu-id="b1204-128">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b1204-129">ID do MPN do revendedor</span><span class="sxs-lookup"><span data-stu-id="b1204-129">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="b1204-130">Só aparece em arquivos de reconciliação para parceiros no modelo indireto.</span><span class="sxs-lookup"><span data-stu-id="b1204-130">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="b1204-131">A ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="b1204-131">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="b1204-132">Isso corresponde à ID de revendedor listada para a assinatura específica no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="b1204-132">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="b1204-133">eTo exibir ou atualizar o revendedor, no menu do centro de parceiros, selecione <strong>clientes</strong>e, em seguida, escolha o cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="b1204-133">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="b1204-134">No menu do cliente, selecione <strong>Assinaturas</strong>, escolha a assinatura na lista.</span><span class="sxs-lookup"><span data-stu-id="b1204-134">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="b1204-135">Selecione <strong>Atualizar</strong> para alterar o <strong>Revendedor (ID do MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="b1204-135">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="b1204-136">Se um parceiro CSP vendeu a assinatura diretamente para o cliente, sua ID do MPN estará listada duas vezes, como a ID do MPN e a ID do MPN do revendedor.</span><span class="sxs-lookup"><span data-stu-id="b1204-136">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="b1204-137">Se um parceiro CSP tiver um revendedor sem ID do MPN, esse valor será definido como a ID do MPN do parceiro.</span><span class="sxs-lookup"><span data-stu-id="b1204-137">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="b1204-138">Se o parceiro CSP remover uma ID de revendedor, esse valor será definido como -1.</span><span class="sxs-lookup"><span data-stu-id="b1204-138">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a><span data-ttu-id="b1204-139">Campos de arquivo com base em licença</span><span class="sxs-lookup"><span data-stu-id="b1204-139">License-based file fields</span></span>


<span data-ttu-id="b1204-140">Para reconciliar seus encargos com os pedidos de seu cliente, compare o campo Syndication\_Partner\_Subscription\_Number do arquivo de reconciliação com a ID de Assinatura do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="b1204-140">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="b1204-141"><strong>Coluna</strong></span><span class="sxs-lookup"><span data-stu-id="b1204-141"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="b1204-142"><strong>Descrição</strong></span><span class="sxs-lookup"><span data-stu-id="b1204-142"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="b1204-143"><strong>Valor de exemplo</strong></span><span class="sxs-lookup"><span data-stu-id="b1204-143"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b1204-144">PartnerID</span><span class="sxs-lookup"><span data-stu-id="b1204-144">PartnerId</span></span></td>
<td><p><span data-ttu-id="b1204-145">Identificador exclusivo de uma entidade de cobrança específica, em formato GUID.</span><span class="sxs-lookup"><span data-stu-id="b1204-145">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="b1204-146">Não é necessário para reconciliação, mas pode ser uma informação útil.</span><span class="sxs-lookup"><span data-stu-id="b1204-146">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="b1204-147">O mesmo em todas as linhas.</span><span class="sxs-lookup"><span data-stu-id="b1204-147">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="b1204-148">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="b1204-148">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b1204-149">CustomerID</span><span class="sxs-lookup"><span data-stu-id="b1204-149">CustomerID</span></span></td>
<td><p><span data-ttu-id="b1204-150">ID exclusiva da Microsoft, no formato GUID, usada para identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="b1204-150">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="b1204-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="b1204-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b1204-152">OrderID</span><span class="sxs-lookup"><span data-stu-id="b1204-152">OrderID</span></span></td>
<td><p><span data-ttu-id="b1204-153">Identificador exclusivo para um pedido na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b1204-153">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="b1204-154">Pode ser útil para identificar o pedido ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="b1204-154">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="b1204-155">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="b1204-155">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b1204-156">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="b1204-156">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="b1204-157">Identificador exclusivo de uma assinatura na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b1204-157">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="b1204-158">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="b1204-158">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="b1204-159">Esse não é o mesmo que o ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="b1204-159">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="b1204-160">Consulte Número_Assinatura_Parceiro_Sindicalização.</span><span class="sxs-lookup"><span data-stu-id="b1204-160">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="b1204-161">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="b1204-161">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b1204-162">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="b1204-162">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="b1204-163">Identificador exclusivo para assinaturas.</span><span class="sxs-lookup"><span data-stu-id="b1204-163">Unique identifier for subscriptions.</span></span> <span data-ttu-id="b1204-164">Target: Um cliente pode ter várias assinaturas para o mesmo plano, portanto, isso é importante para análise de arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="b1204-164">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="b1204-165">Esse campo é mapeado para a ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="b1204-165">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="b1204-166">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="b1204-166">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b1204-167">OfferID</span><span class="sxs-lookup"><span data-stu-id="b1204-167">OfferID</span></span></td>
<td><p><span data-ttu-id="b1204-168">ID exclusivo da oferta.</span><span class="sxs-lookup"><span data-stu-id="b1204-168">Unique offer ID.</span></span> <span data-ttu-id="b1204-169">ID padrão da oferta de acordo com a lista de preços.</span><span class="sxs-lookup"><span data-stu-id="b1204-169">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="b1204-170"><b>Observação</b>: Esse valor não corresponde à ID da oferta da lista de preços.</span><span class="sxs-lookup"><span data-stu-id="b1204-170"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="b1204-171">Veja DurableOfferID abaixo.</span><span class="sxs-lookup"><span data-stu-id="b1204-171">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="b1204-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="b1204-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b1204-173">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="b1204-173">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="b1204-174">ID exclusivo da oferta durável, conforme definido na tabela de preços.</span><span class="sxs-lookup"><span data-stu-id="b1204-174">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="b1204-175"><b>Observação</b>: Esse valor corresponde à ID da oferta da lista de preços.</span><span class="sxs-lookup"><span data-stu-id="b1204-175"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="b1204-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="b1204-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b1204-177">OfferName</span><span class="sxs-lookup"><span data-stu-id="b1204-177">OfferName</span></span></td>
<td><p><span data-ttu-id="b1204-178">O nome da oferta de serviço comprada pelo cliente, conforme definido na tabela de preços.</span><span class="sxs-lookup"><span data-stu-id="b1204-178">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="b1204-179">Microsoft Office 365 (plano E3)</span><span class="sxs-lookup"><span data-stu-id="b1204-179">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b1204-180">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="b1204-180">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="b1204-181">A data de início da assinatura, definida como um dia após o pedido ser enviado.</span><span class="sxs-lookup"><span data-stu-id="b1204-181">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="b1204-182">Verificando a data de início da assinatura em conjunto com a data de término, você pode determinar se o cliente está dentro do primeiro ano da assinatura ou se a assinatura foi renovada para o ano seguinte.</span><span class="sxs-lookup"><span data-stu-id="b1204-182">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="b1204-183">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="b1204-183">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="b1204-184">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="b1204-184">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b1204-185">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="b1204-185">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="b1204-186">A data de término da assinatura: 12 meses + x dias após a data de início (para alinhar com a data de cobrança do parceiro) ou 12 meses a partir da data de renovação.</span><span class="sxs-lookup"><span data-stu-id="b1204-186">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="b1204-187">Na renovação, os preços são atualizados com a tabela de preços atual.</span><span class="sxs-lookup"><span data-stu-id="b1204-187">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="b1204-188">Um comunicado ao cliente pode ser necessário antes da renovação automática.</span><span class="sxs-lookup"><span data-stu-id="b1204-188">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="b1204-189">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="b1204-189">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="b1204-190">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="b1204-190">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b1204-191">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="b1204-191">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="b1204-192">Dia de início dos encargos.</span><span class="sxs-lookup"><span data-stu-id="b1204-192">Start day of the charges.</span></span></p>
<p><span data-ttu-id="b1204-193">Quando o cliente muda o número de assentos, esse número é usado para calcular os encargos por dia (pro-rata).</span><span class="sxs-lookup"><span data-stu-id="b1204-193">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="b1204-194">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="b1204-194">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="b1204-195">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="b1204-195">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b1204-196">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="b1204-196">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="b1204-197">Dia do término dos encargos.</span><span class="sxs-lookup"><span data-stu-id="b1204-197">End day of the charges.</span></span></p>
<p><span data-ttu-id="b1204-198">Quando o cliente muda o número de assentos, esse número é usado para calcular os encargos por dia (pro-rata).</span><span class="sxs-lookup"><span data-stu-id="b1204-198">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="b1204-199">A hora é sempre o fim do dia, 23:59.</span><span class="sxs-lookup"><span data-stu-id="b1204-199">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="b1204-200">28/2/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="b1204-200">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b1204-201">ChargeType</span><span class="sxs-lookup"><span data-stu-id="b1204-201">ChargeType</span></span></td>
<td><p><span data-ttu-id="b1204-202">O tipo de encargo ou ajuste.</span><span class="sxs-lookup"><span data-stu-id="b1204-202">The type of charge or adjustment.</span></span> <span data-ttu-id="b1204-203">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="b1204-203">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="b1204-204">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="b1204-204">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b1204-205">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="b1204-205">UnitPrice</span></span></td>
<td><p><span data-ttu-id="b1204-206">Preço por estação, conforme publicado na lista de preços no momento da compra.</span><span class="sxs-lookup"><span data-stu-id="b1204-206">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="b1204-207">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="b1204-207">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="b1204-208">6.82</span><span class="sxs-lookup"><span data-stu-id="b1204-208">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b1204-209">Quantidade</span><span class="sxs-lookup"><span data-stu-id="b1204-209">Quantity</span></span></td>
<td><p><span data-ttu-id="b1204-210">Número de assentos.</span><span class="sxs-lookup"><span data-stu-id="b1204-210">Number of seats.</span></span> <span data-ttu-id="b1204-211">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="b1204-211">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="b1204-212">2</span><span class="sxs-lookup"><span data-stu-id="b1204-212">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b1204-213">Valor</span><span class="sxs-lookup"><span data-stu-id="b1204-213">Amount</span></span></td>
<td><p><span data-ttu-id="b1204-214">Preço total por quantidade.</span><span class="sxs-lookup"><span data-stu-id="b1204-214">Total of price for quantity.</span></span> <span data-ttu-id="b1204-215">Útil para verificar se o cálculo do valor coincide com a forma como você calcula isso para seus clientes.</span><span class="sxs-lookup"><span data-stu-id="b1204-215">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="b1204-216">13.32</span><span class="sxs-lookup"><span data-stu-id="b1204-216">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b1204-217">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="b1204-217">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="b1204-218">Valor de desconto aplicado a esses encargos.</span><span class="sxs-lookup"><span data-stu-id="b1204-218">Amount of discount applied to these charges.</span></span> <span data-ttu-id="b1204-219">As licenças de produto incluídas com uma competência ou mapas ou novas assinaturas qualificadas para um incentivo também conterão um valor de desconto nesta coluna.</span><span class="sxs-lookup"><span data-stu-id="b1204-219">Product Licenses included with a competency or MAPS or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="b1204-220">2.32</span><span class="sxs-lookup"><span data-stu-id="b1204-220">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b1204-221">Subtotal</span><span class="sxs-lookup"><span data-stu-id="b1204-221">Subtotal</span></span></td>
<td><p><span data-ttu-id="b1204-222">Total sem imposto.</span><span class="sxs-lookup"><span data-stu-id="b1204-222">Total before tax.</span></span> <span data-ttu-id="b1204-223">Verifica se seu subtotal corresponde ao total esperado, em caso de desconto.</span><span class="sxs-lookup"><span data-stu-id="b1204-223">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="b1204-224">11</span><span class="sxs-lookup"><span data-stu-id="b1204-224">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b1204-225">Tax</span><span class="sxs-lookup"><span data-stu-id="b1204-225">Tax</span></span></td>
<td><p><span data-ttu-id="b1204-226">Valor do imposto, com base nas regras&#39;de imposto de s do mercado e em circunstâncias específicas.</span><span class="sxs-lookup"><span data-stu-id="b1204-226">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="b1204-227">0</span><span class="sxs-lookup"><span data-stu-id="b1204-227">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b1204-228">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="b1204-228">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="b1204-229">Total com imposto.</span><span class="sxs-lookup"><span data-stu-id="b1204-229">Total after tax.</span></span> <span data-ttu-id="b1204-230">Verifica se o imposto é cobrado na fatura.</span><span class="sxs-lookup"><span data-stu-id="b1204-230">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="b1204-231">11</span><span class="sxs-lookup"><span data-stu-id="b1204-231">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b1204-232">Currency</span><span class="sxs-lookup"><span data-stu-id="b1204-232">Currency</span></span></td>
<td><p><span data-ttu-id="b1204-233">Tipo de moeda.</span><span class="sxs-lookup"><span data-stu-id="b1204-233">Currency type.</span></span> <span data-ttu-id="b1204-234">Cada entidade de cobrança tem somente uma moeda.</span><span class="sxs-lookup"><span data-stu-id="b1204-234">Each billing entity has only one currency.</span></span> <span data-ttu-id="b1204-235">Verifique se isso coincide com a primeira fatura e faça o mesmo após grandes atualizações na plataforma de cobrança.</span><span class="sxs-lookup"><span data-stu-id="b1204-235">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="b1204-236">EUR</span><span class="sxs-lookup"><span data-stu-id="b1204-236">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b1204-237">CustomerName</span><span class="sxs-lookup"><span data-stu-id="b1204-237">CustomerName</span></span></td>
<td><p><span data-ttu-id="b1204-238">Nome&#39;da organização do cliente como relatado no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="b1204-238">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="b1204-239">Isso é muito importante para reconciliar a fatura com as informações de seu sistema.</span><span class="sxs-lookup"><span data-stu-id="b1204-239">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="b1204-240">Cliente de teste A</span><span class="sxs-lookup"><span data-stu-id="b1204-240">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b1204-241">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="b1204-241">MPNID</span></span></td>
<td><p><span data-ttu-id="b1204-242">ID do MPN do parceiro CSP</span><span class="sxs-lookup"><span data-stu-id="b1204-242">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="b1204-243">4390934</span><span class="sxs-lookup"><span data-stu-id="b1204-243">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b1204-244">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="b1204-244">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="b1204-245">ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="b1204-245">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="b1204-246">Consulte <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Discriminar por parceiro</a>.</span><span class="sxs-lookup"><span data-stu-id="b1204-246">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="b1204-247">4390934</span><span class="sxs-lookup"><span data-stu-id="b1204-247">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b1204-248">DomainName</span><span class="sxs-lookup"><span data-stu-id="b1204-248">DomainName</span></span></td>
<td><p><span data-ttu-id="b1204-249">Nome&#39;de domínio do cliente, usado para ajudar a identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="b1204-249">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="b1204-250">Isso não deve ser usado para identificar exclusivamente o cliente, pois o cliente/parceiro pode atualizar o domínio intuitivo/padrão por meio do portal do O365.</span><span class="sxs-lookup"><span data-stu-id="b1204-250">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="b1204-251">Este campo pode aparecer em branco até o segundo ciclo de cobrança.</span><span class="sxs-lookup"><span data-stu-id="b1204-251">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="b1204-252">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="b1204-252">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b1204-253">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="b1204-253">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="b1204-254">Apelido da Inscrição.</span><span class="sxs-lookup"><span data-stu-id="b1204-254">Subscription nickname.</span></span> <span data-ttu-id="b1204-255">Se nenhum apelido for especificado, o Partner Center usa o OfferName.</span><span class="sxs-lookup"><span data-stu-id="b1204-255">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="b1204-256">PROJETO ONLINE</span><span class="sxs-lookup"><span data-stu-id="b1204-256">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b1204-257">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="b1204-257">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="b1204-258">O nome da oferta de serviço comprada pelo cliente, conforme definido na tabela de preços.</span><span class="sxs-lookup"><span data-stu-id="b1204-258">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="b1204-259">(Este é um campo idêntico ao nome da oferta).</span><span class="sxs-lookup"><span data-stu-id="b1204-259">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="b1204-260">PROJETO ONLINE PREMIUM SEM PROJETO CLIENTE</span><span class="sxs-lookup"><span data-stu-id="b1204-260">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="b1204-261">Campos de arquivo com base no uso</span><span class="sxs-lookup"><span data-stu-id="b1204-261">Usage-based file fields</span></span>


<span data-ttu-id="b1204-262">Para reconciliar seus encargos com o uso de seu cliente, compare ResellerID/ResellerName/ResellerBillableAccount do arquivo de reconciliação com o nome do cliente e a ID da assinatura do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="b1204-262">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="b1204-263">Os campos a seguir explicam quais serviços foram usados e a taxa.</span><span class="sxs-lookup"><span data-stu-id="b1204-263">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="b1204-264"><strong>Coluna</strong></span><span class="sxs-lookup"><span data-stu-id="b1204-264"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="b1204-265"><strong>Descrição</strong></span><span class="sxs-lookup"><span data-stu-id="b1204-265"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="b1204-266"><strong>Valor de exemplo</strong></span><span class="sxs-lookup"><span data-stu-id="b1204-266"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b1204-267">PartnerID</span><span class="sxs-lookup"><span data-stu-id="b1204-267">PartnerID</span></span></td>
<td><p><span data-ttu-id="b1204-268">ID do parceiro, no formato GUID.</span><span class="sxs-lookup"><span data-stu-id="b1204-268">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="b1204-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="b1204-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b1204-270">PartnerName</span><span class="sxs-lookup"><span data-stu-id="b1204-270">PartnerName</span></span></td>
<td><p><span data-ttu-id="b1204-271">Nome do parceiro.</span><span class="sxs-lookup"><span data-stu-id="b1204-271">Partner Name.</span></span></p></td>
<td><span data-ttu-id="b1204-272">Acme incorporado</span><span class="sxs-lookup"><span data-stu-id="b1204-272">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b1204-273">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="b1204-273">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="b1204-274">ID da conta do parceiro.</span><span class="sxs-lookup"><span data-stu-id="b1204-274">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="b1204-275">1010578050</span><span class="sxs-lookup"><span data-stu-id="b1204-275">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b1204-276">CustomerName</span><span class="sxs-lookup"><span data-stu-id="b1204-276">CustomerName</span></span></td>
<td><p><span data-ttu-id="b1204-277">Nome&#39;da organização do cliente como relatado no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="b1204-277">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="b1204-278">Isso é muito importante para reconciliar a fatura com as informações de seu sistema.</span><span class="sxs-lookup"><span data-stu-id="b1204-278">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="b1204-279">Cliente de teste A</span><span class="sxs-lookup"><span data-stu-id="b1204-279">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b1204-280">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="b1204-280">MPNID</span></span></td>
<td><p><span data-ttu-id="b1204-281">ID do MPN do parceiro CSP.</span><span class="sxs-lookup"><span data-stu-id="b1204-281">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="b1204-282">4390934</span><span class="sxs-lookup"><span data-stu-id="b1204-282">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b1204-283">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="b1204-283">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="b1204-284">ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="b1204-284">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="b1204-285">Consulte <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Discriminar por parceiro</a>.</span><span class="sxs-lookup"><span data-stu-id="b1204-285">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="b1204-286">4390934</span><span class="sxs-lookup"><span data-stu-id="b1204-286">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b1204-287">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="b1204-287">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="b1204-288">Número da fatura na qual a transação especificada é exibida.</span><span class="sxs-lookup"><span data-stu-id="b1204-288">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="b1204-289">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="b1204-289">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b1204-290">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="b1204-290">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="b1204-291">Data de início do ciclo de cobrança exceto quando apresentadas as datas de dados de uso latentes anteriormente não cobradas (do ciclo de cobrança anterior).</span><span class="sxs-lookup"><span data-stu-id="b1204-291">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="b1204-292">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="b1204-292">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="b1204-293">1/2/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="b1204-293">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b1204-294">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="b1204-294">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="b1204-295">Data de término do ciclo de cobrança exceto quando apresentadas as datas de dados de uso latentes anteriormente não cobradas (do ciclo de cobrança anterior).</span><span class="sxs-lookup"><span data-stu-id="b1204-295">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="b1204-296">A hora é sempre o fim do dia, 23:59.</span><span class="sxs-lookup"><span data-stu-id="b1204-296">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="b1204-297">28/2/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="b1204-297">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b1204-298">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="b1204-298">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="b1204-299">Identificador exclusivo de uma assinatura na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b1204-299">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="b1204-300">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="b1204-300">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="b1204-301">Esse não é o mesmo que o ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="b1204-301">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="b1204-302">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="b1204-302">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b1204-303">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="b1204-303">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="b1204-304">Apelido da oferta do serviço.</span><span class="sxs-lookup"><span data-stu-id="b1204-304">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="b1204-305">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="b1204-305">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b1204-306">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="b1204-306">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="b1204-307">Linha de negócios da oferta do serviço</span><span class="sxs-lookup"><span data-stu-id="b1204-307">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="b1204-308">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="b1204-308">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b1204-309">OrderID</span><span class="sxs-lookup"><span data-stu-id="b1204-309">OrderID</span></span></td>
<td><p><span data-ttu-id="b1204-310">Identificador exclusivo para um pedido na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b1204-310">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="b1204-311">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="b1204-311">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="b1204-312">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="b1204-312">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b1204-313">ServiceName</span><span class="sxs-lookup"><span data-stu-id="b1204-313">ServiceName</span></span></td>
<td><p><span data-ttu-id="b1204-314">O nome do serviço do Azure em questão.</span><span class="sxs-lookup"><span data-stu-id="b1204-314">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="b1204-315">MÁQUINAS VIRTUAIS</span><span class="sxs-lookup"><span data-stu-id="b1204-315">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b1204-316">ServiceType</span><span class="sxs-lookup"><span data-stu-id="b1204-316">ServiceType</span></span></td>
<td><p><span data-ttu-id="b1204-317">O tipo específico de serviço do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="b1204-317">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="b1204-318">Service Bus – Individual ou pacote</span><span class="sxs-lookup"><span data-stu-id="b1204-318">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="b1204-319">Banco de dados SQL Azure – Edição empresa ou Web</span><span class="sxs-lookup"><span data-stu-id="b1204-319">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b1204-320">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="b1204-320">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="b1204-321">Identificador exclusivo específico de toda a estrutura de serviço de dados e preço.</span><span class="sxs-lookup"><span data-stu-id="b1204-321">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="b1204-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="b1204-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b1204-323">Nome do recurso</span><span class="sxs-lookup"><span data-stu-id="b1204-323">Resource Name</span></span></td>
<td><p><span data-ttu-id="b1204-324">O nome do recurso do Azure.</span><span class="sxs-lookup"><span data-stu-id="b1204-324">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="b1204-325">Dados de entrada transferidos (GB)</span><span class="sxs-lookup"><span data-stu-id="b1204-325">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="b1204-326">Dados de saída transferidos (GB)</span><span class="sxs-lookup"><span data-stu-id="b1204-326">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b1204-327">Região</span><span class="sxs-lookup"><span data-stu-id="b1204-327">Region</span></span></td>
<td><p><span data-ttu-id="b1204-328">A região a qual o uso se aplica.</span><span class="sxs-lookup"><span data-stu-id="b1204-328">The region the usage applies to.</span></span> <span data-ttu-id="b1204-329">Usado principalmente para atribuir as taxas de transferências de dados, já que as taxas variam de acordo com a região.</span><span class="sxs-lookup"><span data-stu-id="b1204-329">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="b1204-330">Pacífico Asiático, Europa, América Latina e América do Norte</span><span class="sxs-lookup"><span data-stu-id="b1204-330">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b1204-331">SKU</span><span class="sxs-lookup"><span data-stu-id="b1204-331">SKU</span></span></td>
<td><p><span data-ttu-id="b1204-332">Identificador exclusivo MSFT da oferta</span><span class="sxs-lookup"><span data-stu-id="b1204-332">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="b1204-333">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="b1204-333">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="b1204-334">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="b1204-334">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="b1204-335">Uma ID e a quantidade para discriminar as taxas diferentes de um serviço ou recurso em um determinado período de cobrança.</span><span class="sxs-lookup"><span data-stu-id="b1204-335">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="b1204-336">Para a classificação em camadas do Azure, pode haver uma taxa para uma determinada quantidade de unidades faturáveis e uma taxa diferente depois disso.</span><span class="sxs-lookup"><span data-stu-id="b1204-336">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="b1204-337">1</span><span class="sxs-lookup"><span data-stu-id="b1204-337">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b1204-338">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="b1204-338">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="b1204-339">A quantidade de serviço consumida (horas, GB etc.) durante o período de relatório.</span><span class="sxs-lookup"><span data-stu-id="b1204-339">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="b1204-340">Também inclui qualquer uso não cobrado de períodos de relatório anteriores.</span><span class="sxs-lookup"><span data-stu-id="b1204-340">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="b1204-341">11</span><span class="sxs-lookup"><span data-stu-id="b1204-341">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b1204-342">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="b1204-342">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="b1204-343">Unidades incluídas como parte da oferta.</span><span class="sxs-lookup"><span data-stu-id="b1204-343">Units included as part of the offer.</span></span> <span data-ttu-id="b1204-344">Normalmente não está presente no CSP.</span><span class="sxs-lookup"><span data-stu-id="b1204-344">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="b1204-345">0</span><span class="sxs-lookup"><span data-stu-id="b1204-345">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="b1204-346">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="b1204-346">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="b1204-347">Unidades não incluídas como parte da oferta devem ser pagas pelo parceiro.</span><span class="sxs-lookup"><span data-stu-id="b1204-347">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="b1204-348">Igual a ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="b1204-348">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="b1204-349">11</span><span class="sxs-lookup"><span data-stu-id="b1204-349">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b1204-350">ListPrice</span><span class="sxs-lookup"><span data-stu-id="b1204-350">ListPrice</span></span></td>
<td><p><span data-ttu-id="b1204-351">Preço da oferta em vigor na data de início da assinatura.</span><span class="sxs-lookup"><span data-stu-id="b1204-351">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="b1204-352">U$ 0,0808</span><span class="sxs-lookup"><span data-stu-id="b1204-352">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b1204-353">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="b1204-353">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="b1204-354">ListPrist vezes OverageQuantity, arredondado para o centavo mais próximo.</span><span class="sxs-lookup"><span data-stu-id="b1204-354">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="b1204-355">U$ 0,085</span><span class="sxs-lookup"><span data-stu-id="b1204-355">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b1204-356">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="b1204-356">TaxAmount</span></span></td>
<td><p><span data-ttu-id="b1204-357">Valor do imposto, com base nas regras&#39;de imposto de s do mercado e em circunstâncias específicas.</span><span class="sxs-lookup"><span data-stu-id="b1204-357">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="b1204-358">U$ 0,08</span><span class="sxs-lookup"><span data-stu-id="b1204-358">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b1204-359">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="b1204-359">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="b1204-360">Total após imposto, quando o imposto é aplicável.</span><span class="sxs-lookup"><span data-stu-id="b1204-360">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="b1204-361">U$ 0,93</span><span class="sxs-lookup"><span data-stu-id="b1204-361">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b1204-362">Currency</span><span class="sxs-lookup"><span data-stu-id="b1204-362">Currency</span></span></td>
<td><p><span data-ttu-id="b1204-363">Tipo de moeda.</span><span class="sxs-lookup"><span data-stu-id="b1204-363">Currency type.</span></span> <span data-ttu-id="b1204-364">Cada entidade de cobrança tem somente uma moeda.</span><span class="sxs-lookup"><span data-stu-id="b1204-364">Each billing entity has only one currency.</span></span> <span data-ttu-id="b1204-365">Verifique se isso coincide com a primeira fatura e faça o mesmo após grandes atualizações na plataforma de cobrança.</span><span class="sxs-lookup"><span data-stu-id="b1204-365">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="b1204-366">EUR</span><span class="sxs-lookup"><span data-stu-id="b1204-366">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b1204-367">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="b1204-367">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="b1204-368">Preço por unidade sem imposto.</span><span class="sxs-lookup"><span data-stu-id="b1204-368">Pretax price per unit.</span></span> <span data-ttu-id="b1204-369">Igual a PretaxCharges / OverageQuantity, arredondado para o centavo mais próximo.</span><span class="sxs-lookup"><span data-stu-id="b1204-369">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="b1204-370">U$ 0,08</span><span class="sxs-lookup"><span data-stu-id="b1204-370">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b1204-371">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="b1204-371">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="b1204-372">Preço pós-imposto por unidade.</span><span class="sxs-lookup"><span data-stu-id="b1204-372">Post tax price per unit.</span></span> <span data-ttu-id="b1204-373">Igual a PostTaxTotal / OverageQuantity, ou PretaxEffectiveRate + taxa de imposto por valor de unidade, arredondado para o centavo mais próximo.</span><span class="sxs-lookup"><span data-stu-id="b1204-373">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="b1204-374">U$ 0,08</span><span class="sxs-lookup"><span data-stu-id="b1204-374">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b1204-375">ChargeType</span><span class="sxs-lookup"><span data-stu-id="b1204-375">ChargeType</span></span></td>
<td><p><span data-ttu-id="b1204-376">O tipo de encargo ou ajuste.</span><span class="sxs-lookup"><span data-stu-id="b1204-376">The type of charge or adjustment.</span></span> <span data-ttu-id="b1204-377">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="b1204-377">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="b1204-378">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="b1204-378">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b1204-379">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="b1204-379">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="b1204-380">ID exclusiva da conta na plataforma de cobrança da MSFT.</span><span class="sxs-lookup"><span data-stu-id="b1204-380">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="b1204-381">1280018095</span><span class="sxs-lookup"><span data-stu-id="b1204-381">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b1204-382">UsageDate</span><span class="sxs-lookup"><span data-stu-id="b1204-382">UsageDate</span></span></td>
<td><p><span data-ttu-id="b1204-383">Data da implantação do serviço.</span><span class="sxs-lookup"><span data-stu-id="b1204-383">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="b1204-384">1/2/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="b1204-384">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b1204-385">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="b1204-385">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="b1204-386">Essa coluna identifica a localização de um data center dentro da região para serviços onde isso é aplicável e preenchido.</span><span class="sxs-lookup"><span data-stu-id="b1204-386">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="b1204-387">Leste da Ásia, Sudeste da Ásia, Norte da Europa, Europa Ocidental, Centro Norte e Centro Sul dos EUA</span><span class="sxs-lookup"><span data-stu-id="b1204-387">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b1204-388">MeteredService</span><span class="sxs-lookup"><span data-stu-id="b1204-388">MeteredService</span></span></td>
<td><p><span data-ttu-id="b1204-389">Essa coluna é utilizada para rastrear o serviço do Microsoft Azure individual que não pode ser identificado especificamente na coluna Nome do Serviço.</span><span class="sxs-lookup"><span data-stu-id="b1204-389">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="b1204-390">Por exemplo, transferências de dados são relatadas como &quot;Microsoft Azure – Todos os Serviços&quot; na coluna Nome do Serviço.</span><span class="sxs-lookup"><span data-stu-id="b1204-390">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="b1204-391">Essa coluna MeteredService indicará ao qual serviço específico o uso pertence.</span><span class="sxs-lookup"><span data-stu-id="b1204-391">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="b1204-392">AccessControl, CDN, Computação, Banco de dados, ServiceBus, Armazenamento</span><span class="sxs-lookup"><span data-stu-id="b1204-392">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b1204-393">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="b1204-393">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="b1204-394">Um subcabeçalho que esclarece ainda mais o serviço Microsoft Azure individual além do nível fornecido pelo campo MeteredService.</span><span class="sxs-lookup"><span data-stu-id="b1204-394">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="b1204-395">EXTERNO</span><span class="sxs-lookup"><span data-stu-id="b1204-395">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b1204-396">Projeto</span><span class="sxs-lookup"><span data-stu-id="b1204-396">Project</span></span></td>
<td><p><span data-ttu-id="b1204-397">Nome definido pelo cliente para a instância do serviço</span><span class="sxs-lookup"><span data-stu-id="b1204-397">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="b1204-398">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="b1204-398">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b1204-399">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="b1204-399">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="b1204-400">O número de conexões ServiceBus que foram provisionados e utilizados em um dia específico.</span><span class="sxs-lookup"><span data-stu-id="b1204-400">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="b1204-401">Por exemplo: se você tivesse uma conexão individualmente provisionada durante um mês de 30 dias, a coluna Informação do Serviço 1 lerá "1,000000 conexões/30 dias".</span><span class="sxs-lookup"><span data-stu-id="b1204-401">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="b1204-402">Se você tiver um pacote de 25 pacotes de conexões do ServiceBus provisionado e tiver utilizado 1 durante esse dia, sua instrução de uso diário para esse dia indicaria "25 conexões/30 dias – usado: 1, 0 ".</span><span class="sxs-lookup"><span data-stu-id="b1204-402">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b1204-403">CustomerID</span><span class="sxs-lookup"><span data-stu-id="b1204-403">CustomerID</span></span></td>
<td><p><span data-ttu-id="b1204-404">ID exclusiva da Microsoft, no formato GUID, usada para identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="b1204-404">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="b1204-405">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="b1204-405">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b1204-406">DomainName</span><span class="sxs-lookup"><span data-stu-id="b1204-406">DomainName</span></span></td>
<td><p><span data-ttu-id="b1204-407">Nome&#39;de domínio do cliente, usado para ajudar a identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="b1204-407">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="b1204-408">Este campo pode aparecer em branco até o segundo ciclo de cobrança.</span><span class="sxs-lookup"><span data-stu-id="b1204-408">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="b1204-409">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="b1204-409">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="b1204-410">Unidade</span><span class="sxs-lookup"><span data-stu-id="b1204-410">Unit</span></span></td>
<td><p><span data-ttu-id="b1204-411">A unidade do nome do recurso</span><span class="sxs-lookup"><span data-stu-id="b1204-411">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="b1204-412">GB ou HORAS</span><span class="sxs-lookup"><span data-stu-id="b1204-412">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="b1204-413">Campos de arquivo de uso único e recorrente</span><span class="sxs-lookup"><span data-stu-id="b1204-413">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="b1204-414">Column</span><span class="sxs-lookup"><span data-stu-id="b1204-414">Column</span></span></th>
<th><span data-ttu-id="b1204-415">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1204-415">Description</span></span></th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td><span data-ttu-id="b1204-416">PartnerID</span><span class="sxs-lookup"><span data-stu-id="b1204-416">PartnerId</span></span></td>
<td><p><span data-ttu-id="b1204-417">Identificador de locatário de Microsoft Azure Active Directory exclusivo para uma entidade de cobrança específica, no formato GUID.</span><span class="sxs-lookup"><span data-stu-id="b1204-417">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="b1204-418">Não é necessário para reconciliação, mas pode ser uma informação útil.</span><span class="sxs-lookup"><span data-stu-id="b1204-418">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="b1204-419">O mesmo em todas as linhas.</span><span class="sxs-lookup"><span data-stu-id="b1204-419">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b1204-420">ID do cliente</span><span class="sxs-lookup"><span data-stu-id="b1204-420">Customer Id</span></span></td>
<td><p><span data-ttu-id="b1204-421">ID de locatário de Microsoft Azure Active Directory exclusiva, no formato GUID, usada para identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="b1204-421">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b1204-422">Nome do cliente</span><span class="sxs-lookup"><span data-stu-id="b1204-422">Customer Name</span></span></td>
<td><p><span data-ttu-id="b1204-423">Nome da organização do cliente como informado no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="b1204-423">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b1204-424">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="b1204-424">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="b1204-425">Nome de domínio do cliente, usado para ajudar a identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="b1204-425">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="b1204-426">Isso não deve ser usado para identificar exclusivamente o cliente, pois o cliente/parceiro pode atualizar o domínio intuitivo/padrão por meio do portal do O365.</span><span class="sxs-lookup"><span data-stu-id="b1204-426">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="b1204-427">Este campo pode aparecer em branco até o segundo ciclo de cobrança.</span><span class="sxs-lookup"><span data-stu-id="b1204-427">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b1204-428">País do cliente</span><span class="sxs-lookup"><span data-stu-id="b1204-428">Customer Country</span></span></td>
<td><p><span data-ttu-id="b1204-429">O país em que o cliente está localizado.</span><span class="sxs-lookup"><span data-stu-id="b1204-429">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b1204-430">Número da fatura</span><span class="sxs-lookup"><span data-stu-id="b1204-430">Invoice number</span></span></td>
<td><p><span data-ttu-id="b1204-431">Número da fatura na qual a transação especificada é exibida.</span><span class="sxs-lookup"><span data-stu-id="b1204-431">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b1204-432">MpnID</span><span class="sxs-lookup"><span data-stu-id="b1204-432">MpnId</span></span></td>
<td><p><span data-ttu-id="b1204-433">ID do MPN do parceiro CSP.</span><span class="sxs-lookup"><span data-stu-id="b1204-433">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b1204-434">MpnId do revendedor</span><span class="sxs-lookup"><span data-stu-id="b1204-434">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="b1204-435">ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="b1204-435">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b1204-436">ID do Pedido</span><span class="sxs-lookup"><span data-stu-id="b1204-436">Order ID</span></span></td>
<td><p><span data-ttu-id="b1204-437">Identificador exclusivo de um pedido na plataforma Microsoft Commerce.</span><span class="sxs-lookup"><span data-stu-id="b1204-437">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="b1204-438">Pode ser útil para identificar o pedido ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="b1204-438">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b1204-439">Data do pedido</span><span class="sxs-lookup"><span data-stu-id="b1204-439">Order date</span></span></td>
<td><p><span data-ttu-id="b1204-440">A data em que o pedido foi feito.</span><span class="sxs-lookup"><span data-stu-id="b1204-440">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b1204-441">ProductId</span><span class="sxs-lookup"><span data-stu-id="b1204-441">ProductId</span></span></td>
<td><p><span data-ttu-id="b1204-442">A ID do produto.</span><span class="sxs-lookup"><span data-stu-id="b1204-442">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b1204-443">SkuId</span><span class="sxs-lookup"><span data-stu-id="b1204-443">SkuId</span></span></td>
<td><p><span data-ttu-id="b1204-444">A ID de uma SKU em particular.</span><span class="sxs-lookup"><span data-stu-id="b1204-444">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b1204-445">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="b1204-445">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="b1204-446">A ID de uma Disponibilidade em particular.</span><span class="sxs-lookup"><span data-stu-id="b1204-446">The ID for a particular Availability.</span></span> <span data-ttu-id="b1204-447">"Disponibilidade" refere-se a se uma SKU em particular está disponível ou não para compra para determinado país, moeda, segmento do setor etc.</span><span class="sxs-lookup"><span data-stu-id="b1204-447">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b1204-448">Nome do SKU</span><span class="sxs-lookup"><span data-stu-id="b1204-448">SKU Name</span></span></td>
<td><p><span data-ttu-id="b1204-449">O título de uma SKU em particular.</span><span class="sxs-lookup"><span data-stu-id="b1204-449">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b1204-450">Nome do produto</span><span class="sxs-lookup"><span data-stu-id="b1204-450">Product name</span></span></td>
<td><p><span data-ttu-id="b1204-451">O nome do produto.</span><span class="sxs-lookup"><span data-stu-id="b1204-451">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b1204-452">PublisherName</span><span class="sxs-lookup"><span data-stu-id="b1204-452">PublisherName</span></span></td>
<td><p><span data-ttu-id="b1204-453">O nome do editor do produto.</span><span class="sxs-lookup"><span data-stu-id="b1204-453">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b1204-454">PublisherID</span><span class="sxs-lookup"><span data-stu-id="b1204-454">PublisherID</span></span></td>
<td><p><span data-ttu-id="b1204-455">ID exclusiva para este Publicador.</span><span class="sxs-lookup"><span data-stu-id="b1204-455">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b1204-456">Descrição da assinatura</span><span class="sxs-lookup"><span data-stu-id="b1204-456">Subscription Description</span></span></td>
<td><p><span data-ttu-id="b1204-457">Nome amigável de uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="b1204-457">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b1204-458">ID da assinatura</span><span class="sxs-lookup"><span data-stu-id="b1204-458">Subscription ID</span></span></td>
<td><p><span data-ttu-id="b1204-459">Identificador exclusivo de uma assinatura na plataforma Microsoft Commerce.</span><span class="sxs-lookup"><span data-stu-id="b1204-459">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="b1204-460">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="b1204-460">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="b1204-461">Esse não é o mesmo que o ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="b1204-461">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b1204-462">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="b1204-462">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="b1204-463">Dia de início dos encargos.</span><span class="sxs-lookup"><span data-stu-id="b1204-463">Start day of the charges.</span></span> <span data-ttu-id="b1204-464">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="b1204-464">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b1204-465">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="b1204-465">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="b1204-466">Dia do término dos encargos.</span><span class="sxs-lookup"><span data-stu-id="b1204-466">End day of the charges.</span></span> <span data-ttu-id="b1204-467">A hora é sempre o fim do dia, 23:59.</span><span class="sxs-lookup"><span data-stu-id="b1204-467">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b1204-468">Termo e Billingcycle</span><span class="sxs-lookup"><span data-stu-id="b1204-468">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="b1204-469">O tamanho do termo e o ciclo de cobrança da compra.</span><span class="sxs-lookup"><span data-stu-id="b1204-469">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="b1204-470">Por exemplo, "1 ano, mensalmente."</span><span class="sxs-lookup"><span data-stu-id="b1204-470">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b1204-471">Tipo de Cobrança</span><span class="sxs-lookup"><span data-stu-id="b1204-471">Charge Type</span></span></td>
<td><p><span data-ttu-id="b1204-472">O tipo de encargo ou ajuste.</span><span class="sxs-lookup"><span data-stu-id="b1204-472">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b1204-473">Preço unitário</span><span class="sxs-lookup"><span data-stu-id="b1204-473">Unit Price</span></span></td>
<td><p><span data-ttu-id="b1204-474">O preço como publicado na tabela de preços no momento da compra.</span><span class="sxs-lookup"><span data-stu-id="b1204-474">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="b1204-475">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="b1204-475">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b1204-476">Preço unitário efetivo</span><span class="sxs-lookup"><span data-stu-id="b1204-476">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="b1204-477">O preço unitário após os ajustes terem sido feitos.</span><span class="sxs-lookup"><span data-stu-id="b1204-477">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b1204-478">Quantidade</span><span class="sxs-lookup"><span data-stu-id="b1204-478">Quantity</span></span></td>
<td><p><span data-ttu-id="b1204-479">Número de unidades.</span><span class="sxs-lookup"><span data-stu-id="b1204-479">Number of units.</span></span> <span data-ttu-id="b1204-480">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="b1204-480">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b1204-481">Tipo de unidade</span><span class="sxs-lookup"><span data-stu-id="b1204-481">Unit type</span></span></td>
<td><p><span data-ttu-id="b1204-482">O tipo de unidade que está sendo adquirida.</span><span class="sxs-lookup"><span data-stu-id="b1204-482">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b1204-483">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="b1204-483">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="b1204-484">Uma explicação de qualquer desconto aplicável.</span><span class="sxs-lookup"><span data-stu-id="b1204-484">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b1204-485">Subtotal</span><span class="sxs-lookup"><span data-stu-id="b1204-485">Sub Total</span></span></td>
<td><p><span data-ttu-id="b1204-486">Total sem imposto.</span><span class="sxs-lookup"><span data-stu-id="b1204-486">Total before tax.</span></span> <span data-ttu-id="b1204-487">Verifica se seu subtotal corresponde ao total esperado, em caso de desconto.</span><span class="sxs-lookup"><span data-stu-id="b1204-487">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b1204-488">Total do imposto</span><span class="sxs-lookup"><span data-stu-id="b1204-488">Tax Total</span></span></td>
<td><p><span data-ttu-id="b1204-489">Valor do imposto cobrado, com base nas regras fiscais do mercado e em circunstâncias específicas.</span><span class="sxs-lookup"><span data-stu-id="b1204-489">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b1204-490">Total</span><span class="sxs-lookup"><span data-stu-id="b1204-490">Total</span></span></td>
<td><p><span data-ttu-id="b1204-491">Total com imposto.</span><span class="sxs-lookup"><span data-stu-id="b1204-491">Total after tax.</span></span> <span data-ttu-id="b1204-492">Verifica se o imposto é cobrado na fatura.</span><span class="sxs-lookup"><span data-stu-id="b1204-492">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b1204-493">Currency</span><span class="sxs-lookup"><span data-stu-id="b1204-493">Currency</span></span></td>
<td><p><span data-ttu-id="b1204-494">Tipo de moeda.</span><span class="sxs-lookup"><span data-stu-id="b1204-494">Currency type.</span></span> <span data-ttu-id="b1204-495">Cada entidade de cobrança tem somente uma moeda.</span><span class="sxs-lookup"><span data-stu-id="b1204-495">Each billing entity has only one currency.</span></span> <span data-ttu-id="b1204-496">Verifique se isso coincide com a primeira fatura e faça o mesmo após grandes atualizações na plataforma de cobrança.</span><span class="sxs-lookup"><span data-stu-id="b1204-496">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b1204-497">Uma alternateid</span><span class="sxs-lookup"><span data-stu-id="b1204-497">AlternateID</span></span></td>
<td><p><span data-ttu-id="b1204-498">Um identificador alternativo para uma ID de pedido.</span><span class="sxs-lookup"><span data-stu-id="b1204-498">An alternate identifier to an order ID.</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="b1204-499">Campos de arquivo de uso com classificação diária</span><span class="sxs-lookup"><span data-stu-id="b1204-499">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="b1204-500">Column</span><span class="sxs-lookup"><span data-stu-id="b1204-500">Column</span></span></th>
<th><span data-ttu-id="b1204-501">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1204-501">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="b1204-502">PartnerID</span><span class="sxs-lookup"><span data-stu-id="b1204-502">PartnerId</span></span></td>
<td><p><span data-ttu-id="b1204-503">ID do parceiro, no formato GUID.</span><span class="sxs-lookup"><span data-stu-id="b1204-503">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b1204-504">PartnerName</span><span class="sxs-lookup"><span data-stu-id="b1204-504">PartnerName</span></span></td>
<td><p><span data-ttu-id="b1204-505">Nome do parceiro.</span><span class="sxs-lookup"><span data-stu-id="b1204-505">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b1204-506">CustomerID</span><span class="sxs-lookup"><span data-stu-id="b1204-506">CustomerId</span></span></td>
<td><p><span data-ttu-id="b1204-507">ID exclusiva da Microsoft, no formato GUID, usada para identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="b1204-507">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b1204-508">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="b1204-508">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="b1204-509">Nome da organização do cliente como informado no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="b1204-509">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="b1204-510">Isso é muito importante para reconciliar a fatura com as informações de seu sistema.</span><span class="sxs-lookup"><span data-stu-id="b1204-510">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b1204-511">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="b1204-511">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="b1204-512">O nome de domínio do cliente.</span><span class="sxs-lookup"><span data-stu-id="b1204-512">The customer’s domain name.</span></span> <span data-ttu-id="b1204-513">Não disponível para a atividade atual.</span><span class="sxs-lookup"><span data-stu-id="b1204-513">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b1204-514">País do cliente</span><span class="sxs-lookup"><span data-stu-id="b1204-514">Customer country</span></span></td>
<td><p><span data-ttu-id="b1204-515">O país em que o cliente está localizado.</span><span class="sxs-lookup"><span data-stu-id="b1204-515">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b1204-516">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="b1204-516">MPNID</span></span></td>
<td><p><span data-ttu-id="b1204-517">ID do MPN do parceiro CSP.</span><span class="sxs-lookup"><span data-stu-id="b1204-517">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b1204-518">MPNID do revendedor</span><span class="sxs-lookup"><span data-stu-id="b1204-518">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="b1204-519">ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="b1204-519">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="b1204-520">Não disponível para a atividade atual.</span><span class="sxs-lookup"><span data-stu-id="b1204-520">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b1204-521">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="b1204-521">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="b1204-522">Número da fatura na qual a transação especificada é exibida.</span><span class="sxs-lookup"><span data-stu-id="b1204-522">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="b1204-523">Não disponível para a atividade atual.</span><span class="sxs-lookup"><span data-stu-id="b1204-523">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b1204-524">ProductId</span><span class="sxs-lookup"><span data-stu-id="b1204-524">ProductId</span></span></td>
<td><p><span data-ttu-id="b1204-525">A ID do produto.</span><span class="sxs-lookup"><span data-stu-id="b1204-525">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b1204-526">SkuId</span><span class="sxs-lookup"><span data-stu-id="b1204-526">SkuId</span></span></td>
<td><p><span data-ttu-id="b1204-527">A ID de uma SKU em particular.</span><span class="sxs-lookup"><span data-stu-id="b1204-527">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b1204-528">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="b1204-528">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="b1204-529">A ID de uma Disponibilidade em particular.</span><span class="sxs-lookup"><span data-stu-id="b1204-529">The ID for a particular Availability.</span></span> <span data-ttu-id="b1204-530">"Disponibilidade" refere-se a se uma SKU em particular está disponível ou não para compra para determinado país, moeda, segmento do setor etc.</span><span class="sxs-lookup"><span data-stu-id="b1204-530">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b1204-531">Nome do SKU</span><span class="sxs-lookup"><span data-stu-id="b1204-531">SKU Name</span></span></td>
<td><p><span data-ttu-id="b1204-532">O título de uma SKU em particular.</span><span class="sxs-lookup"><span data-stu-id="b1204-532">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b1204-533">PublisherName</span><span class="sxs-lookup"><span data-stu-id="b1204-533">PublisherName</span></span></td>
<td><p><span data-ttu-id="b1204-534">O nome do Publicador.</span><span class="sxs-lookup"><span data-stu-id="b1204-534">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b1204-535">PublisherID</span><span class="sxs-lookup"><span data-stu-id="b1204-535">PublisherID</span></span></td>
<td><p><span data-ttu-id="b1204-536">A ID do Publicador, no formato GUID.</span><span class="sxs-lookup"><span data-stu-id="b1204-536">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="b1204-537">Não disponível para a atividade atual.</span><span class="sxs-lookup"><span data-stu-id="b1204-537">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="b1204-538">Descrição da assinatura</span><span class="sxs-lookup"><span data-stu-id="b1204-538">Subscription Description</span></span></td>
<td><p><span data-ttu-id="b1204-539">O nome da oferta de serviço comprada pelo cliente, conforme definido na tabela de preços.</span><span class="sxs-lookup"><span data-stu-id="b1204-539">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="b1204-540">(Este é um campo idêntico ao nome da oferta).</span><span class="sxs-lookup"><span data-stu-id="b1204-540">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b1204-541">ID da assinatura</span><span class="sxs-lookup"><span data-stu-id="b1204-541">Subscription ID</span></span></td>
<td><p><span data-ttu-id="b1204-542">Identificador exclusivo de uma assinatura na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b1204-542">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="b1204-543">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="b1204-543">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="b1204-544">Esse não é o mesmo que o ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="b1204-544">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b1204-545">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="b1204-545">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="b1204-546">Data de início do ciclo de cobrança exceto quando apresentadas as datas de dados de uso latentes anteriormente não cobradas (do ciclo de cobrança anterior).</span><span class="sxs-lookup"><span data-stu-id="b1204-546">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="b1204-547">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="b1204-547">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b1204-548">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="b1204-548">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="b1204-549">Data de término do ciclo de cobrança exceto quando apresentadas as datas de dados de uso latentes anteriormente não cobradas (do ciclo de cobrança anterior).</span><span class="sxs-lookup"><span data-stu-id="b1204-549">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="b1204-550">A hora é sempre o fim do dia, 23:59.</span><span class="sxs-lookup"><span data-stu-id="b1204-550">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b1204-551">Data de uso</span><span class="sxs-lookup"><span data-stu-id="b1204-551">Usage Date</span></span></td>
<td><p><span data-ttu-id="b1204-552">Data de uso do serviço.</span><span class="sxs-lookup"><span data-stu-id="b1204-552">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b1204-553">Tipo de medidor</span><span class="sxs-lookup"><span data-stu-id="b1204-553">Meter Type</span></span></td>
<td><p><span data-ttu-id="b1204-554">O tipo de medidor.</span><span class="sxs-lookup"><span data-stu-id="b1204-554">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b1204-555">Categoria do medidor</span><span class="sxs-lookup"><span data-stu-id="b1204-555">Meter Category</span></span></td>
<td><p><span data-ttu-id="b1204-556">O serviço de nível superior para o uso.</span><span class="sxs-lookup"><span data-stu-id="b1204-556">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b1204-557">ID do medidor</span><span class="sxs-lookup"><span data-stu-id="b1204-557">Meter Id</span></span></td>
<td><p><span data-ttu-id="b1204-558">A ID do medidor que está sendo usado.</span><span class="sxs-lookup"><span data-stu-id="b1204-558">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b1204-559">Subcategoria do medidor</span><span class="sxs-lookup"><span data-stu-id="b1204-559">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="b1204-560">O tipo de serviço do Azure que pode afetar a taxa.</span><span class="sxs-lookup"><span data-stu-id="b1204-560">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b1204-561">Nome do medidor</span><span class="sxs-lookup"><span data-stu-id="b1204-561">Meter Name</span></span></td>
<td><p><span data-ttu-id="b1204-562">A unidade de medida para o medidor que está sendo consumido.</span><span class="sxs-lookup"><span data-stu-id="b1204-562">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b1204-563">Região do medidor</span><span class="sxs-lookup"><span data-stu-id="b1204-563">Meter Region</span></span></td>
<td><p><span data-ttu-id="b1204-564">Essa coluna identifica a localização de um data center dentro da região para serviços onde isso é aplicável e preenchido.</span><span class="sxs-lookup"><span data-stu-id="b1204-564">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b1204-565">Unidade</span><span class="sxs-lookup"><span data-stu-id="b1204-565">Unit</span></span></td>
<td><p><span data-ttu-id="b1204-566">A unidade do nome do recurso.</span><span class="sxs-lookup"><span data-stu-id="b1204-566">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b1204-567">Quantidade consumida</span><span class="sxs-lookup"><span data-stu-id="b1204-567">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="b1204-568">A quantidade de serviço consumida (horas, GB etc.) durante o período de relatório.</span><span class="sxs-lookup"><span data-stu-id="b1204-568">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="b1204-569">Também inclui qualquer uso não cobrado de períodos de relatório anteriores.</span><span class="sxs-lookup"><span data-stu-id="b1204-569">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b1204-570">Local do recurso</span><span class="sxs-lookup"><span data-stu-id="b1204-570">Resource Location</span></span></td>
<td><p><span data-ttu-id="b1204-571">O datacenter em que o medidor está em execução.</span><span class="sxs-lookup"><span data-stu-id="b1204-571">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b1204-572">Serviço consumido</span><span class="sxs-lookup"><span data-stu-id="b1204-572">Consumed Service</span></span></td>
<td><p><span data-ttu-id="b1204-573">O serviço da plataforma do Azure que você usou.</span><span class="sxs-lookup"><span data-stu-id="b1204-573">The Azure platform service that you used.</span></span></p></td>
</tr>


<tr class="even">
<td><span data-ttu-id="b1204-574">URI de recurso</span><span class="sxs-lookup"><span data-stu-id="b1204-574">Resource URI</span></span></td>
<td><p><span data-ttu-id="b1204-575">O URI do recurso que está sendo usado.</span><span class="sxs-lookup"><span data-stu-id="b1204-575">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b1204-576">Tipo de cobrança</span><span class="sxs-lookup"><span data-stu-id="b1204-576">Charge type</span></span></td>
<td><p><span data-ttu-id="b1204-577">O tipo de encargo ou ajuste.</span><span class="sxs-lookup"><span data-stu-id="b1204-577">The type of charge or adjustment.</span></span> <span data-ttu-id="b1204-578">Não disponível para a atividade atual.</span><span class="sxs-lookup"><span data-stu-id="b1204-578">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b1204-579">Preço unitário</span><span class="sxs-lookup"><span data-stu-id="b1204-579">Unit price</span></span></td>
<td><p><span data-ttu-id="b1204-580">Preço por licença, conforme publicado na tabela de preços no momento da compra.</span><span class="sxs-lookup"><span data-stu-id="b1204-580">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="b1204-581">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="b1204-581">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b1204-582">Quantidade</span><span class="sxs-lookup"><span data-stu-id="b1204-582">Quantity</span></span></td>
<td><p><span data-ttu-id="b1204-583">Número de licenças.</span><span class="sxs-lookup"><span data-stu-id="b1204-583">Number of licenses.</span></span> <span data-ttu-id="b1204-584">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="b1204-584">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b1204-585">Tipo de unidade</span><span class="sxs-lookup"><span data-stu-id="b1204-585">Unit type</span></span></td>
<td><p><span data-ttu-id="b1204-586">O tipo de unidade em que o medidor é cobrado.</span><span class="sxs-lookup"><span data-stu-id="b1204-586">The type of unit the meter is charged in.</span></span> <span data-ttu-id="b1204-587">Não disponível para a atividade atual.</span><span class="sxs-lookup"><span data-stu-id="b1204-587">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b1204-588">Pré-imposto de cobrança</span><span class="sxs-lookup"><span data-stu-id="b1204-588">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="b1204-589">Valor total antes dos impostos.</span><span class="sxs-lookup"><span data-stu-id="b1204-589">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b1204-590">Moeda de cobrança</span><span class="sxs-lookup"><span data-stu-id="b1204-590">Billing currency</span></span></td>
<td><p><span data-ttu-id="b1204-591">A moeda na região geográfica do cliente</span><span class="sxs-lookup"><span data-stu-id="b1204-591">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b1204-592">Preço custo total</span><span class="sxs-lookup"><span data-stu-id="b1204-592">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="b1204-593">O preço antes da adição de impostos.</span><span class="sxs-lookup"><span data-stu-id="b1204-593">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b1204-594">Moeda de preços</span><span class="sxs-lookup"><span data-stu-id="b1204-594">Pricing currency</span></span></td>
<td><p><span data-ttu-id="b1204-595">A moeda na tabela de preços.</span><span class="sxs-lookup"><span data-stu-id="b1204-595">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b1204-596">Informações de serviço 1</span><span class="sxs-lookup"><span data-stu-id="b1204-596">Service Info 1</span></span></td>
<td><p><span data-ttu-id="b1204-597">O número de conexões ServiceBus que foram provisionados e utilizados em um dia específico.</span><span class="sxs-lookup"><span data-stu-id="b1204-597">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b1204-598">Informações de serviço 2</span><span class="sxs-lookup"><span data-stu-id="b1204-598">Service Info 2</span></span></td>
<td><p><span data-ttu-id="b1204-599">Um campo herdado que captura metadados específicos do serviço opcionais.</span><span class="sxs-lookup"><span data-stu-id="b1204-599">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b1204-600">Informações adicionais</span><span class="sxs-lookup"><span data-stu-id="b1204-600">Additional Info</span></span></td>
<td><p><span data-ttu-id="b1204-601">Quaisquer informações adicionais não abordadas em outras colunas.</span><span class="sxs-lookup"><span data-stu-id="b1204-601">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="b1204-602">Mapeando cobranças entre uma fatura e o arquivo de reconciliação</span><span class="sxs-lookup"><span data-stu-id="b1204-602">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="b1204-603">Sua fatura fornece um resumo dos encargos, enquanto seu arquivo de reconciliação fornece uma divisão detalhada das transações de item de linha, incluindo os tipos de carga.</span><span class="sxs-lookup"><span data-stu-id="b1204-603">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="b1204-604">Para fazer referência cruzada das quantidades de carga entre o arquivo de reconciliação e fatura, você pode usar opções de filtro do Microsoft Excel para filtrar por tipos de cobrança no arquivo de reconciliação para mapear os encargos de fatura em um conjunto de detalhamentos de cobrança no arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="b1204-604">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="b1204-605">Os arquivos de reconciliação, tanto os baseados em licença quanto os baseados em uso, mostram apenas encargos e transações relacionadas ao uso (unidades consumidas e encargos relacionados).</span><span class="sxs-lookup"><span data-stu-id="b1204-605">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="b1204-606">Créditos únicos, descontos ou reembolsos que aparecem na fatura como "Ajustes" não são mostrados no arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="b1204-606">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="b1204-607">A tabela a seguir mostra os mapeamentos entre uma seção da fatura e os tipos de encargo associados que podem aparecer nos arquivos de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="b1204-607">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="b1204-608"><strong>Descrição da cobrança da fatura</strong></span><span class="sxs-lookup"><span data-stu-id="b1204-608"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="b1204-609"><strong>Descrição do encargo do arquivo de reconciliação (coluna Chargetype)</strong></span><span class="sxs-lookup"><span data-stu-id="b1204-609"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="b1204-610"><strong>Qual é essa cobrança?</strong></span><span class="sxs-lookup"><span data-stu-id="b1204-610"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="b1204-611"><strong>Como fazer mapear esses ChargeTypes para a fatura?</strong></span><span class="sxs-lookup"><span data-stu-id="b1204-611"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="b1204-612"><strong>Encargos baseados em licença</strong></span><span class="sxs-lookup"><span data-stu-id="b1204-612"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="b1204-613">Taxa de ativação</span><span class="sxs-lookup"><span data-stu-id="b1204-613">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="b1204-614">O valor cobrado do cliente quando ele usa a assinatura depois de comprá-la.</span><span class="sxs-lookup"><span data-stu-id="b1204-614">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="b1204-615">No arquivo baseado em licença, some a coluna <strong>Quantidade</strong></span><span class="sxs-lookup"><span data-stu-id="b1204-615">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b1204-616">Taxa de cancelamento</span><span class="sxs-lookup"><span data-stu-id="b1204-616">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="b1204-617">Os encargos proporcionais reembolsados para o cliente quando os assentos associados são alterados</span><span class="sxs-lookup"><span data-stu-id="b1204-617">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b1204-618">Taxa do ciclo</span><span class="sxs-lookup"><span data-stu-id="b1204-618">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="b1204-619">Encargos periódicos de uma assinatura</span><span class="sxs-lookup"><span data-stu-id="b1204-619">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b1204-620">Proporcional à instância do ciclo</span><span class="sxs-lookup"><span data-stu-id="b1204-620">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="b1204-621">Os encargos proporcionais cobrados do cliente quando os assentos associados são alterados</span><span class="sxs-lookup"><span data-stu-id="b1204-621">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b1204-622">Taxas proporcionais durante o cancelamento</span><span class="sxs-lookup"><span data-stu-id="b1204-622">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="b1204-623">Reembolso proporcional para a parte não utilizada do serviço após o cancelamento</span><span class="sxs-lookup"><span data-stu-id="b1204-623">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b1204-624">Taxas proporcionais durante a compra</span><span class="sxs-lookup"><span data-stu-id="b1204-624">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="b1204-625">O tipo de encargo para uma assinatura ao usar a cobrança anual</span><span class="sxs-lookup"><span data-stu-id="b1204-625">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b1204-626">Valor de compra</span><span class="sxs-lookup"><span data-stu-id="b1204-626">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="b1204-627">O tipo de encargo para uma assinatura ao usar a cobrança mensal</span><span class="sxs-lookup"><span data-stu-id="b1204-627">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b1204-628">Taxa proporcional ao renovar</span><span class="sxs-lookup"><span data-stu-id="b1204-628">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="b1204-629">Taxas proporcionais após a renovação da assinatura</span><span class="sxs-lookup"><span data-stu-id="b1204-629">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="b1204-630">Taxa de renovação</span><span class="sxs-lookup"><span data-stu-id="b1204-630">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="b1204-631">Cobrança para renovação de uma assinatura</span><span class="sxs-lookup"><span data-stu-id="b1204-631">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b1204-632">Taxas proporcionais ao ativar</span><span class="sxs-lookup"><span data-stu-id="b1204-632">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="b1204-633">Taxas proporcionais da ativação até o final do período de cobrança</span><span class="sxs-lookup"><span data-stu-id="b1204-633">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>



<tr>
<td rowspan="5">
<p><span data-ttu-id="b1204-634"><strong>Encargos de uso único</strong></span><span class="sxs-lookup"><span data-stu-id="b1204-634"><strong>One-time Charges</strong></span></span></p>

</td>
<td>
<p><span data-ttu-id="b1204-635">Novo</span><span class="sxs-lookup"><span data-stu-id="b1204-635">New</span></span></p>
</td>
<td>
<p><span data-ttu-id="b1204-636">Usado quando uma nova compra é criada</span><span class="sxs-lookup"><span data-stu-id="b1204-636">Used when a new purchase is created</span></span></p>
</td>

<p></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b1204-637">addquantity</span><span class="sxs-lookup"><span data-stu-id="b1204-637">addQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="b1204-638">Usado tanto no reembolso da compra original quanto na nova quantidade após o aumento</span><span class="sxs-lookup"><span data-stu-id="b1204-638">Used in both the refund of the original purchase and the new quantity after increase</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="b1204-639">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="b1204-639">removeQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="b1204-640">Usado tanto no reembolso da compra original quanto na nova quantidade após a diminuição</span><span class="sxs-lookup"><span data-stu-id="b1204-640">Used in both the refund of the original purchase and the new quantity after decrease</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="b1204-641">Cancel</span><span class="sxs-lookup"><span data-stu-id="b1204-641">Cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="b1204-642">Usado quando uma assinatura é cancelada</span><span class="sxs-lookup"><span data-stu-id="b1204-642">Used when a subscription is cancelled</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="b1204-643">Converter</span><span class="sxs-lookup"><span data-stu-id="b1204-643">Convert</span></span></p>
</td>
<td>
<p><span data-ttu-id="b1204-644">Usado quando uma licença é atualizada, mas o número de estações permanece inalterado</span><span class="sxs-lookup"><span data-stu-id="b1204-644">Used when a license is upgraded but the number of seats remains unchanged</span></span></p>
</td>
</tr>

<tr>
<td rowspan="2">
<p><span data-ttu-id="b1204-645"><strong>Encargos de uso</strong></span><span class="sxs-lookup"><span data-stu-id="b1204-645"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="b1204-646">Avaliar a taxa de uso ao cancelar</span><span class="sxs-lookup"><span data-stu-id="b1204-646">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="b1204-647">Taxa de uso de acesso com o cancelamento para uso não pago durante o período de cobrança atual</span><span class="sxs-lookup"><span data-stu-id="b1204-647">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="b1204-648">No arquivo baseado em uso, some a coluna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="b1204-648">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b1204-649">Avalie a taxa de uso para o ciclo atual</span><span class="sxs-lookup"><span data-stu-id="b1204-649">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="b1204-650">Taxa de uso de acesso para o período atual de cobrança</span><span class="sxs-lookup"><span data-stu-id="b1204-650">Access usage fee for the current billing period</span></span></p>
</td>
</tr>

<tr>
<td>
<p><span data-ttu-id="b1204-651"><strong>Crédito</strong></span><span class="sxs-lookup"><span data-stu-id="b1204-651"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="b1204-652">Deslocando um item de linha</span><span class="sxs-lookup"><span data-stu-id="b1204-652">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="b1204-653">Reembolso parcial ou integral para um item de linha, incluindo os impostos</span><span class="sxs-lookup"><span data-stu-id="b1204-653">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="b1204-654">No arquivo baseado em licença, some a coluna <strong>TotalForCustomer</strong></span><span class="sxs-lookup"><span data-stu-id="b1204-654">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="b1204-655">No arquivo baseado em uso, some a coluna <strong>PostTaxTotal</strong></span><span class="sxs-lookup"><span data-stu-id="b1204-655">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="b1204-656"><strong>Descontos com base no uso</strong></span><span class="sxs-lookup"><span data-stu-id="b1204-656"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="b1204-657">Desconto de ativação</span><span class="sxs-lookup"><span data-stu-id="b1204-657">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="b1204-658">Desconto aplicado quando a assinatura é ativada</span><span class="sxs-lookup"><span data-stu-id="b1204-658">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="b1204-659">No arquivo baseado em uso, some a coluna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="b1204-659">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b1204-660">Desconto de ciclo</span><span class="sxs-lookup"><span data-stu-id="b1204-660">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="b1204-661">Desconto aplicado em cobranças periódicas</span><span class="sxs-lookup"><span data-stu-id="b1204-661">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b1204-662">Desconto de renovação</span><span class="sxs-lookup"><span data-stu-id="b1204-662">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="b1204-663">Desconto aplicado quando a assinatura é renovada</span><span class="sxs-lookup"><span data-stu-id="b1204-663">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b1204-664">Desconto de cancelamento</span><span class="sxs-lookup"><span data-stu-id="b1204-664">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="b1204-665">Encargos aplicados quando descontos são cancelados</span><span class="sxs-lookup"><span data-stu-id="b1204-665">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="b1204-666"><strong>Descontos baseados em licença</strong></span><span class="sxs-lookup"><span data-stu-id="b1204-666"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="b1204-667"><em>Pode ser aplicado a vários tipos de cobrança</em></span><span class="sxs-lookup"><span data-stu-id="b1204-667"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="b1204-668">No arquivo baseado em licença, some a coluna <strong>TotalOtherDiscount</strong></span><span class="sxs-lookup"><span data-stu-id="b1204-668">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b1204-669"><strong>Impostos</strong>&nbsp;ou&nbsp;<strong>IVA</strong></span><span class="sxs-lookup"><span data-stu-id="b1204-669"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="b1204-670"><em>Pode ser aplicado a vários tipos de cobrança</em></span><span class="sxs-lookup"><span data-stu-id="b1204-670"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="b1204-671"><em>Exception &quot;Deslocar um item&quot; de linha já inclui impostos. Consulte créditos, acima.</em></span><span class="sxs-lookup"><span data-stu-id="b1204-671"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="b1204-672">Impostos ou impostos sobre valor agregado (IVA)</span><span class="sxs-lookup"><span data-stu-id="b1204-672">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="b1204-673">No arquivo baseado em licença, some a coluna <strong>Imposto</strong></span><span class="sxs-lookup"><span data-stu-id="b1204-673">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="b1204-674">No arquivo baseado em uso, some a coluna <strong>TaxAmount</strong></span><span class="sxs-lookup"><span data-stu-id="b1204-674">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
