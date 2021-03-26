---
title: Tipos de encargo de arquivos de reconciliação
ms.topic: article
ms.date: 06/05/2020
description: Descubra os tipos de encargos (como, baseado em licença, com base no uso e em uma única vez), créditos e descontos em arquivos de reconciliação do Partner Center.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ba42ac5beb28a3cf819c54a86385fb79853cdcd0
ms.sourcegitcommit: 700150044ea4f1a0b96cb4caeb97d7197da29ef6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "105549219"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="80983-103">Entender os diferentes tipos de encargo em arquivos de reconciliação do Partner Center</span><span class="sxs-lookup"><span data-stu-id="80983-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="80983-104">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="80983-104">**Applies to**</span></span>

- <span data-ttu-id="80983-105">Partner Center para nuvem do Microsoft governamental</span><span class="sxs-lookup"><span data-stu-id="80983-105">Partner Center for Microsoft Government cloud</span></span>

<span data-ttu-id="80983-106">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="80983-106">**Appropriate roles**</span></span>

- <span data-ttu-id="80983-107">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="80983-107">Admin agent</span></span>
- <span data-ttu-id="80983-108">Administrador de cobrança</span><span class="sxs-lookup"><span data-stu-id="80983-108">Billing admin</span></span>
- <span data-ttu-id="80983-109">Administrador global</span><span class="sxs-lookup"><span data-stu-id="80983-109">Global admin</span></span>

<span data-ttu-id="80983-110">Este artigo descreve os mapeamentos entre uma seção de fatura e os tipos de encargos associados que podem estar em seu arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="80983-110">This article describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="80983-111">Sua fatura fornece um resumo de encargos.</span><span class="sxs-lookup"><span data-stu-id="80983-111">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="80983-112">O arquivo de reconciliação fornece uma divisão detalhada das transações de item de linha, incluindo tipos de encargo.</span><span class="sxs-lookup"><span data-stu-id="80983-112">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="80983-113">Para obter mais informações sobre arquivos de reconciliação, consulte [como usar arquivos de reconciliação](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="80983-113">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="80983-114">Os [arquivos de reconciliação com base no uso](usage-based-recon-files.md) e os [arquivos de reconciliação baseados em licença](license-based-recon-files.md) mostram apenas transações e encargos relacionados ao uso (unidades consumidas e encargos relacionados).</span><span class="sxs-lookup"><span data-stu-id="80983-114">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="80983-115">Créditos únicos, descontos ou reembolsos que aparecem na fatura como **ajustes** não são mostrados no arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="80983-115">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="80983-116">Mapear tipos de cobrança para encargos de fatura</span><span class="sxs-lookup"><span data-stu-id="80983-116">Map charge types to invoice charges</span></span>

<span data-ttu-id="80983-117">Para fazer referência cruzada de valores entre a fatura e o arquivo de reconciliação, use as opções de filtro no Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="80983-117">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="80983-118">Filtre por tipos de encargo em seu arquivo de reconciliação para mapear os encargos da fatura para um conjunto de divisões de cobrança no arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="80983-118">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="80983-119">Cobranças baseada em licença</span><span class="sxs-lookup"><span data-stu-id="80983-119">License-based charges</span></span>

<span data-ttu-id="80983-120">Para mapear esses encargos baseados em licenças para sua fatura, some a coluna de **valor** do arquivo baseado em licença.</span><span class="sxs-lookup"><span data-stu-id="80983-120">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="80983-121">Descrição da cobrança (coluna Chargetype no arquivo de reconciliação)</span><span class="sxs-lookup"><span data-stu-id="80983-121">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="80983-122">Explicação da cobrança</span><span class="sxs-lookup"><span data-stu-id="80983-122">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="80983-123">Taxa de ativação</span><span class="sxs-lookup"><span data-stu-id="80983-123">Activation fee</span></span> | <span data-ttu-id="80983-124">O valor cobrado para o cliente quando ele usa a assinatura após a compra.</span><span class="sxs-lookup"><span data-stu-id="80983-124">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="80983-125">Taxa de cancelamento</span><span class="sxs-lookup"><span data-stu-id="80983-125">Cancel fee</span></span> | <span data-ttu-id="80983-126">Encargos rateado reembolsados ao cliente quando as licenças associadas são alteradas.</span><span class="sxs-lookup"><span data-stu-id="80983-126">Prorated charges refunded to the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="80983-127">Cancelar ocorrência proporcional</span><span class="sxs-lookup"><span data-stu-id="80983-127">Cancel instance prorate</span></span> | <span data-ttu-id="80983-128">Encargos rateado cancelados quando o cliente com a assinatura mensal tem assinatura suspensa e as licenças associadas foram alteradas no mesmo mês.</span><span class="sxs-lookup"><span data-stu-id="80983-128">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated licenses changed within the same month.</span></span> |
| <span data-ttu-id="80983-129">Taxa do Ciclo</span><span class="sxs-lookup"><span data-stu-id="80983-129">Cycle fee</span></span> | <span data-ttu-id="80983-130">Cobranças periódicas de uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="80983-130">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="80983-131">Proporcional à instância do ciclo</span><span class="sxs-lookup"><span data-stu-id="80983-131">Cycle instance prorate</span></span> | <span data-ttu-id="80983-132">Encargos rateado avaliados do cliente quando as licenças associadas são alteradas.</span><span class="sxs-lookup"><span data-stu-id="80983-132">Prorated charges assessed from the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="80983-133">Taxas proporcionais durante o cancelamento</span><span class="sxs-lookup"><span data-stu-id="80983-133">Prorate fees when cancel</span></span> | <span data-ttu-id="80983-134">Reembolso rateado para parte não usada do serviço após o cancelamento.</span><span class="sxs-lookup"><span data-stu-id="80983-134">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="80983-135">Taxa de taxas ao converter da oferta atual</span><span class="sxs-lookup"><span data-stu-id="80983-135">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="80983-136">Encargos rateado após a conversão da assinatura mensal atual em uma assinatura anual.</span><span class="sxs-lookup"><span data-stu-id="80983-136">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="80983-137">Taxas de taxa ao converter em uma nova oferta</span><span class="sxs-lookup"><span data-stu-id="80983-137">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="80983-138">Encargos rateado após a conversão de uma assinatura mensal em uma nova assinatura anual.</span><span class="sxs-lookup"><span data-stu-id="80983-138">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="80983-139">Taxas proporcionais na compra</span><span class="sxs-lookup"><span data-stu-id="80983-139">Prorate fees when purchase</span></span> | <span data-ttu-id="80983-140">O tipo de encargo para uma assinatura ao usar a cobrança mensal ou anual.</span><span class="sxs-lookup"><span data-stu-id="80983-140">The charge type for a subscription when using both monthly or annual billing.</span></span> |
| <span data-ttu-id="80983-141">Taxa proporcional ao renovar</span><span class="sxs-lookup"><span data-stu-id="80983-141">Prorate fee when renew</span></span> | <span data-ttu-id="80983-142">Taxas rateada após a renovação da assinatura.</span><span class="sxs-lookup"><span data-stu-id="80983-142">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="80983-143">Taxa de renovação</span><span class="sxs-lookup"><span data-stu-id="80983-143">Renew fee</span></span> | <span data-ttu-id="80983-144">Cobrança para renovação de uma assinatura</span><span class="sxs-lookup"><span data-stu-id="80983-144">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="80983-145">Taxas proporcionais ao ativar</span><span class="sxs-lookup"><span data-stu-id="80983-145">Prorate fees when activate</span></span> | <span data-ttu-id="80983-146">Taxas rateada da ativação até o término do período de cobrança.</span><span class="sxs-lookup"><span data-stu-id="80983-146">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="80983-147">Encargos de uso único</span><span class="sxs-lookup"><span data-stu-id="80983-147">One-time charges</span></span>

<span data-ttu-id="80983-148">Para mapear esses encargos de uma vez para sua fatura, some a coluna de **valor** do arquivo baseado em licença.</span><span class="sxs-lookup"><span data-stu-id="80983-148">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="80983-149">Descrição da cobrança (coluna Chargetype no arquivo de reconciliação)</span><span class="sxs-lookup"><span data-stu-id="80983-149">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="80983-150">Explicação da cobrança</span><span class="sxs-lookup"><span data-stu-id="80983-150">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="80983-151">Novo</span><span class="sxs-lookup"><span data-stu-id="80983-151">New</span></span> | <span data-ttu-id="80983-152">Usado quando uma nova compra é criada.</span><span class="sxs-lookup"><span data-stu-id="80983-152">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="80983-153">addQuantity</span><span class="sxs-lookup"><span data-stu-id="80983-153">addQuantity</span></span> | <span data-ttu-id="80983-154">Usado tanto no reembolso da compra original quanto na nova quantidade após um aumento.</span><span class="sxs-lookup"><span data-stu-id="80983-154">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="80983-155">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="80983-155">removeQuantity</span></span> | <span data-ttu-id="80983-156">Usado tanto no reembolso da compra original quanto na nova quantidade após uma diminuição.</span><span class="sxs-lookup"><span data-stu-id="80983-156">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="80983-157">Cancelar</span><span class="sxs-lookup"><span data-stu-id="80983-157">Cancel</span></span> | <span data-ttu-id="80983-158">Usado quando uma assinatura é cancelada.</span><span class="sxs-lookup"><span data-stu-id="80983-158">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="80983-159">Converter</span><span class="sxs-lookup"><span data-stu-id="80983-159">Convert</span></span> | <span data-ttu-id="80983-160">Usado quando uma licença é atualizada, mas o número de licenças permanece inalterado.</span><span class="sxs-lookup"><span data-stu-id="80983-160">Used when a license is upgraded but the number of licenses remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="80983-161">Encargos de uso</span><span class="sxs-lookup"><span data-stu-id="80983-161">Usage charges</span></span>

<span data-ttu-id="80983-162">Para mapear esses encargos de uso para sua fatura, some a coluna **PretaxCharges** do arquivo baseado em uso.</span><span class="sxs-lookup"><span data-stu-id="80983-162">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="80983-163">Descrição da cobrança (coluna Chargetype no arquivo de reconciliação)</span><span class="sxs-lookup"><span data-stu-id="80983-163">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="80983-164">Explicação da cobrança</span><span class="sxs-lookup"><span data-stu-id="80983-164">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="80983-165">Avaliar a taxa de uso ao cancelar</span><span class="sxs-lookup"><span data-stu-id="80983-165">Assess usage fee when cancel</span></span> | <span data-ttu-id="80983-166">Taxa de uso de acesso ao cancelamento para uso não pago durante o período de faturamento atual.</span><span class="sxs-lookup"><span data-stu-id="80983-166">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="80983-167">Avalie a taxa de uso para o ciclo atual</span><span class="sxs-lookup"><span data-stu-id="80983-167">Assess usage fee for current cycle</span></span> | <span data-ttu-id="80983-168">Taxa de uso de acesso para o período de faturamento atual.</span><span class="sxs-lookup"><span data-stu-id="80983-168">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="80983-169">Credits</span><span class="sxs-lookup"><span data-stu-id="80983-169">Credits</span></span>

<span data-ttu-id="80983-170">Para mapear esses créditos para sua fatura:</span><span class="sxs-lookup"><span data-stu-id="80983-170">To map these credits to your invoice:</span></span>

- <span data-ttu-id="80983-171">Some o **TotalForCustomer** do arquivo baseado em licença.</span><span class="sxs-lookup"><span data-stu-id="80983-171">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="80983-172">Some a coluna **PostTaxTotal** do arquivo baseado em uso.</span><span class="sxs-lookup"><span data-stu-id="80983-172">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="80983-173">Descrição da cobrança (coluna Chargetype no arquivo de reconciliação)</span><span class="sxs-lookup"><span data-stu-id="80983-173">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="80983-174">Explicação da cobrança</span><span class="sxs-lookup"><span data-stu-id="80983-174">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="80983-175">Deslocando um item de linha</span><span class="sxs-lookup"><span data-stu-id="80983-175">Offset a line item</span></span> | <span data-ttu-id="80983-176">Reembolso parcial ou total para um item de linha, incluindo impostos.</span><span class="sxs-lookup"><span data-stu-id="80983-176">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="80983-177">Descontos baseados em uso</span><span class="sxs-lookup"><span data-stu-id="80983-177">Usage-based discounts</span></span>

<span data-ttu-id="80983-178">Para mapear esses descontos com base no uso para sua fatura, some a coluna **PretaxCharges** do arquivo baseado em uso.</span><span class="sxs-lookup"><span data-stu-id="80983-178">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="80983-179">Descrição da cobrança (coluna Chargetype no arquivo de reconciliação)</span><span class="sxs-lookup"><span data-stu-id="80983-179">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="80983-180">Explicação da cobrança</span><span class="sxs-lookup"><span data-stu-id="80983-180">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="80983-181">Desconto de ativação</span><span class="sxs-lookup"><span data-stu-id="80983-181">Activation discount</span></span> | <span data-ttu-id="80983-182">Desconto aplicado quando a assinatura é ativada.</span><span class="sxs-lookup"><span data-stu-id="80983-182">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="80983-183">Desconto de ciclo</span><span class="sxs-lookup"><span data-stu-id="80983-183">Cycle discount</span></span> | <span data-ttu-id="80983-184">Desconto aplicado em encargos periódicos.</span><span class="sxs-lookup"><span data-stu-id="80983-184">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="80983-185">Desconto de renovação</span><span class="sxs-lookup"><span data-stu-id="80983-185">Renew discount</span></span> | <span data-ttu-id="80983-186">Desconto aplicado quando a assinatura é renovada.</span><span class="sxs-lookup"><span data-stu-id="80983-186">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="80983-187">Desconto de cancelamento</span><span class="sxs-lookup"><span data-stu-id="80983-187">Cancel discount</span></span> | <span data-ttu-id="80983-188">Encargos aplicados quando descontos são cancelados.</span><span class="sxs-lookup"><span data-stu-id="80983-188">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="80983-189">Descontos baseados em licença</span><span class="sxs-lookup"><span data-stu-id="80983-189">License-based discounts</span></span>

<span data-ttu-id="80983-190">Para mapear descontos baseados em licença para sua fatura, some a coluna **TotalOtherDiscount** do arquivo baseado em licença.</span><span class="sxs-lookup"><span data-stu-id="80983-190">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="80983-191">*Os descontos baseados em licença podem ser aplicados a vários tipos de cobrança.*</span><span class="sxs-lookup"><span data-stu-id="80983-191">*License-based discounts may be applied to multiple charge types.*</span></span>
