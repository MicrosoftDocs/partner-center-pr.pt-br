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
ms.openlocfilehash: aefd5258c778fd8a7b92bfe49f245bf818497fb8
ms.sourcegitcommit: dd51744a4af3797493a5ebbfc766dab86ff00477
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2021
ms.locfileid: "105730064"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="567ce-103">Saiba como ler os itens de linha em seus arquivos de reconciliação do Partner Center</span><span class="sxs-lookup"><span data-stu-id="567ce-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="567ce-104">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="567ce-104">**Appropriate roles**</span></span>

- <span data-ttu-id="567ce-105">Administrador de cobrança</span><span class="sxs-lookup"><span data-stu-id="567ce-105">Billing admin</span></span>
- <span data-ttu-id="567ce-106">Administrador global</span><span class="sxs-lookup"><span data-stu-id="567ce-106">Global admin</span></span>

<span data-ttu-id="567ce-107">Você pode baixar seus arquivos de reconciliação do Partner Center para obter uma exibição detalhada de item de linha de cada encargo em um ciclo de cobrança.</span><span class="sxs-lookup"><span data-stu-id="567ce-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="567ce-108">Os detalhes do item de linha incluem encargos para as assinaturas de cada cliente e eventos detalhados (como uma adição de licenças de médio prazo a uma assinatura).</span><span class="sxs-lookup"><span data-stu-id="567ce-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="567ce-109">Para obter informações sobre como ler sua **fatura**, consulte [ler sua fatura](read-your-bill.md).</span><span class="sxs-lookup"><span data-stu-id="567ce-109">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="567ce-110">Entender os campos de arquivo de reconciliação</span><span class="sxs-lookup"><span data-stu-id="567ce-110">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="567ce-111">Campos do arquivo de reconciliação baseados na licença</span><span class="sxs-lookup"><span data-stu-id="567ce-111">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="567ce-112">Campos do arquivo de reconciliação baseados no uso</span><span class="sxs-lookup"><span data-stu-id="567ce-112">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="567ce-113">Campos do arquivo de reconciliação de uso com classificação diária</span><span class="sxs-lookup"><span data-stu-id="567ce-113">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="567ce-114">Campos de arquivo de reconciliação do CSP de compra única</span><span class="sxs-lookup"><span data-stu-id="567ce-114">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="567ce-115">Entender os tipos de encargo em arquivos de reconciliação</span><span class="sxs-lookup"><span data-stu-id="567ce-115">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="567ce-116">Para entender os tipos de encargos em arquivos de reconciliação (a coluna **chargetype** ), confira [tipos de encargo de arquivo de reconciliação](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="567ce-116">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="567ce-117">Corrigir problemas de formatação</span><span class="sxs-lookup"><span data-stu-id="567ce-117">Fix formatting issues</span></span>

<span data-ttu-id="567ce-118">Ocasionalmente, um arquivo de reconciliação pode conter problemas de formatação.</span><span class="sxs-lookup"><span data-stu-id="567ce-118">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="567ce-119">Por exemplo, esse problema pode ocorrer se a localidade en-US não for usada.</span><span class="sxs-lookup"><span data-stu-id="567ce-119">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="567ce-120">Siga estas etapas para corrigir quaisquer problemas de formatação em seus arquivos de reconciliação:</span><span class="sxs-lookup"><span data-stu-id="567ce-120">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="567ce-121">Abra o arquivo de reconciliação (no formato. csv) no Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="567ce-121">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="567ce-122">Selecione a primeira coluna no arquivo.</span><span class="sxs-lookup"><span data-stu-id="567ce-122">Select the first column in the file.</span></span>
3. <span data-ttu-id="567ce-123">Abra o **Assistente para converter texto em colunas**.</span><span class="sxs-lookup"><span data-stu-id="567ce-123">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="567ce-124">Na faixa de opções, selecione **dados** e, em seguida, selecione **texto para colunas**.</span><span class="sxs-lookup"><span data-stu-id="567ce-124">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="567ce-125">No assistente, selecione **tipo de arquivo delimitado**.</span><span class="sxs-lookup"><span data-stu-id="567ce-125">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="567ce-126">Em seguida, selecione **Avançar**.</span><span class="sxs-lookup"><span data-stu-id="567ce-126">Then, select **Next**.</span></span>
5. <span data-ttu-id="567ce-127">No campo **delimitadores** , selecione **vírgula**.</span><span class="sxs-lookup"><span data-stu-id="567ce-127">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="567ce-128">(Se a **guia** já estiver selecionada, você poderá deixar essa opção selecionada.) Em seguida, selecione **Avançar**.</span><span class="sxs-lookup"><span data-stu-id="567ce-128">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="567ce-129">No campo **formato de dados da coluna** , selecione **Data: MDY**.</span><span class="sxs-lookup"><span data-stu-id="567ce-129">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="567ce-130">Em seguida, selecione **Avançar**.</span><span class="sxs-lookup"><span data-stu-id="567ce-130">Then, select **Next**.</span></span>
7. <span data-ttu-id="567ce-131">No campo **formato de dados da coluna** , selecione **texto** para todas as colunas de valor.</span><span class="sxs-lookup"><span data-stu-id="567ce-131">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="567ce-132">Em seguida, selecione **Concluir**.</span><span class="sxs-lookup"><span data-stu-id="567ce-132">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="567ce-133">Baixar arquivos de reconciliação programaticamente</span><span class="sxs-lookup"><span data-stu-id="567ce-133">Download reconciliation files programmatically</span></span>

<span data-ttu-id="567ce-134">Os arquivos de reconciliação podem ser muito grandes e, às vezes, são difíceis de baixar.</span><span class="sxs-lookup"><span data-stu-id="567ce-134">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="567ce-135">Para baixar arquivos de reconciliação programaticamente, consulte [obter itens de linha da fatura](/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="567ce-135">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a><span data-ttu-id="567ce-136">Se o arquivo exceder o limite de linha no Excel</span><span class="sxs-lookup"><span data-stu-id="567ce-136">If your file exceeds the row limit in Excel</span></span>

<span data-ttu-id="567ce-137">Se você for capaz de baixar um arquivo de reconciliação, mas não abri-lo no Microsoft Excel, provavelmente significa que o arquivo contém mais linhas do que o Excel permitirá.</span><span class="sxs-lookup"><span data-stu-id="567ce-137">If you’re able to download a reconciliation file but not open it in Microsoft Excel, it probably means the file contains more rows than Excel will allow.</span></span> <span data-ttu-id="567ce-138">Se isso acontecer, você poderá usar qualquer um dos procedimentos abaixo para abrir o arquivo.</span><span class="sxs-lookup"><span data-stu-id="567ce-138">If this happens, you can use either of the procedures below to open the file.</span></span>

### <a name="open-a-recon-file-in-power-bi"></a><span data-ttu-id="567ce-139">Abrir um arquivo reconhecimento no Power BI</span><span class="sxs-lookup"><span data-stu-id="567ce-139">Open a recon file in Power BI</span></span>

1. <span data-ttu-id="567ce-140">Baixe o arquivo de reconciliação como faria normalmente.</span><span class="sxs-lookup"><span data-stu-id="567ce-140">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="567ce-141">Baixe, instale e abra uma instância do Power BI.</span><span class="sxs-lookup"><span data-stu-id="567ce-141">Download, install, and open an instance of Power BI.</span></span>
3. <span data-ttu-id="567ce-142">Na guia Power BI **página inicial** , selecione **obter dados**.</span><span class="sxs-lookup"><span data-stu-id="567ce-142">On the Power BI **Home** tab, select **Get data**.</span></span>
4. <span data-ttu-id="567ce-143">Na lista de **fontes de dados comuns**, selecione **texto/CSV**.</span><span class="sxs-lookup"><span data-stu-id="567ce-143">In the list of **Common data sources**, select **Text/CSV**.</span></span>
5. <span data-ttu-id="567ce-144">Quando solicitado, abra o arquivo reconhecimento.</span><span class="sxs-lookup"><span data-stu-id="567ce-144">When prompted, open your recon file.</span></span>

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a><span data-ttu-id="567ce-145">Abrir um arquivo reconhecimento em uma tabela dinâmica do Excel</span><span class="sxs-lookup"><span data-stu-id="567ce-145">Open a recon file in an Excel pivot table</span></span>

1. <span data-ttu-id="567ce-146">Baixe o arquivo de reconciliação como faria normalmente.</span><span class="sxs-lookup"><span data-stu-id="567ce-146">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="567ce-147">Abra um novo arquivo no Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="567ce-147">Open a new file in Microsoft Excel.</span></span>
3. <span data-ttu-id="567ce-148">Na guia **dados** , selecione **obter dados**, selecione **do arquivo** e, em seguida, selecione **texto/CSV**.</span><span class="sxs-lookup"><span data-stu-id="567ce-148">On the **Data** tab, select **Get data**, select **From file**, and then select **Text/CSV**.</span></span>
4. <span data-ttu-id="567ce-149">Quando solicitado, abra o arquivo reconhecimento.</span><span class="sxs-lookup"><span data-stu-id="567ce-149">When prompted, open your recon file.</span></span> <span data-ttu-id="567ce-150">Seus dados serão exibidos.</span><span class="sxs-lookup"><span data-stu-id="567ce-150">Your data will appear.</span></span>
5. <span data-ttu-id="567ce-151">No menu suspenso **carregar** , selecione **carregar para** e, em seguida, **OK**.</span><span class="sxs-lookup"><span data-stu-id="567ce-151">In the **Load** dropdown menu, select **Load to**, and then **OK**.</span></span>
6. <span data-ttu-id="567ce-152">Na caixa de diálogo **importar dados** , selecione **relatório de tabela dinâmica** para abrir o arquivo.</span><span class="sxs-lookup"><span data-stu-id="567ce-152">In the **Import Data** dialog box, select **PivotTable Report** to open your file.</span></span>

## <a name="negative-amount-displayed"></a><span data-ttu-id="567ce-153">Valor negativo exibido</span><span class="sxs-lookup"><span data-stu-id="567ce-153">Negative amount displayed</span></span>

<span data-ttu-id="567ce-154">Você pode ver um valor negativo em seu arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="567ce-154">You may see a negative amount in your reconciliation file.</span></span> <span data-ttu-id="567ce-155">Isso provavelmente é causado por um dos seguintes itens:</span><span class="sxs-lookup"><span data-stu-id="567ce-155">This is probably caused by one of the following things:</span></span>

- <span data-ttu-id="567ce-156">Você cancelou recentemente ou reduziu seu número de licenças</span><span class="sxs-lookup"><span data-stu-id="567ce-156">You recently canceled or reduced your number of licenses</span></span>
- <span data-ttu-id="567ce-157">Você recebeu crédito para um SLA (contrato de licença de serviço) ou para o consumo do Azure</span><span class="sxs-lookup"><span data-stu-id="567ce-157">You received credit for either a service license agreement (SLA) or for Azure consumption</span></span>

<span data-ttu-id="567ce-158">Para obter mais informações sobre essa transação, examine seu atributo de tipo de encargo em seu arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="567ce-158">To get more information about this transaction, review its charge type attribute in your reconciliation file.</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="567ce-159">Impostos do mapa ou IVA</span><span class="sxs-lookup"><span data-stu-id="567ce-159">Map taxes or VAT</span></span>

<span data-ttu-id="567ce-160">Para mapear impostos ou IVA (imposto sobre valor agregado) para sua fatura:</span><span class="sxs-lookup"><span data-stu-id="567ce-160">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="567ce-161">Some a coluna de **impostos** do arquivo baseado em licença.</span><span class="sxs-lookup"><span data-stu-id="567ce-161">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="567ce-162">Some a coluna **TaxAmount** do arquivo baseado em uso.</span><span class="sxs-lookup"><span data-stu-id="567ce-162">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="567ce-163">Discriminar arquivos de reconciliação por parceiro</span><span class="sxs-lookup"><span data-stu-id="567ce-163">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="567ce-164">Os parceiros no **modelo indireto** podem usar esses campos adicionais em arquivos de reconciliação baseados em licença e de uso para discriminar os arquivos pelo revendedor.</span><span class="sxs-lookup"><span data-stu-id="567ce-164">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="567ce-165">ID MPN</span><span class="sxs-lookup"><span data-stu-id="567ce-165">MPN ID</span></span> | <span data-ttu-id="567ce-166">Descrição</span><span class="sxs-lookup"><span data-stu-id="567ce-166">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="567ce-167">ID MPN</span><span class="sxs-lookup"><span data-stu-id="567ce-167">MPN ID</span></span> | <span data-ttu-id="567ce-168">O identificador de Microsoft Partner Network (MPN) do parceiro CSP (provedor de soluções na nuvem) (direto ou indireto).</span><span class="sxs-lookup"><span data-stu-id="567ce-168">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="567ce-169">ID do MPN do revendedor</span><span class="sxs-lookup"><span data-stu-id="567ce-169">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="567ce-170">O [identificador de MPN do revendedor do registro para a assinatura](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="567ce-170">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="567ce-171">Este campo corresponde à ID do revendedor listada para a assinatura específica no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="567ce-171">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="567ce-172">Só aparece em arquivos de reconciliação para parceiros no modelo indireto.</span><span class="sxs-lookup"><span data-stu-id="567ce-172">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="567ce-173">ID do MPN do revendedor</span><span class="sxs-lookup"><span data-stu-id="567ce-173">Reseller MPN ID</span></span>

<span data-ttu-id="567ce-174">Se um parceiro CSP vendeu a assinatura diretamente ao cliente, sua **ID MPN** é listada duas vezes, como a **ID MPN** e a **ID de MPN do revendedor**.</span><span class="sxs-lookup"><span data-stu-id="567ce-174">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="567ce-175">Se um parceiro CSP tiver um revendedor sem **ID MPN**, esse valor será definido como a ID de **MPN** do parceiro em vez disso.</span><span class="sxs-lookup"><span data-stu-id="567ce-175">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="567ce-176">Se o parceiro CSP remover uma **ID de MPN do revendedor**, esse valor será definido como *-1*.</span><span class="sxs-lookup"><span data-stu-id="567ce-176">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="567ce-177">Para exibir ou atualizar a **ID de MPN do revendedor**:</span><span class="sxs-lookup"><span data-stu-id="567ce-177">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="567ce-178">Conecte-se ao Partner Center.</span><span class="sxs-lookup"><span data-stu-id="567ce-178">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="567ce-179">No menu Partner Center, selecione **Clientes**.</span><span class="sxs-lookup"><span data-stu-id="567ce-179">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="567ce-180">Escolha o cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="567ce-180">Choose the customer from the list.</span></span>
4. <span data-ttu-id="567ce-181">No menu cliente, selecione **assinaturas**.</span><span class="sxs-lookup"><span data-stu-id="567ce-181">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="567ce-182">Escolha a assinatura na lista.</span><span class="sxs-lookup"><span data-stu-id="567ce-182">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="567ce-183">Selecione **Atualizar** para alterar o **Revendedor (ID do MPN)**.</span><span class="sxs-lookup"><span data-stu-id="567ce-183">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="567ce-184">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="567ce-184">Next steps</span></span>

- [<span data-ttu-id="567ce-185">Como ler o arquivo Bill & reconhecimento</span><span class="sxs-lookup"><span data-stu-id="567ce-185">How to read your bill & recon file</span></span>](read-your-bill.md) 