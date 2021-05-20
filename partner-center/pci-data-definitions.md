---
title: Definições de dados do Insights
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: O documento lista vários relatórios e suas definições de dados, que podem ser baixados na página de relatório de download do insights.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 721caed2d8b0e24940e7adedeb90cc689a82d2e7
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152827"
---
# <a name="export--data-definitions"></a>Exportar – definições de dados 

**Funções apropriadas**: Visualizador de relatórios | Visualizador de relatórios executivos

## <a name="introduction"></a>Introdução 

Usando o Hub baixar relatórios no painel do insights, você pode exportar os conjuntos de valores brutos. 

Os vários relatórios, que você pode baixar juntamente com suas definições de dados, estão listados nas seguintes tabelas: 

### <a name="partner-profile-report"></a>**Relatório de perfil do parceiro**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| MPNId | Identificador de Microsoft Partner Network (MPN) | 
| PartnerName | Nome do parceiro | 
| PGA_MPNId | Identificador da conta global do parceiro MPN | 
| PGA_PartnerName | Nome da conta global do parceiro | 
| City | Local da cidade do parceiro | 
| País | Local do país do parceiro | 
| HierarchyLevel | Indica se é uma ID de MPN global ou uma ID de MPN de local | 

### <a name="customer-details-report"></a>**Relatório de detalhes do cliente**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| CustomerName | Nome do cliente que comprou a assinatura | 
| CustomerTenantId | Identificador do locatário do cliente | 
| CustomerTpid | Identificador do pai principal do cliente | 
| CustomerSegment | Segmento de cliente | 
| CustomerMarket | Mercado geográfico do cliente | 
| CustomerStatus | Status do cliente (Ativo ou Inativo) | 
| Produto | O produto vendido ao cliente pelo MPN: O365, DYNAMICS 365, Enterprise Mobility + Security, Power BI ou Microsoft Azure | 
| SKU | SKU do Produto | 
| Month | Mês para o qual o uso e a receita são relatados | 
| MPNId | Identificador de Microsoft Partner Network | 
| PartnerName | Nome do parceiro | 
| PartnerLocation | Localização geográfica do parceiro | 
| PartnerAttributionType | Tipo de atribuição do parceiro | 
| SalesChannel | Canal de vendas | 
| AvailableSeats | Lugares disponíveis | 
| RevenueUSD | Receita em dólares americanos | 

### <a name="reseller-performance-report"></a>**Relatório de desempenho do revendedor**

> [!Note]
> Os dados de receita e ACR estão disponíveis apenas para usuários que são visualizadores de relatórios executivos.

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| ResellerMPNid | Identificador de Microsoft Partner Network do revendedor | 
| ResellerName | Nome do revendedor | 
| ResellerMarket | País do revendedor do mercado | 
| IndirectProviderMPNId | Identificador do Microsoft Partner Network do provedor indireto | 
| IndirectProviderName | Nome do provedor indireto | 
| Month | Mês para o qual o uso e a receita são relatados | 
| Produto | Nome do produto | 
| SubscriptionID | Identificador da assinatura | 
| AvailableSeats | Número de estações disponíveis | 
| AssignedSeats | Número de estações atribuídas | 
| BilledRevenueUSD | Receita cobrada em dólares dos EUA | 
| CustomerName | Nome do cliente que comprou a assinatura | 
| CustomerTPid | Identificador do pai principal do cliente | 
| CustomerSegment | Segmento de cliente | 
| CustomerMarket | Mercado geográfico do cliente | 
| ResellerStatus | Status do revendedor | 

### <a name="subscription-details-report"></a>**Relatório de detalhes da assinatura**

>[!Note]
>Os dados de Receita e ACR estão disponíveis somente para usuários que são visualizadores de relatório executivo.

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| SubscriptionId | GUID da assinatura | 
| SubscriptionStartDate | Data de início da assinatura | 
| SubscriptionEndDate | Data de término da assinatura | 
| SubscriptionState | Estado da assinatura (Ativo ou Rotatividade) | 
| Month | Mês para o qual o uso e a receita são relatados | 
| IsAutoRenew | Indica se a assinatura é autorenew (Sim ou Não) | 
| CustomerName | Nome do cliente que comprou a assinatura | 
| CustomerTenantId | GUID do cliente | 
| CustomerTpid | Identificador pai principal do cliente | 
| CustomerSegment | Segmento de mercado do cliente | 
| CustomerMarket | Mercado geográfico do cliente | 
| Produto | Produto vendido ao cliente pelo parceiro | 
| SKU | SKU do produto | 
| MPNId | ID de Microsoft Partner Network do parceiro | 
| PartnerName | Nome do parceiro | 
| PartnerLocation | Localização geográfica do parceiro | 
| PartnerAttributionType | Tipo de atribuição para a assinatura | 
| SalesChannel | Canal de vendas diretas, CSP (provedor de soluções de nuvem) e assim por diante | 
| AvailableSeats | Estação disponível atual | 
| RevenueUSD | Receita em dólares americanos | 
| ID de registro | ID de registro da assinatura | 

### <a name="azure-usage-report"></a>**Relatório de uso do Azure**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| SubscriptionId | GUID da assinatura | 
| SubscriptionStartDate | A data do início da assinatura | 
| SubscriptionEndDate | A data do final da assinatura | 
| SubscriptionState | Estado atual da assinatura (Aberto, Fechado, Ativo ou Em Período de Carência) | 
| Month | Data agregada por mês | 
| ServiceName | Nome do serviço do Azure | 
| MeterCategory | Nome da categoria do medidor | 
| UsageUnits | O número de unidades que são usadas durante o ciclo de cobrança | 
| CustomerName | Nome do cliente que comprou a assinatura | 
| CustomerTenantId | ID do locatário do cliente | 
| CustomerTpid | ID pai principal do cliente | 
| CustomerSegment | Segmento do cliente | 
| CustomerMarket | Mercado geográfico do cliente | 
| MPNId | Microsoft Partner Network ID do cliente | 
| PartnerName | Nome do parceiro | 
| PartnerLocation | Localização geográfica do país do parceiro | 
| PartnerAttributionType | Tipo de atribuição do parceiro | 
| SalesChannel | Canal das vendas (direto/CSP, indireto/CSP, direto e assim por diante) | 
| ACR_USD | Receita consumida do Azure (ACR) em dólares americanos | 
| ID de registro | ID de registro da assinatura do Azure | 

### <a name="office-365-license-usage-report"></a>**Relatório de uso de licenças do Office 365**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| CustomerTenantId | ID do locatário do cliente | 
| CustomerTpid | ID pai superior do cliente | 
| Carga de trabalho | Skype for Business, Teams, Exchange Online | 
| Month | Mês para o qual o uso é relatado | 
| PaidAvailableUnits | Número de unidades pagas disponíveis | 
| MonthlyActiveUsers | Número de usuários ativos mensais | 
| CustomerName | Nome do cliente que comprou a assinatura | 
| CustomerMarket | Localização geográfica do mercado do cliente | 
| CustomerSegment | Segmento de cliente | 
| MPNId | Identificador de Microsoft Partner Network | 
| PartnerName | Nome do parceiro | 
| PartnerLocation | Localização geográfica do parceiro | 
| PartnerAttributionType | Tipo de atribuição do parceiro | 

### <a name="enterprise-mobility-license-usage-report"></a>**Relatório de uso de licença do Enterprise Mobility**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| CustomerTenantId | ID do locatário do cliente | 
| CustomerTpid | ID pai principal do cliente | 
| WorkloadName | Nome da carga de trabalho Enterprise Mobility + Security (EMS) | 
| Month | Mês para o qual o uso é relatado | 
| PaidAvailableUnits | Número de unidades pagas disponíveis | 
| MonthlyActiveUsers | Número de usuários ativos mensais | 
| CustomerName | Nome do cliente que comprou a assinatura | 
| CustomerMarket | Local do país geográfico do mercado do cliente | 
| CustomerSegment | Segmento de cliente | 
| MPNId | Identificador de Microsoft Partner Network | 
| PartnerName | Nome do parceiro | 
| PartnerLocation | Localização geográfica do parceiro | 
| PartnerAttributionType | Tipo de atribuição do parceiro | 

### <a name="dynamics-365-license-usage-report"></a>**Relatório de uso de licenças do Dynamics 365**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| SubscriptionId | GUID da assinatura | 
| SubscriptionStartDate | Data de início da assinatura | 
| SubscriptionEndDate | Data de término da assinatura | 
| SubscriptionStatus | Estado da assinatura | 
| Month | Mês para o qual o uso é relatado | 
| RevSumDivisionName | Nome da divisão da soma da revisão | 
| RevSumCategoryName | Nome da categoria rev sum | 
| SKU | SKU do produto | 
| SKUId | ID do SKU do produto | 
| FreeVsPaidSKU | Indica se é um SKU gratuito ou pago | 
| SalesModel | Canal de vendas usado para vender a assinatura | 
| DetailedSalesModel | Modelo de vendas detalhado para a assinatura | 
| CustomerName | Nome do cliente que comprou a assinatura | 
| CustomerTenantId | GUID do locatário do cliente | 
| CustomerTpid | Identificador pai principal do cliente | 
| CustomerSegment | Segmento de mercado do cliente | 
| CustomerMarket | Mercado geográfico do cliente | 
| MPNId | Identificador de Microsoft Partner Network | 
| PartnerName | Nome do parceiro | 
| PartnerLocation | Localização geográfica do país do parceiro | 
| PartnerAttachType | Tipo de atribuição para a assinatura | 
| AvailableSeats | Estação disponível atual | 
| AssignedSeats | Estação atribuída atual | 
| ActiveSeats | Estações ativas atuais | 
| DeploymentOpportunity | Oportunidade de implantação atual | 
| ActiveUsagePercent | Percentual de uso ativo atual | 

### <a name="power-bi-license-usage-report"></a>**Relatório de uso de licença Power BI**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| SubscriptionId | GUID da assinatura | 
| SubscriptionStartDate | Data de início da assinatura | 
| SubscriptionEndDate | Data de término da assinatura | 
| SubscriptionStatus | Estado da assinatura (ativo, inativo ou no período de carência) | 
| Month | Data agregada por mês | 
| SKU | SKU do produto | 
| SKUId | ID do SKU do produto | 
| FreeVsPaidSKU | Diferencial de SKU gratuito ou pago | 
| SalesModel | Modelo de vendas usado para vender a assinatura | 
| DetailedSalesModel | Modelo de vendas detalhado para a assinatura | 
| CustomerName | Nome do cliente que comprou a assinatura | 
| CustomerTenantId | GUID do locatário do cliente | 
| CustomerTpid | Identificador do pai principal do cliente | 
| CustomerSegment | Segmento de mercado do cliente | 
| CustomerMarket | Mercado geográfico do cliente | 
| MPNId | Identificador de Microsoft Partner Network | 
| PartnerName | Nome do parceiro | 
| PartnerLocation | Localização geográfica do país do parceiro | 
| PartnerAttachType | Tipo de atribuição para a assinatura | 
| AvailableSeats | Estações disponíveis atuais | 
| AssignedSeats | Estações atribuídas atuais | 
| ActiveSeats | Estações ativas atuais | 
| DeploymentOpportunity | Oportunidade de implantação atual | 
| ActiveUsagePercent | Percentual de uso ativo atual | 

### <a name="teams-meetings-and-calls-report"></a>**Relatório de reuniões e chamadas de equipes**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| CustomerTenantId | ID do locatário do cliente | 
| CustomerTpid | Identificador do pai superior do cliente | 
| Month | Mês para o qual o uso é relatado | 
| Subcarga de trabalho | Subtrabalho para o qual o uso é relatado (reuniões, chamadas ou sistemas de telefone) | 
| Contagem de reunião | Número de reuniões | 
| Duração da reunião | Duração total da reunião em horas | 

### <a name="teams-monthly-usage-report"></a>**Relatório de uso mensal do Teams**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| CustomerTenantId | ID do locatário do cliente | 
| CustomerTpid | Identificador do pai principal do cliente | 
| Month | Mês para o qual o uso é relatado | 
| Subtrabalho | Subtrabalho para o qual o uso é relatado (reuniões, chamadas ou sistemas de telefone) | 
| Usuários da área de trabalho | Número de usuários que usam o Teams na área de trabalho | 
| Usuários Móveis | Número de usuários que usam o Teams em dispositivos móveis | 
| Usuários da Web | Número de usuários que usam o Teams na Web | 
| AllUpParticipants | Número de usuários exclusivos do Teams para o mês | 

### <a name="teams-usage-3p-apps-report"></a>**Relatório de aplicativos 3P de uso do Teams**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| CustomerTenantId | ID do locatário do cliente | 
| CustomerTpid | ID pai superior do cliente | 
| Month | Mês para o qual o uso é relatado | 
| Nome do aplicativo 3P | Nome do aplicativo de equipes | 
| Contagem de usuários | Número de usuários para o aplicativo | 


### <a name="training-details-report"></a>**Relatório detalhes de treinamento**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| TrainingActivityId | Identificador do treinamento | 
| TrainingTitle | Título do treinamento | 
| Traintype | Tipo de treinamento (certificação ou exame) | 
| IndividualFirstName | Nome do cliente | 
| IndividualLastName | Sobrenome do cliente | 
| Email | ID de email pessoal do cliente | 
| CorpEmail | ID de email do office do cliente | 
| TrainingCompletionDate | Data de conclusão do treinamento | 
| Month | Mês para o qual os dados são relatados | 
| IcMCP | Indica se o usuário é um MCP (Microsoft Certified Professional) | 
| MCPID | ID do MCP do usuário | 
| MPNId | Identificador de Microsoft Partner Network | 
| PartnerName | Nome do parceiro | 
| PartnerCityLocation | Localização geográfica da cidade do parceiro | 
| PartnerCountryLocation | Localização geográfica do país do parceiro | 

### <a name="microsoft-learn-report"></a>**Microsoft Learn relatório**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| UserName | Nome do usuário | 
| UserId | GUID do usuário | 
| TrainingName | Nome do treinamento | 
| Traintype | Tipo de treinamento (módulo ou roteiro de aprendizagem) | 
| Produtos | Produto ao qual o módulo de aprendizagem é aplicável | 
| Funções | Funções aplicáveis do treinamento | 
| CompletionDate | Data de conclusão do treinamento | 
| MPNId | Identificador de Microsoft Partner Network | 
| PartnerName | Nome do parceiro | 
| País | Localização geográfica do país do parceiro | 

### <a name="competency-summary-and-history-report"></a>**Relatório de Resumo de competência e histórico**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| Competêncianame | Nome da competência | 
| CompetencyLevel | Nível de competência (ouro ou prata) | 
| CompetencyStatus | Status atual da competência (ativo, inativo ou no período de carência) | 
| CompetencyStartDate | Data de início da competência | 
| CompetencyEndDate | Data de término da competência | 

### <a name="competency-performance-report"></a>**Relatório de desempenho de competência**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| CompetencyName | Nome da competência | 
| CompetencyAttainmentOptionName | Nome da opção de alcance de competência | 
| Month | Mês para o qual as métricas são relatadas | 
| MetricName | Nome da métrica relevante para a competência | 
| MetricMonthlyContribution | Contribuição mensal da métrica | 
| TTMAggregate | Métrica agregada para os 12 meses seguintes | 
| AnniversaryYearAggregate | Métrica agregada para o ano de aniversário atual | 
| GoldThreshold | Requisito de desempenho para atender à competência Gold | 
| SilverThreshold | Requisito de desempenho para atender à competência Silver | 

### <a name="cloud-ascent---microsoft-365-propensity-report"></a>**Cloud Ascent – Microsoft 365 de propensão**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| ID MPN | Microsoft Partner Network ID | 
| Nome do parceiro | Nome do parceiro | 
| ID do Cliente | Número do identificador do cliente | 
| Número de DUNS | O Dun & Bradstreet (D&B) número do cliente que está sendo pontuado quanto à propensão | 
| Nome da Conta | Nome da conta | 
| Domínio | Domínio da conta | 
| Tamanho da organização | Tamanho da organização | 
| Setor | Setor ao qual a organização pertence | 
| Vertical | A vertical do cliente que está sendo pontuada pela propensão, conforme identificado pela Microsoft, D&B e outros padrões do setor | 
| Área | Área geográfica do local | 
| Subsidiária | A subsidiária do cliente que está sendo pontuada quanto à propensão | 
| Território de Vendas | A região de vendas do cliente que está sendo pontuada quanto à propensão | 
| City | Local da cidade geográfica da organização | 
| Estado | Local de estado geográfico da organização | 
| Código postal | Código postal da organização | 
| País | Localização geográfica do país da organização | 
| Segment | Segmento de mercado | 
| Subsegmento | Subsegmento de mercado | 
| Resumo do tipo SMC | Tipo SMC | 
| Top Unmanaged - Compute Base | Principais clientes não planejados – computação | 
| Top Unmanaged – User Base | Principais clientes não planejados – usuário | 
| IsNonProfit | Indica se a organização é sem fins lucrativos (Sim ou Não) | 
| Habilitar Trabalho Remoto – Exchange Online de destino | Clientes que têm uma assinatura ativa do Exchange Online, são vendidos para Microsoft 365 | 
| Habilitar o Trabalho Remoto – aquisição local (versão atual) com propensão do Cloud Ascent – +10 licenças | Cliente que tem um cliente atual do Office ou windows local. Ou seja, a versão do cliente é posterior a uma versão de EOL (fim da vida útil). O cliente tem 10 ou mais licenças. Cliente que tem uma pontuação de propensão. O parceiro deve ter como destino a conversão Microsoft 365. | 
| Habilitar o Trabalho Remoto – aquisição local (versão atual) com propensão do Cloud Ascent – <10 licenças | Cliente que tem um cliente atual do Office ou do Windows (ou seja, uma versão posterior à EOL). O cliente tem menos de 10 licenças. Cliente que tem uma pontuação de propensão. O parceiro deve ter como destino a conversão Microsoft 365. | 
| Habilitar a aquisição remota de trabalho local (versão atual) sem a propensão de elevação da nuvem-+ 10 licenças | Cliente que tem um escritório local ou cliente do Windows atual (ou seja, uma versão posterior à EOL). O cliente tem 10 ou mais licenças. O cliente não tem uma pontuação de propensação. O parceiro deve direcionar a conversão para Microsoft 365. | 
| Habilitar a aquisição remota de trabalho local (versão atual) sem a propensão de elevação de nuvem-<10 licenças | Cliente que tem um escritório local ou cliente do Windows atual (ou seja, uma versão posterior à EOL). O cliente tem menos de 10 licenças. O cliente não tem uma pontuação de propensação. O parceiro deve direcionar a conversão para Microsoft 365. | 
| Habilitar a aquisição remota de trabalho local (versão EOL) com a propensão de elevação da nuvem-+ 10 licenças | Cliente que tem um EOL do escritório local ou cliente do Windows (ou seja, uma versão do EOL ou anterior). O cliente tem 10 ou mais licenças. O cliente tem uma pontuação de propensação. O parceiro deve direcionar a conversão para Microsoft 365. | 
| Habilitar a aquisição remota de trabalho local (versão EOL) com a propensão de elevação de nuvem-<10 licenças | Cliente que tem um EOL do escritório local ou cliente do Windows (ou seja, uma versão do EOL ou anterior). O cliente tem menos de 10 licenças. O cliente tem uma pontuação de propensação. O parceiro deve direcionar a conversão para Microsoft 365. | 
| Habilitar o Trabalho Remoto – aquisição local (versão EOL) sem propensão do Cloud Ascent – +10 licenças | Cliente que tenha um cliente atual do Office ou windows local (ou seja, uma versão EOL ou anterior). O cliente tem 10 ou mais licenças. O cliente não tem uma pontuação de propensão. O parceiro deve ter como destino a conversão Microsoft 365. | 
| Habilitar o Trabalho Remoto – aquisição local (versão EOL) sem propensão do Cloud Ascent – <10 licenças | Cliente que tenha um cliente atual do Office ou windows local (ou seja, uma versão EOL ou anterior). O cliente tem menos de 10 licenças. O cliente não tem uma pontuação de propensão. O parceiro deve ter como destino a conversão Microsoft 365. | 
| Habilitar Trabalho Remoto – perspectiva de alta propensão para Microsoft 365 (Act NowithEvaluate) | Cliente potencial com alta propensão para Microsoft 365 | 
| Habilitar Trabalho Remoto – compete (Zoom) com Microsoft 365 | Cliente com Zoom e Microsoft 365, destino para conversão no Teams | 
| Habilitar Trabalho Remoto – compete (Zoom) sem Microsoft 365 | Cliente com Zoom, destino para conversão no Teams | 
| Reduzir custo e gerenciar – Microsoft 365 E3 direcionado para Microsoft 365 E5 | Cliente existente com Microsoft 365 E3, destino para Microsoft 365 E5 | 
| Reduzir o custo e gerenciar – Microsoft 365 Business Basic e Business Standard direcionados para Microsoft 365 Business Premium | Clientes Microsoft 365 Business Basic e Business Standard existentes, destinados ao Microsoft 365 Business Premium | 
| Transformar a produtividade organizacional – propensação da superfície | O cliente mostra uma propensação para a superfície | 
| M365Cluster | Identifica a propensão de um cliente para comprar Microsoft 365. Direcione o Act agora e avalie os clusters porque eles produzirão um rendimento maior. Direcione o incentivá e instrua os clientes somente se ainda houver capacidade após o Act Now e avaliar os clientes. | 
| M365Fit | Pontos de dados internos e externos que definem firmographics. Ajustar a pontuação usa um modelo de lookalike para nossas melhores empresas de pequeno ou médio porte (SMBs) para comparar os clientes e ver se eles são uma possível adequação para os produtos de nuvem da Microsoft. Ajustar Pontuação é atualizado trimestral. | 
| M365Intent | Os sinais relacionados à mídia social e ao comportamento online de um cliente definem a intenção. A pontuação da intenção é sobreposta em ajustar para definir os clusters. A pontuação da intenção é atualizada mensalmente. | 
| SurfaceCluster | Identifica a propensão de um cliente para comprar a superfície consolidando as recomendações de ajuste e de intenção em um cluster. Direcione o Act agora e avalie os clusters porque eles produzirão um rendimento maior. Direcione o incentivá e instrua os clientes somente se ainda houver capacidade após o Act Now e avaliar os clientes. | 
| SurfaceFit | Pontos de dados internos e externos que definem firmographics. A pontuação de ajuste usa um modelo semelhante aos nossos melhores SMBs para comparar os clientes e ver se eles são uma possível opção para produtos de nuvem da Microsoft. A pontuação de ajuste é atualizada trimestralmente. | 
| SurfaceIntent | Sinais relacionados à mídia social e ao comportamento online de um cliente definem Intenção. A pontuação da intenção é sobreposição em Ajustar para definir os clusters. A pontuação da intenção é atualizada mensalmente. | 
| O365Cluster | Identifica a propensão do cliente para comprar o Office 365. Ação de Destino Agora e Avaliar clusters porque eles produzirão um rendimento mais alto. Direcionar e instruir os clientes somente se ainda houver capacidade depois que Agir agora e Avaliar os clientes são direcionados. | 
| O365Fit | Pontos de dados internos e externos que definem firmográficos. A pontuação de ajuste usa um modelo semelhante aos nossos melhores SMBs para comparar os clientes e ver se eles são uma possível opção para produtos de nuvem da Microsoft. A pontuação de ajuste é atualizada trimestralmente. | 
| O365Intent | Sinais relacionados à mídia social e ao comportamento online de um cliente definem Intenção. A pontuação da intenção é sobreposição em Ajustar para definir os clusters. A pontuação da intenção é atualizada mensalmente. | 
| M365UpsellCustomer | Identifica se o cliente mostra a propensão de venda para Microsoft 365 | 
| Tem o Google | Identifica se o cliente mostra sinais competitivos para a propriedade de produtos do Google | 
| Tem AWS | Identifica se o cliente mostra sinais competitivos para produtos aws (Amazon Web Services) | 
| Tem EA | Identifica se uma renovação é um EA (Contrato Enterprise) ou uma assinatura do EA | 
| Tem Aberto | Identifica se uma renovação é um contrato Open ou Open Value | 

### <a name="cloud-ascent---dynamics-365-propensity-report"></a>**Cloud Ascent – relatório de propensão do Dynamics 365**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| ID MPN | Microsoft Partner Network ID | 
| Nome do parceiro | Nome do parceiro | 
| ID do Cliente | Número do identificador do cliente | 
| Número DE DUNS | O número & Dun do cliente que está sendo pontuado para propensão | 
| Nome da Conta | Nome da conta | 
| Domínio | Domínio da conta | 
| Tamanho da organização | Tamanho da organização | 
| Setor | Setor ao que a organização pertence | 
| Vertical | A vertical do cliente que está sendo pontuado para propensão, conforme identificado pela Microsoft, D&B e outros padrões do setor
| Área | Área geográfica do local | 
| Subsidiária | A subsidiária do cliente que está sendo pontuado para propensão | 
| Território de Vendas | O território de vendas do cliente que está sendo pontuado para propensão | 
| City | Localização geográfica da cidade | 
| Estado | Localização do estado geográfico | 
| Código postal | Cep da organização | 
| País | Localização geográfica do país | 
| Segment | Segmento de mercado | 
| Sub-segmento | Subseção de mercado | 
| Resumo do tipo SMC | A categorização de um cliente: as principais bases de usuários não operacionais são clientes com mais de 300 funcionários, as principais bases de computação nãomanuadas são clientes com US$ 10.000 no potencial de três anos do Azure, empresas médias são clientes com 25 funcionários ou mais e pequenas empresas são clientes com menos de 25 funcionários. | 
| Top Unmanaged - Compute Base | Principais clientes não planejados – computação | 
| Top Unmanaged – User Base | Principais clientes não planejados – usuários | 
| IsNonProfit | Indica se a organização é sem fins lucrativos (Sim ou Não) | 
| Ativar Venda Digital – Microsoft 365 – tamanho do banco >= 25 estações (modelo de propensão SalesPro) | Cliente sem o Dynamics 365. Tamanho do banco: 25 ou mais. O parceiro deve ser destinado à venda cruzada do Dynamics 365 SalesPro. | 
| Ativar a venda digital – propensão do Dynamics 365 SalesPro (Agir agora ou Avaliar) | Clientes de alta propensão sem o Dynamics 365. O parceiro deve ser destinado ao Dynamics 365 SalesPro. | 
| Gerenciando fraudes & risco financeiro – base de instalação local do Dynamics – Navision (modelo de propensão do Business Central) | Cliente existente com Navision local. O parceiro deve ser destinado ao Dynamics 365 Business Central. | 
| Gerenciando fraudes de & de risco financeiro – base de instalação local do Dynamics – Dynamics AX (modelo de propensão do Dynamics 365 Finance + Operations) | Cliente existente com AX local. O parceiro deve ser destinado ao Dynamics 365 Finance + Operations. | 
| Gerenciando a & de risco financeiro – base de instalação local do Dynamics – Great Plains (modelo de propensão do Business Central) | Cliente existente com Great Plains local. O parceiro deve ser destinado ao Dynamics 365 Business Central. | 
| Gerenciando fraudes & de risco financeiro – base de instalação local do Dynamics – Ilhas (modelo de propensão do Business Central) | Cliente existente com o Local Dem. O parceiro deve ser destinado ao Dynamics 365 Business Central. | 
| Gerenciando fraudes & risco financeiro – base de instalação local do Dynamics – Outros (modelo de propensão do Business Central) | Cliente existente com outras soluções locais não listadas anteriormente. O parceiro deve ser destinado ao Dynamics 365 Business Central. | 
| Criar processos empresariais Agile – base de instalação local do Dynamics – AX/GP/SL/NAV/Outros (modelo de propensão do Dynamics 365) | Criar processos empresariais Agile – base de instalação local do Dynamics – AX/GP/SL/NAV/Outros (modelo de propensão do Dynamics 365) | 
| Criar Processos de Negócios Agile – Base de competências do Dynamics – Mendix/OutSystems/Salesforce (modelo de propensão do Dynamics 365) | Criar processos empresariais ágeis – Base de competências do Dynamics – Mendix/OutSystems/Salesforce (modelo de propensão do Dynamics 365) | 
| Criar processos de negócios Agile – base de instalação do Dynamics 365 Finance + Operations | Clientes existentes do Dynamics 365 Finance + Operations. Parceiro para direcionar Power Apps. | 
| Criar processos empresariais Agile – base de instalação do Dynamics 365 Business Central | Clientes existentes do Dynamics 365 Business Central. Parceiro para direcionar Power Apps. | 
| Criar processos empresariais Agile – base de instalação do Dynamics 365 Customer Engagement | Clientes existentes do Dynamics 365 Customer Engagement. Parceiro para direcionar Power Apps. | 
| Criar uma cadeia de fornecimento resiliente – Windows e ativar a primeira carga de trabalho do Dynamics 365 como Gerenciamento de Cadeia de Fornecedores do Dynamics 365 com clientes não Oracle ou SAP ERP (planejamento de recursos corporativos) | Clientes de destino para o Gerenciamento da Cadeia de Fornecedores do Dynamics 365 | 
| Criar uma cadeia de fornecedores resiliente – gerenciamento de cadeia de fornecedores do Dynamics 365 e/ou Varejo ou Comércio para clientes existentes do Dynamics 365 Customer Engagement | Os clientes existentes do Dynamics 365 Customer Engagement são destinados ao Gerenciamento de Cadeia de Fornecedores do Dynamics 365. | 
| Criar uma cadeia de fornecedores resiliente – gerenciamento de cadeia de fornecedores do Dynamics 365 e/ou Varejo ou Comércio para o Dynamics 365 Customer Engagement e Oracle ou SAP | Clientes existentes do Dynamics 365 Customer Engagement com Oracle ou SAP para direcionamento para o Gerenciamento da Cadeia de Fornecedores do Dynamics 365 | 
| D365BCCluster | Identifica a propensão do cliente para comprar o Dynamics 365 Business Central. Os clientes que mostrarem uma propensão para o Business central estarão nas categorias média e pequena. Direcione o Act agora e avalie os clusters, pois eles produzirão mais rendimento. Direcione o incentivá e instrua os clientes somente se ainda houver capacidade depois de você direcionar o Act agora e avaliar os clientes. | 
| D365BCFit | Pontos de dados internos e externos que definem firmographics. Ajustar a pontuação usa um modelo lookalike para nosso melhor SMB para comparar os clientes e ver se eles são um ajuste potencial para os produtos de nuvem da Microsoft. Ajustar Pontuação é atualizado trimestral. | 
| D365BCIntent | Os sinais relacionados à mídia social e ao comportamento online de um cliente definem a intenção. A pontuação da intenção é sobreposta em ajustar para definir os clusters. A pontuação da intenção é atualizada mensalmente. | 
| D365FOCluster | Identifica as propensações do cliente para comprar as operações e finanças do Dynamics 365. Os clientes que mostrarem uma propensão para finanças + operações estarão nas principais categorias não gerenciadas. Direcione o Act agora e avalie os clusters, pois eles produzirão mais rendimento. Direcione o incentivá e instrua os clientes somente se ainda houver capacidade depois de você direcionar o Act agora e avaliar os clientes. | 
| D365FOFit | Pontos de dados internos e externos que definem firmographics. Ajustar a pontuação usa um modelo lookalike para nosso melhor SMB para comparar os clientes e ver se eles são um ajuste potencial para os produtos de nuvem da Microsoft. Ajustar Pontuação é atualizado trimestral. | 
| D365FOIntent | Sinais relacionados à mídia social e ao comportamento online de um cliente definem Intenção. A pontuação da intenção é sobreposição em Ajustar para definir os clusters. A pontuação da intenção é atualizada mensalmente. | 
| D365CECluster | Identifica a propensão do cliente para comprar o Dynamics 365 Customer Engagement. Os clientes que mostram uma propensão para o Customer Engagement estarão nas categorias Média e Pequena. Ação de Destino Agora e Avaliar clusters, pois eles produzirão um rendimento mais alto. Direcionar e instruir os clientes somente se ainda houver capacidade depois que você direcionar Agir agora e Avaliar clientes. | 
| D365CEFit | Indica Ajuste para o Dynamics 365 Customer Engagement | 
| D365CEIntent | Indica a intenção do Dynamics 365 Customer Engagement | 
| DynamicsOnPremAXorCRM_HasOpenRenewal | Identifica se o cliente tem uma renovação aberta para o Dynamics AX ou CRM local | 
| M365UpsellCustomer | Identifica se o cliente mostra a propensão de venda para Microsoft 365 | 
| Tem o Google | Identifica se o cliente mostra sinais competitivos para a propriedade de produtos do Google | 
| Tem AWS | Identifica se o cliente mostra sinais competitivos para produtos AWS de propriedade | 
| Tem EA | Identifica se uma renovação é uma assinatura EA ou EA | 
| Está aberto | Identifica se uma renovação é um contrato Open ou Open Value | 

### <a name="cloud-ascent---azure-propensity-report"></a>**Nuvem ascendente – relatório de propensão do Azure**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| ID MPN | ID de Microsoft Partner Network | 
| Nome do parceiro | Nome do parceiro | 
| ID do Cliente | Número do identificador do cliente | 
| Número de DUNS | O Dun & Bradstreet número do cliente que está sendo pontuado quanto à propensão | 
| Nome da Conta | Nome da conta | 
| Domínio | Domínio da conta | 
| Tamanho da organização | Tamanho da organização | 
| Setor | Setor | 
| Vertical | A vertical do cliente que está sendo pontuada pela propensão, conforme identificado pela Microsoft, D&B e outros padrões do setor | 
| Área | Área geográfica do local | 
| Subsidiária | A subsidiária do cliente que está sendo pontuada quanto à propensão | 
| Território de Vendas | A região de vendas do cliente que está sendo pontuada quanto à propensão | 
| City | Local da cidade geográfica | 
| Estado | Local do estado geográfico | 
| Código postal | Cep da organização | 
| País | Localização geográfica do país | 
| Segment | Segmento de mercado | 
| Sub-segmento | Subseção de mercado | 
| Resumo do tipo SMC | Tipo SMC | 
| Top Unmanaged - Compute Base | Principais clientes não planejados – computação | 
| Top Unmanaged – User Base | Principais clientes não planejados – usuários | 
| IsNonProfit | Indica se a organização é sem fins lucrativos (Sim ou Não) | 
| Migrar – EOL Windows Server – EOL Windows Server IB com propensão do Cloud Ascent – 5+ licenças | Cliente que tem um Windows Server local de EOL (ou seja, uma versão EOL ou anterior). O cliente tem 5 ou mais licenças. Cliente que tem uma pontuação de propensão. O parceiro deve direcionar esse cliente para migração para o Azure. | 
| Migrar – EOL Windows Server – EOL Windows Server IB com propensão do Cloud Ascent – <5 licenças | Cliente que tem um Windows Server local de EOL (ou seja, uma versão EOL ou anterior). O cliente tem menos de 5 licenças. Cliente que tem uma pontuação de propensação. O parceiro deve direcionar esse cliente para a migração para o Azure. | 
| Migrate-EOL Windows Server-EOL Windows Server IB sem a nuvem de elevação de linha-5 + licenças | Cliente que tem um EOL do Windows Server local (ou seja, uma versão do EOL ou anterior). O cliente tem mais de 5 licenças. O cliente não tem uma pontuação de propensação. O parceiro deve direcionar esse cliente para a migração para o Azure. | 
| Migrate-EOL Windows Server-EOL Windows Server IB sem Cloud elevação da nuvem-<5 licenças | Cliente que tem um EOL do Windows Server local (ou seja, uma versão do EOL ou anterior). Tem menos de 5 licenças. O cliente não tem uma pontuação de propensação. O parceiro deve direcionar esse cliente para a migração para o Azure. | 
| Migrar-EOL SQL-EOL SQL Server IB com o Cloud ascendence propensation-5 + licenças | Cliente que tem um EOL local SQL Server (ou seja, uma versão de EOL ou anterior). O cliente tem mais de 5 licenças. O cliente tem uma pontuação de propensação. O parceiro deve direcionar esse cliente para a migração para o Azure. | 
| Migrar-EOL SQL-EOL SQL Server IB com a propensação de nuvem ascendente-<5 licenças | Cliente que tem um EOL local SQL Server (ou seja, uma versão de EOL ou anterior). Tem menos de 5 licenças. Cliente que tem uma pontuação de propensão. O parceiro deve direcionar esse cliente para migração para o Azure. | 
| Migrar – EOL SQL – EOL SQL Server IB sem propensão do Cloud Ascent – 5+ licenças | Cliente que tenha um EOL local SQL Server (ou seja, uma versão de EOL ou anterior). O cliente tem 5 ou mais licenças. O cliente não tem uma pontuação de propensão. O parceiro deve direcionar esse cliente para migração para o Azure. | 
| Migrar – EOL SQL – EOL SQL Server IB sem propensão do Cloud Ascent – <5 licenças | Cliente que tenha um EOL local SQL Server (ou seja, uma versão de EOL ou anterior). O cliente tem menos de 5 licenças. O cliente não tem uma pontuação de propensão. O parceiro deve direcionar esse cliente para migração para o Azure. | 
| Migrar – Migrar o Windows Server local – IB atual do Windows Server com propensão do Cloud Ascent – mais de 5 licenças | Cliente que tem um Windows Server local atual (ou seja, uma versão posterior à EOL). O cliente tem mais de 5 licenças. O cliente tem uma pontuação de propensão. O parceiro deve direcionar esse cliente para migração para o Azure. | 
| Migrar – Migrar o Windows Server local – IB atual do Windows Server com propensão do Cloud Ascent – <5 licenças | Cliente que tem um Windows Server local atual (ou seja, uma versão posterior à EOL). O cliente tem menos de 5 licenças. O cliente tem uma pontuação de propensação para o Azure. O parceiro deve direcionar esse cliente para a migração para o Azure. | 
| Migrar-migrar o Windows Server local-Windows Server IB atual sem o Cloud elevação da nuvem-5 + licenças | Cliente que tem um Windows Server local atual (ou seja, uma versão posterior à EOL). O cliente tem mais de 5 licenças. O cliente não tem uma pontuação de propensação. O parceiro deve direcionar esse cliente para a migração para o Azure. | 
| Migrar-migrar o Windows Server local para o Windows Server IB atual sem a propensão de elevação da nuvem-<5 licenças | Cliente que tem um Windows Server local atual (ou seja, uma versão posterior à EOL). O cliente tem menos de 5 licenças. O cliente não tem uma pontuação de propensação. O parceiro deve direcionar esse cliente para a migração para o Azure. | 
| Migrar – migrar para máquinas virtuais (VMs) SQL ou SQL do Azure – atual SQL Server IB com a propensão de elevação de nuvem-5 + licenças | Cliente que tem uma SQL Server local atual (ou seja, uma versão posterior à EOL). O cliente tem mais de 5 licenças. O cliente tem uma pontuação de propensação. O parceiro deve direcionar esse cliente para a migração para o Azure. | 
| Migrar – migrar para VMs SQL ou SQL do Azure-atual SQL Server IB com propensão de elevação de nuvem-<5 licenças | Cliente que tem uma SQL Server local atual (ou seja, uma versão posterior à EOL). O cliente tem menos de 5 licenças. O cliente tem uma pontuação de propensão. O parceiro deve direcionar esse cliente para migração para o Azure. | 
| Migrar – Migrar para VMs SQL do Azure ou SQL – IB de SQL Server atual sem propensão do Cloud Ascent – 5+ licenças | Cliente que tem uma versão atual local SQL Server (ou seja, uma versão posterior à EOL). O cliente tem mais de 5 licenças. O cliente não tem uma pontuação de propensão. O parceiro deve direcionar esse cliente para migração para o Azure. | 
| Migrar – Migrar para VMs SQL do Azure ou SQL – IB de SQL Server atual sem propensão do Cloud Ascent – <5 licenças | Cliente que tem uma versão atual local SQL Server (ou seja, uma versão posterior à EOL). O cliente tem menos de 5 licenças. O cliente não tem uma pontuação de propensão. O parceiro deve direcionar esse cliente para migração para o Azure. | 
| Migrar – OSS – Migrar para o BD OsS (Open Source) | Cliente existente com qualquer um dos seguintes produtos de competição: PostgreSQL, MySQL, MariaDB. O parceiro deve direcionar esse cliente para migração para o Azure. | 
| Migrar – OSS – Linux no Azure | Cliente existente com Linux. O parceiro deve direcionar esse cliente para migração para o Azure. | 
| Migrar – SAP – SAP no Azure | Cliente existente com SAP. O parceiro deve direcionar esse cliente para a migração para o Azure. | 
| Migrar-área de trabalho virtual do Windows-Serviços de Área de Trabalho Remota IB | Identifica os clientes com o Windows Serviços de Área de Trabalho Remota ativo. O parceiro deve direcionar esse cliente para a migração para o Azure. | 
| Migrar-área de trabalho virtual do Windows-vendas modernas de venda cruzada para Azure/WVD | Identifica os clientes com Microsoft 365 e não tem o Azure. O parceiro deve direcionar esse cliente para a migração para o Azure. | 
| Migrar-VMware IB | Cliente existente com o produto: VMware. O parceiro deve direcionar esse cliente para a migração para o Azure. | 
| Migrar – Citrix IB | Cliente existente com o produto: Citrix Systems. O parceiro deve direcionar esse cliente para a migração para o Azure. | 
| Inovar-Analytics-Power BI IB com alta propensão do Azure | Os clientes com a assinatura do e do Active Power BI, incluindo: Power BI – pro autônomos, Power BI conjuntos do Azure, conjuntos de Power BI-Office, pacotes de Power BI-Microsoft 365 | 
| Enable-DevOps com o GitHub – Visual Studio/MSDN IB | Identifica clientes com versões ativas do Visual Studio | 
| Versão standard do Windows Server | Exibe a versão do Windows Server Standard compras pelo cliente | 
| Licença do Windows Server Standard | Exibe o tipo de licença de compras do Windows Server Standard pelo cliente | 
| Versão do Windows Server Data Center | Exibe a versão das compras do Windows Data Center pelo cliente | 
| Licença do Windows Server Data Center | Exibe o tipo de licença de compras do Windows Data Center pelo cliente | 
| AzureFit | Pontos de dados internos e externos que definem firmográficos. A pontuação de ajuste usa um modelo semelhante ao nosso melhor SMB para comparar clientes e ver se eles são uma possível opção para produtos de nuvem da Microsoft. A pontuação de ajuste é atualizada trimestralmente. | 
| AzureIntent | Sinais relacionados à mídia social e ao comportamento online de um cliente definem Intenção. A pontuação da intenção é sobreposição em Ajustar para definir os clusters. A pontuação da intenção é atualizada mensalmente. | 
| AzureCluster | Identifica a propensão do cliente para comprar o Azure consolidando as recomendações de Ajuste e Intenção em um cluster. Ação de Destino Agora e Avaliar clusters, pois eles produzirão um rendimento mais alto. Direcionar e instruir os clientes somente se ainda houver capacidade depois que você direcionar Agir agora e Avaliar clientes. | 
| WindowsServerDataCenter_HasOpenRenewal | Identifica se o cliente tem uma renovação aberta para o Windows Server Datacenter | 
| WindowsServerStandard_HasOpenRenewal | Identifica se o cliente tem uma renovação aberta para o Windows Server Standard | 
| AzureUpsellCustomer | Identifica se o cliente mostra a propensão de venda para o Azure | 
| Tem Google | Identifica se o cliente mostra sinais competitivos para produtos pertencentes ao Google | 
| Tem AWS | Identifica se o cliente mostra sinais competitivos para produtos AWS de propriedade | 
| Tem EA | Identifica se uma renovação é uma assinatura EA ou EA | 
| Está aberto | Identifica se uma renovação é um contrato Open ou Open Value | 

### <a name="cloud-ascent---agreement-renewal-propensity-report"></a>**Relatório de propensão de renovação do contrato de elevação da nuvem**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| ID MPN | ID de Microsoft Partner Network | 
| Nome do parceiro | Nome do parceiro | 
| ID do Cliente | Número do identificador do cliente | 
| Número de DUNS | O Dun & Bradstreet número do cliente que está sendo pontuado quanto à propensão | 
| Nome da Conta | Nome da conta | 
| Domínio | Domínio da conta | 
| Tamanho da organização | Tamanho da organização | 
| Setor | Setor | 
| Vertical | A vertical do cliente que está sendo pontuado para propensão, conforme identificado pela Microsoft, D&B e outros padrões do setor | 
| Área | Área geográfica do local | 
| Subsidiária | A subsidiária do cliente que está sendo pontuado para propensão | 
| Território de Vendas | O território de vendas do cliente que está sendo pontuado para propensão | 
| City | Localização geográfica da cidade | 
| Estado | Localização do estado geográfico | 
| Código postal | Cep da organização | 
| País | Localização geográfica do país | 
| Segment | Segmento de mercado | 
| Sub-segmento | Subseção de mercado | 
| Resumo do tipo SMC | Tipo SMC | 
| Top Unmanaged - Compute Base | Principais clientes não planejados – computação | 
| Top Unmanaged – User Base | Principais clientes não planejados – usuários | 
| IsNonProfit | Indica se a organização é sem fins lucrativos (Sim ou Não) | 
| Tem Google | Identifica se o cliente mostra sinais competitivos para produtos AWS de propriedade | 
| Tem AWS | Identifica se o cliente mostra sinais competitivos para produtos AWS de propriedade | 
| Cluster do Azure | Identifica as propensações do cliente para comprar o Azure. Direcione o Act agora e avalie os clusters, pois eles produzirão mais rendimento. Direcione o incentivá e instrua os clientes somente se ainda houver capacidade depois de você direcionar o Act agora e avaliar os clientes. | 
| D365 Finanças + cluster de operações | Identifica as propensações do cliente para comprar as operações e finanças do Dynamics 365. Os clientes que mostrarem uma propensão para finanças + operações estarão nas principais categorias não gerenciadas. Direcione o Act agora e avalie os clusters, pois eles produzirão mais rendimento. Direcione o incentivá e instrua os clientes somente se ainda houver capacidade depois de você direcionar o Act agora e avaliar os clientes. | 
| Cluster D365 CE | Identifica as propensações do cliente para comprar o compromisso com o cliente do Dynamics 365. Os clientes que mostrarem uma propensação para o envolvimento do cliente estarão nas categorias média e pequena. Direcione o Act agora e avalie os clusters, pois eles produzirão mais rendimento. Direcione o incentivá e instrua os clientes somente se ainda houver capacidade depois de você direcionar o Act agora e avaliar os clientes. | 
| Cluster D365 BC | Identifica as propensações do cliente para comprar o Dynamics 365 Business central. Os clientes que mostram uma propensão para o Business Central estarão nas categorias Média e Pequena. Ação de Destino Agora e Avaliar clusters, pois eles produzirão um rendimento mais alto. Direcionar e instruir os clientes somente se ainda houver capacidade depois que você direcionar Agir agora e Avaliar clientes. | 
| Microsoft 365 Cluster | Identifica a propensão do cliente para comprar Microsoft 365. Ação de Destino Agora e Avaliar clusters, pois eles produzirão um rendimento mais alto. Direcionar e instruir os clientes somente se ainda houver capacidade depois que você direcionar Agir agora e Avaliar clientes. | 
| Programa de licença | Identifica o tipo de programa de licença para a renovação | 
| ID do contrato | Identificador do contrato | 
| Data de término do contrato | Data de término do contrato | 
| Tipo de Expiração | Tipo de expiração | 
| Expirando receita | Receita associada a assinaturas de expiração | 
| Tem EA | Identifica se uma renovação é um EA ou uma assinatura do EA | 
| Tem Aberto | Identifica se uma renovação é um contrato Open ou Open Value | 
| Cliente do Azure Upsell | Identifica se o cliente mostra a propensão de venda para o Azure | 
| Cliente de venda Microsoft 365 | Identifica se o cliente mostra a propensão de venda para Microsoft 365 | 
| RevSumDivisionName | Identifica o produto que está ativo para renovação | 

## <a name="next-steps"></a>Próximas etapas

Para obter mais informações, consulte [baixar relatórios](pci-download-reports.md).
