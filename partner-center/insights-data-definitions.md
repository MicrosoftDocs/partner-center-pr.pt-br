---
title: Definições de dados do Insights
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: o documento lista vários relatórios e suas definições de dados, que podem ser baixados na página Insights download de relatório.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c77f5eb97771c4768f76b8d35c0d4493c5070ff2
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114374874"
---
# <a name="export--data-definitions"></a>Exportar – definições de dados 

**Funções apropriadas**: Visualizador de relatórios | Visualizador de relatórios executivos

## <a name="introduction"></a>Introdução 

usando o hub baixar relatórios no painel do Insights, você pode exportar os conjuntos de valores brutos. 

Os vários relatórios, que você pode baixar juntamente com suas definições de dados, estão listados nas seguintes tabelas: 

### <a name="partner-profile-report"></a>**Relatório de perfil do parceiro**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| MPNId | ID do Microsoft Partner Network (MPN)| 
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
| CustomerTpid | Identificador do pai superior do cliente | 
| CustomerSegment | Segmento de cliente | 
| CustomerMarket | Mercado geográfico do cliente | 
| CustomerStatus | Status do cliente (ativo ou inativo) | 
| Produto | o produto vendido ao cliente por MPN: Office 365, Dynamics 365, Enterprise Mobility and Security, Power BI ou Microsoft Azure | 
| SKU | SKU do Produto | 
| Mês | Mês para o qual o uso e a receita são relatados | 
| MPNId | Identificador de Microsoft Partner Network | 
| PartnerName | Nome do parceiro | 
| PartnerLocation | Localização geográfica do parceiro | 
| PartnerAttributionType | Tipo de atribuição do parceiro | 
| SalesChannel | Canal de vendas | 
| AvailableSeats | Estações disponíveis | 
| RevenueUSD | Receita em dólares americanos | 

### <a name="reseller-performance-report"></a>**Relatório de desempenho do revendedor**

> [!Note]
> A receita e os dados de receita consumida do Azure (ACR) estão disponíveis somente para usuários que são visualizadores de relatórios executivos.

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| ResellerMPNid | Identificador de Microsoft Partner Network do revendedor | 
| ResellerName | Nome do revendedor | 
| ResellerMarket | País do revendedor do mercado | 
| IndirectProviderMPNId | Identificador do Microsoft Partner Network do provedor indireto | 
| IndirectProviderName | Nome do provedor indireto | 
| Mês | Mês para o qual o uso e a receita são relatados | 
| Produto | Nome do produto | 
| SubscriptionID | Identificador da assinatura | 
| AvailableSeats | Número de estações disponíveis | 
| AssignedSeats | Número de estações atribuídas | 
| BilledRevenueUSD | Receita cobrada em dólares dos EUA | 
| CustomerName | Nome do cliente que comprou a assinatura | 
| CustomerTPid | Identificador do pai superior do cliente | 
| CustomerSegment | Segmento de cliente | 
| CustomerMarket | Mercado geográfico do cliente | 
| ResellerStatus | Status do revendedor | 

### <a name="subscription-details-report"></a>**Relatório detalhes da assinatura**

>[!Note]
>Os dados de receita e ACR estão disponíveis apenas para usuários que são visualizadores de relatórios executivos.

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| SubscriptionId | GUID da assinatura | 
| SubscriptionStartDate | Data de início da assinatura | 
| SubscriptionEndDate | Data de término da assinatura | 
| SubscriptionState | Estado da assinatura (Ativo ou Rotatividade) | 
| Mês | Mês para o qual o uso e a receita são relatados | 
| IsAutoRenew | Indica se a assinatura é renovada automaticamente (Sim ou Não) | 
| CustomerName | Nome do cliente que comprou a assinatura | 
| CustomerTenantId | GUID do cliente | 
| CustomerTpid | Identificador pai principal do cliente | 
| CustomerSegment | Segmento de mercado do cliente | 
| CustomerMarket | Mercado geográfico do cliente | 
| Produto | Produto vendido ao cliente pelo parceiro | 
| SKU | SKU do produto | 
| MPNId | Microsoft Partner Network ID do parceiro | 
| PartnerName | Nome do parceiro | 
| PartnerLocation | Localização geográfica do parceiro | 
| PartnerAttributionType | Tipo de atribuição para a assinatura | 
| SalesChannel | Canal de vendas – Direct, Provedor de Soluções na Nuvem (CSP) e assim por diante | 
| AvailableSeats | Banco disponível atual | 
| RevenueUSD | Receita em dólares americanos | 
| ID de Registro | ID de registro da assinatura | 

### <a name="azure-usage-report"></a>**Relatório de uso do Azure**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| SubscriptionId | GUID da assinatura | 
| SubscriptionStartDate | A data do início da assinatura | 
| SubscriptionEndDate | A data do final da assinatura | 
| SubscriptionState | Estado atual da assinatura (Aberto, Fechado, Ativo ou Em Período de Carência) | 
| Mês | Data agregada por mês | 
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
| SalesChannel | Canal de vendas (Direct/CSP, Indirect/CSP, Direct e assim por diante) | 
| ACR_USD | Receita consumida (ACR) do Azure em dólares americanos | 
| ID de Registro | ID de registro da assinatura do Azure | 

### <a name="office-365-license-usage-report"></a>**Office 365 de uso de licença**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| CustomerTenantId | ID do locatário do cliente | 
| CustomerTpid | ID pai principal do cliente | 
| WorkloadName | Skype for Business, Teams, Exchange Online | 
| Mês | Mês para o qual o uso é relatado | 
| PaidAvailableUnits | Número de unidades pagas disponíveis | 
| MonthlyActiveUsers | Número de usuários ativos mensais | 
| CustomerName | Nome do cliente que comprou a assinatura | 
| CustomerMarket | Local do país geográfico do mercado do cliente | 
| CustomerSegment | Segmento de cliente | 
| MPNId | Identificador de Microsoft Partner Network | 
| PartnerName | Nome do parceiro | 
| PartnerLocation | Localização geográfica do parceiro | 
| PartnerAttributionType | Tipo de atribuição do parceiro | 

### <a name="enterprise-mobility-license-usage-report"></a>**Enterprise Relatório de uso de licenças de mobilidade**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| CustomerTenantId | ID do locatário do cliente | 
| CustomerTpid | ID pai superior do cliente | 
| Carga de trabalho | nome da carga de trabalho do Enterprise Mobility + Security (EMS) | 
| Mês | Mês para o qual o uso é relatado | 
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
| Mês | Mês para o qual o uso é relatado | 
| RevSumDivisionName | Nome da divisão da soma da revisão | 
| RevSumCategoryName | Nome da categoria da soma da revisão | 
| SKU | SKU do produto | 
| SKUId | ID do SKU do produto | 
| FreeVsPaidSKU | Indica se é um SKU gratuito ou pago | 
| SalesModel | Canal de vendas que é usado para vender a assinatura | 
| DetailedSalesModel | Modelo de vendas detalhado para a assinatura | 
| CustomerName | Nome do cliente que comprou a assinatura | 
| CustomerTenantId | GUID do locatário do cliente | 
| CustomerTpid | Identificador pai superior do cliente | 
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

### <a name="power-bi-license-usage-report"></a>**relatório de uso de licença Power BI**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| SubscriptionId | GUID da assinatura | 
| SubscriptionStartDate | Data de início da assinatura | 
| SubscriptionEndDate | Data de término da assinatura | 
| SubscriptionStatus | Estado da assinatura (Ativo, Inativo ou Em Período de Carência) | 
| Mês | Data agregada por mês | 
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
| AvailableSeats | Lugares disponíveis atuais | 
| AssignedSeats | Bancos atribuídos atuais | 
| ActiveSeats | Bancos ativos atuais | 
| DeploymentOpportunity | Oportunidade de implantação atual | 
| ActiveUsagePercent | Percentual de uso ativo atual | 

### <a name="teams-meetings-and-calls-report"></a>**Teams relatório de chamadas e reuniões**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| CustomerTenantId | ID do locatário do cliente | 
| CustomerTpid | Identificador do pai principal do cliente | 
| Mês | Mês para o qual o uso é relatado | 
| Subtrabalho | Subtrabalho para o qual o uso é relatado (reuniões, chamadas ou sistemas de telefone) | 
| Contagem de reunião | Número de reuniões | 
| Duração da reunião | Duração total da reunião em horas | 

### <a name="teams-monthly-usage-report"></a>**Teams relatório de uso mensal**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| CustomerTenantId | ID do locatário do cliente | 
| CustomerTpid | Identificador do pai principal do cliente | 
| Mês | Mês para o qual o uso é relatado | 
| Subtrabalho | Subtrabalho para o qual o uso é relatado (reuniões, chamadas ou sistemas de telefone) | 
| Usuários da área de trabalho | Número de usuários que usam Teams área de trabalho | 
| Usuários Móveis | Número de usuários que usam Teams em dispositivos móveis | 
| Usuários da Web | Número de usuários que usam Teams na Web | 
| AllUpParticipants | Número de usuários exclusivos Teams para o mês | 

### <a name="teams-usage-3p-apps-report"></a>**Teams relatório de aplicativos 3P de uso**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| CustomerTenantId | ID do locatário do cliente | 
| CustomerTpid | ID pai principal do cliente | 
| Mês | Mês para o qual o uso é relatado | 
| Nome do aplicativo 3P | Nome do aplicativo Teams aplicativo | 
| Contagem de usuários | Número de usuários para o aplicativo | 


### <a name="training-details-report"></a>**Relatório de detalhes do treinamento**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| TrainingActivityId | Identificador do treinamento | 
| TrainingTitle | Título do treinamento | 
| Traintype | Tipo de treinamento (certificação ou exame) | 
| IndividualFirstName | Nome do cliente | 
| IndividualLastName | Sobrenome do cliente | 
| Email | ID de email pessoal do cliente | 
| CorpEmail | ID de email Office do cliente | 
| TrainingCompletionDate | Data de conclusão do treinamento | 
| Mês | Mês para o qual os dados são relatados | 
| IcMCP | indica se o usuário é um Microsoft certified Professional (MCP) | 
| MCPID | ID do MCP do usuário | 
| MPNId | Identificador de Microsoft Partner Network | 
| PartnerName | Nome do parceiro | 
| PartnerCityLocation | Local da cidade geográfica do parceiro | 
| PartnerCountryLocation | Localização geográfica do país do parceiro | 

### <a name="microsoft-learn-report"></a>**Relatório de Microsoft Learn**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| UserName | Nome do usuário | 
| UserId | GUID do usuário | 
| Trainname | Nome do treinamento | 
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
| Competêncianame | Nome da competência | 
| CompetencyAttainmentOptionName | Nome da opção de obtenção de competência | 
| Mês | Mês para o qual as métricas são relatadas | 
| MetricName | Nome da métrica que é relevante para a competência | 
| MetricMonthlyContribution | Contribuição mensal da métrica | 
| TTMAggregate | Métrica agregada para os 12 meses à direita | 
| AnniversaryYearAggregate | Métrica agregada para o ano de aniversário atual | 
| GoldThreshold | Requisito de desempenho para atender à competência ouro | 
| SilverThreshold | Requisito de desempenho para atender à competência prateada | 

### <a name="cloud-ascent---microsoft-365-propensity-report"></a>**relatório de propensão Microsoft 365 a nuvem ascendente**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| ID MPN | ID de Microsoft Partner Network | 
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
| Resumo do tipo SMC | Tipo do SMC | 
| Superior não gerenciado-base de computação | Principais clientes não gerenciados – computação | 
| Principal base de usuários não gerenciados | Principais clientes não gerenciados – usuário | 
| IsNonProfit | Indica se a organização não é de lucro (Sim ou não) | 
| Habilitar Exchange Online de destino de trabalho remoto | clientes que têm uma assinatura do active Exchange Online, se revender a Microsoft 365 | 
| Habilitar a aquisição remota de trabalho local (versão atual) com a propensação de elevação da nuvem-+ 10 licenças | cliente que tem um cliente local Office ou Windows atual. Ou seja, a versão do cliente é posterior à versão do fim da vida útil (EOL). O cliente tem 10 ou mais licenças. Cliente que tem uma pontuação de propensação. O parceiro deve direcionar a conversão para Microsoft 365. | 
| Habilitar a aquisição remota de trabalho local (versão atual) com a propensão de elevação da nuvem-<10 licenças | cliente que tem um Office local ou Windows cliente atual (ou seja, uma versão posterior à EOL). O cliente tem menos de 10 licenças. Cliente que tem uma pontuação de propensação. O parceiro deve direcionar a conversão para Microsoft 365. | 
| Habilitar a aquisição remota de trabalho local (versão atual) sem a propensão de elevação da nuvem-+ 10 licenças | cliente que tem um Office local ou Windows cliente atual (ou seja, uma versão posterior à EOL). O cliente tem 10 ou mais licenças. O cliente não tem uma pontuação de propensação. O parceiro deve direcionar a conversão para Microsoft 365. | 
| Habilitar a aquisição remota de trabalho local (versão atual) sem a propensão de elevação de nuvem-<10 licenças | cliente que tem um Office local ou Windows cliente atual (ou seja, uma versão posterior à EOL). O cliente tem menos de 10 licenças. O cliente não tem uma pontuação de propensação. O parceiro deve direcionar a conversão para Microsoft 365. | 
| Habilitar a aquisição remota de trabalho local (versão EOL) com a propensão de elevação da nuvem-+ 10 licenças | cliente que tem um eol local Office ou Windows cliente (ou seja, uma versão de eol ou anterior). O cliente tem 10 ou mais licenças. O cliente tem uma pontuação de propensação. O parceiro deve direcionar a conversão para Microsoft 365. | 
| Habilitar a aquisição remota de trabalho local (versão EOL) com a propensão de elevação de nuvem-<10 licenças | cliente que tem um eol local Office ou Windows cliente (ou seja, uma versão de eol ou anterior). O cliente tem menos de 10 licenças. O cliente tem uma pontuação de propensação. O parceiro deve direcionar a conversão para Microsoft 365. | 
| Habilitar a aquisição remota de trabalho local (versão de EOL) sem a propensão de elevação da nuvem-+ 10 licenças | cliente que tem um cliente local Office ou Windows atual (ou seja, uma versão de EOL ou anterior). O cliente tem 10 ou mais licenças. O cliente não tem uma pontuação de propensação. O parceiro deve direcionar a conversão para Microsoft 365. | 
| Habilitar a aquisição remota de trabalho local (versão de EOL) sem a propensão de elevação de nuvem-<10 licenças | cliente que tem um cliente local Office ou Windows atual (ou seja, uma versão de EOL ou anterior). O cliente tem menos de 10 licenças. O cliente não tem uma pontuação de propensação. O parceiro deve direcionar a conversão para Microsoft 365. | 
| habilitar a prospecção de trabalho remoto-alta propensation para Microsoft 365 (Act NowithEvaluate) | Cliente cliente potencial com alta propensão para Microsoft 365 | 
| Habilitar trabalho remoto – competição (zoom) com Microsoft 365 | cliente com Zoom e Microsoft 365, destino para conversão em Teams | 
| Habilitar trabalho remoto – competição (zoom) sem Microsoft 365 | Cliente com zoom, destino para conversão para Teams | 
| reduzir o custo e gerenciar Microsoft 365 E3 direcionados para Microsoft 365 E5 | cliente existente com Microsoft 365 E3, destino para Microsoft 365 E5 | 
| reduza custos e gerencie-Microsoft 365 Business Basic e clientes padrão de negócios direcionados para Microsoft 365 Business Premium | clientes existentes de Microsoft 365 Business Basic e Business Standard, visando Microsoft 365 Business Premium | 
| Transformar a produtividade organizacional – propensação da superfície | O cliente mostra uma propensação para a superfície | 
| M365Cluster | Identifica a propensão de um cliente para comprar Microsoft 365. Direcione o Act agora e avalie os clusters porque eles produzirão um rendimento maior. Direcione o incentivá e instrua os clientes somente se ainda houver capacidade após o Act Now e avaliar os clientes. | 
| M365Fit | Pontos de dados internos e externos que definem firmographics. Ajustar a pontuação usa um modelo de lookalike para nossas melhores empresas de pequeno ou médio porte (SMBs) para comparar os clientes e ver se eles são uma possível adequação para os produtos de nuvem da Microsoft. Ajustar Pontuação é atualizado trimestral. | 
| M365Intent | Os sinais relacionados à mídia social e ao comportamento online de um cliente definem a intenção. A pontuação da intenção é sobreposta em ajustar para definir os clusters. A pontuação da intenção é atualizada mensalmente. | 
| SurfaceCluster | Identifica a propensão de um cliente para comprar a superfície consolidando as recomendações de ajuste e de intenção em um cluster. Direcione o Act agora e avalie os clusters porque eles produzirão um rendimento maior. Direcione o incentivá e instrua os clientes somente se ainda houver capacidade após o Act Now e avaliar os clientes. | 
| SurfaceFit | Pontos de dados internos e externos que definem firmographics. Ajustar a pontuação usa um modelo de lookalike para nossos melhores SMBs para comparar os clientes e ver se eles são um ajuste potencial para os produtos de nuvem da Microsoft. Ajustar Pontuação é atualizado trimestral. | 
| SurfaceIntent | Os sinais relacionados à mídia social e ao comportamento online de um cliente definem a intenção. A pontuação da intenção é sobreposta em ajustar para definir os clusters. A pontuação da intenção é atualizada mensalmente. | 
| O365Cluster | Identifica as propensações do cliente para comprar Office 365. Direcione o Act agora e avalie os clusters porque eles produzirão um rendimento maior. Direcione o incentivá e instrua os clientes somente se ainda houver capacidade após o Act Now e avaliar os clientes. | 
| O365Fit | Pontos de dados internos e externos que definem firmographics. Ajustar a pontuação usa um modelo de lookalike para nossos melhores SMBs para comparar os clientes e ver se eles são um ajuste potencial para os produtos de nuvem da Microsoft. Ajustar Pontuação é atualizado trimestral. | 
| O365Intent | Os sinais relacionados à mídia social e ao comportamento online de um cliente definem a intenção. A pontuação da intenção é sobreposta em ajustar para definir os clusters. A pontuação da intenção é atualizada mensalmente. | 
| M365UpsellCustomer | Identifica se o cliente mostra a propensão de venda para Microsoft 365 | 
| Tem Google | Identifica se o cliente mostra sinais competitivos para produtos pertencentes ao Google | 
| Tem AWS | Identifica se o cliente mostra sinais competitivos para produtos de Amazon Web Services de propriedade (AWS) | 
| Tem EA | Identifica se uma renovação é um EA (Enterprise Agreement) ou uma assinatura EA | 
| Está aberto | Identifica se uma renovação é um contrato Open ou Open Value | 

### <a name="cloud-ascent---dynamics-365-propensity-report"></a>**Relatório de propensabilidade da nuvem ascendente-Dynamics 365**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| ID MPN | ID do Microsoft Partner Network (MPN) | 
| Nome do parceiro | Nome do parceiro | 
| ID do Cliente | Número do identificador do cliente | 
| Número de DUNS | O Dun & Bradstreet número do cliente que está sendo pontuado quanto à propensão | 
| Nome da Conta | Nome da conta | 
| Domínio | Domínio da conta | 
| Tamanho da organização | Tamanho da organização | 
| Setor | Setor ao qual a organização pertence | 
| Vertical | A vertical do cliente que está sendo pontuada pela propensão, conforme identificado pela Microsoft, D&B e outros padrões do setor
| Área | Área geográfica do local | 
| Subsidiária | A subsidiária do cliente que está sendo pontuada quanto à propensão | 
| Território de Vendas | A região de vendas do cliente que está sendo pontuada quanto à propensão | 
| City | Local da cidade geográfica | 
| Estado | Local do estado geográfico | 
| Código postal | Código postal da organização | 
| País | Localização geográfica do país | 
| Segment | Segmento de mercado | 
| Subsegmento | Subsegmento de mercado | 
| Resumo do tipo SMC | A categorização de um cliente: as principais bases de usuários não gerenciadas são clientes com mais de 300 funcionários, as principais bases de computação não gerenciadas são clientes com USD10, 000 em potencial de três anos do Azure, empresas de médio porte são clientes com 25 funcionários ou mais, e pequenas empresas são clientes com menos de 25 funcionários. | 
| Superior não gerenciado-base de computação | Principais clientes não gerenciados – computação | 
| Principal base de usuários não gerenciados | Principais clientes não gerenciados – usuários | 
| IsNonProfit | Indica se a organização não é de lucro (Sim ou não) | 
| ativar o tamanho de venda Digital-Microsoft 365-seat >= 25 estações (modelo de SalesPro propensation) | Cliente sem Dynamics 365. Tamanho do assento: 25 +. O parceiro deve visar a venda cruzada do Dynamics 365 SalesPro. | 
| Ativar vendas digitais – Dynamics 365 SalesPro propensation (Act Now ou Evaluate) | Clientes de alta propensão sem o Dynamics 365. O parceiro deve ser direcionado para o Dynamics 365 SalesPro. | 
| Gerenciando o risco financeiro & fraude-Dynamics local instalação base-Navision (modelo de propensão do Business central) | Cliente existente com o Navision local. O parceiro deve ter como alvo o Dynamics 365 Business central. | 
| Gerenciando o risco financeiro & fraude-Dynamics local instalação base-Dynamics AX (Dynamics 365 Finance + operações modelo de propensation) | Cliente existente com o AX local. O parceiro deve ter como destino as operações do Dynamics 365 Finance +. | 
| Gerenciando o risco financeiro & fraude-base de instalação do Dynamics local – Great Plains (modelo de propensão do Business central) | Cliente existente com excelentes Plains locais. O parceiro deve ter como alvo o Dynamics 365 Business central. | 
| Gerenciando o risco financeiro & fraude-base de instalação do Dynamics local-Solomon (modelo de propensão do Business central) | Cliente existente com Solomon local. O parceiro deve ter como alvo o Dynamics 365 Business central. | 
| Gerenciando o risco financeiro & fraude-base de instalação do Dynamics local-outros (modelo de propensão do Business central) | Cliente existente com outras soluções locais não listadas anteriormente. O parceiro deve ser destinado ao Dynamics 365 Business Central. | 
| Criar processos empresariais Agile – base de instalação local do Dynamics – AX/GP/SL/NAV/Outros (modelo de propensão do Dynamics 365) | Criar processos empresariais Agile – base de instalação local do Dynamics – AX/GP/SL/NAV/Outros (modelo de propensão do Dynamics 365) | 
| Criar Processos de Negócios Agile – Base de competências do Dynamics – Mendix/OutSystems/Salesforce (modelo de propensão do Dynamics 365) | Criar processos empresariais ágeis – Base de competências do Dynamics – Mendix/OutSystems/Salesforce (modelo de propensão do Dynamics 365) | 
| Criar processos de negócios Agile – base de instalação do Dynamics 365 Finance + Operations | Clientes existentes do Dynamics 365 Finance + Operations. Parceiro para direcionar Power Apps. | 
| Criar processos empresariais Agile – base de instalação do Dynamics 365 Business Central | Clientes existentes do Dynamics 365 Business Central. Parceiro para direcionar Power Apps. | 
| Criar processos empresariais Agile – base de instalação do Dynamics 365 Customer Engagement | Clientes existentes do Dynamics 365 Customer Engagement. Parceiro para direcionar Power Apps. | 
| Criar uma cadeia de fornecedores resiliente – Windows e ativar a primeira carga de trabalho do Dynamics 365 como Gerenciamento de Cadeia de Fornecedores do Dynamics 365 com clientes não Oracle ou SAP ERP (planejamento de recursos corporativos) | Clientes de destino para o Gerenciamento da Cadeia de Fornecedores do Dynamics 365 | 
| Criar uma cadeia de fornecedores resiliente – gerenciamento de cadeia de fornecedores do Dynamics 365 e/ou Varejo ou Comércio para clientes existentes do Dynamics 365 Customer Engagement | Os clientes existentes do Dynamics 365 Customer Engagement são destinados ao Gerenciamento de Cadeia de Fornecedores do Dynamics 365. | 
| Criar uma cadeia de fornecedores resiliente – gerenciamento de cadeia de fornecedores do Dynamics 365 e/ou Varejo ou Comércio para o Dynamics 365 Customer Engagement e Oracle ou SAP | Clientes existentes do Dynamics 365 Customer Engagement com Oracle ou SAP para direcionamento para o Gerenciamento da Cadeia de Fornecedores do Dynamics 365 | 
| D365BCCluster | Identifica a propensão do cliente para comprar o Dynamics 365 Business Central. Os clientes que mostram uma propensão para o Business Central estarão nas categorias Média e Pequena. Ação de Destino Agora e Avaliar clusters, pois eles produzirão um rendimento mais alto. Direcionar e instruir os clientes somente se ainda houver capacidade depois que você direcionar Agir agora e Avaliar clientes. | 
| D365BCFit | Pontos de dados internos e externos que definem firmográficos. A pontuação de ajuste usa um modelo semelhante ao nosso melhor SMB para comparar clientes e ver se eles são uma possível opção para produtos de nuvem da Microsoft. A pontuação de ajuste é atualizada trimestralmente. | 
| D365BCIntent | Sinais relacionados à mídia social e ao comportamento online de um cliente definem Intenção. A pontuação da intenção é sobreposição em Ajustar para definir os clusters. A pontuação da intenção é atualizada mensalmente. | 
| D365FOCluster | Identifica a propensão do cliente para comprar o Dynamics 365 Finance and Operations. Os clientes que mostram uma propensão para Finanças + Operações estarão nas principais categorias não realizadas. Ação de Destino Agora e Avaliar clusters, pois eles produzirão um rendimento mais alto. Direcionar e instruir os clientes somente se ainda houver capacidade depois que você direcionar Agir agora e Avaliar clientes. | 
| D365FOFit | Pontos de dados internos e externos que definem firmográficos. A pontuação de ajuste usa um modelo semelhante ao nosso melhor SMB para comparar clientes e ver se eles são uma possível opção para produtos de nuvem da Microsoft. A pontuação de ajuste é atualizada trimestralmente. | 
| D365FOIntent | Sinais relacionados à mídia social e ao comportamento online de um cliente definem Intenção. A pontuação da intenção é sobreposição em Ajustar para definir os clusters. A pontuação da intenção é atualizada mensalmente. | 
| D365CECluster | Identifica a propensão do cliente para comprar o Dynamics 365 Customer Engagement. Os clientes que mostram uma propensão para o Customer Engagement estarão nas categorias Média e Pequena. Ação de Destino Agora e Avaliar clusters, pois eles produzirão um rendimento mais alto. Direcionar e instruir os clientes somente se ainda houver capacidade depois que você direcionar Agir agora e Avaliar clientes. | 
| D365CEFit | Indica Ajuste para o Dynamics 365 Customer Engagement | 
| D365CEIntent | Indica a intenção do Dynamics 365 Customer Engagement | 
| DynamicsOnPremAXorCRM_HasOpenRenewal | Identifica se o cliente tem uma renovação aberta para o Dynamics AX ou CRM local | 
| M365UpsellCustomer | Identifica se o cliente mostra a propensão de venda para Microsoft 365 | 
| Tem o Google | Identifica se o cliente mostra sinais competitivos para a propriedade de produtos do Google | 
| Tem AWS | Identifica se o cliente mostra sinais competitivos para a propriedade de produtos AWS | 
| Tem EA | Identifica se uma renovação é um EA ou uma assinatura do EA | 
| Tem Aberto | Identifica se uma renovação é um contrato Open ou Open Value | 

### <a name="cloud-ascent---azure-propensity-report"></a>**Cloud Ascent – relatório de propensão do Azure**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| ID MPN | ID do Microsoft Partner Network (MPN) | 
| Nome do parceiro | Nome do parceiro | 
| ID do Cliente | Número do identificador do cliente | 
| Número DE DUNS | O número & Dun do cliente que está sendo pontuado para propensão | 
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
| Migrar – EOL Windows Server – EOL Windows Server IB com propensão do Cloud Ascent – 5+ licenças | Cliente que tem um EOL local Windows Server (ou seja, uma versão EOL ou anterior). O cliente tem 5 ou mais licenças. Cliente que tem uma pontuação de propensão. O parceiro deve direcionar esse cliente para migração para o Azure. | 
| Migrar – EOL Windows Server – EOL Windows Server IB com propensão do Cloud Ascent – <5 licenças | Cliente que tem um EOL local Windows Server (ou seja, uma versão EOL ou anterior). O Cliente tem menos de 5 licenças. Cliente que tem uma pontuação de propensão. O parceiro deve direcionar esse cliente para migração para o Azure. | 
| Migrar – EOL Windows Server – EOL Windows Server IB sem propensão do Cloud Ascent – 5+ licenças | Cliente que tem um EOL local Windows Server (ou seja, uma versão EOL ou anterior). O cliente tem mais de 5 licenças. O cliente não tem uma pontuação de propensão. O parceiro deve direcionar esse cliente para migração para o Azure. | 
| Migrar – EOL Windows Server – EOL Windows Server IB sem propensão do Cloud Ascent – <5 licenças | Cliente que tem um EOL local Windows Server (ou seja, uma versão EOL ou anterior). Tem menos de 5 licenças. O cliente não tem uma pontuação de propensão. O parceiro deve direcionar esse cliente para migração para o Azure. | 
| Migrar – EOL SQL – EOL SQL Server IB com propensão do Cloud Ascent – 5+ licenças | Cliente que tem um EOL local SQL Server (ou seja, uma versão EOL ou anterior). O cliente tem mais de 5 licenças. O cliente tem uma pontuação de propensão. O parceiro deve direcionar esse cliente para migração para o Azure. | 
| Migrar – EOL SQL – EOL SQL Server IB com propensão do Cloud Ascent – <5 licenças | Cliente que tem um EOL local SQL Server (ou seja, uma versão EOL ou anterior). Tem menos de 5 licenças. Cliente que tem uma pontuação de propensão. O parceiro deve direcionar esse cliente para migração para o Azure. | 
| Migrar – EOL SQL – EOL SQL Server IB sem propensão do Cloud Ascent – 5+ licenças | Cliente que tem um EOL local SQL Server (ou seja, uma versão EOL ou anterior). O cliente tem 5 ou mais licenças. O cliente não tem uma pontuação de propensão. O parceiro deve direcionar esse cliente para migração para o Azure. | 
| Migrar – EOL SQL – EOL SQL Server IB sem propensão do Cloud Ascent – <5 licenças | Cliente que tem um EOL local SQL Server (ou seja, uma versão EOL ou anterior). O cliente tem menos de 5 licenças. O cliente não tem uma pontuação de propensão. O parceiro deve direcionar esse cliente para migração para o Azure. | 
| Migrar – Migrar o servidor Windows local – IB do Windows Server atual com propensão de Aumento de Nuvem – 5+ licenças | Cliente que tem um servidor Windows local atual (ou seja, uma versão posterior à EOL). O cliente tem mais de 5 licenças. O cliente tem uma pontuação de propensão. O parceiro deve direcionar esse cliente para migração para o Azure. | 
| Migrar – Migrar servidor Windows local – IB do servidor Windows atual com propensão de Aumento de Nuvem – <5 licenças | Cliente que tem um servidor Windows local atual (ou seja, uma versão posterior à EOL). O cliente tem menos de 5 licenças. O cliente tem uma pontuação de propensão para o Azure. O parceiro deve direcionar esse cliente para migração para o Azure. | 
| Migrar – Migrar o servidor Windows local – IB do servidor Windows atual sem propensão do Cloud Ascent – 5+ licenças | Cliente que tem um servidor Windows local atual (ou seja, uma versão posterior à EOL). O cliente tem mais de 5 licenças. O cliente não tem uma pontuação de propensão. O parceiro deve direcionar esse cliente para migração para o Azure. | 
| Migrar – Migrar servidor Windows local – IB do servidor Windows atual sem propensão de Aumento de Nuvem – <5 licenças | Cliente que tem um servidor Windows local atual (ou seja, uma versão posterior à EOL). O cliente tem menos de 5 licenças. O cliente não tem uma pontuação de propensão. O parceiro deve direcionar esse cliente para migração para o Azure. | 
| Migrar – Migrar para VMs (máquinas virtuais) do Azure SQL ou SQL – IB do SQL Server atual com propensão de Aumento de Nuvem – 5+ licenças | Cliente que tem uma versão atual local SQL Server (ou seja, uma versão posterior à EOL). O cliente tem mais de 5 licenças. O cliente tem uma pontuação de propensão. O parceiro deve direcionar esse cliente para migração para o Azure. | 
| Migrar – Migrar para VMs SQL ou SQL do Azure – IB do SQL Server atual com propensão do Cloud Ascent – <5 licenças | Cliente que tem uma versão atual local SQL Server (ou seja, uma versão posterior à EOL). O cliente tem menos de 5 licenças. O cliente tem uma pontuação de propensão. O parceiro deve direcionar esse cliente para migração para o Azure. | 
| Migrar – Migrar para VMs SQL ou SQL do Azure – IB de SQL Server atual sem propensão do Cloud Ascent – mais de 5 licenças | Cliente que tem uma versão atual local SQL Server (ou seja, uma versão posterior à EOL). O cliente tem mais de 5 licenças. O cliente não tem uma pontuação de propensão. O parceiro deve direcionar esse cliente para migração para o Azure. | 
| Migrar – Migrar para VMs SQL ou SQL do Azure – IB do SQL Server atual sem propensão do Cloud Ascent – <5 licenças | Cliente que tem uma versão atual local SQL Server (ou seja, uma versão posterior à EOL). O cliente tem menos de 5 licenças. O cliente não tem uma pontuação de propensão. O parceiro deve direcionar esse cliente para migração para o Azure. | 
| Migrar – OSS – Migrar para o BD OsS (Open Source) | Cliente existente com qualquer um dos seguintes produtos de competição: PostgreSQL, MySQL, MariaDB. O parceiro deve direcionar esse cliente para migração para o Azure. | 
| Migrar – OSS – Linux no Azure | Cliente existente com Linux. O parceiro deve direcionar esse cliente para a migração para o Azure. | 
| Migrar-SAP-SAP no Azure | Cliente existente com SAP. O parceiro deve direcionar esse cliente para a migração para o Azure. | 
| migrar-Windows área de trabalho Virtual-Serviços de Área de Trabalho Remota IB | identifica os clientes com o active Windows Serviços de Área de Trabalho Remota. O parceiro deve direcionar esse cliente para a migração para o Azure. | 
| migrar-Windows área de trabalho Virtual-Cross vender trabalho moderno para o Azure/WVD | identifica os clientes com Microsoft 365 e não tem o Azure. O parceiro deve direcionar esse cliente para a migração para o Azure. | 
| Migrar-VMware IB | Cliente existente com o produto: VMware. O parceiro deve direcionar esse cliente para a migração para o Azure. | 
| Migrar – Citrix IB | Cliente existente com o produto: Citrix Systems. O parceiro deve direcionar esse cliente para a migração para o Azure. | 
| inovar-Analytics-Power BI IB com alta propensão do Azure | os clientes com a assinatura do e do Active Power BI, incluindo: Pro Power BI-autônomo, conjuntos de Power BI-Azure, pacotes Power BI Office, pacotes de Power BI-Microsoft 365 | 
| Enable-DevOps com GitHub-Visual Studio/MSDN IB | identifica clientes com versões do active Visual Studio | 
| Windows Versão padrão do servidor | exibe a versão do Windows Server Standard compras pelo cliente | 
| Windows Licença padrão do servidor | exibe o tipo de licença do Windows Server Standard compras pelo cliente | 
| Windows Versão do Data Center do servidor | exibe a versão do Windows as compras do data Center pelo cliente | 
| Windows Licença do Data Center do servidor | exibe o tipo de licença do Windows as compras do data Center pelo cliente | 
| AzureFit | Pontos de dados internos e externos que definem firmographics. Ajustar a pontuação usa um modelo lookalike para nosso melhor SMB para comparar os clientes e ver se eles são um ajuste potencial para os produtos de nuvem da Microsoft. Ajustar Pontuação é atualizado trimestral. | 
| AzureIntent | Os sinais relacionados à mídia social e ao comportamento online de um cliente definem a intenção. A pontuação da intenção é sobreposta em ajustar para definir os clusters. A pontuação da intenção é atualizada mensalmente. | 
| AzureCluster | Identifica as propensações do cliente para comprar o Azure, consolidando as recomendações de ajuste e de intenção em um cluster. Direcione o Act agora e avalie os clusters, pois eles produzirão mais rendimento. Direcione o incentivá e instrua os clientes somente se ainda houver capacidade depois de você direcionar o Act agora e avaliar os clientes. | 
| WindowsServerDataCenter_HasOpenRenewal | identifica se o cliente tem uma renovação aberta para datacenter do Windows Server | 
| WindowsServerStandard_HasOpenRenewal | identifica se o cliente tem uma renovação aberta para o Windows Server Standard | 
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
| Vertical | A vertical do cliente que está sendo pontuada pela propensão, conforme identificado pela Microsoft, D&B e outros padrões do setor | 
| Área | Área geográfica do local | 
| Subsidiária | A subsidiária do cliente que está sendo pontuada quanto à propensão | 
| Território de Vendas | A região de vendas do cliente que está sendo pontuada quanto à propensão | 
| City | Local da cidade geográfica | 
| Estado | Local do estado geográfico | 
| Código postal | Código postal da organização | 
| País | Localização geográfica do país | 
| Segment | Segmento de mercado | 
| Subsegmento | Subsegmento de mercado | 
| Resumo do tipo SMC | Tipo do SMC | 
| Superior não gerenciado-base de computação | Principais clientes não gerenciados – computação | 
| Principal base de usuários não gerenciados | Principais clientes não gerenciados – usuários | 
| IsNonProfit | Indica se a organização é sem fins lucrativos (Sim ou Não) | 
| Tem o Google | Identifica se o cliente mostra sinais competitivos para a propriedade de produtos AWS | 
| Tem AWS | Identifica se o cliente mostra sinais competitivos para a propriedade de produtos AWS | 
| Azure Cluster | Identifica a propensão do cliente para comprar o Azure. Ação de Destino Agora e Avaliar clusters, pois eles produzirão um rendimento mais alto. Direcionar e instruir os clientes somente se ainda houver capacidade depois que você direcionar Agir agora e Avaliar clientes. | 
| D365 Finance + Operations Cluster | Identifica a propensão do cliente para comprar o Dynamics 365 Finance and Operations. Os clientes que mostram uma propensão para Finanças + Operações estarão nas principais categorias não realizadas. Ação de Destino Agora e Avaliar clusters, pois eles produzirão um rendimento mais alto. Direcionar e instruir os clientes somente se ainda houver capacidade depois que você direcionar Agir agora e Avaliar clientes. | 
| D365 CE Cluster | Identifica a propensão do cliente para comprar o Dynamics 365 Customer Engagement. Os clientes que mostram uma propensão para o Customer Engagement estarão nas categorias Média e Pequena. Ação de Destino Agora e Avaliar clusters, pois eles produzirão um rendimento mais alto. Direcionar e instruir os clientes somente se ainda houver capacidade depois que você direcionar Agir agora e Avaliar clientes. | 
| D365 BC Cluster | Identifica a propensão do cliente para comprar o Dynamics 365 Business Central. Os clientes que mostram uma propensão para o Business Central estarão nas categorias Média e Pequena. Ação de Destino Agora e Avaliar clusters, pois eles produzirão um rendimento mais alto. Direcionar e instruir os clientes somente se ainda houver capacidade depois que você direcionar Agir agora e Avaliar clientes. | 
| Microsoft 365 Cluster | Identifica a propensão do cliente para comprar Microsoft 365. Ação de Destino Agora e Avaliar clusters, pois eles produzirão um rendimento mais alto. Direcionar e instruir os clientes somente se ainda houver capacidade depois que você direcionar Agir agora e Avaliar clientes. | 
| Programa de licença | Identifica o tipo de programa de licença para a renovação | 
| ID do contrato | Identificador do contrato | 
| Data de término do contrato | Data de término do contrato | 
| Tipo de Expiração | Tipo de expiração | 
| Expirando receita | Receita associada a assinaturas de expiração | 
| Tem EA | Identifica se uma renovação é um EA ou uma assinatura do EA | 
| Tem Aberto | Identifica se uma renovação é um contrato Open ou Open Value | 
| Cliente do Azure Upsell | Identifica se o cliente mostra a propensão de venda para o Azure | 
| Microsoft 365 Cliente de upsell | Identifica se o cliente mostra a propensão de venda para Microsoft 365 | 
| RevSumDivisionName | Identifica o produto que está para renovação | 

## <a name="next-steps"></a>Próximas etapas

Para obter mais informações, consulte [Baixar relatórios](insights-download-reports.md).
