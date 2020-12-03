---
title: O conector de televenda para o centro de parceiros do Dynamics 365 CRM
ms.topic: how-to
ms.date: 05/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Sincronize as referências no Partner Center com seu conector de televenda para o Dynamics 365 CRM. Os vendedores podem, então, vender com a Microsoft de dentro de seus sistemas de CRM.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 18a54bf777cb987e8f486f85afcf277e04c1055c
ms.sourcegitcommit: 147813ba322653c989df5afe0b3bf0c252523a92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "96556354"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a><span data-ttu-id="1dcad-104">Conector de venda conjunta para Dynamics 365 CRM – visão geral</span><span class="sxs-lookup"><span data-stu-id="1dcad-104">Co-sell connector for Dynamics 365 CRM – Overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="1dcad-105">Funções apropriadas</span><span class="sxs-lookup"><span data-stu-id="1dcad-105">Appropriate roles</span></span>

- <span data-ttu-id="1dcad-106">Administrador de indicações</span><span class="sxs-lookup"><span data-stu-id="1dcad-106">Referrals admin</span></span>
- <span data-ttu-id="1dcad-107">Administrador do sistema ou personalizador do sistema no CRM</span><span class="sxs-lookup"><span data-stu-id="1dcad-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="1dcad-108">O conector de televenda do Partner Center permite que seus vendedores covendam-se com a Microsoft de dentro de seus sistemas de CRM.</span><span class="sxs-lookup"><span data-stu-id="1dcad-108">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="1dcad-109">Eles não precisarão ser treinados para usar o Partner Center para gerenciar acordos de venda.</span><span class="sxs-lookup"><span data-stu-id="1dcad-109">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="1dcad-110">Use os conectores de venda conjunta, para criar uma nova referência de cooperação para envolver um vendedor da Microsoft, receber referências do vendedor da Microsoft, aceitar/recusar referências, modificar dados de negociações, como valor de negócio e data de fechamento.</span><span class="sxs-lookup"><span data-stu-id="1dcad-110">Use the Co-sell connectors, to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span> <span data-ttu-id="1dcad-111">Você também pode receber todas as atualizações dos vendedores da Microsoft sobre esses acordos de venda conjunta.</span><span class="sxs-lookup"><span data-stu-id="1dcad-111">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="1dcad-112">Você pode fazer todas as suas referências funcionarem no CRM de sua escolha, em vez de no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="1dcad-112">You can do all of your referrals work within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="1dcad-113">A solução baseia-se na solução de automatização de energia da Microsoft e usa as APIs do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="1dcad-113">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="1dcad-114">Antes de instalar-pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1dcad-114">Before you install - pre-requisites</span></span>

|<span data-ttu-id="1dcad-115">**Tópicos**</span><span class="sxs-lookup"><span data-stu-id="1dcad-115">**Topics**</span></span>   |<span data-ttu-id="1dcad-116">**Detalhes**</span><span class="sxs-lookup"><span data-stu-id="1dcad-116">**Details**</span></span>   |<span data-ttu-id="1dcad-117">**Links**</span><span class="sxs-lookup"><span data-stu-id="1dcad-117">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="1dcad-118">ID de Microsoft Partner Network</span><span class="sxs-lookup"><span data-stu-id="1dcad-118">Microsoft Partner Network ID</span></span> |<span data-ttu-id="1dcad-119">Você precisa de uma ID de MPN válida</span><span class="sxs-lookup"><span data-stu-id="1dcad-119">You need a valid MPN ID</span></span>|<span data-ttu-id="1dcad-120">Para ingressar no [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="1dcad-120">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="1dcad-121">Covenda pronta</span><span class="sxs-lookup"><span data-stu-id="1dcad-121">Cosell ready</span></span>|<span data-ttu-id="1dcad-122">Sua solução de IP/serviços deve estar pronta para venda.</span><span class="sxs-lookup"><span data-stu-id="1dcad-122">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="1dcad-123">Venda com a Microsoft</span><span class="sxs-lookup"><span data-stu-id="1dcad-123">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="1dcad-124">Conta do Partner Center</span><span class="sxs-lookup"><span data-stu-id="1dcad-124">Partner Center account</span></span>|<span data-ttu-id="1dcad-125">A ID de MPN associada ao locatário do Partner Center deve ser a mesma que a ID do MPN associada à sua solução de venda conjunta.</span><span class="sxs-lookup"><span data-stu-id="1dcad-125">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="1dcad-126">Verifique se você pode ver suas referências de venda conjunta no portal do Partner Center antes de implantar os conectores.</span><span class="sxs-lookup"><span data-stu-id="1dcad-126">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="1dcad-127">Gerenciar sua conta</span><span class="sxs-lookup"><span data-stu-id="1dcad-127">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="1dcad-128">Funções de usuário da Central de parceiros</span><span class="sxs-lookup"><span data-stu-id="1dcad-128">Partner Center user roles</span></span>|<span data-ttu-id="1dcad-129">O funcionário que irá instalar e usar os conectores deve ser um administrador de referências</span><span class="sxs-lookup"><span data-stu-id="1dcad-129">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="1dcad-130">Atribuir permissões e funções de usuários</span><span class="sxs-lookup"><span data-stu-id="1dcad-130">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)| |<span data-ttu-id="1dcad-131">CRM do Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="1dcad-131">Dynamics 365 CRM</span></span>|<span data-ttu-id="1dcad-132">A função de usuário CRM é administrador do sistema ou personalizador do sistema</span><span class="sxs-lookup"><span data-stu-id="1dcad-132">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="1dcad-133">Atribuir funções no Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="1dcad-133">Assign roles in Dynamics 365</span></span>](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="1dcad-134">Conta de fluxo de automatização de energia</span><span class="sxs-lookup"><span data-stu-id="1dcad-134">Power Automate Flow Account</span></span>|<span data-ttu-id="1dcad-135">Uma conta de [energia ativa automatizada](https://flow.microsoft.com) para o administrador do sistema do CRM ou o personalizador do sistema.</span><span class="sxs-lookup"><span data-stu-id="1dcad-135">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="1dcad-136">Esse usuário deve entrar no [Power Automate](https://flow.microsoft.com) pelo menos uma vez antes da instalação.</span><span class="sxs-lookup"><span data-stu-id="1dcad-136">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a><span data-ttu-id="1dcad-137">Instalar a sincronização de referências do Partner Center para o Dynamics 365 (solução de automatização de energia)</span><span class="sxs-lookup"><span data-stu-id="1dcad-137">Install Partner Center Referrals Synchronization for Dynamics 365 (Power Automate Solution)</span></span>

1. <span data-ttu-id="1dcad-138">Vá para [energia automatizada](https://flow.microsoft.com) e selecione **ambientes** no canto superior direito.</span><span class="sxs-lookup"><span data-stu-id="1dcad-138">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="1dcad-139">Esta etapa mostrará as instâncias do CRM disponíveis.</span><span class="sxs-lookup"><span data-stu-id="1dcad-139">This step will show you the available CRM instances.</span></span>

2. <span data-ttu-id="1dcad-140">Selecione a instância apropriada do CRM na lista suspensa no canto superior direito.</span><span class="sxs-lookup"><span data-stu-id="1dcad-140">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="1dcad-141">Selecione **soluções** na barra de navegação à esquerda.</span><span class="sxs-lookup"><span data-stu-id="1dcad-141">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="1dcad-142">Clique no link **abrir AppSource** no menu superior.</span><span class="sxs-lookup"><span data-stu-id="1dcad-142">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Abrir AppSource":::

5. <span data-ttu-id="1dcad-144">Pesquise **conectores de referências do Partner Center para Dynamics365** na tela pop-up.</span><span class="sxs-lookup"><span data-stu-id="1dcad-144">Search for **Partner Center Referrals Connectors for Dynamics365** in the pop-up screen.</span></span>  

6. <span data-ttu-id="1dcad-145">Clique no botão **obter agora** e em **continuar**.</span><span class="sxs-lookup"><span data-stu-id="1dcad-145">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="1dcad-146">Isso abre a página onde você pode selecionar o ambiente CRM (Dynamics 365) para instalar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1dcad-146">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="1dcad-147">Concorde com os termos e condições.</span><span class="sxs-lookup"><span data-stu-id="1dcad-147">Agree to terms and conditions.</span></span>

8. <span data-ttu-id="1dcad-148">Em seguida, você será direcionado para a página **gerenciar suas soluções** .</span><span class="sxs-lookup"><span data-stu-id="1dcad-148">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="1dcad-149">Navegue até "referências do Partner Center" usando os botões de seta na parte inferior da página.</span><span class="sxs-lookup"><span data-stu-id="1dcad-149">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="1dcad-150">A **instalação agendada** deve aparecer ao lado da solução de referências do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="1dcad-150">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="1dcad-151">A instalação levará 10-15 minutos.</span><span class="sxs-lookup"><span data-stu-id="1dcad-151">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="1dcad-152">Quando a instalação for concluída, navegue de volta para [Power Automate](https://flow.microsoft.com) e selecione **soluções** na área de navegação à esquerda.</span><span class="sxs-lookup"><span data-stu-id="1dcad-152">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="1dcad-153">Observe que a **sincronização de referências do Partner Center para o Dynamics 365** está disponível na lista de soluções.</span><span class="sxs-lookup"><span data-stu-id="1dcad-153">Notice that **Partner Center Referrals Synchronization for Dynamics 365** is available in the Solutions list.</span></span>

10. <span data-ttu-id="1dcad-154">Selecione **sincronização de referências do Partner Center para o Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="1dcad-154">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="1dcad-155">Os fluxos e as entidades automatizados de energia a seguir estão disponíveis:</span><span class="sxs-lookup"><span data-stu-id="1dcad-155">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="CRMS disponíveis":::

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="1dcad-157">Prática recomendada: teste antes de entrar no ar</span><span class="sxs-lookup"><span data-stu-id="1dcad-157">Best practice: test before you go live</span></span>

<span data-ttu-id="1dcad-158">Antes de instalar, configurar e personalizar a solução de automatização de energia no ambiente de produção, certifique-se de testar a solução em uma instância de CRM de preparo.</span><span class="sxs-lookup"><span data-stu-id="1dcad-158">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="1dcad-159">Instale a solução de automatização de energia da Microsoft em uma instância de ambiente de preparo/CRM.</span><span class="sxs-lookup"><span data-stu-id="1dcad-159">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="1dcad-160">Faça uma cópia da solução e execute sua configuração e automatize as personalizações de fluxo no ambiente de preparo.</span><span class="sxs-lookup"><span data-stu-id="1dcad-160">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>
- <span data-ttu-id="1dcad-161">Teste a solução em uma instância de preparo/CRM.</span><span class="sxs-lookup"><span data-stu-id="1dcad-161">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="1dcad-162">Em caso de sucesso, importe como solução gerenciada para a instância de produção.</span><span class="sxs-lookup"><span data-stu-id="1dcad-162">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="1dcad-163">Configurar a solução</span><span class="sxs-lookup"><span data-stu-id="1dcad-163">Configure the solution</span></span>

1. <span data-ttu-id="1dcad-164">Depois de instalar a solução em sua instância do CRM, navegue de volta para o [Power Automate](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="1dcad-164">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>


2. <span data-ttu-id="1dcad-165">Na lista suspensa **ambientes** no canto superior direito, selecione a instância de CRM na qual você instalou a solução de automatização de energia.</span><span class="sxs-lookup"><span data-stu-id="1dcad-165">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="1dcad-166">Você precisará criar conexões que associem as três contas de usuário:</span><span class="sxs-lookup"><span data-stu-id="1dcad-166">You'll need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="1dcad-167">Usuário do Partner Center com credenciais de administrador de referências</span><span class="sxs-lookup"><span data-stu-id="1dcad-167">Partner Center user with referrals admin credentials</span></span>

   - <span data-ttu-id="1dcad-168">Eventos do Partner Center</span><span class="sxs-lookup"><span data-stu-id="1dcad-168">Partner Center Events</span></span>

   - <span data-ttu-id="1dcad-169">Administrador de CRM com os fluxos de energia automatizada na solução.</span><span class="sxs-lookup"><span data-stu-id="1dcad-169">CRM admin with the Power Automate flows in the solution.</span></span>

      1. <span data-ttu-id="1dcad-170">Selecione **conexões** na barra de navegação à esquerda e selecione a solução "referências do Partner Center" na lista.</span><span class="sxs-lookup"><span data-stu-id="1dcad-170">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>

      2. <span data-ttu-id="1dcad-171">Crie uma conexão clicando em **criar uma conexão**.</span><span class="sxs-lookup"><span data-stu-id="1dcad-171">Create a connection by clicking **Create a connection**.</span></span>

         :::image type="content" source="images/cosellconnectors/dynamics1.png" alt-text="Criar conexão":::

      3. <span data-ttu-id="1dcad-173">Procure por **referências do Partner Center (versão prévia)** na barra de pesquisa no canto superior direito.</span><span class="sxs-lookup"><span data-stu-id="1dcad-173">Search for **Partner Center Referrals (preview)** in the search bar on the top-right corner.</span></span>

      4. <span data-ttu-id="1dcad-174">Crie uma conexão para o usuário do Partner Center com a função de credenciais do administrador de referências.</span><span class="sxs-lookup"><span data-stu-id="1dcad-174">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

      5. <span data-ttu-id="1dcad-175">Em seguida, crie uma conexão de eventos do Partner Center para o usuário do Partner Center com as credenciais do administrador de referências.</span><span class="sxs-lookup"><span data-stu-id="1dcad-175">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

      6. <span data-ttu-id="1dcad-176">Crie uma conexão para Common Data Service (ambiente atual) para o usuário administrador do CRM.</span><span class="sxs-lookup"><span data-stu-id="1dcad-176">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>
       
     
      7. <span data-ttu-id="1dcad-177">Depois de adicionar todas as conexões, você deverá ver as seguintes conexões em seu ambiente:</span><span class="sxs-lookup"><span data-stu-id="1dcad-177">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

:::image type="content" source="images/cosellconnectors/dynamics2.png" alt-text="Conexões":::
   
## <a name="edit-the-connections"></a><span data-ttu-id="1dcad-179">Editar as conexões</span><span class="sxs-lookup"><span data-stu-id="1dcad-179">Edit the connections</span></span>

1. <span data-ttu-id="1dcad-180">Volte para a página **soluções** e selecione **solução padrão**.</span><span class="sxs-lookup"><span data-stu-id="1dcad-180">Return to the **Solutions** page and select **Default Solution**.</span></span> <span data-ttu-id="1dcad-181">Selecione **referência de conexão (versão prévia)** clicando em **tudo**.</span><span class="sxs-lookup"><span data-stu-id="1dcad-181">Select **Connection Reference (preview)** by clicking **All**.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics3.png" alt-text="Connect":::

2. <span data-ttu-id="1dcad-183">Edite cada uma das conexões uma por uma selecionando o ícone de três pontos.</span><span class="sxs-lookup"><span data-stu-id="1dcad-183">Edit each of the Connections one by one by selecting the three dots icon.</span></span> <span data-ttu-id="1dcad-184">Adicione as conexões relevantes.</span><span class="sxs-lookup"><span data-stu-id="1dcad-184">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics4.png" alt-text="Conexões listadas"::: 

3.  <span data-ttu-id="1dcad-186">Ative os fluxos na seguinte sequência:</span><span class="sxs-lookup"><span data-stu-id="1dcad-186">Turn on the flows in the following sequence:</span></span>
- <span data-ttu-id="1dcad-187">Registro do webhook do Partner Center (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="1dcad-187">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="1dcad-188">Criar referência de co-venda – Dynamics 365 para o Partner Center (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="1dcad-188">Create Co-sell Referral – Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="1dcad-189">Partner Center Microsoft co-vender atualizações de referência para o Dynamics 365 (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="1dcad-189">Partner Center Microsoft Co-sell Referral Updates to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="1dcad-190">Partner Center para Dynamics 365 (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="1dcad-190">Partner Center to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="1dcad-191">Dynamics 365 para o Partner Center (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="1dcad-191">Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="1dcad-192">Oportunidade do Dynamics 365 para o Partner Center (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="1dcad-192">Dynamics 365 Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="1dcad-193">Dynamics 365 Microsoft Solutions para Partner Center (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="1dcad-193">Dynamics 365 Microsoft Solutions to Partner Center (Insider Preview)</span></span>
 

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="1dcad-194">Usar APIs de webhook para registrar eventos de alteração de recurso</span><span class="sxs-lookup"><span data-stu-id="1dcad-194">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="1dcad-195">As APIs de webhook do Partner Center permitem que você se registre em eventos de alteração de recursos.</span><span class="sxs-lookup"><span data-stu-id="1dcad-195">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="1dcad-196">Esses eventos de alteração são enviados para a URL como postagens HTTP.</span><span class="sxs-lookup"><span data-stu-id="1dcad-196">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="1dcad-197">Para registrar sua URL, selecione o **registro do webhook do Partner Center (insider Preview)** fluxo automatizado de energia.</span><span class="sxs-lookup"><span data-stu-id="1dcad-197">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="1dcad-198">Adicione conexões para o usuário do centro de parceiros (a) com referências credenciais de administrador (b.) os eventos do centro de parceiros conforme realçado abaixo</span><span class="sxs-lookup"><span data-stu-id="1dcad-198">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Gatilho":::

3. <span data-ttu-id="1dcad-200">Ao fazer essas atualizações, você verá</span><span class="sxs-lookup"><span data-stu-id="1dcad-200">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks":::

4. <span data-ttu-id="1dcad-202">Salve as alterações e selecione **Ativar**.</span><span class="sxs-lookup"><span data-stu-id="1dcad-202">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="1dcad-203">Para habilitar o parceiro do Partner Center a ouvir as alterações de evento, execute as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="1dcad-203">To enable Partner Center webhooks to listen to event changes, do the following steps:</span></span>

5. <span data-ttu-id="1dcad-204">Selecione **Partner Center para Dynamics 365 (insider Preview)**.</span><span class="sxs-lookup"><span data-stu-id="1dcad-204">Select **Partner Center to Dynamics 365 (Insider Preview)**.</span></span>

6. <span data-ttu-id="1dcad-205">Selecione o ícone **Editar** e selecione **quando uma solicitação HTTP é recebida**.</span><span class="sxs-lookup"><span data-stu-id="1dcad-205">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="1dcad-206">Selecione o ícone de **cópia** para copiar a URL de postagem http fornecida.</span><span class="sxs-lookup"><span data-stu-id="1dcad-206">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="Copiar URL":::

8. <span data-ttu-id="1dcad-208">Agora, selecione o fluxo "registro do webhook do Partner Center (insider Preview)" automatizar fluxos de energia e selecione **executar**.</span><span class="sxs-lookup"><span data-stu-id="1dcad-208">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="1dcad-209">Verifique se a janela "executar fluxo" é aberta no painel direito e clique em **continuar**.</span><span class="sxs-lookup"><span data-stu-id="1dcad-209">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="1dcad-210">Insira os seguintes detalhes:</span><span class="sxs-lookup"><span data-stu-id="1dcad-210">Enter the following details:</span></span>

    1. <span data-ttu-id="1dcad-211">**Ponto de extremidade de gatilho http**: URL copiada da etapa anterior</span><span class="sxs-lookup"><span data-stu-id="1dcad-211">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="1dcad-212">**Eventos a serem registrados**: "referência criada" e "referência atualizada"</span><span class="sxs-lookup"><span data-stu-id="1dcad-212">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    3. <span data-ttu-id="1dcad-213">**Substituir pontos de extremidade de gatilho existentes, se presente**: Sim (isso substitui todos os pontos de extremidade existentes.)</span><span class="sxs-lookup"><span data-stu-id="1dcad-213">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="1dcad-214">Selecione **executar** e, em seguida, selecione **concluído.**</span><span class="sxs-lookup"><span data-stu-id="1dcad-214">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="1dcad-215">O webhook agora pode escutar criar e atualizar eventos.</span><span class="sxs-lookup"><span data-stu-id="1dcad-215">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="1dcad-216">Personalizar etapas de sincronização</span><span class="sxs-lookup"><span data-stu-id="1dcad-216">Customize synchronization steps</span></span>

<span data-ttu-id="1dcad-217">Quando as referências de venda cruzada são sincronizadas entre o Partner Center e o sistema CRM, os campos sincronizados no PC do Partner Center são listados aqui.</span><span class="sxs-lookup"><span data-stu-id="1dcad-217">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="1dcad-218">Geralmente, os sistemas CRM são altamente personalizados.</span><span class="sxs-lookup"><span data-stu-id="1dcad-218">Often CRM systems are highly customized.</span></span> <span data-ttu-id="1dcad-219">Você pode personalizar os fluxos de energia automatizada.</span><span class="sxs-lookup"><span data-stu-id="1dcad-219">You can customize the Power Automate flows.</span></span> <span data-ttu-id="1dcad-220">Siga o guia de mapeamento de campo e, se necessário, faça as alterações apropriadas nas etapas de fluxos de energia automatizar.</span><span class="sxs-lookup"><span data-stu-id="1dcad-220">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="1dcad-221">Os mapeamentos do Microsoft Partner centers para CRM são fornecidos, mas com base no seu ambiente de CRM, você pode optar por personalizar ainda mais os campos.</span><span class="sxs-lookup"><span data-stu-id="1dcad-221">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="1dcad-222">Várias etapas de cada um dos fluxos de energia automatizada podem ser personalizadas com base em suas necessidades.</span><span class="sxs-lookup"><span data-stu-id="1dcad-222">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="1dcad-223">Veja a seguir exemplos de personalizações disponíveis:</span><span class="sxs-lookup"><span data-stu-id="1dcad-223">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="1dcad-224">Para personalizar os campos de criação ou atualização de eventos no Partner Center para a sincronização de referência do CRM:</span><span class="sxs-lookup"><span data-stu-id="1dcad-224">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="1dcad-225">a.</span><span class="sxs-lookup"><span data-stu-id="1dcad-225">a.</span></span> <span data-ttu-id="1dcad-226">Selecione Partner Center para Dynamics 365 (insider Preview) ou Partner Center para Salesforce (insider Preview).</span><span class="sxs-lookup"><span data-stu-id="1dcad-226">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

    <span data-ttu-id="1dcad-227">b.</span><span class="sxs-lookup"><span data-stu-id="1dcad-227">b.</span></span> <span data-ttu-id="1dcad-228">Selecione **Editar** para editar/personalizar o fluxo de automatização de energia.</span><span class="sxs-lookup"><span data-stu-id="1dcad-228">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="1dcad-229">c.</span><span class="sxs-lookup"><span data-stu-id="1dcad-229">c.</span></span> <span data-ttu-id="1dcad-230">Selecione **(escopo) sincronizar o cliente potencial ou a oportunidade**.</span><span class="sxs-lookup"><span data-stu-id="1dcad-230">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="1dcad-231">Para personalizar mapeamentos de campo de CRM (com base no guia mapeamentos de campo) para criar eventos, selecione **se for nova oportunidade compartilhada e, em seguida,**.</span><span class="sxs-lookup"><span data-stu-id="1dcad-231">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="1dcad-232">Selecione a subetapa **se sim** e, em seguida, expanda **criando uma nova oportunidade no CRM**.</span><span class="sxs-lookup"><span data-stu-id="1dcad-232">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="1dcad-233">Você pode editar os mapeamentos nesta seção usando o guia de mapeamento de campos.</span><span class="sxs-lookup"><span data-stu-id="1dcad-233">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="1dcad-234">d.</span><span class="sxs-lookup"><span data-stu-id="1dcad-234">d.</span></span> <span data-ttu-id="1dcad-235">Para personalizar os mapeamentos de campo do CRM (com base no guia mapeamentos de campo) para eventos de atualização, clique na etapa "(escopo) sincronizar o cliente potencial ou a oportunidade".</span><span class="sxs-lookup"><span data-stu-id="1dcad-235">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="1dcad-236">e.</span><span class="sxs-lookup"><span data-stu-id="1dcad-236">e.</span></span> <span data-ttu-id="1dcad-237">Selecione **se for uma atualização para uma oportunidade e, em seguida,**.</span><span class="sxs-lookup"><span data-stu-id="1dcad-237">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="1dcad-238">Selecione a subetapa **se sim** e, em seguida, expanda **se a diferença entre os objetos de oportunidade no Partner Center e no CRM, em seguida**.</span><span class="sxs-lookup"><span data-stu-id="1dcad-238">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

    <span data-ttu-id="1dcad-239">f.</span><span class="sxs-lookup"><span data-stu-id="1dcad-239">f.</span></span> <span data-ttu-id="1dcad-240">Selecione **se sim** seguido de **Atualizar oportunidade existente**</span><span class="sxs-lookup"><span data-stu-id="1dcad-240">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="1dcad-241">Para personalizar os campos de sincronização de referência do CRM para PC para eventos de atualização:</span><span class="sxs-lookup"><span data-stu-id="1dcad-241">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="1dcad-242">a.</span><span class="sxs-lookup"><span data-stu-id="1dcad-242">a.</span></span> <span data-ttu-id="1dcad-243">Selecione **Editar**  para editar/personalizar o fluxo de automatização de energia.</span><span class="sxs-lookup"><span data-stu-id="1dcad-243">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="1dcad-244">b.</span><span class="sxs-lookup"><span data-stu-id="1dcad-244">b.</span></span> <span data-ttu-id="1dcad-245">Selecione **(escopo) sincronizar a oportunidade**.</span><span class="sxs-lookup"><span data-stu-id="1dcad-245">Select **(Scope) Synchronize the opportunity**.</span></span>

    <span data-ttu-id="1dcad-246">c.</span><span class="sxs-lookup"><span data-stu-id="1dcad-246">c.</span></span> <span data-ttu-id="1dcad-247">Para personalizar mapeamentos de campo de CRM para eventos de atualização, selecione **se houver diferença entre os objetos de cliente potencial no Partner Center e no CRM**.</span><span class="sxs-lookup"><span data-stu-id="1dcad-247">To customize CRM field mappings for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span> 

    <span data-ttu-id="1dcad-248">d.</span><span class="sxs-lookup"><span data-stu-id="1dcad-248">d.</span></span> <span data-ttu-id="1dcad-249">Selecione a subetapa **se sim** e, em seguida, expanda a etapa **atualizar uma referência com dados de oportunidade**.</span><span class="sxs-lookup"><span data-stu-id="1dcad-249">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="1dcad-250">Você pode editar os mapeamentos nesta seção com base no guia de mapeamento de campos.</span><span class="sxs-lookup"><span data-stu-id="1dcad-250">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="1dcad-251">Para personalizar os campos para a sincronização de referência do CRM para PC para criar eventos?</span><span class="sxs-lookup"><span data-stu-id="1dcad-251">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="1dcad-252">a.</span><span class="sxs-lookup"><span data-stu-id="1dcad-252">a.</span></span> <span data-ttu-id="1dcad-253">Selecione **Editar**  para editar/personalizar o fluxo de automatização de energia.</span><span class="sxs-lookup"><span data-stu-id="1dcad-253">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="1dcad-254">b.</span><span class="sxs-lookup"><span data-stu-id="1dcad-254">b.</span></span> <span data-ttu-id="1dcad-255">Selecione **(escopo) sincronizando referências.**</span><span class="sxs-lookup"><span data-stu-id="1dcad-255">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="1dcad-256">c.</span><span class="sxs-lookup"><span data-stu-id="1dcad-256">c.</span></span> <span data-ttu-id="1dcad-257">Para personalizar mapeamentos de campo de CRM (com base no guia mapeamentos de campo) para criar eventos, selecione **criar referência da Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="1dcad-257">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

   <span data-ttu-id="1dcad-258">Você pode editar os mapeamentos nesta seção com base no guia de mapeamento de campos.</span><span class="sxs-lookup"><span data-stu-id="1dcad-258">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

<span data-ttu-id="1dcad-259">Há duas variáveis de ambiente criadas:</span><span class="sxs-lookup"><span data-stu-id="1dcad-259">There are two environment variables created:</span></span>

- <span data-ttu-id="1dcad-260">Marca de seleção: significa se você precisará de um ícone de marca de seleção além das oportunidades sincronizadas bidirecionalmente entre o Partner Center e o Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="1dcad-260">Checkmark: Signifies whether you would need a checkmark icon besides opportunities that are synchronized bi-directionally between Partner Center and Dynamics 365 CRM.</span></span>

- <span data-ttu-id="1dcad-261">Sincronizar somente oportunidades de venda conjuntas: significa se você deseja sincronizar apenas as oportunidades de venda conjunta.</span><span class="sxs-lookup"><span data-stu-id="1dcad-261">Sync co-sell opportunities only: Signifies whether you want to synchronize only Co-sell opportunities.</span></span>

<span data-ttu-id="1dcad-262">Você pode optar por editar o valor padrão para as variáveis de ambiente.</span><span class="sxs-lookup"><span data-stu-id="1dcad-262">You can choose to edit the default value for the environment variables.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics5.png" alt-text="Caixa de edição para valores padrão":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="1dcad-264">Sincronização de referência de cooperação bidirecional de ponta a ponta</span><span class="sxs-lookup"><span data-stu-id="1dcad-264">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="1dcad-265">Depois de instalar, configurar e personalizar a solução de automatização de energia, você pode testar a sincronização de referências de venda entre o Dynamics 365 e o Partner Center.</span><span class="sxs-lookup"><span data-stu-id="1dcad-265">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="1dcad-266">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1dcad-266">Pre-requisites</span></span>

<span data-ttu-id="1dcad-267">Para sincronizar as referências no Partner Center e no Dynamics 365 CRM, a solução de energia automatizada claramente demarcates os campos de referência específicos da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1dcad-267">To synchronize the referrals across Partner Center and Dynamics 365 CRM, the Power Automate solution clearly demarcates Microsoft-specific referral fields.</span></span> <span data-ttu-id="1dcad-268">Essa identificação fornece às equipes do vendedor a capacidade de decidir quais referências eles desejam compartilhar com a Microsoft para fazer a venda.</span><span class="sxs-lookup"><span data-stu-id="1dcad-268">This identification gives your seller teams  the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="1dcad-269">Um conjunto de campos personalizados está disponível como parte da entidade **oportunidade** .</span><span class="sxs-lookup"><span data-stu-id="1dcad-269">A set of custom fields is available as part of the **Opportunity** entity.</span></span> <span data-ttu-id="1dcad-270">Um usuário administrador de CRM precisará criar uma seção de CRM separada com os campos personalizados de **oportunidade** .</span><span class="sxs-lookup"><span data-stu-id="1dcad-270">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="1dcad-271">Os campos personalizados a seguir devem fazer parte da seção CRM:</span><span class="sxs-lookup"><span data-stu-id="1dcad-271">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="1dcad-272">**Sincronizar com o Partner Center**: se deseja sincronizar a oportunidade com o Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="1dcad-272">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="1dcad-273">**Identificador de referência**: um campo de identificador somente leitura para a referência do Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="1dcad-273">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="1dcad-274">**Link de referência**: um link somente leitura para a referência no Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="1dcad-274">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="1dcad-275">**Como a Microsoft pode ajudar?**: ajuda necessária da Microsoft para a referência</span><span class="sxs-lookup"><span data-stu-id="1dcad-275">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="1dcad-276">**Produtos**: lista de produtos associados a esta oportunidade</span><span class="sxs-lookup"><span data-stu-id="1dcad-276">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="1dcad-277">**Auditoria**: uma trilha de auditoria somente leitura para sincronização com as referências do Partner Center</span><span class="sxs-lookup"><span data-stu-id="1dcad-277">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

<span data-ttu-id="1dcad-278">Atualize o formulário oportunidade no Dynamics 365 CRM para incluir o campo soluções para produtos.</span><span class="sxs-lookup"><span data-stu-id="1dcad-278">Update the opportunity form in Dynamics 365 CRM to include Solutions for Products field.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics6.png" alt-text="Formulário de oportunidade":::

:::image type="content" source="images/cosellconnectors/dynamics7.png" alt-text="{alt-text}":::

### <a name="scenarios"></a><span data-ttu-id="1dcad-281">EXEMPLOS</span><span class="sxs-lookup"><span data-stu-id="1dcad-281">SCENARIOS:</span></span>

1. <span data-ttu-id="1dcad-282">Sincronização de referência quando a referência é criada ou atualizada no CRM e sincronizada no Partner Center:</span><span class="sxs-lookup"><span data-stu-id="1dcad-282">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="1dcad-283">Entre no ambiente do Dynamics 365 CRM com o usuário que tem visibilidade na seção **oportunidade** do CRM.</span><span class="sxs-lookup"><span data-stu-id="1dcad-283">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="1dcad-284">Verifique se a seção a seguir está presente quando você cria uma "nova oportunidade" no ambiente do Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="1dcad-284">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="Exemplo de seção de oportunidade mostrando informações do Microsoft Partner Center no Dynamics 365.":::

   3. <span data-ttu-id="1dcad-286">Para sincronizar essa oportunidade com o Microsoft Partner Center, certifique-se de definir os seguintes campos no modo de exibição de cartão:</span><span class="sxs-lookup"><span data-stu-id="1dcad-286">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="1dcad-287">**Sincronizar com o Partner Center**: Sim</span><span class="sxs-lookup"><span data-stu-id="1dcad-287">**Sync with Partner Center**: Yes</span></span>

      - <span data-ttu-id="1dcad-288">**Como a Microsoft pode ajudar?**: selecione uma das seguintes opções:</span><span class="sxs-lookup"><span data-stu-id="1dcad-288">**How can Microsoft help?**: Select from the following:</span></span>

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="Exemplo de seção de oportunidade no Dynamics 365 que mostra as opções de ajuda do Microsoft Partner Center ao lado de um campo chamado como a Microsoft pode ajudar?":::

      - <span data-ttu-id="1dcad-290">**Produtos**: IDs de solução do produto</span><span class="sxs-lookup"><span data-stu-id="1dcad-290">**Products**: Solution IDs of the product</span></span>

   4. <span data-ttu-id="1dcad-291">Depois que a oportunidade for criada no Dynamics 365 com a opção **sincronizar com o Partner Center** definida como **Sim**, aguarde 10 minutos e entre em sua conta do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="1dcad-291">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, and then sign into your Partner Center account.</span></span> <span data-ttu-id="1dcad-292">Suas referências serão sincronizadas com o Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="1dcad-292">Your referrals will be synchronized with Dynamics 365.</span></span>

   5. <span data-ttu-id="1dcad-293">Da mesma forma, para uma oportunidade que tenha a opção "sincronizar com o Partner Center" definida como "Sim", se você atualizar a oportunidade no Dynamics 365 CRM, as alterações serão sincronizadas em sua conta do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="1dcad-293">Likewise, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

   6. <span data-ttu-id="1dcad-294">As oportunidades sincronizadas com êxito com o Partner Center serão identificadas com ✔ ícone no Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="1dcad-294">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="1dcad-295">Sincronização de referência quando a referência é criada ou atualizada no Microsoft Partner Center e sincronizada no ambiente do Dynamics 365:</span><span class="sxs-lookup"><span data-stu-id="1dcad-295">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="1dcad-296">Entre no [painel](https://partner.microsoft.com/dashboard/home)do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="1dcad-296">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   2. <span data-ttu-id="1dcad-297">Selecione **referências** no menu à esquerda.</span><span class="sxs-lookup"><span data-stu-id="1dcad-297">Select **Referrals** from the left-hand menu.</span></span>

   3. <span data-ttu-id="1dcad-298">Crie uma nova referência de revenda do Partner Center clicando na opção "novo negócio".</span><span class="sxs-lookup"><span data-stu-id="1dcad-298">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

   4. <span data-ttu-id="1dcad-299">Entre no ambiente do Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="1dcad-299">Sign into your Dynamics 365 CRM environment.</span></span>

   5. <span data-ttu-id="1dcad-300">Navegue até **oportunidades abertas**.</span><span class="sxs-lookup"><span data-stu-id="1dcad-300">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="1dcad-301">A referência criada no Microsoft Partner Center agora está sincronizada no Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="1dcad-301">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   6. <span data-ttu-id="1dcad-302">Quando você seleciona uma referência sincronizada, os detalhes da exibição do cartão são preenchidos.</span><span class="sxs-lookup"><span data-stu-id="1dcad-302">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1dcad-303">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="1dcad-303">Next steps</span></span>

- [<span data-ttu-id="1dcad-304">Gerenciar clientes potenciais</span><span class="sxs-lookup"><span data-stu-id="1dcad-304">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="1dcad-305">Gerenciar oportunidades de venda conjunta</span><span class="sxs-lookup"><span data-stu-id="1dcad-305">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="1dcad-306">Mais informações sobre a plataforma de automatização de energia da Microsoft?</span><span class="sxs-lookup"><span data-stu-id="1dcad-306">More about Microsoft Power Automate platform?</span></span>](/power-automate/)

- [<span data-ttu-id="1dcad-307">Webhooks do Partner Center</span><span class="sxs-lookup"><span data-stu-id="1dcad-307">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)