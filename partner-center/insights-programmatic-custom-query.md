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
# <a name="custom-query-specification"></a>Especificação de consulta personalizada

Os parceiros podem usar essa especificação de consulta para formular facilmente consultas personalizadas para extrair dados de tabelas de análise. As consultas podem ser usadas para selecionar apenas as colunas e métricas desejadas que corresponderem a um determinado critério. No centro da especificação da linguagem está a definição de conjuntos de dados na qual uma consulta personalizada pode ser escrita.

## <a name="datasets"></a>Conjunto de dados

Da mesma forma que algumas consultas são executados em um banco de dados que tem tabelas e colunas, uma consulta personalizada funciona em conjuntos de dados que têm colunas e métricas. A lista completa de conjuntos de dados disponíveis para formular uma consulta pode ser encontrada usando a API de conjuntos de dados.

Este é um exemplo de um conjuntos de dados mostrado como um JSON:

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

## <a name="parts-of-a-dataset"></a>Partes de um conjunto de dados

- Um nome de conjuntos de dados é como um nome de tabela de banco de dados. Por exemplo, OfficeUsage. Um conjuntos de dados tem uma lista de colunas que podem ser selecionadas, como CustomerTenantId.
- Um conjuntos de dados também tem métricas, que são como funções de agregação em um banco de dados. Por exemplo, TotalMonthlyActiveUsers.
- Há períodos fixos nos quais os dados podem ser exportados.

## <a name="formulating-a-query-on-a-dataset"></a>Formular uma consulta em um conjuntos de dados

Essas são algumas consultas de exemplo, que mostram como extrair vários tipos de dados.

|Consulta|    Descrição    |
|----|    ----    |
|**SELECT** CustomerTenantId, PaidAvailableUnits **FROM** <br>OfficeUsage **TIMESPAN** LAST_MONTH|    Essa consulta obterá todos os CusotmerTenantID e seus PaidAvailableUnits correspondentes no último mês.    |
|**SELECT** CustomerTenantId, PaidAvailableUnits **FROM** <br>OfficeUsage **ORDER** BY PaidAvailableUnits **LIMIT** 10|    Essa consulta obterá os 10 principais locatários de clientes em ordem decrescente do número de unidades pagas disponíveis.     |
|**SELECT** CustomerTenantId, PaidAvailableUnits, MonthlyActiveUsers **FROM** OfficeUsage **WHERE** MonthlyActiveUsers > 100000 **ORDER BY** MonthlyActiveUsers **TIMESPAN** LAST_6_MONTHS |    Essa consulta obterá PaidAvailableUnits e MonthlyActiveUsers de todos os Clientes que têm MonthlyActiveUsers maiores que 100.000.     |
|**SELECT** CustomerTenantId, Month, MonthlyActiveUsers **FROM** <br>OfficeUsage **WHERE** CustomerTpId IN ('2a31c234-1f4e-4c60-909e-76d234f93161', '80780748-3f9a-11eb-b378-0242ac130002') |    Essa consulta obterá o CustomerTenantId e os usuários ativos mensais para cada mês pelos dois valores CustomerTpId: '2a31c234-1f4e-4c60-909e-909e76d234f93161' e '80780748-3f9a-11eb-b378-0242ac130002'.     |
|        |        |

## <a name="query-specification"></a>Especificação da consulta

Esta seção descreve a definição e a estrutura da consulta.

## <a name="grammar-reference"></a>Referência de gramática

Esta tabela descreve os símbolos usados em consultas.

|    Consulta    |    Descrição    |
|    ----    |    ----    |
|    `?`    |    Opcional    |
|    `*`    |    Zero ou mais    |
|    `+`    |    Um ou mais    |
|    `\|`    |    Ou/Uma das listas    |
|        |        |

## <a name="query-definition"></a>Definição da consulta

A instrução de consulta tem as seguintes cláusulas: SelectClause, FromClause, WhereClause, OrderClause, LimitClause e TimeSpan.

- **SelectClause:**`SELECT ColumOrMetricName (, ColumOrMetricName)*`
    - **ColumOrMetricName**: colunas e métricas definidas no conjunto de dados
- **FromClause:**`FROM DatasetName`
    - **DataSetName**: nome do conjunto de dados definido no dentro do conjunto de dados
- **WhereClause:**`WHERE FilterCondition (AND FilterCondition)`
    - **FilterCondition**: valor do operador ColumOrMetricName Operator Value
        - **Operador**:  `=` | `>` | `<` | `>=` | `<=` | `!=` | `LIKE` | `NOT LIKE` | `IN` | `NOT IN`
        - **Valor**: Number | StringLiteral | MultiNumberList | MultiStringList
            - **Número**: `-? [0-9]+ (. [0-9] [0-9]*)?`
            - **StringLiteral:**`' [a-zA-Z0-9_]*'`
            - **MultiNumberList:**`(Number (,Number)*)`
            - **MultiStringList:**`(StringLiteral (,StringLiteral)*)`
- **OrderClause:**`ORDER BY OrderCondition (,OrderCondition)`
    - **OrderCondition:**`ColumOrMetricName (ASC | DESC)*`
- **LimitClause:**`LIMIT [0-9]+`
- **TimeSpan:**`TIMESPAN ( TODAY | YESTERDAY | LAST_7_DAYS | LAST_14_DAYS |LAST_30_DAYS | LAST_90_DAYS | LAST_180_DAYS | LAST_365_DAYS |LAST_MONTH | LAST_3_MONTHS | LAST_6_MONTHS | LAST_1_YEAR | LIFETIME)`

## <a name="query-structure"></a>Estrutura da consulta

Uma Consulta de relatório é constituída de várias partes:
- `SELECT`
- `FROM`
- `WHERE`
- `ORDER BY`
- `LIMIT`
- `TIMESPAN`

Veja a descrição de cada parte abaixo.

### `SELECT`

Essa parte da consulta especifica as colunas que serão exportadas. As colunas que podem ser selecionadas são os campos listados nas seções *selectableColumns* e *availableMetrics* de um conjuntos de dados.

Opcionalmente, `DISTINCT` a palavra-chave pode ser especificada após `SELECT` . Se for especificado, as linhas exportadas finais sempre conterão `DISTINCT` valores distintos das colunas selecionadas. As métricas serão calculadas para cada combinação distinta das colunas selecionadas, portanto, a palavra-chave não é necessária quando uma coluna de métrica é incluída na `DISTINCT` lista selecionar colunas.

**Exemplo:**

```sql
SELECT CustomerTenantId, PaidAvailableUnits; 
SELECT DISTINCT CustomerTenantId
```

### `FROM`

Essa parte da consulta indica o conjuntos de dados do qual os dados precisam ser exportados. O nome do conjuntos de dados aqui precisa ser um nome de conjuntos de dados válido, retornado pela API de conjuntos de dados.

**Exemplo:**

- `FROM  OfficeUsage`
- `FROM  AzureUsage`

### `WHERE`

Essa parte da consulta é usada para especificar condições de filtro no conjunto de dados. Somente as linhas que corresponderem a todas as condições listadas nesta cláusula estarão presentes no arquivo exportado final. A condição de filtro pode estar em qualquer uma das colunas listadas em *selectableColumns* *e availableMetrics*. Os valores especificados na condição de filtro podem ser uma lista de números ou uma lista de cadeias de caracteres somente quando o operador é `IN` ou `NOT IN`. Os valores sempre podem ser fornecidos como uma cadeia de caracteres literal e serão convertidos para os tipos nativos de colunas. Várias condições de filtro precisam ser separadas por uma operação AND.

**Exemplo:**

- `CustomerTenantId= '868368da-957d-4959-8992-3c12dc7e6260'`
- `CustomerName LIKE '%Contoso%'`
- `CustomerId NOT IN (1000, 1001, 1002)`
- `OrderQuantity=100`
- `CustomerTenantId='7b487ac0-ce12-b732-dcd6-91a1e4e74a50' AND CustomerTpId=' 0f8b7fa0-eb83-a183-1225-ca153ef807aa'`

### `ORDER BY`

Esta parte da consulta especifica os critérios de ordenação das linhas exportadas. As colunas nas quais a ordenação pode ser definida precisam ser de *selectableColumns* e *availableMetrics* do conjuntos de dados. Se não houver nenhuma direção de ordenação especificada, ela será padrão para DESC na coluna. A ordenação pode ser definida em várias colunas, separando os critérios com uma vírgula.

**Exemplo:**

- `ORDER BY  MonthlyActiveUsers ASC,  Month DESC`
- `ORDER BY CustomerName ASC,  Month`

### `LIMIT`

Essa parte da consulta especifica o número de linhas que serão exportadas. O número especificado precisa ser um inteiro positivo diferente de zero.

### `TIMESPAN`

Essa parte da consulta especifica o tempo de exportação dos dados. Os valores possíveis devem ser do *campo availableDateRanges* na definição do conjuntos de dados.

### <a name="case-sensitivity-in-query-specification"></a>Distinção de maiúsculas e minúsculas na especificação de consulta

A especificação não diferencia maiúsculas de minúsculas. Palavras-chave predefinidas, nomes de coluna e valores podem ser especificados usando letras maiúsculas ou minúsculas.

## <a name="next-steps"></a>Próximas etapas

- [Lista de consultas do sistema](insights-programmatic-system-queries.md)
- [Lista de consultas de exemplo](insights-programmatic-sample-queries.md)