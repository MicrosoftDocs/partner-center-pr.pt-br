---
title: Gerenciar o licenciamento em ofertas do Marketplace
ms.topic: how-to
ms.date: 04/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como configurar e gerenciar o licenciamento para suas ofertas de Marketplace comercial de ISV.
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3b2281696a2fe69253cd033eb2a7eef7fb3046f3
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284865"
---
# <a name="manage-licensing-in-marketplace-offers"></a><span data-ttu-id="44283-103">Gerenciar o licenciamento em ofertas do Marketplace</span><span class="sxs-lookup"><span data-stu-id="44283-103">Manage licensing in marketplace offers</span></span>

<span data-ttu-id="44283-104">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="44283-104">**Appropriate roles**</span></span>

- <span data-ttu-id="44283-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="44283-105">Global admin</span></span>
- <span data-ttu-id="44283-106">Administrador de conta</span><span class="sxs-lookup"><span data-stu-id="44283-106">Account admin</span></span>

<span data-ttu-id="44283-107">Este artigo orienta você pelo processo de configuração de uma oferta no Partner Center, disponibilizando-o em Microsoft AppSource e, em seguida, gerenciando licenças para essa oferta.</span><span class="sxs-lookup"><span data-stu-id="44283-107">This article walks you through the process of setting up an offer in Partner Center, making it available in Microsoft AppSource, and then managing licenses for that offer.</span></span>  

>[!IMPORTANT]
><span data-ttu-id="44283-108">Os recursos neste artigo estão atualmente em visualização pública.</span><span class="sxs-lookup"><span data-stu-id="44283-108">The capabilities in this article are currently in Public Preview.</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="44283-109">Antes de começar</span><span class="sxs-lookup"><span data-stu-id="44283-109">Before you begin</span></span>

<span data-ttu-id="44283-110">Antes de iniciar este processo, você deve se familiarizar com as informações abaixo.</span><span class="sxs-lookup"><span data-stu-id="44283-110">Before beginning this process, you should familiarize yourself with the information below.</span></span>

### <a name="review-the-azure-marketplace-documentation"></a><span data-ttu-id="44283-111">Examine a documentação do Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="44283-111">Review the Azure Marketplace documentation</span></span>

<span data-ttu-id="44283-112">Os artigos abaixo contêm informações que você deve saber antes de continuar.</span><span class="sxs-lookup"><span data-stu-id="44283-112">The articles below contain information you should know before continuing.</span></span> 

- [<span data-ttu-id="44283-113">Criar uma oferta do Dynamics 365 for Customer Engagement e PowerApps</span><span class="sxs-lookup"><span data-stu-id="44283-113">Create a Dynamics 365 for Customer Engagement & PowerApps offer</span></span>](https://docs.microsoft.com/azure/marketplace/dynamics-365-customer-engage-offer-setup)
- [<span data-ttu-id="44283-114">Criar uma conta do Marketplace comercial no Partner Center</span><span class="sxs-lookup"><span data-stu-id="44283-114">Create a commercial marketplace account in Partner Center</span></span>](https://docs.microsoft.com/azure/marketplace/create-account)

### <a name="create-your-offer-id"></a><span data-ttu-id="44283-115">Criar sua ID de oferta</span><span class="sxs-lookup"><span data-stu-id="44283-115">Create your Offer ID</span></span>

<span data-ttu-id="44283-116">Nos procedimentos abaixo, você será solicitado a inserir uma ID de oferta.</span><span class="sxs-lookup"><span data-stu-id="44283-116">In the procedures below, you’ll be prompted to enter an Offer ID.</span></span> <span data-ttu-id="44283-117">Reserve algum tempo agora para criar uma ID de oferta adequada, tendo em mente os seguintes pontos:</span><span class="sxs-lookup"><span data-stu-id="44283-117">Take some time now to come up with a suitable Offer ID, keeping in mind the following points:</span></span>

- <span data-ttu-id="44283-118">Essa ID é visível para os clientes no endereço da Web para a oferta do Marketplace e nos modelos do Azure Resource Manager, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="44283-118">This ID is visible to customers in the web address for the marketplace offer and Azure Resource Manager templates, if applicable.</span></span>
- <span data-ttu-id="44283-119">A ID da oferta combinada com a ID do Publicador deve ter menos de 40 caracteres de comprimento.</span><span class="sxs-lookup"><span data-stu-id="44283-119">The Offer ID combined with the Publisher ID must be under 40 characters in length.</span></span>
- <span data-ttu-id="44283-120">Use apenas letras minúsculas e números.</span><span class="sxs-lookup"><span data-stu-id="44283-120">Use only lowercase letters and numbers.</span></span> <span data-ttu-id="44283-121">A ID da oferta pode incluir hifens e sublinhados, mas sem espaços.</span><span class="sxs-lookup"><span data-stu-id="44283-121">The Offer ID can include hyphens and underscores, but no spaces.</span></span> <span data-ttu-id="44283-122">Por exemplo, se sua ID de editor for testpublisherid e você inserir Test-offer-1, o endereço Web da oferta será https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1 .</span><span class="sxs-lookup"><span data-stu-id="44283-122">For example, if your Publisher ID is testpublisherid and you enter test-offer-1, the offer web address will be https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1.</span></span>
- <span data-ttu-id="44283-123">Essa ID não pode ser alterada depois que você seleciona **criar**.</span><span class="sxs-lookup"><span data-stu-id="44283-123">This ID can't be changed after you select **Create**.</span></span>

### <a name="create-your-offer-alias"></a><span data-ttu-id="44283-124">Criar seu alias de oferta</span><span class="sxs-lookup"><span data-stu-id="44283-124">Create your Offer alias</span></span>

<span data-ttu-id="44283-125">O alias da oferta é o nome usado para a oferta no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="44283-125">The Offer alias is the name used for the offer in Partner Center.</span></span> <span data-ttu-id="44283-126">Você também precisará de um alias de oferta apropriado que siga as diretrizes abaixo:</span><span class="sxs-lookup"><span data-stu-id="44283-126">You’ll also need an appropriate Offer alias that follows the guidelines below:</span></span>

- <span data-ttu-id="44283-127">Esse nome não é usado no Marketplace e é diferente do nome da oferta e de outros valores mostrados aos clientes.</span><span class="sxs-lookup"><span data-stu-id="44283-127">This name isn't used in the marketplace and is different from the offer name and other values shown to customers.</span></span>
- <span data-ttu-id="44283-128">Esse nome não pode ser alterado depois que você seleciona criar.</span><span class="sxs-lookup"><span data-stu-id="44283-128">This name can't be changed after you select Create.</span></span>

## <a name="create-your-offer"></a><span data-ttu-id="44283-129">Criar sua oferta</span><span class="sxs-lookup"><span data-stu-id="44283-129">Create your offer</span></span>

<span data-ttu-id="44283-130">A primeira etapa do processo de licenciamento é criar sua oferta do Marketplace comercial.</span><span class="sxs-lookup"><span data-stu-id="44283-130">The first step in the licensing process is to create your commercial marketplace offer.</span></span> 

1. <span data-ttu-id="44283-131">Entre no painel [Partner Center](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="44283-131">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="44283-132">No menu de navegação à esquerda, selecione **Marketplace comercial/visão geral**.</span><span class="sxs-lookup"><span data-stu-id="44283-132">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="44283-133">Na parte superior da página Visão geral, selecione **nova oferta** e, em seguida, selecione **Dynamics 365 para compromisso com o cliente & PowerApps**.</span><span class="sxs-lookup"><span data-stu-id="44283-133">At the top of the Overview page, select **New offer**, and then select **Dynamics 365 for Customer Engagement & PowerApps**.</span></span>
4. <span data-ttu-id="44283-134">Insira a **ID da oferta** e o **alias da oferta** que você criou anteriormente.</span><span class="sxs-lookup"><span data-stu-id="44283-134">Enter the **Offer ID** and **Offer alias** you created earlier.</span></span>
5. <span data-ttu-id="44283-135">Selecione **Criar** para gerar a oferta e continuar.</span><span class="sxs-lookup"><span data-stu-id="44283-135">Select **Create** to generate the offer and continue.</span></span>
6. <span data-ttu-id="44283-136">Escolha suas opções de licenciamento.</span><span class="sxs-lookup"><span data-stu-id="44283-136">Choose your licensing options.</span></span>

    - <span data-ttu-id="44283-137">Para habilitar o gerenciamento de licenças para sua oferta, selecione **habilitar o gerenciamento de licenças de aplicativos por meio da Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="44283-137">To enable license management for your offer, select **Enable app license management through Microsoft**.</span></span> <span data-ttu-id="44283-138">Essa é uma configuração única, e você não poderá alterá-la depois que sua oferta for publicada.</span><span class="sxs-lookup"><span data-stu-id="44283-138">This is a one-time setting, and you can’t change it once your offer is published.</span></span>

    - <span data-ttu-id="44283-139">Você também pode permitir que os clientes executem a funcionalidade base do aplicativo sem uma licença e executem recursos premium depois de adquirirem uma licença.</span><span class="sxs-lookup"><span data-stu-id="44283-139">You can also enable customers to run your app’s base functionality without a license, and run premium features once they’ve purchased a license.</span></span> <span data-ttu-id="44283-140">Para fazer isso, selecione **permitir que os clientes instalem meu aplicativo mesmo se as licenças não forem atribuídas**.</span><span class="sxs-lookup"><span data-stu-id="44283-140">To do this, select **Allow customers to install my app even if licenses are not assigned**.</span></span>

    - <span data-ttu-id="44283-141">Se você não quiser que sua oferta tenha o gerenciamento de licenças habilitado, selecione **obtê-lo agora (gratuito)**, **avaliação gratuita** ou **entre em contato comigo**.</span><span class="sxs-lookup"><span data-stu-id="44283-141">If you don’t want your offer to have license management enabled, select **Get it now (Free)**, **Free trial**, or **Contact me**.</span></span>

## <a name="create-your-plan"></a><span data-ttu-id="44283-142">Criar o plano</span><span class="sxs-lookup"><span data-stu-id="44283-142">Create your plan</span></span>

<span data-ttu-id="44283-143">Nestas etapas, você definirá o plano ou planos que deseja habilitar para sua oferta.</span><span class="sxs-lookup"><span data-stu-id="44283-143">In these steps you’ll define the plan or plans you want to enable for your offer.</span></span>

1. <span data-ttu-id="44283-144">No menu de navegação à esquerda, selecione **visão geral do plano** e, em seguida, selecione **criar novo plano**.</span><span class="sxs-lookup"><span data-stu-id="44283-144">On the left navigation menu, select **Plan overview**, and then select **Create new plan**.</span></span>
2. <span data-ttu-id="44283-145">Insira uma **ID do plano** e o **nome do plano** e, em seguida, selecione **criar**.</span><span class="sxs-lookup"><span data-stu-id="44283-145">Enter a **Plan ID** and **Plan name**, and then select **Create**.</span></span>
3. <span data-ttu-id="44283-146">Na página de **listagem do plano** , insira a descrição do **plano**.</span><span class="sxs-lookup"><span data-stu-id="44283-146">On the **Plan listing** page, enter your **Plan description**.</span></span>
4. <span data-ttu-id="44283-147">Para salvar a descrição e concluir mais tarde, selecione **salvar rascunho**.</span><span class="sxs-lookup"><span data-stu-id="44283-147">To save the description and finish later, select **Save draft**.</span></span>

5. <span data-ttu-id="44283-148">Quando tiver terminado, selecione **revisar e publicar**.</span><span class="sxs-lookup"><span data-stu-id="44283-148">When you’re finished, select **Review and publish**.</span></span> <span data-ttu-id="44283-149">As informações do plano agora serão exibidas em appsource.microsoft.com Em listagem de oferta (seção planos).</span><span class="sxs-lookup"><span data-stu-id="44283-149">The plan information will now be displayed on appsource.microsoft.com under offer listing (plans section).</span></span>

6. <span data-ttu-id="44283-150">Depois de criar todos os planos para esta oferta, você precisará copiar a ID de serviço de cada plano.</span><span class="sxs-lookup"><span data-stu-id="44283-150">After you’ve created all of the plans for this offer, you’ll need to copy each plan’s Service ID.</span></span> <span data-ttu-id="44283-151">Selecione **visão geral do plano** na parte superior da página de listagem do plano.</span><span class="sxs-lookup"><span data-stu-id="44283-151">Select **Plan overview** at the top of the Plan listing page.</span></span> <span data-ttu-id="44283-152">Copie a ID de serviço de cada plano para um local seguro.</span><span class="sxs-lookup"><span data-stu-id="44283-152">Copy the Service ID for each plan to a safe location.</span></span>

## <a name="add-service-ids-to-your-solution"></a><span data-ttu-id="44283-153">Adicionar IDs de serviço à sua solução</span><span class="sxs-lookup"><span data-stu-id="44283-153">Add Service IDs to your solution</span></span>

<span data-ttu-id="44283-154">A próxima etapa é atualizar sua solução adicionando as IDs de serviço para cada plano que você acabou de copiar.</span><span class="sxs-lookup"><span data-stu-id="44283-154">The next step is to update your solution by adding the Service IDs for each plan that you just copied.</span></span> <span data-ttu-id="44283-155">Para obter diretrizes sobre isso, consulte [criar um pacote AppSource para sua solução](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource).</span><span class="sxs-lookup"><span data-stu-id="44283-155">For guidance on this, see [Create an AppSource Package for your solution](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource).</span></span>

## <a name="upload-your-package-and-publish-your-offer"></a><span data-ttu-id="44283-156">Carregue seu pacote e publique sua oferta</span><span class="sxs-lookup"><span data-stu-id="44283-156">Upload your package and publish your offer</span></span>

1. <span data-ttu-id="44283-157">No painel de navegação esquerdo, selecione **Marketplace comercial** e, em seguida, selecione **configuração técnica**.</span><span class="sxs-lookup"><span data-stu-id="44283-157">On the left navigation pane, select **Commercial Marketplace**, and then select **Technical configuration**.</span></span>
2. <span data-ttu-id="44283-158">Em **modelo de licença base**, selecione **usuário**.</span><span class="sxs-lookup"><span data-stu-id="44283-158">Under **Base License Model**, select **User**.</span></span>
3. <span data-ttu-id="44283-159">Em **pacote do CRM**, insira a URL do local do pacote.</span><span class="sxs-lookup"><span data-stu-id="44283-159">Under **CRM Package**, enter the URL of your package location.</span></span>
4. <span data-ttu-id="44283-160">Use as outras guias no painel de navegação esquerdo para inserir outras informações necessárias.</span><span class="sxs-lookup"><span data-stu-id="44283-160">Use the other tabs on the left navigation pane to enter any other required information.</span></span> <span data-ttu-id="44283-161">Quando terminar, selecione **revisar e publicar**.</span><span class="sxs-lookup"><span data-stu-id="44283-161">When you’re done, select **Review and publish**.</span></span>

<span data-ttu-id="44283-162">Depois de publicar a oferta, vamos revisar e verificar suas informações.</span><span class="sxs-lookup"><span data-stu-id="44283-162">After you publish the offer, we’ll review and verify your information.</span></span> <span data-ttu-id="44283-163">Se houver algum problema com esse processo, você será notificado.</span><span class="sxs-lookup"><span data-stu-id="44283-163">If there are any issues with this process, we’ll notify you.</span></span> <span data-ttu-id="44283-164">Quando todos os problemas forem resolvidos, você receberá uma notificação de que sua oferta está disponível no AppSource.</span><span class="sxs-lookup"><span data-stu-id="44283-164">When all issues have been resolved, you’ll get a notification that your offer is available in AppSource.</span></span> <span data-ttu-id="44283-165">Nesse ponto, você pode torná-lo dinâmico.</span><span class="sxs-lookup"><span data-stu-id="44283-165">At that point you can make it live.</span></span>

## <a name="make-your-offer-live-in-partner-center"></a><span data-ttu-id="44283-166">Torne sua oferta ativa no Partner Center</span><span class="sxs-lookup"><span data-stu-id="44283-166">Make your offer live in Partner Center</span></span>

<span data-ttu-id="44283-167">O procedimento a seguir orienta você pelo processo de tornar sua oferta ativa no AppSource.</span><span class="sxs-lookup"><span data-stu-id="44283-167">The procedure below walks you through the process of making your offer live in AppSource.</span></span> <span data-ttu-id="44283-168">Para saber mais sobre esse processo, consulte [introdução às opções de listagem](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type).</span><span class="sxs-lookup"><span data-stu-id="44283-168">To learn more about this process, see [Introduction to listing options](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type).</span></span>

>[!NOTE]
><span data-ttu-id="44283-169">Depois de publicar sua oferta, levará 4-6 horas para entrar em tempo real.</span><span class="sxs-lookup"><span data-stu-id="44283-169">Once you publish your offer, it will take 4-6 hours to go live.</span></span>

1. <span data-ttu-id="44283-170">Entre no painel [Partner Center](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="44283-170">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="44283-171">No menu de navegação à esquerda, selecione **Marketplace comercial/visão geral**.</span><span class="sxs-lookup"><span data-stu-id="44283-171">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="44283-172">Na página **visão geral** , localize a oferta que você está procurando.</span><span class="sxs-lookup"><span data-stu-id="44283-172">On the **Overview** page, find the offer you’re looking for.</span></span> <span data-ttu-id="44283-173">As ofertas prontas para serem publicadas terão um status de versão **prévia**.</span><span class="sxs-lookup"><span data-stu-id="44283-173">Offers ready to be published will have a status of **Preview**.</span></span> <span data-ttu-id="44283-174">Selecione a oferta.</span><span class="sxs-lookup"><span data-stu-id="44283-174">Select the offer.</span></span>
4. <span data-ttu-id="44283-175">Na página **visão geral da oferta** , selecione **entrar em tempo real**.</span><span class="sxs-lookup"><span data-stu-id="44283-175">On the **Offer overview** page, select **Go live**.</span></span>
<span data-ttu-id="44283-176">A oferta será ativa em 4-6 horas.</span><span class="sxs-lookup"><span data-stu-id="44283-176">The offer will be live in 4-6 hours.</span></span>
5. <span data-ttu-id="44283-177">Para ver sua listagem de ofertas em AppSource, selecione o link **AppSource** na parte inferior da página **visão geral da oferta** .</span><span class="sxs-lookup"><span data-stu-id="44283-177">To see your offer listing on AppSource, select the **AppSource** link at the bottom of the **Offer overview** page.</span></span>

    - <span data-ttu-id="44283-178">**Para ofertas habilitadas para licença**: se sua oferta exigir uma verificação de licença, os usuários só poderão inserir um cliente potencial clicando **em entrar em contato comigo**, para que você possa se comunicar com eles.</span><span class="sxs-lookup"><span data-stu-id="44283-178">**For license-enabled offers**: If your offer requires a license check, users will only be able to enter a lead by clicking **Contact Me**, so that you can communicate with them.</span></span>

    - <span data-ttu-id="44283-179">**Para ofertas com licença habilitada com a opção de instalação gratuita**: se sua oferta não exigir uma verificação de licença, os usuários administradores verão um botão **obter agora** , além de **entrar em contato comigo**.</span><span class="sxs-lookup"><span data-stu-id="44283-179">**For license-enabled offers with free installation option**: If your offer does not require a license check, admin users will see a **Get It Now** button in addition to **Contact Me**.</span></span> <span data-ttu-id="44283-180">Os usuários que desejam experimentar sua opção de instalação gratuita devem clicar em **obter agora**, o que os levará para instalar a oferta no centro de administração do Power Platform.</span><span class="sxs-lookup"><span data-stu-id="44283-180">Users who want to try your free installation option should click **Get It Now**, which will bring them to install the offer on Power Platform Admin Center.</span></span> <span data-ttu-id="44283-181">Os usuários ainda poderão usar **entrar em contato comigo** se tiverem alguma dúvida ou se quiserem atualizar para um plano pago.</span><span class="sxs-lookup"><span data-stu-id="44283-181">Users can still use **Contact Me** if they have any questions, or if they want to upgrade to a paid plan.</span></span>

## <a name="register-isv-connect-deal-in-dealreg"></a><span data-ttu-id="44283-182">Registrar o negócio do ISV Connect no DealReg</span><span class="sxs-lookup"><span data-stu-id="44283-182">Register ISV Connect deal in DealReg</span></span>

<span data-ttu-id="44283-183">A próxima etapa é registrar seu negócio.</span><span class="sxs-lookup"><span data-stu-id="44283-183">The next step is to register your deal.</span></span> <span data-ttu-id="44283-184">Para fazer isso, consulte [registrar suas negociações](https://docs.microsoft.com/partner-center/register-deals).</span><span class="sxs-lookup"><span data-stu-id="44283-184">To do this, see [Register your deals](https://docs.microsoft.com/partner-center/register-deals).</span></span>

## <a name="invite-the-customer"></a><span data-ttu-id="44283-185">Convidar o cliente</span><span class="sxs-lookup"><span data-stu-id="44283-185">Invite the customer</span></span>

<span data-ttu-id="44283-186">Use o procedimento a seguir para convidar o cliente a participar desse negócio.</span><span class="sxs-lookup"><span data-stu-id="44283-186">Use the following procedure to invite the customer to participate in this deal.</span></span>  

1. <span data-ttu-id="44283-187">Entre no painel [Partner Center](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="44283-187">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="44283-188">No menu de navegação à esquerda, selecione **Marketplace comercial/visão geral**.</span><span class="sxs-lookup"><span data-stu-id="44283-188">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="44283-189">Filtrar para negociações **enviadas** , selecione a guia **em andamento** e, em seguida, selecione o negócio desejado.</span><span class="sxs-lookup"><span data-stu-id="44283-189">Filter for **Submitted** deals, select the **In Progress** tab, and then select the deal you want.</span></span>
4. <span data-ttu-id="44283-190">Na página Visão geral desse negócio, selecione **gerenciar licenças**.</span><span class="sxs-lookup"><span data-stu-id="44283-190">On the overview page for this deal, select **Manage licenses**.</span></span>
5. <span data-ttu-id="44283-191">Na janela **gerenciar licenças** , selecione o cliente na lista suspensa **detalhes do cliente** .</span><span class="sxs-lookup"><span data-stu-id="44283-191">In the **Manage licenses** window, select the customer from the **Customer details** dropdown list.</span></span> <span data-ttu-id="44283-192">Se a relação do cliente ainda não existir, selecione **+ convidar um novo cliente para consentir**.</span><span class="sxs-lookup"><span data-stu-id="44283-192">If the customer relationship does not exist yet, select **+Invite a new customer to consent**.</span></span>
6. <span data-ttu-id="44283-193">Copie o link que é exibido.</span><span class="sxs-lookup"><span data-stu-id="44283-193">Copy the link that is displayed.</span></span>
7. <span data-ttu-id="44283-194">Envie este link por email para o administrador de cobrança ou administrador global do seu cliente e faça com que eles usem esse link para acessar o admin.microsoft.com e aceitar e autorizar a relação que você está estabelecendo.</span><span class="sxs-lookup"><span data-stu-id="44283-194">Email this link to your customer’s billing admin or global admin, and have them use this link to access admin.microsoft.com and accept and authorize the relationship you’re establishing.</span></span>

    >[!NOTE]
    ><span data-ttu-id="44283-195">A relação não será estabelecida até que o cliente execute esta etapa.</span><span class="sxs-lookup"><span data-stu-id="44283-195">The relationship will not be established until the customer performs this step.</span></span>

## <a name="activate-manage-and-remove-your-licenses"></a><span data-ttu-id="44283-196">Ativar, gerenciar e remover suas licenças</span><span class="sxs-lookup"><span data-stu-id="44283-196">Activate, manage, and remove your licenses</span></span>

<span data-ttu-id="44283-197">Depois que o cliente tiver sido estabelecido, você poderá começar a adicionar planos de sua oferta e atribuir licenças a cada plano.</span><span class="sxs-lookup"><span data-stu-id="44283-197">Once your customer has been established, you can start adding plans from your offer and assigning licenses to each plan.</span></span>

1. <span data-ttu-id="44283-198">Na janela Gerenciar licenças para esse negócio, selecione **+ Adicionar um plano**.</span><span class="sxs-lookup"><span data-stu-id="44283-198">In the Manage licenses window for this deal, select **+Add a plan**.</span></span>
2. <span data-ttu-id="44283-199">Preencha os **planos para esta solução** e **número de campos de licenças** e, em seguida, selecione **Atualizar licenças**.</span><span class="sxs-lookup"><span data-stu-id="44283-199">Complete the **Plans for this solution** and **Number of licenses** fields, and then select **Update licenses**.</span></span> <span data-ttu-id="44283-200">As licenças estarão disponíveis em admin.microsoft.com para que os clientes gerenciem e atribuam a funcionários.</span><span class="sxs-lookup"><span data-stu-id="44283-200">The licenses will be available at admin.microsoft.com for customers to manage and assign to employees.</span></span>

    - <span data-ttu-id="44283-201">Para alterar o número de licenças de um plano existente, insira o novo número no campo **número de licenças** e, em seguida, selecione **Atualizar licenças**.</span><span class="sxs-lookup"><span data-stu-id="44283-201">To change the number of licenses for an existing plan, enter the new number in the **Number of licenses** field and then select **Update licenses**.</span></span>

    - <span data-ttu-id="44283-202">Para desativar ou remover licenças de um negócio, selecione o ícone de lixeira no campo **ações** e, em seguida, selecione **Atualizar licenças**.</span><span class="sxs-lookup"><span data-stu-id="44283-202">To deactivate or remove licenses for a deal, select the trash can icon in the **Actions** field and then select **Update licenses**.</span></span>