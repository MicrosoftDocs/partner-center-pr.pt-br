---
title: Usar os arquivos de reconciliação | Partner Center
ms.topic: article
ms.date: 11/07/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Para obter uma exibição detalhada de item de linha de cada encargo em um ciclo de cobrança, baixe os arquivos de reconciliação do Partner Center.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 217d5e9c068a07b51f74333f605daca8ab573c9a
ms.sourcegitcommit: 8425d3435892651e3e6cb1147cd3b268b2b1869b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/07/2019
ms.locfileid: "73753856"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="0a6cc-103">Usar os arquivos de reconciliação</span><span class="sxs-lookup"><span data-stu-id="0a6cc-103">Use the reconciliation files</span></span>

<span data-ttu-id="0a6cc-104">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="0a6cc-104">**Applies to**</span></span>

-  <span data-ttu-id="0a6cc-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="0a6cc-105">Partner Center</span></span>
-  <span data-ttu-id="0a6cc-106">Partner Center do Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="0a6cc-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="0a6cc-107">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="0a6cc-107">**Appropriate roles**</span></span>

- <span data-ttu-id="0a6cc-108">Administrador de cobrança</span><span class="sxs-lookup"><span data-stu-id="0a6cc-108">Billing admin</span></span>
- <span data-ttu-id="0a6cc-109">Administração global</span><span class="sxs-lookup"><span data-stu-id="0a6cc-109">Global admin</span></span>

<span data-ttu-id="0a6cc-110">Para obter uma exibição detalhada de item de linha de cada encargo em um ciclo de cobrança, baixe os arquivos de reconciliação do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-110">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="0a6cc-111">Os detalhes incluem encargos por assinaturas de cada cliente e eventos detalhados (como a adição de assentos a uma assinatura no meio do período).</span><span class="sxs-lookup"><span data-stu-id="0a6cc-111">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="0a6cc-112">Problemas de formatação</span><span class="sxs-lookup"><span data-stu-id="0a6cc-112">Formatting issues</span></span>

<span data-ttu-id="0a6cc-113">Ocasionalmente, seu arquivo reconhecimento pode ter problemas de formatação.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-113">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="0a6cc-114">(Isso pode acontecer, por exemplo, se a localidade EN-US não for usada.) Siga as etapas abaixo para corrigir esses problemas.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-114">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="0a6cc-115">Abra o arquivo. csv no Excel e selecione a primeira coluna.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-115">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="0a6cc-116">Na faixa de opções, selecione <strong>dados</strong>e, em seguida, selecione <strong>texto para colunas</strong>.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-116">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="0a6cc-117">No assistente converter texto em colunas, selecione <strong>tipo de arquivo delimitado</strong>e, em seguida, selecione <strong>Avançar</strong>.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-117">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="0a6cc-118">No campo delimitadores, selecione <strong>vírgula</strong>.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-118">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="0a6cc-119">Se a <strong>guia</strong> já estiver selecionada, você poderá deixá-la.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-119">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="0a6cc-120">Selecione <strong>Avançar</strong>.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-120">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="0a6cc-121">No campo formato de dados da coluna, selecione <strong>Data: MDY</strong>e, em seguida, selecione <strong>Avançar</strong>.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-121">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="0a6cc-122">No campo formato de dados da coluna, selecione <strong>texto</strong> para todas as colunas de valor e, em seguida, selecione <strong>concluir</strong>.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-122">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a name="downloading-a-large-recon-file"></a><span data-ttu-id="0a6cc-123">Baixando um arquivo reconhecimento grande</span><span class="sxs-lookup"><span data-stu-id="0a6cc-123">Downloading a large recon file</span></span>

<span data-ttu-id="0a6cc-124">Os arquivos reconhecimento podem crescer muito e, às vezes, são difíceis de baixar.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-124">Recon files can grow very large and are sometimes difficult to download.</span></span> <span data-ttu-id="0a6cc-125">Para obter um script do PowerShell para ajudar a baixar arquivos grandes do reconhecimento, consulte [obter itens de linha da fatura](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="0a6cc-125">For a PowerShell script to help download large recon files, see [Get invoice line items](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="0a6cc-126">Discriminar por parceiro</span><span class="sxs-lookup"><span data-stu-id="0a6cc-126">Itemize by partner</span></span>


<span data-ttu-id="0a6cc-127">Os parceiros no modelo indireto podem usar esses campos adicionais nos arquivos de reconciliação baseados em uso e em licença para discriminar por revendedor.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-127">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="0a6cc-128">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="0a6cc-128">MPN ID</span></span></th>
<th><span data-ttu-id="0a6cc-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a6cc-129">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="0a6cc-130">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="0a6cc-130">MPN ID</span></span></td>
<td><p><span data-ttu-id="0a6cc-131">A ID do Microsoft Partner Network (MPN) do parceiro CSP (direta ou indireta).</span><span class="sxs-lookup"><span data-stu-id="0a6cc-131">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0a6cc-132">ID do MPN do revendedor</span><span class="sxs-lookup"><span data-stu-id="0a6cc-132">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="0a6cc-133">Só aparece em arquivos de reconciliação para parceiros no modelo indireto.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-133">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="0a6cc-134">A ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-134">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="0a6cc-135">Isso corresponde à ID de revendedor listada para a assinatura específica no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-135">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="0a6cc-136">eTo exibir ou atualizar o revendedor, no menu do centro de parceiros, selecione <strong>clientes</strong>e, em seguida, escolha o cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-136">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="0a6cc-137">No menu do cliente, selecione <strong>Assinaturas</strong>, escolha a assinatura na lista.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-137">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="0a6cc-138">Selecione <strong>Atualizar</strong> para alterar o <strong>Revendedor (ID do MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-138">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="0a6cc-139">Se um parceiro CSP vendeu a assinatura diretamente para o cliente, sua ID do MPN estará listada duas vezes, como a ID do MPN e a ID do MPN do revendedor.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-139">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="0a6cc-140">Se um parceiro CSP tiver um revendedor sem ID MPN, esse valor será definido como a ID de MPN do parceiro em vez disso.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-140">If a CSP partner has a reseller with no MPN ID, this value is set to the partner's MPN ID instead.</span></span></p>
<p><span data-ttu-id="0a6cc-141">Se o parceiro CSP remover uma ID de revendedor, esse valor será definido como -1.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-141">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a><span data-ttu-id="0a6cc-142">Campos de arquivo com base em licença</span><span class="sxs-lookup"><span data-stu-id="0a6cc-142">License-based file fields</span></span>


<span data-ttu-id="0a6cc-143">Para reconciliar seus encargos com os pedidos de seu cliente, compare o campo Syndication\_Partner\_Subscription\_Number do arquivo de reconciliação com a ID de Assinatura do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-143">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="0a6cc-144"><strong>Pilha</strong></span><span class="sxs-lookup"><span data-stu-id="0a6cc-144"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="0a6cc-145"><strong>Descrição</strong></span><span class="sxs-lookup"><span data-stu-id="0a6cc-145"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="0a6cc-146"><strong>Valor de exemplo</strong></span><span class="sxs-lookup"><span data-stu-id="0a6cc-146"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0a6cc-147">PartnerID</span><span class="sxs-lookup"><span data-stu-id="0a6cc-147">PartnerId</span></span></td>
<td><p><span data-ttu-id="0a6cc-148">Identificador exclusivo de uma entidade de cobrança específica, em formato GUID.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-148">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="0a6cc-149">Não é necessário para reconciliação, mas pode ser uma informação útil.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-149">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="0a6cc-150">O mesmo em todas as linhas.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-150">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="0a6cc-151">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="0a6cc-151">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0a6cc-152">CustomerID</span><span class="sxs-lookup"><span data-stu-id="0a6cc-152">CustomerID</span></span></td>
<td><p><span data-ttu-id="0a6cc-153">ID exclusiva da Microsoft, no formato GUID, usada para identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-153">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="0a6cc-154">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="0a6cc-154">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0a6cc-155">OrderID</span><span class="sxs-lookup"><span data-stu-id="0a6cc-155">OrderID</span></span></td>
<td><p><span data-ttu-id="0a6cc-156">Identificador exclusivo para um pedido na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-156">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="0a6cc-157">Pode ser útil para identificar o pedido ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-157">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="0a6cc-158">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="0a6cc-158">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0a6cc-159">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="0a6cc-159">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="0a6cc-160">Identificador exclusivo de uma assinatura na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-160">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="0a6cc-161">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-161">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="0a6cc-162">Esse não é o mesmo que o ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-162">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="0a6cc-163">Consulte Número_Assinatura_Parceiro_Sindicalização.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-163">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="0a6cc-164">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="0a6cc-164">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0a6cc-165">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="0a6cc-165">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="0a6cc-166">Identificador exclusivo para assinaturas.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-166">Unique identifier for subscriptions.</span></span> <span data-ttu-id="0a6cc-167">Target: Um cliente pode ter várias assinaturas para o mesmo plano, portanto, isso é importante para análise de arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-167">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="0a6cc-168">Esse campo é mapeado para a ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-168">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="0a6cc-169">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="0a6cc-169">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0a6cc-170">OfferID</span><span class="sxs-lookup"><span data-stu-id="0a6cc-170">OfferID</span></span></td>
<td><p><span data-ttu-id="0a6cc-171">ID exclusivo da oferta.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-171">Unique offer ID.</span></span> <span data-ttu-id="0a6cc-172">ID padrão da oferta de acordo com a lista de preços.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-172">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="0a6cc-173"><b>Observação</b>: esse valor não coincide com a ID de oferta da lista de preços.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-173"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="0a6cc-174">Veja DurableOfferID abaixo.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-174">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="0a6cc-175">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="0a6cc-175">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0a6cc-176">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="0a6cc-176">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="0a6cc-177">ID exclusiva da oferta durável, conforme definido na tabela de preços.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-177">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="0a6cc-178"><b>Observação</b>: esse valor corresponde à ID de oferta da lista de preços.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-178"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="0a6cc-179">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="0a6cc-179">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0a6cc-180">OfferName</span><span class="sxs-lookup"><span data-stu-id="0a6cc-180">OfferName</span></span></td>
<td><p><span data-ttu-id="0a6cc-181">O nome da oferta de serviço comprada pelo cliente, conforme definido na tabela de preços.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-181">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="0a6cc-182">Microsoft Office 365 (plano E3)</span><span class="sxs-lookup"><span data-stu-id="0a6cc-182">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0a6cc-183">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="0a6cc-183">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="0a6cc-184">A data de início da assinatura, definida como um dia após o pedido ser enviado.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-184">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="0a6cc-185">Verificando a data de início da assinatura em conjunto com a data de término, você pode determinar se o cliente está dentro do primeiro ano da assinatura ou se a assinatura foi renovada para o ano seguinte.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-185">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="0a6cc-186">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-186">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="0a6cc-187">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="0a6cc-187">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0a6cc-188">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="0a6cc-188">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="0a6cc-189">A data do término da assinatura: 12 meses + x dias após a data de início (para se alinhar com a data de cobrança do parceiro) ou 12 meses a partir da data de renovação.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-189">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="0a6cc-190">Na renovação, os preços são atualizados com a tabela de preços atual.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-190">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="0a6cc-191">Um comunicado ao cliente pode ser necessário antes da renovação automática.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-191">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="0a6cc-192">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-192">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="0a6cc-193">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="0a6cc-193">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0a6cc-194">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="0a6cc-194">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="0a6cc-195">Dia de início dos encargos.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-195">Start day of the charges.</span></span></p>
<p><span data-ttu-id="0a6cc-196">Quando o cliente muda o número de assentos, esse número é usado para calcular os encargos por dia (pro-rata).</span><span class="sxs-lookup"><span data-stu-id="0a6cc-196">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="0a6cc-197">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-197">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="0a6cc-198">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="0a6cc-198">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0a6cc-199">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="0a6cc-199">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="0a6cc-200">Dia do término dos encargos.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-200">End day of the charges.</span></span></p>
<p><span data-ttu-id="0a6cc-201">Quando o cliente muda o número de assentos, esse número é usado para calcular os encargos por dia (pro-rata).</span><span class="sxs-lookup"><span data-stu-id="0a6cc-201">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="0a6cc-202">A hora é sempre o fim do dia, 23:59.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-202">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="0a6cc-203">28/2/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="0a6cc-203">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0a6cc-204">ChargeType</span><span class="sxs-lookup"><span data-stu-id="0a6cc-204">ChargeType</span></span></td>
<td><p><span data-ttu-id="0a6cc-205">O tipo de encargo ou ajuste.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-205">The type of charge or adjustment.</span></span> <span data-ttu-id="0a6cc-206">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="0a6cc-206">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="0a6cc-207">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="0a6cc-207">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0a6cc-208">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="0a6cc-208">UnitPrice</span></span></td>
<td><p><span data-ttu-id="0a6cc-209">Preço por estação, conforme publicado na lista de preços no momento da compra.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-209">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="0a6cc-210">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-210">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="0a6cc-211">6.82</span><span class="sxs-lookup"><span data-stu-id="0a6cc-211">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0a6cc-212">Quantity</span><span class="sxs-lookup"><span data-stu-id="0a6cc-212">Quantity</span></span></td>
<td><p><span data-ttu-id="0a6cc-213">Número de assentos.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-213">Number of seats.</span></span> <span data-ttu-id="0a6cc-214">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-214">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="0a6cc-215">2</span><span class="sxs-lookup"><span data-stu-id="0a6cc-215">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0a6cc-216">Valor</span><span class="sxs-lookup"><span data-stu-id="0a6cc-216">Amount</span></span></td>
<td><p><span data-ttu-id="0a6cc-217">Preço total por quantidade.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-217">Total of price for quantity.</span></span> <span data-ttu-id="0a6cc-218">Útil para verificar se o cálculo do valor coincide com a forma como você calcula isso para seus clientes.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-218">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="0a6cc-219">13.32</span><span class="sxs-lookup"><span data-stu-id="0a6cc-219">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0a6cc-220">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="0a6cc-220">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="0a6cc-221">Valor de desconto aplicado a esses encargos.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-221">Amount of discount applied to these charges.</span></span> <span data-ttu-id="0a6cc-222">As licenças de produto incluídas com uma competência ou mapas ou novas assinaturas qualificadas para um incentivo também conterão um valor de desconto nesta coluna.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-222">Product Licenses included with a competency or MAPS or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="0a6cc-223">2.32</span><span class="sxs-lookup"><span data-stu-id="0a6cc-223">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0a6cc-224">Subtotal</span><span class="sxs-lookup"><span data-stu-id="0a6cc-224">Subtotal</span></span></td>
<td><p><span data-ttu-id="0a6cc-225">Total sem imposto.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-225">Total before tax.</span></span> <span data-ttu-id="0a6cc-226">Verifica se seu subtotal corresponde ao total esperado, em caso de desconto.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-226">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="0a6cc-227">11</span><span class="sxs-lookup"><span data-stu-id="0a6cc-227">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0a6cc-228">Tax</span><span class="sxs-lookup"><span data-stu-id="0a6cc-228">Tax</span></span></td>
<td><p><span data-ttu-id="0a6cc-229">Valor do imposto, com base nas regras&#39;de imposto de s do mercado e em circunstâncias específicas.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-229">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="0a6cc-230">0</span><span class="sxs-lookup"><span data-stu-id="0a6cc-230">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0a6cc-231">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="0a6cc-231">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="0a6cc-232">Total com imposto.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-232">Total after tax.</span></span> <span data-ttu-id="0a6cc-233">Verifica se o imposto é cobrado na fatura.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-233">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="0a6cc-234">11</span><span class="sxs-lookup"><span data-stu-id="0a6cc-234">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0a6cc-235">Currency</span><span class="sxs-lookup"><span data-stu-id="0a6cc-235">Currency</span></span></td>
<td><p><span data-ttu-id="0a6cc-236">Tipo de moeda.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-236">Currency type.</span></span> <span data-ttu-id="0a6cc-237">Cada entidade de cobrança tem somente uma moeda.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-237">Each billing entity has only one currency.</span></span> <span data-ttu-id="0a6cc-238">Verifique se isso coincide com a primeira fatura e faça o mesmo após grandes atualizações na plataforma de cobrança.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-238">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="0a6cc-239">EUR</span><span class="sxs-lookup"><span data-stu-id="0a6cc-239">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0a6cc-240">CustomerName</span><span class="sxs-lookup"><span data-stu-id="0a6cc-240">CustomerName</span></span></td>
<td><p><span data-ttu-id="0a6cc-241">Nome&#39;da organização do cliente como relatado no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-241">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="0a6cc-242">Isso é muito importante para reconciliar a fatura com as informações de seu sistema.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-242">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="0a6cc-243">Cliente de teste A</span><span class="sxs-lookup"><span data-stu-id="0a6cc-243">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0a6cc-244">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="0a6cc-244">MPNID</span></span></td>
<td><p><span data-ttu-id="0a6cc-245">ID do MPN do parceiro CSP</span><span class="sxs-lookup"><span data-stu-id="0a6cc-245">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="0a6cc-246">4390934</span><span class="sxs-lookup"><span data-stu-id="0a6cc-246">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0a6cc-247">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="0a6cc-247">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="0a6cc-248">ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-248">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="0a6cc-249">Consulte <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Discriminar por parceiro</a>.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-249">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="0a6cc-250">4390934</span><span class="sxs-lookup"><span data-stu-id="0a6cc-250">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0a6cc-251">DomainName</span><span class="sxs-lookup"><span data-stu-id="0a6cc-251">DomainName</span></span></td>
<td><p><span data-ttu-id="0a6cc-252">Nome&#39;de domínio do cliente, usado para ajudar a identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-252">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="0a6cc-253">Isso não deve ser usado para identificar exclusivamente o cliente, pois o cliente/parceiro pode atualizar o domínio intuitivo/padrão por meio do portal do O365.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-253">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="0a6cc-254">Este campo pode aparecer em branco até o segundo ciclo de cobrança.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-254">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="0a6cc-255">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="0a6cc-255">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0a6cc-256">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="0a6cc-256">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="0a6cc-257">Apelido da Inscrição.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-257">Subscription nickname.</span></span> <span data-ttu-id="0a6cc-258">Se nenhum apelido for especificado, o Partner Center usa o OfferName.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-258">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="0a6cc-259">PROJETO ONLINE</span><span class="sxs-lookup"><span data-stu-id="0a6cc-259">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0a6cc-260">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="0a6cc-260">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="0a6cc-261">O nome da oferta de serviço comprada pelo cliente, conforme definido na tabela de preços.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-261">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="0a6cc-262">(Este é um campo idêntico ao nome da oferta).</span><span class="sxs-lookup"><span data-stu-id="0a6cc-262">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="0a6cc-263">PROJETO ONLINE PREMIUM SEM PROJETO CLIENTE</span><span class="sxs-lookup"><span data-stu-id="0a6cc-263">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="0a6cc-264">Campos de arquivo com base no uso</span><span class="sxs-lookup"><span data-stu-id="0a6cc-264">Usage-based file fields</span></span>


<span data-ttu-id="0a6cc-265">Para reconciliar seus encargos com o uso de seu cliente, compare ResellerID/ResellerName/ResellerBillableAccount do arquivo de reconciliação com o nome do cliente e a ID da assinatura do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-265">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="0a6cc-266">Os campos a seguir explicam quais serviços foram usados e a taxa.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-266">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="0a6cc-267"><strong>Pilha</strong></span><span class="sxs-lookup"><span data-stu-id="0a6cc-267"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="0a6cc-268"><strong>Descrição</strong></span><span class="sxs-lookup"><span data-stu-id="0a6cc-268"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="0a6cc-269"><strong>Valor de exemplo</strong></span><span class="sxs-lookup"><span data-stu-id="0a6cc-269"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0a6cc-270">PartnerID</span><span class="sxs-lookup"><span data-stu-id="0a6cc-270">PartnerID</span></span></td>
<td><p><span data-ttu-id="0a6cc-271">ID do parceiro, no formato GUID.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-271">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="0a6cc-272">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="0a6cc-272">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0a6cc-273">PartnerName</span><span class="sxs-lookup"><span data-stu-id="0a6cc-273">PartnerName</span></span></td>
<td><p><span data-ttu-id="0a6cc-274">Nome do parceiro.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-274">Partner Name.</span></span></p></td>
<td><span data-ttu-id="0a6cc-275">Acme incorporado</span><span class="sxs-lookup"><span data-stu-id="0a6cc-275">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0a6cc-276">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="0a6cc-276">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="0a6cc-277">ID da conta do parceiro.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-277">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="0a6cc-278">1010578050</span><span class="sxs-lookup"><span data-stu-id="0a6cc-278">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0a6cc-279">CustomerName</span><span class="sxs-lookup"><span data-stu-id="0a6cc-279">CustomerName</span></span></td>
<td><p><span data-ttu-id="0a6cc-280">Nome&#39;da organização do cliente como relatado no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-280">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="0a6cc-281">Isso é muito importante para reconciliar a fatura com as informações de seu sistema.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-281">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="0a6cc-282">Cliente de teste A</span><span class="sxs-lookup"><span data-stu-id="0a6cc-282">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0a6cc-283">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="0a6cc-283">MPNID</span></span></td>
<td><p><span data-ttu-id="0a6cc-284">ID do MPN do parceiro CSP.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-284">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="0a6cc-285">4390934</span><span class="sxs-lookup"><span data-stu-id="0a6cc-285">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0a6cc-286">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="0a6cc-286">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="0a6cc-287">ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-287">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="0a6cc-288">Consulte <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Discriminar por parceiro</a>.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-288">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="0a6cc-289">4390934</span><span class="sxs-lookup"><span data-stu-id="0a6cc-289">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0a6cc-290">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="0a6cc-290">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="0a6cc-291">Número da fatura na qual a transação especificada é exibida.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-291">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="0a6cc-292">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="0a6cc-292">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0a6cc-293">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="0a6cc-293">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="0a6cc-294">Data de início do ciclo de cobrança exceto quando apresentadas as datas de dados de uso latentes anteriormente não cobradas (do ciclo de cobrança anterior).</span><span class="sxs-lookup"><span data-stu-id="0a6cc-294">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="0a6cc-295">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-295">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="0a6cc-296">1/2/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="0a6cc-296">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0a6cc-297">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="0a6cc-297">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="0a6cc-298">Data de término do ciclo de cobrança exceto quando apresentadas as datas de dados de uso latentes anteriormente não cobradas (do ciclo de cobrança anterior).</span><span class="sxs-lookup"><span data-stu-id="0a6cc-298">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="0a6cc-299">A hora é sempre o fim do dia, 23:59.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-299">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="0a6cc-300">28/2/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="0a6cc-300">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0a6cc-301">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="0a6cc-301">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="0a6cc-302">Identificador exclusivo de uma assinatura na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-302">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="0a6cc-303">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-303">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="0a6cc-304">Esse não é o mesmo que o ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-304">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="0a6cc-305">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="0a6cc-305">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0a6cc-306">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="0a6cc-306">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="0a6cc-307">Apelido da oferta do serviço.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-307">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="0a6cc-308">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="0a6cc-308">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0a6cc-309">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="0a6cc-309">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="0a6cc-310">Linha de negócios da oferta do serviço</span><span class="sxs-lookup"><span data-stu-id="0a6cc-310">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="0a6cc-311">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="0a6cc-311">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0a6cc-312">OrderID</span><span class="sxs-lookup"><span data-stu-id="0a6cc-312">OrderID</span></span></td>
<td><p><span data-ttu-id="0a6cc-313">Identificador exclusivo para um pedido na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-313">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="0a6cc-314">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-314">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="0a6cc-315">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="0a6cc-315">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0a6cc-316">ServiceName</span><span class="sxs-lookup"><span data-stu-id="0a6cc-316">ServiceName</span></span></td>
<td><p><span data-ttu-id="0a6cc-317">O nome do serviço do Azure em questão.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-317">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="0a6cc-318">MÁQUINAS VIRTUAIS</span><span class="sxs-lookup"><span data-stu-id="0a6cc-318">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0a6cc-319">ServiceType</span><span class="sxs-lookup"><span data-stu-id="0a6cc-319">ServiceType</span></span></td>
<td><p><span data-ttu-id="0a6cc-320">O tipo específico de serviço do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-320">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="0a6cc-321">Barramento de serviço-individual ou pacote</span><span class="sxs-lookup"><span data-stu-id="0a6cc-321">Service Bus - Individual or Pack</span></span></li>
<li><span data-ttu-id="0a6cc-322">Banco de dados do SQL Azure-Business ou Web Edition</span><span class="sxs-lookup"><span data-stu-id="0a6cc-322">SQL Azure database - Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0a6cc-323">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="0a6cc-323">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="0a6cc-324">Identificador exclusivo específico de toda a estrutura de serviço de dados e preço.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-324">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="0a6cc-325">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="0a6cc-325">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0a6cc-326">Nome do recurso</span><span class="sxs-lookup"><span data-stu-id="0a6cc-326">Resource Name</span></span></td>
<td><p><span data-ttu-id="0a6cc-327">O nome do recurso do Azure.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-327">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="0a6cc-328">Dados de entrada transferidos (GB)</span><span class="sxs-lookup"><span data-stu-id="0a6cc-328">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="0a6cc-329">Dados de saída transferidos (GB)</span><span class="sxs-lookup"><span data-stu-id="0a6cc-329">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0a6cc-330">Region</span><span class="sxs-lookup"><span data-stu-id="0a6cc-330">Region</span></span></td>
<td><p><span data-ttu-id="0a6cc-331">A região a qual o uso se aplica.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-331">The region the usage applies to.</span></span> <span data-ttu-id="0a6cc-332">Usado principalmente para atribuir as taxas de transferências de dados, já que as taxas variam de acordo com a região.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-332">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="0a6cc-333">Pacífico Asiático, Europa, América Latina e América do Norte</span><span class="sxs-lookup"><span data-stu-id="0a6cc-333">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0a6cc-334">SKU</span><span class="sxs-lookup"><span data-stu-id="0a6cc-334">SKU</span></span></td>
<td><p><span data-ttu-id="0a6cc-335">Identificador exclusivo MSFT da oferta</span><span class="sxs-lookup"><span data-stu-id="0a6cc-335">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="0a6cc-336">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="0a6cc-336">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="0a6cc-337">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="0a6cc-337">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="0a6cc-338">Uma ID e a quantidade para discriminar as taxas diferentes de um serviço ou recurso em um determinado período de cobrança.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-338">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="0a6cc-339">Para a classificação em camadas do Azure, pode haver uma taxa para uma determinada quantidade de unidades faturáveis e uma taxa diferente depois disso.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-339">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="0a6cc-340">1</span><span class="sxs-lookup"><span data-stu-id="0a6cc-340">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0a6cc-341">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="0a6cc-341">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="0a6cc-342">A quantidade de serviço consumida (horas, GB etc.) durante o período de relatório.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-342">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="0a6cc-343">Também inclui qualquer uso não cobrado de períodos de relatório anteriores.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-343">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="0a6cc-344">11</span><span class="sxs-lookup"><span data-stu-id="0a6cc-344">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0a6cc-345">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="0a6cc-345">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="0a6cc-346">Unidades incluídas como parte da oferta.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-346">Units included as part of the offer.</span></span> <span data-ttu-id="0a6cc-347">Normalmente não está presente no CSP.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-347">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="0a6cc-348">0</span><span class="sxs-lookup"><span data-stu-id="0a6cc-348">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="0a6cc-349">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="0a6cc-349">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="0a6cc-350">Unidades não incluídas como parte da oferta devem ser pagas pelo parceiro.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-350">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="0a6cc-351">Igual a ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-351">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="0a6cc-352">11</span><span class="sxs-lookup"><span data-stu-id="0a6cc-352">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0a6cc-353">ListPrice</span><span class="sxs-lookup"><span data-stu-id="0a6cc-353">ListPrice</span></span></td>
<td><p><span data-ttu-id="0a6cc-354">Preço da oferta em vigor na data de início da assinatura.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-354">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="0a6cc-355">U$ 0,0808</span><span class="sxs-lookup"><span data-stu-id="0a6cc-355">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0a6cc-356">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="0a6cc-356">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="0a6cc-357">ListPrist vezes OverageQuantity, arredondado para o centavo mais próximo.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-357">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="0a6cc-358">U$ 0,085</span><span class="sxs-lookup"><span data-stu-id="0a6cc-358">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0a6cc-359">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="0a6cc-359">TaxAmount</span></span></td>
<td><p><span data-ttu-id="0a6cc-360">Valor do imposto, com base nas regras&#39;de imposto de s do mercado e em circunstâncias específicas.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-360">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="0a6cc-361">U$ 0,08</span><span class="sxs-lookup"><span data-stu-id="0a6cc-361">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0a6cc-362">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="0a6cc-362">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="0a6cc-363">Total após imposto, quando o imposto é aplicável.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-363">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="0a6cc-364">U$ 0,93</span><span class="sxs-lookup"><span data-stu-id="0a6cc-364">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0a6cc-365">Currency</span><span class="sxs-lookup"><span data-stu-id="0a6cc-365">Currency</span></span></td>
<td><p><span data-ttu-id="0a6cc-366">Tipo de moeda.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-366">Currency type.</span></span> <span data-ttu-id="0a6cc-367">Cada entidade de cobrança tem somente uma moeda.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-367">Each billing entity has only one currency.</span></span> <span data-ttu-id="0a6cc-368">Verifique se isso coincide com a primeira fatura e faça o mesmo após grandes atualizações na plataforma de cobrança.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-368">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="0a6cc-369">EUR</span><span class="sxs-lookup"><span data-stu-id="0a6cc-369">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0a6cc-370">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="0a6cc-370">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="0a6cc-371">Preço por unidade sem imposto.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-371">Pretax price per unit.</span></span> <span data-ttu-id="0a6cc-372">Igual a PretaxCharges / OverageQuantity, arredondado para o centavo mais próximo.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-372">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="0a6cc-373">U$ 0,08</span><span class="sxs-lookup"><span data-stu-id="0a6cc-373">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0a6cc-374">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="0a6cc-374">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="0a6cc-375">Preço pós-imposto por unidade.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-375">Post tax price per unit.</span></span> <span data-ttu-id="0a6cc-376">Igual a PostTaxTotal / OverageQuantity, ou PretaxEffectiveRate + taxa de imposto por valor de unidade, arredondado para o centavo mais próximo.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-376">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="0a6cc-377">U$ 0,08</span><span class="sxs-lookup"><span data-stu-id="0a6cc-377">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0a6cc-378">ChargeType</span><span class="sxs-lookup"><span data-stu-id="0a6cc-378">ChargeType</span></span></td>
<td><p><span data-ttu-id="0a6cc-379">O tipo de encargo ou ajuste.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-379">The type of charge or adjustment.</span></span> <span data-ttu-id="0a6cc-380">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="0a6cc-380">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="0a6cc-381">Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></span><span class="sxs-lookup"><span data-stu-id="0a6cc-381">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0a6cc-382">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="0a6cc-382">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="0a6cc-383">ID exclusiva da conta na plataforma de cobrança da MSFT.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-383">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="0a6cc-384">1280018095</span><span class="sxs-lookup"><span data-stu-id="0a6cc-384">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0a6cc-385">UsageDate</span><span class="sxs-lookup"><span data-stu-id="0a6cc-385">UsageDate</span></span></td>
<td><p><span data-ttu-id="0a6cc-386">Data da implantação do serviço.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-386">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="0a6cc-387">1/2/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="0a6cc-387">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0a6cc-388">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="0a6cc-388">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="0a6cc-389">Essa coluna identifica a localização de um data center dentro da região para serviços onde isso é aplicável e preenchido.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-389">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="0a6cc-390">Leste da Ásia, Sudeste da Ásia, Norte da Europa, Europa Ocidental, Centro Norte e Centro Sul dos EUA</span><span class="sxs-lookup"><span data-stu-id="0a6cc-390">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0a6cc-391">MeteredService</span><span class="sxs-lookup"><span data-stu-id="0a6cc-391">MeteredService</span></span></td>
<td><p><span data-ttu-id="0a6cc-392">Essa coluna é utilizada para rastrear o serviço do Microsoft Azure individual que não pode ser identificado especificamente na coluna Nome do Serviço.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-392">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="0a6cc-393">Por exemplo, transferências de dados são relatadas como &quot;Microsoft Azure – Todos os Serviços&quot; na coluna Nome do Serviço.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-393">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="0a6cc-394">Essa coluna MeteredService indicará ao qual serviço específico o uso pertence.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-394">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="0a6cc-395">AccessControl, CDN, Computação, Banco de dados, ServiceBus, Armazenamento</span><span class="sxs-lookup"><span data-stu-id="0a6cc-395">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0a6cc-396">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="0a6cc-396">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="0a6cc-397">Um subcabeçalho que esclarece ainda mais o serviço Microsoft Azure individual além do nível fornecido pelo campo MeteredService.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-397">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="0a6cc-398">EXTERNO</span><span class="sxs-lookup"><span data-stu-id="0a6cc-398">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0a6cc-399">Projeto</span><span class="sxs-lookup"><span data-stu-id="0a6cc-399">Project</span></span></td>
<td><p><span data-ttu-id="0a6cc-400">Nome definido pelo cliente para a instância do serviço</span><span class="sxs-lookup"><span data-stu-id="0a6cc-400">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="0a6cc-401">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="0a6cc-401">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0a6cc-402">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="0a6cc-402">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="0a6cc-403">O número de conexões ServiceBus que foram provisionados e utilizados em um dia específico.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-403">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="0a6cc-404">Por exemplo: se você tivesse uma conexão provisionada individualmente durante um mês de 30 dias, a informação de serviço 1 lerá "1, 0 conexões/30 dias".</span><span class="sxs-lookup"><span data-stu-id="0a6cc-404">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days".</span></span> <span data-ttu-id="0a6cc-405">Se você tiver um pacote de 25 pacotes de conexões do ServiceBus provisionado e tiver utilizado 1 durante esse dia, sua instrução de uso diário para esse dia indicaria "25 conexões/30 dias-usado: 1, 0".</span><span class="sxs-lookup"><span data-stu-id="0a6cc-405">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days - Used: 1.000000".</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0a6cc-406">CustomerID</span><span class="sxs-lookup"><span data-stu-id="0a6cc-406">CustomerID</span></span></td>
<td><p><span data-ttu-id="0a6cc-407">ID exclusiva da Microsoft, no formato GUID, usada para identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-407">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="0a6cc-408">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="0a6cc-408">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0a6cc-409">DomainName</span><span class="sxs-lookup"><span data-stu-id="0a6cc-409">DomainName</span></span></td>
<td><p><span data-ttu-id="0a6cc-410">Nome&#39;de domínio do cliente, usado para ajudar a identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-410">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="0a6cc-411">Este campo pode aparecer em branco até o segundo ciclo de cobrança.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-411">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="0a6cc-412">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="0a6cc-412">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="0a6cc-413">Unidade</span><span class="sxs-lookup"><span data-stu-id="0a6cc-413">Unit</span></span></td>
<td><p><span data-ttu-id="0a6cc-414">A unidade do nome do recurso</span><span class="sxs-lookup"><span data-stu-id="0a6cc-414">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="0a6cc-415">GB ou HORAS</span><span class="sxs-lookup"><span data-stu-id="0a6cc-415">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="0a6cc-416">Campos de arquivo de uso único e recorrente</span><span class="sxs-lookup"><span data-stu-id="0a6cc-416">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="0a6cc-417">Column</span><span class="sxs-lookup"><span data-stu-id="0a6cc-417">Column</span></span></th>
<th><span data-ttu-id="0a6cc-418">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a6cc-418">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="0a6cc-419">PartnerID</span><span class="sxs-lookup"><span data-stu-id="0a6cc-419">PartnerId</span></span></td>
<td><p><span data-ttu-id="0a6cc-420">Identificador de locatário de Microsoft Azure Active Directory exclusivo para uma entidade de cobrança específica, no formato GUID.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-420">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="0a6cc-421">Não é necessário para reconciliação, mas pode ser uma informação útil.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-421">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="0a6cc-422">O mesmo em todas as linhas.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-422">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0a6cc-423">ID do cliente</span><span class="sxs-lookup"><span data-stu-id="0a6cc-423">Customer Id</span></span></td>
<td><p><span data-ttu-id="0a6cc-424">ID de locatário de Microsoft Azure Active Directory exclusiva, no formato GUID, usada para identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-424">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0a6cc-425">Nome do cliente</span><span class="sxs-lookup"><span data-stu-id="0a6cc-425">Customer Name</span></span></td>
<td><p><span data-ttu-id="0a6cc-426">Nome da organização do cliente como informado no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-426">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0a6cc-427">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="0a6cc-427">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="0a6cc-428">Nome de domínio do cliente, usado para ajudar a identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-428">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="0a6cc-429">Isso não deve ser usado para identificar exclusivamente o cliente, pois o cliente/parceiro pode atualizar o domínio intuitivo/padrão por meio do portal do O365.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-429">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="0a6cc-430">Este campo pode aparecer em branco até o segundo ciclo de cobrança.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-430">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0a6cc-431">País do cliente</span><span class="sxs-lookup"><span data-stu-id="0a6cc-431">Customer Country</span></span></td>
<td><p><span data-ttu-id="0a6cc-432">O país em que o cliente está localizado.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-432">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0a6cc-433">Número da fatura</span><span class="sxs-lookup"><span data-stu-id="0a6cc-433">Invoice number</span></span></td>
<td><p><span data-ttu-id="0a6cc-434">Número da fatura na qual a transação especificada é exibida.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-434">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0a6cc-435">MpnId</span><span class="sxs-lookup"><span data-stu-id="0a6cc-435">MpnId</span></span></td>
<td><p><span data-ttu-id="0a6cc-436">ID do MPN do parceiro CSP.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-436">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0a6cc-437">MpnId do revendedor</span><span class="sxs-lookup"><span data-stu-id="0a6cc-437">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="0a6cc-438">ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-438">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0a6cc-439">ID do Pedido</span><span class="sxs-lookup"><span data-stu-id="0a6cc-439">Order ID</span></span></td>
<td><p><span data-ttu-id="0a6cc-440">Identificador exclusivo de um pedido na plataforma Microsoft Commerce.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-440">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="0a6cc-441">Pode ser útil para identificar o pedido ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-441">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0a6cc-442">Data do pedido</span><span class="sxs-lookup"><span data-stu-id="0a6cc-442">Order date</span></span></td>
<td><p><span data-ttu-id="0a6cc-443">A data em que o pedido foi feito.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-443">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0a6cc-444">ProductId</span><span class="sxs-lookup"><span data-stu-id="0a6cc-444">ProductId</span></span></td>
<td><p><span data-ttu-id="0a6cc-445">A ID do produto.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-445">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0a6cc-446">SkuId</span><span class="sxs-lookup"><span data-stu-id="0a6cc-446">SkuId</span></span></td>
<td><p><span data-ttu-id="0a6cc-447">A ID de uma SKU em particular.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-447">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0a6cc-448">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="0a6cc-448">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="0a6cc-449">A ID de uma Disponibilidade em particular.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-449">The ID for a particular Availability.</span></span> <span data-ttu-id="0a6cc-450">"Disponibilidade" refere-se a uma SKU específica que está ou não disponível para compra de determinado país, moeda, segmento do setor, etc.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-450">“Availability" refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0a6cc-451">Nome do SKU</span><span class="sxs-lookup"><span data-stu-id="0a6cc-451">SKU Name</span></span></td>
<td><p><span data-ttu-id="0a6cc-452">O título de uma SKU em particular.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-452">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0a6cc-453">Nome do produto</span><span class="sxs-lookup"><span data-stu-id="0a6cc-453">Product name</span></span></td>
<td><p><span data-ttu-id="0a6cc-454">O nome do produto.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-454">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0a6cc-455">PublisherName</span><span class="sxs-lookup"><span data-stu-id="0a6cc-455">PublisherName</span></span></td>
<td><p><span data-ttu-id="0a6cc-456">O nome do editor do produto.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-456">The name of the product's publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0a6cc-457">PublisherID</span><span class="sxs-lookup"><span data-stu-id="0a6cc-457">PublisherID</span></span></td>
<td><p><span data-ttu-id="0a6cc-458">ID exclusiva para este Publicador.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-458">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0a6cc-459">Descrição da assinatura</span><span class="sxs-lookup"><span data-stu-id="0a6cc-459">Subscription Description</span></span></td>
<td><p><span data-ttu-id="0a6cc-460">Nome amigável de uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-460">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0a6cc-461">ID da assinatura</span><span class="sxs-lookup"><span data-stu-id="0a6cc-461">Subscription ID</span></span></td>
<td><p><span data-ttu-id="0a6cc-462">Identificador exclusivo de uma assinatura na plataforma Microsoft Commerce.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-462">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="0a6cc-463">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-463">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="0a6cc-464">Esse não é o mesmo que o ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-464">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0a6cc-465">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="0a6cc-465">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="0a6cc-466">Dia de início dos encargos.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-466">Start day of the charges.</span></span> <span data-ttu-id="0a6cc-467">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-467">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0a6cc-468">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="0a6cc-468">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="0a6cc-469">Dia do término dos encargos.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-469">End day of the charges.</span></span> <span data-ttu-id="0a6cc-470">A hora é sempre o fim do dia, 23:59.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-470">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0a6cc-471">Termo e Billingcycle</span><span class="sxs-lookup"><span data-stu-id="0a6cc-471">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="0a6cc-472">O tamanho do termo e o ciclo de cobrança da compra.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-472">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="0a6cc-473">Por exemplo, "1 ano, mensalmente."</span><span class="sxs-lookup"><span data-stu-id="0a6cc-473">For example, “1 Year, Monthly."</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0a6cc-474">Tipo de Cobrança</span><span class="sxs-lookup"><span data-stu-id="0a6cc-474">Charge Type</span></span></td>
<td><p><span data-ttu-id="0a6cc-475">O tipo de encargo ou ajuste.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-475">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0a6cc-476">Preço unitário</span><span class="sxs-lookup"><span data-stu-id="0a6cc-476">Unit Price</span></span></td>
<td><p><span data-ttu-id="0a6cc-477">O preço como publicado na tabela de preços no momento da compra.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-477">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="0a6cc-478">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-478">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0a6cc-479">Preço unitário efetivo</span><span class="sxs-lookup"><span data-stu-id="0a6cc-479">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="0a6cc-480">O preço unitário após os ajustes terem sido feitos.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-480">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0a6cc-481">Quantity</span><span class="sxs-lookup"><span data-stu-id="0a6cc-481">Quantity</span></span></td>
<td><p><span data-ttu-id="0a6cc-482">Número de unidades.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-482">Number of units.</span></span> <span data-ttu-id="0a6cc-483">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-483">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0a6cc-484">Tipo de unidade</span><span class="sxs-lookup"><span data-stu-id="0a6cc-484">Unit type</span></span></td>
<td><p><span data-ttu-id="0a6cc-485">O tipo de unidade que está sendo adquirida.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-485">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0a6cc-486">PriceAdjustmentDescription</span><span class="sxs-lookup"><span data-stu-id="0a6cc-486">PriceAdjustmentDescription</span></span></td>
<td><p><span data-ttu-id="0a6cc-487">Uma explicação de qualquer desconto aplicável.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-487">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0a6cc-488">Subtotal</span><span class="sxs-lookup"><span data-stu-id="0a6cc-488">Sub Total</span></span></td>
<td><p><span data-ttu-id="0a6cc-489">Total sem imposto.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-489">Total before tax.</span></span> <span data-ttu-id="0a6cc-490">Verifica se seu subtotal corresponde ao total esperado, em caso de desconto.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-490">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0a6cc-491">Total do imposto</span><span class="sxs-lookup"><span data-stu-id="0a6cc-491">Tax Total</span></span></td>
<td><p><span data-ttu-id="0a6cc-492">Valor do imposto cobrado, com base nas regras fiscais do mercado e em circunstâncias específicas.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-492">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0a6cc-493">Total</span><span class="sxs-lookup"><span data-stu-id="0a6cc-493">Total</span></span></td>
<td><p><span data-ttu-id="0a6cc-494">Total com imposto.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-494">Total after tax.</span></span> <span data-ttu-id="0a6cc-495">Verifica se o imposto é cobrado na fatura.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-495">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0a6cc-496">Currency</span><span class="sxs-lookup"><span data-stu-id="0a6cc-496">Currency</span></span></td>
<td><p><span data-ttu-id="0a6cc-497">Tipo de moeda.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-497">Currency type.</span></span> <span data-ttu-id="0a6cc-498">Cada entidade de cobrança tem somente uma moeda.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-498">Each billing entity has only one currency.</span></span> <span data-ttu-id="0a6cc-499">Verifique se isso coincide com a primeira fatura e faça o mesmo após grandes atualizações na plataforma de cobrança.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-499">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0a6cc-500">Uma alternateid</span><span class="sxs-lookup"><span data-stu-id="0a6cc-500">AlternateID</span></span></td>
<td><p><span data-ttu-id="0a6cc-501">Um identificador alternativo para uma ID de pedido.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-501">An alternate identifier to an order ID.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0a6cc-502">BillingFrequency</span><span class="sxs-lookup"><span data-stu-id="0a6cc-502">BillingFrequency</span></span></td>
<td><p> <span data-ttu-id="0a6cc-503">Exibe mensalmente quando a cobrança mensal está habilitada.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-503">Displays monthly when monthly billing is enabled.</span></span> <span data-ttu-id="0a6cc-504">Caso contrário, em branco.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-504">Otherwise blank.</span></span> </p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0a6cc-505">BillableQuantity</span><span class="sxs-lookup"><span data-stu-id="0a6cc-505">BillableQuantity</span></span></td>
<td><p> <span data-ttu-id="0a6cc-506">Representa o total de unidades adquiridas ou consumidas.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-506">Represents the total units purchased or consumed.</span></span> </p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0a6cc-507">pricingCurrency</span><span class="sxs-lookup"><span data-stu-id="0a6cc-507">PricingCurrency</span></span></td>
<td><p> <span data-ttu-id="0a6cc-508">Lista o preço do recurso ou oferta</span><span class="sxs-lookup"><span data-stu-id="0a6cc-508">Lists the price for resource or offer</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0a6cc-509">PCToBCExchangeRate</span><span class="sxs-lookup"><span data-stu-id="0a6cc-509">PCToBCExchangeRate</span></span> </td>
<td><p> <span data-ttu-id="0a6cc-510">Taxa de câmbio aplicada para moeda de preço para a moeda de cobrança (clientes)</span><span class="sxs-lookup"><span data-stu-id="0a6cc-510">Exchange rate applied for pricing currency to (customers) billing currency</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0a6cc-511">PCToBCExchangeRateDate</span><span class="sxs-lookup"><span data-stu-id="0a6cc-511">PCToBCExchangeRateDate</span></span> </td>
<td><p> <span data-ttu-id="0a6cc-512">Data em que a moeda de preço para a taxa de câmbio da moeda de cobrança é determinada.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-512">Date at which pricing currency to billing currency exchange rate is determined.</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0a6cc-513">MeterDescription</span><span class="sxs-lookup"><span data-stu-id="0a6cc-513">MeterDescription</span></span> </td>
<td><p> <span data-ttu-id="0a6cc-514">Descrição do medidor para item de linha de consumo</span><span class="sxs-lookup"><span data-stu-id="0a6cc-514">Meter description for consumption line item</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="0a6cc-515">Campos de arquivo de uso com classificação diária</span><span class="sxs-lookup"><span data-stu-id="0a6cc-515">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="0a6cc-516">Column</span><span class="sxs-lookup"><span data-stu-id="0a6cc-516">Column</span></span></th>
<th><span data-ttu-id="0a6cc-517">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a6cc-517">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="0a6cc-518">PartnerID</span><span class="sxs-lookup"><span data-stu-id="0a6cc-518">PartnerId</span></span></td>
<td><p><span data-ttu-id="0a6cc-519">ID do parceiro, no formato GUID.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-519">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0a6cc-520">PartnerName</span><span class="sxs-lookup"><span data-stu-id="0a6cc-520">PartnerName</span></span></td>
<td><p><span data-ttu-id="0a6cc-521">Nome do parceiro.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-521">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0a6cc-522">CustomerID</span><span class="sxs-lookup"><span data-stu-id="0a6cc-522">CustomerId</span></span></td>
<td><p><span data-ttu-id="0a6cc-523">ID exclusiva da Microsoft, no formato GUID, usada para identificar o cliente.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-523">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0a6cc-524">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="0a6cc-524">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="0a6cc-525">Nome da organização do cliente como informado no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-525">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="0a6cc-526">Isso é muito importante para reconciliar a fatura com as informações de seu sistema.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-526">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0a6cc-527">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="0a6cc-527">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="0a6cc-528">O nome de domínio do cliente.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-528">The customer's domain name.</span></span> <span data-ttu-id="0a6cc-529">Não disponível para a atividade atual.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-529">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0a6cc-530">País do cliente</span><span class="sxs-lookup"><span data-stu-id="0a6cc-530">Customer country</span></span></td>
<td><p><span data-ttu-id="0a6cc-531">O país em que o cliente está localizado.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-531">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0a6cc-532">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="0a6cc-532">MPNID</span></span></td>
<td><p><span data-ttu-id="0a6cc-533">ID do MPN do parceiro CSP.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-533">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0a6cc-534">MPNID do revendedor</span><span class="sxs-lookup"><span data-stu-id="0a6cc-534">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="0a6cc-535">ID do MPN do revendedor de registro da assinatura.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-535">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="0a6cc-536">Não disponível para a atividade atual.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-536">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0a6cc-537">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="0a6cc-537">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="0a6cc-538">Número da fatura na qual a transação especificada é exibida.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-538">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="0a6cc-539">Não disponível para a atividade atual.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-539">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0a6cc-540">ProductId</span><span class="sxs-lookup"><span data-stu-id="0a6cc-540">ProductId</span></span></td>
<td><p><span data-ttu-id="0a6cc-541">A ID do produto.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-541">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0a6cc-542">SkuId</span><span class="sxs-lookup"><span data-stu-id="0a6cc-542">SkuId</span></span></td>
<td><p><span data-ttu-id="0a6cc-543">A ID de uma SKU em particular.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-543">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0a6cc-544">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="0a6cc-544">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="0a6cc-545">A ID de uma Disponibilidade em particular.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-545">The ID for a particular Availability.</span></span> <span data-ttu-id="0a6cc-546">"Disponibilidade" refere-se a uma SKU específica que está ou não disponível para compra de determinado país, moeda, segmento do setor, etc.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-546">“Availability" refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0a6cc-547">Nome do SKU</span><span class="sxs-lookup"><span data-stu-id="0a6cc-547">SKU Name</span></span></td>
<td><p><span data-ttu-id="0a6cc-548">O título de uma SKU em particular.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-548">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0a6cc-549">PublisherName</span><span class="sxs-lookup"><span data-stu-id="0a6cc-549">PublisherName</span></span></td>
<td><p><span data-ttu-id="0a6cc-550">O nome do Publicador.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-550">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0a6cc-551">PublisherID</span><span class="sxs-lookup"><span data-stu-id="0a6cc-551">PublisherID</span></span></td>
<td><p><span data-ttu-id="0a6cc-552">A ID do Publicador, no formato GUID.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-552">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="0a6cc-553">Não disponível para a atividade atual.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-553">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0a6cc-554">Descrição da assinatura</span><span class="sxs-lookup"><span data-stu-id="0a6cc-554">Subscription Description</span></span></td>
<td><p><span data-ttu-id="0a6cc-555">O nome da oferta de serviço comprada pelo cliente, conforme definido na tabela de preços.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-555">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="0a6cc-556">(Este é um campo idêntico ao nome da oferta).</span><span class="sxs-lookup"><span data-stu-id="0a6cc-556">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0a6cc-557">ID da assinatura</span><span class="sxs-lookup"><span data-stu-id="0a6cc-557">Subscription ID</span></span></td>
<td><p><span data-ttu-id="0a6cc-558">Identificador exclusivo de uma assinatura na plataforma de cobrança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-558">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="0a6cc-559">Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-559">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="0a6cc-560">Esse não é o mesmo que o ID da assinatura no Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-560">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0a6cc-561">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="0a6cc-561">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="0a6cc-562">Data de início do ciclo de cobrança exceto quando apresentadas as datas de dados de uso latentes anteriormente não cobradas (do ciclo de cobrança anterior).</span><span class="sxs-lookup"><span data-stu-id="0a6cc-562">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="0a6cc-563">A hora é sempre o início do dia, 0:00.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-563">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0a6cc-564">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="0a6cc-564">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="0a6cc-565">Data de término do ciclo de cobrança exceto quando apresentadas as datas de dados de uso latentes anteriormente não cobradas (do ciclo de cobrança anterior).</span><span class="sxs-lookup"><span data-stu-id="0a6cc-565">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="0a6cc-566">A hora é sempre o fim do dia, 23:59.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-566">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0a6cc-567">Data de uso</span><span class="sxs-lookup"><span data-stu-id="0a6cc-567">Usage Date</span></span></td>
<td><p><span data-ttu-id="0a6cc-568">Data de uso do serviço.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-568">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0a6cc-569">Tipo de medidor</span><span class="sxs-lookup"><span data-stu-id="0a6cc-569">Meter Type</span></span></td>
<td><p><span data-ttu-id="0a6cc-570">O tipo de medidor.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-570">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0a6cc-571">Categoria do medidor</span><span class="sxs-lookup"><span data-stu-id="0a6cc-571">Meter Category</span></span></td>
<td><p><span data-ttu-id="0a6cc-572">O serviço de nível superior para o uso.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-572">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0a6cc-573">ID do medidor</span><span class="sxs-lookup"><span data-stu-id="0a6cc-573">Meter Id</span></span></td>
<td><p><span data-ttu-id="0a6cc-574">A ID do medidor que está sendo usado.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-574">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0a6cc-575">Subcategoria do medidor</span><span class="sxs-lookup"><span data-stu-id="0a6cc-575">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="0a6cc-576">O tipo de serviço do Azure que pode afetar a taxa.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-576">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0a6cc-577">Nome do medidor</span><span class="sxs-lookup"><span data-stu-id="0a6cc-577">Meter Name</span></span></td>
<td><p><span data-ttu-id="0a6cc-578">A unidade de medida para o medidor que está sendo consumido.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-578">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0a6cc-579">Região do medidor</span><span class="sxs-lookup"><span data-stu-id="0a6cc-579">Meter Region</span></span></td>
<td><p><span data-ttu-id="0a6cc-580">Essa coluna identifica a localização de um data center dentro da região para serviços onde isso é aplicável e preenchido.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-580">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0a6cc-581">Unidade</span><span class="sxs-lookup"><span data-stu-id="0a6cc-581">Unit</span></span></td>
<td><p><span data-ttu-id="0a6cc-582">A unidade do nome do recurso.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-582">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0a6cc-583">Quantidade consumida</span><span class="sxs-lookup"><span data-stu-id="0a6cc-583">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="0a6cc-584">A quantidade de serviço consumida (horas, GB etc.) durante o período de relatório.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-584">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="0a6cc-585">Também inclui qualquer uso não cobrado de períodos de relatório anteriores.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-585">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0a6cc-586">Local do recurso</span><span class="sxs-lookup"><span data-stu-id="0a6cc-586">Resource Location</span></span></td>
<td><p><span data-ttu-id="0a6cc-587">O datacenter em que o medidor está em execução.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-587">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0a6cc-588">Serviço consumido</span><span class="sxs-lookup"><span data-stu-id="0a6cc-588">Consumed Service</span></span></td>
<td><p><span data-ttu-id="0a6cc-589">O serviço da plataforma do Azure que você usou.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-589">The Azure platform service that you used.</span></span></p></td>
</tr>


<tr class="even">
<td><span data-ttu-id="0a6cc-590">URI de recurso</span><span class="sxs-lookup"><span data-stu-id="0a6cc-590">Resource URI</span></span></td>
<td><p><span data-ttu-id="0a6cc-591">O URI do recurso que está sendo usado.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-591">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0a6cc-592">Tipo de cobrança</span><span class="sxs-lookup"><span data-stu-id="0a6cc-592">Charge type</span></span></td>
<td><p><span data-ttu-id="0a6cc-593">O tipo de encargo ou ajuste.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-593">The type of charge or adjustment.</span></span> <span data-ttu-id="0a6cc-594">Não disponível para a atividade atual.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-594">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0a6cc-595">Preço unitário</span><span class="sxs-lookup"><span data-stu-id="0a6cc-595">Unit price</span></span></td>
<td><p><span data-ttu-id="0a6cc-596">Preço por licença, conforme publicado na tabela de preços no momento da compra.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-596">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="0a6cc-597">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-597">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0a6cc-598">Quantity</span><span class="sxs-lookup"><span data-stu-id="0a6cc-598">Quantity</span></span></td>
<td><p><span data-ttu-id="0a6cc-599">Número de licenças.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-599">Number of licenses.</span></span> <span data-ttu-id="0a6cc-600">Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-600">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0a6cc-601">Tipo de unidade</span><span class="sxs-lookup"><span data-stu-id="0a6cc-601">Unit type</span></span></td>
<td><p><span data-ttu-id="0a6cc-602">O tipo de unidade em que o medidor é cobrado.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-602">The type of unit the meter is charged in.</span></span> <span data-ttu-id="0a6cc-603">Não disponível para a atividade atual.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-603">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0a6cc-604">Pré-imposto de cobrança</span><span class="sxs-lookup"><span data-stu-id="0a6cc-604">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="0a6cc-605">Valor total antes dos impostos.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-605">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0a6cc-606">Moeda de cobrança</span><span class="sxs-lookup"><span data-stu-id="0a6cc-606">Billing currency</span></span></td>
<td><p><span data-ttu-id="0a6cc-607">A moeda na região geográfica do cliente</span><span class="sxs-lookup"><span data-stu-id="0a6cc-607">The currency in the customer's geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0a6cc-608">Preço custo total</span><span class="sxs-lookup"><span data-stu-id="0a6cc-608">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="0a6cc-609">O preço antes da adição de impostos.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-609">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0a6cc-610">Moeda de preços</span><span class="sxs-lookup"><span data-stu-id="0a6cc-610">Pricing currency</span></span></td>
<td><p><span data-ttu-id="0a6cc-611">A moeda na tabela de preços.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-611">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0a6cc-612">Informações de serviço 1</span><span class="sxs-lookup"><span data-stu-id="0a6cc-612">Service Info 1</span></span></td>
<td><p><span data-ttu-id="0a6cc-613">O número de conexões ServiceBus que foram provisionados e utilizados em um dia específico.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-613">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0a6cc-614">Informações de serviço 2</span><span class="sxs-lookup"><span data-stu-id="0a6cc-614">Service Info 2</span></span></td>
<td><p><span data-ttu-id="0a6cc-615">Um campo herdado que captura metadados específicos do serviço opcionais.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-615">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0a6cc-616">Informações adicionais</span><span class="sxs-lookup"><span data-stu-id="0a6cc-616">Additional Info</span></span></td>
<td><p><span data-ttu-id="0a6cc-617">Quaisquer informações adicionais não abordadas em outras colunas.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-617">Any additional information not covered in other columns.</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0a6cc-618">EffectiveUnitPrice</span><span class="sxs-lookup"><span data-stu-id="0a6cc-618">EffectiveUnitPrice</span></span></td>
<td><p> <span data-ttu-id="0a6cc-619">Valor real cobrado por unidade (isso inclui descontos, crédito acumulado etc.).</span><span class="sxs-lookup"><span data-stu-id="0a6cc-619">Actual value charged per unit (this includes discounts, earned credit etc).</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0a6cc-620">PCToBCExchangeRate</span><span class="sxs-lookup"><span data-stu-id="0a6cc-620">PCToBCExchangeRate</span></span> </td>
<td><p><span data-ttu-id="0a6cc-621">Taxa de câmbio aplicada para moeda de preço para a moeda de cobrança (clientes).</span><span class="sxs-lookup"><span data-stu-id="0a6cc-621">Exchange rate applied for pricing currency to (customers) billing currency.</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0a6cc-622">PCToBCExchangeRateDate</span><span class="sxs-lookup"><span data-stu-id="0a6cc-622">PCToBCExchangeRateDate</span></span> </td>
<td><p><span data-ttu-id="0a6cc-623">Data em que a moeda de preço para a taxa de câmbio da moeda de cobrança é determinada.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-623">Date at which the pricing currency to billing currency exchange rate is determined.</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0a6cc-624">EntitlementID</span><span class="sxs-lookup"><span data-stu-id="0a6cc-624">EntitlementID</span></span></td>
<td><p><span data-ttu-id="0a6cc-625">Representa a assinatura do Azure.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-625">Represents Azure subscriptionID.</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0a6cc-626">EntitlementDescription</span><span class="sxs-lookup"><span data-stu-id="0a6cc-626">EntitlementDescription</span></span></td>
<td><p><span data-ttu-id="0a6cc-627">Representa o nome da assinatura do Azure.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-627">Represents name of Azure subscription.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="0a6cc-628">Mapeando cobranças entre uma fatura e o arquivo de reconciliação</span><span class="sxs-lookup"><span data-stu-id="0a6cc-628">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="0a6cc-629">Sua fatura fornece um resumo dos encargos, enquanto seu arquivo de reconciliação fornece uma divisão detalhada das transações de item de linha, incluindo os tipos de carga.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-629">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="0a6cc-630">Para fazer referência cruzada das quantidades de carga entre o arquivo de reconciliação e fatura, você pode usar opções de filtro do Microsoft Excel para filtrar por tipos de cobrança no arquivo de reconciliação para mapear os encargos de fatura em um conjunto de detalhamentos de cobrança no arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-630">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="0a6cc-631">Os arquivos de reconciliação, tanto os baseados em licença quanto os baseados em uso, mostram apenas encargos e transações relacionadas ao uso (unidades consumidas e encargos relacionados).</span><span class="sxs-lookup"><span data-stu-id="0a6cc-631">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="0a6cc-632">Créditos, descontos ou reembolsos que aparecem na fatura como "ajustes" não são mostrados no arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-632">One off credits, discounts or refunds which appear on the invoice as “Adjustments" are not shown in the reconciliation file.</span></span>

<span data-ttu-id="0a6cc-633">A tabela a seguir mostra os mapeamentos entre uma seção da fatura e os tipos de encargo associados que podem aparecer nos arquivos de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-633">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="0a6cc-634"><strong>Descrição da cobrança da fatura</strong></span><span class="sxs-lookup"><span data-stu-id="0a6cc-634"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="0a6cc-635"><strong>Descrição do encargo do arquivo de reconciliação (coluna Chargetype)</strong></span><span class="sxs-lookup"><span data-stu-id="0a6cc-635"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="0a6cc-636"><strong>Qual é essa cobrança?</strong></span><span class="sxs-lookup"><span data-stu-id="0a6cc-636"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="0a6cc-637"><strong>Como fazer mapear esses ChargeTypes para a fatura?</strong></span><span class="sxs-lookup"><span data-stu-id="0a6cc-637"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="0a6cc-638"><strong>Encargos baseados em licença</strong></span><span class="sxs-lookup"><span data-stu-id="0a6cc-638"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="0a6cc-639">Taxa de ativação</span><span class="sxs-lookup"><span data-stu-id="0a6cc-639">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="0a6cc-640">O valor cobrado do cliente quando ele usa a assinatura depois de comprá-la.</span><span class="sxs-lookup"><span data-stu-id="0a6cc-640">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="0a6cc-641">No arquivo baseado em licença, some a coluna <strong>Quantidade</strong></span><span class="sxs-lookup"><span data-stu-id="0a6cc-641">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="0a6cc-642">Taxa de cancelamento</span><span class="sxs-lookup"><span data-stu-id="0a6cc-642">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="0a6cc-643">Os encargos proporcionais reembolsados para o cliente quando os assentos associados são alterados</span><span class="sxs-lookup"><span data-stu-id="0a6cc-643">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="0a6cc-644">Taxa do Ciclo</span><span class="sxs-lookup"><span data-stu-id="0a6cc-644">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="0a6cc-645">Encargos periódicos de uma assinatura</span><span class="sxs-lookup"><span data-stu-id="0a6cc-645">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="0a6cc-646">Proporcional à instância do ciclo</span><span class="sxs-lookup"><span data-stu-id="0a6cc-646">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="0a6cc-647">Os encargos proporcionais cobrados do cliente quando os assentos associados são alterados</span><span class="sxs-lookup"><span data-stu-id="0a6cc-647">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="0a6cc-648">Taxas proporcionais durante o cancelamento</span><span class="sxs-lookup"><span data-stu-id="0a6cc-648">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="0a6cc-649">Reembolso proporcional para a parte não utilizada do serviço após o cancelamento</span><span class="sxs-lookup"><span data-stu-id="0a6cc-649">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="0a6cc-650">Taxas proporcionais na compra</span><span class="sxs-lookup"><span data-stu-id="0a6cc-650">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="0a6cc-651">O tipo de encargo para uma assinatura ao usar a cobrança anual</span><span class="sxs-lookup"><span data-stu-id="0a6cc-651">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="0a6cc-652">Valor de compra</span><span class="sxs-lookup"><span data-stu-id="0a6cc-652">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="0a6cc-653">O tipo de encargo para uma assinatura ao usar a cobrança mensal</span><span class="sxs-lookup"><span data-stu-id="0a6cc-653">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="0a6cc-654">Taxa proporcional ao renovar</span><span class="sxs-lookup"><span data-stu-id="0a6cc-654">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="0a6cc-655">Taxas proporcionais após a renovação da assinatura</span><span class="sxs-lookup"><span data-stu-id="0a6cc-655">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="0a6cc-656">Taxa de renovação</span><span class="sxs-lookup"><span data-stu-id="0a6cc-656">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="0a6cc-657">Cobrança para renovação de uma assinatura</span><span class="sxs-lookup"><span data-stu-id="0a6cc-657">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="0a6cc-658">Taxas proporcionais ao ativar</span><span class="sxs-lookup"><span data-stu-id="0a6cc-658">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="0a6cc-659">Taxas proporcionais da ativação até o final do período de cobrança</span><span class="sxs-lookup"><span data-stu-id="0a6cc-659">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>



<tr>
<td rowspan="5">
<p><span data-ttu-id="0a6cc-660"><strong>Encargos de uso único</strong></span><span class="sxs-lookup"><span data-stu-id="0a6cc-660"><strong>One-time Charges</strong></span></span></p>

</td>
<td>
<p><span data-ttu-id="0a6cc-661">Novo</span><span class="sxs-lookup"><span data-stu-id="0a6cc-661">New</span></span></p>
</td>
<td>
<p><span data-ttu-id="0a6cc-662">Usado quando uma nova compra é criada</span><span class="sxs-lookup"><span data-stu-id="0a6cc-662">Used when a new purchase is created</span></span></p>
</td>

<p></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="0a6cc-663">addQuantity</span><span class="sxs-lookup"><span data-stu-id="0a6cc-663">addQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="0a6cc-664">Usado tanto no reembolso da compra original quanto na nova quantidade após o aumento</span><span class="sxs-lookup"><span data-stu-id="0a6cc-664">Used in both the refund of the original purchase and the new quantity after increase</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="0a6cc-665">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="0a6cc-665">removeQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="0a6cc-666">Usado tanto no reembolso da compra original quanto na nova quantidade após a diminuição</span><span class="sxs-lookup"><span data-stu-id="0a6cc-666">Used in both the refund of the original purchase and the new quantity after decrease</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="0a6cc-667">Cancelar</span><span class="sxs-lookup"><span data-stu-id="0a6cc-667">Cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="0a6cc-668">Usado quando uma assinatura é cancelada</span><span class="sxs-lookup"><span data-stu-id="0a6cc-668">Used when a subscription is cancelled</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="0a6cc-669">Converter</span><span class="sxs-lookup"><span data-stu-id="0a6cc-669">Convert</span></span></p>
</td>
<td>
<p><span data-ttu-id="0a6cc-670">Usado quando uma licença é atualizada, mas o número de estações permanece inalterado</span><span class="sxs-lookup"><span data-stu-id="0a6cc-670">Used when a license is upgraded but the number of seats remains unchanged</span></span></p>
</td>
</tr>

<tr>
<td rowspan="2">
<p><span data-ttu-id="0a6cc-671"><strong>Encargos de uso</strong></span><span class="sxs-lookup"><span data-stu-id="0a6cc-671"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="0a6cc-672">Avaliar a taxa de uso ao cancelar</span><span class="sxs-lookup"><span data-stu-id="0a6cc-672">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="0a6cc-673">Taxa de uso de acesso com o cancelamento para uso não pago durante o período de cobrança atual</span><span class="sxs-lookup"><span data-stu-id="0a6cc-673">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="0a6cc-674">No arquivo baseado em uso, some a coluna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="0a6cc-674">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="0a6cc-675">Avalie a taxa de uso para o ciclo atual</span><span class="sxs-lookup"><span data-stu-id="0a6cc-675">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="0a6cc-676">Taxa de uso de acesso para o período atual de cobrança</span><span class="sxs-lookup"><span data-stu-id="0a6cc-676">Access usage fee for the current billing period</span></span></p>
</td>
</tr>

<tr>
<td>
<p><span data-ttu-id="0a6cc-677"><strong>Crédito</strong></span><span class="sxs-lookup"><span data-stu-id="0a6cc-677"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="0a6cc-678">Deslocando um item de linha</span><span class="sxs-lookup"><span data-stu-id="0a6cc-678">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="0a6cc-679">Reembolso parcial ou integral para um item de linha, incluindo os impostos</span><span class="sxs-lookup"><span data-stu-id="0a6cc-679">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="0a6cc-680">No arquivo baseado em licença, some a coluna <strong>TotalForCustomer</strong></span><span class="sxs-lookup"><span data-stu-id="0a6cc-680">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="0a6cc-681">No arquivo baseado em uso, some a coluna <strong>PostTaxTotal</strong></span><span class="sxs-lookup"><span data-stu-id="0a6cc-681">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="0a6cc-682"><strong>Descontos com base no uso</strong></span><span class="sxs-lookup"><span data-stu-id="0a6cc-682"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="0a6cc-683">Desconto de ativação</span><span class="sxs-lookup"><span data-stu-id="0a6cc-683">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="0a6cc-684">Desconto aplicado quando a assinatura é ativada</span><span class="sxs-lookup"><span data-stu-id="0a6cc-684">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="0a6cc-685">No arquivo baseado em uso, some a coluna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="0a6cc-685">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="0a6cc-686">Desconto de ciclo</span><span class="sxs-lookup"><span data-stu-id="0a6cc-686">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="0a6cc-687">Desconto aplicado em cobranças periódicas</span><span class="sxs-lookup"><span data-stu-id="0a6cc-687">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="0a6cc-688">Desconto de renovação</span><span class="sxs-lookup"><span data-stu-id="0a6cc-688">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="0a6cc-689">Desconto aplicado quando a assinatura é renovada</span><span class="sxs-lookup"><span data-stu-id="0a6cc-689">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="0a6cc-690">Desconto de cancelamento</span><span class="sxs-lookup"><span data-stu-id="0a6cc-690">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="0a6cc-691">Encargos aplicados quando descontos são cancelados</span><span class="sxs-lookup"><span data-stu-id="0a6cc-691">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="0a6cc-692"><strong>Descontos baseados em licença</strong></span><span class="sxs-lookup"><span data-stu-id="0a6cc-692"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="0a6cc-693"><em>Pode ser aplicado a vários tipos de cobrança</em></span><span class="sxs-lookup"><span data-stu-id="0a6cc-693"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="0a6cc-694">No arquivo baseado em licença, some a coluna <strong>TotalOtherDiscount</strong></span><span class="sxs-lookup"><span data-stu-id="0a6cc-694">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="0a6cc-695"><strong>Impostos</strong>&nbsp;ou&nbsp;<strong>IVA</strong></span><span class="sxs-lookup"><span data-stu-id="0a6cc-695"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="0a6cc-696"><em>Pode ser aplicado a vários tipos de cobrança</em></span><span class="sxs-lookup"><span data-stu-id="0a6cc-696"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="0a6cc-697"><em>Exceção: &quot;Offset um item de linha &quot; já inclui impostos. Consulte créditos, acima.</em></span><span class="sxs-lookup"><span data-stu-id="0a6cc-697"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="0a6cc-698">Impostos ou impostos sobre valor agregado (IVA)</span><span class="sxs-lookup"><span data-stu-id="0a6cc-698">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="0a6cc-699">No arquivo baseado em licença, some a coluna <strong>Imposto</strong></span><span class="sxs-lookup"><span data-stu-id="0a6cc-699">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="0a6cc-700">No arquivo baseado em uso, some a coluna <strong>TaxAmount</strong></span><span class="sxs-lookup"><span data-stu-id="0a6cc-700">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
