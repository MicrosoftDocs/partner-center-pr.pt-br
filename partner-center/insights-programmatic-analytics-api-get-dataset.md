---
title: obter todos os conjuntos de dados API-Insights data
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Use esta API para obter detalhes de todos os conjuntos de resultados disponíveis nos insights do Partner Center.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 42ff7cc1f097e2423be5f1f7f9a7f62214d64949
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114374787"
---
# <a name="get-all-datasets-api"></a>API Obter todos os conjuntos de dados

A API Obter todos os conjuntos de dados obtém todos os conjuntos de dados disponíveis. Conjuntos de dados listam tabelas, colunas, métricas e intervalos de tempo.

**Sintaxe da solicitação**

|    Método    |    URI da solicitação    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledDataset?datasetName={Dataset Name}`     |
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
|    datasetName    |    string    |    No    |    Filtrar para obter detalhes de apenas um conjunto de dados    |
|        |        |        |        |

**Conteúdo da solicitação**

Nenhum

**Glossário**

Não

**Resposta**

A carga de solicitação é estrutura conforme a seguir:

Código de resposta: 200, 400, 401, 403, 404, 500

Exemplo de conteúdo de resposta:

```json
{ 
   "Value":[ 
      { 
         "DatasetName ":"string", 
         "SelectableColumns":[ 
            "string" 
         ], 
         "AvailableMetrics":[ 
            "string" 
         ], 
         "AvailableDateRanges":[ 
            "string" 
         ], 
         "minimumRecurrenceInterval":0 
      } 
   ], 
   "TotalCount":0, 
   "Message":"<Error Message>", 
   "StatusCode": 0, 
} 
```

**Glossário**

Esta tabela define os principais elementos na resposta:

|    Parâmetro    |    Descrição    |
|    ----    |    ----    |
|    DatasetName     |    Nome do conjunto de dados que este objeto de matriz define     |
|    SelectableColumns     |    Colunas brutas que podem ser especificadas nas colunas selecionadas     |
|    AvailableMetrics     |    Nomes de coluna de agregação/métrica que podem ser especificados nas colunas selecionadas     |
|    AvailableDateRanges     |    Intervalo de datas que pode ser usado em consultas de relatório para o conjunto de dados     |
|    minimumRecurrenceInterval     |    Valor mínimo do intervalo de recorrência     |
|    TotalCount     |    Número de conjuntos de dados na matriz de valores     |
|    Mensagem     |    Mensagem do status da execução da API     |
|    StatusCode     |    Código de resultado. Os valores possíveis são 200, 400, 401, 403, 500     |
|        |        |
