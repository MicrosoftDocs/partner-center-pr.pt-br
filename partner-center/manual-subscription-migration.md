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
ms.openlocfilehash: 5ba6992eff64031aed0dafeb5a5010983396ab63
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151637"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="80e5b-103">Migrar o Dynamics 365 e o Customer Engagement Plan de Basic (ofertas qualificadas) para versões mais recentes</span><span class="sxs-lookup"><span data-stu-id="80e5b-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="80e5b-104">**Funções apropriadas**: Administração Global | Administrador de gerenciamento de usuários | Agente de administração | Agente de vendas</span><span class="sxs-lookup"><span data-stu-id="80e5b-104">**Appropriate roles**: Global admin | User management admin | Admin agent | Sales agent</span></span>

<span data-ttu-id="80e5b-105">A partir de 1º de janeiro de 2019, os clientes com Dynamics 365 para o plano de vendas/envolvimento do cliente das assinaturas básicas (ofertas qualificadas) não podem mais renovar essas ofertas herdadas; as assinaturas existentes não serão renovadas automaticamente quando expirarem.</span><span class="sxs-lookup"><span data-stu-id="80e5b-105">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="80e5b-106">Na página de detalhes da assinatura, o status da assinatura será alterado para "expira em [data]" de "renovações automáticas em [data]".</span><span class="sxs-lookup"><span data-stu-id="80e5b-106">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="80e5b-107">Para garantir a continuidade dos clientes, você deve fazer a transição deles com assinaturas expirando para uma opção com suporte, listada abaixo.</span><span class="sxs-lookup"><span data-stu-id="80e5b-107">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="80e5b-108">É recomendável mover os clientes para novas assinaturas antes da data de término anual da assinatura para evitar qualquer interrupção de serviço para os clientes.</span><span class="sxs-lookup"><span data-stu-id="80e5b-108">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="80e5b-109">Se você usar a API (CREST ou o Partner Center), poderá encontrar assinaturas expirando, avaliando a data de término da assinatura junto com a propriedade renovação automática = falso.</span><span class="sxs-lookup"><span data-stu-id="80e5b-109">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="80e5b-110">As assinaturas em questão serão definidas para renovação automática = falso em 1º de janeiro de 2019.</span><span class="sxs-lookup"><span data-stu-id="80e5b-110">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="80e5b-111">Você pode mover os clientes para um novo plano a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="80e5b-111">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="80e5b-112">As ofertas do Dynamics 365 estão sendo desativadas</span><span class="sxs-lookup"><span data-stu-id="80e5b-112">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="80e5b-113">Dynamics 365 para sales Enterprise Edition CRMOL Basic (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="80e5b-113">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="80e5b-114">Dynamics 365 para sales Enterprise Edition CRMOL Basic (oferta qualificada) para docentes</span><span class="sxs-lookup"><span data-stu-id="80e5b-114">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="80e5b-115">Dynamics 365 para sales Enterprise Edition CRMOL Basic (oferta qualificada) para estudantes</span><span class="sxs-lookup"><span data-stu-id="80e5b-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="80e5b-116">Dynamics 365 para sales Enterprise Edition (preços do governo) CRMOL básico (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="80e5b-116">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="80e5b-117">Dynamics 365 para sales Enterprise Edition do SA para CRM básico (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="80e5b-117">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="80e5b-118">Dynamics 365 para sales Enterprise Edition do SA para CRM básico (oferta qualificada) para docentes</span><span class="sxs-lookup"><span data-stu-id="80e5b-118">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="80e5b-119">Dynamics 365 para sales Enterprise Edition do SA para CRM básico (oferta qualificada) para estudantes</span><span class="sxs-lookup"><span data-stu-id="80e5b-119">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="80e5b-120">Dynamics 365 para sales Enterprise Edition (preços do governo) do SA para CRM básico (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="80e5b-120">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="80e5b-121">Dynamics 365 para sales Enterprise Edition Add-On para CRM Basic (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="80e5b-121">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="80e5b-122">Dynamics 365 for Sales Edição Enterprise Add-On for CRM Basic (Oferta Qualificada) para Docentes</span><span class="sxs-lookup"><span data-stu-id="80e5b-122">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="80e5b-123">Dynamics 365 for Sales Edição Enterprise Add-On for CRM Basic (Oferta Qualificada) para Alunos</span><span class="sxs-lookup"><span data-stu-id="80e5b-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="80e5b-124">Dynamics 365 for Sales Edição Enterprise (Preços governamentais) Add-On para CRM Basic (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="80e5b-124">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="80e5b-125">Plano de Participação do Cliente do Dynamics 365 Edição Enterprise CRMOL Basic (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="80e5b-125">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="80e5b-126">Plano de participação do cliente do Dynamics 365 Edição Enterprise (preços governamentais) CRMOL Basic (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="80e5b-126">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="80e5b-127">Plano de Participação do Cliente do Dynamics 365 Edição Enterprise CRMOL Basic (oferta qualificada) para alunos</span><span class="sxs-lookup"><span data-stu-id="80e5b-127">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="80e5b-128">Plano de Participação do Cliente do Dynamics 365 Edição Enterprise CRMOL Basic (oferta qualificada) para docentes</span><span class="sxs-lookup"><span data-stu-id="80e5b-128">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="80e5b-129">Plano de Participação do Cliente do Dynamics 365 Edição Enterprise do SA para CRM Basic (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="80e5b-129">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="80e5b-130">Plano de participação do cliente do Dynamics 365 Edição Enterprise (preços governamentais) do SA para CRM Basic (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="80e5b-130">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="80e5b-131">Plano de Participação do Cliente do Dynamics 365 Edição Enterprise do SA para CRM Basic (oferta qualificada) para alunos</span><span class="sxs-lookup"><span data-stu-id="80e5b-131">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="80e5b-132">Plano de Participação do Cliente do Dynamics 365 Edição Enterprise do SA para CRM Basic (oferta qualificada) para docentes</span><span class="sxs-lookup"><span data-stu-id="80e5b-132">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="80e5b-133">Plano de participação do cliente do Dynamics 365 Edição Enterprise Add-On para CRM Basic (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="80e5b-133">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="80e5b-134">Plano de participação do cliente do Dynamics 365 Edição Enterprise (preços governamentais) Add-On para CRM Basic (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="80e5b-134">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="80e5b-135">Plano de participação do cliente do Dynamics 365 Edição Enterprise Add-On para CRM Basic (oferta qualificada) para alunos</span><span class="sxs-lookup"><span data-stu-id="80e5b-135">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="80e5b-136">Plano de participação do cliente do Dynamics 365 Edição Enterprise Add-On para CRM Basic (oferta qualificada) para docentes</span><span class="sxs-lookup"><span data-stu-id="80e5b-136">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="80e5b-137">Dynamics 365 for Sales/Customer Engagement Plan from Basic (Qualified Offers) replacement plans (Qualified Offers)</span><span class="sxs-lookup"><span data-stu-id="80e5b-137">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="80e5b-138">**Ofertas retiradas**</span><span class="sxs-lookup"><span data-stu-id="80e5b-138">**Retired offers**</span></span>   

- <span data-ttu-id="80e5b-139">Dynamics 365 for Sales do CRM Basic ou CRMOL Basic (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="80e5b-139">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="80e5b-140">Plano de Participação do Cliente do Dynamics 365 do CRM Basic ou CRMOL Basic (oferta qualificada)</span><span class="sxs-lookup"><span data-stu-id="80e5b-140">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="80e5b-141">**Opções de substituição**</span><span class="sxs-lookup"><span data-stu-id="80e5b-141">**Replacement options**</span></span>
- <span data-ttu-id="80e5b-142">Dynamics 365 for Sales Professional (NOVO)</span><span class="sxs-lookup"><span data-stu-id="80e5b-142">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="80e5b-143">Dynamics 365 for Sales Professional (NOVO)</span><span class="sxs-lookup"><span data-stu-id="80e5b-143">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="80e5b-144">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="80e5b-144">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="80e5b-145">Plano de Participação do Cliente do Dynamics 365 ou</span><span class="sxs-lookup"><span data-stu-id="80e5b-145">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="80e5b-146">Membros da equipe do Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="80e5b-146">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="80e5b-147">Transição dos clientes para novos planos do produto</span><span class="sxs-lookup"><span data-stu-id="80e5b-147">Transition customers to new product plans</span></span>

<span data-ttu-id="80e5b-148">Mover os clientes de SKUs antigos para os mais novos requer as seguintes etapas nesta ordem:</span><span class="sxs-lookup"><span data-stu-id="80e5b-148">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="80e5b-149">Comprar a nova assinatura</span><span class="sxs-lookup"><span data-stu-id="80e5b-149">Purchase the new subscription</span></span>
- <span data-ttu-id="80e5b-150">Reatribuir as licenças de usuário atuais</span><span class="sxs-lookup"><span data-stu-id="80e5b-150">Reassign current user licenses</span></span>
- <span data-ttu-id="80e5b-151">Cancelar a assinatura antiga</span><span class="sxs-lookup"><span data-stu-id="80e5b-151">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="80e5b-152">Comprar o novo plano para seu cliente</span><span class="sxs-lookup"><span data-stu-id="80e5b-152">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="80e5b-153">Selecione **Clientes** no nav à esquerda e, em seguida, selecione o cliente que você deseja mover para a nova assinatura.</span><span class="sxs-lookup"><span data-stu-id="80e5b-153">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="80e5b-154">Selecione **Adicionar Assinatura**.</span><span class="sxs-lookup"><span data-stu-id="80e5b-154">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="80e5b-155">Selecione a assinatura que deseja comprar no catálogo (nesse caso, uma das opções acima), insira o número de licenças e selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="80e5b-155">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="80e5b-156">Seu cliente agora terá a assinatura antiga e a nova.</span><span class="sxs-lookup"><span data-stu-id="80e5b-156">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="80e5b-157">A próxima etapa é reatribuir licenças aos usuários do cliente.</span><span class="sxs-lookup"><span data-stu-id="80e5b-157">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="80e5b-158">Selecione **Clientes** no nav à esquerda e, em seguida, selecione o cliente que você está movendo.</span><span class="sxs-lookup"><span data-stu-id="80e5b-158">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="80e5b-159">Selecione **Usuários e licenças**.</span><span class="sxs-lookup"><span data-stu-id="80e5b-159">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="80e5b-160">Para reatribuir uma licença a um usuário, selecione o usuário e, em seguida, **selecione Gerenciar licenças**.</span><span class="sxs-lookup"><span data-stu-id="80e5b-160">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="80e5b-161">Na página Gerenciar **licenças, des** marque a caixa de seleção Dynamics 365 for Sales/Customer Engagement Plan da licença Básica (Oferta Qualificada) e selecione um novo plano de serviço para a assinatura para a qual o cliente está mudando.</span><span class="sxs-lookup"><span data-stu-id="80e5b-161">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="80e5b-162">Selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="80e5b-162">Select **Submit**.</span></span> <span data-ttu-id="80e5b-163">Você fará isso para cada usuário que precisa da nova licença.</span><span class="sxs-lookup"><span data-stu-id="80e5b-163">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="80e5b-164">Depois de ter movido as licenças para a nova assinatura, você pode cancelar a assinatura antiga.</span><span class="sxs-lookup"><span data-stu-id="80e5b-164">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="80e5b-165">Selecione **Clientes** no nav à esquerda e, em seguida, selecione o cliente que você está movendo.</span><span class="sxs-lookup"><span data-stu-id="80e5b-165">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="80e5b-166">Na página de detalhes da assinatura, de definir a assinatura antiga como **Suspensa** e selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="80e5b-166">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="80e5b-167">A assinatura antiga agora está suspensa e a nova assinatura está ativa.</span><span class="sxs-lookup"><span data-stu-id="80e5b-167">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="80e5b-168">A assinatura suspensa será desprovisionada automaticamente após 120 dias.</span><span class="sxs-lookup"><span data-stu-id="80e5b-168">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="80e5b-169">Seu cliente não incorre em custos adicionais para a assinatura antiga.</span><span class="sxs-lookup"><span data-stu-id="80e5b-169">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



