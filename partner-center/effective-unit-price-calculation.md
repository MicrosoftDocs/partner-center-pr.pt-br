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
ms.openlocfilehash: a662e0b815c979b3454762c5b35eb510887c96ad
ms.sourcegitcommit: c6c741475604b8daf386fb54bb2795a6445ac887
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/05/2021
ms.locfileid: "106374376"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="3c162-104">Cálculo de preço unitário efetivo para consumo do plano do Azure</span><span class="sxs-lookup"><span data-stu-id="3c162-104">Effective unit price calculation for Azure plan consumption</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="3c162-105">O preço unitário efetivo</span><span class="sxs-lookup"><span data-stu-id="3c162-105">The effective unit price</span></span>

<span data-ttu-id="3c162-106">O preço unitário efetivo é calculado no nível de medidor (ao contrário do nível de recurso) e é ajustado diariamente de acordo com o uso do medidor.</span><span class="sxs-lookup"><span data-stu-id="3c162-106">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="3c162-107">Calculamos o preço unitário efetivo usando os três fatores a seguir:</span><span class="sxs-lookup"><span data-stu-id="3c162-107">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="3c162-108">Consumo, que é monitorado diariamente durante todo o ciclo de cobrança</span><span class="sxs-lookup"><span data-stu-id="3c162-108">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="3c162-109">Custo Faturável para o medidor</span><span class="sxs-lookup"><span data-stu-id="3c162-109">Billable cost for the meter</span></span>
- <span data-ttu-id="3c162-110">Camadas (se aplicável)</span><span class="sxs-lookup"><span data-stu-id="3c162-110">Tiering (if applicable)</span></span>

<span data-ttu-id="3c162-111">Como monitoramos o consumo diário durante todo o ciclo de cobrança, o preço unitário efetivo ficará flutuando.</span><span class="sxs-lookup"><span data-stu-id="3c162-111">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="3c162-112">O preço final de um determinado ciclo de cobrança estará disponível depois de parar o cálculo de consumo e fechar o período de cobrança.</span><span class="sxs-lookup"><span data-stu-id="3c162-112">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="3c162-113">Você verá a maioria das alterações no consumo após o quarto ou quinto lugar decimal.</span><span class="sxs-lookup"><span data-stu-id="3c162-113">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="3c162-114">Descubra se seu medidor usa preços em camadas</span><span class="sxs-lookup"><span data-stu-id="3c162-114">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="3c162-115">Se você não souber se o medidor usa preços em camadas, use o procedimento abaixo para descobrir.</span><span class="sxs-lookup"><span data-stu-id="3c162-115">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="3c162-116">Entre no painel [Partner Center](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="3c162-116">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="3c162-117">Selecione **vender**, selecione **preços e ofertas** e, em seguida, selecione **preços do plano do Azure**.</span><span class="sxs-lookup"><span data-stu-id="3c162-117">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="3c162-118">Localize seu medidor por ID e, em seguida, baixe os dados de preços.</span><span class="sxs-lookup"><span data-stu-id="3c162-118">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="3c162-119">Exemplo de cálculo</span><span class="sxs-lookup"><span data-stu-id="3c162-119">Sample calculation</span></span>

<span data-ttu-id="3c162-120">A tabela a seguir fornece um exemplo de como calculamos o preço unitário efetivo durante o período de abertura.</span><span class="sxs-lookup"><span data-stu-id="3c162-120">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="3c162-121">Na tabela, os seguintes valores se aplicam:</span><span class="sxs-lookup"><span data-stu-id="3c162-121">In the table, the following values apply:</span></span> 

- <span data-ttu-id="3c162-122">**Up** = preço unitário do recurso/hora = 0,868</span><span class="sxs-lookup"><span data-stu-id="3c162-122">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="3c162-123">**BCU** = unidade de consumo Faturável para o medidor</span><span class="sxs-lookup"><span data-stu-id="3c162-123">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="3c162-124">**BC** = custo Faturável para o medidor = BCU \* UP \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="3c162-124">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="3c162-125">Isso reflete um ajuste para o desconto de 15% do PEC.</span><span class="sxs-lookup"><span data-stu-id="3c162-125">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="3c162-126">Em seguida, usamos o limite inferior da função para limitar o valor a dois dígitos após o ponto decimal, a fim de cobrar o valor mínimo.</span><span class="sxs-lookup"><span data-stu-id="3c162-126">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="3c162-127">**Preço unitário efetivo** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="3c162-127">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]
><span data-ttu-id="3c162-128">O medidor neste exemplo não tem camadas em preços.</span><span class="sxs-lookup"><span data-stu-id="3c162-128">The meter in this example does not have tiers in pricing.</span></span> <span data-ttu-id="3c162-129">Os fatores de preço unitário efetivo em percentuais de desconto e outros ajustes.</span><span class="sxs-lookup"><span data-stu-id="3c162-129">The Effective Unit Price factors in discount percentages and other adjustments.</span></span>

| <span data-ttu-id="3c162-130">Data</span><span class="sxs-lookup"><span data-stu-id="3c162-130">Date</span></span> | <span data-ttu-id="3c162-131">BCU (unidade de consumo Faturável)</span><span class="sxs-lookup"><span data-stu-id="3c162-131">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="3c162-132">BC (custo Faturável)</span><span class="sxs-lookup"><span data-stu-id="3c162-132">BC (Billable cost)</span></span> | <span data-ttu-id="3c162-133">Preço unitário efetivo</span><span class="sxs-lookup"><span data-stu-id="3c162-133">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="3c162-134">3 de agosto</span><span class="sxs-lookup"><span data-stu-id="3c162-134">3-Aug</span></span> | <span data-ttu-id="3c162-135">29</span><span class="sxs-lookup"><span data-stu-id="3c162-135">29</span></span> | <span data-ttu-id="3c162-136">21,39</span><span class="sxs-lookup"><span data-stu-id="3c162-136">21.39</span></span> | <span data-ttu-id="3c162-137">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="3c162-137">0.737586206896552</span></span> |
| <span data-ttu-id="3c162-138">10 de agosto</span><span class="sxs-lookup"><span data-stu-id="3c162-138">10-Aug</span></span> | <span data-ttu-id="3c162-139">210,950039</span><span class="sxs-lookup"><span data-stu-id="3c162-139">210.950039</span></span> | <span data-ttu-id="3c162-140">155,63</span><span class="sxs-lookup"><span data-stu-id="3c162-140">155.63</span></span> | <span data-ttu-id="3c162-141">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="3c162-141">0.737757626107858</span></span> |
| <span data-ttu-id="3c162-142">25 de agosto</span><span class="sxs-lookup"><span data-stu-id="3c162-142">25-Aug</span></span> | <span data-ttu-id="3c162-143">555,950039</span><span class="sxs-lookup"><span data-stu-id="3c162-143">555.950039</span></span> | <span data-ttu-id="3c162-144">410,17</span><span class="sxs-lookup"><span data-stu-id="3c162-144">410.17</span></span> | <span data-ttu-id="3c162-145">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="3c162-145">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="3c162-146">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="3c162-146">Next steps</span></span>

- [<span data-ttu-id="3c162-147">Cobrança e impostos</span><span class="sxs-lookup"><span data-stu-id="3c162-147">Billing and taxes</span></span>](billing.md)
