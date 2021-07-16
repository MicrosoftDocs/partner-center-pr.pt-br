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
# <a name="programmatic-access-paradigm"></a>Paradigma do acesso programático

Este diagrama mostra o padrão de chamada de API usado para criar um novo modelo de relatório, agendar o relatório personalizado e recuperar dados de falha.

:::image type="content" source="images/insights/prog-acc-paradigm.png" alt-text="Fluxo de alto nível":::
***Figura 1: Fluxo de alto nível do padrão de chamada à API***

Esta lista fornece mais detalhes sobre a Figura 1.

1. O aplicativo cliente pode definir o esquema/modelo de relatório personalizado chamando a [API Criar relatório de consulta](#create-report-query-api). Como alternativa, você pode escolher um modelo de relatório (QueryId) nos exemplos de biblioteca de modelos de relatório listados [aqui.](insights-programmatic-system-queries.md)
2. Em caso de êxito, a API Criar Consulta de Relatório retorna a QueryId.
3. Em seguida, o aplicativo cliente precisa chamar a [API](#create-report-api) Criar Relatório usando a QueryId juntamente com a data de início do relatório, Intervalo de Repetição, Recorrência e um URI de Retorno de Chamada opcional.
4. Em Caso de êxito, [a API Criar Relatório](#create-report-api) retorna a ReportId.
5. O aplicativo cliente é notificado na URL de retorno de chamada assim que os dados do relatório estão prontos para download.
6. Em seguida, o aplicativo cliente usa a [API](#get-report-execution-api) Obter Execuções de Relatório para consultar o status do relatório com a ID do relatório e o intervalo de datas.
7. Em caso de sucesso, o link de download do relatório é retornado e o aplicativo pode iniciar o download dos dados.

## <a name="report-query-language-specification"></a>Especificação de linguagem de consulta de relatório

Embora forneçamos consultas [do sistema que](insights-programmatic-system-queries.md) você pode usar para criar relatórios, você também pode criar suas próprias consultas com base em suas necessidades de negócios. Para saber mais sobre consultas personalizadas, consulte [Especificação de consulta personalizada.](insights-programmatic-custom-query.md)

## <a name="create-report-query-api"></a>Criar API Criar relatório

A API ajuda a criar consultas personalizadas que definem o conjuntos de dados do qual colunas e métricas precisam ser exportadas. A API fornece a flexibilidade para criar um novo modelo de relatório com base nas necessidades de seus negócios.  

Também é possível usar as [consultas do sistema](insights-programmatic-system-queries.md) que fornecemos. Quando modelos de relatório personalizados não são necessários, você pode chamar Criar [API](#create-report-api) de Relatório diretamente usando as QueryIds das consultas do sistema fornecidas.  

O exemplo a seguir mostra como criar uma consulta personalizada para obter os 10 principais clientes por receita do mês passado.

### <a name="request-syntax"></a>Sintaxe da solicitação

|    Método     |    URI da solicitação     |
|----- | -----|
|    POST     |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries`|
|||

### <a name="request-header"></a>Cabeçalho da solicitação

|    parâmetro     |    Tipo     |    Descrição     |
|-------|-----|------|
|    Autorização     |    string |Obrigatórios. O token de acesso do Azure Active Directory (Azure AD). O formato é  `Bearer <token>` .|
|    Tipo de conteúdo     |string |`Application/JSON` |
||||

### <a name="path-parameter"></a>Parâmetro path

Nenhum

### <a name="query-parameter"></a>Parâmetro de consulta

Nenhum

### <a name="sample-request-payload"></a>Carga de solicitação de exemplo

```json
{ 
  "Name": "CustomersRevenueQuery", 
  "Description": "Query to get top 10 customers by revenue for last month", 
  "Query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH" 
}
```

### <a name="glossary"></a>Glossário

Esta tabela fornece as principais definições dos elementos da carga de solicitação.

|Parâmetro|    Obrigatório     |    Descrição     |    Valores Permitidos     |
|-----|    -----    |    -----    |    -----    |
|Nome |    Yes     |    Nome amigável da consulta     |    string     |
|    Descrição     |    Não     |    Descrição do que a consulta retorna     |    string     |
|    Consulta     |    Yes     |    Cadeia de caracteres de consulta de relatório     |    Tipo de dados: cadeia de caracteres <br> [Consulta personalizada](insights-programmatic-custom-query.md) com base na necessidade de negócios |
|        |        |        |        |

> [!Note]
> Para exemplos de consulta personalizada, consulte [Exemplos de consultas de exemplo.](insights-programmatic-sample-queries.md)

### <a name="sample-response"></a>Resposta de exemplo

A carga de solicitação é estrutura conforme a seguir:

Códigos de resposta: 200, 400, 401, 403, 500

Exemplo de conteúdo de resposta:

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

### <a name="glossary"></a>Glossário

Esta tabela fornece as principais definições dos elementos da carga de solicitação.

|    Parâmetro     |    Descrição     |
|    ----    |    ----    |
|    QueryId     |    UUID (identificador universal exclusivo) da consulta criada     |
|    Nome     |    Nome amigável fornecido à consulta na carga de solicitação     |
|    Descrição     |    Descrição fornecida durante a criação da consulta     |
|    Consulta     |    Consulta de relatório passada como entrada durante a criação da consulta     |
|    Tipo     |    Definida como `userDefined`     |
|    Usuário     |    ID de usuário usada para criar a consulta     |
|    CreatedTime     |    Hora UTC em que a consulta foi criada neste formato: aaaa-mm-ddThh:mm:ssZ     |
|    TotalCount     |    Número de conjuntos de dados na matriz de valores     |
|    StatusCode     |    Código de Resultado <br> Os valores possíveis são 200, 400, 401, 403, 500     |
|    message     |    Mensagem do status da execução da API     |
|        |        |

## <a name="create-report-api"></a>Criar API de relatório

Ao criar um modelo de relatório personalizado com êxito [](#create-report-query-api) e receber a QueryID como parte da resposta Criar Consulta de Relatório, essa API pode ser chamada para agendar uma consulta a ser executada em intervalos regulares. É possível definir uma frequência e um agendamento para o relatório a ser entregue.
Para consultas do sistema que fornecemos, a API criar relatório também pode ser chamada com [QueryId](insights-programmatic-system-queries.md).

### <a name="callback-url"></a>URL de retorno de chamada

A API de criação de relatório aceita uma URL de retorno de chamada. Essa URL será chamada depois que a geração de relatório for bem-sucedida. A URL de retorno de chamada deve estar acessível publicamente. Além da URL, um método de retorno de chamada também pode ser dado. O método de retorno de chamada só pode ser "GET" ou "POST". O método padrão se nenhum valor for passado será "POST". A reportId que concluiu a geração sempre será passada de volta durante o retorno de chamada.

Retorno de chamada POST: se a URL passada for `https://www.contosso.com/callback` , a URL chamada de volta será `https://www.contosso.com/callback/<reportID>` 

Retorno de chamada GET: se a URL passada for `https://www.contosso.com/callback` , a URL chamada de volta será `https://www.contosso.com/callback?reportId=<reportID>` 

### <a name="executenow-reports"></a>Relatórios do ExecuteNow

Há um provisionamento para gerar um relatório sem agendamento. O conteúdo da API de criação de relatório pode aceitar um parâmetro , que ensocará o relatório a ser gerado assim que a `ExecuteNow` API for chamada. Quando `ExecuteNow` é definido como true, os campos: , , são `StartTime` `RecurrenceCount` `RecurrenceInterval` ignorados, pois esses relatórios não são agendados.

Dois campos adicionais podem ser passados `ExecuteNow` quando for true e `QueryStartTime` `QueryEndTime` . Esses dois campos substituirão `TIMESPAN` o campo na consulta. Esses campos não são aplicáveis a relatórios agendados, pois os dados serão gerados continuamente por um período de tempo fixo que não muda.

### <a name="request-syntax"></a>Sintaxe da solicitação

|    Método     |    URI da solicitação     |
|----- | -----|
|    POST     |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport` |

### <a name="request-header"></a>Cabeçalho da solicitação

|    parâmetro     |    Tipo     |    Descrição     |
|-------|-----|------|
|    Autorização     |    string |Obrigatórios. O token de acesso do Azure Active Directory (Azure AD). O formato é  `Bearer <token>` .|
|    Tipo de conteúdo     |string |`Application/JSON` |

### <a name="path-parameter"></a>Parâmetro de caminho

Nenhum

### <a name="query-parameter"></a>Parâmetro de consulta

Nenhum

### <a name="sample-request-payload"></a>Carga de solicitação de exemplo

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

### <a name="glossary"></a>Glossário

As principais definições de elementos na carga de solicitação são articuladas abaixo:

|    Parâmetro     |    Obrigatório     |    Descrição     |    Valores Permitidos     |
|    ----    |    ----    |    ----    |    ----    |
|    ReportName     |    Yes     |    Nome a ser atribuído ao relatório     |    string     |
|    Descrição     |    Não     |    Descrição do relatório criado     |    string     |
|    QueryId     |    Yes     |    ID da consulta de relatório     |    string     |
|    StartTime     |    Yes     |    Carimbo de data/hora UTC no qual a geração de relatório será iniciada. <br> O formato deve ser: aaaa-mm-ddThh:mm:ssZ       |    string     |
|    ExecuteNow     |    Não     |    Esse parâmetro deve ser usado para criar um relatório que será executado apenas uma vez. `StartTime`, `RecurrenceInterval` e `RecurrenceCount` serão ignorados se isso estiver definido como true. O relatório é executado imediatamente de forma assíncrona     |    true/false     |
|    QueryStartTime     |    Não     |    Opcionalmente, especifica a hora de início para a consulta que extrai os dados. Esse parâmetro é aplicável somente a um relatório de execução única que `ExecuteNow` foi definido como true. Definir esse parâmetro substitui `TIMESPAN` determinadas na consulta. O formato deve ser: aaaa-MM-ddTHH:mm:ssZ     |    Carimbo de data/hora como cadeia de caracteres     |
|    QueryEndTime     |    Não     |    Opcionalmente, especifica a hora de início para a consulta que extrai os dados. Esse parâmetro é aplicável somente a um relatório de execução única que `ExecuteNow` foi definido como true. Definir esse parâmetro substitui `TIMESPAN` determinadas na consulta. O formato deve ser: aaaa-MM-ddTHH:mm:ssZ     |    Carimbo de data/hora como cadeia de caracteres     |
|    RecorrênciaInterval     |    Yes     |    Frequência em horas em que o relatório deve ser gerado. <br> O valor mínimo é 4 e o valor máximo é 2160.      |    Número inteiro     |
|    RecorrênciaCount     |    Não     |    Número de relatórios a serem gerados.     |    Número inteiro     |
|    Formatar     |    Não     |    Formato de arquivo do arquivo exportado. <br> O padrão é CSV.    |    "CSV"/"TSV"     |
|    CallbackUrl     |    Não     |    URL acessível publicamente que pode ser configurada opcionalmente como destino de retorno de chamada     |    Cadeia de caracteres (URL http)     |
|    CallbackMethod     |    Não     |    O método a ser usado para retorno de chamada     |    GET/POST     |
|        |        |        |        |

### <a name="sample-response"></a>Resposta de exemplo

A carga de solicitação é estrutura conforme a seguir:

Códigos de resposta: 200, 400, 401, 403, 404, 500

Exemplo de conteúdo de resposta:

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

### <a name="glossary"></a>Glossário

As principais definições de elementos na resposta são articuladas abaixo:

|    Parâmetro     |    Descrição     |
|    ----    |    ----    |
|    ReportId     |    UUID (identificador universal exclusivo) do relatório criado     |
|    ReportName     |    Nome fornecido ao relatório na carga de solicitação     |
|    Descrição     |    Descrição fornecida durante a criação do relatório     |
|    QueryId     |    ID de consulta passada no momento da criação do relatório     |
|    Consulta     |    Texto da consulta que será executada para este relatório     |
|    Usuário     |    ID de usuário usada para criar o relatório     |
|    CreatedTime     |    Hora UTC em que o relatório foi criado neste formato: aaaa-MM-ddTHH:mm:ssZ     |
|    ModifiedTime     |    Hora UTC em que o relatório foi modificado pela última vez neste formato: aaaa-MM-ddTHH:mm:ssZ     |
|    ExecuteNow     |    `ExecuteNow` sinalizador definido no momento em que o relatório foi criado     |
|    StartTime     |    Hora UTC em que a execução do relatório será iniciada neste formato: aaaa-MM-ddTHH:mm:ssZ     |
|    Reportstatus     |    Status da execução do relatório. Os valores possíveis `Paused` são `Active` , e `Inactive`     |
|    RecorrênciaInterval     |    Intervalo de recorrência fornecido durante a criação do relatório     |
|    RecorrênciaCount     |    Contagem de recorrência fornecida durante a criação do relatório.      |
|    CallbackUrl     |    URL de retorno de chamada fornecida na solicitação     |
|    CallbackMethod     |    Método de retorno de chamada fornecido na solicitação     |
|    Formatar     |    Formato dos arquivos de relatório. Os valores possíveis são `CSV` ou `TSV` .     |
|    TotalCount     |    Número de registros na matriz Value     |
|    StatusCode     |    Código de Resultado     |
|    message     |    Os valores possíveis são 200, 400, 401, 403, 500. Mensagem do status da execução da API     |
|        |        |

## <a name="get-report-execution-api"></a>Obter API de execução de relatório

Você pode usar esse método para consultar o status de uma execução de relatório usando a ReportId recebida de [Criar API de Relatório.](#create-report-api) O método retornará o link de download do relatório se o relatório estiver pronto para download. Caso contrário, o método retornará o status. Também é possível usar essa API para obter todas as execuções que ocorreram para um determinado relatório.  

>[!IMPORTANT]
>Essa API tem parâmetros de consulta padrão definidos para `executionStatus=Completed` e `getLatestExecution=true` . Portanto, chamar a API antes da primeira execução bem-sucedida do relatório retornará 404. Execuções pendentes podem ser obtidas pela configuração `executionStatus=Pending`.

### <a name="request-syntax"></a>Sintaxe da solicitação

|    Método     |    URI da solicitação     |
|----- | -----|
|    GET    |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/execution/{reportId}?executionId={executionId}&executionStatus={executionStatus}&getLatestExecution={getLatestExecution}`  |

### <a name="request-header"></a>Cabeçalho da solicitação

|    parâmetro     |    Tipo     |    Descrição     |
|-------|-----|------|
|    Autorização     |    string |Obrigatórios. O token de acesso do Azure Active Directory (Azure AD). O formato é  `Bearer <token>` .|
|    Tipo de conteúdo     |string |`Application/JSON` |

### <a name="path-parameter"></a>Parâmetro path

|    Nome do Parâmetro    |    Obrigatório    |    Type    |    Descrição    |
|    ----    |    ----    |    ----    |    ----    |
|    reportId    |    Sim    |    string    |    Filtre para obter detalhes de execução apenas de relatórios com a reportId fornecidas neste argumento. Várias reportIds podem ser especificadas separando-as com um ponto e vírgula ";".    |
|        |        |        |        |

### <a name="query-parameter"></a>Parâmetro de consulta

|    Nome do Parâmetro    |    Obrigatório    |    Type    |    Descrição    |
|    ----    |    ----    |    ----    |    ----    |
|    Executionid    |    Não    |    string    |    Filtre para obter detalhes apenas de relatórios com executionId determinado neste argumento. Várias executionIds podem ser especificadas separando-as com um ponto e vírgula ";".    |
|    Executionstatus    |    Não    |    Cadeia de caracteres/enum    |    Filtre para obter detalhes apenas de relatórios com executionStatus dado neste argumento. <br> Os valores válidos são: `Pending` `Running` , e `Paused` `Completed` . <br> O valor padrão é `Completed`. <br> Vários status podem ser especificados separando-os com um ponto e vírgula ";".    |
|    getLatestExecution    |    Não    |    booleano    |    A API retornará detalhes da execução mais recente. Por padrão, esse parâmetro é definido como true.<br> Se você optar por passar o valor desse parâmetro como false, a API retornará as últimas 90 dias de execução de instâncias.    |
|        |        |        |        |

### <a name="sample-request-payload"></a>Exemplo de carga de solicitação

Nenhum

### <a name="sample-response"></a>Exemplo de Resposta

A carga de solicitação é estrutura conforme a seguir:

Códigos de resposta: 200, 400, 401, 403, 404, 500

Exemplo de conteúdo de resposta:

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

Depois que a execução do relatório for concluída, o status de execução `Completed` será mostrado. É possível baixar o relatório selecionando a URL no `reportAccessSecureLink`.

### <a name="glossary"></a>Glossário

Principais definições dos elementos na resposta.

|    Parâmetro    |    Descrição    |
|    ----    |    ----    |
|    ExecutionId    |    UUID (identificador universal exclusivo) da instância de execução    |
|    ReportId    |    ID do relatório associada à instância de execução    |
|    RecurrenceInterval    |    Intervalo de recorrência fornecido durante a criação do relatório    |
|    RecurrenceCount    |    Contagem de recorrência fornecida durante a criação do relatório    |
|    CallbackUrl    |    URL de retorno de chamada associada à instância de execução    |
|    CallbackMethod    |    Método de retorno de chamada associado à instância de execução    |
|    Formatar    |    Formato do arquivo gerado no final da execução    |
|    ExecutionStatus    |    Status da instância de execução do relatório. <br> Os valores válidos são: `Pending`, `Running`, `Paused`, e `Completed`    |
|    ReportAccessSecureLink    |Link pelo qual o relatório pode ser acessado com segurança        |
|    ReportExpiryTime    |    Hora UTC após a qual o link do relatório expirará neste formato: aaaa-MM-ddTHH:mm:ssZ    |
|    ReportGeneratedTime    |    Hora UTC em que o relatório foi gerado neste formato: aaaa-MM-ddTHH:mm:ssZ    |
|    TotalCount    |    Número de conjuntos de dados na matriz de valores    |
|    StatusCode    |    Código de Resultado <br> Os valores possíveis são 200, 400, 401, 403, 404 e 500    |
|    message    |    Mensagem do status da execução da API    |
|        |        |

## <a name="next-steps"></a>Próximas etapas

- Experimente as APIs por meio da [URL da API do Swagger](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)
- [Faça sua primeira chamada à API](insights-programmatic-first-api-call.md)