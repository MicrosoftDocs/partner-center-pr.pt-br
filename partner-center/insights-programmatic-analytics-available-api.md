---
title: Lista de APIs para acessar dados de informações de parceiros
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lista de APIs para acessar dados de informações de parceiros.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 71d04b6927e27b1d7a8d72bbdaa56b41cb113625
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114374847"
---
# <a name="available-apis-for-partner-insights-analytics"></a>APIs disponíveis para análise de insights do parceiro

A seguir, a lista de APIs para análise do parceiro insights e suas funcionalidades associadas.

## <a name="dataset-pull-apis"></a>APIs pull do conjuntos de dados

***Tabela 1: APIs pull do conjuntos de dados***

| **API** | **Funcionalidade** |
| --- | --- |
| [Obter todos os conjuntos de dados](insights-programmatic-analytics-api-get-dataset.md) | Obtém todos os conjuntos de dados disponíveis. Conjuntos de dados listam tabelas, colunas, métricas e intervalos de tempo. |
|||

## <a name="query-management-apis"></a>APIs de gerenciamento de consulta

***Tabela 2: APIs de gerenciamento de consulta***

| **API** | **Funcionalidade** |
| --- | --- |
| [Criar consulta de relatório](insights-programmatic-access-paradigm.md#create-report-query-api) | Cria consultas personalizadas que definem o conjunto de linhas do qual as colunas e métricas precisam ser exportadas. |
| [OBTER consulta de relatório](insights-programmatic-analytics-api-get-report-queries.md) | Obtém todas as consultas disponíveis para uso em relatórios. Obtém todas as consultas definidas pelo sistema e pelo usuário por padrão. |
| [Excluir consulta de relatório](insights-programmatic-analytics-api-delete-report-queries.md) | Exclui consultas definidas pelo usuário. |
|||

## <a name="report-management-apis"></a>APIs de gerenciamento de relatório

***Tabela 3: APIs de gerenciamento de relatório***

| **API** | **Funcionalidade** |
| --- | --- |
| [Criar Relatório](insights-programmatic-access-paradigm.md#create-report-api) | Agenda uma consulta a ser executada em intervalos regulares. |
| [TENTAR consulta de relatório](insights-programmatic-analytics-api-try-report-queries.md) | Executa uma instrução de consulta de Relatório. Retorna apenas 10 registros que um parceiro pode usar para verificar se os dados são os esperados. |
| [Obter relatório](insights-programmatic-analytics-api-get-report.md) | Obtém todos os relatórios que foram agendados. |
| [Atualizar relatório](insights-programmatic-analytics-api-update-report.md) | Modifique um parâmetro de relatório. |
| [Excluir relatório](insights-programmatic-analytics-api-delete-report.md) | Exclui todos os registros de execução de relatório e relatório. |
| [Pausar execuções de relatório](insights-programmatic-analytics-api-pause-report-executions.md) | Pausa a execução agendada de relatórios. |
| [Retomar execuções de relatório](insights-programmatic-analytics-api-resume-report-executions.md) | Retoma a execução agendada de relatórios pausados. |
|||

## <a name="report-execution-pull-apis"></a>APIs pull de execução de relatório

***Tabela 4: APIs pull de execução de relatório***

| **API** | **Funcionalidade** |
| --- | --- |
| [Obter execuções de relatório](insights-programmatic-access-paradigm.md#get-report-execution-api) | Obtém todas as execuções que ocorreram para um determinado relatório. |
|||

## <a name="next-steps"></a>Próximas etapas

- É possível experimentar as APIs por meio da [URL da API do Swagger](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html).