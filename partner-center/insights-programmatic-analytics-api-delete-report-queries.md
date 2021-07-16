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
# <a name="delete-report-queries-api"></a><span data-ttu-id="b9dd3-103">Excluir API de consultas de relatório</span><span class="sxs-lookup"><span data-stu-id="b9dd3-103">Delete report queries API</span></span>

<span data-ttu-id="b9dd3-104">Essa API exclui consultas definidas pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="b9dd3-104">This API deletes user-defined queries.</span></span>

<span data-ttu-id="b9dd3-105">**Sintaxe da solicitação**</span><span class="sxs-lookup"><span data-stu-id="b9dd3-105">**Request syntax**</span></span>

|    <span data-ttu-id="b9dd3-106">Método</span><span class="sxs-lookup"><span data-stu-id="b9dd3-106">Method</span></span>    |    <span data-ttu-id="b9dd3-107">URI da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9dd3-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="b9dd3-108">DELETE</span><span class="sxs-lookup"><span data-stu-id="b9dd3-108">DELETE</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/{queryId}` |
|        |        |

<span data-ttu-id="b9dd3-109">**Cabeçalho da solicitação**</span><span class="sxs-lookup"><span data-stu-id="b9dd3-109">**Request header**</span></span>

|    <span data-ttu-id="b9dd3-110">parâmetro</span><span class="sxs-lookup"><span data-stu-id="b9dd3-110">Header</span></span>    |    <span data-ttu-id="b9dd3-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9dd3-111">Type</span></span>    |    <span data-ttu-id="b9dd3-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9dd3-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="b9dd3-113">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9dd3-113">Authorization</span></span>    |    <span data-ttu-id="b9dd3-114">string</span><span class="sxs-lookup"><span data-stu-id="b9dd3-114">string</span></span>    |    <span data-ttu-id="b9dd3-115">Obrigatórios.</span><span class="sxs-lookup"><span data-stu-id="b9dd3-115">Required.</span></span> <span data-ttu-id="b9dd3-116">O token de acesso Azure Active Directory (AAD) no formulário`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="b9dd3-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="b9dd3-117">Tipo de conteúdo</span><span class="sxs-lookup"><span data-stu-id="b9dd3-117">Content-Type</span></span>    |    <span data-ttu-id="b9dd3-118">string</span><span class="sxs-lookup"><span data-stu-id="b9dd3-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="b9dd3-119">**Parâmetro de caminho**</span><span class="sxs-lookup"><span data-stu-id="b9dd3-119">**Path parameter**</span></span>

|    <span data-ttu-id="b9dd3-120">Nome do Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b9dd3-120">Parameter Name</span></span>    |    <span data-ttu-id="b9dd3-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9dd3-121">Type</span></span>    |    <span data-ttu-id="b9dd3-122">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="b9dd3-122">Required</span></span>    |    <span data-ttu-id="b9dd3-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9dd3-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="b9dd3-124">queryId</span><span class="sxs-lookup"><span data-stu-id="b9dd3-124">queryId</span></span>     |    <span data-ttu-id="b9dd3-125">string</span><span class="sxs-lookup"><span data-stu-id="b9dd3-125">string</span></span>     |    <span data-ttu-id="b9dd3-126">No</span><span class="sxs-lookup"><span data-stu-id="b9dd3-126">No</span></span>    |    <span data-ttu-id="b9dd3-127">Filtrar para obter detalhes somente de consultas com a ID fornecida neste argumento</span><span class="sxs-lookup"><span data-stu-id="b9dd3-127">Filter to get details of only queries with the ID given in the argument</span></span>     |
|        |        |        |        |

<span data-ttu-id="b9dd3-128">**Parâmetro de consulta**</span><span class="sxs-lookup"><span data-stu-id="b9dd3-128">**Query parameter**</span></span>

<span data-ttu-id="b9dd3-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b9dd3-129">None</span></span>

<span data-ttu-id="b9dd3-130">**Carga de solicitação**</span><span class="sxs-lookup"><span data-stu-id="b9dd3-130">**Request payload**</span></span>

<span data-ttu-id="b9dd3-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b9dd3-131">None</span></span>

<span data-ttu-id="b9dd3-132">**Glossário**</span><span class="sxs-lookup"><span data-stu-id="b9dd3-132">**Glossary**</span></span>

<span data-ttu-id="b9dd3-133">Não</span><span class="sxs-lookup"><span data-stu-id="b9dd3-133">None</span></span>

<span data-ttu-id="b9dd3-134">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="b9dd3-134">**Response**</span></span>

<span data-ttu-id="b9dd3-135">A carga de solicitação é estrutura conforme a seguir:</span><span class="sxs-lookup"><span data-stu-id="b9dd3-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="b9dd3-136">Código de resposta: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="b9dd3-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="b9dd3-137">Exemplo de conteúdo de resposta:</span><span class="sxs-lookup"><span data-stu-id="b9dd3-137">Response payload example:</span></span>

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

<span data-ttu-id="b9dd3-138">**Glossário**</span><span class="sxs-lookup"><span data-stu-id="b9dd3-138">**Glossary**</span></span>

<span data-ttu-id="b9dd3-139">Esta tabela define os principais elementos na resposta:</span><span class="sxs-lookup"><span data-stu-id="b9dd3-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="b9dd3-140">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b9dd3-140">Parameter</span></span>    |    <span data-ttu-id="b9dd3-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9dd3-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="b9dd3-142">QueryId</span><span class="sxs-lookup"><span data-stu-id="b9dd3-142">QueryId</span></span>     |    <span data-ttu-id="b9dd3-143">UUID exclusivo da consulta que foi excluída</span><span class="sxs-lookup"><span data-stu-id="b9dd3-143">Unique UUID of the query that was deleted</span></span>    |
|    <span data-ttu-id="b9dd3-144">Nome</span><span class="sxs-lookup"><span data-stu-id="b9dd3-144">Name</span></span>     |    <span data-ttu-id="b9dd3-145">Nome da consulta que foi excluída</span><span class="sxs-lookup"><span data-stu-id="b9dd3-145">Name of the query that was deleted</span></span>    |
|    <span data-ttu-id="b9dd3-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9dd3-146">Description</span></span>     |    <span data-ttu-id="b9dd3-147">Descrição da consulta excluída</span><span class="sxs-lookup"><span data-stu-id="b9dd3-147">Description of the deleted query</span></span>     |
|    <span data-ttu-id="b9dd3-148">Consulta</span><span class="sxs-lookup"><span data-stu-id="b9dd3-148">Query</span></span>     |    <span data-ttu-id="b9dd3-149">Cadeia de caracteres de consulta de relatório da consulta excluída</span><span class="sxs-lookup"><span data-stu-id="b9dd3-149">Report query string of the deleted query</span></span>    |
|    <span data-ttu-id="b9dd3-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9dd3-150">Type</span></span>     |    <span data-ttu-id="b9dd3-151">Defina como userDefined para consultas criadas pelo usuário</span><span class="sxs-lookup"><span data-stu-id="b9dd3-151">Set to userDefined for user created queries</span></span>     |
|    <span data-ttu-id="b9dd3-152">Usuário</span><span class="sxs-lookup"><span data-stu-id="b9dd3-152">User</span></span>     |    <span data-ttu-id="b9dd3-153">ID de usuário que criou a consulta</span><span class="sxs-lookup"><span data-stu-id="b9dd3-153">User ID who created the query</span></span>     |
|    <span data-ttu-id="b9dd3-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="b9dd3-154">CreatedTime</span></span>     |    <span data-ttu-id="b9dd3-155">Hora da criação da consulta</span><span class="sxs-lookup"><span data-stu-id="b9dd3-155">Time of creation of query</span></span>     |
|    <span data-ttu-id="b9dd3-156">TotalCount</span><span class="sxs-lookup"><span data-stu-id="b9dd3-156">TotalCount</span></span>     |    <span data-ttu-id="b9dd3-157">Número de conjuntos de dados na matriz de valores</span><span class="sxs-lookup"><span data-stu-id="b9dd3-157">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="b9dd3-158">Mensagem</span><span class="sxs-lookup"><span data-stu-id="b9dd3-158">Message</span></span>     |    <span data-ttu-id="b9dd3-159">Mensagem do status da execução da API</span><span class="sxs-lookup"><span data-stu-id="b9dd3-159">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="b9dd3-160">StatusCode</span><span class="sxs-lookup"><span data-stu-id="b9dd3-160">StatusCode</span></span>     |    <span data-ttu-id="b9dd3-161">Código de resultado.</span><span class="sxs-lookup"><span data-stu-id="b9dd3-161">Result Code.</span></span> <span data-ttu-id="b9dd3-162">Os valores possíveis são 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="b9dd3-162">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
