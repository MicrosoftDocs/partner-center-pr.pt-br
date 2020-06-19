---
title: Usar seus arquivos de reconciliação
ms.topic: article
ms.date: 06/08/2020
description: Saiba mais sobre os arquivos de reconciliação no Partner Center e como interpretar as exibições detalhadas de item de linha de encargos para um determinado ciclo de cobrança.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f52c0b3d53fde6d5b5f68c54f8967e26a33b8c76
ms.sourcegitcommit: e0a1b4506840486f4bb82620051e0f6a5e81662a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "84991768"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="edead-103">Saiba como ler os itens de linha em seus arquivos de reconciliação do Partner Center</span><span class="sxs-lookup"><span data-stu-id="edead-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="edead-104">Aplica-se a:</span><span class="sxs-lookup"><span data-stu-id="edead-104">Applies to:</span></span>

- <span data-ttu-id="edead-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="edead-105">Partner Center</span></span>
- <span data-ttu-id="edead-106">Partner Center do Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="edead-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="edead-107">Você pode baixar seus arquivos de reconciliação do Partner Center para obter uma exibição detalhada de item de linha de cada encargo em um ciclo de cobrança.</span><span class="sxs-lookup"><span data-stu-id="edead-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="edead-108">Os detalhes do item de linha incluem encargos para as assinaturas de cada cliente e eventos detalhados (como uma adição de estações de mercado para uma assinatura).</span><span class="sxs-lookup"><span data-stu-id="edead-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

<span data-ttu-id="edead-109">Funções apropriadas:</span><span class="sxs-lookup"><span data-stu-id="edead-109">Appropriate roles:</span></span>

- <span data-ttu-id="edead-110">Administrador de cobrança</span><span class="sxs-lookup"><span data-stu-id="edead-110">Billing admin</span></span>
- <span data-ttu-id="edead-111">Administrador global</span><span class="sxs-lookup"><span data-stu-id="edead-111">Global admin</span></span>

<span data-ttu-id="edead-112">Para obter informações sobre como ler sua **fatura**, consulte [ler sua fatura](read-your-bill.md).</span><span class="sxs-lookup"><span data-stu-id="edead-112">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="edead-113">Entender os campos de arquivo de reconciliação</span><span class="sxs-lookup"><span data-stu-id="edead-113">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="edead-114">Campos de arquivo de reconciliação com base em licença</span><span class="sxs-lookup"><span data-stu-id="edead-114">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="edead-115">Campos de arquivo de reconciliação com base no uso</span><span class="sxs-lookup"><span data-stu-id="edead-115">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="edead-116">Campos de arquivo de reconciliação recorrentes e de uso único</span><span class="sxs-lookup"><span data-stu-id="edead-116">One-time and recurring reconciliation file fields</span></span>](one-time-recurring-recon-files.md)
- [<span data-ttu-id="edead-117">Campos de arquivo de reconciliação de uso com classificação diária</span><span class="sxs-lookup"><span data-stu-id="edead-117">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="edead-118">Entender os tipos de encargo em arquivos de reconciliação</span><span class="sxs-lookup"><span data-stu-id="edead-118">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="edead-119">Para entender os tipos de encargos em arquivos de reconciliação (a coluna **chargetype** ), confira [tipos de encargo de arquivo de reconciliação](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="edead-119">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="edead-120">Corrigir problemas de formatação</span><span class="sxs-lookup"><span data-stu-id="edead-120">Fix formatting issues</span></span>

<span data-ttu-id="edead-121">Ocasionalmente, um arquivo de reconciliação pode conter problemas de formatação.</span><span class="sxs-lookup"><span data-stu-id="edead-121">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="edead-122">Por exemplo, esse problema pode ocorrer se a localidade en-US não for usada.</span><span class="sxs-lookup"><span data-stu-id="edead-122">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="edead-123">Siga estas etapas para corrigir quaisquer problemas de formatação em seus arquivos de reconciliação:</span><span class="sxs-lookup"><span data-stu-id="edead-123">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="edead-124">Abra o arquivo de reconciliação (no formato. csv) no Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="edead-124">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="edead-125">Selecione a primeira coluna no arquivo.</span><span class="sxs-lookup"><span data-stu-id="edead-125">Select the first column in the file.</span></span>
3. <span data-ttu-id="edead-126">Abra o **Assistente para converter texto em colunas**.</span><span class="sxs-lookup"><span data-stu-id="edead-126">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="edead-127">Na faixa de opções, selecione **dados**e, em seguida, selecione **texto para colunas**.</span><span class="sxs-lookup"><span data-stu-id="edead-127">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="edead-128">No assistente, selecione **tipo de arquivo delimitado**.</span><span class="sxs-lookup"><span data-stu-id="edead-128">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="edead-129">Em seguida, selecione **Avançar**.</span><span class="sxs-lookup"><span data-stu-id="edead-129">Then, select **Next**.</span></span>
5. <span data-ttu-id="edead-130">No campo **delimitadores** , selecione **vírgula**.</span><span class="sxs-lookup"><span data-stu-id="edead-130">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="edead-131">(Se a **guia** já estiver selecionada, você poderá deixar essa opção selecionada.) Em seguida, selecione **Avançar**.</span><span class="sxs-lookup"><span data-stu-id="edead-131">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="edead-132">No campo **formato de dados da coluna** , selecione **Data: MDY**.</span><span class="sxs-lookup"><span data-stu-id="edead-132">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="edead-133">Em seguida, selecione **Avançar**.</span><span class="sxs-lookup"><span data-stu-id="edead-133">Then, select **Next**.</span></span>
7. <span data-ttu-id="edead-134">No campo **formato de dados da coluna** , selecione **texto** para todas as colunas de valor.</span><span class="sxs-lookup"><span data-stu-id="edead-134">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="edead-135">Em seguida, selecione **Concluir**.</span><span class="sxs-lookup"><span data-stu-id="edead-135">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="edead-136">Baixar arquivos de reconciliação programaticamente</span><span class="sxs-lookup"><span data-stu-id="edead-136">Download reconciliation files programmatically</span></span>

<span data-ttu-id="edead-137">Os arquivos de reconciliação podem ser muito grandes e, às vezes, são difíceis de baixar.</span><span class="sxs-lookup"><span data-stu-id="edead-137">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="edead-138">Para baixar arquivos de reconciliação programaticamente, consulte [obter itens de linha da fatura](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="edead-138">To download reconciliation files programmatically, see [Get invoice line items](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="edead-139">Impostos do mapa ou IVA</span><span class="sxs-lookup"><span data-stu-id="edead-139">Map taxes or VAT</span></span>

<span data-ttu-id="edead-140">Para mapear impostos ou IVA (imposto sobre valor agregado) para sua fatura:</span><span class="sxs-lookup"><span data-stu-id="edead-140">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="edead-141">Some a coluna de **impostos** do arquivo baseado em licença.</span><span class="sxs-lookup"><span data-stu-id="edead-141">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="edead-142">Some a coluna **TaxAmount** do arquivo baseado em uso.</span><span class="sxs-lookup"><span data-stu-id="edead-142">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="edead-143">Discriminar arquivos de reconciliação por parceiro</span><span class="sxs-lookup"><span data-stu-id="edead-143">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="edead-144">Os parceiros no **modelo indireto** podem usar esses campos adicionais em arquivos de reconciliação baseados em licença e de uso para discriminar os arquivos pelo revendedor.</span><span class="sxs-lookup"><span data-stu-id="edead-144">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="edead-145">ID MPN</span><span class="sxs-lookup"><span data-stu-id="edead-145">MPN ID</span></span> | <span data-ttu-id="edead-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="edead-146">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="edead-147">ID MPN</span><span class="sxs-lookup"><span data-stu-id="edead-147">MPN ID</span></span> | <span data-ttu-id="edead-148">O identificador de Microsoft Partner Network (MPN) do parceiro CSP (provedor de soluções na nuvem) (direto ou indireto).</span><span class="sxs-lookup"><span data-stu-id="edead-148">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="edead-149">ID do MPN do revendedor</span><span class="sxs-lookup"><span data-stu-id="edead-149">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="edead-150">O [identificador de MPN do revendedor do registro para a assinatura](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="edead-150">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="edead-151">Este campo corresponde à ID do revendedor listada para a assinatura específica no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="edead-151">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="edead-152">Só aparece em arquivos de reconciliação para parceiros no modelo indireto.</span><span class="sxs-lookup"><span data-stu-id="edead-152">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="edead-153">ID do MPN do revendedor</span><span class="sxs-lookup"><span data-stu-id="edead-153">Reseller MPN ID</span></span>

<span data-ttu-id="edead-154">Se um parceiro CSP vendeu a assinatura diretamente ao cliente, sua **ID MPN** é listada duas vezes, como a **ID MPN** e a **ID de MPN do revendedor**.</span><span class="sxs-lookup"><span data-stu-id="edead-154">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="edead-155">Se um parceiro CSP tiver um revendedor sem **ID MPN**, esse valor será definido como a ID de **MPN** do parceiro em vez disso.</span><span class="sxs-lookup"><span data-stu-id="edead-155">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="edead-156">Se o parceiro CSP remover uma **ID de MPN do revendedor**, esse valor será definido como *-1*.</span><span class="sxs-lookup"><span data-stu-id="edead-156">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="edead-157">Para exibir ou atualizar a **ID de MPN do revendedor**:</span><span class="sxs-lookup"><span data-stu-id="edead-157">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="edead-158">Conecte-se ao Partner Center.</span><span class="sxs-lookup"><span data-stu-id="edead-158">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="edead-159">No menu Partner Center, selecione **Clientes**.</span><span class="sxs-lookup"><span data-stu-id="edead-159">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="edead-160">Escolha o cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="edead-160">Choose the customer from the list.</span></span>
4. <span data-ttu-id="edead-161">No menu cliente, selecione **assinaturas**.</span><span class="sxs-lookup"><span data-stu-id="edead-161">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="edead-162">Escolha a assinatura na lista.</span><span class="sxs-lookup"><span data-stu-id="edead-162">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="edead-163">Selecione **Atualizar** para alterar o **Revendedor (ID do MPN)**.</span><span class="sxs-lookup"><span data-stu-id="edead-163">Select **update** to change the **Reseller (MPN ID)**.</span></span>
