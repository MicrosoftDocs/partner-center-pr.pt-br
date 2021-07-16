---
title: Perguntas comuns sobre o acesso programático do Partner Insights
description: Obter respostas para perguntas frequentes sobre como acessar dados de insights de parceiros por meio da API.
ms.topic: troubleshooting
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 5645a834c2b6a84920ba032198f7f62aa1487c47
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114374842"
---
# <a name="programmatic-access-of-analytics-data-common-questions"></a>Perguntas comuns sobre acesso programático a dados de análise

Este artigo aborda as perguntas frequentes sobre como acessar programaticamente os dados do Partner Insights Partner Center.

## <a name="api-responses"></a>Respostas da API

Quais são os diferentes cenários sob os quais posso receber uma resposta de API diferente de 200 (êxito)?

Esta tabela descreve as respostas da API e o que fazer se você as receber.

|    Descrição do erro     |    Código do erro     |    Solucionar problemas     |
|    ----    |    ----    |    ----    |
|    Não Autorizado     |    401     |    Esta é uma exceção de autenticação. Verifique a correção do token Azure Active Directory (AAD). O token do AAD é válido por 60 minutos, após o qual você precisaria regenerar o token do AAD.     |
|    Nome de tabela inválido     |    400     |    O nome do conjunto de dados está errado. Verifique novamente o nome do conjuntos de dados chamando a API "Obter Todos os Conjuntos de Dados".     |
|    Nome de coluna incorreto     |    400     |    O nome da coluna na consulta está incorreto. Verifique novamente o nome da coluna chamando a API "Obter Todos os Conjuntos de Dados" ou consulte os nomes de coluna nas Definições de Dados    |
|    Valor nulo ou ausente     |    400     |    Você pode estar ignorando parâmetros obrigatórios como parte do conteúdo solicitado pela API.     |
|    Parâmetros de relatório inválidos     |    400     |    Verifique se os parâmetros de relatório estão corretos. Por exemplo, você pode estar dando um valor menor que 4 para o parâmetro RecurrenceInterval.     |
|    O intervalo de recorrência deve estar entre 4 e 2160     |    400     |    Certifique-se de que o valor do parâmetro de solicitação RecurrenceInterval esteja entre 4 e 2160.     |
|    QueryId Inválido     |    400     |    Verifique novamente a QueryId gerada.     |
|    Parâmetros de relatório inválidos para criação – a hora de início do relatório deve ser pelo menos 4 horas a partir da hora UTC atual     |    400     |    O parâmetro Hora de Início como parte do payload da solicitação não deve estar no passado. A hora de início do relatório deve ser pelo menos 4 horas a partir da hora UTC atual.     |
|    Valor solicitado 'string' não encontrado     |    400     |    Verifique se você atualizou os parâmetros de solicitação `callbackurl` ou o formato.     |
|    Nenhum item encontrado com os filtros informados.     |    404     |    Verifique o parâmetro reportID usado na API Obter Execuções de Relatório.     |
|    Não há ocorrência de relatórios com os filtros informados. Verifique a reportId ou executionId e repetir a API após o tempo de execução agendado do relatório     |    404     |    Certifique-se de que a reportId está correta. Repetir a API após o tempo de execução agendado do relatório, conforme especificado no conteúdo da solicitação.     |
|    Encontrado um erro interno ao criar o relatório. ID de correlação <>     |    500     |    Certifique-se de que o formato de data para os campos *StartTime,* *QueryStartTime* e *QueryEndTime* está correto.     |
|    Serviço indisponível    |    500     |    Se você receber continuamente um serviço indisponível (erro 5xx), abra um tíquete de suporte.    |
|        |        |        |

## <a name="no-records"></a>Sem registros

Eu recebo a resposta 200 da API quando faço o download do relatório a partir do local seguro. Por que eu não recebo nenhum registro?
Verifique se a cadeia de caracteres na consulta tem um dos valores permitidos para o cabeçalho da coluna. Por exemplo, essa consulta retornará zero resultados:

```sql
SELECT CustomerTenantId, CustomerTpId, WorkloadName, Month, MonthlyActiveUsers 
FROM OfficeUsage 
WHERE IsDuplicateRowForPGA = 'False' 
ORDER BY CustomerTenantId DESC
```

Neste exemplo, os valores permiteis para `IsDuplicateRowForPGA` são 0 ou 1. Consulte as [Definições de Dados](insights-data-definitions.md) para ver todos os valores possíveis para as várias colunas.
