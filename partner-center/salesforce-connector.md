---
title: O conector de televenda para o centro de parceiros do Salesforce CRM
ms.topic: article
ms.date: 05/22/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Usando o conector CRM do Salesforce, obtenha referências da Microsoft
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: ''
ms.localizationpriority: medium
ms.openlocfilehash: ad39bdde92611066d0dd0c56d8b9133f4d9dcaa9
ms.sourcegitcommit: 97f1ff7386562cbb945bdfbcf15c85bc8303cac2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2020
ms.locfileid: "83825693"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="8a53d-103">Conector de venda conjunta para o Salesforce CRM-visão geral</span><span class="sxs-lookup"><span data-stu-id="8a53d-103">Co-sell connector for Salesforce CRM - overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="8a53d-104">Funções apropriadas</span><span class="sxs-lookup"><span data-stu-id="8a53d-104">Appropriate roles</span></span>

- <span data-ttu-id="8a53d-105">Administrador de indicações</span><span class="sxs-lookup"><span data-stu-id="8a53d-105">Referrals admin</span></span>
- <span data-ttu-id="8a53d-106">Administrador do sistema ou personalizador do sistema no CRM</span><span class="sxs-lookup"><span data-stu-id="8a53d-106">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="8a53d-107">O conector de televenda do Partner Center permite que seus vendedores covendam-se com a Microsoft de dentro de seus sistemas de CRM.</span><span class="sxs-lookup"><span data-stu-id="8a53d-107">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="8a53d-108">Eles não precisarão ser treinados para usar o Partner Center para gerenciar acordos de venda.</span><span class="sxs-lookup"><span data-stu-id="8a53d-108">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="8a53d-109">Usando os conectores de televenda, você poderá criar uma nova referência de cooperação para envolver um vendedor da Microsoft, receber referências do vendedor da Microsoft, aceitar/recusar referências, modificar dados de negociações, como valor de negócio, data de fechamento, etc., além de receber quaisquer atualizações dos vendedores da Microsoft nessas negociações de venda.</span><span class="sxs-lookup"><span data-stu-id="8a53d-109">Using the Co-sell connectors, you will be able to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, closing date etc. as well as receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="8a53d-110">Você pode fazer tudo isso enquanto trabalha no CRM de sua escolha, em vez de no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="8a53d-110">You can do all of this while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="8a53d-111">A solução baseia-se na solução de automatização de energia da Microsoft e usa as APIs do Microsoft Partner Center.</span><span class="sxs-lookup"><span data-stu-id="8a53d-111">The solution is based on Microsoft Power Automate Solution and uses Microsoft Partner Center APIs.</span></span>


## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="8a53d-112">Antes de instalar-pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8a53d-112">Before you install - pre-requisites</span></span>

|<span data-ttu-id="8a53d-113">**Tópicos**</span><span class="sxs-lookup"><span data-stu-id="8a53d-113">**Topics**</span></span>   |<span data-ttu-id="8a53d-114">**Detalhes**</span><span class="sxs-lookup"><span data-stu-id="8a53d-114">**Details**</span></span>   |<span data-ttu-id="8a53d-115">**Links**</span><span class="sxs-lookup"><span data-stu-id="8a53d-115">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="8a53d-116">ID de Microsoft Partner Network</span><span class="sxs-lookup"><span data-stu-id="8a53d-116">Microsoft Partner Network ID</span></span> |<span data-ttu-id="8a53d-117">Você precisa de uma ID de MPN válida</span><span class="sxs-lookup"><span data-stu-id="8a53d-117">You need a valid MPN ID</span></span>|<span data-ttu-id="8a53d-118">Para ingressar no [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="8a53d-118">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="8a53d-119">Co-venda pronta</span><span class="sxs-lookup"><span data-stu-id="8a53d-119">Co-sell ready</span></span>|<span data-ttu-id="8a53d-120">Sua solução de IP/serviços deve estar pronta para venda.</span><span class="sxs-lookup"><span data-stu-id="8a53d-120">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="8a53d-121">Venda com a Microsoft</span><span class="sxs-lookup"><span data-stu-id="8a53d-121">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="8a53d-122">Conta do Partner Center</span><span class="sxs-lookup"><span data-stu-id="8a53d-122">Partner Center account</span></span>|<span data-ttu-id="8a53d-123">A ID de MPN associada ao locatário do Partner Center deve ser a mesma que a ID do MPN associada à sua solução de venda conjunta.</span><span class="sxs-lookup"><span data-stu-id="8a53d-123">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="8a53d-124">Verifique se você pode ver suas referências de venda conjunta no portal do Partner Center antes de implantar os conectores.</span><span class="sxs-lookup"><span data-stu-id="8a53d-124">Verify that you can see your co-sell referrals in Partner Center portal prior to deploying the connectors.</span></span>|[<span data-ttu-id="8a53d-125">Gerenciar sua conta</span><span class="sxs-lookup"><span data-stu-id="8a53d-125">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="8a53d-126">Funções de usuário da Central de parceiros</span><span class="sxs-lookup"><span data-stu-id="8a53d-126">Partner Center user roles</span></span>|<span data-ttu-id="8a53d-127">O funcionário que irá instalar e usar os conectores deve ser um administrador de referências</span><span class="sxs-lookup"><span data-stu-id="8a53d-127">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="8a53d-128">Atribuir permissões e funções de usuários</span><span class="sxs-lookup"><span data-stu-id="8a53d-128">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="8a53d-129">CRM do Salesforce</span><span class="sxs-lookup"><span data-stu-id="8a53d-129">Salesforce CRM</span></span>|<span data-ttu-id="8a53d-130">A função de usuário CRM é administrador do sistema ou personalizador do sistema</span><span class="sxs-lookup"><span data-stu-id="8a53d-130">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="8a53d-131">Atribuir funções no Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="8a53d-131">Assign roles in Dynamics 365</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="8a53d-132">Conta de fluxo de automatização de energia</span><span class="sxs-lookup"><span data-stu-id="8a53d-132">Power Automate Flow Account</span></span>|<span data-ttu-id="8a53d-133">Uma conta de [energia ativa automatizada](https://flow.microsoft.com) para o administrador do sistema do CRM ou o personalizador do sistema.</span><span class="sxs-lookup"><span data-stu-id="8a53d-133">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="8a53d-134">Esse usuário deve entrar no [Power Automate](https://flow.microsoft.com) pelo menos uma vez antes da instalação.</span><span class="sxs-lookup"><span data-stu-id="8a53d-134">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="8a53d-135">Instalar a sincronização de referências do Partner Center para o Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="8a53d-135">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="8a53d-136">Vá para [energia automatizada](https://flow.microsoft.com) e selecione **ambientes** no canto superior direito.</span><span class="sxs-lookup"><span data-stu-id="8a53d-136">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="8a53d-137">Isso mostrará as instâncias do CRM disponíveis.</span><span class="sxs-lookup"><span data-stu-id="8a53d-137">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="8a53d-138">Selecione a instância apropriada do CRM na lista suspensa no canto superior direito.</span><span class="sxs-lookup"><span data-stu-id="8a53d-138">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span> 

3. <span data-ttu-id="8a53d-139">Selecione **soluções** na barra de navegação à esquerda.</span><span class="sxs-lookup"><span data-stu-id="8a53d-139">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="8a53d-140">Clique no link **abrir AppSource** no menu superior.</span><span class="sxs-lookup"><span data-stu-id="8a53d-140">Click on the **Open AppSource** link on the top menu.</span></span>

![Abrir AppSource](images/cosellconnectors/openappsource.png)

5. <span data-ttu-id="8a53d-142">Procure **conectores de referências do Partner Center para Salesforce** na tela pop-up.</span><span class="sxs-lookup"><span data-stu-id="8a53d-142">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

6. <span data-ttu-id="8a53d-143">Clique no botão **obter agora** e em **continuar**.</span><span class="sxs-lookup"><span data-stu-id="8a53d-143">Click the **Get it now** button and then **Continue**.</span></span> 

7. <span data-ttu-id="8a53d-144">Isso abre a página onde você pode selecionar o ambiente CRM (Dynamics 365) para instalar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8a53d-144">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="8a53d-145">Concorde com os termos e condições.</span><span class="sxs-lookup"><span data-stu-id="8a53d-145">Agree to terms and conditions.</span></span> 

8. <span data-ttu-id="8a53d-146">Em seguida, você será direcionado para a página **gerenciar suas soluções** .</span><span class="sxs-lookup"><span data-stu-id="8a53d-146">You are then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="8a53d-147">Navegue até "referências do Partner Center" usando os botões de seta na parte inferior da página.</span><span class="sxs-lookup"><span data-stu-id="8a53d-147">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="8a53d-148">A **instalação agendada** deve aparecer ao lado da solução de referências do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="8a53d-148">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="8a53d-149">A instalação levará 10-15 minutos.</span><span class="sxs-lookup"><span data-stu-id="8a53d-149">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="8a53d-150">Quando a instalação for concluída, navegue de volta para [Power Automate](https://flow.microsoft.com) e selecione **soluções** na área de navegação à esquerda.</span><span class="sxs-lookup"><span data-stu-id="8a53d-150">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="8a53d-151">Observe que a **sincronização de referências do Partner Center para o Salesforce** está disponível na lista de soluções.</span><span class="sxs-lookup"><span data-stu-id="8a53d-151">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="8a53d-152">Selecione **sincronização de referências do Partner Center para o Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="8a53d-152">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="8a53d-153">Os fluxos e as entidades automatizados de energia a seguir estão disponíveis:</span><span class="sxs-lookup"><span data-stu-id="8a53d-153">The following Power Automate flows and entities are available:</span></span>

![CRMS disponíveis](images/cosellconnectors/dynamics-available-crms.png)

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="8a53d-155">Prática recomendada: teste antes de entrar no ar</span><span class="sxs-lookup"><span data-stu-id="8a53d-155">Best Practice: Test before you go live</span></span>

<span data-ttu-id="8a53d-156">Antes de instalar, configurar e personalizar a solução de automatização de energia no ambiente de produção, certifique-se de testar a solução em uma instância de CRM de preparo.</span><span class="sxs-lookup"><span data-stu-id="8a53d-156">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="8a53d-157">Instale a solução de automatização de energia da Microsoft em uma instância de ambiente de preparo/CRM.</span><span class="sxs-lookup"><span data-stu-id="8a53d-157">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="8a53d-158">Faça uma cópia da solução e realize suas configurações e automatize as personalizações de fluxo no ambiente de preparo.</span><span class="sxs-lookup"><span data-stu-id="8a53d-158">Make a copy of the solution and perform your configuration and Power Automate flow customizations on the staging environment.</span></span>
- <span data-ttu-id="8a53d-159">Teste a solução em uma instância de preparo/CRM.</span><span class="sxs-lookup"><span data-stu-id="8a53d-159">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="8a53d-160">Em caso de sucesso, importe como solução gerenciada para a instância de produção.</span><span class="sxs-lookup"><span data-stu-id="8a53d-160">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="8a53d-161">Configurar a solução</span><span class="sxs-lookup"><span data-stu-id="8a53d-161">Configure the solution</span></span>

1. <span data-ttu-id="8a53d-162">Depois de instalar a solução em sua instância do CRM, navegue de volta para o [Power Automate](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="8a53d-162">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="8a53d-163">Na lista suspensa **ambientes** no canto superior direito, selecione a instância de CRM na qual você instalou a solução de automatização de energia.</span><span class="sxs-lookup"><span data-stu-id="8a53d-163">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="8a53d-164">Será necessário criar conexões que associem as três contas de usuário:</span><span class="sxs-lookup"><span data-stu-id="8a53d-164">You will need to create connections that associate the three user accounts:</span></span> 

- <span data-ttu-id="8a53d-165">Usuário do Partner Center com credenciais de administrador de referências</span><span class="sxs-lookup"><span data-stu-id="8a53d-165">Partner Center user with referrals admin credentials</span></span> 
- <span data-ttu-id="8a53d-166">Eventos do Partner Center</span><span class="sxs-lookup"><span data-stu-id="8a53d-166">Partner Center Events</span></span>
- <span data-ttu-id="8a53d-167">Administrador de CRM com os fluxos de energia automatizada na solução.</span><span class="sxs-lookup"><span data-stu-id="8a53d-167">CRM admin with the Power Automate flows in the solution.</span></span> 

    <span data-ttu-id="8a53d-168">a.</span><span class="sxs-lookup"><span data-stu-id="8a53d-168">a.</span></span> <span data-ttu-id="8a53d-169">Selecione **conexões** na barra de navegação à esquerda e selecione a solução "referências do Partner Center" na lista.</span><span class="sxs-lookup"><span data-stu-id="8a53d-169">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>
    <span data-ttu-id="8a53d-170">b.</span><span class="sxs-lookup"><span data-stu-id="8a53d-170">b.</span></span> <span data-ttu-id="8a53d-171">Crie uma conexão clicando em **criar uma conexão**.</span><span class="sxs-lookup"><span data-stu-id="8a53d-171">Create a connection by clicking **Create a connection**.</span></span> 

    ![Criar conexão](images/cosellconnectors/createconnection.png)

    <span data-ttu-id="8a53d-173">c.</span><span class="sxs-lookup"><span data-stu-id="8a53d-173">c.</span></span> <span data-ttu-id="8a53d-174">Procure por **referências do Partner Center (versão prévia)** na barra de pesquisa no canto superior direito.</span><span class="sxs-lookup"><span data-stu-id="8a53d-174">Search for **Partner Center Referrals (preview)** in the search bar on the top right corner.</span></span>
    <span data-ttu-id="8a53d-175">d.</span><span class="sxs-lookup"><span data-stu-id="8a53d-175">d.</span></span> <span data-ttu-id="8a53d-176">Crie uma conexão para o usuário do Partner Center com a função de credenciais do administrador de referências. Oriental.</span><span class="sxs-lookup"><span data-stu-id="8a53d-176">Create a connection for your Partner Center user with the credentials role of Referrals admin. e.</span></span> <span data-ttu-id="8a53d-177">Em seguida, crie uma conexão de eventos do Partner Center para o usuário do Partner Center com as credenciais do administrador de referências. fixo.</span><span class="sxs-lookup"><span data-stu-id="8a53d-177">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin. f.</span></span> <span data-ttu-id="8a53d-178">Crie uma conexão para Common Data Service (ambiente atual) para o usuário administrador do CRM.</span><span class="sxs-lookup"><span data-stu-id="8a53d-178">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

4. <span data-ttu-id="8a53d-179">Para associar os fluxos de energia automatizada com as conexões, edite cada um dos fluxos de energia automatizada para se conectar às referências do Common Data Service e do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="8a53d-179">To associate the Power Automate flows with the connections, edit each of the Power Automate flows to connect to Common Data Service and Partner Center Referrals.</span></span> <span data-ttu-id="8a53d-180">Salve as alterações.</span><span class="sxs-lookup"><span data-stu-id="8a53d-180">Save the changes.</span></span>

5. <span data-ttu-id="8a53d-181">**Ative** os fluxos de energia automatizada.</span><span class="sxs-lookup"><span data-stu-id="8a53d-181">**Turn on** the the Power Automate flows.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8a53d-182">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="8a53d-182">Next steps</span></span>

- [<span data-ttu-id="8a53d-183">Usar WebHooks para obter eventos de alteração de recurso</span><span class="sxs-lookup"><span data-stu-id="8a53d-183">Use Webhooks to get resource change events</span></span>](referral-connector-webhooks.md)

- [<span data-ttu-id="8a53d-184">Mais informações sobre a plataforma de automatização de energia da Microsoft?</span><span class="sxs-lookup"><span data-stu-id="8a53d-184">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/power-automate/)

- [<span data-ttu-id="8a53d-185">Gerenciar clientes potenciais</span><span class="sxs-lookup"><span data-stu-id="8a53d-185">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="8a53d-186">Gerenciar oportunidades de venda conjunta</span><span class="sxs-lookup"><span data-stu-id="8a53d-186">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
