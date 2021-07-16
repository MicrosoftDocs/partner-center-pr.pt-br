---
title: EXCLUIR API de consultas de relatório – Insights dados
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Use essa API para excluir a consulta definida pelo usuário Partner Center insights.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: e608068613edad1fca277ba5886c9c4bc962ffd2
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114374792"
---
# <a name="delete-report-queries-api"></a>Excluir API de consultas de relatório

Essa API exclui consultas definidas pelo usuário.

**Sintaxe da solicitação**

|    Método    |    URI da solicitação    |
|    ----    |    ----    |
|    DELETE    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/{queryId}` |
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
|    queryId     |    string     |    No    |    Filtrar para obter detalhes somente de consultas com a ID fornecida neste argumento     |
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
      "QueryId": "string", 
      "Name": "string", 
      "Description": "string", 
      "Query": "string", 
      "Type": "string", 
      "User": "string", 
      "CreatedTime": "string", 
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
|    QueryId     |    UUID exclusivo da consulta que foi excluída    |
|    Nome     |    Nome da consulta que foi excluída    |
|    Descrição     |    Descrição da consulta excluída     |
|    Consulta     |    Cadeia de caracteres de consulta de relatório da consulta excluída    |
|    Tipo     |    Defina como userDefined para consultas criadas pelo usuário     |
|    Usuário     |    ID de usuário que criou a consulta     |
|    CreatedTime     |    Hora da criação da consulta     |
|    TotalCount     |    Número de conjuntos de dados na matriz de valores     |
|    Mensagem     |    Mensagem do status da execução da API     |
|    StatusCode     |    Código de resultado. Os valores possíveis são 200, 400, 401, 403, 500     |
|        |        |
