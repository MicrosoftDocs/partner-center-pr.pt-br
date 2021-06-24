---
title: Usar Partner Center Analytics para Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como exibir seus dados empresariais usando o aplicativo Análise do Partner Center para Power BI (para parceiros diretos no programa Provedor de Soluções na Nuvem (CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 95eb018a3284d2de98c0ce6a9cd0ce6299d5571a
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "112564974"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="060b2-103">Visualize seus dados de negócio com o aplicativo de análise do Partner Center para Microsoft Power BI</span><span class="sxs-lookup"><span data-stu-id="060b2-103">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>



<span data-ttu-id="060b2-104">**Funções apropriadas**: Administrador global | Administrador de gerenciamento de usuários | Agente de vendas | Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="060b2-104">**Appropriate roles**: Global admin | User management admin | Sales agent | Admin agent</span></span>

## <a name="view-your-business-data"></a><span data-ttu-id="060b2-105">Visualize seus dados de negócio</span><span class="sxs-lookup"><span data-stu-id="060b2-105">View your business data</span></span>

<span data-ttu-id="060b2-106">Obter uma representação visual dos dados de negócios com o aplicativo Partner Center Analytics para Microsoft Power BI, incluindo:</span><span class="sxs-lookup"><span data-stu-id="060b2-106">Get a visual representation of your business data with the Partner Center Analytics app for Microsoft Power BI, including:</span></span>

- <span data-ttu-id="060b2-107">Crescimento de sua base de clientes, assinaturas e licenças</span><span class="sxs-lookup"><span data-stu-id="060b2-107">Growth of your customer base, subscriptions, and licenses</span></span>

- <span data-ttu-id="060b2-108">O uso de produtos do Office 365, Microsoft Dynamics e Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="060b2-108">Usage of Office 365, Microsoft Dynamics, and Microsoft Azure products</span></span>

- <span data-ttu-id="060b2-109">As unidades de consumo diário de cada recurso limitado em cada assinatura do Azure nos últimos 60 dias</span><span class="sxs-lookup"><span data-stu-id="060b2-109">Daily consumption units for each metered resource in each Azure subscription for the last 60 days</span></span>

- <span data-ttu-id="060b2-110">Custo estimado (com base na tabela de tarifas mais recente)</span><span class="sxs-lookup"><span data-stu-id="060b2-110">Estimated cost (based on latest rate card)</span></span>

- <span data-ttu-id="060b2-111">Capacidade de exportar conjuntos de dados e criar relatórios personalizados, incluindo por cliente.</span><span class="sxs-lookup"><span data-stu-id="060b2-111">Ability to export datasets and create custom reports, including per customer.</span></span>

### <a name="about-the-partner-center-analytics-app-preview-release"></a><span data-ttu-id="060b2-112">Sobre a versão de visualização do aplicativo de análises do Partner Center</span><span class="sxs-lookup"><span data-stu-id="060b2-112">About the Partner Center Analytics app preview release</span></span>

- <span data-ttu-id="060b2-113">Este aplicativo é destinado somente a parceiros diretos no programa Provedor de Soluções na Nuvem (CSP).</span><span class="sxs-lookup"><span data-stu-id="060b2-113">This app is for direct partners in the Cloud Solution Provider (CSP) program only.</span></span> <span data-ttu-id="060b2-114">Outros parceiros no CSP (revendedores indiretos, por exemplo) não poderão se conectar.</span><span class="sxs-lookup"><span data-stu-id="060b2-114">Other partners in CSP (indirect resellers, for example) will not be able to sign in.</span></span>

- <span data-ttu-id="060b2-115">Todos os custos estimados são pré-taxados na cobrança/ dados da fatura, e não são vinculados legalmente.</span><span class="sxs-lookup"><span data-stu-id="060b2-115">Any estimated costs are pre-tax billing / invoice data, and are not legally binding.</span></span> <span data-ttu-id="060b2-116">Os Custos estimados destinam-se a ser usados somente para percepções.</span><span class="sxs-lookup"><span data-stu-id="060b2-116">Estimated costs are meant to be used for data insights only.</span></span>

- <span data-ttu-id="060b2-117">As informações do cliente são baseadas em assinaturas.</span><span class="sxs-lookup"><span data-stu-id="060b2-117">Customer information is based on subscriptions.</span></span> <span data-ttu-id="060b2-118">Todos os clientes para os que você criou contas recentemente, mas que ainda não têm assinaturas, não estão incluídos em contagens.</span><span class="sxs-lookup"><span data-stu-id="060b2-118">Any customers that you've recently created accounts for, but who don't yet have subscriptions, aren't included in counts.</span></span>

- <span data-ttu-id="060b2-119">Os custos estimados baseiam-se na tabela de taxa mais recente, que baseia-se nos preços CSP.</span><span class="sxs-lookup"><span data-stu-id="060b2-119">Estimated cost is based on latest rate card, which is based on CSP pricing.</span></span>

- <span data-ttu-id="060b2-120">Os dias são dias calendários.</span><span class="sxs-lookup"><span data-stu-id="060b2-120">Days are calendar days.</span></span>

### <a name="business-insights-report"></a><span data-ttu-id="060b2-121">Relatório de ideias de negócios</span><span class="sxs-lookup"><span data-stu-id="060b2-121">Business Insights report</span></span>

- <span data-ttu-id="060b2-122">**Locatários do** cliente: número de locatários Azure Active Directory (Azure AD) distintos de clientes que compraram assinaturas</span><span class="sxs-lookup"><span data-stu-id="060b2-122">**Customer tenants**: Number of distinct Azure Active Directory (Azure AD) tenants of customers that have purchased subscriptions</span></span>

- <span data-ttu-id="060b2-123">**Novo (últimos 30 dias)**: Novos clientes comprando pelo menos uma assinatura nos últimos 30 dias</span><span class="sxs-lookup"><span data-stu-id="060b2-123">**New (last 30 days)**: New customers purchasing at least one subscription in last 30 days</span></span>

- <span data-ttu-id="060b2-124">**Variação (últimos 30 dias)**: clientes sem assinaturas "ativas", "em carência" ou "desabilitadas"</span><span class="sxs-lookup"><span data-stu-id="060b2-124">**Churn (last 30 days)**: Customers without any “active", “in grace" or “disabled" subscriptions</span></span>

- <span data-ttu-id="060b2-125">**Novo (últimas 24 horas)**: Novos clientes comprando pelo menos uma assinatura nos últimas 24 horas</span><span class="sxs-lookup"><span data-stu-id="060b2-125">**New (last 24 hours)**: New customers purchasing at least one subscription in last 24 hours</span></span>

- <span data-ttu-id="060b2-126">**Custo mensal estimado nos últimos 12 meses**: Tendência mês a mês do valor pré-taxado em dólar estimado para a fatura agregado mensalmente durante o período dos últimos 12 meses</span><span class="sxs-lookup"><span data-stu-id="060b2-126">**Estimated monthly cost over last 12 months**: Month over month trend of estimated pre-tax invoice dollar amount aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="060b2-127">**Custo mensal por produto estimado nos últimos 12 meses**: Produtos vendidos classificados pelo valor pré-taxado em dólar estimado para a fatura agregado mensalmente durante o período dos últimos 12 meses.</span><span class="sxs-lookup"><span data-stu-id="060b2-127">**Estimated cost by product over last 12 months**: Products sold sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="060b2-128">Esse status indica os principais produtos que trazem a maior parte da receita.</span><span class="sxs-lookup"><span data-stu-id="060b2-128">This status indicates top products bringing most revenue.</span></span>

- <span data-ttu-id="060b2-129">**Clientes nos últimos 12 meses**: Tendência mês a mês de novos clientes e clientes de variação agregados mensalmente durante o período de últimos 12 meses</span><span class="sxs-lookup"><span data-stu-id="060b2-129">**Customers over last 12 months**: Month over month trend of new customers and churn customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="060b2-130">**Custo mensal por cliente estimado nos últimos 12 meses**: Clientes classificados pelo valor pré-taxado em dólar estimado para a fatura agregado mensalmente durante o período dos últimos 12 meses.</span><span class="sxs-lookup"><span data-stu-id="060b2-130">**Estimated cost by customer over last 12 months**: Customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="060b2-131">Esse status indica os principais clientes que trazem a maior parte da receita.</span><span class="sxs-lookup"><span data-stu-id="060b2-131">This status indicates top customers bringing most revenue.</span></span>

- <span data-ttu-id="060b2-132">**Contagem de cliente por produto**: Produtos vendidos classificados por clientes associados.</span><span class="sxs-lookup"><span data-stu-id="060b2-132">**Customer count by product**: Products sold sorted by associated customers.</span></span> <span data-ttu-id="060b2-133">Esse status indica os principais produtos vendidos para a maioria dos clientes.</span><span class="sxs-lookup"><span data-stu-id="060b2-133">This status indicates top products sold to most customers.</span></span>

### <a name="subscription-insights-report"></a><span data-ttu-id="060b2-134">Relatório de ideias de assinatura</span><span class="sxs-lookup"><span data-stu-id="060b2-134">Subscription Insights report</span></span>

- <span data-ttu-id="060b2-135">**Status da assinatura:**</span><span class="sxs-lookup"><span data-stu-id="060b2-135">**Subscription status**:</span></span>

- <span data-ttu-id="060b2-136">Ativo: assinaturas que pertencem ao estado "ativo" ou "em carência"</span><span class="sxs-lookup"><span data-stu-id="060b2-136">Active: Subscriptions belonging to either “active" or “in grace" state</span></span>

  - <span data-ttu-id="060b2-137">Suspenso: assinaturas que pertencem ao estado "desabilitado"</span><span class="sxs-lookup"><span data-stu-id="060b2-137">Suspended: Subscriptions belonging to “disabled" state</span></span>

  - <span data-ttu-id="060b2-138">Des provisionado: assinaturas que pertencem ao status "des provisionado" ou "expirado"</span><span class="sxs-lookup"><span data-stu-id="060b2-138">De-provisioned: Subscriptions belonging to “de-provisioned" or “expired" status</span></span>

- <span data-ttu-id="060b2-139">**Status de expiração**:</span><span class="sxs-lookup"><span data-stu-id="060b2-139">**Expiry status**:</span></span>

  - <span data-ttu-id="060b2-140">Expirado: Assinaturas que já expiraram (onde a data de término da assinatura está no passado)</span><span class="sxs-lookup"><span data-stu-id="060b2-140">Expired: Subscriptions that have already expired (where subscription end date is in past)</span></span>

  - <span data-ttu-id="060b2-141">Expiram após 30 dias: Assinaturas que expirarão após 30 dias (onde data de término da assinatura é depois dos próximos 30 dias)</span><span class="sxs-lookup"><span data-stu-id="060b2-141">Expiring after 30 days: Subscriptions that will expire after 30 days (where subscription end date is after next 30 days)</span></span>

  - <span data-ttu-id="060b2-142">Expiram em 30 dias: Assinaturas que expirarão nos próximos 30 dias (onde data de término da assinatura é entre hoje e os próximos 30 dias)</span><span class="sxs-lookup"><span data-stu-id="060b2-142">Expiring in 30 days: Subscriptions that will expire within next 30 days (where subscription end date is between today and next 30 days)</span></span>

- <span data-ttu-id="060b2-143">**Total de assinaturas:** assinaturas no status "ativo", "em carência" ou "desabilitado"</span><span class="sxs-lookup"><span data-stu-id="060b2-143">**Total subscriptions**: Subscriptions in “active," “in grace" or “disabled" status</span></span>

- <span data-ttu-id="060b2-144">**Novo (últimos 30 dias)**: Novas assinaturas compradas por clientes nos últimos 30 dias</span><span class="sxs-lookup"><span data-stu-id="060b2-144">**New (last 30 days)**: New subscriptions purchased by customers within last 30 days</span></span>

- <span data-ttu-id="060b2-145">**Novo (últimas 24 horas)**: Novas assinaturas compradas por clientes nas últimas 24 horas</span><span class="sxs-lookup"><span data-stu-id="060b2-145">**New (last 24 hours)**: New subscriptions purchased by customers within last 24 hours</span></span>

- <span data-ttu-id="060b2-146">**Expira em 30 dias**: Assinaturas que expirarão nos próximos 30 dias</span><span class="sxs-lookup"><span data-stu-id="060b2-146">**Expiring in 30 days**: Subscriptions that will expire within next 30 days</span></span>

- <span data-ttu-id="060b2-147">**Variação (últimos 30 dias)**: assinaturas que foram des provisionadas ou suspensas (desabilitadas) nos últimos 30 dias</span><span class="sxs-lookup"><span data-stu-id="060b2-147">**Churn (last 30 days)**: Subscriptions that have been de-provisioned or suspended (disabled) within last 30 days</span></span>

- <span data-ttu-id="060b2-148">**Distribuição por tipos de assinatura:**% de distribuição do total de assinaturas por tipo de assinatura baseado em licença e com base no uso</span><span class="sxs-lookup"><span data-stu-id="060b2-148">**Distribution by subscription types**: % distribution of total subscriptions by License based and usage-based subscription type</span></span>

- <span data-ttu-id="060b2-149">**Contagem de assinatura ativa por produto**: Produtos vendidos classificados por contagem de assinaturas ativas</span><span class="sxs-lookup"><span data-stu-id="060b2-149">**Active subscription count by product**: Products sold sorted by active subscriptions count</span></span>

- <span data-ttu-id="060b2-150">**Assinaturas nos últimos 12 meses**: Tendência mês a mês de novas assinaturas e assinaturas com rotatividade agregadas mensalmente durante o período de últimos 12 meses</span><span class="sxs-lookup"><span data-stu-id="060b2-150">**Subscriptions over last 12 months**: Month over month trend of new subscriptions and churn subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="060b2-151">**Detalhes da assinatura do** cliente: exibição detalhada dos clientes, assinaturas e ofertas</span><span class="sxs-lookup"><span data-stu-id="060b2-151">**Customer subscription details**: Detailed view of the customers, subscriptions, and offers</span></span>

### <a name="license-insights-report"></a><span data-ttu-id="060b2-152">Relatório de ideias de licença:</span><span class="sxs-lookup"><span data-stu-id="060b2-152">License Insights report:</span></span>

- <span data-ttu-id="060b2-153">**Total de licenças:** número total de licenças agregadas em todas as assinaturas baseadas em licença</span><span class="sxs-lookup"><span data-stu-id="060b2-153">**Total licenses**: Total number of licenses aggregated across all license-based subscriptions</span></span>

- <span data-ttu-id="060b2-154">**Novo (últimos 30 dias)**: Adição de licenças nos últimos 30 dias</span><span class="sxs-lookup"><span data-stu-id="060b2-154">**New (last 30 days)**: License addition within last 30 days</span></span>

- <span data-ttu-id="060b2-155">**Rotatividade (últimos 30 dias)**: Redução de licenças nos últimos 30 dias</span><span class="sxs-lookup"><span data-stu-id="060b2-155">**Churn (last 30 days)**: License reduction within last 30 days</span></span>

- <span data-ttu-id="060b2-156">**Novo (últimas 24 horas)**: Adição de licenças nas últimas 24 horas</span><span class="sxs-lookup"><span data-stu-id="060b2-156">**New (last 24 hours)**: License addition within last 24 hours</span></span>

- <span data-ttu-id="060b2-157">**Licenças nos últimos 90 dias**: Tendência mês a mês de adições e reduções de licença agregadas mensalmente durante o período dos últimos 90 dias</span><span class="sxs-lookup"><span data-stu-id="060b2-157">**Licenses over last 90 days**: Month over month trend of license additions and reductions aggregated monthly over the period of last 90 days</span></span>

- <span data-ttu-id="060b2-158">**Contagem de licença ativa por produto**: Produtos vendidos classificados por contagem de licenças ativas</span><span class="sxs-lookup"><span data-stu-id="060b2-158">**Active license count by product**: Products sold sorted by active license count</span></span>

- <span data-ttu-id="060b2-159">**Contagem de licenças ativas por cliente:** clientes classificaram por contagem de licenças ativas</span><span class="sxs-lookup"><span data-stu-id="060b2-159">**Active license count by customer**: Customers sorted by active license count</span></span>

- <span data-ttu-id="060b2-160">Detalhes do evento de licença do cliente nos últimos **90** dias: exibição detalhada dos clientes, assinaturas e eventos de assinatura, incluindo data do evento, nome do evento, quantidade e alteração na quantidade.</span><span class="sxs-lookup"><span data-stu-id="060b2-160">**Customer license event details over last 90 days**: Detailed view of the customers, subscriptions, and subscription events including event date, event name, quantity, and change in quantity.</span></span>

### <a name="licenses-usage-report"></a><span data-ttu-id="060b2-161">Relatório de uso de licenças:</span><span class="sxs-lookup"><span data-stu-id="060b2-161">Licenses Usage report:</span></span>

- <span data-ttu-id="060b2-162">**Licenças atribuídas por produto**: Produtos vendidos classificados por contagem de atribuição</span><span class="sxs-lookup"><span data-stu-id="060b2-162">**Licenses assigned by product**: Products sold sorted by license assignment count</span></span>

- <span data-ttu-id="060b2-163">**Licenças em uso por produto**: Produtos vendidos classificados por contagem de uso de licença</span><span class="sxs-lookup"><span data-stu-id="060b2-163">**Licenses in use by product**: Products sold sorted by license usage count</span></span>

- <span data-ttu-id="060b2-164">**Distribuição de cliente de licenças atribuídas**: distribuição % do total de clientes desfeitos em classificações de faixas de 20% por % de atribuição de licença</span><span class="sxs-lookup"><span data-stu-id="060b2-164">**Customer distribution of licenses assigned**: % distribution of total customers broken in buckets of 20% range by license assignment %</span></span>

- <span data-ttu-id="060b2-165">**Distribuição de cliente de licenças em uso**: distribuição % do total de clientes desfeitos em classificações de faixas de 20% por % de uso de licença</span><span class="sxs-lookup"><span data-stu-id="060b2-165">**Customer distribution of licenses in use**: % distribution of total customers broken in buckets of 20% range by license usage %</span></span>

- <span data-ttu-id="060b2-166">**Licenças atribuídas pelo cliente**: Visualização detalhada de licenças vendidas e licenças atribuídas por cliente e produto</span><span class="sxs-lookup"><span data-stu-id="060b2-166">**Licenses assigned by customer**: Detailed view of licenses sold and licenses assigned by customers and products</span></span>

- <span data-ttu-id="060b2-167">**Licenças em uso por cliente**: Visualização detalhada de licenças em uso por cliente e produto</span><span class="sxs-lookup"><span data-stu-id="060b2-167">**Licenses in use by customer**: Detailed view of licenses sold and licenses in use by customers and products</span></span>

### <a name="azure-insights-report"></a><span data-ttu-id="060b2-168">Relatório de ideias do Azure:</span><span class="sxs-lookup"><span data-stu-id="060b2-168">Azure Insights report:</span></span>

- <span data-ttu-id="060b2-169">Clientes baseados em uso nos últimos **12** meses: tendência mês a mês de novos clientes baseados em uso e clientes baseados em uso rotativos agregados mensalmente ao longo do período dos últimos 12 meses</span><span class="sxs-lookup"><span data-stu-id="060b2-169">**Usage-based customers over last 12 months**: Month over month trend of new usage-based customers and churned usage-based customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="060b2-170">Assinaturas baseadas em uso nos últimos **12** meses: tendência mensal de novas assinaturas baseadas em uso e assinaturas baseadas em uso rotativas agregadas mensalmente durante o período dos últimos 12 meses</span><span class="sxs-lookup"><span data-stu-id="060b2-170">**Usage-based subscriptions over last 12 months**: Month over month trend of new usage-based subscriptions and churned usage-based subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="060b2-171">Custo estimado de uso pelo cliente nos últimos **60** dias: clientes baseados em uso classificaram pelo valor estimado em dinheiro da fatura pré-fiscal agregada ao longo do período dos últimos 60 dias.</span><span class="sxs-lookup"><span data-stu-id="060b2-171">**Estimated cost of usage by customer over last 60 days**: Usage-based customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span> <span data-ttu-id="060b2-172">Esse status indica os principais clientes baseados em uso que trazem a maior parte da receita</span><span class="sxs-lookup"><span data-stu-id="060b2-172">This status indicates top usage-based customers bringing most revenue</span></span>

- <span data-ttu-id="060b2-173">Custo estimado de uso por categoria nos últimos **60** dias: categorias de medidores de assinaturas baseadas em uso, classificação pelo valor estimado em dinheiro da fatura pré-fiscal agregada ao longo do período dos últimos 60 dias.</span><span class="sxs-lookup"><span data-stu-id="060b2-173">**Estimated cost of usage by category over last 60 days**: Meter categories of usage-based subscriptions sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="060b2-174">Custo estimado de uso por assinatura nos últimos **60** dias: assinaturas baseadas em uso pelo valor estimado em dinheiro da fatura pré-fiscal agregada ao longo do período dos últimos 60 dias.</span><span class="sxs-lookup"><span data-stu-id="060b2-174">**Estimated cost of usage by subscription over last 60 days**: Usage-based subscriptions by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="060b2-175">**Custos estimados de uso de cliente por orçamento de gastos**: Clientes classificados por percentual de seu orçamento de gastos com uso atual excedendo o limite (100%).</span><span class="sxs-lookup"><span data-stu-id="060b2-175">**Customer estimated usage cost by spending budget**: Customers sorted by percentage of their current usage spending budget exceeding threshold (100%).</span></span>

### <a name="azure-resource-usage-report"></a><span data-ttu-id="060b2-176">Relatório de uso de recurso Azure:</span><span class="sxs-lookup"><span data-stu-id="060b2-176">Azure Resource Usage report:</span></span>

- <span data-ttu-id="060b2-177">**Uso de recursos do Azure** por dia para o período selecionado: unidades de consumo diário para cada recurso limitado em cada assinatura baseada em uso para o período selecionado nos últimos 60 dias.</span><span class="sxs-lookup"><span data-stu-id="060b2-177">**Usage of Azure resources by day for selected period**: Daily consumption units for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span>

- <span data-ttu-id="060b2-178">Custo de uso estimado dos recursos do **Azure** para o período selecionado: custo estimado com base no cartão de taxa mais recente para cada recurso limitado em cada assinatura baseada em uso para o período selecionado nos últimos 60 dias.</span><span class="sxs-lookup"><span data-stu-id="060b2-178">**Estimated usage cost of Azure resources for selected period**: Estimated cost based on latest rate card for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="060b2-179">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="060b2-179">Next steps</span></span>

- [<span data-ttu-id="060b2-180">Visão geral do aplicativo de análise do Partner Center para Power BI</span><span class="sxs-lookup"><span data-stu-id="060b2-180">Partner Center Analytics for Power BI app overview</span></span>](power-bi-app-for-direct-partners.md)

- [<span data-ttu-id="060b2-181">Instalar e visualizar o aplicativo Análise do Partner Center para Microsoft Power BI</span><span class="sxs-lookup"><span data-stu-id="060b2-181">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-install.md)
