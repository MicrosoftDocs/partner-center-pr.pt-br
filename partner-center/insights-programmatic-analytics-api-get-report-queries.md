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
# <a name="get-report-queries-api"></a><span data-ttu-id="49db6-103">Obter API de consultas de relatório</span><span class="sxs-lookup"><span data-stu-id="49db6-103">Get report queries API</span></span>

<span data-ttu-id="49db6-104">A API obter consultas de relatório obtém todas as consultas que estão disponíveis para uso em relatórios.</span><span class="sxs-lookup"><span data-stu-id="49db6-104">The Get report queries API gets all the queries that are available for use in reports.</span></span> <span data-ttu-id="49db6-105">Ela obtém todas as consultas definidas pelo sistema e pelo usuário por padrão.</span><span class="sxs-lookup"><span data-stu-id="49db6-105">It gets all the system and user-defined queries by default.</span></span>

<span data-ttu-id="49db6-106">**Sintaxe da solicitação**</span><span class="sxs-lookup"><span data-stu-id="49db6-106">**Request syntax**</span></span>

|    <span data-ttu-id="49db6-107">Método</span><span class="sxs-lookup"><span data-stu-id="49db6-107">Method</span></span>    |    <span data-ttu-id="49db6-108">URI da solicitação</span><span class="sxs-lookup"><span data-stu-id="49db6-108">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="49db6-109">GET</span><span class="sxs-lookup"><span data-stu-id="49db6-109">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries?queryId={QueryID}&queryName={QueryName}&includeSystemQueries={include_system_queries}&includeOnlySystemQueries={include_only_system_queries}`     |
|        |        |

<span data-ttu-id="49db6-110">**Cabeçalho da solicitação**</span><span class="sxs-lookup"><span data-stu-id="49db6-110">**Request header**</span></span>

|    <span data-ttu-id="49db6-111">parâmetro</span><span class="sxs-lookup"><span data-stu-id="49db6-111">Header</span></span>    |    <span data-ttu-id="49db6-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="49db6-112">Type</span></span>    |    <span data-ttu-id="49db6-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="49db6-113">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="49db6-114">Autorização</span><span class="sxs-lookup"><span data-stu-id="49db6-114">Authorization</span></span>    |    <span data-ttu-id="49db6-115">string</span><span class="sxs-lookup"><span data-stu-id="49db6-115">string</span></span>    |    <span data-ttu-id="49db6-116">Obrigatórios.</span><span class="sxs-lookup"><span data-stu-id="49db6-116">Required.</span></span> <span data-ttu-id="49db6-117">o token de acesso do Azure Active Directory (AAD) no formulário`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="49db6-117">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="49db6-118">Tipo de conteúdo</span><span class="sxs-lookup"><span data-stu-id="49db6-118">Content-Type</span></span>    |    <span data-ttu-id="49db6-119">string</span><span class="sxs-lookup"><span data-stu-id="49db6-119">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="49db6-120">**Parâmetro de caminho**</span><span class="sxs-lookup"><span data-stu-id="49db6-120">**Path parameter**</span></span>

<span data-ttu-id="49db6-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="49db6-121">None</span></span>

<span data-ttu-id="49db6-122">**Parâmetro de consulta**</span><span class="sxs-lookup"><span data-stu-id="49db6-122">**Query parameter**</span></span>

|    <span data-ttu-id="49db6-123">Nome do Parâmetro</span><span class="sxs-lookup"><span data-stu-id="49db6-123">Parameter Name</span></span>    |    <span data-ttu-id="49db6-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="49db6-124">Type</span></span>    |    <span data-ttu-id="49db6-125">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="49db6-125">Required</span></span>    |    <span data-ttu-id="49db6-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="49db6-126">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="49db6-127">queryId</span><span class="sxs-lookup"><span data-stu-id="49db6-127">queryId</span></span>     |    <span data-ttu-id="49db6-128">string</span><span class="sxs-lookup"><span data-stu-id="49db6-128">string</span></span>     |    <span data-ttu-id="49db6-129">No</span><span class="sxs-lookup"><span data-stu-id="49db6-129">No</span></span>    |    <span data-ttu-id="49db6-130">Filtrar para obter detalhes somente de consultas com a ID fornecida neste argumento</span><span class="sxs-lookup"><span data-stu-id="49db6-130">Filter to get details of only queries with the ID given in the argument</span></span>     |
|    <span data-ttu-id="49db6-131">queryName</span><span class="sxs-lookup"><span data-stu-id="49db6-131">queryName</span></span>     |    <span data-ttu-id="49db6-132">string</span><span class="sxs-lookup"><span data-stu-id="49db6-132">string</span></span>     |    <span data-ttu-id="49db6-133">No</span><span class="sxs-lookup"><span data-stu-id="49db6-133">No</span></span>    |    <span data-ttu-id="49db6-134">Filtrar para obter detalhes somente de consultas com o nome fornecido neste argumento</span><span class="sxs-lookup"><span data-stu-id="49db6-134">Filter to get details of only queries with the name given in the argument</span></span>     |
|    <span data-ttu-id="49db6-135">IncludeSystemQueries</span><span class="sxs-lookup"><span data-stu-id="49db6-135">IncludeSystemQueries</span></span>     |    <span data-ttu-id="49db6-136">booleano</span><span class="sxs-lookup"><span data-stu-id="49db6-136">boolean</span></span>     |    <span data-ttu-id="49db6-137">No</span><span class="sxs-lookup"><span data-stu-id="49db6-137">No</span></span>    |    <span data-ttu-id="49db6-138">Incluir consultas de sistema predefinidas na resposta</span><span class="sxs-lookup"><span data-stu-id="49db6-138">Include predefined system queries in the response</span></span>     |
|    <span data-ttu-id="49db6-139">IncludeOnlySystemQueries</span><span class="sxs-lookup"><span data-stu-id="49db6-139">IncludeOnlySystemQueries</span></span>     |    <span data-ttu-id="49db6-140">booleano</span><span class="sxs-lookup"><span data-stu-id="49db6-140">boolean</span></span>     |    <span data-ttu-id="49db6-141">No</span><span class="sxs-lookup"><span data-stu-id="49db6-141">No</span></span>    |    <span data-ttu-id="49db6-142">Incluir somente consultas de sistema na resposta</span><span class="sxs-lookup"><span data-stu-id="49db6-142">Include only system queries in the response</span></span>     |
|        |        |        |        |


<span data-ttu-id="49db6-143">**Carga de solicitação**</span><span class="sxs-lookup"><span data-stu-id="49db6-143">**Request payload**</span></span>

<span data-ttu-id="49db6-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="49db6-144">None</span></span>

<span data-ttu-id="49db6-145">**Glossário**</span><span class="sxs-lookup"><span data-stu-id="49db6-145">**Glossary**</span></span>

<span data-ttu-id="49db6-146">Não</span><span class="sxs-lookup"><span data-stu-id="49db6-146">None</span></span>

<span data-ttu-id="49db6-147">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="49db6-147">**Response**</span></span>

<span data-ttu-id="49db6-148">A carga de solicitação é estrutura conforme a seguir:</span><span class="sxs-lookup"><span data-stu-id="49db6-148">The response payload is structured as follows:</span></span>

<span data-ttu-id="49db6-149">Código de resposta: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="49db6-149">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="49db6-150">Exemplo de conteúdo de resposta:</span><span class="sxs-lookup"><span data-stu-id="49db6-150">Response payload example:</span></span>

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

<span data-ttu-id="49db6-151">**Glossário**</span><span class="sxs-lookup"><span data-stu-id="49db6-151">**Glossary**</span></span>

<span data-ttu-id="49db6-152">Esta tabela define os principais elementos na resposta:</span><span class="sxs-lookup"><span data-stu-id="49db6-152">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="49db6-153">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="49db6-153">Parameter</span></span>    |    <span data-ttu-id="49db6-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="49db6-154">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="49db6-155">QueryId</span><span class="sxs-lookup"><span data-stu-id="49db6-155">QueryId</span></span>     |    <span data-ttu-id="49db6-156">UUID exclusivo da consulta</span><span class="sxs-lookup"><span data-stu-id="49db6-156">Unique UUID of the query</span></span>     |
|    <span data-ttu-id="49db6-157">Nome</span><span class="sxs-lookup"><span data-stu-id="49db6-157">Name</span></span>     |    <span data-ttu-id="49db6-158">Nome fornecido à consulta no momento da criação da consulta</span><span class="sxs-lookup"><span data-stu-id="49db6-158">Name given to the query at the time of query creation</span></span>     |
|    <span data-ttu-id="49db6-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="49db6-159">Description</span></span>     |    <span data-ttu-id="49db6-160">Descrição fornecida durante a criação da consulta</span><span class="sxs-lookup"><span data-stu-id="49db6-160">Description given during creation of the query</span></span>     |
|    <span data-ttu-id="49db6-161">Consulta</span><span class="sxs-lookup"><span data-stu-id="49db6-161">Query</span></span>     |    <span data-ttu-id="49db6-162">Cadeia de caracteres de consulta de relatório</span><span class="sxs-lookup"><span data-stu-id="49db6-162">Report query string</span></span>     |
|    <span data-ttu-id="49db6-163">Tipo</span><span class="sxs-lookup"><span data-stu-id="49db6-163">Type</span></span>     |    <span data-ttu-id="49db6-164">Definido como UserDefined para consultas criadas pelo usuário e para o sistema para consultas de sistema predefinidas</span><span class="sxs-lookup"><span data-stu-id="49db6-164">Set to userDefined for user created queries and system for predefined system queries</span></span>     |
|    <span data-ttu-id="49db6-165">Usuário</span><span class="sxs-lookup"><span data-stu-id="49db6-165">User</span></span>     |    <span data-ttu-id="49db6-166">ID de usuário que criou a consulta</span><span class="sxs-lookup"><span data-stu-id="49db6-166">User ID who created the query</span></span>     |
|    <span data-ttu-id="49db6-167">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="49db6-167">CreatedTime</span></span>     |    <span data-ttu-id="49db6-168">Hora da criação da consulta</span><span class="sxs-lookup"><span data-stu-id="49db6-168">Time of creation of query</span></span>     |
|    <span data-ttu-id="49db6-169">TotalCount</span><span class="sxs-lookup"><span data-stu-id="49db6-169">TotalCount</span></span>     |    <span data-ttu-id="49db6-170">Número de conjuntos de dados na matriz de valores</span><span class="sxs-lookup"><span data-stu-id="49db6-170">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="49db6-171">Mensagem</span><span class="sxs-lookup"><span data-stu-id="49db6-171">Message</span></span>     |    <span data-ttu-id="49db6-172">Mensagem do status da execução da API</span><span class="sxs-lookup"><span data-stu-id="49db6-172">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="49db6-173">StatusCode</span><span class="sxs-lookup"><span data-stu-id="49db6-173">StatusCode</span></span>     |    <span data-ttu-id="49db6-174">Código de resultado.</span><span class="sxs-lookup"><span data-stu-id="49db6-174">Result Code.</span></span> <span data-ttu-id="49db6-175">Os valores possíveis são 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="49db6-175">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
