---
title: pausar API de execução de relatório – dados de Insights
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Use essa API para pausar a execução de qualquer relatório no Partner Center insights.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 1e490a6d5120d729f0ea4979a201e9a80ba2991c
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114374857"
---
# <a name="pause-report-executions-api"></a><span data-ttu-id="2db4a-103">Pausar API de execuções de relatório</span><span class="sxs-lookup"><span data-stu-id="2db4a-103">Pause report executions API</span></span>

<span data-ttu-id="2db4a-104">Na execução, essa API pausa a execução agendada de relatórios.</span><span class="sxs-lookup"><span data-stu-id="2db4a-104">On execution, this API pauses the scheduled execution of reports.</span></span>

<span data-ttu-id="2db4a-105">**Sintaxe da solicitação**</span><span class="sxs-lookup"><span data-stu-id="2db4a-105">**Request syntax**</span></span>

|    <span data-ttu-id="2db4a-106">Método</span><span class="sxs-lookup"><span data-stu-id="2db4a-106">Method</span></span>    |    <span data-ttu-id="2db4a-107">URI da solicitação</span><span class="sxs-lookup"><span data-stu-id="2db4a-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="2db4a-108">PUT</span><span class="sxs-lookup"><span data-stu-id="2db4a-108">PUT</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/pause/{ReportID}`    |
|        |        |

<span data-ttu-id="2db4a-109">**Cabeçalho da solicitação**</span><span class="sxs-lookup"><span data-stu-id="2db4a-109">**Request header**</span></span>

|    <span data-ttu-id="2db4a-110">parâmetro</span><span class="sxs-lookup"><span data-stu-id="2db4a-110">Header</span></span>    |    <span data-ttu-id="2db4a-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="2db4a-111">Type</span></span>    |    <span data-ttu-id="2db4a-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="2db4a-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="2db4a-113">Autorização</span><span class="sxs-lookup"><span data-stu-id="2db4a-113">Authorization</span></span>    |    <span data-ttu-id="2db4a-114">string</span><span class="sxs-lookup"><span data-stu-id="2db4a-114">string</span></span>    |    <span data-ttu-id="2db4a-115">Obrigatórios.</span><span class="sxs-lookup"><span data-stu-id="2db4a-115">Required.</span></span> <span data-ttu-id="2db4a-116">o token de acesso do Azure Active Directory (AAD) no formulário`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="2db4a-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="2db4a-117">Tipo de conteúdo</span><span class="sxs-lookup"><span data-stu-id="2db4a-117">Content-Type</span></span>    |    <span data-ttu-id="2db4a-118">string</span><span class="sxs-lookup"><span data-stu-id="2db4a-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="2db4a-119">**Parâmetro de caminho**</span><span class="sxs-lookup"><span data-stu-id="2db4a-119">**Path parameter**</span></span>

|    <span data-ttu-id="2db4a-120">Nome do Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2db4a-120">Parameter Name</span></span>    |    <span data-ttu-id="2db4a-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="2db4a-121">Type</span></span>    |    <span data-ttu-id="2db4a-122">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="2db4a-122">Required</span></span>    |    <span data-ttu-id="2db4a-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="2db4a-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="2db4a-124">reportId</span><span class="sxs-lookup"><span data-stu-id="2db4a-124">reportId</span></span>     |    <span data-ttu-id="2db4a-125">string</span><span class="sxs-lookup"><span data-stu-id="2db4a-125">string</span></span>    |    <span data-ttu-id="2db4a-126">Não</span><span class="sxs-lookup"><span data-stu-id="2db4a-126">No</span></span>    |    <span data-ttu-id="2db4a-127">ID do relatório que está sendo modificado</span><span class="sxs-lookup"><span data-stu-id="2db4a-127">ID of the report being modified</span></span>     |
|        |        |        |        |

<span data-ttu-id="2db4a-128">**Parâmetro de consulta**</span><span class="sxs-lookup"><span data-stu-id="2db4a-128">**Query parameter**</span></span>

<span data-ttu-id="2db4a-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2db4a-129">None</span></span>

<span data-ttu-id="2db4a-130">**Carga de solicitação**</span><span class="sxs-lookup"><span data-stu-id="2db4a-130">**Request payload**</span></span>

<span data-ttu-id="2db4a-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2db4a-131">None</span></span>

<span data-ttu-id="2db4a-132">**Glossário**</span><span class="sxs-lookup"><span data-stu-id="2db4a-132">**Glossary**</span></span>

<span data-ttu-id="2db4a-133">Não</span><span class="sxs-lookup"><span data-stu-id="2db4a-133">None</span></span>

<span data-ttu-id="2db4a-134">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="2db4a-134">**Response**</span></span>

<span data-ttu-id="2db4a-135">A carga de solicitação é estrutura conforme a seguir:</span><span class="sxs-lookup"><span data-stu-id="2db4a-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="2db4a-136">Código de resposta: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="2db4a-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="2db4a-137">Exemplo de conteúdo de resposta:</span><span class="sxs-lookup"><span data-stu-id="2db4a-137">Response payload example:</span></span>

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

<span data-ttu-id="2db4a-138">**Glossário**</span><span class="sxs-lookup"><span data-stu-id="2db4a-138">**Glossary**</span></span>

<span data-ttu-id="2db4a-139">Esta tabela define os principais elementos na resposta:</span><span class="sxs-lookup"><span data-stu-id="2db4a-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="2db4a-140">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2db4a-140">Parameter</span></span>    |    <span data-ttu-id="2db4a-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="2db4a-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="2db4a-142">ReportId</span><span class="sxs-lookup"><span data-stu-id="2db4a-142">ReportId</span></span>     |    <span data-ttu-id="2db4a-143">UUID (identificador universal exclusivo) do relatório pausado</span><span class="sxs-lookup"><span data-stu-id="2db4a-143">Universally unique identifier (UUID) of the paused report</span></span>     |
|    <span data-ttu-id="2db4a-144">ReportName</span><span class="sxs-lookup"><span data-stu-id="2db4a-144">ReportName</span></span>     |    <span data-ttu-id="2db4a-145">Nome dado ao relatório durante a criação</span><span class="sxs-lookup"><span data-stu-id="2db4a-145">Name given to the report during creation</span></span>     |
|    <span data-ttu-id="2db4a-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="2db4a-146">Description</span></span>     |    <span data-ttu-id="2db4a-147">Descrição fornecida durante a criação do relatório</span><span class="sxs-lookup"><span data-stu-id="2db4a-147">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="2db4a-148">QueryId</span><span class="sxs-lookup"><span data-stu-id="2db4a-148">QueryId</span></span>     |    <span data-ttu-id="2db4a-149">ID de consulta passada no momento da criação do relatório</span><span class="sxs-lookup"><span data-stu-id="2db4a-149">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="2db4a-150">Consulta</span><span class="sxs-lookup"><span data-stu-id="2db4a-150">Query</span></span>     |    <span data-ttu-id="2db4a-151">Texto da consulta que será executada para este relatório</span><span class="sxs-lookup"><span data-stu-id="2db4a-151">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="2db4a-152">Usuário</span><span class="sxs-lookup"><span data-stu-id="2db4a-152">User</span></span>     |    <span data-ttu-id="2db4a-153">ID de usuário usada para criar o relatório</span><span class="sxs-lookup"><span data-stu-id="2db4a-153">User ID used to create the report</span></span>     |
|    <span data-ttu-id="2db4a-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="2db4a-154">CreatedTime</span></span>     |    <span data-ttu-id="2db4a-155">Hora de criação do relatório.</span><span class="sxs-lookup"><span data-stu-id="2db4a-155">Time the report was created.</span></span> <span data-ttu-id="2db4a-156">O formato de hora é aaaa-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="2db4a-156">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="2db4a-157">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="2db4a-157">ModifiedTime</span></span>     |    <span data-ttu-id="2db4a-158">Hora em que o relatório foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="2db4a-158">Time the report was last modified.</span></span> <span data-ttu-id="2db4a-159">O formato de hora é aaaa-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="2db4a-159">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="2db4a-160">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="2db4a-160">ExecuteNow</span></span>     |    <span data-ttu-id="2db4a-161">Sinalizador ExecuteNow definido no momento em que o relatório foi criado</span><span class="sxs-lookup"><span data-stu-id="2db4a-161">ExecuteNow flag set at the time the report was created</span></span>     |
|    <span data-ttu-id="2db4a-162">StartTime</span><span class="sxs-lookup"><span data-stu-id="2db4a-162">StartTime</span></span>     |    <span data-ttu-id="2db4a-163">Hora em que a execução do relatório será iniciada.</span><span class="sxs-lookup"><span data-stu-id="2db4a-163">Time the report execution will begin.</span></span> <span data-ttu-id="2db4a-164">O formato de hora é aaaa-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="2db4a-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="2db4a-165">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="2db4a-165">ReportStatus</span></span>     |    <span data-ttu-id="2db4a-166">Status da execução do relatório.</span><span class="sxs-lookup"><span data-stu-id="2db4a-166">Status of the report execution.</span></span> <span data-ttu-id="2db4a-167">Os valores possíveis são Pausado, Ativo e Inativo.</span><span class="sxs-lookup"><span data-stu-id="2db4a-167">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="2db4a-168">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="2db4a-168">RecurrenceInterval</span></span>     |    <span data-ttu-id="2db4a-169">Intervalo de recorrência fornecido durante a criação do relatório</span><span class="sxs-lookup"><span data-stu-id="2db4a-169">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="2db4a-170">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="2db4a-170">RecurrenceCount</span></span>     |    <span data-ttu-id="2db4a-171">Contagem de recorrência fornecida durante a criação do relatório</span><span class="sxs-lookup"><span data-stu-id="2db4a-171">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="2db4a-172">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="2db4a-172">CallbackUrl</span></span>     |    <span data-ttu-id="2db4a-173">URL de retorno de chamada fornecida na solicitação</span><span class="sxs-lookup"><span data-stu-id="2db4a-173">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="2db4a-174">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="2db4a-174">CallbackMethod</span></span>    |    <span data-ttu-id="2db4a-175">Método de retorno de chamada fornecido na solicitação</span><span class="sxs-lookup"><span data-stu-id="2db4a-175">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="2db4a-176">Formatar</span><span class="sxs-lookup"><span data-stu-id="2db4a-176">Format</span></span>     |    <span data-ttu-id="2db4a-177">Formato dos arquivos do relatório</span><span class="sxs-lookup"><span data-stu-id="2db4a-177">Format of the report files</span></span>     |
|    <span data-ttu-id="2db4a-178">TotalCount</span><span class="sxs-lookup"><span data-stu-id="2db4a-178">TotalCount</span></span>     |    <span data-ttu-id="2db4a-179">Número de conjuntos de dados na matriz de valores</span><span class="sxs-lookup"><span data-stu-id="2db4a-179">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="2db4a-180">Mensagem</span><span class="sxs-lookup"><span data-stu-id="2db4a-180">Message</span></span>     |    <span data-ttu-id="2db4a-181">Mensagem do status da execução da API</span><span class="sxs-lookup"><span data-stu-id="2db4a-181">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="2db4a-182">StatusCode</span><span class="sxs-lookup"><span data-stu-id="2db4a-182">StatusCode</span></span>     |    <span data-ttu-id="2db4a-183">Código de resultado.</span><span class="sxs-lookup"><span data-stu-id="2db4a-183">Result Code.</span></span> <span data-ttu-id="2db4a-184">Os valores possíveis são 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="2db4a-184">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
