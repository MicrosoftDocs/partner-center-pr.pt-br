---
title: Excluir API de relatório – Insights dados
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Use essa API para excluir qualquer relatório no Partner Center insights.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: e060104f8f09f69c213ab1b22d4be08d58babced
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114374862"
---
# <a name="delete-report-api"></a>Excluir API de relatório

Na execução, essa API exclui todos os relatórios e registros de execução do relatório.

**Sintaxe da solicitação**

|    Método    |    URI da solicitação    |
|    ----    |    ----    |
|    DELETE    |    ` https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
|        |        |

**Cabeçalho da solicitação**

|    parâmetro    |    Tipo    |    Descrição    |
|    ----    |    ----    |    ----    |
|    Autorização    |    string    |    Obrigatórios. O token de acesso Azure Active Directory (AAD) no formulário`Bearer <token>`    |
|    Tipo de conteúdo    |    string    |    `Application/JSON`    |
|        |        |        |

**Parâmetro de caminho**

|    Nome do Parâmetro    |    Tipo    |    Obrigatório    |    Descrição    |
|    ----    |    ----    |    ----    |    ----    |
|    reportId     |    string    |    Não    |    ID do relatório que está sendo excluído    |
|        |        |        |        |

**Parâmetro de consulta**

Nenhum

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
      "ExecuteNow": true, 
      "StartTime": "string", 
      "ReportStatus": "string", 
      "RecurrenceInterval": 0, 
      "RecurrenceCount": 0, 
      "CallbackUrl": "string",
      "CallbackMethod": "string",
      "Format": "string" 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0, 
} 
```

**Glossário**

Esta tabela define os principais elementos na resposta:

|    Parâmetro    |    Descrição    |
|    ----    |    ----    |
|    ReportId     |    Identificador universal exclusivo (UUID) do relatório excluído     |
|    ReportName     |    Nome dado ao relatório durante a criação     |
|    Descrição     |    Descrição fornecida durante a criação do relatório     |
|    QueryId     |    ID de consulta passada no momento da criação do relatório     |
|    Consulta     |    Texto da consulta que será executada para este relatório     |
|    Usuário     |    ID de usuário usada para criar o relatório     |
|    CreatedTime     |    Hora de criação do relatório. O formato de hora é aaaa-MM-ddTHH:mm:ssZ     |
|    ModifiedTime     |    Hora em que o relatório foi modificado pela última vez. O formato de hora é aaaa-MM-ddTHH:mm:ssZ     |
|    ExecuteNow     |    Sinalizador ExecuteNow definido no momento em que o relatório foi criado     |
|    StartTime     |    Hora em que a execução do relatório será iniciada. O formato de hora é aaaa-MM-ddTHH:mm:ssZ     |
|    Reportstatus     |    Status da execução do relatório. Os valores possíveis são Pausado, Ativo e Inativo.     |
|    RecorrênciaInterval     |    Intervalo de recorrência fornecido durante a criação do relatório     |
|    RecorrênciaCount     |    Contagem de recorrência fornecida durante a criação do relatório     |
|    CallbackUrl     |    URL de retorno de chamada fornecida na solicitação     |
|    CallbackMethod    |    Método de retorno de chamada fornecido na solicitação    |
|    Formatar     |    Formato dos arquivos do relatório     |
|    TotalCount     |    Número de conjuntos de dados na matriz de valores     |
|    Mensagem     |    Mensagem do status da execução da API     |
|    StatusCode     |    Código de resultado. Os valores possíveis são 200, 400, 401, 403, 500     |
|        |        |
