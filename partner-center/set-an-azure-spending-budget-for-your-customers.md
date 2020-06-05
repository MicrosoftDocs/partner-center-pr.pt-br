---
title: Definir um orçamento de gastos do Azure para clientes
ms.topic: article
ms.date: 06/03/2020
description: Saiba como definir ou remover orçamentos mensais de gastos do Azure para seus clientes e também para exibir dados de gastos do Azure e definir notificações relacionadas ao orçamento.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.assetid: DDE80361-D04E-432C-BC15-D735D2AE954F
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 17b6186d7e6cddaf598dc663c70841275c0db853
ms.sourcegitcommit: 7ec7514ee9693d62d8eb930aa38fe701cd152835
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2020
ms.locfileid: "84425985"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="de0f5-103">Definir, verificar ou remover orçamentos mensais de gastos do Azure para clientes no Partner Center</span><span class="sxs-lookup"><span data-stu-id="de0f5-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="de0f5-104">Aplica-se a:</span><span class="sxs-lookup"><span data-stu-id="de0f5-104">Applies to:</span></span>

- <span data-ttu-id="de0f5-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="de0f5-105">Partner Center</span></span>
- <span data-ttu-id="de0f5-106">Partner Center do Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="de0f5-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="de0f5-107">Você pode [definir um orçamento de gastos do Azure mensal para seus clientes](#set-azure-spending-budget) no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="de0f5-107">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="de0f5-108">Isso ajuda seus clientes a gerenciar seus gastos com o Azure.</span><span class="sxs-lookup"><span data-stu-id="de0f5-108">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="de0f5-109">Essa opção permite que você compare os gastos do Azure dos clientes com o orçamento durante o mês.</span><span class="sxs-lookup"><span data-stu-id="de0f5-109">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="de0f5-110">Ele também ajuda seus clientes a orçar seus gastos do Azure para que sua fatura mensal não seja maior do que a previsão.</span><span class="sxs-lookup"><span data-stu-id="de0f5-110">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="de0f5-111">Esse recurso não está disponível na área restrita ou no teste em contas de produção (TIP).</span><span class="sxs-lookup"><span data-stu-id="de0f5-111">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="de0f5-112">Depois [de definir um orçamento de gastos do Azure para seus clientes](#set-azure-spending-budget), você também pode examinar o uso do cliente das seguintes maneiras.</span><span class="sxs-lookup"><span data-stu-id="de0f5-112">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="de0f5-113">Essas opções podem ajudá-lo a identificar serviços mal configurados ou tendências incomuns que podem sugerir fraudes.</span><span class="sxs-lookup"><span data-stu-id="de0f5-113">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="de0f5-114">Em seguida, você pode trabalhar com seus clientes para identificar a causa raiz e gerenciar os custos.</span><span class="sxs-lookup"><span data-stu-id="de0f5-114">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="de0f5-115">Se necessário, você também pode [alterar o orçamento do cliente](#set-azure-spending-budget) para um valor mais alto.</span><span class="sxs-lookup"><span data-stu-id="de0f5-115">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="de0f5-116">Verificar os gastos atuais do Azure</span><span class="sxs-lookup"><span data-stu-id="de0f5-116">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="de0f5-117">Ativar notificações por email para quando o gasto de um cliente estiver se aproximando de seu limite de orçamento</span><span class="sxs-lookup"><span data-stu-id="de0f5-117">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="de0f5-118">Exibir custos discriminados por serviço para assinaturas baseadas em uso</span><span class="sxs-lookup"><span data-stu-id="de0f5-118">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="de0f5-119">Você também pode [remover um orçamento de gastos do Azure](#remove-azure-spending-budget) para clientes a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="de0f5-119">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="de0f5-120">Dados de gastos do Azure</span><span class="sxs-lookup"><span data-stu-id="de0f5-120">Azure spending data</span></span>

<span data-ttu-id="de0f5-121">Os dados de gastos do Azure são uma *estimativa* e *valores de cobrança reais podem variar*.</span><span class="sxs-lookup"><span data-stu-id="de0f5-121">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="de0f5-122">O valor dos dados *não reflete* impostos, créditos, ajustes ou outros encargos que podem ser aplicados.</span><span class="sxs-lookup"><span data-stu-id="de0f5-122">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="de0f5-123">Os dados de gastos são *atualizados uma vez por dia*.</span><span class="sxs-lookup"><span data-stu-id="de0f5-123">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="de0f5-124">Os clientes podem continuar a usar (e serem cobrados) os serviços e recursos do Azure, a menos que você altere as configurações de conta no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="de0f5-124">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="de0f5-125">Definir orçamento de gastos do Azure</span><span class="sxs-lookup"><span data-stu-id="de0f5-125">Set Azure spending budget</span></span>

<span data-ttu-id="de0f5-126">Você pode *definir um orçamento de gastos do Azure mensal* para vários clientes no Partner Center:</span><span class="sxs-lookup"><span data-stu-id="de0f5-126">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="de0f5-127">Entre no painel do [Partner Center](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="de0f5-127">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="de0f5-128">No menu à esquerda, em **CSP**, escolha **gastos do Azure**.</span><span class="sxs-lookup"><span data-stu-id="de0f5-128">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="de0f5-129">Na página **gastos do Azure** , em **clientes com assinaturas Microsoft Azure**, selecione os clientes para os quais você deseja definir um orçamento.</span><span class="sxs-lookup"><span data-stu-id="de0f5-129">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="de0f5-130">Insira um valor para o **orçamento mensal**.</span><span class="sxs-lookup"><span data-stu-id="de0f5-130">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="de0f5-131">Escolha **aplicar** para salvar as alterações.</span><span class="sxs-lookup"><span data-stu-id="de0f5-131">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="de0f5-132">Você também pode *definir um orçamento para um cliente individual* em suas configurações de assinatura:</span><span class="sxs-lookup"><span data-stu-id="de0f5-132">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="de0f5-133">Entre no Painel do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="de0f5-133">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="de0f5-134">No menu à esquerda, em **CSP**, escolha **clientes**.</span><span class="sxs-lookup"><span data-stu-id="de0f5-134">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="de0f5-135">Na página **clientes** , selecione o **nome da empresa**do cliente.</span><span class="sxs-lookup"><span data-stu-id="de0f5-135">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="de0f5-136">Na página **assinaturas** do cliente, em **assinatura baseada em uso**, escolha **alterar orçamento**.</span><span class="sxs-lookup"><span data-stu-id="de0f5-136">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="de0f5-137">Insira um valor para o orçamento.</span><span class="sxs-lookup"><span data-stu-id="de0f5-137">Enter a value for the budget.</span></span>

6. <span data-ttu-id="de0f5-138">Escolha **aplicar** para salvar as alterações.</span><span class="sxs-lookup"><span data-stu-id="de0f5-138">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="de0f5-139">Remover orçamento de gastos do Azure</span><span class="sxs-lookup"><span data-stu-id="de0f5-139">Remove Azure spending budget</span></span>

<span data-ttu-id="de0f5-140">Você pode *remover um orçamento de gastos do Azure mensal* para seus clientes no Partner Center:</span><span class="sxs-lookup"><span data-stu-id="de0f5-140">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="de0f5-141">Entre no painel do [Partner Center](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="de0f5-141">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="de0f5-142">No menu à esquerda, em **CSP**, escolha **gastos do Azure**.</span><span class="sxs-lookup"><span data-stu-id="de0f5-142">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="de0f5-143">Na página **gastos do Azure** , em **clientes com assinaturas Microsoft Azure**, selecione os clientes cujo orçamento você deseja remover.</span><span class="sxs-lookup"><span data-stu-id="de0f5-143">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="de0f5-144">Escolha **remover orçamento**.</span><span class="sxs-lookup"><span data-stu-id="de0f5-144">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="de0f5-145">Verificar os gastos atuais do Azure</span><span class="sxs-lookup"><span data-stu-id="de0f5-145">Check current Azure spending</span></span>

<span data-ttu-id="de0f5-146">Você pode *acompanhar os gastos atuais dos clientes do Azure e os orçamentos mensais* a qualquer momento:</span><span class="sxs-lookup"><span data-stu-id="de0f5-146">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="de0f5-147">Entre no painel do [Partner Center](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="de0f5-147">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="de0f5-148">No menu à esquerda, em **CSP**, escolha **gastos do Azure**.</span><span class="sxs-lookup"><span data-stu-id="de0f5-148">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="de0f5-149">Na página de **gastos do Azure** , em **clientes com assinaturas Microsoft Azure**, você pode ver uma visão geral dos Orçamentos mensais dos clientes, estimativas de gastos atuais e percentual de orçamento usado.</span><span class="sxs-lookup"><span data-stu-id="de0f5-149">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="de0f5-150">Notificações para limites de orçamento</span><span class="sxs-lookup"><span data-stu-id="de0f5-150">Notifications for budget limits</span></span>

<span data-ttu-id="de0f5-151">Você pode *ativar as notificações por email* para quando o gasto mensal do cliente estiver se aproximando de seu limite de orçamento.</span><span class="sxs-lookup"><span data-stu-id="de0f5-151">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="de0f5-152">Ao ativar essa opção, você será notificado quando os clientes usarem 80% ou mais de seu orçamento mensal.</span><span class="sxs-lookup"><span data-stu-id="de0f5-152">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="de0f5-153">Essa opção ajuda você a ficar atento à sua fatura do Azure.</span><span class="sxs-lookup"><span data-stu-id="de0f5-153">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="de0f5-154">Para configurar notificações por email:</span><span class="sxs-lookup"><span data-stu-id="de0f5-154">To configure email notifications:</span></span>

1. <span data-ttu-id="de0f5-155">Conecte-se ao Partner Center.</span><span class="sxs-lookup"><span data-stu-id="de0f5-155">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="de0f5-156">No menu à esquerda, em **CSP**, escolha **gastos do Azure**.</span><span class="sxs-lookup"><span data-stu-id="de0f5-156">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="de0f5-157">Na página **gastos do Azure** , em **notificações por email**, alterne a configuração **obter emails** para **ativado**.</span><span class="sxs-lookup"><span data-stu-id="de0f5-157">On the **Azure spending** page, under **Email notifications**, toggle the **Get emails** setting to **On**.</span></span>

4. <span data-ttu-id="de0f5-158">Escolha **Alterar endereço de email** para ver o endereço de email para notificações.</span><span class="sxs-lookup"><span data-stu-id="de0f5-158">Choose **Change email address** to see the email address for notifications.</span></span>

5. <span data-ttu-id="de0f5-159">Se o endereço de email *não estiver correto*, insira o endereço de email correto e escolha **Atualizar**.</span><span class="sxs-lookup"><span data-stu-id="de0f5-159">If the email address *isn't correct*, enter the correct email address and choose **Update**.</span></span> <span data-ttu-id="de0f5-160">Se o endereço de email *estiver correto*, escolha **Cancelar**.</span><span class="sxs-lookup"><span data-stu-id="de0f5-160">If the email address *is correct*, choose **Cancel**.</span></span>

## <a name="itemized-costs-by-service"></a><span data-ttu-id="de0f5-161">Custos discriminados por serviço</span><span class="sxs-lookup"><span data-stu-id="de0f5-161">Itemized costs by service</span></span>

<span data-ttu-id="de0f5-162">Você pode *exibir os custos discriminados (e o uso estimado) por serviço para assinaturas baseadas em uso*:</span><span class="sxs-lookup"><span data-stu-id="de0f5-162">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="de0f5-163">Conecte-se ao Partner Center.</span><span class="sxs-lookup"><span data-stu-id="de0f5-163">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="de0f5-164">No menu à esquerda, em **CSP**, escolha **clientes**.</span><span class="sxs-lookup"><span data-stu-id="de0f5-164">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="de0f5-165">Na página **clientes** , selecione o **nome da empresa**do cliente.</span><span class="sxs-lookup"><span data-stu-id="de0f5-165">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="de0f5-166">Na página **assinaturas** do cliente, em **assinaturas baseadas em uso**, selecione o nome da **assinatura**.</span><span class="sxs-lookup"><span data-stu-id="de0f5-166">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="de0f5-167">Na página da assinatura, você pode examinar os **custos discriminados** por serviço e o **uso estimado** para o mês atual.</span><span class="sxs-lookup"><span data-stu-id="de0f5-167">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>
