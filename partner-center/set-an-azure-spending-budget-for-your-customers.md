---
title: Definir um orçamento de gasto do Azure para um cliente
ms.topic: how-to
ms.date: 03/17/2021
description: Saiba como definir ou remover orçamentos mensais de gastos do Azure para seus clientes e também para exibir dados de gastos do Azure e definir notificações relacionadas ao orçamento.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: eaf54898d7a130ca38e5a2aaeba279fb722c9e66
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712742"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="ccf4e-103">Definir, verificar ou remover orçamentos mensais de gastos do Azure para clientes no Partner Center</span><span class="sxs-lookup"><span data-stu-id="ccf4e-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="ccf4e-104">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="ccf4e-104">**Appropriate roles**</span></span>

- <span data-ttu-id="ccf4e-105">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="ccf4e-105">Admin agent</span></span>

<span data-ttu-id="ccf4e-106">Você pode [definir um orçamento de gastos do Azure mensal para seus clientes](#set-azure-spending-budget) no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-106">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="ccf4e-107">Isso ajuda seus clientes a gerenciar seus gastos com o Azure.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-107">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="ccf4e-108">Essa opção permite que você compare os gastos do Azure dos clientes com o orçamento durante o mês.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-108">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="ccf4e-109">Ele também ajuda seus clientes a orçar seus gastos do Azure para que sua fatura mensal não seja maior do que a previsão.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-109">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="ccf4e-110">Esse recurso não está disponível na área restrita ou no teste em contas de produção (TIP).</span><span class="sxs-lookup"><span data-stu-id="ccf4e-110">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="ccf4e-111">Depois [de definir um orçamento de gastos do Azure para seus clientes](#set-azure-spending-budget), você também pode examinar o uso do cliente das seguintes maneiras.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-111">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="ccf4e-112">Essas opções podem ajudá-lo a identificar serviços mal configurados ou tendências incomuns que podem sugerir fraudes.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-112">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="ccf4e-113">Em seguida, você pode trabalhar com seus clientes para identificar a causa raiz e gerenciar os custos.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-113">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="ccf4e-114">Se necessário, você também pode [alterar o orçamento do cliente](#set-azure-spending-budget) para um valor mais alto.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-114">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="ccf4e-115">Verificar os gastos atuais do Azure</span><span class="sxs-lookup"><span data-stu-id="ccf4e-115">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="ccf4e-116">Ativar notificações por email para quando o gasto de um cliente estiver se aproximando de seu limite de orçamento</span><span class="sxs-lookup"><span data-stu-id="ccf4e-116">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="ccf4e-117">Exibir custos discriminados por serviço para assinaturas baseadas em uso</span><span class="sxs-lookup"><span data-stu-id="ccf4e-117">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="ccf4e-118">Você também pode [remover um orçamento de gastos do Azure](#remove-azure-spending-budget) para clientes a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-118">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="ccf4e-119">Dados de gastos do Azure</span><span class="sxs-lookup"><span data-stu-id="ccf4e-119">Azure spending data</span></span>

<span data-ttu-id="ccf4e-120">Os dados de gastos do Azure são uma *estimativa* e *valores de cobrança reais podem variar*.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-120">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="ccf4e-121">O valor dos dados *não reflete* impostos, créditos, ajustes ou outros encargos que podem ser aplicados.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-121">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="ccf4e-122">Os dados de gastos são *atualizados uma vez por dia*.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-122">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="ccf4e-123">Os clientes podem continuar a usar (e serem cobrados) os serviços e recursos do Azure, a menos que você altere as configurações de conta no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-123">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="ccf4e-124">Definir orçamento de gastos do Azure</span><span class="sxs-lookup"><span data-stu-id="ccf4e-124">Set Azure spending budget</span></span>

<span data-ttu-id="ccf4e-125">Você pode *definir um orçamento de gastos do Azure mensal* para vários clientes no Partner Center:</span><span class="sxs-lookup"><span data-stu-id="ccf4e-125">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="ccf4e-126">Entre no [Painel do Partner Center](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="ccf4e-126">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="ccf4e-127">No menu à esquerda, em **CSP**, escolha **gastos do Azure**.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-127">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="ccf4e-128">Na página **gastos do Azure** , em **clientes com assinaturas Microsoft Azure**, selecione os clientes para os quais você deseja definir um orçamento.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-128">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="ccf4e-129">Insira um valor para o **orçamento mensal**.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-129">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="ccf4e-130">Escolha **aplicar** para salvar as alterações.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-130">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="ccf4e-131">Você também pode *definir um orçamento para um cliente individual* em suas configurações de assinatura:</span><span class="sxs-lookup"><span data-stu-id="ccf4e-131">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="ccf4e-132">Entre no Painel do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-132">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="ccf4e-133">No menu à esquerda, em **CSP**, escolha **clientes**.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-133">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="ccf4e-134">Na página **clientes** , selecione o **nome da empresa** do cliente.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-134">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="ccf4e-135">Na página **assinaturas** do cliente, em **assinatura baseada em uso**, escolha **alterar orçamento**.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-135">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="ccf4e-136">Insira um valor para o orçamento.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-136">Enter a value for the budget.</span></span>

6. <span data-ttu-id="ccf4e-137">Escolha **aplicar** para salvar as alterações.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-137">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="ccf4e-138">Remover orçamento de gastos do Azure</span><span class="sxs-lookup"><span data-stu-id="ccf4e-138">Remove Azure spending budget</span></span>

<span data-ttu-id="ccf4e-139">Você pode *remover um orçamento de gastos do Azure mensal* para seus clientes no Partner Center:</span><span class="sxs-lookup"><span data-stu-id="ccf4e-139">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="ccf4e-140">Entre no [Painel do Partner Center](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="ccf4e-140">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="ccf4e-141">No menu à esquerda, em **CSP**, escolha **gastos do Azure**.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-141">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="ccf4e-142">Na página **gastos do Azure** , em **clientes com assinaturas Microsoft Azure**, selecione os clientes cujo orçamento você deseja remover.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-142">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="ccf4e-143">Escolha **remover orçamento**.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-143">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="ccf4e-144">Verificar os gastos atuais do Azure</span><span class="sxs-lookup"><span data-stu-id="ccf4e-144">Check current Azure spending</span></span>

<span data-ttu-id="ccf4e-145">Você pode *acompanhar os gastos atuais dos clientes do Azure e os orçamentos mensais* a qualquer momento:</span><span class="sxs-lookup"><span data-stu-id="ccf4e-145">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="ccf4e-146">Entre no [Painel do Partner Center](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="ccf4e-146">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="ccf4e-147">No menu à esquerda, em **CSP**, escolha **gastos do Azure**.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-147">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="ccf4e-148">Na página de **gastos do Azure** , em **clientes com assinaturas Microsoft Azure**, você pode ver uma visão geral dos Orçamentos mensais dos clientes, estimativas de gastos atuais e percentual de orçamento usado.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-148">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="ccf4e-149">Notificações para limites de orçamento</span><span class="sxs-lookup"><span data-stu-id="ccf4e-149">Notifications for budget limits</span></span>

<span data-ttu-id="ccf4e-150">Você pode *ativar as notificações por email* para quando o gasto mensal do cliente estiver se aproximando de seu limite de orçamento.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-150">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="ccf4e-151">Ao ativar essa opção, você será notificado quando os clientes usarem 80% ou mais de seu orçamento mensal.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-151">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="ccf4e-152">Essa opção ajuda você a ficar atento à sua fatura do Azure.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-152">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="ccf4e-153">Para configurar notificações por email:</span><span class="sxs-lookup"><span data-stu-id="ccf4e-153">To configure email notifications:</span></span>

1. <span data-ttu-id="ccf4e-154">Conecte-se ao Partner Center.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-154">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="ccf4e-155">Vá para **Configurações**.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-155">Go to **Settings**.</span></span>

3. <span data-ttu-id="ccf4e-156">Selecione **minhas preferências**.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-156">Select **My preferences**.</span></span>

4. <span data-ttu-id="ccf4e-157">Se você ainda não tiver feito isso, configure um endereço de email preferencial.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-157">Configure a preferred email address if you haven't.</span></span>

5. <span data-ttu-id="ccf4e-158">Configure o idioma preferencial para a notificação.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-158">Configure the preferred language for the notification.</span></span>

6. <span data-ttu-id="ccf4e-159">Selecione a guia **CSP** na seção **preferências de notificação** .</span><span class="sxs-lookup"><span data-stu-id="ccf4e-159">Select **CSP** tab under **Notification preferences** section.</span></span>

7. <span data-ttu-id="ccf4e-160">Marque a opção de email para notificação de **gastos do Azure** e **salve**.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-160">Check the Email option for **Azure Spending** notification, and **Save**.</span></span>


## <a name="itemized-costs-by-service"></a><span data-ttu-id="ccf4e-161">Custos discriminados por serviço</span><span class="sxs-lookup"><span data-stu-id="ccf4e-161">Itemized costs by service</span></span>

<span data-ttu-id="ccf4e-162">Você pode *exibir os custos discriminados (e o uso estimado) por serviço para assinaturas baseadas em uso*:</span><span class="sxs-lookup"><span data-stu-id="ccf4e-162">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="ccf4e-163">Conecte-se ao Partner Center.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-163">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="ccf4e-164">No menu à esquerda, em **CSP**, escolha **clientes**.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-164">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="ccf4e-165">Na página **clientes** , selecione o **nome da empresa** do cliente.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-165">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="ccf4e-166">Na página **assinaturas** do cliente, em **assinaturas baseadas em uso**, selecione o nome da **assinatura**.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-166">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="ccf4e-167">Na página da assinatura, você pode examinar os **custos discriminados** por serviço e o **uso estimado** para o mês atual.</span><span class="sxs-lookup"><span data-stu-id="ccf4e-167">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>


## <a name="next-steps"></a><span data-ttu-id="ccf4e-168">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="ccf4e-168">Next steps</span></span>

- [<span data-ttu-id="ccf4e-169">Nova experiência de comércio no CSP – cobrança do Azure</span><span class="sxs-lookup"><span data-stu-id="ccf4e-169">New commerce experience in CSP - Azure billing</span></span>](azure-plan-billing.md)
