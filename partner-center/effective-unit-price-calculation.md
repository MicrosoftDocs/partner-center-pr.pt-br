---
title: Cálculo de preço unitário efetivo
ms.topic: how-to
ms.date: 04/02/2021
description: Saiba mais sobre o preço unitário efetivo e como ele é calculado. Este artigo também inclui um cálculo de exemplo.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 84beac77d41b8c11be9ac3cad87460eec9632ac4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147115"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="e3998-104">Cálculo de preço unitário efetivo para consumo do plano do Azure</span><span class="sxs-lookup"><span data-stu-id="e3998-104">Effective unit price calculation for Azure plan consumption</span></span>

<span data-ttu-id="e3998-105">**Funções apropriadas**: administrador de cobrança</span><span class="sxs-lookup"><span data-stu-id="e3998-105">**Appropriate roles**: Billing admin</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="e3998-106">O preço unitário efetivo</span><span class="sxs-lookup"><span data-stu-id="e3998-106">The effective unit price</span></span>

<span data-ttu-id="e3998-107">O preço unitário efetivo é calculado no nível de medidor (ao contrário do nível de recurso) e é ajustado diariamente de acordo com o uso do medidor.</span><span class="sxs-lookup"><span data-stu-id="e3998-107">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="e3998-108">Calculamos o preço unitário efetivo usando os três fatores a seguir:</span><span class="sxs-lookup"><span data-stu-id="e3998-108">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="e3998-109">Consumo, que é monitorado diariamente durante todo o ciclo de cobrança</span><span class="sxs-lookup"><span data-stu-id="e3998-109">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="e3998-110">Custo Faturável para o medidor</span><span class="sxs-lookup"><span data-stu-id="e3998-110">Billable cost for the meter</span></span>
- <span data-ttu-id="e3998-111">Camadas (se aplicável)</span><span class="sxs-lookup"><span data-stu-id="e3998-111">Tiering (if applicable)</span></span>

<span data-ttu-id="e3998-112">Como monitoramos o consumo diário durante todo o ciclo de cobrança, o preço unitário efetivo ficará flutuando.</span><span class="sxs-lookup"><span data-stu-id="e3998-112">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="e3998-113">O preço final de um determinado ciclo de cobrança estará disponível depois de parar o cálculo de consumo e fechar o período de cobrança.</span><span class="sxs-lookup"><span data-stu-id="e3998-113">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="e3998-114">Você verá a maioria das alterações no consumo após o quarto ou quinto lugar decimal.</span><span class="sxs-lookup"><span data-stu-id="e3998-114">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="e3998-115">Descubra se seu medidor usa preços em camadas</span><span class="sxs-lookup"><span data-stu-id="e3998-115">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="e3998-116">Se você não souber se o medidor usa preços em camadas, use o procedimento abaixo para descobrir.</span><span class="sxs-lookup"><span data-stu-id="e3998-116">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="e3998-117">Entre no painel [Partner Center](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="e3998-117">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="e3998-118">Selecione **vender**, selecione **preços e ofertas** e, em seguida, selecione **preços do plano do Azure**.</span><span class="sxs-lookup"><span data-stu-id="e3998-118">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="e3998-119">Localize seu medidor por ID e, em seguida, baixe os dados de preços.</span><span class="sxs-lookup"><span data-stu-id="e3998-119">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="e3998-120">Exemplo de cálculo</span><span class="sxs-lookup"><span data-stu-id="e3998-120">Sample calculation</span></span>

<span data-ttu-id="e3998-121">A tabela a seguir fornece um exemplo de como calculamos o preço unitário efetivo durante o período de abertura.</span><span class="sxs-lookup"><span data-stu-id="e3998-121">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="e3998-122">Na tabela, os seguintes valores se aplicam:</span><span class="sxs-lookup"><span data-stu-id="e3998-122">In the table, the following values apply:</span></span> 

- <span data-ttu-id="e3998-123">**UP** = Preço unitar do recurso/hora = 0,868</span><span class="sxs-lookup"><span data-stu-id="e3998-123">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="e3998-124">**BCU** = unidade de consumo de cobrança para o medidor</span><span class="sxs-lookup"><span data-stu-id="e3998-124">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="e3998-125">**BC** = Custo cobrado pelo medidor = BCU \* UP \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="e3998-125">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="e3998-126">Isso reflete um ajuste para o desconto de PEC de 15%.</span><span class="sxs-lookup"><span data-stu-id="e3998-126">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="e3998-127">Em seguida, usamos o limite inferior da função para limitar o valor a dois dígitos após o ponto decimal, para cobrar a quantidade mínima.</span><span class="sxs-lookup"><span data-stu-id="e3998-127">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="e3998-128">**Preço unitártico** efetivo = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="e3998-128">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]

><span data-ttu-id="e3998-129">Observação: o medidor neste exemplo não tem camadas em preços ou outros descontos— os fatores de Preço Unitário Efetivo em percentuais de desconto e outros ajustes.</span><span class="sxs-lookup"><span data-stu-id="e3998-129">Note: The meter in this example does not have tiers in pricing or other discounts—the Effective Unit Price factors in discount percentages and other adjustments.</span></span>


| <span data-ttu-id="e3998-130">Data</span><span class="sxs-lookup"><span data-stu-id="e3998-130">Date</span></span> | <span data-ttu-id="e3998-131">BCU (unidade de consumo de cobrança)</span><span class="sxs-lookup"><span data-stu-id="e3998-131">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="e3998-132">BC (custo cobrado)</span><span class="sxs-lookup"><span data-stu-id="e3998-132">BC (Billable cost)</span></span> | <span data-ttu-id="e3998-133">Preço unitidade efetivo</span><span class="sxs-lookup"><span data-stu-id="e3998-133">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="e3998-134">3 de agosto</span><span class="sxs-lookup"><span data-stu-id="e3998-134">3-Aug</span></span> | <span data-ttu-id="e3998-135">29</span><span class="sxs-lookup"><span data-stu-id="e3998-135">29</span></span> | <span data-ttu-id="e3998-136">21.39</span><span class="sxs-lookup"><span data-stu-id="e3998-136">21.39</span></span> | <span data-ttu-id="e3998-137">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="e3998-137">0.737586206896552</span></span> |
| <span data-ttu-id="e3998-138">10 de agosto</span><span class="sxs-lookup"><span data-stu-id="e3998-138">10-Aug</span></span> | <span data-ttu-id="e3998-139">210.950039</span><span class="sxs-lookup"><span data-stu-id="e3998-139">210.950039</span></span> | <span data-ttu-id="e3998-140">155.63</span><span class="sxs-lookup"><span data-stu-id="e3998-140">155.63</span></span> | <span data-ttu-id="e3998-141">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="e3998-141">0.737757626107858</span></span> |
| <span data-ttu-id="e3998-142">25 de agosto</span><span class="sxs-lookup"><span data-stu-id="e3998-142">25-Aug</span></span> | <span data-ttu-id="e3998-143">555.950039</span><span class="sxs-lookup"><span data-stu-id="e3998-143">555.950039</span></span> | <span data-ttu-id="e3998-144">410.17</span><span class="sxs-lookup"><span data-stu-id="e3998-144">410.17</span></span> | <span data-ttu-id="e3998-145">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="e3998-145">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="e3998-146">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="e3998-146">Next steps</span></span>

- [<span data-ttu-id="e3998-147">Cobrança e impostos</span><span class="sxs-lookup"><span data-stu-id="e3998-147">Billing and taxes</span></span>](billing.md)
