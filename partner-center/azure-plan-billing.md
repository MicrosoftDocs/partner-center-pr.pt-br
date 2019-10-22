---
title: Plano do Azure – Cobrança | Partner Center
ms.topic: article
ms.date: 10/04/2019
description: Descreve a estrutura de arquivos de faturamento e reconhecimento
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: High
ms.openlocfilehash: 28e670635ca7fcff60041fcb5c93b3ddd5e4069d
ms.sourcegitcommit: cd90a59ff0ea81197b603abcb7bf462c4fb1edbe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2019
ms.locfileid: "72171297"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a><span data-ttu-id="15daf-103">Nova experiência de comércio no CSP – Cobrança do Azure</span><span class="sxs-lookup"><span data-stu-id="15daf-103">New commerce experience in CSP - Azure billing</span></span> 

<span data-ttu-id="15daf-104">A cobrança no âmbito do plano do Azure é uma experiência de cobrança simplificada usando uma data de cobrança única alinhada e um período de cobrança baseado no mês civil.</span><span class="sxs-lookup"><span data-stu-id="15daf-104">Billing under the Azure plan is a simplified billing experience by using an aligned single billing date and calendar month-based billing period.</span></span> <span data-ttu-id="15daf-105">Para obter informações sobre a plataforma de cobrança, leia [Guia operacional de comércio moderno do Partner Center](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx).</span><span class="sxs-lookup"><span data-stu-id="15daf-105">For information on the billing platform, read  [Partner Center Modern Commerce Operating Guide](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx).</span></span>

## <a name="summary-of-billing-essentials"></a><span data-ttu-id="15daf-106">Resumo dos conceitos básicos de cobrança</span><span class="sxs-lookup"><span data-stu-id="15daf-106">Summary of billing essentials</span></span>

- <span data-ttu-id="15daf-107">**Data da fatura**: A fatura e o arquivo de reconciliação estarão disponíveis na API/no Painel do Partner Center até o dia oito (à meia-noite, UTC).</span><span class="sxs-lookup"><span data-stu-id="15daf-107">**Invoice date**: Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).</span></span>

- <span data-ttu-id="15daf-108">**Período de cobrança da fatura**: O período de cobrança da fatura é alinhado ao mês civil, por exemplo, 1/10 – 31/10, 1/11 – 30/11.</span><span class="sxs-lookup"><span data-stu-id="15daf-108">**Invoice billing period**: The invoice billing period is aligned to the calendar month, for example,  10/1-10/31, 11/1-11/30.</span></span>

- <span data-ttu-id="15daf-109">**Períodos de serviço de cobrança**: As cobranças serão alinhadas ao mês civil.</span><span class="sxs-lookup"><span data-stu-id="15daf-109">**Charge service periods**: Charges will align to the calendar month.</span></span> <span data-ttu-id="15daf-110">Por exemplo, se o parceiro cobrado adicionar serviços do Azure por meio de um plano do Azure em 15/10 e o cliente iniciar o consumo de serviços do Azure em 10/15, então o parceiro cobrado receberá a fatura/o reconhecimento em 8/11 para o consumo do cliente referente ao período de serviço 15/10 – 31/10.</span><span class="sxs-lookup"><span data-stu-id="15daf-110">For example, if billed partner adds Azure services through an Azure plan on 10/15 and the customer begins consumption of Azure services on 10/15, then billed partner will receive invoice/recon on 11/8 for customer consumption for the service period 10/15 - 10/31.</span></span> <span data-ttu-id="15daf-111">A fatura do próximo mês, que será gerada em 8/12, conterá todos os encargos referentes ao período de serviço de 1/11 – 31/11.</span><span class="sxs-lookup"><span data-stu-id="15daf-111">The next month’s invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.</span></span>

- <span data-ttu-id="15daf-112">**Condição de pagamento da fatura**: Líquido de 60 dias.</span><span class="sxs-lookup"><span data-stu-id="15daf-112">**Invoice payment term**: Net 60 days.</span></span>

- <span data-ttu-id="15daf-113">**Moeda da fatura**: Os parceiros continuarão sendo cobrados na moeda atribuída ao país do cliente.</span><span class="sxs-lookup"><span data-stu-id="15daf-113">**Invoice currency**: Partners will continue to be billed in the customer's country's assigned currency.</span></span> <span data-ttu-id="15daf-114">Por exemplo, se o parceiro cobrado estiver na Irlanda com clientes no Reino Unido, na Noruega e na Alemanha, ele receberá faturas/reconhecimentos em GBP, NOK e EUR.</span><span class="sxs-lookup"><span data-stu-id="15daf-114">For example, if the billed partner is in Ireland with customers in the UK, Norway, and Germany, then the billed partner will receive a GBP, NOK, and EUR invoice/recon.</span></span>

- <span data-ttu-id="15daf-115">**Incentivos para Parceiros**: pago 45 dias após o final do mês da fatura.</span><span class="sxs-lookup"><span data-stu-id="15daf-115">**Partner incentives**: Paid 45 days from the end of the invoice month.</span></span>

##  <a name="access-your-invoices-and-recon-files"></a><span data-ttu-id="15daf-116">Acessar seus arquivos de fatura e reconhecimento</span><span class="sxs-lookup"><span data-stu-id="15daf-116">Access your invoices and recon files</span></span>

<span data-ttu-id="15daf-117">O administrador global ou de cobrança da sua empresa receberá um email quando a fatura estiver pronta para ser exibida.</span><span class="sxs-lookup"><span data-stu-id="15daf-117">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span> 

<span data-ttu-id="15daf-118">**Para acessar o arquivo de fatura e reconhecimento**</span><span class="sxs-lookup"><span data-stu-id="15daf-118">**To access the invoice and recon file**</span></span>

1. <span data-ttu-id="15daf-119">Entre no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="15daf-119">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="15daf-120">No menu do Partner Center, selecione **Cobrança**.</span><span class="sxs-lookup"><span data-stu-id="15daf-120">From the Partner Center menu, select **Billing**.</span></span>

3. <span data-ttu-id="15daf-121">Selecione a guia para **baseado em calendário** e moeda em que você está interessado.</span><span class="sxs-lookup"><span data-stu-id="15daf-121">Select the tab for the **Calendar-based** and currency you are interested in.</span></span>

![cobrança](images/azure/billing1.png)

4. <span data-ttu-id="15daf-123">Selecione **arquivo de Fatura e Reconhecimento**.</span><span class="sxs-lookup"><span data-stu-id="15daf-123">Select **Invoice and Recon file**.</span></span>  

<span data-ttu-id="15daf-124">Para exibir os arquivos históricos de faturas e reconhecimento, expanda a linha do histórico de cobrança, abaixo.</span><span class="sxs-lookup"><span data-stu-id="15daf-124">To view historical invoices and recon files expand the Billing history row below.</span></span>

## <a name="read-the-invoice"></a><span data-ttu-id="15daf-125">Leia a fatura</span><span class="sxs-lookup"><span data-stu-id="15daf-125">Read the invoice</span></span>

1. <span data-ttu-id="15daf-126">A fatura estará disponível até o dia oito de cada mês.</span><span class="sxs-lookup"><span data-stu-id="15daf-126">Invoice will be available no later than the 8th of each month.</span></span>

2. <span data-ttu-id="15daf-127">Os parceiros têm 60 dias para remeterem o pagamento.</span><span class="sxs-lookup"><span data-stu-id="15daf-127">Partners have 60 days to remit payment.</span></span>

3. <span data-ttu-id="15daf-128">O período de cobrança abrangerá um determinado mês civil, por exemplo, de 1/10 – 31/10.</span><span class="sxs-lookup"><span data-stu-id="15daf-128">The billing period will cover a given calendar month, for example, 10/1-10/31.</span></span>

4. <span data-ttu-id="15daf-129">As cobranças são líquidas de ajustes (o valor é líquido de "Créditos ganhos pelo parceiro para serviços gerenciados").</span><span class="sxs-lookup"><span data-stu-id="15daf-129">Charges are net of adjustments (amount is net of “Partner earned credit for services managed”).</span></span>

5. <span data-ttu-id="15daf-130">Examine o arquivo de reconhecimento de fatura e o arquivo de uso de classificação diária para obter detalhes adicionais de cobrança.</span><span class="sxs-lookup"><span data-stu-id="15daf-130">Review the invoice recon file and daily rated usage file for additional billing details.</span></span>

![fatura](images/azure/invoice1.png)

## <a name="read-the-recon-file"></a><span data-ttu-id="15daf-132">Ler o arquivo de reconhecimento</span><span class="sxs-lookup"><span data-stu-id="15daf-132">Read the recon file</span></span>

1. <span data-ttu-id="15daf-133">Cada medidor da assinatura do Azure pode ter até duas linhas de cobrança no arquivo reconhecimento.</span><span class="sxs-lookup"><span data-stu-id="15daf-133">Each Azure subscription meter may have up to two billing lines on the recon file.</span></span>

2. <span data-ttu-id="15daf-134">Se o medidor for qualificado para qualquer tipo de desconto ou crédito (como descontos de nível 1 ou créditos ganhos pelo parceiro para serviços gerenciados) durante todo o mês civil, então o arquivo de reconhecimento conterá apenas uma linha de cobrança.</span><span class="sxs-lookup"><span data-stu-id="15daf-134">If the meter qualified for any type of discount or credit (such as tier 1 discounts or the Partner earned credit for managed services) throughout the entire calendar month, then the recon file will only contain one billing line.</span></span> <span data-ttu-id="15daf-135">A coluna **PriceAdjusmentDescription** fará referência ao desconto ou ao crédito ganho; o preço unitário efetivo será o preço de varejo menos o crédito ganho pelo parceiro ou outros descontos eventualmente aplicados.</span><span class="sxs-lookup"><span data-stu-id="15daf-135">The column **PriceAdjusmentDescription** will reference the discount or earned credit; the effective unit price will be the retail price minus partner earned credit or any other discounts.</span></span>

3. <span data-ttu-id="15daf-136">Se o medidor não se qualificou para os créditos ganhos pelo parceiro para serviços gerenciados durante todo o mês civil, então o arquivo de reconhecimento conterá apenas uma linha de cobrança e o preço unitário efetivo será o preço de varejo (que é o preço unitário).</span><span class="sxs-lookup"><span data-stu-id="15daf-136">If the meter didn’t qualify for the Partner earned credit for managed services throughout the entire calendar month, then the recon file will only contain one billing line and the effective unit price will be the retail price (which is the unit price).</span></span>

4. <span data-ttu-id="15daf-137">Se o medidor se qualificou para **Créditos ganhos pelo parceiro para serviços gerenciados** em uma parte do mês, então o arquivo de reconhecimento conterá duas linhas de cobrança.</span><span class="sxs-lookup"><span data-stu-id="15daf-137">If the meter qualified for **Partner earned credit for services managed** for a part of the month, the recon file will contain two billing lines.</span></span> <span data-ttu-id="15daf-138">Uma linha representará os dias em que o medidor se qualificou, ao passo que a outra linha representará os dias em que o medidor não se qualificou.</span><span class="sxs-lookup"><span data-stu-id="15daf-138">One line will represent the days the meter qualified and the second line will represent the days the meter did not qualify.</span></span> 

## <a name="read-the-daily-usage-file"></a><span data-ttu-id="15daf-139">Ler o arquivo de uso diário</span><span class="sxs-lookup"><span data-stu-id="15daf-139">Read the daily usage file</span></span>

- <span data-ttu-id="15daf-140">Os medidores de assinatura no âmbito de um plano do Azure são classificados e acumulados diariamente.</span><span class="sxs-lookup"><span data-stu-id="15daf-140">Subscription meters under an Azure plan are rated, and are cumulated, on a daily basis.</span></span> 

- <span data-ttu-id="15daf-141">**O crédito ganho pelo parceiro para serviços gerenciados** é determinado e aplicado diariamente.</span><span class="sxs-lookup"><span data-stu-id="15daf-141">**Partner earned credit for services managed** is determined and applied on a daily basis.</span></span>

- <span data-ttu-id="15daf-142">Cada medidor de assinatura terá uma linha para cada dia do mês em que houve consumo.</span><span class="sxs-lookup"><span data-stu-id="15daf-142">Every subscription meter will have a row for every day of the month where there was consumption.</span></span>

- <span data-ttu-id="15daf-143">No exemplo a seguir:</span><span class="sxs-lookup"><span data-stu-id="15daf-143">In the example below:</span></span>

  - <span data-ttu-id="15daf-144">O medidor se qualificou para **Crédito ganho pelo parceiro para serviços gerenciados** de 01/07 – 03/07 (observe que o preço unitário efetivo é o preço de varejo menos os créditos ganhos pelo parceiro).</span><span class="sxs-lookup"><span data-stu-id="15daf-144">Meter qualified for **Partner earned credit for services managed** from 7/1 – 7/3 (note the effective unit price is retail price less partner earned credit.</span></span>

   - <span data-ttu-id="15daf-145">O medidor não se qualificou para **Crédito ganho pelo parceiro para serviços gerenciados** de 04/07 – 07/07 (observe que o preço unitário efetivo é o preço de varejo).</span><span class="sxs-lookup"><span data-stu-id="15daf-145">Meter didn’t qualify for **Partner earned credit for services managed** from 7/4 – 7/7 (note the effective unit price is retail price).</span></span>

    - <span data-ttu-id="15daf-146">O medidor se qualificou para **Crédito ganho pelo parceiro para serviços gerenciados** de 08/07 – 31/07 (observe que o preço unitário efetivo é o preço de varejo menos os créditos ganhos pelo parceiro).</span><span class="sxs-lookup"><span data-stu-id="15daf-146">Meter qualified for **Partner earned credit for services managed** from 7/8 – 7/31 (note the effective unit price is retail price less partner earned credit).</span></span>

![recon2](images/azure/billing2.png) 

## <a name="invoice-in-customer-currency"></a><span data-ttu-id="15daf-148">Fatura na moeda do cliente</span><span class="sxs-lookup"><span data-stu-id="15daf-148">Invoice in customer currency</span></span> 

<span data-ttu-id="15daf-149">Os serviços do Azure por meio de um plano do Azure serão precificados em USD e cobrados na moeda atribuída ao país do cliente.</span><span class="sxs-lookup"><span data-stu-id="15daf-149">Azure services through an Azure plan will be priced in USD and billed in the customer country assigned currency.</span></span> <span data-ttu-id="15daf-150">Se a moeda de cobrança não for USD, então a taxa de câmbio usada será mostrada na última página da fatura.</span><span class="sxs-lookup"><span data-stu-id="15daf-150">If the billing currency is non-USD, then the FX rate used will be shown on the last page of the invoice.</span></span> <span data-ttu-id="15daf-151">As taxas de câmbio são determinadas mensalmente e aplicadas à fatura a seguir.</span><span class="sxs-lookup"><span data-stu-id="15daf-151">FX rates are determined monthly and applied to the following invoice.</span></span> <span data-ttu-id="15daf-152">Para obter a lista completa das moedas dos países, consulte a [Matriz de moedas do cliente e disponibilidade por país de novas ofertas de comércio](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3Qn1V).</span><span class="sxs-lookup"><span data-stu-id="15daf-152">For a full list of country currencies, please view the [New commerce offers country availability and customer currency matrix](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3Qn1V).</span></span> 

<span data-ttu-id="15daf-153">A Microsoft usará o [Thompson Reuters](https://developers.thomsonreuters.com/content/wm-company) para estabelecer a taxa de câmbio usada para determinar a moeda de preço para a conversão de moeda da fatura.</span><span class="sxs-lookup"><span data-stu-id="15daf-153">Microsoft will use [Thompson Reuters](https://developers.thomsonreuters.com/content/wm-company) to determine the FX rate used to determine pricing currency to invoice currency conversion.</span></span> <span data-ttu-id="15daf-154">A taxa de câmbio será atualizada e disponibilizada no dia anterior ao primeiro dia de cada mês em que ela será aplicada.</span><span class="sxs-lookup"><span data-stu-id="15daf-154">The FX rate will be refreshed and available on the day before the first of the month for which they apply.</span></span>

<span data-ttu-id="15daf-155">**Exemplo**:  Os encargos de uso do período de serviço de 1º de agosto a 31 de agosto serão cobrados usando a taxa de câmbio publicada no dia 1º de agosto.</span><span class="sxs-lookup"><span data-stu-id="15daf-155">**Example**:  Usage charges for the service period August 1 – August 31 will be billed using the FX rate published on August 1.</span></span> <span data-ttu-id="15daf-156">Esses encargos serão exibidos na fatura de setembro e a taxa de câmbio poderá ser observada na última página da fatura.</span><span class="sxs-lookup"><span data-stu-id="15daf-156">These charges will appear on the September invoice and the FX rate will be noted on the last page of the invoice.</span></span> 

<span data-ttu-id="15daf-157">Os usuários do locatário do parceiro continuarão a ver informações relacionadas à função específica sobre todos os clientes e todos os pedidos, independentemente da moeda de cobrança.</span><span class="sxs-lookup"><span data-stu-id="15daf-157">Partner tenant users will continue to see role-specific related information regarding all customers and all orders, regardless of the billing currency.</span></span> <span data-ttu-id="15daf-158">Além disso, o usuário poderá ver todas as faturas em todas as moedas.</span><span class="sxs-lookup"><span data-stu-id="15daf-158">Additionally, the user will be able to see all the invoices in all currencies.</span></span>  
 
## <a name="azure-reservations"></a><span data-ttu-id="15daf-159">Reservas do Azure</span><span class="sxs-lookup"><span data-stu-id="15daf-159">Azure reservations</span></span> 

<span data-ttu-id="15daf-160">Ao comprar [Reservas do Azure](https://docs.microsoft.com/partner-center/azure-reservations) por meio de um plano do Azure, inicialmente, só será possível escolher a cobrança única no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="15daf-160">If purchasing [Azure reservations](https://docs.microsoft.com/partner-center/azure-reservations) through an Azure plan, initially,  it will only be possible to choose one-time billing in Partner Center.</span></span> <span data-ttu-id="15daf-161">A cobrança mensal está disponível no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="15daf-161">Monthly billing is available on the Azure portal.</span></span> <span data-ttu-id="15daf-162">A cobrança mensal será disponibilizada no Partner Center em uma data posterior.</span><span class="sxs-lookup"><span data-stu-id="15daf-162">Monthly billing will be available in Partner Center at a later date.</span></span> 

## <a name="azure-cost-management"></a><span data-ttu-id="15daf-163">Gerenciamento de Custos do Azure</span><span class="sxs-lookup"><span data-stu-id="15daf-163">Azure cost management</span></span> 

<span data-ttu-id="15daf-164">As ferramentas de Gerenciamento de Custos do Azure ajudarão as organizações a visualizar, gerenciar e otimizar os custos em todo o Microsoft Azure.</span><span class="sxs-lookup"><span data-stu-id="15daf-164">Azure Cost Management tools will help organizations visualize, manage and optimize costs across Microsoft Azure.</span></span> <span data-ttu-id="15daf-165">Esse recurso estará disponível na portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="15daf-165">This feature will be available in the Azure portal.</span></span> <span data-ttu-id="15daf-166">Os parceiros terão uma solução sempre ativa e de baixa latência com os seguintes recursos disponíveis:</span><span class="sxs-lookup"><span data-stu-id="15daf-166">Partners will have an always-on, low-latency solution with the following features available:</span></span> 

- <span data-ttu-id="15daf-167">Análise e alertas de orçamento mais abundantes</span><span class="sxs-lookup"><span data-stu-id="15daf-167">Richer analysis and budget alerting</span></span> 
- <span data-ttu-id="15daf-168">APIs e conectores do Power BI</span><span class="sxs-lookup"><span data-stu-id="15daf-168">APIs and Power BI connectors</span></span> 
- <span data-ttu-id="15daf-169">Exibição de vários clientes</span><span class="sxs-lookup"><span data-stu-id="15daf-169">Multi-customer view</span></span> 
- <span data-ttu-id="15daf-170">Gratuito para gerenciar os custos do Azure</span><span class="sxs-lookup"><span data-stu-id="15daf-170">Free to manage Azure costs</span></span> 
- <span data-ttu-id="15daf-171">Expansão de funções/usuários</span><span class="sxs-lookup"><span data-stu-id="15daf-171">Expansion of roles/users</span></span> 

<span data-ttu-id="15daf-172">Consulte o [Gerenciamento de Custos do Azure](https://azure.microsoft.com/services/cost-management) para obter mais informações sobre esse recurso, que foi disponibilizado para contratos corporativos em fevereiro de 2019.</span><span class="sxs-lookup"><span data-stu-id="15daf-172">See [Azure cost management](https://azure.microsoft.com/services/cost-management) for more information on this feature, which became available for enterprise agreements in February, 2019.</span></span> <span data-ttu-id="15daf-173">Isso está disponível somente com os serviços do Azure adquiridos como parte dessa nova experiência se comércio do Azure no CSP.</span><span class="sxs-lookup"><span data-stu-id="15daf-173">This is available only with Azure services purchased as part of this new Azure commerce experience in CSP.</span></span> 
 
## <a name="azure-spending"></a><span data-ttu-id="15daf-174">Gastos do Azure</span><span class="sxs-lookup"><span data-stu-id="15daf-174">Azure spending</span></span> 

<span data-ttu-id="15daf-175">Uma ferramenta de gastos do Azure estará disponível no Partner Center para a nova experiência de comércio no CSP.</span><span class="sxs-lookup"><span data-stu-id="15daf-175">An Azure spending tool will be available in Partner Center for the new commerce experience in CSP.</span></span> <span data-ttu-id="15daf-176">Quando aplicada, essa funcionalidade permitirá que os parceiros enxerguem:</span><span class="sxs-lookup"><span data-stu-id="15daf-176">When applied, this capability will enable partners to see:</span></span>  

- <span data-ttu-id="15daf-177">O orçamento total de um cliente</span><span class="sxs-lookup"><span data-stu-id="15daf-177">Total budget on a customer</span></span> 
- <span data-ttu-id="15daf-178">O total de gastos estimados em um plano do Azure existente</span><span class="sxs-lookup"><span data-stu-id="15daf-178">Total estimated spending on an existing Azure plan</span></span> 
- <span data-ttu-id="15daf-179">O percentual de uso de clientes em cada período de cobrança</span><span class="sxs-lookup"><span data-stu-id="15daf-179">Percentage of customers usage in each billing period</span></span> 

<span data-ttu-id="15daf-180">Como o modelo de cobrança para os serviços do Azure por meio de um plano do Azure é o consumo pós-pago, para evitar uma cobrança maior do que o previsto, os parceiros podem aplicar um orçamento mensal e acompanhar o percentual de uso.</span><span class="sxs-lookup"><span data-stu-id="15daf-180">Because the billing model for Azure services through an Azure plan is post-pay consumption, to avoid a bigger bill than anticipated,partners can apply a monthly budget and track the percentage of usage.</span></span> <span data-ttu-id="15daf-181">Um orçamento pode ser aplicado a um cliente ou a vários clientes ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="15daf-181">A budget can be applied to one customer or multiple customers at one time.</span></span> 

![Gastos do Azure](images/azure/azurespend.png)

<span data-ttu-id="15daf-183">**Para saber mais**</span><span class="sxs-lookup"><span data-stu-id="15daf-183">**For more information**</span></span>

-  <span data-ttu-id="15daf-184">Como o PEC (crédito ganho pelo parceiro) é calculado está localizado na lista de preços disponível por meio do Painel do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="15daf-184">How the partner earned credit (PEC) is calculated is located on the price list available through your Partner Center dashboard.</span></span> 
   
-  [<span data-ttu-id="15daf-185">Comprar o plano do Azure</span><span class="sxs-lookup"><span data-stu-id="15daf-185">Purchase the Azure plan</span></span>](purchase-azure-plan.md)

-  [<span data-ttu-id="15daf-186">Lista de preços para a nova experiência de comércio no CSP</span><span class="sxs-lookup"><span data-stu-id="15daf-186">Price list for the new commerce experience in CSP </span></span>](azure-plan-price-list.md)
