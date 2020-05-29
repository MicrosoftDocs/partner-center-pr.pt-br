---
title: O conector de televenda para o centro de parceiros do Salesforce CRM
ms.topic: article
ms.date: 05/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Sincronize suas referências no Partner Center com seu Salesforce CRM
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: ''
ms.localizationpriority: medium
ms.openlocfilehash: 128ae914ef76ba0e1431b0aa7319442b51677973
ms.sourcegitcommit: c13723216761e60d2b37596efc71f5fdecb30be1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/28/2020
ms.locfileid: "84145100"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="2448b-103">Conector de venda conjunta para o Salesforce CRM-visão geral</span><span class="sxs-lookup"><span data-stu-id="2448b-103">Co-sell connector for Salesforce CRM - overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="2448b-104">Funções apropriadas</span><span class="sxs-lookup"><span data-stu-id="2448b-104">Appropriate roles</span></span>

- <span data-ttu-id="2448b-105">Administrador de indicações</span><span class="sxs-lookup"><span data-stu-id="2448b-105">Referrals admin</span></span>
- <span data-ttu-id="2448b-106">Administrador do sistema ou personalizador do sistema no CRM</span><span class="sxs-lookup"><span data-stu-id="2448b-106">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="2448b-107">O conector de televenda do Partner Center permite que seus vendedores covendam-se com a Microsoft de dentro de seus sistemas de CRM.</span><span class="sxs-lookup"><span data-stu-id="2448b-107">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="2448b-108">Eles não precisarão ser treinados para usar o Partner Center para gerenciar acordos de venda.</span><span class="sxs-lookup"><span data-stu-id="2448b-108">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="2448b-109">Usando os conectores de venda conjunta, você pode criar uma nova referência de covenda para envolver um vendedor da Microsoft, receber referências do vendedor da Microsoft, aceitar/recusar referências, modificar dados de negociações, como valor de negócio e data de fechamento.</span><span class="sxs-lookup"><span data-stu-id="2448b-109">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="2448b-110">Você também pode receber todas as atualizações dos vendedores da Microsoft sobre esses acordos de venda conjunta.</span><span class="sxs-lookup"><span data-stu-id="2448b-110">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="2448b-111">Você pode fazer todas as suas referências funcionarem enquanto trabalha no CRM de sua escolha em vez de no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="2448b-111">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="2448b-112">A solução baseia-se na solução de automatização de energia da Microsoft e usa as APIs do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="2448b-112">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>


## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="2448b-113">Antes de instalar-pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2448b-113">Before you install - pre-requisites</span></span>

|<span data-ttu-id="2448b-114">**Tópicos**</span><span class="sxs-lookup"><span data-stu-id="2448b-114">**Topics**</span></span>   |<span data-ttu-id="2448b-115">**Detalhes**</span><span class="sxs-lookup"><span data-stu-id="2448b-115">**Details**</span></span>   |<span data-ttu-id="2448b-116">**Links**</span><span class="sxs-lookup"><span data-stu-id="2448b-116">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="2448b-117">ID de Microsoft Partner Network</span><span class="sxs-lookup"><span data-stu-id="2448b-117">Microsoft Partner Network ID</span></span> |<span data-ttu-id="2448b-118">Você precisa de uma ID de MPN válida</span><span class="sxs-lookup"><span data-stu-id="2448b-118">You need a valid MPN ID</span></span>|<span data-ttu-id="2448b-119">Para ingressar no [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="2448b-119">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="2448b-120">Co-venda pronta</span><span class="sxs-lookup"><span data-stu-id="2448b-120">Co-sell ready</span></span>|<span data-ttu-id="2448b-121">Sua solução de IP/serviços deve estar pronta para venda.</span><span class="sxs-lookup"><span data-stu-id="2448b-121">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="2448b-122">Venda com a Microsoft</span><span class="sxs-lookup"><span data-stu-id="2448b-122">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="2448b-123">Conta do Partner Center</span><span class="sxs-lookup"><span data-stu-id="2448b-123">Partner Center account</span></span>|<span data-ttu-id="2448b-124">A ID de MPN associada ao locatário do Partner Center deve ser a mesma que a ID do MPN associada à sua solução de venda conjunta.</span><span class="sxs-lookup"><span data-stu-id="2448b-124">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="2448b-125">Verifique se você pode ver suas referências de venda conjunta no portal do Partner Center antes de implantar os conectores.</span><span class="sxs-lookup"><span data-stu-id="2448b-125">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="2448b-126">Gerenciar sua conta</span><span class="sxs-lookup"><span data-stu-id="2448b-126">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="2448b-127">Funções de usuário da Central de parceiros</span><span class="sxs-lookup"><span data-stu-id="2448b-127">Partner Center user roles</span></span>|<span data-ttu-id="2448b-128">O funcionário que irá instalar e usar os conectores deve ser um administrador de referências</span><span class="sxs-lookup"><span data-stu-id="2448b-128">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="2448b-129">Atribuir permissões e funções de usuários</span><span class="sxs-lookup"><span data-stu-id="2448b-129">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="2448b-130">CRM do Salesforce</span><span class="sxs-lookup"><span data-stu-id="2448b-130">Salesforce CRM</span></span>|<span data-ttu-id="2448b-131">A função de usuário CRM é administrador do sistema ou personalizador do sistema</span><span class="sxs-lookup"><span data-stu-id="2448b-131">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="2448b-132">Atribuir funções no Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="2448b-132">Assign roles in Salesforce CRM</span></span>](https://docs.microsoft.com/SalesforceCRM/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="2448b-133">Conta de fluxo de automatização de energia</span><span class="sxs-lookup"><span data-stu-id="2448b-133">Power Automate Flow Account</span></span>|<span data-ttu-id="2448b-134">Uma conta de [energia ativa automatizada](https://flow.microsoft.com) para o administrador do sistema do CRM ou o personalizador do sistema.</span><span class="sxs-lookup"><span data-stu-id="2448b-134">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="2448b-135">Esse usuário deve entrar no [Power Automate](https://flow.microsoft.com) pelo menos uma vez antes da instalação.</span><span class="sxs-lookup"><span data-stu-id="2448b-135">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="2448b-136">Instalar a sincronização de referências do Partner Center para o Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="2448b-136">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="2448b-137">Vá para [energia automatizada](https://flow.microsoft.com) e selecione **ambientes** no canto superior direito.</span><span class="sxs-lookup"><span data-stu-id="2448b-137">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="2448b-138">Isso mostrará as instâncias do CRM disponíveis.</span><span class="sxs-lookup"><span data-stu-id="2448b-138">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="2448b-139">Selecione a instância apropriada do CRM na lista suspensa no canto superior direito.</span><span class="sxs-lookup"><span data-stu-id="2448b-139">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span> 

3. <span data-ttu-id="2448b-140">Selecione **soluções** na barra de navegação à esquerda.</span><span class="sxs-lookup"><span data-stu-id="2448b-140">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="2448b-141">Clique no link **abrir AppSource** no menu superior.</span><span class="sxs-lookup"><span data-stu-id="2448b-141">Click on the **Open AppSource** link on the top menu.</span></span>

![Abrir AppSource](images/cosellconnectors/openappsource.png)

5. <span data-ttu-id="2448b-143">Procure **conectores de referências do Partner Center para Salesforce** na tela pop-up.</span><span class="sxs-lookup"><span data-stu-id="2448b-143">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

![Salesforce](images/salesforce/salesforce1.png)

6. <span data-ttu-id="2448b-145">Clique no botão **obter agora** e em **continuar**.</span><span class="sxs-lookup"><span data-stu-id="2448b-145">Click the **Get it now** button and then **Continue**.</span></span> 

7. <span data-ttu-id="2448b-146">Isso abre a página onde você pode selecionar o ambiente do Salesforce CRM para instalar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2448b-146">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="2448b-147">Concorde com os termos e condições.</span><span class="sxs-lookup"><span data-stu-id="2448b-147">Agree to terms and conditions.</span></span>

![CRMS disponíveis](images/salesforce/available-crm.png)

8. <span data-ttu-id="2448b-149">Em seguida, você será direcionado para a página **gerenciar suas soluções** .</span><span class="sxs-lookup"><span data-stu-id="2448b-149">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="2448b-150">Navegue até "referências do Partner Center" usando os botões de seta na parte inferior da página.</span><span class="sxs-lookup"><span data-stu-id="2448b-150">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="2448b-151">A **instalação agendada** deve aparecer ao lado da solução de referências do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="2448b-151">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="2448b-152">A instalação levará 10-15 minutos.</span><span class="sxs-lookup"><span data-stu-id="2448b-152">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="2448b-153">Quando a instalação for concluída, navegue de volta para [Power Automate](https://flow.microsoft.com) e selecione **soluções** na área de navegação à esquerda.</span><span class="sxs-lookup"><span data-stu-id="2448b-153">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="2448b-154">Observe que a **sincronização de referências do Partner Center para o Salesforce** está disponível na lista de soluções.</span><span class="sxs-lookup"><span data-stu-id="2448b-154">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="2448b-155">Selecione **sincronização de referências do Partner Center para Salesforce**.</span><span class="sxs-lookup"><span data-stu-id="2448b-155">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="2448b-156">Os fluxos e as entidades automatizados de energia a seguir estão disponíveis:</span><span class="sxs-lookup"><span data-stu-id="2448b-156">The following Power Automate flows and entities are available:</span></span>

![Fluxos do Salesforce](images/salesforce/salesforce-flows.png)

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="2448b-158">Prática recomendada: teste antes de entrar no ar</span><span class="sxs-lookup"><span data-stu-id="2448b-158">Best Practice: Test before you go live</span></span>

<span data-ttu-id="2448b-159">Antes de instalar, configurar e personalizar a solução de automatização de energia no ambiente de produção, certifique-se de testar a solução em uma instância de CRM de preparo.</span><span class="sxs-lookup"><span data-stu-id="2448b-159">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="2448b-160">Instale a solução de automatização de energia da Microsoft em uma instância de ambiente de preparo/CRM.</span><span class="sxs-lookup"><span data-stu-id="2448b-160">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="2448b-161">Faça uma cópia da solução e execute sua configuração e automatize as personalizações de fluxo no ambiente de preparo.</span><span class="sxs-lookup"><span data-stu-id="2448b-161">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="2448b-162">Teste a solução em uma instância de preparo/CRM.</span><span class="sxs-lookup"><span data-stu-id="2448b-162">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="2448b-163">Em caso de sucesso, importe como solução gerenciada para a instância de produção.</span><span class="sxs-lookup"><span data-stu-id="2448b-163">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="2448b-164">Configurar a solução</span><span class="sxs-lookup"><span data-stu-id="2448b-164">Configure the solution</span></span>

1. <span data-ttu-id="2448b-165">Depois de instalar a solução em sua instância do CRM, navegue de volta para o [Power Automate](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="2448b-165">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="2448b-166">Na lista suspensa **ambientes** no canto superior direito, selecione a instância de CRM na qual você instalou a solução de automatização de energia.</span><span class="sxs-lookup"><span data-stu-id="2448b-166">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="2448b-167">Será necessário criar conexões que associem as três contas de usuário:</span><span class="sxs-lookup"><span data-stu-id="2448b-167">You will need to create connections that associate the three user accounts:</span></span> 

- <span data-ttu-id="2448b-168">Usuário do Partner Center com credenciais de administrador de referências</span><span class="sxs-lookup"><span data-stu-id="2448b-168">Partner Center user with referrals admin credentials</span></span> 
- <span data-ttu-id="2448b-169">Eventos do Partner Center</span><span class="sxs-lookup"><span data-stu-id="2448b-169">Partner Center Events</span></span>
- <span data-ttu-id="2448b-170">Administrador de CRM com os fluxos de energia automatizada na solução.</span><span class="sxs-lookup"><span data-stu-id="2448b-170">CRM admin with the Power Automate flows in the solution.</span></span> 

    <span data-ttu-id="2448b-171">a.</span><span class="sxs-lookup"><span data-stu-id="2448b-171">a.</span></span> <span data-ttu-id="2448b-172">Selecione **conexões** na barra de navegação à esquerda e selecione a solução "referências do Partner Center" na lista.</span><span class="sxs-lookup"><span data-stu-id="2448b-172">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>

    <span data-ttu-id="2448b-173">b.</span><span class="sxs-lookup"><span data-stu-id="2448b-173">b.</span></span> <span data-ttu-id="2448b-174">Crie uma conexão clicando em **criar uma conexão**.</span><span class="sxs-lookup"><span data-stu-id="2448b-174">Create a connection by clicking **Create a connection**.</span></span> 

    ![Criar conexão](images/cosellconnectors/createconnection.png)

    <span data-ttu-id="2448b-176">c.</span><span class="sxs-lookup"><span data-stu-id="2448b-176">c.</span></span> <span data-ttu-id="2448b-177">Procure por **referências do Partner Center (versão prévia)** na barra de pesquisa no canto superior direito.</span><span class="sxs-lookup"><span data-stu-id="2448b-177">Search for **Partner Center Referrals (preview)** in the search bar on the top right corner.</span></span>

    <span data-ttu-id="2448b-178">d.</span><span class="sxs-lookup"><span data-stu-id="2448b-178">d.</span></span> <span data-ttu-id="2448b-179">Crie uma conexão para o usuário do Partner Center com a função de credenciais do administrador de referências.</span><span class="sxs-lookup"><span data-stu-id="2448b-179">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

    <span data-ttu-id="2448b-180">e.</span><span class="sxs-lookup"><span data-stu-id="2448b-180">e.</span></span> <span data-ttu-id="2448b-181">Em seguida, crie uma conexão de eventos do Partner Center para o usuário do Partner Center com as credenciais do administrador de referências.</span><span class="sxs-lookup"><span data-stu-id="2448b-181">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>
    
    <span data-ttu-id="2448b-182">f.</span><span class="sxs-lookup"><span data-stu-id="2448b-182">f.</span></span> <span data-ttu-id="2448b-183">Crie uma conexão para Common Data Service (ambiente atual) para o usuário administrador do CRM.</span><span class="sxs-lookup"><span data-stu-id="2448b-183">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

4. <span data-ttu-id="2448b-184">Para associar os fluxos de energia automatizada com as conexões, edite cada um dos fluxos de energia automatizada para se conectar às referências do Common Data Service e do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="2448b-184">To associate the Power Automate flows with the connections, edit each of the Power Automate flows to connect to Common Data Service and Partner Center Referrals.</span></span> <span data-ttu-id="2448b-185">Salve as alterações.</span><span class="sxs-lookup"><span data-stu-id="2448b-185">Save the changes.</span></span>

5. <span data-ttu-id="2448b-186">**Ative** os fluxos de energia automatizada.</span><span class="sxs-lookup"><span data-stu-id="2448b-186">**Turn on** the the Power Automate flows.</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="2448b-187">Usar APIs de webhook para registrar eventos de alteração de recurso</span><span class="sxs-lookup"><span data-stu-id="2448b-187">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="2448b-188">As APIs de webhook do Partner Center permitem que você se registre em eventos de alteração de recursos.</span><span class="sxs-lookup"><span data-stu-id="2448b-188">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="2448b-189">Esses eventos de alteração são enviados para a URL como postagens HTTP.</span><span class="sxs-lookup"><span data-stu-id="2448b-189">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="2448b-190">Para registrar sua URL, selecione o **registro do webhook do Partner Center (insider Preview)** fluxo automatizado de energia.</span><span class="sxs-lookup"><span data-stu-id="2448b-190">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="2448b-191">Adicionar conexões para (a) Usuário do Partner Center com as referências credenciais de administrador (b.) Eventos do Partner Center conforme realçado abaixo</span><span class="sxs-lookup"><span data-stu-id="2448b-191">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

![Gatilho](images/cosellconnectors/triggerflow.png)

3. <span data-ttu-id="2448b-193">Ao fazer essas atualizações, você verá</span><span class="sxs-lookup"><span data-stu-id="2448b-193">When you make these updates, you'll see</span></span>

![Webhooks](images/cosellconnectors/webhook1.png)

4. <span data-ttu-id="2448b-195">Salve as alterações e selecione **Ativar**.</span><span class="sxs-lookup"><span data-stu-id="2448b-195">Save your changes and select **Turn on**.</span></span> 

<span data-ttu-id="2448b-196">Para habilitar o parceiro do Partner Center a ouvir as alterações de evento, execute as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="2448b-196">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="2448b-197">Selecione **Partner Center para SALESFORCE CRM (insider Preview)**.</span><span class="sxs-lookup"><span data-stu-id="2448b-197">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="2448b-198">Selecione o ícone **Editar** e selecione **quando uma solicitação HTTP é recebida**.</span><span class="sxs-lookup"><span data-stu-id="2448b-198">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="2448b-199">Selecione o ícone de **cópia** para copiar a URL de postagem http fornecida.</span><span class="sxs-lookup"><span data-stu-id="2448b-199">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

![Copiar URL](images/salesforce/copy-url.png)

8. <span data-ttu-id="2448b-201">Agora, selecione o fluxo "registro do webhook do Partner Center (insider Preview)" automatizar fluxos de energia e selecione **executar**.</span><span class="sxs-lookup"><span data-stu-id="2448b-201">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="2448b-202">Verifique se a janela "executar fluxo" é aberta no painel direito e clique em **continuar**.</span><span class="sxs-lookup"><span data-stu-id="2448b-202">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="2448b-203">Insira os seguintes detalhes:</span><span class="sxs-lookup"><span data-stu-id="2448b-203">Enter the following details:</span></span> 

    <span data-ttu-id="2448b-204">a.</span><span class="sxs-lookup"><span data-stu-id="2448b-204">a.</span></span> <span data-ttu-id="2448b-205">**Ponto de extremidade de gatilho http**: URL copiada da etapa anterior</span><span class="sxs-lookup"><span data-stu-id="2448b-205">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    <span data-ttu-id="2448b-206">b.</span><span class="sxs-lookup"><span data-stu-id="2448b-206">b.</span></span> <span data-ttu-id="2448b-207">**Eventos a serem registrados**: "referência criada" e "referência atualizada"</span><span class="sxs-lookup"><span data-stu-id="2448b-207">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    <span data-ttu-id="2448b-208">c.</span><span class="sxs-lookup"><span data-stu-id="2448b-208">c.</span></span> <span data-ttu-id="2448b-209">**Substituir pontos de extremidade de gatilho existentes, se presente**: Sim (isso substitui todos os pontos de extremidade existentes.)</span><span class="sxs-lookup"><span data-stu-id="2448b-209">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span> 

11. <span data-ttu-id="2448b-210">Selecione **executar** e, em seguida, selecione **concluído.**</span><span class="sxs-lookup"><span data-stu-id="2448b-210">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="2448b-211">O webhook agora pode escutar criar e atualizar eventos.</span><span class="sxs-lookup"><span data-stu-id="2448b-211">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="2448b-212">Personalizar etapas de sincronização</span><span class="sxs-lookup"><span data-stu-id="2448b-212">Customize synchronization steps</span></span>

<span data-ttu-id="2448b-213">Quando as referências de venda cruzada são sincronizadas entre o Partner Center e o sistema CRM, os campos sincronizados no PC do Partner Center são listados aqui.</span><span class="sxs-lookup"><span data-stu-id="2448b-213">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="2448b-214">Geralmente, os sistemas CRM são altamente personalizados.</span><span class="sxs-lookup"><span data-stu-id="2448b-214">Often CRM systems are highly customized.</span></span> <span data-ttu-id="2448b-215">Você pode personalizar os fluxos de energia automatizada.</span><span class="sxs-lookup"><span data-stu-id="2448b-215">You can customize the Power Automate flows.</span></span> <span data-ttu-id="2448b-216">Siga o guia de mapeamento de campo e, se necessário, faça as alterações apropriadas nas etapas de fluxos de energia automatizar.</span><span class="sxs-lookup"><span data-stu-id="2448b-216">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="2448b-217">Os mapeamentos do Microsoft Partner centers para CRM são fornecidos, mas com base no seu ambiente de CRM, você pode optar por personalizar ainda mais os campos.</span><span class="sxs-lookup"><span data-stu-id="2448b-217">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="2448b-218">Várias etapas de cada um dos fluxos de energia automatizada podem ser personalizadas com base em suas necessidades.</span><span class="sxs-lookup"><span data-stu-id="2448b-218">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="2448b-219">Veja a seguir exemplos de personalizações disponíveis:</span><span class="sxs-lookup"><span data-stu-id="2448b-219">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="2448b-220">Para personalizar os campos de criação ou atualização de eventos no Partner Center para a sincronização de referência do CRM:</span><span class="sxs-lookup"><span data-stu-id="2448b-220">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="2448b-221">a.</span><span class="sxs-lookup"><span data-stu-id="2448b-221">a.</span></span> <span data-ttu-id="2448b-222">Selecione Partner Center para Salesforce CRM (insider Preview).</span><span class="sxs-lookup"><span data-stu-id="2448b-222">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

    <span data-ttu-id="2448b-223">b.</span><span class="sxs-lookup"><span data-stu-id="2448b-223">b.</span></span> <span data-ttu-id="2448b-224">Selecione **Editar** para editar/personalizar o fluxo de automatização de energia.</span><span class="sxs-lookup"><span data-stu-id="2448b-224">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="2448b-225">c.</span><span class="sxs-lookup"><span data-stu-id="2448b-225">c.</span></span> <span data-ttu-id="2448b-226">Selecione **(escopo) sincronizar o cliente potencial ou a oportunidade**.</span><span class="sxs-lookup"><span data-stu-id="2448b-226">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="2448b-227">Para personalizar mapeamentos de campo de CRM para criar eventos, selecione **se for nova oportunidade compartilhada e, em seguida,**.</span><span class="sxs-lookup"><span data-stu-id="2448b-227">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="2448b-228">Selecione a subetapa **se sim** e, em seguida, expanda **criando uma nova oportunidade no CRM**.</span><span class="sxs-lookup"><span data-stu-id="2448b-228">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="2448b-229">Você pode editar os mapeamentos nesta seção usando o guia de mapeamento de campos.</span><span class="sxs-lookup"><span data-stu-id="2448b-229">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="2448b-230">d.</span><span class="sxs-lookup"><span data-stu-id="2448b-230">d.</span></span> <span data-ttu-id="2448b-231">Para personalizar mapeamentos de campo de CRM para eventos de atualização, clique na etapa "(escopo) sincronizar o cliente potencial ou a oportunidade".</span><span class="sxs-lookup"><span data-stu-id="2448b-231">To customize CRM field mappings for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="2448b-232">e.</span><span class="sxs-lookup"><span data-stu-id="2448b-232">e.</span></span> <span data-ttu-id="2448b-233">Selecione **se for uma atualização para uma oportunidade e, em seguida,**.</span><span class="sxs-lookup"><span data-stu-id="2448b-233">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="2448b-234">Selecione a subetapa **se sim** e, em seguida, expanda **se a diferença entre os objetos de oportunidade no Partner Center e no CRM, em seguida**.</span><span class="sxs-lookup"><span data-stu-id="2448b-234">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

    <span data-ttu-id="2448b-235">f.</span><span class="sxs-lookup"><span data-stu-id="2448b-235">f.</span></span> <span data-ttu-id="2448b-236">Selecione **se sim** seguido de **Atualizar oportunidade existente**</span><span class="sxs-lookup"><span data-stu-id="2448b-236">Select **If yes** followed with **Update existing opportunity**</span></span>
       
3. <span data-ttu-id="2448b-237">Para personalizar os campos de sincronização de referência do CRM para PC para eventos de atualização:</span><span class="sxs-lookup"><span data-stu-id="2448b-237">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="2448b-238">a.</span><span class="sxs-lookup"><span data-stu-id="2448b-238">a.</span></span> <span data-ttu-id="2448b-239">Selecione **Editar** para editar/personalizar o fluxo de automatização de energia.</span><span class="sxs-lookup"><span data-stu-id="2448b-239">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="2448b-240">b.</span><span class="sxs-lookup"><span data-stu-id="2448b-240">b.</span></span> <span data-ttu-id="2448b-241">Selecione **(escopo) sincronizar a oportunidade**.</span><span class="sxs-lookup"><span data-stu-id="2448b-241">Select **(Scope) Synchronize the opportunity**.</span></span>

    <span data-ttu-id="2448b-242">c.</span><span class="sxs-lookup"><span data-stu-id="2448b-242">c.</span></span> <span data-ttu-id="2448b-243">Para personalizar os mapeamentos de campo do CRM (com base no guia mapeamentos de campo) para eventos de atualização, selecione **se houver diferença entre os objetos Lead no Partner Center e CRM, em seguida**.</span><span class="sxs-lookup"><span data-stu-id="2448b-243">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span> 

    <span data-ttu-id="2448b-244">d.</span><span class="sxs-lookup"><span data-stu-id="2448b-244">d.</span></span> <span data-ttu-id="2448b-245">Selecione a subetapa **se sim** e, em seguida, expanda a etapa **atualizar uma referência com dados de oportunidade**.</span><span class="sxs-lookup"><span data-stu-id="2448b-245">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

<span data-ttu-id="2448b-246">Você pode editar os mapeamentos nesta seção com base no guia de mapeamento de campos.</span><span class="sxs-lookup"><span data-stu-id="2448b-246">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="2448b-247">Para personalizar os campos para a sincronização de referência do CRM para PC para criar eventos?</span><span class="sxs-lookup"><span data-stu-id="2448b-247">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="2448b-248">a.</span><span class="sxs-lookup"><span data-stu-id="2448b-248">a.</span></span> <span data-ttu-id="2448b-249">Selecione **Editar** para editar/personalizar o fluxo de automatização de energia.</span><span class="sxs-lookup"><span data-stu-id="2448b-249">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="2448b-250">b.</span><span class="sxs-lookup"><span data-stu-id="2448b-250">b.</span></span> <span data-ttu-id="2448b-251">Selecione **(escopo) sincronizando referências.**</span><span class="sxs-lookup"><span data-stu-id="2448b-251">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="2448b-252">c.</span><span class="sxs-lookup"><span data-stu-id="2448b-252">c.</span></span> <span data-ttu-id="2448b-253">Para personalizar mapeamentos de campo de CRM (com base no guia mapeamentos de campo) para criar eventos, selecione **criar referência da Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="2448b-253">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span> 

<span data-ttu-id="2448b-254">Você pode editar os mapeamentos nesta seção com base no guia de mapeamento de campos.</span><span class="sxs-lookup"><span data-stu-id="2448b-254">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="create-separate-section-in-salesforce-crm-opportunity-layout"></a><span data-ttu-id="2448b-255">Criar uma seção separada no layout de oportunidade do CRM Salesforce</span><span class="sxs-lookup"><span data-stu-id="2448b-255">Create Separate Section in Salesforce CRM Opportunity Layout</span></span>

<span data-ttu-id="2448b-256">Para sincronizar as referências no Partner Center e no Salesforce CRM, a solução de automatização de energia precisa demarcar claramente os campos de referência específicos da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="2448b-256">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="2448b-257">Isso fornece às suas equipes do vendedor a capacidade de decidir quais referências eles desejam compartilhar com a Microsoft para fazer a venda.</span><span class="sxs-lookup"><span data-stu-id="2448b-257">This provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="2448b-258">Um conjunto de campos personalizados está disponível como parte da sincronização de referências do Partner Center para a entidade de **oportunidade** do Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="2448b-258">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM **Opportunity** entity.</span></span> <span data-ttu-id="2448b-259">Um usuário administrador de CRM precisará criar uma seção de CRM separada com os campos personalizados de **oportunidade** .</span><span class="sxs-lookup"><span data-stu-id="2448b-259">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>
<span data-ttu-id="2448b-260">O usuário administrador do Salesforce CRM precisará criar uma seção de CRM separada.</span><span class="sxs-lookup"><span data-stu-id="2448b-260">Salesforce CRM administrator user will need to create a separate CRM section.</span></span>

<span data-ttu-id="2448b-261">Os campos personalizados a seguir devem fazer parte da seção CRM:</span><span class="sxs-lookup"><span data-stu-id="2448b-261">The following custom fields should be part of the CRM section:</span></span>

<span data-ttu-id="2448b-262">• **Sincronizar com o Partner Center**: se deseja sincronizar a oportunidade com o Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="2448b-262">• **Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

<span data-ttu-id="2448b-263">• **Identificador de referência**: um campo de identificador somente leitura para a referência do Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="2448b-263">• **Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

<span data-ttu-id="2448b-264">• **Link de referência**: um link somente leitura para a referência no Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="2448b-264">• **Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

<span data-ttu-id="2448b-265">• **Como a Microsoft pode ajudar?**</span><span class="sxs-lookup"><span data-stu-id="2448b-265">• **How can Microsoft help?**</span></span> <span data-ttu-id="2448b-266">Ajuda necessária da Microsoft para a referência</span><span class="sxs-lookup"><span data-stu-id="2448b-266">Help required from Microsoft for the referral</span></span>

<span data-ttu-id="2448b-267">• **Produtos**: lista de produtos associados a esta oportunidade</span><span class="sxs-lookup"><span data-stu-id="2448b-267">• **Products**: List of products associated with this opportunity</span></span>

<span data-ttu-id="2448b-268">• **Auditoria**: uma trilha de auditoria somente leitura para sincronizar com a referência do Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="2448b-268">• **Audit**: A read only audit trail for syncing with Microsoft Partner Center referral</span></span>

### <a name="set-up-fields-and-relationships"></a><span data-ttu-id="2448b-269">Configurar campos e relações</span><span class="sxs-lookup"><span data-stu-id="2448b-269">Set up fields and relationships</span></span>

1. <span data-ttu-id="2448b-270">Entre em sua conta do Salesforce e vá para **oportunidade**.</span><span class="sxs-lookup"><span data-stu-id="2448b-270">Sign into your Salesforce account and go to **Opportunity**.</span></span> 

2. <span data-ttu-id="2448b-271">Clique nas opções **Configurar** e **Editar objeto** para adicionar os campos necessários.</span><span class="sxs-lookup"><span data-stu-id="2448b-271">Click on the **Setup** and **Edit Object** options to add the necessary fields.</span></span>


3. <span data-ttu-id="2448b-272">Selecionar **campos & relações** no painel de navegação esquerdo</span><span class="sxs-lookup"><span data-stu-id="2448b-272">Select **Fields & Relationships** from the left navigation</span></span>

![Campos](images/salesforce/fields1.png)

4. <span data-ttu-id="2448b-274">Adicione os seguintes campos na tabela "Fields & relationship":</span><span class="sxs-lookup"><span data-stu-id="2448b-274">Add the following fields in the “Fields & Relationship” table:</span></span>

|<span data-ttu-id="2448b-275">**Rótulo do campo**</span><span class="sxs-lookup"><span data-stu-id="2448b-275">**Field label**</span></span>   |<span data-ttu-id="2448b-276">**Nome do campo**</span><span class="sxs-lookup"><span data-stu-id="2448b-276">**Field name**</span></span>|<span data-ttu-id="2448b-277">**Data type**</span><span class="sxs-lookup"><span data-stu-id="2448b-277">**Data type**</span></span>|<span data-ttu-id="2448b-278">**Indexa**</span><span class="sxs-lookup"><span data-stu-id="2448b-278">**Indexed**</span></span>|
|---------------------|:-------------------|:--------------|:----------------|
|<span data-ttu-id="2448b-279">Sincronizar com o Partner Center</span><span class="sxs-lookup"><span data-stu-id="2448b-279">Sync with Partner Center</span></span>|<span data-ttu-id="2448b-280">sincronizar-com-Partner-Center-c</span><span class="sxs-lookup"><span data-stu-id="2448b-280">sync-with-partner-center-c</span></span>|<span data-ttu-id="2448b-281">Caixa de seleção (padrão desmarcado)</span><span class="sxs-lookup"><span data-stu-id="2448b-281">Checkbox (default unchecked)</span></span>||
|<span data-ttu-id="2448b-282">Produtos</span><span class="sxs-lookup"><span data-stu-id="2448b-282">Products</span></span>|<span data-ttu-id="2448b-283">Produtos-c</span><span class="sxs-lookup"><span data-stu-id="2448b-283">Products-c</span></span>|<span data-ttu-id="2448b-284">texto (255)</span><span class="sxs-lookup"><span data-stu-id="2448b-284">text (255)</span></span>||
|<span data-ttu-id="2448b-285">Indicação</span><span class="sxs-lookup"><span data-stu-id="2448b-285">Referral</span></span> | <span data-ttu-id="2448b-286">Referral_Identifier__c</span><span class="sxs-lookup"><span data-stu-id="2448b-286">Referral_Identifier__c</span></span>|<span data-ttu-id="2448b-287">Texto (100) (ID externa)</span><span class="sxs-lookup"><span data-stu-id="2448b-287">Text(100)(External ID)</span></span>|<span data-ttu-id="2448b-288">sim</span><span class="sxs-lookup"><span data-stu-id="2448b-288">yes</span></span>|
|<span data-ttu-id="2448b-289">Link de referência</span><span class="sxs-lookup"><span data-stu-id="2448b-289">Referral Link</span></span>| <span data-ttu-id="2448b-290">Referral_Link__c_</span><span class="sxs-lookup"><span data-stu-id="2448b-290">Referral_Link__c_</span></span>|<span data-ttu-id="2448b-291">URL (255)</span><span class="sxs-lookup"><span data-stu-id="2448b-291">URL(255)</span></span>||
|<span data-ttu-id="2448b-292">Audit</span><span class="sxs-lookup"><span data-stu-id="2448b-292">Audit</span></span>| <span data-ttu-id="2448b-293">Audit__c</span><span class="sxs-lookup"><span data-stu-id="2448b-293">Audit__c</span></span>|<span data-ttu-id="2448b-294">Área de texto longo (100.000) (linha visível 4)</span><span class="sxs-lookup"><span data-stu-id="2448b-294">Long Text Area(100000)(visible line 4)</span></span>||
|<span data-ttu-id="2448b-295">Como a Microsoft pode ajudar?</span><span class="sxs-lookup"><span data-stu-id="2448b-295">How can Microsoft help?</span></span>|<span data-ttu-id="2448b-296">How_can_Microsoft_help__c</span><span class="sxs-lookup"><span data-stu-id="2448b-296">How_can_Microsoft_help__c</span></span>|<span data-ttu-id="2448b-297">Seleção</span><span class="sxs-lookup"><span data-stu-id="2448b-297">Picklist\*</span></span>|

<span data-ttu-id="2448b-298">\* Valores da lista de seleção:</span><span class="sxs-lookup"><span data-stu-id="2448b-298">\*Picklist values:</span></span>

<span data-ttu-id="2448b-299">• Proposta de valor específico da carga de trabalho</span><span class="sxs-lookup"><span data-stu-id="2448b-299">• Workload specific value proposition</span></span>

<span data-ttu-id="2448b-300">• Arquitetura técnica do cliente</span><span class="sxs-lookup"><span data-stu-id="2448b-300">• Customer technical architecture</span></span>

<span data-ttu-id="2448b-301">• Prova de conceito ou demonstração</span><span class="sxs-lookup"><span data-stu-id="2448b-301">• Proof of concept or demo</span></span>

<span data-ttu-id="2448b-302">• Cotas ou licenciamento</span><span class="sxs-lookup"><span data-stu-id="2448b-302">• Quotes or licensing</span></span>

<span data-ttu-id="2448b-303">• Sucesso do cliente de vendas por postagem</span><span class="sxs-lookup"><span data-stu-id="2448b-303">• Post sales customer success</span></span>

<span data-ttu-id="2448b-304">• Geral ou outros</span><span class="sxs-lookup"><span data-stu-id="2448b-304">• General or other</span></span>

<span data-ttu-id="2448b-305">5. os campos serão criados em "Fields & Relationships"</span><span class="sxs-lookup"><span data-stu-id="2448b-305">5.The fields would get created under “Fields & Relationships”</span></span>

![Campos criados](images/salesforce/fields2.png)

6. <span data-ttu-id="2448b-307">No layout da oportunidade, crie uma seção separada com os campos listados acima.</span><span class="sxs-lookup"><span data-stu-id="2448b-307">In the Opportunity layout, create a separate section with the fields as listed above.</span></span> 

    <span data-ttu-id="2448b-308">• Esta seção deve estar disponível para os vendedores no layout da oportunidade</span><span class="sxs-lookup"><span data-stu-id="2448b-308">• This section should be available for the sellers in the Opportunity layout</span></span>


![Layout de campos do Partner Center](images/salesforce/pc-fields-layout.png)

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="2448b-310">Sincronização de referência de cooperação bidirecional de ponta a ponta</span><span class="sxs-lookup"><span data-stu-id="2448b-310">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="2448b-311">Depois de instalar, configurar e personalizar a solução de automatização de energia, você pode testar a sincronização de referências de venda entre o Salesforce CRM e o Partner Center.</span><span class="sxs-lookup"><span data-stu-id="2448b-311">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="2448b-312">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2448b-312">Pre-requisites</span></span>

<span data-ttu-id="2448b-313">Para sincronizar as referências no Partner Center e no Salesforce CRM, a solução de automatização de energia precisa demarcar claramente os campos de referência específicos da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="2448b-313">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="2448b-314">Essa identificação fornece às suas equipes do vendedor a capacidade de decidir quais referências eles desejam compartilhar com a Microsoft para fazer a venda.</span><span class="sxs-lookup"><span data-stu-id="2448b-314">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="2448b-315">Um conjunto de campos personalizados está disponível como parte da sincronização de referências do Partner Center para a entidade **oportunidade** de solução do Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="2448b-315">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="2448b-316">Um usuário administrador de CRM precisará criar uma seção de CRM separada com os campos personalizados de **oportunidade** .</span><span class="sxs-lookup"><span data-stu-id="2448b-316">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="2448b-317">Os campos personalizados a seguir devem fazer parte da seção CRM:</span><span class="sxs-lookup"><span data-stu-id="2448b-317">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="2448b-318">**Sincronizar com o Partner Center**: se deseja sincronizar a oportunidade com o Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="2448b-318">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="2448b-319">**Identificador de referência**: um campo de identificador somente leitura para a referência do Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="2448b-319">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="2448b-320">**Link de referência**: um link somente leitura para a referência no Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="2448b-320">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="2448b-321">**Como a Microsoft pode ajudar**: a ajuda necessária da Microsoft para a referência</span><span class="sxs-lookup"><span data-stu-id="2448b-321">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="2448b-322">**Produtos**: lista de produtos associados a esta oportunidade</span><span class="sxs-lookup"><span data-stu-id="2448b-322">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="2448b-323">**Auditoria**: uma trilha de auditoria somente leitura para sincronização com as referências do Partner Center</span><span class="sxs-lookup"><span data-stu-id="2448b-323">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>


### <a name="scenarios"></a><span data-ttu-id="2448b-324">EXEMPLOS</span><span class="sxs-lookup"><span data-stu-id="2448b-324">SCENARIOS:</span></span>

1. <span data-ttu-id="2448b-325">Sincronização de referência quando a referência é criada ou atualizada no CRM e sincronizada no Partner Center:</span><span class="sxs-lookup"><span data-stu-id="2448b-325">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

    <span data-ttu-id="2448b-326">a.</span><span class="sxs-lookup"><span data-stu-id="2448b-326">a.</span></span> <span data-ttu-id="2448b-327">Entre no ambiente do Salesforce CRM com o usuário que tem visibilidade na seção **oportunidade** do CRM.</span><span class="sxs-lookup"><span data-stu-id="2448b-327">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

    <span data-ttu-id="2448b-328">b.</span><span class="sxs-lookup"><span data-stu-id="2448b-328">b.</span></span> <span data-ttu-id="2448b-329">Verifique se a seção a seguir está presente quando você cria uma "nova oportunidade" no ambiente CRM do Salesforce</span><span class="sxs-lookup"><span data-stu-id="2448b-329">Ensure that the following section is present when you create a “New Opportunity” in Salesforce CRM environment</span></span>

    ![Ambiente do Salesforce](images/salesforce/salesforce-scenario-1.png)

   

    <span data-ttu-id="2448b-331">c.</span><span class="sxs-lookup"><span data-stu-id="2448b-331">c.</span></span> <span data-ttu-id="2448b-332">Para sincronizar essa oportunidade com o Microsoft Partner Center, certifique-se de definir os seguintes campos no modo de exibição de cartão:</span><span class="sxs-lookup"><span data-stu-id="2448b-332">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

    - <span data-ttu-id="2448b-333">"Sincronizar com o Partner Center": Sim</span><span class="sxs-lookup"><span data-stu-id="2448b-333">“Sync with Partner Center”: Yes</span></span>

    - <span data-ttu-id="2448b-334">"Como a Microsoft pode ajudar?": selecione uma das seguintes opções:</span><span class="sxs-lookup"><span data-stu-id="2448b-334">"How can Microsoft help?”: Select from the following options:</span></span>

   

    - <span data-ttu-id="2448b-335">Produtos: IDs de solução do produto</span><span class="sxs-lookup"><span data-stu-id="2448b-335">Products: Solution IDs of the product</span></span>

    <span data-ttu-id="2448b-336">d.</span><span class="sxs-lookup"><span data-stu-id="2448b-336">d.</span></span> <span data-ttu-id="2448b-337">Depois de definir a opção sincronização de oportunidade **com o Partner Center** como **Sim**, aguarde 10 minutos e entre em sua conta do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="2448b-337">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="2448b-338">Suas referências serão sincronizadas com o Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="2448b-338">Your referrals will be synchronized with Salesforce CRM.</span></span>

    <span data-ttu-id="2448b-339">e.</span><span class="sxs-lookup"><span data-stu-id="2448b-339">e.</span></span> <span data-ttu-id="2448b-340">Quando a opção "sincronizar com o Partner Center" for definida como "Sim", se você atualizar a oportunidade no Salesforce CRM, as alterações serão sincronizadas com sua conta do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="2448b-340">When the “Sync with Partner Center” option is set to “Yes”, if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

    <span data-ttu-id="2448b-341">f.</span><span class="sxs-lookup"><span data-stu-id="2448b-341">f.</span></span> <span data-ttu-id="2448b-342">As oportunidades sincronizadas com êxito com o Partner Center serão identificadas com ✔ ícone no Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="2448b-342">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="2448b-343">Sincronização de referência quando a referência é criada ou atualizada no Microsoft Partner Center e sincronizada no ambiente do Salesforce CRM:</span><span class="sxs-lookup"><span data-stu-id="2448b-343">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span> 

    <span data-ttu-id="2448b-344">a.</span><span class="sxs-lookup"><span data-stu-id="2448b-344">a.</span></span> <span data-ttu-id="2448b-345">Entre no [painel](https://partner.microsoft.com/dashboard/home)do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="2448b-345">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    <span data-ttu-id="2448b-346">b.</span><span class="sxs-lookup"><span data-stu-id="2448b-346">b.</span></span> <span data-ttu-id="2448b-347">Selecione **referências** no menu à esquerda.</span><span class="sxs-lookup"><span data-stu-id="2448b-347">Select **Referrals** from the left-hand menu.</span></span>

    <span data-ttu-id="2448b-348">c.</span><span class="sxs-lookup"><span data-stu-id="2448b-348">c.</span></span> <span data-ttu-id="2448b-349">Crie uma nova referência de revenda do Partner Center clicando na opção "novo negócio".</span><span class="sxs-lookup"><span data-stu-id="2448b-349">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

    <span data-ttu-id="2448b-350">d.</span><span class="sxs-lookup"><span data-stu-id="2448b-350">d.</span></span> <span data-ttu-id="2448b-351">Entre no ambiente do Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="2448b-351">Sign into your Salesforce CRM environment.</span></span> 

    <span data-ttu-id="2448b-352">e.</span><span class="sxs-lookup"><span data-stu-id="2448b-352">e.</span></span> <span data-ttu-id="2448b-353">Navegue até **oportunidades abertas**.</span><span class="sxs-lookup"><span data-stu-id="2448b-353">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="2448b-354">A referência criada no Microsoft Partner Center agora está sincronizada no Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="2448b-354">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

    ![Tela de oportunidade do Salesforce](images/salesforce/salesforce-casino-e.png)

    <span data-ttu-id="2448b-356">f.</span><span class="sxs-lookup"><span data-stu-id="2448b-356">f.</span></span> <span data-ttu-id="2448b-357">Quando você seleciona uma referência sincronizada, os detalhes da exibição do cartão são preenchidos.</span><span class="sxs-lookup"><span data-stu-id="2448b-357">When you select a synchronized referral, the card view details are populated.</span></span>





## <a name="next-steps"></a><span data-ttu-id="2448b-358">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="2448b-358">Next steps</span></span>

- [<span data-ttu-id="2448b-359">Mais informações sobre a plataforma de automatização de energia da Microsoft?</span><span class="sxs-lookup"><span data-stu-id="2448b-359">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/-automate/)

- [<span data-ttu-id="2448b-360">Gerenciar clientes potenciais</span><span class="sxs-lookup"><span data-stu-id="2448b-360">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="2448b-361">Gerenciar oportunidades de venda conjunta</span><span class="sxs-lookup"><span data-stu-id="2448b-361">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="2448b-362">Webhooks do Partner Center</span><span class="sxs-lookup"><span data-stu-id="2448b-362">Partner Center webhooks</span></span>](https://docs.microsoft.com/partner-center/develop/partner-center-webhooks)