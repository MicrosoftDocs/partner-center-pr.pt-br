---
title: Migrar do Dynamics 365 e plano de envolvimento de cliente de Basic (ofertas qualificadas) para versões mais recentes | Partner Center
ms.topic: article
ms.date: 12/12/2018
description: Dynamics 365 for Sales / plano de envolvimento de cliente de assinaturas Basic (oferece qualificado) não pode ser renovada.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: labrenne
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 offers, renew offers, new Dynamics 365 SKUs
ms.openlocfilehash: b4b25dd80a684c9060b28461a9e6f594651ae224
ms.sourcegitcommit: 23adf424dd43ed0281473f97d535d73c59c92b01
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/13/2018
ms.locfileid: "8968266"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="6e003-103">Migrar do Dynamics 365 e plano de envolvimento de cliente de Basic (ofertas qualificadas) para versões mais recentes</span><span class="sxs-lookup"><span data-stu-id="6e003-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

**<span data-ttu-id="6e003-104">Aplica-se ao</span><span class="sxs-lookup"><span data-stu-id="6e003-104">Applies to</span></span>**

-  <span data-ttu-id="6e003-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="6e003-105">Partner Center</span></span>

<span data-ttu-id="6e003-106">Clientes de 1º de janeiro de 2019, eficazes com Dynamics 365 for Sales / plano de envolvimento de cliente de assinaturas Basic (oferece qualificado) não pode renovar essas ofertas herdadas; as assinaturas existentes não serão renovadas automaticamente quando expirarem.</span><span class="sxs-lookup"><span data-stu-id="6e003-106">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="6e003-107">Na página de detalhes da assinatura, o status da assinatura será alterado para "Expira em [Data]" de "Renovação automática em [Data]".</span><span class="sxs-lookup"><span data-stu-id="6e003-107">On the subscription’s detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 


<span data-ttu-id="6e003-108">Para garantir a continuidade dos clientes, você deve fazer a transição aqueles com assinaturas E4 vencidas para uma opção com suporte, listada abaixo.</span><span class="sxs-lookup"><span data-stu-id="6e003-108">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="6e003-109">É recomendável mover os clientes para as novas assinaturas antes da data de término da assinatura anual, para evitar possíveis interrupções de serviço.</span><span class="sxs-lookup"><span data-stu-id="6e003-109">We recommend moving customers to new subscriptions before the subscription’s yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="6e003-110">Se você usar a API (CREST ou Partner Center), você pode encontrar assinaturas vencidas avaliando a data de término da assinatura juntamente com automática = falsa propriedade.</span><span class="sxs-lookup"><span data-stu-id="6e003-110">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="6e003-111">As assinaturas em questão serão definidas como automático renovar = falso em 1º de janeiro de 2019.</span><span class="sxs-lookup"><span data-stu-id="6e003-111">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="6e003-112">Você pode mover os clientes para um novo plano a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="6e003-112">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="6e003-113">O Dynamics 365 oferece sendo desativado</span><span class="sxs-lookup"><span data-stu-id="6e003-113">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="6e003-114">Dynamics 365 para venda Enterprise Edition CRMOL Basic (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="6e003-114">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="6e003-115">Dynamics 365 para venda Enterprise Edition CRMOL Basic (oferta qualificada) para professores</span><span class="sxs-lookup"><span data-stu-id="6e003-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="6e003-116">Dynamics 365 para venda Enterprise Edition CRMOL Basic (oferta qualificada) para estudantes</span><span class="sxs-lookup"><span data-stu-id="6e003-116">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="6e003-117">Dynamics 365 para venda Enterprise Edition (preço do governo dos Estados Unidos) CRMOL Basic (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="6e003-117">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="6e003-118">Dynamics 365 para a edição Enterprise vendas do SA para CRM Basic (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="6e003-118">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="6e003-119">Dynamics 365 para a edição Enterprise vendas do SA para CRM Basic (oferta qualificada) para professores</span><span class="sxs-lookup"><span data-stu-id="6e003-119">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="6e003-120">Dynamics 365 para a edição Enterprise vendas do SA para CRM Basic (oferta qualificada) para estudantes</span><span class="sxs-lookup"><span data-stu-id="6e003-120">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="6e003-121">Dynamics 365 para venda Enterprise Edition (preço do governo dos Estados Unidos) do SA para CRM Basic (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="6e003-121">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="6e003-122">Dynamics 365 para venda Enterprise Edition complemento para o CRM Basic (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="6e003-122">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="6e003-123">Dynamics 365 para venda Enterprise Edition complemento para o CRM Basic (oferta qualificada) para professores</span><span class="sxs-lookup"><span data-stu-id="6e003-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="6e003-124">Dynamics 365 para venda Enterprise Edition complemento para o CRM Basic (oferta qualificada) para estudantes</span><span class="sxs-lookup"><span data-stu-id="6e003-124">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="6e003-125">Dynamics 365 para venda Enterprise Edition (preço do governo dos Estados Unidos) complemento para o CRM Basic (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="6e003-125">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="6e003-126">Dynamics 365 Customer envolvimento plano Enterprise Edition CRMOL Basic (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="6e003-126">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="6e003-127">Dynamics 365 Customer envolvimento plano Enterprise Edition (preço do governo dos Estados Unidos) CRMOL Basic (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="6e003-127">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="6e003-128">Dynamics 365 cliente envolvimento plano Enterprise Edition CRMOL Basic (oferta qualificada) para estudantes</span><span class="sxs-lookup"><span data-stu-id="6e003-128">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="6e003-129">Dynamics 365 Customer envolvimento plano Enterprise Edition CRMOL Basic (oferta qualificada) para professores</span><span class="sxs-lookup"><span data-stu-id="6e003-129">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="6e003-130">Dynamics 365 Customer envolvimento plano Enterprise Edition do SA para CRM Basic (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="6e003-130">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="6e003-131">Dynamics 365 Customer envolvimento plano edição Enterprise (preço do governo dos Estados Unidos) do SA para CRM Basic (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="6e003-131">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="6e003-132">Dynamics 365 Customer envolvimento plano Enterprise Edition do SA para CRM Basic (oferta qualificada) para estudantes</span><span class="sxs-lookup"><span data-stu-id="6e003-132">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="6e003-133">Envolvimento do cliente de Dynamics 365 plano edição Enterprise do SA para CRM Basic (oferta qualificada) para professores</span><span class="sxs-lookup"><span data-stu-id="6e003-133">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="6e003-134">Dynamics 365 cliente envolvimento plano Enterprise Edition complemento para CRM Basic (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="6e003-134">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="6e003-135">Dynamics 365 cliente envolvimento plano Enterprise Edition (preço do governo dos Estados Unidos) complemento para CRM Basic (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="6e003-135">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="6e003-136">Dynamics 365 cliente envolvimento plano Enterprise Edition complemento para CRM Basic (oferta qualificada) para estudantes</span><span class="sxs-lookup"><span data-stu-id="6e003-136">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="6e003-137">Dynamics 365 Customer envolvimento plano Enterprise Edition complemento para CRM Basic (oferta qualificada) para professores</span><span class="sxs-lookup"><span data-stu-id="6e003-137">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="6e003-138">Dynamics 365 for Sales / planos de plano de envolvimento de cliente de substituição Basic (oferece qualificado)</span><span class="sxs-lookup"><span data-stu-id="6e003-138">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

**<span data-ttu-id="6e003-139">Ofertas desativadas</span><span class="sxs-lookup"><span data-stu-id="6e003-139">Retired offers</span></span>**   

- <span data-ttu-id="6e003-140">Dynamics 365 para vendas do CRM Basic ou CRMOL Basic (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="6e003-140">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="6e003-141">Dynamics 365 Customer Engagement Plan do CRM Basic ou CRMOL Basic (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="6e003-141">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

**<span data-ttu-id="6e003-142">Opções de substituição</span><span class="sxs-lookup"><span data-stu-id="6e003-142">Replacement options</span></span>**
- <span data-ttu-id="6e003-143">Dynamics 365 para venda Professional (novo)</span><span class="sxs-lookup"><span data-stu-id="6e003-143">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="6e003-144">Dynamics 365 para venda Professional (novo)</span><span class="sxs-lookup"><span data-stu-id="6e003-144">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="6e003-145">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="6e003-145">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="6e003-146">Dynamics 365 Customer Engagement Plan ou</span><span class="sxs-lookup"><span data-stu-id="6e003-146">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="6e003-147">Membros da equipe do Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="6e003-147">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="6e003-148">Transição dos clientes para novos planos do produto</span><span class="sxs-lookup"><span data-stu-id="6e003-148">Transition customers to new product plans</span></span>

<span data-ttu-id="6e003-149">Mover os clientes de SKUs desativadas para as mais recentes requer as etapas a seguir nesta ordem:</span><span class="sxs-lookup"><span data-stu-id="6e003-149">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="6e003-150">Comprar a nova assinatura</span><span class="sxs-lookup"><span data-stu-id="6e003-150">Purchase the new subscription</span></span>
- <span data-ttu-id="6e003-151">Reatribuir as licenças de usuário atuais</span><span class="sxs-lookup"><span data-stu-id="6e003-151">Reassign current user licenses</span></span>
- <span data-ttu-id="6e003-152">Cancelar a assinatura antiga</span><span class="sxs-lookup"><span data-stu-id="6e003-152">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="6e003-153">O novo plano de compra para seu cliente</span><span class="sxs-lookup"><span data-stu-id="6e003-153">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="6e003-154">Selecione **os clientes** no painel de navegação esquerdo e, em seguida, selecione o cliente que você deseja mover para a nova assinatura.</span><span class="sxs-lookup"><span data-stu-id="6e003-154">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="6e003-155">Selecione **Adicionar assinatura**.</span><span class="sxs-lookup"><span data-stu-id="6e003-155">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="6e003-156">Selecione a assinatura que deseja comprar no catálogo (nesse caso, uma das opções acima), insira o número de licenças e selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="6e003-156">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="6e003-157">Seu cliente agora terá a assinatura antiga e uma nova.</span><span class="sxs-lookup"><span data-stu-id="6e003-157">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="6e003-158">A próxima etapa é reatribuir as licenças para os usuários do cliente.</span><span class="sxs-lookup"><span data-stu-id="6e003-158">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="6e003-159">Selecione **os clientes** no painel de navegação esquerdo e, em seguida, selecione o cliente que você está movendo.</span><span class="sxs-lookup"><span data-stu-id="6e003-159">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="6e003-160">Selecione **Usuários e licenças**.</span><span class="sxs-lookup"><span data-stu-id="6e003-160">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="6e003-161">Para reatribuir uma licença para um usuário, selecione o usuário e, em seguida, selecione **Gerenciar licenças**.</span><span class="sxs-lookup"><span data-stu-id="6e003-161">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="6e003-162">Na página **Gerenciar licenças** , desmarque o Dynamics 365 for Sales / plano de envolvimento de cliente do Basic (oferecer qualificado) a caixa de seleção da licença e selecione um novo plano de serviço para a assinatura que o cliente está mudando.</span><span class="sxs-lookup"><span data-stu-id="6e003-162">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="6e003-163">Selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="6e003-163">Select **Submit**.</span></span> <span data-ttu-id="6e003-164">Você fará isso para cada usuário que precisa a nova licença.</span><span class="sxs-lookup"><span data-stu-id="6e003-164">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="6e003-165">Quando você tiver movido as licenças para a nova assinatura, você pode cancelar a assinatura antiga.</span><span class="sxs-lookup"><span data-stu-id="6e003-165">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="6e003-166">Selecione **os clientes** no painel de navegação esquerdo e, em seguida, selecione o cliente que você está movendo.</span><span class="sxs-lookup"><span data-stu-id="6e003-166">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="6e003-167">Na página de detalhes de assinatura, defina a assinatura antiga como **suspensa** e selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="6e003-167">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="6e003-168">A assinatura antiga agora é suspenso, e a nova assinatura está ativa.</span><span class="sxs-lookup"><span data-stu-id="6e003-168">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="6e003-169">A assinatura suspensa será desprovisionada automaticamente após 120 dias.</span><span class="sxs-lookup"><span data-stu-id="6e003-169">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="6e003-170">Seu cliente provocará sem custos adicionais para a assinatura antiga.</span><span class="sxs-lookup"><span data-stu-id="6e003-170">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



