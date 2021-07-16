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
# <a name="sample-queries-for-partner-center-insights-report"></a>Exemplos de consultas para o relatório do Partner Center insights

este artigo fornece exemplos de consultas para os relatórios de Insights de parceiros. Você pode usar essas consultas chamando o ponto de extremidade da API Criar Consulta de Relatório. Se necessário, a chamada de [API de consulta criar relatório](insights-programmatic-access-paradigm.md#create-report-query-api) pode ser modificada para adicionar mais colunas, ajustar o período de computação e adicionar condições de filtro.

Para obter detalhes sobre os nomes de coluna, atributos e descrições, consulte as [definições de dados](insights-data-definitions.md).

## <a name="customer-details"></a>Detalhes do cliente

Estas consultas de exemplo se aplicam ao relatório detalhes dos clientes:

### <a name="by-geography"></a>Por geografia

Lista de clientes de uma geografia específica no último mês.

```sql
SELECT CustomerName, CustomerTpid, Product 
FROM CustomersAndTenants 
WHERE CustomerMarket='United States' TIMESPAN LAST_MONTH
```

### <a name="by-sku-and-billed-revenue"></a>Por SKU e receita cobrada

A lista de clientes que usam SKU específica e receita cobrada é de mais de 20.000 nos últimos 6 meses

```sql
SELECT CustomerName, CustomerTpid, SKU, Month, BilledRevenueUSD 
FROM CustomersAndTenants 
WHERE SKU='MICROSOFT 365 BUSINESS STANDARD' AND BilledRevenueUSD>20000 TIMESPAN LAST_6_MONTHS
```

### <a name="by-available-seats"></a>Por estações disponíveis

10 principais clientes com base em estações disponíveis no último mês

```sql
SELECT CustomerName, CustomerTpid, Product, AvailableSeats 
FROM CustomersAndTenants ORDER BY AvailableSeats DESC LIMIT 10 TIMESPAN LAST_MONTH
```

## <a name="partner-profile"></a>Perfil do parceiro

Estas consultas de exemplo se aplicam ao relatório perfil do parceiro:

### <a name="by-geography"></a>Por geografia

Lista de parceiros de uma geografia específica.

```sql
SELECT MPNId, PartnerName 
FROM Profile 
WHERE Country='United States'
```

### <a name="by-mpn-partner"></a>Por parceiro MPN

Lista de parceiros sob o mesmo parceiro de PGA MPN

```sql
SELECT MPNId, PartnerName, PGAMpnId 
FROM Profile 
WHERE PGAMpnId='1001xx'
```

## <a name="reseller-performance"></a>Desempenho do revendedor

Estas consultas de exemplo se aplicam ao relatório de desempenho revendedor:

### <a name="by-geography"></a>Por geografia

Lista de revendedores de uma geografia específica no último mês.

```sql
SELECT ResellerMpnId, ResellerName 
FROM ResellerPerformance 
WHERE ResellerMarket='US' TIMESPAN LAST_MONTH
```

### <a name="by-reseller"></a>Por revendedor

Contagem de clientes, contagem de assinaturas, estações disponíveis totais, total de estações atribuídas, receita total para um revendedor específico.

```sql
SELECT ResellerMpnId, ResellerName, CustomerCount, SubscriptionCount, TotalAvailableSeats, TotalAssignedSeats, TotalRevenue 
FROM ResellerPerformance 
WHERE ResellerMpnId='1051xxx'
```

### <a name="top-10-by-revenue"></a>10 principais por receita

10 principais revendedores com base na receita total no último mês.

```sql
SELECT ResellerMpnId, ResellerName, TotalRevenue 
FROM ResellerPerformance 
ORDER BY TotalRevenue 
LIMIT 10 
TIMESPAN LAST_MONTH
```

## <a name="subscription-details"></a>Detalhes da assinatura

Estas consultas de exemplo se aplicam ao relatório detalhes da assinatura:

### <a name="by-renewal-eligibility"></a>Por qualificação para renovação

Lista de assinaturas que não estão qualificadas para renovação automática no último mês.

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE IsAutoRenew='N' TIMESPAN LAST_MONTH
```

### <a name="by-subscription-state"></a>Por estado de assinatura

Lista de assinaturas que estão no estado de desabilitação no último mês.

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE SubscriptionState='Disabled' TIMESPAN LAST_MONTH
```

### <a name="counts-for-six-months"></a>Contagens por seis meses

Contagem de assinaturas, total de estações vendidas, contagem de clientes para um parceiro específico nos últimos seis meses.

```sql
SELECT MPNId, SubscriptionCount, TotalSoldSeats, BilledRevenueUSD, CustomerCount 
FROM SeatsSubscriptionsAndRevenue 
WHERE MPNId=6096xxx TIMESPAN LAST_6_MONTHS
```

## <a name="azure-usage"></a>Uso do Azure

Estas consultas de exemplo se aplicam ao relatório de uso do Azure:

### <a name="by-meter-category"></a>Por categoria de medidor

Lista de assinaturas de uso do Azure com unidades de uso e ACR para categoria de medidor específico nos últimos seis meses.

```sql
SELECT SubscriptionId, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE MeterCategory='Azure DNS' 
TIMESPAN LAST_6_MONTHS
```

### <a name="by-total-acr"></a>Por ACR total

Lista de assinaturas de uso do Azure em que o ACR total é maior que 20.000 nos últimos seis meses

```sql
SELECT SubscriptionId, ServiceName, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE TotalACR>20000 TIMESPAN LAST_6_MONTHS
```

## <a name="next-steps"></a>Próximas etapas

- [APIs para acessar dados de análise de informações de parceiros](insights-programmatic-analytics-available-api.md)