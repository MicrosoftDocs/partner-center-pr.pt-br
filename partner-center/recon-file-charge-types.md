---
title: Tipos de encargo de arquivo de reconciliação | Centro de parceiros
ms.topic: article
ms.date: 08/26/2019
description: Tipos de encargos (baseados em licença, com base no uso e uma única vez), créditos e descontos em arquivos de reconciliação do Partner Center.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 064ed6dda28f5a8ace64942d55ef2a6327528ff5
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389804"
---
# <a name="understand-charge-types"></a><span data-ttu-id="bccb1-103">Entender os tipos de encargo</span><span class="sxs-lookup"><span data-stu-id="bccb1-103">Understand charge types</span></span>

<span data-ttu-id="bccb1-104">Aplica-se a:</span><span class="sxs-lookup"><span data-stu-id="bccb1-104">Applies to:</span></span>

- <span data-ttu-id="bccb1-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="bccb1-105">Partner Center</span></span>
- <span data-ttu-id="bccb1-106">Partner Center do Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="bccb1-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="bccb1-107">Este tópico descreve os mapeamentos entre uma seção de fatura e os tipos de encargos associados que podem estar em seu arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="bccb1-107">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="bccb1-108">Sua fatura fornece um resumo de encargos.</span><span class="sxs-lookup"><span data-stu-id="bccb1-108">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="bccb1-109">O arquivo de reconciliação fornece uma divisão detalhada das transações de item de linha, incluindo tipos de encargo.</span><span class="sxs-lookup"><span data-stu-id="bccb1-109">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="bccb1-110">Para obter mais informações sobre arquivos de reconciliação, consulte [como usar arquivos de reconciliação](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="bccb1-110">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="bccb1-111">Os [arquivos de reconciliação com base no uso](usage-based-recon-files.md) e os [arquivos de reconciliação baseados em licença](license-based-recon-files.md) mostram apenas transações e encargos relacionados ao uso (unidades consumidas e encargos relacionados).</span><span class="sxs-lookup"><span data-stu-id="bccb1-111">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="bccb1-112">Créditos únicos, descontos ou reembolsos que aparecem na fatura como **ajustes** não são mostrados no arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="bccb1-112">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="bccb1-113">Mapear tipos de cobrança para encargos de fatura</span><span class="sxs-lookup"><span data-stu-id="bccb1-113">Map charge types to invoice charges</span></span>

<span data-ttu-id="bccb1-114">Para fazer referência cruzada de valores entre a fatura e o arquivo de reconciliação, use as opções de filtro no Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="bccb1-114">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="bccb1-115">Filtre por tipos de encargo em seu arquivo de reconciliação para mapear os encargos da fatura para um conjunto de divisões de cobrança no arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="bccb1-115">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="bccb1-116">Cobranças baseada em licença</span><span class="sxs-lookup"><span data-stu-id="bccb1-116">License-based charges</span></span>

<span data-ttu-id="bccb1-117">Para mapear esses encargos baseados em licenças para sua fatura, some a coluna de **valor** do arquivo baseado em licença.</span><span class="sxs-lookup"><span data-stu-id="bccb1-117">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="bccb1-118">Descrição da cobrança (coluna Chargetype no arquivo de reconciliação)</span><span class="sxs-lookup"><span data-stu-id="bccb1-118">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="bccb1-119">Explicação da cobrança</span><span class="sxs-lookup"><span data-stu-id="bccb1-119">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="bccb1-120">Taxa de ativação</span><span class="sxs-lookup"><span data-stu-id="bccb1-120">Activation fee</span></span> | <span data-ttu-id="bccb1-121">O valor cobrado para o cliente quando ele usa a assinatura após a compra.</span><span class="sxs-lookup"><span data-stu-id="bccb1-121">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="bccb1-122">Taxa de cancelamento</span><span class="sxs-lookup"><span data-stu-id="bccb1-122">Cancel fee</span></span> | <span data-ttu-id="bccb1-123">Encargos rateado reembolsados ao cliente quando as estações associadas são alteradas.</span><span class="sxs-lookup"><span data-stu-id="bccb1-123">Prorated charges refunded to the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="bccb1-124">Taxa do ciclo</span><span class="sxs-lookup"><span data-stu-id="bccb1-124">Cycle fee</span></span> | <span data-ttu-id="bccb1-125">Cobranças periódicas de uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="bccb1-125">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="bccb1-126">Proporcional à instância do ciclo</span><span class="sxs-lookup"><span data-stu-id="bccb1-126">Cycle instance prorate</span></span> | <span data-ttu-id="bccb1-127">Encargos rateado avaliados do cliente quando as estações associadas são alteradas.</span><span class="sxs-lookup"><span data-stu-id="bccb1-127">Prorated charges assessed from the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="bccb1-128">Taxas proporcionais durante o cancelamento</span><span class="sxs-lookup"><span data-stu-id="bccb1-128">Prorate fees when cancel</span></span> | <span data-ttu-id="bccb1-129">Reembolso rateado para parte não usada do serviço após o cancelamento.</span><span class="sxs-lookup"><span data-stu-id="bccb1-129">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="bccb1-130">Taxas proporcionais na compra</span><span class="sxs-lookup"><span data-stu-id="bccb1-130">Prorate fees when purchase</span></span> | <span data-ttu-id="bccb1-131">O tipo de encargo para uma assinatura ao usar a cobrança anual.</span><span class="sxs-lookup"><span data-stu-id="bccb1-131">The charge type for a subscription when using annual billing.</span></span> |
| <span data-ttu-id="bccb1-132">Valor de compra</span><span class="sxs-lookup"><span data-stu-id="bccb1-132">Purchase fee</span></span> | <span data-ttu-id="bccb1-133">O tipo de encargo para uma assinatura ao usar a cobrança mensal.</span><span class="sxs-lookup"><span data-stu-id="bccb1-133">The charge type for a subscription when using monthly billing.</span></span> |
| <span data-ttu-id="bccb1-134">Taxa proporcional ao renovar</span><span class="sxs-lookup"><span data-stu-id="bccb1-134">Prorate fee when renew</span></span> | <span data-ttu-id="bccb1-135">Taxas rateada após a renovação da assinatura.</span><span class="sxs-lookup"><span data-stu-id="bccb1-135">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="bccb1-136">Taxa de renovação</span><span class="sxs-lookup"><span data-stu-id="bccb1-136">Renew fee</span></span> | <span data-ttu-id="bccb1-137">Cobrança para renovação de uma assinatura</span><span class="sxs-lookup"><span data-stu-id="bccb1-137">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="bccb1-138">Taxas proporcionais ao ativar</span><span class="sxs-lookup"><span data-stu-id="bccb1-138">Prorate fees when activate</span></span> | <span data-ttu-id="bccb1-139">> taxas rateada da ativação até o término do período de cobrança.</span><span class="sxs-lookup"><span data-stu-id="bccb1-139">>Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="bccb1-140">Encargos de uso único</span><span class="sxs-lookup"><span data-stu-id="bccb1-140">One-time charges</span></span>

<span data-ttu-id="bccb1-141">Para mapear esses encargos de uma vez para sua fatura, some a coluna de **valor** do arquivo baseado em licença.</span><span class="sxs-lookup"><span data-stu-id="bccb1-141">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="bccb1-142">Descrição da cobrança (coluna Chargetype no arquivo de reconciliação)</span><span class="sxs-lookup"><span data-stu-id="bccb1-142">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="bccb1-143">Explicação da cobrança</span><span class="sxs-lookup"><span data-stu-id="bccb1-143">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="bccb1-144">Novo</span><span class="sxs-lookup"><span data-stu-id="bccb1-144">New</span></span> | <span data-ttu-id="bccb1-145">Usado quando uma nova compra é criada.</span><span class="sxs-lookup"><span data-stu-id="bccb1-145">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="bccb1-146">addQuantity</span><span class="sxs-lookup"><span data-stu-id="bccb1-146">addQuantity</span></span> | <span data-ttu-id="bccb1-147">Usado tanto no reembolso da compra original quanto na nova quantidade após um aumento.</span><span class="sxs-lookup"><span data-stu-id="bccb1-147">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="bccb1-148">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="bccb1-148">removeQuantity</span></span> | <span data-ttu-id="bccb1-149">Usado tanto no reembolso da compra original quanto na nova quantidade após uma diminuição.</span><span class="sxs-lookup"><span data-stu-id="bccb1-149">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="bccb1-150">Cancel</span><span class="sxs-lookup"><span data-stu-id="bccb1-150">Cancel</span></span> | <span data-ttu-id="bccb1-151">Usado quando uma assinatura é cancelada.</span><span class="sxs-lookup"><span data-stu-id="bccb1-151">Used when a subscription is cancelled.</span></span> |
| <span data-ttu-id="bccb1-152">Converter</span><span class="sxs-lookup"><span data-stu-id="bccb1-152">Convert</span></span> | <span data-ttu-id="bccb1-153">Usado quando uma licença é atualizada, mas o número de estações permanece inalterado.</span><span class="sxs-lookup"><span data-stu-id="bccb1-153">Used when a license is upgraded but the number of seats remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="bccb1-154">Tarifas de uso</span><span class="sxs-lookup"><span data-stu-id="bccb1-154">Usage charges</span></span>

<span data-ttu-id="bccb1-155">Para mapear esses encargos de uso para sua fatura, some a coluna **PretaxCharges** do arquivo baseado em uso.</span><span class="sxs-lookup"><span data-stu-id="bccb1-155">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="bccb1-156">Descrição da cobrança (coluna Chargetype no arquivo de reconciliação)</span><span class="sxs-lookup"><span data-stu-id="bccb1-156">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="bccb1-157">Explicação da cobrança</span><span class="sxs-lookup"><span data-stu-id="bccb1-157">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="bccb1-158">Avaliar a taxa de uso ao cancelar</span><span class="sxs-lookup"><span data-stu-id="bccb1-158">Assess usage fee when cancel</span></span> | <span data-ttu-id="bccb1-159">Taxa de uso de acesso no cancelamento para uso não pago durante o período de cobrança atual.</span><span class="sxs-lookup"><span data-stu-id="bccb1-159">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="bccb1-160">Avalie a taxa de uso para o ciclo atual</span><span class="sxs-lookup"><span data-stu-id="bccb1-160">Assess usage fee for current cycle</span></span> | <span data-ttu-id="bccb1-161">Taxa de uso de acesso para o período de cobrança atual.</span><span class="sxs-lookup"><span data-stu-id="bccb1-161">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="bccb1-162">Créditos</span><span class="sxs-lookup"><span data-stu-id="bccb1-162">Credits</span></span>

<span data-ttu-id="bccb1-163">Para mapear esses créditos para sua fatura:</span><span class="sxs-lookup"><span data-stu-id="bccb1-163">To map these credits to your invoice:</span></span>

- <span data-ttu-id="bccb1-164">Some o **TotalForCustomer** do arquivo baseado em licença.</span><span class="sxs-lookup"><span data-stu-id="bccb1-164">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="bccb1-165">Some a coluna **PostTaxTotal** do arquivo baseado em uso.</span><span class="sxs-lookup"><span data-stu-id="bccb1-165">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="bccb1-166">Descrição da cobrança (coluna Chargetype no arquivo de reconciliação)</span><span class="sxs-lookup"><span data-stu-id="bccb1-166">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="bccb1-167">Explicação da cobrança</span><span class="sxs-lookup"><span data-stu-id="bccb1-167">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="bccb1-168">Deslocando um item de linha</span><span class="sxs-lookup"><span data-stu-id="bccb1-168">Offset a line item</span></span> | <span data-ttu-id="bccb1-169">Reembolso parcial ou total para um item de linha, incluindo impostos.</span><span class="sxs-lookup"><span data-stu-id="bccb1-169">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="bccb1-170">Descontos baseados em uso</span><span class="sxs-lookup"><span data-stu-id="bccb1-170">Usage-based discounts</span></span>

<span data-ttu-id="bccb1-171">Para mapear esses descontos com base no uso para sua fatura, some a coluna **PretaxCharges** do arquivo baseado em uso.</span><span class="sxs-lookup"><span data-stu-id="bccb1-171">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="bccb1-172">Descrição da cobrança (coluna Chargetype no arquivo de reconciliação)</span><span class="sxs-lookup"><span data-stu-id="bccb1-172">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="bccb1-173">Explicação da cobrança</span><span class="sxs-lookup"><span data-stu-id="bccb1-173">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="bccb1-174">Desconto de ativação</span><span class="sxs-lookup"><span data-stu-id="bccb1-174">Activation discount</span></span> | <span data-ttu-id="bccb1-175">Desconto aplicado quando a assinatura é ativada.</span><span class="sxs-lookup"><span data-stu-id="bccb1-175">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="bccb1-176">Desconto de ciclo</span><span class="sxs-lookup"><span data-stu-id="bccb1-176">Cycle discount</span></span> | <span data-ttu-id="bccb1-177">Desconto aplicado em encargos periódicos.</span><span class="sxs-lookup"><span data-stu-id="bccb1-177">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="bccb1-178">Desconto de renovação</span><span class="sxs-lookup"><span data-stu-id="bccb1-178">Renew discount</span></span> | <span data-ttu-id="bccb1-179">Desconto aplicado quando a assinatura é renovada.</span><span class="sxs-lookup"><span data-stu-id="bccb1-179">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="bccb1-180">Desconto de cancelamento</span><span class="sxs-lookup"><span data-stu-id="bccb1-180">Cancel discount</span></span> | <span data-ttu-id="bccb1-181">Encargos aplicados quando os descontos foram cancelados.</span><span class="sxs-lookup"><span data-stu-id="bccb1-181">Charges applied when discounts cancelled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="bccb1-182">Descontos baseados em licença</span><span class="sxs-lookup"><span data-stu-id="bccb1-182">License-based discounts</span></span>

<span data-ttu-id="bccb1-183">Para mapear descontos baseados em licença para sua fatura, some a coluna **TotalOtherDiscount** do arquivo baseado em licença.</span><span class="sxs-lookup"><span data-stu-id="bccb1-183">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="bccb1-184">*Os descontos baseados em licença podem ser aplicados a vários tipos de cobrança.*</span><span class="sxs-lookup"><span data-stu-id="bccb1-184">*License-based discounts may be applied to multiple charge types.*</span></span>
