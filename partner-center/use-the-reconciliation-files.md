---
title: Usar seus arquivos de reconciliação
ms.topic: article
ms.date: 03/26/2021
description: Saiba mais sobre os arquivos de reconciliação no Partner Center e como interpretar as exibições detalhadas de item de linha de encargos para um determinado ciclo de cobrança.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4a6a1455304f12e364d71e666cbd548821f8be55
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633889"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="11d88-103">Saiba como ler os itens de linha em seus arquivos de reconciliação do Partner Center</span><span class="sxs-lookup"><span data-stu-id="11d88-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="11d88-104">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="11d88-104">**Appropriate roles**</span></span>

- <span data-ttu-id="11d88-105">Administrador de cobrança</span><span class="sxs-lookup"><span data-stu-id="11d88-105">Billing admin</span></span>
- <span data-ttu-id="11d88-106">Administrador global</span><span class="sxs-lookup"><span data-stu-id="11d88-106">Global admin</span></span>

<span data-ttu-id="11d88-107">Você pode baixar seus arquivos de reconciliação do Partner Center para obter uma exibição detalhada de item de linha de cada encargo em um ciclo de cobrança.</span><span class="sxs-lookup"><span data-stu-id="11d88-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="11d88-108">Os detalhes do item de linha incluem encargos para as assinaturas de cada cliente e eventos detalhados (como uma adição de licenças de médio prazo a uma assinatura).</span><span class="sxs-lookup"><span data-stu-id="11d88-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="11d88-109">Para obter informações sobre como ler sua **fatura**, consulte [ler sua fatura](read-your-bill.md).</span><span class="sxs-lookup"><span data-stu-id="11d88-109">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="11d88-110">Entender os campos de arquivo de reconciliação</span><span class="sxs-lookup"><span data-stu-id="11d88-110">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="11d88-111">Campos do arquivo de reconciliação baseados na licença</span><span class="sxs-lookup"><span data-stu-id="11d88-111">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="11d88-112">Campos do arquivo de reconciliação baseados no uso</span><span class="sxs-lookup"><span data-stu-id="11d88-112">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="11d88-113">Campos do arquivo de reconciliação de uso com classificação diária</span><span class="sxs-lookup"><span data-stu-id="11d88-113">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="11d88-114">Campos de arquivo de reconciliação do CSP de compra única</span><span class="sxs-lookup"><span data-stu-id="11d88-114">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="11d88-115">Entender os tipos de encargo em arquivos de reconciliação</span><span class="sxs-lookup"><span data-stu-id="11d88-115">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="11d88-116">Para entender os tipos de encargos em arquivos de reconciliação (a coluna **chargetype** ), confira [tipos de encargo de arquivo de reconciliação](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="11d88-116">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="11d88-117">Corrigir problemas de formatação</span><span class="sxs-lookup"><span data-stu-id="11d88-117">Fix formatting issues</span></span>

<span data-ttu-id="11d88-118">Ocasionalmente, um arquivo de reconciliação pode conter problemas de formatação.</span><span class="sxs-lookup"><span data-stu-id="11d88-118">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="11d88-119">Por exemplo, esse problema pode ocorrer se a localidade en-US não for usada.</span><span class="sxs-lookup"><span data-stu-id="11d88-119">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="11d88-120">Siga estas etapas para corrigir quaisquer problemas de formatação em seus arquivos de reconciliação:</span><span class="sxs-lookup"><span data-stu-id="11d88-120">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="11d88-121">Abra o arquivo de reconciliação (no formato. csv) no Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="11d88-121">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="11d88-122">Selecione a primeira coluna no arquivo.</span><span class="sxs-lookup"><span data-stu-id="11d88-122">Select the first column in the file.</span></span>
3. <span data-ttu-id="11d88-123">Abra o **Assistente para converter texto em colunas**.</span><span class="sxs-lookup"><span data-stu-id="11d88-123">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="11d88-124">Na faixa de opções, selecione **dados** e, em seguida, selecione **texto para colunas**.</span><span class="sxs-lookup"><span data-stu-id="11d88-124">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="11d88-125">No assistente, selecione **tipo de arquivo delimitado**.</span><span class="sxs-lookup"><span data-stu-id="11d88-125">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="11d88-126">Em seguida, selecione **Avançar**.</span><span class="sxs-lookup"><span data-stu-id="11d88-126">Then, select **Next**.</span></span>
5. <span data-ttu-id="11d88-127">No campo **delimitadores** , selecione **vírgula**.</span><span class="sxs-lookup"><span data-stu-id="11d88-127">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="11d88-128">(Se a **guia** já estiver selecionada, você poderá deixar essa opção selecionada.) Em seguida, selecione **Avançar**.</span><span class="sxs-lookup"><span data-stu-id="11d88-128">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="11d88-129">No campo **formato de dados da coluna** , selecione **Data: MDY**.</span><span class="sxs-lookup"><span data-stu-id="11d88-129">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="11d88-130">Em seguida, selecione **Avançar**.</span><span class="sxs-lookup"><span data-stu-id="11d88-130">Then, select **Next**.</span></span>
7. <span data-ttu-id="11d88-131">No campo **formato de dados da coluna** , selecione **texto** para todas as colunas de valor.</span><span class="sxs-lookup"><span data-stu-id="11d88-131">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="11d88-132">Em seguida, selecione **Concluir**.</span><span class="sxs-lookup"><span data-stu-id="11d88-132">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="11d88-133">Baixar arquivos de reconciliação programaticamente</span><span class="sxs-lookup"><span data-stu-id="11d88-133">Download reconciliation files programmatically</span></span>

<span data-ttu-id="11d88-134">Os arquivos de reconciliação podem ser muito grandes e, às vezes, são difíceis de baixar.</span><span class="sxs-lookup"><span data-stu-id="11d88-134">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="11d88-135">Para baixar arquivos de reconciliação programaticamente, consulte [obter itens de linha da fatura](/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="11d88-135">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a><span data-ttu-id="11d88-136">Se o arquivo exceder o limite de linha no Excel</span><span class="sxs-lookup"><span data-stu-id="11d88-136">If your file exceeds the row limit in Excel</span></span>

<span data-ttu-id="11d88-137">Se você for capaz de baixar um arquivo de reconciliação, mas não abri-lo no Microsoft Excel, provavelmente significa que o arquivo contém mais linhas do que o Excel permitirá.</span><span class="sxs-lookup"><span data-stu-id="11d88-137">If you’re able to download a reconciliation file but not open it in Microsoft Excel, it probably means the file contains more rows than Excel will allow.</span></span> <span data-ttu-id="11d88-138">Se isso acontecer, você poderá usar qualquer um dos procedimentos abaixo para abrir o arquivo.</span><span class="sxs-lookup"><span data-stu-id="11d88-138">If this happens, you can use either of the procedures below to open the file.</span></span>

### <a name="open-a-recon-file-in-power-bi"></a><span data-ttu-id="11d88-139">Abrir um arquivo reconhecimento no Power BI</span><span class="sxs-lookup"><span data-stu-id="11d88-139">Open a recon file in Power BI</span></span>

1. <span data-ttu-id="11d88-140">Baixe o arquivo de reconciliação como faria normalmente.</span><span class="sxs-lookup"><span data-stu-id="11d88-140">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="11d88-141">Baixe, instale e abra uma instância do Power BI.</span><span class="sxs-lookup"><span data-stu-id="11d88-141">Download, install, and open an instance of Power BI.</span></span>
3. <span data-ttu-id="11d88-142">Na guia Power BI **página inicial** , selecione **obter dados**.</span><span class="sxs-lookup"><span data-stu-id="11d88-142">On the Power BI **Home** tab, select **Get data**.</span></span>
4. <span data-ttu-id="11d88-143">Na lista de **fontes de dados comuns**, selecione **texto/CSV**.</span><span class="sxs-lookup"><span data-stu-id="11d88-143">In the list of **Common data sources**, select **Text/CSV**.</span></span>
5. <span data-ttu-id="11d88-144">Quando solicitado, abra o arquivo reconhecimento.</span><span class="sxs-lookup"><span data-stu-id="11d88-144">When prompted, open your recon file.</span></span>

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a><span data-ttu-id="11d88-145">Abrir um arquivo reconhecimento em uma tabela dinâmica do Excel</span><span class="sxs-lookup"><span data-stu-id="11d88-145">Open a recon file in an Excel pivot table</span></span>

1. <span data-ttu-id="11d88-146">Baixe o arquivo de reconciliação como faria normalmente.</span><span class="sxs-lookup"><span data-stu-id="11d88-146">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="11d88-147">Abra um novo arquivo no Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="11d88-147">Open a new file in Microsoft Excel.</span></span>
3. <span data-ttu-id="11d88-148">Na guia **dados** , selecione **obter dados**, selecione **do arquivo** e, em seguida, selecione **texto/CSV**.</span><span class="sxs-lookup"><span data-stu-id="11d88-148">On the **Data** tab, select **Get data**, select **From file**, and then select **Text/CSV**.</span></span>
4. <span data-ttu-id="11d88-149">Quando solicitado, abra o arquivo reconhecimento.</span><span class="sxs-lookup"><span data-stu-id="11d88-149">When prompted, open your recon file.</span></span> <span data-ttu-id="11d88-150">Seus dados serão exibidos.</span><span class="sxs-lookup"><span data-stu-id="11d88-150">Your data will appear.</span></span>
5. <span data-ttu-id="11d88-151">No menu suspenso **carregar** , selecione **carregar para** e, em seguida, **OK**.</span><span class="sxs-lookup"><span data-stu-id="11d88-151">In the **Load** dropdown menu, select **Load to**, and then **OK**.</span></span>
6. <span data-ttu-id="11d88-152">Na caixa de diálogo **importar dados** , selecione **relatório de tabela dinâmica** para abrir o arquivo.</span><span class="sxs-lookup"><span data-stu-id="11d88-152">In the **Import Data** dialog box, select **PivotTable Report** to open your file.</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="11d88-153">Impostos do mapa ou IVA</span><span class="sxs-lookup"><span data-stu-id="11d88-153">Map taxes or VAT</span></span>

<span data-ttu-id="11d88-154">Para mapear impostos ou IVA (imposto sobre valor agregado) para sua fatura:</span><span class="sxs-lookup"><span data-stu-id="11d88-154">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="11d88-155">Some a coluna de **impostos** do arquivo baseado em licença.</span><span class="sxs-lookup"><span data-stu-id="11d88-155">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="11d88-156">Some a coluna **TaxAmount** do arquivo baseado em uso.</span><span class="sxs-lookup"><span data-stu-id="11d88-156">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="11d88-157">Discriminar arquivos de reconciliação por parceiro</span><span class="sxs-lookup"><span data-stu-id="11d88-157">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="11d88-158">Os parceiros no **modelo indireto** podem usar esses campos adicionais em arquivos de reconciliação baseados em licença e de uso para discriminar os arquivos pelo revendedor.</span><span class="sxs-lookup"><span data-stu-id="11d88-158">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="11d88-159">ID MPN</span><span class="sxs-lookup"><span data-stu-id="11d88-159">MPN ID</span></span> | <span data-ttu-id="11d88-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="11d88-160">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="11d88-161">ID MPN</span><span class="sxs-lookup"><span data-stu-id="11d88-161">MPN ID</span></span> | <span data-ttu-id="11d88-162">O identificador de Microsoft Partner Network (MPN) do parceiro CSP (provedor de soluções na nuvem) (direto ou indireto).</span><span class="sxs-lookup"><span data-stu-id="11d88-162">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="11d88-163">ID do MPN do revendedor</span><span class="sxs-lookup"><span data-stu-id="11d88-163">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="11d88-164">O [identificador de MPN do revendedor do registro para a assinatura](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="11d88-164">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="11d88-165">Este campo corresponde à ID do revendedor listada para a assinatura específica no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="11d88-165">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="11d88-166">Só aparece em arquivos de reconciliação para parceiros no modelo indireto.</span><span class="sxs-lookup"><span data-stu-id="11d88-166">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="11d88-167">ID do MPN do revendedor</span><span class="sxs-lookup"><span data-stu-id="11d88-167">Reseller MPN ID</span></span>

<span data-ttu-id="11d88-168">Se um parceiro CSP vendeu a assinatura diretamente ao cliente, sua **ID MPN** é listada duas vezes, como a **ID MPN** e a **ID de MPN do revendedor**.</span><span class="sxs-lookup"><span data-stu-id="11d88-168">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="11d88-169">Se um parceiro CSP tiver um revendedor sem **ID MPN**, esse valor será definido como a ID de **MPN** do parceiro em vez disso.</span><span class="sxs-lookup"><span data-stu-id="11d88-169">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="11d88-170">Se o parceiro CSP remover uma **ID de MPN do revendedor**, esse valor será definido como *-1*.</span><span class="sxs-lookup"><span data-stu-id="11d88-170">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="11d88-171">Para exibir ou atualizar a **ID de MPN do revendedor**:</span><span class="sxs-lookup"><span data-stu-id="11d88-171">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="11d88-172">Conecte-se ao Partner Center.</span><span class="sxs-lookup"><span data-stu-id="11d88-172">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="11d88-173">No menu Partner Center, selecione **Clientes**.</span><span class="sxs-lookup"><span data-stu-id="11d88-173">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="11d88-174">Escolha o cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="11d88-174">Choose the customer from the list.</span></span>
4. <span data-ttu-id="11d88-175">No menu cliente, selecione **assinaturas**.</span><span class="sxs-lookup"><span data-stu-id="11d88-175">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="11d88-176">Escolha a assinatura na lista.</span><span class="sxs-lookup"><span data-stu-id="11d88-176">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="11d88-177">Selecione **Atualizar** para alterar o **Revendedor (ID do MPN)**.</span><span class="sxs-lookup"><span data-stu-id="11d88-177">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="11d88-178">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="11d88-178">Next steps</span></span>

- [<span data-ttu-id="11d88-179">Como ler o arquivo Bill & reconhecimento</span><span class="sxs-lookup"><span data-stu-id="11d88-179">How to read your bill & recon file</span></span>](read-your-bill.md) 