---
title: Tipos de encargo de arquivo de reconciliação
ms.topic: article
ms.date: 06/05/2020
description: Descubra os tipos de encargos (como, baseado em licença, com base no uso e em uma única vez), créditos e descontos em arquivos de reconciliação do Partner Center.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1ec4f4a483ecfd106f7ec41b85372e136524a046
ms.sourcegitcommit: 1796d3d0ec2e06a3792852377ff81127b4d22fe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2020
ms.locfileid: "84909104"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="757f8-103">Entender os diferentes tipos de encargo em arquivos de reconciliação do Partner Center</span><span class="sxs-lookup"><span data-stu-id="757f8-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="757f8-104">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="757f8-104">**Applies to**</span></span>

- <span data-ttu-id="757f8-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="757f8-105">Partner Center</span></span>
- <span data-ttu-id="757f8-106">Partner Center do Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="757f8-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="757f8-107">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="757f8-107">**Appropriate roles**</span></span>

- <span data-ttu-id="757f8-108">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="757f8-108">Admin agent</span></span>
- <span data-ttu-id="757f8-109">Administrador de cobrança</span><span class="sxs-lookup"><span data-stu-id="757f8-109">Billing admin</span></span>
- <span data-ttu-id="757f8-110">Administrador global</span><span class="sxs-lookup"><span data-stu-id="757f8-110">Global admin</span></span>

<span data-ttu-id="757f8-111">Este tópico descreve os mapeamentos entre uma seção de fatura e os tipos de encargos associados que podem estar em seu arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="757f8-111">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="757f8-112">Sua fatura fornece um resumo de encargos.</span><span class="sxs-lookup"><span data-stu-id="757f8-112">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="757f8-113">O arquivo de reconciliação fornece uma divisão detalhada das transações de item de linha, incluindo tipos de encargo.</span><span class="sxs-lookup"><span data-stu-id="757f8-113">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="757f8-114">Para obter mais informações sobre arquivos de reconciliação, consulte [como usar arquivos de reconciliação](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="757f8-114">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="757f8-115">Os [arquivos de reconciliação com base no uso](usage-based-recon-files.md) e os [arquivos de reconciliação baseados em licença](license-based-recon-files.md) mostram apenas transações e encargos relacionados ao uso (unidades consumidas e encargos relacionados).</span><span class="sxs-lookup"><span data-stu-id="757f8-115">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="757f8-116">Créditos únicos, descontos ou reembolsos que aparecem na fatura como **ajustes** não são mostrados no arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="757f8-116">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="757f8-117">Mapear tipos de cobrança para encargos de fatura</span><span class="sxs-lookup"><span data-stu-id="757f8-117">Map charge types to invoice charges</span></span>

<span data-ttu-id="757f8-118">Para fazer referência cruzada de valores entre a fatura e o arquivo de reconciliação, use as opções de filtro no Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="757f8-118">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="757f8-119">Filtre por tipos de encargo em seu arquivo de reconciliação para mapear os encargos da fatura para um conjunto de divisões de cobrança no arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="757f8-119">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="757f8-120">Cobranças baseada em licença</span><span class="sxs-lookup"><span data-stu-id="757f8-120">License-based charges</span></span>

<span data-ttu-id="757f8-121">Para mapear esses encargos baseados em licenças para sua fatura, some a coluna de **valor** do arquivo baseado em licença.</span><span class="sxs-lookup"><span data-stu-id="757f8-121">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="757f8-122">Descrição da cobrança (coluna Chargetype no arquivo de reconciliação)</span><span class="sxs-lookup"><span data-stu-id="757f8-122">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="757f8-123">Explicação da cobrança</span><span class="sxs-lookup"><span data-stu-id="757f8-123">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="757f8-124">Taxa de ativação</span><span class="sxs-lookup"><span data-stu-id="757f8-124">Activation fee</span></span> | <span data-ttu-id="757f8-125">O valor cobrado para o cliente quando ele usa a assinatura após a compra.</span><span class="sxs-lookup"><span data-stu-id="757f8-125">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="757f8-126">Taxa de cancelamento</span><span class="sxs-lookup"><span data-stu-id="757f8-126">Cancel fee</span></span> | <span data-ttu-id="757f8-127">Encargos rateado reembolsados ao cliente quando as estações associadas são alteradas.</span><span class="sxs-lookup"><span data-stu-id="757f8-127">Prorated charges refunded to the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="757f8-128">Cancelar ocorrência proporcional</span><span class="sxs-lookup"><span data-stu-id="757f8-128">Cancel instance prorate</span></span> | <span data-ttu-id="757f8-129">Encargos rateado cancelados quando o cliente com a assinatura mensal tem assinatura suspensa e estações associadas foram alteradas no mesmo mês.</span><span class="sxs-lookup"><span data-stu-id="757f8-129">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated seats changed within the same month.</span></span> |
| <span data-ttu-id="757f8-130">Taxa do Ciclo</span><span class="sxs-lookup"><span data-stu-id="757f8-130">Cycle fee</span></span> | <span data-ttu-id="757f8-131">Cobranças periódicas de uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="757f8-131">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="757f8-132">Proporcional à instância do ciclo</span><span class="sxs-lookup"><span data-stu-id="757f8-132">Cycle instance prorate</span></span> | <span data-ttu-id="757f8-133">Encargos rateado avaliados do cliente quando as estações associadas são alteradas.</span><span class="sxs-lookup"><span data-stu-id="757f8-133">Prorated charges assessed from the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="757f8-134">Taxas proporcionais durante o cancelamento</span><span class="sxs-lookup"><span data-stu-id="757f8-134">Prorate fees when cancel</span></span> | <span data-ttu-id="757f8-135">Reembolso rateado para parte não usada do serviço após o cancelamento.</span><span class="sxs-lookup"><span data-stu-id="757f8-135">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="757f8-136">Taxa de taxas ao converter da oferta atual</span><span class="sxs-lookup"><span data-stu-id="757f8-136">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="757f8-137">Encargos rateado após a conversão da assinatura mensal atual em uma assinatura anual.</span><span class="sxs-lookup"><span data-stu-id="757f8-137">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="757f8-138">Taxas de taxa ao converter em uma nova oferta</span><span class="sxs-lookup"><span data-stu-id="757f8-138">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="757f8-139">Encargos rateado após a conversão de uma assinatura mensal em uma nova assinatura anual.</span><span class="sxs-lookup"><span data-stu-id="757f8-139">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="757f8-140">Taxas proporcionais na compra</span><span class="sxs-lookup"><span data-stu-id="757f8-140">Prorate fees when purchase</span></span> | <span data-ttu-id="757f8-141">O tipo de encargo para uma assinatura ao usar a cobrança anual.</span><span class="sxs-lookup"><span data-stu-id="757f8-141">The charge type for a subscription when using annual billing.</span></span> |
| <span data-ttu-id="757f8-142">Valor de compra</span><span class="sxs-lookup"><span data-stu-id="757f8-142">Purchase fee</span></span> | <span data-ttu-id="757f8-143">O tipo de encargo para uma assinatura ao usar a cobrança mensal.</span><span class="sxs-lookup"><span data-stu-id="757f8-143">The charge type for a subscription when using monthly billing.</span></span> |
| <span data-ttu-id="757f8-144">Taxa proporcional ao renovar</span><span class="sxs-lookup"><span data-stu-id="757f8-144">Prorate fee when renew</span></span> | <span data-ttu-id="757f8-145">Taxas rateada após a renovação da assinatura.</span><span class="sxs-lookup"><span data-stu-id="757f8-145">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="757f8-146">Taxa de renovação</span><span class="sxs-lookup"><span data-stu-id="757f8-146">Renew fee</span></span> | <span data-ttu-id="757f8-147">Cobrança para renovação de uma assinatura</span><span class="sxs-lookup"><span data-stu-id="757f8-147">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="757f8-148">Taxas proporcionais ao ativar</span><span class="sxs-lookup"><span data-stu-id="757f8-148">Prorate fees when activate</span></span> | <span data-ttu-id="757f8-149">Taxas rateada da ativação até o término do período de cobrança.</span><span class="sxs-lookup"><span data-stu-id="757f8-149">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="757f8-150">Encargos de uso único</span><span class="sxs-lookup"><span data-stu-id="757f8-150">One-time charges</span></span>

<span data-ttu-id="757f8-151">Para mapear esses encargos de uma vez para sua fatura, some a coluna de **valor** do arquivo baseado em licença.</span><span class="sxs-lookup"><span data-stu-id="757f8-151">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="757f8-152">Descrição da cobrança (coluna Chargetype no arquivo de reconciliação)</span><span class="sxs-lookup"><span data-stu-id="757f8-152">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="757f8-153">Explicação da cobrança</span><span class="sxs-lookup"><span data-stu-id="757f8-153">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="757f8-154">Novo</span><span class="sxs-lookup"><span data-stu-id="757f8-154">New</span></span> | <span data-ttu-id="757f8-155">Usado quando uma nova compra é criada.</span><span class="sxs-lookup"><span data-stu-id="757f8-155">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="757f8-156">addQuantity</span><span class="sxs-lookup"><span data-stu-id="757f8-156">addQuantity</span></span> | <span data-ttu-id="757f8-157">Usado tanto no reembolso da compra original quanto na nova quantidade após um aumento.</span><span class="sxs-lookup"><span data-stu-id="757f8-157">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="757f8-158">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="757f8-158">removeQuantity</span></span> | <span data-ttu-id="757f8-159">Usado tanto no reembolso da compra original quanto na nova quantidade após uma diminuição.</span><span class="sxs-lookup"><span data-stu-id="757f8-159">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="757f8-160">Cancelar</span><span class="sxs-lookup"><span data-stu-id="757f8-160">Cancel</span></span> | <span data-ttu-id="757f8-161">Usado quando uma assinatura é cancelada.</span><span class="sxs-lookup"><span data-stu-id="757f8-161">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="757f8-162">Converter</span><span class="sxs-lookup"><span data-stu-id="757f8-162">Convert</span></span> | <span data-ttu-id="757f8-163">Usado quando uma licença é atualizada, mas o número de estações permanece inalterado.</span><span class="sxs-lookup"><span data-stu-id="757f8-163">Used when a license is upgraded but the number of seats remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="757f8-164">Encargos de uso</span><span class="sxs-lookup"><span data-stu-id="757f8-164">Usage charges</span></span>

<span data-ttu-id="757f8-165">Para mapear esses encargos de uso para sua fatura, some a coluna **PretaxCharges** do arquivo baseado em uso.</span><span class="sxs-lookup"><span data-stu-id="757f8-165">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="757f8-166">Descrição da cobrança (coluna Chargetype no arquivo de reconciliação)</span><span class="sxs-lookup"><span data-stu-id="757f8-166">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="757f8-167">Explicação da cobrança</span><span class="sxs-lookup"><span data-stu-id="757f8-167">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="757f8-168">Avaliar a taxa de uso ao cancelar</span><span class="sxs-lookup"><span data-stu-id="757f8-168">Assess usage fee when cancel</span></span> | <span data-ttu-id="757f8-169">Taxa de uso de acesso ao cancelamento para uso não pago durante o período de faturamento atual.</span><span class="sxs-lookup"><span data-stu-id="757f8-169">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="757f8-170">Avalie a taxa de uso para o ciclo atual</span><span class="sxs-lookup"><span data-stu-id="757f8-170">Assess usage fee for current cycle</span></span> | <span data-ttu-id="757f8-171">Taxa de uso de acesso para o período de faturamento atual.</span><span class="sxs-lookup"><span data-stu-id="757f8-171">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="757f8-172">Credits</span><span class="sxs-lookup"><span data-stu-id="757f8-172">Credits</span></span>

<span data-ttu-id="757f8-173">Para mapear esses créditos para sua fatura:</span><span class="sxs-lookup"><span data-stu-id="757f8-173">To map these credits to your invoice:</span></span>

- <span data-ttu-id="757f8-174">Some o **TotalForCustomer** do arquivo baseado em licença.</span><span class="sxs-lookup"><span data-stu-id="757f8-174">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="757f8-175">Some a coluna **PostTaxTotal** do arquivo baseado em uso.</span><span class="sxs-lookup"><span data-stu-id="757f8-175">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="757f8-176">Descrição da cobrança (coluna Chargetype no arquivo de reconciliação)</span><span class="sxs-lookup"><span data-stu-id="757f8-176">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="757f8-177">Explicação da cobrança</span><span class="sxs-lookup"><span data-stu-id="757f8-177">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="757f8-178">Deslocando um item de linha</span><span class="sxs-lookup"><span data-stu-id="757f8-178">Offset a line item</span></span> | <span data-ttu-id="757f8-179">Reembolso parcial ou total para um item de linha, incluindo impostos.</span><span class="sxs-lookup"><span data-stu-id="757f8-179">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="757f8-180">Descontos baseados em uso</span><span class="sxs-lookup"><span data-stu-id="757f8-180">Usage-based discounts</span></span>

<span data-ttu-id="757f8-181">Para mapear esses descontos com base no uso para sua fatura, some a coluna **PretaxCharges** do arquivo baseado em uso.</span><span class="sxs-lookup"><span data-stu-id="757f8-181">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="757f8-182">Descrição da cobrança (coluna Chargetype no arquivo de reconciliação)</span><span class="sxs-lookup"><span data-stu-id="757f8-182">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="757f8-183">Explicação da cobrança</span><span class="sxs-lookup"><span data-stu-id="757f8-183">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="757f8-184">Desconto de ativação</span><span class="sxs-lookup"><span data-stu-id="757f8-184">Activation discount</span></span> | <span data-ttu-id="757f8-185">Desconto aplicado quando a assinatura é ativada.</span><span class="sxs-lookup"><span data-stu-id="757f8-185">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="757f8-186">Desconto de ciclo</span><span class="sxs-lookup"><span data-stu-id="757f8-186">Cycle discount</span></span> | <span data-ttu-id="757f8-187">Desconto aplicado em encargos periódicos.</span><span class="sxs-lookup"><span data-stu-id="757f8-187">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="757f8-188">Desconto de renovação</span><span class="sxs-lookup"><span data-stu-id="757f8-188">Renew discount</span></span> | <span data-ttu-id="757f8-189">Desconto aplicado quando a assinatura é renovada.</span><span class="sxs-lookup"><span data-stu-id="757f8-189">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="757f8-190">Desconto de cancelamento</span><span class="sxs-lookup"><span data-stu-id="757f8-190">Cancel discount</span></span> | <span data-ttu-id="757f8-191">Encargos aplicados quando descontos são cancelados.</span><span class="sxs-lookup"><span data-stu-id="757f8-191">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="757f8-192">Descontos baseados em licença</span><span class="sxs-lookup"><span data-stu-id="757f8-192">License-based discounts</span></span>

<span data-ttu-id="757f8-193">Para mapear descontos baseados em licença para sua fatura, some a coluna **TotalOtherDiscount** do arquivo baseado em licença.</span><span class="sxs-lookup"><span data-stu-id="757f8-193">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="757f8-194">*Os descontos baseados em licença podem ser aplicados a vários tipos de cobrança.*</span><span class="sxs-lookup"><span data-stu-id="757f8-194">*License-based discounts may be applied to multiple charge types.*</span></span>
