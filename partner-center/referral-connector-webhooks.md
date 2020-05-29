---
title: Usar WebHooks para obter eventos de alteração de recurso
ms.topic: article
ms.date: 05/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Usar as APIs de webhook para descobrir quando as alterações de recursos de referências ocorrem
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: referências, API de webhook, eventos de alteração de recursos
ms.localizationpriority: medium
ms.openlocfilehash: 4e1eb2e9bd8ceb4f8c4bf43684305504c8594e5c
ms.sourcegitcommit: c13723216761e60d2b37596efc71f5fdecb30be1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/28/2020
ms.locfileid: "84145080"
---
# <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="f17ab-104">Usar APIs de webhook para registrar eventos de alteração de recurso</span><span class="sxs-lookup"><span data-stu-id="f17ab-104">Use Webhook APIs to register for resource change events</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="f17ab-105">Funções apropriadas</span><span class="sxs-lookup"><span data-stu-id="f17ab-105">Appropriate roles</span></span>

- <span data-ttu-id="f17ab-106">Administrador de indicações</span><span class="sxs-lookup"><span data-stu-id="f17ab-106">Referrals admin</span></span>
- <span data-ttu-id="f17ab-107">Administrador do sistema ou personalizador do sistema para Dynamics 365 CRM ou Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="f17ab-107">System admin or System customizer for Dynamics 365 CRM or Salesforce CRM</span></span>


<span data-ttu-id="f17ab-108">As APIs de webhook do Partner Center permitem que você se registre em eventos de alteração de recursos.</span><span class="sxs-lookup"><span data-stu-id="f17ab-108">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="f17ab-109">Esses eventos de alteração são enviados para a URL como postagens HTTP.</span><span class="sxs-lookup"><span data-stu-id="f17ab-109">These change events are sent to your url as HTTP posts.</span></span>

>[!NOTE]
><span data-ttu-id="f17ab-110">Este tópico explica as APIs de webhook para o Dynamics 365 CRM e o Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="f17ab-110">This topic explains Webhook APIs for both Dynamics 365 CRM and Salesforce CRM.</span></span>

1. <span data-ttu-id="f17ab-111">Para registrar sua URL, selecione o **registro do webhook do Partner Center (insider Preview)** fluxo automatizado de energia.</span><span class="sxs-lookup"><span data-stu-id="f17ab-111">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="f17ab-112">Adicionar conexões para (a) Usuário do Partner Center com as referências credenciais de administrador (b.) Eventos do Partner Center conforme realçado abaixo</span><span class="sxs-lookup"><span data-stu-id="f17ab-112">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

![Gatilho](images/cosellconnectors/triggerflow.png)

3. <span data-ttu-id="f17ab-114">Ao fazer essas atualizações, você verá</span><span class="sxs-lookup"><span data-stu-id="f17ab-114">When you make these updates, you will see</span></span>

![Webhooks](images/cosellconnectors/webhook1.png)

4. <span data-ttu-id="f17ab-116">Salve as alterações e selecione **Ativar**.</span><span class="sxs-lookup"><span data-stu-id="f17ab-116">Save your changes and select **Turn on**.</span></span> 

<span data-ttu-id="f17ab-117">Para permitir que os WebHooks do Partner Center escutem as alterações de evento nos objetos de referência de covenda/independente de IP no Partner Center e em sistemas de CRM, execute as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="f17ab-117">To enable Partner Center webhooks to listen to event changes in the IP Co-sell/independent referral objects in Partner Center and CRM systems perform the following steps:</span></span>

5. <span data-ttu-id="f17ab-118">Selecione **Partner Center para Dynamics 365 (insider Preview)** ou **Partner Center para Salesforce (insider Preview)**.</span><span class="sxs-lookup"><span data-stu-id="f17ab-118">Select **Partner Center to Dynamics 365 (Insider Preview)** or **Partner Center to Salesforce (Insider Preview)**.</span></span>

6. <span data-ttu-id="f17ab-119">Selecione o ícone **Editar** e selecione **quando uma solicitação HTTP é recebida**.</span><span class="sxs-lookup"><span data-stu-id="f17ab-119">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="f17ab-120">Selecione o ícone de **cópia** para copiar a URL de postagem http fornecida.</span><span class="sxs-lookup"><span data-stu-id="f17ab-120">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

![Copiar URL](images/cosellconnectors/copyurl.png)

8. <span data-ttu-id="f17ab-122">Agora, selecione o fluxo "registro do webhook do Partner Center (insider Preview)" automatizar fluxos de energia e selecione **executar**.</span><span class="sxs-lookup"><span data-stu-id="f17ab-122">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="f17ab-123">Verifique se a janela "executar fluxo" é aberta no painel direito e clique em **continuar**.</span><span class="sxs-lookup"><span data-stu-id="f17ab-123">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="f17ab-124">Insira os seguintes detalhes:</span><span class="sxs-lookup"><span data-stu-id="f17ab-124">Enter the following details:</span></span> 

    <span data-ttu-id="f17ab-125">a.</span><span class="sxs-lookup"><span data-stu-id="f17ab-125">a.</span></span> <span data-ttu-id="f17ab-126">**Ponto de extremidade de gatilho http**: URL copiada da etapa anterior</span><span class="sxs-lookup"><span data-stu-id="f17ab-126">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    <span data-ttu-id="f17ab-127">b.</span><span class="sxs-lookup"><span data-stu-id="f17ab-127">b.</span></span> <span data-ttu-id="f17ab-128">**Eventos a serem registrados**: "referência criada" e "referência atualizada"</span><span class="sxs-lookup"><span data-stu-id="f17ab-128">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    <span data-ttu-id="f17ab-129">c.</span><span class="sxs-lookup"><span data-stu-id="f17ab-129">c.</span></span> <span data-ttu-id="f17ab-130">**Substituir pontos de extremidade de gatilho existentes, se presente**: Sim (isso substitui todos os pontos de extremidade existentes.)</span><span class="sxs-lookup"><span data-stu-id="f17ab-130">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

<span data-ttu-id="f17ab-131">O webhook agora pode escutar alterações (criar e atualizar eventos).</span><span class="sxs-lookup"><span data-stu-id="f17ab-131">The webhook can now listen to changes (create and update events).</span></span> 

11. <span data-ttu-id="f17ab-132">Selecione **executar** e, em seguida, selecione **concluído.**</span><span class="sxs-lookup"><span data-stu-id="f17ab-132">Select **Run** and then select **Done.**</span></span>

 ## <a name="customize-synchronization-steps"></a><span data-ttu-id="f17ab-133">Personalizar etapas de sincronização</span><span class="sxs-lookup"><span data-stu-id="f17ab-133">Customize synchronization steps</span></span>

<span data-ttu-id="f17ab-134">Quando as referências de venda cruzada são sincronizadas entre o Partner Center e o sistema CRM, os campos sincronizados no PC do Partner Center são listados aqui.</span><span class="sxs-lookup"><span data-stu-id="f17ab-134">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="f17ab-135">Geralmente, os sistemas CRM são altamente personalizados.</span><span class="sxs-lookup"><span data-stu-id="f17ab-135">Often CRM systems are highly customized.</span></span> <span data-ttu-id="f17ab-136">Você pode personalizar os fluxos de energia automatizada.</span><span class="sxs-lookup"><span data-stu-id="f17ab-136">You can customize the Power Automate flows.</span></span> <span data-ttu-id="f17ab-137">Siga o guia de mapeamento de campo e, se necessário, faça as alterações apropriadas nas etapas de fluxos de energia automatizar.</span><span class="sxs-lookup"><span data-stu-id="f17ab-137">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="f17ab-138">Os mapeamentos do Microsoft Partner Center para CRM são fornecidos, mas com base no seu ambiente de CRM, você pode optar por personalizar ainda mais os campos.</span><span class="sxs-lookup"><span data-stu-id="f17ab-138">Microsoft Partner Center to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="f17ab-139">Várias etapas de cada um dos fluxos de energia automatizada podem ser personalizadas com base em suas necessidades.</span><span class="sxs-lookup"><span data-stu-id="f17ab-139">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="f17ab-140">Veja a seguir exemplos de personalizações disponíveis:</span><span class="sxs-lookup"><span data-stu-id="f17ab-140">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="f17ab-141">Para personalizar os campos de criação ou atualização de eventos no Partner Center para a sincronização de referência do CRM:</span><span class="sxs-lookup"><span data-stu-id="f17ab-141">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="f17ab-142">a.</span><span class="sxs-lookup"><span data-stu-id="f17ab-142">a.</span></span> <span data-ttu-id="f17ab-143">Selecione Partner Center para Dynamics 365 (insider Preview) ou Partner Center para Salesforce (insider Preview).</span><span class="sxs-lookup"><span data-stu-id="f17ab-143">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

    <span data-ttu-id="f17ab-144">b.</span><span class="sxs-lookup"><span data-stu-id="f17ab-144">b.</span></span> <span data-ttu-id="f17ab-145">Selecione **Editar** para editar/personalizar o fluxo de automatização de energia.</span><span class="sxs-lookup"><span data-stu-id="f17ab-145">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="f17ab-146">c.</span><span class="sxs-lookup"><span data-stu-id="f17ab-146">c.</span></span> <span data-ttu-id="f17ab-147">Selecione **(escopo) sincronizar o cliente potencial ou a oportunidade**.</span><span class="sxs-lookup"><span data-stu-id="f17ab-147">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="f17ab-148">Para personalizar mapeamentos de campo de CRM (com base no guia mapeamentos de campo) para criar eventos, selecione **se for nova oportunidade compartilhada e, em seguida,**.</span><span class="sxs-lookup"><span data-stu-id="f17ab-148">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="f17ab-149">Selecione a subetapa **se sim** e, em seguida, expanda **criando uma nova oportunidade no CRM**.</span><span class="sxs-lookup"><span data-stu-id="f17ab-149">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="f17ab-150">Você pode editar os mapeamentos nesta seção usando o guia de mapeamento de campos.</span><span class="sxs-lookup"><span data-stu-id="f17ab-150">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="f17ab-151">d.</span><span class="sxs-lookup"><span data-stu-id="f17ab-151">d.</span></span> <span data-ttu-id="f17ab-152">Para personalizar os mapeamentos de campo do CRM (com base no guia mapeamentos de campo) para eventos de atualização, clique na etapa "(escopo) sincronizar o cliente potencial ou a oportunidade".</span><span class="sxs-lookup"><span data-stu-id="f17ab-152">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="f17ab-153">e.</span><span class="sxs-lookup"><span data-stu-id="f17ab-153">e.</span></span> <span data-ttu-id="f17ab-154">Selecione **se for uma atualização para uma oportunidade e, em seguida,**.</span><span class="sxs-lookup"><span data-stu-id="f17ab-154">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="f17ab-155">Selecione a subetapa **se sim** e, em seguida, expanda **se a diferença entre os objetos de oportunidade no Partner Center e no CRM, em seguida**.</span><span class="sxs-lookup"><span data-stu-id="f17ab-155">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

    <span data-ttu-id="f17ab-156">f.</span><span class="sxs-lookup"><span data-stu-id="f17ab-156">f.</span></span> <span data-ttu-id="f17ab-157">Selecione **se sim** seguido de **Atualizar oportunidade existente**</span><span class="sxs-lookup"><span data-stu-id="f17ab-157">Select **If yes** followed with **Update existing opportunity**</span></span>
       
3. <span data-ttu-id="f17ab-158">Para personalizar os campos de sincronização de referência do CRM para PC para eventos de atualização:</span><span class="sxs-lookup"><span data-stu-id="f17ab-158">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="f17ab-159">a.</span><span class="sxs-lookup"><span data-stu-id="f17ab-159">a.</span></span> <span data-ttu-id="f17ab-160">Selecione **Editar** para editar/personalizar o fluxo de automatização de energia.</span><span class="sxs-lookup"><span data-stu-id="f17ab-160">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="f17ab-161">b.</span><span class="sxs-lookup"><span data-stu-id="f17ab-161">b.</span></span> <span data-ttu-id="f17ab-162">Selecione **(escopo) sincronizar a oportunidade**.</span><span class="sxs-lookup"><span data-stu-id="f17ab-162">Select **(Scope) Synchronize the opportunity**.</span></span>

    <span data-ttu-id="f17ab-163">c.</span><span class="sxs-lookup"><span data-stu-id="f17ab-163">c.</span></span> <span data-ttu-id="f17ab-164">Para personalizar os mapeamentos de campo do CRM (com base no guia mapeamentos de campo) para eventos de atualização, selecione **se houver diferença entre os objetos Lead no Partner Center e CRM, em seguida**.</span><span class="sxs-lookup"><span data-stu-id="f17ab-164">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span> 

    <span data-ttu-id="f17ab-165">d.</span><span class="sxs-lookup"><span data-stu-id="f17ab-165">d.</span></span> <span data-ttu-id="f17ab-166">Selecione a subetapa **se sim** e, em seguida, expanda a etapa **atualizar uma referência com dados de oportunidade**.</span><span class="sxs-lookup"><span data-stu-id="f17ab-166">Select the substep **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

<span data-ttu-id="f17ab-167">Você pode editar os mapeamentos nesta seção com base no guia de mapeamento de campos.</span><span class="sxs-lookup"><span data-stu-id="f17ab-167">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="f17ab-168">Para personalizar os campos para a sincronização de referência do CRM para PC para criar eventos?</span><span class="sxs-lookup"><span data-stu-id="f17ab-168">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="f17ab-169">a.</span><span class="sxs-lookup"><span data-stu-id="f17ab-169">a.</span></span> <span data-ttu-id="f17ab-170">Selecione **Editar** para editar/personalizar o fluxo de automatização de energia.</span><span class="sxs-lookup"><span data-stu-id="f17ab-170">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="f17ab-171">b.</span><span class="sxs-lookup"><span data-stu-id="f17ab-171">b.</span></span> <span data-ttu-id="f17ab-172">Selecione **(escopo) sincronizando referências.**</span><span class="sxs-lookup"><span data-stu-id="f17ab-172">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="f17ab-173">c.</span><span class="sxs-lookup"><span data-stu-id="f17ab-173">c.</span></span> <span data-ttu-id="f17ab-174">Para personalizar mapeamentos de campo de CRM (com base no guia mapeamentos de campo) para criar eventos, selecione **criar referência da Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="f17ab-174">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span> 

<span data-ttu-id="f17ab-175">Você pode editar os mapeamentos nesta seção com base no guia de mapeamento de campos.</span><span class="sxs-lookup"><span data-stu-id="f17ab-175">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="f17ab-176">Sincronização de referência de cooperação bidirecional de ponta a ponta</span><span class="sxs-lookup"><span data-stu-id="f17ab-176">End-to-End Bi-directional Co-sell Referral Synchronization</span></span>

<span data-ttu-id="f17ab-177">Depois de instalar, configurar e personalizar a solução de automatização de energia, você pode testar a sincronização de referências de venda entre o Dynamics 365 ou o Salesforce e o Partner Center.</span><span class="sxs-lookup"><span data-stu-id="f17ab-177">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 or Salesforce and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="f17ab-178">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f17ab-178">Pre-requisites</span></span>

<span data-ttu-id="f17ab-179">Para sincronizar as referências no Partner Center e no Dynamics 365 CRM ou no Partner Center e no Salesforce CRM, a solução de automatização de energia precisa demarcar claramente os campos de referência específicos da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f17ab-179">To synchronize the referrals across Partner Center and Dynamics 365 CRM or across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="f17ab-180">Isso fornece às suas equipes do vendedor a capacidade de decidir quais referências eles desejam compartilhar com a Microsoft para fazer a venda.</span><span class="sxs-lookup"><span data-stu-id="f17ab-180">This provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="f17ab-181">Um conjunto de campos personalizados está disponível como parte da sincronização de referências do Partner Center para a entidade **oportunidade** de solução do Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="f17ab-181">A set of custom fields is available as part of Partner Center Referrals Synchronization for Dynamics 365 solution **Opportunity** entity.</span></span> <span data-ttu-id="f17ab-182">Um usuário administrador de CRM precisará criar uma seção de CRM separada com os campos personalizados de **oportunidade** .</span><span class="sxs-lookup"><span data-stu-id="f17ab-182">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="f17ab-183">Os campos personalizados a seguir devem fazer parte da seção CRM:</span><span class="sxs-lookup"><span data-stu-id="f17ab-183">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="f17ab-184">**Sincronizar com o Partner Center**: se deseja sincronizar a oportunidade com o Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="f17ab-184">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="f17ab-185">**Identificador de referência**: um campo de identificador somente leitura para a referência do Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="f17ab-185">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="f17ab-186">**Link de referência**: um link somente leitura para a referência no Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="f17ab-186">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="f17ab-187">**Como a Microsoft pode ajudar?**: ajuda necessária da Microsoft para a referência</span><span class="sxs-lookup"><span data-stu-id="f17ab-187">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="f17ab-188">**Produtos**: lista de produtos associados a esta oportunidade</span><span class="sxs-lookup"><span data-stu-id="f17ab-188">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="f17ab-189">**Auditoria**: uma trilha de auditoria somente leitura para sincronização com as referências do Partner Center</span><span class="sxs-lookup"><span data-stu-id="f17ab-189">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="f17ab-190">EXEMPLOS</span><span class="sxs-lookup"><span data-stu-id="f17ab-190">SCENARIOS:</span></span>

1. <span data-ttu-id="f17ab-191">Sincronização de referência quando a referência é criada ou atualizada no CRM e sincronizada no Partner Center:</span><span class="sxs-lookup"><span data-stu-id="f17ab-191">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

    <span data-ttu-id="f17ab-192">a.</span><span class="sxs-lookup"><span data-stu-id="f17ab-192">a.</span></span> <span data-ttu-id="f17ab-193">Entre no ambiente do Dynamics 365 CRM com o usuário que tem visibilidade na seção **oportunidade** do CRM.</span><span class="sxs-lookup"><span data-stu-id="f17ab-193">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

    <span data-ttu-id="f17ab-194">b.</span><span class="sxs-lookup"><span data-stu-id="f17ab-194">b.</span></span> <span data-ttu-id="f17ab-195">Verifique se a seção a seguir está presente quando você cria uma "nova oportunidade" no ambiente do Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="f17ab-195">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

   ![Oportunidade](images/cosellconnectors/opportunity.png)

    <span data-ttu-id="f17ab-197">c.</span><span class="sxs-lookup"><span data-stu-id="f17ab-197">c.</span></span> <span data-ttu-id="f17ab-198">Para sincronizar essa oportunidade com o Microsoft Partner Center, certifique-se de definir os seguintes campos no modo de exibição de cartão:</span><span class="sxs-lookup"><span data-stu-id="f17ab-198">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

    - <span data-ttu-id="f17ab-199">"Sincronizar com o Partner Center": Sim</span><span class="sxs-lookup"><span data-stu-id="f17ab-199">“Sync with Partner Center”: Yes</span></span>

    - <span data-ttu-id="f17ab-200">"Como a Microsoft pode ajudar?": selecione uma das seguintes opções:</span><span class="sxs-lookup"><span data-stu-id="f17ab-200">"How can Microsoft help?”: Select from the following:</span></span>

    ![Seleções de ajuda](images/cosellconnectors/help.png)

    - <span data-ttu-id="f17ab-202">Produtos: IDs de solução do produto</span><span class="sxs-lookup"><span data-stu-id="f17ab-202">Products: Solution IDs of the product</span></span>

    <span data-ttu-id="f17ab-203">d.</span><span class="sxs-lookup"><span data-stu-id="f17ab-203">d.</span></span> <span data-ttu-id="f17ab-204">Depois que a oportunidade for criada no Dynamics 365 com a opção **sincronizar com o Partner Center** definida como **Sim**, aguarde 10 minutos, entre em sua conta do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="f17ab-204">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="f17ab-205">Suas referências serão sincronizadas com o Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="f17ab-205">Your referrals will be synchronized with Dynamics 365.</span></span>

    <span data-ttu-id="f17ab-206">e.</span><span class="sxs-lookup"><span data-stu-id="f17ab-206">e.</span></span> <span data-ttu-id="f17ab-207">Consequentemente, para uma oportunidade que tenha a opção "sincronizar com o Partner Center" definida como "Sim", se você atualizar a oportunidade no Dynamics 365 CRM, as alterações serão sincronizadas em sua conta do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="f17ab-207">Consequently, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

    <span data-ttu-id="f17ab-208">f.</span><span class="sxs-lookup"><span data-stu-id="f17ab-208">f.</span></span> <span data-ttu-id="f17ab-209">As oportunidades sincronizadas com êxito com o Partner Center serão identificadas com ✔ ícone no Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="f17ab-209">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="f17ab-210">Sincronização de referência quando a referência é criada ou atualizada no Microsoft Partner Center e sincronizada no ambiente do Dynamics 365:</span><span class="sxs-lookup"><span data-stu-id="f17ab-210">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span> 

    <span data-ttu-id="f17ab-211">a.</span><span class="sxs-lookup"><span data-stu-id="f17ab-211">a.</span></span> <span data-ttu-id="f17ab-212">Entre no [painel](https://partner.microsoft.com/dashboard/home)do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="f17ab-212">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    <span data-ttu-id="f17ab-213">b.</span><span class="sxs-lookup"><span data-stu-id="f17ab-213">b.</span></span> <span data-ttu-id="f17ab-214">Selecione **referências** no menu à esquerda.</span><span class="sxs-lookup"><span data-stu-id="f17ab-214">Select **Referrals** from the left-hand menu.</span></span>

    <span data-ttu-id="f17ab-215">c.</span><span class="sxs-lookup"><span data-stu-id="f17ab-215">c.</span></span> <span data-ttu-id="f17ab-216">Crie uma nova referência de revenda do Partner Center clicando na opção "novo negócio".</span><span class="sxs-lookup"><span data-stu-id="f17ab-216">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

    <span data-ttu-id="f17ab-217">d.</span><span class="sxs-lookup"><span data-stu-id="f17ab-217">d.</span></span> <span data-ttu-id="f17ab-218">Entre no ambiente do Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="f17ab-218">Sign into your Dynamics 365 CRM environment.</span></span> 

    <span data-ttu-id="f17ab-219">e.</span><span class="sxs-lookup"><span data-stu-id="f17ab-219">e.</span></span> <span data-ttu-id="f17ab-220">Navegue até **oportunidades abertas**.</span><span class="sxs-lookup"><span data-stu-id="f17ab-220">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="f17ab-221">A referência criada no Microsoft Partner Center agora está sincronizada no Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="f17ab-221">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

    <span data-ttu-id="f17ab-222">f.</span><span class="sxs-lookup"><span data-stu-id="f17ab-222">f.</span></span> <span data-ttu-id="f17ab-223">Quando você seleciona uma referência sincronizada, os detalhes da exibição do cartão são preenchidos.</span><span class="sxs-lookup"><span data-stu-id="f17ab-223">When you select a synchronized referral, the card view details are populated.</span></span>

 ### <a name="next-steps"></a><span data-ttu-id="f17ab-224">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="f17ab-224">Next steps</span></span>

- [<span data-ttu-id="f17ab-225">Mais informações sobre a plataforma de automatização de energia da Microsoft?</span><span class="sxs-lookup"><span data-stu-id="f17ab-225">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/power-automate/)

- [<span data-ttu-id="f17ab-226">Eventos de webhook do Partner Center</span><span class="sxs-lookup"><span data-stu-id="f17ab-226">Partner Center webhook events</span></span>](https://docs.microsoft.com/partner-center/develop/partner-center-webhook-events)

- [<span data-ttu-id="f17ab-227">Gerenciar clientes potenciais</span><span class="sxs-lookup"><span data-stu-id="f17ab-227">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="f17ab-228">Gerenciar oportunidades de venda conjunta</span><span class="sxs-lookup"><span data-stu-id="f17ab-228">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
