---
title: Transferir a assinatura do Azure em um plano do Azure para outro parceiro CSP
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como alterar o parceiro de programa do provedor de soluções na nuvem associado às assinaturas do Azure de um cliente em um plano do Azure.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: e792e4af2999924ba8be77ec0517ce56c1db7a27
ms.sourcegitcommit: ed5c873d19f0464cc986fe6e852383cd4280daf6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/05/2021
ms.locfileid: "97893199"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a><span data-ttu-id="2ced2-103">Transferir as assinaturas do plano do Azure de um cliente para um parceiro diferente</span><span class="sxs-lookup"><span data-stu-id="2ced2-103">Transfer a customer's Azure plan subscriptions to a different partner</span></span>

<span data-ttu-id="2ced2-104">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="2ced2-104">**Appropriate roles**</span></span>

- <span data-ttu-id="2ced2-105">Parceiros no programa CSP (Provedor de Soluções na Nuvem)</span><span class="sxs-lookup"><span data-stu-id="2ced2-105">Partners in the Cloud Solution Provider (CSP) program</span></span>

<span data-ttu-id="2ced2-106">Este artigo descreve como um cliente pode mudar suas assinaturas do Azure em um plano do Azure de um CSP (provedor de soluções de nuvem) para outro.</span><span class="sxs-lookup"><span data-stu-id="2ced2-106">This article describes how a customer can switch their Azure subscriptions under an Azure plan from one Cloud Solution Provider (CSP) to another.</span></span>

<span data-ttu-id="2ced2-107">Para mudar as assinaturas do Azure do cliente de um parceiro diferente, siga estas etapas.</span><span class="sxs-lookup"><span data-stu-id="2ced2-107">To switch a customer's Azure subscriptions from a different partner, follow these steps.</span></span> <span data-ttu-id="2ced2-108">O parceiro e o cliente têm as etapas a serem concluídas.</span><span class="sxs-lookup"><span data-stu-id="2ced2-108">Both the partner and the customer have steps to complete.</span></span>

>[!Note]  
><span data-ttu-id="2ced2-109">Somente parceiros com uma relação de cobrança direta com a Microsoft podem acessar as ferramentas de transição.</span><span class="sxs-lookup"><span data-stu-id="2ced2-109">Only partners with a direct billing relationship with Microsoft can access the transition tooling.</span></span> <span data-ttu-id="2ced2-110">Revendedores indiretos devem trabalhar com seus provedores indiretos para aproveitar essa ferramenta de transição.</span><span class="sxs-lookup"><span data-stu-id="2ced2-110">Indirect Resellers must work with their Indirect Providers to leverage this transition tool.</span></span>

<span data-ttu-id="2ced2-111">O cliente deve estar em conversa com os dois parceiros (atuais e futuros) antes da utilização dessa ferramenta.</span><span class="sxs-lookup"><span data-stu-id="2ced2-111">The customer must be in conversation with both partners (current and future) prior to this tool being leveraged.</span></span> <span data-ttu-id="2ced2-112">Uma conversa offline precisa ser necessária para evitar confusão e variações.</span><span class="sxs-lookup"><span data-stu-id="2ced2-112">An offline conversation needs to be had to avoid confusion and churn.</span></span> <span data-ttu-id="2ced2-113">Além disso, os parceiros e os clientes devem entender essas considerações e pré-requisitos antes de iniciar uma transição:</span><span class="sxs-lookup"><span data-stu-id="2ced2-113">In addition, partners and customers should understand these considerations and prerequisites prior to initiating a transition:</span></span>

<span data-ttu-id="2ced2-114">**Principais considerações:**</span><span class="sxs-lookup"><span data-stu-id="2ced2-114">**Key considerations:**</span></span>

- <span data-ttu-id="2ced2-115">As reservas do Azure não serão movidas com a assinatura para o parceiro futuro</span><span class="sxs-lookup"><span data-stu-id="2ced2-115">Azure Reservations will not move with the subscription to future partner</span></span>
- <span data-ttu-id="2ced2-116">O preço do CSP para serviços do Azure sob o parceiro atual não fará a transição</span><span class="sxs-lookup"><span data-stu-id="2ced2-116">CSP pricing for Azure services under current partner will not transition</span></span>  
- <span data-ttu-id="2ced2-117">As responsabilidades de suporte para o cliente passarão para o futuro parceiro</span><span class="sxs-lookup"><span data-stu-id="2ced2-117">Support responsibilities for customer will move to future partner</span></span>
- <span data-ttu-id="2ced2-118">Cobrança e faturamento serão transferidos para o futuro parceiro no momento da transferência</span><span class="sxs-lookup"><span data-stu-id="2ced2-118">Billing and invoicing will move to future partner at time of transfer</span></span>
- <span data-ttu-id="2ced2-119">O RBAC (controle de acesso do Role-Based do Azure) não é afetado pela transferência</span><span class="sxs-lookup"><span data-stu-id="2ced2-119">Azure Role-Based Access Control (RBAC) is not affected by the transfer</span></span>
- <span data-ttu-id="2ced2-120">O administrador em nome de (AOBO) não será concedido por padrão ao parceiro futuro</span><span class="sxs-lookup"><span data-stu-id="2ced2-120">Admin on Behalf Of (AOBO) will not be granted by default to the future partner</span></span>
- <span data-ttu-id="2ced2-121">Os produtos do Marketplace de terceiros serão transferidos desde que os produtos passem pela verificação de qualificação do Marketplace.</span><span class="sxs-lookup"><span data-stu-id="2ced2-121">Third-party marketplace products will transfer as long as the products pass the Marketplace eligibility check.</span></span>
    - <span data-ttu-id="2ced2-122">Não há descontos especiais ou restrições regionais</span><span class="sxs-lookup"><span data-stu-id="2ced2-122">There are no special discounts or regional restrictions</span></span>
    - <span data-ttu-id="2ced2-123">Os produtos não são baseados em assinatura</span><span class="sxs-lookup"><span data-stu-id="2ced2-123">The products are non-subscription based</span></span>
    - <span data-ttu-id="2ced2-124">O parceiro futuro deve funcionar com o editor para garantir que eles estejam na lista de permissões para implantação do produto</span><span class="sxs-lookup"><span data-stu-id="2ced2-124">The future partner should work with the publisher to make sure they are on the allow-list for deployment of the product</span></span>
    - <span data-ttu-id="2ced2-125">Se nem todas essas condições forem atendidas para transferir os produtos do Marketplace devem ser cancelados, as assinaturas do Azure transferidas e, em seguida, adquirir novamente de produtos do Marketplace com o novo parceiro</span><span class="sxs-lookup"><span data-stu-id="2ced2-125">If not all of these conditions are met in order to transfer the Marketplace products should be canceled, the Azure subscriptions transferred, and then repurchase of Marketplace products with the new partner</span></span>

<span data-ttu-id="2ced2-126">**Pré-requisitos:**</span><span class="sxs-lookup"><span data-stu-id="2ced2-126">**Prerequisites:**</span></span>

- <span data-ttu-id="2ced2-127">O cliente participa do parceiro CSP atual em sua intenção de fazer a transição</span><span class="sxs-lookup"><span data-stu-id="2ced2-127">Customer engages current CSP partner on their intent to transition</span></span>
- <span data-ttu-id="2ced2-128">O futuro parceiro CSP trabalha com o cliente para garantir que as necessidades do cliente possam ser atendidas</span><span class="sxs-lookup"><span data-stu-id="2ced2-128">Future CSP partner works with customer to ensure customer needs can be met</span></span>
- <span data-ttu-id="2ced2-129">O parceiro CSP futuro estabelece uma relação com o cliente e adquire um plano do Azure antes que a transição comece</span><span class="sxs-lookup"><span data-stu-id="2ced2-129">Future CSP partner establishes a relationship with customer and purchases an Azure plan before the transition begins</span></span>  
- <span data-ttu-id="2ced2-130">O cliente deve assinar o contrato do cliente da Microsoft com o futuro parceiro CSP</span><span class="sxs-lookup"><span data-stu-id="2ced2-130">Customer must sign Microsoft Customer Agreement with future CSP partner</span></span>
- <span data-ttu-id="2ced2-131">O parceiro CSP futuro deve ter assinado o Microsoft Partner Agreement para usar essa ferramenta</span><span class="sxs-lookup"><span data-stu-id="2ced2-131">Future CSP partner must have signed the Microsoft Partner Agreement to use this tool</span></span>

## <a name="customer-tasks-to-be-completed"></a><span data-ttu-id="2ced2-132">Tarefas do cliente a serem concluídas</span><span class="sxs-lookup"><span data-stu-id="2ced2-132">Customer tasks to be completed</span></span>

<span data-ttu-id="2ced2-133">Para transferir uma assinatura do Azure em um plano do Azure, o cliente deve iniciar o processo entrando em contato com o parceiro atual.</span><span class="sxs-lookup"><span data-stu-id="2ced2-133">To transfer an Azure subscription under an Azure plan, the customer must start the process by contacting their current partner.</span></span> <span data-ttu-id="2ced2-134">Eles devem coletar o nome e o domínio da empresa do seu parceiro atual para que seu parceiro futuro possa concluir o formulário de solicitação de transferência em seu nome.</span><span class="sxs-lookup"><span data-stu-id="2ced2-134">They should collect their current partner's company name and domain so their future partner can complete the transfer request form on their behalf.</span></span>

<span data-ttu-id="2ced2-135">O cliente também deve identificar as assinaturas que desejam transferir de seu parceiro atual.</span><span class="sxs-lookup"><span data-stu-id="2ced2-135">The customer must also identify the subscriptions they wish to transfer from their current partner.</span></span> <span data-ttu-id="2ced2-136">Você não pode alterar parceiros para as assinaturas do Office 365, Enterprise Mobility Suite ou Microsoft Dynamics CRM.</span><span class="sxs-lookup"><span data-stu-id="2ced2-136">You can't change partners for Office 365, Enterprise Mobility Suite, or Microsoft Dynamics CRM subscriptions.</span></span>

>[!Note]  
><span data-ttu-id="2ced2-137">É responsabilidade do parceiro futuro concluir o formulário de solicitação de transferência que inicia o processo de transferência.</span><span class="sxs-lookup"><span data-stu-id="2ced2-137">It is the future partner's responsibility to complete the transfer request form that initiates the transfer process.</span></span> <span data-ttu-id="2ced2-138">A Microsoft não pode intervir em nome do cliente ou do parceiro atual.</span><span class="sxs-lookup"><span data-stu-id="2ced2-138">Microsoft cannot intervene on behalf of the customer or the current partner.</span></span> <span data-ttu-id="2ced2-139">O cliente deve planejar trabalhar em conjunto com seus parceiros futuros e atuais para fazer a transição funcionar sem problemas.</span><span class="sxs-lookup"><span data-stu-id="2ced2-139">The customer should plan to work closely with their future and current partner to make the transition go smoothly.</span></span>

## <a name="future-partner-tasks-to-be-completed"></a><span data-ttu-id="2ced2-140">Tarefas futuras do parceiro a serem concluídas</span><span class="sxs-lookup"><span data-stu-id="2ced2-140">Future partner tasks to be completed</span></span>

<span data-ttu-id="2ced2-141">O parceiro futuro da assinatura precisa concluir um formulário de solicitação de transferência do Partner Center para solicitar uma transferência de assinatura:</span><span class="sxs-lookup"><span data-stu-id="2ced2-141">The future partner of the subscription needs to complete a transfer request form from Partner Center to request a subscription transfer:</span></span>

1.  <span data-ttu-id="2ced2-142">No menu do centro de parceiros, selecione **clientes** e selecione o cliente para o qual você deseja concluir um formulário de solicitação de transferência em nome de.</span><span class="sxs-lookup"><span data-stu-id="2ced2-142">From the Partner Center menu, select **Customers**, then select the customer you wish to complete a transfer request form on behalf of.</span></span>
2.  <span data-ttu-id="2ced2-143">No menu cliente, selecione **assinaturas**.</span><span class="sxs-lookup"><span data-stu-id="2ced2-143">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="2ced2-144">Selecione a seção **solicitação de transferência** .</span><span class="sxs-lookup"><span data-stu-id="2ced2-144">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="2ced2-145">Na **seção solicitação de transferência**, selecione **Adicionar nova solicitação**.</span><span class="sxs-lookup"><span data-stu-id="2ced2-145">From the **Transfer request section**, select **Add new request**.</span></span>

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Seção de transferências":::

5.  <span data-ttu-id="2ced2-147">Preencha o formulário de **nova solicitação de transferência** .</span><span class="sxs-lookup"><span data-stu-id="2ced2-147">Complete the **New transfer request** form.</span></span>

6.  <span data-ttu-id="2ced2-148">Selecione **Enviar solicitação de transferência**  >  **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="2ced2-148">Select **Send transfer request** > **Send**.</span></span>

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Formulário concluir solicitação de transferência":::

7.  <span data-ttu-id="2ced2-150">Examinar a confirmação da solicitação de transferência</span><span class="sxs-lookup"><span data-stu-id="2ced2-150">Review Transfer request confirmation</span></span>

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Revisar transferência pendente":::

    >[!Note]
    ><span data-ttu-id="2ced2-152">O parceiro futuro pode cancelar a solicitação de transferência selecionando **Cancelar solicitação** no canto superior direito somente quando o status da solicitação de transferência for "pendente".</span><span class="sxs-lookup"><span data-stu-id="2ced2-152">The future partner can cancel the transfer request by selecting **cancel request** in the upper right-hand corner only when the transfer request status is “pending”.</span></span> <span data-ttu-id="2ced2-153">Depois que o status da solicitação de transferência for "em andamento" ou "concluído", os cancelamentos não serão possíveis.</span><span class="sxs-lookup"><span data-stu-id="2ced2-153">Once the transfer request status is “in progress” or “complete”, cancellations will not be possible.</span></span>

## <a name="current-partner-tasks-to-be-completed"></a><span data-ttu-id="2ced2-154">Tarefas do parceiro atual a serem concluídas</span><span class="sxs-lookup"><span data-stu-id="2ced2-154">Current partner tasks to be completed</span></span>

<span data-ttu-id="2ced2-155">O agente de administrador do parceiro atual do cliente receberá um email informando que o cliente está solicitando uma transferência de suas assinaturas:</span><span class="sxs-lookup"><span data-stu-id="2ced2-155">The current partner's Admin Agent of the customer will receive an email that their customer is requesting a transfer of their subscriptions:</span></span>

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Examinar":::

<span data-ttu-id="2ced2-157">Examine e aceite o formulário de solicitação de transferência do centro de parceiros para concluir a transferência da assinatura.</span><span class="sxs-lookup"><span data-stu-id="2ced2-157">Review and accept the transfer request form from Partner Center to complete the subscription transfer.</span></span>

>[!Note]  
><span data-ttu-id="2ced2-158">Se nenhuma ação for realizada pelo parceiro atual dentro de 30 dias, a solicitação expirará e o parceiro futuro terá um para criar uma nova solicitação de transferência.</span><span class="sxs-lookup"><span data-stu-id="2ced2-158">If no action is taken by the current partner within 30 days the request will expire and the future partner will have a to create a new transfer request.</span></span>

1.  <span data-ttu-id="2ced2-159">Selecione **examinar solicitação de transferência** do email ou</span><span class="sxs-lookup"><span data-stu-id="2ced2-159">Select **Review transfer Request** from the email OR</span></span>
1.  <span data-ttu-id="2ced2-160">No menu do centro de parceiros, selecione **clientes** e, em seguida, selecione o cliente para o qual uma solicitação de transferência foi enviada em nome de.</span><span class="sxs-lookup"><span data-stu-id="2ced2-160">From the Partner Center menu, select **Customers**, then select the customer that a transfer request has been submitted on behalf of.</span></span>
2.  <span data-ttu-id="2ced2-161">No menu cliente, selecione **assinaturas**.</span><span class="sxs-lookup"><span data-stu-id="2ced2-161">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="2ced2-162">Selecione a seção **solicitação de transferência** .</span><span class="sxs-lookup"><span data-stu-id="2ced2-162">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="2ced2-163">Expanda informações de transferência selecionando a **ID da solicitação de transferência** escolhida em **solicitações recebidas**</span><span class="sxs-lookup"><span data-stu-id="2ced2-163">Expand transfer information by selecting the chosen **Transfer request ID** under **Received requests**</span></span>

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Solicitação de transferência de revisões de origem":::

5.  <span data-ttu-id="2ced2-165">Examine a solicitação de transferência.</span><span class="sxs-lookup"><span data-stu-id="2ced2-165">Review transfer request.</span></span> <span data-ttu-id="2ced2-166">Selecione as assinaturas do Azure solicitadas a serem transferidas.</span><span class="sxs-lookup"><span data-stu-id="2ced2-166">Select the requested Azure subscriptions to transfer.</span></span>

>[!Note]  
> <span data-ttu-id="2ced2-167">Antes de continuar, observe: você não terá mais acesso às assinaturas selecionadas.</span><span class="sxs-lookup"><span data-stu-id="2ced2-167">Before proceeding please note: You will no longer have access to the selected subscriptions.</span></span>
> <span data-ttu-id="2ced2-168">Você não será faturado para uso adicional.</span><span class="sxs-lookup"><span data-stu-id="2ced2-168">You will not be invoiced for further usage.</span></span>
> <span data-ttu-id="2ced2-169">As reservas do Azure não são transferidas com as assinaturas.</span><span class="sxs-lookup"><span data-stu-id="2ced2-169">Azure reservations do not transfer with the subscriptions.</span></span>

6.  <span data-ttu-id="2ced2-170">Em seguida, selecione **aceitar e transferir** para concluir o processo de transferência.</span><span class="sxs-lookup"><span data-stu-id="2ced2-170">Then select **Accept and transfer** to complete the transfer process.</span></span>

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Selecione as assinaturas a serem transferidas em seus planos do Azure":::

7.  <span data-ttu-id="2ced2-172">Exibir confirmação de aceitação da transferência.</span><span class="sxs-lookup"><span data-stu-id="2ced2-172">View transfer acceptance confirmation.</span></span>

   <span data-ttu-id="2ced2-173">Neste ponto, o parceiro futuro, o cliente e o parceiro atual serão notificados sobre a solicitação de transferência aceita por email.</span><span class="sxs-lookup"><span data-stu-id="2ced2-173">At this point, the future partner, the customer, and current partner will be notified of the accepted transfer request via email.</span></span>

   <span data-ttu-id="2ced2-174">Depois, a transição foi aceita, o status da transferência pode permanecer pendente por até 15 minutos enquanto o sistema é atualizado.</span><span class="sxs-lookup"><span data-stu-id="2ced2-174">After, the transition has been accepted the transfer status might remain Pending for up to 15 minutes while the system is updated.</span></span> <span data-ttu-id="2ced2-175">Se demorar mais, o sistema continuará tentando por três dias.</span><span class="sxs-lookup"><span data-stu-id="2ced2-175">If it takes longer, the system will keep trying for three days.</span></span> <span data-ttu-id="2ced2-176">Se o status da transferência ainda permanecer pendente, o parceiro deverá enviar uma solicitação de serviço.</span><span class="sxs-lookup"><span data-stu-id="2ced2-176">If the transfer status still remains Pending, the partner should submit a service request.</span></span>

   <span data-ttu-id="2ced2-177">Depois que a transferência for concluída, as assinaturas incluídas na solicitação aparecerão no plano do Azure do parceiro futuro e não serão mais listadas com você.</span><span class="sxs-lookup"><span data-stu-id="2ced2-177">Once the transfer is complete, the subscriptions included within the request will appear in the Azure plan of the future partner, and no longer be listed with you.</span></span>

>[!Note]  
><span data-ttu-id="2ced2-178">Para provedores indiretos: Informe seu revendedor indireto de que a solicitação de transferência foi aceita.</span><span class="sxs-lookup"><span data-stu-id="2ced2-178">For Indirect Providers: Please inform your Indirect Reseller that the transfer request has been accepted.</span></span>

### <a name="managing-your-transferred-customer-subscriptions"></a><span data-ttu-id="2ced2-179">Gerenciando suas assinaturas de cliente transferidas</span><span class="sxs-lookup"><span data-stu-id="2ced2-179">Managing your transferred customer subscriptions</span></span>
- <span data-ttu-id="2ced2-180">O acesso a usuários, grupos ou entidades de serviço existentes que foram atribuídos usando o RBAC (controle de acesso baseado em função) do Azure não é afetado durante a transição.</span><span class="sxs-lookup"><span data-stu-id="2ced2-180">Access to existing users, groups, or service principals that were assigned using Azure role-based access control (RBAC) isn't affected during the transition.</span></span> <span data-ttu-id="2ced2-181">O Azure [RBAC (](/azure/role-based-access-control/overview) controle de acesso baseado em função) ajuda seu cliente a gerenciar quem tem acesso aos recursos do Azure, o que eles podem fazer com esses recursos e em quais áreas eles têm acesso.</span><span class="sxs-lookup"><span data-stu-id="2ced2-181">Azure role-based access control [(Azure RBAC)](/azure/role-based-access-control/overview) helps your customer manage who has access to Azure resources, what they can do with those resources, and what areas they have access to.</span></span> <span data-ttu-id="2ced2-182">Como o novo parceiro, você não recebe nenhum acesso de RBAC aos recursos do cliente após a transferência da assinatura.</span><span class="sxs-lookup"><span data-stu-id="2ced2-182">As the new partner you aren't given any RBAC access to your customer’s resources after the subscription transfer.</span></span> <span data-ttu-id="2ced2-183">O parceiro anterior do seu cliente retém o acesso do RBAC.</span><span class="sxs-lookup"><span data-stu-id="2ced2-183">Your customer’s previous partner retains their RBAC access.</span></span> <span data-ttu-id="2ced2-184">Trabalhe com seu cliente para entender quem tem informações sobre suas assinaturas e como fazer as alterações desejadas.</span><span class="sxs-lookup"><span data-stu-id="2ced2-184">Work with your customer to understand who has insight into their subscriptions and how to make any wanted changes.</span></span>

- <span data-ttu-id="2ced2-185">Consequentemente, é importante que o cliente remova o acesso RBAC do Azure para seu parceiro anterior e adicione acesso para o novo parceiro.</span><span class="sxs-lookup"><span data-stu-id="2ced2-185">Consequently, it’s important that your customer removes Azure RBAC access for their previous partner and add access for the new partner.</span></span> <span data-ttu-id="2ced2-186">Para obter mais informações sobre o cliente que oferece acesso novo, consulte [o que é o Azure RBAC (controle de acesso baseado em função)?](/azure/role-based-access-control/overview)</span><span class="sxs-lookup"><span data-stu-id="2ced2-186">For more information about your customer giving new access, see [What is Azure role-based access control (Azure RBAC)?](/azure/role-based-access-control/overview)</span></span> <span data-ttu-id="2ced2-187">Para obter mais informações sobre o cliente que remove o acesso RBAC do parceiro anterior, consulte [remover uma atribuição de função](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span><span class="sxs-lookup"><span data-stu-id="2ced2-187">For more information about your customer removing your previous partner’s RBAC access, see [Remove a role assignment](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span></span>

- <span data-ttu-id="2ced2-188">Além disso, você não obtém automaticamente o [administrador em nome do (Aobo)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) acesso às suas assinaturas.</span><span class="sxs-lookup"><span data-stu-id="2ced2-188">Additionally, you don’t automatically get [Admin on Behalf Of (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) access to your subscriptions.</span></span> <span data-ttu-id="2ced2-189">O AOBO é necessário para que o parceiro gerencie as assinaturas do Azure do cliente em seu nome.</span><span class="sxs-lookup"><span data-stu-id="2ced2-189">AOBO is necessary for partner’s to manage their customer’s Azure subscriptions on their behalf.</span></span> <span data-ttu-id="2ced2-190">Para obter mais informações sobre os privilégios do Azure, consulte [obter permissões para gerenciar o serviço ou a assinatura de um cliente.](./customers-revoke-admin-privileges.md)</span><span class="sxs-lookup"><span data-stu-id="2ced2-190">For more information about Azure privileges, see [Obtain permissions to manage a customer’s service or subscription.](./customers-revoke-admin-privileges.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="2ced2-191">Próximas etapas:</span><span class="sxs-lookup"><span data-stu-id="2ced2-191">Next steps:</span></span>

- [<span data-ttu-id="2ced2-192">(RBAC do Azure)</span><span class="sxs-lookup"><span data-stu-id="2ced2-192">(Azure RBAC)</span></span>](/azure/role-based-access-control/overview)
- [<span data-ttu-id="2ced2-193">Obtenha permissões para gerenciar o serviço ou a assinatura de um cliente.</span><span class="sxs-lookup"><span data-stu-id="2ced2-193">Obtain permissions to manage a customer’s service or subscription.</span></span>](./customers-revoke-admin-privileges.md)
