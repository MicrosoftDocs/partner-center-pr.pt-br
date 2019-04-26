---
title: Migrar do Dynamics 365 e o plano de envolvimento do cliente do Basic (ofertas qualificadas) para versões mais recentes | Partner Center
ms.topic: article
ms.date: 12/12/2018
description: Dynamics 365 para vendas / Customer Engagement planejar de assinaturas do Basic (oferece qualificado) não pode ser renovado.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 oferece, renovar ofertas, novas SKUs do Dynamics 365
ms.openlocfilehash: e5128abe71cfab4e2cdabb0cafcd5fd7df56b116
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2019
ms.locfileid: "62134396"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="731dd-104">Migrar o Dynamics 365 e o Customer Engagement Plan de Basic (ofertas qualificadas) para versões mais recentes</span><span class="sxs-lookup"><span data-stu-id="731dd-104">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="731dd-105">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="731dd-105">**Applies to**</span></span>

-  <span data-ttu-id="731dd-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="731dd-106">Partner Center</span></span>

<span data-ttu-id="731dd-107">Clientes de 1 de janeiro de 2019 efetivos com o Dynamics 365 para vendas / Customer Engagement planejar de assinaturas do Basic (oferece qualificado) não pode renovar essas ofertas herdadas; as assinaturas existentes não serão renovadas automaticamente quando eles expiram.</span><span class="sxs-lookup"><span data-stu-id="731dd-107">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="731dd-108">Na página de detalhes da assinatura, o status da assinatura será alterado para "Expira em [Data]" de "Automático renova em [Data]".</span><span class="sxs-lookup"><span data-stu-id="731dd-108">On the subscription’s detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 


<span data-ttu-id="731dd-109">Para garantir a continuidade para os clientes, você deve fazer a transição aquelas com assinatura prestes a expirar para uma opção com suporte, listados abaixo.</span><span class="sxs-lookup"><span data-stu-id="731dd-109">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="731dd-110">É recomendável mover os clientes para as novas assinaturas antes da data de término da assinatura anual, para evitar possíveis interrupções de serviço.</span><span class="sxs-lookup"><span data-stu-id="731dd-110">We recommend moving customers to new subscriptions before the subscription’s yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="731dd-111">Se você usar a API (CREST ou Partner Center), você pode encontrar a renovação de assinaturas prestes a expirar, avaliando a data de término da assinatura, juntamente com o auto = False propriedade.</span><span class="sxs-lookup"><span data-stu-id="731dd-111">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="731dd-112">As assinaturas em questão serão definidas como auto renovar = False em 1 de janeiro de 2019.</span><span class="sxs-lookup"><span data-stu-id="731dd-112">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="731dd-113">Você pode mover os clientes para um novo plano a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="731dd-113">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="731dd-114">O Dynamics 365 oferece o que está sendo desativado</span><span class="sxs-lookup"><span data-stu-id="731dd-114">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="731dd-115">Dynamics 365 for Sales, Enterprise Edition CRMOL Basic (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="731dd-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="731dd-116">Dynamics 365 for Sales, Enterprise Edition CRMOL Basic (oferta qualificada) para docentes</span><span class="sxs-lookup"><span data-stu-id="731dd-116">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="731dd-117">Dynamics 365 for Sales, Enterprise Edition CRMOL Basic (oferta qualificada) para alunos</span><span class="sxs-lookup"><span data-stu-id="731dd-117">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="731dd-118">Dynamics 365 for Sales, Enterprise Edition (preços governamentais) CRMOL Basic (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="731dd-118">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="731dd-119">Dynamics 365 for Sales, Enterprise Edition do SA para CRM Basic (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="731dd-119">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="731dd-120">Dynamics 365 for Sales, Enterprise Edition do SA para CRM Basic (oferta qualificada) para docentes</span><span class="sxs-lookup"><span data-stu-id="731dd-120">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="731dd-121">Dynamics 365 for Sales, Enterprise Edition do SA para CRM Basic (oferta qualificada) para alunos</span><span class="sxs-lookup"><span data-stu-id="731dd-121">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="731dd-122">Dynamics 365 para Sales, Enterprise Edition (preços governamentais) do SA para CRM Basic (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="731dd-122">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="731dd-123">Dynamics 365 para Sales, Enterprise Edition complemento para o Basic CRM (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="731dd-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="731dd-124">Dynamics 365 para Sales, Enterprise Edition complemento para o Basic CRM (oferta qualificada) para docentes</span><span class="sxs-lookup"><span data-stu-id="731dd-124">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="731dd-125">Dynamics 365 para Sales, Enterprise Edition complemento para o Basic CRM (oferta qualificada) para alunos</span><span class="sxs-lookup"><span data-stu-id="731dd-125">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="731dd-126">Dynamics 365 para Sales, Enterprise Edition (preços governamentais) complemento para o Basic CRM (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="731dd-126">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="731dd-127">Dynamics 365 Customer Engagement plano Enterprise Edition CRMOL básico (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="731dd-127">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="731dd-128">Dynamics 365 Customer Engagement plano Enterprise Edition (preços governamentais) CRMOL básico (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="731dd-128">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="731dd-129">Dynamics 365 Customer Engagement plano Enterprise Edition CRMOL básico (oferta qualificado) para alunos</span><span class="sxs-lookup"><span data-stu-id="731dd-129">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="731dd-130">Dynamics 365 Customer Engagement plano Enterprise Edition CRMOL básico (oferta qualificado) para docentes</span><span class="sxs-lookup"><span data-stu-id="731dd-130">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="731dd-131">Dynamics 365 Customer Engagement plano Enterprise Edition do SA para CRM Basic (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="731dd-131">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="731dd-132">Dynamics 365 Customer Engagement plano Enterprise Edition (preços governamentais) do SA para CRM Basic (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="731dd-132">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="731dd-133">Dynamics 365 Customer Engagement plano Enterprise Edition do SA para CRM Basic (oferta qualificada) para alunos</span><span class="sxs-lookup"><span data-stu-id="731dd-133">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="731dd-134">Dynamics 365 Customer Engagement plano Enterprise Edition do SA para CRM Basic (oferta qualificada) para docentes</span><span class="sxs-lookup"><span data-stu-id="731dd-134">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="731dd-135">Dynamics 365 Customer Engagement plano Enterprise Edition complemento para o Basic CRM (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="731dd-135">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="731dd-136">Dynamics 365 Customer Engagement plano Enterprise Edition (preços governamentais) complemento para o Basic CRM (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="731dd-136">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="731dd-137">Dynamics 365 Customer Engagement plano Enterprise Edition complemento para o Basic CRM (oferta qualificada) para alunos</span><span class="sxs-lookup"><span data-stu-id="731dd-137">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="731dd-138">Dynamics 365 Customer Engagement plano Enterprise Edition complemento para o Basic CRM (oferta qualificada) para docentes</span><span class="sxs-lookup"><span data-stu-id="731dd-138">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="731dd-139">Dynamics 365 para vendas / planos de Customer Engagement planejar de substituição de básico (oferece qualificado)</span><span class="sxs-lookup"><span data-stu-id="731dd-139">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="731dd-140">**Ofertas descontinuadas**</span><span class="sxs-lookup"><span data-stu-id="731dd-140">**Retired offers**</span></span>   

- <span data-ttu-id="731dd-141">Dynamics 365 para vendas do CRM Basic ou CRMOL Basic (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="731dd-141">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="731dd-142">Plano de envolvimento do cliente do Dynamics 365 do CRM Basic ou CRMOL Basic (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="731dd-142">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="731dd-143">**Opções de substituição**</span><span class="sxs-lookup"><span data-stu-id="731dd-143">**Replacement options**</span></span>
- <span data-ttu-id="731dd-144">Dynamics 365 para profissionais de vendas (novo)</span><span class="sxs-lookup"><span data-stu-id="731dd-144">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="731dd-145">Dynamics 365 para profissionais de vendas (novo)</span><span class="sxs-lookup"><span data-stu-id="731dd-145">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="731dd-146">Dynamics 365 para atendimento ao cliente</span><span class="sxs-lookup"><span data-stu-id="731dd-146">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="731dd-147">Plano do Dynamics 365 Customer Engagement ou</span><span class="sxs-lookup"><span data-stu-id="731dd-147">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="731dd-148">Membros da equipe do Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="731dd-148">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="731dd-149">Transição dos clientes para novos planos do produto</span><span class="sxs-lookup"><span data-stu-id="731dd-149">Transition customers to new product plans</span></span>

<span data-ttu-id="731dd-150">Mover os clientes de SKUs desativados para as mais novas exige as seguintes etapas nesta ordem:</span><span class="sxs-lookup"><span data-stu-id="731dd-150">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="731dd-151">Comprar a nova assinatura</span><span class="sxs-lookup"><span data-stu-id="731dd-151">Purchase the new subscription</span></span>
- <span data-ttu-id="731dd-152">Reatribuir as licenças de usuário atuais</span><span class="sxs-lookup"><span data-stu-id="731dd-152">Reassign current user licenses</span></span>
- <span data-ttu-id="731dd-153">Cancelar a assinatura antiga</span><span class="sxs-lookup"><span data-stu-id="731dd-153">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="731dd-154">O novo plano de compra para seu cliente</span><span class="sxs-lookup"><span data-stu-id="731dd-154">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="731dd-155">Selecione **clientes** da navegação à esquerda e em seguida, selecione o cliente que você deseja mover para a nova assinatura.</span><span class="sxs-lookup"><span data-stu-id="731dd-155">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="731dd-156">Selecione **Adicionar assinatura**.</span><span class="sxs-lookup"><span data-stu-id="731dd-156">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="731dd-157">Selecione a assinatura que deseja comprar no catálogo (nesse caso, uma das opções acima), insira o número de licenças e selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="731dd-157">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="731dd-158">Agora, o cliente terá a assinatura antiga e nova.</span><span class="sxs-lookup"><span data-stu-id="731dd-158">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="731dd-159">A próxima etapa é reatribuir licenças aos usuários do cliente.</span><span class="sxs-lookup"><span data-stu-id="731dd-159">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="731dd-160">Selecione **clientes** da barra de navegação à esquerda e selecione o cliente estiver movendo.</span><span class="sxs-lookup"><span data-stu-id="731dd-160">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="731dd-161">Selecione **Usuários e licenças**.</span><span class="sxs-lookup"><span data-stu-id="731dd-161">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="731dd-162">Para reatribuir uma licença a um usuário, selecione o usuário e, em seguida, selecione **gerenciar licenças**.</span><span class="sxs-lookup"><span data-stu-id="731dd-162">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="731dd-163">Sobre o **gerenciar licenças** página, desmarque o Dynamics 365 para vendas / plano de envolvimento do cliente do Basic (oferecer qualificado) caixa de seleção de licença e selecione um novo plano de serviço para a assinatura que o cliente está se movendo para.</span><span class="sxs-lookup"><span data-stu-id="731dd-163">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="731dd-164">Selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="731dd-164">Select **Submit**.</span></span> <span data-ttu-id="731dd-165">Você fará isso para cada usuário que precisa da nova licença.</span><span class="sxs-lookup"><span data-stu-id="731dd-165">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="731dd-166">Depois de mover as licenças ao longo para a nova assinatura, você pode cancelar a assinatura antiga.</span><span class="sxs-lookup"><span data-stu-id="731dd-166">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="731dd-167">Selecione **clientes** da barra de navegação à esquerda e selecione o cliente estiver movendo.</span><span class="sxs-lookup"><span data-stu-id="731dd-167">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="731dd-168">Na página de detalhes da assinatura, defina a assinatura antiga **Suspended** e selecione **enviar**.</span><span class="sxs-lookup"><span data-stu-id="731dd-168">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="731dd-169">A assinatura antiga agora está suspenso e a nova assinatura está ativa.</span><span class="sxs-lookup"><span data-stu-id="731dd-169">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="731dd-170">A assinatura suspensa será desprovisionada automaticamente após 120 dias.</span><span class="sxs-lookup"><span data-stu-id="731dd-170">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="731dd-171">Seu cliente não incorrerá em nenhum custo adicional para a assinatura antiga.</span><span class="sxs-lookup"><span data-stu-id="731dd-171">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



