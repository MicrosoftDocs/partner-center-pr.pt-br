---
title: O conector de televenda para o centro de parceiros do Salesforce CRM
ms.topic: how-to
ms.date: 05/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Sincronize suas referências no Partner Center com seu Salesforce CRM
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 1b658f04b1348eb48f694fac069518a7a7fc6a70
ms.sourcegitcommit: 505c38436780a31692f5f5694830fcfe01502977
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/25/2020
ms.locfileid: "91372806"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="f7134-103">Conector de venda conjunta para o Salesforce CRM – visão geral</span><span class="sxs-lookup"><span data-stu-id="f7134-103">Co-sell connector for Salesforce CRM - overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="f7134-104">Funções apropriadas</span><span class="sxs-lookup"><span data-stu-id="f7134-104">Appropriate roles</span></span>

- <span data-ttu-id="f7134-105">Administrador de indicações</span><span class="sxs-lookup"><span data-stu-id="f7134-105">Referrals admin</span></span>
- <span data-ttu-id="f7134-106">Administrador do sistema ou personalizador do sistema no CRM</span><span class="sxs-lookup"><span data-stu-id="f7134-106">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="f7134-107">O conector de televenda do Partner Center permite que seus vendedores covendam-se com a Microsoft de dentro de seus sistemas de CRM.</span><span class="sxs-lookup"><span data-stu-id="f7134-107">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="f7134-108">Eles não precisarão ser treinados para usar o Partner Center para gerenciar acordos de venda.</span><span class="sxs-lookup"><span data-stu-id="f7134-108">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="f7134-109">Usando os conectores de venda conjunta, você pode criar uma nova referência de covenda para envolver um vendedor da Microsoft, receber referências do vendedor da Microsoft, aceitar/recusar referências, modificar dados de negociações, como valor de negócio e data de fechamento.</span><span class="sxs-lookup"><span data-stu-id="f7134-109">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="f7134-110">Você também pode receber todas as atualizações dos vendedores da Microsoft sobre esses acordos de venda conjunta.</span><span class="sxs-lookup"><span data-stu-id="f7134-110">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="f7134-111">Você pode fazer todas as suas referências funcionarem enquanto trabalha no CRM de sua escolha em vez de no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="f7134-111">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="f7134-112">A solução baseia-se na solução de automatização de energia da Microsoft e usa as APIs do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="f7134-112">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="f7134-113">Antes de instalar-pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f7134-113">Before you install - pre-requisites</span></span>

|<span data-ttu-id="f7134-114">**Tópicos**</span><span class="sxs-lookup"><span data-stu-id="f7134-114">**Topics**</span></span>   |<span data-ttu-id="f7134-115">**Detalhes**</span><span class="sxs-lookup"><span data-stu-id="f7134-115">**Details**</span></span>   |<span data-ttu-id="f7134-116">**Links**</span><span class="sxs-lookup"><span data-stu-id="f7134-116">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="f7134-117">ID de Microsoft Partner Network</span><span class="sxs-lookup"><span data-stu-id="f7134-117">Microsoft Partner Network ID</span></span> |<span data-ttu-id="f7134-118">Você precisa de uma ID de MPN válida</span><span class="sxs-lookup"><span data-stu-id="f7134-118">You need a valid MPN ID</span></span>|<span data-ttu-id="f7134-119">Para ingressar no [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="f7134-119">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="f7134-120">Co-venda pronta</span><span class="sxs-lookup"><span data-stu-id="f7134-120">Co-sell ready</span></span>|<span data-ttu-id="f7134-121">Sua solução de IP/serviços deve estar pronta para venda.</span><span class="sxs-lookup"><span data-stu-id="f7134-121">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="f7134-122">Venda com a Microsoft</span><span class="sxs-lookup"><span data-stu-id="f7134-122">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="f7134-123">Conta do Partner Center</span><span class="sxs-lookup"><span data-stu-id="f7134-123">Partner Center account</span></span>|<span data-ttu-id="f7134-124">A ID de MPN associada ao locatário do Partner Center deve ser a mesma que a ID do MPN associada à sua solução de venda conjunta.</span><span class="sxs-lookup"><span data-stu-id="f7134-124">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="f7134-125">Verifique se você pode ver suas referências de venda conjunta no portal do Partner Center antes de implantar os conectores.</span><span class="sxs-lookup"><span data-stu-id="f7134-125">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="f7134-126">Gerenciar sua conta</span><span class="sxs-lookup"><span data-stu-id="f7134-126">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="f7134-127">Funções de usuário da Central de parceiros</span><span class="sxs-lookup"><span data-stu-id="f7134-127">Partner Center user roles</span></span>|<span data-ttu-id="f7134-128">O funcionário que irá instalar e usar os conectores deve ser um administrador de referências</span><span class="sxs-lookup"><span data-stu-id="f7134-128">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="f7134-129">Atribuir permissões e funções de usuários</span><span class="sxs-lookup"><span data-stu-id="f7134-129">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="f7134-130">CRM do Salesforce</span><span class="sxs-lookup"><span data-stu-id="f7134-130">Salesforce CRM</span></span>|<span data-ttu-id="f7134-131">A função de usuário CRM é administrador do sistema ou personalizador do sistema</span><span class="sxs-lookup"><span data-stu-id="f7134-131">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="f7134-132">Atribuir funções no Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="f7134-132">Assign roles in Salesforce CRM</span></span>](/SalesforceCRM/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="f7134-133">Conta de fluxo de automatização de energia</span><span class="sxs-lookup"><span data-stu-id="f7134-133">Power Automate Flow Account</span></span>|<span data-ttu-id="f7134-134">Uma conta de [energia ativa automatizada](https://flow.microsoft.com) para o administrador do sistema do CRM ou o personalizador do sistema.</span><span class="sxs-lookup"><span data-stu-id="f7134-134">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="f7134-135">Esse usuário deve entrar no [Power Automate](https://flow.microsoft.com) pelo menos uma vez antes da instalação.</span><span class="sxs-lookup"><span data-stu-id="f7134-135">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="f7134-136">Instalação do pacote do Salesforce para campos personalizados da Microsoft</span><span class="sxs-lookup"><span data-stu-id="f7134-136">Installation of Salesforce Package for Microsoft Custom Fields</span></span> 

<span data-ttu-id="f7134-137">Para sincronizar as referências no Partner Center e no Salesforce CRM, a solução de automatização de energia precisa identificar claramente os campos de referência específicos da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f7134-137">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft specific referral fields.</span></span> <span data-ttu-id="f7134-138">Essa demarcação fornece às equipes do vendedor do parceiro a capacidade de decidir quais referências eles desejam compartilhar com a Microsoft para venda.</span><span class="sxs-lookup"><span data-stu-id="f7134-138">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="f7134-139">No Salesforce, ative as **anotações** e adicione-as à lista de oportunidades relacionadas.</span><span class="sxs-lookup"><span data-stu-id="f7134-139">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> 
[<span data-ttu-id="f7134-140">Referência</span><span class="sxs-lookup"><span data-stu-id="f7134-140">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. <span data-ttu-id="f7134-141">Ative as **equipes de oportunidades** seguindo as etapas:</span><span class="sxs-lookup"><span data-stu-id="f7134-141">Activate **Opportunity teams** by following the steps:</span></span> 
    - <span data-ttu-id="f7134-142">Na instalação, use a caixa **localização rápida** para localizar as configurações da equipe de oportunidade.</span><span class="sxs-lookup"><span data-stu-id="f7134-142">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="f7134-143">Defina as configurações conforme necessário.</span><span class="sxs-lookup"><span data-stu-id="f7134-143">Define the settings as needed.</span></span>
[<span data-ttu-id="f7134-144">Referência</span><span class="sxs-lookup"><span data-stu-id="f7134-144">Reference</span></span>](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. <span data-ttu-id="f7134-145">No Salesforce, instale campos personalizados e objetos usando o instalador de pacote abaixo.</span><span class="sxs-lookup"><span data-stu-id="f7134-145">In Salesforce, install custom fields and objects using package installer below.</span></span>
  
<span data-ttu-id="f7134-146">Acesse [aqui](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006Vs9a) para instalar o pacote em qualquer empresa:</span><span class="sxs-lookup"><span data-stu-id="f7134-146">Go [here](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006Vs9a) to install the package into any company:</span></span>


<span data-ttu-id="f7134-147">Observação: se você estiver instalando em uma área restrita, deverá substituir a parte inicial da URL por http://test.salesforce.com</span><span class="sxs-lookup"><span data-stu-id="f7134-147">Note: If you are installing into a sandbox you must replace the initial portion of the URL with http://test.salesforce.com</span></span>

4. <span data-ttu-id="f7134-148">No Salesforce, adicione soluções da Microsoft à lista de **oportunidades** relacionadas.</span><span class="sxs-lookup"><span data-stu-id="f7134-148">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="f7134-149">Depois de adicionado, clique no ícone de **chave inglesa** e atualize as propriedades</span><span class="sxs-lookup"><span data-stu-id="f7134-149">Once added, click on the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="f7134-150">Prática recomendada: teste antes de entrar no ar</span><span class="sxs-lookup"><span data-stu-id="f7134-150">Best Practice: Test before you go live</span></span>

<span data-ttu-id="f7134-151">Antes de instalar, configurar e personalizar a solução de automatização de energia no ambiente de produção, certifique-se de testar a solução em uma instância de CRM de preparo.</span><span class="sxs-lookup"><span data-stu-id="f7134-151">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="f7134-152">Instale a solução de automatização de energia da Microsoft em uma instância de ambiente de preparo/CRM.</span><span class="sxs-lookup"><span data-stu-id="f7134-152">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="f7134-153">Faça uma cópia da solução e execute sua configuração e automatize as personalizações de fluxo no ambiente de preparo.</span><span class="sxs-lookup"><span data-stu-id="f7134-153">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="f7134-154">Teste a solução em uma instância de preparo/CRM.</span><span class="sxs-lookup"><span data-stu-id="f7134-154">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="f7134-155">Em caso de sucesso, importe como uma solução gerenciada para a instância de produção.</span><span class="sxs-lookup"><span data-stu-id="f7134-155">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="f7134-156">Instalar a sincronização de referências do Partner Center para o Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="f7134-156">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="f7134-157">Vá para [energia automatizada](https://flow.microsoft.com) e selecione **ambientes** no canto superior direito.</span><span class="sxs-lookup"><span data-stu-id="f7134-157">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="f7134-158">Isso mostrará as instâncias do CRM disponíveis.</span><span class="sxs-lookup"><span data-stu-id="f7134-158">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="f7134-159">Selecione a instância apropriada do CRM na lista suspensa no canto superior direito.</span><span class="sxs-lookup"><span data-stu-id="f7134-159">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="f7134-160">Selecione **soluções** na barra de navegação à esquerda.</span><span class="sxs-lookup"><span data-stu-id="f7134-160">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="f7134-161">Clique no link **abrir AppSource** no menu superior.</span><span class="sxs-lookup"><span data-stu-id="f7134-161">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Abrir AppSource":::

5. <span data-ttu-id="f7134-163">Procure **conectores de referências do Partner Center para Salesforce** na tela pop-up.</span><span class="sxs-lookup"><span data-stu-id="f7134-163">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. <span data-ttu-id="f7134-165">Clique no botão **obter agora** e em **continuar**.</span><span class="sxs-lookup"><span data-stu-id="f7134-165">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="f7134-166">Isso abre a página onde você pode selecionar o ambiente do Salesforce CRM para instalar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f7134-166">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="f7134-167">Concorde com os termos e condições.</span><span class="sxs-lookup"><span data-stu-id="f7134-167">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="CRMS disponíveis":::

8. <span data-ttu-id="f7134-169">Em seguida, você será direcionado para a página **gerenciar suas soluções** .</span><span class="sxs-lookup"><span data-stu-id="f7134-169">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="f7134-170">Navegue até "referências do Partner Center" usando os botões de seta na parte inferior da página.</span><span class="sxs-lookup"><span data-stu-id="f7134-170">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="f7134-171">A **instalação agendada** deve aparecer ao lado da solução de referências do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="f7134-171">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="f7134-172">A instalação levará 10-15 minutos.</span><span class="sxs-lookup"><span data-stu-id="f7134-172">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="f7134-173">Quando a instalação for concluída, navegue de volta para [Power Automate](https://flow.microsoft.com) e selecione **soluções** na área de navegação à esquerda.</span><span class="sxs-lookup"><span data-stu-id="f7134-173">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="f7134-174">Observe que a **sincronização de referências do Partner Center para o Salesforce** está disponível na lista de soluções.</span><span class="sxs-lookup"><span data-stu-id="f7134-174">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="f7134-175">Selecione **sincronização de referências do Partner Center para Salesforce**.</span><span class="sxs-lookup"><span data-stu-id="f7134-175">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="f7134-176">Os fluxos e as entidades automatizados de energia a seguir estão disponíveis:</span><span class="sxs-lookup"><span data-stu-id="f7134-176">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Fluxos do Salesforce":::



## <a name="configure-the-solution"></a><span data-ttu-id="f7134-178">Configurar a solução</span><span class="sxs-lookup"><span data-stu-id="f7134-178">Configure the solution</span></span>

1. <span data-ttu-id="f7134-179">Depois de instalar a solução em sua instância do CRM, navegue de volta para o [Power Automate](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="f7134-179">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="f7134-180">Na lista suspensa **ambientes** no canto superior direito, selecione a instância de CRM na qual você instalou a solução de automatização de energia.</span><span class="sxs-lookup"><span data-stu-id="f7134-180">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>
3. <span data-ttu-id="f7134-181">Será necessário criar conexões que associem as três contas de usuário:</span><span class="sxs-lookup"><span data-stu-id="f7134-181">You will need to create connections that associate the three user accounts:</span></span>
    - <span data-ttu-id="f7134-182">Usuário do Partner Center com credenciais de administrador de referências</span><span class="sxs-lookup"><span data-stu-id="f7134-182">Partner Center user with referrals admin credentials</span></span>
    - <span data-ttu-id="f7134-183">Eventos do Partner Center</span><span class="sxs-lookup"><span data-stu-id="f7134-183">Partner Center Events</span></span>
    - <span data-ttu-id="f7134-184">Administrador de CRM com os fluxos de energia automatizada na solução.</span><span class="sxs-lookup"><span data-stu-id="f7134-184">CRM admin with the Power Automate flows in the solution.</span></span>
4. <span data-ttu-id="f7134-185">Selecione **conexões** na barra de navegação à esquerda e selecione a solução "referências do Partner Center" na lista.</span><span class="sxs-lookup"><span data-stu-id="f7134-185">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

5. <span data-ttu-id="f7134-186">Crie uma conexão clicando em **criar uma conexão**.</span><span class="sxs-lookup"><span data-stu-id="f7134-186">Create a connection by clicking **Create a connection**.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Criar conexão":::

- <span data-ttu-id="f7134-188">Procure por referências do Partner Center (versão prévia) na barra de pesquisa no canto superior direito.</span><span class="sxs-lookup"><span data-stu-id="f7134-188">Search for Partner Center Referrals (preview) in the search bar on the top right corner.</span></span>

- <span data-ttu-id="f7134-189">Crie uma conexão para o usuário do Partner Center com a função de credenciais do administrador de referências.</span><span class="sxs-lookup"><span data-stu-id="f7134-189">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

-  <span data-ttu-id="f7134-190">Em seguida, crie uma conexão de eventos do Partner Center para o usuário do Partner Center com as credenciais do administrador de referências.</span><span class="sxs-lookup"><span data-stu-id="f7134-190">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

- <span data-ttu-id="f7134-191">Crie uma conexão para Common Data Service (ambiente atual) para o usuário administrador do CRM.</span><span class="sxs-lookup"><span data-stu-id="f7134-191">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

-  <span data-ttu-id="f7134-192">Depois de adicionar todas as conexões, você deverá ver as seguintes conexões em seu ambiente:</span><span class="sxs-lookup"><span data-stu-id="f7134-192">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Observar conexões":::

### <a name="edit-the-connections"></a><span data-ttu-id="f7134-194">Editar as conexões</span><span class="sxs-lookup"><span data-stu-id="f7134-194">Edit the connections</span></span>

1. <span data-ttu-id="f7134-195">Volte para a página soluções e selecione **solução padrão**.</span><span class="sxs-lookup"><span data-stu-id="f7134-195">Return to the Solutions page and select **Default Solution**.</span></span>  <span data-ttu-id="f7134-196">Selecione **referência de conexão (versão prévia)** clicando em **tudo**.</span><span class="sxs-lookup"><span data-stu-id="f7134-196">Select **Connection Reference (preview)** by clicking **All**.</span></span>
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Iniciar edição do conector":::

2. <span data-ttu-id="f7134-198">Edite cada uma das conexões uma por uma selecionando o ícone de três pontos.</span><span class="sxs-lookup"><span data-stu-id="f7134-198">Edit each of the Connections one by one by selecting the three dots icon.</span></span> <span data-ttu-id="f7134-199">Adicione as conexões relevantes.</span><span class="sxs-lookup"><span data-stu-id="f7134-199">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Editar conectores":::

3. <span data-ttu-id="f7134-201">Ative os fluxos na seguinte sequência:</span><span class="sxs-lookup"><span data-stu-id="f7134-201">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="f7134-202">Registro do webhook do Partner Center (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="f7134-202">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="f7134-203">Criar referência de co-venda-Salesforce para o Partner Center (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="f7134-203">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="f7134-204">Partner Center Microsoft co-vender atualizações de referência para o Salesforce (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="f7134-204">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="f7134-205">Partner Center para Salesforce (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="f7134-205">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="f7134-206">Salesforce para o Partner Center (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="f7134-206">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="f7134-207">Oportunidade do Salesforce para o Partner Center (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="f7134-207">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="f7134-208">Salesforce Microsoft Solutions para Partner Center (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="f7134-208">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="f7134-209">Usar APIs de webhook para registrar eventos de alteração de recurso</span><span class="sxs-lookup"><span data-stu-id="f7134-209">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="f7134-210">As APIs de webhook do Partner Center permitem que você se registre em eventos de alteração de recursos.</span><span class="sxs-lookup"><span data-stu-id="f7134-210">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="f7134-211">Esses eventos de alteração são enviados para a URL como postagens HTTP.</span><span class="sxs-lookup"><span data-stu-id="f7134-211">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="f7134-212">Para registrar sua URL, selecione o **registro do webhook do Partner Center (insider Preview)** fluxo automatizado de energia.</span><span class="sxs-lookup"><span data-stu-id="f7134-212">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="f7134-213">Adicione conexões para o usuário do centro de parceiros (a) com referências credenciais de administrador (b.) os eventos do centro de parceiros conforme realçado abaixo</span><span class="sxs-lookup"><span data-stu-id="f7134-213">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Gatilho":::

3. <span data-ttu-id="f7134-215">Ao fazer essas atualizações, você verá</span><span class="sxs-lookup"><span data-stu-id="f7134-215">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks":::

4. <span data-ttu-id="f7134-217">Salve as alterações e selecione **Ativar**.</span><span class="sxs-lookup"><span data-stu-id="f7134-217">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="f7134-218">Para habilitar o parceiro do Partner Center a ouvir as alterações de evento, execute as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="f7134-218">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="f7134-219">Selecione **Partner Center para SALESFORCE CRM (insider Preview)**.</span><span class="sxs-lookup"><span data-stu-id="f7134-219">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="f7134-220">Selecione o ícone **Editar** e selecione **quando uma solicitação HTTP é recebida**.</span><span class="sxs-lookup"><span data-stu-id="f7134-220">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="f7134-221">Selecione o ícone de **cópia** para copiar a URL de postagem http fornecida.</span><span class="sxs-lookup"><span data-stu-id="f7134-221">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Copiar URL":::

8. <span data-ttu-id="f7134-223">Agora, selecione o fluxo "registro do webhook do Partner Center (insider Preview)" automatizar fluxos de energia e selecione **executar**.</span><span class="sxs-lookup"><span data-stu-id="f7134-223">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="f7134-224">Verifique se a janela "executar fluxo" é aberta no painel direito e clique em **continuar**.</span><span class="sxs-lookup"><span data-stu-id="f7134-224">Ensure that the "Run Flow" window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="f7134-225">Insira os seguintes detalhes:</span><span class="sxs-lookup"><span data-stu-id="f7134-225">Enter the following details:</span></span>

    1. <span data-ttu-id="f7134-226">**Ponto de extremidade de gatilho http**: URL copiada da etapa anterior</span><span class="sxs-lookup"><span data-stu-id="f7134-226">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="f7134-227">**Eventos a serem registrados**: "referência criada" e "referência atualizada"</span><span class="sxs-lookup"><span data-stu-id="f7134-227">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="f7134-228">**Substituir pontos de extremidade de gatilho existentes, se presente**: Sim (isso substitui todos os pontos de extremidade existentes.)</span><span class="sxs-lookup"><span data-stu-id="f7134-228">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="f7134-229">Selecione **executar** e, em seguida, selecione **concluído.**</span><span class="sxs-lookup"><span data-stu-id="f7134-229">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="f7134-230">O webhook agora pode escutar criar e atualizar eventos.</span><span class="sxs-lookup"><span data-stu-id="f7134-230">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="f7134-231">Personalizar etapas de sincronização</span><span class="sxs-lookup"><span data-stu-id="f7134-231">Customize synchronization steps</span></span>

<span data-ttu-id="f7134-232">Quando as referências de venda cruzada são sincronizadas entre o Partner Center e o sistema CRM, os campos sincronizados no PC do Partner Center são listados aqui.</span><span class="sxs-lookup"><span data-stu-id="f7134-232">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="f7134-233">Geralmente, os sistemas CRM são altamente personalizados.</span><span class="sxs-lookup"><span data-stu-id="f7134-233">Often CRM systems are highly customized.</span></span> <span data-ttu-id="f7134-234">Você pode personalizar os fluxos de energia automatizada.</span><span class="sxs-lookup"><span data-stu-id="f7134-234">You can customize the Power Automate flows.</span></span> <span data-ttu-id="f7134-235">Siga o guia de mapeamento de campo e, se necessário, faça as alterações apropriadas nas etapas de fluxos de energia automatizar.</span><span class="sxs-lookup"><span data-stu-id="f7134-235">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="f7134-236">Os mapeamentos do Microsoft Partner centers para CRM são fornecidos, mas com base no seu ambiente de CRM, você pode optar por personalizar ainda mais os campos.</span><span class="sxs-lookup"><span data-stu-id="f7134-236">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="f7134-237">Várias etapas de cada um dos fluxos de energia automatizada podem ser personalizadas com base em suas necessidades.</span><span class="sxs-lookup"><span data-stu-id="f7134-237">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="f7134-238">Veja a seguir exemplos de personalizações disponíveis:</span><span class="sxs-lookup"><span data-stu-id="f7134-238">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="f7134-239">Para personalizar os campos de criação ou atualização de eventos no Partner Center para a sincronização de referência do CRM:</span><span class="sxs-lookup"><span data-stu-id="f7134-239">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="f7134-240">Selecione Partner Center para Salesforce CRM (insider Preview).</span><span class="sxs-lookup"><span data-stu-id="f7134-240">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="f7134-241">Selecione **Editar** para editar/personalizar o fluxo de automatização de energia.</span><span class="sxs-lookup"><span data-stu-id="f7134-241">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="f7134-242">Selecione **(escopo) sincronizar o cliente potencial ou a oportunidade**.</span><span class="sxs-lookup"><span data-stu-id="f7134-242">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="f7134-243">Para personalizar mapeamentos de campo de CRM para criar eventos, selecione **se for nova oportunidade compartilhada e, em seguida,**.</span><span class="sxs-lookup"><span data-stu-id="f7134-243">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="f7134-244">Selecione a subetapa **se sim** e, em seguida, expanda **criando uma nova oportunidade no CRM**.</span><span class="sxs-lookup"><span data-stu-id="f7134-244">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="f7134-245">Você pode editar os mapeamentos nesta seção usando o guia de mapeamento de campos.</span><span class="sxs-lookup"><span data-stu-id="f7134-245">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="f7134-246">Para personalizar mapeamentos de campo de CRM para eventos de atualização, clique na etapa "(escopo) sincronizar o cliente potencial ou a oportunidade".</span><span class="sxs-lookup"><span data-stu-id="f7134-246">To customize CRM field mappings for update events, click on the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="f7134-247">Selecione **se for uma atualização para uma oportunidade e, em seguida,**.</span><span class="sxs-lookup"><span data-stu-id="f7134-247">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="f7134-248">Selecione a subetapa **se sim** e, em seguida, expanda **se a diferença entre os objetos de oportunidade no Partner Center e no CRM, em seguida**.</span><span class="sxs-lookup"><span data-stu-id="f7134-248">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="f7134-249">Selecione **se sim** seguido de **Atualizar oportunidade existente**</span><span class="sxs-lookup"><span data-stu-id="f7134-249">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="f7134-250">Para personalizar os campos de sincronização de referência do CRM para PC para eventos de atualização:</span><span class="sxs-lookup"><span data-stu-id="f7134-250">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="f7134-251">Selecione **Editar**  para editar/personalizar o fluxo de automatização de energia.</span><span class="sxs-lookup"><span data-stu-id="f7134-251">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="f7134-252">Selecione **(escopo) sincronizar a oportunidade**.</span><span class="sxs-lookup"><span data-stu-id="f7134-252">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="f7134-253">Para personalizar os mapeamentos de campo do CRM (com base no guia mapeamentos de campo) para eventos de atualização, selecione **se houver diferença entre os objetos Lead no Partner Center e CRM, em seguida**.</span><span class="sxs-lookup"><span data-stu-id="f7134-253">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="f7134-254">Selecione a subetapa **se sim** e, em seguida, expanda a etapa **atualizar uma referência com dados de oportunidade**.</span><span class="sxs-lookup"><span data-stu-id="f7134-254">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="f7134-255">Você pode editar os mapeamentos nesta seção com base no guia de mapeamento de campos.</span><span class="sxs-lookup"><span data-stu-id="f7134-255">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="f7134-256">Para personalizar os campos para a sincronização de referência do CRM para PC para criar eventos?</span><span class="sxs-lookup"><span data-stu-id="f7134-256">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="f7134-257">Selecione **Editar**  para editar/personalizar o fluxo de automatização de energia.</span><span class="sxs-lookup"><span data-stu-id="f7134-257">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="f7134-258">Selecione **(escopo) sincronizando referências.**</span><span class="sxs-lookup"><span data-stu-id="f7134-258">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="f7134-259">Para personalizar mapeamentos de campo de CRM (com base no guia mapeamentos de campo) para criar eventos, selecione **criar referência da Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="f7134-259">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="f7134-260">Você pode editar os mapeamentos nesta seção com base no guia de mapeamento de campos.</span><span class="sxs-lookup"><span data-stu-id="f7134-260">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

### <a name="set-up-fields-and-relationships"></a><span data-ttu-id="f7134-261">Configurar campos e relações</span><span class="sxs-lookup"><span data-stu-id="f7134-261">Set up fields and relationships</span></span>

1. <span data-ttu-id="f7134-262">Entre em sua conta do Salesforce e vá para **oportunidade**.</span><span class="sxs-lookup"><span data-stu-id="f7134-262">Sign into your Salesforce account and go to **Opportunity**.</span></span>

2. <span data-ttu-id="f7134-263">Clique nas opções **Configurar** e **Editar objeto** para adicionar os campos necessários.</span><span class="sxs-lookup"><span data-stu-id="f7134-263">Click on the **Setup** and **Edit Object** options to add the necessary fields.</span></span>

3. <span data-ttu-id="f7134-264">Selecionar **campos & relações** no painel de navegação esquerdo</span><span class="sxs-lookup"><span data-stu-id="f7134-264">Select **Fields & Relationships** from the left navigation</span></span>

   :::image type="content" source="images/salesforce/fields1.png" alt-text="Fields":::

4. <span data-ttu-id="f7134-266">Adicione os campos a seguir nos **campos &** tabela de relações:</span><span class="sxs-lookup"><span data-stu-id="f7134-266">Add the following fields in the **Fields & Relationship** table:</span></span>

   |<span data-ttu-id="f7134-267">**Rótulo do campo**</span><span class="sxs-lookup"><span data-stu-id="f7134-267">**Field label**</span></span>   |<span data-ttu-id="f7134-268">**Nome do campo**</span><span class="sxs-lookup"><span data-stu-id="f7134-268">**Field name**</span></span>|<span data-ttu-id="f7134-269">**Data type**</span><span class="sxs-lookup"><span data-stu-id="f7134-269">**Data type**</span></span>|<span data-ttu-id="f7134-270">**Indexa**</span><span class="sxs-lookup"><span data-stu-id="f7134-270">**Indexed**</span></span>|
   |---------------------|:-------------------|:--------------|:----------------|
   |<span data-ttu-id="f7134-271">Audit</span><span class="sxs-lookup"><span data-stu-id="f7134-271">Audit</span></span>| <span data-ttu-id="f7134-272">Audit__c</span><span class="sxs-lookup"><span data-stu-id="f7134-272">Audit__c</span></span>|<span data-ttu-id="f7134-273">Área de texto longo (100.000) (linha visível 4)</span><span class="sxs-lookup"><span data-stu-id="f7134-273">Long Text Area(100000)(visible line 4)</span></span>||
   |<span data-ttu-id="f7134-274">Como a Microsoft pode ajudar?</span><span class="sxs-lookup"><span data-stu-id="f7134-274">How can Microsoft help?</span></span>|<span data-ttu-id="f7134-275">How_can_Microsoft_help_c</span><span class="sxs-lookup"><span data-stu-id="f7134-275">How_can_Microsoft_help_c</span></span>|<span data-ttu-id="f7134-276">Seleção</span><span class="sxs-lookup"><span data-stu-id="f7134-276">Picklist\*</span></span>|
   |<span data-ttu-id="f7134-277">Produtos</span><span class="sxs-lookup"><span data-stu-id="f7134-277">Products</span></span>|<span data-ttu-id="f7134-278">Products_c</span><span class="sxs-lookup"><span data-stu-id="f7134-278">Products_c</span></span>|<span data-ttu-id="f7134-279">texto (255)</span><span class="sxs-lookup"><span data-stu-id="f7134-279">text (255)</span></span>||
   |<span data-ttu-id="f7134-280">Indicação</span><span class="sxs-lookup"><span data-stu-id="f7134-280">Referral</span></span> | <span data-ttu-id="f7134-281">Referral_Identfier_c</span><span class="sxs-lookup"><span data-stu-id="f7134-281">Referral_Identfier_c</span></span>|<span data-ttu-id="f7134-282">Texto (100) (ID externa)</span><span class="sxs-lookup"><span data-stu-id="f7134-282">Text(100)(External ID)</span></span>|<span data-ttu-id="f7134-283">sim</span><span class="sxs-lookup"><span data-stu-id="f7134-283">yes</span></span>|
   |<span data-ttu-id="f7134-284">Link de referência</span><span class="sxs-lookup"><span data-stu-id="f7134-284">Referral Link</span></span>| <span data-ttu-id="f7134-285">Referral_Link_c_</span><span class="sxs-lookup"><span data-stu-id="f7134-285">Referral_Link_c_</span></span>|<span data-ttu-id="f7134-286">URL (255)</span><span class="sxs-lookup"><span data-stu-id="f7134-286">URL(255)</span></span>||
   |<span data-ttu-id="f7134-287">Sincronizar com o Partner Center</span><span class="sxs-lookup"><span data-stu-id="f7134-287">Sync with Partner Center</span></span>|<span data-ttu-id="f7134-288">sync_with_partner_center_c</span><span class="sxs-lookup"><span data-stu-id="f7134-288">sync_with_partner_center_c</span></span>|<span data-ttu-id="f7134-289">Caixa de seleção (padrão desmarcado)</span><span class="sxs-lookup"><span data-stu-id="f7134-289">Checkbox (default unchecked)</span></span>||

   <span data-ttu-id="f7134-290">\* Valores da lista de seleção:</span><span class="sxs-lookup"><span data-stu-id="f7134-290">\*Picklist values:</span></span>

   - <span data-ttu-id="f7134-291">Proposta de valor específico da carga de trabalho</span><span class="sxs-lookup"><span data-stu-id="f7134-291">Workload specific value proposition</span></span>
   - <span data-ttu-id="f7134-292">Arquitetura técnica do cliente</span><span class="sxs-lookup"><span data-stu-id="f7134-292">Customer technical architecture</span></span>
   - <span data-ttu-id="f7134-293">Prova de conceito ou demonstração</span><span class="sxs-lookup"><span data-stu-id="f7134-293">Proof of concept or demo</span></span>
   - <span data-ttu-id="f7134-294">Cotações ou licenciamento</span><span class="sxs-lookup"><span data-stu-id="f7134-294">Quotes or licensing</span></span>
   - <span data-ttu-id="f7134-295">Sucesso do cliente do post Sales</span><span class="sxs-lookup"><span data-stu-id="f7134-295">Post sales customer success</span></span>
   - <span data-ttu-id="f7134-296">Geral ou outros</span><span class="sxs-lookup"><span data-stu-id="f7134-296">General or other</span></span>

5. <span data-ttu-id="f7134-297">Os campos serão criados em **campos & relações**</span><span class="sxs-lookup"><span data-stu-id="f7134-297">The fields would get created under **Fields & Relationships**</span></span>

   :::image type="content" source="images/salesforce/fields2.png" alt-text="Campos criados":::

6. <span data-ttu-id="f7134-299">No layout da oportunidade, crie uma seção separada com os campos listados acima.</span><span class="sxs-lookup"><span data-stu-id="f7134-299">In the Opportunity layout, create a separate section with the fields as listed above.</span></span>

   - <span data-ttu-id="f7134-300">Esta seção deve estar disponível para os vendedores no layout da oportunidade</span><span class="sxs-lookup"><span data-stu-id="f7134-300">This section should be available for the sellers in the Opportunity layout</span></span>

   :::image type="content" source="images/salesforce/pc-fields-layout.png" alt-text="Layout de campos do Partner Center":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="f7134-302">Sincronização de referência de cooperação bidirecional de ponta a ponta</span><span class="sxs-lookup"><span data-stu-id="f7134-302">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="f7134-303">Depois de instalar, configurar e personalizar a solução de automatização de energia, você pode testar a sincronização de referências de venda entre o Salesforce CRM e o Partner Center.</span><span class="sxs-lookup"><span data-stu-id="f7134-303">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="f7134-304">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f7134-304">Pre-requisites</span></span>

<span data-ttu-id="f7134-305">Para sincronizar as referências no Partner Center e no Salesforce CRM, a solução de automatização de energia precisa demarcar claramente os campos de referência específicos da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f7134-305">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="f7134-306">Essa identificação fornece às suas equipes do vendedor a capacidade de decidir quais referências eles desejam compartilhar com a Microsoft para fazer a venda.</span><span class="sxs-lookup"><span data-stu-id="f7134-306">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="f7134-307">Um conjunto de campos personalizados está disponível como parte da sincronização de referências do Partner Center para a entidade **oportunidade** de solução do Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="f7134-307">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="f7134-308">Um usuário administrador de CRM precisará criar uma seção de CRM separada com os campos personalizados de **oportunidade** .</span><span class="sxs-lookup"><span data-stu-id="f7134-308">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="f7134-309">Os campos personalizados a seguir devem fazer parte da seção CRM:</span><span class="sxs-lookup"><span data-stu-id="f7134-309">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="f7134-310">**Sincronizar com o Partner Center**: se deseja sincronizar a oportunidade com o Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="f7134-310">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="f7134-311">**Identificador de referência**: um campo de identificador somente leitura para a referência do Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="f7134-311">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="f7134-312">**Link de referência**: um link somente leitura para a referência no Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="f7134-312">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="f7134-313">**Como a Microsoft pode ajudar**: a ajuda necessária da Microsoft para a referência</span><span class="sxs-lookup"><span data-stu-id="f7134-313">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="f7134-314">**Produtos**: lista de produtos associados a esta oportunidade</span><span class="sxs-lookup"><span data-stu-id="f7134-314">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="f7134-315">**Auditoria**: uma trilha de auditoria somente leitura para sincronização com as referências do Partner Center</span><span class="sxs-lookup"><span data-stu-id="f7134-315">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="f7134-316">EXEMPLOS</span><span class="sxs-lookup"><span data-stu-id="f7134-316">SCENARIOS:</span></span>

1. <span data-ttu-id="f7134-317">Sincronização de referência quando a referência é criada ou atualizada no CRM e sincronizada no Partner Center:</span><span class="sxs-lookup"><span data-stu-id="f7134-317">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="f7134-318">Entre no ambiente do Salesforce CRM com o usuário que tem visibilidade na seção **oportunidade** do CRM.</span><span class="sxs-lookup"><span data-stu-id="f7134-318">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="f7134-319">Verifique se a seção a seguir está presente quando você cria uma "nova oportunidade" no ambiente CRM do Salesforce</span><span class="sxs-lookup"><span data-stu-id="f7134-319">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Ambiente do Salesforce":::

   3. <span data-ttu-id="f7134-321">Para sincronizar essa oportunidade com o Microsoft Partner Center, certifique-se de definir os seguintes campos no modo de exibição de cartão:</span><span class="sxs-lookup"><span data-stu-id="f7134-321">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="f7134-322">"Sincronizar com o Partner Center": Sim</span><span class="sxs-lookup"><span data-stu-id="f7134-322">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="f7134-323">"Como a Microsoft pode ajudar?": selecione uma das seguintes opções:</span><span class="sxs-lookup"><span data-stu-id="f7134-323">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="f7134-324">Produtos: IDs de solução do produto</span><span class="sxs-lookup"><span data-stu-id="f7134-324">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="f7134-325">Depois de definir a opção sincronização de oportunidade  **com o Partner Center** como **Sim**, aguarde 10 minutos e entre em sua conta do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="f7134-325">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="f7134-326">Suas referências serão sincronizadas com o Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="f7134-326">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="f7134-327">Quando a opção "sincronizar com o Partner Center" for definida como "Sim", se você atualizar a oportunidade no Salesforce CRM, as alterações serão sincronizadas com sua conta do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="f7134-327">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="f7134-328">As oportunidades sincronizadas com êxito com o Partner Center serão identificadas com ✔ ícone no Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="f7134-328">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="f7134-329">Sincronização de referência quando a referência é criada ou atualizada no Microsoft Partner Center e sincronizada no ambiente do Salesforce CRM:</span><span class="sxs-lookup"><span data-stu-id="f7134-329">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="f7134-330">Entre no [painel](https://partner.microsoft.com/dashboard/home)do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="f7134-330">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="f7134-331">Selecione **referências** no menu à esquerda.</span><span class="sxs-lookup"><span data-stu-id="f7134-331">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="f7134-332">Crie uma nova referência de revenda do Partner Center clicando na opção "novo negócio".</span><span class="sxs-lookup"><span data-stu-id="f7134-332">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="f7134-333">Entre no ambiente do Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="f7134-333">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="f7134-334">Navegue até **oportunidades abertas**.</span><span class="sxs-lookup"><span data-stu-id="f7134-334">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="f7134-335">A referência criada no Microsoft Partner Center agora está sincronizada no Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="f7134-335">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Tela de oportunidade do Salesforce":::

    6. <span data-ttu-id="f7134-337">Quando você seleciona uma referência sincronizada, os detalhes da exibição do cartão são preenchidos.</span><span class="sxs-lookup"><span data-stu-id="f7134-337">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f7134-338">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="f7134-338">Next steps</span></span>

- [<span data-ttu-id="f7134-339">Gerenciar clientes potenciais</span><span class="sxs-lookup"><span data-stu-id="f7134-339">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="f7134-340">Gerenciar oportunidades de venda conjunta</span><span class="sxs-lookup"><span data-stu-id="f7134-340">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="f7134-341">Webhooks do Partner Center</span><span class="sxs-lookup"><span data-stu-id="f7134-341">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)