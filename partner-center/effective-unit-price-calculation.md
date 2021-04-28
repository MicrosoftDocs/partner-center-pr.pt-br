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
ms.openlocfilehash: 1473b3c0b90cca1152b4dab0b8efec86dbc3d22d
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172210"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="e92b0-104">Cálculo de preço unitário efetivo para consumo do plano do Azure</span><span class="sxs-lookup"><span data-stu-id="e92b0-104">Effective unit price calculation for Azure plan consumption</span></span>

<span data-ttu-id="e92b0-105">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="e92b0-105">**Appropriate roles**</span></span>

- <span data-ttu-id="e92b0-106">Administrador de cobrança</span><span class="sxs-lookup"><span data-stu-id="e92b0-106">Billing admin</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="e92b0-107">O preço unitário efetivo</span><span class="sxs-lookup"><span data-stu-id="e92b0-107">The effective unit price</span></span>

<span data-ttu-id="e92b0-108">O preço unitário efetivo é calculado no nível de medidor (ao contrário do nível de recurso) e é ajustado diariamente de acordo com o uso do medidor.</span><span class="sxs-lookup"><span data-stu-id="e92b0-108">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="e92b0-109">Calculamos o preço unitário efetivo usando os três fatores a seguir:</span><span class="sxs-lookup"><span data-stu-id="e92b0-109">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="e92b0-110">Consumo, que é monitorado diariamente durante todo o ciclo de cobrança</span><span class="sxs-lookup"><span data-stu-id="e92b0-110">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="e92b0-111">Custo Faturável para o medidor</span><span class="sxs-lookup"><span data-stu-id="e92b0-111">Billable cost for the meter</span></span>
- <span data-ttu-id="e92b0-112">Camadas (se aplicável)</span><span class="sxs-lookup"><span data-stu-id="e92b0-112">Tiering (if applicable)</span></span>

<span data-ttu-id="e92b0-113">Como monitoramos o consumo diário durante todo o ciclo de cobrança, o preço unitário efetivo ficará flutuando.</span><span class="sxs-lookup"><span data-stu-id="e92b0-113">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="e92b0-114">O preço final de um determinado ciclo de cobrança estará disponível depois de parar o cálculo de consumo e fechar o período de cobrança.</span><span class="sxs-lookup"><span data-stu-id="e92b0-114">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="e92b0-115">Você verá a maioria das alterações no consumo após o quarto ou quinto lugar decimal.</span><span class="sxs-lookup"><span data-stu-id="e92b0-115">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="e92b0-116">Descubra se seu medidor usa preços em camadas</span><span class="sxs-lookup"><span data-stu-id="e92b0-116">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="e92b0-117">Se você não souber se o medidor usa preços em camadas, use o procedimento abaixo para descobrir.</span><span class="sxs-lookup"><span data-stu-id="e92b0-117">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="e92b0-118">Entre no painel [Partner Center](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="e92b0-118">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="e92b0-119">Selecione **vender**, selecione **preços e ofertas** e, em seguida, selecione **preços do plano do Azure**.</span><span class="sxs-lookup"><span data-stu-id="e92b0-119">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="e92b0-120">Localize seu medidor por ID e, em seguida, baixe os dados de preços.</span><span class="sxs-lookup"><span data-stu-id="e92b0-120">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="e92b0-121">Exemplo de cálculo</span><span class="sxs-lookup"><span data-stu-id="e92b0-121">Sample calculation</span></span>

<span data-ttu-id="e92b0-122">A tabela a seguir fornece um exemplo de como calculamos o preço unitário efetivo durante o período de abertura.</span><span class="sxs-lookup"><span data-stu-id="e92b0-122">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="e92b0-123">Na tabela, os seguintes valores se aplicam:</span><span class="sxs-lookup"><span data-stu-id="e92b0-123">In the table, the following values apply:</span></span> 

- <span data-ttu-id="e92b0-124">**Up** = preço unitário do recurso/hora = 0,868</span><span class="sxs-lookup"><span data-stu-id="e92b0-124">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="e92b0-125">**BCU** = unidade de consumo Faturável para o medidor</span><span class="sxs-lookup"><span data-stu-id="e92b0-125">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="e92b0-126">**BC** = custo Faturável para o medidor = BCU \* UP \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="e92b0-126">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="e92b0-127">Isso reflete um ajuste para o desconto de 15% do PEC.</span><span class="sxs-lookup"><span data-stu-id="e92b0-127">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="e92b0-128">Em seguida, usamos o limite inferior da função para limitar o valor a dois dígitos após o ponto decimal, a fim de cobrar o valor mínimo.</span><span class="sxs-lookup"><span data-stu-id="e92b0-128">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="e92b0-129">**Preço unitário efetivo** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="e92b0-129">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]

><span data-ttu-id="e92b0-130">Observação: o medidor neste exemplo não tem camadas em preços ou outros descontos — os fatores de preço unitário efetivo em percentuais de desconto e outros ajustes.</span><span class="sxs-lookup"><span data-stu-id="e92b0-130">Note: The meter in this example does not have tiers in pricing or other discounts—the Effective Unit Price factors in discount percentages and other adjustments.</span></span>


| <span data-ttu-id="e92b0-131">Data</span><span class="sxs-lookup"><span data-stu-id="e92b0-131">Date</span></span> | <span data-ttu-id="e92b0-132">BCU (unidade de consumo Faturável)</span><span class="sxs-lookup"><span data-stu-id="e92b0-132">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="e92b0-133">BC (custo Faturável)</span><span class="sxs-lookup"><span data-stu-id="e92b0-133">BC (Billable cost)</span></span> | <span data-ttu-id="e92b0-134">Preço unitário efetivo</span><span class="sxs-lookup"><span data-stu-id="e92b0-134">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="e92b0-135">3 de agosto</span><span class="sxs-lookup"><span data-stu-id="e92b0-135">3-Aug</span></span> | <span data-ttu-id="e92b0-136">29</span><span class="sxs-lookup"><span data-stu-id="e92b0-136">29</span></span> | <span data-ttu-id="e92b0-137">21,39</span><span class="sxs-lookup"><span data-stu-id="e92b0-137">21.39</span></span> | <span data-ttu-id="e92b0-138">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="e92b0-138">0.737586206896552</span></span> |
| <span data-ttu-id="e92b0-139">10 de agosto</span><span class="sxs-lookup"><span data-stu-id="e92b0-139">10-Aug</span></span> | <span data-ttu-id="e92b0-140">210,950039</span><span class="sxs-lookup"><span data-stu-id="e92b0-140">210.950039</span></span> | <span data-ttu-id="e92b0-141">155,63</span><span class="sxs-lookup"><span data-stu-id="e92b0-141">155.63</span></span> | <span data-ttu-id="e92b0-142">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="e92b0-142">0.737757626107858</span></span> |
| <span data-ttu-id="e92b0-143">25 de agosto</span><span class="sxs-lookup"><span data-stu-id="e92b0-143">25-Aug</span></span> | <span data-ttu-id="e92b0-144">555,950039</span><span class="sxs-lookup"><span data-stu-id="e92b0-144">555.950039</span></span> | <span data-ttu-id="e92b0-145">410,17</span><span class="sxs-lookup"><span data-stu-id="e92b0-145">410.17</span></span> | <span data-ttu-id="e92b0-146">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="e92b0-146">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="e92b0-147">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="e92b0-147">Next steps</span></span>

- [<span data-ttu-id="e92b0-148">Cobrança e impostos</span><span class="sxs-lookup"><span data-stu-id="e92b0-148">Billing and taxes</span></span>](billing.md)
