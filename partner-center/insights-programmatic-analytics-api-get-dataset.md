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
# <a name="get-all-datasets-api"></a><span data-ttu-id="1f585-103">API Obter todos os conjuntos de dados</span><span class="sxs-lookup"><span data-stu-id="1f585-103">Get all datasets API</span></span>

<span data-ttu-id="1f585-104">A API Obter todos os conjuntos de dados obtém todos os conjuntos de dados disponíveis.</span><span class="sxs-lookup"><span data-stu-id="1f585-104">The Get all datasets API gets all the available datasets.</span></span> <span data-ttu-id="1f585-105">Conjuntos de dados listam tabelas, colunas, métricas e intervalos de tempo.</span><span class="sxs-lookup"><span data-stu-id="1f585-105">Datasets list the tables, columns, metrics, and time ranges.</span></span>

<span data-ttu-id="1f585-106">**Sintaxe da solicitação**</span><span class="sxs-lookup"><span data-stu-id="1f585-106">**Request syntax**</span></span>

|    <span data-ttu-id="1f585-107">Método</span><span class="sxs-lookup"><span data-stu-id="1f585-107">Method</span></span>    |    <span data-ttu-id="1f585-108">URI da solicitação</span><span class="sxs-lookup"><span data-stu-id="1f585-108">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="1f585-109">GET</span><span class="sxs-lookup"><span data-stu-id="1f585-109">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledDataset?datasetName={Dataset Name}`     |
|        |        |

<span data-ttu-id="1f585-110">**Cabeçalho da solicitação**</span><span class="sxs-lookup"><span data-stu-id="1f585-110">**Request header**</span></span>

|    <span data-ttu-id="1f585-111">parâmetro</span><span class="sxs-lookup"><span data-stu-id="1f585-111">Header</span></span>    |    <span data-ttu-id="1f585-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f585-112">Type</span></span>    |    <span data-ttu-id="1f585-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f585-113">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="1f585-114">Autorização</span><span class="sxs-lookup"><span data-stu-id="1f585-114">Authorization</span></span>    |    <span data-ttu-id="1f585-115">string</span><span class="sxs-lookup"><span data-stu-id="1f585-115">string</span></span>    |    <span data-ttu-id="1f585-116">Obrigatórios.</span><span class="sxs-lookup"><span data-stu-id="1f585-116">Required.</span></span> <span data-ttu-id="1f585-117">o token de acesso do Azure Active Directory (AAD) no formulário`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="1f585-117">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="1f585-118">Tipo de conteúdo</span><span class="sxs-lookup"><span data-stu-id="1f585-118">Content-Type</span></span>    |    <span data-ttu-id="1f585-119">string</span><span class="sxs-lookup"><span data-stu-id="1f585-119">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="1f585-120">**Parâmetro de caminho**</span><span class="sxs-lookup"><span data-stu-id="1f585-120">**Path parameter**</span></span>

<span data-ttu-id="1f585-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1f585-121">None</span></span>

<span data-ttu-id="1f585-122">**Parâmetro de consulta**</span><span class="sxs-lookup"><span data-stu-id="1f585-122">**Query parameter**</span></span>

|    <span data-ttu-id="1f585-123">Nome do Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1f585-123">Parameter Name</span></span>    |    <span data-ttu-id="1f585-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f585-124">Type</span></span>    |    <span data-ttu-id="1f585-125">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="1f585-125">Required</span></span>    |    <span data-ttu-id="1f585-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f585-126">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="1f585-127">datasetName</span><span class="sxs-lookup"><span data-stu-id="1f585-127">datasetName</span></span>    |    <span data-ttu-id="1f585-128">string</span><span class="sxs-lookup"><span data-stu-id="1f585-128">string</span></span>    |    <span data-ttu-id="1f585-129">No</span><span class="sxs-lookup"><span data-stu-id="1f585-129">No</span></span>    |    <span data-ttu-id="1f585-130">Filtrar para obter detalhes de apenas um conjunto de dados</span><span class="sxs-lookup"><span data-stu-id="1f585-130">Filter to get details of only one dataset</span></span>    |
|        |        |        |        |

<span data-ttu-id="1f585-131">**Conteúdo da solicitação**</span><span class="sxs-lookup"><span data-stu-id="1f585-131">**Request payload**</span></span>

<span data-ttu-id="1f585-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1f585-132">None</span></span>

<span data-ttu-id="1f585-133">**Glossário**</span><span class="sxs-lookup"><span data-stu-id="1f585-133">**Glossary**</span></span>

<span data-ttu-id="1f585-134">Não</span><span class="sxs-lookup"><span data-stu-id="1f585-134">None</span></span>

<span data-ttu-id="1f585-135">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="1f585-135">**Response**</span></span>

<span data-ttu-id="1f585-136">A carga de solicitação é estrutura conforme a seguir:</span><span class="sxs-lookup"><span data-stu-id="1f585-136">The response payload is structured as follows:</span></span>

<span data-ttu-id="1f585-137">Código de resposta: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="1f585-137">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="1f585-138">Exemplo de conteúdo de resposta:</span><span class="sxs-lookup"><span data-stu-id="1f585-138">Response payload example:</span></span>

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

<span data-ttu-id="1f585-139">**Glossário**</span><span class="sxs-lookup"><span data-stu-id="1f585-139">**Glossary**</span></span>

<span data-ttu-id="1f585-140">Esta tabela define os principais elementos na resposta:</span><span class="sxs-lookup"><span data-stu-id="1f585-140">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="1f585-141">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1f585-141">Parameter</span></span>    |    <span data-ttu-id="1f585-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f585-142">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="1f585-143">DatasetName</span><span class="sxs-lookup"><span data-stu-id="1f585-143">DatasetName</span></span>     |    <span data-ttu-id="1f585-144">Nome do conjunto de dados que este objeto de matriz define</span><span class="sxs-lookup"><span data-stu-id="1f585-144">Name of the dataset that this array object defines</span></span>     |
|    <span data-ttu-id="1f585-145">SelectableColumns</span><span class="sxs-lookup"><span data-stu-id="1f585-145">SelectableColumns</span></span>     |    <span data-ttu-id="1f585-146">Colunas brutas que podem ser especificadas nas colunas selecionadas</span><span class="sxs-lookup"><span data-stu-id="1f585-146">Raw columns that can be specified in the select columns</span></span>     |
|    <span data-ttu-id="1f585-147">AvailableMetrics</span><span class="sxs-lookup"><span data-stu-id="1f585-147">AvailableMetrics</span></span>     |    <span data-ttu-id="1f585-148">Nomes de coluna de agregação/métrica que podem ser especificados nas colunas selecionadas</span><span class="sxs-lookup"><span data-stu-id="1f585-148">Aggregation/metric column names that can be specified in the select columns</span></span>     |
|    <span data-ttu-id="1f585-149">AvailableDateRanges</span><span class="sxs-lookup"><span data-stu-id="1f585-149">AvailableDateRanges</span></span>     |    <span data-ttu-id="1f585-150">Intervalo de datas que pode ser usado em consultas de relatório para o conjunto de dados</span><span class="sxs-lookup"><span data-stu-id="1f585-150">Date range that can be used in report queries for the dataset</span></span>     |
|    <span data-ttu-id="1f585-151">minimumRecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="1f585-151">minimumRecurrenceInterval</span></span>     |    <span data-ttu-id="1f585-152">Valor mínimo do intervalo de recorrência</span><span class="sxs-lookup"><span data-stu-id="1f585-152">Minimum value of Recurrence Interval</span></span>     |
|    <span data-ttu-id="1f585-153">TotalCount</span><span class="sxs-lookup"><span data-stu-id="1f585-153">TotalCount</span></span>     |    <span data-ttu-id="1f585-154">Número de conjuntos de dados na matriz de valores</span><span class="sxs-lookup"><span data-stu-id="1f585-154">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="1f585-155">Mensagem</span><span class="sxs-lookup"><span data-stu-id="1f585-155">Message</span></span>     |    <span data-ttu-id="1f585-156">Mensagem do status da execução da API</span><span class="sxs-lookup"><span data-stu-id="1f585-156">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="1f585-157">StatusCode</span><span class="sxs-lookup"><span data-stu-id="1f585-157">StatusCode</span></span>     |    <span data-ttu-id="1f585-158">Código de resultado.</span><span class="sxs-lookup"><span data-stu-id="1f585-158">Result Code.</span></span> <span data-ttu-id="1f585-159">Os valores possíveis são 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="1f585-159">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
