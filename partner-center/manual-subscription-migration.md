---
title: Migrar assinaturas do Dynamics 365 qualificadas
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como migrar de assinaturas do Dynamics 365 básicas e qualificadas para uma nova assinatura antes que as assinaturas existentes expirem.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
Keywords: O Dynamics 365 oferece, renovar ofertas, novas SKUs do Dynamics 365
ms.openlocfilehash: 1fb7a58d3c777f39bdd3594d6d2bc0be04fbf573
ms.sourcegitcommit: e0a1b4506840486f4bb82620051e0f6a5e81662a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "84992103"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="443b4-104">Migrar o Dynamics 365 e o Customer Engagement Plan de Basic (ofertas qualificadas) para versões mais recentes</span><span class="sxs-lookup"><span data-stu-id="443b4-104">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="443b4-105">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="443b4-105">**Applies to**</span></span>

-  <span data-ttu-id="443b4-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="443b4-106">Partner Center</span></span>

<span data-ttu-id="443b4-107">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="443b4-107">**Appropriate roles**</span></span>
-   <span data-ttu-id="443b4-108">Administrador global</span><span class="sxs-lookup"><span data-stu-id="443b4-108">Global admin</span></span>
-   <span data-ttu-id="443b4-109">Administrador de usuários</span><span class="sxs-lookup"><span data-stu-id="443b4-109">User admin</span></span>
-   <span data-ttu-id="443b4-110">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="443b4-110">Admin agent</span></span>
-   <span data-ttu-id="443b4-111">Agente de vendas</span><span class="sxs-lookup"><span data-stu-id="443b4-111">Sales agent</span></span>

<span data-ttu-id="443b4-112">A partir de 1º de janeiro de 2019, os clientes com Dynamics 365 para o plano de vendas/envolvimento do cliente das assinaturas básicas (ofertas qualificadas) não podem mais renovar essas ofertas herdadas; as assinaturas existentes não serão renovadas automaticamente quando expirarem.</span><span class="sxs-lookup"><span data-stu-id="443b4-112">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="443b4-113">Na página de detalhes da assinatura, o status da assinatura será alterado para "expira em [data]" de "renovações automáticas em [data]".</span><span class="sxs-lookup"><span data-stu-id="443b4-113">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="443b4-114">Para garantir a continuidade dos clientes, você deve fazer a transição deles com assinaturas expirando para uma opção com suporte, listada abaixo.</span><span class="sxs-lookup"><span data-stu-id="443b4-114">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="443b4-115">É recomendável mover os clientes para novas assinaturas antes da data de término anual da assinatura para evitar qualquer interrupção de serviço para os clientes.</span><span class="sxs-lookup"><span data-stu-id="443b4-115">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="443b4-116">Se você usar a API (CREST ou o Partner Center), poderá encontrar assinaturas expirando, avaliando a data de término da assinatura junto com a propriedade renovação automática = falso.</span><span class="sxs-lookup"><span data-stu-id="443b4-116">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="443b4-117">As assinaturas em questão serão definidas para renovação automática = falso em 1º de janeiro de 2019.</span><span class="sxs-lookup"><span data-stu-id="443b4-117">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="443b4-118">Você pode mover os clientes para um novo plano a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="443b4-118">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="443b4-119">As ofertas do Dynamics 365 estão sendo desativadas</span><span class="sxs-lookup"><span data-stu-id="443b4-119">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="443b4-120">Dynamics 365 para sales Enterprise Edition CRMOL Basic (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="443b4-120">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="443b4-121">Dynamics 365 para sales Enterprise Edition CRMOL Basic (oferta qualificada) para docentes</span><span class="sxs-lookup"><span data-stu-id="443b4-121">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="443b4-122">Dynamics 365 para sales Enterprise Edition CRMOL Basic (oferta qualificada) para estudantes</span><span class="sxs-lookup"><span data-stu-id="443b4-122">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="443b4-123">Dynamics 365 para sales Enterprise Edition (preços do governo) CRMOL básico (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="443b4-123">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="443b4-124">Dynamics 365 para sales Enterprise Edition do SA para CRM básico (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="443b4-124">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="443b4-125">Dynamics 365 para sales Enterprise Edition do SA para CRM básico (oferta qualificada) para docentes</span><span class="sxs-lookup"><span data-stu-id="443b4-125">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="443b4-126">Dynamics 365 para sales Enterprise Edition do SA para CRM básico (oferta qualificada) para estudantes</span><span class="sxs-lookup"><span data-stu-id="443b4-126">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="443b4-127">Dynamics 365 para sales Enterprise Edition (preços do governo) do SA para CRM básico (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="443b4-127">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="443b4-128">Complemento do Dynamics 365 para sales Enterprise Edition para CRM básico (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="443b4-128">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="443b4-129">Dynamics 365 for Sales Enterprise Edition complemento para CRM básico (oferta qualificada) para docentes</span><span class="sxs-lookup"><span data-stu-id="443b4-129">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="443b4-130">Dynamics 365 for Sales Enterprise Edition complemento para CRM básico (oferta qualificada) para estudantes</span><span class="sxs-lookup"><span data-stu-id="443b4-130">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="443b4-131">Complemento do Dynamics 365 para sales Enterprise Edition (preços do governo) para CRM básico (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="443b4-131">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="443b4-132">Plano de envolvimento do cliente do Dynamics 365 Enterprise Edition CRMOL Basic (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="443b4-132">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="443b4-133">Plano de envolvimento do cliente do Dynamics 365 Enterprise Edition (preços do governo) CRMOL básico (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="443b4-133">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="443b4-134">Plano de envolvimento do cliente do Dynamics 365 Enterprise Edition CRMOL Basic (oferta qualificada) para estudantes</span><span class="sxs-lookup"><span data-stu-id="443b4-134">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="443b4-135">Plano de envolvimento do cliente do Dynamics 365 Enterprise Edition CRMOL Basic (oferta qualificada) para docentes</span><span class="sxs-lookup"><span data-stu-id="443b4-135">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="443b4-136">Plano de envolvimento do cliente do Dynamics 365 Enterprise Edition do SA para CRM básico (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="443b4-136">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="443b4-137">Plano de envolvimento do cliente do Dynamics 365 Enterprise Edition (preço governamental) do SA para CRM básico (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="443b4-137">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="443b4-138">Plano de envolvimento do cliente do Dynamics 365 Enterprise Edition do SA para CRM básico (oferta qualificada) para estudantes</span><span class="sxs-lookup"><span data-stu-id="443b4-138">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="443b4-139">Plano de envolvimento do cliente do Dynamics 365 Enterprise Edition do SA para CRM básico (oferta qualificada) para docentes</span><span class="sxs-lookup"><span data-stu-id="443b4-139">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="443b4-140">Dynamics 365 plano de envolvimento do cliente Enterprise Edition complemento para CRM básico (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="443b4-140">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="443b4-141">Plano de envolvimento do cliente do Dynamics 365 Enterprise Edition (preço do governo) complemento para CRM básico (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="443b4-141">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="443b4-142">Dynamics 365 plano de envolvimento do cliente Enterprise Edition complemento para CRM básico (oferta qualificada) para estudantes</span><span class="sxs-lookup"><span data-stu-id="443b4-142">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="443b4-143">Dynamics 365 plano de envolvimento do cliente Enterprise Edition complemento para CRM básico (oferta qualificada) para docentes</span><span class="sxs-lookup"><span data-stu-id="443b4-143">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="443b4-144">Dynamics 365 para vendas/plano de envolvimento com o cliente de planos de substituição básicos (ofertas qualificadas)</span><span class="sxs-lookup"><span data-stu-id="443b4-144">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="443b4-145">**Ofertas desativadas**</span><span class="sxs-lookup"><span data-stu-id="443b4-145">**Retired offers**</span></span>   

- <span data-ttu-id="443b4-146">Dynamics 365 para vendas do CRM Basic ou do CRMOL Basic (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="443b4-146">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="443b4-147">Plano de envolvimento do cliente do Dynamics 365 do CRM Basic ou do CRMOL Basic (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="443b4-147">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="443b4-148">**Opções de substituição**</span><span class="sxs-lookup"><span data-stu-id="443b4-148">**Replacement options**</span></span>
- <span data-ttu-id="443b4-149">Dynamics 365 for Sales Professional (novo)</span><span class="sxs-lookup"><span data-stu-id="443b4-149">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="443b4-150">Dynamics 365 for Sales Professional (novo)</span><span class="sxs-lookup"><span data-stu-id="443b4-150">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="443b4-151">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="443b4-151">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="443b4-152">Plano de envolvimento do cliente do Dynamics 365 ou</span><span class="sxs-lookup"><span data-stu-id="443b4-152">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="443b4-153">Membros da equipe do Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="443b4-153">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="443b4-154">Transição dos clientes para novos planos do produto</span><span class="sxs-lookup"><span data-stu-id="443b4-154">Transition customers to new product plans</span></span>

<span data-ttu-id="443b4-155">Mover clientes de SKUs desativados para os mais recentes requer as seguintes etapas nesta ordem:</span><span class="sxs-lookup"><span data-stu-id="443b4-155">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="443b4-156">Comprar a nova assinatura</span><span class="sxs-lookup"><span data-stu-id="443b4-156">Purchase the new subscription</span></span>
- <span data-ttu-id="443b4-157">Reatribuir as licenças de usuário atuais</span><span class="sxs-lookup"><span data-stu-id="443b4-157">Reassign current user licenses</span></span>
- <span data-ttu-id="443b4-158">Cancelar a assinatura antiga</span><span class="sxs-lookup"><span data-stu-id="443b4-158">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="443b4-159">Comprar o novo plano para o cliente</span><span class="sxs-lookup"><span data-stu-id="443b4-159">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="443b4-160">Selecione **clientes** na barra de navegação à esquerda e, em seguida, selecione o cliente que você deseja mover para a nova assinatura.</span><span class="sxs-lookup"><span data-stu-id="443b4-160">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="443b4-161">Selecione **Adicionar assinatura**.</span><span class="sxs-lookup"><span data-stu-id="443b4-161">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="443b4-162">Selecione a assinatura que deseja comprar no catálogo (nesse caso, uma das opções acima), insira o número de licenças e selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="443b4-162">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="443b4-163">Agora, seu cliente terá a assinatura antiga e a nova.</span><span class="sxs-lookup"><span data-stu-id="443b4-163">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="443b4-164">A próxima etapa é reatribuir licenças aos usuários do cliente.</span><span class="sxs-lookup"><span data-stu-id="443b4-164">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="443b4-165">Selecione **clientes** na barra de navegação à esquerda e, em seguida, selecione o cliente que você está movendo.</span><span class="sxs-lookup"><span data-stu-id="443b4-165">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="443b4-166">Selecione **usuários e licenças**.</span><span class="sxs-lookup"><span data-stu-id="443b4-166">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="443b4-167">Para reatribuir uma licença a um usuário, selecione o usuário e, em seguida, selecione **gerenciar licenças**.</span><span class="sxs-lookup"><span data-stu-id="443b4-167">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="443b4-168">Na página **gerenciar licenças** , desmarque a caixa de seleção Dynamics 365 para vendas/plano de envolvimento do cliente da licença básica (oferta qualificada) e selecione um novo plano de serviço para a assinatura à qual o cliente está se movendo.</span><span class="sxs-lookup"><span data-stu-id="443b4-168">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="443b4-169">Selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="443b4-169">Select **Submit**.</span></span> <span data-ttu-id="443b4-170">Você fará isso para cada usuário que precisa da nova licença.</span><span class="sxs-lookup"><span data-stu-id="443b4-170">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="443b4-171">Depois de mover as licenças para a nova assinatura, você poderá cancelar a assinatura antiga.</span><span class="sxs-lookup"><span data-stu-id="443b4-171">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="443b4-172">Selecione **clientes** na barra de navegação à esquerda e, em seguida, selecione o cliente que você está movendo.</span><span class="sxs-lookup"><span data-stu-id="443b4-172">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="443b4-173">Na página detalhes da assinatura, defina a assinatura antiga como **suspensa** e selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="443b4-173">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="443b4-174">A assinatura antiga agora está suspensa e a nova assinatura está ativa.</span><span class="sxs-lookup"><span data-stu-id="443b4-174">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="443b4-175">A assinatura suspensa será desprovisionada automaticamente após 120 dias.</span><span class="sxs-lookup"><span data-stu-id="443b4-175">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="443b4-176">Seu cliente não incorrerá em nenhum custo adicional para a assinatura antiga.</span><span class="sxs-lookup"><span data-stu-id="443b4-176">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



