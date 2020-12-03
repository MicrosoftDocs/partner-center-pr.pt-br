---
title: Cálculo de preço unitário efetivo
ms.topic: how-to
ms.date: 11/10/2020
description: Saiba mais sobre o preço unitário efetivo e como ele é calculado. Este artigo também inclui um cálculo de exemplo.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6ca6e9bf6a49e695314a3e33e36d2d1d5d4d2a25
ms.sourcegitcommit: 147813ba322653c989df5afe0b3bf0c252523a92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "96556320"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="d1c53-104">Cálculo de preço unitário efetivo para consumo do plano do Azure</span><span class="sxs-lookup"><span data-stu-id="d1c53-104">Effective unit price calculation for Azure plan consumption</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="d1c53-105">O preço unitário efetivo</span><span class="sxs-lookup"><span data-stu-id="d1c53-105">The effective unit price</span></span>

<span data-ttu-id="d1c53-106">O preço unitário efetivo é calculado no nível de medidor (ao contrário do nível de recurso) e é ajustado diariamente de acordo com o uso do medidor.</span><span class="sxs-lookup"><span data-stu-id="d1c53-106">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="d1c53-107">Calculamos o preço unitário efetivo usando os três fatores a seguir:</span><span class="sxs-lookup"><span data-stu-id="d1c53-107">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="d1c53-108">Consumo, que é monitorado diariamente durante todo o ciclo de cobrança</span><span class="sxs-lookup"><span data-stu-id="d1c53-108">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="d1c53-109">Custo Faturável para o medidor</span><span class="sxs-lookup"><span data-stu-id="d1c53-109">Billable cost for the meter</span></span>
- <span data-ttu-id="d1c53-110">Camadas (se aplicável)</span><span class="sxs-lookup"><span data-stu-id="d1c53-110">Tiering (if applicable)</span></span>

<span data-ttu-id="d1c53-111">Como monitoramos o consumo diário durante todo o ciclo de cobrança, o preço unitário efetivo ficará flutuando.</span><span class="sxs-lookup"><span data-stu-id="d1c53-111">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="d1c53-112">O preço final de um determinado ciclo de cobrança estará disponível depois de parar o cálculo de consumo e fechar o período de cobrança.</span><span class="sxs-lookup"><span data-stu-id="d1c53-112">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="d1c53-113">Você verá a maioria das alterações no consumo após o quarto ou quinto lugar decimal.</span><span class="sxs-lookup"><span data-stu-id="d1c53-113">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="d1c53-114">Descubra se seu medidor usa preços em camadas</span><span class="sxs-lookup"><span data-stu-id="d1c53-114">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="d1c53-115">Se você não souber se o medidor usa preços em camadas, use o procedimento abaixo para descobrir.</span><span class="sxs-lookup"><span data-stu-id="d1c53-115">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="d1c53-116">Entre no painel [Partner Center](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="d1c53-116">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="d1c53-117">Selecione **vender**, selecione **preços e ofertas** e, em seguida, selecione **preços do plano do Azure**.</span><span class="sxs-lookup"><span data-stu-id="d1c53-117">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="d1c53-118">Localize seu medidor por ID e, em seguida, baixe os dados de preços.</span><span class="sxs-lookup"><span data-stu-id="d1c53-118">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="d1c53-119">Exemplo de cálculo</span><span class="sxs-lookup"><span data-stu-id="d1c53-119">Sample calculation</span></span>

<span data-ttu-id="d1c53-120">A tabela a seguir fornece um exemplo de como calculamos o preço unitário efetivo durante o período de abertura.</span><span class="sxs-lookup"><span data-stu-id="d1c53-120">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="d1c53-121">Na tabela, os seguintes valores se aplicam:</span><span class="sxs-lookup"><span data-stu-id="d1c53-121">In the table, the following values apply:</span></span> 

- <span data-ttu-id="d1c53-122">**Up** = preço unitário do recurso/hora = 0,868</span><span class="sxs-lookup"><span data-stu-id="d1c53-122">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="d1c53-123">**BCU** = unidade de consumo Faturável para o medidor</span><span class="sxs-lookup"><span data-stu-id="d1c53-123">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="d1c53-124">**BC** = custo Faturável para o medidor = BCU \* UP \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="d1c53-124">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="d1c53-125">Isso reflete um ajuste para o desconto de 15% do PEC.</span><span class="sxs-lookup"><span data-stu-id="d1c53-125">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="d1c53-126">Em seguida, usamos o limite inferior da função para limitar o valor a dois dígitos após o ponto decimal, a fim de cobrar o valor mínimo.</span><span class="sxs-lookup"><span data-stu-id="d1c53-126">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="d1c53-127">**Preço unitário efetivo** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="d1c53-127">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]
><span data-ttu-id="d1c53-128">Observação: o medidor neste exemplo não tem camadas em preços.</span><span class="sxs-lookup"><span data-stu-id="d1c53-128">Note: The meter in this example does not have tiers in pricing.</span></span>

| <span data-ttu-id="d1c53-129">Data</span><span class="sxs-lookup"><span data-stu-id="d1c53-129">Date</span></span> | <span data-ttu-id="d1c53-130">BCU (unidade de consumo Faturável)</span><span class="sxs-lookup"><span data-stu-id="d1c53-130">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="d1c53-131">BC (custo Faturável)</span><span class="sxs-lookup"><span data-stu-id="d1c53-131">BC (Billable cost)</span></span> | <span data-ttu-id="d1c53-132">Preço unitário efetivo</span><span class="sxs-lookup"><span data-stu-id="d1c53-132">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="d1c53-133">3 de agosto</span><span class="sxs-lookup"><span data-stu-id="d1c53-133">3-Aug</span></span> | <span data-ttu-id="d1c53-134">29</span><span class="sxs-lookup"><span data-stu-id="d1c53-134">29</span></span> | <span data-ttu-id="d1c53-135">21,39</span><span class="sxs-lookup"><span data-stu-id="d1c53-135">21.39</span></span> | <span data-ttu-id="d1c53-136">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="d1c53-136">0.737586206896552</span></span> |
| <span data-ttu-id="d1c53-137">10 de agosto</span><span class="sxs-lookup"><span data-stu-id="d1c53-137">10-Aug</span></span> | <span data-ttu-id="d1c53-138">210,950039</span><span class="sxs-lookup"><span data-stu-id="d1c53-138">210.950039</span></span> | <span data-ttu-id="d1c53-139">155,63</span><span class="sxs-lookup"><span data-stu-id="d1c53-139">155.63</span></span> | <span data-ttu-id="d1c53-140">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="d1c53-140">0.737757626107858</span></span> |
| <span data-ttu-id="d1c53-141">25 de agosto</span><span class="sxs-lookup"><span data-stu-id="d1c53-141">25-Aug</span></span> | <span data-ttu-id="d1c53-142">555,950039</span><span class="sxs-lookup"><span data-stu-id="d1c53-142">555.950039</span></span> | <span data-ttu-id="d1c53-143">410,17</span><span class="sxs-lookup"><span data-stu-id="d1c53-143">410.17</span></span> | <span data-ttu-id="d1c53-144">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="d1c53-144">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="d1c53-145">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="d1c53-145">Next steps</span></span>

- [<span data-ttu-id="d1c53-146">Cobrança e impostos</span><span class="sxs-lookup"><span data-stu-id="d1c53-146">Billing and taxes</span></span>](billing.md)
