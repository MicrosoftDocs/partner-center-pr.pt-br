---
title: obter consultas de relatório Insights dados da API
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Use essa API para obter todas as consultas disponíveis para uso na API de relatório.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 3bf140576a19439990405cfef23190045e0a98be
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114374859"
---
# <a name="get-report-queries-api"></a>Obter API de consultas de relatório

A API obter consultas de relatório obtém todas as consultas que estão disponíveis para uso em relatórios. Ela obtém todas as consultas definidas pelo sistema e pelo usuário por padrão.

**Sintaxe da solicitação**

|    Método    |    URI da solicitação    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries?queryId={QueryID}&queryName={QueryName}&includeSystemQueries={include_system_queries}&includeOnlySystemQueries={include_only_system_queries}`     |
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
|    queryId     |    string     |    No    |    Filtrar para obter detalhes somente de consultas com a ID fornecida neste argumento     |
|    queryName     |    string     |    No    |    Filtrar para obter detalhes somente de consultas com o nome fornecido neste argumento     |
|    IncludeSystemQueries     |    booleano     |    No    |    Incluir consultas de sistema predefinidas na resposta     |
|    IncludeOnlySystemQueries     |    booleano     |    No    |    Incluir somente consultas de sistema na resposta     |
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
|    QueryId     |    UUID exclusivo da consulta     |
|    Nome     |    Nome fornecido à consulta no momento da criação da consulta     |
|    Descrição     |    Descrição fornecida durante a criação da consulta     |
|    Consulta     |    Cadeia de caracteres de consulta de relatório     |
|    Tipo     |    Definido como UserDefined para consultas criadas pelo usuário e para o sistema para consultas de sistema predefinidas     |
|    Usuário     |    ID de usuário que criou a consulta     |
|    CreatedTime     |    Hora da criação da consulta     |
|    TotalCount     |    Número de conjuntos de dados na matriz de valores     |
|    Mensagem     |    Mensagem do status da execução da API     |
|    StatusCode     |    Código de resultado. Os valores possíveis são 200, 400, 401, 403, 500     |
|        |        |
