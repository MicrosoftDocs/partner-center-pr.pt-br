---
title: Usar WebHooks para obter eventos de alteração de recurso
ms.topic: article
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Use as APIs de webhook do Partner Center para saber quando as alterações de recursos de referências ocorrem para o Dynamics 365 CRM ou o Salesforce CRM.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2335c06d9c410d44ed5f444574d9bc8fb3e48fc0
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2020
ms.locfileid: "86434015"
---
# <a name="use-webhook-apis-to-register-for-resource-change-events-for-dynamics-365-crm-and-salesforce-crm"></a><span data-ttu-id="9ef22-103">Usar APIs de webhook para registrar eventos de alteração de recursos do Dynamics 365 CRM e do Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="9ef22-103">Use Webhook APIs to register for resource change events for Dynamics 365 CRM and Salesforce CRM</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="9ef22-104">Funções apropriadas</span><span class="sxs-lookup"><span data-stu-id="9ef22-104">Appropriate roles</span></span>

- <span data-ttu-id="9ef22-105">Administrador de indicações</span><span class="sxs-lookup"><span data-stu-id="9ef22-105">Referrals admin</span></span>
- <span data-ttu-id="9ef22-106">Administrador do sistema ou personalizador do sistema para Dynamics 365 CRM ou Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="9ef22-106">System admin or System customizer for Dynamics 365 CRM or Salesforce CRM</span></span>

<span data-ttu-id="9ef22-107">As APIs de webhook do Partner Center permitem que você se registre em eventos de alteração de recursos.</span><span class="sxs-lookup"><span data-stu-id="9ef22-107">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="9ef22-108">Esses eventos de alteração são enviados para a URL como postagens HTTP.</span><span class="sxs-lookup"><span data-stu-id="9ef22-108">These change events are sent to your url as HTTP posts.</span></span>

>[!NOTE]
><span data-ttu-id="9ef22-109">Este tópico explica as APIs de webhook para o Dynamics 365 CRM e o Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="9ef22-109">This topic explains Webhook APIs for both Dynamics 365 CRM and Salesforce CRM.</span></span>

## <a name="configure-the-webhook"></a><span data-ttu-id="9ef22-110">Configurar o webhook</span><span class="sxs-lookup"><span data-stu-id="9ef22-110">Configure the webhook</span></span>

1. <span data-ttu-id="9ef22-111">Para registrar sua URL, selecione o **registro do webhook do Partner Center (insider Preview)** fluxo automatizado de energia.</span><span class="sxs-lookup"><span data-stu-id="9ef22-111">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="9ef22-112">Adicionar conexões para (a) Usuário do Partner Center com as referências credenciais de administrador (b.) Eventos do Partner Center conforme realçado abaixo</span><span class="sxs-lookup"><span data-stu-id="9ef22-112">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Gatilho":::

3. <span data-ttu-id="9ef22-114">Ao fazer essas atualizações, você verá</span><span class="sxs-lookup"><span data-stu-id="9ef22-114">When you make these updates, you will see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks":::

4. <span data-ttu-id="9ef22-116">Salve as alterações e selecione **Ativar**.</span><span class="sxs-lookup"><span data-stu-id="9ef22-116">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="9ef22-117">Para permitir que os WebHooks do Partner Center escutem as alterações de evento nos objetos de referência de covenda/independente de IP no Partner Center e em sistemas de CRM, execute as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="9ef22-117">To enable Partner Center webhooks to listen to event changes in the IP Co-sell/independent referral objects in Partner Center and CRM systems perform the following steps:</span></span>

5. <span data-ttu-id="9ef22-118">Selecione **Partner Center para Dynamics 365 (insider Preview)** ou **Partner Center para Salesforce (insider Preview)**.</span><span class="sxs-lookup"><span data-stu-id="9ef22-118">Select **Partner Center to Dynamics 365 (Insider Preview)** or **Partner Center to Salesforce (Insider Preview)**.</span></span>

6. <span data-ttu-id="9ef22-119">Selecione o ícone **Editar** e selecione **quando uma solicitação HTTP é recebida**.</span><span class="sxs-lookup"><span data-stu-id="9ef22-119">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="9ef22-120">Selecione o ícone de **cópia** para copiar a URL de postagem http fornecida.</span><span class="sxs-lookup"><span data-stu-id="9ef22-120">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="Copiar URL":::

8. <span data-ttu-id="9ef22-122">Agora, selecione o fluxo "registro do webhook do Partner Center (insider Preview)" automatizar fluxos de energia e selecione **executar**.</span><span class="sxs-lookup"><span data-stu-id="9ef22-122">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="9ef22-123">Verifique se a janela "executar fluxo" é aberta no painel direito e clique em **continuar**.</span><span class="sxs-lookup"><span data-stu-id="9ef22-123">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="9ef22-124">Insira os seguintes detalhes:</span><span class="sxs-lookup"><span data-stu-id="9ef22-124">Enter the following details:</span></span>

    1. <span data-ttu-id="9ef22-125">**Ponto de extremidade de gatilho http**: URL copiada da etapa anterior</span><span class="sxs-lookup"><span data-stu-id="9ef22-125">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="9ef22-126">**Eventos a serem registrados**: "referência criada" e "referência atualizada"</span><span class="sxs-lookup"><span data-stu-id="9ef22-126">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    3. <span data-ttu-id="9ef22-127">**Substituir pontos de extremidade de gatilho existentes, se presente**: Sim (isso substitui todos os pontos de extremidade existentes.)</span><span class="sxs-lookup"><span data-stu-id="9ef22-127">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

    <span data-ttu-id="9ef22-128">O webhook agora pode escutar alterações (criar e atualizar eventos).</span><span class="sxs-lookup"><span data-stu-id="9ef22-128">The webhook can now listen to changes (create and update events).</span></span>

11. <span data-ttu-id="9ef22-129">Selecione **executar** e, em seguida, selecione **concluído.**</span><span class="sxs-lookup"><span data-stu-id="9ef22-129">Select **Run** and then select **Done.**</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="9ef22-130">Personalizar etapas de sincronização</span><span class="sxs-lookup"><span data-stu-id="9ef22-130">Customize synchronization steps</span></span>

<span data-ttu-id="9ef22-131">Quando as referências de venda cruzada são sincronizadas entre o Partner Center e o sistema CRM, os campos sincronizados no PC do Partner Center são listados aqui.</span><span class="sxs-lookup"><span data-stu-id="9ef22-131">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="9ef22-132">Geralmente, os sistemas CRM são altamente personalizados.</span><span class="sxs-lookup"><span data-stu-id="9ef22-132">Often CRM systems are highly customized.</span></span> <span data-ttu-id="9ef22-133">Você pode personalizar os fluxos de energia automatizada.</span><span class="sxs-lookup"><span data-stu-id="9ef22-133">You can customize the Power Automate flows.</span></span> <span data-ttu-id="9ef22-134">Siga o guia de mapeamento de campo e, se necessário, faça as alterações apropriadas nas etapas de fluxos de energia automatizar.</span><span class="sxs-lookup"><span data-stu-id="9ef22-134">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="9ef22-135">Os mapeamentos do Microsoft Partner Center para CRM são fornecidos, mas com base no seu ambiente de CRM, você pode optar por personalizar ainda mais os campos.</span><span class="sxs-lookup"><span data-stu-id="9ef22-135">Microsoft Partner Center to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="9ef22-136">Várias etapas de cada um dos fluxos de energia automatizada podem ser personalizadas com base em suas necessidades.</span><span class="sxs-lookup"><span data-stu-id="9ef22-136">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="9ef22-137">Veja a seguir exemplos de personalizações disponíveis:</span><span class="sxs-lookup"><span data-stu-id="9ef22-137">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="9ef22-138">Para personalizar os campos de criação ou atualização de eventos no Partner Center para a sincronização de referência do CRM:</span><span class="sxs-lookup"><span data-stu-id="9ef22-138">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="9ef22-139">Selecione Partner Center para Dynamics 365 (insider Preview) ou Partner Center para Salesforce (insider Preview).</span><span class="sxs-lookup"><span data-stu-id="9ef22-139">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

   2. <span data-ttu-id="9ef22-140">Selecione **Editar** para editar/personalizar o fluxo de automatização de energia.</span><span class="sxs-lookup"><span data-stu-id="9ef22-140">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="9ef22-141">Selecione **(escopo) sincronizar o cliente potencial ou a oportunidade**.</span><span class="sxs-lookup"><span data-stu-id="9ef22-141">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="9ef22-142">Para personalizar mapeamentos de campo de CRM (com base no guia mapeamentos de campo) para criar eventos, selecione **se for nova oportunidade compartilhada e, em seguida,**.</span><span class="sxs-lookup"><span data-stu-id="9ef22-142">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="9ef22-143">Selecione a subetapa **se sim** e, em seguida, expanda **criando uma nova oportunidade no CRM**.</span><span class="sxs-lookup"><span data-stu-id="9ef22-143">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="9ef22-144">Você pode editar os mapeamentos nesta seção usando o guia de mapeamento de campos.</span><span class="sxs-lookup"><span data-stu-id="9ef22-144">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="9ef22-145">Para personalizar os mapeamentos de campo do CRM (com base no guia mapeamentos de campo) para eventos de atualização, clique na etapa "(escopo) sincronizar o cliente potencial ou a oportunidade".</span><span class="sxs-lookup"><span data-stu-id="9ef22-145">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

   2. <span data-ttu-id="9ef22-146">Selecione **se for uma atualização para uma oportunidade e, em seguida,**.</span><span class="sxs-lookup"><span data-stu-id="9ef22-146">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="9ef22-147">Selecione a subetapa **se sim** e, em seguida, expanda **se a diferença entre os objetos de oportunidade no Partner Center e no CRM, em seguida**.</span><span class="sxs-lookup"><span data-stu-id="9ef22-147">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="9ef22-148">Selecione **se sim** seguido de **Atualizar oportunidade existente**</span><span class="sxs-lookup"><span data-stu-id="9ef22-148">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="9ef22-149">Para personalizar os campos de sincronização de referência do CRM para PC para eventos de atualização:</span><span class="sxs-lookup"><span data-stu-id="9ef22-149">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="9ef22-150">Selecione **Editar** para editar/personalizar o fluxo de automatização de energia.</span><span class="sxs-lookup"><span data-stu-id="9ef22-150">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="9ef22-151">Selecione **(escopo) sincronizar a oportunidade**.</span><span class="sxs-lookup"><span data-stu-id="9ef22-151">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="9ef22-152">Para personalizar os mapeamentos de campo do CRM (com base no guia mapeamentos de campo) para eventos de atualização, selecione **se houver diferença entre os objetos Lead no Partner Center e CRM, em seguida**.</span><span class="sxs-lookup"><span data-stu-id="9ef22-152">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="9ef22-153">Selecione a subetapa **se sim** e, em seguida, expanda a etapa **atualizar uma referência com dados de oportunidade**.</span><span class="sxs-lookup"><span data-stu-id="9ef22-153">Select the substep **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="9ef22-154">Você pode editar os mapeamentos nesta seção com base no guia de mapeamento de campos.</span><span class="sxs-lookup"><span data-stu-id="9ef22-154">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="9ef22-155">Para personalizar os campos para a sincronização de referência do CRM para PC para criar eventos?</span><span class="sxs-lookup"><span data-stu-id="9ef22-155">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="9ef22-156">Selecione **Editar** para editar/personalizar o fluxo de automatização de energia.</span><span class="sxs-lookup"><span data-stu-id="9ef22-156">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="9ef22-157">Selecione **(escopo) sincronizando referências.**</span><span class="sxs-lookup"><span data-stu-id="9ef22-157">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="9ef22-158">Para personalizar mapeamentos de campo de CRM (com base no guia mapeamentos de campo) para criar eventos, selecione **criar referência da Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="9ef22-158">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="9ef22-159">Você pode editar os mapeamentos nesta seção com base no guia de mapeamento de campos.</span><span class="sxs-lookup"><span data-stu-id="9ef22-159">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="9ef22-160">Sincronização de referência de cooperação bidirecional de ponta a ponta</span><span class="sxs-lookup"><span data-stu-id="9ef22-160">End-to-End Bi-directional Co-sell Referral Synchronization</span></span>

<span data-ttu-id="9ef22-161">Depois de instalar, configurar e personalizar a solução de automatização de energia, você pode testar a sincronização de referências de venda entre o Dynamics 365 ou o Salesforce e o Partner Center.</span><span class="sxs-lookup"><span data-stu-id="9ef22-161">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 or Salesforce and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="9ef22-162">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9ef22-162">Pre-requisites</span></span>

<span data-ttu-id="9ef22-163">Para sincronizar as referências no Partner Center e no Dynamics 365 CRM ou no Partner Center e no Salesforce CRM, a solução de automatização de energia precisa demarcar claramente os campos de referência específicos da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="9ef22-163">To synchronize the referrals across Partner Center and Dynamics 365 CRM or across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="9ef22-164">Isso fornece às suas equipes do vendedor a capacidade de decidir quais referências eles desejam compartilhar com a Microsoft para fazer a venda.</span><span class="sxs-lookup"><span data-stu-id="9ef22-164">This provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="9ef22-165">Um conjunto de campos personalizados está disponível como parte da sincronização de referências do Partner Center para a entidade **oportunidade** de solução do Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="9ef22-165">A set of custom fields is available as part of Partner Center Referrals Synchronization for Dynamics 365 solution **Opportunity** entity.</span></span> <span data-ttu-id="9ef22-166">Um usuário administrador de CRM precisará criar uma seção de CRM separada com os campos personalizados de **oportunidade** .</span><span class="sxs-lookup"><span data-stu-id="9ef22-166">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="9ef22-167">Os campos personalizados a seguir devem fazer parte da seção CRM:</span><span class="sxs-lookup"><span data-stu-id="9ef22-167">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="9ef22-168">**Sincronizar com o Partner Center**: se deseja sincronizar a oportunidade com o Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="9ef22-168">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="9ef22-169">**Identificador de referência**: um campo de identificador somente leitura para a referência do Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="9ef22-169">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="9ef22-170">**Link de referência**: um link somente leitura para a referência no Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="9ef22-170">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="9ef22-171">**Como a Microsoft pode ajudar?**: ajuda necessária da Microsoft para a referência</span><span class="sxs-lookup"><span data-stu-id="9ef22-171">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="9ef22-172">**Produtos**: lista de produtos associados a esta oportunidade</span><span class="sxs-lookup"><span data-stu-id="9ef22-172">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="9ef22-173">**Auditoria**: uma trilha de auditoria somente leitura para sincronização com as referências do Partner Center</span><span class="sxs-lookup"><span data-stu-id="9ef22-173">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="9ef22-174">EXEMPLOS</span><span class="sxs-lookup"><span data-stu-id="9ef22-174">SCENARIOS:</span></span>

1. <span data-ttu-id="9ef22-175">Sincronização de referência quando a referência é criada ou atualizada no CRM e sincronizada no Partner Center:</span><span class="sxs-lookup"><span data-stu-id="9ef22-175">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="9ef22-176">Entre no ambiente do Dynamics 365 CRM com o usuário que tem visibilidade na seção **oportunidade** do CRM.</span><span class="sxs-lookup"><span data-stu-id="9ef22-176">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="9ef22-177">Verifique se a seção a seguir está presente quando você cria uma "nova oportunidade" no ambiente do Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="9ef22-177">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="Oportunidade":::

   3. <span data-ttu-id="9ef22-179">Para sincronizar essa oportunidade com o Microsoft Partner Center, certifique-se de definir os seguintes campos no modo de exibição de cartão:</span><span class="sxs-lookup"><span data-stu-id="9ef22-179">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="9ef22-180">**Sincronizar com o Partner Center**: Sim</span><span class="sxs-lookup"><span data-stu-id="9ef22-180">**Sync with Partner Center**: Yes</span></span>

      - <span data-ttu-id="9ef22-181">**Como a Microsoft pode ajudar?**: selecione uma das seguintes opções:</span><span class="sxs-lookup"><span data-stu-id="9ef22-181">**How can Microsoft help?**: Select from the following:</span></span>

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="Seleções de ajuda":::

      - <span data-ttu-id="9ef22-183">**Produtos**: IDs de solução do produto</span><span class="sxs-lookup"><span data-stu-id="9ef22-183">**Products**: Solution IDs of the product</span></span>

   4. <span data-ttu-id="9ef22-184">Depois que a oportunidade for criada no Dynamics 365 com a opção **sincronizar com o Partner Center** definida como **Sim**, aguarde 10 minutos, entre em sua conta do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="9ef22-184">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="9ef22-185">Suas referências serão sincronizadas com o Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="9ef22-185">Your referrals will be synchronized with Dynamics 365.</span></span>

   5. <span data-ttu-id="9ef22-186">Consequentemente, para uma oportunidade que tenha a opção "sincronizar com o Partner Center" definida como "Sim", se você atualizar a oportunidade no Dynamics 365 CRM, as alterações serão sincronizadas em sua conta do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="9ef22-186">Consequently, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

   6. <span data-ttu-id="9ef22-187">As oportunidades sincronizadas com êxito com o Partner Center serão identificadas com ✔ ícone no Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="9ef22-187">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="9ef22-188">Sincronização de referência quando a referência é criada ou atualizada no Microsoft Partner Center e sincronizada no ambiente do Dynamics 365:</span><span class="sxs-lookup"><span data-stu-id="9ef22-188">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="9ef22-189">Entre no [painel](https://partner.microsoft.com/dashboard/home)do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="9ef22-189">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   2. <span data-ttu-id="9ef22-190">Selecione **referências** no menu à esquerda.</span><span class="sxs-lookup"><span data-stu-id="9ef22-190">Select **Referrals** from the left-hand menu.</span></span>

   3. <span data-ttu-id="9ef22-191">Crie uma nova referência de revenda do Partner Center clicando na opção "novo negócio".</span><span class="sxs-lookup"><span data-stu-id="9ef22-191">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

   4. <span data-ttu-id="9ef22-192">Entre no ambiente do Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="9ef22-192">Sign into your Dynamics 365 CRM environment.</span></span>

   5. <span data-ttu-id="9ef22-193">Navegue até **oportunidades abertas**.</span><span class="sxs-lookup"><span data-stu-id="9ef22-193">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="9ef22-194">A referência criada no Microsoft Partner Center agora está sincronizada no Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="9ef22-194">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   6. <span data-ttu-id="9ef22-195">Quando você seleciona uma referência sincronizada, os detalhes da exibição do cartão são preenchidos.</span><span class="sxs-lookup"><span data-stu-id="9ef22-195">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="9ef22-196">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="9ef22-196">Next steps</span></span>

- [<span data-ttu-id="9ef22-197">Mais informações sobre a plataforma de automatização de energia da Microsoft?</span><span class="sxs-lookup"><span data-stu-id="9ef22-197">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/power-automate/)

- [<span data-ttu-id="9ef22-198">Eventos de webhook do Partner Center</span><span class="sxs-lookup"><span data-stu-id="9ef22-198">Partner Center webhook events</span></span>](https://docs.microsoft.com/partner-center/develop/partner-center-webhook-events)

- [<span data-ttu-id="9ef22-199">Gerenciar clientes potenciais</span><span class="sxs-lookup"><span data-stu-id="9ef22-199">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="9ef22-200">Gerenciar oportunidades de venda conjunta</span><span class="sxs-lookup"><span data-stu-id="9ef22-200">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
