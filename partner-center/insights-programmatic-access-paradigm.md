---
title: Paradigma de acesso programático para Insights dados
description: Entenda o fluxo de alto nível do padrão de chamada à API para análise programática. As APIs para acessar relatórios de análise do Partner Insights também são abordadas.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: dcdd54fcc744fdb1683259203188c309a3949eff
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114374793"
---
# <a name="programmatic-access-paradigm"></a><span data-ttu-id="bbb9e-104">Paradigma do acesso programático</span><span class="sxs-lookup"><span data-stu-id="bbb9e-104">Programmatic access paradigm</span></span>

<span data-ttu-id="bbb9e-105">Este diagrama mostra o padrão de chamada de API usado para criar um novo modelo de relatório, agendar o relatório personalizado e recuperar dados de falha.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-105">This diagram shows the API call pattern used to create a new report template, schedule the custom report and retrieve failure data.</span></span>

:::image type="content" source="images/insights/prog-acc-paradigm.png" alt-text="Fluxo de alto nível":::
<span data-ttu-id="bbb9e-107">***Figura 1: Fluxo de alto nível do padrão de chamada à API***</span><span class="sxs-lookup"><span data-stu-id="bbb9e-107">***Figure 1: High level flow of the API call pattern***</span></span>

<span data-ttu-id="bbb9e-108">Esta lista fornece mais detalhes sobre a Figura 1.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-108">This list provides more details about Figure 1.</span></span>

1. <span data-ttu-id="bbb9e-109">O aplicativo cliente pode definir o esquema/modelo de relatório personalizado chamando a [API Criar relatório de consulta](#create-report-query-api).</span><span class="sxs-lookup"><span data-stu-id="bbb9e-109">The Client Application can define the custom report schema/template by calling the [Create Report Query API](#create-report-query-api).</span></span> <span data-ttu-id="bbb9e-110">Como alternativa, você pode escolher um modelo de relatório (QueryId) nos exemplos de biblioteca de modelos de relatório listados [aqui.](insights-programmatic-system-queries.md)</span><span class="sxs-lookup"><span data-stu-id="bbb9e-110">Alternately, you can pick a report template (QueryId) from the report template library samples listed [here.](insights-programmatic-system-queries.md)</span></span>
2. <span data-ttu-id="bbb9e-111">Em caso de êxito, a API Criar Consulta de Relatório retorna a QueryId.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-111">On success, the Create Report Query API returns the QueryId.</span></span>
3. <span data-ttu-id="bbb9e-112">Em seguida, o aplicativo cliente precisa chamar a [API](#create-report-api) Criar Relatório usando a QueryId juntamente com a data de início do relatório, Intervalo de Repetição, Recorrência e um URI de Retorno de Chamada opcional.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-112">The client application then needs to call the [Create Report API](#create-report-api) using the QueryId along with the report start date, Repeat Interval, Recurrence, and an optional Callback URI.</span></span>
4. <span data-ttu-id="bbb9e-113">Em Caso de êxito, [a API Criar Relatório](#create-report-api) retorna a ReportId.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-113">On Success, the [Create Report API](#create-report-api) returns the ReportId.</span></span>
5. <span data-ttu-id="bbb9e-114">O aplicativo cliente é notificado na URL de retorno de chamada assim que os dados do relatório estão prontos para download.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-114">The client application gets notified at the callback URL as soon as the report data is ready for download.</span></span>
6. <span data-ttu-id="bbb9e-115">Em seguida, o aplicativo cliente usa a [API](#get-report-execution-api) Obter Execuções de Relatório para consultar o status do relatório com a ID do relatório e o intervalo de datas.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-115">The client application then uses the [Get Report Executions API](#get-report-execution-api) to query the status of the report with the Report ID and date range.</span></span>
7. <span data-ttu-id="bbb9e-116">Em caso de sucesso, o link de download do relatório é retornado e o aplicativo pode iniciar o download dos dados.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-116">On success, the report download link is returned and the application can initiate download of the data.</span></span>

## <a name="report-query-language-specification"></a><span data-ttu-id="bbb9e-117">Especificação de linguagem de consulta de relatório</span><span class="sxs-lookup"><span data-stu-id="bbb9e-117">Report query language specification</span></span>

<span data-ttu-id="bbb9e-118">Embora forneçamos consultas [do sistema que](insights-programmatic-system-queries.md) você pode usar para criar relatórios, você também pode criar suas próprias consultas com base em suas necessidades de negócios.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-118">While we do provide [system queries](insights-programmatic-system-queries.md) you can use to create reports, you can also create your own queries based on your business needs.</span></span> <span data-ttu-id="bbb9e-119">Para saber mais sobre consultas personalizadas, consulte [Especificação de consulta personalizada.](insights-programmatic-custom-query.md)</span><span class="sxs-lookup"><span data-stu-id="bbb9e-119">To learn more about custom queries, see [Custom Query Specification](insights-programmatic-custom-query.md).</span></span>

## <a name="create-report-query-api"></a><span data-ttu-id="bbb9e-120">Criar API Criar relatório</span><span class="sxs-lookup"><span data-stu-id="bbb9e-120">Create report query API</span></span>

<span data-ttu-id="bbb9e-121">A API ajuda a criar consultas personalizadas que definem o conjuntos de dados do qual colunas e métricas precisam ser exportadas.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-121">The API helps to create custom queries that define the dataset from which columns and metrics need to be exported.</span></span> <span data-ttu-id="bbb9e-122">A API fornece a flexibilidade para criar um novo modelo de relatório com base nas necessidades de seus negócios.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-122">The API provides the flexibility to create a new reporting template based on your business needs.</span></span>  

<span data-ttu-id="bbb9e-123">Também é possível usar as [consultas do sistema](insights-programmatic-system-queries.md) que fornecemos.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-123">You can also use the [system queries](insights-programmatic-system-queries.md) we provide.</span></span> <span data-ttu-id="bbb9e-124">Quando modelos de relatório personalizados não são necessários, você pode chamar Criar [API](#create-report-api) de Relatório diretamente usando as QueryIds das consultas do sistema fornecidas.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-124">When custom report templates are not needed, you can call [Create Report API](#create-report-api) directly using the QueryIds of the system queries that are provided.</span></span>  

<span data-ttu-id="bbb9e-125">O exemplo a seguir mostra como criar uma consulta personalizada para obter os 10 principais clientes por receita do mês passado.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-125">The following example shows how to create a custom query to get top 10 customers by revenue for last month.</span></span>

### <a name="request-syntax"></a><span data-ttu-id="bbb9e-126">Sintaxe da solicitação</span><span class="sxs-lookup"><span data-stu-id="bbb9e-126">Request syntax</span></span>

|    <span data-ttu-id="bbb9e-127">Método</span><span class="sxs-lookup"><span data-stu-id="bbb9e-127">Method</span></span>     |    <span data-ttu-id="bbb9e-128">URI da solicitação</span><span class="sxs-lookup"><span data-stu-id="bbb9e-128">Request URI</span></span>     |
|----- | -----|
|    <span data-ttu-id="bbb9e-129">POST</span><span class="sxs-lookup"><span data-stu-id="bbb9e-129">POST</span></span>     |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries`|
|||

### <a name="request-header"></a><span data-ttu-id="bbb9e-130">Cabeçalho da solicitação</span><span class="sxs-lookup"><span data-stu-id="bbb9e-130">Request header</span></span>

|    <span data-ttu-id="bbb9e-131">parâmetro</span><span class="sxs-lookup"><span data-stu-id="bbb9e-131">Header</span></span>     |    <span data-ttu-id="bbb9e-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="bbb9e-132">Type</span></span>     |    <span data-ttu-id="bbb9e-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbb9e-133">Description</span></span>     |
|-------|-----|------|
|    <span data-ttu-id="bbb9e-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="bbb9e-134">Authorization</span></span>     |    <span data-ttu-id="bbb9e-135">string</span><span class="sxs-lookup"><span data-stu-id="bbb9e-135">string</span></span> |<span data-ttu-id="bbb9e-136">Obrigatórios.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-136">Required.</span></span> <span data-ttu-id="bbb9e-137">O token de acesso do Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="bbb9e-137">The Azure Active Directory (Azure AD) access token.</span></span> <span data-ttu-id="bbb9e-138">O formato é  `Bearer <token>` .</span><span class="sxs-lookup"><span data-stu-id="bbb9e-138">The format is `Bearer <token>`.</span></span>|
|    <span data-ttu-id="bbb9e-139">Tipo de conteúdo</span><span class="sxs-lookup"><span data-stu-id="bbb9e-139">Content-Type</span></span>     |<span data-ttu-id="bbb9e-140">string</span><span class="sxs-lookup"><span data-stu-id="bbb9e-140">string</span></span> |`Application/JSON` |
||||

### <a name="path-parameter"></a><span data-ttu-id="bbb9e-141">Parâmetro path</span><span class="sxs-lookup"><span data-stu-id="bbb9e-141">Path parameter</span></span>

<span data-ttu-id="bbb9e-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bbb9e-142">None</span></span>

### <a name="query-parameter"></a><span data-ttu-id="bbb9e-143">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="bbb9e-143">Query parameter</span></span>

<span data-ttu-id="bbb9e-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bbb9e-144">None</span></span>

### <a name="sample-request-payload"></a><span data-ttu-id="bbb9e-145">Carga de solicitação de exemplo</span><span class="sxs-lookup"><span data-stu-id="bbb9e-145">Sample request payload</span></span>

```json
{ 
  "Name": "CustomersRevenueQuery", 
  "Description": "Query to get top 10 customers by revenue for last month", 
  "Query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH" 
}
```

### <a name="glossary"></a><span data-ttu-id="bbb9e-146">Glossário</span><span class="sxs-lookup"><span data-stu-id="bbb9e-146">Glossary</span></span>

<span data-ttu-id="bbb9e-147">Esta tabela fornece as principais definições dos elementos da carga de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-147">This table provides the key definitions of elements in the request payload.</span></span>

|<span data-ttu-id="bbb9e-148">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="bbb9e-148">Parameter</span></span>|    <span data-ttu-id="bbb9e-149">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="bbb9e-149">Required</span></span>     |    <span data-ttu-id="bbb9e-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbb9e-150">Description</span></span>     |    <span data-ttu-id="bbb9e-151">Valores Permitidos</span><span class="sxs-lookup"><span data-stu-id="bbb9e-151">Allowed Values</span></span>     |
|-----|    -----    |    -----    |    -----    |
|<span data-ttu-id="bbb9e-152">Nome</span><span class="sxs-lookup"><span data-stu-id="bbb9e-152">Name</span></span> |    <span data-ttu-id="bbb9e-153">Yes</span><span class="sxs-lookup"><span data-stu-id="bbb9e-153">Yes</span></span>     |    <span data-ttu-id="bbb9e-154">Nome amigável da consulta</span><span class="sxs-lookup"><span data-stu-id="bbb9e-154">Friendly name of the query</span></span>     |    <span data-ttu-id="bbb9e-155">string</span><span class="sxs-lookup"><span data-stu-id="bbb9e-155">string</span></span>     |
|    <span data-ttu-id="bbb9e-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbb9e-156">Description</span></span>     |    <span data-ttu-id="bbb9e-157">Não</span><span class="sxs-lookup"><span data-stu-id="bbb9e-157">No</span></span>     |    <span data-ttu-id="bbb9e-158">Descrição do que a consulta retorna</span><span class="sxs-lookup"><span data-stu-id="bbb9e-158">Description of what the query returns</span></span>     |    <span data-ttu-id="bbb9e-159">string</span><span class="sxs-lookup"><span data-stu-id="bbb9e-159">string</span></span>     |
|    <span data-ttu-id="bbb9e-160">Consulta</span><span class="sxs-lookup"><span data-stu-id="bbb9e-160">Query</span></span>     |    <span data-ttu-id="bbb9e-161">Yes</span><span class="sxs-lookup"><span data-stu-id="bbb9e-161">Yes</span></span>     |    <span data-ttu-id="bbb9e-162">Cadeia de caracteres de consulta de relatório</span><span class="sxs-lookup"><span data-stu-id="bbb9e-162">Report query string</span></span>     |    <span data-ttu-id="bbb9e-163">Tipo de dados: cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bbb9e-163">Data type: string</span></span> <br> <span data-ttu-id="bbb9e-164">[Consulta personalizada](insights-programmatic-custom-query.md) com base na necessidade de negócios</span><span class="sxs-lookup"><span data-stu-id="bbb9e-164">[Custom query](insights-programmatic-custom-query.md) based on business need</span></span> |
|        |        |        |        |

> [!Note]
> <span data-ttu-id="bbb9e-165">Para exemplos de consulta personalizada, consulte [Exemplos de consultas de exemplo.](insights-programmatic-sample-queries.md)</span><span class="sxs-lookup"><span data-stu-id="bbb9e-165">For custom query samples, see [Examples of sample queries.](insights-programmatic-sample-queries.md)</span></span>

### <a name="sample-response"></a><span data-ttu-id="bbb9e-166">Resposta de exemplo</span><span class="sxs-lookup"><span data-stu-id="bbb9e-166">Sample response</span></span>

<span data-ttu-id="bbb9e-167">A carga de solicitação é estrutura conforme a seguir:</span><span class="sxs-lookup"><span data-stu-id="bbb9e-167">The response payload is structured as follows:</span></span>

<span data-ttu-id="bbb9e-168">Códigos de resposta: 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="bbb9e-168">Response Codes: 200, 400, 401, 403, 500</span></span>

<span data-ttu-id="bbb9e-169">Exemplo de conteúdo de resposta:</span><span class="sxs-lookup"><span data-stu-id="bbb9e-169">Response payload example:</span></span>

```json
{ 
  "value": [ 
    { 
      "queryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033",
      "name": "CustomersRevenueQuery",
      "description": "Query to get top 10 customers by revenue for last month",
      "query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH",
      "type": "userDefined",
      "user": "GAUser@PITEST2.ccsctp.net", 
      "createdTime": "2021-03-30T12:52:39Z" 
    }
  ], 
  "nextLink": null,
  "totalCount": 1,
  "message": "Query created successfully",
  "statusCode": 200,
  "dataRedacted": false
} 
```

### <a name="glossary"></a><span data-ttu-id="bbb9e-170">Glossário</span><span class="sxs-lookup"><span data-stu-id="bbb9e-170">Glossary</span></span>

<span data-ttu-id="bbb9e-171">Esta tabela fornece as principais definições dos elementos da carga de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-171">This table provides the key definitions of elements in the request payload.</span></span>

|    <span data-ttu-id="bbb9e-172">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="bbb9e-172">Parameter</span></span>     |    <span data-ttu-id="bbb9e-173">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbb9e-173">Description</span></span>     |
|    ----    |    ----    |
|    <span data-ttu-id="bbb9e-174">QueryId</span><span class="sxs-lookup"><span data-stu-id="bbb9e-174">QueryId</span></span>     |    <span data-ttu-id="bbb9e-175">UUID (identificador universal exclusivo) da consulta criada</span><span class="sxs-lookup"><span data-stu-id="bbb9e-175">Universally unique identifier (UUID) of the query you created</span></span>     |
|    <span data-ttu-id="bbb9e-176">Nome</span><span class="sxs-lookup"><span data-stu-id="bbb9e-176">Name</span></span>     |    <span data-ttu-id="bbb9e-177">Nome amigável fornecido à consulta na carga de solicitação</span><span class="sxs-lookup"><span data-stu-id="bbb9e-177">Friendly name given to the query in the request payload</span></span>     |
|    <span data-ttu-id="bbb9e-178">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbb9e-178">Description</span></span>     |    <span data-ttu-id="bbb9e-179">Descrição fornecida durante a criação da consulta</span><span class="sxs-lookup"><span data-stu-id="bbb9e-179">Description given during creation of the query</span></span>     |
|    <span data-ttu-id="bbb9e-180">Consulta</span><span class="sxs-lookup"><span data-stu-id="bbb9e-180">Query</span></span>     |    <span data-ttu-id="bbb9e-181">Consulta de relatório passada como entrada durante a criação da consulta</span><span class="sxs-lookup"><span data-stu-id="bbb9e-181">Report query passed as input during query creation</span></span>     |
|    <span data-ttu-id="bbb9e-182">Tipo</span><span class="sxs-lookup"><span data-stu-id="bbb9e-182">Type</span></span>     |    <span data-ttu-id="bbb9e-183">Definida como `userDefined`</span><span class="sxs-lookup"><span data-stu-id="bbb9e-183">Set to `userDefined`</span></span>     |
|    <span data-ttu-id="bbb9e-184">Usuário</span><span class="sxs-lookup"><span data-stu-id="bbb9e-184">User</span></span>     |    <span data-ttu-id="bbb9e-185">ID de usuário usada para criar a consulta</span><span class="sxs-lookup"><span data-stu-id="bbb9e-185">User ID used to create of the query</span></span>     |
|    <span data-ttu-id="bbb9e-186">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="bbb9e-186">CreatedTime</span></span>     |    <span data-ttu-id="bbb9e-187">Hora UTC em que a consulta foi criada neste formato: aaaa-mm-ddThh:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="bbb9e-187">UTC Time the query was created in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="bbb9e-188">TotalCount</span><span class="sxs-lookup"><span data-stu-id="bbb9e-188">TotalCount</span></span>     |    <span data-ttu-id="bbb9e-189">Número de conjuntos de dados na matriz de valores</span><span class="sxs-lookup"><span data-stu-id="bbb9e-189">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="bbb9e-190">StatusCode</span><span class="sxs-lookup"><span data-stu-id="bbb9e-190">StatusCode</span></span>     |    <span data-ttu-id="bbb9e-191">Código de Resultado</span><span class="sxs-lookup"><span data-stu-id="bbb9e-191">Result Code</span></span> <br> <span data-ttu-id="bbb9e-192">Os valores possíveis são 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="bbb9e-192">The possible values are 200, 400, 401, 403, 500</span></span>     |
|    <span data-ttu-id="bbb9e-193">message</span><span class="sxs-lookup"><span data-stu-id="bbb9e-193">message</span></span>     |    <span data-ttu-id="bbb9e-194">Mensagem do status da execução da API</span><span class="sxs-lookup"><span data-stu-id="bbb9e-194">Status message from the execution of the API</span></span>     |
|        |        |

## <a name="create-report-api"></a><span data-ttu-id="bbb9e-195">Criar API de relatório</span><span class="sxs-lookup"><span data-stu-id="bbb9e-195">Create report API</span></span>

<span data-ttu-id="bbb9e-196">Ao criar um modelo de relatório personalizado com êxito [](#create-report-query-api) e receber a QueryID como parte da resposta Criar Consulta de Relatório, essa API pode ser chamada para agendar uma consulta a ser executada em intervalos regulares.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-196">On creating a custom report template successfully and receiving the QueryID as part of [Create Report Query](#create-report-query-api) response, this API can be called to schedule a query to be executed at regular intervals.</span></span> <span data-ttu-id="bbb9e-197">É possível definir uma frequência e um agendamento para o relatório a ser entregue.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-197">You can set a frequency and schedule for the report to be delivered.</span></span>
<span data-ttu-id="bbb9e-198">Para consultas do sistema que fornecemos, a API criar relatório também pode ser chamada com [QueryId](insights-programmatic-system-queries.md).</span><span class="sxs-lookup"><span data-stu-id="bbb9e-198">For system queries we provide, the Create Report API can also be called with [QueryId](insights-programmatic-system-queries.md).</span></span>

### <a name="callback-url"></a><span data-ttu-id="bbb9e-199">URL de retorno de chamada</span><span class="sxs-lookup"><span data-stu-id="bbb9e-199">Callback URL</span></span>

<span data-ttu-id="bbb9e-200">A API de criação de relatório aceita uma URL de retorno de chamada.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-200">The create report API accepts a callback URL.</span></span> <span data-ttu-id="bbb9e-201">Essa URL será chamada depois que a geração de relatório for bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-201">This URL will be called once the report generation is successful.</span></span> <span data-ttu-id="bbb9e-202">A URL de retorno de chamada deve estar acessível publicamente.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-202">The callback URL should be publicly reachable.</span></span> <span data-ttu-id="bbb9e-203">Além da URL, um método de retorno de chamada também pode ser dado.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-203">In addition to the URL a callback method can also be given.</span></span> <span data-ttu-id="bbb9e-204">O método de retorno de chamada só pode ser "GET" ou "POST".</span><span class="sxs-lookup"><span data-stu-id="bbb9e-204">The callback method can only be "GET" or "POST".</span></span> <span data-ttu-id="bbb9e-205">O método padrão se nenhum valor for passado será "POST".</span><span class="sxs-lookup"><span data-stu-id="bbb9e-205">The default method if no value is passed will be "POST".</span></span> <span data-ttu-id="bbb9e-206">A reportId que concluiu a geração sempre será passada de volta durante o retorno de chamada.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-206">The reportId that has completed generation will always be passed back during the callback.</span></span>

<span data-ttu-id="bbb9e-207">Retorno de chamada POST: se a URL passada for `https://www.contosso.com/callback` , a URL chamada de volta será `https://www.contosso.com/callback/<reportID>`</span><span class="sxs-lookup"><span data-stu-id="bbb9e-207">POST callback: If the URL passed was `https://www.contosso.com/callback`, then the called back URL will be `https://www.contosso.com/callback/<reportID>`</span></span> 

<span data-ttu-id="bbb9e-208">Retorno de chamada GET: se a URL passada for `https://www.contosso.com/callback` , a URL chamada de volta será `https://www.contosso.com/callback?reportId=<reportID>`</span><span class="sxs-lookup"><span data-stu-id="bbb9e-208">GET callback: If the URL passed was `https://www.contosso.com/callback`, then the called back URL will be `https://www.contosso.com/callback?reportId=<reportID>`</span></span> 

### <a name="executenow-reports"></a><span data-ttu-id="bbb9e-209">Relatórios do ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="bbb9e-209">ExecuteNow reports</span></span>

<span data-ttu-id="bbb9e-210">Há um provisionamento para gerar um relatório sem agendamento.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-210">There is a provision to generate a report without scheduling.</span></span> <span data-ttu-id="bbb9e-211">O conteúdo da API de criação de relatório pode aceitar um parâmetro , que ensocará o relatório a ser gerado assim que a `ExecuteNow` API for chamada.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-211">The report create API payload can accept a parameter `ExecuteNow`, which will enqueue the report to be generated as soon as the API is called.</span></span> <span data-ttu-id="bbb9e-212">Quando `ExecuteNow` é definido como true, os campos: , , são `StartTime` `RecurrenceCount` `RecurrenceInterval` ignorados, pois esses relatórios não são agendados.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-212">When `ExecuteNow` is set to true, the fields: `StartTime`, `RecurrenceCount`, `RecurrenceInterval` are ignored as these reports are not scheduled.</span></span>

<span data-ttu-id="bbb9e-213">Dois campos adicionais podem ser passados `ExecuteNow` quando for true e `QueryStartTime` `QueryEndTime` .</span><span class="sxs-lookup"><span data-stu-id="bbb9e-213">Two additional fields can be passed when `ExecuteNow` is true, `QueryStartTime` and `QueryEndTime`.</span></span> <span data-ttu-id="bbb9e-214">Esses dois campos substituirão `TIMESPAN` o campo na consulta.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-214">These two fields will override the `TIMESPAN` field in the query.</span></span> <span data-ttu-id="bbb9e-215">Esses campos não são aplicáveis a relatórios agendados, pois os dados serão gerados continuamente por um período de tempo fixo que não muda.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-215">These fields are not applicable for scheduled reports as data will get continuously generated for a fixed time period that does not change.</span></span>

### <a name="request-syntax"></a><span data-ttu-id="bbb9e-216">Sintaxe da solicitação</span><span class="sxs-lookup"><span data-stu-id="bbb9e-216">Request syntax</span></span>

|    <span data-ttu-id="bbb9e-217">Método</span><span class="sxs-lookup"><span data-stu-id="bbb9e-217">Method</span></span>     |    <span data-ttu-id="bbb9e-218">URI da solicitação</span><span class="sxs-lookup"><span data-stu-id="bbb9e-218">Request URI</span></span>     |
|----- | -----|
|    <span data-ttu-id="bbb9e-219">POST</span><span class="sxs-lookup"><span data-stu-id="bbb9e-219">POST</span></span>     |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport` |

### <a name="request-header"></a><span data-ttu-id="bbb9e-220">Cabeçalho da solicitação</span><span class="sxs-lookup"><span data-stu-id="bbb9e-220">Request header</span></span>

|    <span data-ttu-id="bbb9e-221">parâmetro</span><span class="sxs-lookup"><span data-stu-id="bbb9e-221">Header</span></span>     |    <span data-ttu-id="bbb9e-222">Tipo</span><span class="sxs-lookup"><span data-stu-id="bbb9e-222">Type</span></span>     |    <span data-ttu-id="bbb9e-223">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbb9e-223">Description</span></span>     |
|-------|-----|------|
|    <span data-ttu-id="bbb9e-224">Autorização</span><span class="sxs-lookup"><span data-stu-id="bbb9e-224">Authorization</span></span>     |    <span data-ttu-id="bbb9e-225">string</span><span class="sxs-lookup"><span data-stu-id="bbb9e-225">string</span></span> |<span data-ttu-id="bbb9e-226">Obrigatórios.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-226">Required.</span></span> <span data-ttu-id="bbb9e-227">O token de acesso do Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="bbb9e-227">The Azure Active Directory (Azure AD) access token.</span></span> <span data-ttu-id="bbb9e-228">O formato é  `Bearer <token>` .</span><span class="sxs-lookup"><span data-stu-id="bbb9e-228">The format is `Bearer <token>`.</span></span>|
|    <span data-ttu-id="bbb9e-229">Tipo de conteúdo</span><span class="sxs-lookup"><span data-stu-id="bbb9e-229">Content-Type</span></span>     |<span data-ttu-id="bbb9e-230">string</span><span class="sxs-lookup"><span data-stu-id="bbb9e-230">string</span></span> |`Application/JSON` |

### <a name="path-parameter"></a><span data-ttu-id="bbb9e-231">Parâmetro de caminho</span><span class="sxs-lookup"><span data-stu-id="bbb9e-231">Path Parameter</span></span>

<span data-ttu-id="bbb9e-232">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bbb9e-232">None</span></span>

### <a name="query-parameter"></a><span data-ttu-id="bbb9e-233">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="bbb9e-233">Query Parameter</span></span>

<span data-ttu-id="bbb9e-234">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bbb9e-234">None</span></span>

### <a name="sample-request-payload"></a><span data-ttu-id="bbb9e-235">Carga de solicitação de exemplo</span><span class="sxs-lookup"><span data-stu-id="bbb9e-235">Sample request payload</span></span>

```json
{
  "ReportName": "Top10_CustomersReport",
  "Description": "Top 10 customers by revenue for last month",
  "QueryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033",
  "StartTime": "2021-03-31T18:41:00Z",
  "ExecuteNow": false,
  "QueryStartTime": null,
  "QueryEndTime": null,
  "RecurrenceInterval": 24,
  "RecurrenceCount": 100,
  "Format": "CSV",
  "CallbackUrl": "https://<SampleCallbackUrl>",
  "CallbackMethod": "GET"
}
```

### <a name="glossary"></a><span data-ttu-id="bbb9e-236">Glossário</span><span class="sxs-lookup"><span data-stu-id="bbb9e-236">Glossary</span></span>

<span data-ttu-id="bbb9e-237">As principais definições de elementos na carga de solicitação são articuladas abaixo:</span><span class="sxs-lookup"><span data-stu-id="bbb9e-237">Key definitions of elements in the request payload are articulated below:</span></span>

|    <span data-ttu-id="bbb9e-238">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="bbb9e-238">Parameter</span></span>     |    <span data-ttu-id="bbb9e-239">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="bbb9e-239">Required</span></span>     |    <span data-ttu-id="bbb9e-240">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbb9e-240">Description</span></span>     |    <span data-ttu-id="bbb9e-241">Valores Permitidos</span><span class="sxs-lookup"><span data-stu-id="bbb9e-241">Allowed Values</span></span>     |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="bbb9e-242">ReportName</span><span class="sxs-lookup"><span data-stu-id="bbb9e-242">ReportName</span></span>     |    <span data-ttu-id="bbb9e-243">Yes</span><span class="sxs-lookup"><span data-stu-id="bbb9e-243">Yes</span></span>     |    <span data-ttu-id="bbb9e-244">Nome a ser atribuído ao relatório</span><span class="sxs-lookup"><span data-stu-id="bbb9e-244">Name to be assigned to the report</span></span>     |    <span data-ttu-id="bbb9e-245">string</span><span class="sxs-lookup"><span data-stu-id="bbb9e-245">string</span></span>     |
|    <span data-ttu-id="bbb9e-246">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbb9e-246">Description</span></span>     |    <span data-ttu-id="bbb9e-247">Não</span><span class="sxs-lookup"><span data-stu-id="bbb9e-247">No</span></span>     |    <span data-ttu-id="bbb9e-248">Descrição do relatório criado</span><span class="sxs-lookup"><span data-stu-id="bbb9e-248">Description of the created report</span></span>     |    <span data-ttu-id="bbb9e-249">string</span><span class="sxs-lookup"><span data-stu-id="bbb9e-249">string</span></span>     |
|    <span data-ttu-id="bbb9e-250">QueryId</span><span class="sxs-lookup"><span data-stu-id="bbb9e-250">QueryId</span></span>     |    <span data-ttu-id="bbb9e-251">Yes</span><span class="sxs-lookup"><span data-stu-id="bbb9e-251">Yes</span></span>     |    <span data-ttu-id="bbb9e-252">ID da consulta de relatório</span><span class="sxs-lookup"><span data-stu-id="bbb9e-252">Report query ID</span></span>     |    <span data-ttu-id="bbb9e-253">string</span><span class="sxs-lookup"><span data-stu-id="bbb9e-253">string</span></span>     |
|    <span data-ttu-id="bbb9e-254">StartTime</span><span class="sxs-lookup"><span data-stu-id="bbb9e-254">StartTime</span></span>     |    <span data-ttu-id="bbb9e-255">Yes</span><span class="sxs-lookup"><span data-stu-id="bbb9e-255">Yes</span></span>     |    <span data-ttu-id="bbb9e-256">Carimbo de data/hora UTC no qual a geração de relatório será iniciada.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-256">UTC Timestamp at which the report generation will begin.</span></span> <br> <span data-ttu-id="bbb9e-257">O formato deve ser: aaaa-mm-ddThh:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="bbb9e-257">The format should be: yyyy-MM-ddTHH:mm:ssZ</span></span>       |    <span data-ttu-id="bbb9e-258">string</span><span class="sxs-lookup"><span data-stu-id="bbb9e-258">string</span></span>     |
|    <span data-ttu-id="bbb9e-259">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="bbb9e-259">ExecuteNow</span></span>     |    <span data-ttu-id="bbb9e-260">Não</span><span class="sxs-lookup"><span data-stu-id="bbb9e-260">No</span></span>     |    <span data-ttu-id="bbb9e-261">Esse parâmetro deve ser usado para criar um relatório que será executado apenas uma vez.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-261">This parameter should be used to create a report that will be executed only once.</span></span> <span data-ttu-id="bbb9e-262">`StartTime`, `RecurrenceInterval` e `RecurrenceCount` serão ignorados se isso estiver definido como true.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-262">`StartTime`, `RecurrenceInterval` and `RecurrenceCount` are ignored if this is set to true.</span></span> <span data-ttu-id="bbb9e-263">O relatório é executado imediatamente de forma assíncrona</span><span class="sxs-lookup"><span data-stu-id="bbb9e-263">The report is executed immediately in an asynchronous fashion</span></span>     |    <span data-ttu-id="bbb9e-264">true/false</span><span class="sxs-lookup"><span data-stu-id="bbb9e-264">true/false</span></span>     |
|    <span data-ttu-id="bbb9e-265">QueryStartTime</span><span class="sxs-lookup"><span data-stu-id="bbb9e-265">QueryStartTime</span></span>     |    <span data-ttu-id="bbb9e-266">Não</span><span class="sxs-lookup"><span data-stu-id="bbb9e-266">No</span></span>     |    <span data-ttu-id="bbb9e-267">Opcionalmente, especifica a hora de início para a consulta que extrai os dados.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-267">Optionally specifies the start time for the query extracting the data.</span></span> <span data-ttu-id="bbb9e-268">Esse parâmetro é aplicável somente a um relatório de execução única que `ExecuteNow` foi definido como true.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-268">This parameter is applicable only for one time execution report that have `ExecuteNow` set to true.</span></span> <span data-ttu-id="bbb9e-269">Definir esse parâmetro substitui `TIMESPAN` determinadas na consulta.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-269">Setting this parameter overrides `TIMESPAN` given in the query.</span></span> <span data-ttu-id="bbb9e-270">O formato deve ser: aaaa-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="bbb9e-270">The format should be yyyy-MM-ddTHH:mm:ssZ</span></span>     |    <span data-ttu-id="bbb9e-271">Carimbo de data/hora como cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bbb9e-271">Timestamp as string</span></span>     |
|    <span data-ttu-id="bbb9e-272">QueryEndTime</span><span class="sxs-lookup"><span data-stu-id="bbb9e-272">QueryEndTime</span></span>     |    <span data-ttu-id="bbb9e-273">Não</span><span class="sxs-lookup"><span data-stu-id="bbb9e-273">No</span></span>     |    <span data-ttu-id="bbb9e-274">Opcionalmente, especifica a hora de início para a consulta que extrai os dados.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-274">Optionally specifies the end time for the query extracting the data.</span></span> <span data-ttu-id="bbb9e-275">Esse parâmetro é aplicável somente a um relatório de execução única que `ExecuteNow` foi definido como true.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-275">This parameter is applicable only for one time execution report that have `ExecuteNow` set to true.</span></span> <span data-ttu-id="bbb9e-276">Definir esse parâmetro substitui `TIMESPAN` determinadas na consulta.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-276">Setting this parameter overrides `TIMESPAN` given in the query.</span></span> <span data-ttu-id="bbb9e-277">O formato deve ser: aaaa-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="bbb9e-277">The format should be yyyy-MM-ddTHH:mm:ssZ</span></span>     |    <span data-ttu-id="bbb9e-278">Carimbo de data/hora como cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bbb9e-278">Timestamp as string</span></span>     |
|    <span data-ttu-id="bbb9e-279">RecorrênciaInterval</span><span class="sxs-lookup"><span data-stu-id="bbb9e-279">RecurrenceInterval</span></span>     |    <span data-ttu-id="bbb9e-280">Yes</span><span class="sxs-lookup"><span data-stu-id="bbb9e-280">Yes</span></span>     |    <span data-ttu-id="bbb9e-281">Frequência em horas em que o relatório deve ser gerado.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-281">Frequency in hours at which the report should be generated.</span></span> <br> <span data-ttu-id="bbb9e-282">O valor mínimo é 4 e o valor máximo é 2160.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-282">Minimum value is 4 and Maximum value is 2160.</span></span>      |    <span data-ttu-id="bbb9e-283">Número inteiro</span><span class="sxs-lookup"><span data-stu-id="bbb9e-283">integer</span></span>     |
|    <span data-ttu-id="bbb9e-284">RecorrênciaCount</span><span class="sxs-lookup"><span data-stu-id="bbb9e-284">RecurrenceCount</span></span>     |    <span data-ttu-id="bbb9e-285">Não</span><span class="sxs-lookup"><span data-stu-id="bbb9e-285">No</span></span>     |    <span data-ttu-id="bbb9e-286">Número de relatórios a serem gerados.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-286">Number of reports to be generated.</span></span>     |    <span data-ttu-id="bbb9e-287">Número inteiro</span><span class="sxs-lookup"><span data-stu-id="bbb9e-287">integer</span></span>     |
|    <span data-ttu-id="bbb9e-288">Formatar</span><span class="sxs-lookup"><span data-stu-id="bbb9e-288">Format</span></span>     |    <span data-ttu-id="bbb9e-289">Não</span><span class="sxs-lookup"><span data-stu-id="bbb9e-289">No</span></span>     |    <span data-ttu-id="bbb9e-290">Formato de arquivo do arquivo exportado.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-290">File format of the exported file.</span></span> <br> <span data-ttu-id="bbb9e-291">O padrão é CSV.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-291">Default is CSV.</span></span>    |    <span data-ttu-id="bbb9e-292">"CSV"/"TSV"</span><span class="sxs-lookup"><span data-stu-id="bbb9e-292">"CSV"/"TSV"</span></span>     |
|    <span data-ttu-id="bbb9e-293">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="bbb9e-293">CallbackUrl</span></span>     |    <span data-ttu-id="bbb9e-294">Não</span><span class="sxs-lookup"><span data-stu-id="bbb9e-294">No</span></span>     |    <span data-ttu-id="bbb9e-295">URL acessível publicamente que pode ser configurada opcionalmente como destino de retorno de chamada</span><span class="sxs-lookup"><span data-stu-id="bbb9e-295">Publicly reachable URL that can be optionally configured as callback destination</span></span>     |    <span data-ttu-id="bbb9e-296">Cadeia de caracteres (URL http)</span><span class="sxs-lookup"><span data-stu-id="bbb9e-296">String (http URL)</span></span>     |
|    <span data-ttu-id="bbb9e-297">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="bbb9e-297">CallbackMethod</span></span>     |    <span data-ttu-id="bbb9e-298">Não</span><span class="sxs-lookup"><span data-stu-id="bbb9e-298">No</span></span>     |    <span data-ttu-id="bbb9e-299">O método a ser usado para retorno de chamada</span><span class="sxs-lookup"><span data-stu-id="bbb9e-299">The method to be used for callback</span></span>     |    <span data-ttu-id="bbb9e-300">GET/POST</span><span class="sxs-lookup"><span data-stu-id="bbb9e-300">GET/POST</span></span>     |
|        |        |        |        |

### <a name="sample-response"></a><span data-ttu-id="bbb9e-301">Resposta de exemplo</span><span class="sxs-lookup"><span data-stu-id="bbb9e-301">Sample response</span></span>

<span data-ttu-id="bbb9e-302">A carga de solicitação é estrutura conforme a seguir:</span><span class="sxs-lookup"><span data-stu-id="bbb9e-302">The response payload is structured as follows:</span></span>

<span data-ttu-id="bbb9e-303">Códigos de resposta: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="bbb9e-303">Response Codes: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="bbb9e-304">Exemplo de conteúdo de resposta:</span><span class="sxs-lookup"><span data-stu-id="bbb9e-304">Response payload example:</span></span>

```json
{ 
  "value": [
    { 
      "reportId": "d9548477-16d4-492a-bf9c-0cf91a9f69bf", 
      "reportName": "Top10_CustomersReport", 
      "description": "Top 10 customers by revenue for last month", 
      "queryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033", 
      "query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH", 
      "user": "GAUser@PITEST2.ccsctp.net", 
      "createdTime": "2021-03-30T13:11:58Z", 
      "modifiedTime": null, 
      "executeNow": false, 
      "startTime": "2021-03-31T18:41:00Z", 
      "reportStatus": "Active", 
      "recurrenceInterval": 24, 
      "recurrenceCount": 100, 
      "callbackUrl": "https://<SampleCallbackUrl>", 
      "callbackMethod": "GET", 
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

### <a name="glossary"></a><span data-ttu-id="bbb9e-305">Glossário</span><span class="sxs-lookup"><span data-stu-id="bbb9e-305">Glossary</span></span>

<span data-ttu-id="bbb9e-306">As principais definições de elementos na resposta são articuladas abaixo:</span><span class="sxs-lookup"><span data-stu-id="bbb9e-306">Key definitions of elements in the response are articulated below:</span></span>

|    <span data-ttu-id="bbb9e-307">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="bbb9e-307">Parameter</span></span>     |    <span data-ttu-id="bbb9e-308">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbb9e-308">Description</span></span>     |
|    ----    |    ----    |
|    <span data-ttu-id="bbb9e-309">ReportId</span><span class="sxs-lookup"><span data-stu-id="bbb9e-309">ReportId</span></span>     |    <span data-ttu-id="bbb9e-310">UUID (identificador universal exclusivo) do relatório criado</span><span class="sxs-lookup"><span data-stu-id="bbb9e-310">Universally unique identifier (UUID) of the report you created</span></span>     |
|    <span data-ttu-id="bbb9e-311">ReportName</span><span class="sxs-lookup"><span data-stu-id="bbb9e-311">ReportName</span></span>     |    <span data-ttu-id="bbb9e-312">Nome fornecido ao relatório na carga de solicitação</span><span class="sxs-lookup"><span data-stu-id="bbb9e-312">Name given to the report in the request payload</span></span>     |
|    <span data-ttu-id="bbb9e-313">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbb9e-313">Description</span></span>     |    <span data-ttu-id="bbb9e-314">Descrição fornecida durante a criação do relatório</span><span class="sxs-lookup"><span data-stu-id="bbb9e-314">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="bbb9e-315">QueryId</span><span class="sxs-lookup"><span data-stu-id="bbb9e-315">QueryId</span></span>     |    <span data-ttu-id="bbb9e-316">ID de consulta passada no momento da criação do relatório</span><span class="sxs-lookup"><span data-stu-id="bbb9e-316">Query ID passed at the time you created the report</span></span>     |
|    <span data-ttu-id="bbb9e-317">Consulta</span><span class="sxs-lookup"><span data-stu-id="bbb9e-317">Query</span></span>     |    <span data-ttu-id="bbb9e-318">Texto da consulta que será executada para este relatório</span><span class="sxs-lookup"><span data-stu-id="bbb9e-318">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="bbb9e-319">Usuário</span><span class="sxs-lookup"><span data-stu-id="bbb9e-319">User</span></span>     |    <span data-ttu-id="bbb9e-320">ID de usuário usada para criar o relatório</span><span class="sxs-lookup"><span data-stu-id="bbb9e-320">User ID used to create the report</span></span>     |
|    <span data-ttu-id="bbb9e-321">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="bbb9e-321">CreatedTime</span></span>     |    <span data-ttu-id="bbb9e-322">Hora UTC em que o relatório foi criado neste formato: aaaa-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="bbb9e-322">UTC Time the report was created in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="bbb9e-323">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="bbb9e-323">ModifiedTime</span></span>     |    <span data-ttu-id="bbb9e-324">Hora UTC em que o relatório foi modificado pela última vez neste formato: aaaa-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="bbb9e-324">UTC Time the report was last modified in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="bbb9e-325">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="bbb9e-325">ExecuteNow</span></span>     |    <span data-ttu-id="bbb9e-326">`ExecuteNow` sinalizador definido no momento em que o relatório foi criado</span><span class="sxs-lookup"><span data-stu-id="bbb9e-326">`ExecuteNow` flag set at the time the report was created</span></span>     |
|    <span data-ttu-id="bbb9e-327">StartTime</span><span class="sxs-lookup"><span data-stu-id="bbb9e-327">StartTime</span></span>     |    <span data-ttu-id="bbb9e-328">Hora UTC em que a execução do relatório será iniciada neste formato: aaaa-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="bbb9e-328">UTC Time the report execution will begin in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="bbb9e-329">Reportstatus</span><span class="sxs-lookup"><span data-stu-id="bbb9e-329">ReportStatus</span></span>     |    <span data-ttu-id="bbb9e-330">Status da execução do relatório.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-330">Status of the report execution.</span></span> <span data-ttu-id="bbb9e-331">Os valores possíveis `Paused` são `Active` , e `Inactive`</span><span class="sxs-lookup"><span data-stu-id="bbb9e-331">The possible values are `Paused`, `Active`, and `Inactive`</span></span>     |
|    <span data-ttu-id="bbb9e-332">RecorrênciaInterval</span><span class="sxs-lookup"><span data-stu-id="bbb9e-332">RecurrenceInterval</span></span>     |    <span data-ttu-id="bbb9e-333">Intervalo de recorrência fornecido durante a criação do relatório</span><span class="sxs-lookup"><span data-stu-id="bbb9e-333">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="bbb9e-334">RecorrênciaCount</span><span class="sxs-lookup"><span data-stu-id="bbb9e-334">RecurrenceCount</span></span>     |    <span data-ttu-id="bbb9e-335">Contagem de recorrência fornecida durante a criação do relatório.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-335">Recurrence count provided during report creation.</span></span>      |
|    <span data-ttu-id="bbb9e-336">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="bbb9e-336">CallbackUrl</span></span>     |    <span data-ttu-id="bbb9e-337">URL de retorno de chamada fornecida na solicitação</span><span class="sxs-lookup"><span data-stu-id="bbb9e-337">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="bbb9e-338">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="bbb9e-338">CallbackMethod</span></span>     |    <span data-ttu-id="bbb9e-339">Método de retorno de chamada fornecido na solicitação</span><span class="sxs-lookup"><span data-stu-id="bbb9e-339">Callback method provided in the request</span></span>     |
|    <span data-ttu-id="bbb9e-340">Formatar</span><span class="sxs-lookup"><span data-stu-id="bbb9e-340">Format</span></span>     |    <span data-ttu-id="bbb9e-341">Formato dos arquivos de relatório.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-341">Format of the report files.</span></span> <span data-ttu-id="bbb9e-342">Os valores possíveis são `CSV` ou `TSV` .</span><span class="sxs-lookup"><span data-stu-id="bbb9e-342">The possible values are `CSV` or `TSV`.</span></span>     |
|    <span data-ttu-id="bbb9e-343">TotalCount</span><span class="sxs-lookup"><span data-stu-id="bbb9e-343">TotalCount</span></span>     |    <span data-ttu-id="bbb9e-344">Número de registros na matriz Value</span><span class="sxs-lookup"><span data-stu-id="bbb9e-344">Number of records in the Value array</span></span>     |
|    <span data-ttu-id="bbb9e-345">StatusCode</span><span class="sxs-lookup"><span data-stu-id="bbb9e-345">StatusCode</span></span>     |    <span data-ttu-id="bbb9e-346">Código de Resultado</span><span class="sxs-lookup"><span data-stu-id="bbb9e-346">Result Code</span></span>     |
|    <span data-ttu-id="bbb9e-347">message</span><span class="sxs-lookup"><span data-stu-id="bbb9e-347">message</span></span>     |    <span data-ttu-id="bbb9e-348">Os valores possíveis são 200, 400, 401, 403, 500.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-348">The possible values are 200, 400, 401, 403, 500.</span></span> <span data-ttu-id="bbb9e-349">Mensagem do status da execução da API</span><span class="sxs-lookup"><span data-stu-id="bbb9e-349">Status message from the execution of the API</span></span>     |
|        |        |

## <a name="get-report-execution-api"></a><span data-ttu-id="bbb9e-350">Obter API de execução de relatório</span><span class="sxs-lookup"><span data-stu-id="bbb9e-350">Get report execution API</span></span>

<span data-ttu-id="bbb9e-351">Você pode usar esse método para consultar o status de uma execução de relatório usando a ReportId recebida de [Criar API de Relatório.](#create-report-api)</span><span class="sxs-lookup"><span data-stu-id="bbb9e-351">You can use this method to query the status of a report execution using the ReportId received from [Create Report API](#create-report-api).</span></span> <span data-ttu-id="bbb9e-352">O método retornará o link de download do relatório se o relatório estiver pronto para download.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-352">The method returns the report download link if the report is ready for download.</span></span> <span data-ttu-id="bbb9e-353">Caso contrário, o método retornará o status.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-353">Otherwise, the method returns the status.</span></span> <span data-ttu-id="bbb9e-354">Também é possível usar essa API para obter todas as execuções que ocorreram para um determinado relatório.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-354">You can also use this API to get all the executions that have happened for a given report.</span></span>  

>[!IMPORTANT]
><span data-ttu-id="bbb9e-355">Essa API tem parâmetros de consulta padrão definidos para `executionStatus=Completed` e `getLatestExecution=true` .</span><span class="sxs-lookup"><span data-stu-id="bbb9e-355">This API has default query parameters set for `executionStatus=Completed` and `getLatestExecution=true`.</span></span> <span data-ttu-id="bbb9e-356">Portanto, chamar a API antes da primeira execução bem-sucedida do relatório retornará 404.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-356">Hence, calling the API before the first successful execution of the report will return 404.</span></span> <span data-ttu-id="bbb9e-357">Execuções pendentes podem ser obtidas pela configuração `executionStatus=Pending`.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-357">Pending executions can be obtained by setting `executionStatus=Pending`.</span></span>

### <a name="request-syntax"></a><span data-ttu-id="bbb9e-358">Sintaxe da solicitação</span><span class="sxs-lookup"><span data-stu-id="bbb9e-358">Request syntax</span></span>

|    <span data-ttu-id="bbb9e-359">Método</span><span class="sxs-lookup"><span data-stu-id="bbb9e-359">Method</span></span>     |    <span data-ttu-id="bbb9e-360">URI da solicitação</span><span class="sxs-lookup"><span data-stu-id="bbb9e-360">Request URI</span></span>     |
|----- | -----|
|    <span data-ttu-id="bbb9e-361">GET</span><span class="sxs-lookup"><span data-stu-id="bbb9e-361">GET</span></span>    |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/execution/{reportId}?executionId={executionId}&executionStatus={executionStatus}&getLatestExecution={getLatestExecution}`  |

### <a name="request-header"></a><span data-ttu-id="bbb9e-362">Cabeçalho da solicitação</span><span class="sxs-lookup"><span data-stu-id="bbb9e-362">Request header</span></span>

|    <span data-ttu-id="bbb9e-363">parâmetro</span><span class="sxs-lookup"><span data-stu-id="bbb9e-363">Header</span></span>     |    <span data-ttu-id="bbb9e-364">Tipo</span><span class="sxs-lookup"><span data-stu-id="bbb9e-364">Type</span></span>     |    <span data-ttu-id="bbb9e-365">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbb9e-365">Description</span></span>     |
|-------|-----|------|
|    <span data-ttu-id="bbb9e-366">Autorização</span><span class="sxs-lookup"><span data-stu-id="bbb9e-366">Authorization</span></span>     |    <span data-ttu-id="bbb9e-367">string</span><span class="sxs-lookup"><span data-stu-id="bbb9e-367">string</span></span> |<span data-ttu-id="bbb9e-368">Obrigatórios.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-368">Required.</span></span> <span data-ttu-id="bbb9e-369">O token de acesso do Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="bbb9e-369">The Azure Active Directory (Azure AD) access token.</span></span> <span data-ttu-id="bbb9e-370">O formato é  `Bearer <token>` .</span><span class="sxs-lookup"><span data-stu-id="bbb9e-370">The format is `Bearer <token>`.</span></span>|
|    <span data-ttu-id="bbb9e-371">Tipo de conteúdo</span><span class="sxs-lookup"><span data-stu-id="bbb9e-371">Content-Type</span></span>     |<span data-ttu-id="bbb9e-372">string</span><span class="sxs-lookup"><span data-stu-id="bbb9e-372">string</span></span> |`Application/JSON` |

### <a name="path-parameter"></a><span data-ttu-id="bbb9e-373">Parâmetro path</span><span class="sxs-lookup"><span data-stu-id="bbb9e-373">Path parameter</span></span>

|    <span data-ttu-id="bbb9e-374">Nome do Parâmetro</span><span class="sxs-lookup"><span data-stu-id="bbb9e-374">Parameter Name</span></span>    |    <span data-ttu-id="bbb9e-375">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="bbb9e-375">Required</span></span>    |    <span data-ttu-id="bbb9e-376">Type</span><span class="sxs-lookup"><span data-stu-id="bbb9e-376">Type</span></span>    |    <span data-ttu-id="bbb9e-377">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbb9e-377">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="bbb9e-378">reportId</span><span class="sxs-lookup"><span data-stu-id="bbb9e-378">reportId</span></span>    |    <span data-ttu-id="bbb9e-379">Sim</span><span class="sxs-lookup"><span data-stu-id="bbb9e-379">Yes</span></span>    |    <span data-ttu-id="bbb9e-380">string</span><span class="sxs-lookup"><span data-stu-id="bbb9e-380">string</span></span>    |    <span data-ttu-id="bbb9e-381">Filtre para obter detalhes de execução apenas de relatórios com a reportId fornecidas neste argumento.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-381">Filter to get execution details of only reports with the reportId given in this argument.</span></span> <span data-ttu-id="bbb9e-382">Várias reportIds podem ser especificadas separando-as com um ponto e vírgula ";".</span><span class="sxs-lookup"><span data-stu-id="bbb9e-382">Multiple reportIds can be specified by separating them with a semicolon ";".</span></span>    |
|        |        |        |        |

### <a name="query-parameter"></a><span data-ttu-id="bbb9e-383">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="bbb9e-383">Query parameter</span></span>

|    <span data-ttu-id="bbb9e-384">Nome do Parâmetro</span><span class="sxs-lookup"><span data-stu-id="bbb9e-384">Parameter Name</span></span>    |    <span data-ttu-id="bbb9e-385">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="bbb9e-385">Required</span></span>    |    <span data-ttu-id="bbb9e-386">Type</span><span class="sxs-lookup"><span data-stu-id="bbb9e-386">Type</span></span>    |    <span data-ttu-id="bbb9e-387">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbb9e-387">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="bbb9e-388">Executionid</span><span class="sxs-lookup"><span data-stu-id="bbb9e-388">executionId</span></span>    |    <span data-ttu-id="bbb9e-389">Não</span><span class="sxs-lookup"><span data-stu-id="bbb9e-389">No</span></span>    |    <span data-ttu-id="bbb9e-390">string</span><span class="sxs-lookup"><span data-stu-id="bbb9e-390">string</span></span>    |    <span data-ttu-id="bbb9e-391">Filtre para obter detalhes apenas de relatórios com executionId determinado neste argumento.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-391">Filter to get details of only reports with the executionId given in this argument.</span></span> <span data-ttu-id="bbb9e-392">Várias executionIds podem ser especificadas separando-as com um ponto e vírgula ";".</span><span class="sxs-lookup"><span data-stu-id="bbb9e-392">Multiple executionIds can be specified by separating them with a semicolon ";".</span></span>    |
|    <span data-ttu-id="bbb9e-393">Executionstatus</span><span class="sxs-lookup"><span data-stu-id="bbb9e-393">executionStatus</span></span>    |    <span data-ttu-id="bbb9e-394">Não</span><span class="sxs-lookup"><span data-stu-id="bbb9e-394">No</span></span>    |    <span data-ttu-id="bbb9e-395">Cadeia de caracteres/enum</span><span class="sxs-lookup"><span data-stu-id="bbb9e-395">String/enum</span></span>    |    <span data-ttu-id="bbb9e-396">Filtre para obter detalhes apenas de relatórios com executionStatus dado neste argumento.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-396">Filter to get details of only reports with the executionStatus given in this argument.</span></span> <br> <span data-ttu-id="bbb9e-397">Os valores válidos são: `Pending` `Running` , e `Paused` `Completed` .</span><span class="sxs-lookup"><span data-stu-id="bbb9e-397">Valid values are: `Pending`, `Running`, `Paused` and `Completed`.</span></span> <br> <span data-ttu-id="bbb9e-398">O valor padrão é `Completed`.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-398">The default value is `Completed`.</span></span> <br> <span data-ttu-id="bbb9e-399">Vários status podem ser especificados separando-os com um ponto e vírgula ";".</span><span class="sxs-lookup"><span data-stu-id="bbb9e-399">Multiple statuses can be specified by separating them with a semicolon ";".</span></span>    |
|    <span data-ttu-id="bbb9e-400">getLatestExecution</span><span class="sxs-lookup"><span data-stu-id="bbb9e-400">getLatestExecution</span></span>    |    <span data-ttu-id="bbb9e-401">Não</span><span class="sxs-lookup"><span data-stu-id="bbb9e-401">No</span></span>    |    <span data-ttu-id="bbb9e-402">booleano</span><span class="sxs-lookup"><span data-stu-id="bbb9e-402">boolean</span></span>    |    <span data-ttu-id="bbb9e-403">A API retornará detalhes da execução mais recente.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-403">The API will return details of the latest execution.</span></span> <span data-ttu-id="bbb9e-404">Por padrão, esse parâmetro é definido como true.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-404">By default, this parameter is set to true.</span></span><br> <span data-ttu-id="bbb9e-405">Se você optar por passar o valor desse parâmetro como false, a API retornará as últimas 90 dias de execução de instâncias.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-405">If you choose to pass the value of this parameter as false, then the API will return the last 90 days execution instances.</span></span>    |
|        |        |        |        |

### <a name="sample-request-payload"></a><span data-ttu-id="bbb9e-406">Exemplo de carga de solicitação</span><span class="sxs-lookup"><span data-stu-id="bbb9e-406">Sample Request Payload</span></span>

<span data-ttu-id="bbb9e-407">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bbb9e-407">None</span></span>

### <a name="sample-response"></a><span data-ttu-id="bbb9e-408">Exemplo de Resposta</span><span class="sxs-lookup"><span data-stu-id="bbb9e-408">Sample Response</span></span>

<span data-ttu-id="bbb9e-409">A carga de solicitação é estrutura conforme a seguir:</span><span class="sxs-lookup"><span data-stu-id="bbb9e-409">The response payload is structured as follows:</span></span>

<span data-ttu-id="bbb9e-410">Códigos de resposta: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="bbb9e-410">Response Codes: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="bbb9e-411">Exemplo de conteúdo de resposta:</span><span class="sxs-lookup"><span data-stu-id="bbb9e-411">Response payload example:</span></span>

```json
{
  "value": [
    {
      "executionId": "906931dc-4f2f-4195-bbb2-d7295c7550d3",
      "reportId": "d9548477-16d4-492a-bf9c-0cf91a9f69bf",
      "recurrenceInterval": 24,
      "recurrenceCount": 100,
      "callbackUrl": null,
      "callbackMethod": null,
      "format": "csv",
      "executionStatus": "Completed",
      "reportLocation": null,
      "reportAccessSecureLink": "https://<path to report for download>",
      "reportExpiryTime": null,
      "reportGeneratedTime": "2021-03-31T18:41:00Z"
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": null,
  "statusCode": 200,
  "dataRedacted": false
}
```

<span data-ttu-id="bbb9e-412">Depois que a execução do relatório for concluída, o status de execução `Completed` será mostrado.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-412">Once report execution is complete, the execution status `Completed` is shown.</span></span> <span data-ttu-id="bbb9e-413">É possível baixar o relatório selecionando a URL no `reportAccessSecureLink`.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-413">You can download the report by selecting the URL in the `reportAccessSecureLink`.</span></span>

### <a name="glossary"></a><span data-ttu-id="bbb9e-414">Glossário</span><span class="sxs-lookup"><span data-stu-id="bbb9e-414">Glossary</span></span>

<span data-ttu-id="bbb9e-415">Principais definições dos elementos na resposta.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-415">Key definitions of elements in the response.</span></span>

|    <span data-ttu-id="bbb9e-416">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="bbb9e-416">Parameter</span></span>    |    <span data-ttu-id="bbb9e-417">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbb9e-417">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="bbb9e-418">ExecutionId</span><span class="sxs-lookup"><span data-stu-id="bbb9e-418">ExecutionId</span></span>    |    <span data-ttu-id="bbb9e-419">UUID (identificador universal exclusivo) da instância de execução</span><span class="sxs-lookup"><span data-stu-id="bbb9e-419">Universally unique identifier (UUID) of the execution instance</span></span>    |
|    <span data-ttu-id="bbb9e-420">ReportId</span><span class="sxs-lookup"><span data-stu-id="bbb9e-420">ReportId</span></span>    |    <span data-ttu-id="bbb9e-421">ID do relatório associada à instância de execução</span><span class="sxs-lookup"><span data-stu-id="bbb9e-421">Report ID associated with the execution instance</span></span>    |
|    <span data-ttu-id="bbb9e-422">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="bbb9e-422">RecurrenceInterval</span></span>    |    <span data-ttu-id="bbb9e-423">Intervalo de recorrência fornecido durante a criação do relatório</span><span class="sxs-lookup"><span data-stu-id="bbb9e-423">Recurrence interval provided during report creation</span></span>    |
|    <span data-ttu-id="bbb9e-424">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="bbb9e-424">RecurrenceCount</span></span>    |    <span data-ttu-id="bbb9e-425">Contagem de recorrência fornecida durante a criação do relatório</span><span class="sxs-lookup"><span data-stu-id="bbb9e-425">Recurrence count provided during report creation</span></span>    |
|    <span data-ttu-id="bbb9e-426">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="bbb9e-426">CallbackUrl</span></span>    |    <span data-ttu-id="bbb9e-427">URL de retorno de chamada associada à instância de execução</span><span class="sxs-lookup"><span data-stu-id="bbb9e-427">Callback URL associated with the execution instance</span></span>    |
|    <span data-ttu-id="bbb9e-428">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="bbb9e-428">CallbackMethod</span></span>    |    <span data-ttu-id="bbb9e-429">Método de retorno de chamada associado à instância de execução</span><span class="sxs-lookup"><span data-stu-id="bbb9e-429">Callback method associated with the execution instance</span></span>    |
|    <span data-ttu-id="bbb9e-430">Formatar</span><span class="sxs-lookup"><span data-stu-id="bbb9e-430">Format</span></span>    |    <span data-ttu-id="bbb9e-431">Formato do arquivo gerado no final da execução</span><span class="sxs-lookup"><span data-stu-id="bbb9e-431">Format of the generated file at the end of execution</span></span>    |
|    <span data-ttu-id="bbb9e-432">ExecutionStatus</span><span class="sxs-lookup"><span data-stu-id="bbb9e-432">ExecutionStatus</span></span>    |    <span data-ttu-id="bbb9e-433">Status da instância de execução do relatório.</span><span class="sxs-lookup"><span data-stu-id="bbb9e-433">Status of the report execution instance.</span></span> <br> <span data-ttu-id="bbb9e-434">Os valores válidos são: `Pending`, `Running`, `Paused`, e `Completed`</span><span class="sxs-lookup"><span data-stu-id="bbb9e-434">Valid values are: `Pending`, `Running`, `Paused`, and `Completed`</span></span>    |
|    <span data-ttu-id="bbb9e-435">ReportAccessSecureLink</span><span class="sxs-lookup"><span data-stu-id="bbb9e-435">ReportAccessSecureLink</span></span>    |<span data-ttu-id="bbb9e-436">Link pelo qual o relatório pode ser acessado com segurança</span><span class="sxs-lookup"><span data-stu-id="bbb9e-436">Link through which the report can be accessed securely</span></span>        |
|    <span data-ttu-id="bbb9e-437">ReportExpiryTime</span><span class="sxs-lookup"><span data-stu-id="bbb9e-437">ReportExpiryTime</span></span>    |    <span data-ttu-id="bbb9e-438">Hora UTC após a qual o link do relatório expirará neste formato: aaaa-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="bbb9e-438">UTC Time after which the report link will expire in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>    |
|    <span data-ttu-id="bbb9e-439">ReportGeneratedTime</span><span class="sxs-lookup"><span data-stu-id="bbb9e-439">ReportGeneratedTime</span></span>    |    <span data-ttu-id="bbb9e-440">Hora UTC em que o relatório foi gerado neste formato: aaaa-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="bbb9e-440">UTC Time at which the report was generated in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>    |
|    <span data-ttu-id="bbb9e-441">TotalCount</span><span class="sxs-lookup"><span data-stu-id="bbb9e-441">TotalCount</span></span>    |    <span data-ttu-id="bbb9e-442">Número de conjuntos de dados na matriz de valores</span><span class="sxs-lookup"><span data-stu-id="bbb9e-442">Number of datasets in the Value array</span></span>    |
|    <span data-ttu-id="bbb9e-443">StatusCode</span><span class="sxs-lookup"><span data-stu-id="bbb9e-443">StatusCode</span></span>    |    <span data-ttu-id="bbb9e-444">Código de Resultado</span><span class="sxs-lookup"><span data-stu-id="bbb9e-444">Result Code</span></span> <br> <span data-ttu-id="bbb9e-445">Os valores possíveis são 200, 400, 401, 403, 404 e 500</span><span class="sxs-lookup"><span data-stu-id="bbb9e-445">The possible values are 200, 400, 401, 403, 404 and 500</span></span>    |
|    <span data-ttu-id="bbb9e-446">message</span><span class="sxs-lookup"><span data-stu-id="bbb9e-446">message</span></span>    |    <span data-ttu-id="bbb9e-447">Mensagem do status da execução da API</span><span class="sxs-lookup"><span data-stu-id="bbb9e-447">Status message from the execution of the API</span></span>    |
|        |        |

## <a name="next-steps"></a><span data-ttu-id="bbb9e-448">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="bbb9e-448">Next steps</span></span>

- <span data-ttu-id="bbb9e-449">Experimente as APIs por meio da [URL da API do Swagger](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)</span><span class="sxs-lookup"><span data-stu-id="bbb9e-449">Try out the APIs through the [swagger API URL](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)</span></span>
- [<span data-ttu-id="bbb9e-450">Faça sua primeira chamada à API</span><span class="sxs-lookup"><span data-stu-id="bbb9e-450">Make your first API call</span></span>](insights-programmatic-first-api-call.md)