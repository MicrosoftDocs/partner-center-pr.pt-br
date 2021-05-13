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
ms.openlocfilehash: 14e901f51841e58b28a3cbbb1b7a19ce89d7c324
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855345"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="089fa-103">Definir, verificar ou remover orçamentos mensais de gastos do Azure para clientes no Partner Center</span><span class="sxs-lookup"><span data-stu-id="089fa-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="089fa-104">**Funções apropriadas**: agente de administração</span><span class="sxs-lookup"><span data-stu-id="089fa-104">**Appropriate roles**: Admin agent</span></span>

<span data-ttu-id="089fa-105">Você pode [definir um orçamento de gastos do Azure mensal para seus clientes](#set-azure-spending-budget) no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="089fa-105">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="089fa-106">Isso ajuda seus clientes a gerenciar seus gastos com o Azure.</span><span class="sxs-lookup"><span data-stu-id="089fa-106">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="089fa-107">Essa opção permite que você compare os gastos do Azure dos clientes com o orçamento durante o mês.</span><span class="sxs-lookup"><span data-stu-id="089fa-107">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="089fa-108">Ele também ajuda seus clientes a orçar seus gastos do Azure para que sua fatura mensal não seja maior do que a previsão.</span><span class="sxs-lookup"><span data-stu-id="089fa-108">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="089fa-109">Esse recurso não está disponível na área restrita ou no teste em contas de produção (TIP).</span><span class="sxs-lookup"><span data-stu-id="089fa-109">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="089fa-110">Depois [de definir um orçamento de gastos do Azure para seus clientes](#set-azure-spending-budget), você também pode examinar o uso do cliente das seguintes maneiras.</span><span class="sxs-lookup"><span data-stu-id="089fa-110">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="089fa-111">Essas opções podem ajudá-lo a identificar serviços mal configurados ou tendências incomuns que podem sugerir fraudes.</span><span class="sxs-lookup"><span data-stu-id="089fa-111">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="089fa-112">Em seguida, você pode trabalhar com seus clientes para identificar a causa raiz e gerenciar os custos.</span><span class="sxs-lookup"><span data-stu-id="089fa-112">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="089fa-113">Se necessário, você também pode [alterar o orçamento do cliente](#set-azure-spending-budget) para um valor mais alto.</span><span class="sxs-lookup"><span data-stu-id="089fa-113">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="089fa-114">Verificar os gastos atuais do Azure</span><span class="sxs-lookup"><span data-stu-id="089fa-114">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="089fa-115">Ativar notificações por email para quando o gasto de um cliente estiver se aproximando de seu limite de orçamento</span><span class="sxs-lookup"><span data-stu-id="089fa-115">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="089fa-116">Exibir custos discriminados por serviço para assinaturas baseadas em uso</span><span class="sxs-lookup"><span data-stu-id="089fa-116">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="089fa-117">Você também pode [remover um orçamento de gastos do Azure](#remove-azure-spending-budget) para clientes a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="089fa-117">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="089fa-118">Dados de gastos do Azure</span><span class="sxs-lookup"><span data-stu-id="089fa-118">Azure spending data</span></span>

<span data-ttu-id="089fa-119">Os dados de gastos do Azure são uma *estimativa* e *valores de cobrança reais podem variar*.</span><span class="sxs-lookup"><span data-stu-id="089fa-119">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="089fa-120">O valor dos dados *não reflete* impostos, créditos, ajustes ou outros encargos que podem ser aplicados.</span><span class="sxs-lookup"><span data-stu-id="089fa-120">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="089fa-121">Os dados de gastos são *atualizados uma vez por dia*.</span><span class="sxs-lookup"><span data-stu-id="089fa-121">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="089fa-122">Seus clientes podem continuar a usar (e ser cobrados por) serviços e recursos do Azure, a menos que você altere suas configurações de conta no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="089fa-122">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="089fa-123">Definir o orçamento de gastos do Azure</span><span class="sxs-lookup"><span data-stu-id="089fa-123">Set Azure spending budget</span></span>

<span data-ttu-id="089fa-124">Você pode definir um orçamento mensal de gastos do *Azure* para vários clientes Partner Center:</span><span class="sxs-lookup"><span data-stu-id="089fa-124">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="089fa-125">Entre no [Painel do Partner Center](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="089fa-125">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="089fa-126">No menu à esquerda, em **CSP,** escolha **Gastos do Azure.**</span><span class="sxs-lookup"><span data-stu-id="089fa-126">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="089fa-127">Na página de gastos do **Azure,** em Clientes com **Microsoft Azure assinaturas,** selecione os clientes para os quais você deseja definir um orçamento.</span><span class="sxs-lookup"><span data-stu-id="089fa-127">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="089fa-128">Insira um valor para **Orçamento mensal.**</span><span class="sxs-lookup"><span data-stu-id="089fa-128">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="089fa-129">Escolha **Aplicar** para salvar suas alterações.</span><span class="sxs-lookup"><span data-stu-id="089fa-129">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="089fa-130">Você também pode *definir um orçamento para um cliente individual em* suas configurações de assinatura:</span><span class="sxs-lookup"><span data-stu-id="089fa-130">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="089fa-131">Entre no Painel do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="089fa-131">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="089fa-132">No menu à esquerda em **CSP,** escolha **Clientes**.</span><span class="sxs-lookup"><span data-stu-id="089fa-132">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="089fa-133">Na página **Clientes,** selecione o Nome da empresa **do cliente.**</span><span class="sxs-lookup"><span data-stu-id="089fa-133">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="089fa-134">Na página **Assinaturas** do cliente, em Assinatura **baseada em uso,** escolha **Alterar orçamento.**</span><span class="sxs-lookup"><span data-stu-id="089fa-134">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="089fa-135">Insira um valor para o orçamento.</span><span class="sxs-lookup"><span data-stu-id="089fa-135">Enter a value for the budget.</span></span>

6. <span data-ttu-id="089fa-136">Escolha **Aplicar** para salvar suas alterações.</span><span class="sxs-lookup"><span data-stu-id="089fa-136">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="089fa-137">Remover o orçamento de gastos do Azure</span><span class="sxs-lookup"><span data-stu-id="089fa-137">Remove Azure spending budget</span></span>

<span data-ttu-id="089fa-138">Você pode remover um orçamento mensal de gastos do *Azure* para seus clientes Partner Center:</span><span class="sxs-lookup"><span data-stu-id="089fa-138">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="089fa-139">Entre no [Painel do Partner Center](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="089fa-139">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="089fa-140">No menu à esquerda, em **CSP,** escolha **Gastos do Azure.**</span><span class="sxs-lookup"><span data-stu-id="089fa-140">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="089fa-141">Na página de gastos do **Azure,** em Clientes com **assinaturas Microsoft Azure**, selecione os clientes cujo orçamento você deseja remover.</span><span class="sxs-lookup"><span data-stu-id="089fa-141">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="089fa-142">Escolha **Remover orçamento**.</span><span class="sxs-lookup"><span data-stu-id="089fa-142">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="089fa-143">Verificar os gastos atuais do Azure</span><span class="sxs-lookup"><span data-stu-id="089fa-143">Check current Azure spending</span></span>

<span data-ttu-id="089fa-144">Você pode *acompanhar os gastos atuais do Azure e os orçamentos mensais* de seus clientes a qualquer momento:</span><span class="sxs-lookup"><span data-stu-id="089fa-144">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="089fa-145">Entre no [Painel do Partner Center](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="089fa-145">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="089fa-146">No menu à esquerda, em **CSP**, escolha **gastos do Azure**.</span><span class="sxs-lookup"><span data-stu-id="089fa-146">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="089fa-147">Na página de **gastos do Azure** , em **clientes com assinaturas Microsoft Azure**, você pode ver uma visão geral dos Orçamentos mensais dos clientes, estimativas de gastos atuais e percentual de orçamento usado.</span><span class="sxs-lookup"><span data-stu-id="089fa-147">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="089fa-148">Notificações para limites de orçamento</span><span class="sxs-lookup"><span data-stu-id="089fa-148">Notifications for budget limits</span></span>

<span data-ttu-id="089fa-149">Você pode *ativar as notificações por email* para quando o gasto mensal do cliente estiver se aproximando de seu limite de orçamento.</span><span class="sxs-lookup"><span data-stu-id="089fa-149">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="089fa-150">Ao ativar essa opção, você será notificado quando os clientes usarem 80% ou mais de seu orçamento mensal.</span><span class="sxs-lookup"><span data-stu-id="089fa-150">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="089fa-151">Essa opção ajuda você a ficar atento à sua fatura do Azure.</span><span class="sxs-lookup"><span data-stu-id="089fa-151">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="089fa-152">Para configurar notificações por email:</span><span class="sxs-lookup"><span data-stu-id="089fa-152">To configure email notifications:</span></span>

1. <span data-ttu-id="089fa-153">Conecte-se ao Partner Center.</span><span class="sxs-lookup"><span data-stu-id="089fa-153">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="089fa-154">Vá para **Configurações**.</span><span class="sxs-lookup"><span data-stu-id="089fa-154">Go to **Settings**.</span></span>

3. <span data-ttu-id="089fa-155">Selecione **minhas preferências**.</span><span class="sxs-lookup"><span data-stu-id="089fa-155">Select **My preferences**.</span></span>

4. <span data-ttu-id="089fa-156">Se você ainda não tiver feito isso, configure um endereço de email preferencial.</span><span class="sxs-lookup"><span data-stu-id="089fa-156">Configure a preferred email address if you haven't.</span></span>

5. <span data-ttu-id="089fa-157">Configure o idioma preferencial para a notificação.</span><span class="sxs-lookup"><span data-stu-id="089fa-157">Configure the preferred language for the notification.</span></span>

6. <span data-ttu-id="089fa-158">Selecione a guia **CSP** na seção **preferências de notificação** .</span><span class="sxs-lookup"><span data-stu-id="089fa-158">Select **CSP** tab under **Notification preferences** section.</span></span>

7. <span data-ttu-id="089fa-159">Marque a opção de email para notificação de **gastos do Azure** e **salve**.</span><span class="sxs-lookup"><span data-stu-id="089fa-159">Check the Email option for **Azure Spending** notification, and **Save**.</span></span>


## <a name="itemized-costs-by-service"></a><span data-ttu-id="089fa-160">Custos discriminados por serviço</span><span class="sxs-lookup"><span data-stu-id="089fa-160">Itemized costs by service</span></span>

<span data-ttu-id="089fa-161">Você pode *exibir os custos discriminados (e o uso estimado) por serviço para assinaturas baseadas em uso*:</span><span class="sxs-lookup"><span data-stu-id="089fa-161">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="089fa-162">Conecte-se ao Partner Center.</span><span class="sxs-lookup"><span data-stu-id="089fa-162">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="089fa-163">No menu à esquerda, em **CSP**, escolha **clientes**.</span><span class="sxs-lookup"><span data-stu-id="089fa-163">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="089fa-164">Na página **clientes** , selecione o **nome da empresa** do cliente.</span><span class="sxs-lookup"><span data-stu-id="089fa-164">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="089fa-165">Na página **assinaturas** do cliente, em **assinaturas baseadas em uso**, selecione o nome da **assinatura**.</span><span class="sxs-lookup"><span data-stu-id="089fa-165">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="089fa-166">Na página da assinatura, você pode examinar os **custos discriminados** por serviço e o **uso estimado** para o mês atual.</span><span class="sxs-lookup"><span data-stu-id="089fa-166">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>


## <a name="next-steps"></a><span data-ttu-id="089fa-167">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="089fa-167">Next steps</span></span>

- [<span data-ttu-id="089fa-168">Nova experiência de comércio no CSP – cobrança do Azure</span><span class="sxs-lookup"><span data-stu-id="089fa-168">New commerce experience in CSP - Azure billing</span></span>](azure-plan-billing.md)
