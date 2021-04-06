---
title: Criar assinaturas de cliente no Partner Center
ms.topic: how-to
ms.date: 07/22/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como vender assinaturas para seus clientes para produtos publicados pela Microsoft, bem como produtos de SaaS publicados por ISVs de terceiros.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 559d1fbd2efc1417ae89931279b9d3c9a1d67f7c
ms.sourcegitcommit: 3d7d5064c5e021079ed7e6f93f03869cbf425a32
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/06/2021
ms.locfileid: "106502928"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="95373-103">Criar, suspender ou cancelar assinaturas de clientes</span><span class="sxs-lookup"><span data-stu-id="95373-103">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="95373-104">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="95373-104">**Applies to**</span></span>

- <span data-ttu-id="95373-105">Partner Center do Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="95373-105">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="95373-106">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="95373-106">**Appropriate roles**</span></span>

- <span data-ttu-id="95373-107">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="95373-107">Admin agent</span></span>
- <span data-ttu-id="95373-108">Administrador de cobrança</span><span class="sxs-lookup"><span data-stu-id="95373-108">Billing admin</span></span>
- <span data-ttu-id="95373-109">Administrador global</span><span class="sxs-lookup"><span data-stu-id="95373-109">Global admin</span></span>
- <span data-ttu-id="95373-110">Agente de suporte técnico</span><span class="sxs-lookup"><span data-stu-id="95373-110">Helpdesk agent</span></span>
- <span data-ttu-id="95373-111">Agente de vendas</span><span class="sxs-lookup"><span data-stu-id="95373-111">Sales agent</span></span>

<span data-ttu-id="95373-112">Depois de criar um registro de seu cliente no Partner Center, você pode vender as assinaturas para os produtos no catálogo.</span><span class="sxs-lookup"><span data-stu-id="95373-112">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="95373-113">Isso inclui produtos publicados pela Microsoft e por produtos SaaS (software como serviço) publicados por ISVs (fornecedores de software independentes) de terceiros no [mercado comercial](https://azuremarketplace.microsoft.com/marketplace).</span><span class="sxs-lookup"><span data-stu-id="95373-113">This includes products published by Microsoft and Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="95373-114">Algumas ofertas são limitadas a uma assinatura por cliente.</span><span class="sxs-lookup"><span data-stu-id="95373-114">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="95373-115">Para ver uma lista das ofertas restritas, visite a página Ofertas e Preços do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="95373-115">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="95373-116">Como um parceiro no programa CSP, você pode comprar assinaturas SaaS **limitadas** ou **baseadas em licença** de editores ISV no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="95373-116">As a partner in the CSP program, you can purchase **license-based** or **metered** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="95373-117">Isso significa que você pode comprar qualquer oferta de SaaS **limitada** ou **baseada em licença** que o editor ISV tenha disponibilizado para você, incluindo [ofertas exclusivas](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) às quais você tem acesso.</span><span class="sxs-lookup"><span data-stu-id="95373-117">This means you can purchase any **license-based** or **metered** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="95373-118">Para comprar ou gerenciar outras ofertas de Marketplace comercial de ISVs (como ofertas baseadas em uso que envolvem aplicativos, contêineres ou VMs do Azure), você deve ir para a [portal do Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="95373-118">To purchase or manage other, commercial marketplace offers from ISVs (such as usage-based offers involving Azure applications, Containers or VMs), you must go to the [Azure portal](https://portal.azure.com/).</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="95373-119">Criar uma nova assinatura</span><span class="sxs-lookup"><span data-stu-id="95373-119">Create a new subscription</span></span>

1. <span data-ttu-id="95373-120">Entre no painel [Partner Center](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="95373-120">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="95373-121">No menu do centro de parceiros, **selecione** clientes e, em seguida, escolha um cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="95373-121">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="95373-122">Selecione **Adicionar assinatura**.</span><span class="sxs-lookup"><span data-stu-id="95373-122">Select **Add subscription**.</span></span> <span data-ttu-id="95373-123">A guia **serviços online** mostrará todas as ofertas de SaaS do Marketplace disponíveis.</span><span class="sxs-lookup"><span data-stu-id="95373-123">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="95373-124">Para ver apenas determinados tipos de assinaturas, faça seleções nos filtros disponíveis:</span><span class="sxs-lookup"><span data-stu-id="95373-124">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="95373-125">**Publicador**: escolha a **Microsoft** para ver apenas as ofertas da Microsoft ou o **parceiro** para ver os produtos do Marketplace comercial publicados por ISVs.</span><span class="sxs-lookup"><span data-stu-id="95373-125">**Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="95373-126">**Tipo de cobrança**: selecione o tipo de cobrança de assinatura que você deseja usar: **licença** ou **uso**.</span><span class="sxs-lookup"><span data-stu-id="95373-126">**Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="95373-127">Consulte [cobrança baseada em licença](license-based-billing.md) para obter informações que o ajudarão a decidir entre a frequência de cobrança mensal e anual.</span><span class="sxs-lookup"><span data-stu-id="95373-127">See [License-based billing](license-based-billing.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="95373-128">**Categoria**: escolha **Enterprise**, **Small Business** ou **Trial**.</span><span class="sxs-lookup"><span data-stu-id="95373-128">**Category**: Choose **Enterprise**, **Small business**, or **Trial**.</span></span> <span data-ttu-id="95373-129">Para obter informações sobre assinaturas de avaliação, consulte [oferecer a seus clientes avaliações de produtos da Microsoft](offer-your-customers-trials-of-microsoft-products.md).</span><span class="sxs-lookup"><span data-stu-id="95373-129">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="95373-130">Selecione as assinaturas de produto que você deseja comprar para o cliente.</span><span class="sxs-lookup"><span data-stu-id="95373-130">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="95373-131">Os produtos que você vê dependem do tipo de segmento de cliente (educação, governo, etc.) e dos filtros que você aplicou.</span><span class="sxs-lookup"><span data-stu-id="95373-131">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="95373-132">Algumas ofertas mostradas no Marketplace talvez nem sempre estejam disponíveis para um cliente específico ou um parceiro CSP específico.</span><span class="sxs-lookup"><span data-stu-id="95373-132">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="95373-133">Isso pode ocorrer porque:</span><span class="sxs-lookup"><span data-stu-id="95373-133">This can be because:</span></span>

   - <span data-ttu-id="95373-134">O cliente já tem uma assinatura para esse produto e só é permitido um</span><span class="sxs-lookup"><span data-stu-id="95373-134">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="95373-135">A assinatura do cliente pode ter sido suspensa (nesse caso, você pode reativar a assinatura em vez de comprar uma nova).</span><span class="sxs-lookup"><span data-stu-id="95373-135">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="95373-136">Para ofertas de SaaS de ISV, pode haver alguns motivos pelos quais a oferta não está disponível para compra: o ISV pode não oferecer suporte ao país ou à região de cobrança do cliente; Talvez o ISV tenha optado por não disponibilizar a oferta por meio do programa CSP; ou, o ISV pode ter tornado a oferta [exclusiva](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) para apenas determinados parceiros CSP.</span><span class="sxs-lookup"><span data-stu-id="95373-136">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="95373-137">A oferta de ISV também pode não ser proficada por meio do Partner Center (por exemplo, contêineres ou algumas ofertas baseadas em uso).</span><span class="sxs-lookup"><span data-stu-id="95373-137">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="95373-138">Para cada assinatura que você deseja adicionar, insira o número de licenças (se necessário) e selecione **Adicionar ao carrinho**.</span><span class="sxs-lookup"><span data-stu-id="95373-138">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="95373-139">Quando terminar de adicionar assinaturas, selecione **revisar** e examine seu pedido.</span><span class="sxs-lookup"><span data-stu-id="95373-139">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="95373-140">Depois de revisar seus pedidos e estar pronto para comprar essas assinaturas, selecione **comprar**.</span><span class="sxs-lookup"><span data-stu-id="95373-140">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="95373-141">Depois de comprar uma assinatura para um cliente, ocorrerá o seguinte:</span><span class="sxs-lookup"><span data-stu-id="95373-141">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="95373-142">Você pode revisar ou editar a assinatura selecionando o nome da assinatura na página de **assinaturas** do cliente.</span><span class="sxs-lookup"><span data-stu-id="95373-142">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="95373-143">A partir daqui, você pode selecionar licenças de complemento, se houver alguma disponível, alterar a quantidade de licenças ou suspender a assinatura.</span><span class="sxs-lookup"><span data-stu-id="95373-143">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="95373-144">**Para assinaturas SaaS do ISV (baseadas em licença e limitadas):**</span><span class="sxs-lookup"><span data-stu-id="95373-144">**For ISV SaaS (license-based and metered) subscriptions:**</span></span>
    - <span data-ttu-id="95373-145">Você receberá um link para o site do fornecedor ISV.</span><span class="sxs-lookup"><span data-stu-id="95373-145">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="95373-146">Esse link deve ajudá-lo a concluir a configuração de implantação ou conta da assinatura do cliente.</span><span class="sxs-lookup"><span data-stu-id="95373-146">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="95373-147">Nem você nem seu cliente receberá um email com instruções para concluir a configuração/provisionamento de conta para esse tipo de assinatura de ISV.)</span><span class="sxs-lookup"><span data-stu-id="95373-147">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="95373-148">Se sua assinatura vier com uma avaliação gratuita de 30 dias, o período de avaliação gratuita será aplicado automaticamente.</span><span class="sxs-lookup"><span data-stu-id="95373-148">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="95373-149">Como um parceiro no programa CSP, não é possível renunciar ao período de avaliação gratuita em ofertas que você compra para os clientes.</span><span class="sxs-lookup"><span data-stu-id="95373-149">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="95373-150">Depois que o período de avaliação gratuita terminar, o prazo da assinatura será iniciado e a assinatura será convertida em status pago.</span><span class="sxs-lookup"><span data-stu-id="95373-150">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="95373-151">A assinatura será renovada automaticamente de acordo com a mesma agenda.</span><span class="sxs-lookup"><span data-stu-id="95373-151">The subscription will then auto-renew according to the same schedule.</span></span>
   
## <a name="update-subscriptions-with-add-ons"></a><span data-ttu-id="95373-152">Atualizar assinaturas com complementos</span><span class="sxs-lookup"><span data-stu-id="95373-152">Update subscriptions with add-ons</span></span> 

<span data-ttu-id="95373-153">Para comprar um complemento, o cliente deve primeiro ter uma assinatura base ativa.</span><span class="sxs-lookup"><span data-stu-id="95373-153">To purchase an add-on, the customer must first have an active base subscription.</span></span>  <span data-ttu-id="95373-154">Você não pode comprar complementos pelo catálogo.</span><span class="sxs-lookup"><span data-stu-id="95373-154">You can't purchase add-ons through the catalog.</span></span>

1. <span data-ttu-id="95373-155">Entre no [painel](https://partner.microsoft.com/dashboard) do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="95373-155">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="95373-156">No menu do centro de parceiros, **selecione** clientes e, em seguida, escolha um cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="95373-156">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="95373-157">Escolha a assinatura que deseja gerenciar.</span><span class="sxs-lookup"><span data-stu-id="95373-157">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="95373-158">Abaixo da seção **status** , há uma lista de Complementos disponíveis para a assinatura.</span><span class="sxs-lookup"><span data-stu-id="95373-158">Below the **Status** section, are a list of available Add-ons for the subscription.</span></span>  

5. <span data-ttu-id="95373-159">Atualize a quantidade de licenças para cada complemento necessário.</span><span class="sxs-lookup"><span data-stu-id="95373-159">Update the quantity of licenses for each required Add-on.</span></span> <span data-ttu-id="95373-160">**Envie** suas alterações.</span><span class="sxs-lookup"><span data-stu-id="95373-160">Then **Submit** your changes.</span></span>

<span data-ttu-id="95373-161">A capacidade de comprar Complementos por meio do Partner Center só está disponível para provedores diretos de fatura e indiretos.</span><span class="sxs-lookup"><span data-stu-id="95373-161">The ability to purchase add-ons through Partner Center is only available to direct bill and indirect providers.</span></span>
<span data-ttu-id="95373-162">Somente Complementos qualificados são exibidos com base nos requisitos básicos e na disponibilidade regional.</span><span class="sxs-lookup"><span data-stu-id="95373-162">Only eligible add-ons are displayed based on the base requirements and regional availability.</span></span> <span data-ttu-id="95373-163">Para obter mais informações sobre preços e ofertas, consulte a matriz de oferta de revendedor de nuvem.</span><span class="sxs-lookup"><span data-stu-id="95373-163">For more information about pricing and offers, refer to the Cloud Reseller offer matrix.</span></span> <span data-ttu-id="95373-164">Suspender a assinatura base fará com que os complementos associados sejam suspensos.</span><span class="sxs-lookup"><span data-stu-id="95373-164">Suspending the base subscription will also suspend any associated add-ons.</span></span>

<span data-ttu-id="95373-165">As datas de início dos complementos estão alinhadas à assinatura base e as cobranças são calculadas da data de início à data de término de cobrança, com taxas proporcionais na primeira fatura.</span><span class="sxs-lookup"><span data-stu-id="95373-165">Start dates for add-ons align to the base subscription and charges are calculated from the Charge start date and Charge end date with pro-rata charges in the first invoice.</span></span> <span data-ttu-id="95373-166">Para obter informações adicionais, consulte [cobrança baseada em licença](license-based-billing.md).</span><span class="sxs-lookup"><span data-stu-id="95373-166">For additional information see, [License-based billing](license-based-billing.md).</span></span>


## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="95373-167">Suspender ou cancelar uma assinatura</span><span class="sxs-lookup"><span data-stu-id="95373-167">Suspend or cancel a subscription</span></span>

<span data-ttu-id="95373-168">Os parceiros podem suspender ou cancelar uma assinatura se solicitado pelo cliente ou em casos de fraude ou falta de pagamento.</span><span class="sxs-lookup"><span data-stu-id="95373-168">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="95373-169">Suspender uma assinatura</span><span class="sxs-lookup"><span data-stu-id="95373-169">Suspend a subscription</span></span>

<span data-ttu-id="95373-170">Quando você alterar o status de uma assinatura para **Suspensa**, os usuários não poderão entrar nem acessar os serviços.</span><span class="sxs-lookup"><span data-stu-id="95373-170">When you change the status of a subscription to **Suspended**, users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="95373-171">Entre no [painel](https://partner.microsoft.com/dashboard) do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="95373-171">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="95373-172">No menu do centro de parceiros, **selecione** clientes e, em seguida, escolha um cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="95373-172">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="95373-173">Escolha a assinatura que deseja gerenciar.</span><span class="sxs-lookup"><span data-stu-id="95373-173">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="95373-174">Na seção **Status**, escolha **Suspensa**.</span><span class="sxs-lookup"><span data-stu-id="95373-174">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="95373-175">**Envie** suas alterações.</span><span class="sxs-lookup"><span data-stu-id="95373-175">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="95373-176">Todos os dados serão excluídos, a menos que a assinatura seja reativada dentro de 90 dias ou 90 dias mais o número de dias entre a hora em que a conta foi aberta e o primeiro período de cobrança (máximo de 120 dias).</span><span class="sxs-lookup"><span data-stu-id="95373-176">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="95373-177">Quando você suspende uma assinatura, a data que você vê abaixo **do** botão suspenso indica quando a assinatura expirará automaticamente se você não a reativar.</span><span class="sxs-lookup"><span data-stu-id="95373-177">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> 

### <a name="cancel-a-subscription"></a><span data-ttu-id="95373-178">Cancelar uma assinatura</span><span class="sxs-lookup"><span data-stu-id="95373-178">Cancel a subscription</span></span>

<span data-ttu-id="95373-179">Você pode cancelar assinaturas SaaS baseadas em licenças de editores de ISVs de terceiros no [Marketplace comercial](csp-commercial-marketplace-overview.md)do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="95373-179">You can cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="95373-180">Desde que você Cancele dentro do período de cancelamento, você receberá um reembolso total.</span><span class="sxs-lookup"><span data-stu-id="95373-180">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="95373-181">Para ofertas de ISV cobradas mensalmente:</span><span class="sxs-lookup"><span data-stu-id="95373-181">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="95373-182">Se você cancelar menos de 24 horas depois de colocar o pedido, receberá um crédito completo na próxima fatura.</span><span class="sxs-lookup"><span data-stu-id="95373-182">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="95373-183">Se você cancelar mais tarde que 24 horas depois de colocar o pedido, o cancelamento será agendado para ocorrer na renovação.</span><span class="sxs-lookup"><span data-stu-id="95373-183">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="95373-184">Para ofertas cobradas anualmente:</span><span class="sxs-lookup"><span data-stu-id="95373-184">For offers billed annually:</span></span>

- <span data-ttu-id="95373-185">Se você cancelar menos de 14 dias depois de fazer o pedido, receberá um crédito completo na próxima fatura.</span><span class="sxs-lookup"><span data-stu-id="95373-185">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="95373-186">Se você cancelar depois de 14 dias depois de fazer o pedido, o cancelamento será agendado para ocorrer na renovação.</span><span class="sxs-lookup"><span data-stu-id="95373-186">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="95373-187">Depois que esses períodos terminarem, você não verá mais a opção de cancelar a assinatura.</span><span class="sxs-lookup"><span data-stu-id="95373-187">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="95373-188">Os serviços ISV de terceiros baseados em uso e limitados (que usam máquinas virtuais ou contêineres, por exemplo) não são elegíveis para retorno.</span><span class="sxs-lookup"><span data-stu-id="95373-188">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="95373-189">Os serviços baseados em uso podem ser desprovisionados como um método de cancelamento.</span><span class="sxs-lookup"><span data-stu-id="95373-189">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="95373-190">Como os encargos são cobrados após o uso, esses serviços não são elegíveis para reembolso.</span><span class="sxs-lookup"><span data-stu-id="95373-190">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="95373-191">Para cancelar uma assinatura de SaaS baseada em licença de um publicador ISV, faça o seguinte:</span><span class="sxs-lookup"><span data-stu-id="95373-191">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="95373-192">Entre no [painel](https://partner.microsoft.com/dashboard) do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="95373-192">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="95373-193">No menu do centro de parceiros, **selecione** clientes e, em seguida, escolha um cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="95373-193">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="95373-194">Localize a assinatura que você deseja cancelar.</span><span class="sxs-lookup"><span data-stu-id="95373-194">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="95373-195">Na coluna **status** , selecione **Cancelar**.</span><span class="sxs-lookup"><span data-stu-id="95373-195">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="95373-196">**Envie** suas alterações.</span><span class="sxs-lookup"><span data-stu-id="95373-196">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="95373-197">Se uma caixa de diálogo for exibida, preencha todos os detalhes relevantes e selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="95373-197">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="95373-198">Para confirmar o cancelamento, selecione **Sim, cancelar**.</span><span class="sxs-lookup"><span data-stu-id="95373-198">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="95373-199">Você também pode optar por cancelar uma assinatura do Azure Marketplace usando APIs.</span><span class="sxs-lookup"><span data-stu-id="95373-199">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="95373-200">Para fazer isso, consulte [cancelar uma assinatura do Azure Marketplace](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span><span class="sxs-lookup"><span data-stu-id="95373-200">To do so, see [Cancel an Azure Marketplace subscription](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="95373-201">Escolha se deseja renovar automaticamente uma assinatura do Marketplace comercial</span><span class="sxs-lookup"><span data-stu-id="95373-201">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="95373-202">Por padrão, as assinaturas ativas são definidas para serem renovadas automaticamente ao término do período de assinatura.</span><span class="sxs-lookup"><span data-stu-id="95373-202">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="95373-203">Para [assinaturas para produtos do Marketplace comercial](csp-commercial-marketplace-overview.md), opcionalmente, você pode optar por não renovar automaticamente a assinatura.</span><span class="sxs-lookup"><span data-stu-id="95373-203">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="95373-204">Para interromper uma assinatura do Marketplace comercial ativa de renovar automaticamente:</span><span class="sxs-lookup"><span data-stu-id="95373-204">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="95373-205">Entre no [painel](https://partner.microsoft.com/dashboard) do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="95373-205">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="95373-206">No menu do centro de parceiros, **selecione** clientes e, em seguida, escolha um cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="95373-206">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="95373-207">Selecione **Assinaturas**.</span><span class="sxs-lookup"><span data-stu-id="95373-207">Select **Subscriptions**.</span></span> <span data-ttu-id="95373-208">Isso lista todas as assinaturas baseadas em licença que você comprou para o cliente.</span><span class="sxs-lookup"><span data-stu-id="95373-208">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="95373-209">Na coluna **assinatura** , selecione a assinatura que você deseja modificar.</span><span class="sxs-lookup"><span data-stu-id="95373-209">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="95373-210">Na página detalhes da assinatura, localize a seção **status** e desmarque a caixa **renovação automática** .</span><span class="sxs-lookup"><span data-stu-id="95373-210">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="95373-211">Selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="95373-211">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="95373-212">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="95373-212">Next steps</span></span>

- [<span data-ttu-id="95373-213">Comprar produtos do Marketplace comercial para seus clientes</span><span class="sxs-lookup"><span data-stu-id="95373-213">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="95373-214">Gerenciar produtos do Marketplace comercial para seus clientes</span><span class="sxs-lookup"><span data-stu-id="95373-214">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="95373-215">Visão geral do marketplace comercial</span><span class="sxs-lookup"><span data-stu-id="95373-215">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)