---
title: Excluir API de relatório – Insights dados
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Use essa API para excluir qualquer relatório no Partner Center insights.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: e060104f8f09f69c213ab1b22d4be08d58babced
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114374862"
---
# <a name="delete-report-api"></a><span data-ttu-id="346c8-103">Excluir API de relatório</span><span class="sxs-lookup"><span data-stu-id="346c8-103">Delete report API</span></span>

<span data-ttu-id="346c8-104">Na execução, essa API exclui todos os relatórios e registros de execução do relatório.</span><span class="sxs-lookup"><span data-stu-id="346c8-104">On execution, this API deletes all of the report and report execution records.</span></span>

<span data-ttu-id="346c8-105">**Sintaxe da solicitação**</span><span class="sxs-lookup"><span data-stu-id="346c8-105">**Request syntax**</span></span>

|    <span data-ttu-id="346c8-106">Método</span><span class="sxs-lookup"><span data-stu-id="346c8-106">Method</span></span>    |    <span data-ttu-id="346c8-107">URI da solicitação</span><span class="sxs-lookup"><span data-stu-id="346c8-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="346c8-108">DELETE</span><span class="sxs-lookup"><span data-stu-id="346c8-108">DELETE</span></span>    |    ` https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
|        |        |

<span data-ttu-id="346c8-109">**Cabeçalho da solicitação**</span><span class="sxs-lookup"><span data-stu-id="346c8-109">**Request header**</span></span>

|    <span data-ttu-id="346c8-110">parâmetro</span><span class="sxs-lookup"><span data-stu-id="346c8-110">Header</span></span>    |    <span data-ttu-id="346c8-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="346c8-111">Type</span></span>    |    <span data-ttu-id="346c8-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="346c8-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="346c8-113">Autorização</span><span class="sxs-lookup"><span data-stu-id="346c8-113">Authorization</span></span>    |    <span data-ttu-id="346c8-114">string</span><span class="sxs-lookup"><span data-stu-id="346c8-114">string</span></span>    |    <span data-ttu-id="346c8-115">Obrigatórios.</span><span class="sxs-lookup"><span data-stu-id="346c8-115">Required.</span></span> <span data-ttu-id="346c8-116">O token de acesso Azure Active Directory (AAD) no formulário`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="346c8-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="346c8-117">Tipo de conteúdo</span><span class="sxs-lookup"><span data-stu-id="346c8-117">Content-Type</span></span>    |    <span data-ttu-id="346c8-118">string</span><span class="sxs-lookup"><span data-stu-id="346c8-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="346c8-119">**Parâmetro de caminho**</span><span class="sxs-lookup"><span data-stu-id="346c8-119">**Path parameter**</span></span>

|    <span data-ttu-id="346c8-120">Nome do Parâmetro</span><span class="sxs-lookup"><span data-stu-id="346c8-120">Parameter Name</span></span>    |    <span data-ttu-id="346c8-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="346c8-121">Type</span></span>    |    <span data-ttu-id="346c8-122">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="346c8-122">Required</span></span>    |    <span data-ttu-id="346c8-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="346c8-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="346c8-124">reportId</span><span class="sxs-lookup"><span data-stu-id="346c8-124">reportId</span></span>     |    <span data-ttu-id="346c8-125">string</span><span class="sxs-lookup"><span data-stu-id="346c8-125">string</span></span>    |    <span data-ttu-id="346c8-126">Não</span><span class="sxs-lookup"><span data-stu-id="346c8-126">No</span></span>    |    <span data-ttu-id="346c8-127">ID do relatório que está sendo excluído</span><span class="sxs-lookup"><span data-stu-id="346c8-127">ID of the report being deleted</span></span>    |
|        |        |        |        |

<span data-ttu-id="346c8-128">**Parâmetro de consulta**</span><span class="sxs-lookup"><span data-stu-id="346c8-128">**Query parameter**</span></span>

<span data-ttu-id="346c8-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="346c8-129">None</span></span>

<span data-ttu-id="346c8-130">**Carga de solicitação**</span><span class="sxs-lookup"><span data-stu-id="346c8-130">**Request payload**</span></span>

<span data-ttu-id="346c8-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="346c8-131">None</span></span>

<span data-ttu-id="346c8-132">**Glossário**</span><span class="sxs-lookup"><span data-stu-id="346c8-132">**Glossary**</span></span>

<span data-ttu-id="346c8-133">Não</span><span class="sxs-lookup"><span data-stu-id="346c8-133">None</span></span>

<span data-ttu-id="346c8-134">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="346c8-134">**Response**</span></span>

<span data-ttu-id="346c8-135">A carga de solicitação é estrutura conforme a seguir:</span><span class="sxs-lookup"><span data-stu-id="346c8-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="346c8-136">Código de resposta: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="346c8-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="346c8-137">Exemplo de conteúdo de resposta:</span><span class="sxs-lookup"><span data-stu-id="346c8-137">Response payload example:</span></span>

```json
{ 
  "Value": [ 
    { 
      "ReportId": "string", 
      "ReportName": "string", 
      "Description": "string", 
      "QueryId": "string", 
      "Query": "string", 
      "User": "string", 
      "CreatedTime": "string", 
      "ModifiedTime": "string", 
      "ExecuteNow": true, 
      "StartTime": "string", 
      "ReportStatus": "string", 
      "RecurrenceInterval": 0, 
      "RecurrenceCount": 0, 
      "CallbackUrl": "string",
      "CallbackMethod": "string",
      "Format": "string" 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0, 
} 
```

<span data-ttu-id="346c8-138">**Glossário**</span><span class="sxs-lookup"><span data-stu-id="346c8-138">**Glossary**</span></span>

<span data-ttu-id="346c8-139">Esta tabela define os principais elementos na resposta:</span><span class="sxs-lookup"><span data-stu-id="346c8-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="346c8-140">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="346c8-140">Parameter</span></span>    |    <span data-ttu-id="346c8-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="346c8-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="346c8-142">ReportId</span><span class="sxs-lookup"><span data-stu-id="346c8-142">ReportId</span></span>     |    <span data-ttu-id="346c8-143">Identificador universal exclusivo (UUID) do relatório excluído</span><span class="sxs-lookup"><span data-stu-id="346c8-143">Universally unique identifier (UUID) of the deleted report</span></span>     |
|    <span data-ttu-id="346c8-144">ReportName</span><span class="sxs-lookup"><span data-stu-id="346c8-144">ReportName</span></span>     |    <span data-ttu-id="346c8-145">Nome dado ao relatório durante a criação</span><span class="sxs-lookup"><span data-stu-id="346c8-145">Name given to the report during creation</span></span>     |
|    <span data-ttu-id="346c8-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="346c8-146">Description</span></span>     |    <span data-ttu-id="346c8-147">Descrição fornecida durante a criação do relatório</span><span class="sxs-lookup"><span data-stu-id="346c8-147">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="346c8-148">QueryId</span><span class="sxs-lookup"><span data-stu-id="346c8-148">QueryId</span></span>     |    <span data-ttu-id="346c8-149">ID de consulta passada no momento da criação do relatório</span><span class="sxs-lookup"><span data-stu-id="346c8-149">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="346c8-150">Consulta</span><span class="sxs-lookup"><span data-stu-id="346c8-150">Query</span></span>     |    <span data-ttu-id="346c8-151">Texto da consulta que será executada para este relatório</span><span class="sxs-lookup"><span data-stu-id="346c8-151">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="346c8-152">Usuário</span><span class="sxs-lookup"><span data-stu-id="346c8-152">User</span></span>     |    <span data-ttu-id="346c8-153">ID de usuário usada para criar o relatório</span><span class="sxs-lookup"><span data-stu-id="346c8-153">User ID used to create the report</span></span>     |
|    <span data-ttu-id="346c8-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="346c8-154">CreatedTime</span></span>     |    <span data-ttu-id="346c8-155">Hora de criação do relatório.</span><span class="sxs-lookup"><span data-stu-id="346c8-155">Time the report was created.</span></span> <span data-ttu-id="346c8-156">O formato de hora é aaaa-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="346c8-156">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="346c8-157">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="346c8-157">ModifiedTime</span></span>     |    <span data-ttu-id="346c8-158">Hora em que o relatório foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="346c8-158">Time the report was last modified.</span></span> <span data-ttu-id="346c8-159">O formato de hora é aaaa-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="346c8-159">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="346c8-160">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="346c8-160">ExecuteNow</span></span>     |    <span data-ttu-id="346c8-161">Sinalizador ExecuteNow definido no momento em que o relatório foi criado</span><span class="sxs-lookup"><span data-stu-id="346c8-161">ExecuteNow flag set at the time the report was created</span></span>     |
|    <span data-ttu-id="346c8-162">StartTime</span><span class="sxs-lookup"><span data-stu-id="346c8-162">StartTime</span></span>     |    <span data-ttu-id="346c8-163">Hora em que a execução do relatório será iniciada.</span><span class="sxs-lookup"><span data-stu-id="346c8-163">Time the report execution will begin.</span></span> <span data-ttu-id="346c8-164">O formato de hora é aaaa-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="346c8-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="346c8-165">Reportstatus</span><span class="sxs-lookup"><span data-stu-id="346c8-165">ReportStatus</span></span>     |    <span data-ttu-id="346c8-166">Status da execução do relatório.</span><span class="sxs-lookup"><span data-stu-id="346c8-166">Status of the report execution.</span></span> <span data-ttu-id="346c8-167">Os valores possíveis são Pausado, Ativo e Inativo.</span><span class="sxs-lookup"><span data-stu-id="346c8-167">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="346c8-168">RecorrênciaInterval</span><span class="sxs-lookup"><span data-stu-id="346c8-168">RecurrenceInterval</span></span>     |    <span data-ttu-id="346c8-169">Intervalo de recorrência fornecido durante a criação do relatório</span><span class="sxs-lookup"><span data-stu-id="346c8-169">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="346c8-170">RecorrênciaCount</span><span class="sxs-lookup"><span data-stu-id="346c8-170">RecurrenceCount</span></span>     |    <span data-ttu-id="346c8-171">Contagem de recorrência fornecida durante a criação do relatório</span><span class="sxs-lookup"><span data-stu-id="346c8-171">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="346c8-172">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="346c8-172">CallbackUrl</span></span>     |    <span data-ttu-id="346c8-173">URL de retorno de chamada fornecida na solicitação</span><span class="sxs-lookup"><span data-stu-id="346c8-173">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="346c8-174">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="346c8-174">CallbackMethod</span></span>    |    <span data-ttu-id="346c8-175">Método de retorno de chamada fornecido na solicitação</span><span class="sxs-lookup"><span data-stu-id="346c8-175">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="346c8-176">Formatar</span><span class="sxs-lookup"><span data-stu-id="346c8-176">Format</span></span>     |    <span data-ttu-id="346c8-177">Formato dos arquivos do relatório</span><span class="sxs-lookup"><span data-stu-id="346c8-177">Format of the report files</span></span>     |
|    <span data-ttu-id="346c8-178">TotalCount</span><span class="sxs-lookup"><span data-stu-id="346c8-178">TotalCount</span></span>     |    <span data-ttu-id="346c8-179">Número de conjuntos de dados na matriz de valores</span><span class="sxs-lookup"><span data-stu-id="346c8-179">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="346c8-180">Mensagem</span><span class="sxs-lookup"><span data-stu-id="346c8-180">Message</span></span>     |    <span data-ttu-id="346c8-181">Mensagem do status da execução da API</span><span class="sxs-lookup"><span data-stu-id="346c8-181">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="346c8-182">StatusCode</span><span class="sxs-lookup"><span data-stu-id="346c8-182">StatusCode</span></span>     |    <span data-ttu-id="346c8-183">Código de resultado.</span><span class="sxs-lookup"><span data-stu-id="346c8-183">Result Code.</span></span> <span data-ttu-id="346c8-184">Os valores possíveis são 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="346c8-184">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
