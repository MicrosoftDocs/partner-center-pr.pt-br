---
title: Aplicativo de análise do Partner Center para Power BI | Partner Center
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Use o aplicativo de análise do Partner Center para Power BI (parceiros diretos no CSP)
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 4db94f32b035be52dea575d4f731d981beb8c1b8
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "73652230"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="130a0-103">Visualize seus dados de negócio com o aplicativo de análise do Partner Center para Microsoft Power BI</span><span class="sxs-lookup"><span data-stu-id="130a0-103">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>

<span data-ttu-id="130a0-104">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="130a0-104">**Applies to**</span></span>

-   <span data-ttu-id="130a0-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="130a0-105">Partner Center</span></span>

## <a name="view-your-business-data"></a><span data-ttu-id="130a0-106">Visualize seus dados de negócio</span><span class="sxs-lookup"><span data-stu-id="130a0-106">View your business data</span></span>

<span data-ttu-id="130a0-107">Obtenha uma representação visual de seus dados corporativos com o aplicativo de análise do Partner Center para Power BI, incluindo:</span><span class="sxs-lookup"><span data-stu-id="130a0-107">Get a visual representation of your business data with the Partner Center Analytics app for Power BI, including:</span></span>

- <span data-ttu-id="130a0-108">Crescimento de sua base de clientes, assinaturas e licenças</span><span class="sxs-lookup"><span data-stu-id="130a0-108">Growth of your customer base, subscriptions, and licenses</span></span>

- <span data-ttu-id="130a0-109">O uso de produtos do Office 365, Microsoft Dynamics e Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="130a0-109">Usage of Office 365, Microsoft Dynamics, and Microsoft Azure products</span></span>

- <span data-ttu-id="130a0-110">As unidades de consumo diário de cada recurso limitado em cada assinatura do Azure nos últimos 60 dias</span><span class="sxs-lookup"><span data-stu-id="130a0-110">Daily consumption units for each metered resource in each Azure subscription for the last 60 days</span></span>

- <span data-ttu-id="130a0-111">Custo estimado (com base na tabela de tarifas mais recente)</span><span class="sxs-lookup"><span data-stu-id="130a0-111">Estimated cost (based on latest rate card)</span></span>

- <span data-ttu-id="130a0-112">Capacidade de exportar conjuntos de dados e criar relatórios personalizados, incluindo por cliente</span><span class="sxs-lookup"><span data-stu-id="130a0-112">Ability to export datasets and create custom reports, including per customer</span></span> 

### <a name="about-the-partner-center-analytics-app-preview-release"></a><span data-ttu-id="130a0-113">Sobre a versão de visualização do aplicativo de análises do Partner Center</span><span class="sxs-lookup"><span data-stu-id="130a0-113">About the Partner Center Analytics app preview release</span></span>

 - <span data-ttu-id="130a0-114">Este aplicativo é apenas para provedores diretos no programa Provedor de Soluções na Nuvem</span><span class="sxs-lookup"><span data-stu-id="130a0-114">This app is for direct partners in the Cloud Solution Provider program only.</span></span> <span data-ttu-id="130a0-115">Outros parceiros no CSP (revendedores indiretos, por exemplo) não poderão se conectar.</span><span class="sxs-lookup"><span data-stu-id="130a0-115">Other partners in CSP (indirect resellers, for example) will not be able to sign in.</span></span>

- <span data-ttu-id="130a0-116">Todos os custos estimados são pré-taxados na cobrança/ dados da fatura, e não são vinculados legalmente.</span><span class="sxs-lookup"><span data-stu-id="130a0-116">Any estimated costs are pre-tax billing / invoice data, and are not legally binding.</span></span> <span data-ttu-id="130a0-117">Os Custos estimados destinam-se a ser usados somente para percepções.</span><span class="sxs-lookup"><span data-stu-id="130a0-117">Estimated costs are meant to be used for data insights only.</span></span>

- <span data-ttu-id="130a0-118">As informações do cliente são baseadas em assinaturas.</span><span class="sxs-lookup"><span data-stu-id="130a0-118">Customer information is based on subscriptions.</span></span> <span data-ttu-id="130a0-119">Todos os clientes para os quais você criou contas recentemente, mas que ainda não tem assinaturas, não estão incluídos nas contagens.</span><span class="sxs-lookup"><span data-stu-id="130a0-119">Any customers that you've recently created accounts for, but who do not yet have subscriptions, are not included in counts.</span></span> 

- <span data-ttu-id="130a0-120">Os custos estimados baseiam-se na tabela de taxa mais recente, que baseia-se nos preços CSP.</span><span class="sxs-lookup"><span data-stu-id="130a0-120">Estimated cost is based on latest rate card, which is based on CSP pricing.</span></span> 

- <span data-ttu-id="130a0-121">Os dias são dias calendários.</span><span class="sxs-lookup"><span data-stu-id="130a0-121">Days are calendar days.</span></span> 


### <a name="business-insights-report"></a><span data-ttu-id="130a0-122">Relatório de ideias de negócios</span><span class="sxs-lookup"><span data-stu-id="130a0-122">Business Insights report</span></span>

-  <span data-ttu-id="130a0-123">**Locatários do cliente**: Número de locatários Azure distintos de clientes que adquiriram assinaturas</span><span class="sxs-lookup"><span data-stu-id="130a0-123">**Customer tenants**: Number of distinct Azure AD tenants of customers that have purchased subscriptions</span></span>

-  <span data-ttu-id="130a0-124">**Novo (últimos 30 dias)** : Novos clientes comprando pelo menos uma assinatura nos últimos 30 dias</span><span class="sxs-lookup"><span data-stu-id="130a0-124">**New (last 30 days)**: New customers purchasing at least one subscription in last 30 days</span></span>

-  <span data-ttu-id="130a0-125">**Rotatividade (últimos 30 dias)** : clientes sem nenhuma assinatura "ativa", "em cortesia" ou "desabilitada"</span><span class="sxs-lookup"><span data-stu-id="130a0-125">**Churn (last 30 days)**: Customers without any “active", “in grace" or “disabled" subscriptions</span></span>

- <span data-ttu-id="130a0-126">**Novo (últimas 24 horas)** : Novos clientes comprando pelo menos uma assinatura nos últimas 24 horas</span><span class="sxs-lookup"><span data-stu-id="130a0-126">**New (last 24 hours)**: New customers purchasing at least one subscription in last 24 hours</span></span>

- <span data-ttu-id="130a0-127">**Custo mensal estimado nos últimos 12 meses**: Tendência mês a mês do valor pré-taxado em dólar estimado para a fatura agregado mensalmente durante o período dos últimos 12 meses</span><span class="sxs-lookup"><span data-stu-id="130a0-127">**Estimated monthly cost over last 12 months**: Month over month trend of estimated pre-tax invoice dollar amount aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="130a0-128">**Custo mensal por produto estimado nos últimos 12 meses**: Produtos vendidos classificados pelo valor pré-taxado em dólar estimado para a fatura agregado mensalmente durante o período dos últimos 12 meses.</span><span class="sxs-lookup"><span data-stu-id="130a0-128">**Estimated cost by product over last 12 months**: Products sold sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="130a0-129">Isso indicará os principais produtos que contribuem para a maior parte da receita.</span><span class="sxs-lookup"><span data-stu-id="130a0-129">This will indicate top products bringing most revenue.</span></span>

- <span data-ttu-id="130a0-130">**Clientes nos últimos 12 meses**: Tendência mês a mês de novos clientes e clientes de variação agregados mensalmente durante o período de últimos 12 meses</span><span class="sxs-lookup"><span data-stu-id="130a0-130">**Customers over last 12 months**: Month over month trend of new customers and churn customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="130a0-131">**Custo mensal por cliente estimado nos últimos 12 meses**: Clientes classificados pelo valor pré-taxado em dólar estimado para a fatura agregado mensalmente durante o período dos últimos 12 meses.</span><span class="sxs-lookup"><span data-stu-id="130a0-131">**Estimated cost by customer over last 12 months**: Customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="130a0-132">Isso indicará os principais clientes que contribuem para a maior parte da receita.</span><span class="sxs-lookup"><span data-stu-id="130a0-132">This will indicate top customers bringing most revenue.</span></span>

- <span data-ttu-id="130a0-133">**Contagem de cliente por produto**: Produtos vendidos classificados por clientes associados.</span><span class="sxs-lookup"><span data-stu-id="130a0-133">**Customer count by product**: Products sold sorted by associated customers.</span></span> <span data-ttu-id="130a0-134">Isso indicará principais produtos vendidos para a maioria dos clientes.</span><span class="sxs-lookup"><span data-stu-id="130a0-134">This will indicate top products sold to most customers.</span></span> 


### <a name="subscription-insights-report"></a><span data-ttu-id="130a0-135">Relatório de ideias de assinatura</span><span class="sxs-lookup"><span data-stu-id="130a0-135">Subscription Insights report</span></span> 

- <span data-ttu-id="130a0-136">**Status da assinatura**:</span><span class="sxs-lookup"><span data-stu-id="130a0-136">**Subscription status**:</span></span>

    - <span data-ttu-id="130a0-137">Ativo: assinaturas pertencentes ao estado "ativo" ou "em carência"</span><span class="sxs-lookup"><span data-stu-id="130a0-137">Active: Subscriptions belonging to either “active" or “in grace" state</span></span>

    - <span data-ttu-id="130a0-138">Suspenso: assinaturas que pertencem ao estado "desabilitado"</span><span class="sxs-lookup"><span data-stu-id="130a0-138">Suspended: Subscriptions belonging to “disabled" state</span></span>

    - <span data-ttu-id="130a0-139">Desprovisionado: assinaturas que pertencem ao status "desprovisionado" ou "expirado"</span><span class="sxs-lookup"><span data-stu-id="130a0-139">De-provisioned: Subscriptions belonging to “de-provisioned" or “expired" status</span></span>

- <span data-ttu-id="130a0-140">**Status de expiração**:</span><span class="sxs-lookup"><span data-stu-id="130a0-140">**Expiry status**:</span></span>

    - <span data-ttu-id="130a0-141">Expirado: Assinaturas que já expiraram (onde a data de término da assinatura está no passado)</span><span class="sxs-lookup"><span data-stu-id="130a0-141">Expired: Subscriptions that have already expired (where subscription end date is in past)</span></span>

    - <span data-ttu-id="130a0-142">Expiram após 30 dias: Assinaturas que expirarão após 30 dias (onde data de término da assinatura é depois dos próximos 30 dias)</span><span class="sxs-lookup"><span data-stu-id="130a0-142">Expiring after 30 days: Subscriptions that will expire after 30 days (where subscription end date is after next 30 days)</span></span>

    - <span data-ttu-id="130a0-143">Expiram em 30 dias: Assinaturas que expirarão nos próximos 30 dias (onde data de término da assinatura é entre hoje e os próximos 30 dias)</span><span class="sxs-lookup"><span data-stu-id="130a0-143">Expiring in 30 days: Subscriptions that will expire within next 30 days (where subscription end date is between today and next 30 days)</span></span>

-  <span data-ttu-id="130a0-144">**Total de assinaturas**: assinaturas no status "ativo", "em carência" ou "desabilitado"</span><span class="sxs-lookup"><span data-stu-id="130a0-144">**Total subscriptions**: Subscriptions in “active," “in grace" or “disabled" status</span></span>

- <span data-ttu-id="130a0-145">**Novo (últimos 30 dias)** : Novas assinaturas compradas por clientes nos últimos 30 dias</span><span class="sxs-lookup"><span data-stu-id="130a0-145">**New (last 30 days)**: New subscriptions purchased by customers within last 30 days</span></span>

- <span data-ttu-id="130a0-146">**Novo (últimas 24 horas)** : Novas assinaturas compradas por clientes nas últimas 24 horas</span><span class="sxs-lookup"><span data-stu-id="130a0-146">**New (last 24 hours)**: New subscriptions purchased by customers within last 24 hours</span></span>

- <span data-ttu-id="130a0-147">**Expira em 30 dias**: Assinaturas que expirarão nos próximos 30 dias</span><span class="sxs-lookup"><span data-stu-id="130a0-147">**Expiring in 30 days**: Subscriptions that will expire within next 30 days</span></span>

- <span data-ttu-id="130a0-148">**Rotatividade (últimos 30 dias)** : Assinaturas que tiveram o provisionamento cancelado ou que foram suspensas (desabilitadas) nos últimos 30 dias</span><span class="sxs-lookup"><span data-stu-id="130a0-148">**Churn (last 30 days)**: Subscriptions that have been de-provisioned or Suspended (disabled) within last 30 days</span></span>

- <span data-ttu-id="130a0-149">**Distribuição por tipos de assinatura**: % distribuição do total de assinaturas por licença com base e o uso com base no tipo de assinatura</span><span class="sxs-lookup"><span data-stu-id="130a0-149">**Distribution by subscription types**: % distribution of total subscriptions by License based and usage based subscription type</span></span>

- <span data-ttu-id="130a0-150">**Contagem de assinatura ativa por produto**: Produtos vendidos classificados por contagem de assinaturas ativas</span><span class="sxs-lookup"><span data-stu-id="130a0-150">**Active subscription count by product**: Products sold sorted by active subscriptions count</span></span>

- <span data-ttu-id="130a0-151">**Assinaturas nos últimos 12 meses**: Tendência mês a mês de novas assinaturas e assinaturas com rotatividade agregadas mensalmente durante o período de últimos 12 meses</span><span class="sxs-lookup"><span data-stu-id="130a0-151">**Subscriptions over last 12 months**: Month over month trend of new subscriptions and churn subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="130a0-152">**Detalhes de assinatura do cliente**: Visualização detalhada dos clientes, assinaturas e ofertas</span><span class="sxs-lookup"><span data-stu-id="130a0-152">**Customer subscription details**: Detailed view of the customers, subscriptions and offers</span></span> 


### <a name="license-insights-report"></a><span data-ttu-id="130a0-153">Relatório de ideias de licença:</span><span class="sxs-lookup"><span data-stu-id="130a0-153">License Insights report:</span></span>

- <span data-ttu-id="130a0-154">**Total de licenças**: Número total de licenças agregadas em todas as assinaturas com base na licença</span><span class="sxs-lookup"><span data-stu-id="130a0-154">**Total licenses**: Total number of licenses aggregated across all license based subscriptions</span></span>

- <span data-ttu-id="130a0-155">**Novo (últimos 30 dias)** : Adição de licenças nos últimos 30 dias</span><span class="sxs-lookup"><span data-stu-id="130a0-155">**New (last 30 days)**: License addition within last 30 days</span></span>

- <span data-ttu-id="130a0-156">**Rotatividade (últimos 30 dias)** : Redução de licenças nos últimos 30 dias</span><span class="sxs-lookup"><span data-stu-id="130a0-156">**Churn (last 30 days)**: License reduction within last 30 days</span></span>

- <span data-ttu-id="130a0-157">**Novo (últimas 24 horas)** : Adição de licenças nas últimas 24 horas</span><span class="sxs-lookup"><span data-stu-id="130a0-157">**New (last 24 hours)**: License addition within last 24 hours</span></span>

- <span data-ttu-id="130a0-158">**Licenças nos últimos 90 dias**: Tendência mês a mês de adições e reduções de licença agregadas mensalmente durante o período dos últimos 90 dias</span><span class="sxs-lookup"><span data-stu-id="130a0-158">**Licenses over last 90 days**: Month over month trend of license additions and reductions aggregated monthly over the period of last 90 days</span></span>

- <span data-ttu-id="130a0-159">**Contagem de licença ativa por produto**: Produtos vendidos classificados por contagem de licenças ativas</span><span class="sxs-lookup"><span data-stu-id="130a0-159">**Active license count by product**: Products sold sorted by active license count</span></span>

- <span data-ttu-id="130a0-160">**Contagem de licença ativa por cliente**: Clientes classificados por contagem de licenças ativas</span><span class="sxs-lookup"><span data-stu-id="130a0-160">**Active license count by customer**: Customers sorted by sorted by active license count</span></span>

- <span data-ttu-id="130a0-161">**Detalhes do evento de licença de cliente nos últimos 90 dias**: Visualização detalhada de clientes, assinaturas e eventos de assinatura, incluindo eventos data, nome do evento, quantidade e alteração na quantidade.</span><span class="sxs-lookup"><span data-stu-id="130a0-161">**Customer license event details over last 90 days**: Detailed view of the customers, subscriptions and subscription events including event date, event name, quantity and change in quantity.</span></span>


### <a name="licenses-usage-report"></a><span data-ttu-id="130a0-162">Relatório de uso de licenças:</span><span class="sxs-lookup"><span data-stu-id="130a0-162">Licenses Usage report:</span></span>

- <span data-ttu-id="130a0-163">**Licenças atribuídas por produto**: Produtos vendidos classificados por contagem de atribuição</span><span class="sxs-lookup"><span data-stu-id="130a0-163">**Licenses assigned by product**: Products sold sorted by license assignment count</span></span>

- <span data-ttu-id="130a0-164">**Licenças em uso por produto**: Produtos vendidos classificados por contagem de uso de licença</span><span class="sxs-lookup"><span data-stu-id="130a0-164">**Licenses in use by product**: Products sold sorted by license usage count</span></span>

- <span data-ttu-id="130a0-165">**Distribuição de cliente de licenças atribuídas**: distribuição % do total de clientes desfeitos em classificações de faixas de 20% por % de atribuição de licença</span><span class="sxs-lookup"><span data-stu-id="130a0-165">**Customer distribution of licenses assigned**: % distribution of total customers broken in buckets of 20% range by license assignment %</span></span>

- <span data-ttu-id="130a0-166">**Distribuição de cliente de licenças em uso**: distribuição % do total de clientes desfeitos em classificações de faixas de 20% por % de uso de licença</span><span class="sxs-lookup"><span data-stu-id="130a0-166">**Customer distribution of licenses in use**: % distribution of total customers broken in buckets of 20% range by license usage %</span></span>

- <span data-ttu-id="130a0-167">**Licenças atribuídas pelo cliente**: Visualização detalhada de licenças vendidas e licenças atribuídas por cliente e produto</span><span class="sxs-lookup"><span data-stu-id="130a0-167">**Licenses assigned by customer**: Detailed view of licenses sold and licenses assigned by customers and products</span></span>

- <span data-ttu-id="130a0-168">**Licenças em uso por cliente**: Visualização detalhada de licenças em uso por cliente e produto</span><span class="sxs-lookup"><span data-stu-id="130a0-168">**Licenses in use by customer**: Detailed view of licenses sold and licenses in use by customers and products</span></span>


### <a name="azure-insights-report"></a><span data-ttu-id="130a0-169">Relatório de ideias do Azure:</span><span class="sxs-lookup"><span data-stu-id="130a0-169">Azure Insights report:</span></span>

- <span data-ttu-id="130a0-170">**Clientes baseado no uso nos últimos 12 meses**: Tendência mês a mês de novos clientes e clientes com rotatividade baseados no uso agregados mensalmente durante o período de últimos 12 meses</span><span class="sxs-lookup"><span data-stu-id="130a0-170">**Usage based customers over last 12 months**: Month over month trend of new usage based customers and churned usage based customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="130a0-171">**Assinaturas baseado no uso nos últimos 12 meses**: Tendência mês a mês de novas assinaturas e assinaturas com rotatividade baseados no uso agregados mensalmente durante o período de últimos 12 meses</span><span class="sxs-lookup"><span data-stu-id="130a0-171">**Usage based subscriptions over last 12 months**: Month over month trend of new usage based subscriptions and churned usage based subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="130a0-172">**Custo mensal de uso por cliente estimado nos últimos 60 dias**: Clientes com base no uso classificados pelo valor pré-taxado em dólar estimado para a fatura agregado mensalmente durante o período dos últimos 60 dias.</span><span class="sxs-lookup"><span data-stu-id="130a0-172">**Estimated cost of usage by customer over last 60 days**: Usage based customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span> <span data-ttu-id="130a0-173">Isso indicará os principais clientes com base no uso que contribuem para a maior parte da receita.</span><span class="sxs-lookup"><span data-stu-id="130a0-173">This will indicate top usage based customers bringing most revenue</span></span>

- <span data-ttu-id="130a0-174">**Custo mensal de uso por categoria estimado nos últimos 60 dias**: Categorias de medição com base no uso de assinaturas classificadas pelo valor pré-taxado em dólar estimado para a fatura agregado mensalmente durante o período dos últimos 60 dias.</span><span class="sxs-lookup"><span data-stu-id="130a0-174">**Estimated cost of usage by category over last 60 days**: Meter categories of usage based subscriptions sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="130a0-175">**Custo mensal de uso por assinatura estimado nos últimos 60 dias**: Assinaturas com base no uso classificados pelo valor pré-taxado em dólar estimado para a fatura agregado mensalmente durante o período dos últimos 60 dias.</span><span class="sxs-lookup"><span data-stu-id="130a0-175">**Estimated cost of usage by subscription over last 60 days**: Usage based subscriptions by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="130a0-176">**Custos estimados de uso de cliente por orçamento de gastos**: Clientes classificados por percentual de seu orçamento de gastos com uso atual excedendo o limite (100%).</span><span class="sxs-lookup"><span data-stu-id="130a0-176">**Customer estimated usage cost by spending budget**: Customers sorted by percentage of their current usage spending budget exceeding threshold (100%).</span></span>


### <a name="azure-resource-usage-report"></a><span data-ttu-id="130a0-177">Relatório de uso de recurso Azure:</span><span class="sxs-lookup"><span data-stu-id="130a0-177">Azure Resource Usage report:</span></span>

- <span data-ttu-id="130a0-178">**Uso de recursos Azure por dia nos período selecionado**: Unidades de consumo diárias para cada recurso medido em cada uso baseado na assinatura para o período selecionado nos últimos 60 dias.</span><span class="sxs-lookup"><span data-stu-id="130a0-178">**Usage of Azure resources by day for selected period**: Daily consumption units for each metered resource in each usage based subscription for selected period within the last 60 days.</span></span>

- <span data-ttu-id="130a0-179">**Custo estimado de uso de recursos Azure no período selecionado**: Custo estimado baseado na última tabela de taxa para cada recurso medido baseado na assinatura para o período selecionado dos últimos 60 dias.</span><span class="sxs-lookup"><span data-stu-id="130a0-179">**Estimated usage cost of Azure resources for selected period**: Estimated cost based on latest rate card for each metered resource in each usage based subscription for selected period within the last 60 days.</span></span> 

## <a name="see-also"></a><span data-ttu-id="130a0-180">Consulte também</span><span class="sxs-lookup"><span data-stu-id="130a0-180">See also</span></span>

[<span data-ttu-id="130a0-181">Visão geral do aplicativo Partner Center Analytics for Power BI app</span><span class="sxs-lookup"><span data-stu-id="130a0-181">Partner Center Analytics for Power BI app overview</span></span>](power-bi-app-for-direct-partners.md)


[<span data-ttu-id="130a0-182">Instalar e visualizar o aplicativo Análise do Partner Center para Microsoft Power BI</span><span class="sxs-lookup"><span data-stu-id="130a0-182">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-install.md)
