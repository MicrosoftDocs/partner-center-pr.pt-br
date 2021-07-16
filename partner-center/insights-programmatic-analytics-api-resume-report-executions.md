---
title: retomar API de execução de relatório-Insights dados
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Use essa API para retomar a execução de qualquer relatório em pausa no Partner Center insights.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 1372823425f3aefd025ffc3441623c1ceee34e1e
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114374855"
---
# <a name="resume-report-executions-api"></a><span data-ttu-id="165f5-103">Retomar API de execuções de relatório</span><span class="sxs-lookup"><span data-stu-id="165f5-103">Resume report executions API</span></span>

<span data-ttu-id="165f5-104">Na execução, essa API retoma a execução agendada de um relatório em pausa.</span><span class="sxs-lookup"><span data-stu-id="165f5-104">On execution, this API resumes the scheduled execution of a paused report.</span></span>

<span data-ttu-id="165f5-105">**Sintaxe da solicitação**</span><span class="sxs-lookup"><span data-stu-id="165f5-105">**Request syntax**</span></span>

|    <span data-ttu-id="165f5-106">Método</span><span class="sxs-lookup"><span data-stu-id="165f5-106">Method</span></span>    |    <span data-ttu-id="165f5-107">URI da solicitação</span><span class="sxs-lookup"><span data-stu-id="165f5-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="165f5-108">PUT</span><span class="sxs-lookup"><span data-stu-id="165f5-108">PUT</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/resume/{ReportID}`    |
|        |        |

<span data-ttu-id="165f5-109">**Cabeçalho da solicitação**</span><span class="sxs-lookup"><span data-stu-id="165f5-109">**Request header**</span></span>

|    <span data-ttu-id="165f5-110">parâmetro</span><span class="sxs-lookup"><span data-stu-id="165f5-110">Header</span></span>    |    <span data-ttu-id="165f5-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="165f5-111">Type</span></span>    |    <span data-ttu-id="165f5-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="165f5-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="165f5-113">Autorização</span><span class="sxs-lookup"><span data-stu-id="165f5-113">Authorization</span></span>    |    <span data-ttu-id="165f5-114">string</span><span class="sxs-lookup"><span data-stu-id="165f5-114">string</span></span>    |    <span data-ttu-id="165f5-115">Obrigatórios.</span><span class="sxs-lookup"><span data-stu-id="165f5-115">Required.</span></span> <span data-ttu-id="165f5-116">o token de acesso do Azure Active Directory (AAD) no formulário`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="165f5-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="165f5-117">Tipo de conteúdo</span><span class="sxs-lookup"><span data-stu-id="165f5-117">Content-Type</span></span>    |    <span data-ttu-id="165f5-118">string</span><span class="sxs-lookup"><span data-stu-id="165f5-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="165f5-119">**Parâmetro de caminho**</span><span class="sxs-lookup"><span data-stu-id="165f5-119">**Path parameter**</span></span>

|    <span data-ttu-id="165f5-120">Nome do Parâmetro</span><span class="sxs-lookup"><span data-stu-id="165f5-120">Parameter Name</span></span>    |    <span data-ttu-id="165f5-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="165f5-121">Type</span></span>    |    <span data-ttu-id="165f5-122">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="165f5-122">Required</span></span>    |    <span data-ttu-id="165f5-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="165f5-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="165f5-124">reportId</span><span class="sxs-lookup"><span data-stu-id="165f5-124">reportId</span></span>     |    <span data-ttu-id="165f5-125">string</span><span class="sxs-lookup"><span data-stu-id="165f5-125">string</span></span>    |    <span data-ttu-id="165f5-126">Não</span><span class="sxs-lookup"><span data-stu-id="165f5-126">No</span></span>    |    <span data-ttu-id="165f5-127">ID do relatório que está sendo modificado</span><span class="sxs-lookup"><span data-stu-id="165f5-127">ID of the report being modified</span></span>     |
|        |        |        |        |

<span data-ttu-id="165f5-128">**Parâmetro de consulta**</span><span class="sxs-lookup"><span data-stu-id="165f5-128">**Query parameter**</span></span>

<span data-ttu-id="165f5-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="165f5-129">None</span></span>

<span data-ttu-id="165f5-130">**Carga de solicitação**</span><span class="sxs-lookup"><span data-stu-id="165f5-130">**Request payload**</span></span>

<span data-ttu-id="165f5-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="165f5-131">None</span></span>

<span data-ttu-id="165f5-132">**Glossário**</span><span class="sxs-lookup"><span data-stu-id="165f5-132">**Glossary**</span></span>

<span data-ttu-id="165f5-133">Não</span><span class="sxs-lookup"><span data-stu-id="165f5-133">None</span></span>

<span data-ttu-id="165f5-134">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="165f5-134">**Response**</span></span>

<span data-ttu-id="165f5-135">A carga de solicitação é estrutura conforme a seguir:</span><span class="sxs-lookup"><span data-stu-id="165f5-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="165f5-136">Código de resposta: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="165f5-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="165f5-137">Exemplo de conteúdo de resposta:</span><span class="sxs-lookup"><span data-stu-id="165f5-137">Response payload example:</span></span>

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

<span data-ttu-id="165f5-138">**Glossário**</span><span class="sxs-lookup"><span data-stu-id="165f5-138">**Glossary**</span></span>

<span data-ttu-id="165f5-139">Esta tabela define os principais elementos na resposta:</span><span class="sxs-lookup"><span data-stu-id="165f5-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="165f5-140">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="165f5-140">Parameter</span></span>    |    <span data-ttu-id="165f5-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="165f5-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="165f5-142">ReportId</span><span class="sxs-lookup"><span data-stu-id="165f5-142">ReportId</span></span>     |    <span data-ttu-id="165f5-143">Identificador universal exclusivo (UUID) do relatório retomado</span><span class="sxs-lookup"><span data-stu-id="165f5-143">Universally unique identifier (UUID) of the resumed report</span></span>     |
|    <span data-ttu-id="165f5-144">ReportName</span><span class="sxs-lookup"><span data-stu-id="165f5-144">ReportName</span></span>     |    <span data-ttu-id="165f5-145">Nome dado ao relatório durante a criação</span><span class="sxs-lookup"><span data-stu-id="165f5-145">Name given to the report during creation</span></span>     |
|    <span data-ttu-id="165f5-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="165f5-146">Description</span></span>     |    <span data-ttu-id="165f5-147">Descrição fornecida durante a criação do relatório</span><span class="sxs-lookup"><span data-stu-id="165f5-147">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="165f5-148">QueryId</span><span class="sxs-lookup"><span data-stu-id="165f5-148">QueryId</span></span>     |    <span data-ttu-id="165f5-149">ID de consulta passada no momento da criação do relatório</span><span class="sxs-lookup"><span data-stu-id="165f5-149">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="165f5-150">Consulta</span><span class="sxs-lookup"><span data-stu-id="165f5-150">Query</span></span>     |    <span data-ttu-id="165f5-151">Texto da consulta que será executada para este relatório</span><span class="sxs-lookup"><span data-stu-id="165f5-151">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="165f5-152">Usuário</span><span class="sxs-lookup"><span data-stu-id="165f5-152">User</span></span>     |    <span data-ttu-id="165f5-153">ID de usuário usada para criar o relatório</span><span class="sxs-lookup"><span data-stu-id="165f5-153">User ID used to create the report</span></span>     |
|    <span data-ttu-id="165f5-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="165f5-154">CreatedTime</span></span>     |    <span data-ttu-id="165f5-155">Hora de criação do relatório.</span><span class="sxs-lookup"><span data-stu-id="165f5-155">Time the report was created.</span></span> <span data-ttu-id="165f5-156">O formato de hora é aaaa-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="165f5-156">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="165f5-157">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="165f5-157">ModifiedTime</span></span>     |    <span data-ttu-id="165f5-158">Hora em que o relatório foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="165f5-158">Time the report was last modified.</span></span> <span data-ttu-id="165f5-159">O formato de hora é aaaa-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="165f5-159">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="165f5-160">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="165f5-160">ExecuteNow</span></span>     |    <span data-ttu-id="165f5-161">Sinalizador ExecuteNow definido no momento em que o relatório foi criado</span><span class="sxs-lookup"><span data-stu-id="165f5-161">ExecuteNow flag set at the time the report was created</span></span>    |
|    <span data-ttu-id="165f5-162">StartTime</span><span class="sxs-lookup"><span data-stu-id="165f5-162">StartTime</span></span>     |    <span data-ttu-id="165f5-163">Hora em que a execução do relatório será iniciada.</span><span class="sxs-lookup"><span data-stu-id="165f5-163">Time the report execution will begin.</span></span> <span data-ttu-id="165f5-164">O formato de hora é aaaa-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="165f5-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="165f5-165">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="165f5-165">ReportStatus</span></span>     |    <span data-ttu-id="165f5-166">Status da execução do relatório.</span><span class="sxs-lookup"><span data-stu-id="165f5-166">Status of the report execution.</span></span> <span data-ttu-id="165f5-167">Os valores possíveis são Pausado, Ativo e Inativo.</span><span class="sxs-lookup"><span data-stu-id="165f5-167">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="165f5-168">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="165f5-168">RecurrenceInterval</span></span>     |    <span data-ttu-id="165f5-169">Intervalo de recorrência fornecido durante a criação do relatório</span><span class="sxs-lookup"><span data-stu-id="165f5-169">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="165f5-170">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="165f5-170">RecurrenceCount</span></span>     |    <span data-ttu-id="165f5-171">Contagem de recorrência fornecida durante a criação do relatório</span><span class="sxs-lookup"><span data-stu-id="165f5-171">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="165f5-172">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="165f5-172">CallbackUrl</span></span>     |    <span data-ttu-id="165f5-173">URL de retorno de chamada fornecida na solicitação</span><span class="sxs-lookup"><span data-stu-id="165f5-173">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="165f5-174">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="165f5-174">CallbackMethod</span></span>    |    <span data-ttu-id="165f5-175">Método de retorno de chamada fornecido na solicitação</span><span class="sxs-lookup"><span data-stu-id="165f5-175">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="165f5-176">Formatar</span><span class="sxs-lookup"><span data-stu-id="165f5-176">Format</span></span>     |    <span data-ttu-id="165f5-177">Formato dos arquivos do relatório</span><span class="sxs-lookup"><span data-stu-id="165f5-177">Format of the report files</span></span>     |
|    <span data-ttu-id="165f5-178">TotalCount</span><span class="sxs-lookup"><span data-stu-id="165f5-178">TotalCount</span></span>     |    <span data-ttu-id="165f5-179">Número de conjuntos de dados na matriz de valores</span><span class="sxs-lookup"><span data-stu-id="165f5-179">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="165f5-180">Mensagem</span><span class="sxs-lookup"><span data-stu-id="165f5-180">Message</span></span>     |    <span data-ttu-id="165f5-181">Mensagem do status da execução da API</span><span class="sxs-lookup"><span data-stu-id="165f5-181">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="165f5-182">StatusCode</span><span class="sxs-lookup"><span data-stu-id="165f5-182">StatusCode</span></span>     |    <span data-ttu-id="165f5-183">Código de resultado.</span><span class="sxs-lookup"><span data-stu-id="165f5-183">Result Code.</span></span> <span data-ttu-id="165f5-184">Os valores possíveis são 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="165f5-184">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
