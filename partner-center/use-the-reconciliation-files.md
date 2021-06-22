---
title: Usar seus arquivos de reconciliação
ms.topic: article
ms.date: 03/26/2021
description: Saiba mais sobre arquivos de reconciliação Partner Center e como interpretar as exibições detalhadas de itens de linha de encargos para um determinado ciclo de cobrança.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1a7d5f3169c4b338a07475a7e246e87841b8dcfb
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431566"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="b36d0-103">Saiba como ler os itens de linha em seus arquivos Partner Center reconciliação</span><span class="sxs-lookup"><span data-stu-id="b36d0-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="b36d0-104">**Funções apropriadas:** administração de cobrança | Administrador global</span><span class="sxs-lookup"><span data-stu-id="b36d0-104">**Appropriate roles**: Billing admin | Global admin</span></span>

<span data-ttu-id="b36d0-105">Você pode baixar seus arquivos de reconciliação Partner Center para uma exibição detalhada de item de linha de cada cobrança em um ciclo de cobrança.</span><span class="sxs-lookup"><span data-stu-id="b36d0-105">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="b36d0-106">Os detalhes do item de linha incluem encargos para assinaturas de cada cliente e eventos detalhados (como uma adição de licenças de médio prazo a uma assinatura).</span><span class="sxs-lookup"><span data-stu-id="b36d0-106">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="b36d0-107">Para obter informações sobre como ler sua **fatura,** consulte [Ler sua fatura.](read-your-bill.md)</span><span class="sxs-lookup"><span data-stu-id="b36d0-107">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="b36d0-108">Entender os campos do arquivo de reconciliação</span><span class="sxs-lookup"><span data-stu-id="b36d0-108">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="b36d0-109">Campos do arquivo de reconciliação baseados na licença</span><span class="sxs-lookup"><span data-stu-id="b36d0-109">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="b36d0-110">Campos do arquivo de reconciliação baseados no uso</span><span class="sxs-lookup"><span data-stu-id="b36d0-110">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="b36d0-111">Campos do arquivo de reconciliação de uso com classificação diária</span><span class="sxs-lookup"><span data-stu-id="b36d0-111">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="b36d0-112">Campos de arquivo de reconciliação do CSP de compra única</span><span class="sxs-lookup"><span data-stu-id="b36d0-112">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="b36d0-113">Entender os tipos de cobrança em arquivos de reconciliação</span><span class="sxs-lookup"><span data-stu-id="b36d0-113">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="b36d0-114">Para entender os tipos de encargos em arquivos de reconciliação (a **coluna ChargeType),** consulte Tipos de cobrança de arquivo [de reconciliação](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="b36d0-114">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="b36d0-115">Corrigir problemas de formatação</span><span class="sxs-lookup"><span data-stu-id="b36d0-115">Fix formatting issues</span></span>

<span data-ttu-id="b36d0-116">Ocasionalmente, um arquivo de reconciliação pode conter problemas de formatação.</span><span class="sxs-lookup"><span data-stu-id="b36d0-116">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="b36d0-117">Por exemplo, esse problema poderá ocorrer se a localidade en-US não for usada.</span><span class="sxs-lookup"><span data-stu-id="b36d0-117">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="b36d0-118">Siga estas etapas para corrigir problemas de formatação em seus arquivos de reconciliação:</span><span class="sxs-lookup"><span data-stu-id="b36d0-118">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="b36d0-119">Abra o arquivo de reconciliação (no .csv) no Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="b36d0-119">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="b36d0-120">Selecione a primeira coluna no arquivo.</span><span class="sxs-lookup"><span data-stu-id="b36d0-120">Select the first column in the file.</span></span>
3. <span data-ttu-id="b36d0-121">Abra o **Assistente para Converter Texto em Colunas**.</span><span class="sxs-lookup"><span data-stu-id="b36d0-121">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="b36d0-122">Na faixa de opções, selecione **Dados** e, em **seguida, selecione Texto em Colunas.**</span><span class="sxs-lookup"><span data-stu-id="b36d0-122">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="b36d0-123">No assistente, selecione **Tipo de arquivo delimitado**.</span><span class="sxs-lookup"><span data-stu-id="b36d0-123">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="b36d0-124">Em seguida, selecione **Avançar**.</span><span class="sxs-lookup"><span data-stu-id="b36d0-124">Then, select **Next**.</span></span>
5. <span data-ttu-id="b36d0-125">No campo **Delimitadores,** selecione **Vírgula**.</span><span class="sxs-lookup"><span data-stu-id="b36d0-125">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="b36d0-126">(Se **Tab** já estiver selecionado, você poderá deixar essa opção selecionada.) Em seguida, selecione **Próximo.**</span><span class="sxs-lookup"><span data-stu-id="b36d0-126">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="b36d0-127">No campo **Formato de dados da** coluna, selecione **Data:MDY.**</span><span class="sxs-lookup"><span data-stu-id="b36d0-127">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="b36d0-128">Em seguida, selecione **Avançar**.</span><span class="sxs-lookup"><span data-stu-id="b36d0-128">Then, select **Next**.</span></span>
7. <span data-ttu-id="b36d0-129">No campo **Formato de dados de** coluna, selecione Texto **para** todas as colunas de valor.</span><span class="sxs-lookup"><span data-stu-id="b36d0-129">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="b36d0-130">Em seguida, selecione **Concluir**.</span><span class="sxs-lookup"><span data-stu-id="b36d0-130">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="b36d0-131">Baixar arquivos de reconciliação programaticamente</span><span class="sxs-lookup"><span data-stu-id="b36d0-131">Download reconciliation files programmatically</span></span>

<span data-ttu-id="b36d0-132">Os arquivos de reconciliação podem ser muito grandes e, às vezes, são difíceis de baixar.</span><span class="sxs-lookup"><span data-stu-id="b36d0-132">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="b36d0-133">Para baixar arquivos de reconciliação programaticamente, consulte [Obter itens de linha da fatura](/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="b36d0-133">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a><span data-ttu-id="b36d0-134">Se o arquivo exceder o limite de linha no Excel</span><span class="sxs-lookup"><span data-stu-id="b36d0-134">If your file exceeds the row limit in Excel</span></span>

<span data-ttu-id="b36d0-135">Se você conseguir baixar um arquivo de reconciliação, mas não abri-lo no Microsoft Excel, isso provavelmente significa que o arquivo contém mais linhas do que o Excel permitirá.</span><span class="sxs-lookup"><span data-stu-id="b36d0-135">If you’re able to download a reconciliation file but not open it in Microsoft Excel, it probably means the file contains more rows than Excel will allow.</span></span> <span data-ttu-id="b36d0-136">Se isso acontecer, você poderá usar qualquer um dos procedimentos abaixo para abrir o arquivo.</span><span class="sxs-lookup"><span data-stu-id="b36d0-136">If this happens, you can use either of the procedures below to open the file.</span></span>

### <a name="open-a-recon-file-in-power-bi"></a><span data-ttu-id="b36d0-137">Abra um arquivo de reconhecimento no Power BI</span><span class="sxs-lookup"><span data-stu-id="b36d0-137">Open a recon file in Power BI</span></span>

1. <span data-ttu-id="b36d0-138">Baixe o arquivo de reconciliação como faria normalmente.</span><span class="sxs-lookup"><span data-stu-id="b36d0-138">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="b36d0-139">Baixe, instale e abra uma instância do Microsoft Power BI.</span><span class="sxs-lookup"><span data-stu-id="b36d0-139">Download, install, and open an instance of Microsoft Power BI.</span></span>
3. <span data-ttu-id="b36d0-140">Na guia Power BI **Página** Base, selecione **Obter dados**.</span><span class="sxs-lookup"><span data-stu-id="b36d0-140">On the Power BI **Home** tab, select **Get data**.</span></span>
4. <span data-ttu-id="b36d0-141">Na lista de fontes **de dados comuns,** selecione **Texto/CSV.**</span><span class="sxs-lookup"><span data-stu-id="b36d0-141">In the list of **Common data sources**, select **Text/CSV**.</span></span>
5. <span data-ttu-id="b36d0-142">Quando solicitado, abra o arquivo de reconhecimento.</span><span class="sxs-lookup"><span data-stu-id="b36d0-142">When prompted, open your recon file.</span></span>

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a><span data-ttu-id="b36d0-143">Abrir um arquivo de reconhecimento em uma tabela dinâmica do Excel</span><span class="sxs-lookup"><span data-stu-id="b36d0-143">Open a recon file in an Excel pivot table</span></span>

1. <span data-ttu-id="b36d0-144">Baixe o arquivo de reconciliação como faria normalmente.</span><span class="sxs-lookup"><span data-stu-id="b36d0-144">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="b36d0-145">Abra um novo arquivo no Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="b36d0-145">Open a new file in Microsoft Excel.</span></span>
3. <span data-ttu-id="b36d0-146">Na guia **Dados,** selecione **Obter dados,** selecione **Do arquivo** e, em seguida, **selecione Texto/CSV.**</span><span class="sxs-lookup"><span data-stu-id="b36d0-146">On the **Data** tab, select **Get data**, select **From file**, and then select **Text/CSV**.</span></span>
4. <span data-ttu-id="b36d0-147">Quando solicitado, abra o arquivo de reconhecimento.</span><span class="sxs-lookup"><span data-stu-id="b36d0-147">When prompted, open your recon file.</span></span> <span data-ttu-id="b36d0-148">Seus dados serão exibidos.</span><span class="sxs-lookup"><span data-stu-id="b36d0-148">Your data will appear.</span></span>
5. <span data-ttu-id="b36d0-149">No menu **suspenso** Carregar, selecione **Carregar para** e, em seguida, selecione **OK.**</span><span class="sxs-lookup"><span data-stu-id="b36d0-149">In the **Load** dropdown menu, select **Load to**, and then select **OK**.</span></span>
6. <span data-ttu-id="b36d0-150">Na caixa **de diálogo Importar** Dados, selecione Relatório de Tabela **Dinâmica** para abrir o arquivo.</span><span class="sxs-lookup"><span data-stu-id="b36d0-150">In the **Import Data** dialog box, select **PivotTable Report** to open your file.</span></span>

## <a name="negative-amount-displayed"></a><span data-ttu-id="b36d0-151">Valor negativo exibido</span><span class="sxs-lookup"><span data-stu-id="b36d0-151">Negative amount displayed</span></span>

<span data-ttu-id="b36d0-152">Você pode ver uma quantidade negativa em seu arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="b36d0-152">You may see a negative amount in your reconciliation file.</span></span> <span data-ttu-id="b36d0-153">As causas podem ser:</span><span class="sxs-lookup"><span data-stu-id="b36d0-153">This is probably caused by one of the following things:</span></span>

- <span data-ttu-id="b36d0-154">Você cancelou ou reduziu recentemente seu número de licenças</span><span class="sxs-lookup"><span data-stu-id="b36d0-154">You recently canceled or reduced your number of licenses</span></span>
- <span data-ttu-id="b36d0-155">Você recebeu crédito por um SLA (Contrato de Licença de Serviço) ou pelo consumo do Azure</span><span class="sxs-lookup"><span data-stu-id="b36d0-155">You received credit for either a service license agreement (SLA) or for Azure consumption</span></span>

<span data-ttu-id="b36d0-156">Confira mais informações sobre essa transação examinando o atributo de tipo de encargo em seu arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="b36d0-156">To get more information about this transaction, review its charge type attribute in your reconciliation file.</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="b36d0-157">Mapear impostos ou IVA</span><span class="sxs-lookup"><span data-stu-id="b36d0-157">Map taxes or VAT</span></span>

<span data-ttu-id="b36d0-158">Para mapear os impostos ou o IVA (imposto sobre valor agregado) para sua fatura:</span><span class="sxs-lookup"><span data-stu-id="b36d0-158">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="b36d0-159">Soma a **coluna Imposto** do arquivo baseado em licença.</span><span class="sxs-lookup"><span data-stu-id="b36d0-159">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="b36d0-160">Soma a **coluna TaxAmount** do arquivo baseado em uso.</span><span class="sxs-lookup"><span data-stu-id="b36d0-160">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="b36d0-161">Itemizar arquivos de reconciliação por parceiro</span><span class="sxs-lookup"><span data-stu-id="b36d0-161">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="b36d0-162">Os parceiros no **modelo indireto** podem usar esses campos adicionais em arquivos de reconciliação baseados em licença e em uso para itemizar os arquivos por revendedor.</span><span class="sxs-lookup"><span data-stu-id="b36d0-162">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="b36d0-163">ID MPN</span><span class="sxs-lookup"><span data-stu-id="b36d0-163">MPN ID</span></span> | <span data-ttu-id="b36d0-164">Descrição</span><span class="sxs-lookup"><span data-stu-id="b36d0-164">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="b36d0-165">ID MPN</span><span class="sxs-lookup"><span data-stu-id="b36d0-165">MPN ID</span></span> | <span data-ttu-id="b36d0-166">O Microsoft Partner Network (MPN) do parceiro Provedor de Soluções na Nuvem (CSP) (direto ou indireto).</span><span class="sxs-lookup"><span data-stu-id="b36d0-166">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="b36d0-167">ID do MPN do revendedor</span><span class="sxs-lookup"><span data-stu-id="b36d0-167">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="b36d0-168">O [identificador MPN do revendedor de registro para a assinatura](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="b36d0-168">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="b36d0-169">Esse campo corresponde à ID do revendedor listada para a assinatura específica no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="b36d0-169">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="b36d0-170">Só aparece em arquivos de reconciliação para parceiros no modelo indireto.</span><span class="sxs-lookup"><span data-stu-id="b36d0-170">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="b36d0-171">ID do MPN do revendedor</span><span class="sxs-lookup"><span data-stu-id="b36d0-171">Reseller MPN ID</span></span>

<span data-ttu-id="b36d0-172">Se um parceiro CSP vender a assinatura diretamente para o cliente, sua ID do **MPN** será listada duas vezes, como a **ID** do MPN e a ID do **MPN do Revendedor.**</span><span class="sxs-lookup"><span data-stu-id="b36d0-172">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="b36d0-173">Se um parceiro CSP tiver um revendedor sem ID do **MPN,** esse valor será definido como a ID do **MPN do** parceiro.</span><span class="sxs-lookup"><span data-stu-id="b36d0-173">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="b36d0-174">Se o parceiro CSP remover uma **ID do MPN** do Revendedor, esse valor será definido como *-1*.</span><span class="sxs-lookup"><span data-stu-id="b36d0-174">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="b36d0-175">Para exibir ou atualizar a **ID do MPN do Revendedor:**</span><span class="sxs-lookup"><span data-stu-id="b36d0-175">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="b36d0-176">Conecte-se ao Partner Center.</span><span class="sxs-lookup"><span data-stu-id="b36d0-176">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="b36d0-177">No menu Partner Center, selecione **Clientes**.</span><span class="sxs-lookup"><span data-stu-id="b36d0-177">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="b36d0-178">Escolha o cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="b36d0-178">Choose the customer from the list.</span></span>
4. <span data-ttu-id="b36d0-179">No menu do cliente, selecione **Assinaturas**.</span><span class="sxs-lookup"><span data-stu-id="b36d0-179">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="b36d0-180">Escolha a assinatura na lista.</span><span class="sxs-lookup"><span data-stu-id="b36d0-180">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="b36d0-181">Selecione **Atualizar** para alterar o **Revendedor (ID do MPN)**.</span><span class="sxs-lookup"><span data-stu-id="b36d0-181">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="b36d0-182">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="b36d0-182">Next steps</span></span>

- [<span data-ttu-id="b36d0-183">Como ler seu arquivo de & reconhecimento</span><span class="sxs-lookup"><span data-stu-id="b36d0-183">How to read your bill & recon file</span></span>](read-your-bill.md) 