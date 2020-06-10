---
title: Migrar assinaturas do Kaizala pro para o Microsoft365
description: Saiba como migrar assinaturas do Kaizala pro para as versões do Microsoft365 ou do Office 365.
ms.topic: article
ms.service: partner-dashboard
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 842f4c0f88eec370821fa05c40cfadeee7fee12a
ms.sourcegitcommit: 8b7ef46a88aa5eb52ceefadfc5b0a06c3702d123
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/09/2020
ms.locfileid: "84611232"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft365-or-office-365-versions"></a><span data-ttu-id="d2fde-103">Migrar assinaturas autônomas do Kaizala pro para as versões do Microsoft365 ou do Office 365</span><span class="sxs-lookup"><span data-stu-id="d2fde-103">Migrate Kaizala Pro Standalone subscriptions to Microsoft365 or Office 365 versions</span></span>

<span data-ttu-id="d2fde-104">A partir de 1º de julho de 2020, a Microsoft está terminando as vendas do serviço autônomo do Kaizala pro.</span><span class="sxs-lookup"><span data-stu-id="d2fde-104">Effective July 1, 2020, Microsoft is ending sales of the Kaizala Pro standalone service.</span></span> <span data-ttu-id="d2fde-105">Os clientes não poderão mais comprar novas assinaturas do Kaizala pro após essa data, e as assinaturas existentes do Kaizala pro não serão renovadas automaticamente quando expirarem.</span><span class="sxs-lookup"><span data-stu-id="d2fde-105">Customers will no longer be able to purchase new Kaizala Pro subscriptions after this date, and existing Kaizala Pro subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="d2fde-106">Para garantir a continuidade dos clientes, você deve fazer a transição de clientes com assinaturas do Kaizala pro standalone expiradas para uma opção de SKU com suporte, listada abaixo.</span><span class="sxs-lookup"><span data-stu-id="d2fde-106">To ensure continuity for customers, you should transition customers with expiring Kaizala Pro standalone subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="d2fde-107">É recomendável mover os clientes para novas assinaturas antes da data de término anual da assinatura para evitar qualquer interrupção de serviço para os clientes.</span><span class="sxs-lookup"><span data-stu-id="d2fde-107">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="d2fde-108">Se você usar a API (CREST ou o Partner Center), poderá descobrir assinaturas expirando avaliando a data de término da assinatura junto com a propriedade de renovação automática definida como false: `auto renew = False` .</span><span class="sxs-lookup"><span data-stu-id="d2fde-108">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew property set to false: `auto renew = False`.</span></span>

<span data-ttu-id="d2fde-109">As assinaturas do E4 serão definidas `auto renew=False` em 1º de julho de 2020.</span><span class="sxs-lookup"><span data-stu-id="d2fde-109">The E4 subscriptions will be set to `auto renew=False` on July 1, 2020.</span></span> <span data-ttu-id="d2fde-110">Você pode mover os clientes para um novo plano a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="d2fde-110">You can move customers to a new plan at any time.</span></span>

## <a name="kaizala-pro-standalone-replacement-plans"></a><span data-ttu-id="d2fde-111">Planos de substituição autônomos do Kaizala pro</span><span class="sxs-lookup"><span data-stu-id="d2fde-111">Kaizala Pro Standalone replacement plans</span></span>

<span data-ttu-id="d2fde-112">Com os novos planos, os clientes podem aproveitar os recursos e as funcionalidades mais recentes no Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d2fde-112">With the new plans, your customers can take advantage of newer features and functionality in Microsoft 365.</span></span> <span data-ttu-id="d2fde-113">Detalhes de preço são encontrados na lista de preços e oferecem a matriz de lista no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="d2fde-113">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span>

- <span data-ttu-id="d2fde-114">[**Microsoft 365 para negócios**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), incluindo:</span><span class="sxs-lookup"><span data-stu-id="d2fde-114">[**Microsoft 365 for Business**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), including:</span></span>  
   - <span data-ttu-id="d2fde-115">Microsoft 365 Business Basic</span><span class="sxs-lookup"><span data-stu-id="d2fde-115">Microsoft 365 Business Basic</span></span>
   - <span data-ttu-id="d2fde-116">Padrão de Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="d2fde-116">Microsoft 365 Business Standard</span></span>
   - <span data-ttu-id="d2fde-117">Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="d2fde-117">Microsoft 365 Business Premium</span></span>
    
- <span data-ttu-id="d2fde-118">[**Microsoft 365 para frente**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), incluindo:</span><span class="sxs-lookup"><span data-stu-id="d2fde-118">[**Microsoft 365 for Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), including:</span></span>
   - <span data-ttu-id="d2fde-119">Microsoft 365 F3 (anteriormente Microsoft 365 F1) e Office 365 F3</span><span class="sxs-lookup"><span data-stu-id="d2fde-119">Microsoft 365 F3 (formerly Microsoft 365 F1) and Office 365 F3</span></span>
    
- <span data-ttu-id="d2fde-120">[**Microsoft 365 para empresas**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), incluindo:</span><span class="sxs-lookup"><span data-stu-id="d2fde-120">[**Microsoft 365 for Enterprise**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), including:</span></span> 
   - <span data-ttu-id="d2fde-121">Office 365 E1</span><span class="sxs-lookup"><span data-stu-id="d2fde-121">Office 365 E1</span></span>
   - <span data-ttu-id="d2fde-122">Microsoft 365 E3 e Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="d2fde-122">Microsoft 365 E3 and Office 365 E3</span></span>
   - <span data-ttu-id="d2fde-123">Microsoft 365 E5 e Office 365 e5</span><span class="sxs-lookup"><span data-stu-id="d2fde-123">Microsoft 365 E5 and Office 365 E5</span></span>

- <span data-ttu-id="d2fde-124">[**Microsoft 365 para educação**](https://www.microsoft.com/education/buy-license/microsoft365), incluindo:</span><span class="sxs-lookup"><span data-stu-id="d2fde-124">[**Microsoft 365 for Education**](https://www.microsoft.com/education/buy-license/microsoft365), including:</span></span> 
    - <span data-ttu-id="d2fde-125">Microsoft 365 a1 e Office 365 a1</span><span class="sxs-lookup"><span data-stu-id="d2fde-125">Microsoft 365 A1 and Office 365 A1</span></span>
    - <span data-ttu-id="d2fde-126">Microsoft 365 a3 e Office 365 a3</span><span class="sxs-lookup"><span data-stu-id="d2fde-126">Microsoft 365 A3 and Office 365 A3</span></span>
    - <span data-ttu-id="d2fde-127">Microsoft 365 a5 e Office 365 a5</span><span class="sxs-lookup"><span data-stu-id="d2fde-127">Microsoft 365 A5 and Office 365 A5</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="d2fde-128">Transição dos clientes para novos planos do produto</span><span class="sxs-lookup"><span data-stu-id="d2fde-128">Transition customers to new product plans</span></span>

<span data-ttu-id="d2fde-129">A Microsoft oferece continuamente novos produtos e serviços para nossos parceiros.</span><span class="sxs-lookup"><span data-stu-id="d2fde-129">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="d2fde-130">Nesses casos, você pode precisar fazer o upgrade dos clientes para novos serviços ou migrar as assinaturas de SKUs que serão encerradas em breve.</span><span class="sxs-lookup"><span data-stu-id="d2fde-130">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="d2fde-131">A migração dos clientes de SKUs desativadas para as mais recentes requer as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="d2fde-131">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

<span data-ttu-id="d2fde-132">A.</span><span class="sxs-lookup"><span data-stu-id="d2fde-132">A.</span></span> <span data-ttu-id="d2fde-133">Comprar a nova assinatura</span><span class="sxs-lookup"><span data-stu-id="d2fde-133">Purchase the new subscription</span></span>

<span data-ttu-id="d2fde-134">B.</span><span class="sxs-lookup"><span data-stu-id="d2fde-134">B.</span></span> <span data-ttu-id="d2fde-135">Reatribuir as licenças de usuário atuais</span><span class="sxs-lookup"><span data-stu-id="d2fde-135">Reassign current user licenses</span></span>

<span data-ttu-id="d2fde-136">C.</span><span class="sxs-lookup"><span data-stu-id="d2fde-136">C.</span></span> <span data-ttu-id="d2fde-137">Cancelar a assinatura antiga</span><span class="sxs-lookup"><span data-stu-id="d2fde-137">Cancel old subscription</span></span>


## <a name="migrate-your-customers-to-new-plans"></a><span data-ttu-id="d2fde-138">Migrar seus clientes para novos planos</span><span class="sxs-lookup"><span data-stu-id="d2fde-138">Migrate your customers to new plans</span></span>

### <a name="a-purchase-the-new-subscription"></a><span data-ttu-id="d2fde-139">A.</span><span class="sxs-lookup"><span data-stu-id="d2fde-139">A.</span></span> <span data-ttu-id="d2fde-140">Comprar a nova assinatura</span><span class="sxs-lookup"><span data-stu-id="d2fde-140">Purchase the new subscription</span></span>

1. <span data-ttu-id="d2fde-141">Para comprar a nova assinatura, no menu do **Partner Center** , selecione **clientes**, selecione o cliente que você deseja mover e, em seguida, selecione **adicionar assinaturas**.</span><span class="sxs-lookup"><span data-stu-id="d2fde-141">To purchase the new subscription, from the **Partner Center** menu, select **Customers**, select the customer you want to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="d2fde-142">Selecione a assinatura que deseja comprar no catálogo (nesse caso, uma das opções acima), insira o número de licenças e selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="d2fde-142">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

<span data-ttu-id="d2fde-143">Agora, o cliente deve ter assinaturas antigas e novas, a antiga assinatura autônoma do Kaizala pro e a nova assinatura de "destino", por exemplo, a opção 1-Office 365 Enterprise F1.</span><span class="sxs-lookup"><span data-stu-id="d2fde-143">Your customer should now have both old and new subscriptions, the old Kaizala Pro Standalone subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise F1.</span></span>

### <a name="b-reassign-current-user-licenses"></a><span data-ttu-id="d2fde-144">B.</span><span class="sxs-lookup"><span data-stu-id="d2fde-144">B.</span></span> <span data-ttu-id="d2fde-145">Reatribuir as licenças de usuário atuais</span><span class="sxs-lookup"><span data-stu-id="d2fde-145">Reassign current user licenses</span></span>

1. <span data-ttu-id="d2fde-146">Para reatribuir as licenças dos usuários do cliente, no menu do **centro de parceiros** , selecione **clientes**, selecione o cliente que você está movendo e, em seguida, selecione **usuários e licenças**.</span><span class="sxs-lookup"><span data-stu-id="d2fde-146">To reassign the customer's users' licenses, from the **Partner Center** menu, select **Customers**, select the customer you are moving, and then select **Users and licenses**.</span></span> <span data-ttu-id="d2fde-147">A página usuários e licenças do cliente é aberta.</span><span class="sxs-lookup"><span data-stu-id="d2fde-147">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="d2fde-148">Para reatribuir a licença de usuário, selecione o usuário a ser reatribuído e, em seguida, selecione **gerenciar licenças**.</span><span class="sxs-lookup"><span data-stu-id="d2fde-148">To reassign user license, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="d2fde-149">Na página **gerenciar licenças** , desmarque a caixa de seleção licença do Kaizala pro standalone e selecione um novo plano de serviço para a assinatura à qual o cliente está se movendo.</span><span class="sxs-lookup"><span data-stu-id="d2fde-149">On the **Manage licenses** page, clear the Kaizala Pro Standalone license check box, and select a new service plan for the subscription the customer is moving to.</span></span>

4.  <span data-ttu-id="d2fde-150">Selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="d2fde-150">Select **Submit**.</span></span> <span data-ttu-id="d2fde-151">Uma página de confirmação lista as novas atribuições de licença.</span><span class="sxs-lookup"><span data-stu-id="d2fde-151">A confirmation page lists the new license assignments.</span></span> <span data-ttu-id="d2fde-152">Continue esse mesmo processo para outros usuários que precisam de atribuições de licença.</span><span class="sxs-lookup"><span data-stu-id="d2fde-152">Continue this same process for other users who need license assignments.</span></span>

### <a name="c-cancel-old-subscription"></a><span data-ttu-id="d2fde-153">C.</span><span class="sxs-lookup"><span data-stu-id="d2fde-153">C.</span></span> <span data-ttu-id="d2fde-154">Cancelar a assinatura antiga</span><span class="sxs-lookup"><span data-stu-id="d2fde-154">Cancel old subscription</span></span>

<span data-ttu-id="d2fde-155">Depois de migrar a licença do usuário para o novo serviço, você pode cancelar com segurança a assinatura desativada no nível do cliente.</span><span class="sxs-lookup"><span data-stu-id="d2fde-155">After moving the user license to the new service, you can safely cancel the retired subscription at the customer level.</span></span>

1.  <span data-ttu-id="d2fde-156">No menu do **centro de parceiros** , selecione **clientes**.</span><span class="sxs-lookup"><span data-stu-id="d2fde-156">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="d2fde-157">Selecione o cliente cuja assinatura você está cancelando.</span><span class="sxs-lookup"><span data-stu-id="d2fde-157">Select the customer whose subscription you are canceling.</span></span>

2.  <span data-ttu-id="d2fde-158">Na página de detalhe da assinatura, defina o status da assinatura como **Suspensa**.</span><span class="sxs-lookup"><span data-stu-id="d2fde-158">In the subscription detail page, set the subscription to **Suspended**.</span></span>

3.  <span data-ttu-id="d2fde-159">Selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="d2fde-159">Select **Submit**.</span></span>

<span data-ttu-id="d2fde-160">A assinatura antiga será suspensa e a nova assinatura será ativada.</span><span class="sxs-lookup"><span data-stu-id="d2fde-160">The old subscription is suspended, and the new subscription is active.</span></span> <span data-ttu-id="d2fde-161">A assinatura suspensa será desprovisionada automaticamente após 120 dias.</span><span class="sxs-lookup"><span data-stu-id="d2fde-161">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="d2fde-162">O cliente não pagará custos adicionais pela assinatura antiga.</span><span class="sxs-lookup"><span data-stu-id="d2fde-162">The customer incurs no additional costs for the old subscription.</span></span>
