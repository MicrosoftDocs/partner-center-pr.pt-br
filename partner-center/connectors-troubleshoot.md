---
title: Solucionar problemas de conectores de referências de venda conjunta
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba respostas para perguntas comuns sobre como usar conectores de venda em comum. Leia essas perguntas frequentes sobre como solucionar problemas de conectores de venda em cooperação.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: bb7a227624c548a29046b80d3bd5fa363a4aee2f
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276919"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a><span data-ttu-id="ccb41-104">Solucionar problemas de conectores de referências de venda conjunta</span><span class="sxs-lookup"><span data-stu-id="ccb41-104">Troubleshoot co-sell referrals connectors</span></span>

<span data-ttu-id="ccb41-105">**Aplica-se a**: Dynamics 365 CRM | Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="ccb41-105">**Applies to**: Dynamics 365 CRM | Salesforce CRM</span></span>

<span data-ttu-id="ccb41-106">**Funções apropriadas:** indicações de administrador | Administrador do sistema ou personalizador de sistema no CRM</span><span class="sxs-lookup"><span data-stu-id="ccb41-106">**Appropriate roles**: Referrals admin | System admin or system customizer on the CRM</span></span>

 ## <a name="questions-and-answers-about-pre-requisites"></a><span data-ttu-id="ccb41-107">Perguntas e respostas sobre pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ccb41-107">Questions and answers about pre-requisites</span></span>

1. <span data-ttu-id="ccb41-108">Você pode usar uma solução de conectores de indicações de venda co-venda de avaliação para seu ambiente?</span><span class="sxs-lookup"><span data-stu-id="ccb41-108">Can you use a trial co-sell referrals connectors solution for your environment?</span></span>

<span data-ttu-id="ccb41-109">Se você estiver no ambiente de teste/preparação, poderá optar pela solução de avaliação.</span><span class="sxs-lookup"><span data-stu-id="ccb41-109">If you are on the test/staging environment, you can opt for trial solution.</span></span> <span data-ttu-id="ccb41-110">A versão paga dos Conectores está disponível no AppSource por US$ 15/mês.</span><span class="sxs-lookup"><span data-stu-id="ccb41-110">The paid version of the Connectors is available in AppSource at US$ 15/month.</span></span> <span data-ttu-id="ccb41-111">Com a conexão paga, você receberá chamadas à API de 10 mil por dia.</span><span class="sxs-lookup"><span data-stu-id="ccb41-111">With the paid connection, you will be getting 10K API calls per day.</span></span> <span data-ttu-id="ccb41-112">Os Conectores são wrappers sobre as APIs Partner Center referência.</span><span class="sxs-lookup"><span data-stu-id="ccb41-112">The Connectors are wrappers on top of Partner Center referral APIs.</span></span> <span data-ttu-id="ccb41-113">Sempre que as soluções  de conector são executados para um evento Criar ou Atualizar nas oportunidades no lado Partner Center crm, uma chamada à API é feita. </span><span class="sxs-lookup"><span data-stu-id="ccb41-113">Whenever the connector solutions run for a **Create** or **Update** event on the opportunities on either Partner Center or the CRM side, an API call is made.</span></span>

2. <span data-ttu-id="ccb41-114">Qual função você precisa para criar seções no ambiente crm?</span><span class="sxs-lookup"><span data-stu-id="ccb41-114">What role do you need to create sections in CRM environment?</span></span>

<span data-ttu-id="ccb41-115">Os usuários que são administradores do sistema ou personalizadores do sistema podem aplicar alterações a todos.</span><span class="sxs-lookup"><span data-stu-id="ccb41-115">Users who are system admins or system customizers can apply changes for everyone.</span></span> <span data-ttu-id="ccb41-116">No entanto, todos os usuários do aplicativo podem personalizar o sistema e até mesmo compartilhar algumas de suas personalizações com outras pessoas.</span><span class="sxs-lookup"><span data-stu-id="ccb41-116">All app users, however,  can personalize the system and even share some of their customizations with others.</span></span> 

3. <span data-ttu-id="ccb41-117">Os vendedores parceiros precisam de funções especiais para trabalhar Partner Center?</span><span class="sxs-lookup"><span data-stu-id="ccb41-117">Do partner sellers need special roles to work on Partner Center?</span></span>
 
<span data-ttu-id="ccb41-118">Os vendedores parceiros devem ser atribuídos à função "Administrador de indicações".</span><span class="sxs-lookup"><span data-stu-id="ccb41-118">Partner sellers must be assigned the “Referrals admin” role.</span></span> <span data-ttu-id="ccb41-119">Para obter mais informações, consulte [Visão geral de permissões.](create-user-accounts-and-set-permissions.md)</span><span class="sxs-lookup"><span data-stu-id="ccb41-119">For more information, see [Permissions overview](create-user-accounts-and-set-permissions.md).</span></span>

4. <span data-ttu-id="ccb41-120">Quais campos precisam ser definidos primeiro em seu ambiente crm?</span><span class="sxs-lookup"><span data-stu-id="ccb41-120">What fields need to be set up first in your CRM environment?</span></span> 

<span data-ttu-id="ccb41-121">• Verifique se a moeda é apropriada para sua localização e se está em seu ambiente crm com precisão.</span><span class="sxs-lookup"><span data-stu-id="ccb41-121">• Make sure your currency is appropriate to your location and is in your CRM environment accurately.</span></span> <span data-ttu-id="ccb41-122">• Sua equipe de vendas deve estar listada em seu ambiente de CRM como usuários do CRM.</span><span class="sxs-lookup"><span data-stu-id="ccb41-122">• Your sales team should be listed in your CRM environment as CRM users.</span></span>

5. <span data-ttu-id="ccb41-123">Quais pré-requisitos são necessários para a criação Power Automate ambiente?</span><span class="sxs-lookup"><span data-stu-id="ccb41-123">What pre-requisites are required for Power Automate environment creation?</span></span>

<span data-ttu-id="ccb41-124">Para usar o Power Automate, você precisa:</span><span class="sxs-lookup"><span data-stu-id="ccb41-124">To use the Power Automate environment, you need:</span></span>

- <span data-ttu-id="ccb41-125">Uma Power Automate é necessária.</span><span class="sxs-lookup"><span data-stu-id="ccb41-125">A Power Automate license is required.</span></span>
- <span data-ttu-id="ccb41-126">Um mínimo de 1 GB de armazenamento é necessário.</span><span class="sxs-lookup"><span data-stu-id="ccb41-126">A minimum of 1-GB storage is required.</span></span>

6.  <span data-ttu-id="ccb41-127">Você precisa de uma assinatura do Dynamics 365 para usar a solução Conectores do Salesforce?</span><span class="sxs-lookup"><span data-stu-id="ccb41-127">Do you need a Dynamics 365 subscription to use Salesforce Connectors solution?</span></span>

<span data-ttu-id="ccb41-128">A solução conector do Salesforce é do tipo "Dynamics Flow" que dá suporte à sincronização com outros sistemas CRM.</span><span class="sxs-lookup"><span data-stu-id="ccb41-128">The Salesforce Connector solution is of type “Dynamics Flow” that supports synchronizing with other CRM systems.</span></span> <span data-ttu-id="ccb41-129">A solução não exige que você tenha uma instância do Dynamics 365 ou uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="ccb41-129">The solution doesn’t require you to have a Dynamics 365 instance or a subscription.</span></span> <span data-ttu-id="ccb41-130">Durante a instalação da solução Salesforce, uma lista listada com o ambiente CDS existente em sua empresa pode aparecer.</span><span class="sxs-lookup"><span data-stu-id="ccb41-130">While installing the Salesforce solution, a drop-down with existing CDS environment in your company may appear.</span></span> <span data-ttu-id="ccb41-131">Você precisa selecionar esse ambiente.</span><span class="sxs-lookup"><span data-stu-id="ccb41-131">You need to select that environment.</span></span> <span data-ttu-id="ccb41-132">Além disso, se você receber o erro "Não foi possível encontrar uma organização do Dynamics 365 conectada ao usuário conectado", será necessário criar um novo ambiente para o conector.</span><span class="sxs-lookup"><span data-stu-id="ccb41-132">In addition, if you get the error "We couldn't find a Dynamics 365 organization connected to signed-in user", then you will need to create new environment for connector.</span></span>

## <a name="questions-and-answers-about-configuration"></a><span data-ttu-id="ccb41-133">Perguntas e respostas sobre a configuração</span><span class="sxs-lookup"><span data-stu-id="ccb41-133">Questions and answers about configuration</span></span>

1. <span data-ttu-id="ccb41-134">O que você deve fazer se enfrentar o seguinte erro ao ativar fluxos no Power Automate Platform?</span><span class="sxs-lookup"><span data-stu-id="ccb41-134">What should you do if you face the following error while activating flows in Power Automate Platform?</span></span>

<span data-ttu-id="ccb41-135">Erro: a solicitação para Azure Resource Manager falhou com o erro: '{"error":{"code":"WorkflowTriggerNotFound","message":"O fluxo de trabalho 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' não pôde ser encontrado."}}'.</span><span class="sxs-lookup"><span data-stu-id="ccb41-135">Error: Request to Azure Resource Manager failed with error: '{"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'.</span></span> 

<span data-ttu-id="ccb41-136">Siga estas etapas de solução de problemas:</span><span class="sxs-lookup"><span data-stu-id="ccb41-136">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="ccb41-137">Exclua a conexão CDS e recrie as conexões CDS.</span><span class="sxs-lookup"><span data-stu-id="ccb41-137">Delete the CDS connection and then recreate the CDS connections.</span></span>
- <span data-ttu-id="ccb41-138">Ativar e desativar o fluxo filho</span><span class="sxs-lookup"><span data-stu-id="ccb41-138">Turn the child flow off and on</span></span> 
- <span data-ttu-id="ccb41-139">Exclua a solução e reinstale a solução.</span><span class="sxs-lookup"><span data-stu-id="ccb41-139">Delete solution and then reinstall the solution.</span></span> 

2.  <span data-ttu-id="ccb41-140">O que você deve fazer se enfrentar o erro "Entrar" ao adicionar um conector Partner Center na Power Automate Platform?</span><span class="sxs-lookup"><span data-stu-id="ccb41-140">What should you do if you face the "Sign in" error while adding a Partner Center connector in Power Automate Platform?</span></span>

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Mensagem de erro que exige a login.":::

<span data-ttu-id="ccb41-142">Siga esta etapa de solução de problemas:</span><span class="sxs-lookup"><span data-stu-id="ccb41-142">Follow this troubleshooting step:</span></span>

- <span data-ttu-id="ccb41-143">Use suas Partner Center de usuário para entrar no ambiente de fluxo uma vez (flow.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="ccb41-143">Use your Partner Center credentials to sign into the flow environment once (flow.microsoft.com).</span></span>


3. <span data-ttu-id="ccb41-144">O que você deve fazer se receber o erro a seguir ao ativar o fluxo Partner Center crm no Power Automate Platform?</span><span class="sxs-lookup"><span data-stu-id="ccb41-144">What should you do if you receive the following error while activating the Partner Center to CRM flow in Power Automate Platform?</span></span>
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Mensagem de erro que exige atualizações.":::

<span data-ttu-id="ccb41-146">Siga estas etapas de solução de problemas:</span><span class="sxs-lookup"><span data-stu-id="ccb41-146">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="ccb41-147">Primeiro, ative os dois fluxos filho a seguir antes de ativar a Partner Center para o fluxo crm.</span><span class="sxs-lookup"><span data-stu-id="ccb41-147">Activate the following two child flows first before you activate the Partner Center to CRM flow.</span></span>
      - <span data-ttu-id="ccb41-148">Partner Center CRM – Auxiliar (Visualização do Insider)</span><span class="sxs-lookup"><span data-stu-id="ccb41-148">Partner Center to CRM - Helper (Insider Preview)</span></span>
      - <span data-ttu-id="ccb41-149">Partner Center atualizações de indicação de venda co-venda da Microsoft para CRM (Visualização do Insider)</span><span class="sxs-lookup"><span data-stu-id="ccb41-149">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span></span>

4. <span data-ttu-id="ccb41-150">O que você deve fazer quando não é possível adicionar conexões ao fluxo ao tentar editar o fluxo?</span><span class="sxs-lookup"><span data-stu-id="ccb41-150">What should you do when you aren't able to add connections to the flow when you try to edit the flow?</span></span>

<span data-ttu-id="ccb41-151">Você adiciona conexões ao fluxo enquanto o fluxo está em execução e adiciona a cada fluxo separadamente.</span><span class="sxs-lookup"><span data-stu-id="ccb41-151">You add connections to the flow while the flow is running, and you add to each flow separately.</span></span>  <span data-ttu-id="ccb41-152">Se a caixa de diálogo para adicionar conexões não for aberta automaticamente durante a edição do fluxo, você poderá editar cada uma das etapas e sub etapas dos fluxos individualmente.</span><span class="sxs-lookup"><span data-stu-id="ccb41-152">If the dialog to add connections doesn't open up automatically while editing the flow, then you can edit each of the steps and sub steps of the flows individually.</span></span>

- <span data-ttu-id="ccb41-153">Selecione cada fluxo e edite-os individualmente.</span><span class="sxs-lookup"><span data-stu-id="ccb41-153">Select each flow and edit them individually.</span></span>
- <span data-ttu-id="ccb41-154">Expanda todas as etapas no fluxo</span><span class="sxs-lookup"><span data-stu-id="ccb41-154">Expand all the steps in the flow</span></span> 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Etapas que precisam de conexões.":::

- <span data-ttu-id="ccb41-156">Selecione as etapas em que você vê um ícone de aviso solicitando a associação de conexões e adicione conexões.</span><span class="sxs-lookup"><span data-stu-id="ccb41-156">Select the steps where you see a warning icon asking to associate connections, and add connections.</span></span> 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Edite o fluxo passo a passo.":::


5. <span data-ttu-id="ccb41-158">O que você deve fazer se os fluxos da solução Conectores de Indicações de Venda Co-venda não ativarem?</span><span class="sxs-lookup"><span data-stu-id="ccb41-158">What should you do if the flows of the Co-sell Referrals Connectors solution don’t turn on?</span></span>

<span data-ttu-id="ccb41-159">a.</span><span class="sxs-lookup"><span data-stu-id="ccb41-159">A.</span></span> <span data-ttu-id="ccb41-160">Em Power Automate, você precisará editar fluxos na seguinte ordem e atualizá-los para usar as conexões corretas:</span><span class="sxs-lookup"><span data-stu-id="ccb41-160">In Power Automate, you'll need to edit flows in the following order and update them to use the correct connections:</span></span>

- <span data-ttu-id="ccb41-161">Partner Center de webhook (visualização do insider)</span><span class="sxs-lookup"><span data-stu-id="ccb41-161">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="ccb41-162">Criar indicação de venda co-venda – Salesforce para Partner Center (Visualização do Insider)</span><span class="sxs-lookup"><span data-stu-id="ccb41-162">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="ccb41-163">Partner Center atualizações de indicação de venda co-venda da Microsoft para o Salesforce (Visualização do Insider)</span><span class="sxs-lookup"><span data-stu-id="ccb41-163">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="ccb41-164">Partner Center ao Salesforce (Visualização do Insider)</span><span class="sxs-lookup"><span data-stu-id="ccb41-164">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="ccb41-165">Salesforce para Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="ccb41-165">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="ccb41-166">Salesforce Opportunity to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="ccb41-166">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="ccb41-167">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="ccb41-167">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

 <span data-ttu-id="ccb41-168">B.</span><span class="sxs-lookup"><span data-stu-id="ccb41-168">B.</span></span> <span data-ttu-id="ccb41-169">Para cada fluxo, selecione a **opção Executar somente usuários.**</span><span class="sxs-lookup"><span data-stu-id="ccb41-169">For each of flow, select **Run only users** option.</span></span> <span data-ttu-id="ccb41-170">Selecione **Usar conexão** em vez de Fornecido pelo usuário somente de **run.**</span><span class="sxs-lookup"><span data-stu-id="ccb41-170">Select **Use connection** instead of **Provided by run-only user**.</span></span>  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Para ativar um fluxo.":::


<span data-ttu-id="ccb41-172">C.</span><span class="sxs-lookup"><span data-stu-id="ccb41-172">C.</span></span> <span data-ttu-id="ccb41-173">Ative estes fluxos mencionados abaixo:</span><span class="sxs-lookup"><span data-stu-id="ccb41-173">Activate these below mentioned flows:</span></span>

 - <span data-ttu-id="ccb41-174">Partner Center atualizações de indicação de venda co-venda da Microsoft para o Salesforce (Visualização do Insider)</span><span class="sxs-lookup"><span data-stu-id="ccb41-174">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>

- <span data-ttu-id="ccb41-175">Salesforce para Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="ccb41-175">Salesforce to Partner Center (Insider Preview)</span></span>

    
<span data-ttu-id="ccb41-176">D.</span><span class="sxs-lookup"><span data-stu-id="ccb41-176">D.</span></span> <span data-ttu-id="ccb41-177">Ative todos os fluxos restantes.</span><span class="sxs-lookup"><span data-stu-id="ccb41-177">Activate all the remaining flows.</span></span>

<span data-ttu-id="ccb41-178">E.</span><span class="sxs-lookup"><span data-stu-id="ccb41-178">E.</span></span> <span data-ttu-id="ccb41-179">No fluxo Partner Center Registro de Webhook, selecione **Executar**.</span><span class="sxs-lookup"><span data-stu-id="ccb41-179">At flow Partner Center Webhook Registration, select **Run**.</span></span> <span data-ttu-id="ccb41-180">Forneça a **URL http** da primeira ação no Partner Center ao fluxo **do Salesforce.**</span><span class="sxs-lookup"><span data-stu-id="ccb41-180">Provide the **http url** from the first action in **Partner Center to Salesforce** flow.</span></span> <span data-ttu-id="ccb41-181">Select all quatro opções em **Eventos para registrar** e selecionar **sim** para Substituir.</span><span class="sxs-lookup"><span data-stu-id="ccb41-181">Select all four options under **Events to register** and select **yes** for Overwrite.</span></span>

## <a name="questions-and-answers-about-runmaintenance"></a><span data-ttu-id="ccb41-182">Perguntas e respostas sobre a manutenção/a manutenção</span><span class="sxs-lookup"><span data-stu-id="ccb41-182">Questions and answers about Run/Maintenance</span></span>

1. <span data-ttu-id="ccb41-183">Como solucionar problemas de falhas durante a execução Power Automate fluxo?</span><span class="sxs-lookup"><span data-stu-id="ccb41-183">How do you troubleshoot failures during Power Automate flow execution?</span></span>

<span data-ttu-id="ccb41-184">Para garantir que seus fluxos de Power Automate executados conforme o esperado e solucionar falhas durante a execução, consulte Corrigir falhas [de fluxo.](/power-automate/fix-flow-failures)</span><span class="sxs-lookup"><span data-stu-id="ccb41-184">To ensure that your Power Automate flows run as you expect and to troubleshoot failures during execution, refer to [Fix flow failures](/power-automate/fix-flow-failures).</span></span>

2. <span data-ttu-id="ccb41-185">O que você deve fazer se vir indicações que não estão sincronizadas corretamente no Partner Center ou ambiente crm?</span><span class="sxs-lookup"><span data-stu-id="ccb41-185">What should you do if you see referrals that aren't synchronized properly in Partner Center or CRM environment?</span></span>
 
<span data-ttu-id="ccb41-186">Para determinar o status da sincronização de indicação, selecione **Auditar**.</span><span class="sxs-lookup"><span data-stu-id="ccb41-186">To determine the status of referral synchronization, select **Audit**.</span></span> 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Como sincronizar indicações.":::

<span data-ttu-id="ccb41-188">Verifique se as seguintes condições foram atendidas:</span><span class="sxs-lookup"><span data-stu-id="ccb41-188">Ensure that the following conditions are met:</span></span>

- <span data-ttu-id="ccb41-189">A ID da solução é fornecida como parte da oportunidade.</span><span class="sxs-lookup"><span data-stu-id="ccb41-189">Solution ID is provided as part of the opportunity.</span></span>

- <span data-ttu-id="ccb41-190">O código de país de duas letras é necessário.</span><span class="sxs-lookup"><span data-stu-id="ccb41-190">Two letter country code is required.</span></span>

- <span data-ttu-id="ccb41-191">Quando a ajuda da Microsoft é selecionada para a oportunidade, as informações de contato do cliente são necessárias.</span><span class="sxs-lookup"><span data-stu-id="ccb41-191">When help from Microsoft is selected for the opportunity, customer contact information is required.</span></span>

3. <span data-ttu-id="ccb41-192">Como garantir que uma indicação seja sincronizada de forma bi-direcional?</span><span class="sxs-lookup"><span data-stu-id="ccb41-192">How to ensure that a referral will synchronize bi-directionally?</span></span>

<span data-ttu-id="ccb41-193">Execute as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="ccb41-193">Do the following steps:</span></span>

- <span data-ttu-id="ccb41-194">Os vendedores parceiros precisam garantir que tenham habilitado a opção Sincronizar **com Partner Center** na seção CRM.</span><span class="sxs-lookup"><span data-stu-id="ccb41-194">Partner sellers need to ensure that they have enabled **Sync with Partner Center** option in the CRM section.</span></span>

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Verifique se você habilitar o Synch.":::

- <span data-ttu-id="ccb41-196">Os vendedores precisam fornecer a receita e a data de fechamento ao qualificar um lead.</span><span class="sxs-lookup"><span data-stu-id="ccb41-196">Sellers need to provide revenue and closing date when qualifying a lead.</span></span>

- <span data-ttu-id="ccb41-197">Se a ID do  CRM  for fornecida no estágio de criação ou atualização da oportunidade de venda co-venda, mas uma oportunidade de venda futura com essa ID não for encontrada no CRM, a atualização ou a criação será ignorada.</span><span class="sxs-lookup"><span data-stu-id="ccb41-197">If CRM ID is provided in the **create** or **update** stage of co-sell opportunity, but a lead opportunity with that ID is not found in CRM, then update or create will be ignored.</span></span>

- <span data-ttu-id="ccb41-198">Verifique se o campo moeda de indicação está configurado no ambiente do Salesforce.</span><span class="sxs-lookup"><span data-stu-id="ccb41-198">Ensure that referral currency field is configured on Salesforce environment.</span></span> 

4. <span data-ttu-id="ccb41-199">O que você deve fazer se o conector for desconectado e você perder uma sincronização de indicação.?</span><span class="sxs-lookup"><span data-stu-id="ccb41-199">What should you do if the connector gets disconnected and you miss a referral synchronization.?</span></span>

<span data-ttu-id="ccb41-200">A seguir estão algumas das opções que você pode experimentar:</span><span class="sxs-lookup"><span data-stu-id="ccb41-200">Following are few of the options that you can try out:</span></span>

- <span data-ttu-id="ccb41-201">Verifique se o nome de usuário ou a senha expirou para o Partner Center usuário com funções de administrador de indicação.</span><span class="sxs-lookup"><span data-stu-id="ccb41-201">Check whether username or password has expired for the Partner Center user with referral admin roles.</span></span>

- <span data-ttu-id="ccb41-202">Você pode ir para a oportunidade não sincronizada, fazer uma atualização secundária e observar se a indicação foi sincronizada.</span><span class="sxs-lookup"><span data-stu-id="ccb41-202">You can go to the un-synchronized opportunity, make a minor update, and observe whether the referral has synchronized.</span></span>

- <span data-ttu-id="ccb41-203">Se os fluxos foram executados e falharam, selecione o fluxo e envie a sequência que falhou.</span><span class="sxs-lookup"><span data-stu-id="ccb41-203">If the flows have run and failed, then select the flow and re-submit the run that has failed.</span></span>

5. <span data-ttu-id="ccb41-204">O que você deve fazer quando recebe erros de acesso negado?</span><span class="sxs-lookup"><span data-stu-id="ccb41-204">What should you do when you get access denied errors?</span></span>

<span data-ttu-id="ccb41-205">Certifique-se de que as funções apropriadas existam</span><span class="sxs-lookup"><span data-stu-id="ccb41-205">Make sure the appropriate roles exist</span></span>

- <span data-ttu-id="ccb41-206">Função administrador de indicação para Partner Center vendedor</span><span class="sxs-lookup"><span data-stu-id="ccb41-206">Referral Administrator role for Partner Center seller</span></span> 
 
- <span data-ttu-id="ccb41-207">Função administrador do sistema ou personalizador do sistema em sua instância do CRM</span><span class="sxs-lookup"><span data-stu-id="ccb41-207">System Administrator or System Customizer role on your CRM instance</span></span>

- <span data-ttu-id="ccb41-208">Verifique se o usuário Power Automate conta de fluxo de dados faz logo no https://flow.microsoft.com pelo menos uma vez com antecedência</span><span class="sxs-lookup"><span data-stu-id="ccb41-208">Ensure that the Power Automate flow account user logs into https://flow.microsoft.com at least once beforehand</span></span>

6. <span data-ttu-id="ccb41-209">Se você vir que **o código do país** da conta do cliente está ausente durante a criação de uma oportunidade de venda de venda, o que você deve fazer?</span><span class="sxs-lookup"><span data-stu-id="ccb41-209">If you see that **Customer account country code** is missing while creating a Co-sell opportunity, what should you do?</span></span>

<span data-ttu-id="ccb41-210">Você precisará adicionar o código do país ISO de duas letras à conta do cliente no CRM.</span><span class="sxs-lookup"><span data-stu-id="ccb41-210">You will need to add the ISO two-letter country code to the Customer account in CRM.</span></span>

7. <span data-ttu-id="ccb41-211">O que você deve fazer se vir o erro de que a **ID da Solução é necessária** durante a criação de uma oportunidade de venda co-venda?</span><span class="sxs-lookup"><span data-stu-id="ccb41-211">What should you do if you see the error that **Solution ID is required** while creating a Co-sell opportunity?</span></span>

<span data-ttu-id="ccb41-212">Para criar uma indicação de venda em cooperação, você precisa de uma solução pronta para venda em cooperação da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ccb41-212">In order to create a co-sell referral, you need a Microsoft co-sell ready solution.</span></span> 

8. <span data-ttu-id="ccb41-213">O que você deve fazer quando vir oportunidades de venda de Partner Center criadas no Partner Center que não estão sincronizadas com o CRM, mesmo que não haja erros de fluxo?</span><span class="sxs-lookup"><span data-stu-id="ccb41-213">What should you do when you see Co-sell opportunities created in Partner Center that aren't synchronized to CRM even though there are no flow errors?</span></span>

<span data-ttu-id="ccb41-214">Faça o seguinte:</span><span class="sxs-lookup"><span data-stu-id="ccb41-214">Do the following:</span></span>

- <span data-ttu-id="ccb41-215">Depois de criar uma nova oferta de venda em Partner Center, verifique se Partner Center para o fluxo do Dynamics 365 é invocado (ele pode ser invocado várias vezes).</span><span class="sxs-lookup"><span data-stu-id="ccb41-215">After you have created a new co-sell deal in Partner Center, check if Partner Center to Dynamics 365 flow gets invoked (it might get invoked multiple times).</span></span>

- <span data-ttu-id="ccb41-216">Se o fluxo for invocado, verifique todos os fluxos invocados e identifique a run de fluxo que atualizaria o CRM.</span><span class="sxs-lookup"><span data-stu-id="ccb41-216">If the flow gets invoked, check all invoked flows, and identify the flow run which that would update the CRM.</span></span> <span data-ttu-id="ccb41-217">Você pode seguir as ações e verificar se ele atualiza o CRM ou se encontrou um problema.</span><span class="sxs-lookup"><span data-stu-id="ccb41-217">You can follow the actions and verify if it did update the CRM or encountered a problem.</span></span>

- <span data-ttu-id="ccb41-218">Verifique **Nova oferta** no Partner Center para ver se ela é preenchida com a ID do CRM.</span><span class="sxs-lookup"><span data-stu-id="ccb41-218">Check **New deal** in Partner Center to see if it gets populated with CRM ID.</span></span>

- <span data-ttu-id="ccb41-219">Certifique-se de que o negócio não foi fechado acidentalmente **como Won** ou **Lost** no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="ccb41-219">Make sure that the deal is not accidentally closed as **Won** or **Lost** in Partner Center.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ccb41-220">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="ccb41-220">Next steps</span></span>

- [<span data-ttu-id="ccb41-221">Gerenciar clientes potenciais</span><span class="sxs-lookup"><span data-stu-id="ccb41-221">Manage leads</span></span>](manage-leads.md)
 
- [<span data-ttu-id="ccb41-222">Gerenciar oportunidades de venda conjunta</span><span class="sxs-lookup"><span data-stu-id="ccb41-222">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
