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
ms.openlocfilehash: 5a1f45de59fc9dac6a443bb8a14c3a80b36ba3f7
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855872"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="3e582-103">Entender os diferentes tipos de encargo em arquivos de reconciliação do Partner Center</span><span class="sxs-lookup"><span data-stu-id="3e582-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="3e582-104">**Aplica-se a**: Partner Center | Partner Center para Microsoft Cloud do governo dos EUA</span><span class="sxs-lookup"><span data-stu-id="3e582-104">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="3e582-105">**Funções apropriadas**: agente de administração | Administrador de cobrança | Administrador global</span><span class="sxs-lookup"><span data-stu-id="3e582-105">**Appropriate roles**: Admin agent | Billing admin | Global admin</span></span>

<span data-ttu-id="3e582-106">Este artigo descreve os mapeamentos entre uma seção de fatura e os tipos de encargos associados que podem estar em seu arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="3e582-106">This article describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="3e582-107">Sua fatura fornece um resumo de encargos.</span><span class="sxs-lookup"><span data-stu-id="3e582-107">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="3e582-108">O arquivo de reconciliação fornece uma divisão detalhada das transações de item de linha, incluindo tipos de encargo.</span><span class="sxs-lookup"><span data-stu-id="3e582-108">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="3e582-109">Para obter mais informações sobre arquivos de reconciliação, consulte [como usar arquivos de reconciliação](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="3e582-109">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="3e582-110">Os [arquivos de reconciliação com base no uso](usage-based-recon-files.md) e os [arquivos de reconciliação baseados em licença](license-based-recon-files.md) mostram apenas transações e encargos relacionados ao uso (unidades consumidas e encargos relacionados).</span><span class="sxs-lookup"><span data-stu-id="3e582-110">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="3e582-111">Créditos únicos, descontos ou reembolsos que aparecem na fatura como **ajustes** não são mostrados no arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="3e582-111">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="3e582-112">Mapear tipos de cobrança para encargos de fatura</span><span class="sxs-lookup"><span data-stu-id="3e582-112">Map charge types to invoice charges</span></span>

<span data-ttu-id="3e582-113">Para fazer referência cruzada de valores entre a fatura e o arquivo de reconciliação, use as opções de filtro no Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="3e582-113">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="3e582-114">Filtre por tipos de encargo em seu arquivo de reconciliação para mapear os encargos da fatura para um conjunto de divisões de cobrança no arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="3e582-114">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="3e582-115">Cobranças baseada em licença</span><span class="sxs-lookup"><span data-stu-id="3e582-115">License-based charges</span></span>

<span data-ttu-id="3e582-116">Para mapear esses encargos baseados em licenças para sua fatura, some a coluna de **valor** do arquivo baseado em licença.</span><span class="sxs-lookup"><span data-stu-id="3e582-116">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="3e582-117">Descrição da cobrança (coluna Chargetype no arquivo de reconciliação)</span><span class="sxs-lookup"><span data-stu-id="3e582-117">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="3e582-118">Explicação da cobrança</span><span class="sxs-lookup"><span data-stu-id="3e582-118">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="3e582-119">Taxa de ativação</span><span class="sxs-lookup"><span data-stu-id="3e582-119">Activation fee</span></span> | <span data-ttu-id="3e582-120">O valor cobrado para o cliente quando ele usa a assinatura após a compra.</span><span class="sxs-lookup"><span data-stu-id="3e582-120">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="3e582-121">Taxa de cancelamento</span><span class="sxs-lookup"><span data-stu-id="3e582-121">Cancel fee</span></span> | <span data-ttu-id="3e582-122">Encargos rateado reembolsados ao cliente quando as licenças associadas são alteradas.</span><span class="sxs-lookup"><span data-stu-id="3e582-122">Prorated charges refunded to the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="3e582-123">Cancelar ocorrência proporcional</span><span class="sxs-lookup"><span data-stu-id="3e582-123">Cancel instance prorate</span></span> | <span data-ttu-id="3e582-124">Encargos rateado cancelados quando o cliente com a assinatura mensal tem assinatura suspensa e as licenças associadas foram alteradas no mesmo mês.</span><span class="sxs-lookup"><span data-stu-id="3e582-124">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated licenses changed within the same month.</span></span> |
| <span data-ttu-id="3e582-125">Taxa do Ciclo</span><span class="sxs-lookup"><span data-stu-id="3e582-125">Cycle fee</span></span> | <span data-ttu-id="3e582-126">Cobranças periódicas de uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="3e582-126">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="3e582-127">Proporcional à instância do ciclo</span><span class="sxs-lookup"><span data-stu-id="3e582-127">Cycle instance prorate</span></span> | <span data-ttu-id="3e582-128">Encargos rateados avaliados pelo cliente quando as licenças associadas são alteradas.</span><span class="sxs-lookup"><span data-stu-id="3e582-128">Prorated charges assessed from the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="3e582-129">Taxas proporcionais durante o cancelamento</span><span class="sxs-lookup"><span data-stu-id="3e582-129">Prorate fees when cancel</span></span> | <span data-ttu-id="3e582-130">Reembolso rateado por parte nãoutilizada do serviço após o cancelamento.</span><span class="sxs-lookup"><span data-stu-id="3e582-130">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="3e582-131">Taxas de taxa de taxa ao converter fora da oferta atual</span><span class="sxs-lookup"><span data-stu-id="3e582-131">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="3e582-132">Encargos rateados após a conversão da assinatura mensal atual em uma assinatura anual.</span><span class="sxs-lookup"><span data-stu-id="3e582-132">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="3e582-133">Taxas de taxa ao converter em uma nova oferta</span><span class="sxs-lookup"><span data-stu-id="3e582-133">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="3e582-134">Encargos rateados depois de converter uma assinatura mensal em uma nova assinatura anual.</span><span class="sxs-lookup"><span data-stu-id="3e582-134">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="3e582-135">Taxas proporcionais na compra</span><span class="sxs-lookup"><span data-stu-id="3e582-135">Prorate fees when purchase</span></span> | <span data-ttu-id="3e582-136">O tipo de cobrança de uma assinatura ao usar a cobrança mensal ou anual.</span><span class="sxs-lookup"><span data-stu-id="3e582-136">The charge type for a subscription when using both monthly or annual billing.</span></span> |
| <span data-ttu-id="3e582-137">Taxa proporcional ao renovar</span><span class="sxs-lookup"><span data-stu-id="3e582-137">Prorate fee when renew</span></span> | <span data-ttu-id="3e582-138">Valores rateados após a renovação da assinatura.</span><span class="sxs-lookup"><span data-stu-id="3e582-138">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="3e582-139">Taxa de renovação</span><span class="sxs-lookup"><span data-stu-id="3e582-139">Renew fee</span></span> | <span data-ttu-id="3e582-140">Cobrança para renovação de uma assinatura</span><span class="sxs-lookup"><span data-stu-id="3e582-140">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="3e582-141">Taxas proporcionais ao ativar</span><span class="sxs-lookup"><span data-stu-id="3e582-141">Prorate fees when activate</span></span> | <span data-ttu-id="3e582-142">Valores rateados da ativação até o final do período de cobrança.</span><span class="sxs-lookup"><span data-stu-id="3e582-142">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="3e582-143">Encargos único</span><span class="sxs-lookup"><span data-stu-id="3e582-143">One-time charges</span></span>

<span data-ttu-id="3e582-144">Para mapear esses encargos de uso único para sua fatura, soma a **coluna Valor** do arquivo baseado em licença.</span><span class="sxs-lookup"><span data-stu-id="3e582-144">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="3e582-145">Descrição da cobrança (coluna ChargeType no arquivo de reconciliação)</span><span class="sxs-lookup"><span data-stu-id="3e582-145">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="3e582-146">Explicação da cobrança</span><span class="sxs-lookup"><span data-stu-id="3e582-146">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="3e582-147">Novo</span><span class="sxs-lookup"><span data-stu-id="3e582-147">New</span></span> | <span data-ttu-id="3e582-148">Usado quando uma nova compra é criada.</span><span class="sxs-lookup"><span data-stu-id="3e582-148">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="3e582-149">addQuantity</span><span class="sxs-lookup"><span data-stu-id="3e582-149">addQuantity</span></span> | <span data-ttu-id="3e582-150">Usado no reembolso da compra original e na nova quantidade após um aumento.</span><span class="sxs-lookup"><span data-stu-id="3e582-150">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="3e582-151">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="3e582-151">removeQuantity</span></span> | <span data-ttu-id="3e582-152">Usado no reembolso da compra original e na nova quantidade após uma diminuição.</span><span class="sxs-lookup"><span data-stu-id="3e582-152">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="3e582-153">Cancelar</span><span class="sxs-lookup"><span data-stu-id="3e582-153">Cancel</span></span> | <span data-ttu-id="3e582-154">Usado quando uma assinatura é cancelada.</span><span class="sxs-lookup"><span data-stu-id="3e582-154">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="3e582-155">Converter</span><span class="sxs-lookup"><span data-stu-id="3e582-155">Convert</span></span> | <span data-ttu-id="3e582-156">Usado quando uma licença é atualizada, mas o número de licenças permanece inalterado.</span><span class="sxs-lookup"><span data-stu-id="3e582-156">Used when a license is upgraded but the number of licenses remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="3e582-157">Encargos de uso</span><span class="sxs-lookup"><span data-stu-id="3e582-157">Usage charges</span></span>

<span data-ttu-id="3e582-158">Para mapear esses encargos de uso para sua fatura, soma a **coluna PretaxCharges** do arquivo baseado em uso.</span><span class="sxs-lookup"><span data-stu-id="3e582-158">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="3e582-159">Descrição da cobrança (coluna ChargeType no arquivo de reconciliação)</span><span class="sxs-lookup"><span data-stu-id="3e582-159">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="3e582-160">Explicação da cobrança</span><span class="sxs-lookup"><span data-stu-id="3e582-160">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="3e582-161">Avaliar a taxa de uso ao cancelar</span><span class="sxs-lookup"><span data-stu-id="3e582-161">Assess usage fee when cancel</span></span> | <span data-ttu-id="3e582-162">Taxa de uso de acesso ao cancelamento para uso não pago durante o período de faturamento atual.</span><span class="sxs-lookup"><span data-stu-id="3e582-162">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="3e582-163">Avalie a taxa de uso para o ciclo atual</span><span class="sxs-lookup"><span data-stu-id="3e582-163">Assess usage fee for current cycle</span></span> | <span data-ttu-id="3e582-164">Taxa de uso de acesso para o período de faturamento atual.</span><span class="sxs-lookup"><span data-stu-id="3e582-164">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="3e582-165">Credits</span><span class="sxs-lookup"><span data-stu-id="3e582-165">Credits</span></span>

<span data-ttu-id="3e582-166">Para mapear esses créditos para sua fatura:</span><span class="sxs-lookup"><span data-stu-id="3e582-166">To map these credits to your invoice:</span></span>

- <span data-ttu-id="3e582-167">Some o **TotalForCustomer** do arquivo baseado em licença.</span><span class="sxs-lookup"><span data-stu-id="3e582-167">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="3e582-168">Some a coluna **PostTaxTotal** do arquivo baseado em uso.</span><span class="sxs-lookup"><span data-stu-id="3e582-168">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="3e582-169">Descrição da cobrança (coluna Chargetype no arquivo de reconciliação)</span><span class="sxs-lookup"><span data-stu-id="3e582-169">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="3e582-170">Explicação da cobrança</span><span class="sxs-lookup"><span data-stu-id="3e582-170">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="3e582-171">Deslocando um item de linha</span><span class="sxs-lookup"><span data-stu-id="3e582-171">Offset a line item</span></span> | <span data-ttu-id="3e582-172">Reembolso parcial ou total para um item de linha, incluindo impostos.</span><span class="sxs-lookup"><span data-stu-id="3e582-172">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="3e582-173">Descontos baseados em uso</span><span class="sxs-lookup"><span data-stu-id="3e582-173">Usage-based discounts</span></span>

<span data-ttu-id="3e582-174">Para mapear esses descontos com base no uso para sua fatura, some a coluna **PretaxCharges** do arquivo baseado em uso.</span><span class="sxs-lookup"><span data-stu-id="3e582-174">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="3e582-175">Descrição da cobrança (coluna Chargetype no arquivo de reconciliação)</span><span class="sxs-lookup"><span data-stu-id="3e582-175">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="3e582-176">Explicação da cobrança</span><span class="sxs-lookup"><span data-stu-id="3e582-176">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="3e582-177">Desconto de ativação</span><span class="sxs-lookup"><span data-stu-id="3e582-177">Activation discount</span></span> | <span data-ttu-id="3e582-178">Desconto aplicado quando a assinatura é ativada.</span><span class="sxs-lookup"><span data-stu-id="3e582-178">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="3e582-179">Desconto de ciclo</span><span class="sxs-lookup"><span data-stu-id="3e582-179">Cycle discount</span></span> | <span data-ttu-id="3e582-180">Desconto aplicado em encargos periódicos.</span><span class="sxs-lookup"><span data-stu-id="3e582-180">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="3e582-181">Desconto de renovação</span><span class="sxs-lookup"><span data-stu-id="3e582-181">Renew discount</span></span> | <span data-ttu-id="3e582-182">Desconto aplicado quando a assinatura é renovada.</span><span class="sxs-lookup"><span data-stu-id="3e582-182">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="3e582-183">Desconto de cancelamento</span><span class="sxs-lookup"><span data-stu-id="3e582-183">Cancel discount</span></span> | <span data-ttu-id="3e582-184">Encargos aplicados quando descontos são cancelados.</span><span class="sxs-lookup"><span data-stu-id="3e582-184">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="3e582-185">Descontos baseados em licença</span><span class="sxs-lookup"><span data-stu-id="3e582-185">License-based discounts</span></span>

<span data-ttu-id="3e582-186">Para mapear descontos baseados em licença para sua fatura, some a coluna **TotalOtherDiscount** do arquivo baseado em licença.</span><span class="sxs-lookup"><span data-stu-id="3e582-186">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="3e582-187">*Os descontos baseados em licença podem ser aplicados a vários tipos de cobrança.*</span><span class="sxs-lookup"><span data-stu-id="3e582-187">*License-based discounts may be applied to multiple charge types.*</span></span>
