---
title: Atualizar API de relatório
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Use esta API para atualizar parâmetros de relatório no Partner Center insights.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: c5ab1059e9be9b42918d268da6a6c1a3cbfe52af
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114374850"
---
# <a name="update-report-api"></a>Atualizar API de relatório

Essa API ajuda a modificar um parâmetro de relatório.

**Sintaxe da solicitação**

|    Método    |    URI da solicitação    |
|    ----    |    ----    |
|    PUT    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
|        |        |

**Cabeçalho da solicitação**

|    parâmetro    |    Tipo    |    Descrição    |
|    ----    |    ----    |    ----    |
|    Autorização    |    string    |    Obrigatórios. o token de acesso do Azure Active Directory (AAD) no formulário`Bearer <token>`    |
|    Tipo de conteúdo    |    string    |    `Application/JSON`    |
|        |        |        |

**Parâmetro de caminho**

|    Nome do Parâmetro    |    Tipo    |    Obrigatório    |    Descrição    |
|    ----    |    ----    |    ----    |    ----    |
|    reportId     |    string    |    Não    |    ID do relatório que está sendo modificado     |
|        |        |        |        |

**Parâmetro de consulta**

Nenhum

**Carga de solicitação**

```json
{ 
  "ReportName": "string", 
  "Description": "string", 
  "StartTime": "string", 
  "RecurrenceInterval": 0, 
  "RecurrenceCount": 0, 
  "Format": "string", 
  "CallbackUrl": "string",
 "CallbackMethod": "string"
}
```

**Glossário**

Esta tabela lista as principais definições dos elementos da resposta.

|    Parâmetro    |    Obrigatório    |    Descrição    |    Valores Permitidos    |
|    ----    |    ----    |    ----    |    ----    |
|    ReportName     |    Yes     |    Nome a ser atribuído ao relatório     |    String     |
|    Descrição     |    Não     |    Descrição do relatório criado     |    String     |
|    StartTime     |    Yes    |    Carimbo de data/hora após o qual a geração de relatório será iniciada     |    String     |
|    RecurrenceInterval     |    No     |    Frequência em horas em que o relatório deve ser gerado. O valor mínimo é 4     |    Integer     |
|    RecurrenceCount     |    Não     |    Números de relatório a ser gerado. O padrão é indefinido.     |    Integer     |
|    Formatar     |    Não    |    Formato de arquivo do arquivo exportado. O padrão é CSV     |    CSV/TSV     |
|    CallbackURL     |    Não     |    URL de retorno de chamada https a ser chamada na geração de relatório     |    String     |
|    CallbackMethod    |    Não    |    Método http a ser usado para retorno de chamada    |    OBTER/POSTAR    |
|        |        |        |        |


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
|    ReportId     |    UUID (identificador universal exclusivo) do relatório sendo atualizado     |
|    ReportName     |    Nome fornecido ao relatório na carga de solicitação     |
|    Descrição     |    Descrição fornecida ao relatório na carga de solicitação     |
|    QueryId     |    ID de consulta passada no momento da criação do relatório     |
|    Consulta     |    Texto da consulta que será executada para este relatório     |
|    Usuário     |    ID de usuário usada para criar o relatório     |
|    CreatedTime     |    Hora de criação do relatório. O formato de hora é aaaa-MM-ddTHH:mm:ssZ     |
|    ModifiedTime     |    Hora em que o relatório foi modificado pela última vez. O formato de hora é aaaa-MM-ddTHH:mm:ssZ     |
|    ExecuteNow     |    Sinalizador ExecuteNow definido no momento em que o relatório foi criado    |
|    StartTime     |    Hora em que a execução do relatório será iniciada. O formato de hora é aaaa-MM-ddTHH:mm:ssZ     |
|    Reportstatus     |    Status da execução do relatório. Os valores possíveis são Pausado, Ativo e Inativo.     |
|    RecorrênciaInterval     |    Intervalo de recorrência fornecido no payload da solicitação     |
|    RecorrênciaCount     |    Contagem de recorrência fornecida no payload da solicitação     |
|    CallbackUrl     |    URL de retorno de chamada fornecida na solicitação     |
|    CallbackMethod    |    Método de retorno de chamada fornecido na solicitação    |
|    Formatar     |    Formato dos arquivos do relatório     |
|    TotalCount     |    Número de conjuntos de dados na matriz de valores     |
|    Mensagem     |    Mensagem do status da execução da API     |
|    StatusCode     |    Código de resultado. Os valores possíveis são 200, 400, 401, 403, 500     |
|        |        |