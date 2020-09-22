---
title: Usar seus arquivos de reconciliação
ms.topic: article
ms.date: 06/08/2020
description: Saiba mais sobre os arquivos de reconciliação no Partner Center e como interpretar as exibições detalhadas de item de linha de encargos para um determinado ciclo de cobrança.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 98bfd9a9ce6f03ad62a830f05ba82f9b90268326
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "90999700"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="4f69c-103">Saiba como ler os itens de linha em seus arquivos de reconciliação do Partner Center</span><span class="sxs-lookup"><span data-stu-id="4f69c-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="4f69c-104">Aplica-se a:</span><span class="sxs-lookup"><span data-stu-id="4f69c-104">Applies to:</span></span>

- <span data-ttu-id="4f69c-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="4f69c-105">Partner Center</span></span>
- <span data-ttu-id="4f69c-106">Partner Center do Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="4f69c-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="4f69c-107">Você pode baixar seus arquivos de reconciliação do Partner Center para obter uma exibição detalhada de item de linha de cada encargo em um ciclo de cobrança.</span><span class="sxs-lookup"><span data-stu-id="4f69c-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="4f69c-108">Os detalhes do item de linha incluem encargos para as assinaturas de cada cliente e eventos detalhados (como uma adição de licenças de médio prazo a uma assinatura).</span><span class="sxs-lookup"><span data-stu-id="4f69c-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="4f69c-109">Funções apropriadas:</span><span class="sxs-lookup"><span data-stu-id="4f69c-109">Appropriate roles:</span></span>

- <span data-ttu-id="4f69c-110">Administrador de cobrança</span><span class="sxs-lookup"><span data-stu-id="4f69c-110">Billing admin</span></span>
- <span data-ttu-id="4f69c-111">Administrador global</span><span class="sxs-lookup"><span data-stu-id="4f69c-111">Global admin</span></span>

<span data-ttu-id="4f69c-112">Para obter informações sobre como ler sua **fatura**, consulte [ler sua fatura](read-your-bill.md).</span><span class="sxs-lookup"><span data-stu-id="4f69c-112">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="4f69c-113">Entender os campos de arquivo de reconciliação</span><span class="sxs-lookup"><span data-stu-id="4f69c-113">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="4f69c-114">Campos de arquivo de reconciliação com base em licença</span><span class="sxs-lookup"><span data-stu-id="4f69c-114">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="4f69c-115">Campos de arquivo de reconciliação com base no uso</span><span class="sxs-lookup"><span data-stu-id="4f69c-115">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="4f69c-116">Campos de arquivo de reconciliação de uso com classificação diária</span><span class="sxs-lookup"><span data-stu-id="4f69c-116">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="4f69c-117">Entender os tipos de encargo em arquivos de reconciliação</span><span class="sxs-lookup"><span data-stu-id="4f69c-117">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="4f69c-118">Para entender os tipos de encargos em arquivos de reconciliação (a coluna **chargetype** ), confira [tipos de encargo de arquivo de reconciliação](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="4f69c-118">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="4f69c-119">Corrigir problemas de formatação</span><span class="sxs-lookup"><span data-stu-id="4f69c-119">Fix formatting issues</span></span>

<span data-ttu-id="4f69c-120">Ocasionalmente, um arquivo de reconciliação pode conter problemas de formatação.</span><span class="sxs-lookup"><span data-stu-id="4f69c-120">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="4f69c-121">Por exemplo, esse problema pode ocorrer se a localidade en-US não for usada.</span><span class="sxs-lookup"><span data-stu-id="4f69c-121">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="4f69c-122">Siga estas etapas para corrigir quaisquer problemas de formatação em seus arquivos de reconciliação:</span><span class="sxs-lookup"><span data-stu-id="4f69c-122">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="4f69c-123">Abra o arquivo de reconciliação (no formato. csv) no Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="4f69c-123">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="4f69c-124">Selecione a primeira coluna no arquivo.</span><span class="sxs-lookup"><span data-stu-id="4f69c-124">Select the first column in the file.</span></span>
3. <span data-ttu-id="4f69c-125">Abra o **Assistente para converter texto em colunas**.</span><span class="sxs-lookup"><span data-stu-id="4f69c-125">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="4f69c-126">Na faixa de opções, selecione **dados**e, em seguida, selecione **texto para colunas**.</span><span class="sxs-lookup"><span data-stu-id="4f69c-126">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="4f69c-127">No assistente, selecione **tipo de arquivo delimitado**.</span><span class="sxs-lookup"><span data-stu-id="4f69c-127">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="4f69c-128">Em seguida, selecione **Avançar**.</span><span class="sxs-lookup"><span data-stu-id="4f69c-128">Then, select **Next**.</span></span>
5. <span data-ttu-id="4f69c-129">No campo **delimitadores** , selecione **vírgula**.</span><span class="sxs-lookup"><span data-stu-id="4f69c-129">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="4f69c-130">(Se a **guia** já estiver selecionada, você poderá deixar essa opção selecionada.) Em seguida, selecione **Avançar**.</span><span class="sxs-lookup"><span data-stu-id="4f69c-130">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="4f69c-131">No campo **formato de dados da coluna** , selecione **Data: MDY**.</span><span class="sxs-lookup"><span data-stu-id="4f69c-131">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="4f69c-132">Em seguida, selecione **Avançar**.</span><span class="sxs-lookup"><span data-stu-id="4f69c-132">Then, select **Next**.</span></span>
7. <span data-ttu-id="4f69c-133">No campo **formato de dados da coluna** , selecione **texto** para todas as colunas de valor.</span><span class="sxs-lookup"><span data-stu-id="4f69c-133">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="4f69c-134">Em seguida, selecione **Concluir**.</span><span class="sxs-lookup"><span data-stu-id="4f69c-134">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="4f69c-135">Baixar arquivos de reconciliação programaticamente</span><span class="sxs-lookup"><span data-stu-id="4f69c-135">Download reconciliation files programmatically</span></span>

<span data-ttu-id="4f69c-136">Os arquivos de reconciliação podem ser muito grandes e, às vezes, são difíceis de baixar.</span><span class="sxs-lookup"><span data-stu-id="4f69c-136">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="4f69c-137">Para baixar arquivos de reconciliação programaticamente, consulte [obter itens de linha da fatura](/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="4f69c-137">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="4f69c-138">Impostos do mapa ou IVA</span><span class="sxs-lookup"><span data-stu-id="4f69c-138">Map taxes or VAT</span></span>

<span data-ttu-id="4f69c-139">Para mapear impostos ou IVA (imposto sobre valor agregado) para sua fatura:</span><span class="sxs-lookup"><span data-stu-id="4f69c-139">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="4f69c-140">Some a coluna de **impostos** do arquivo baseado em licença.</span><span class="sxs-lookup"><span data-stu-id="4f69c-140">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="4f69c-141">Some a coluna **TaxAmount** do arquivo baseado em uso.</span><span class="sxs-lookup"><span data-stu-id="4f69c-141">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="4f69c-142">Discriminar arquivos de reconciliação por parceiro</span><span class="sxs-lookup"><span data-stu-id="4f69c-142">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="4f69c-143">Os parceiros no **modelo indireto** podem usar esses campos adicionais em arquivos de reconciliação baseados em licença e de uso para discriminar os arquivos pelo revendedor.</span><span class="sxs-lookup"><span data-stu-id="4f69c-143">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="4f69c-144">ID MPN</span><span class="sxs-lookup"><span data-stu-id="4f69c-144">MPN ID</span></span> | <span data-ttu-id="4f69c-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f69c-145">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="4f69c-146">ID MPN</span><span class="sxs-lookup"><span data-stu-id="4f69c-146">MPN ID</span></span> | <span data-ttu-id="4f69c-147">O identificador de Microsoft Partner Network (MPN) do parceiro CSP (provedor de soluções na nuvem) (direto ou indireto).</span><span class="sxs-lookup"><span data-stu-id="4f69c-147">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="4f69c-148">ID do MPN do revendedor</span><span class="sxs-lookup"><span data-stu-id="4f69c-148">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="4f69c-149">O [identificador de MPN do revendedor do registro para a assinatura](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="4f69c-149">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="4f69c-150">Este campo corresponde à ID do revendedor listada para a assinatura específica no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="4f69c-150">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="4f69c-151">Só aparece em arquivos de reconciliação para parceiros no modelo indireto.</span><span class="sxs-lookup"><span data-stu-id="4f69c-151">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="4f69c-152">ID do MPN do revendedor</span><span class="sxs-lookup"><span data-stu-id="4f69c-152">Reseller MPN ID</span></span>

<span data-ttu-id="4f69c-153">Se um parceiro CSP vendeu a assinatura diretamente ao cliente, sua **ID MPN** é listada duas vezes, como a **ID MPN** e a **ID de MPN do revendedor**.</span><span class="sxs-lookup"><span data-stu-id="4f69c-153">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="4f69c-154">Se um parceiro CSP tiver um revendedor sem **ID MPN**, esse valor será definido como a ID de **MPN** do parceiro em vez disso.</span><span class="sxs-lookup"><span data-stu-id="4f69c-154">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="4f69c-155">Se o parceiro CSP remover uma **ID de MPN do revendedor**, esse valor será definido como *-1*.</span><span class="sxs-lookup"><span data-stu-id="4f69c-155">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="4f69c-156">Para exibir ou atualizar a **ID de MPN do revendedor**:</span><span class="sxs-lookup"><span data-stu-id="4f69c-156">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="4f69c-157">Conecte-se ao Partner Center.</span><span class="sxs-lookup"><span data-stu-id="4f69c-157">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="4f69c-158">No menu Partner Center, selecione **Clientes**.</span><span class="sxs-lookup"><span data-stu-id="4f69c-158">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="4f69c-159">Escolha o cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="4f69c-159">Choose the customer from the list.</span></span>
4. <span data-ttu-id="4f69c-160">No menu cliente, selecione **assinaturas**.</span><span class="sxs-lookup"><span data-stu-id="4f69c-160">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="4f69c-161">Escolha a assinatura na lista.</span><span class="sxs-lookup"><span data-stu-id="4f69c-161">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="4f69c-162">Selecione **Atualizar** para alterar o **Revendedor (ID do MPN)**.</span><span class="sxs-lookup"><span data-stu-id="4f69c-162">Select **update** to change the **Reseller (MPN ID)**.</span></span>