---
title: Lista de consultas de exemplo
description: Use as consultas de exemplo para acessar programaticamente dados de análise do Revisions do parceiro.
ms.topic: reference
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: e25784585a1ac505db99e58265939a8851edcbad
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114374781"
---
# <a name="sample-queries-for-partner-center-insights-report"></a><span data-ttu-id="1ca91-103">Exemplos de consultas para o relatório do Partner Center insights</span><span class="sxs-lookup"><span data-stu-id="1ca91-103">Sample queries for Partner Center insights report</span></span>

<span data-ttu-id="1ca91-104">este artigo fornece exemplos de consultas para os relatórios de Insights de parceiros.</span><span class="sxs-lookup"><span data-stu-id="1ca91-104">This article provides sample queries for the Partner Insights reports.</span></span> <span data-ttu-id="1ca91-105">Você pode usar essas consultas chamando o ponto de extremidade da API Criar Consulta de Relatório.</span><span class="sxs-lookup"><span data-stu-id="1ca91-105">You can use these queries by calling the Create Report Query API endpoint.</span></span> <span data-ttu-id="1ca91-106">Se necessário, a chamada de [API de consulta criar relatório](insights-programmatic-access-paradigm.md#create-report-query-api) pode ser modificada para adicionar mais colunas, ajustar o período de computação e adicionar condições de filtro.</span><span class="sxs-lookup"><span data-stu-id="1ca91-106">If necessary, the [Create Report Query API](insights-programmatic-access-paradigm.md#create-report-query-api) call can be modified to add more columns, adjust the computation period, and add filter conditions.</span></span>

<span data-ttu-id="1ca91-107">Para obter detalhes sobre os nomes de coluna, atributos e descrições, consulte as [definições de dados](insights-data-definitions.md).</span><span class="sxs-lookup"><span data-stu-id="1ca91-107">For details about the column names, attributes, and descriptions, refer to the [Data Definitions](insights-data-definitions.md).</span></span>

## <a name="customer-details"></a><span data-ttu-id="1ca91-108">Detalhes do cliente</span><span class="sxs-lookup"><span data-stu-id="1ca91-108">Customer details</span></span>

<span data-ttu-id="1ca91-109">Estas consultas de exemplo se aplicam ao relatório detalhes dos clientes:</span><span class="sxs-lookup"><span data-stu-id="1ca91-109">These sample queries apply to the customers details report:</span></span>

### <a name="by-geography"></a><span data-ttu-id="1ca91-110">Por geografia</span><span class="sxs-lookup"><span data-stu-id="1ca91-110">By geography</span></span>

<span data-ttu-id="1ca91-111">Lista de clientes de uma geografia específica no último mês.</span><span class="sxs-lookup"><span data-stu-id="1ca91-111">List of customers from a specific geography in last month.</span></span>

```sql
SELECT CustomerName, CustomerTpid, Product 
FROM CustomersAndTenants 
WHERE CustomerMarket='United States' TIMESPAN LAST_MONTH
```

### <a name="by-sku-and-billed-revenue"></a><span data-ttu-id="1ca91-112">Por SKU e receita cobrada</span><span class="sxs-lookup"><span data-stu-id="1ca91-112">By SKU and billed revenue</span></span>

<span data-ttu-id="1ca91-113">A lista de clientes que usam SKU específica e receita cobrada é de mais de 20.000 nos últimos 6 meses</span><span class="sxs-lookup"><span data-stu-id="1ca91-113">List of customers using specific SKU and Billed Revenue is more than 20,000 in the last 6 months</span></span>

```sql
SELECT CustomerName, CustomerTpid, SKU, Month, BilledRevenueUSD 
FROM CustomersAndTenants 
WHERE SKU='MICROSOFT 365 BUSINESS STANDARD' AND BilledRevenueUSD>20000 TIMESPAN LAST_6_MONTHS
```

### <a name="by-available-seats"></a><span data-ttu-id="1ca91-114">Por estações disponíveis</span><span class="sxs-lookup"><span data-stu-id="1ca91-114">By available seats</span></span>

<span data-ttu-id="1ca91-115">10 principais clientes com base em estações disponíveis no último mês</span><span class="sxs-lookup"><span data-stu-id="1ca91-115">Top 10 customers based on Available seats in last month</span></span>

```sql
SELECT CustomerName, CustomerTpid, Product, AvailableSeats 
FROM CustomersAndTenants ORDER BY AvailableSeats DESC LIMIT 10 TIMESPAN LAST_MONTH
```

## <a name="partner-profile"></a><span data-ttu-id="1ca91-116">Perfil do parceiro</span><span class="sxs-lookup"><span data-stu-id="1ca91-116">Partner Profile</span></span>

<span data-ttu-id="1ca91-117">Estas consultas de exemplo se aplicam ao relatório perfil do parceiro:</span><span class="sxs-lookup"><span data-stu-id="1ca91-117">These sample queries apply to the partner profile report:</span></span>

### <a name="by-geography"></a><span data-ttu-id="1ca91-118">Por geografia</span><span class="sxs-lookup"><span data-stu-id="1ca91-118">By geography</span></span>

<span data-ttu-id="1ca91-119">Lista de parceiros de uma geografia específica.</span><span class="sxs-lookup"><span data-stu-id="1ca91-119">List of partners from a specific geography.</span></span>

```sql
SELECT MPNId, PartnerName 
FROM Profile 
WHERE Country='United States'
```

### <a name="by-mpn-partner"></a><span data-ttu-id="1ca91-120">Por parceiro MPN</span><span class="sxs-lookup"><span data-stu-id="1ca91-120">By MPN partner</span></span>

<span data-ttu-id="1ca91-121">Lista de parceiros sob o mesmo parceiro de PGA MPN</span><span class="sxs-lookup"><span data-stu-id="1ca91-121">List of partners under same PGA MPN Partner</span></span>

```sql
SELECT MPNId, PartnerName, PGAMpnId 
FROM Profile 
WHERE PGAMpnId='1001xx'
```

## <a name="reseller-performance"></a><span data-ttu-id="1ca91-122">Desempenho do revendedor</span><span class="sxs-lookup"><span data-stu-id="1ca91-122">Reseller Performance</span></span>

<span data-ttu-id="1ca91-123">Estas consultas de exemplo se aplicam ao relatório de desempenho revendedor:</span><span class="sxs-lookup"><span data-stu-id="1ca91-123">These sample queries apply to the reseller performance report:</span></span>

### <a name="by-geography"></a><span data-ttu-id="1ca91-124">Por geografia</span><span class="sxs-lookup"><span data-stu-id="1ca91-124">By geography</span></span>

<span data-ttu-id="1ca91-125">Lista de revendedores de uma geografia específica no último mês.</span><span class="sxs-lookup"><span data-stu-id="1ca91-125">List of resellers from a specific geography in last month.</span></span>

```sql
SELECT ResellerMpnId, ResellerName 
FROM ResellerPerformance 
WHERE ResellerMarket='US' TIMESPAN LAST_MONTH
```

### <a name="by-reseller"></a><span data-ttu-id="1ca91-126">Por revendedor</span><span class="sxs-lookup"><span data-stu-id="1ca91-126">By reseller</span></span>

<span data-ttu-id="1ca91-127">Contagem de clientes, contagem de assinaturas, estações disponíveis totais, total de estações atribuídas, receita total para um revendedor específico.</span><span class="sxs-lookup"><span data-stu-id="1ca91-127">Customer count, subscription count, total available seats, total assigned seats, total revenue for a specific reseller.</span></span>

```sql
SELECT ResellerMpnId, ResellerName, CustomerCount, SubscriptionCount, TotalAvailableSeats, TotalAssignedSeats, TotalRevenue 
FROM ResellerPerformance 
WHERE ResellerMpnId='1051xxx'
```

### <a name="top-10-by-revenue"></a><span data-ttu-id="1ca91-128">10 principais por receita</span><span class="sxs-lookup"><span data-stu-id="1ca91-128">Top 10 by revenue</span></span>

<span data-ttu-id="1ca91-129">10 principais revendedores com base na receita total no último mês.</span><span class="sxs-lookup"><span data-stu-id="1ca91-129">Top 10 resellers based on total revenue in last month.</span></span>

```sql
SELECT ResellerMpnId, ResellerName, TotalRevenue 
FROM ResellerPerformance 
ORDER BY TotalRevenue 
LIMIT 10 
TIMESPAN LAST_MONTH
```

## <a name="subscription-details"></a><span data-ttu-id="1ca91-130">Detalhes da assinatura</span><span class="sxs-lookup"><span data-stu-id="1ca91-130">Subscription Details</span></span>

<span data-ttu-id="1ca91-131">Estas consultas de exemplo se aplicam ao relatório detalhes da assinatura:</span><span class="sxs-lookup"><span data-stu-id="1ca91-131">These sample queries apply to the subscription details report:</span></span>

### <a name="by-renewal-eligibility"></a><span data-ttu-id="1ca91-132">Por qualificação para renovação</span><span class="sxs-lookup"><span data-stu-id="1ca91-132">By renewal eligibility</span></span>

<span data-ttu-id="1ca91-133">Lista de assinaturas que não estão qualificadas para renovação automática no último mês.</span><span class="sxs-lookup"><span data-stu-id="1ca91-133">List of subscriptions who are not eligible for auto renewal in last month.</span></span>

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE IsAutoRenew='N' TIMESPAN LAST_MONTH
```

### <a name="by-subscription-state"></a><span data-ttu-id="1ca91-134">Por estado de assinatura</span><span class="sxs-lookup"><span data-stu-id="1ca91-134">By subscription state</span></span>

<span data-ttu-id="1ca91-135">Lista de assinaturas que estão no estado de desabilitação no último mês.</span><span class="sxs-lookup"><span data-stu-id="1ca91-135">List of subscriptions who are in Disable state in last month.</span></span>

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE SubscriptionState='Disabled' TIMESPAN LAST_MONTH
```

### <a name="counts-for-six-months"></a><span data-ttu-id="1ca91-136">Contagens por seis meses</span><span class="sxs-lookup"><span data-stu-id="1ca91-136">Counts for six months</span></span>

<span data-ttu-id="1ca91-137">Contagem de assinaturas, total de estações vendidas, contagem de clientes para um parceiro específico nos últimos seis meses.</span><span class="sxs-lookup"><span data-stu-id="1ca91-137">Subscription count, total sold seats, customer count for a specific partner in last six months.</span></span>

```sql
SELECT MPNId, SubscriptionCount, TotalSoldSeats, BilledRevenueUSD, CustomerCount 
FROM SeatsSubscriptionsAndRevenue 
WHERE MPNId=6096xxx TIMESPAN LAST_6_MONTHS
```

## <a name="azure-usage"></a><span data-ttu-id="1ca91-138">Uso do Azure</span><span class="sxs-lookup"><span data-stu-id="1ca91-138">Azure Usage</span></span>

<span data-ttu-id="1ca91-139">Estas consultas de exemplo se aplicam ao relatório de uso do Azure:</span><span class="sxs-lookup"><span data-stu-id="1ca91-139">These sample queries apply to the Azure usage report:</span></span>

### <a name="by-meter-category"></a><span data-ttu-id="1ca91-140">Por categoria de medidor</span><span class="sxs-lookup"><span data-stu-id="1ca91-140">By meter category</span></span>

<span data-ttu-id="1ca91-141">Lista de assinaturas de uso do Azure com unidades de uso e ACR para categoria de medidor específico nos últimos seis meses.</span><span class="sxs-lookup"><span data-stu-id="1ca91-141">List of Azure usage subscriptions with usage units and ACR for specific meter category in last six months.</span></span>

```sql
SELECT SubscriptionId, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE MeterCategory='Azure DNS' 
TIMESPAN LAST_6_MONTHS
```

### <a name="by-total-acr"></a><span data-ttu-id="1ca91-142">Por ACR total</span><span class="sxs-lookup"><span data-stu-id="1ca91-142">By total ACR</span></span>

<span data-ttu-id="1ca91-143">Lista de assinaturas de uso do Azure em que o ACR total é maior que 20.000 nos últimos seis meses</span><span class="sxs-lookup"><span data-stu-id="1ca91-143">List of Azure usage subscriptions where total ACR is greater than 20,000 in last six months</span></span>

```sql
SELECT SubscriptionId, ServiceName, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE TotalACR>20000 TIMESPAN LAST_6_MONTHS
```

## <a name="next-steps"></a><span data-ttu-id="1ca91-144">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="1ca91-144">Next steps</span></span>

- [<span data-ttu-id="1ca91-145">APIs para acessar dados de análise de informações de parceiros</span><span class="sxs-lookup"><span data-stu-id="1ca91-145">APIs for accessing partner insights analytics data</span></span>](insights-programmatic-analytics-available-api.md)