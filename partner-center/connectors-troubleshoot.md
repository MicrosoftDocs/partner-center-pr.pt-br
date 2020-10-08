---
title: Solucionar problemas de conectores de referências de venda conjunta
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Perguntas frequentes sobre como solucionar problemas de conectores de televenda.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 312ff9155ab4c2d84fb38bb6ccd093505e628832
ms.sourcegitcommit: df7643f3b7978e164e419e447a4dc3c163cb3bd2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/08/2020
ms.locfileid: "91844650"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a><span data-ttu-id="747a1-103">Solucionar problemas de conectores de referências de venda conjunta</span><span class="sxs-lookup"><span data-stu-id="747a1-103">Troubleshoot co-sell referrals connectors</span></span>

<span data-ttu-id="747a1-104">**Aplica-se a:**</span><span class="sxs-lookup"><span data-stu-id="747a1-104">**Applies to:**</span></span>

- <span data-ttu-id="747a1-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="747a1-105">Partner Center</span></span>
- <span data-ttu-id="747a1-106">CRM do Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="747a1-106">Dynamics 365 CRM</span></span>
- <span data-ttu-id="747a1-107">CRM do Salesforce</span><span class="sxs-lookup"><span data-stu-id="747a1-107">Salesforce CRM</span></span>

<span data-ttu-id="747a1-108">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="747a1-108">**Appropriate roles**</span></span>

- <span data-ttu-id="747a1-109">Administrador de indicações</span><span class="sxs-lookup"><span data-stu-id="747a1-109">Referrals admin</span></span>
- <span data-ttu-id="747a1-110">Administrador do sistema ou personalizador do sistema no CRM</span><span class="sxs-lookup"><span data-stu-id="747a1-110">System admin or system customizer on the CRM</span></span>

 ## <a name="questions-and-answers-about-pre-requisites"></a><span data-ttu-id="747a1-111">Perguntas e respostas sobre os pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="747a1-111">Questions and answers about pre-requisites</span></span>

1. <span data-ttu-id="747a1-112">É possível usar uma solução de avaliação de conectores de indicações para o seu ambiente?</span><span class="sxs-lookup"><span data-stu-id="747a1-112">Can you use a trial co-sell referrals connectors solution for your environment?</span></span>

<span data-ttu-id="747a1-113">Se você estiver no ambiente de teste/preparo, poderá optar pela solução de avaliação.</span><span class="sxs-lookup"><span data-stu-id="747a1-113">If you are on the test/staging environment, you can opt for trial solution.</span></span> <span data-ttu-id="747a1-114">A versão paga dos conectores está disponível em AppSource a US $15/mês.</span><span class="sxs-lookup"><span data-stu-id="747a1-114">The paid version of the Connectors is available in AppSource at US$ 15/month.</span></span> <span data-ttu-id="747a1-115">Com a conexão paga, você receberá chamadas de API de 10K por dia.</span><span class="sxs-lookup"><span data-stu-id="747a1-115">With the paid connection, you will be getting 10K API calls per day.</span></span> <span data-ttu-id="747a1-116">Os conectores são wrappers sobre as APIs de referência do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="747a1-116">The Connectors are wrappers on top of Partner Center referral APIs.</span></span> <span data-ttu-id="747a1-117">Sempre que as soluções de conector são executadas para um evento de **criação** ou **atualização** nas oportunidades no lado do parceiro ou do CRM, é feita uma chamada à API.</span><span class="sxs-lookup"><span data-stu-id="747a1-117">Whenever the connector solutions run for a **Create** or **Update** event on the opportunities on either Partner Center or the CRM side, an API call is made.</span></span>

2. <span data-ttu-id="747a1-118">Que função você precisa para criar seções no ambiente CRM?</span><span class="sxs-lookup"><span data-stu-id="747a1-118">What role do you need to create sections in CRM environment?</span></span>

<span data-ttu-id="747a1-119">Os usuários que são administradores de sistema ou personalizadores de sistema podem aplicar alterações para todos.</span><span class="sxs-lookup"><span data-stu-id="747a1-119">Users who are system admins or system customizers can apply changes for everyone.</span></span> <span data-ttu-id="747a1-120">No entanto, todos os usuários do aplicativo podem personalizar o sistema e até compartilhar algumas de suas personalizações com outras pessoas.</span><span class="sxs-lookup"><span data-stu-id="747a1-120">All app users, however,  can personalize the system and even share some of their customizations with others.</span></span> 

3. <span data-ttu-id="747a1-121">Os vendedores de parceiros precisam de funções especiais para trabalhar no Partner Center?</span><span class="sxs-lookup"><span data-stu-id="747a1-121">Do partner sellers need special roles to work on Partner Center?</span></span>
 
<span data-ttu-id="747a1-122">Os vendedores do parceiro devem ser atribuídos à função "administrador de referências".</span><span class="sxs-lookup"><span data-stu-id="747a1-122">Partner sellers must be assigned the “Referrals admin” role.</span></span> <span data-ttu-id="747a1-123">Para obter mais informações, consulte o seguinte [Visão geral de permissões) (Create-User-Accounts-and-Set-Permissions).</span><span class="sxs-lookup"><span data-stu-id="747a1-123">For more information, refer to the following [Permissions overview)(create-user-accounts-and-set-permissions).</span></span>

4. <span data-ttu-id="747a1-124">Quais campos precisam ser configurados primeiro em seu ambiente de CRM?</span><span class="sxs-lookup"><span data-stu-id="747a1-124">What fields need to be set up first in your CRM environment?</span></span> 

<span data-ttu-id="747a1-125">• Verifique se sua moeda é apropriada para seu local e se está em seu ambiente CRM com precisão.</span><span class="sxs-lookup"><span data-stu-id="747a1-125">• Make sure your currency is appropriate to your location and is in your CRM environment accurately.</span></span> <span data-ttu-id="747a1-126">• Sua equipe de vendas deve estar listada em seu ambiente de CRM como usuários do CRM.</span><span class="sxs-lookup"><span data-stu-id="747a1-126">• Your sales team should be listed in your CRM environment as CRM users.</span></span>

5. <span data-ttu-id="747a1-127">Quais pré-requisitos são necessários para a criação do ambiente de automatização de energia?</span><span class="sxs-lookup"><span data-stu-id="747a1-127">What pre-requisites are required for Power Automate environment creation?</span></span>

<span data-ttu-id="747a1-128">Para usar o ambiente de automatização de energia, você precisa:</span><span class="sxs-lookup"><span data-stu-id="747a1-128">To use the Power Automate environment, you need:</span></span>

- <span data-ttu-id="747a1-129">Uma licença de automatização de energia é necessária.</span><span class="sxs-lookup"><span data-stu-id="747a1-129">A Power Automate license is required.</span></span>
- <span data-ttu-id="747a1-130">É necessário um mínimo de armazenamento de 1 GB.</span><span class="sxs-lookup"><span data-stu-id="747a1-130">A minimum of 1-GB storage is required.</span></span>

6.  <span data-ttu-id="747a1-131">Você precisa de uma assinatura do Dynamics 365 para usar a solução de conectores do Salesforce?</span><span class="sxs-lookup"><span data-stu-id="747a1-131">Do you need a Dynamics 365 subscription to use Salesforce Connectors solution?</span></span>

<span data-ttu-id="747a1-132">A solução do conector do Salesforce é do tipo "fluxo do Dynamics" que dá suporte à sincronização com outros sistemas de CRM.</span><span class="sxs-lookup"><span data-stu-id="747a1-132">The Salesforce Connector solution is of type “Dynamics Flow” that supports synchronizing with other CRM systems.</span></span> <span data-ttu-id="747a1-133">A solução não exige que você tenha uma instância ou assinatura do Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="747a1-133">The solution doesn’t require you to have a Dynamics 365 instance or a subscription.</span></span> <span data-ttu-id="747a1-134">Ao instalar a solução Salesforce, uma lista suspensa com um ambiente de CDS existente em sua empresa pode ser exibida.</span><span class="sxs-lookup"><span data-stu-id="747a1-134">While installing the Salesforce solution, a drop-down with existing CDS environment in your company may appear.</span></span> <span data-ttu-id="747a1-135">Você precisa selecionar esse ambiente.</span><span class="sxs-lookup"><span data-stu-id="747a1-135">You need to select that environment.</span></span> <span data-ttu-id="747a1-136">Além disso, se você receber o erro "não foi possível encontrar uma organização do Dynamics 365 conectada ao usuário conectado", será necessário criar um novo ambiente para o conector.</span><span class="sxs-lookup"><span data-stu-id="747a1-136">In addition, if you get the error "We couldn't find a Dynamics 365 organization connected to signed-in user", then you will need to create new environment for connector.</span></span>

## <a name="questions-and-answers-about-configuration"></a><span data-ttu-id="747a1-137">Perguntas e respostas sobre a configuração</span><span class="sxs-lookup"><span data-stu-id="747a1-137">Questions and answers about configuration</span></span>

1. <span data-ttu-id="747a1-138">O que você deve fazer se enfrentar o seguinte erro ao ativar fluxos na plataforma Power Automate?</span><span class="sxs-lookup"><span data-stu-id="747a1-138">What should you do if you face the following error while activating flows in Power Automate Platform?</span></span>

<span data-ttu-id="747a1-139">Erro: a solicitação para Azure Resource Manager falhou com o erro: ' {"erro": {"código": "WorkflowTriggerNotFound", "Message": "não foi possível encontrar o gatilho ' manual ' do fluxo de trabalho ' e14d00f1-1fdf-4b1b-AAAC-54a5064093d3 '."}} '.</span><span class="sxs-lookup"><span data-stu-id="747a1-139">Error: Request to Azure Resource Manager failed with error: '{"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'.</span></span> 

<span data-ttu-id="747a1-140">Siga estas etapas de solução de problemas:</span><span class="sxs-lookup"><span data-stu-id="747a1-140">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="747a1-141">Exclua a conexão de CDS e recrie as conexões de CDS.</span><span class="sxs-lookup"><span data-stu-id="747a1-141">Delete the CDS connection and then recreate the CDS connections.</span></span>
- <span data-ttu-id="747a1-142">Desativar e ativar o fluxo filho</span><span class="sxs-lookup"><span data-stu-id="747a1-142">Turn the child flow off and on</span></span> 
- <span data-ttu-id="747a1-143">Exclua a solução e reinstale a solução.</span><span class="sxs-lookup"><span data-stu-id="747a1-143">Delete solution and then reinstall the solution.</span></span> 

2.  <span data-ttu-id="747a1-144">O que você deve fazer se enfrentar o erro "entrar" ao adicionar um conector do Partner Center na plataforma Power Automate?</span><span class="sxs-lookup"><span data-stu-id="747a1-144">What should you do if you face the "Sign in" error while adding a Partner Center connector in Power Automate Platform?</span></span>

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Mensagem de erro que requer entrada":::

<span data-ttu-id="747a1-146">Siga esta etapa de solução de problemas:</span><span class="sxs-lookup"><span data-stu-id="747a1-146">Follow this troubleshooting step:</span></span>

- <span data-ttu-id="747a1-147">Use suas credenciais do Partner Center para entrar no ambiente de fluxo uma vez (flow.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="747a1-147">Use your Partner Center credentials to sign into the flow environment once (flow.microsoft.com).</span></span>


3. <span data-ttu-id="747a1-148">O que você deve fazer se receber o seguinte erro ao ativar o Partner Center para o fluxo do CRM na plataforma de energia automatizada?</span><span class="sxs-lookup"><span data-stu-id="747a1-148">What should you do if you receive the following error while activating the Partner Center to CRM flow in Power Automate Platform?</span></span>
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Mensagem de erro que requer entrada":::

<span data-ttu-id="747a1-150">Siga estas etapas de solução de problemas:</span><span class="sxs-lookup"><span data-stu-id="747a1-150">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="747a1-151">Ative primeiro os dois fluxos filho a seguir antes de ativar o Partner Center para o fluxo do CRM.</span><span class="sxs-lookup"><span data-stu-id="747a1-151">Activate the following two child flows first before you activate the Partner Center to CRM flow.</span></span>
      - <span data-ttu-id="747a1-152">Partner Center para CRM-Helper (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="747a1-152">Partner Center to CRM - Helper (Insider Preview)</span></span>
      - <span data-ttu-id="747a1-153">Partner Center Microsoft co-vender atualizações de referência para CRM (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="747a1-153">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span></span>

4. <span data-ttu-id="747a1-154">O que você deve fazer quando não é possível adicionar conexões ao fluxo ao tentar editar o fluxo?</span><span class="sxs-lookup"><span data-stu-id="747a1-154">What should you do when you aren't able to add connections to the flow when you try to edit the flow?</span></span>

<span data-ttu-id="747a1-155">Você adiciona conexões ao fluxo enquanto o fluxo está em execução e adiciona a cada fluxo separadamente.</span><span class="sxs-lookup"><span data-stu-id="747a1-155">You add connections to the flow while the flow is running, and you add to each flow separately.</span></span>  <span data-ttu-id="747a1-156">Se a caixa de diálogo para adicionar conexões não abrir automaticamente ao editar o fluxo, você poderá editar cada uma das etapas e as subetapas dos fluxos individualmente.</span><span class="sxs-lookup"><span data-stu-id="747a1-156">If the dialog to add connections doesn't open up automatically while editing the flow, then you can edit each of the steps and sub steps of the flows individually.</span></span>

- <span data-ttu-id="747a1-157">Selecione cada fluxo e edite-os individualmente.</span><span class="sxs-lookup"><span data-stu-id="747a1-157">Select each flow and edit them individually.</span></span>
- <span data-ttu-id="747a1-158">Expandir todas as etapas no fluxo</span><span class="sxs-lookup"><span data-stu-id="747a1-158">Expand all the steps in the flow</span></span> 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Mensagem de erro que requer entrada":::

- <span data-ttu-id="747a1-160">Selecione as etapas em que você verá um ícone de aviso solicitando a associação de conexões e adicionar conexões.</span><span class="sxs-lookup"><span data-stu-id="747a1-160">Select the steps where you see a warning icon asking to associate connections, and add connections.</span></span> 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Mensagem de erro que requer entrada":::


5. <span data-ttu-id="747a1-162">O que você deve fazer se os fluxos da solução covenda de conectores de referências não estiverem ativados?</span><span class="sxs-lookup"><span data-stu-id="747a1-162">What should you do if the flows of the Co-sell Referrals Connectors solution don’t turn on?</span></span>

<span data-ttu-id="747a1-163">a.</span><span class="sxs-lookup"><span data-stu-id="747a1-163">A.</span></span> <span data-ttu-id="747a1-164">Na energia automatizada, você precisará editar os fluxos na seguinte ordem e atualizá-los para usar as conexões corretas:</span><span class="sxs-lookup"><span data-stu-id="747a1-164">In Power Automate, you'll need to edit flows in the following order and update them to use the correct connections:</span></span>

- <span data-ttu-id="747a1-165">Registro do webhook do Partner Center (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="747a1-165">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="747a1-166">Criar referência de co-venda-Salesforce para o Partner Center (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="747a1-166">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="747a1-167">Partner Center Microsoft co-vender atualizações de referência para o Salesforce (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="747a1-167">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="747a1-168">Partner Center para Salesforce (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="747a1-168">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="747a1-169">Salesforce para o Partner Center (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="747a1-169">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="747a1-170">Oportunidade do Salesforce para o Partner Center (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="747a1-170">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="747a1-171">Salesforce Microsoft Solutions para Partner Center (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="747a1-171">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

 <span data-ttu-id="747a1-172">B.</span><span class="sxs-lookup"><span data-stu-id="747a1-172">B.</span></span> <span data-ttu-id="747a1-173">Para cada fluxo, selecione a opção **executar somente usuários** .</span><span class="sxs-lookup"><span data-stu-id="747a1-173">For each of flow, select **Run only users** option.</span></span> <span data-ttu-id="747a1-174">Selecione **usar conexão** em vez de **fornecido pelo usuário somente execução**.</span><span class="sxs-lookup"><span data-stu-id="747a1-174">Select **Use connection** instead of **Provided by run-only user**.</span></span>  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Mensagem de erro que requer entrada":::


<span data-ttu-id="747a1-176">C.</span><span class="sxs-lookup"><span data-stu-id="747a1-176">C.</span></span> <span data-ttu-id="747a1-177">Ative-os abaixo dos fluxos mencionados:</span><span class="sxs-lookup"><span data-stu-id="747a1-177">Activate these below mentioned flows:</span></span>

 - <span data-ttu-id="747a1-178">Partner Center Microsoft co-vender atualizações de referência para o Salesforce (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="747a1-178">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>

- <span data-ttu-id="747a1-179">Salesforce para o Partner Center (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="747a1-179">Salesforce to Partner Center (Insider Preview)</span></span>

    
<span data-ttu-id="747a1-180">D.</span><span class="sxs-lookup"><span data-stu-id="747a1-180">D.</span></span> <span data-ttu-id="747a1-181">Ative todos os fluxos restantes.</span><span class="sxs-lookup"><span data-stu-id="747a1-181">Activate all the remaining flows.</span></span>

<span data-ttu-id="747a1-182">E.</span><span class="sxs-lookup"><span data-stu-id="747a1-182">E.</span></span> <span data-ttu-id="747a1-183">Em registro de webhook do Flow Center de fluxo, selecione **executar**.</span><span class="sxs-lookup"><span data-stu-id="747a1-183">At flow Partner Center Webhook Registration, select **Run**.</span></span> <span data-ttu-id="747a1-184">Forneça a **URL http** da primeira ação no **Partner Center para** o fluxo do Salesforce.</span><span class="sxs-lookup"><span data-stu-id="747a1-184">Provide the **http url** from the first action in **Partner Center to Salesforce** flow.</span></span> <span data-ttu-id="747a1-185">Selecione todas as quatro opções em **eventos para registrar** e selecione **Sim** para substituir.</span><span class="sxs-lookup"><span data-stu-id="747a1-185">Select all four options under **Events to register** and select **yes** for Overwrite.</span></span>

## <a name="questions-and-answers-about-runmaintenance"></a><span data-ttu-id="747a1-186">Perguntas e respostas sobre a execução/manutenção</span><span class="sxs-lookup"><span data-stu-id="747a1-186">Questions and answers about Run/Maintenance</span></span>

1. <span data-ttu-id="747a1-187">Como solucionar problemas em caso de falhas durante a execução do fluxo de energia automatizada?</span><span class="sxs-lookup"><span data-stu-id="747a1-187">How do you troubleshoot in case of failures during Power Automate flow execution?</span></span>

<span data-ttu-id="747a1-188">Para garantir que seus fluxos de energia automatizada sejam executados conforme esperado e para solucionar falhas durante a execução, consulte [corrigir falhas de fluxo](/power-automate/fix-flow-failures).</span><span class="sxs-lookup"><span data-stu-id="747a1-188">To ensure that your Power Automate flows run as you expect and to troubleshoot failures during execution, refer to [Fix flow failures](/power-automate/fix-flow-failures).</span></span>

2. <span data-ttu-id="747a1-189">O que você deve fazer se vir as referências que não estão sincronizadas corretamente no ambiente do Partner Center ou CRM?</span><span class="sxs-lookup"><span data-stu-id="747a1-189">What should you do if you see referrals that aren't synchronized properly in Partner Center or CRM environment?</span></span>
 
<span data-ttu-id="747a1-190">Para determinar o status da sincronização de referência, selecione **auditoria**.</span><span class="sxs-lookup"><span data-stu-id="747a1-190">To determine the status of referral synchronization, select **Audit**.</span></span> 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Mensagem de erro que requer entrada":::

<span data-ttu-id="747a1-192">Certifique-se de que as seguintes condições sejam atendidas:</span><span class="sxs-lookup"><span data-stu-id="747a1-192">Ensure that the following conditions are met:</span></span>

- <span data-ttu-id="747a1-193">A ID da solução é fornecida como parte da oportunidade.</span><span class="sxs-lookup"><span data-stu-id="747a1-193">Solution id is provided as part of the opportunity.</span></span>

- <span data-ttu-id="747a1-194">O código do país de duas letras é necessário.</span><span class="sxs-lookup"><span data-stu-id="747a1-194">Two letter country code is required.</span></span>

- <span data-ttu-id="747a1-195">Quando a ajuda da Microsoft é selecionada para a oportunidade, as informações de contato do cliente são necessárias.</span><span class="sxs-lookup"><span data-stu-id="747a1-195">When help from Microsoft is selected for the opportunity, customer contact information is required.</span></span>

3. <span data-ttu-id="747a1-196">Como garantir que uma referência seja sincronizada bidirecionalmente?</span><span class="sxs-lookup"><span data-stu-id="747a1-196">How to ensure that a referral will synchronize bi-directionally?</span></span>

<span data-ttu-id="747a1-197">Execute as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="747a1-197">Do the following steps:</span></span>

- <span data-ttu-id="747a1-198">Os vendedores do parceiro precisam garantir que tenham habilitado a opção **sincronizar com o Partner Center** na seção CRM.</span><span class="sxs-lookup"><span data-stu-id="747a1-198">Partner sellers need to ensure that they have enabled **Sync with Partner Center** option in the CRM section.</span></span>

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Mensagem de erro que requer entrada":::

- <span data-ttu-id="747a1-200">Os vendedores precisam fornecer receita e data de fechamento ao qualificar um cliente potencial.</span><span class="sxs-lookup"><span data-stu-id="747a1-200">Sellers need to provide revenue and closing date when qualifying a lead.</span></span>

- <span data-ttu-id="747a1-201">Se a ID do CRM for fornecida no estágio **criar** ou **Atualizar** da oportunidade de venda conjunta, mas uma oportunidade de cliente potencial com essa ID não for encontrada no CRM, a atualização ou criação será ignorada.</span><span class="sxs-lookup"><span data-stu-id="747a1-201">If CRM ID is provided in the **create** or **update** stage of co-sell opportunity, but a lead opportunity with that ID is not found in CRM, then update or create will be ignored.</span></span>

- <span data-ttu-id="747a1-202">Verifique se o campo moeda de referência está configurado no ambiente do Salesforce.</span><span class="sxs-lookup"><span data-stu-id="747a1-202">Ensure that referral currency field is configured on Salesforce environment.</span></span> 

4. <span data-ttu-id="747a1-203">O que você deve fazer se o conector for desconectado e você perder uma sincronização de referência.</span><span class="sxs-lookup"><span data-stu-id="747a1-203">What should you do if the connector gets disconnected and you miss a referral synchronization.</span></span> 

<span data-ttu-id="747a1-204">A seguir estão algumas das opções que você pode experimentar:</span><span class="sxs-lookup"><span data-stu-id="747a1-204">Following are few of the options that you can try out:</span></span>

- <span data-ttu-id="747a1-205">Verifique se o nome de usuário ou a senha expiraram para os usuários do Partner Center com funções de administrador de referência.</span><span class="sxs-lookup"><span data-stu-id="747a1-205">Check whether username or password has expired for the Partner Center user with referral admin roles.</span></span>

- <span data-ttu-id="747a1-206">Você pode ir para a oportunidade não sincronizada, fazer uma atualização secundária e observar se a referência foi sincronizada.</span><span class="sxs-lookup"><span data-stu-id="747a1-206">You can go to the un-synchronized opportunity, make a minor update, and observe whether the referral has synchronized.</span></span>

- <span data-ttu-id="747a1-207">Se os fluxos tiverem sido executados e falharem, selecione o fluxo e envie novamente a execução que falhou.</span><span class="sxs-lookup"><span data-stu-id="747a1-207">If the flows have run and failed, then select the flow and re-submit the run which has failed.</span></span>

5. <span data-ttu-id="747a1-208">O que você deve fazer quando obtiver erros de acesso negado?</span><span class="sxs-lookup"><span data-stu-id="747a1-208">What should you do when you get access denied errors?</span></span>

<span data-ttu-id="747a1-209">Verifique se as funções apropriadas existem</span><span class="sxs-lookup"><span data-stu-id="747a1-209">Make sure the appropriate roles exist</span></span>

- <span data-ttu-id="747a1-210">Função de administrador de referência para o vendedor do Partner Center</span><span class="sxs-lookup"><span data-stu-id="747a1-210">Referral Administrator role for Partner Center seller</span></span> 
 
- <span data-ttu-id="747a1-211">Função Administrador do sistema ou personalizador do sistema na sua instância do CRM</span><span class="sxs-lookup"><span data-stu-id="747a1-211">System Administrator or System Customizer role on your CRM instance</span></span>

- <span data-ttu-id="747a1-212">Verifique se a energia automatizar os logs de usuário da conta de fluxo em https://flow.microsoft.com pelo menos uma vez antes</span><span class="sxs-lookup"><span data-stu-id="747a1-212">Ensure that the Power Automate flow account user logs into https://flow.microsoft.com at least once beforehand</span></span>

6. <span data-ttu-id="747a1-213">Se você vir que o **código do país da conta do cliente** está ausente durante a criação de uma oportunidade de venda conjunta, o que você deve fazer?</span><span class="sxs-lookup"><span data-stu-id="747a1-213">If you see that **Customer account country code** is missing while creating a Co-sell opportunity, what should you do?</span></span>

<span data-ttu-id="747a1-214">Você precisará adicionar o código do país ISO de duas letras à conta do cliente no CRM.</span><span class="sxs-lookup"><span data-stu-id="747a1-214">You will need to add the ISO two-letter country code to the Customer account in CRM.</span></span>

7. <span data-ttu-id="747a1-215">O que você deve fazer se você vir o erro de que a **ID da solução é necessária** ao criar uma oportunidade de venda conjunta?</span><span class="sxs-lookup"><span data-stu-id="747a1-215">What should you do if you see the error that **Solution ID is required** while creating a Co-sell opportunity?</span></span>

<span data-ttu-id="747a1-216">Para criar uma referência de venda conjunta, você precisa de uma solução de venda pronta da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="747a1-216">In order to create a co-sell referral, you need a Microsoft co-sell ready solution.</span></span> 

8. <span data-ttu-id="747a1-217">O que você deve fazer ao ver as oportunidades de venda conjuntas criadas no Partner Center que não são sincronizadas com o CRM, mesmo que não haja nenhum erro de fluxo:</span><span class="sxs-lookup"><span data-stu-id="747a1-217">What should you do when you see Co-sell opportunities created in Partner Center that aren't synchronized to CRM even though there are no flow errors:</span></span>

<span data-ttu-id="747a1-218">Faça o seguinte:</span><span class="sxs-lookup"><span data-stu-id="747a1-218">Do the following:</span></span>

- <span data-ttu-id="747a1-219">Depois de criar um novo negócio de revenda no Partner Center, verifique se o Partner Center para o fluxo do Dynamics 365 é invocado (ele pode ser invocado várias vezes).</span><span class="sxs-lookup"><span data-stu-id="747a1-219">After you have created a new co-sell deal in Partner Center, check if Partner Center to Dynamics 365 flow gets invoked (it might get invoked multiple times).</span></span>

- <span data-ttu-id="747a1-220">Se o fluxo for invocado, verifique todos os fluxos invocados e identifique a execução do fluxo que atualizará o CRM.</span><span class="sxs-lookup"><span data-stu-id="747a1-220">If the flow gets invoked, check all invoked flows, and identify the flow run which would update the CRM.</span></span> <span data-ttu-id="747a1-221">Você pode seguir as ações e verificar se ele atualizou o CRM ou encontrou um problema.</span><span class="sxs-lookup"><span data-stu-id="747a1-221">You can follow the actions and verify if it did update the CRM or encountered a problem.</span></span>

- <span data-ttu-id="747a1-222">Verifique o *novo negócio*\* no Partner Center para ver se ele é preenchido com a ID do CRM.</span><span class="sxs-lookup"><span data-stu-id="747a1-222">Check *New deal*\* in Partner Center to see if it gets populated with CRM ID.</span></span>

- <span data-ttu-id="747a1-223">Certifique-se de que o negócio não seja fechado acidentalmente como "ganho" ou "perdido" no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="747a1-223">Make sure that the deal is not accidentally closed as “Won” or “Lost” in Partner Center.</span></span>

## <a name="next-steps"></a><span data-ttu-id="747a1-224">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="747a1-224">Next steps</span></span>

- [<span data-ttu-id="747a1-225">Gerenciar clientes potenciais</span><span class="sxs-lookup"><span data-stu-id="747a1-225">Manage leads</span></span>](manage-leads.md)
 
- [<span data-ttu-id="747a1-226">Gerenciar oportunidades de venda conjunta</span><span class="sxs-lookup"><span data-stu-id="747a1-226">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)