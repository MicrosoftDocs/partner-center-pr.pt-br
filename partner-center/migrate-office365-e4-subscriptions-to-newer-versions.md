---
title: Migrar assinaturas do Office 365 E4 para versões mais recentes do Office 365 | Partner Center
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Edições do Microsoft Office 365 Enterprise E4 estarão desativadas a partir de 7 de abril de 2017. Saiba como migrar suas assinaturas de cliente para versões mais recentes do Office 365.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 02d383172595e09a4ab0bf9c6db34862fcc17204
ms.sourcegitcommit: faf7b1ac1653497f963b428bbfafcd821378adaa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2020
ms.locfileid: "82798872"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="848b9-104">Migrar inscrições do Office 365 E4 para versões do Office 365 mais recentes</span><span class="sxs-lookup"><span data-stu-id="848b9-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="848b9-105">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="848b9-105">**Applies to**</span></span>

-  <span data-ttu-id="848b9-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="848b9-106">Partner Center</span></span>

<span data-ttu-id="848b9-107">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="848b9-107">**Appropriate roles**</span></span>
-   <span data-ttu-id="848b9-108">Administrador global</span><span class="sxs-lookup"><span data-stu-id="848b9-108">Global admin</span></span>
-   <span data-ttu-id="848b9-109">Administrador de usuários</span><span class="sxs-lookup"><span data-stu-id="848b9-109">User admin</span></span>
-   <span data-ttu-id="848b9-110">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="848b9-110">Admin agent</span></span>
-   <span data-ttu-id="848b9-111">Agente de vendas</span><span class="sxs-lookup"><span data-stu-id="848b9-111">Sales agent</span></span>

<span data-ttu-id="848b9-112">O plano do Office 365 Enterprise E4 está desativado desde 7 de abril de 2017.</span><span class="sxs-lookup"><span data-stu-id="848b9-112">The Office 365 Enterprise E4 plan is retired, effective April 7, 2017.</span></span> <span data-ttu-id="848b9-113">Você não pode comprar novas assinaturas do Office 365 E4 após essa data, e assinaturas E4 existentes não serão renovadas automaticamente quando expirarem.</span><span class="sxs-lookup"><span data-stu-id="848b9-113">You can no longer purchase new Office 365 E4 subscriptions after this date, and existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="848b9-114">Quando as assinaturas E4 terminarem, elas serão canceladas.</span><span class="sxs-lookup"><span data-stu-id="848b9-114">When E4 subscriptions end, they will be canceled.</span></span> <span data-ttu-id="848b9-115">Para garantir a continuidade dos clientes, você deve fazer a transição de clientes com assinaturas E4 vencidas para uma opção de SKU com suporte, listada abaixo.</span><span class="sxs-lookup"><span data-stu-id="848b9-115">To ensure continuity for customers, you should transition customers with expiring E4 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="848b9-116">É recomendável mover os clientes para novas assinaturas antes da data de término anual da assinatura para evitar qualquer interrupção de serviço para os clientes.</span><span class="sxs-lookup"><span data-stu-id="848b9-116">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

> [!NOTE]  
>  <span data-ttu-id="848b9-117">Os SKUs comerciais e governamentais do Office 365 Enterprise E4 são desativados.</span><span class="sxs-lookup"><span data-stu-id="848b9-117">Both Office 365 Enterprise E4 commercial and government SKUs are retired.</span></span>
 
<span data-ttu-id="848b9-118">Na página de detalhes da assinatura, o status da assinatura E4 foi alterado para "Expira em [data]" de "Renovação automática em [data]".</span><span class="sxs-lookup"><span data-stu-id="848b9-118">On the subscription's detail page, the E4 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="848b9-119">Se você usar a API (CREST ou Partner Center), você pode descobrir assinaturas vencidas avaliando a data de término da assinatura juntamente com a propriedade de renovação automática = Falso.</span><span class="sxs-lookup"><span data-stu-id="848b9-119">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> 

<span data-ttu-id="848b9-120">As inscrições do E4 serão definidas para renovação automática=Falso em 7 de abril de 2017.</span><span class="sxs-lookup"><span data-stu-id="848b9-120">The E4 subscriptions will be set to auto renew=False in April 7, 2017.</span></span> <span data-ttu-id="848b9-121">Você pode mover os clientes para um novo plano a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="848b9-121">You can move customers to a new plan at any time.</span></span> 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a><span data-ttu-id="848b9-122">Planos de substituição da edição do Office 365 E4 Enterprise</span><span class="sxs-lookup"><span data-stu-id="848b9-122">Office 365 Enterprise E4 edition replacement plans</span></span>

<span data-ttu-id="848b9-123">Você pode optar por manter a mesma funcionalidade com E4 ou deixar seus clientes tirarem vantagem de novos recursos e funcionalidades no Office 365 e Skype for Business Online.</span><span class="sxs-lookup"><span data-stu-id="848b9-123">You can choose to maintain the same functionality with E4 or have your customers take advantage of newer features and functionality in Office 365 and Skype for Business Online.</span></span> <span data-ttu-id="848b9-124">Detalhes de preço são encontrados na lista de preços e oferecem a matriz de lista no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="848b9-124">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> <span data-ttu-id="848b9-125">Secure Product Enterprise E3 ou Secure Productive Enterprise E5 podem ser substituídos nas opções a seguir para Office 365 Enterprise E3 ou Office 365 Enterprise E5, respectivamente.</span><span class="sxs-lookup"><span data-stu-id="848b9-125">Secure Product Enterprise E3 or Secure Productive Enterprise E5 may be substituted in the following options for Office 365 Enterprise E3 or Office 365 Enterprise E5 respectively.</span></span>

- <span data-ttu-id="848b9-126">Opção 1: Office 365 Enterprise E5</span><span class="sxs-lookup"><span data-stu-id="848b9-126">Option 1: Office 365 Enterprise E5</span></span>

- <span data-ttu-id="848b9-127">Opção 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span><span class="sxs-lookup"><span data-stu-id="848b9-127">Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span></span>

- <span data-ttu-id="848b9-128">Opção 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (preço e paridade funcional com E4)</span><span class="sxs-lookup"><span data-stu-id="848b9-128">Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (price and functionality parity with E4)</span></span>

- <span data-ttu-id="848b9-129">Opção 4: Office 365 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="848b9-129">Option 4: Office 365 Enterprise E3</span></span>


| <span data-ttu-id="848b9-130">Recurso</span><span class="sxs-lookup"><span data-stu-id="848b9-130">Feature</span></span> | <span data-ttu-id="848b9-131">Opção 1</span><span class="sxs-lookup"><span data-stu-id="848b9-131">Option 1</span></span> | <span data-ttu-id="848b9-132">Opção 2</span><span class="sxs-lookup"><span data-stu-id="848b9-132">Option 2</span></span> | <span data-ttu-id="848b9-133">Opção 3</span><span class="sxs-lookup"><span data-stu-id="848b9-133">Option 3</span></span> | <span data-ttu-id="848b9-134">Opção 4</span><span class="sxs-lookup"><span data-stu-id="848b9-134">Option 4</span></span> |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| <span data-ttu-id="848b9-135">Obter todos os recursos incluídos no Office 365 Enterprise E4?</span><span class="sxs-lookup"><span data-stu-id="848b9-135">Get all the features included in Office 365 Enterprise E4?</span></span> | <span data-ttu-id="848b9-136">Sim</span><span class="sxs-lookup"><span data-stu-id="848b9-136">Yes</span></span> | <span data-ttu-id="848b9-137">Sim</span><span class="sxs-lookup"><span data-stu-id="848b9-137">Yes</span></span> | <span data-ttu-id="848b9-138">Sim</span><span class="sxs-lookup"><span data-stu-id="848b9-138">Yes</span></span> | <span data-ttu-id="848b9-139">Não</span><span class="sxs-lookup"><span data-stu-id="848b9-139">No</span></span> |
| <span data-ttu-id="848b9-140">Números de telefone gerenciados no Office 365?</span><span class="sxs-lookup"><span data-stu-id="848b9-140">Phone numbers managed in Office 365?</span></span> | <span data-ttu-id="848b9-141">Sim</span><span class="sxs-lookup"><span data-stu-id="848b9-141">Yes</span></span> | <span data-ttu-id="848b9-142">Sim</span><span class="sxs-lookup"><span data-stu-id="848b9-142">Yes</span></span> | <span data-ttu-id="848b9-143">Não</span><span class="sxs-lookup"><span data-stu-id="848b9-143">No</span></span> | <span data-ttu-id="848b9-144">Não</span><span class="sxs-lookup"><span data-stu-id="848b9-144">No</span></span> |
| <span data-ttu-id="848b9-145">Números de telefone gerenciado no local e no Office 365 (implantação híbrida)?</span><span class="sxs-lookup"><span data-stu-id="848b9-145">Phone numbers managed both on-premises and in Office 365 (hybrid deployment)?</span></span> | <span data-ttu-id="848b9-146">Sim</span><span class="sxs-lookup"><span data-stu-id="848b9-146">Yes</span></span> | <span data-ttu-id="848b9-147">Sim</span><span class="sxs-lookup"><span data-stu-id="848b9-147">Yes</span></span> | <span data-ttu-id="848b9-148">Não</span><span class="sxs-lookup"><span data-stu-id="848b9-148">No</span></span> | <span data-ttu-id="848b9-149">Não</span><span class="sxs-lookup"><span data-stu-id="848b9-149">No</span></span> |
| <span data-ttu-id="848b9-150">Opção de adicionar um plano de chamada de voz PSTN?</span><span class="sxs-lookup"><span data-stu-id="848b9-150">Option to add a PSTN voice calling plan?</span></span> | <span data-ttu-id="848b9-151">Sim</span><span class="sxs-lookup"><span data-stu-id="848b9-151">Yes</span></span> | <span data-ttu-id="848b9-152">Sim</span><span class="sxs-lookup"><span data-stu-id="848b9-152">Yes</span></span> | <span data-ttu-id="848b9-153">Não</span><span class="sxs-lookup"><span data-stu-id="848b9-153">No</span></span> | <span data-ttu-id="848b9-154">Não</span><span class="sxs-lookup"><span data-stu-id="848b9-154">No</span></span> |
| <span data-ttu-id="848b9-155">Conferência por PSTN?</span><span class="sxs-lookup"><span data-stu-id="848b9-155">PSTN Conferencing?</span></span> | <span data-ttu-id="848b9-156">Sim</span><span class="sxs-lookup"><span data-stu-id="848b9-156">Yes</span></span> | <span data-ttu-id="848b9-157">Não</span><span class="sxs-lookup"><span data-stu-id="848b9-157">No</span></span> | <span data-ttu-id="848b9-158">Não</span><span class="sxs-lookup"><span data-stu-id="848b9-158">No</span></span> | <span data-ttu-id="848b9-159">Não</span><span class="sxs-lookup"><span data-stu-id="848b9-159">No</span></span> |
| <span data-ttu-id="848b9-160">Ferramentas avançadas de colaboração, análises e segurança?</span><span class="sxs-lookup"><span data-stu-id="848b9-160">Advanced tools for collaboration, analytics, and security?</span></span> | <span data-ttu-id="848b9-161">Sim</span><span class="sxs-lookup"><span data-stu-id="848b9-161">Yes</span></span> | <span data-ttu-id="848b9-162">Não</span><span class="sxs-lookup"><span data-stu-id="848b9-162">No</span></span> | <span data-ttu-id="848b9-163">Não</span><span class="sxs-lookup"><span data-stu-id="848b9-163">No</span></span> | <span data-ttu-id="848b9-164">Não</span><span class="sxs-lookup"><span data-stu-id="848b9-164">No</span></span> |
| <span data-ttu-id="848b9-165">Visualizações de relatórios, painéis e dados interativos?</span><span class="sxs-lookup"><span data-stu-id="848b9-165">Interactive reports, dashboards, and data visualizations?</span></span> | <span data-ttu-id="848b9-166">Sim</span><span class="sxs-lookup"><span data-stu-id="848b9-166">Yes</span></span> | <span data-ttu-id="848b9-167">Não</span><span class="sxs-lookup"><span data-stu-id="848b9-167">No</span></span> | <span data-ttu-id="848b9-168">Não</span><span class="sxs-lookup"><span data-stu-id="848b9-168">No</span></span> | <span data-ttu-id="848b9-169">Não</span><span class="sxs-lookup"><span data-stu-id="848b9-169">No</span></span> | 
| <span data-ttu-id="848b9-170">Mais controle sobre a segurança dos dados e a conformidade com privacidade interna, transparência e controles de usuário refinados?</span><span class="sxs-lookup"><span data-stu-id="848b9-170">More control over data security and compliance with built-in privacy, transparency, and refined user controls?</span></span> | <span data-ttu-id="848b9-171">Sim</span><span class="sxs-lookup"><span data-stu-id="848b9-171">Yes</span></span> | <span data-ttu-id="848b9-172">Não</span><span class="sxs-lookup"><span data-stu-id="848b9-172">No</span></span> | <span data-ttu-id="848b9-173">Não</span><span class="sxs-lookup"><span data-stu-id="848b9-173">No</span></span> | <span data-ttu-id="848b9-174">Não</span><span class="sxs-lookup"><span data-stu-id="848b9-174">No</span></span> | 

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="848b9-175">Transição dos clientes para novos planos do produto</span><span class="sxs-lookup"><span data-stu-id="848b9-175">Transition customers to new product plans</span></span>

<span data-ttu-id="848b9-176">A Microsoft oferece continuamente novos produtos e serviços para nossos parceiros.</span><span class="sxs-lookup"><span data-stu-id="848b9-176">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="848b9-177">Nesses casos, você pode precisar fazer o upgrade dos clientes para novos serviços ou migrar as assinaturas de SKUs que serão encerradas em breve.</span><span class="sxs-lookup"><span data-stu-id="848b9-177">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="848b9-178">A migração dos clientes de SKUs desativadas para as mais recentes requer as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="848b9-178">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

-   <span data-ttu-id="848b9-179">Comprar a nova assinatura</span><span class="sxs-lookup"><span data-stu-id="848b9-179">Purchase the new subscription</span></span>
-   <span data-ttu-id="848b9-180">Reatribuir as licenças de usuário atuais</span><span class="sxs-lookup"><span data-stu-id="848b9-180">Reassign current user licenses</span></span>
-   <span data-ttu-id="848b9-181">Cancelar a assinatura antiga</span><span class="sxs-lookup"><span data-stu-id="848b9-181">Cancel the old subscription</span></span>

<span data-ttu-id="848b9-182">Siga estas etapas para migrar a assinatura do Office 365 Enterprise E4 de cliente para uma das opções na tabela acima.</span><span class="sxs-lookup"><span data-stu-id="848b9-182">Follow these steps to migrate a customer's Office 365 Enterprise E4 subscription to one of the options in the table above.</span></span>

### <a name="step-1---purchase-the-new-subscription"></a><span data-ttu-id="848b9-183">Etapa 1 - Comprar a nova assinatura</span><span class="sxs-lookup"><span data-stu-id="848b9-183">Step 1 - Purchase the new subscription</span></span>

1. <span data-ttu-id="848b9-184">No menu do **centro de parceiros** , selecione **clientes**, selecione o cliente que você deseja mover e, em seguida, selecione **adicionar assinaturas**.</span><span class="sxs-lookup"><span data-stu-id="848b9-184">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="848b9-185">Selecione a assinatura que deseja comprar no catálogo (nesse caso, uma das opções acima), insira o número de licenças e selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="848b9-185">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

   <span data-ttu-id="848b9-186">Seu cliente agora deve ter assinaturas antigas e novas, a antiga assinatura do Office 365 Enterprise E4 e a nova assinatura de "destino", por exemplo, a opção 1-Office 365 Enterprise e5.</span><span class="sxs-lookup"><span data-stu-id="848b9-186">Your customer should now have both old and new subscriptions, the old Office 365 Enterprise E4 subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise E5.</span></span>

### <a name="step-2---reassign-the-customers-users-licenses"></a><span data-ttu-id="848b9-187">Etapa 2 - Reatribuir licenças dos usuários do cliente</span><span class="sxs-lookup"><span data-stu-id="848b9-187">Step 2 - Reassign the customer's users' licenses</span></span>

1. <span data-ttu-id="848b9-188">No menu do **centro de parceiros** , selecione **clientes**, selecione o cliente que você deseja mover e, em seguida, selecione **usuários e licenças**.</span><span class="sxs-lookup"><span data-stu-id="848b9-188">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Users and licenses**.</span></span> <span data-ttu-id="848b9-189">A página usuários e licenças do cliente é aberta.</span><span class="sxs-lookup"><span data-stu-id="848b9-189">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="848b9-190">Para reatribuir licenças de usuário, selecione o usuário a ser reatribuído e selecione **Gerenciar licenças**.</span><span class="sxs-lookup"><span data-stu-id="848b9-190">To re-assign user licenses, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="848b9-191">Na página **Gerenciar licenças**, desmarque a caixa de seleção da licença do **Office 365 Enterprise E4** e selecione um novo plano de serviço para onde o cliente está movendo a assinatura.</span><span class="sxs-lookup"><span data-stu-id="848b9-191">On the **Manage licenses** page, clear the **Office 365 Enterprise E4** license check box and select a new service plan for the subscription the customer is moving to.</span></span>

4. <span data-ttu-id="848b9-192">Selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="848b9-192">Select **Submit**.</span></span> <span data-ttu-id="848b9-193">Uma página de confirmação lista as novas atribuições de licença.</span><span class="sxs-lookup"><span data-stu-id="848b9-193">A confirmation page lists the new license assignments.</span></span>

5. <span data-ttu-id="848b9-194">Siga as mesmas etapas com outros usuários do cliente que precisam de reatribuição de licença.</span><span class="sxs-lookup"><span data-stu-id="848b9-194">Continue the same steps with any other customer users that need license reassignment.</span></span>

<span data-ttu-id="848b9-195">Depois de migrar as licenças de usuário para o novo serviço, você pode cancelar com segurança a assinatura desativada no nível superior do cliente.</span><span class="sxs-lookup"><span data-stu-id="848b9-195">After moving the user licenses to the new service, you can safely cancel the retired subscription at the top Customer level.</span></span>

### <a name="step-3---cancel-the-old-subscription"></a><span data-ttu-id="848b9-196">Etapa 3 - Cancelar a assinatura antiga</span><span class="sxs-lookup"><span data-stu-id="848b9-196">Step 3 - Cancel the old subscription</span></span>

1. <span data-ttu-id="848b9-197">No menu do **centro de parceiros** , selecione **clientes**.</span><span class="sxs-lookup"><span data-stu-id="848b9-197">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="848b9-198">Selecione o cliente que você deseja mover e selecione a assinatura que deseja cancelar.</span><span class="sxs-lookup"><span data-stu-id="848b9-198">Select the customer you want to move, and select the subscription you want to cancel.</span></span>

2. <span data-ttu-id="848b9-199">Na página detalhes da assinatura, defina o status da assinatura como **suspenso**.</span><span class="sxs-lookup"><span data-stu-id="848b9-199">In the subscription details page, set the subscription status to **Suspended**.</span></span>

3. <span data-ttu-id="848b9-200">Selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="848b9-200">Select **Submit**.</span></span>

<span data-ttu-id="848b9-201">A assinatura antiga será suspensa e a nova assinatura será ativada.</span><span class="sxs-lookup"><span data-stu-id="848b9-201">The old subscription is suspended and the new subscription is active.</span></span> <span data-ttu-id="848b9-202">A assinatura suspensa será desprovisionada automaticamente após 120 dias.</span><span class="sxs-lookup"><span data-stu-id="848b9-202">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="848b9-203">O cliente não pagará custos adicionais pela assinatura antiga.</span><span class="sxs-lookup"><span data-stu-id="848b9-203">The customer incurs no additional costs for the old subscription.</span></span>



 



