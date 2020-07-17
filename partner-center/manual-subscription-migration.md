---
title: Migrar assinaturas do Dynamics 365 qualificadas
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como migrar de assinaturas do Dynamics 365 básicas e qualificadas para uma nova assinatura antes que as assinaturas existentes expirem.
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8575d87ab3c4c7970135a87b7ef7564c4fe06232
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2020
ms.locfileid: "86436845"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="96e80-103">Migrar o Dynamics 365 e o Customer Engagement Plan de Basic (ofertas qualificadas) para versões mais recentes</span><span class="sxs-lookup"><span data-stu-id="96e80-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="96e80-104">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="96e80-104">**Applies to**</span></span>

-  <span data-ttu-id="96e80-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="96e80-105">Partner Center</span></span>

<span data-ttu-id="96e80-106">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="96e80-106">**Appropriate roles**</span></span>
-   <span data-ttu-id="96e80-107">Administrador global</span><span class="sxs-lookup"><span data-stu-id="96e80-107">Global admin</span></span>
-   <span data-ttu-id="96e80-108">Administrador de usuários</span><span class="sxs-lookup"><span data-stu-id="96e80-108">User admin</span></span>
-   <span data-ttu-id="96e80-109">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="96e80-109">Admin agent</span></span>
-   <span data-ttu-id="96e80-110">Agente de vendas</span><span class="sxs-lookup"><span data-stu-id="96e80-110">Sales agent</span></span>

<span data-ttu-id="96e80-111">A partir de 1º de janeiro de 2019, os clientes com Dynamics 365 para o plano de vendas/envolvimento do cliente das assinaturas básicas (ofertas qualificadas) não podem mais renovar essas ofertas herdadas; as assinaturas existentes não serão renovadas automaticamente quando expirarem.</span><span class="sxs-lookup"><span data-stu-id="96e80-111">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="96e80-112">Na página de detalhes da assinatura, o status da assinatura será alterado para "expira em [data]" de "renovações automáticas em [data]".</span><span class="sxs-lookup"><span data-stu-id="96e80-112">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="96e80-113">Para garantir a continuidade dos clientes, você deve fazer a transição deles com assinaturas expirando para uma opção com suporte, listada abaixo.</span><span class="sxs-lookup"><span data-stu-id="96e80-113">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="96e80-114">É recomendável mover os clientes para novas assinaturas antes da data de término anual da assinatura para evitar qualquer interrupção de serviço para os clientes.</span><span class="sxs-lookup"><span data-stu-id="96e80-114">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="96e80-115">Se você usar a API (CREST ou o Partner Center), poderá encontrar assinaturas expirando, avaliando a data de término da assinatura junto com a propriedade renovação automática = falso.</span><span class="sxs-lookup"><span data-stu-id="96e80-115">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="96e80-116">As assinaturas em questão serão definidas para renovação automática = falso em 1º de janeiro de 2019.</span><span class="sxs-lookup"><span data-stu-id="96e80-116">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="96e80-117">Você pode mover os clientes para um novo plano a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="96e80-117">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="96e80-118">As ofertas do Dynamics 365 estão sendo desativadas</span><span class="sxs-lookup"><span data-stu-id="96e80-118">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="96e80-119">Dynamics 365 para sales Enterprise Edition CRMOL Basic (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="96e80-119">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="96e80-120">Dynamics 365 para sales Enterprise Edition CRMOL Basic (oferta qualificada) para docentes</span><span class="sxs-lookup"><span data-stu-id="96e80-120">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="96e80-121">Dynamics 365 para sales Enterprise Edition CRMOL Basic (oferta qualificada) para estudantes</span><span class="sxs-lookup"><span data-stu-id="96e80-121">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="96e80-122">Dynamics 365 para sales Enterprise Edition (preços do governo) CRMOL básico (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="96e80-122">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="96e80-123">Dynamics 365 para sales Enterprise Edition do SA para CRM básico (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="96e80-123">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="96e80-124">Dynamics 365 para sales Enterprise Edition do SA para CRM básico (oferta qualificada) para docentes</span><span class="sxs-lookup"><span data-stu-id="96e80-124">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="96e80-125">Dynamics 365 para sales Enterprise Edition do SA para CRM básico (oferta qualificada) para estudantes</span><span class="sxs-lookup"><span data-stu-id="96e80-125">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="96e80-126">Dynamics 365 para sales Enterprise Edition (preços do governo) do SA para CRM básico (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="96e80-126">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="96e80-127">Complemento do Dynamics 365 para sales Enterprise Edition para CRM básico (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="96e80-127">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="96e80-128">Dynamics 365 for Sales Enterprise Edition complemento para CRM básico (oferta qualificada) para docentes</span><span class="sxs-lookup"><span data-stu-id="96e80-128">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="96e80-129">Dynamics 365 for Sales Enterprise Edition complemento para CRM básico (oferta qualificada) para estudantes</span><span class="sxs-lookup"><span data-stu-id="96e80-129">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="96e80-130">Complemento do Dynamics 365 para sales Enterprise Edition (preços do governo) para CRM básico (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="96e80-130">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="96e80-131">Plano de envolvimento do cliente do Dynamics 365 Enterprise Edition CRMOL Basic (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="96e80-131">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="96e80-132">Plano de envolvimento do cliente do Dynamics 365 Enterprise Edition (preços do governo) CRMOL básico (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="96e80-132">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="96e80-133">Plano de envolvimento do cliente do Dynamics 365 Enterprise Edition CRMOL Basic (oferta qualificada) para estudantes</span><span class="sxs-lookup"><span data-stu-id="96e80-133">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="96e80-134">Plano de envolvimento do cliente do Dynamics 365 Enterprise Edition CRMOL Basic (oferta qualificada) para docentes</span><span class="sxs-lookup"><span data-stu-id="96e80-134">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="96e80-135">Plano de envolvimento do cliente do Dynamics 365 Enterprise Edition do SA para CRM básico (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="96e80-135">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="96e80-136">Plano de envolvimento do cliente do Dynamics 365 Enterprise Edition (preço governamental) do SA para CRM básico (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="96e80-136">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="96e80-137">Plano de envolvimento do cliente do Dynamics 365 Enterprise Edition do SA para CRM básico (oferta qualificada) para estudantes</span><span class="sxs-lookup"><span data-stu-id="96e80-137">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="96e80-138">Plano de envolvimento do cliente do Dynamics 365 Enterprise Edition do SA para CRM básico (oferta qualificada) para docentes</span><span class="sxs-lookup"><span data-stu-id="96e80-138">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="96e80-139">Dynamics 365 plano de envolvimento do cliente Enterprise Edition complemento para CRM básico (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="96e80-139">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="96e80-140">Plano de envolvimento do cliente do Dynamics 365 Enterprise Edition (preço do governo) complemento para CRM básico (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="96e80-140">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="96e80-141">Dynamics 365 plano de envolvimento do cliente Enterprise Edition complemento para CRM básico (oferta qualificada) para estudantes</span><span class="sxs-lookup"><span data-stu-id="96e80-141">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="96e80-142">Dynamics 365 plano de envolvimento do cliente Enterprise Edition complemento para CRM básico (oferta qualificada) para docentes</span><span class="sxs-lookup"><span data-stu-id="96e80-142">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="96e80-143">Dynamics 365 para vendas/plano de envolvimento com o cliente de planos de substituição básicos (ofertas qualificadas)</span><span class="sxs-lookup"><span data-stu-id="96e80-143">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="96e80-144">**Ofertas desativadas**</span><span class="sxs-lookup"><span data-stu-id="96e80-144">**Retired offers**</span></span>   

- <span data-ttu-id="96e80-145">Dynamics 365 para vendas do CRM Basic ou do CRMOL Basic (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="96e80-145">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="96e80-146">Plano de envolvimento do cliente do Dynamics 365 do CRM Basic ou do CRMOL Basic (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="96e80-146">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="96e80-147">**Opções de substituição**</span><span class="sxs-lookup"><span data-stu-id="96e80-147">**Replacement options**</span></span>
- <span data-ttu-id="96e80-148">Dynamics 365 for Sales Professional (novo)</span><span class="sxs-lookup"><span data-stu-id="96e80-148">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="96e80-149">Dynamics 365 for Sales Professional (novo)</span><span class="sxs-lookup"><span data-stu-id="96e80-149">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="96e80-150">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="96e80-150">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="96e80-151">Plano de envolvimento do cliente do Dynamics 365 ou</span><span class="sxs-lookup"><span data-stu-id="96e80-151">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="96e80-152">Membros da equipe do Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="96e80-152">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="96e80-153">Transição dos clientes para novos planos do produto</span><span class="sxs-lookup"><span data-stu-id="96e80-153">Transition customers to new product plans</span></span>

<span data-ttu-id="96e80-154">Mover clientes de SKUs desativados para os mais recentes requer as seguintes etapas nesta ordem:</span><span class="sxs-lookup"><span data-stu-id="96e80-154">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="96e80-155">Comprar a nova assinatura</span><span class="sxs-lookup"><span data-stu-id="96e80-155">Purchase the new subscription</span></span>
- <span data-ttu-id="96e80-156">Reatribuir as licenças de usuário atuais</span><span class="sxs-lookup"><span data-stu-id="96e80-156">Reassign current user licenses</span></span>
- <span data-ttu-id="96e80-157">Cancelar a assinatura antiga</span><span class="sxs-lookup"><span data-stu-id="96e80-157">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="96e80-158">Comprar o novo plano para o cliente</span><span class="sxs-lookup"><span data-stu-id="96e80-158">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="96e80-159">Selecione **clientes** na barra de navegação à esquerda e, em seguida, selecione o cliente que você deseja mover para a nova assinatura.</span><span class="sxs-lookup"><span data-stu-id="96e80-159">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="96e80-160">Selecione **Adicionar assinatura**.</span><span class="sxs-lookup"><span data-stu-id="96e80-160">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="96e80-161">Selecione a assinatura que deseja comprar no catálogo (nesse caso, uma das opções acima), insira o número de licenças e selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="96e80-161">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="96e80-162">Agora, seu cliente terá a assinatura antiga e a nova.</span><span class="sxs-lookup"><span data-stu-id="96e80-162">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="96e80-163">A próxima etapa é reatribuir licenças aos usuários do cliente.</span><span class="sxs-lookup"><span data-stu-id="96e80-163">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="96e80-164">Selecione **clientes** na barra de navegação à esquerda e, em seguida, selecione o cliente que você está movendo.</span><span class="sxs-lookup"><span data-stu-id="96e80-164">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="96e80-165">Selecione **usuários e licenças**.</span><span class="sxs-lookup"><span data-stu-id="96e80-165">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="96e80-166">Para reatribuir uma licença a um usuário, selecione o usuário e, em seguida, selecione **gerenciar licenças**.</span><span class="sxs-lookup"><span data-stu-id="96e80-166">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="96e80-167">Na página **gerenciar licenças** , desmarque a caixa de seleção Dynamics 365 para vendas/plano de envolvimento do cliente da licença básica (oferta qualificada) e selecione um novo plano de serviço para a assinatura à qual o cliente está se movendo.</span><span class="sxs-lookup"><span data-stu-id="96e80-167">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="96e80-168">Selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="96e80-168">Select **Submit**.</span></span> <span data-ttu-id="96e80-169">Você fará isso para cada usuário que precisa da nova licença.</span><span class="sxs-lookup"><span data-stu-id="96e80-169">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="96e80-170">Depois de mover as licenças para a nova assinatura, você poderá cancelar a assinatura antiga.</span><span class="sxs-lookup"><span data-stu-id="96e80-170">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="96e80-171">Selecione **clientes** na barra de navegação à esquerda e, em seguida, selecione o cliente que você está movendo.</span><span class="sxs-lookup"><span data-stu-id="96e80-171">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="96e80-172">Na página detalhes da assinatura, defina a assinatura antiga como **suspensa** e selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="96e80-172">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="96e80-173">A assinatura antiga agora está suspensa e a nova assinatura está ativa.</span><span class="sxs-lookup"><span data-stu-id="96e80-173">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="96e80-174">A assinatura suspensa será desprovisionada automaticamente após 120 dias.</span><span class="sxs-lookup"><span data-stu-id="96e80-174">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="96e80-175">Seu cliente não incorrerá em nenhum custo adicional para a assinatura antiga.</span><span class="sxs-lookup"><span data-stu-id="96e80-175">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



