---
title: Análises do Partner Center – relatórios de CloudAscent propensation
description: Saiba mais sobre os relatórios de CloudAscent propensation no Partner Center. Inclui informações sobre as propensações de um cliente para comprar produtos da Microsoft.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 09/18/2020
ms.openlocfilehash: fd017884c29df3874a06e8c4213c6fe5f05a8995
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/19/2020
ms.locfileid: "92175280"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a><span data-ttu-id="3b77c-104">Relatórios de CloudAscent propensation disponíveis no painel do Partner Center</span><span class="sxs-lookup"><span data-stu-id="3b77c-104">CloudAscent Propensity reports available from Partner Center dashboard</span></span>

<span data-ttu-id="3b77c-105">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="3b77c-105">**Appropriate roles**</span></span>
- <span data-ttu-id="3b77c-106">Visualizador de relatórios executivos</span><span class="sxs-lookup"><span data-stu-id="3b77c-106">Executive report viewer</span></span>
- <span data-ttu-id="3b77c-107">Visualizador de relatórios</span><span class="sxs-lookup"><span data-stu-id="3b77c-107">Report viewer</span></span>

<span data-ttu-id="3b77c-108">O painel do Partner Center fornece dados de propensação baixáveis do programa CloudAscent.</span><span class="sxs-lookup"><span data-stu-id="3b77c-108">The Partner Center Dashboard provides downloadable propensity data from the CloudAscent Program.</span></span> <span data-ttu-id="3b77c-109">Os dados mostram a propensão dos clientes para comprar produtos da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="3b77c-109">The data shows the customers' propensity to purchase Microsoft products.</span></span>  <span data-ttu-id="3b77c-110">Este artigo descreve a divisão desses dados, como utilizar a pontuação e o que isso significa.</span><span class="sxs-lookup"><span data-stu-id="3b77c-110">This articles describes the breakdown of this data, how to utilize the scoring, and what it means.</span></span>

## <a name="summary-definitions"></a><span data-ttu-id="3b77c-111">Definições de resumo</span><span class="sxs-lookup"><span data-stu-id="3b77c-111">Summary definitions</span></span>

- <span data-ttu-id="3b77c-112">**Clientes do SMC**– este é o número total de clientes nos downloads de propensação.</span><span class="sxs-lookup"><span data-stu-id="3b77c-112">**SMC Customers**– This is the total number of customers in the propensity downloads.</span></span>  <span data-ttu-id="3b77c-113">Os clientes são identificados pelo parceiro do registro.</span><span class="sxs-lookup"><span data-stu-id="3b77c-113">Customers are identified by partner of record.</span></span>
- <span data-ttu-id="3b77c-114">**Contratos de expiração**– dentro do ano fiscal atual, estamos fornecendo o número de contratos expirando.</span><span class="sxs-lookup"><span data-stu-id="3b77c-114">**Expire Agreements**– within the current fiscal year, we're providing the number of expiring agreements.</span></span>
- <span data-ttu-id="3b77c-115">**Receita de expiração**– a receita associada aos contratos expirados.</span><span class="sxs-lookup"><span data-stu-id="3b77c-115">**Expiring Revenue**– the revenue associated to the expiring agreements.</span></span>
- <span data-ttu-id="3b77c-116">**Abrir receita de expiração**– a receita associada aos contratos expirados abertos.</span><span class="sxs-lookup"><span data-stu-id="3b77c-116">**Open Expiring Revenue**– The revenue associated to the open expiring agreements.</span></span>

:::image type="content" source="images/pci/cust-oppor-1.png" alt-text="Captura de tela do painel de Resumo de oportunidades de clientes.":::

## <a name="cloudascent-smb-segmentation"></a><span data-ttu-id="3b77c-118">Segmentação SMB do CloudAscent</span><span class="sxs-lookup"><span data-stu-id="3b77c-118">CloudAscent SMB segmentation</span></span>

<span data-ttu-id="3b77c-119">O segmento SMB (de pequeno a médio porte) é dividido em três subsegmentos distintos.</span><span class="sxs-lookup"><span data-stu-id="3b77c-119">The small to medium business (SMB) segment is further divided into three distinct sub segments.</span></span>

1. <span data-ttu-id="3b77c-120">A **parte superior não gerenciada** inclui os maiores clientes SMB com mais oportunidade para a Microsoft.</span><span class="sxs-lookup"><span data-stu-id="3b77c-120">**Top Unmanaged** includes the largest SMB customers with the most opportunity for Microsoft.</span></span> <span data-ttu-id="3b77c-121">Os principais clientes não gerenciados compartilham características semelhantes às contas gerenciadas, com grande número de funcionários, grandes orçamentos de ti e gastos e grandes quantidades de receitas potenciais para a Microsoft.</span><span class="sxs-lookup"><span data-stu-id="3b77c-121">Typical Top Unmanaged customers share similar characteristics as Managed accounts, with large number of employees, large IT budgets and spend, and large amounts of potential revenue for Microsoft.</span></span>

   <span data-ttu-id="3b77c-122">Definimos duas maneiras principais não gerenciadas:</span><span class="sxs-lookup"><span data-stu-id="3b77c-122">We define Top Unmanaged two ways:</span></span>

   - <span data-ttu-id="3b77c-123">**Com base em principais usuários não gerenciados**– inclui contas com 300 ou mais funcionários.</span><span class="sxs-lookup"><span data-stu-id="3b77c-123">**Top Unmanaged User Based**– includes accounts with 300 or more employees.</span></span> <span data-ttu-id="3b77c-124">User-Based contas são ótimos alvos para compra pela primeira vez ou expansão de produtos de assinatura baseados em usuário, como M365, D365 ou Surface.</span><span class="sxs-lookup"><span data-stu-id="3b77c-124">User-Based accounts are great targets for first-time purchase, or expansion of user-based subscription products such as M365, D365, or Surface.</span></span>
   - <span data-ttu-id="3b77c-125">**Base de computação não gerenciada superior** – inclui contas com o potencial do Azure maior que $10K.</span><span class="sxs-lookup"><span data-stu-id="3b77c-125">**Top Unmanaged Compute Based** – includes accounts with Azure potential greater than $10k.</span></span> <span data-ttu-id="3b77c-126">As contas baseadas em computação incluem o Azure existente.</span><span class="sxs-lookup"><span data-stu-id="3b77c-126">Compute based accounts include existing Azure.</span></span> <span data-ttu-id="3b77c-127">Acesse as contas com potencial do ano futuro e contas que ainda não compraram o Azure, mas têm potencial para o Azure com mais de US $10.000.</span><span class="sxs-lookup"><span data-stu-id="3b77c-127">accounts with significant future year potential and accounts who have yet to purchase Azure yet but have potential for Azure greater than $10k.</span></span>

2. <span data-ttu-id="3b77c-128">Os **negócios médios** incluem clientes existentes e contas de clientes potenciais com 25 a 300 funcionários.</span><span class="sxs-lookup"><span data-stu-id="3b77c-128">**Medium Business** includes existing customers and prospect accounts with 25 to 300 employees.</span></span>

3. <span data-ttu-id="3b77c-129">A **pequena empresa** inclui todas as empresas restantes com menos de 25 funcionários.</span><span class="sxs-lookup"><span data-stu-id="3b77c-129">**Small Business** includes all remaining businesses with fewer than 25 employees.</span></span>

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="Captura de tela do painel de Resumo de oportunidades de clientes.":::

<span data-ttu-id="3b77c-131">Os principais subsegmentos de negócios **não gerenciados** e **médios** representam clientes LTV (valor de tempo de vida alta) para a Microsoft e parceiros da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="3b77c-131">**Top Unmanaged** and **Medium Business** subsegments represent high life-time value (LTV) customers for Microsoft, and Microsoft Partners.</span></span> <span data-ttu-id="3b77c-132">Portanto, elas são as áreas potenciais de foco para impulsionar o crescimento nesse segmento.</span><span class="sxs-lookup"><span data-stu-id="3b77c-132">Hence they are the lead areas of focus for driving growth in this segment.</span></span> <span data-ttu-id="3b77c-133">Nesses dois subsegmentos, estamos mais bem posicionados para adquirir o soquete com M365, monetizar ainda mais com os aplicativos de LOB (linha de negócios) D365/Azure e percebem um LTV alto para a Microsoft.</span><span class="sxs-lookup"><span data-stu-id="3b77c-133">In these two subsegments, we are better positioned to acquire the socket with M365, monetize further with D365/Azure line of business (LOB) apps, and realize a high LTV for Microsoft.</span></span>

<span data-ttu-id="3b77c-134">Hoje temos duas áreas-chave de oportunidade – 1.</span><span class="sxs-lookup"><span data-stu-id="3b77c-134">Today we have two key areas of opportunity – 1.</span></span> <span data-ttu-id="3b77c-135">nosso cliente adiciona crescimento; 2.</span><span class="sxs-lookup"><span data-stu-id="3b77c-135">our customer adds growth; 2.</span></span> <span data-ttu-id="3b77c-136">Embora tenhamos adquirido bem os soquetes de nuvem que levam com o M365, temos uma grande oportunidade no D365 e no Azure.</span><span class="sxs-lookup"><span data-stu-id="3b77c-136">while we do well acquiring cloud sockets leading with M365, we have a large opportunity in D365 and Azure.</span></span>

<span data-ttu-id="3b77c-137">A captura de tela a seguir representa os três subsegmentos SMB e as rotas otimizadas para o mercado.</span><span class="sxs-lookup"><span data-stu-id="3b77c-137">The following screenshot represents the three SMB Subsegments and optimized routes to market.</span></span> <span data-ttu-id="3b77c-138">CloudAscent priorize a criação de perfil, a pontuação e a modelagem de todas as principais contas de negócios não gerenciadas e médias.</span><span class="sxs-lookup"><span data-stu-id="3b77c-138">CloudAscent prioritize the profiling, scoring, and modeling of all Top Unmanaged and Medium Business accounts.</span></span>

:::image type="content" source="images/pci/cust-oppor-3.png" alt-text="Captura de tela do painel de Resumo de oportunidades de clientes.":::

## <a name="cloudascent-machine-learning"></a><span data-ttu-id="3b77c-140">Machine Learning CloudAscent</span><span class="sxs-lookup"><span data-stu-id="3b77c-140">CloudAscent Machine Learning</span></span>

<span data-ttu-id="3b77c-141">O SMB usa a tecnologia de aprendizado de máquina para orientar as previsões de vendas e marketing dos clientes dentro dos principais segmentos de negócios não gerenciados e médios.</span><span class="sxs-lookup"><span data-stu-id="3b77c-141">SMB uses machine learning technology to drive sales and marketing customer predictions within the Top Unmanaged and Medium Business segments.</span></span> <span data-ttu-id="3b77c-142">Como os sinais são coletados e transformados nas recomendações de propensação?</span><span class="sxs-lookup"><span data-stu-id="3b77c-142">How are signals collected and turned into propensity recommendations?</span></span>

- <span data-ttu-id="3b77c-143">**Coleta de dados**: os rastreadores da Web examinam e coletam bilhões de sinais de clientes ao executar ping nos domínios da empresa e monitoramento: Postagens de blog, Press Releases, fluxos sociais e fóruns técnicos.</span><span class="sxs-lookup"><span data-stu-id="3b77c-143">**Data Collection**: Web crawlers scan and collect billions of customer signals by pinging the company domains, and monitoring: blog posts, press releases, social streams, and technical forums.</span></span>  <span data-ttu-id="3b77c-144">Além dos sinais coletados, as informações de firmographics são coletadas de fontes internas e externas, como D&B, assinatura interna da Microsoft e dados transacionais.</span><span class="sxs-lookup"><span data-stu-id="3b77c-144">In addition to the collected signals, firmographics information is collected from both internal and external sources such as D&B, Microsoft Internal subscription and transactional data.</span></span>

- <span data-ttu-id="3b77c-145">**Machine Learning**: os sinais são inseridos no modelo de aprendizado de máquina que gera um conjunto de dados estruturado de previsões de vendas e marketing para cada cliente por produto e cluster de nuvem.</span><span class="sxs-lookup"><span data-stu-id="3b77c-145">**Machine Learning**: The signals are fed into the machine learning model that outputs a structured data set of Sales and Marketing predictions for each customer by cloud product and cluster.</span></span>  <span data-ttu-id="3b77c-146">Cada cliente é pontuado usando um modelo semelhante ao principal SMB da Microsoft que determina o ajuste do cliente e os algoritmos de aprendizado de máquina que integram o comportamento online do cliente, defina como intenção.</span><span class="sxs-lookup"><span data-stu-id="3b77c-146">Each customer is scored using a look alike model to Microsoft's top SMB that determines the customer's Fit, and machine learning algorithms that integrate the customer's online behavior define as Intent.</span></span> <span data-ttu-id="3b77c-147">A pontuação é mesclada em clusters que mostram a propensão de um cliente para comprar Microsoft Cloud produtos.</span><span class="sxs-lookup"><span data-stu-id="3b77c-147">The scoring is merged into clusters that show a customer's propensity to purchase Microsoft Cloud Products.</span></span>

- <span data-ttu-id="3b77c-148">**Otimização**: o sistema de Machine Learning otimiza os modelos consumindo os dados de transação mensalmente e os dados de assinatura trimestral.</span><span class="sxs-lookup"><span data-stu-id="3b77c-148">**Optimization**: The Machine Learning system optimizes the models by consuming the transaction data monthly and the subscription data quarterly.</span></span>  <span data-ttu-id="3b77c-149">Usando os dados de ganho/perda, o Machine Learning ajusta os algoritmos e valida que os modelos estão funcionando conforme o esperado, comparando as recomendações de cluster às oportunidades trabalhadas no MSX.</span><span class="sxs-lookup"><span data-stu-id="3b77c-149">Using the win/loss data, the Machine Learning adjusts the algorithms and validates that the models are working as expected by comparing cluster recommendations to opportunities acted upon in MSX.</span></span>

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="Captura de tela do painel de Resumo de oportunidades de clientes.":::

## <a name="cloudascent-propensity"></a><span data-ttu-id="3b77c-151">CloudAscent propensaity</span><span class="sxs-lookup"><span data-stu-id="3b77c-151">CloudAscent Propensity</span></span>

<span data-ttu-id="3b77c-152">Como as recomendações de propensação são criadas?</span><span class="sxs-lookup"><span data-stu-id="3b77c-152">How are propensity recommendations created?</span></span>

<span data-ttu-id="3b77c-153">Usando sinais coletados por meio de rastreadores da Web e dados fornecidos de várias fontes, consolidamos os dados de firmographics e os sinais de mídia social do cliente.</span><span class="sxs-lookup"><span data-stu-id="3b77c-153">Using signals collected via web crawlers and data provided from various sources, we consolidate the firmographics data and customer's social media signals.</span></span>  <span data-ttu-id="3b77c-154">A pontuação usa esses sinais e dados em modelos de comparação para os modelos de ajuste e pontuação para a intenção.</span><span class="sxs-lookup"><span data-stu-id="3b77c-154">The scoring uses these signals and data in comparison models for fit and scoring models for Intent.</span></span>

1. <span data-ttu-id="3b77c-155">Ajuste de conta do cliente</span><span class="sxs-lookup"><span data-stu-id="3b77c-155">Customer Account Fit</span></span>

   - <span data-ttu-id="3b77c-156">Pontos de dados internos e externos que definem firmographics.</span><span class="sxs-lookup"><span data-stu-id="3b77c-156">Internal and External data points that define firmographics.</span></span>

   - <span data-ttu-id="3b77c-157">Ajustar a pontuação usa um modelo semelhante ao nosso melhor SMB para comparar os clientes e ver se eles são um ajuste potencial para Microsoft Cloud produtos.</span><span class="sxs-lookup"><span data-stu-id="3b77c-157">Fit scoring uses a look alike model to our best SMB to compare customers and see if they're a potential  fit for Microsoft Cloud Products.</span></span>

   - <span data-ttu-id="3b77c-158">Ajustar Pontuação é atualizado trimestral</span><span class="sxs-lookup"><span data-stu-id="3b77c-158">Fit scoring is updated quarterly</span></span>

2. <span data-ttu-id="3b77c-159">Intenção de conta de cliente</span><span class="sxs-lookup"><span data-stu-id="3b77c-159">Customer Account Intent</span></span>

   - <span data-ttu-id="3b77c-160">Os sinais relacionados à mídia social e ao comportamento online de um cliente definem a intenção.</span><span class="sxs-lookup"><span data-stu-id="3b77c-160">Signals related to Social media and a customer's online behavior define Intent.</span></span>

   - <span data-ttu-id="3b77c-161">A pontuação da intenção é sobreposta sobre ajustar para definir os clusters.</span><span class="sxs-lookup"><span data-stu-id="3b77c-161">Intent scoring is overlaid on top of fit to define the clusters.</span></span>

   - <span data-ttu-id="3b77c-162">A pontuação da intenção é atualizada mensalmente.</span><span class="sxs-lookup"><span data-stu-id="3b77c-162">Intent scoring is updated monthly.</span></span>

   :::image type="content" source="images/pci/cust-oppor-5.png" alt-text="Captura de tela do painel de Resumo de oportunidades de clientes.":::

3. <span data-ttu-id="3b77c-164">Clustering</span><span class="sxs-lookup"><span data-stu-id="3b77c-164">Clustering</span></span>

   <span data-ttu-id="3b77c-165">Os sinais para ajuste e intenção são consolidados em uma pontuação de clustering.</span><span class="sxs-lookup"><span data-stu-id="3b77c-165">The Signals for fit and intent are consolidated into a clustering score.</span></span> <span data-ttu-id="3b77c-166">O CloudAscent tem quatro clusters:</span><span class="sxs-lookup"><span data-stu-id="3b77c-166">CloudAscent has four clusters:</span></span>

      - <span data-ttu-id="3b77c-167">Clientes do Act Now-Sales Ready</span><span class="sxs-lookup"><span data-stu-id="3b77c-167">Act Now - sales ready customers</span></span>
      - <span data-ttu-id="3b77c-168">Avaliar-clientes prontos para marketing</span><span class="sxs-lookup"><span data-stu-id="3b77c-168">Evaluate - marketing ready customers</span></span>
      - <span data-ttu-id="3b77c-169">Campanhas de reconhecimento de incentivá</span><span class="sxs-lookup"><span data-stu-id="3b77c-169">Nurture - drive awareness campaigns</span></span>
      - <span data-ttu-id="3b77c-170">Instrua-instrua e monitore para a intenção</span><span class="sxs-lookup"><span data-stu-id="3b77c-170">Educate - educate and monitor for intent</span></span>

   <span data-ttu-id="3b77c-171">O clustering permite que os usuários direcionem clientes específicos para iniciativas de vendas e marketing com base em fatores de segmento, por exemplo: produto, geográfico, setor e vertical.</span><span class="sxs-lookup"><span data-stu-id="3b77c-171">The clustering allows users to target specific customers for sales and marketing initiatives based on segment factors, for example: product, geo, industry and vertical.</span></span>

   <span data-ttu-id="3b77c-172">A guia **modelo** de propensão nas pastas de trabalho CloudAscent compartilha a propensão e a receita de espaço em branco estimada.</span><span class="sxs-lookup"><span data-stu-id="3b77c-172">The **Propensity model** tab in the CloudAscent Workbooks shares the propensity and the estimated whitespace revenue.</span></span> <span data-ttu-id="3b77c-173">Para definir o clustering de ajuste e intenção, percorreremos as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="3b77c-173">To define the clustering of Fit and Intent, we go through the following steps:</span></span>

      1. <span data-ttu-id="3b77c-174">Usando modelos de ML, primeiro calculamos a pontuação de ajuste do cliente e a pontuação de intenção em uma escala de 100.</span><span class="sxs-lookup"><span data-stu-id="3b77c-174">Using ML Models, we first calculate Customer Fit Score and intent Score on a scale of 100.</span></span>  <span data-ttu-id="3b77c-175">As pontuações exatas variarão com base nos modelos de ML.</span><span class="sxs-lookup"><span data-stu-id="3b77c-175">Exact Scores will vary based on ML Models.</span></span>  <span data-ttu-id="3b77c-176">Pontuação de exemplo abaixo:</span><span class="sxs-lookup"><span data-stu-id="3b77c-176">Example Scores Below:</span></span>

         |<span data-ttu-id="3b77c-177">**Classificação**</span><span class="sxs-lookup"><span data-stu-id="3b77c-177">**Classification**</span></span>|<span data-ttu-id="3b77c-178">**Pontuação**</span><span class="sxs-lookup"><span data-stu-id="3b77c-178">**Score**</span></span>|
         |---------|:---------|
         |<span data-ttu-id="3b77c-179">Alto</span><span class="sxs-lookup"><span data-stu-id="3b77c-179">High</span></span>|<span data-ttu-id="3b77c-180">75-100</span><span class="sxs-lookup"><span data-stu-id="3b77c-180">75 - 100</span></span>|
         |<span data-ttu-id="3b77c-181">Médio</span><span class="sxs-lookup"><span data-stu-id="3b77c-181">Medium</span></span>|<span data-ttu-id="3b77c-182">55-74</span><span class="sxs-lookup"><span data-stu-id="3b77c-182">55 - 74</span></span>|
         |<span data-ttu-id="3b77c-183">Baixo</span><span class="sxs-lookup"><span data-stu-id="3b77c-183">Low</span></span>|<span data-ttu-id="3b77c-184">30 - 54</span><span class="sxs-lookup"><span data-stu-id="3b77c-184">30 - 54</span></span>|
         |<span data-ttu-id="3b77c-185">Muito baixo</span><span class="sxs-lookup"><span data-stu-id="3b77c-185">Very Low</span></span>|<span data-ttu-id="3b77c-186">0 - 29</span><span class="sxs-lookup"><span data-stu-id="3b77c-186">0 - 29</span></span>|

      2. <span data-ttu-id="3b77c-187">Usando a regra acima, classificamos as empresas para serem altas, médias, baixas e muito baixas entre os sinais de ajuste do cliente e de intenção.</span><span class="sxs-lookup"><span data-stu-id="3b77c-187">Using the rule above, we classify companies to be High, Medium, Low, and Very Low across both Customer Fit    and Intent Signals.</span></span>

      3. <span data-ttu-id="3b77c-188">Nós plotamos os sinais de ajuste do cliente e de intenção em uma matriz 2D com cada interseção que representa a propensação.</span><span class="sxs-lookup"><span data-stu-id="3b77c-188">We plot customer fit and intent signals on a 2D matrix with each intersection representing the propensity.</span></span>     <span data-ttu-id="3b77c-189">Por exemplo, alto ajuste + alta tentativa = a1, representando a mais alta propensação.</span><span class="sxs-lookup"><span data-stu-id="3b77c-189">For Example, High Fit + High Intent = A1, representing the highest propensity.</span></span>

      4. <span data-ttu-id="3b77c-190">Por fim, esses segmentos agrupam-se para formar clusters.</span><span class="sxs-lookup"><span data-stu-id="3b77c-190">Finally, these segments group to form clusters.</span></span>  <span data-ttu-id="3b77c-191">Por exemplo, a1, a2, a3, A4 forma o cluster Act Now.</span><span class="sxs-lookup"><span data-stu-id="3b77c-191">For Example, A1, A2, A3, A4 form the Act Now cluster.</span></span>

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="Captura de tela do painel de Resumo de oportunidades de clientes.":::

   <span data-ttu-id="3b77c-193">Para esses clientes, é recomendável direcionar o Act agora e avaliar os clientes.</span><span class="sxs-lookup"><span data-stu-id="3b77c-193">For these customers, we recommend targeting Act Now and Evaluate customers.</span></span>

## <a name="cloudascent-products--models"></a><span data-ttu-id="3b77c-194">CloudAscent produtos & modelos</span><span class="sxs-lookup"><span data-stu-id="3b77c-194">CloudAscent Products & Models</span></span>

<span data-ttu-id="3b77c-195">O gráfico a seguir fornece uma exibição de cada modelo de propensação dentro de CloudAscent:</span><span class="sxs-lookup"><span data-stu-id="3b77c-195">The following graphic provides a view of each propensity model within CloudAscent:</span></span>

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="Captura de tela do painel de Resumo de oportunidades de clientes.":::

<span data-ttu-id="3b77c-197">Os modelos de espaço em branco são compostos de previsões para clientes da Microsoft existentes onde não têm um produto e/ou são clientes novos de cliente potencial.</span><span class="sxs-lookup"><span data-stu-id="3b77c-197">Whitespace models are composed of predictions for existing Microsoft customers where they don't have a product and/or are net new prospect customers.</span></span>

<span data-ttu-id="3b77c-198">Os modelos de venda cruzada usam dados de transação para prever o potencial de venda no Azure e em SKUs M365.</span><span class="sxs-lookup"><span data-stu-id="3b77c-198">Upsell models use transaction data to predict the potential for upsell in Azure and M365 SKUs.</span></span>

<span data-ttu-id="3b77c-199">O EOS compartilha o fim dos clientes de serviço para o Win 7, o Office 2010, o SQL Server e o Windows Server.</span><span class="sxs-lookup"><span data-stu-id="3b77c-199">EOS shares the end of service customers for Win 7, Office 2010, SQL Server, and Windows Server.</span></span> <span data-ttu-id="3b77c-200">Os dados de EOS são extraídos da MS Sales e sobrepostos com a modelagem de propensão CloudAscent, quando disponível.</span><span class="sxs-lookup"><span data-stu-id="3b77c-200">The EOS data is pulled from MS Sales and overlaid with the CloudAscent propensity modeling where available.</span></span> <span data-ttu-id="3b77c-201">Os dados de EOS residem no trabalho moderno e nas atividades de vendas do Azure.</span><span class="sxs-lookup"><span data-stu-id="3b77c-201">EOS data lives in the Modern Work and Azure Sales plays.</span></span>
