---
title: Migrar o Dynamics 365 Business Edition
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como migrar ofertas do Dynamics 365 Business Edition qualificadas para versões mais recentes antes que elas expirem.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e83c06c11638bdde508fd27904038bcb6d8c9e9c
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132631"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="405b7-103">Migrar as ofertas do Dynamics 365 Business Edition para versões mais recentes</span><span class="sxs-lookup"><span data-stu-id="405b7-103">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span>

<span data-ttu-id="405b7-104">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="405b7-104">**Appropriate roles**</span></span>

- <span data-ttu-id="405b7-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="405b7-105">Global admin</span></span>
- <span data-ttu-id="405b7-106">Administrador de gerenciamento de usuário</span><span class="sxs-lookup"><span data-stu-id="405b7-106">User management admin</span></span>
- <span data-ttu-id="405b7-107">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="405b7-107">Admin agent</span></span>
- <span data-ttu-id="405b7-108">Agente de vendas</span><span class="sxs-lookup"><span data-stu-id="405b7-108">Sales agent</span></span>

<span data-ttu-id="405b7-109">A partir de 1º de janeiro de 2019, os clientes com as assinaturas do Dynamics 365 Business Edition não podem mais renovar essas ofertas herdadas; as assinaturas existentes não serão renovadas automaticamente quando expirarem.</span><span class="sxs-lookup"><span data-stu-id="405b7-109">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="405b7-110">Na página de detalhes da assinatura, o status da assinatura será alterado para "expira em [data]" de "renovações automáticas em [data]".</span><span class="sxs-lookup"><span data-stu-id="405b7-110">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="405b7-111">Para garantir a continuidade dos clientes, você deve fazer a transição deles com assinaturas expirando para uma opção com suporte, listada abaixo.</span><span class="sxs-lookup"><span data-stu-id="405b7-111">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="405b7-112">É recomendável mover os clientes para novas assinaturas antes da data de término anual da assinatura para evitar qualquer interrupção de serviço para os clientes.</span><span class="sxs-lookup"><span data-stu-id="405b7-112">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="405b7-113">Se você usar a API (CREST ou o Partner Center), poderá encontrar assinaturas expirando, avaliando a data de término da assinatura junto com a propriedade renovação automática = falso.</span><span class="sxs-lookup"><span data-stu-id="405b7-113">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="405b7-114">As assinaturas em questão serão definidas para renovação automática = falso em 1º de janeiro de 2019.</span><span class="sxs-lookup"><span data-stu-id="405b7-114">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="405b7-115">Você pode mover os clientes para um novo plano a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="405b7-115">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="405b7-116">As edições Business do Dynamics 365 estão sendo desativadas</span><span class="sxs-lookup"><span data-stu-id="405b7-116">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="405b7-117">Dynamics 365 for Finance and Operations, Business Edition</span><span class="sxs-lookup"><span data-stu-id="405b7-117">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="405b7-118">Dynamics 365 para Team Members, Business Edition</span><span class="sxs-lookup"><span data-stu-id="405b7-118">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="405b7-119">Dynamics Business Central-as novas ofertas do Dynamics 365 Business Edition</span><span class="sxs-lookup"><span data-stu-id="405b7-119">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="405b7-120">Com as novas ofertas do Dynamics Business central, seus clientes podem conectar suas finanças, vendas, serviços e operações para simplificar os processos de negócios, melhorar as interações com o cliente e tomar decisões melhores.</span><span class="sxs-lookup"><span data-stu-id="405b7-120">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="405b7-121">O Dynamics 365 Business central é baseado em nuvem e está disponível somente por meio de parceiros do programa CSP (provedor de soluções na nuvem).</span><span class="sxs-lookup"><span data-stu-id="405b7-121">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="405b7-122">Os clientes do Dynamics 365 Business Edition estão qualificados a receber preços de transição com desconto para as novas ofertas do Business central até 30 de junho de 2020.</span><span class="sxs-lookup"><span data-stu-id="405b7-122">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="405b7-123">Transição dos clientes para novos planos do produto</span><span class="sxs-lookup"><span data-stu-id="405b7-123">Transition customers to new product plans</span></span>

 <span data-ttu-id="405b7-124">Mover clientes de SKUs desativados para os mais recentes requer as seguintes etapas nesta ordem:</span><span class="sxs-lookup"><span data-stu-id="405b7-124">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="405b7-125">Comprar a nova assinatura</span><span class="sxs-lookup"><span data-stu-id="405b7-125">Purchase the new subscription</span></span>
- <span data-ttu-id="405b7-126">Reatribuir as licenças de usuário atuais</span><span class="sxs-lookup"><span data-stu-id="405b7-126">Reassign current user licenses</span></span>
- <span data-ttu-id="405b7-127">Cancelar a assinatura antiga</span><span class="sxs-lookup"><span data-stu-id="405b7-127">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="405b7-128">Comprar o novo plano para o cliente</span><span class="sxs-lookup"><span data-stu-id="405b7-128">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="405b7-129">Selecione **clientes** na barra de navegação à esquerda e, em seguida, selecione o cliente que você deseja mover para a nova assinatura.</span><span class="sxs-lookup"><span data-stu-id="405b7-129">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="405b7-130">Selecione **Adicionar assinatura**.</span><span class="sxs-lookup"><span data-stu-id="405b7-130">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="405b7-131">Selecione a assinatura que deseja comprar no catálogo (nesse caso, uma das opções acima), insira o número de licenças e selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="405b7-131">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="405b7-132">Agora, seu cliente terá a assinatura antiga e a nova.</span><span class="sxs-lookup"><span data-stu-id="405b7-132">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="405b7-133">A próxima etapa é reatribuir licenças aos usuários do cliente.</span><span class="sxs-lookup"><span data-stu-id="405b7-133">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="405b7-134">Selecione **clientes** na barra de navegação à esquerda e, em seguida, selecione o cliente que você está movendo.</span><span class="sxs-lookup"><span data-stu-id="405b7-134">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="405b7-135">Selecione **usuários e licenças**.</span><span class="sxs-lookup"><span data-stu-id="405b7-135">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="405b7-136">Para reatribuir uma licença a um usuário, selecione o usuário e, em seguida, selecione **gerenciar licenças**.</span><span class="sxs-lookup"><span data-stu-id="405b7-136">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="405b7-137">Na página **gerenciar licenças** , desmarque a caixa de seleção Dynamics 365 para vendas/plano de envolvimento do cliente da licença básica (oferta qualificada) e selecione um novo plano de serviço para a assinatura à qual o cliente está se movendo.</span><span class="sxs-lookup"><span data-stu-id="405b7-137">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="405b7-138">Selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="405b7-138">Select **Submit**.</span></span> <span data-ttu-id="405b7-139">Você fará isso para cada usuário que precisa da nova licença.</span><span class="sxs-lookup"><span data-stu-id="405b7-139">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="405b7-140">Depois de mover as licenças para a nova assinatura, você poderá cancelar a assinatura antiga.</span><span class="sxs-lookup"><span data-stu-id="405b7-140">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="405b7-141">Selecione **clientes** na barra de navegação à esquerda e, em seguida, selecione o cliente que você está movendo.</span><span class="sxs-lookup"><span data-stu-id="405b7-141">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="405b7-142">Na página detalhes da assinatura, defina a assinatura antiga como **suspensa** e selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="405b7-142">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="405b7-143">A assinatura antiga agora está suspensa e a nova assinatura está ativa.</span><span class="sxs-lookup"><span data-stu-id="405b7-143">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="405b7-144">A assinatura suspensa será desprovisionada automaticamente após 120 dias.</span><span class="sxs-lookup"><span data-stu-id="405b7-144">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="405b7-145">Seu cliente não incorrerá em nenhum custo adicional para a assinatura antiga.</span><span class="sxs-lookup"><span data-stu-id="405b7-145">Your customer will incur no additional costs for the old subscription.</span></span>
