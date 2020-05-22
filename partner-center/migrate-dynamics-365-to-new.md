---
title: Migrar o Dynamics 365 Business Edition
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como migrar ofertas do Dynamics 365 Business Edition qualificadas para versões mais recentes antes que elas expirem.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
Keywords: O Dynamics 365 oferece, renovar ofertas, novas SKUs do Dynamics 365
ms.openlocfilehash: d49966db4a2c9de50b0723abf9ccd0fe589a442a
ms.sourcegitcommit: 2a980b50cf177753c15ebfd7770e14cf6d486cf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2020
ms.locfileid: "83795975"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="34f09-104">Migrar as ofertas do Dynamics 365 Business Edition para versões mais recentes</span><span class="sxs-lookup"><span data-stu-id="34f09-104">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span>

<span data-ttu-id="34f09-105">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="34f09-105">**Applies to**</span></span>

- <span data-ttu-id="34f09-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="34f09-106">Partner Center</span></span>

<span data-ttu-id="34f09-107">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="34f09-107">**Appropriate roles**</span></span>
- <span data-ttu-id="34f09-108">Administrador global</span><span class="sxs-lookup"><span data-stu-id="34f09-108">Global admin</span></span>
- <span data-ttu-id="34f09-109">Administrador de usuários</span><span class="sxs-lookup"><span data-stu-id="34f09-109">User admin</span></span>
- <span data-ttu-id="34f09-110">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="34f09-110">Admin agent</span></span>
- <span data-ttu-id="34f09-111">Agente de vendas</span><span class="sxs-lookup"><span data-stu-id="34f09-111">Sales agent</span></span>

<span data-ttu-id="34f09-112">A partir de 1º de janeiro de 2019, os clientes com as assinaturas do Dynamics 365 Business Edition não podem mais renovar essas ofertas herdadas; as assinaturas existentes não serão renovadas automaticamente quando expirarem.</span><span class="sxs-lookup"><span data-stu-id="34f09-112">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="34f09-113">Na página de detalhes da assinatura, o status da assinatura será alterado para "expira em [data]" de "renovações automáticas em [data]".</span><span class="sxs-lookup"><span data-stu-id="34f09-113">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="34f09-114">Para garantir a continuidade dos clientes, você deve fazer a transição deles com assinaturas expirando para uma opção com suporte, listada abaixo.</span><span class="sxs-lookup"><span data-stu-id="34f09-114">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="34f09-115">É recomendável mover os clientes para novas assinaturas antes da data de término anual da assinatura para evitar qualquer interrupção de serviço para os clientes.</span><span class="sxs-lookup"><span data-stu-id="34f09-115">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="34f09-116">Se você usar a API (CREST ou o Partner Center), poderá encontrar assinaturas expirando, avaliando a data de término da assinatura junto com a propriedade renovação automática = falso.</span><span class="sxs-lookup"><span data-stu-id="34f09-116">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="34f09-117">As assinaturas em questão serão definidas para renovação automática = falso em 1º de janeiro de 2019.</span><span class="sxs-lookup"><span data-stu-id="34f09-117">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="34f09-118">Você pode mover os clientes para um novo plano a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="34f09-118">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="34f09-119">As edições Business do Dynamics 365 estão sendo desativadas</span><span class="sxs-lookup"><span data-stu-id="34f09-119">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="34f09-120">Dynamics 365 for Finance and Operations, Business Edition</span><span class="sxs-lookup"><span data-stu-id="34f09-120">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="34f09-121">Dynamics 365 para Team Members, Business Edition</span><span class="sxs-lookup"><span data-stu-id="34f09-121">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="34f09-122">Dynamics Business Central-as novas ofertas do Dynamics 365 Business Edition</span><span class="sxs-lookup"><span data-stu-id="34f09-122">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="34f09-123">Com as novas ofertas do Dynamics Business central, seus clientes podem conectar suas finanças, vendas, serviços e operações para simplificar os processos de negócios, melhorar as interações com o cliente e tomar decisões melhores.</span><span class="sxs-lookup"><span data-stu-id="34f09-123">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="34f09-124">O Dynamics 365 Business central é baseado em nuvem e está disponível somente por meio de parceiros do programa CSP (provedor de soluções na nuvem).</span><span class="sxs-lookup"><span data-stu-id="34f09-124">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="34f09-125">Os clientes do Dynamics 365 Business Edition estão qualificados a receber preços de transição com desconto para as novas ofertas do Business central até 30 de junho de 2020.</span><span class="sxs-lookup"><span data-stu-id="34f09-125">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="34f09-126">Transição dos clientes para novos planos do produto</span><span class="sxs-lookup"><span data-stu-id="34f09-126">Transition customers to new product plans</span></span>

 <span data-ttu-id="34f09-127">Mover clientes de SKUs desativados para os mais recentes requer as seguintes etapas nesta ordem:</span><span class="sxs-lookup"><span data-stu-id="34f09-127">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="34f09-128">Comprar a nova assinatura</span><span class="sxs-lookup"><span data-stu-id="34f09-128">Purchase the new subscription</span></span>
- <span data-ttu-id="34f09-129">Reatribuir as licenças de usuário atuais</span><span class="sxs-lookup"><span data-stu-id="34f09-129">Reassign current user licenses</span></span>
- <span data-ttu-id="34f09-130">Cancelar a assinatura antiga</span><span class="sxs-lookup"><span data-stu-id="34f09-130">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="34f09-131">Comprar o novo plano para o cliente</span><span class="sxs-lookup"><span data-stu-id="34f09-131">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="34f09-132">Selecione **clientes** na barra de navegação à esquerda e, em seguida, selecione o cliente que você deseja mover para a nova assinatura.</span><span class="sxs-lookup"><span data-stu-id="34f09-132">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="34f09-133">Selecione **Adicionar assinatura**.</span><span class="sxs-lookup"><span data-stu-id="34f09-133">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="34f09-134">Selecione a assinatura que deseja comprar no catálogo (nesse caso, uma das opções acima), insira o número de licenças e selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="34f09-134">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="34f09-135">Agora, seu cliente terá a assinatura antiga e a nova.</span><span class="sxs-lookup"><span data-stu-id="34f09-135">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="34f09-136">A próxima etapa é reatribuir licenças aos usuários do cliente.</span><span class="sxs-lookup"><span data-stu-id="34f09-136">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="34f09-137">Selecione **clientes** na barra de navegação à esquerda e, em seguida, selecione o cliente que você está movendo.</span><span class="sxs-lookup"><span data-stu-id="34f09-137">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="34f09-138">Selecione **usuários e licenças**.</span><span class="sxs-lookup"><span data-stu-id="34f09-138">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="34f09-139">Para reatribuir uma licença a um usuário, selecione o usuário e, em seguida, selecione **gerenciar licenças**.</span><span class="sxs-lookup"><span data-stu-id="34f09-139">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="34f09-140">Na página **gerenciar licenças** , desmarque a caixa de seleção Dynamics 365 para vendas/plano de envolvimento do cliente da licença básica (oferta qualificada) e selecione um novo plano de serviço para a assinatura à qual o cliente está se movendo.</span><span class="sxs-lookup"><span data-stu-id="34f09-140">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="34f09-141">Selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="34f09-141">Select **Submit**.</span></span> <span data-ttu-id="34f09-142">Você fará isso para cada usuário que precisa da nova licença.</span><span class="sxs-lookup"><span data-stu-id="34f09-142">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="34f09-143">Depois de mover as licenças para a nova assinatura, você poderá cancelar a assinatura antiga.</span><span class="sxs-lookup"><span data-stu-id="34f09-143">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="34f09-144">Selecione **clientes** na barra de navegação à esquerda e, em seguida, selecione o cliente que você está movendo.</span><span class="sxs-lookup"><span data-stu-id="34f09-144">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="34f09-145">Na página detalhes da assinatura, defina a assinatura antiga como **suspensa** e selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="34f09-145">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="34f09-146">A assinatura antiga agora está suspensa e a nova assinatura está ativa.</span><span class="sxs-lookup"><span data-stu-id="34f09-146">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="34f09-147">A assinatura suspensa será desprovisionada automaticamente após 120 dias.</span><span class="sxs-lookup"><span data-stu-id="34f09-147">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="34f09-148">Seu cliente não incorrerá em nenhum custo adicional para a assinatura antiga.</span><span class="sxs-lookup"><span data-stu-id="34f09-148">Your customer will incur no additional costs for the old subscription.</span></span>
