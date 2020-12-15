---
title: Definições de dados do insights
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: O documento fornece a lista de vários relatórios e as definições de dados de cada relatório, que podem ser baixados na página de relatório de download do insights.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d4a805957fac7c7cff373d807347b7c6d0b13d6f
ms.sourcegitcommit: 4e36d1a4ca2f074b55f9b9a08e300734eae1f06d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2020
ms.locfileid: "97501741"
---
# <a name="export--data-definitions"></a>Exportar – definições de dados 

 **Funções apropriadas** 

- Visualizador de relatórios 
- Visualizador de relatórios executivos 

## <a name="introduction"></a>Introdução 

O Hub baixar relatórios no painel do insights permite que você exporte os conjuntos de dados brutos.  

Os vários relatórios, que podem ser baixados junto com a definição de dados, são os seguintes: 

**Perfil de parceiro**: as definições de dados dos vários campos do relatório de perfil são: 


| **Nome da Coluna** | **Descrição de dados** |
|---------|:---------|
|MPNId|ID de Microsoft Partner Network|
|PartnerName|Nome do parceiro |
|PGA_MPNId|ID de MPN da conta global do parceiro|
|PGA_PartnerName|Nome da conta global do parceiro|
|City|Local da cidade do parceiro |
|País|Local do país do parceiro |
|HierarchyLevel|Indica se é uma ID de MPN global ou uma ID de MPN de local|

**Detalhes do cliente**: as definições de dados dos vários campos do relatório detalhes do cliente são:

| **Nome da Coluna** | **Descrição de dados** |
|---------|:---------|
|CustomerName|Nome do cliente |
|CustomerTenantId|ID de locatário do cliente |
|CustomerTpid|Identificador pai superior do cliente |
|CustomerSegment|Segmento de cliente |
|CustomerMarket|Mercado geográfico do cliente  |
|CustomerStatus|Status do cliente (Active/Inactive) |
|Produto|O produto vendido ao cliente pelo MPN. Este será um dos O365, D365, Enterprise Mobility, Power BI Microsoft Azure.|
|SKU|   SKU do Produto|
|Mês| Mês para o qual o uso e a receita são relatados|
|MPNId| ID de Microsoft Partner Network|
|PartnerName|   Nome do parceiro|
|PartnerLocation|   Localização geográfica do parceiro|
|PartnerAttributionType|    Tipo de atribuição de parceiro|
|SalesChannel|  Canal de vendas|
|AvailableSeats|    Estações disponíveis| 
|RevenueUSD|    Receita em USD|

**Desempenho do revendedor**: as definições de dados dos vários campos dos relatórios de desempenho do revendedor são:

> [!Note]
> Os dados de receita e ACR só estão disponíveis para usuários que são visualizadores de relatórios executivos.

| **Nome da Coluna** | **Descrição de dados** |
|---------|:---------|
|ResellerMpnid|Identificador de Microsoft Partner Network do revendedor| 
|ResellerName|Nome do revendedor|
|ResellerMarket|País do revendedor do mercado| 
|IndirectProviderMPNId|Identificador de Microsoft Partner Network de provedor indireto|
|IndirectProviderName|Nome do provedor indireto|
|Mês|Mês para o qual o uso e a receita são relatados|
|Produto|Nome do Produto|
|SubscriptionID|Identificador de assinatura|
|AvailableSeats|Número de estações disponíveis|
|AssignedSeats|Número de estações atribuídas|
|BilledRevenueUSD|Receita cobrada (em $)|
|CustomerName|Nome do cliente| 
|CustomerTPid|Identificador pai superior do cliente| 
|CustomerSegment|Segmento de cliente |
|CustomerMarket|Mercado geográfico do cliente |
|ResellerStatus|Status do revendedor| 

**Detalhes de assinaturas**: as definições de dados dos vários campos do relatório detalhes da assinatura são:

>[!Note]
>Os dados de receita e ACR só estão disponíveis para usuários que são visualizadores de relatórios executivos

| **Nome da Coluna** | **Descrição de dados** |
|---------|:---------|
|SubscriptionId|    GUID da assinatura|
|SubscriptionStartDate| Data de início da assinatura|
|SubscriptionEndDate|   Data de término da assinatura|
|SubscriptionState| Estado da assinatura (ativa ou com variação)|
|Mês| Mês para o qual o uso e a receita são relatados|
|IsAutoRenew|   Indica se a assinatura é renovada automaticamente ou não (s/N)|
|CustomerName|  Nome do Cliente| 
|CustomerTenantId|  GUID do cliente|
|CustomerTpid|  Identificador pai superior do cliente| 
|CustomerSegment|   Segmento de mercado do cliente| 
|CustomerMarket|    Mercado geográfico do cliente|
|Produto|   Produto vendido ao cliente pelo parceiro| 
|SKU|   SKU do produto |
|MPNId| ID de Microsoft Partner Network do parceiro |
|PartnerName|   Nome do parceiro |
|PartnerLocation|   Localização geográfica do parceiro |
|PartnerAttributionType|    Tipo de atribuição para a assinatura|
|SalesChannel|  Canal das vendas (direto/CSP, etc.) |
|AvailableSeats|    Estação disponível atual|
|RevenueUSD|    Receita em USD|
|ID de registro| ID de registro da assinatura|

**Uso do Azure**: as definições de dados dos vários campos do relatório de uso do Azure são:

| **Nome da Coluna** | **Descrição de dados** |
|---------|:---------|
|SubscriptionId|    GUID da assinatura|
|SubscriptionStartDate| A data do início da assinatura.|
|SubscriptionEndDate|   A data em que a assinatura termina.|
|SubscriptionState| Estado atual da assinatura (aberto/fechado/ativo/período de incarência)|
|Mês| Data agregada por mês |
|ServiceName|   Nome do serviço do Azure|
|MeterCategory| Nome da categoria do medidor|
|UsageUnits|    O número de unidades usadas durante o ciclo de cobrança |
|CustomerName|  Nome do cliente |
|CustomerTenantId|  ID do locatário do cliente |
|CustomerTpid|  ID pai superior do cliente |
|CustomerSegment|   Segmento do cliente |
|CustomerMarket|    Mercado geográfico do cliente |
|MPNId  |ID de Microsoft Partner Network do cliente |
|PartnerName|   Nome do parceiro |
|PartnerLocation    |Localização geográfica do país do parceiro |
|PartnerAttributionType |Tipo de atribuição de parceiro|
|SalesChannel|  Canal das vendas (direto/CSP direto/CSP direta, etc.) |
|ACR_USD|   Receita consumida pelo Azure em USD|
|ID de registro| ID de registro da assinatura do Azure|

**Office 365-uso de licença**: as definições de dados dos vários campos do relatório de uso de licença do Office 365 são:

| **Nome da Coluna** | **Descrição de dados** |
|---------|:---------|
|CustomerTenantId|  ID do locatário do cliente| 
|CustomerTpid|  ID pai superior do cliente |
|Carga de trabalho|  SFB, equipes, EXO |
|Mês| Mês para o qual o uso é relatado|
|PaidAvailableUnits|    Número de unidades pagas disponíveis|
|MonthlyActiveUsers|    Número de usuários ativos mensais|
|CustomerName|  Nome do cliente|
|CustomerMarket|    Localização geográfica do país do mercado do cliente |
|CustomerSegment|   Segmento de cliente |
|MPNId| ID de Microsoft Partner Network|
|PartnerName|   Nome do parceiro|
|PartnerLocation|   Localização geográfica do parceiro|
|PartnerAttributionType|    Tipo de atribuição de parceiro|

**Enterprise Mobility – uso de licença**: a definição de dados dos vários campos do EMS – relatório de uso de licença são:

| **Nome da Coluna** | **Descrição de dados** |
|---------|:---------|
|CustomerTenantId|  ID do locatário do cliente| 
|CustomerTpid|  ID pai superior do cliente |
|Carga de trabalho|  Nome da carga de trabalho do EMS |
|Mês| Mês para o qual o uso é relatado|
|PaidAvailableUnits|    Número de unidades pagas disponíveis|
|MonthlyActiveUsers|    Número de usuários ativos mensais|
|CustomerName|  Nome do cliente|
|CustomerMarket|Localização geográfica do país do mercado do cliente |
|CustomerSegment|   Segmento de cliente |
|MPNId| ID de Microsoft Partner Network|
|PartnerName|   Nome do parceiro|
|PartnerLocation|   Localização geográfica do parceiro|
|PartnerAttributionType|    Tipo de atribuição de parceiro|

**Dynamics 365 – uso de licença**: a definição de dados dos vários campos do relatório de uso da licença Dynamics 365 – é:

| **Nome da Coluna** | **Descrição de dados** |
|---------|:---------|
|SubscriptionId|GUID da assinatura|
|SubscriptionStartDate| Data de início da assinatura|
|SubscriptionEndDate|   Data de término da assinatura|
|SubscriptionStatus|    Estado da assinatura |
|Mês| Mês para o qual o uso é relatado|
|RevSumDivisionName|    Nome da divisão da soma da revisão|
|RevSumCategoryName|    Nome da categoria da soma da revisão|
|SKU|   SKU do produto |
|SKUId| ID do SKU do produto |
|FreeVsPaidSKU| Indica se é um SKU gratuito ou pago |
|SalesModel|    Canal de vendas usado para vender a assinatura|
|DetailedSalesModel|    Modelo de vendas detalhado para a assinatura|
|CustomerName|  Nome do Cliente |
|CustomerTenantId|  GUID de locatário do cliente |
|CustomerTpid|  Identificador pai superior do cliente |
|CustomerSegment|   Segmento de mercado do cliente |
|CustomerMarket|    Mercado geográfico do cliente |
|MPNId| ID da Microsoft Partner Network |
|PartnerName|   Nome do parceiro |
|PartnerLocation|   Localização geográfica do país do parceiro |
|PartnerAttachType| Tipo de atribuição para a assinatura|
|AvailableSeats|    Estação disponível atual|
|AssignedSeats| Estação atribuída atual |
|ActiveSeats|   Estações ativas atuais |
|DeploymentOpportunity| Oportunidade de implantação atual|
|ActiveUsagePercent|    Porcentagem de uso ativo atual|
 
**Power bi uso da licença**: a definição de dados dos vários campos do relatório de uso Power bi – licença são:

| **Nome da Coluna** | **Descrição de dados** |
|---------|:---------|
|SubscriptionId|    GUID da assinatura|
|SubscriptionStartDate| Data de início da assinatura|
|SubscriptionEndDate|   Data de término da assinatura|
|SubscriptionStatus|    Estado da assinatura (ativo ou In-Active ou período de cortesia)|
|Mês| Data agregada por mês |
|SKU|   SKU do produto |
|SKUId| ID do SKU do produto |
|FreeVsPaidSKU| Diferenciador de SKU gratuito ou pago |
|SalesModel|    Modelo de vendas usado para vender a assinatura|
|DetailedSalesModel|    Modelo de vendas detalhado para a assinatura|
|CustomerName|  Nome do Cliente |
|CustomerTenantId|  GUID de locatário do cliente |
|CustomerTpid|  Identificador pai superior do cliente| 
|CustomerSegment|   Segmento de mercado do cliente |
|CustomerMarket|    Mercado geográfico do cliente |
|MPNId| ID de Microsoft Partner Network |
|PartnerName|   Nome do parceiro |
|PartnerLocation|   Localização geográfica do país do parceiro |
|PartnerAttachType| Tipo de atribuição para a assinatura|
|AvailableSeats|    Estações disponíveis atuais|
|AssignedSeats| Estações atribuídas atuais|
|ActiveSeats|   Estações ativas atuais|
|DeploymentOpportunity| Oportunidade de implantação atual|
|ActiveUsagePercent|    Porcentagem de uso ativo atual|

**Uso de equipes – reuniões e chamadas**: as definições de dados dos vários campos são:

| **Nome da Coluna** | **Descrição de dados** |
|---------|:---------|
|CustomerTenantId|  ID do locatário do cliente |
|CustomerTpid|  ID pai superior do cliente |
|Mês| Mês para o qual o uso é relatado|
|Subcarga de trabalho|   Subcarga de trabalho para a qual o uso é relatado (reuniões, chamadas, sistemas de telefone)|
|Contagem de reuniões| Número de reuniões|
|Duração da reunião|  Duração total da reunião em horas|

**Equipes-detalhes de uso mensal**: as definições de dados dos vários campos são:

| **Nome da Coluna** | **Descrição de dados** |
|---------|:---------|
|CustomerTenantId|  ID do locatário do cliente |
|CustomerTpid|  ID pai superior do cliente |
|Mês| Mês para o qual o uso é relatado|
|Subcarga de trabalho|   Subcarga de trabalho para a qual o uso é relatado (reuniões, chamadas, sistemas de telefone)|
|Usuários da área de trabalho| Número de usuários usando equipes no desktop|
|Usuários Móveis|  Número de usuários usando equipes em dispositivos móveis|
|Usuários da Web| Número de usuários usando equipes na Web|
|AllUpParticipants| Número de usuários distintos de equipes para o mês|

**Uso de equipes – aplicativos 3P**: as definições de dados dos vários campos são:

| **Nome da Coluna** | **Descrição de dados** |
|---------|:---------|
|CustomerTenantId|  ID do locatário do cliente| 
|CustomerTpid|  ID pai superior do cliente |
|Mês| Mês para o qual o uso é relatado|
|Nome do aplicativo 3P|   Nome do aplicativo de equipes|
|Contagem de usuários|    Número de usuários para o aplicativo|


**Detalhes de treinamento**: as definições de dados dos vários campos do relatório detalhes de treinamento são:

| **Nome da Coluna** | **Descrição de dados** |
|---------|:---------|
|TrainingActivityId|    Identificador do treinamento |
|TrainingTitle| Título do treinamento |
|Traintype|  Tipo de treinamento (certificação/exame)|
|IndividualFirstName|   Nome do cliente| 
|IndividualLastName|    Sobrenome do cliente| 
|Email| ID de email pessoal do cliente|
|CorpEmail| ID de email do Office do cliente|
|TrainingCompletionDate|    Data de conclusão do treinamento |
|Mês| Mês para o qual os dados são relatados|
|IcMCP| Indica se o usuário é um Microsoft Certified Professional|
|MCPID| ID do MCP do usuário|
|MPNId| ID de Microsoft Partner Network |
|PartnerName|   Nome do parceiro |
|PartnerCityLocation|   Local da cidade geográfica do parceiro |
|PartnerCountryLocation|    Localização geográfica do país do parceiro |

**Microsoft Learn**: as definições de dados dos vários campos do relatório de Microsoft Learn são:

| **Nome da Coluna** | **Descrição de dados** |
|---------|:---------|
|UserName|Nome do usuário| 
|UserId|GUID do usuário |
|Trainname|Nome do treinamento |
|Traintype|Tipo de treinamento (caminho/Learning do módulo)|
|Produtos|Produto ao qual o módulo de aprendizagem é aplicável|
|Funções|Funções aplicáveis do treinamento |
|CompletionDate|Data da conclusão do treinamento |
|MPNId|ID de Microsoft Partner Network |
|PartnerName|Nome do parceiro |
|País|Localização geográfica do país do parceiro |

**Resumo de competência e histórico**: a definição de dados dos vários campos do relatório de Resumo de competência e histórico é:

| **Nome da Coluna** | **Descrição de dados** |
|---------|:---------|
|Competêncianame|Nome da competência |
|CompetencyLevel|Nível de competência (ouro/Silver)|
|CompetencyStatus|Status atual de competência (ativo/inativo/em período de carência)|
|CompetencyStartDate|Data de início de determinada competência| 
|CompetencyEndDate|Data de término de determinada competência |

**Desempenho de competência**: as definições de dados dos vários campos do relatório de desempenho de competência são:

| **Nome da Coluna** | **Descrição de dados** |
|---------|:---------|
|Competêncianame|    Nome da competência |
|CompetencyAttainmentOptionName|    Nome da opção de obtenção de competência|
|Mês| Mês para o qual as métricas são relatadas|
|MetricName|    Nome da métrica relevante para a competência|
|MetricMonthlyContribution| Contribuição mensal da métrica|
|TTMAggregate|  Métrica agregada para os 12 meses à direita|
|AnniversaryYearAggregate|  Métrica agregada para o ano de aniversário atual|
|GoldThreshold| Requisito de desempenho para atender à competência ouro|
|SilverThreshold|   Requisito de desempenho para atender à competência prateada|

Propensão **M365 da nuvem**: as definições de dados dos vários campos do relatório de propensão do Cloud ascendente M365 são:

| **Nome da Coluna** | **Descrição de dados** |
|---------|:---------|
|ID MPN|    ID de Microsoft Partner Network|
|Nome do parceiro|  Nome do parceiro|
|ID do Cliente|   Número do identificador do cliente |
|Número de DUNS|   O Dun & Bradstreet número do cliente que está sendo pontuado quanto à propensão|
|Nome da Conta|  Nome da conta |
|Domínio|    Domínio da conta|
|Tamanho da organização|  Tamanho da organização|
|Setor|  Setor  |
|Vertical|  A vertical do cliente que está sendo pontuado pela propensão, conforme identificado pela Microsoft e por outros padrões do setor (D&B)|
|Área|  Área geográfica do local|
|Subsidiária|    A subsidiária do cliente que está sendo classificada quanto à propensão|
|Território de Vendas|   A região de vendas do cliente que está sendo classificada quanto à propensão|
|City|  Local da cidade geográfica |
|Estado| Local do estado geográfico|
|Código postal|   Código postal|
|País|   Localização geográfica do país |
|Segment|   Segmento de mercado |
|Subsegmento|   Subsegmento de mercado |
|Resumo do tipo SMC|  Tipo do SMC |
|Superior não gerenciado-base de computação|  Principais clientes não gerenciados – computação|
|Principal base de usuários não gerenciados| Principais clientes não gerenciados – usuário|
|IsNonProfit|   Se não há lucro ou lucro (Sim/não)|
|Habilitar o Exchange Online de destino de trabalho remoto|   Clientes que têm uma assinatura ativa do Exchange Online, que se revendam a M365|
|Habilitar a aquisição remota de trabalho local (versão atual) com o CLAS propensation-+ 10 licenças|Cliente que tem o atual escritório local ou cliente do Win (ou seja, versões que são posteriores a produtos EOS). O cliente tem 10 ou mais licenças. Cliente que tem uma pontuação de propensação. Os parceiros devem ter como destino a conversão em M365.|
|Habilitar a aquisição remota de trabalho local (versão atual) com a CLAS propensation-<10 licenças|Cliente que tem o atual escritório local ou cliente do Win (ou seja, versões que são posteriores a produtos EOS). O cliente tem menos de 10 licenças. Cliente que tem uma pontuação de propensação. Os parceiros devem ter como destino a conversão em M365.|
|Habilitar a aquisição remota de trabalho local (versão atual) sem a CLAS propensation-+ 10 licenças| Cliente que tem o atual escritório local ou cliente do Win (ou seja, versões que são posteriores a produtos EOS). O cliente tem 10 ou mais licenças. O cliente não tem uma pontuação de propensação. Os parceiros devem ter como destino a conversão em M365.|
|Habilitar a aquisição remota de trabalho local (versão atual) sem a CLAS propensation-<10 licenças| Cliente que tem o atual escritório local ou cliente do Win (ou seja, versões que são posteriores a produtos EOS). O cliente tem menos de 10 licenças. O cliente não tem uma pontuação de propensação. Os parceiros devem ter como destino a conversão em M365.|
|Habilitar o EOS (aquisição remota de trabalho local) com CLAS propensation-+ 10 licenças|Cliente que tem um EOS local ou cliente de vitória (ou seja, versões anteriores a e incluindo produtos EOS. O cliente tem 10 ou mais licenças. O cliente tem uma pontuação de propensação. Os parceiros devem ter como destino a conversão em M365.|
|Habilitar o EOS (aquisição remota de trabalho local) com CLAS propensation-<10 licenças|Cliente que tem um EOS local ou cliente de vitória (ou seja, versões anteriores a e incluindo produtos EOS. O cliente tem menos de 10 licenças. O cliente tem uma pontuação de propensação. Os parceiros devem ter como destino a conversão em M365.|
|Habilitar o EOS (aquisição local remota) sem a CLAS da propensão-+ 10 licenças| Cliente que tem o atual escritório local ou cliente do Win (ou seja, versões anteriores a e incluindo produtos EOS). O cliente tem 10 ou mais licenças. O cliente não tem uma pontuação de propensação. Os parceiros devem ter como destino a conversão em M365.|
|Habilitar o EOS (aquisição local remota) sem a CLASção da propensão-<10 licenças| Cliente que tem o atual escritório local ou cliente do Win (ou seja, versões anteriores a e incluindo produtos EOS). O cliente tem menos de 10 licenças. O cliente não tem uma pontuação de propensação. Os parceiros devem ter como destino a conversão em M365.|
|Habilitar o cliente em potencial de propensão de trabalho remoto-alta para M365 (agir agora/avaliar)| Cliente cliente potencial com alta propensão para M365.|
|Habilitar trabalho remoto – competição (zoom) com M365| Clientes com zoom e M365, destino para conversão para equipes|
|Habilitar trabalho remoto – competição (zoom) sem M365|  Clientes com zoom, destino para conversão para equipes|
|Reduzir o custo e gerenciar o M365 E3 direcionado para M365 e5| Cliente existente com M365 E3, alvo para M365 e5|
|Reduzir custos e gerenciar-M365 BB e clientes de BS destinados a M365 BP|    Clientes M365 BB e BS existentes, direcione-os para M365 BP|
|Transformar a produtividade organizacional – propensação da superfície|    O cliente está mostrando a propensão para a superfície.|
|M365Cluster|Identifica as propensações do cliente para comprar o M365.  Os clusters atuam agora e avaliados devem ser direcionados, pois produzirão um rendimento maior.  Incentivá e instrua os clientes só devem ser direcionados se ainda houver capacidade depois de direcionar o Act agora e avaliar os clientes.|
|M365Fit|   Pontos de dados internos e externos que definem firmographics. Ajustar a pontuação usa um modelo semelhante ao nosso melhor SMB para comparar os clientes e ver se eles são um ajuste potencial para Microsoft Cloud produtos. Ajustar Pontuação é atualizado trimestral.|
|M365Intent|    Os sinais relacionados à mídia social e ao comportamento online de um cliente definem a intenção. A pontuação da intenção é sobreposta sobre ajustar para definir os clusters. A pontuação da intenção é atualizada mensalmente.|
|SurfaceCluster|    Isso identifica a propensão do cliente para comprar a superfície ao consolidar as recomendações de ajuste e de intenção em um cluster.  Os clusters atuam agora e avaliados devem ser direcionados, pois produzirão um rendimento maior.  Incentivá e instrua os clientes só devem ser direcionados se ainda houver capacidade depois de direcionar o Act agora e avaliar os clientes.|
|SurfaceFit|    Pontos de dados internos e externos que definem firmographics. Ajustar a pontuação usa um modelo semelhante ao nosso melhor SMB para comparar os clientes e ver se eles são um ajuste potencial para Microsoft Cloud produtos. Ajustar Pontuação é atualizado trimestral.|
|SurfaceIntent| Os sinais relacionados à mídia social e ao comportamento online de um cliente definem a intenção. A pontuação da intenção é sobreposta sobre ajustar para definir os clusters. A pontuação da intenção é atualizada mensalmente.|
|O365Cluster|   Isso identifica as propensações do cliente para comprar o O365.  Os clusters atuam agora e avaliados devem ser direcionados, pois produzirão um rendimento maior.  Incentivá e instrua os clientes só devem ser direcionados se ainda houver capacidade depois de direcionar o Act agora e avaliar os clientes.|
|O365Fit|   Pontos de dados internos e externos que definem firmographics. Ajustar a pontuação usa um modelo semelhante ao nosso melhor SMB para comparar os clientes e ver se eles são um ajuste potencial para Microsoft Cloud produtos. Ajustar Pontuação é atualizado trimestral.|
|O365Intent|    Os sinais relacionados à mídia social e ao comportamento online de um cliente definem a intenção. A pontuação da intenção é sobreposta sobre ajustar para definir os clusters. A pontuação da intenção é atualizada mensalmente.|
|M365UpsellCustomer|    Isso identifica se o cliente está mostrando a propensão de venda para M365|
|Tem Google|    Esse sinalizador identifica se um cliente está mostrando sinais competitivos para produtos pertencentes ao Google|
|Tem AWS|   Esse sinalizador identifica se um cliente está mostrando sinais competitivos para produtos de AWS de propriedade|
|Tem EA|    Isso identifica se uma renovação é um EA (Enterprise Agreement) ou uma assinatura EA|
|Está aberto|  Isso identifica se uma renovação é um contrato aberto ou um valor aberto|

Propensão **D365 da nuvem**: as definições de dados dos vários campos do relatório de propensão do Cloud ascendente D365 são:

| **Nome da Coluna** | **Descrição de dados** |
|---------|:---------|
|ID MPN|    ID de Microsoft Partner Network|
|Nome do parceiro|  Nome do parceiro|
|ID do Cliente|   Número do identificador do cliente |
|Número de DUNS|   O Dun & Bradstreet número do cliente que está sendo pontuado quanto à propensão|
|Nome da Conta|  Nome da conta |
|Domínio|    Domínio da conta|
|Tamanho da organização|  Tamanho da organização|
|Setor|  Setor  |
|Vertical|  A vertical do cliente que está sendo pontuado pela propensão, conforme identificado pela Microsoft e por outros padrões do setor (D&B)
|Área|  Área geográfica do local|
|Subsidiária|    A subsidiária do cliente que está sendo classificada quanto à propensão|
|Território de Vendas|   Território de Vendas|
|City|  Local da cidade geográfica |
|Estado| Local do estado geográfico|
|Código postal|   Código postal|
|País|   Localização geográfica do país |
|Segment|   Segmento de mercado |
|Subsegmento|   Subsegmento de mercado |
|Resumo do tipo SMC|  A categorização de um cliente: as principais bases de usuários não gerenciadas são clientes com mais de 300 funcionários, a principal base de computação não gerenciada são clientes com US $10 mil no Azure de três anos em potencial, empresas de médio porte são clientes com 25 funcionários ou mais, pequenas empresas são clientes com menos de 25 funcionários|
|Superior não gerenciado-base de computação   |Principais clientes não gerenciados – computação|
|Principal base de usuários não gerenciados| Principais clientes não gerenciados – usuários|
|IsNonProfit|   Se não há lucro ou lucro (Sim/não)|
|Ativar vendas digitais – tamanho do M365-assento >= 25 estações (modelo de propensão SalesPro)|   Cliente sem D365. Tamanho do assento: 25 +. Os parceiros devem visar a venda cruzada de D365 Salespro|
|Ativar vendas digitais-D365 SalesPro propensation (Act Now/Evaluate) |Clientes com alta propensão, sem D365.  Os parceiros devem ter como alvo D365 SalesPro.|
|Gerenciando o risco financeiro & fraude-a instalação local do Dynamics-Navision (modelo de propensação de BC)|Cliente existente com o onlocal Navision.  O parceiro deve ter como alvo D365 BC|
|Gerenciamento de riscos financeiros & fraude-a instalação local do Dynamics base-AX (modelo de propensão & F&O)    |Cliente existente com AX local.  O parceiro deve ser direcionado para D365 F&O|
|Gerenciamento de riscos financeiros & fraude-base de instalação local do Dynamics – Great Plains (modelo de propensão de BC)|  Cliente existente com grande custo local.  O parceiro deve ter como alvo D365 BC|
|Gerenciando o risco financeiro & fraude-base de instalação local do Dynamics-Solomon (modelo de propensão de BC)|Cliente existente com Solomon local.  O parceiro deve ter como alvo D365 BC|
|Gerenciando o risco financeiro & fraude – base de instalação do Dynamics local-outros (modelo de propensão de BC) |Cliente existente com outras soluções locais não listadas acima.  O parceiro deve ter como alvo D365 BC|
|Criar processos de negócios ágeis-base de instalação do Dynamics local-AX/GP/SL/NAV/Other (modelo de D365 propensation)|   Criar processos de negócios ágeis-base de instalação do Dynamics local-AX/GP/SL/NAV/Other (modelo de D365 propensation)|
|Criar processos de negócios ágeis-base de concorrência do Dynamics-Mendix/outsubsystems/Salesforce (modelo de D365 propensation)| Criar processos de negócios ágeis-base de concorrência do Dynamics-Mendix/outsubsystems/Salesforce (modelo de D365 propensation)|
|Criar processos de negócios ágeis-base de instalação do D365 F&O |Clientes D365 F&O existentes.  Parceiro para direcionar os aplicativos de energia.|
|Criar processos de negócios ágeis-base de instalação do D365 BC| Clientes D365 BC existentes. Parceiro para direcionar os aplicativos de energia.|
|Criar processos de negócios ágeis-base de instalação do D365 CE| Clientes D365 CE existentes. Parceiro para direcionar os aplicativos de energia.|
|Crie uma cadeia de suprimentos resiliente – vença e ative a primeira carga de trabalho D365 como cadeia de fornecimento D365 com clientes não Oracle/SAP ERP|  Direcionar clientes para a cadeia de suprimentos D365.|
|Crie uma cadeia de suprimentos resiliente-venda cruzada D365 cadeia de suprimentos e/ou varejo/comércio para clientes existentes do D365 CE |Clientes D365 CE existentes a serem alvo de venda cruzada D365 cadeia de suprimentos|
|Crie uma cadeia de fornecimento resiliente – venda cruzada D365 sup. Cadeia e/ou varejo/comércio para D365 CE e (Oracle ou SAP)| Clientes D365 CE existentes com Oracle ou SAP para direcionar para a cadeia de suprimentos D365|
|D365BCCluster| Isso identifica a propensão do cliente para comprar o D365 Business central.  Os clientes que mostram a propensão para BC estarão nas categorias média e pequena.  Os clusters atuam agora e avaliados devem ser direcionados, pois produzirão um rendimento maior.  Incentivá e instrua os clientes só devem ser direcionados se ainda houver capacidade depois de direcionar o Act agora e avaliar os clientes.|
|D365BCFit| Pontos de dados internos e externos que definem firmographics. Ajustar a pontuação usa um modelo semelhante ao nosso melhor SMB para comparar os clientes e ver se eles são um ajuste potencial para Microsoft Cloud produtos. Ajustar Pontuação é atualizado trimestral.|
|D365BCIntent|  Os sinais relacionados à mídia social e ao comportamento online de um cliente definem a intenção. A pontuação da intenção é sobreposta sobre ajustar para definir os clusters. A pontuação da intenção é atualizada mensalmente.|
|D365FOCluster| Isso identifica a propensão do cliente para comprar operações e Finanças D365s.  Os clientes que mostrarem a propensão para O F&O estarão nas principais categorias não gerenciadas. Os clusters atuam agora e avaliados devem ser direcionados, pois produzirão um rendimento maior.  Incentivá e instrua os clientes só devem ser direcionados se ainda houver capacidade depois de direcionar o Act agora e avaliar os clientes.|
|D365FOFit| Pontos de dados internos e externos que definem firmographics. Ajustar a pontuação usa um modelo semelhante ao nosso melhor SMB para comparar os clientes e ver se eles são um ajuste potencial para Microsoft Cloud produtos. Ajustar Pontuação é atualizado trimestral.|
|D365FOIntent|  Os sinais relacionados à mídia social e ao comportamento online de um cliente definem a intenção. A pontuação da intenção é sobreposta sobre ajustar para definir os clusters. A pontuação da intenção é atualizada mensalmente.|
|D365CECluster| Isso identifica a propensão do cliente para comprar o engajamento do cliente D365.  Os clientes que mostram a propensão para CE estarão nas categorias média e pequena.  Os clusters atuam agora e avaliados devem ser direcionados, pois produzirão um rendimento maior.  Incentivá e instrua os clientes só devem ser direcionados se ainda houver capacidade depois de direcionar o Act agora e avaliar os clientes.|
|D365CEFit| Ajustar para D365 CE|
|D365CEIntent|  Intenção do D365 CE|
|DynamicsOnPremAXorCRM_HasOpenRenewal|  Isso identifica se um cliente tem uma renovação aberta para o Dynamics local ou o CRM.|
|M365UpsellCustomer|    Isso identifica se o cliente está mostrando a propensão de venda para M365|
|Tem Google|    Esse sinalizador identifica se um cliente está mostrando sinais competitivos para produtos pertencentes ao Google|
|Tem AWS|   Esse sinalizador identifica se um cliente está mostrando sinais competitivos para produtos de AWS de propriedade|
|Tem EA |Isso identifica se uma renovação é um EA (Enterprise Agreement) ou uma assinatura EA|
|Está aberto|  Isso identifica se uma renovação é um contrato aberto ou um valor aberto|

**Propensabilidade de Ascent-Azure de nuvem**: as definições de dados dos vários campos do relatório de propensão Ascent-Azure de nuvem são:

|**Nome da Coluna** |**Descrição de dados** |
|---------|:---------|
|ID MPN|    ID de Microsoft Partner Network|
|Nome do parceiro|  Nome do parceiro|
|ID do Cliente|   Número do identificador do cliente |
|Número de DUNS|   O Dun & Bradstreet número do cliente que está sendo pontuado quanto à propensão|
|Nome da Conta|  Nome da conta |
|Domínio|    Domínio da conta|
|Tamanho da organização|  Tamanho da organização|
|Setor|  Setor  |
|Vertical|  A vertical do cliente que está sendo pontuado pela propensão, conforme identificado pela Microsoft e por outros padrões do setor (D&B)|
|Área|  Área geográfica do local|
|Subsidiária|    A subsidiária do cliente que está sendo classificada quanto à propensão|
|Território de Vendas|   Território de Vendas|
|City|  Local da cidade geográfica |
|Estado| Local do estado geográfico|
|Código postal|   Código postal|
|País|   Localização geográfica do país |
|Segment|   Segmento de mercado |
|Subsegmento|   Subsegmento de mercado |
|Resumo do tipo SMC|  Tipo do SMC |
|Superior não gerenciado-base de computação|  Principais clientes não gerenciados – computação|
|Principal base de usuários não gerenciados| Principais clientes não gerenciados – usuários|
|IsNonProfit|   Se não há lucro ou lucro (Sim/não)|
|Migrate-EOS Win Server-EOS Windows Server IB com CLAS propensation-5 + licenças|   Cliente que tem um servidor de vitória local EOS (ou seja, versões anteriores a e incluindo produtos EOS). O cliente tem 5 ou mais licenças. Cliente que tem uma pontuação de propensação.  Os parceiros devem direcionar esses clientes para a migração para o Azure.|
|Migration-EOS Win Server-EOS Windows Server IB com CLAS propensation-<5 licenças|   Cliente que tem EOS (fim do serviço) servidor de vitória local (ou seja, versões anteriores a e incluindo produtos EOS). O cliente tem menos de 5 licenças. Cliente que tem uma pontuação de propensação.  Os parceiros devem direcionar esses clientes para a migração para o Azure.|
|Migrate-EOS Win Server-EOS Windows Server IB sem CLAS propensation-5 + licenças |Cliente que tem um servidor de vitória local EOS (ou seja, versões anteriores a e incluindo produtos EOS). O cliente tem mais de 5 licenças. O cliente não tem uma pontuação de propensação. Os parceiros devem direcionar esses clientes para a migração para o Azure.|
|Migration-EOS Win Server-EOS Windows Server IB sem CLAS propensation-<5 licenças|    Cliente que tem um servidor de vitória local EOS (ou seja, versões anteriores a e incluindo produtos EOS). Tem menos de 5 licenças. O cliente não tem uma pontuação de propensação. Os parceiros devem direcionar esses clientes para a migração para o Azure.|
|Migration-EOS SQL-EOS SQL Server IB com CLAS propensation-5 + licenças|  Cliente que tem EOS SQL Server local (ou seja, versões anteriores a e incluindo produtos EOS). O cliente tem mais de 5 licenças. O cliente tem uma pontuação de propensação.  Os parceiros devem direcionar esses clientes para a migração para o Azure.|
|Migration-EOS SQL-EOS SQL Server IB com CLAS propensation-<5 licenças|  Cliente que tem EOS SQL Server local (ou seja, versões anteriores a e incluindo produtos EOS). Tem menos de 5 licenças. Cliente que tem uma pontuação de propensação. Os parceiros devem direcionar esses clientes para a migração para o Azure.|
|Migration-EOS SQL-EOS SQL Server IB sem a CLAS propensation-5 + licenças|   Cliente que tem EOS SQL Server local (ou seja, versões anteriores a e incluindo produtos EOS). O cliente tem 5 ou mais licenças. O cliente não tem uma pontuação de propensação. Os parceiros devem direcionar esses clientes para a migração para o Azure.|
|Migration-EOS SQL-EOS SQL Server IB sem a CLAS propensation-<5 licenças|   Cliente que tem EOS SQL Server local (ou seja, versões anteriores a e incluindo produtos EOS). O cliente tem menos de 5 licenças. O cliente não tem uma pontuação de propensação. Os parceiros devem direcionar esses clientes para a migração para o Azure.|
|Migrar – migrar o servidor win local-atual Windows Server IB com CLAS propensation-5 + licenças|   Cliente que tem o servidor win local atual (ou seja, versões que são posteriores a produtos EOS). O cliente tem mais de 5 licenças. O cliente tem uma pontuação de propensação. Os parceiros devem direcionar esses clientes para a migração para o Azure.|
|Migrar – migrar o servidor win local – licenças atuais do Windows Server IB com CLAS propensation-<5|   Cliente que tem o servidor win local atual (ou seja, versões que são posteriores a produtos EOS). O cliente tem menos de 5 licenças. O cliente tem uma pontuação de propensação para o Azure. Os parceiros devem direcionar esses clientes para a migração para o Azure.|
|Migrar – migrar o servidor win local-Server Server IB atual sem a CLAS propensation-5 + licenças|    Cliente que tem o servidor win local atual (ou seja, versões que são posteriores a produtos EOS). O cliente tem mais de 5 licenças. O cliente não tem uma pontuação de propensação. Os parceiros devem direcionar esses clientes para a migração para o Azure.|
|Migrar – migrar o servidor win local – Windows Server IB atual sem a CLAS propensation-<5 licenças |Cliente que tem o servidor win local atual (ou seja, versões que são posteriores a produtos EOS). O cliente tem menos de 5 licenças. O cliente não tem uma pontuação de propensação. Os parceiros devem direcionar esses clientes para a migração para o Azure.|
|Migrar – migrar para VMs SQL ou SQL do Azure-atual SQL Server IB com CLAS propensation-5 + licenças|  Cliente que tem o SQL Server local atual (ou seja, versões que são posteriores a produtos EOS). O cliente tem mais de 5 licenças. O cliente tem uma pontuação de propensação. Os parceiros devem direcionar esses clientes para a migração para o Azure.|
|Migrar – migrar para VMs do SQL ou SQL do Azure-atual SQL Server IB com CLAS propensation-<5 licenças|  Cliente que tem o SQL Server local atual (ou seja, versões que são posteriores a produtos EOS). O cliente tem menos de 5 licenças. O cliente tem uma pontuação de propensação. Os parceiros devem direcionar esses clientes para a migração para o Azure.|
|Migrar – migrar para VMs do SQL ou SQL do Azure-atual SQL Server IB sem a CLAS propensation-5 + licenças|   Cliente que tem o SQL Server local atual (ou seja, versões que são posteriores a produtos EOS). O cliente tem mais de 5 licenças. O cliente não tem uma pontuação de propensação. Os parceiros devem direcionar esses clientes para a migração para o Azure.|
|Migrar – migrar para VMs do SQL ou SQL do Azure-atual SQL Server IB sem a propensão CLAS-<5 licenças|   Cliente que tem o SQL Server local atual (ou seja, versões que são posteriores a produtos EOS). O cliente tem menos de 5 licenças. O cliente não tem uma pontuação de propensação. Os parceiros devem direcionar esses clientes para a migração para o Azure.|
|Migrar-OSS-migrar para o BD OSS| Cliente existente com qualquer um dos seguintes produtos concorrentes: PostgreSQL, MySQL, MariaDB. Os parceiros devem direcionar esses clientes para a migração para o Azure.|
|Migrar-OSS-Linux no Azure |Cliente existente com o produto: Linux. Os parceiros devem direcionar esses clientes para a migração para o Azure.|
|Migrar-SAP-SAP no Azure|  Cliente existente com o produto: SAP. Os parceiros devem direcionar esses clientes para a migração para o Azure.|
|Migrar-WVD-RDS IB |Identifica os clientes com o Windows Serviços de Área de Trabalho Remota ativo. Os parceiros devem direcionar esses clientes para a migração para o Azure.|
|Migrar-WVD-cross venda trabalho moderno para o Azure/WVD|   Identifica os clientes com o M365 e não tem o Azure. Os parceiros devem direcionar esses clientes para a migração para o Azure.|
|Migrar-VMware IB|   Cliente existente com o produto: VMware. Os parceiros devem direcionar esses clientes para a migração para o Azure.|
|Migrar – Citrix IB|   Cliente existente com o produto: Citrix Systems. Os parceiros devem direcionar esses clientes para a migração para o Azure.|
|Inovações-Analytics-Power BI IB w/high-interrupções do Azure|   Os clientes com a assinatura do e do Active Power BI, incluindo: Power BI-M365-autônomos pro, Power BI-conjuntos do Azure, conjuntos de Power BI-Office, pacotes de Power BI|
|Enable-DevOps com GitHub-VisualStudio/MSDN IB|    Clientes identificados com Visual estúdios ativo|
|Versão padrão do Win Server|   Isso mostra a versão do Windows Server Standard compras pelo cliente|
|Licença padrão do Win Server|   Isso mostra o tipo de licença do Windows Server Standard compras pelo cliente|
|Versão do Data Center do Win Server|    Isso mostra a versão do Windows Data Center comprada pelo cliente|
|Licença do Data Center do Win Server| Isso mostra o tipo de licença de compras do Data Center do Windows pelo cliente|
|AzureFit|  Pontos de dados internos e externos que definem firmographics. Ajustar a pontuação usa um modelo semelhante ao nosso melhor SMB para comparar os clientes e ver se eles são um ajuste potencial para Microsoft Cloud produtos. Ajustar Pontuação é atualizado trimestral.|
|AzureIntent|   Os sinais relacionados à mídia social e ao comportamento online de um cliente definem a intenção. A pontuação da intenção é sobreposta sobre ajustar para definir os clusters. A pontuação da intenção é atualizada mensalmente.|
|AzureCluster|  Isso identifica as propensações do cliente para comprar o Azure, consolidando as recomendações de ajuste e de intenção em um cluster.  Os clusters atuam agora e avaliados devem ser direcionados, pois produzirão um rendimento maior.  Incentivá e instrua os clientes só devem ser direcionados se ainda houver capacidade depois de direcionar o Act agora e avaliar os clientes.|
|WindowsServerDataCenter_HasOpenRenewal|    Isso identifica se um cliente tem uma renovação aberta para um Windows Server data center|
|WindowsServerStandard_HasOpenRenewal|  Isso identifica se um cliente tem uma renovação aberta para um Windows Server Standard|
|AzureUpsellCustomer|   Isso identifica se o cliente está mostrando a propensão de venda para o Azure|
|Tem Google|    Esse sinalizador identifica se um cliente está mostrando sinais competitivos para produtos pertencentes ao Google|
|Tem AWS|   Esse sinalizador identifica se um cliente está mostrando sinais competitivos para produtos de AWS de propriedade|
|Tem EA |Isso identifica se uma renovação é um EA (Enterprise Agreement) ou uma assinatura EA|
|Está aberto|  Isso identifica se uma renovação é um contrato aberto ou um valor aberto|

**Propensações de renovações de Ascent-Agreement de nuvem**: as definições de dados dos vários campos do relatório de propensações de renovações de contratos ascendentes da nuvem são:

|**Nome da Coluna** |**Descrição de dados** |
|---------|:---------|
|ID MPN|    ID de Microsoft Partner Network|
|Nome do parceiro|  Nome do parceiro|
|ID do Cliente|   Número do identificador do cliente |
|Número de DUNS|   O Dun & Bradstreet número do cliente que está sendo pontuado quanto à propensão|
|Nome da Conta|  Nome da conta |
|Domínio|    Domínio da conta|
|Tamanho da organização|  Tamanho da organização|
|Setor|  Setor  |
|Vertical|  A vertical do cliente que está sendo pontuado pela propensão, conforme identificado pela Microsoft e por outros padrões do setor (D&B)|
|Área|  Área geográfica do local|
|Subsidiária|    A subsidiária do cliente que está sendo classificada quanto à propensão|
|Território de Vendas|   Território de Vendas|
|City|  Local da cidade geográfica |
|Estado| Local do estado geográfico|
|Código postal|   Código postal|
|País|   Localização geográfica do país |
|Segment|   Segmento de mercado |
|Subsegmento|   Subsegmento de mercado |
|Resumo do tipo SMC|  Tipo do SMC |
|Superior não gerenciado-base de computação|  Principais clientes não gerenciados – computação|
|Principal base de usuários não gerenciados| Principais clientes não gerenciados – usuários|
|IsNonProfit|Se não há lucro ou lucro (Sim/não)|
|Tem Google|Esse sinalizador identifica se um cliente está mostrando sinais competitivos para produtos de AWS de propriedade|
|Tem AWS|Esse sinalizador identifica se um cliente está mostrando sinais competitivos para produtos de AWS de propriedade|
|Cluster do Azure|Isso identifica as propensações do cliente para comprar o Azure.  Os clusters atuam agora e avaliados devem ser direcionados, pois produzirão um rendimento maior.  Incentivá e instrua os clientes só devem ser direcionados se ainda houver capacidade depois de direcionar o Act agora e avaliar os clientes.|
|Cluster D365 F&O|  Isso identifica a propensão do cliente para comprar operações e Finanças D365s.  Os clientes que mostrarem a propensão para O F&O estarão nas principais categorias não gerenciadas.  Os clusters atuam agora e avaliados devem ser direcionados, pois produzirão um rendimento maior.  Incentivá e instrua os clientes só devem ser direcionados se ainda houver capacidade depois de direcionar o Act agora e avaliar os clientes.|
|Cluster D365 CE|   Isso identifica a propensão do cliente para comprar o engajamento do cliente D365.  Os clientes que mostram a propensão para CE estarão nas categorias média e pequena.  Os clusters atuam agora e avaliados devem ser direcionados, pois produzirão um rendimento maior.  Incentivá e instrua os clientes só devem ser direcionados se ainda houver capacidade depois de direcionar o Act agora e avaliar os clientes.|
|Cluster D365 BC|   Isso identifica a propensão do cliente para comprar o D365 Business central.  Os clientes que mostram a propensão para BC estarão nas categorias média e pequena.  Os clusters atuam agora e avaliados devem ser direcionados, pois produzirão um rendimento maior.  Incentivá e instrua os clientes só devem ser direcionados se ainda houver capacidade depois de direcionar o Act agora e avaliar os clientes.|
|Cluster M365|  Isso identifica a propensão do cliente para comprar o M365.  Os clusters atuam agora e avaliados devem ser direcionados, pois produzirão um rendimento maior.  Incentivá e instrua os clientes só devem ser direcionados se ainda houver capacidade depois de direcionar o Act agora e avaliar os clientes.|
|Programa de licença|   Isso identifica o tipo de programa de licença para a renovação|
|ID do contrato|  Identificador de contrato|
|Data de término do contrato|    Data de término do contrato |
|Tipo de Expiração|   Tipo de expiração|
|Receita de vencimento|  Receita associada a assinaturas expiradas|
|Tem EA|    Isso identifica se uma renovação é um EA (Enterprise Agreement) ou uma assinatura EA|
|Está aberto|  Isso identifica se uma renovação é um contrato aberto ou um valor aberto|
|Cliente de venda do Azure| Isso identifica se o cliente está mostrando a propensão de venda para o Azure|
|Cliente de venda M365|  Isso identifica se o cliente está mostrando a propensão de venda para M365|
|RevSumDivisionName|    Isso identifica o produto que está ativo para a renovação|

## <a name="next-steps"></a>Próximas etapas

Para relatórios, consulte [baixar relatórios](pci-download-reports.md).
