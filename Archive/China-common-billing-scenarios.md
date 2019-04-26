---
title: Cenários comuns de cobrança (operado pela 21Vianet do Partner Center)
ms.topic: article
ms.date: 10/29/2018
description: Este tópico explica o que você deve esperar ver em sua fatura depois de adicionar novas assinaturas, ajustar o número de estações em uma assinatura ou cancelar uma assinatura.
author: MaggiePucciEvans
ms.author: evansma
ms.openlocfilehash: 0da5bbf6a5c3259589973e25f592457da7e3e42e
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2019
ms.locfileid: "62132336"
---
# <a name="common-billing-scenarios"></a><span data-ttu-id="41bf0-103">Cenários comuns de cobrança</span><span class="sxs-lookup"><span data-stu-id="41bf0-103">Common billing scenarios</span></span>

<span data-ttu-id="41bf0-104">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="41bf0-104">**Applies to**</span></span>

-   <span data-ttu-id="41bf0-105">Partner Center operado pela 21Vianet</span><span class="sxs-lookup"><span data-stu-id="41bf0-105">Partner Center operated by 21Vianet</span></span>


<span data-ttu-id="41bf0-106">Este tópico explica o que você deve esperar ver em sua fatura depois de adicionar novas assinaturas, ajustar o número de estações em uma assinatura ou cancelar uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="41bf0-106">This topic explains what you should expect to see on your bill after you add new subscriptions, adjust the number of seats in a subscription, or cancel a subscription.</span></span> 


## <a name="licence-based-billing"></a><span data-ttu-id="41bf0-107">Cobrança baseada em licença</span><span class="sxs-lookup"><span data-stu-id="41bf0-107">Licence-based billing</span></span>


<span data-ttu-id="41bf0-108">Meses sem alterações para assinaturas de licença, você verá um único item de linha para cada assinatura no seu arquivo de reconciliação e a fatura para o encargo de avanço para o próximo mês.</span><span class="sxs-lookup"><span data-stu-id="41bf0-108">For months without changes to licence-based subscriptions, you'll see a single line item for each subscription on your reconciliation file and invoice for the advance charge for the coming month.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="41bf0-109">Cenário</span><span class="sxs-lookup"><span data-stu-id="41bf0-109">Scenario</span></span></td>
<td><span data-ttu-id="41bf0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="41bf0-110">Description</span></span></td>
<td><span data-ttu-id="41bf0-111">Exemplo</span><span class="sxs-lookup"><span data-stu-id="41bf0-111">Example</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="41bf0-112">Nova assinatura</span><span class="sxs-lookup"><span data-stu-id="41bf0-112">New subscription</span></span></td>
<td><p><span data-ttu-id="41bf0-113">O período entre a data de início da assinatura e a data da primeira cobrança é GRÁTIS.</span><span class="sxs-lookup"><span data-stu-id="41bf0-113">The period between the start date of the subscription and the first billing date is FREE.</span></span></p>
<p><span data-ttu-id="41bf0-114">Seu arquivo de reconciliação conterá um único item de linha:</span><span class="sxs-lookup"><span data-stu-id="41bf0-114">Your reconciliation file will contain a single line-item:</span></span></p>
<ul>
<li><span data-ttu-id="41bf0-115">cobrança antecipada do próximo mês</span><span class="sxs-lookup"><span data-stu-id="41bf0-115">next month's advance charge</span></span></li>
</ul></td>
<td></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="41bf0-116">Nova assinatura: cancelada antes do fechamento da fatura</span><span class="sxs-lookup"><span data-stu-id="41bf0-116">New subscription: cancelled before the billing cut</span></span></td>
<td><span data-ttu-id="41bf0-117">Os encargos não serão aplicados à conta.</span><span class="sxs-lookup"><span data-stu-id="41bf0-117">Charges will not be applied to the account.</span></span> <span data-ttu-id="41bf0-118">A assinatura não aparecerá no arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="41bf0-118">The subscription won't appear in the reconciliation file.</span></span> <span data-ttu-id="41bf0-119">Isso é útil se você quiser fazer um teste sem precisar pagar os encargos da assinatura.</span><span class="sxs-lookup"><span data-stu-id="41bf0-119">This is useful if you want to perform testing without incurring subscription charges.</span></span></td>
<td></td>
</tr>
<tr class="even">
<td><span data-ttu-id="41bf0-120">Nova assinatura: com ajustes de quantidade de licenças durante o período gratuito</span><span class="sxs-lookup"><span data-stu-id="41bf0-120">New subscription: with licence quantity adjustments during the free period</span></span></td>
<td><p><span data-ttu-id="41bf0-121">Seu arquivo de reconciliação conterá vários itens de linha:</span><span class="sxs-lookup"><span data-stu-id="41bf0-121">Your reconciliation file will contain multiple line-items:</span></span></p>
<ul>
<li><span data-ttu-id="41bf0-122">alterações na quantidade de licenças, cobradas no preço unitário 0.</span><span class="sxs-lookup"><span data-stu-id="41bf0-122">license quantity changes, charged at 0 Unit Price.</span></span> <span data-ttu-id="41bf0-123">(Não há custo para alterações de assentos durante o período gratuito)</span><span class="sxs-lookup"><span data-stu-id="41bf0-123">(There is no cost for seat changes during the free period)</span></span></li>
<li><span data-ttu-id="41bf0-124">cobrança antecipada pelo próximo mês, refletindo a nova quantidade.</span><span class="sxs-lookup"><span data-stu-id="41bf0-124">advance charge for the next month, reflecting the new quantity.</span></span></li>
</ul></td>
<td><span data-ttu-id="41bf0-125">Uso proporcional:</span><span class="sxs-lookup"><span data-stu-id="41bf0-125">Prorated usage:</span></span>
<ul>
<li><span data-ttu-id="41bf0-126">De 3 de junho a 7 de junho para 10 assentos = custo ZERO</span><span class="sxs-lookup"><span data-stu-id="41bf0-126">June 3rd to June 7th for 10 seats = ZERO charge</span></span></li>
<li><span data-ttu-id="41bf0-127">De 8 de junho a 11 de junho para 20 assentos = custo ZERO</span><span class="sxs-lookup"><span data-stu-id="41bf0-127">June 8th to June 11th for 20 seats = ZERO charge</span></span></li>
<li><span data-ttu-id="41bf0-128">De 12 de junho a 14 de junho para 15 assentos = custo ZERO</span><span class="sxs-lookup"><span data-stu-id="41bf0-128">June 12th to June 14th for 15 seats = ZERO charge</span></span></li>
</ul>
<p><span data-ttu-id="41bf0-129">Recortar de cobrança: Avançar o custo para o período do mês inteiro de 15 de junho para 14 de julho para estações de 15.</span><span class="sxs-lookup"><span data-stu-id="41bf0-129">Billing cut: Advance charge for the whole month period from June 15th to July 14th for 15 seats.</span></span> <span data-ttu-id="41bf0-130">Supondo que a cobrança por assinatura mensal seja US$ 10, o valor será US$ 10 x 15 assentos = US$ 150.</span><span class="sxs-lookup"><span data-stu-id="41bf0-130">Assuming the charge per subscription per month is 10 USD, the charge would be 10 USD x 15 seats = 150 USD.</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="41bf0-131">Assinatura existente: Aumentar ou diminuir a quantidade de licença</span><span class="sxs-lookup"><span data-stu-id="41bf0-131">Existing subscription: Increase or decrease in licence quantity</span></span></td>
<td><p><span data-ttu-id="41bf0-132">Seu arquivo de reconciliação conterá vários itens de linha:</span><span class="sxs-lookup"><span data-stu-id="41bf0-132">Your reconciliation file will contain multiple line-items:</span></span></p>
<ul>
<li><span data-ttu-id="41bf0-133">a reversão da cobrança antecipada</span><span class="sxs-lookup"><span data-stu-id="41bf0-133">the advance charge reversal</span></span></li>
<li><span data-ttu-id="41bf0-134">encargos de uso proporcional</span><span class="sxs-lookup"><span data-stu-id="41bf0-134">prorated usage charges</span></span></li>
<li><span data-ttu-id="41bf0-135">cobrança antecipada do próximo mês</span><span class="sxs-lookup"><span data-stu-id="41bf0-135">next month's advance charge</span></span></li>
</ul></td>
<td><p><span data-ttu-id="41bf0-136">Uso proporcional:</span><span class="sxs-lookup"><span data-stu-id="41bf0-136">Prorated usage:</span></span></p>
<ul>
<li><span data-ttu-id="41bf0-137">De 15 de julho a 19 de julho para 15 assentos = US$ 26,61</span><span class="sxs-lookup"><span data-stu-id="41bf0-137">July 15th to July 19th for 15 seats = 26.61 USD</span></span></li>
<li><span data-ttu-id="41bf0-138">De 20 de julho a 30 de julho para 12 assentos = US$ 46,84</span><span class="sxs-lookup"><span data-stu-id="41bf0-138">July 20th to July 30th for 12 seats = 46.84 USD</span></span></li>
<li><span data-ttu-id="41bf0-139">De 31 de julho a 9 de agosto para 18 assentos = US$ 63,87</span><span class="sxs-lookup"><span data-stu-id="41bf0-139">July 31st to August 9th for 18 seats = 63.87 USD</span></span></li>
<li><span data-ttu-id="41bf0-140">De 10 de agosto a 14 de agosto para 10 assentos = US$ 17,74</span><span class="sxs-lookup"><span data-stu-id="41bf0-140">August 10th to August 14th for 10 seats = 17.74 USD</span></span></li>
</ul>
<span data-ttu-id="41bf0-141">Reversão da cobrança antecipada para todo o período mensal de 15 de julho a 14 de agosto = US$ -165.</span><span class="sxs-lookup"><span data-stu-id="41bf0-141">Reversal of the advance charge for the whole month period from July 15th to August 14th = -165 USD.</span></span>
<p><span data-ttu-id="41bf0-142">Recortar de cobrança: Avançar o custo para o período do mês inteiro de 15 de agosto para 14 de setembro para 10 estações = USD 110.</span><span class="sxs-lookup"><span data-stu-id="41bf0-142">Billing cut: Advance charge for the whole month period from August 15th to September 14th for 10 seats = 110 USD.</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="41bf0-143">Cancelamento: sem alterações de assentos anteriores</span><span class="sxs-lookup"><span data-stu-id="41bf0-143">Cancellation: no prior seat changes</span></span></td>
<td><p><span data-ttu-id="41bf0-144">Seu arquivo de reconciliação conterá um único item de linha:</span><span class="sxs-lookup"><span data-stu-id="41bf0-144">Your reconciliation file will contain a single line-item:</span></span></p>
<ul>
<li><span data-ttu-id="41bf0-145">Um crédito pelos dias não utilizados, já que o período integral foi cobrado antecipadamente no extrato de cobrança anterior.</span><span class="sxs-lookup"><span data-stu-id="41bf0-145">A credit for unused days, because the whole period was billed in advance in the previous billing statement.</span></span> <span data-ttu-id="41bf0-146">Isso é calculado com base na data de término da assinatura.</span><span class="sxs-lookup"><span data-stu-id="41bf0-146">This is calculated based on the Subscription End date.</span></span></li>
</ul></td>
<td><span data-ttu-id="41bf0-147">Anteriormente cobrados encargos de avanço: 15 de agosto de 14 de setembro para 10 se ajuste = 100 USD.</span><span class="sxs-lookup"><span data-stu-id="41bf0-147">Previously billed advance charge: August 15th to September 14th for 10 seats = 100 USD.</span></span>
<p><span data-ttu-id="41bf0-148">Parte consumida da cobrança antecipada de 15 de agosto de 24 de agosto.</span><span class="sxs-lookup"><span data-stu-id="41bf0-148">Consumed portion of the advance charge from August 15th to August 24th.</span></span></p>
<p><span data-ttu-id="41bf0-149">Crédito por dias não utilizados: 25 de agosto a 14 de setembro para 10 se ajuste =-74.51.</span><span class="sxs-lookup"><span data-stu-id="41bf0-149">Credit for unused days: August 25th to September 14th for 10 seats = -74.51.</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="41bf0-150">Cancelamento: com as alterações de assentos anteriores</span><span class="sxs-lookup"><span data-stu-id="41bf0-150">Cancellation: with prior seat changes</span></span></td>
<td><p><span data-ttu-id="41bf0-151">Seu arquivo de reconciliação conterá vários itens de linha:</span><span class="sxs-lookup"><span data-stu-id="41bf0-151">Your reconciliation file will contain multiple line-items:</span></span></p>
<ul>
<li><span data-ttu-id="41bf0-152">a reversão da cobrança antecipada</span><span class="sxs-lookup"><span data-stu-id="41bf0-152">the advance charge reversal</span></span></li>
<li><span data-ttu-id="41bf0-153">encargos de uso proporcional</span><span class="sxs-lookup"><span data-stu-id="41bf0-153">prorated usage charges</span></span></li>
<li><span data-ttu-id="41bf0-154">um crédito pelos dias não utilizados</span><span class="sxs-lookup"><span data-stu-id="41bf0-154">a credit for any unused days</span></span></li>
</ul></td>
<td><span data-ttu-id="41bf0-155">Anteriormente cobrados encargos de avanço: 15 de agosto de 14 de setembro para 10 se ajuste = 100 USD.</span><span class="sxs-lookup"><span data-stu-id="41bf0-155">Previously billed advance charge: August 15th to September 14th for 10 seats = 100 USD.</span></span>
<p><span data-ttu-id="41bf0-156">Uso proporcional:</span><span class="sxs-lookup"><span data-stu-id="41bf0-156">Prorated usage:</span></span></p>
<ul>
<li><span data-ttu-id="41bf0-157">De 15 de agosto a 24 de agosto para 10 assentos</span><span class="sxs-lookup"><span data-stu-id="41bf0-157">August 15th to August 24th for 10 seats</span></span></li>
<li><span data-ttu-id="41bf0-158">De 25 de agosto a 14 de setembro para 5 assentos</span><span class="sxs-lookup"><span data-stu-id="41bf0-158">August 25th to September 14th for 5 seats</span></span></li>
</ul>
<p><span data-ttu-id="41bf0-159">Crédito por dias não utilizados: 1º de setembro para 14 de setembro de 5 estações.</span><span class="sxs-lookup"><span data-stu-id="41bf0-159">Credit for unused days: September 1st to September 14th for 5 seats.</span></span></p>
<p><span data-ttu-id="41bf0-160">Reversão da cobrança antecipada para todo o período mensal de 15 de agosto a 14 de setembro = US$ -100.</span><span class="sxs-lookup"><span data-stu-id="41bf0-160">Reversal of the advance charge for the whole month period from August 15th to September 14th = -100 USD.</span></span></p></td>
</tr>
</tbody>
</table>
