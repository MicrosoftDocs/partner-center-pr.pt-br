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
# <a name="try-report-queries-api"></a><span data-ttu-id="5f6cd-103">Experimentar API de consultas de relatório</span><span class="sxs-lookup"><span data-stu-id="5f6cd-103">Try report queries API</span></span>

<span data-ttu-id="5f6cd-104">Essa API executa uma instrução de consulta de relatório.</span><span class="sxs-lookup"><span data-stu-id="5f6cd-104">This API executes a Report query statement.</span></span> <span data-ttu-id="5f6cd-105">A API retorna apenas 100 registros que você como parceiro pode usar para verificar se os dados são conforme o esperado.</span><span class="sxs-lookup"><span data-stu-id="5f6cd-105">The API returns only 100 records that you as a partner can use to verify if the data is as you expected.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="5f6cd-106">Essa API tem um tempo limite de execução de consulta de 100 segundos.</span><span class="sxs-lookup"><span data-stu-id="5f6cd-106">This API has a query execution timeout of 100 seconds.</span></span> <span data-ttu-id="5f6cd-107">Se você observar que a API está demorando mais de 100 segundos, é muito provável que a consulta esteja sintaticamente correta ou, caso contrário, você receberia um código de erro diferente de 200.</span><span class="sxs-lookup"><span data-stu-id="5f6cd-107">If you notice the API is taking more than 100 seconds, it is highly likely that the query is syntactically correct or else you would have received an error code other than 200.</span></span> <span data-ttu-id="5f6cd-108">A geração de relatório real será aprovada se a sintaxe da consulta estiver correta.</span><span class="sxs-lookup"><span data-stu-id="5f6cd-108">The actual report generation will pass if the query syntax is correct.</span></span>

<span data-ttu-id="5f6cd-109">**Sintaxe da solicitação**</span><span class="sxs-lookup"><span data-stu-id="5f6cd-109">**Request syntax**</span></span>

|    <span data-ttu-id="5f6cd-110">Método</span><span class="sxs-lookup"><span data-stu-id="5f6cd-110">Method</span></span>    |    <span data-ttu-id="5f6cd-111">URI da solicitação</span><span class="sxs-lookup"><span data-stu-id="5f6cd-111">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="5f6cd-112">GET</span><span class="sxs-lookup"><span data-stu-id="5f6cd-112">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/testQueryResult?<exportQuery={query text}|queryId={queryId}>`    |
|        |        |

<span data-ttu-id="5f6cd-113">**Cabeçalho da solicitação**</span><span class="sxs-lookup"><span data-stu-id="5f6cd-113">**Request header**</span></span>

|    <span data-ttu-id="5f6cd-114">parâmetro</span><span class="sxs-lookup"><span data-stu-id="5f6cd-114">Header</span></span>    |    <span data-ttu-id="5f6cd-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f6cd-115">Type</span></span>    |    <span data-ttu-id="5f6cd-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f6cd-116">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="5f6cd-117">Autorização</span><span class="sxs-lookup"><span data-stu-id="5f6cd-117">Authorization</span></span>    |    <span data-ttu-id="5f6cd-118">string</span><span class="sxs-lookup"><span data-stu-id="5f6cd-118">string</span></span>    |    <span data-ttu-id="5f6cd-119">Obrigatórios.</span><span class="sxs-lookup"><span data-stu-id="5f6cd-119">Required.</span></span> <span data-ttu-id="5f6cd-120">O token de acesso Azure Active Directory (AAD) no formulário`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="5f6cd-120">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="5f6cd-121">Tipo de conteúdo</span><span class="sxs-lookup"><span data-stu-id="5f6cd-121">Content-Type</span></span>    |    <span data-ttu-id="5f6cd-122">string</span><span class="sxs-lookup"><span data-stu-id="5f6cd-122">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="5f6cd-123">**Parâmetro de caminho**</span><span class="sxs-lookup"><span data-stu-id="5f6cd-123">**Path parameter**</span></span>

<span data-ttu-id="5f6cd-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5f6cd-124">None</span></span>

<span data-ttu-id="5f6cd-125">**Parâmetro de consulta**</span><span class="sxs-lookup"><span data-stu-id="5f6cd-125">**Query parameter**</span></span>

|    <span data-ttu-id="5f6cd-126">Nome do Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5f6cd-126">Parameter Name</span></span>    |    <span data-ttu-id="5f6cd-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f6cd-127">Type</span></span>    |    <span data-ttu-id="5f6cd-128">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="5f6cd-128">Required</span></span>    |    <span data-ttu-id="5f6cd-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f6cd-129">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="5f6cd-130">exportQuery</span><span class="sxs-lookup"><span data-stu-id="5f6cd-130">exportQuery</span></span>     |    <span data-ttu-id="5f6cd-131">string</span><span class="sxs-lookup"><span data-stu-id="5f6cd-131">string</span></span>    |    <span data-ttu-id="5f6cd-132">Não</span><span class="sxs-lookup"><span data-stu-id="5f6cd-132">No</span></span>    |    <span data-ttu-id="5f6cd-133">Cadeia de caracteres de consulta de relatório que precisa ser executada</span><span class="sxs-lookup"><span data-stu-id="5f6cd-133">Report query string that needs to be executed</span></span>     |
|    <span data-ttu-id="5f6cd-134">queryId</span><span class="sxs-lookup"><span data-stu-id="5f6cd-134">queryId</span></span>     |    <span data-ttu-id="5f6cd-135">string</span><span class="sxs-lookup"><span data-stu-id="5f6cd-135">string</span></span>    |    <span data-ttu-id="5f6cd-136">Não</span><span class="sxs-lookup"><span data-stu-id="5f6cd-136">No</span></span>    |    <span data-ttu-id="5f6cd-137">Uma ID de consulta existente válida.</span><span class="sxs-lookup"><span data-stu-id="5f6cd-137">A valid existing query ID.</span></span> <span data-ttu-id="5f6cd-138">Mutuamente exclusivo com a cadeia de caracteres de consulta especificada no parâmetro exportQuery</span><span class="sxs-lookup"><span data-stu-id="5f6cd-138">Mutually exclusive with query string specified in exportQuery parameter</span></span>    |
|    <span data-ttu-id="5f6cd-139">startTime</span><span class="sxs-lookup"><span data-stu-id="5f6cd-139">startTime</span></span>     |    <span data-ttu-id="5f6cd-140">string</span><span class="sxs-lookup"><span data-stu-id="5f6cd-140">string</span></span>    |    <span data-ttu-id="5f6cd-141">Não</span><span class="sxs-lookup"><span data-stu-id="5f6cd-141">No</span></span>    |    <span data-ttu-id="5f6cd-142">Hora de início da qual queremos os dados.</span><span class="sxs-lookup"><span data-stu-id="5f6cd-142">Start time from which we want the data.</span></span> <span data-ttu-id="5f6cd-143">Ele substitui o período de tempo especificado na consulta</span><span class="sxs-lookup"><span data-stu-id="5f6cd-143">It overrides timespan specified in the query</span></span>    |
|    <span data-ttu-id="5f6cd-144">endTime</span><span class="sxs-lookup"><span data-stu-id="5f6cd-144">endTime</span></span>     |    <span data-ttu-id="5f6cd-145">string</span><span class="sxs-lookup"><span data-stu-id="5f6cd-145">string</span></span>    |    <span data-ttu-id="5f6cd-146">Não</span><span class="sxs-lookup"><span data-stu-id="5f6cd-146">No</span></span>    |    <span data-ttu-id="5f6cd-147">Hora de término até a qual desejamos os dados.</span><span class="sxs-lookup"><span data-stu-id="5f6cd-147">End time till which we want the data.</span></span> <span data-ttu-id="5f6cd-148">Ele substitui o período de tempo especificado na consulta</span><span class="sxs-lookup"><span data-stu-id="5f6cd-148">It overrides timespan specified in the query</span></span>    |
|        |        |        |        |

<span data-ttu-id="5f6cd-149">**Carga de solicitação**</span><span class="sxs-lookup"><span data-stu-id="5f6cd-149">**Request payload**</span></span>

<span data-ttu-id="5f6cd-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5f6cd-150">None</span></span>

<span data-ttu-id="5f6cd-151">**Glossário**</span><span class="sxs-lookup"><span data-stu-id="5f6cd-151">**Glossary**</span></span>

<span data-ttu-id="5f6cd-152">Não</span><span class="sxs-lookup"><span data-stu-id="5f6cd-152">None</span></span>

<span data-ttu-id="5f6cd-153">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="5f6cd-153">**Response**</span></span>

<span data-ttu-id="5f6cd-154">A carga de solicitação é estrutura conforme a seguir:</span><span class="sxs-lookup"><span data-stu-id="5f6cd-154">The response payload is structured as follows:</span></span>

<span data-ttu-id="5f6cd-155">Código de resposta: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="5f6cd-155">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="5f6cd-156">Exemplo de conteúdo de resposta:</span><span class="sxs-lookup"><span data-stu-id="5f6cd-156">Response payload example:</span></span>

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

<span data-ttu-id="5f6cd-157">**Glossário**</span><span class="sxs-lookup"><span data-stu-id="5f6cd-157">**Glossary**</span></span>

<span data-ttu-id="5f6cd-158">Esta tabela define os principais elementos na resposta:</span><span class="sxs-lookup"><span data-stu-id="5f6cd-158">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="5f6cd-159">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5f6cd-159">Parameter</span></span>    |    <span data-ttu-id="5f6cd-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f6cd-160">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="5f6cd-161">TotalCount</span><span class="sxs-lookup"><span data-stu-id="5f6cd-161">TotalCount</span></span>     |    <span data-ttu-id="5f6cd-162">Número de conjuntos de dados na matriz de valores</span><span class="sxs-lookup"><span data-stu-id="5f6cd-162">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="5f6cd-163">Mensagem</span><span class="sxs-lookup"><span data-stu-id="5f6cd-163">Message</span></span>     |    <span data-ttu-id="5f6cd-164">Mensagem do status da execução da API</span><span class="sxs-lookup"><span data-stu-id="5f6cd-164">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="5f6cd-165">StatusCode</span><span class="sxs-lookup"><span data-stu-id="5f6cd-165">StatusCode</span></span>     |    <span data-ttu-id="5f6cd-166">Código de resultado.</span><span class="sxs-lookup"><span data-stu-id="5f6cd-166">Result Code.</span></span> <span data-ttu-id="5f6cd-167">Os valores possíveis são 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="5f6cd-167">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
