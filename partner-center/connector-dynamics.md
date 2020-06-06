---
title: O conector de televenda para o centro de parceiros do Dynamics 365 CRM
ms.topic: article
ms.date: 05/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Sincronize suas referências no Partner Center com o Dynamics 365 CRM
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: ''
ms.localizationpriority: medium
ms.openlocfilehash: fef5468e0dc51cd9830fda6fb2ae60df5d9f39b5
ms.sourcegitcommit: ca6e0d4a9034120dd600c52ac67b9927dc63b7f5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/05/2020
ms.locfileid: "84453243"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a><span data-ttu-id="057e0-103">Conector de venda conjunta para Dynamics 365 CRM – visão geral</span><span class="sxs-lookup"><span data-stu-id="057e0-103">Co-sell connector for Dynamics 365 CRM – Overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="057e0-104">Funções apropriadas</span><span class="sxs-lookup"><span data-stu-id="057e0-104">Appropriate roles</span></span>

- <span data-ttu-id="057e0-105">Administrador de indicações</span><span class="sxs-lookup"><span data-stu-id="057e0-105">Referrals admin</span></span>
- <span data-ttu-id="057e0-106">Administrador do sistema ou personalizador do sistema no CRM</span><span class="sxs-lookup"><span data-stu-id="057e0-106">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="057e0-107">O conector de televenda do Partner Center permite que seus vendedores covendam-se com a Microsoft de dentro de seus sistemas de CRM.</span><span class="sxs-lookup"><span data-stu-id="057e0-107">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="057e0-108">Eles não precisarão ser treinados para usar o Partner Center para gerenciar acordos de venda.</span><span class="sxs-lookup"><span data-stu-id="057e0-108">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="057e0-109">Use os conectores de venda conjunta, para criar uma nova referência de cooperação para envolver um vendedor da Microsoft, receber referências do vendedor da Microsoft, aceitar/recusar referências, modificar dados de negociações, como valor de negócio e data de fechamento.</span><span class="sxs-lookup"><span data-stu-id="057e0-109">Use the Co-sell connectors, to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span> <span data-ttu-id="057e0-110">Você também pode receber todas as atualizações dos vendedores da Microsoft sobre esses acordos de venda conjunta.</span><span class="sxs-lookup"><span data-stu-id="057e0-110">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="057e0-111">Você pode fazer todas as suas referências funcionarem no CRM de sua escolha, em vez de no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="057e0-111">You can do all of your referrals work within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="057e0-112">A solução baseia-se na solução de automatização de energia da Microsoft e usa as APIs do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="057e0-112">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="057e0-113">Antes de instalar-pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="057e0-113">Before you install - pre-requisites</span></span>

|<span data-ttu-id="057e0-114">**Tópicos**</span><span class="sxs-lookup"><span data-stu-id="057e0-114">**Topics**</span></span>   |<span data-ttu-id="057e0-115">**Detalhes**</span><span class="sxs-lookup"><span data-stu-id="057e0-115">**Details**</span></span>   |<span data-ttu-id="057e0-116">**Links**</span><span class="sxs-lookup"><span data-stu-id="057e0-116">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="057e0-117">ID de Microsoft Partner Network</span><span class="sxs-lookup"><span data-stu-id="057e0-117">Microsoft Partner Network ID</span></span> |<span data-ttu-id="057e0-118">Você precisa de uma ID de MPN válida</span><span class="sxs-lookup"><span data-stu-id="057e0-118">You need a valid MPN ID</span></span>|<span data-ttu-id="057e0-119">Para ingressar no [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="057e0-119">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="057e0-120">Covenda pronta</span><span class="sxs-lookup"><span data-stu-id="057e0-120">Cosell ready</span></span>|<span data-ttu-id="057e0-121">Sua solução de IP/serviços deve estar pronta para venda.</span><span class="sxs-lookup"><span data-stu-id="057e0-121">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="057e0-122">Venda com a Microsoft</span><span class="sxs-lookup"><span data-stu-id="057e0-122">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="057e0-123">Conta do Partner Center</span><span class="sxs-lookup"><span data-stu-id="057e0-123">Partner Center account</span></span>|<span data-ttu-id="057e0-124">A ID de MPN associada ao locatário do Partner Center deve ser a mesma que a ID do MPN associada à sua solução de venda conjunta.</span><span class="sxs-lookup"><span data-stu-id="057e0-124">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="057e0-125">Verifique se você pode ver suas referências de venda conjunta no portal do Partner Center antes de implantar os conectores.</span><span class="sxs-lookup"><span data-stu-id="057e0-125">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="057e0-126">Gerenciar sua conta</span><span class="sxs-lookup"><span data-stu-id="057e0-126">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="057e0-127">Funções de usuário da Central de parceiros</span><span class="sxs-lookup"><span data-stu-id="057e0-127">Partner Center user roles</span></span>|<span data-ttu-id="057e0-128">O funcionário que irá instalar e usar os conectores deve ser um administrador de referências</span><span class="sxs-lookup"><span data-stu-id="057e0-128">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="057e0-129">Atribuir permissões e funções de usuários</span><span class="sxs-lookup"><span data-stu-id="057e0-129">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)| |<span data-ttu-id="057e0-130">CRM do Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="057e0-130">Dynamics 365 CRM</span></span>|<span data-ttu-id="057e0-131">A função de usuário CRM é administrador do sistema ou personalizador do sistema</span><span class="sxs-lookup"><span data-stu-id="057e0-131">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="057e0-132">Atribuir funções no Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="057e0-132">Assign roles in Dynamics 365</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="057e0-133">Conta de fluxo de automatização de energia</span><span class="sxs-lookup"><span data-stu-id="057e0-133">Power Automate Flow Account</span></span>|<span data-ttu-id="057e0-134">Uma conta de [energia ativa automatizada](https://flow.microsoft.com) para o administrador do sistema do CRM ou o personalizador do sistema.</span><span class="sxs-lookup"><span data-stu-id="057e0-134">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="057e0-135">Esse usuário deve entrar no [Power Automate](https://flow.microsoft.com) pelo menos uma vez antes da instalação.</span><span class="sxs-lookup"><span data-stu-id="057e0-135">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a><span data-ttu-id="057e0-136">Instalar a sincronização de referências do Partner Center para o Dynamics 365 (solução de automatização de energia)</span><span class="sxs-lookup"><span data-stu-id="057e0-136">Install Partner Center Referrals Synchronization for Dynamics 365 (Power Automate Solution)</span></span>

1. <span data-ttu-id="057e0-137">Vá para [energia automatizada](https://flow.microsoft.com) e selecione **ambientes** no canto superior direito.</span><span class="sxs-lookup"><span data-stu-id="057e0-137">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="057e0-138">Esta etapa mostrará as instâncias do CRM disponíveis.</span><span class="sxs-lookup"><span data-stu-id="057e0-138">This step will show you the available CRM instances.</span></span>

2. <span data-ttu-id="057e0-139">Selecione a instância apropriada do CRM na lista suspensa no canto superior direito.</span><span class="sxs-lookup"><span data-stu-id="057e0-139">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="057e0-140">Selecione **soluções** na barra de navegação à esquerda.</span><span class="sxs-lookup"><span data-stu-id="057e0-140">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="057e0-141">Clique no link **abrir AppSource** no menu superior.</span><span class="sxs-lookup"><span data-stu-id="057e0-141">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Abrir AppSource":::

5. <span data-ttu-id="057e0-143">Pesquise **conectores de referências do Partner Center para Dynamics365** na tela pop-up.</span><span class="sxs-lookup"><span data-stu-id="057e0-143">Search for **Partner Center Referrals Connectors for Dynamics365** in the pop-up screen.</span></span>  

6. <span data-ttu-id="057e0-144">Clique no botão **obter agora** e em **continuar**.</span><span class="sxs-lookup"><span data-stu-id="057e0-144">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="057e0-145">Isso abre a página onde você pode selecionar o ambiente CRM (Dynamics 365) para instalar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="057e0-145">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="057e0-146">Concorde com os termos e condições.</span><span class="sxs-lookup"><span data-stu-id="057e0-146">Agree to terms and conditions.</span></span>

8. <span data-ttu-id="057e0-147">Em seguida, você será direcionado para a página **gerenciar suas soluções** .</span><span class="sxs-lookup"><span data-stu-id="057e0-147">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="057e0-148">Navegue até "referências do Partner Center" usando os botões de seta na parte inferior da página.</span><span class="sxs-lookup"><span data-stu-id="057e0-148">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="057e0-149">A **instalação agendada** deve aparecer ao lado da solução de referências do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="057e0-149">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="057e0-150">A instalação levará 10-15 minutos.</span><span class="sxs-lookup"><span data-stu-id="057e0-150">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="057e0-151">Quando a instalação for concluída, navegue de volta para [Power Automate](https://flow.microsoft.com) e selecione **soluções** na área de navegação à esquerda.</span><span class="sxs-lookup"><span data-stu-id="057e0-151">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="057e0-152">Observe que a **sincronização de referências do Partner Center para o Dynamics 365** está disponível na lista de soluções.</span><span class="sxs-lookup"><span data-stu-id="057e0-152">Notice that **Partner Center Referrals Synchronization for Dynamics 365** is available in the Solutions list.</span></span>

10. <span data-ttu-id="057e0-153">Selecione **sincronização de referências do Partner Center para o Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="057e0-153">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="057e0-154">Os fluxos e as entidades automatizados de energia a seguir estão disponíveis:</span><span class="sxs-lookup"><span data-stu-id="057e0-154">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="CRMS disponíveis":::

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="057e0-156">Prática recomendada: teste antes de entrar no ar</span><span class="sxs-lookup"><span data-stu-id="057e0-156">Best practice: test before you go live</span></span>

<span data-ttu-id="057e0-157">Antes de instalar, configurar e personalizar a solução de automatização de energia no ambiente de produção, certifique-se de testar a solução em uma instância de CRM de preparo.</span><span class="sxs-lookup"><span data-stu-id="057e0-157">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="057e0-158">Instale a solução de automatização de energia da Microsoft em uma instância de ambiente de preparo/CRM.</span><span class="sxs-lookup"><span data-stu-id="057e0-158">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="057e0-159">Faça uma cópia da solução e execute sua configuração e automatize as personalizações de fluxo no ambiente de preparo.</span><span class="sxs-lookup"><span data-stu-id="057e0-159">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>
- <span data-ttu-id="057e0-160">Teste a solução em uma instância de preparo/CRM.</span><span class="sxs-lookup"><span data-stu-id="057e0-160">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="057e0-161">Em caso de sucesso, importe como solução gerenciada para a instância de produção.</span><span class="sxs-lookup"><span data-stu-id="057e0-161">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="057e0-162">Configurar a solução</span><span class="sxs-lookup"><span data-stu-id="057e0-162">Configure the solution</span></span>

1. <span data-ttu-id="057e0-163">Depois de instalar a solução em sua instância do CRM, navegue de volta para o [Power Automate](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="057e0-163">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="057e0-164">Na lista suspensa **ambientes** no canto superior direito, selecione a instância de CRM na qual você instalou a solução de automatização de energia.</span><span class="sxs-lookup"><span data-stu-id="057e0-164">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="057e0-165">Você precisará criar conexões que associem as três contas de usuário:</span><span class="sxs-lookup"><span data-stu-id="057e0-165">You'll need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="057e0-166">Usuário do Partner Center com credenciais de administrador de referências</span><span class="sxs-lookup"><span data-stu-id="057e0-166">Partner Center user with referrals admin credentials</span></span>

   - <span data-ttu-id="057e0-167">Eventos do Partner Center</span><span class="sxs-lookup"><span data-stu-id="057e0-167">Partner Center Events</span></span>

   - <span data-ttu-id="057e0-168">Administrador de CRM com os fluxos de energia automatizada na solução.</span><span class="sxs-lookup"><span data-stu-id="057e0-168">CRM admin with the Power Automate flows in the solution.</span></span>

      1. <span data-ttu-id="057e0-169">Selecione **conexões** na barra de navegação à esquerda e selecione a solução "referências do Partner Center" na lista.</span><span class="sxs-lookup"><span data-stu-id="057e0-169">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>

      2. <span data-ttu-id="057e0-170">Crie uma conexão clicando em **criar uma conexão**.</span><span class="sxs-lookup"><span data-stu-id="057e0-170">Create a connection by clicking **Create a connection**.</span></span>

         :::image type="content" source="images/cosellconnectors/createconnection.png" alt-text="Criar conexão":::

      3. <span data-ttu-id="057e0-172">Procure por **referências do Partner Center (versão prévia)** na barra de pesquisa no canto superior direito.</span><span class="sxs-lookup"><span data-stu-id="057e0-172">Search for **Partner Center Referrals (preview)** in the search bar on the top-right corner.</span></span>

      4. <span data-ttu-id="057e0-173">Crie uma conexão para o usuário do Partner Center com a função de credenciais do administrador de referências.</span><span class="sxs-lookup"><span data-stu-id="057e0-173">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

      5. <span data-ttu-id="057e0-174">Em seguida, crie uma conexão de eventos do Partner Center para o usuário do Partner Center com as credenciais do administrador de referências.</span><span class="sxs-lookup"><span data-stu-id="057e0-174">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

      6. <span data-ttu-id="057e0-175">Crie uma conexão para Common Data Service (ambiente atual) para o usuário administrador do CRM.</span><span class="sxs-lookup"><span data-stu-id="057e0-175">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

4. <span data-ttu-id="057e0-176">Para associar os fluxos de energia automatizada com as conexões, edite cada um dos fluxos de energia automatizada para se conectar às referências do Common Data Service e do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="057e0-176">To associate the Power Automate flows with the connections, edit each of the Power Automate flows to connect to Common Data Service and Partner Center Referrals.</span></span> <span data-ttu-id="057e0-177">Salve as alterações.</span><span class="sxs-lookup"><span data-stu-id="057e0-177">Save the changes.</span></span>

5. <span data-ttu-id="057e0-178">**Ative** os fluxos de energia automatizada.</span><span class="sxs-lookup"><span data-stu-id="057e0-178">**Turn on** the Power Automate flows.</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="057e0-179">Usar APIs de webhook para registrar eventos de alteração de recurso</span><span class="sxs-lookup"><span data-stu-id="057e0-179">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="057e0-180">As APIs de webhook do Partner Center permitem que você se registre em eventos de alteração de recursos.</span><span class="sxs-lookup"><span data-stu-id="057e0-180">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="057e0-181">Esses eventos de alteração são enviados para a URL como postagens HTTP.</span><span class="sxs-lookup"><span data-stu-id="057e0-181">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="057e0-182">Para registrar sua URL, selecione o **registro do webhook do Partner Center (insider Preview)** fluxo automatizado de energia.</span><span class="sxs-lookup"><span data-stu-id="057e0-182">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="057e0-183">Adicionar conexões para (a) Usuário do Partner Center com as referências credenciais de administrador (b.) Eventos do Partner Center conforme realçado abaixo</span><span class="sxs-lookup"><span data-stu-id="057e0-183">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Gatilho":::

3. <span data-ttu-id="057e0-185">Ao fazer essas atualizações, você verá</span><span class="sxs-lookup"><span data-stu-id="057e0-185">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks":::

4. <span data-ttu-id="057e0-187">Salve as alterações e selecione **Ativar**.</span><span class="sxs-lookup"><span data-stu-id="057e0-187">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="057e0-188">Para habilitar o parceiro do Partner Center a ouvir as alterações de evento, execute as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="057e0-188">To enable Partner Center webhooks to listen to event changes, do the following steps:</span></span>

5. <span data-ttu-id="057e0-189">Selecione **Partner Center para Dynamics 365 (insider Preview)**.</span><span class="sxs-lookup"><span data-stu-id="057e0-189">Select **Partner Center to Dynamics 365 (Insider Preview)**.</span></span>

6. <span data-ttu-id="057e0-190">Selecione o ícone **Editar** e selecione **quando uma solicitação HTTP é recebida**.</span><span class="sxs-lookup"><span data-stu-id="057e0-190">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="057e0-191">Selecione o ícone de **cópia** para copiar a URL de postagem http fornecida.</span><span class="sxs-lookup"><span data-stu-id="057e0-191">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="Copiar URL":::

8. <span data-ttu-id="057e0-193">Agora, selecione o fluxo "registro do webhook do Partner Center (insider Preview)" automatizar fluxos de energia e selecione **executar**.</span><span class="sxs-lookup"><span data-stu-id="057e0-193">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="057e0-194">Verifique se a janela "executar fluxo" é aberta no painel direito e clique em **continuar**.</span><span class="sxs-lookup"><span data-stu-id="057e0-194">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="057e0-195">Insira os seguintes detalhes:</span><span class="sxs-lookup"><span data-stu-id="057e0-195">Enter the following details:</span></span>

    1. <span data-ttu-id="057e0-196">**Ponto de extremidade de gatilho http**: URL copiada da etapa anterior</span><span class="sxs-lookup"><span data-stu-id="057e0-196">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="057e0-197">**Eventos a serem registrados**: "referência criada" e "referência atualizada"</span><span class="sxs-lookup"><span data-stu-id="057e0-197">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    3. <span data-ttu-id="057e0-198">**Substituir pontos de extremidade de gatilho existentes, se presente**: Sim (isso substitui todos os pontos de extremidade existentes.)</span><span class="sxs-lookup"><span data-stu-id="057e0-198">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="057e0-199">Selecione **executar** e, em seguida, selecione **concluído.**</span><span class="sxs-lookup"><span data-stu-id="057e0-199">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="057e0-200">O webhook agora pode escutar criar e atualizar eventos.</span><span class="sxs-lookup"><span data-stu-id="057e0-200">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="057e0-201">Personalizar etapas de sincronização</span><span class="sxs-lookup"><span data-stu-id="057e0-201">Customize synchronization steps</span></span>

<span data-ttu-id="057e0-202">Quando as referências de venda cruzada são sincronizadas entre o Partner Center e o sistema CRM, os campos sincronizados no PC do Partner Center são listados aqui.</span><span class="sxs-lookup"><span data-stu-id="057e0-202">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="057e0-203">Geralmente, os sistemas CRM são altamente personalizados.</span><span class="sxs-lookup"><span data-stu-id="057e0-203">Often CRM systems are highly customized.</span></span> <span data-ttu-id="057e0-204">Você pode personalizar os fluxos de energia automatizada.</span><span class="sxs-lookup"><span data-stu-id="057e0-204">You can customize the Power Automate flows.</span></span> <span data-ttu-id="057e0-205">Siga o guia de mapeamento de campo e, se necessário, faça as alterações apropriadas nas etapas de fluxos de energia automatizar.</span><span class="sxs-lookup"><span data-stu-id="057e0-205">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="057e0-206">Os mapeamentos do Microsoft Partner centers para CRM são fornecidos, mas com base no seu ambiente de CRM, você pode optar por personalizar ainda mais os campos.</span><span class="sxs-lookup"><span data-stu-id="057e0-206">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="057e0-207">Várias etapas de cada um dos fluxos de energia automatizada podem ser personalizadas com base em suas necessidades.</span><span class="sxs-lookup"><span data-stu-id="057e0-207">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="057e0-208">Veja a seguir exemplos de personalizações disponíveis:</span><span class="sxs-lookup"><span data-stu-id="057e0-208">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="057e0-209">Para personalizar os campos de criação ou atualização de eventos no Partner Center para a sincronização de referência do CRM:</span><span class="sxs-lookup"><span data-stu-id="057e0-209">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="057e0-210">a.</span><span class="sxs-lookup"><span data-stu-id="057e0-210">a.</span></span> <span data-ttu-id="057e0-211">Selecione Partner Center para Dynamics 365 (insider Preview) ou Partner Center para Salesforce (insider Preview).</span><span class="sxs-lookup"><span data-stu-id="057e0-211">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

    <span data-ttu-id="057e0-212">b.</span><span class="sxs-lookup"><span data-stu-id="057e0-212">b.</span></span> <span data-ttu-id="057e0-213">Selecione **Editar** para editar/personalizar o fluxo de automatização de energia.</span><span class="sxs-lookup"><span data-stu-id="057e0-213">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="057e0-214">c.</span><span class="sxs-lookup"><span data-stu-id="057e0-214">c.</span></span> <span data-ttu-id="057e0-215">Selecione **(escopo) sincronizar o cliente potencial ou a oportunidade**.</span><span class="sxs-lookup"><span data-stu-id="057e0-215">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="057e0-216">Para personalizar mapeamentos de campo de CRM (com base no guia mapeamentos de campo) para criar eventos, selecione **se for nova oportunidade compartilhada e, em seguida,**.</span><span class="sxs-lookup"><span data-stu-id="057e0-216">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="057e0-217">Selecione a subetapa **se sim** e, em seguida, expanda **criando uma nova oportunidade no CRM**.</span><span class="sxs-lookup"><span data-stu-id="057e0-217">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="057e0-218">Você pode editar os mapeamentos nesta seção usando o guia de mapeamento de campos.</span><span class="sxs-lookup"><span data-stu-id="057e0-218">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="057e0-219">d.</span><span class="sxs-lookup"><span data-stu-id="057e0-219">d.</span></span> <span data-ttu-id="057e0-220">Para personalizar os mapeamentos de campo do CRM (com base no guia mapeamentos de campo) para eventos de atualização, clique na etapa "(escopo) sincronizar o cliente potencial ou a oportunidade".</span><span class="sxs-lookup"><span data-stu-id="057e0-220">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="057e0-221">e.</span><span class="sxs-lookup"><span data-stu-id="057e0-221">e.</span></span> <span data-ttu-id="057e0-222">Selecione **se for uma atualização para uma oportunidade e, em seguida,**.</span><span class="sxs-lookup"><span data-stu-id="057e0-222">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="057e0-223">Selecione a subetapa **se sim** e, em seguida, expanda **se a diferença entre os objetos de oportunidade no Partner Center e no CRM, em seguida**.</span><span class="sxs-lookup"><span data-stu-id="057e0-223">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

    <span data-ttu-id="057e0-224">f.</span><span class="sxs-lookup"><span data-stu-id="057e0-224">f.</span></span> <span data-ttu-id="057e0-225">Selecione **se sim** seguido de **Atualizar oportunidade existente**</span><span class="sxs-lookup"><span data-stu-id="057e0-225">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="057e0-226">Para personalizar os campos de sincronização de referência do CRM para PC para eventos de atualização:</span><span class="sxs-lookup"><span data-stu-id="057e0-226">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="057e0-227">a.</span><span class="sxs-lookup"><span data-stu-id="057e0-227">a.</span></span> <span data-ttu-id="057e0-228">Selecione **Editar** para editar/personalizar o fluxo de automatização de energia.</span><span class="sxs-lookup"><span data-stu-id="057e0-228">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="057e0-229">b.</span><span class="sxs-lookup"><span data-stu-id="057e0-229">b.</span></span> <span data-ttu-id="057e0-230">Selecione **(escopo) sincronizar a oportunidade**.</span><span class="sxs-lookup"><span data-stu-id="057e0-230">Select **(Scope) Synchronize the opportunity**.</span></span>

    <span data-ttu-id="057e0-231">c.</span><span class="sxs-lookup"><span data-stu-id="057e0-231">c.</span></span> <span data-ttu-id="057e0-232">Para personalizar mapeamentos de campo de CRM para eventos de atualização, selecione **se houver diferença entre os objetos de cliente potencial no Partner Center e no CRM**.</span><span class="sxs-lookup"><span data-stu-id="057e0-232">To customize CRM field mappings for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span> 

    <span data-ttu-id="057e0-233">d.</span><span class="sxs-lookup"><span data-stu-id="057e0-233">d.</span></span> <span data-ttu-id="057e0-234">Selecione a subetapa **se sim** e, em seguida, expanda a etapa **atualizar uma referência com dados de oportunidade**.</span><span class="sxs-lookup"><span data-stu-id="057e0-234">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="057e0-235">Você pode editar os mapeamentos nesta seção com base no guia de mapeamento de campos.</span><span class="sxs-lookup"><span data-stu-id="057e0-235">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="057e0-236">Para personalizar os campos para a sincronização de referência do CRM para PC para criar eventos?</span><span class="sxs-lookup"><span data-stu-id="057e0-236">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="057e0-237">a.</span><span class="sxs-lookup"><span data-stu-id="057e0-237">a.</span></span> <span data-ttu-id="057e0-238">Selecione **Editar** para editar/personalizar o fluxo de automatização de energia.</span><span class="sxs-lookup"><span data-stu-id="057e0-238">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="057e0-239">b.</span><span class="sxs-lookup"><span data-stu-id="057e0-239">b.</span></span> <span data-ttu-id="057e0-240">Selecione **(escopo) sincronizando referências.**</span><span class="sxs-lookup"><span data-stu-id="057e0-240">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="057e0-241">c.</span><span class="sxs-lookup"><span data-stu-id="057e0-241">c.</span></span> <span data-ttu-id="057e0-242">Para personalizar mapeamentos de campo de CRM (com base no guia mapeamentos de campo) para criar eventos, selecione **criar referência da Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="057e0-242">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

   <span data-ttu-id="057e0-243">Você pode editar os mapeamentos nesta seção com base no guia de mapeamento de campos.</span><span class="sxs-lookup"><span data-stu-id="057e0-243">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="057e0-244">Sincronização de referência de cooperação bidirecional de ponta a ponta</span><span class="sxs-lookup"><span data-stu-id="057e0-244">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="057e0-245">Depois de instalar, configurar e personalizar a solução de automatização de energia, você pode testar a sincronização de referências de venda entre o Dynamics 365 e o Partner Center.</span><span class="sxs-lookup"><span data-stu-id="057e0-245">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="057e0-246">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="057e0-246">Pre-requisites</span></span>

<span data-ttu-id="057e0-247">Para sincronizar as referências no Partner Center e no Dynamics 365 CRM, a solução de energia automatizada claramente demarcates os campos de referência específicos da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="057e0-247">To synchronize the referrals across Partner Center and Dynamics 365 CRM, the Power Automate solution clearly demarcates Microsoft-specific referral fields.</span></span> <span data-ttu-id="057e0-248">Essa identificação fornece às equipes do vendedor a capacidade de decidir quais referências eles desejam compartilhar com a Microsoft para fazer a venda.</span><span class="sxs-lookup"><span data-stu-id="057e0-248">This identification gives your seller teams  the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="057e0-249">Um conjunto de campos personalizados está disponível como parte da entidade **oportunidade** .</span><span class="sxs-lookup"><span data-stu-id="057e0-249">A set of custom fields is available as part of the **Opportunity** entity.</span></span> <span data-ttu-id="057e0-250">Um usuário administrador de CRM precisará criar uma seção de CRM separada com os campos personalizados de **oportunidade** .</span><span class="sxs-lookup"><span data-stu-id="057e0-250">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="057e0-251">Os campos personalizados a seguir devem fazer parte da seção CRM:</span><span class="sxs-lookup"><span data-stu-id="057e0-251">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="057e0-252">**Sincronizar com o Partner Center**: se deseja sincronizar a oportunidade com o Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="057e0-252">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="057e0-253">**Identificador de referência**: um campo de identificador somente leitura para a referência do Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="057e0-253">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="057e0-254">**Link de referência**: um link somente leitura para a referência no Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="057e0-254">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="057e0-255">**Como a Microsoft pode ajudar?**: ajuda necessária da Microsoft para a referência</span><span class="sxs-lookup"><span data-stu-id="057e0-255">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="057e0-256">**Produtos**: lista de produtos associados a esta oportunidade</span><span class="sxs-lookup"><span data-stu-id="057e0-256">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="057e0-257">**Auditoria**: uma trilha de auditoria somente leitura para sincronização com as referências do Partner Center</span><span class="sxs-lookup"><span data-stu-id="057e0-257">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="057e0-258">EXEMPLOS</span><span class="sxs-lookup"><span data-stu-id="057e0-258">SCENARIOS:</span></span>

1. <span data-ttu-id="057e0-259">Sincronização de referência quando a referência é criada ou atualizada no CRM e sincronizada no Partner Center:</span><span class="sxs-lookup"><span data-stu-id="057e0-259">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="057e0-260">Entre no ambiente do Dynamics 365 CRM com o usuário que tem visibilidade na seção **oportunidade** do CRM.</span><span class="sxs-lookup"><span data-stu-id="057e0-260">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="057e0-261">Verifique se a seção a seguir está presente quando você cria uma "nova oportunidade" no ambiente do Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="057e0-261">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="Oportunidade":::

   3. <span data-ttu-id="057e0-263">Para sincronizar essa oportunidade com o Microsoft Partner Center, certifique-se de definir os seguintes campos no modo de exibição de cartão:</span><span class="sxs-lookup"><span data-stu-id="057e0-263">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="057e0-264">**Sincronizar com o Partner Center**: Sim</span><span class="sxs-lookup"><span data-stu-id="057e0-264">**Sync with Partner Center**: Yes</span></span>

      - <span data-ttu-id="057e0-265">**Como a Microsoft pode ajudar?**: selecione uma das seguintes opções:</span><span class="sxs-lookup"><span data-stu-id="057e0-265">**How can Microsoft help?**: Select from the following:</span></span>

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="Seleções de ajuda":::

      - <span data-ttu-id="057e0-267">**Produtos**: IDs de solução do produto</span><span class="sxs-lookup"><span data-stu-id="057e0-267">**Products**: Solution IDs of the product</span></span>

   4. <span data-ttu-id="057e0-268">Depois que a oportunidade for criada no Dynamics 365 com a opção **sincronizar com o Partner Center** definida como **Sim**, aguarde 10 minutos e entre em sua conta do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="057e0-268">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, and then sign into your Partner Center account.</span></span> <span data-ttu-id="057e0-269">Suas referências serão sincronizadas com o Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="057e0-269">Your referrals will be synchronized with Dynamics 365.</span></span>

   5. <span data-ttu-id="057e0-270">Da mesma forma, para uma oportunidade que tenha a opção "sincronizar com o Partner Center" definida como "Sim", se você atualizar a oportunidade no Dynamics 365 CRM, as alterações serão sincronizadas em sua conta do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="057e0-270">Likewise, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

   6. <span data-ttu-id="057e0-271">As oportunidades sincronizadas com êxito com o Partner Center serão identificadas com ✔ ícone no Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="057e0-271">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="057e0-272">Sincronização de referência quando a referência é criada ou atualizada no Microsoft Partner Center e sincronizada no ambiente do Dynamics 365:</span><span class="sxs-lookup"><span data-stu-id="057e0-272">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="057e0-273">Entre no [painel](https://partner.microsoft.com/dashboard/home)do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="057e0-273">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   2. <span data-ttu-id="057e0-274">Selecione **referências** no menu à esquerda.</span><span class="sxs-lookup"><span data-stu-id="057e0-274">Select **Referrals** from the left-hand menu.</span></span>

   3. <span data-ttu-id="057e0-275">Crie uma nova referência de revenda do Partner Center clicando na opção "novo negócio".</span><span class="sxs-lookup"><span data-stu-id="057e0-275">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

   4. <span data-ttu-id="057e0-276">Entre no ambiente do Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="057e0-276">Sign into your Dynamics 365 CRM environment.</span></span>

   5. <span data-ttu-id="057e0-277">Navegue até **oportunidades abertas**.</span><span class="sxs-lookup"><span data-stu-id="057e0-277">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="057e0-278">A referência criada no Microsoft Partner Center agora está sincronizada no Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="057e0-278">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   6. <span data-ttu-id="057e0-279">Quando você seleciona uma referência sincronizada, os detalhes da exibição do cartão são preenchidos.</span><span class="sxs-lookup"><span data-stu-id="057e0-279">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="057e0-280">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="057e0-280">Next steps</span></span>

- [<span data-ttu-id="057e0-281">Gerenciar clientes potenciais</span><span class="sxs-lookup"><span data-stu-id="057e0-281">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="057e0-282">Gerenciar oportunidades de venda conjunta</span><span class="sxs-lookup"><span data-stu-id="057e0-282">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="057e0-283">Mais informações sobre a plataforma de automatização de energia da Microsoft?</span><span class="sxs-lookup"><span data-stu-id="057e0-283">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/power-automate/)

- [<span data-ttu-id="057e0-284">Webhooks do Partner Center</span><span class="sxs-lookup"><span data-stu-id="057e0-284">Partner Center webhooks</span></span>](https://docs.microsoft.com/partner-center/develop/partner-center-webhooks)