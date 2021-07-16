---
title: Faça sua primeira chamada à API para acessar dados de análise do Partner Insights
description: Exemplos para aprender a usar a API para acessar dados de análise do Partner Insights.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: d2252ccfb601ae22ce106d87fb06b67bf0927df5
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114374786"
---
# <a name="make-your-first-api-call-to-access-partner-insights-analytics-data"></a>Faça sua primeira chamada à API para acessar dados de análise do Partner Insights

Para ver uma lista das APIs para acessar dados de análise do Partner Insights, consulte [APIs](insights-programmatic-analytics-available-api.md)para acessar dados de análise do Partner Insights . Antes de fazer sua primeira chamada à API, certifique-se de que você atendeu aos [pré-requisitos](insights-programmatic-prerequisites.md) para acessar programaticamente os dados de análise Insights parceiros.

## <a name="token-generation"></a>Geração de token

Antes de chamar qualquer um dos métodos, primeiro você deve obter um token de acesso Azure Active Directory (AAD). Você precisa passar o token de acesso do Azure AD para o título autorização de cada método na API. Depois de obter um token de acesso, você tem 60 minutos para usá-lo antes que ele expire. Depois que o token expirar, você poderá atualizar o token e continuar a usá-lo para chamadas adicionais à API.

Consulte uma solicitação de exemplo abaixo para gerar um token. Os três valores necessários para gerar o token são `clientId` , `clientSecret` e `tenantId` . O parâmetro de recurso deve ser definido como `https://api.partnercenter.microsoft.com`

#### <a name="request-example"></a>Exemplo de solicitação

```console
curl --location --request POST 'https://login.microsoftonline.com/<tenantId>/oauth2/token' \
--header 'return-client-request-id: true' \
--header 'Content-Type: application/x-www-form-urlencoded' \
--header 'Cookie: fpc=Ar2GMei7JwdKg4Y4onHrMpvxqd4FAQAAAEhU_tcOAAAA; stsservicecookie=estsfd; x-ms-gateway-slice=estsfd' \
--data-urlencode 'resource= https://api.partnercenter.microsoft.com' \
--data-urlencode 'client_id= ' \
--data-urlencode 'client_secret= ' \
--data-urlencode 'grant_type=password' \
--data-urlencode 'scope=openid' \
--data-urlencode 'username= ' \
--data-urlencode 'password= '
```

#### <a name="response-example"></a>Exemplo de resposta

```json
{
    "token_type": "Bearer",
    "expires_in": "3599",
    "ext_expires_in": "3599",
    "expires_on": "1612794445",
    "not_before": "1612790545",
    "resource": "https://api.partnercenter.microsoft.com",
    "access_token": {Token}
}
```

Para obter mais informações sobre como obter um token do Azure AD para seu aplicativo, consulte Acessar dados de análise [usando serviços da Store.](/windows/uwp/monetize/access-analytics-data-using-windows-store-services#step-2-obtain-an-azure-ad-access-token)

## <a name="programmatic-api-call"></a>Chamada à API programática

Depois de obter o Token do AAD, conforme descrito na seção anterior, siga estas etapas para criar seu primeiro relatório de acesso programático.

Os dados podem ser baixados dos seguintes conjuntos de dados (datasetName):

- CustomersAndTenants
- SeatsSubscriptionsAndRevenue
- AzureUsage
- MSLearn
- OfficeUsage
- Perfil
- TrainingCompletions
- DynamicsUsage
- CompetencySummaryHistory
- PowerBIUsage
- EMSUsage
- CompetencyPeformanceRequirement
- ResellerPerformance
- CLASAgreementRenewalsPropensity
- CLASAzurePropensity
- CLASD365Propensity
- CLASM365Propensity
- TeamsUsage3PApps
- TeamsUsageWorkload
- TeamsUsageMeetingsAndCalls

Na seção a seguir, veremos exemplos de como acessar programaticamente do conjuntos de dados `SubscriptionId` DynamicsUsage.

### <a name="step-1-make-a-rest-call-using-the-get-datasets-api"></a>Etapa 1: Fazer uma chamada REST usando a API obter conjuntos de dados

A resposta da API fornece o nome do conjuntos de dados do qual você pode baixar o relatório. Para o conjuntos de dados específico, a resposta da API também fornece a lista de colunas selecionáveis que podem ser usadas para o modelo de relatório personalizado. Você também pode consultar as [Definições de Dados](insights-data-definitions.md) para obter os nomes das colunas.

#### <a name="request-example"></a>Exemplo de solicitação

```cli
curl 
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledDataset'\
--header 'Authorization: Bearer <AADToken>'
```

#### <a name="response-example"></a>Exemplo de resposta

```json
{
  "value": [
    {
      "datasetName": "DynamicsUsage",
      "selectableColumns": [
        "PGAMpnId",
        "SubscriptionId",
        "SubscriptionStartDate",
        "SubscriptionEndDate",
        "SubscriptionStatus",
        "Month",
        "RevSumDivisionName",
        "RevSumCategoryName",
        "SKU",
        "SKUId",
        "FreeVsPaidSKU",
        "SalesModel",
        "DetailedSalesModel",
        "CustomerName",
        "CustomerTenantId",
        "CustomerTpid",
        "CustomerSegment",
        "CustomerMarket",
        "MPNId",
        "PartnerName",
        "PartnerLocation",
        "PartnerAttachType",
        "AvailableSeats",
        "AssignedSeats",
        "ActiveSeats",
        "DeploymentOpportunity",
        "ActiveUsagePercent"
      ],
      "availableMetrics": [
        "SubscriptionCount",
        "TotalAssignedSeats",
        "TotalSoldSeats",
        "TotalActiveSeats",
        "TotalRevenueAndACR",
        "CustomerCount",
        "CustomerTenantCount"
      ],
      "availableDateRanges": [
        "LAST_MONTH",
        "LAST_3_MONTHS",
        "LAST_6_MONTHS",
        "LAST_1_YEAR",
        "LIFETIME"
      ],
      "minimumRecurrenceInterval": 24
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": "Dataset fetched successfully",
  "statusCode": 200,
  "dataRedacted": false
}
```

### <a name="step-2-create-the-custom-query"></a>Etapa 2: Criar a consulta personalizada

Nesta etapa, vamos usar SubscriptionId do conjuntos de dados DynamicsUsage para criar uma consulta personalizada para o relatório que desejamos. O período de tempo padrão, se não especificado na consulta, é de 6 meses.

#### <a name="request-example"></a>Exemplo de solicitação

```cli
curl 
--location 
--request POST 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries' \ 
--header ' Authorization: Bearer <AADToken>' \ 
--header 'Content-Type: application/json' \ 
--data-raw 
{
  "Name": "SubscriptionId Dynamics ",
  "Description": "List of Subscription Id from DynamicsUsage",
  "Query": "SELECT SubscriptionId from DynamicsUsage "
            }"
```

#### <a name="response-example"></a>Exemplo de resposta

```json
{
  "value": [
    {
      "queryId": "7d19305c-56db-4edc-b776-428340e3a9c8",
      "name": "SubscriptionId Dynamics",
      "description": "List of Subscription Id from DynamicsUsage",
      "query": "SELECT SubscriptionId from DynamicsUsage",
      "type": "userDefined",
      "user": "GAUser@PITEST2.ccsctp.net",
      "createdTime": "2021-03-31T07:28:37Z"
    }
 ],
  "nextLink": null,
  "totalCount": 1,
  "message": "Query created successfully",
  "statusCode": 200,
  "dataRedacted": false
}
```

Na execução bem-sucedida da consulta, é `queryId` gerado um que precisa ser usado para gerar o relatório.

### <a name="step-3-execute-test-query-api"></a>Etapa 3: Executar a API de consulta de teste

Nesta etapa, vamos usar a API de consulta de teste para obter as 100 primeiras linhas para a consulta que foi criada.

#### <a name="request-example"></a>Exemplo de solicitação

```cli
curl 
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/testQueryResult?queryId=7d19305c-56db-4edc-b776-428340e3a9c8' \
--header ' Authorization: Bearer <AADToken>'
```

#### <a name="response-example"></a>Exemplo de resposta

```json
{
  "value": [
    {
      "SubscriptionId": "251DE3D4-8868-4032-B518-F142DA50522F"
    },
    {
      "SubscriptionId": "758A0647-790C-435B-BEAA-652DF47E327C"
    },
    {
      "SubscriptionId": "ACE5A84B-9794-4480-82C5-AF9462DE2589"
    },
    {
      "SubscriptionId": "C75163EE-A0CA-4822-8275-E29E2490FF1C"
    },
    {
      "SubscriptionId": "082A8A18-0834-4376-A9A4-3AA4ECD02826"
    },
    .
    .
    .
    {
      "SubscriptionId": "5E10B817-7FCB-43CE-9F32-9CB60CF14658"
    },
    {
      "SubscriptionId": "7578872A-18C1-4E6B-8F51-469555337389"
    },
    {
      "SubscriptionId": "00601E10-4C05-4BA2-B977-6578F5C81D69"
    },
    {
      "SubscriptionId": "7EBFC3A9-D502-4EA2-87E7-C42971639E8C"
    },
    {
      "SubscriptionId": "2AC30AE1-5934-48FB-A0E5-EF6985761138"
    }
  ],
  "nextLink": null,
  "totalCount": 100,
  "message": null,
  "statusCode": 200,
  "dataRedacted": false
}
```

### <a name="step-4-create-the-report"></a>Etapa 4: Criar o relatório

Nesta etapa, vamos usar a QueryId gerada anteriormente para criar o relatório.

#### <a name="request-example"></a>Exemplo de solicitação

```cli
curl 
--location 
--request POST 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport'\
--header ' Authorization: Bearer <AADToken>' \ 
--header 'Content-Type: application/json' \ 
--data-raw 
'{
  "ReportName": "DynamicsUsage Subscription ID Report",
  "Description": "Report for getting list of Subscription Id for Dynamics Usage",
  "QueryId": "7d19305c-56db-4edc-b776-428340e3a9c8",
  "StartTime": "2021-04-01T18:41:00Z",
  "ExecuteNow": false,
  "QueryStartTime": "2021-03-31T18:41:00Z",
  "QueryEndTime": "2021-06-30T18:41:00Z",
  "RecurrenceInterval": 48,
  "RecurrenceCount": 20,
  "Format": "csv",
  "CallbackUrl": "https://<SampleCallbackUrl>",
  "CallbackMethod": "GET"
}'
```

#### <a name="response-example"></a>Exemplo de resposta

```json
{
  "value": [
    {
      "reportId": "cdc61cfe-d028-4333-a215-a1df51ccbfd4",
      "reportName": "DynamicsUsage Subscription ID Report",
      "description": "Report for getting list of Subscription Id for Dynamics Usage",
      "queryId": "7d19305c-56db-4edc-b776-428340e3a9c8",
      "query": "SELECT SubscriptionId from DynamicsUsage",
      "user": "GAUser@PITEST2.ccsctp.net",
      "createdTime": "2021-03-31T08:15:15Z",
      "modifiedTime": null,
      "executeNow": false,
      "startTime": "2021-04-01T18:41:00Z",
      "reportStatus": "Active",
      "recurrenceInterval": 48,
      "recurrenceCount": 20,
      "callbackUrl": "https://<SampleCallbackUrl>",
      "CallbackMethod": "GET",
      "format": "csv"
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": "Report created successfully",
  "statusCode": 200,
  "dataRedacted": false
}
```

Na execução bem-sucedida, `reportId` é gerado um que precisa ser usado para agendar um download do relatório.

### <a name="step-5-execute-report-executions-api"></a>Etapa 5: Executar API de Execuções de Relatório

Nesta etapa, vamos usar a API de Execuções de Relatório para obter o local seguro (URL) do relatório.

#### <a name="request-example"></a>Exemplo de solicitação

```cli
Curl
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/execution/ cdc61cfe-d028-4333-a215-a1df51ccbfd4?getLatestExecution=true'\
--header ' Authorization: Bearer <AADToken>' \
```

#### <a name="response-example"></a>Exemplo de resposta

```json
{
  "value": [
    {
      "executionId": "315eb63e-e2b2-41a2-ad8e-790b040fdce3",
      "reportId": "cdc61cfe-d028-4333-a215-a1df51ccbfd4",
      "recurrenceInterval": 48,
      "recurrenceCount": 20,
      "callbackUrl": null,
      "CallbackMethod": null,
      "format": "csv",
      "executionStatus": "Pending",
      "reportLocation": null,
      "reportAccessSecureLink": null,
      "reportExpiryTime": null,
      "reportGeneratedTime": null
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": null,
  "statusCode": 200,
  "dataRedacted": false
}
```

## <a name="next-steps"></a>Próximas etapas

- Experimente as APIs por meio da [URL da API do Swagger](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)