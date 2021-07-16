---
title: Atualizar API de relatório
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Use esta API para atualizar parâmetros de relatório no Partner Center insights.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: c5ab1059e9be9b42918d268da6a6c1a3cbfe52af
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114374850"
---
# <a name="update-report-api"></a><span data-ttu-id="d7db3-103">Atualizar API de relatório</span><span class="sxs-lookup"><span data-stu-id="d7db3-103">Update report API</span></span>

<span data-ttu-id="d7db3-104">Essa API ajuda a modificar um parâmetro de relatório.</span><span class="sxs-lookup"><span data-stu-id="d7db3-104">This API helps you modify a report parameter.</span></span>

<span data-ttu-id="d7db3-105">**Sintaxe da solicitação**</span><span class="sxs-lookup"><span data-stu-id="d7db3-105">**Request syntax**</span></span>

|    <span data-ttu-id="d7db3-106">Método</span><span class="sxs-lookup"><span data-stu-id="d7db3-106">Method</span></span>    |    <span data-ttu-id="d7db3-107">URI da solicitação</span><span class="sxs-lookup"><span data-stu-id="d7db3-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="d7db3-108">PUT</span><span class="sxs-lookup"><span data-stu-id="d7db3-108">PUT</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
|        |        |

<span data-ttu-id="d7db3-109">**Cabeçalho da solicitação**</span><span class="sxs-lookup"><span data-stu-id="d7db3-109">**Request header**</span></span>

|    <span data-ttu-id="d7db3-110">parâmetro</span><span class="sxs-lookup"><span data-stu-id="d7db3-110">Header</span></span>    |    <span data-ttu-id="d7db3-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7db3-111">Type</span></span>    |    <span data-ttu-id="d7db3-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7db3-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="d7db3-113">Autorização</span><span class="sxs-lookup"><span data-stu-id="d7db3-113">Authorization</span></span>    |    <span data-ttu-id="d7db3-114">string</span><span class="sxs-lookup"><span data-stu-id="d7db3-114">string</span></span>    |    <span data-ttu-id="d7db3-115">Obrigatórios.</span><span class="sxs-lookup"><span data-stu-id="d7db3-115">Required.</span></span> <span data-ttu-id="d7db3-116">o token de acesso do Azure Active Directory (AAD) no formulário`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="d7db3-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="d7db3-117">Tipo de conteúdo</span><span class="sxs-lookup"><span data-stu-id="d7db3-117">Content-Type</span></span>    |    <span data-ttu-id="d7db3-118">string</span><span class="sxs-lookup"><span data-stu-id="d7db3-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="d7db3-119">**Parâmetro de caminho**</span><span class="sxs-lookup"><span data-stu-id="d7db3-119">**Path parameter**</span></span>

|    <span data-ttu-id="d7db3-120">Nome do Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d7db3-120">Parameter Name</span></span>    |    <span data-ttu-id="d7db3-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7db3-121">Type</span></span>    |    <span data-ttu-id="d7db3-122">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="d7db3-122">Required</span></span>    |    <span data-ttu-id="d7db3-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7db3-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="d7db3-124">reportId</span><span class="sxs-lookup"><span data-stu-id="d7db3-124">reportId</span></span>     |    <span data-ttu-id="d7db3-125">string</span><span class="sxs-lookup"><span data-stu-id="d7db3-125">string</span></span>    |    <span data-ttu-id="d7db3-126">Não</span><span class="sxs-lookup"><span data-stu-id="d7db3-126">No</span></span>    |    <span data-ttu-id="d7db3-127">ID do relatório que está sendo modificado</span><span class="sxs-lookup"><span data-stu-id="d7db3-127">ID of the report being modified</span></span>     |
|        |        |        |        |

<span data-ttu-id="d7db3-128">**Parâmetro de consulta**</span><span class="sxs-lookup"><span data-stu-id="d7db3-128">**Query parameter**</span></span>

<span data-ttu-id="d7db3-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d7db3-129">None</span></span>

<span data-ttu-id="d7db3-130">**Carga de solicitação**</span><span class="sxs-lookup"><span data-stu-id="d7db3-130">**Request payload**</span></span>

```json
{ 
  "ReportName": "string", 
  "Description": "string", 
  "StartTime": "string", 
  "RecurrenceInterval": 0, 
  "RecurrenceCount": 0, 
  "Format": "string", 
  "CallbackUrl": "string",
 "CallbackMethod": "string"
}
```

<span data-ttu-id="d7db3-131">**Glossário**</span><span class="sxs-lookup"><span data-stu-id="d7db3-131">**Glossary**</span></span>

<span data-ttu-id="d7db3-132">Esta tabela lista as principais definições dos elementos da resposta.</span><span class="sxs-lookup"><span data-stu-id="d7db3-132">This table lists the key definitions of elements in the response.</span></span>

|    <span data-ttu-id="d7db3-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d7db3-133">Parameter</span></span>    |    <span data-ttu-id="d7db3-134">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="d7db3-134">Required</span></span>    |    <span data-ttu-id="d7db3-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7db3-135">Description</span></span>    |    <span data-ttu-id="d7db3-136">Valores Permitidos</span><span class="sxs-lookup"><span data-stu-id="d7db3-136">Allowed Values</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="d7db3-137">ReportName</span><span class="sxs-lookup"><span data-stu-id="d7db3-137">ReportName</span></span>     |    <span data-ttu-id="d7db3-138">Yes</span><span class="sxs-lookup"><span data-stu-id="d7db3-138">Yes</span></span>     |    <span data-ttu-id="d7db3-139">Nome a ser atribuído ao relatório</span><span class="sxs-lookup"><span data-stu-id="d7db3-139">Name to be assigned to the report</span></span>     |    <span data-ttu-id="d7db3-140">String</span><span class="sxs-lookup"><span data-stu-id="d7db3-140">String</span></span>     |
|    <span data-ttu-id="d7db3-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7db3-141">Description</span></span>     |    <span data-ttu-id="d7db3-142">Não</span><span class="sxs-lookup"><span data-stu-id="d7db3-142">No</span></span>     |    <span data-ttu-id="d7db3-143">Descrição do relatório criado</span><span class="sxs-lookup"><span data-stu-id="d7db3-143">Description of the created report</span></span>     |    <span data-ttu-id="d7db3-144">String</span><span class="sxs-lookup"><span data-stu-id="d7db3-144">String</span></span>     |
|    <span data-ttu-id="d7db3-145">StartTime</span><span class="sxs-lookup"><span data-stu-id="d7db3-145">StartTime</span></span>     |    <span data-ttu-id="d7db3-146">Yes</span><span class="sxs-lookup"><span data-stu-id="d7db3-146">Yes</span></span>    |    <span data-ttu-id="d7db3-147">Carimbo de data/hora após o qual a geração de relatório será iniciada</span><span class="sxs-lookup"><span data-stu-id="d7db3-147">Timestamp after which the report generation will begin</span></span>     |    <span data-ttu-id="d7db3-148">String</span><span class="sxs-lookup"><span data-stu-id="d7db3-148">String</span></span>     |
|    <span data-ttu-id="d7db3-149">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="d7db3-149">RecurrenceInterval</span></span>     |    <span data-ttu-id="d7db3-150">No</span><span class="sxs-lookup"><span data-stu-id="d7db3-150">No</span></span>     |    <span data-ttu-id="d7db3-151">Frequência em horas em que o relatório deve ser gerado.</span><span class="sxs-lookup"><span data-stu-id="d7db3-151">Frequency at which the report should be generated in hours.</span></span> <span data-ttu-id="d7db3-152">O valor mínimo é 4</span><span class="sxs-lookup"><span data-stu-id="d7db3-152">Minimum value is 4</span></span>     |    <span data-ttu-id="d7db3-153">Integer</span><span class="sxs-lookup"><span data-stu-id="d7db3-153">Integer</span></span>     |
|    <span data-ttu-id="d7db3-154">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="d7db3-154">RecurrenceCount</span></span>     |    <span data-ttu-id="d7db3-155">Não</span><span class="sxs-lookup"><span data-stu-id="d7db3-155">No</span></span>     |    <span data-ttu-id="d7db3-156">Números de relatório a ser gerado.</span><span class="sxs-lookup"><span data-stu-id="d7db3-156">Numbers of report to be generated.</span></span> <span data-ttu-id="d7db3-157">O padrão é indefinido.</span><span class="sxs-lookup"><span data-stu-id="d7db3-157">Default is indefinite.</span></span>     |    <span data-ttu-id="d7db3-158">Integer</span><span class="sxs-lookup"><span data-stu-id="d7db3-158">Integer</span></span>     |
|    <span data-ttu-id="d7db3-159">Formatar</span><span class="sxs-lookup"><span data-stu-id="d7db3-159">Format</span></span>     |    <span data-ttu-id="d7db3-160">Não</span><span class="sxs-lookup"><span data-stu-id="d7db3-160">No</span></span>    |    <span data-ttu-id="d7db3-161">Formato de arquivo do arquivo exportado.</span><span class="sxs-lookup"><span data-stu-id="d7db3-161">File format of the exported file.</span></span> <span data-ttu-id="d7db3-162">O padrão é CSV</span><span class="sxs-lookup"><span data-stu-id="d7db3-162">Default is CSV</span></span>     |    <span data-ttu-id="d7db3-163">CSV/TSV</span><span class="sxs-lookup"><span data-stu-id="d7db3-163">CSV/TSV</span></span>     |
|    <span data-ttu-id="d7db3-164">CallbackURL</span><span class="sxs-lookup"><span data-stu-id="d7db3-164">CallbackURL</span></span>     |    <span data-ttu-id="d7db3-165">Não</span><span class="sxs-lookup"><span data-stu-id="d7db3-165">No</span></span>     |    <span data-ttu-id="d7db3-166">URL de retorno de chamada https a ser chamada na geração de relatório</span><span class="sxs-lookup"><span data-stu-id="d7db3-166">https callback URL to be called on report generation</span></span>     |    <span data-ttu-id="d7db3-167">String</span><span class="sxs-lookup"><span data-stu-id="d7db3-167">String</span></span>     |
|    <span data-ttu-id="d7db3-168">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="d7db3-168">CallbackMethod</span></span>    |    <span data-ttu-id="d7db3-169">Não</span><span class="sxs-lookup"><span data-stu-id="d7db3-169">No</span></span>    |    <span data-ttu-id="d7db3-170">Método http a ser usado para retorno de chamada</span><span class="sxs-lookup"><span data-stu-id="d7db3-170">Http method to be used for callback</span></span>    |    <span data-ttu-id="d7db3-171">OBTER/POSTAR</span><span class="sxs-lookup"><span data-stu-id="d7db3-171">GET/POST</span></span>    |
|        |        |        |        |


<span data-ttu-id="d7db3-172">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="d7db3-172">**Response**</span></span>

<span data-ttu-id="d7db3-173">A carga de solicitação é estrutura conforme a seguir:</span><span class="sxs-lookup"><span data-stu-id="d7db3-173">The response payload is structured as follows:</span></span>

<span data-ttu-id="d7db3-174">Código de resposta: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="d7db3-174">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="d7db3-175">Exemplo de conteúdo de resposta:</span><span class="sxs-lookup"><span data-stu-id="d7db3-175">Response payload example:</span></span>

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

<span data-ttu-id="d7db3-176">**Glossário**</span><span class="sxs-lookup"><span data-stu-id="d7db3-176">**Glossary**</span></span>

<span data-ttu-id="d7db3-177">Esta tabela define os principais elementos na resposta:</span><span class="sxs-lookup"><span data-stu-id="d7db3-177">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="d7db3-178">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d7db3-178">Parameter</span></span>    |    <span data-ttu-id="d7db3-179">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7db3-179">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="d7db3-180">ReportId</span><span class="sxs-lookup"><span data-stu-id="d7db3-180">ReportId</span></span>     |    <span data-ttu-id="d7db3-181">UUID (identificador universal exclusivo) do relatório sendo atualizado</span><span class="sxs-lookup"><span data-stu-id="d7db3-181">Universally unique identifier (UUID) of the report being updated</span></span>     |
|    <span data-ttu-id="d7db3-182">ReportName</span><span class="sxs-lookup"><span data-stu-id="d7db3-182">ReportName</span></span>     |    <span data-ttu-id="d7db3-183">Nome fornecido ao relatório na carga de solicitação</span><span class="sxs-lookup"><span data-stu-id="d7db3-183">Name given to the report in the request payload</span></span>     |
|    <span data-ttu-id="d7db3-184">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7db3-184">Description</span></span>     |    <span data-ttu-id="d7db3-185">Descrição fornecida ao relatório na carga de solicitação</span><span class="sxs-lookup"><span data-stu-id="d7db3-185">Description given to the report in the request payload</span></span>     |
|    <span data-ttu-id="d7db3-186">QueryId</span><span class="sxs-lookup"><span data-stu-id="d7db3-186">QueryId</span></span>     |    <span data-ttu-id="d7db3-187">ID de consulta passada no momento da criação do relatório</span><span class="sxs-lookup"><span data-stu-id="d7db3-187">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="d7db3-188">Consulta</span><span class="sxs-lookup"><span data-stu-id="d7db3-188">Query</span></span>     |    <span data-ttu-id="d7db3-189">Texto da consulta que será executada para este relatório</span><span class="sxs-lookup"><span data-stu-id="d7db3-189">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="d7db3-190">Usuário</span><span class="sxs-lookup"><span data-stu-id="d7db3-190">User</span></span>     |    <span data-ttu-id="d7db3-191">ID de usuário usada para criar o relatório</span><span class="sxs-lookup"><span data-stu-id="d7db3-191">User ID used to create the report</span></span>     |
|    <span data-ttu-id="d7db3-192">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="d7db3-192">CreatedTime</span></span>     |    <span data-ttu-id="d7db3-193">Hora de criação do relatório.</span><span class="sxs-lookup"><span data-stu-id="d7db3-193">Time the report was created.</span></span> <span data-ttu-id="d7db3-194">O formato de hora é aaaa-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="d7db3-194">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="d7db3-195">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="d7db3-195">ModifiedTime</span></span>     |    <span data-ttu-id="d7db3-196">Hora em que o relatório foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="d7db3-196">Time the report was last modified.</span></span> <span data-ttu-id="d7db3-197">O formato de hora é aaaa-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="d7db3-197">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="d7db3-198">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="d7db3-198">ExecuteNow</span></span>     |    <span data-ttu-id="d7db3-199">Sinalizador ExecuteNow definido no momento em que o relatório foi criado</span><span class="sxs-lookup"><span data-stu-id="d7db3-199">ExecuteNow flag set at the time the report was created</span></span>    |
|    <span data-ttu-id="d7db3-200">StartTime</span><span class="sxs-lookup"><span data-stu-id="d7db3-200">StartTime</span></span>     |    <span data-ttu-id="d7db3-201">Hora em que a execução do relatório será iniciada.</span><span class="sxs-lookup"><span data-stu-id="d7db3-201">Time the report execution will begin.</span></span> <span data-ttu-id="d7db3-202">O formato de hora é aaaa-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="d7db3-202">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="d7db3-203">Reportstatus</span><span class="sxs-lookup"><span data-stu-id="d7db3-203">ReportStatus</span></span>     |    <span data-ttu-id="d7db3-204">Status da execução do relatório.</span><span class="sxs-lookup"><span data-stu-id="d7db3-204">Status of the report execution.</span></span> <span data-ttu-id="d7db3-205">Os valores possíveis são Pausado, Ativo e Inativo.</span><span class="sxs-lookup"><span data-stu-id="d7db3-205">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="d7db3-206">RecorrênciaInterval</span><span class="sxs-lookup"><span data-stu-id="d7db3-206">RecurrenceInterval</span></span>     |    <span data-ttu-id="d7db3-207">Intervalo de recorrência fornecido no payload da solicitação</span><span class="sxs-lookup"><span data-stu-id="d7db3-207">Recurrence interval provided in the request payload</span></span>     |
|    <span data-ttu-id="d7db3-208">RecorrênciaCount</span><span class="sxs-lookup"><span data-stu-id="d7db3-208">RecurrenceCount</span></span>     |    <span data-ttu-id="d7db3-209">Contagem de recorrência fornecida no payload da solicitação</span><span class="sxs-lookup"><span data-stu-id="d7db3-209">Recurrence count provided in the request payload</span></span>     |
|    <span data-ttu-id="d7db3-210">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="d7db3-210">CallbackUrl</span></span>     |    <span data-ttu-id="d7db3-211">URL de retorno de chamada fornecida na solicitação</span><span class="sxs-lookup"><span data-stu-id="d7db3-211">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="d7db3-212">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="d7db3-212">CallbackMethod</span></span>    |    <span data-ttu-id="d7db3-213">Método de retorno de chamada fornecido na solicitação</span><span class="sxs-lookup"><span data-stu-id="d7db3-213">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="d7db3-214">Formatar</span><span class="sxs-lookup"><span data-stu-id="d7db3-214">Format</span></span>     |    <span data-ttu-id="d7db3-215">Formato dos arquivos do relatório</span><span class="sxs-lookup"><span data-stu-id="d7db3-215">Format of the report files</span></span>     |
|    <span data-ttu-id="d7db3-216">TotalCount</span><span class="sxs-lookup"><span data-stu-id="d7db3-216">TotalCount</span></span>     |    <span data-ttu-id="d7db3-217">Número de conjuntos de dados na matriz de valores</span><span class="sxs-lookup"><span data-stu-id="d7db3-217">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="d7db3-218">Mensagem</span><span class="sxs-lookup"><span data-stu-id="d7db3-218">Message</span></span>     |    <span data-ttu-id="d7db3-219">Mensagem do status da execução da API</span><span class="sxs-lookup"><span data-stu-id="d7db3-219">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="d7db3-220">StatusCode</span><span class="sxs-lookup"><span data-stu-id="d7db3-220">StatusCode</span></span>     |    <span data-ttu-id="d7db3-221">Código de resultado.</span><span class="sxs-lookup"><span data-stu-id="d7db3-221">Result Code.</span></span> <span data-ttu-id="d7db3-222">Os valores possíveis são 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="d7db3-222">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |