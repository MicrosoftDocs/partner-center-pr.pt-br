---
title: Cobrança do plano do Azure – arquivos de reconciliação e fatura
ms.topic: article
ms.date: 07/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como acessar e entender a estrutura do arquivo de reconciliação e da fatura relacionada à cobrança do plano do Azure.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 1dc683c194de158dc7a4dac541b37631f3be1f1e
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534685"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a><span data-ttu-id="c5a2f-103">Nova experiência de comércio no CSP – Cobrança do Azure</span><span class="sxs-lookup"><span data-stu-id="c5a2f-103">New commerce experience in CSP - Azure billing</span></span> 

<span data-ttu-id="c5a2f-104">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="c5a2f-104">**Appropriate roles**</span></span>

- <span data-ttu-id="c5a2f-105">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="c5a2f-105">Admin agent</span></span>
- <span data-ttu-id="c5a2f-106">Administrador de cobrança</span><span class="sxs-lookup"><span data-stu-id="c5a2f-106">Billing admin</span></span>
- <span data-ttu-id="c5a2f-107">Administrador global</span><span class="sxs-lookup"><span data-stu-id="c5a2f-107">Global admin</span></span>

<span data-ttu-id="c5a2f-108">Este artigo explica como acessar e entender a estrutura do arquivo de reconciliação e da fatura relacionada à cobrança do plano do Azure.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-108">This article explains how to access and understand the invoice and reconciliation file structure related to billing for the Azure plan.</span></span> <span data-ttu-id="c5a2f-109">A cobrança no âmbito do plano do Azure é uma experiência de cobrança simplificada usando uma data de cobrança única alinhada e um período de cobrança baseado no mês civil.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-109">Billing under the Azure plan is a simplified billing experience using an aligned single billing date and calendar month-based billing period.</span></span>

## <a name="summary-of-billing-essentials"></a><span data-ttu-id="c5a2f-110">Resumo dos conceitos básicos de cobrança</span><span class="sxs-lookup"><span data-stu-id="c5a2f-110">Summary of billing essentials</span></span>

- <span data-ttu-id="c5a2f-111">**Data da fatura**: A fatura e o arquivo de reconciliação estarão disponíveis na API/no Painel do Partner Center até o dia oito (à meia-noite, UTC).</span><span class="sxs-lookup"><span data-stu-id="c5a2f-111">**Invoice date**: Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).</span></span>

- <span data-ttu-id="c5a2f-112">**Período de cobrança da fatura**: O período de cobrança da fatura é alinhado ao mês civil, por exemplo, 1/10 – 31/10, 1/11 – 30/11.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-112">**Invoice billing period**: The invoice billing period is aligned to the calendar month, for example,  10/1-10/31, 11/1-11/30.</span></span>

- <span data-ttu-id="c5a2f-113">**Períodos de serviço de cobrança**: As cobranças serão alinhadas ao mês civil.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-113">**Charge service periods**: Charges will align to the calendar month.</span></span> <span data-ttu-id="c5a2f-114">Por exemplo, se o parceiro cobrado adicionar serviços do Azure por meio de um plano do Azure em 15/10 e o cliente iniciar o consumo de serviços do Azure em 10/15, então o parceiro cobrado receberá a fatura/o reconhecimento em 8/11 para o consumo do cliente referente ao período de serviço 15/10 – 31/10.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-114">For example, if billed partner adds Azure services through an Azure plan on 10/15 and the customer begins consumption of Azure services on 10/15, then billed partner will receive invoice/recon on 11/8 for customer consumption for the service period 10/15 - 10/31.</span></span> <span data-ttu-id="c5a2f-115">A fatura do próximo mês, que será gerada em 08/12, conterá todos os encargos referentes ao período de serviço de 01/11 – 31/11.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-115">The next month's invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.</span></span>

- <span data-ttu-id="c5a2f-116">**Condição de pagamento da fatura**: Líquido de 60 dias.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-116">**Invoice payment term**: Net 60 days.</span></span>

- <span data-ttu-id="c5a2f-117">**Moeda da fatura**: Os parceiros continuarão sendo cobrados na moeda atribuída ao país do cliente.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-117">**Invoice currency**: Partners will continue to be billed in the customer's country's assigned currency.</span></span> <span data-ttu-id="c5a2f-118">Por exemplo, se o parceiro cobrado estiver na Irlanda com clientes no Reino Unido, na Noruega e na Alemanha, ele receberá faturas/reconhecimentos em GBP, NOK e EUR.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-118">For example, if the billed partner is in Ireland with customers in the UK, Norway, and Germany, then the billed partner will receive a GBP, NOK, and EUR invoice/recon.</span></span>

- <span data-ttu-id="c5a2f-119">**Incentivos para Parceiros**: pago 45 dias após o final do mês da fatura.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-119">**Partner incentives**: Paid 45 days from the end of the invoice month.</span></span>

## <a name="access-your-invoices-and-reconciliation-files"></a><span data-ttu-id="c5a2f-120">Acessar seus arquivos de fatura e reconciliação</span><span class="sxs-lookup"><span data-stu-id="c5a2f-120">Access your invoices and reconciliation files</span></span>

<span data-ttu-id="c5a2f-121">O administrador global ou de cobrança da sua empresa receberá um email quando a fatura estiver pronta para ser exibida.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-121">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span>

<span data-ttu-id="c5a2f-122">Para acessar o arquivo de fatura e reconciliação:</span><span class="sxs-lookup"><span data-stu-id="c5a2f-122">To access the invoice and reconciliation file:</span></span>

1. <span data-ttu-id="c5a2f-123">Entre no [Painel](https://partner.microsoft.com/dashboard/) do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-123">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="c5a2f-124">No menu do Partner Center, selecione **Cobrança**.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-124">From the Partner Center menu, select **Billing**.</span></span>

3. <span data-ttu-id="c5a2f-125">Selecione a guia para a **Recorrente** e a **Única** e a moeda em que você está interessado.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-125">Select the tab for the **Recurring** and **One-time** and the currency you are interested in.</span></span>

   :::image type="content" source="images/azure/billing3.png" alt-text="cobrança":::

4. <span data-ttu-id="c5a2f-127">Selecione **Fatura** ou **Arquivo de reconciliação**.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-127">Select **Invoice** or **Reconciliation file**.</span></span>  

   <span data-ttu-id="c5a2f-128">Para exibir os arquivos históricos de faturas e reconhecimento, expanda a linha do histórico de cobrança, abaixo.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-128">To view historical invoices and recon files expand the Billing history row below.</span></span>

## <a name="understanding-usage-data"></a><span data-ttu-id="c5a2f-129">Noções básicas sobre dados de uso</span><span class="sxs-lookup"><span data-stu-id="c5a2f-129">Understanding usage data</span></span> 

1. <span data-ttu-id="c5a2f-130">O plano do Azure é o contêiner raiz ou de nível superior para uso.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-130">Azure plan is the root or top-level container for usage.</span></span> <span data-ttu-id="c5a2f-131">Todo o uso está vinculado de volta a um único plano do Azure.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-131">All usage is tied back to a single Azure plan.</span></span>

2. <span data-ttu-id="c5a2f-132">Em um plano, haverá uma ou mais assinaturas do Azure.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-132">Within a plan, there will be one or more Azure subscriptions.</span></span> <span data-ttu-id="c5a2f-133">Esses são contêineres usados para gerenciamento de recursos e implantação.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-133">These are containers used for resource management and deployment.</span></span> 

3. <span data-ttu-id="c5a2f-134">Em uma assinatura, os grupos de recursos são adicionados aos recursos de grupo.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-134">Within a subscription, resource groups add to group resources.</span></span> <span data-ttu-id="c5a2f-135">Cada recurso é implantado em um grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-135">Every resource is deployed to one resource group.</span></span> 

4. <span data-ttu-id="c5a2f-136">Exemplos de recursos incluem máquinas virtuais e contas de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-136">Examples of resources include virtual machines and storage accounts.</span></span> 

5. <span data-ttu-id="c5a2f-137">Medidores de emissão de recurso: Os medidores são medidas de consumo de um recurso, sendo que um recurso pode emitir o uso de vários medidores.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-137">Resource emit meters: Meters are measurements of consumption of a resource, and one resource may emit usage for multiple meters.</span></span> <span data-ttu-id="c5a2f-138">Os medidores são identificados por um ProductId, um SKUId e um AvailabilityId.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-138">Meters are identified by a ProductId, SKUId, and AvailabilityId.</span></span> 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a><span data-ttu-id="c5a2f-139">Hierarquia de grupos de recursos de assinatura e medição</span><span class="sxs-lookup"><span data-stu-id="c5a2f-139">Hierarchy of subscription resource groups and metering</span></span>

<span data-ttu-id="c5a2f-140">**Conta do Azure (locatário)**</span><span class="sxs-lookup"><span data-stu-id="c5a2f-140">**Azure account (tenant)**</span></span>

- <span data-ttu-id="c5a2f-141">Assinatura A</span><span class="sxs-lookup"><span data-stu-id="c5a2f-141">Subscription A</span></span>
    - <span data-ttu-id="c5a2f-142">ResourceGroup 1</span><span class="sxs-lookup"><span data-stu-id="c5a2f-142">ResourceGroup 1</span></span>
        - <span data-ttu-id="c5a2f-143">Máquina virtual (recurso)</span><span class="sxs-lookup"><span data-stu-id="c5a2f-143">Virtual machine (resource)</span></span>
            - <span data-ttu-id="c5a2f-144">Medidor de computação</span><span class="sxs-lookup"><span data-stu-id="c5a2f-144">Compute meter</span></span>
        - <span data-ttu-id="c5a2f-145">Rede virtual (recurso)</span><span class="sxs-lookup"><span data-stu-id="c5a2f-145">Virtual network (resource)</span></span>
            - <span data-ttu-id="c5a2f-146">Sem medidor de cobrança</span><span class="sxs-lookup"><span data-stu-id="c5a2f-146">No billing meter</span></span>

    - <span data-ttu-id="c5a2f-147">ResourceGroup 2</span><span class="sxs-lookup"><span data-stu-id="c5a2f-147">ResourceGroup 2</span></span>
        - <span data-ttu-id="c5a2f-148">Máquina virtual (recurso)</span><span class="sxs-lookup"><span data-stu-id="c5a2f-148">Virtual machine (resource)</span></span>
            - <span data-ttu-id="c5a2f-149">Medidor do computador</span><span class="sxs-lookup"><span data-stu-id="c5a2f-149">Computer meter</span></span>
        - <span data-ttu-id="c5a2f-150">Disco gerenciado por SSD Premium (recurso)</span><span class="sxs-lookup"><span data-stu-id="c5a2f-150">Premium SSD-managed disk (resource)</span></span>
            - <span data-ttu-id="c5a2f-151">Medidor de capacidade de armazenamento</span><span class="sxs-lookup"><span data-stu-id="c5a2f-151">Storage capacity meter</span></span>
            - <span data-ttu-id="c5a2f-152">Medidor de operações de armazenamento</span><span class="sxs-lookup"><span data-stu-id="c5a2f-152">Storage operations meter</span></span>

- <span data-ttu-id="c5a2f-153">Assinatura B   – ResourceGroup 1       – SQL do Azure (recurso)           – medidor DTU       – Gateway de VPN (recurso)           – medidor de Gateway de VPN</span><span class="sxs-lookup"><span data-stu-id="c5a2f-153">Subscription B   -ResourceGroup 1       - Azure SQL (resource)           - DTU meter       - VPN Gateway (resource)           - VPN gateway meter</span></span>

    - <span data-ttu-id="c5a2f-154">ResourceGroup 2</span><span class="sxs-lookup"><span data-stu-id="c5a2f-154">ResourceGroup 2</span></span>
        - <span data-ttu-id="c5a2f-155">Adaptador de rede virtual (recurso)</span><span class="sxs-lookup"><span data-stu-id="c5a2f-155">Virtual Network Interface (resource)</span></span>
            - <span data-ttu-id="c5a2f-156">Sem medidor de cobrança</span><span class="sxs-lookup"><span data-stu-id="c5a2f-156">No billing meter</span></span>

## <a name="read-the-invoice"></a><span data-ttu-id="c5a2f-157">Leia a fatura</span><span class="sxs-lookup"><span data-stu-id="c5a2f-157">Read the invoice</span></span>

1. <span data-ttu-id="c5a2f-158">A fatura estará disponível até o dia oito de cada mês.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-158">Invoice will be available no later than the eighth of each month.</span></span>

2. <span data-ttu-id="c5a2f-159">Os parceiros têm 60 dias para remeterem o pagamento.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-159">Partners have 60 days to remit payment.</span></span>

3. <span data-ttu-id="c5a2f-160">O período de cobrança abrangerá um determinado mês civil, por exemplo, de 1/10 – 31/10.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-160">The billing period will cover a given calendar month, for example, 10/1-10/31.</span></span>

4. <span data-ttu-id="c5a2f-161">As cobranças são líquidas de ajustes (o valor é líquido de "Créditos ganhos pelo parceiro para serviços gerenciados").</span><span class="sxs-lookup"><span data-stu-id="c5a2f-161">Charges are net of adjustments (amount is net of “Partner earned credit for services managed").</span></span>

5. <span data-ttu-id="c5a2f-162">Examine o arquivo de reconhecimento de fatura e o arquivo de uso de classificação diária para obter detalhes adicionais de cobrança.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-162">Review the invoice recon file and daily rated usage file for additional billing details.</span></span>

   :::image type="content" source="images/azure/invoice1.png" alt-text="fatura":::

## <a name="read-the-invoice-reconciliation-file"></a><span data-ttu-id="c5a2f-164">Ler o arquivo de reconciliação/fatura</span><span class="sxs-lookup"><span data-stu-id="c5a2f-164">Read the invoice reconciliation file</span></span>

1. <span data-ttu-id="c5a2f-165">Cada combinação de plano e medidor do Azure pode ter até duas linhas de cobrança no arquivo de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-165">Each Azure plan and meter combination may have up to two billing lines on the recon file.</span></span>

2. <span data-ttu-id="c5a2f-166">Se o medidor for qualificado para qualquer tipo de desconto ou crédito (como descontos por nível ou créditos ganhos pelo parceiro para serviços gerenciados) durante todo o mês civil, então o arquivo de reconciliação conterá apenas uma linha de cobrança.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-166">If the meter qualified for any type of discount or credit (such as tiered discounts or the Partner earned credit for services managed) throughout the entire calendar month, then the recon file will only contain one billing line.</span></span> <span data-ttu-id="c5a2f-167">A coluna **PriceAdjusmentDescription** fará referência ao desconto ou crédito obtido.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-167">The column **PriceAdjusmentDescription** will reference the discount or earned credit.</span></span>

3. <span data-ttu-id="c5a2f-168">Se não houver recursos para um medidor específico qualificado para o desconto ou créditos ganhos pelo parceiro, então o arquivo de reconciliação conterá apenas uma linha de cobrança e o preço unitário efetivo será o preço de varejo (que é o preço unitário).</span><span class="sxs-lookup"><span data-stu-id="c5a2f-168">If there are no resources for a particular meter that qualified for discount or partner earned credit, then the recon file will only contain one billing line and the effective unit price will be the retail price (which is the unit price).</span></span>

4. <span data-ttu-id="c5a2f-169">Se o medidor, ou os recursos que emitirem esse medidor, tiver se qualificado para **Créditos ganhos pelo parceiro para serviços gerenciados** em uma parte do mês, então o arquivo de reconciliação conterá duas linhas de cobrança.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-169">If the meter, or any resources emitting that meter, qualified for **Partner earned credit for services managed** for a part of the month, the recon file will contain two billing lines.</span></span> <span data-ttu-id="c5a2f-170">Uma linha representará os dias em que o medidor se qualificou, ao passo que a outra linha representará os dias em que o medidor não se qualificou.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-170">One line will represent the days the meter qualified and the second line will represent the days the meter did not qualify.</span></span>

## <a name="read-the-daily-usage-file"></a><span data-ttu-id="c5a2f-171">Ler o arquivo de uso diário</span><span class="sxs-lookup"><span data-stu-id="c5a2f-171">Read the daily usage file</span></span>

- <span data-ttu-id="c5a2f-172">Os medidores de assinatura no âmbito de um plano do Azure são classificados e acumulados diariamente.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-172">Subscription meters under an Azure plan are rated, and are cumulated, on a daily basis.</span></span>

- <span data-ttu-id="c5a2f-173">**O crédito ganho pelo parceiro para serviços gerenciados** é determinado e aplicado diariamente.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-173">**Partner earned credit for services managed** is determined and applied on a daily basis.</span></span>

- <span data-ttu-id="c5a2f-174">Cada medidor de assinatura terá uma linha para cada dia do mês em que houve consumo.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-174">Every subscription meter will have a row for every day of the month where there was consumption.</span></span>

- <span data-ttu-id="c5a2f-175">No exemplo a seguir:</span><span class="sxs-lookup"><span data-stu-id="c5a2f-175">In the example below:</span></span>

  - <span data-ttu-id="c5a2f-176">O medidor se qualificou para **Crédito ganho pelo parceiro para serviços gerenciados** de 01/07 – 03/07 (observe que o preço unitário efetivo é o preço de varejo menos os créditos ganhos pelo parceiro).</span><span class="sxs-lookup"><span data-stu-id="c5a2f-176">Meter qualified for **Partner earned credit for services managed** from 7/1 - 7/3 (note the effective unit price is retail price less partner earned credit.</span></span>

  - <span data-ttu-id="c5a2f-177">O medidor não se qualificou para **Crédito ganho pelo parceiro para serviços gerenciados** de 04/07 – 07/07 (observe que o preço unitário efetivo é o preço de varejo).</span><span class="sxs-lookup"><span data-stu-id="c5a2f-177">Meter didn't qualify for **Partner earned credit for services managed** from 7/4 - 7/7 (note the effective unit price is retail price).</span></span>

  - <span data-ttu-id="c5a2f-178">O medidor se qualificou para **Crédito ganho pelo parceiro para serviços gerenciados** de 08/07 – 31/07 (observe que o preço unitário efetivo é o preço de varejo menos os créditos ganhos pelo parceiro).</span><span class="sxs-lookup"><span data-stu-id="c5a2f-178">Meter qualified for **Partner earned credit for services managed** from 7/8 - 7/31 (note the effective unit price is retail price less partner earned credit).</span></span>

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2":::

## <a name="invoice-in-customer-currency"></a><span data-ttu-id="c5a2f-180">Fatura na moeda do cliente</span><span class="sxs-lookup"><span data-stu-id="c5a2f-180">Invoice in customer currency</span></span>

<span data-ttu-id="c5a2f-181">Os serviços do Azure por meio de um plano do Azure serão precificados em USD e cobrados na moeda atribuída ao país do cliente.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-181">Azure services through an Azure plan will be priced in USD and billed in the customer country assigned currency.</span></span> <span data-ttu-id="c5a2f-182">Se a moeda de cobrança não for USD, então a taxa de câmbio usada será mostrada na última página da fatura.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-182">If the billing currency is non-USD, then the Foreign exchange (FX) rate used will be shown on the last page of the invoice.</span></span> <span data-ttu-id="c5a2f-183">As taxas de câmbio são determinadas mensalmente e aplicadas à fatura a seguir.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-183">FX rates are determined monthly and applied to the following invoice.</span></span> <span data-ttu-id="c5a2f-184">Para obter uma lista completa de moedas por país, exiba a [matriz de moedas do cliente e a disponibilidade por país de novas ofertas de comércio](https://go.microsoft.com/fwlink/?linkid=2112354).</span><span class="sxs-lookup"><span data-stu-id="c5a2f-184">For a full list of country currencies, please view the [new commerce offers country availability and customer currency matrix](https://go.microsoft.com/fwlink/?linkid=2112354).</span></span>

<span data-ttu-id="c5a2f-185">A Microsoft usará o Thomson Reuters para determinar a taxa de FX para o preço da moeda para a conversão de cobrança.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-185">Microsoft will use Thomson Reuters to determine the FX rates used to determine pricing currency to billing currency conversion.</span></span> <span data-ttu-id="c5a2f-186">As taxas de câmbio serão atualizadas e disponibilizadas no dia anterior ao primeiro dia de cada mês em que forem aplicadas.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-186">The FX rates will be refreshed and available on the day before the first of the month for which they apply.</span></span>

<span data-ttu-id="c5a2f-187">**Exemplo**:  Os encargos de uso do período de serviço de 1º de agosto a 31 de agosto serão cobrados usando a taxa de câmbio publicada no dia 31 de julho.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-187">**Example**:  Usage charges for the service period August 1 - August 31 will be billed using the FX rate published on July 31.</span></span> <span data-ttu-id="c5a2f-188">Esses encargos serão exibidos na fatura de setembro e a taxa de câmbio poderá ser observada na última página da fatura.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-188">These charges will appear on the September invoice and the FX rate will be noted on the last page of the invoice.</span></span>

## <a name="azure-reservations"></a><span data-ttu-id="c5a2f-189">Reservas do Azure</span><span class="sxs-lookup"><span data-stu-id="c5a2f-189">Azure reservations</span></span>


<span data-ttu-id="c5a2f-190">Se você estiver comprando [reservas do Azure](azure-reservations.md) por meio de um plano do Azure, escolha a cobrança única ou mensal.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-190">If purchasing [Azure reservations](azure-reservations.md) through an Azure plan, you can choose either one-time or monthly billing.</span></span>


## <a name="azure-spending"></a><span data-ttu-id="c5a2f-191">Gastos do Azure</span><span class="sxs-lookup"><span data-stu-id="c5a2f-191">Azure spending</span></span>

<span data-ttu-id="c5a2f-192">A experiência de gastos do Azure existente é atualizada para dar suporte à nova cobrança do plano do Azure no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-192">The existing Azure spending experience is updated to support the new Azure plan billing in Partner Center.</span></span> <span data-ttu-id="c5a2f-193">Isso permite aos parceiros:</span><span class="sxs-lookup"><span data-stu-id="c5a2f-193">This enables partners to:</span></span>

- <span data-ttu-id="c5a2f-194">exibir, gerenciar e receber alertas do conjunto de orçamentos em um nível de cliente;</span><span class="sxs-lookup"><span data-stu-id="c5a2f-194">View, manage, and receive alerts for budget set at a customer level</span></span> 

- <span data-ttu-id="c5a2f-195">exibir o gasto total estimado em um plano do Azure (dividido por recurso e nível de medidor)</span><span class="sxs-lookup"><span data-stu-id="c5a2f-195">View total estimated spending on an Azure plan (broken down by resource and meter level)</span></span>

<span data-ttu-id="c5a2f-196">Já que o modelo de cobrança para os serviços do Azure por meio de um plano do Azure é o consumo pós-pago, para evitar uma cobrança maior do que o previsto, os parceiros podem aplicar um orçamento mensal e acompanhar o percentual de uso.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-196">Because the billing model for Azure services through an Azure plan is post-pay consumption, to avoid a bigger bill than anticipated, partners can apply a monthly budget and track the percentage of usage.</span></span> <span data-ttu-id="c5a2f-197">Um orçamento pode ser aplicado a um cliente ou a vários clientes ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-197">A budget can be applied to one customer or multiple customers at one time.</span></span> 

:::image type="content" source="images/azure/azurespend.png" alt-text="Gastos do Azure":::

## <a name="next-steps"></a><span data-ttu-id="c5a2f-199">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="c5a2f-199">Next steps</span></span>

- <span data-ttu-id="c5a2f-200">Veja como o PEC (crédito ganho pelo parceiro) é calculado.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-200">See how the partner earned credit (PEC) is calculated.</span></span> <span data-ttu-id="c5a2f-201">Entre no [Painel](https://partner.microsoft.com/dashboard/) do Partner Center e localize a lista de preços disponível.</span><span class="sxs-lookup"><span data-stu-id="c5a2f-201">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/) and locate the price list available.</span></span>

- <span data-ttu-id="c5a2f-202">Saiba mais sobre [como comprar o plano do Azure](purchase-azure-plan.md)</span><span class="sxs-lookup"><span data-stu-id="c5a2f-202">Learn about [purchasing the Azure plan](purchase-azure-plan.md)</span></span>

- <span data-ttu-id="c5a2f-203">Veja a [lista de preços para a nova experiência de comércio no CSP](azure-plan-price-list.md)</span><span class="sxs-lookup"><span data-stu-id="c5a2f-203">See the [price list for the new commerce experience in CSP](azure-plan-price-list.md)</span></span>
