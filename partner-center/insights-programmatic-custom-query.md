---
title: Especificação de consulta personalizada
description: Saiba como criar consultas personalizadas para extrair dados de tabelas de análise.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 57f2109044e604dca21b0109b5be56f40170628e
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114374845"
---
# <a name="custom-query-specification"></a><span data-ttu-id="7af6d-103">Especificação de consulta personalizada</span><span class="sxs-lookup"><span data-stu-id="7af6d-103">Custom query specification</span></span>

<span data-ttu-id="7af6d-104">Os parceiros podem usar essa especificação de consulta para formular facilmente consultas personalizadas para extrair dados de tabelas de análise.</span><span class="sxs-lookup"><span data-stu-id="7af6d-104">Partners can use this query specification to easily formulate custom queries for extracting data from analytics tables.</span></span> <span data-ttu-id="7af6d-105">As consultas podem ser usadas para selecionar apenas as colunas e métricas desejadas que corresponderem a um determinado critério.</span><span class="sxs-lookup"><span data-stu-id="7af6d-105">The queries can be used to select only the desired columns and metrics that match a certain criterion.</span></span> <span data-ttu-id="7af6d-106">No centro da especificação da linguagem está a definição de conjuntos de dados na qual uma consulta personalizada pode ser escrita.</span><span class="sxs-lookup"><span data-stu-id="7af6d-106">At the heart of the language specification is the dataset definition on which a custom query can be written.</span></span>

## <a name="datasets"></a><span data-ttu-id="7af6d-107">Conjunto de dados</span><span class="sxs-lookup"><span data-stu-id="7af6d-107">Datasets</span></span>

<span data-ttu-id="7af6d-108">Da mesma forma que algumas consultas são executados em um banco de dados que tem tabelas e colunas, uma consulta personalizada funciona em conjuntos de dados que têm colunas e métricas.</span><span class="sxs-lookup"><span data-stu-id="7af6d-108">In the same way that some queries are run against a database that has tables and columns, a custom query works on Datasets that have columns and metrics.</span></span> <span data-ttu-id="7af6d-109">A lista completa de conjuntos de dados disponíveis para formular uma consulta pode ser encontrada usando a API de conjuntos de dados.</span><span class="sxs-lookup"><span data-stu-id="7af6d-109">The full list of available datasets for formulating a query can be obtained by using the datasets API.</span></span>

<span data-ttu-id="7af6d-110">Este é um exemplo de um conjuntos de dados mostrado como um JSON:</span><span class="sxs-lookup"><span data-stu-id="7af6d-110">This is an example of a dataset shown as a JSON:</span></span>

```json
{ 
      "datasetName": "OfficeUsage", 
      "selectableColumns": [ 
        "CustomerTenantId", 
        "CustomerTpid", 
        "WorkloadName", 
        "Month", 
        "PaidAvailableUnits", 
        "MonthlyActiveUsers", 
        "CustomerName", 
        "CustomerMarket", 
        "CustomerSegment",  
        "MPNId", 
        "PartnerName", 
        "PartnerLocation", 
        "PartnerAttributionType", 
        "IsDuplicateRowForPGA" 
      ], 
      "availableMetrics": [ 
        "CustomerCount", 
        "CustomerTenantCount", 
        "TotalPaidAvailableUnits", 
        "TotalMonthlyActiveUsers" 
      ], 
      "availableDateRanges": [ 
        "LAST_MONTH", 
        "LAST_3_MONTHS", 
        "LAST_6_MONTHS", 
        "LAST_1_YEAR", 
        "LIFETIME" 
      ], 
      "minimumRecurrenceInterval": 24 
    },
```

## <a name="parts-of-a-dataset"></a><span data-ttu-id="7af6d-111">Partes de um conjunto de dados</span><span class="sxs-lookup"><span data-stu-id="7af6d-111">Parts of a dataset</span></span>

- <span data-ttu-id="7af6d-112">Um nome de conjuntos de dados é como um nome de tabela de banco de dados.</span><span class="sxs-lookup"><span data-stu-id="7af6d-112">A dataset name is like a database table name.</span></span> <span data-ttu-id="7af6d-113">Por exemplo, OfficeUsage.</span><span class="sxs-lookup"><span data-stu-id="7af6d-113">For example, OfficeUsage.</span></span> <span data-ttu-id="7af6d-114">Um conjuntos de dados tem uma lista de colunas que podem ser selecionadas, como CustomerTenantId.</span><span class="sxs-lookup"><span data-stu-id="7af6d-114">A dataset has a list of columns that can be selected, such as CustomerTenantId.</span></span>
- <span data-ttu-id="7af6d-115">Um conjuntos de dados também tem métricas, que são como funções de agregação em um banco de dados.</span><span class="sxs-lookup"><span data-stu-id="7af6d-115">A dataset also has metrics, which are like aggregation functions in a database.</span></span> <span data-ttu-id="7af6d-116">Por exemplo, TotalMonthlyActiveUsers.</span><span class="sxs-lookup"><span data-stu-id="7af6d-116">For example, TotalMonthlyActiveUsers.</span></span>
- <span data-ttu-id="7af6d-117">Há períodos fixos nos quais os dados podem ser exportados.</span><span class="sxs-lookup"><span data-stu-id="7af6d-117">There are fixed time spans over which data can be exported.</span></span>

## <a name="formulating-a-query-on-a-dataset"></a><span data-ttu-id="7af6d-118">Formular uma consulta em um conjuntos de dados</span><span class="sxs-lookup"><span data-stu-id="7af6d-118">Formulating a query on a dataset</span></span>

<span data-ttu-id="7af6d-119">Essas são algumas consultas de exemplo, que mostram como extrair vários tipos de dados.</span><span class="sxs-lookup"><span data-stu-id="7af6d-119">These are some sample queries that show how to extract various types of data.</span></span>

|<span data-ttu-id="7af6d-120">Consulta</span><span class="sxs-lookup"><span data-stu-id="7af6d-120">Query</span></span>|    <span data-ttu-id="7af6d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="7af6d-121">Description</span></span>    |
|----|    ----    |
|<span data-ttu-id="7af6d-122">**SELECT** CustomerTenantId, PaidAvailableUnits **FROM**</span><span class="sxs-lookup"><span data-stu-id="7af6d-122">**SELECT** CustomerTenantId, PaidAvailableUnits **FROM**</span></span> <br><span data-ttu-id="7af6d-123">OfficeUsage **TIMESPAN** LAST_MONTH</span><span class="sxs-lookup"><span data-stu-id="7af6d-123">OfficeUsage **TIMESPAN** LAST_MONTH</span></span>|    <span data-ttu-id="7af6d-124">Essa consulta obterá todos os CusotmerTenantID e seus PaidAvailableUnits correspondentes no último mês.</span><span class="sxs-lookup"><span data-stu-id="7af6d-124">This query will get every CusotmerTenantID and its corresponding PaidAvailableUnits in the last 1 month.</span></span>    |
|<span data-ttu-id="7af6d-125">**SELECT** CustomerTenantId, PaidAvailableUnits **FROM**</span><span class="sxs-lookup"><span data-stu-id="7af6d-125">**SELECT** CustomerTenantId, PaidAvailableUnits **FROM**</span></span> <br><span data-ttu-id="7af6d-126">OfficeUsage **ORDER** BY PaidAvailableUnits **LIMIT** 10</span><span class="sxs-lookup"><span data-stu-id="7af6d-126">OfficeUsage **ORDER** BY PaidAvailableUnits **LIMIT** 10</span></span>|    <span data-ttu-id="7af6d-127">Essa consulta obterá os 10 principais locatários de clientes em ordem decrescente do número de unidades pagas disponíveis.</span><span class="sxs-lookup"><span data-stu-id="7af6d-127">This query will get the top 10 customer tenants in decreasing order of the number of paid available units.</span></span>     |
|<span data-ttu-id="7af6d-128">**SELECT** CustomerTenantId, PaidAvailableUnits, MonthlyActiveUsers **FROM** OfficeUsage **WHERE** MonthlyActiveUsers > 100000 **ORDER BY** MonthlyActiveUsers **TIMESPAN** LAST_6_MONTHS</span><span class="sxs-lookup"><span data-stu-id="7af6d-128">**SELECT** CustomerTenantId, PaidAvailableUnits, MonthlyActiveUsers **FROM** OfficeUsage **WHERE** MonthlyActiveUsers > 100000 **ORDER BY** MonthlyActiveUsers **TIMESPAN** LAST_6_MONTHS</span></span> |    <span data-ttu-id="7af6d-129">Essa consulta obterá PaidAvailableUnits e MonthlyActiveUsers de todos os Clientes que têm MonthlyActiveUsers maiores que 100.000.</span><span class="sxs-lookup"><span data-stu-id="7af6d-129">This query will get the PaidAvailableUnits and MonthlyActiveUsers of all the Customers who have MonthlyActiveUsers greater than 100,000.</span></span>     |
|<span data-ttu-id="7af6d-130">**SELECT** CustomerTenantId, Month, MonthlyActiveUsers **FROM**</span><span class="sxs-lookup"><span data-stu-id="7af6d-130">**SELECT** CustomerTenantId, Month, MonthlyActiveUsers **FROM**</span></span> <br><span data-ttu-id="7af6d-131">OfficeUsage **WHERE** CustomerTpId IN ('2a31c234-1f4e-4c60-909e-76d234f93161', '80780748-3f9a-11eb-b378-0242ac130002')</span><span class="sxs-lookup"><span data-stu-id="7af6d-131">OfficeUsage **WHERE** CustomerTpId IN ('2a31c234-1f4e-4c60-909e-76d234f93161', '80780748-3f9a-11eb-b378-0242ac130002')</span></span> |    <span data-ttu-id="7af6d-132">Essa consulta obterá o CustomerTenantId e os usuários ativos mensais para cada mês pelos dois valores CustomerTpId: '2a31c234-1f4e-4c60-909e-909e76d234f93161' e '80780748-3f9a-11eb-b378-0242ac130002'.</span><span class="sxs-lookup"><span data-stu-id="7af6d-132">This query will get the CustomerTenantId and the monthly active users for every month by the two CustomerTpId values: '2a31c234-1f4e-4c60-909e-76d234f93161' and '80780748-3f9a-11eb-b378-0242ac130002'.</span></span>     |
|        |        |

## <a name="query-specification"></a><span data-ttu-id="7af6d-133">Especificação da consulta</span><span class="sxs-lookup"><span data-stu-id="7af6d-133">Query specification</span></span>

<span data-ttu-id="7af6d-134">Esta seção descreve a definição e a estrutura da consulta.</span><span class="sxs-lookup"><span data-stu-id="7af6d-134">This section describes the query definition and structure.</span></span>

## <a name="grammar-reference"></a><span data-ttu-id="7af6d-135">Referência de gramática</span><span class="sxs-lookup"><span data-stu-id="7af6d-135">Grammar reference</span></span>

<span data-ttu-id="7af6d-136">Esta tabela descreve os símbolos usados em consultas.</span><span class="sxs-lookup"><span data-stu-id="7af6d-136">This table describes the symbols used in queries.</span></span>

|    <span data-ttu-id="7af6d-137">Consulta</span><span class="sxs-lookup"><span data-stu-id="7af6d-137">Query</span></span>    |    <span data-ttu-id="7af6d-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="7af6d-138">Description</span></span>    |
|    ----    |    ----    |
|    `?`    |    <span data-ttu-id="7af6d-139">Opcional</span><span class="sxs-lookup"><span data-stu-id="7af6d-139">Optional</span></span>    |
|    `*`    |    <span data-ttu-id="7af6d-140">Zero ou mais</span><span class="sxs-lookup"><span data-stu-id="7af6d-140">Zero or more</span></span>    |
|    `+`    |    <span data-ttu-id="7af6d-141">Um ou mais</span><span class="sxs-lookup"><span data-stu-id="7af6d-141">One or more</span></span>    |
|    `\|`    |    <span data-ttu-id="7af6d-142">Ou/Uma das listas</span><span class="sxs-lookup"><span data-stu-id="7af6d-142">Or / One of the lists</span></span>    |
|        |        |

## <a name="query-definition"></a><span data-ttu-id="7af6d-143">Definição da consulta</span><span class="sxs-lookup"><span data-stu-id="7af6d-143">Query definition</span></span>

<span data-ttu-id="7af6d-144">A instrução de consulta tem as seguintes cláusulas: SelectClause, FromClause, WhereClause, OrderClause, LimitClause e TimeSpan.</span><span class="sxs-lookup"><span data-stu-id="7af6d-144">The query statement has the following clauses: SelectClause, FromClause, WhereClause, OrderClause, LimitClause, and TimeSpan.</span></span>

- <span data-ttu-id="7af6d-145">**SelectClause:**`SELECT ColumOrMetricName (, ColumOrMetricName)*`</span><span class="sxs-lookup"><span data-stu-id="7af6d-145">**SelectClause**: `SELECT ColumOrMetricName (, ColumOrMetricName)*`</span></span>
    - <span data-ttu-id="7af6d-146">**ColumOrMetricName**: colunas e métricas definidas no conjunto de dados</span><span class="sxs-lookup"><span data-stu-id="7af6d-146">**ColumOrMetricName**: Columns and Metrics defined within the Dataset</span></span>
- <span data-ttu-id="7af6d-147">**FromClause:**`FROM DatasetName`</span><span class="sxs-lookup"><span data-stu-id="7af6d-147">**FromClause**: `FROM DatasetName`</span></span>
    - <span data-ttu-id="7af6d-148">**DataSetName**: nome do conjunto de dados definido no dentro do conjunto de dados</span><span class="sxs-lookup"><span data-stu-id="7af6d-148">**DatasetName**: Dataset name defined within the Dataset</span></span>
- <span data-ttu-id="7af6d-149">**WhereClause:**`WHERE FilterCondition (AND FilterCondition)`</span><span class="sxs-lookup"><span data-stu-id="7af6d-149">**WhereClause**: `WHERE FilterCondition (AND FilterCondition)`</span></span>
    - <span data-ttu-id="7af6d-150">**FilterCondition**: valor do operador ColumOrMetricName Operator Value</span><span class="sxs-lookup"><span data-stu-id="7af6d-150">**FilterCondition**: ColumOrMetricName Operator Value</span></span>
        - <span data-ttu-id="7af6d-151">**Operador**:  `=` | `>` | `<` | `>=` | `<=` | `!=` | `LIKE` | `NOT LIKE` | `IN` | `NOT IN`</span><span class="sxs-lookup"><span data-stu-id="7af6d-151">**Operator**:  `=` | `>` | `<` | `>=` | `<=` | `!=` | `LIKE` | `NOT LIKE` | `IN` | `NOT IN`</span></span>
        - <span data-ttu-id="7af6d-152">**Valor**: Number | StringLiteral | MultiNumberList | MultiStringList</span><span class="sxs-lookup"><span data-stu-id="7af6d-152">**Value**: Number | StringLiteral | MultiNumberList | MultiStringList</span></span>
            - <span data-ttu-id="7af6d-153">**Número**: `-? [0-9]+ (. [0-9] [0-9]*)?`</span><span class="sxs-lookup"><span data-stu-id="7af6d-153">**Number**: `-? [0-9]+ (. [0-9] [0-9]*)?`</span></span>
            - <span data-ttu-id="7af6d-154">**StringLiteral:**`' [a-zA-Z0-9_]*'`</span><span class="sxs-lookup"><span data-stu-id="7af6d-154">**StringLiteral**:  `' [a-zA-Z0-9_]*'`</span></span>
            - <span data-ttu-id="7af6d-155">**MultiNumberList:**`(Number (,Number)*)`</span><span class="sxs-lookup"><span data-stu-id="7af6d-155">**MultiNumberList**: `(Number (,Number)*)`</span></span>
            - <span data-ttu-id="7af6d-156">**MultiStringList:**`(StringLiteral (,StringLiteral)*)`</span><span class="sxs-lookup"><span data-stu-id="7af6d-156">**MultiStringList**: `(StringLiteral (,StringLiteral)*)`</span></span>
- <span data-ttu-id="7af6d-157">**OrderClause:**`ORDER BY OrderCondition (,OrderCondition)`</span><span class="sxs-lookup"><span data-stu-id="7af6d-157">**OrderClause**: `ORDER BY OrderCondition (,OrderCondition)`</span></span>
    - <span data-ttu-id="7af6d-158">**OrderCondition:**`ColumOrMetricName (ASC | DESC)*`</span><span class="sxs-lookup"><span data-stu-id="7af6d-158">**OrderCondition**: `ColumOrMetricName (ASC | DESC)*`</span></span>
- <span data-ttu-id="7af6d-159">**LimitClause:**`LIMIT [0-9]+`</span><span class="sxs-lookup"><span data-stu-id="7af6d-159">**LimitClause**: `LIMIT [0-9]+`</span></span>
- <span data-ttu-id="7af6d-160">**TimeSpan:**`TIMESPAN ( TODAY | YESTERDAY | LAST_7_DAYS | LAST_14_DAYS |LAST_30_DAYS | LAST_90_DAYS | LAST_180_DAYS | LAST_365_DAYS |LAST_MONTH | LAST_3_MONTHS | LAST_6_MONTHS | LAST_1_YEAR | LIFETIME)`</span><span class="sxs-lookup"><span data-stu-id="7af6d-160">**TimeSpan**: `TIMESPAN ( TODAY | YESTERDAY | LAST_7_DAYS | LAST_14_DAYS |LAST_30_DAYS | LAST_90_DAYS | LAST_180_DAYS | LAST_365_DAYS |LAST_MONTH | LAST_3_MONTHS | LAST_6_MONTHS | LAST_1_YEAR | LIFETIME)`</span></span>

## <a name="query-structure"></a><span data-ttu-id="7af6d-161">Estrutura da consulta</span><span class="sxs-lookup"><span data-stu-id="7af6d-161">Query Structure</span></span>

<span data-ttu-id="7af6d-162">Uma Consulta de relatório é constituída de várias partes:</span><span class="sxs-lookup"><span data-stu-id="7af6d-162">A Report query is made up of multiple parts:</span></span>
- `SELECT`
- `FROM`
- `WHERE`
- `ORDER BY`
- `LIMIT`
- `TIMESPAN`

<span data-ttu-id="7af6d-163">Veja a descrição de cada parte abaixo.</span><span class="sxs-lookup"><span data-stu-id="7af6d-163">Each part is described below.</span></span>

### `SELECT`

<span data-ttu-id="7af6d-164">Essa parte da consulta especifica as colunas que serão exportadas.</span><span class="sxs-lookup"><span data-stu-id="7af6d-164">This part of the query specifies the columns that will get exported.</span></span> <span data-ttu-id="7af6d-165">As colunas que podem ser selecionadas são os campos listados nas seções *selectableColumns* e *availableMetrics* de um conjuntos de dados.</span><span class="sxs-lookup"><span data-stu-id="7af6d-165">The columns that can be selected are the fields listed in *selectableColumns* and *availableMetrics* sections of a dataset.</span></span>

<span data-ttu-id="7af6d-166">Opcionalmente, `DISTINCT` a palavra-chave pode ser especificada após `SELECT` .</span><span class="sxs-lookup"><span data-stu-id="7af6d-166">Optionally, `DISTINCT` keyword can be specified after `SELECT`.</span></span> <span data-ttu-id="7af6d-167">Se for especificado, as linhas exportadas finais sempre conterão `DISTINCT` valores distintos das colunas selecionadas.</span><span class="sxs-lookup"><span data-stu-id="7af6d-167">If `DISTINCT` is specified, then the final exported rows will always contain distinct values of the selected columns.</span></span> <span data-ttu-id="7af6d-168">As métricas serão calculadas para cada combinação distinta das colunas selecionadas, portanto, a palavra-chave não é necessária quando uma coluna de métrica é incluída na `DISTINCT` lista selecionar colunas.</span><span class="sxs-lookup"><span data-stu-id="7af6d-168">Metrics will be calculated for every distinct combination of the selected columns, hence `DISTINCT` keyword is not required when a metric column is included in the select column list.</span></span>

<span data-ttu-id="7af6d-169">**Exemplo:**</span><span class="sxs-lookup"><span data-stu-id="7af6d-169">**Example:**</span></span>

```sql
SELECT CustomerTenantId, PaidAvailableUnits; 
SELECT DISTINCT CustomerTenantId
```

### `FROM`

<span data-ttu-id="7af6d-170">Essa parte da consulta indica o conjuntos de dados do qual os dados precisam ser exportados.</span><span class="sxs-lookup"><span data-stu-id="7af6d-170">This part of the query indicates the dataset from which data needs to be exported.</span></span> <span data-ttu-id="7af6d-171">O nome do conjuntos de dados aqui precisa ser um nome de conjuntos de dados válido, retornado pela API de conjuntos de dados.</span><span class="sxs-lookup"><span data-stu-id="7af6d-171">The dataset name given here needs to be a valid dataset name returned by the datasets API.</span></span>

<span data-ttu-id="7af6d-172">**Exemplo:**</span><span class="sxs-lookup"><span data-stu-id="7af6d-172">**Example:**</span></span>

- `FROM  OfficeUsage`
- `FROM  AzureUsage`

### `WHERE`

<span data-ttu-id="7af6d-173">Essa parte da consulta é usada para especificar condições de filtro no conjunto de dados.</span><span class="sxs-lookup"><span data-stu-id="7af6d-173">This part of the query is used to specify filter conditions on the dataset.</span></span> <span data-ttu-id="7af6d-174">Somente as linhas que corresponderem a todas as condições listadas nesta cláusula estarão presentes no arquivo exportado final.</span><span class="sxs-lookup"><span data-stu-id="7af6d-174">Only rows matching all the conditions listed in this clause will be present in the final exported file.</span></span> <span data-ttu-id="7af6d-175">A condição de filtro pode estar em qualquer uma das colunas listadas em *selectableColumns* *e availableMetrics*.</span><span class="sxs-lookup"><span data-stu-id="7af6d-175">The filter condition can be on any of the columns listed in *selectableColumns* and *availableMetrics*.</span></span> <span data-ttu-id="7af6d-176">Os valores especificados na condição de filtro podem ser uma lista de números ou uma lista de cadeias de caracteres somente quando o operador é `IN` ou `NOT IN`.</span><span class="sxs-lookup"><span data-stu-id="7af6d-176">The values specified in the filter condition can be a list of numbers or a list of strings only when the operator is `IN` or `NOT IN`.</span></span> <span data-ttu-id="7af6d-177">Os valores sempre podem ser fornecidos como uma cadeia de caracteres literal e serão convertidos para os tipos nativos de colunas.</span><span class="sxs-lookup"><span data-stu-id="7af6d-177">The values can always be given as a literal string and they will be converted to the native types of columns.</span></span> <span data-ttu-id="7af6d-178">Várias condições de filtro precisam ser separadas por uma operação AND.</span><span class="sxs-lookup"><span data-stu-id="7af6d-178">Multiple filter conditions need to be separated with an AND operation.</span></span>

<span data-ttu-id="7af6d-179">**Exemplo:**</span><span class="sxs-lookup"><span data-stu-id="7af6d-179">**Example:**</span></span>

- `CustomerTenantId= '868368da-957d-4959-8992-3c12dc7e6260'`
- `CustomerName LIKE '%Contoso%'`
- `CustomerId NOT IN (1000, 1001, 1002)`
- `OrderQuantity=100`
- `CustomerTenantId='7b487ac0-ce12-b732-dcd6-91a1e4e74a50' AND CustomerTpId=' 0f8b7fa0-eb83-a183-1225-ca153ef807aa'`

### `ORDER BY`

<span data-ttu-id="7af6d-180">Esta parte da consulta especifica os critérios de ordenação das linhas exportadas.</span><span class="sxs-lookup"><span data-stu-id="7af6d-180">This part of the query specifies the ordering criteria for the exported rows.</span></span> <span data-ttu-id="7af6d-181">As colunas nas quais a ordenação pode ser definida precisam ser de *selectableColumns* e *availableMetrics* do conjuntos de dados.</span><span class="sxs-lookup"><span data-stu-id="7af6d-181">The columns on which ordering can be defined need to be from the *selectableColumns* and *availableMetrics* of the dataset.</span></span> <span data-ttu-id="7af6d-182">Se não houver nenhuma direção de ordenação especificada, ela será padrão para DESC na coluna.</span><span class="sxs-lookup"><span data-stu-id="7af6d-182">If there is no ordering direction specified, it will be defaulted to DESC on the column.</span></span> <span data-ttu-id="7af6d-183">A ordenação pode ser definida em várias colunas, separando os critérios com uma vírgula.</span><span class="sxs-lookup"><span data-stu-id="7af6d-183">Ordering can be defined on multiple columns by separating the criteria with a comma.</span></span>

<span data-ttu-id="7af6d-184">**Exemplo:**</span><span class="sxs-lookup"><span data-stu-id="7af6d-184">**Example:**</span></span>

- `ORDER BY  MonthlyActiveUsers ASC,  Month DESC`
- `ORDER BY CustomerName ASC,  Month`

### `LIMIT`

<span data-ttu-id="7af6d-185">Essa parte da consulta especifica o número de linhas que serão exportadas.</span><span class="sxs-lookup"><span data-stu-id="7af6d-185">This part of the query specifies the number of rows that will be exported.</span></span> <span data-ttu-id="7af6d-186">O número especificado precisa ser um inteiro positivo diferente de zero.</span><span class="sxs-lookup"><span data-stu-id="7af6d-186">The number you specify needs to be a positive nonzero integer.</span></span>

### `TIMESPAN`

<span data-ttu-id="7af6d-187">Essa parte da consulta especifica o tempo de exportação dos dados.</span><span class="sxs-lookup"><span data-stu-id="7af6d-187">This part of the query specifies the time duration for which the data needs to be exported.</span></span> <span data-ttu-id="7af6d-188">Os valores possíveis devem ser do *campo availableDateRanges* na definição do conjuntos de dados.</span><span class="sxs-lookup"><span data-stu-id="7af6d-188">The possible values should be from the *availableDateRanges* field in the dataset definition.</span></span>

### <a name="case-sensitivity-in-query-specification"></a><span data-ttu-id="7af6d-189">Distinção de maiúsculas e minúsculas na especificação de consulta</span><span class="sxs-lookup"><span data-stu-id="7af6d-189">Case sensitivity in query specification</span></span>

<span data-ttu-id="7af6d-190">A especificação não diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="7af6d-190">The specification is completely case insensitive.</span></span> <span data-ttu-id="7af6d-191">Palavras-chave predefinidas, nomes de coluna e valores podem ser especificados usando letras maiúsculas ou minúsculas.</span><span class="sxs-lookup"><span data-stu-id="7af6d-191">Predefined keywords, column names and values can be specified using upper or lower case.</span></span>

## <a name="next-steps"></a><span data-ttu-id="7af6d-192">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="7af6d-192">Next steps</span></span>

- [<span data-ttu-id="7af6d-193">Lista de consultas do sistema</span><span class="sxs-lookup"><span data-stu-id="7af6d-193">List of system queries</span></span>](insights-programmatic-system-queries.md)
- [<span data-ttu-id="7af6d-194">Lista de consultas de exemplo</span><span class="sxs-lookup"><span data-stu-id="7af6d-194">List of sample queries</span></span>](insights-programmatic-sample-queries.md)