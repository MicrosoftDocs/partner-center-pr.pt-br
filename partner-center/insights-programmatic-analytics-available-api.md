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
# <a name="available-apis-for-partner-insights-analytics"></a><span data-ttu-id="f5a73-103">APIs disponíveis para análise de insights do parceiro</span><span class="sxs-lookup"><span data-stu-id="f5a73-103">Available APIs for partner insights analytics</span></span>

<span data-ttu-id="f5a73-104">A seguir, a lista de APIs para análise do parceiro insights e suas funcionalidades associadas.</span><span class="sxs-lookup"><span data-stu-id="f5a73-104">Following are the list of APIs for partner insights analytics and their associated functionalities.</span></span>

## <a name="dataset-pull-apis"></a><span data-ttu-id="f5a73-105">APIs pull do conjuntos de dados</span><span class="sxs-lookup"><span data-stu-id="f5a73-105">Dataset pull APIs</span></span>

<span data-ttu-id="f5a73-106">***Tabela 1: APIs pull do conjuntos de dados***</span><span class="sxs-lookup"><span data-stu-id="f5a73-106">***Table 1: Dataset pull APIs***</span></span>

| <span data-ttu-id="f5a73-107">**API**</span><span class="sxs-lookup"><span data-stu-id="f5a73-107">**API**</span></span> | <span data-ttu-id="f5a73-108">**Funcionalidade**</span><span class="sxs-lookup"><span data-stu-id="f5a73-108">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="f5a73-109">Obter todos os conjuntos de dados</span><span class="sxs-lookup"><span data-stu-id="f5a73-109">Get all datasets</span></span>](insights-programmatic-analytics-api-get-dataset.md) | <span data-ttu-id="f5a73-110">Obtém todos os conjuntos de dados disponíveis.</span><span class="sxs-lookup"><span data-stu-id="f5a73-110">Gets all the available datasets.</span></span> <span data-ttu-id="f5a73-111">Conjuntos de dados listam tabelas, colunas, métricas e intervalos de tempo.</span><span class="sxs-lookup"><span data-stu-id="f5a73-111">Datasets list the tables, columns, metrics, and time ranges.</span></span> |
|||

## <a name="query-management-apis"></a><span data-ttu-id="f5a73-112">APIs de gerenciamento de consulta</span><span class="sxs-lookup"><span data-stu-id="f5a73-112">Query management APIs</span></span>

<span data-ttu-id="f5a73-113">***Tabela 2: APIs de gerenciamento de consulta***</span><span class="sxs-lookup"><span data-stu-id="f5a73-113">***Table 2: Query management APIs***</span></span>

| <span data-ttu-id="f5a73-114">**API**</span><span class="sxs-lookup"><span data-stu-id="f5a73-114">**API**</span></span> | <span data-ttu-id="f5a73-115">**Funcionalidade**</span><span class="sxs-lookup"><span data-stu-id="f5a73-115">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="f5a73-116">Criar consulta de relatório</span><span class="sxs-lookup"><span data-stu-id="f5a73-116">Create Report Query</span></span>](insights-programmatic-access-paradigm.md#create-report-query-api) | <span data-ttu-id="f5a73-117">Cria consultas personalizadas que definem o conjunto de linhas do qual as colunas e métricas precisam ser exportadas.</span><span class="sxs-lookup"><span data-stu-id="f5a73-117">Creates custom queries that define the dataset from which columns and metrics need to be exported.</span></span> |
| [<span data-ttu-id="f5a73-118">OBTER consulta de relatório</span><span class="sxs-lookup"><span data-stu-id="f5a73-118">GET Report Query</span></span>](insights-programmatic-analytics-api-get-report-queries.md) | <span data-ttu-id="f5a73-119">Obtém todas as consultas disponíveis para uso em relatórios.</span><span class="sxs-lookup"><span data-stu-id="f5a73-119">Gets all the queries available for use in reports.</span></span> <span data-ttu-id="f5a73-120">Obtém todas as consultas definidas pelo sistema e pelo usuário por padrão.</span><span class="sxs-lookup"><span data-stu-id="f5a73-120">Gets all the system and user-defined queries by default.</span></span> |
| [<span data-ttu-id="f5a73-121">Excluir consulta de relatório</span><span class="sxs-lookup"><span data-stu-id="f5a73-121">DELETE Report Query</span></span>](insights-programmatic-analytics-api-delete-report-queries.md) | <span data-ttu-id="f5a73-122">Exclui consultas definidas pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="f5a73-122">Deletes user-defined queries.</span></span> |
|||

## <a name="report-management-apis"></a><span data-ttu-id="f5a73-123">APIs de gerenciamento de relatório</span><span class="sxs-lookup"><span data-stu-id="f5a73-123">Report management APIs</span></span>

<span data-ttu-id="f5a73-124">***Tabela 3: APIs de gerenciamento de relatório***</span><span class="sxs-lookup"><span data-stu-id="f5a73-124">***Table 3: Report management APIs***</span></span>

| <span data-ttu-id="f5a73-125">**API**</span><span class="sxs-lookup"><span data-stu-id="f5a73-125">**API**</span></span> | <span data-ttu-id="f5a73-126">**Funcionalidade**</span><span class="sxs-lookup"><span data-stu-id="f5a73-126">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="f5a73-127">Criar Relatório</span><span class="sxs-lookup"><span data-stu-id="f5a73-127">Create Report</span></span>](insights-programmatic-access-paradigm.md#create-report-api) | <span data-ttu-id="f5a73-128">Agenda uma consulta a ser executada em intervalos regulares.</span><span class="sxs-lookup"><span data-stu-id="f5a73-128">Schedules a query to be executed at regular intervals.</span></span> |
| [<span data-ttu-id="f5a73-129">TENTAR consulta de relatório</span><span class="sxs-lookup"><span data-stu-id="f5a73-129">TRY Report Query</span></span>](insights-programmatic-analytics-api-try-report-queries.md) | <span data-ttu-id="f5a73-130">Executa uma instrução de consulta de Relatório.</span><span class="sxs-lookup"><span data-stu-id="f5a73-130">Executes a Report query statement.</span></span> <span data-ttu-id="f5a73-131">Retorna apenas 10 registros que um parceiro pode usar para verificar se os dados são os esperados.</span><span class="sxs-lookup"><span data-stu-id="f5a73-131">Returns only 10 records that a partner can use to verify if the data is as expected.</span></span> |
| [<span data-ttu-id="f5a73-132">Obter relatório</span><span class="sxs-lookup"><span data-stu-id="f5a73-132">Get Report</span></span>](insights-programmatic-analytics-api-get-report.md) | <span data-ttu-id="f5a73-133">Obtém todos os relatórios que foram agendados.</span><span class="sxs-lookup"><span data-stu-id="f5a73-133">Get all the reports that have been scheduled.</span></span> |
| [<span data-ttu-id="f5a73-134">Atualizar relatório</span><span class="sxs-lookup"><span data-stu-id="f5a73-134">Update Report</span></span>](insights-programmatic-analytics-api-update-report.md) | <span data-ttu-id="f5a73-135">Modifique um parâmetro de relatório.</span><span class="sxs-lookup"><span data-stu-id="f5a73-135">Modify a report parameter.</span></span> |
| [<span data-ttu-id="f5a73-136">Excluir relatório</span><span class="sxs-lookup"><span data-stu-id="f5a73-136">Delete Report</span></span>](insights-programmatic-analytics-api-delete-report.md) | <span data-ttu-id="f5a73-137">Exclui todos os registros de execução de relatório e relatório.</span><span class="sxs-lookup"><span data-stu-id="f5a73-137">Deletes all the report and report execution records.</span></span> |
| [<span data-ttu-id="f5a73-138">Pausar execuções de relatório</span><span class="sxs-lookup"><span data-stu-id="f5a73-138">Pause Report Executions</span></span>](insights-programmatic-analytics-api-pause-report-executions.md) | <span data-ttu-id="f5a73-139">Pausa a execução agendada de relatórios.</span><span class="sxs-lookup"><span data-stu-id="f5a73-139">Pauses the scheduled execution of reports.</span></span> |
| [<span data-ttu-id="f5a73-140">Retomar execuções de relatório</span><span class="sxs-lookup"><span data-stu-id="f5a73-140">Resume Report Executions</span></span>](insights-programmatic-analytics-api-resume-report-executions.md) | <span data-ttu-id="f5a73-141">Retoma a execução agendada de relatórios pausados.</span><span class="sxs-lookup"><span data-stu-id="f5a73-141">Resumes the scheduled execution of a paused report.</span></span> |
|||

## <a name="report-execution-pull-apis"></a><span data-ttu-id="f5a73-142">APIs pull de execução de relatório</span><span class="sxs-lookup"><span data-stu-id="f5a73-142">Report execution pull APIs</span></span>

<span data-ttu-id="f5a73-143">***Tabela 4: APIs pull de execução de relatório***</span><span class="sxs-lookup"><span data-stu-id="f5a73-143">***Table 4: Report execution pull APIs***</span></span>

| <span data-ttu-id="f5a73-144">**API**</span><span class="sxs-lookup"><span data-stu-id="f5a73-144">**API**</span></span> | <span data-ttu-id="f5a73-145">**Funcionalidade**</span><span class="sxs-lookup"><span data-stu-id="f5a73-145">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="f5a73-146">Obter execuções de relatório</span><span class="sxs-lookup"><span data-stu-id="f5a73-146">Get Report Executions</span></span>](insights-programmatic-access-paradigm.md#get-report-execution-api) | <span data-ttu-id="f5a73-147">Obtém todas as execuções que ocorreram para um determinado relatório.</span><span class="sxs-lookup"><span data-stu-id="f5a73-147">Get all the executions that have happened for a given report.</span></span> |
|||

## <a name="next-steps"></a><span data-ttu-id="f5a73-148">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="f5a73-148">Next steps</span></span>

- <span data-ttu-id="f5a73-149">É possível experimentar as APIs por meio da [URL da API do Swagger](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html).</span><span class="sxs-lookup"><span data-stu-id="f5a73-149">You can try out the APIs through the [Swagger API URL](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html).</span></span>