---
title: Experimentar API de consultas de relatório
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Use essa API para testar sua consulta e validar os resultados em Partner Center insights.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 13ad6fe385a4d31390b6806d863da3f647105b2c
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114374851"
---
# <a name="try-report-queries-api"></a>Experimentar API de consultas de relatório

Essa API executa uma instrução de consulta de relatório. A API retorna apenas 100 registros que você como parceiro pode usar para verificar se os dados são conforme o esperado.

> [!IMPORTANT]
> Essa API tem um tempo limite de execução de consulta de 100 segundos. Se você observar que a API está demorando mais de 100 segundos, é muito provável que a consulta esteja sintaticamente correta ou, caso contrário, você receberia um código de erro diferente de 200. A geração de relatório real será aprovada se a sintaxe da consulta estiver correta.

**Sintaxe da solicitação**

|    Método    |    URI da solicitação    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/testQueryResult?<exportQuery={query text}|queryId={queryId}>`    |
|        |        |

**Cabeçalho da solicitação**

|    parâmetro    |    Tipo    |    Descrição    |
|    ----    |    ----    |    ----    |
|    Autorização    |    string    |    Obrigatórios. O token de acesso Azure Active Directory (AAD) no formulário`Bearer <token>`    |
|    Tipo de conteúdo    |    string    |    `Application/JSON`    |
|        |        |        |

**Parâmetro de caminho**

Nenhum

**Parâmetro de consulta**

|    Nome do Parâmetro    |    Tipo    |    Obrigatório    |    Descrição    |
|    ----    |    ----    |    ----    |    ----    |
|    exportQuery     |    string    |    Não    |    Cadeia de caracteres de consulta de relatório que precisa ser executada     |
|    queryId     |    string    |    Não    |    Uma ID de consulta existente válida. Mutuamente exclusivo com a cadeia de caracteres de consulta especificada no parâmetro exportQuery    |
|    startTime     |    string    |    Não    |    Hora de início da qual queremos os dados. Ele substitui o período de tempo especificado na consulta    |
|    endTime     |    string    |    Não    |    Hora de término até a qual desejamos os dados. Ele substitui o período de tempo especificado na consulta    |
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
Top 100 rows of query execution 
{ 
  "Value": [ 
    { 
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
|    TotalCount     |    Número de conjuntos de dados na matriz de valores     |
|    Mensagem     |    Mensagem do status da execução da API     |
|    StatusCode     |    Código de resultado. Os valores possíveis são 200, 400, 401, 403, 500     |
|        |        |
