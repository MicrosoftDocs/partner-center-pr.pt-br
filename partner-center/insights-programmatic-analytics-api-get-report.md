---
title: obter API de relatório-dados de Insights
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Use esta API para obter toda a ID de relatório disponível no Partner Center insights.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 174a2f60a36cb46b287b787b177dd32236cef4eb
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114374858"
---
# <a name="get-report-api"></a><span data-ttu-id="af660-103">Obter API de relatório</span><span class="sxs-lookup"><span data-stu-id="af660-103">Get report API</span></span>

<span data-ttu-id="af660-104">Esta API Obtém todos os relatórios que foram agendados.</span><span class="sxs-lookup"><span data-stu-id="af660-104">This API gets all the reports that have been scheduled.</span></span>

<span data-ttu-id="af660-105">**Sintaxe da solicitação**</span><span class="sxs-lookup"><span data-stu-id="af660-105">**Request syntax**</span></span>

|    <span data-ttu-id="af660-106">Método</span><span class="sxs-lookup"><span data-stu-id="af660-106">Method</span></span>    |    <span data-ttu-id="af660-107">URI da solicitação</span><span class="sxs-lookup"><span data-stu-id="af660-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="af660-108">GET</span><span class="sxs-lookup"><span data-stu-id="af660-108">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport?reportId={Report ID}&reportName={Report Name}&queryId={Query ID}` |
|        |        |

<span data-ttu-id="af660-109">**Cabeçalho da solicitação**</span><span class="sxs-lookup"><span data-stu-id="af660-109">**Request header**</span></span>

|    <span data-ttu-id="af660-110">parâmetro</span><span class="sxs-lookup"><span data-stu-id="af660-110">Header</span></span>    |    <span data-ttu-id="af660-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="af660-111">Type</span></span>    |    <span data-ttu-id="af660-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="af660-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="af660-113">Autorização</span><span class="sxs-lookup"><span data-stu-id="af660-113">Authorization</span></span>    |    <span data-ttu-id="af660-114">string</span><span class="sxs-lookup"><span data-stu-id="af660-114">string</span></span>    |    <span data-ttu-id="af660-115">Obrigatórios.</span><span class="sxs-lookup"><span data-stu-id="af660-115">Required.</span></span> <span data-ttu-id="af660-116">o token de acesso do Azure Active Directory (AAD) no formulário`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="af660-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="af660-117">Tipo de conteúdo</span><span class="sxs-lookup"><span data-stu-id="af660-117">Content-Type</span></span>    |    <span data-ttu-id="af660-118">string</span><span class="sxs-lookup"><span data-stu-id="af660-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="af660-119">**Parâmetro de caminho**</span><span class="sxs-lookup"><span data-stu-id="af660-119">**Path parameter**</span></span>

<span data-ttu-id="af660-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="af660-120">None</span></span>

<span data-ttu-id="af660-121">**Parâmetro de consulta**</span><span class="sxs-lookup"><span data-stu-id="af660-121">**Query parameter**</span></span>

|    <span data-ttu-id="af660-122">Nome do Parâmetro</span><span class="sxs-lookup"><span data-stu-id="af660-122">Parameter Name</span></span>    |    <span data-ttu-id="af660-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="af660-123">Type</span></span>    |    <span data-ttu-id="af660-124">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="af660-124">Required</span></span>    |    <span data-ttu-id="af660-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="af660-125">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="af660-126">reportId</span><span class="sxs-lookup"><span data-stu-id="af660-126">reportId</span></span>     |    <span data-ttu-id="af660-127">string</span><span class="sxs-lookup"><span data-stu-id="af660-127">string</span></span>    |    <span data-ttu-id="af660-128">Não</span><span class="sxs-lookup"><span data-stu-id="af660-128">No</span></span>    |    <span data-ttu-id="af660-129">Filtre para obter detalhes de apenas relatórios com o ReportID fornecido neste argumento</span><span class="sxs-lookup"><span data-stu-id="af660-129">Filter to get details of only reports with the reportId given in this argument</span></span>     |
|    <span data-ttu-id="af660-130">reportName</span><span class="sxs-lookup"><span data-stu-id="af660-130">reportName</span></span>     |    <span data-ttu-id="af660-131">string</span><span class="sxs-lookup"><span data-stu-id="af660-131">string</span></span>    |    <span data-ttu-id="af660-132">Não</span><span class="sxs-lookup"><span data-stu-id="af660-132">No</span></span>    |    <span data-ttu-id="af660-133">Filtre para obter detalhes de apenas relatórios com o ReportName fornecido neste argumento</span><span class="sxs-lookup"><span data-stu-id="af660-133">Filter to get details of only reports with the reportName given in this argument</span></span>     |
|    <span data-ttu-id="af660-134">queryId</span><span class="sxs-lookup"><span data-stu-id="af660-134">queryId</span></span>     |    <span data-ttu-id="af660-135">string</span><span class="sxs-lookup"><span data-stu-id="af660-135">string</span></span>    |    <span data-ttu-id="af660-136">Não</span><span class="sxs-lookup"><span data-stu-id="af660-136">No</span></span>    |    <span data-ttu-id="af660-137">Filtre para obter detalhes de apenas relatórios com a QueryId fornecida neste argumento</span><span class="sxs-lookup"><span data-stu-id="af660-137">Filter to get details of only reports with the queryId given in this argument</span></span>     |
|        |        |        |        |


<span data-ttu-id="af660-138">**Carga de solicitação**</span><span class="sxs-lookup"><span data-stu-id="af660-138">**Request payload**</span></span>

<span data-ttu-id="af660-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="af660-139">None</span></span>

<span data-ttu-id="af660-140">**Glossário**</span><span class="sxs-lookup"><span data-stu-id="af660-140">**Glossary**</span></span>

<span data-ttu-id="af660-141">Não</span><span class="sxs-lookup"><span data-stu-id="af660-141">None</span></span>

<span data-ttu-id="af660-142">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="af660-142">**Response**</span></span>

<span data-ttu-id="af660-143">A carga de solicitação é estrutura conforme a seguir:</span><span class="sxs-lookup"><span data-stu-id="af660-143">The response payload is structured as follows:</span></span>

<span data-ttu-id="af660-144">Código de resposta: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="af660-144">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="af660-145">Exemplo de conteúdo de resposta:</span><span class="sxs-lookup"><span data-stu-id="af660-145">Response payload example:</span></span>

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
      "executeNow": true, 
      "StartTime": "string", 
      "ReportStatus": "string", 
      "RecurrenceInterval": 0, 
      " RecurrenceCount": 0, 
      "CallbackUrl": "string",
      "CallbackMethod": null,
      "Format": "string" 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0 
}
```

<span data-ttu-id="af660-146">**Glossário**</span><span class="sxs-lookup"><span data-stu-id="af660-146">**Glossary**</span></span>

<span data-ttu-id="af660-147">Esta tabela define os principais elementos na resposta:</span><span class="sxs-lookup"><span data-stu-id="af660-147">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="af660-148">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="af660-148">Parameter</span></span>    |    <span data-ttu-id="af660-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="af660-149">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="af660-150">ReportId</span><span class="sxs-lookup"><span data-stu-id="af660-150">ReportId</span></span>     |    <span data-ttu-id="af660-151">UUID exclusivo do relatório que foi criado</span><span class="sxs-lookup"><span data-stu-id="af660-151">Unique UUID of the report that was created</span></span>     |
|    <span data-ttu-id="af660-152">ReportName</span><span class="sxs-lookup"><span data-stu-id="af660-152">ReportName</span></span>     |    <span data-ttu-id="af660-153">Nome fornecido ao relatório na carga de solicitação</span><span class="sxs-lookup"><span data-stu-id="af660-153">Name given to the report in the request payload</span></span>     |
|    <span data-ttu-id="af660-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="af660-154">Description</span></span>     |    <span data-ttu-id="af660-155">Descrição fornecida quando o relatório foi criado</span><span class="sxs-lookup"><span data-stu-id="af660-155">Description given when the report was created</span></span>     |
|    <span data-ttu-id="af660-156">QueryId</span><span class="sxs-lookup"><span data-stu-id="af660-156">QueryId</span></span>     |    <span data-ttu-id="af660-157">ID de consulta passada no momento da criação do relatório</span><span class="sxs-lookup"><span data-stu-id="af660-157">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="af660-158">Consulta</span><span class="sxs-lookup"><span data-stu-id="af660-158">Query</span></span>     |    <span data-ttu-id="af660-159">Texto da consulta que será executada para este relatório</span><span class="sxs-lookup"><span data-stu-id="af660-159">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="af660-160">Usuário</span><span class="sxs-lookup"><span data-stu-id="af660-160">User</span></span>     |    <span data-ttu-id="af660-161">ID de usuário usada para criar o relatório</span><span class="sxs-lookup"><span data-stu-id="af660-161">User ID used to create the report</span></span>     |
|    <span data-ttu-id="af660-162">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="af660-162">CreatedTime</span></span>     |    <span data-ttu-id="af660-163">Hora de criação do relatório.</span><span class="sxs-lookup"><span data-stu-id="af660-163">Time the report was created.</span></span> <span data-ttu-id="af660-164">O formato de hora é aaaa-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="af660-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="af660-165">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="af660-165">ModifiedTime</span></span>     |    <span data-ttu-id="af660-166">Hora em que o relatório foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="af660-166">Time the report was last modified.</span></span> <span data-ttu-id="af660-167">O formato de hora é aaaa-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="af660-167">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="af660-168">executeNow</span><span class="sxs-lookup"><span data-stu-id="af660-168">executeNow</span></span>     |    <span data-ttu-id="af660-169">Sinalizador ExecuteNow definido no momento em que o relatório foi criado</span><span class="sxs-lookup"><span data-stu-id="af660-169">ExecuteNow flag set at the time the report was created</span></span>    |
|    <span data-ttu-id="af660-170">StartTime</span><span class="sxs-lookup"><span data-stu-id="af660-170">StartTime</span></span>     |    <span data-ttu-id="af660-171">A execução de tempo será iniciada.</span><span class="sxs-lookup"><span data-stu-id="af660-171">Time execution will begin.</span></span> <span data-ttu-id="af660-172">O formato de hora é aaaa-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="af660-172">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="af660-173">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="af660-173">ReportStatus</span></span>     |    <span data-ttu-id="af660-174">Status da execução do relatório.</span><span class="sxs-lookup"><span data-stu-id="af660-174">Status of the report execution.</span></span> <span data-ttu-id="af660-175">Os valores possíveis são Pausado, Ativo e Inativo.</span><span class="sxs-lookup"><span data-stu-id="af660-175">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="af660-176">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="af660-176">RecurrenceInterval</span></span>     |    <span data-ttu-id="af660-177">Intervalo de recorrência fornecido durante a criação do relatório</span><span class="sxs-lookup"><span data-stu-id="af660-177">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="af660-178">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="af660-178">RecurrenceCount</span></span>     |    <span data-ttu-id="af660-179">Contagem de recorrência fornecida durante a criação do relatório</span><span class="sxs-lookup"><span data-stu-id="af660-179">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="af660-180">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="af660-180">CallbackUrl</span></span>     |    <span data-ttu-id="af660-181">URL de retorno de chamada fornecida na solicitação</span><span class="sxs-lookup"><span data-stu-id="af660-181">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="af660-182">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="af660-182">CallbackMethod</span></span>    |    <span data-ttu-id="af660-183">Método de retorno de chamada fornecido na solicitação</span><span class="sxs-lookup"><span data-stu-id="af660-183">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="af660-184">Formatar</span><span class="sxs-lookup"><span data-stu-id="af660-184">Format</span></span>     |    <span data-ttu-id="af660-185">Formato dos arquivos do relatório</span><span class="sxs-lookup"><span data-stu-id="af660-185">Format of the report files</span></span>     |
|    <span data-ttu-id="af660-186">TotalCount</span><span class="sxs-lookup"><span data-stu-id="af660-186">TotalCount</span></span>     |    <span data-ttu-id="af660-187">Número de conjuntos de dados na matriz de valores</span><span class="sxs-lookup"><span data-stu-id="af660-187">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="af660-188">Mensagem</span><span class="sxs-lookup"><span data-stu-id="af660-188">Message</span></span>     |    <span data-ttu-id="af660-189">Mensagem do status da execução da API</span><span class="sxs-lookup"><span data-stu-id="af660-189">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="af660-190">StatusCode</span><span class="sxs-lookup"><span data-stu-id="af660-190">StatusCode</span></span>     |    <span data-ttu-id="af660-191">Código de resultado.</span><span class="sxs-lookup"><span data-stu-id="af660-191">Result Code.</span></span> <span data-ttu-id="af660-192">Os valores possíveis são 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="af660-192">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |