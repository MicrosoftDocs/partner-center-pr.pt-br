---
title: Usar a análise do Partner Center para Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como exibir seus dados de negócios usando o aplicativo de análise do Partner Center para Power BI (para parceiros diretos no CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 244cb852728d47360cf8ecd1d1e9ccb641466b1d
ms.sourcegitcommit: 1a0c83e2089cb58221bdb24525127378f5197ea8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/14/2021
ms.locfileid: "98215740"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="a48d8-103">Visualize seus dados de negócio com o aplicativo de análise do Partner Center para Microsoft Power BI</span><span class="sxs-lookup"><span data-stu-id="a48d8-103">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>



<span data-ttu-id="a48d8-104">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="a48d8-104">**Appropriate roles**</span></span>

- <span data-ttu-id="a48d8-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="a48d8-105">Global admin</span></span>
- <span data-ttu-id="a48d8-106">Administrador de usuários</span><span class="sxs-lookup"><span data-stu-id="a48d8-106">User admin</span></span>
- <span data-ttu-id="a48d8-107">Agente de vendas</span><span class="sxs-lookup"><span data-stu-id="a48d8-107">Sales agent</span></span>
- <span data-ttu-id="a48d8-108">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="a48d8-108">Admin agent</span></span>

## <a name="view-your-business-data"></a><span data-ttu-id="a48d8-109">Visualize seus dados de negócio</span><span class="sxs-lookup"><span data-stu-id="a48d8-109">View your business data</span></span>

<span data-ttu-id="a48d8-110">Obtenha uma representação visual de seus dados corporativos com o aplicativo de análise do Partner Center para Power BI, incluindo:</span><span class="sxs-lookup"><span data-stu-id="a48d8-110">Get a visual representation of your business data with the Partner Center Analytics app for Power BI, including:</span></span>

- <span data-ttu-id="a48d8-111">Crescimento de sua base de clientes, assinaturas e licenças</span><span class="sxs-lookup"><span data-stu-id="a48d8-111">Growth of your customer base, subscriptions, and licenses</span></span>

- <span data-ttu-id="a48d8-112">O uso de produtos do Office 365, Microsoft Dynamics e Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="a48d8-112">Usage of Office 365, Microsoft Dynamics, and Microsoft Azure products</span></span>

- <span data-ttu-id="a48d8-113">As unidades de consumo diário de cada recurso limitado em cada assinatura do Azure nos últimos 60 dias</span><span class="sxs-lookup"><span data-stu-id="a48d8-113">Daily consumption units for each metered resource in each Azure subscription for the last 60 days</span></span>

- <span data-ttu-id="a48d8-114">Custo estimado (com base na tabela de tarifas mais recente)</span><span class="sxs-lookup"><span data-stu-id="a48d8-114">Estimated cost (based on latest rate card)</span></span>

- <span data-ttu-id="a48d8-115">Capacidade de exportar conjuntos de clientes e criar relatórios personalizados, incluindo por cliente.</span><span class="sxs-lookup"><span data-stu-id="a48d8-115">Ability to export datasets and create custom reports, including per customer.</span></span>

### <a name="about-the-partner-center-analytics-app-preview-release"></a><span data-ttu-id="a48d8-116">Sobre a versão de visualização do aplicativo de análises do Partner Center</span><span class="sxs-lookup"><span data-stu-id="a48d8-116">About the Partner Center Analytics app preview release</span></span>

- <span data-ttu-id="a48d8-117">Este aplicativo é apenas para provedores diretos no programa Provedor de Soluções na Nuvem</span><span class="sxs-lookup"><span data-stu-id="a48d8-117">This app is for direct partners in the Cloud Solution Provider program only.</span></span> <span data-ttu-id="a48d8-118">Outros parceiros no CSP (revendedores indiretos, por exemplo) não poderão se conectar.</span><span class="sxs-lookup"><span data-stu-id="a48d8-118">Other partners in CSP (indirect resellers, for example) will not be able to sign in.</span></span>

- <span data-ttu-id="a48d8-119">Todos os custos estimados são pré-taxados na cobrança/ dados da fatura, e não são vinculados legalmente.</span><span class="sxs-lookup"><span data-stu-id="a48d8-119">Any estimated costs are pre-tax billing / invoice data, and are not legally binding.</span></span> <span data-ttu-id="a48d8-120">Os Custos estimados destinam-se a ser usados somente para percepções.</span><span class="sxs-lookup"><span data-stu-id="a48d8-120">Estimated costs are meant to be used for data insights only.</span></span>

- <span data-ttu-id="a48d8-121">As informações do cliente são baseadas em assinaturas.</span><span class="sxs-lookup"><span data-stu-id="a48d8-121">Customer information is based on subscriptions.</span></span> <span data-ttu-id="a48d8-122">Todos os clientes para os quais você criou contas recentemente, mas que ainda não tem assinaturas, não estão incluídos nas contagens.</span><span class="sxs-lookup"><span data-stu-id="a48d8-122">Any customers that you've recently created accounts for, but who do not yet have subscriptions, are not included in counts.</span></span>

- <span data-ttu-id="a48d8-123">Os custos estimados baseiam-se na tabela de taxa mais recente, que baseia-se nos preços CSP.</span><span class="sxs-lookup"><span data-stu-id="a48d8-123">Estimated cost is based on latest rate card, which is based on CSP pricing.</span></span>

- <span data-ttu-id="a48d8-124">Os dias são dias calendários.</span><span class="sxs-lookup"><span data-stu-id="a48d8-124">Days are calendar days.</span></span>

### <a name="business-insights-report"></a><span data-ttu-id="a48d8-125">Relatório de ideias de negócios</span><span class="sxs-lookup"><span data-stu-id="a48d8-125">Business Insights report</span></span>

- <span data-ttu-id="a48d8-126">**Locatários do cliente**: Número de locatários Azure distintos de clientes que adquiriram assinaturas</span><span class="sxs-lookup"><span data-stu-id="a48d8-126">**Customer tenants**: Number of distinct Azure AD tenants of customers that have purchased subscriptions</span></span>

- <span data-ttu-id="a48d8-127">**Novo (últimos 30 dias)**: Novos clientes comprando pelo menos uma assinatura nos últimos 30 dias</span><span class="sxs-lookup"><span data-stu-id="a48d8-127">**New (last 30 days)**: New customers purchasing at least one subscription in last 30 days</span></span>

- <span data-ttu-id="a48d8-128">**Rotatividade (últimos 30 dias)**: clientes sem nenhuma assinatura "ativa", "em cortesia" ou "desabilitada"</span><span class="sxs-lookup"><span data-stu-id="a48d8-128">**Churn (last 30 days)**: Customers without any “active", “in grace" or “disabled" subscriptions</span></span>

- <span data-ttu-id="a48d8-129">**Novo (últimas 24 horas)**: Novos clientes comprando pelo menos uma assinatura nos últimas 24 horas</span><span class="sxs-lookup"><span data-stu-id="a48d8-129">**New (last 24 hours)**: New customers purchasing at least one subscription in last 24 hours</span></span>

- <span data-ttu-id="a48d8-130">**Custo mensal estimado nos últimos 12 meses**: Tendência mês a mês do valor pré-taxado em dólar estimado para a fatura agregado mensalmente durante o período dos últimos 12 meses</span><span class="sxs-lookup"><span data-stu-id="a48d8-130">**Estimated monthly cost over last 12 months**: Month over month trend of estimated pre-tax invoice dollar amount aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="a48d8-131">**Custo mensal por produto estimado nos últimos 12 meses**: Produtos vendidos classificados pelo valor pré-taxado em dólar estimado para a fatura agregado mensalmente durante o período dos últimos 12 meses.</span><span class="sxs-lookup"><span data-stu-id="a48d8-131">**Estimated cost by product over last 12 months**: Products sold sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="a48d8-132">Esse status indica os principais produtos que trazem a maior parte da receita.</span><span class="sxs-lookup"><span data-stu-id="a48d8-132">This status indicates top products bringing most revenue.</span></span>

- <span data-ttu-id="a48d8-133">**Clientes nos últimos 12 meses**: Tendência mês a mês de novos clientes e clientes de variação agregados mensalmente durante o período de últimos 12 meses</span><span class="sxs-lookup"><span data-stu-id="a48d8-133">**Customers over last 12 months**: Month over month trend of new customers and churn customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="a48d8-134">**Custo mensal por cliente estimado nos últimos 12 meses**: Clientes classificados pelo valor pré-taxado em dólar estimado para a fatura agregado mensalmente durante o período dos últimos 12 meses.</span><span class="sxs-lookup"><span data-stu-id="a48d8-134">**Estimated cost by customer over last 12 months**: Customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="a48d8-135">Esse status indica os principais clientes que trazem mais receita.</span><span class="sxs-lookup"><span data-stu-id="a48d8-135">This status indicates top customers bringing most revenue.</span></span>

- <span data-ttu-id="a48d8-136">**Contagem de cliente por produto**: Produtos vendidos classificados por clientes associados.</span><span class="sxs-lookup"><span data-stu-id="a48d8-136">**Customer count by product**: Products sold sorted by associated customers.</span></span> <span data-ttu-id="a48d8-137">Esse status indica os principais produtos vendidos para a maioria dos clientes.</span><span class="sxs-lookup"><span data-stu-id="a48d8-137">This status indicates top products sold to most customers.</span></span>

### <a name="subscription-insights-report"></a><span data-ttu-id="a48d8-138">Relatório de ideias de assinatura</span><span class="sxs-lookup"><span data-stu-id="a48d8-138">Subscription Insights report</span></span>

- <span data-ttu-id="a48d8-139">**Status da assinatura**:</span><span class="sxs-lookup"><span data-stu-id="a48d8-139">**Subscription status**:</span></span>

- <span data-ttu-id="a48d8-140">Ativo: assinaturas pertencentes ao estado "ativo" ou "em carência"</span><span class="sxs-lookup"><span data-stu-id="a48d8-140">Active: Subscriptions belonging to either “active" or “in grace" state</span></span>

  - <span data-ttu-id="a48d8-141">Suspenso: assinaturas que pertencem ao estado "desabilitado"</span><span class="sxs-lookup"><span data-stu-id="a48d8-141">Suspended: Subscriptions belonging to “disabled" state</span></span>

  - <span data-ttu-id="a48d8-142">Desprovisionado: assinaturas que pertencem ao status "desprovisionado" ou "expirado"</span><span class="sxs-lookup"><span data-stu-id="a48d8-142">De-provisioned: Subscriptions belonging to “de-provisioned" or “expired" status</span></span>

- <span data-ttu-id="a48d8-143">**Status de expiração**:</span><span class="sxs-lookup"><span data-stu-id="a48d8-143">**Expiry status**:</span></span>

  - <span data-ttu-id="a48d8-144">Expirado: Assinaturas que já expiraram (onde a data de término da assinatura está no passado)</span><span class="sxs-lookup"><span data-stu-id="a48d8-144">Expired: Subscriptions that have already expired (where subscription end date is in past)</span></span>

  - <span data-ttu-id="a48d8-145">Expiram após 30 dias: Assinaturas que expirarão após 30 dias (onde data de término da assinatura é depois dos próximos 30 dias)</span><span class="sxs-lookup"><span data-stu-id="a48d8-145">Expiring after 30 days: Subscriptions that will expire after 30 days (where subscription end date is after next 30 days)</span></span>

  - <span data-ttu-id="a48d8-146">Expiram em 30 dias: Assinaturas que expirarão nos próximos 30 dias (onde data de término da assinatura é entre hoje e os próximos 30 dias)</span><span class="sxs-lookup"><span data-stu-id="a48d8-146">Expiring in 30 days: Subscriptions that will expire within next 30 days (where subscription end date is between today and next 30 days)</span></span>

- <span data-ttu-id="a48d8-147">**Total de assinaturas**: assinaturas no status "ativo", "em carência" ou "desabilitado"</span><span class="sxs-lookup"><span data-stu-id="a48d8-147">**Total subscriptions**: Subscriptions in “active," “in grace" or “disabled" status</span></span>

- <span data-ttu-id="a48d8-148">**Novo (últimos 30 dias)**: Novas assinaturas compradas por clientes nos últimos 30 dias</span><span class="sxs-lookup"><span data-stu-id="a48d8-148">**New (last 30 days)**: New subscriptions purchased by customers within last 30 days</span></span>

- <span data-ttu-id="a48d8-149">**Novo (últimas 24 horas)**: Novas assinaturas compradas por clientes nas últimas 24 horas</span><span class="sxs-lookup"><span data-stu-id="a48d8-149">**New (last 24 hours)**: New subscriptions purchased by customers within last 24 hours</span></span>

- <span data-ttu-id="a48d8-150">**Expira em 30 dias**: Assinaturas que expirarão nos próximos 30 dias</span><span class="sxs-lookup"><span data-stu-id="a48d8-150">**Expiring in 30 days**: Subscriptions that will expire within next 30 days</span></span>

- <span data-ttu-id="a48d8-151">**Rotatividade (últimos 30 dias)**: Assinaturas que tiveram o provisionamento cancelado ou que foram suspensas (desabilitadas) nos últimos 30 dias</span><span class="sxs-lookup"><span data-stu-id="a48d8-151">**Churn (last 30 days)**: Subscriptions that have been de-provisioned or Suspended (disabled) within last 30 days</span></span>

- <span data-ttu-id="a48d8-152">**Distribuição por tipos de assinatura**:% de distribuição de assinaturas totais por licença com base em tipo de assinatura baseada em uso</span><span class="sxs-lookup"><span data-stu-id="a48d8-152">**Distribution by subscription types**: % distribution of total subscriptions by License based and usage-based subscription type</span></span>

- <span data-ttu-id="a48d8-153">**Contagem de assinatura ativa por produto**: Produtos vendidos classificados por contagem de assinaturas ativas</span><span class="sxs-lookup"><span data-stu-id="a48d8-153">**Active subscription count by product**: Products sold sorted by active subscriptions count</span></span>

- <span data-ttu-id="a48d8-154">**Assinaturas nos últimos 12 meses**: Tendência mês a mês de novas assinaturas e assinaturas com rotatividade agregadas mensalmente durante o período de últimos 12 meses</span><span class="sxs-lookup"><span data-stu-id="a48d8-154">**Subscriptions over last 12 months**: Month over month trend of new subscriptions and churn subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="a48d8-155">**Detalhes da assinatura do cliente**: exibição detalhada dos clientes, assinaturas e ofertas</span><span class="sxs-lookup"><span data-stu-id="a48d8-155">**Customer subscription details**: Detailed view of the customers, subscriptions, and offers</span></span>

### <a name="license-insights-report"></a><span data-ttu-id="a48d8-156">Relatório de ideias de licença:</span><span class="sxs-lookup"><span data-stu-id="a48d8-156">License Insights report:</span></span>

- <span data-ttu-id="a48d8-157">**Total de licenças**: o número total de licenças agregadas em todas as assinaturas baseadas em licença</span><span class="sxs-lookup"><span data-stu-id="a48d8-157">**Total licenses**: Total number of licenses aggregated across all license-based subscriptions</span></span>

- <span data-ttu-id="a48d8-158">**Novo (últimos 30 dias)**: Adição de licenças nos últimos 30 dias</span><span class="sxs-lookup"><span data-stu-id="a48d8-158">**New (last 30 days)**: License addition within last 30 days</span></span>

- <span data-ttu-id="a48d8-159">**Rotatividade (últimos 30 dias)**: Redução de licenças nos últimos 30 dias</span><span class="sxs-lookup"><span data-stu-id="a48d8-159">**Churn (last 30 days)**: License reduction within last 30 days</span></span>

- <span data-ttu-id="a48d8-160">**Novo (últimas 24 horas)**: Adição de licenças nas últimas 24 horas</span><span class="sxs-lookup"><span data-stu-id="a48d8-160">**New (last 24 hours)**: License addition within last 24 hours</span></span>

- <span data-ttu-id="a48d8-161">**Licenças nos últimos 90 dias**: Tendência mês a mês de adições e reduções de licença agregadas mensalmente durante o período dos últimos 90 dias</span><span class="sxs-lookup"><span data-stu-id="a48d8-161">**Licenses over last 90 days**: Month over month trend of license additions and reductions aggregated monthly over the period of last 90 days</span></span>

- <span data-ttu-id="a48d8-162">**Contagem de licença ativa por produto**: Produtos vendidos classificados por contagem de licenças ativas</span><span class="sxs-lookup"><span data-stu-id="a48d8-162">**Active license count by product**: Products sold sorted by active license count</span></span>

- <span data-ttu-id="a48d8-163">**Contagem de licenças ativas por cliente**: clientes classificados por contagem de licenças ativas</span><span class="sxs-lookup"><span data-stu-id="a48d8-163">**Active license count by customer**: Customers sorted by active license count</span></span>

- <span data-ttu-id="a48d8-164">**Detalhes do evento de licença do cliente nos últimos 90 dias**: exibição detalhada dos clientes, assinaturas e eventos de assinatura, incluindo data do evento, nome do evento, quantidade e alteração na quantidade.</span><span class="sxs-lookup"><span data-stu-id="a48d8-164">**Customer license event details over last 90 days**: Detailed view of the customers, subscriptions, and subscription events including event date, event name, quantity, and change in quantity.</span></span>

### <a name="licenses-usage-report"></a><span data-ttu-id="a48d8-165">Relatório de uso de licenças:</span><span class="sxs-lookup"><span data-stu-id="a48d8-165">Licenses Usage report:</span></span>

- <span data-ttu-id="a48d8-166">**Licenças atribuídas por produto**: Produtos vendidos classificados por contagem de atribuição</span><span class="sxs-lookup"><span data-stu-id="a48d8-166">**Licenses assigned by product**: Products sold sorted by license assignment count</span></span>

- <span data-ttu-id="a48d8-167">**Licenças em uso por produto**: Produtos vendidos classificados por contagem de uso de licença</span><span class="sxs-lookup"><span data-stu-id="a48d8-167">**Licenses in use by product**: Products sold sorted by license usage count</span></span>

- <span data-ttu-id="a48d8-168">**Distribuição de cliente de licenças atribuídas**: distribuição % do total de clientes desfeitos em classificações de faixas de 20% por % de atribuição de licença</span><span class="sxs-lookup"><span data-stu-id="a48d8-168">**Customer distribution of licenses assigned**: % distribution of total customers broken in buckets of 20% range by license assignment %</span></span>

- <span data-ttu-id="a48d8-169">**Distribuição de cliente de licenças em uso**: distribuição % do total de clientes desfeitos em classificações de faixas de 20% por % de uso de licença</span><span class="sxs-lookup"><span data-stu-id="a48d8-169">**Customer distribution of licenses in use**: % distribution of total customers broken in buckets of 20% range by license usage %</span></span>

- <span data-ttu-id="a48d8-170">**Licenças atribuídas pelo cliente**: Visualização detalhada de licenças vendidas e licenças atribuídas por cliente e produto</span><span class="sxs-lookup"><span data-stu-id="a48d8-170">**Licenses assigned by customer**: Detailed view of licenses sold and licenses assigned by customers and products</span></span>

- <span data-ttu-id="a48d8-171">**Licenças em uso por cliente**: Visualização detalhada de licenças em uso por cliente e produto</span><span class="sxs-lookup"><span data-stu-id="a48d8-171">**Licenses in use by customer**: Detailed view of licenses sold and licenses in use by customers and products</span></span>

### <a name="azure-insights-report"></a><span data-ttu-id="a48d8-172">Relatório de ideias do Azure:</span><span class="sxs-lookup"><span data-stu-id="a48d8-172">Azure Insights report:</span></span>

- <span data-ttu-id="a48d8-173">**Clientes baseados em uso nos últimos 12 meses**: tendência de mês a mês de novos clientes baseados em uso e clientes baseados em uso com variação agregados mensalmente durante o período dos últimos 12 meses</span><span class="sxs-lookup"><span data-stu-id="a48d8-173">**Usage-based customers over last 12 months**: Month over month trend of new usage-based customers and churned usage-based customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="a48d8-174">**Assinaturas baseadas em uso nos últimos 12 meses**: tendência de mês a mês de novas assinaturas baseadas em uso e assinaturas baseadas em uso com rotatividade agregadas mensalmente durante o período dos últimos 12 meses</span><span class="sxs-lookup"><span data-stu-id="a48d8-174">**Usage-based subscriptions over last 12 months**: Month over month trend of new usage-based subscriptions and churned usage-based subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="a48d8-175">**Custo estimado de uso pelo cliente nos últimos 60 dias**: clientes com base no uso classificados por valor estimado em dólar de nota fiscal de imposto agregado no período dos últimos 60 dias.</span><span class="sxs-lookup"><span data-stu-id="a48d8-175">**Estimated cost of usage by customer over last 60 days**: Usage-based customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span> <span data-ttu-id="a48d8-176">Esse status indica os principais clientes baseados em uso que trazem a maior parte da receita</span><span class="sxs-lookup"><span data-stu-id="a48d8-176">This status indicates top usage-based customers bringing most revenue</span></span>

- <span data-ttu-id="a48d8-177">**Custo estimado de uso por categoria nos últimos 60 dias**: categorias de medidores de assinaturas baseadas em uso classificadas pelo valor estimado de dólar da nota fiscal de imposto sobre o período dos últimos 60 dias.</span><span class="sxs-lookup"><span data-stu-id="a48d8-177">**Estimated cost of usage by category over last 60 days**: Meter categories of usage-based subscriptions sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="a48d8-178">**Custo estimado de uso por assinatura nos últimos 60 dias**: assinaturas com base no uso pelo valor estimado em dólar de nota fiscal de imposto agregado no período dos últimos 60 dias.</span><span class="sxs-lookup"><span data-stu-id="a48d8-178">**Estimated cost of usage by subscription over last 60 days**: Usage-based subscriptions by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="a48d8-179">**Custos estimados de uso de cliente por orçamento de gastos**: Clientes classificados por percentual de seu orçamento de gastos com uso atual excedendo o limite (100%).</span><span class="sxs-lookup"><span data-stu-id="a48d8-179">**Customer estimated usage cost by spending budget**: Customers sorted by percentage of their current usage spending budget exceeding threshold (100%).</span></span>

### <a name="azure-resource-usage-report"></a><span data-ttu-id="a48d8-180">Relatório de uso de recurso Azure:</span><span class="sxs-lookup"><span data-stu-id="a48d8-180">Azure Resource Usage report:</span></span>

- <span data-ttu-id="a48d8-181">**Uso de recursos do Azure por dia para o período selecionado**: unidades de consumo diário para cada recurso medido em cada assinatura baseada em uso para o período selecionado nos últimos 60 dias.</span><span class="sxs-lookup"><span data-stu-id="a48d8-181">**Usage of Azure resources by day for selected period**: Daily consumption units for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span>

- <span data-ttu-id="a48d8-182">**Custo estimado de uso dos recursos do Azure para o período selecionado**: custo estimado com base no cartão de taxas mais recente para cada recurso medido em cada assinatura baseada em uso para o período selecionado nos últimos 60 dias.</span><span class="sxs-lookup"><span data-stu-id="a48d8-182">**Estimated usage cost of Azure resources for selected period**: Estimated cost based on latest rate card for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="a48d8-183">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="a48d8-183">Next steps</span></span>

- [<span data-ttu-id="a48d8-184">Visão geral do aplicativo de análise do Partner Center para Power BI</span><span class="sxs-lookup"><span data-stu-id="a48d8-184">Partner Center Analytics for Power BI app overview</span></span>](power-bi-app-for-direct-partners.md)

- [<span data-ttu-id="a48d8-185">Instalar e visualizar o aplicativo Análise do Partner Center para Microsoft Power BI</span><span class="sxs-lookup"><span data-stu-id="a48d8-185">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-install.md)
