---
title: obter API de relatório-dados de Insights
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Use esta API para obter toda a ID de relatório disponível no Partner Center insights.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 174a2f60a36cb46b287b787b177dd32236cef4eb
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114374858"
---
# <a name="get-report-api"></a>Obter API de relatório

Esta API Obtém todos os relatórios que foram agendados.

**Sintaxe da solicitação**

|    Método    |    URI da solicitação    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport?reportId={Report ID}&reportName={Report Name}&queryId={Query ID}` |
|        |        |

**Cabeçalho da solicitação**

|    parâmetro    |    Tipo    |    Descrição    |
|    ----    |    ----    |    ----    |
|    Autorização    |    string    |    Obrigatórios. o token de acesso do Azure Active Directory (AAD) no formulário`Bearer <token>`    |
|    Tipo de conteúdo    |    string    |    `Application/JSON`    |
|        |        |        |

**Parâmetro de caminho**

Nenhum

**Parâmetro de consulta**

|    Nome do Parâmetro    |    Tipo    |    Obrigatório    |    Descrição    |
|    ----    |    ----    |    ----    |    ----    |
|    reportId     |    string    |    Não    |    Filtre para obter detalhes de apenas relatórios com o ReportID fornecido neste argumento     |
|    reportName     |    string    |    Não    |    Filtre para obter detalhes de apenas relatórios com o ReportName fornecido neste argumento     |
|    queryId     |    string    |    Não    |    Filtre para obter detalhes de apenas relatórios com a QueryId fornecida neste argumento     |
|        |        |        |        |


**Carga de solicitação**

Nenhum

**Glossário**

Não

**Resposta**

A carga de solicitação é estrutura conforme a seguir:

Código de resposta: 200, 400, 401, 403, 404, 500

Exemplo de conteúdo de resposta:

```json
{ 
  "Value": [ 
    { 
      "ReportId": "string", 
      "ReportName": "string", 
      "Description": "string", 
      "QueryId": "string", 
      "Query": "string", 
      "User": "string", 
      "CreatedTime": "string", 
      "ModifiedTime": "string", 
      "executeNow": true, 
      "StartTime": "string", 
      "ReportStatus": "string", 
      "RecurrenceInterval": 0, 
      " RecurrenceCount": 0, 
      "CallbackUrl": "string",
      "CallbackMethod": null,
      "Format": "string" 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0 
}
```

**Glossário**

Esta tabela define os principais elementos na resposta:

|    Parâmetro    |    Descrição    |
|    ----    |    ----    |
|    ReportId     |    UUID exclusivo do relatório que foi criado     |
|    ReportName     |    Nome fornecido ao relatório na carga de solicitação     |
|    Descrição     |    Descrição fornecida quando o relatório foi criado     |
|    QueryId     |    ID de consulta passada no momento da criação do relatório     |
|    Consulta     |    Texto da consulta que será executada para este relatório     |
|    Usuário     |    ID de usuário usada para criar o relatório     |
|    CreatedTime     |    Hora de criação do relatório. O formato de hora é aaaa-MM-ddTHH:mm:ssZ     |
|    ModifiedTime     |    Hora em que o relatório foi modificado pela última vez. O formato de hora é aaaa-MM-ddTHH:mm:ssZ     |
|    executeNow     |    Sinalizador ExecuteNow definido no momento em que o relatório foi criado    |
|    StartTime     |    A execução de tempo será iniciada. O formato de hora é aaaa-MM-ddTHH:mm:ssZ     |
|    ReportStatus     |    Status da execução do relatório. Os valores possíveis são Pausado, Ativo e Inativo.     |
|    RecurrenceInterval     |    Intervalo de recorrência fornecido durante a criação do relatório     |
|    RecurrenceCount     |    Contagem de recorrência fornecida durante a criação do relatório     |
|    CallbackUrl     |    URL de retorno de chamada fornecida na solicitação     |
|    CallbackMethod    |    Método de retorno de chamada fornecido na solicitação    |
|    Formatar     |    Formato dos arquivos do relatório     |
|    TotalCount     |    Número de conjuntos de dados na matriz de valores     |
|    Mensagem     |    Mensagem do status da execução da API     |
|    StatusCode     |    Código de resultado. Os valores possíveis são 200, 400, 401, 403, 500     |
|        |        |