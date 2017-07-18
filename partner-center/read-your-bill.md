---
title: "Ler sua cobrança | Partner Center"
description: "Sua fatura é um resumo de todos os encargos (entre programa, produtos e clientes) para o período atual mensal. Está disponível no painel do Partner Center."
ms.assetid: E1BA3415-732F-4385-8996-5E79E200F7F7
author: MaggiePucciEvans
ms.openlocfilehash: 65c3777c0bd35933f2622fc0de105c051001974e
ms.sourcegitcommit: e8b504fa98b3ec4c7c8fd954f63ea81299791906
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2017
---
# <a name="read-your-bill"></a><span data-ttu-id="04825-104">Ler sua cobrança</span><span class="sxs-lookup"><span data-stu-id="04825-104">Read your bill</span></span>

**<span data-ttu-id="04825-105">Aplicável a</span><span class="sxs-lookup"><span data-stu-id="04825-105">Applies to</span></span>**

-  <span data-ttu-id="04825-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="04825-106">Partner Center</span></span>
-  <span data-ttu-id="04825-107">Partner Center for Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="04825-107">Partner Center for Microsoft Cloud for US Government</span></span>
-  <span data-ttu-id="04825-108">Partner Center for Microsoft Cloud Germany</span><span class="sxs-lookup"><span data-stu-id="04825-108">Partner Center for Microsoft Cloud Germany</span></span>

<span data-ttu-id="04825-109">Sua fatura é um resumo de todos os encargos (entre programa, produtos e clientes) para o período atual mensal.</span><span class="sxs-lookup"><span data-stu-id="04825-109">Your invoice is a summary of all charges (across the program, products, and customers) for the current monthly period.</span></span> <span data-ttu-id="04825-110">Está disponível no painel do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="04825-110">It is available on the Partner Center Dashboard.</span></span>

<span data-ttu-id="04825-111">Para obter detalhes por itens sobre os encargos, use os arquivos de reconciliação acompanhantes.</span><span class="sxs-lookup"><span data-stu-id="04825-111">For itemized details about the charges, use the accompanying reconciliation files.</span></span> <span data-ttu-id="04825-112">Os arquivos de reconciliação contêm os IDs de clientes e assinaturas que você usará para criar as faturas dos clientes.</span><span class="sxs-lookup"><span data-stu-id="04825-112">The reconciliation files include the customer IDs and subscription IDs that you will use to create customer invoices.</span></span> <span data-ttu-id="04825-113">Para obter mais informações, consulte [Como usar os arquivos de reconciliação](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="04825-113">For more information, see [How to use the reconciliation files](use-the-reconciliation-files.md).</span></span>

## <a name="invoice-file-definitions"></a><span data-ttu-id="04825-114">Definições do arquivo de fatura</span><span class="sxs-lookup"><span data-stu-id="04825-114">Invoice file definitions</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="04825-115">Campo</span><span class="sxs-lookup"><span data-stu-id="04825-115">Field</span></span></strong></td>
<td><strong><span data-ttu-id="04825-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="04825-116">Description</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="04825-117">EUA FEIN</span><span class="sxs-lookup"><span data-stu-id="04825-117">US FEIN</span></span></td>
<td><span data-ttu-id="04825-118">O ID do Imposto Federal.</span><span class="sxs-lookup"><span data-stu-id="04825-118">Your Federal Tax ID Number.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="04825-119">Número do cliente</span><span class="sxs-lookup"><span data-stu-id="04825-119">Customer number</span></span></td>
<td><span data-ttu-id="04825-120">Seu número do cliente.</span><span class="sxs-lookup"><span data-stu-id="04825-120">Your customer number.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="04825-121">Cobrar de</span><span class="sxs-lookup"><span data-stu-id="04825-121">Bill to</span></span></td>
<td><span data-ttu-id="04825-122">O endereço onde podemos enviar sua fatura.</span><span class="sxs-lookup"><span data-stu-id="04825-122">The address where we send your invoice.</span></span> <span data-ttu-id="04825-123">Para alterar esse endereço, edite seu perfil da conta do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="04825-123">To change this address, edit your Partner Center account profile.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="04825-124">Encargos recorrentes</span><span class="sxs-lookup"><span data-stu-id="04825-124">Recurring charges</span></span></td>
<td><span data-ttu-id="04825-125">Os encargos mensais (ou anuais) fixos das licenças baseadas em uso compradas, cobradas antecipadamente pelo serviço.</span><span class="sxs-lookup"><span data-stu-id="04825-125">The flat monthly (or annual) charges for the purchased usage-based licenses, billed in advance of the service.</span></span> <span data-ttu-id="04825-126">Esse número é a soma de todos os encargos da coluna &quot;Subtotal&quot; no arquivo de reconciliação com base em licença (coluna T).</span><span class="sxs-lookup"><span data-stu-id="04825-126">This number is the sum of all charges in the &quot;Subtotal&quot; column in the License-based reconciliation file (column T).</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="04825-127">Tarifas de uso</span><span class="sxs-lookup"><span data-stu-id="04825-127">Usage charges</span></span></td>
<td><span data-ttu-id="04825-128">Uso do Azure, incluindo novos serviços ou aplicativos habilitados e usados durante o mês de cobrança.</span><span class="sxs-lookup"><span data-stu-id="04825-128">Azure usage, including new services or applications enabled and used during the billing month.</span></span> <span data-ttu-id="04825-129">Esse número é a soma de todos os encargos na coluna &quot;PretaxCharges&quot; no arquivo de reconciliação com base em uso (coluna Z).</span><span class="sxs-lookup"><span data-stu-id="04825-129">This number is the sum of all charges in the &quot;PretaxCharges&quot; column in the Usage-based reconciliation file (column Z).</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="04825-130">Créditos e ajustes</span><span class="sxs-lookup"><span data-stu-id="04825-130">Credits &amp; adjustments</span></span></td>
<td><span data-ttu-id="04825-131">Créditos ou ajustes para alterações de assinaturas (exemplo: aumentos ou diminuição de assento).</span><span class="sxs-lookup"><span data-stu-id="04825-131">Credits or adjustments for changes made to subscriptions (example: seat increases or decreases).</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="04825-132">Outros descontos</span><span class="sxs-lookup"><span data-stu-id="04825-132">Other discounts</span></span></td>
<td><span data-ttu-id="04825-133">Por exemplo, o desconto que o cliente recebe do preço normal da assinatura.</span><span class="sxs-lookup"><span data-stu-id="04825-133">For example, the discount that the customer receives from the normal price of the subscription.</span></span> <span data-ttu-id="04825-134">Isso é mostrado como um valor simples, não como um preço por unidade ou licença.</span><span class="sxs-lookup"><span data-stu-id="04825-134">This is shown as a flat amount, not as a price per unit or license.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="04825-135">Impostos</span><span class="sxs-lookup"><span data-stu-id="04825-135">Taxes</span></span></td>
<td><span data-ttu-id="04825-136">O total de imposto para os encargos atuais como o total no início da seção detalhes na página 2 da fatura.</span><span class="sxs-lookup"><span data-stu-id="04825-136">The total tax for the current charges as totaled in the details section beginning on page 2 of the invoice.</span></span> <span data-ttu-id="04825-137">Esse número é a soma de todos os encargos na:</span><span class="sxs-lookup"><span data-stu-id="04825-137">This number is the sum of all the charges in:</span></span>
<ul>
<li><span data-ttu-id="04825-138">coluna &quot;TaxAmount&quot; do arquivo de reconciliação com base em uso (coluna AA), e</span><span class="sxs-lookup"><span data-stu-id="04825-138">the &quot;TaxAmount&quot; column of the Usage-based reconciliation file (column AA), and</span></span></li>
<li><span data-ttu-id="04825-139">coluna &quot;Tax&quot; do arquivo com base em licença (coluna U).</span><span class="sxs-lookup"><span data-stu-id="04825-139">the &quot;Tax&quot; column of the License-based file (column U).</span></span></li>
</ul></td>
</tr>
<tr class="even">
<td><span data-ttu-id="04825-140">Total dos encargos atuais</span><span class="sxs-lookup"><span data-stu-id="04825-140">Total current charges</span></span></td>
<td><span data-ttu-id="04825-141">O valor devido em moeda de cobrança para o período de faturamento, pago no dia do vencimento.</span><span class="sxs-lookup"><span data-stu-id="04825-141">The amount due in your billing currency for the billing period, due by the payment due date.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="04825-142">Instruções de pagamento</span><span class="sxs-lookup"><span data-stu-id="04825-142">Payment instructions</span></span></td>
<td><span data-ttu-id="04825-143">Descreve como pagar sua fatura, com base em sua região.</span><span class="sxs-lookup"><span data-stu-id="04825-143">Describes how to pay your invoice, based on your region.</span></span> <span data-ttu-id="04825-144">Inclua o número de sua fatura quando efetuar o pagamento.</span><span class="sxs-lookup"><span data-stu-id="04825-144">Always include your invoice number when making a payment.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="04825-145">Número da fatura</span><span class="sxs-lookup"><span data-stu-id="04825-145">Invoice no</span></span></td>
<td><span data-ttu-id="04825-146">O número da sua fatura.</span><span class="sxs-lookup"><span data-stu-id="04825-146">The number of your invoice.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="04825-147">Período de cobrança</span><span class="sxs-lookup"><span data-stu-id="04825-147">Billing period</span></span></td>
<td><span data-ttu-id="04825-148">Os parceiros CSP são cobrados mensalmente ou anualmente.</span><span class="sxs-lookup"><span data-stu-id="04825-148">CSP partners are billed either monthly or annually.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="04825-149">Data da fatura</span><span class="sxs-lookup"><span data-stu-id="04825-149">Invoice date</span></span></td>
<td><span data-ttu-id="04825-150">A data que você recebe sua fatura.</span><span class="sxs-lookup"><span data-stu-id="04825-150">The date you receive your invoice.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="04825-151">Data do pagamento</span><span class="sxs-lookup"><span data-stu-id="04825-151">Payment due date</span></span></td>
<td><span data-ttu-id="04825-152">Seu pagamento deve ser recebido até essa data.</span><span class="sxs-lookup"><span data-stu-id="04825-152">Your payment must be received by this date.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="04825-153">PO do cliente</span><span class="sxs-lookup"><span data-stu-id="04825-153">Customer PO</span></span></td>
<td><span data-ttu-id="04825-154">O número da ordem de compra.</span><span class="sxs-lookup"><span data-stu-id="04825-154">Your purchase order number.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="04825-155">Atendimento ao cliente</span><span class="sxs-lookup"><span data-stu-id="04825-155">Customer service</span></span></td>
<td><span data-ttu-id="04825-156">O endereço do site para acessar o atendimento ao cliente.</span><span class="sxs-lookup"><span data-stu-id="04825-156">The website address to access customer service.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="04825-157">Destinatário do serviço</span><span class="sxs-lookup"><span data-stu-id="04825-157">Service recipient</span></span></td>
<td><span data-ttu-id="04825-158">O endereço onde o serviço é usado.</span><span class="sxs-lookup"><span data-stu-id="04825-158">The address where the service is used.</span></span> <span data-ttu-id="04825-159">(Esse é o endereço de pessoa jurídica associado à verificação da empresa e não pode ser alterado.)</span><span class="sxs-lookup"><span data-stu-id="04825-159">(This is the legal company address associated with company vetting and cannot be changed.)</span></span></td>
</tr>
</tbody>
</table>

 

 

 



