---
title: O conector de venda co-venda para o Salesforce CRM Partner Center
ms.topic: how-to
ms.date: 01/06/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Sincronizar suas indicações no Partner Center com o Salesforce CRM. Em seguida, os vendedores podem fazer a venda em cooperação com a Microsoft de dentro de seus sistemas crm.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: fa9b35343e1251cfce5caff107de8dff344f4e68
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148407"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="38159-104">Conector de venda conjunta para o Salesforce CRM – visão geral</span><span class="sxs-lookup"><span data-stu-id="38159-104">Co-sell connector for Salesforce CRM - overview</span></span>

<span data-ttu-id="38159-105">**Funções apropriadas:** indicações de administrador | Administrador do sistema ou personalizador de sistema no CRM</span><span class="sxs-lookup"><span data-stu-id="38159-105">**Appropriate roles**: Referrals admin | System admin or system customizer on the CRM</span></span>

<span data-ttu-id="38159-106">Partner Center conector de venda co-venda permite que os vendedores vendam com a Microsoft de dentro de seus sistemas CRM.</span><span class="sxs-lookup"><span data-stu-id="38159-106">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="38159-107">Eles não precisam ser treinados para usar o Partner Center gerenciar acordos de venda em cooperação.</span><span class="sxs-lookup"><span data-stu-id="38159-107">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="38159-108">Usando os conectores de venda de co-venda, você pode criar uma nova indicação de venda co-venda para envolver um vendedor da Microsoft, receber indicações do vendedor da Microsoft, aceitar/recusar indicações, modificar dados de negociação, como valor da oferta e data de fechamento.</span><span class="sxs-lookup"><span data-stu-id="38159-108">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="38159-109">Você também pode receber atualizações dos vendedores da Microsoft nesses acordos de venda em cooperação.</span><span class="sxs-lookup"><span data-stu-id="38159-109">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="38159-110">Você pode fazer todas as suas indicações funcionarem enquanto trabalham dentro do CRM de sua escolha em vez de em Partner Center.</span><span class="sxs-lookup"><span data-stu-id="38159-110">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="38159-111">A solução baseia-se na solução microsoft Power Automate e usa apIs Partner Center aplicativo.</span><span class="sxs-lookup"><span data-stu-id="38159-111">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="38159-112">Antes de instalar – pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="38159-112">Before you install - pre-requisites</span></span>

|<span data-ttu-id="38159-113">**Tópicos**</span><span class="sxs-lookup"><span data-stu-id="38159-113">**Topics**</span></span>   |<span data-ttu-id="38159-114">**Detalhes**</span><span class="sxs-lookup"><span data-stu-id="38159-114">**Details**</span></span>   |<span data-ttu-id="38159-115">**Links**</span><span class="sxs-lookup"><span data-stu-id="38159-115">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="38159-116">Microsoft Partner Network ID</span><span class="sxs-lookup"><span data-stu-id="38159-116">Microsoft Partner Network ID</span></span> |<span data-ttu-id="38159-117">Você precisa de uma ID de MPN válida</span><span class="sxs-lookup"><span data-stu-id="38159-117">You need a valid MPN ID</span></span>|<span data-ttu-id="38159-118">Para ingressar no [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="38159-118">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="38159-119">Venda em cooperação pronta</span><span class="sxs-lookup"><span data-stu-id="38159-119">Co-sell ready</span></span>|<span data-ttu-id="38159-120">Sua solução de IP/Serviços deve estar pronta para venda em cooperação.</span><span class="sxs-lookup"><span data-stu-id="38159-120">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="38159-121">Vender com a Microsoft</span><span class="sxs-lookup"><span data-stu-id="38159-121">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="38159-122">Conta do Partner Center</span><span class="sxs-lookup"><span data-stu-id="38159-122">Partner Center account</span></span>|<span data-ttu-id="38159-123">A ID do MPN associada ao locatário Partner Center deve ser igual à ID do MPN associada à sua solução de venda co-venda.</span><span class="sxs-lookup"><span data-stu-id="38159-123">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="38159-124">Verifique se você pode ver suas indicações de venda em Partner Center portal antes de implantar os conectores.</span><span class="sxs-lookup"><span data-stu-id="38159-124">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="38159-125">Gerenciar sua conta</span><span class="sxs-lookup"><span data-stu-id="38159-125">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="38159-126">Funções de usuário da Central de parceiros</span><span class="sxs-lookup"><span data-stu-id="38159-126">Partner Center user roles</span></span>|<span data-ttu-id="38159-127">O funcionário que instalará e usará os conectores deve ser um administrador de indicações</span><span class="sxs-lookup"><span data-stu-id="38159-127">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="38159-128">Atribuir permissões e funções de usuários</span><span class="sxs-lookup"><span data-stu-id="38159-128">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="38159-129">CRM do Salesforce</span><span class="sxs-lookup"><span data-stu-id="38159-129">Salesforce CRM</span></span>|<span data-ttu-id="38159-130">A função de usuário CRM é administrador do sistema ou personalizador do sistema</span><span class="sxs-lookup"><span data-stu-id="38159-130">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="38159-131">Atribuir funções no Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="38159-131">Assign roles in Salesforce CRM</span></span>](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|<span data-ttu-id="38159-132">Conta de fluxo de automatização de energia</span><span class="sxs-lookup"><span data-stu-id="38159-132">Power Automate Flow Account</span></span>|<span data-ttu-id="38159-133">Uma conta de [energia ativa automatizada](https://flow.microsoft.com) para o administrador do sistema do CRM ou o personalizador do sistema.</span><span class="sxs-lookup"><span data-stu-id="38159-133">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="38159-134">Esse usuário deve entrar no [Power Automate](https://flow.microsoft.com) pelo menos uma vez antes da instalação.</span><span class="sxs-lookup"><span data-stu-id="38159-134">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="38159-135">Instalação do pacote do Salesforce para campos personalizados da Microsoft</span><span class="sxs-lookup"><span data-stu-id="38159-135">Installation of Salesforce Package for Microsoft Custom Fields</span></span> 

<span data-ttu-id="38159-136">Para sincronizar as referências no Partner Center e no Salesforce CRM, a solução de automatização de energia precisa identificar claramente os campos de referência específicos da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="38159-136">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft-specific referral fields.</span></span> <span data-ttu-id="38159-137">Essa demarcação fornece às equipes do vendedor do parceiro a capacidade de decidir quais referências eles desejam compartilhar com a Microsoft para venda.</span><span class="sxs-lookup"><span data-stu-id="38159-137">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="38159-138">No Salesforce, ative as **anotações** e adicione-as à lista de oportunidades relacionadas.</span><span class="sxs-lookup"><span data-stu-id="38159-138">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> 
[<span data-ttu-id="38159-139">Referência</span><span class="sxs-lookup"><span data-stu-id="38159-139">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. <span data-ttu-id="38159-140">Ative as **equipes de oportunidades** seguindo as etapas:</span><span class="sxs-lookup"><span data-stu-id="38159-140">Activate **Opportunity teams** by following the steps:</span></span> 
    - <span data-ttu-id="38159-141">Na instalação, use a caixa **localização rápida** para localizar as configurações da equipe de oportunidade.</span><span class="sxs-lookup"><span data-stu-id="38159-141">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="38159-142">Defina as configurações conforme necessário.</span><span class="sxs-lookup"><span data-stu-id="38159-142">Define the settings as needed.</span></span>
[<span data-ttu-id="38159-143">Referência</span><span class="sxs-lookup"><span data-stu-id="38159-143">Reference</span></span>](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. <span data-ttu-id="38159-144">No Salesforce, instale campos personalizados e objetos usando o [instalador de pacote](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV).</span><span class="sxs-lookup"><span data-stu-id="38159-144">In Salesforce, install custom fields and objects using the [package installer](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV).</span></span> <span data-ttu-id="38159-145">Use isso para instalar o pacote em qualquer empresa.</span><span class="sxs-lookup"><span data-stu-id="38159-145">Use this to install the package into any company.</span></span>

>[!NOTE]
><span data-ttu-id="38159-146">Se você estiver instalando em uma área restrita, deverá substituir a parte inicial da URL por http://test.salesforce.com</span><span class="sxs-lookup"><span data-stu-id="38159-146">If you are installing into a sandbox, you must replace the initial portion of the URL with http://test.salesforce.com</span></span>

4. <span data-ttu-id="38159-147">No Salesforce, adicione soluções da Microsoft à lista de **oportunidades** relacionadas.</span><span class="sxs-lookup"><span data-stu-id="38159-147">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="38159-148">Depois de adicionado, selecione o ícone de **chave inglesa** e atualize as propriedades</span><span class="sxs-lookup"><span data-stu-id="38159-148">Once added, select the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="38159-149">Prática recomendada: teste antes de entrar no ar</span><span class="sxs-lookup"><span data-stu-id="38159-149">Best Practice: Test before you go live</span></span>

<span data-ttu-id="38159-150">Antes de instalar, configurar e personalizar a solução de automatização de energia no ambiente de produção, certifique-se de testar a solução em uma instância de CRM de preparo.</span><span class="sxs-lookup"><span data-stu-id="38159-150">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="38159-151">Instale a solução microsoft Power Automate em um ambiente de preparação/instância crm.</span><span class="sxs-lookup"><span data-stu-id="38159-151">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="38159-152">Faça uma cópia da solução e execute sua configuração e Power Automate personalizações de fluxo no ambiente de preparação.</span><span class="sxs-lookup"><span data-stu-id="38159-152">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="38159-153">Teste a solução em uma instância de preparação/CRM.</span><span class="sxs-lookup"><span data-stu-id="38159-153">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="38159-154">Em caso de sucesso, importe como uma solução gerenciada para a instância de produção.</span><span class="sxs-lookup"><span data-stu-id="38159-154">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="38159-155">Instalar Partner Center sincronização de indicações do Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="38159-155">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="38159-156">Vá para [Power Automate](https://flow.microsoft.com) e selecione **Ambientes** no canto superior direito.</span><span class="sxs-lookup"><span data-stu-id="38159-156">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="38159-157">Isso mostrará as instâncias de CRM disponíveis.</span><span class="sxs-lookup"><span data-stu-id="38159-157">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="38159-158">Selecione a instância de CRM apropriada na lista inferior no canto superior direito.</span><span class="sxs-lookup"><span data-stu-id="38159-158">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="38159-159">Selecione **Soluções** na barra de navegação à esquerda.</span><span class="sxs-lookup"><span data-stu-id="38159-159">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="38159-160">Selecione o link **Abrir AppSource** no menu superior.</span><span class="sxs-lookup"><span data-stu-id="38159-160">Select the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Abra o AppSource":::

5. <span data-ttu-id="38159-162">**Pesquise Partner Center conectores de indicações para Salesforce** na tela pop-up.</span><span class="sxs-lookup"><span data-stu-id="38159-162">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. <span data-ttu-id="38159-164">Selecione o **botão Obter agora e,** em seguida, **Continuar.**</span><span class="sxs-lookup"><span data-stu-id="38159-164">Select the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="38159-165">Isso abre a página em que você pode selecionar o ambiente do Salesforce CRM para instalar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="38159-165">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="38159-166">Concorde com os termos e condições.</span><span class="sxs-lookup"><span data-stu-id="38159-166">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="CRMS disponíveis":::

8. <span data-ttu-id="38159-168">Em seguida, você será direcionado para a **página Gerenciar suas soluções.**</span><span class="sxs-lookup"><span data-stu-id="38159-168">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="38159-169">Navegue até "Partner Center indicações" usando os botões de seta na parte inferior da página.</span><span class="sxs-lookup"><span data-stu-id="38159-169">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="38159-170">**A instalação agendada** deve aparecer ao lado Partner Center de indicações.</span><span class="sxs-lookup"><span data-stu-id="38159-170">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="38159-171">A instalação levará de 10 a 15 minutos.</span><span class="sxs-lookup"><span data-stu-id="38159-171">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="38159-172">Quando a instalação for concluída, navegue de volta para [Power Automate](https://flow.microsoft.com) e selecione **soluções** na área de navegação à esquerda.</span><span class="sxs-lookup"><span data-stu-id="38159-172">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="38159-173">Observe que a **sincronização de referências do Partner Center para o Salesforce** está disponível na lista de soluções.</span><span class="sxs-lookup"><span data-stu-id="38159-173">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="38159-174">Selecione **sincronização de referências do Partner Center para Salesforce**.</span><span class="sxs-lookup"><span data-stu-id="38159-174">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="38159-175">Os fluxos e as entidades automatizados de energia a seguir estão disponíveis:</span><span class="sxs-lookup"><span data-stu-id="38159-175">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Fluxos do Salesforce":::



## <a name="configure-the-solution"></a><span data-ttu-id="38159-177">Configurar a solução</span><span class="sxs-lookup"><span data-stu-id="38159-177">Configure the solution</span></span>

1. <span data-ttu-id="38159-178">Depois de instalar a solução em sua instância do CRM, navegue de volta para o [Power Automate](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="38159-178">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="38159-179">Na lista suspensa **ambientes** no canto superior direito, selecione a instância de CRM na qual você instalou a solução de automatização de energia.</span><span class="sxs-lookup"><span data-stu-id="38159-179">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>
3. <span data-ttu-id="38159-180">Será necessário criar conexões que associem as três contas de usuário:</span><span class="sxs-lookup"><span data-stu-id="38159-180">You will need to create connections that associate the three user accounts:</span></span>
    - <span data-ttu-id="38159-181">Usuário do Partner Center com credenciais de administrador de referências</span><span class="sxs-lookup"><span data-stu-id="38159-181">Partner Center user with referrals admin credentials</span></span>
    - <span data-ttu-id="38159-182">Eventos do Partner Center</span><span class="sxs-lookup"><span data-stu-id="38159-182">Partner Center Events</span></span>
    - <span data-ttu-id="38159-183">Administrador de CRM com os fluxos de energia automatizada na solução.</span><span class="sxs-lookup"><span data-stu-id="38159-183">CRM admin with the Power Automate flows in the solution.</span></span>
4. <span data-ttu-id="38159-184">Selecione **conexões** na barra de navegação à esquerda e selecione a solução "referências do Partner Center" na lista.</span><span class="sxs-lookup"><span data-stu-id="38159-184">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

5. <span data-ttu-id="38159-185">Crie uma conexão clicando em **criar uma conexão**.</span><span class="sxs-lookup"><span data-stu-id="38159-185">Create a connection by clicking **Create a connection**.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Criar conexão":::

- <span data-ttu-id="38159-187">Procure por referências do Partner Center (versão prévia) na barra de pesquisa no canto superior direito.</span><span class="sxs-lookup"><span data-stu-id="38159-187">Search for Partner Center Referrals (preview) in the search bar on the top-right corner.</span></span>

- <span data-ttu-id="38159-188">Crie uma conexão para o usuário do Partner Center com a função de credenciais do administrador de referências.</span><span class="sxs-lookup"><span data-stu-id="38159-188">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

-  <span data-ttu-id="38159-189">Em seguida, crie uma conexão de eventos do Partner Center para o usuário do Partner Center com as credenciais do administrador de referências.</span><span class="sxs-lookup"><span data-stu-id="38159-189">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

- <span data-ttu-id="38159-190">Crie uma conexão para o Salesforce para o usuário administrador do CRM.</span><span class="sxs-lookup"><span data-stu-id="38159-190">Create a connection for Salesforce for the CRM administrator user.</span></span>

-  <span data-ttu-id="38159-191">Depois de adicionar todas as conexões, você deverá ver as seguintes conexões em seu ambiente:</span><span class="sxs-lookup"><span data-stu-id="38159-191">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Observar conexões":::

### <a name="edit-the-connections"></a><span data-ttu-id="38159-193">Editar as conexões</span><span class="sxs-lookup"><span data-stu-id="38159-193">Edit the connections</span></span>

1. <span data-ttu-id="38159-194">Volte para a página soluções e selecione **solução padrão**.</span><span class="sxs-lookup"><span data-stu-id="38159-194">Return to the Solutions page and select **Default Solution**.</span></span>  <span data-ttu-id="38159-195">Selecione **Referência de Conexão (versão prévia)** clicando em **Todos.**</span><span class="sxs-lookup"><span data-stu-id="38159-195">Select **Connection Reference (preview)** by clicking **All**.</span></span>
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Iniciar edição do conector":::

2. <span data-ttu-id="38159-197">Edite cada uma das Conexões individualmente selecionando o ícone de três pontos.</span><span class="sxs-lookup"><span data-stu-id="38159-197">Edit each of the Connections individually by selecting the three dots icon.</span></span> <span data-ttu-id="38159-198">Adicione as conexões relevantes.</span><span class="sxs-lookup"><span data-stu-id="38159-198">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Editar conectores":::

3. <span data-ttu-id="38159-200">A ligar os fluxos na sequência a seguir:</span><span class="sxs-lookup"><span data-stu-id="38159-200">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="38159-201">Partner Center de webhook (visualização do insider)</span><span class="sxs-lookup"><span data-stu-id="38159-201">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="38159-202">Criar indicação de venda co-venda – Salesforce para Partner Center (Visualização do Insider)</span><span class="sxs-lookup"><span data-stu-id="38159-202">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="38159-203">Partner Center atualizações de indicação de venda co-venda da Microsoft para o Salesforce (Visualização do Insider)</span><span class="sxs-lookup"><span data-stu-id="38159-203">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="38159-204">Partner Center ao Salesforce (Visualização do Insider)</span><span class="sxs-lookup"><span data-stu-id="38159-204">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="38159-205">Salesforce para Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="38159-205">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="38159-206">Salesforce Opportunity to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="38159-206">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="38159-207">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="38159-207">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="38159-208">Usar APIs de webhook para se registrar para eventos de alteração de recursos</span><span class="sxs-lookup"><span data-stu-id="38159-208">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="38159-209">As APIs Partner Center Webhook permitem que você se registre para eventos de alteração de recursos.</span><span class="sxs-lookup"><span data-stu-id="38159-209">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="38159-210">Esses eventos de alteração são enviados para sua URL como postagens HTTP.</span><span class="sxs-lookup"><span data-stu-id="38159-210">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="38159-211">Para registrar sua URL, selecione Partner Center **registro de webhook (visualização do insider)** Power Automate fluxo.</span><span class="sxs-lookup"><span data-stu-id="38159-211">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="38159-212">Adicione conexões para (a.) Partner Center usuário com credenciais de administrador de indicações (b.) Partner Center Eventos conforme realçada abaixo</span><span class="sxs-lookup"><span data-stu-id="38159-212">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Gatilho":::

3. <span data-ttu-id="38159-214">Ao fazer essas atualizações, você verá</span><span class="sxs-lookup"><span data-stu-id="38159-214">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks":::

4. <span data-ttu-id="38159-216">Salve suas alterações e selecione **Ativar**.</span><span class="sxs-lookup"><span data-stu-id="38159-216">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="38159-217">Para habilitar o parceiro do Partner Center a ouvir as alterações de evento, execute as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="38159-217">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="38159-218">Selecione **Partner Center para SALESFORCE CRM (insider Preview)**.</span><span class="sxs-lookup"><span data-stu-id="38159-218">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="38159-219">Selecione o ícone **Editar** e selecione **quando uma solicitação HTTP é recebida**.</span><span class="sxs-lookup"><span data-stu-id="38159-219">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="38159-220">Selecione o ícone de **cópia** para copiar a URL de postagem http fornecida.</span><span class="sxs-lookup"><span data-stu-id="38159-220">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Copiar URL":::

8. <span data-ttu-id="38159-222">Agora, selecione o fluxo "registro do webhook do Partner Center (insider Preview)" automatizar fluxos de energia e selecione **executar**.</span><span class="sxs-lookup"><span data-stu-id="38159-222">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="38159-223">Verifique se a janela "executar fluxo" é aberta no painel direito e selecione **continuar**.</span><span class="sxs-lookup"><span data-stu-id="38159-223">Ensure that the "Run Flow" window opens on the right-hand pane and select **Continue**.</span></span>

10. <span data-ttu-id="38159-224">Insira os seguintes detalhes:</span><span class="sxs-lookup"><span data-stu-id="38159-224">Enter the following details:</span></span>

    1. <span data-ttu-id="38159-225">**Ponto de extremidade de gatilho http**: URL copiada da etapa anterior</span><span class="sxs-lookup"><span data-stu-id="38159-225">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="38159-226">**Eventos a serem registrados**: "referência criada" e "referência atualizada"</span><span class="sxs-lookup"><span data-stu-id="38159-226">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="38159-227">**Substituir pontos de extremidade de gatilho existentes, se presente**: Sim (isso substitui todos os pontos de extremidade existentes.)</span><span class="sxs-lookup"><span data-stu-id="38159-227">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="38159-228">Selecione **executar** e, em seguida, selecione **concluído.**</span><span class="sxs-lookup"><span data-stu-id="38159-228">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="38159-229">O webhook agora pode escutar criar e atualizar eventos.</span><span class="sxs-lookup"><span data-stu-id="38159-229">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="38159-230">Personalizar etapas de sincronização</span><span class="sxs-lookup"><span data-stu-id="38159-230">Customize synchronization steps</span></span>

<span data-ttu-id="38159-231">Quando as referências de venda cruzada são sincronizadas entre o Partner Center e o sistema CRM, os campos sincronizados no PC do Partner Center são listados aqui.</span><span class="sxs-lookup"><span data-stu-id="38159-231">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="38159-232">Geralmente, os sistemas CRM são altamente personalizados.</span><span class="sxs-lookup"><span data-stu-id="38159-232">Often CRM systems are highly customized.</span></span> <span data-ttu-id="38159-233">Você pode personalizar os fluxos de energia automatizada.</span><span class="sxs-lookup"><span data-stu-id="38159-233">You can customize the Power Automate flows.</span></span> <span data-ttu-id="38159-234">Siga o guia de mapeamento de campo e, se necessário, faça as alterações apropriadas nas etapas de fluxos de energia automatizar.</span><span class="sxs-lookup"><span data-stu-id="38159-234">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="38159-235">Os mapeamentos do Microsoft Partner centers para CRM são fornecidos, mas com base no seu ambiente de CRM, você pode optar por personalizar ainda mais os campos.</span><span class="sxs-lookup"><span data-stu-id="38159-235">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="38159-236">Várias etapas de cada um dos fluxos de energia automatizada podem ser personalizadas com base em suas necessidades.</span><span class="sxs-lookup"><span data-stu-id="38159-236">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="38159-237">Veja a seguir exemplos de personalizações disponíveis:</span><span class="sxs-lookup"><span data-stu-id="38159-237">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="38159-238">Para personalizar os campos de criação ou atualização de eventos no Partner Center para a sincronização de referência do CRM:</span><span class="sxs-lookup"><span data-stu-id="38159-238">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="38159-239">Selecione Partner Center Salesforce CRM (Insider Preview).</span><span class="sxs-lookup"><span data-stu-id="38159-239">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="38159-240">Selecione **Editar** para editar/personalizar o Power Automate fluxo.</span><span class="sxs-lookup"><span data-stu-id="38159-240">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="38159-241">Selecione **(Escopo) Sincronizar o lead ou a oportunidade**.</span><span class="sxs-lookup"><span data-stu-id="38159-241">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="38159-242">Para personalizar mapeamentos de campo crm para criar eventos, selecione **Se for uma nova oportunidade compartilhada, em seguida,**.</span><span class="sxs-lookup"><span data-stu-id="38159-242">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="38159-243">Selecione a sub-etapa **se sim e,** em seguida, expanda **Criando uma nova oportunidade no CRM.**</span><span class="sxs-lookup"><span data-stu-id="38159-243">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="38159-244">Você pode editar os mapeamentos nesta seção usando o Guia de Mapeamento de Campo.</span><span class="sxs-lookup"><span data-stu-id="38159-244">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="38159-245">Para personalizar mapeamentos de campo crm para eventos de atualização, selecione a etapa "(Escopo) Sincronizar o cliente ou a oportunidade".</span><span class="sxs-lookup"><span data-stu-id="38159-245">To customize CRM field mappings for update events, select the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="38159-246">Selecione **Se for uma atualização para uma oportunidade, em seguida,**.</span><span class="sxs-lookup"><span data-stu-id="38159-246">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="38159-247">Selecione a sub-etapa **se sim e** expanda Se diferença entre os objetos de oportunidade no Partner Center e **CRM, em seguida,**.</span><span class="sxs-lookup"><span data-stu-id="38159-247">Select the sub-step **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="38159-248">Selecione **Se sim seguido** de Atualizar oportunidade **existente**</span><span class="sxs-lookup"><span data-stu-id="38159-248">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="38159-249">Para personalizar os campos para a sincronização de indicação de CRM para PC para eventos de atualização:</span><span class="sxs-lookup"><span data-stu-id="38159-249">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="38159-250">Selecione **Editar**  para editar/personalizar o Power Automate fluxo.</span><span class="sxs-lookup"><span data-stu-id="38159-250">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="38159-251">Selecione **(Escopo) Sincronizar a oportunidade.**</span><span class="sxs-lookup"><span data-stu-id="38159-251">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="38159-252">Para personalizar mapeamentos de campo crm (com base no guia de mapeamentos de campo) para eventos de atualização, selecione Se houver diferença entre os objetos de cliente Partner Center e **CRM, em seguida,**.</span><span class="sxs-lookup"><span data-stu-id="38159-252">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="38159-253">Selecione a sub-etapa se **sim e** expanda a etapa Atualizar **uma indicação com dados de oportunidade**.</span><span class="sxs-lookup"><span data-stu-id="38159-253">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="38159-254">Você pode editar os mapeamentos nesta seção com base no Guia de Mapeamento de Campo.</span><span class="sxs-lookup"><span data-stu-id="38159-254">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="38159-255">Para personalizar os campos para a sincronização de indicação de CRM para PC para criar eventos?</span><span class="sxs-lookup"><span data-stu-id="38159-255">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="38159-256">Selecione **Editar**  para editar/personalizar o Power Automate fluxo.</span><span class="sxs-lookup"><span data-stu-id="38159-256">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="38159-257">Selecione **(Escopo) Sincronizando Indicações.**</span><span class="sxs-lookup"><span data-stu-id="38159-257">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="38159-258">Para personalizar mapeamentos de campo crm (com base no guia de mapeamentos de campo) para criar eventos, **selecione Criar Referência da Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="38159-258">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="38159-259">Você pode editar os mapeamentos nesta seção com base no guia de mapeamento de campos.</span><span class="sxs-lookup"><span data-stu-id="38159-259">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="38159-260">Sincronização de referência de cooperação bidirecional de ponta a ponta</span><span class="sxs-lookup"><span data-stu-id="38159-260">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="38159-261">Depois de instalar, configurar e personalizar a solução de automatização de energia, você pode testar a sincronização de referências de venda entre o Salesforce CRM e o Partner Center.</span><span class="sxs-lookup"><span data-stu-id="38159-261">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="38159-262">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="38159-262">Pre-requisites</span></span>

<span data-ttu-id="38159-263">Para sincronizar as referências no Partner Center e no Salesforce CRM, a solução de automatização de energia precisa demarcar claramente os campos de referência específicos da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="38159-263">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="38159-264">Essa identificação fornece às suas equipes do vendedor a capacidade de decidir quais referências eles desejam compartilhar com a Microsoft para fazer a venda.</span><span class="sxs-lookup"><span data-stu-id="38159-264">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="38159-265">Um conjunto de campos personalizados está disponível como parte da sincronização de referências do Partner Center para a entidade **oportunidade** de solução do Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="38159-265">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="38159-266">Um usuário administrador de CRM precisará criar uma seção de CRM separada com os campos personalizados de **oportunidade** .</span><span class="sxs-lookup"><span data-stu-id="38159-266">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="38159-267">Os campos personalizados a seguir devem fazer parte da seção CRM:</span><span class="sxs-lookup"><span data-stu-id="38159-267">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="38159-268">**Sincronizar com o Partner Center**: se deseja sincronizar a oportunidade com o Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="38159-268">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="38159-269">**Identificador de referência**: um campo de identificador somente leitura para a referência do Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="38159-269">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="38159-270">**Link de referência**: um link somente leitura para a referência no Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="38159-270">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="38159-271">**Como a Microsoft pode ajudar**: a ajuda necessária da Microsoft para a referência</span><span class="sxs-lookup"><span data-stu-id="38159-271">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="38159-272">**Produtos**: lista de produtos associados a esta oportunidade</span><span class="sxs-lookup"><span data-stu-id="38159-272">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="38159-273">**Auditoria**: uma trilha de auditoria somente leitura para sincronização com as referências do Partner Center</span><span class="sxs-lookup"><span data-stu-id="38159-273">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="38159-274">EXEMPLOS</span><span class="sxs-lookup"><span data-stu-id="38159-274">SCENARIOS:</span></span>

1. <span data-ttu-id="38159-275">Sincronização de referência quando a referência é criada ou atualizada no CRM e sincronizada no Partner Center:</span><span class="sxs-lookup"><span data-stu-id="38159-275">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="38159-276">Entre no ambiente do Salesforce CRM com o usuário que tem visibilidade na seção **oportunidade** do CRM.</span><span class="sxs-lookup"><span data-stu-id="38159-276">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="38159-277">Verifique se a seção a seguir está presente quando você cria uma "nova oportunidade" no ambiente CRM do Salesforce</span><span class="sxs-lookup"><span data-stu-id="38159-277">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Ambiente do Salesforce":::

   3. <span data-ttu-id="38159-279">Para sincronizar essa oportunidade com o Microsoft Partner Center, certifique-se de definir os seguintes campos no modo de exibição de cartão:</span><span class="sxs-lookup"><span data-stu-id="38159-279">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="38159-280">"Sincronizar com Partner Center": Sim</span><span class="sxs-lookup"><span data-stu-id="38159-280">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="38159-281">"Como a Microsoft pode ajudar?": selecione uma das seguintes opções:</span><span class="sxs-lookup"><span data-stu-id="38159-281">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="38159-282">Produtos: IDs de solução do produto</span><span class="sxs-lookup"><span data-stu-id="38159-282">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="38159-283">Depois de definir a opção  **Sincronizar** com Partner Center oportunidade como **Sim,** aguarde 10 minutos, entre em sua conta Partner Center.</span><span class="sxs-lookup"><span data-stu-id="38159-283">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="38159-284">Suas indicações serão sincronizadas com o Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="38159-284">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="38159-285">Quando a opção "Sincronizar com Partner Center" estiver definida como "Sim", se você atualizar a oportunidade no Salesforce CRM, as alterações serão sincronizadas com sua Partner Center cliente.</span><span class="sxs-lookup"><span data-stu-id="38159-285">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="38159-286">As oportunidades sincronizadas com êxito com Partner Center serão identificadas com ✔icon no Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="38159-286">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="38159-287">Sincronização de indicação quando a indicação é criada ou atualizada no Microsoft Partner Center sincronizada no ambiente salesforce CRM:</span><span class="sxs-lookup"><span data-stu-id="38159-287">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="38159-288">Entre em seu painel Partner Center [.](https://partner.microsoft.com/dashboard/home)</span><span class="sxs-lookup"><span data-stu-id="38159-288">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="38159-289">Selecione **Indicações** no menu à esquerda.</span><span class="sxs-lookup"><span data-stu-id="38159-289">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="38159-290">Crie uma nova indicação de venda de Partner Center clicando na opção "Nova oferta".</span><span class="sxs-lookup"><span data-stu-id="38159-290">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="38159-291">Entre em seu ambiente do Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="38159-291">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="38159-292">Navegue até **Abrir Oportunidades**.</span><span class="sxs-lookup"><span data-stu-id="38159-292">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="38159-293">A indicação criada no Microsoft Partner Center agora está sincronizada no Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="38159-293">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Tela de oportunidade do Salesforce":::

    6. <span data-ttu-id="38159-295">Quando você seleciona uma indicação sincronizada, os detalhes da exibição de cartão são preenchidos.</span><span class="sxs-lookup"><span data-stu-id="38159-295">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="38159-296">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="38159-296">Next steps</span></span>

- [<span data-ttu-id="38159-297">Gerenciar clientes potenciais</span><span class="sxs-lookup"><span data-stu-id="38159-297">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="38159-298">Gerenciar oportunidades de venda conjunta</span><span class="sxs-lookup"><span data-stu-id="38159-298">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="38159-299">Webhooks do Partner Center</span><span class="sxs-lookup"><span data-stu-id="38159-299">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)
