---
title: Criar assinaturas de cliente no Partner Center
ms.topic: how-to
ms.date: 07/22/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como vender suas assinaturas de clientes para produtos publicados pela Microsoft, bem como produtos de SaaS publicados por ISVs de terceiros.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 85a40974557817825d58246c2c010c7cf8a6a5e1
ms.sourcegitcommit: f34f2f69e6df4f260479a205d94010cf47987ff2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/25/2020
ms.locfileid: "96038873"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="d0499-103">Criar, suspender ou cancelar assinaturas de clientes</span><span class="sxs-lookup"><span data-stu-id="d0499-103">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="d0499-104">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="d0499-104">**Applies to**</span></span>

- <span data-ttu-id="d0499-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="d0499-105">Partner Center</span></span>
- <span data-ttu-id="d0499-106">Partner Center do Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="d0499-106">Partner Center for Microsoft Cloud for US Government</span></span>
- <span data-ttu-id="d0499-107">Parceiros CSP</span><span class="sxs-lookup"><span data-stu-id="d0499-107">CSP partners</span></span>

<span data-ttu-id="d0499-108">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="d0499-108">**Appropriate roles**</span></span>

- <span data-ttu-id="d0499-109">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="d0499-109">Admin agent</span></span>
- <span data-ttu-id="d0499-110">Administrador de cobrança</span><span class="sxs-lookup"><span data-stu-id="d0499-110">Billing admin</span></span>
- <span data-ttu-id="d0499-111">Administrador global</span><span class="sxs-lookup"><span data-stu-id="d0499-111">Global admin</span></span>
- <span data-ttu-id="d0499-112">Agente de suporte técnico</span><span class="sxs-lookup"><span data-stu-id="d0499-112">Helpdesk agent</span></span>
- <span data-ttu-id="d0499-113">Agente de vendas</span><span class="sxs-lookup"><span data-stu-id="d0499-113">Sales agent</span></span>

<span data-ttu-id="d0499-114">Depois de criar um registro de seu cliente no Partner Center, você pode vender as assinaturas para os produtos no catálogo.</span><span class="sxs-lookup"><span data-stu-id="d0499-114">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="d0499-115">Isso inclui produtos publicados pela Microsoft, bem como produtos SaaS (software como serviço) publicados por ISVs (fornecedores de software independentes) de terceiros no [mercado comercial](https://azuremarketplace.microsoft.com/marketplace).</span><span class="sxs-lookup"><span data-stu-id="d0499-115">This includes products published by Microsoft as well as Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="d0499-116">Algumas ofertas são limitadas a uma assinatura por cliente.</span><span class="sxs-lookup"><span data-stu-id="d0499-116">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="d0499-117">Para ver uma lista das ofertas restritas, visite a página Ofertas e Preços do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="d0499-117">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="d0499-118">Como um parceiro no programa CSP, você pode comprar assinaturas SaaS **limitadas** ou **baseadas em licença** de editores ISV no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="d0499-118">As a partner in the CSP program, you can purchase **license-based** or **metered** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="d0499-119">Isso significa que você pode comprar qualquer oferta de SaaS **limitada** ou **baseada em licença** que o editor ISV tenha disponibilizado para você, incluindo [ofertas exclusivas](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) às quais você tem acesso.</span><span class="sxs-lookup"><span data-stu-id="d0499-119">This means you can purchase any **license-based** or **metered** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="d0499-120">Para comprar ou gerenciar outras ofertas de Marketplace comercial de ISVs (como ofertas baseadas em uso que envolvem aplicativos, contêineres ou VMs do Azure), você deve ir para a [portal do Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="d0499-120">To purchase or manage other, commercial marketplace offers from ISVs (such as usage-based offers involving Azure applications, Containers or VMs), you must go to the [Azure portal](https://portal.azure.com/).</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="d0499-121">Criar uma nova assinatura</span><span class="sxs-lookup"><span data-stu-id="d0499-121">Create a new subscription</span></span>

1. <span data-ttu-id="d0499-122">Entre no painel [Partner Center](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="d0499-122">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="d0499-123">No menu do centro de parceiros, **selecione** clientes e, em seguida, escolha um cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="d0499-123">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="d0499-124">Selecione **Adicionar assinatura**.</span><span class="sxs-lookup"><span data-stu-id="d0499-124">Select **Add subscription**.</span></span> <span data-ttu-id="d0499-125">A guia **serviços online** mostrará todas as ofertas de SaaS do Marketplace disponíveis.</span><span class="sxs-lookup"><span data-stu-id="d0499-125">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="d0499-126">Para ver apenas determinados tipos de assinaturas, faça seleções nos filtros disponíveis:</span><span class="sxs-lookup"><span data-stu-id="d0499-126">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="d0499-127">**Publicador**: escolha a **Microsoft** para ver apenas as ofertas da Microsoft ou o **parceiro** para ver os produtos do Marketplace comercial publicados por ISVs.</span><span class="sxs-lookup"><span data-stu-id="d0499-127">**Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="d0499-128">**Tipo de cobrança**: selecione o tipo de cobrança de assinatura que você deseja usar: **licença** ou **uso**.</span><span class="sxs-lookup"><span data-stu-id="d0499-128">**Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="d0499-129">Consulte [cobrança baseada em licença](license-based-billing.md) para obter informações que o ajudarão a decidir entre a frequência de cobrança mensal e anual.</span><span class="sxs-lookup"><span data-stu-id="d0499-129">See [License-based billing](license-based-billing.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="d0499-130">**Categoria**: escolha **Enterprise**, **Small Business** ou **Trial**.</span><span class="sxs-lookup"><span data-stu-id="d0499-130">**Category**: Choose **Enterprise**, **Small business**, or **Trial**.</span></span> <span data-ttu-id="d0499-131">Para obter informações sobre assinaturas de avaliação, consulte [oferecer a seus clientes avaliações de produtos da Microsoft](offer-your-customers-trials-of-microsoft-products.md).</span><span class="sxs-lookup"><span data-stu-id="d0499-131">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="d0499-132">Selecione as assinaturas de produto que você deseja comprar para o cliente.</span><span class="sxs-lookup"><span data-stu-id="d0499-132">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="d0499-133">Os produtos que você vê dependem do tipo de segmento de cliente (educação, governo, etc.) e dos filtros que você aplicou.</span><span class="sxs-lookup"><span data-stu-id="d0499-133">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="d0499-134">Algumas ofertas mostradas no Marketplace talvez nem sempre estejam disponíveis para um cliente específico ou um parceiro CSP específico.</span><span class="sxs-lookup"><span data-stu-id="d0499-134">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="d0499-135">Isso pode ocorrer porque:</span><span class="sxs-lookup"><span data-stu-id="d0499-135">This can be because:</span></span>

   - <span data-ttu-id="d0499-136">O cliente já tem uma assinatura para esse produto e só é permitido um</span><span class="sxs-lookup"><span data-stu-id="d0499-136">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="d0499-137">A assinatura do cliente pode ter sido suspensa (nesse caso, você pode reativar a assinatura em vez de comprar uma nova).</span><span class="sxs-lookup"><span data-stu-id="d0499-137">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="d0499-138">Para ofertas de SaaS de ISV, pode haver alguns motivos pelos quais a oferta não está disponível para compra: o ISV pode não oferecer suporte ao país ou à região de cobrança do cliente; Talvez o ISV tenha optado por não disponibilizar a oferta por meio do programa CSP; ou, o ISV pode ter tornado a oferta [exclusiva](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) para apenas determinados parceiros CSP.</span><span class="sxs-lookup"><span data-stu-id="d0499-138">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="d0499-139">A oferta de ISV também pode não ser proficada por meio do Partner Center (por exemplo, contêineres ou algumas ofertas baseadas em uso).</span><span class="sxs-lookup"><span data-stu-id="d0499-139">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="d0499-140">Para cada assinatura que você deseja adicionar, insira o número de licenças (se necessário) e selecione **Adicionar ao carrinho**.</span><span class="sxs-lookup"><span data-stu-id="d0499-140">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="d0499-141">Quando terminar de adicionar assinaturas, selecione **revisar** e examine seu pedido.</span><span class="sxs-lookup"><span data-stu-id="d0499-141">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="d0499-142">Depois de revisar seus pedidos e estar pronto para comprar essas assinaturas, selecione **comprar**.</span><span class="sxs-lookup"><span data-stu-id="d0499-142">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="d0499-143">Depois de comprar uma assinatura para um cliente, ocorrerá o seguinte:</span><span class="sxs-lookup"><span data-stu-id="d0499-143">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="d0499-144">Você pode revisar ou editar a assinatura selecionando o nome da assinatura na página de **assinaturas** do cliente.</span><span class="sxs-lookup"><span data-stu-id="d0499-144">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="d0499-145">A partir daqui, você pode selecionar licenças de complemento, se houver alguma disponível, alterar a quantidade de licenças ou suspender a assinatura.</span><span class="sxs-lookup"><span data-stu-id="d0499-145">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="d0499-146">**Para assinaturas SaaS do ISV (baseadas em licença e limitadas):**</span><span class="sxs-lookup"><span data-stu-id="d0499-146">**For ISV SaaS (license-based and metered) subscriptions:**</span></span>
    - <span data-ttu-id="d0499-147">Você receberá um link para o site do fornecedor ISV.</span><span class="sxs-lookup"><span data-stu-id="d0499-147">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="d0499-148">Esse link deve ajudá-lo a concluir a configuração de implantação ou conta da assinatura do cliente.</span><span class="sxs-lookup"><span data-stu-id="d0499-148">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="d0499-149">Nem você nem seu cliente receberá um email com instruções para concluir a configuração/provisionamento de conta para esse tipo de assinatura de ISV.)</span><span class="sxs-lookup"><span data-stu-id="d0499-149">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="d0499-150">Se sua assinatura vier com uma avaliação gratuita de 30 dias, o período de avaliação gratuita será aplicado automaticamente.</span><span class="sxs-lookup"><span data-stu-id="d0499-150">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="d0499-151">Como um parceiro no programa CSP, não é possível renunciar ao período de avaliação gratuita em ofertas que você compra para os clientes.</span><span class="sxs-lookup"><span data-stu-id="d0499-151">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="d0499-152">Depois que o período de avaliação gratuita terminar, o prazo da assinatura será iniciado e a assinatura será convertida em status pago.</span><span class="sxs-lookup"><span data-stu-id="d0499-152">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="d0499-153">A assinatura será renovada automaticamente de acordo com a mesma agenda.</span><span class="sxs-lookup"><span data-stu-id="d0499-153">The subscription will then auto-renew according to the same schedule.</span></span>
   
## <a name="update-subscriptions-with-add-ons"></a><span data-ttu-id="d0499-154">Atualizar assinaturas com complementos</span><span class="sxs-lookup"><span data-stu-id="d0499-154">Update subscriptions with add-ons</span></span> 

<span data-ttu-id="d0499-155">Para comprar um complemento, o cliente precisará primeiro ter uma assinatura base ativa.</span><span class="sxs-lookup"><span data-stu-id="d0499-155">To purchase an add-on the customer must first have an active base subscription.</span></span>  <span data-ttu-id="d0499-156">Você não pode comprar complementos pelo catálogo.</span><span class="sxs-lookup"><span data-stu-id="d0499-156">You can't purchase add-ons through the catalog.</span></span>

1. <span data-ttu-id="d0499-157">Entre no [painel](https://partner.microsoft.com/dashboard) do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="d0499-157">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="d0499-158">No menu do centro de parceiros, **selecione** clientes e, em seguida, escolha um cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="d0499-158">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="d0499-159">Escolha a assinatura que deseja gerenciar.</span><span class="sxs-lookup"><span data-stu-id="d0499-159">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="d0499-160">Abaixo da seção **status** , há uma lista de Complementos disponíveis para a assinatura.</span><span class="sxs-lookup"><span data-stu-id="d0499-160">Below the **Status** section, are a list of available Add-ons for the subscription.</span></span>  

5. <span data-ttu-id="d0499-161">Atualize a quantidade de licenças para cada complemento necessário.</span><span class="sxs-lookup"><span data-stu-id="d0499-161">Update the quantity of licenses for each required Add-on.</span></span> <span data-ttu-id="d0499-162">**Envie** suas alterações.</span><span class="sxs-lookup"><span data-stu-id="d0499-162">Then **Submit** your changes.</span></span>

<span data-ttu-id="d0499-163">A capacidade de comprar Complementos por meio do Partner Center só está disponível para provedores diretos de fatura e indiretos.</span><span class="sxs-lookup"><span data-stu-id="d0499-163">The ability to purchase add-ons through Partner Center is only available to direct bill and indirect providers.</span></span>
<span data-ttu-id="d0499-164">Somente Complementos qualificados são exibidos com base nos requisitos básicos e na disponibilidade regional.</span><span class="sxs-lookup"><span data-stu-id="d0499-164">Only eligible add-ons are displayed based on the base requirements and regional availability.</span></span> <span data-ttu-id="d0499-165">Consulte a matriz de ofertas do revendedor de nuvem para mais informações sobre preços e ofertas.</span><span class="sxs-lookup"><span data-stu-id="d0499-165">Refer to the Cloud Reseller offer matrix for more information about pricing and offers.</span></span>  <span data-ttu-id="d0499-166">Suspender a assinatura base fará com que os complementos associados sejam suspensos.</span><span class="sxs-lookup"><span data-stu-id="d0499-166">Suspending the base subscription will also suspend any associated add-ons.</span></span>

<span data-ttu-id="d0499-167">As datas de início dos complementos estão alinhadas à assinatura base e as cobranças são calculadas da data de início à data de término de cobrança, com taxas proporcionais na primeira fatura.</span><span class="sxs-lookup"><span data-stu-id="d0499-167">Start dates for add-ons align to the base subscription and charges are calculated from the Charge start date and Charge end date with pro-rata charges in the first invoice.</span></span> <span data-ttu-id="d0499-168">Para obter informações adicionais, consulte [cobrança baseada em licença](license-based-billing.md).</span><span class="sxs-lookup"><span data-stu-id="d0499-168">For additional information see, [License-based billing](license-based-billing.md).</span></span>


## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="d0499-169">Suspender ou cancelar uma assinatura</span><span class="sxs-lookup"><span data-stu-id="d0499-169">Suspend or cancel a subscription</span></span>

<span data-ttu-id="d0499-170">Os parceiros podem suspender ou cancelar uma assinatura se solicitado pelo cliente ou em casos de fraude ou falta de pagamento.</span><span class="sxs-lookup"><span data-stu-id="d0499-170">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="d0499-171">Suspender uma assinatura</span><span class="sxs-lookup"><span data-stu-id="d0499-171">Suspend a subscription</span></span>

<span data-ttu-id="d0499-172">Quando você alterar o status de uma assinatura para **Suspensa**, os usuários não poderão entrar nem acessar os serviços.</span><span class="sxs-lookup"><span data-stu-id="d0499-172">When you change the status of a subscription to **Suspended**, users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="d0499-173">Entre no [painel](https://partner.microsoft.com/dashboard) do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="d0499-173">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="d0499-174">No menu do centro de parceiros, **selecione** clientes e, em seguida, escolha um cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="d0499-174">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="d0499-175">Escolha a assinatura que deseja gerenciar.</span><span class="sxs-lookup"><span data-stu-id="d0499-175">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="d0499-176">Na seção **Status**, escolha **Suspensa**.</span><span class="sxs-lookup"><span data-stu-id="d0499-176">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="d0499-177">**Envie** suas alterações.</span><span class="sxs-lookup"><span data-stu-id="d0499-177">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="d0499-178">Todos os dados serão excluídos, a menos que a assinatura seja reativada dentro de 90 dias ou 90 dias mais o número de dias entre a hora em que a conta foi aberta e o primeiro período de cobrança (máximo de 120 dias).</span><span class="sxs-lookup"><span data-stu-id="d0499-178">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="d0499-179">Quando você suspende uma assinatura, a data que você vê abaixo **do** botão suspenso indica quando a assinatura expirará automaticamente se você não a reativar.</span><span class="sxs-lookup"><span data-stu-id="d0499-179">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> 

### <a name="cancel-a-subscription"></a><span data-ttu-id="d0499-180">Cancelar uma assinatura</span><span class="sxs-lookup"><span data-stu-id="d0499-180">Cancel a subscription</span></span>

<span data-ttu-id="d0499-181">Você tem a opção de cancelar assinaturas de SaaS baseadas em licença de editores de ISVs de terceiros no [Marketplace comercial](csp-commercial-marketplace-overview.md)do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="d0499-181">You have the option to cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="d0499-182">Desde que você Cancele dentro do período de cancelamento, você receberá um reembolso total.</span><span class="sxs-lookup"><span data-stu-id="d0499-182">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="d0499-183">Para ofertas de ISV cobradas mensalmente:</span><span class="sxs-lookup"><span data-stu-id="d0499-183">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="d0499-184">Se você cancelar menos de 24 horas depois de colocar o pedido, receberá um crédito completo na próxima fatura.</span><span class="sxs-lookup"><span data-stu-id="d0499-184">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="d0499-185">Se você cancelar mais tarde que 24 horas depois de colocar o pedido, o cancelamento será agendado para ocorrer na renovação.</span><span class="sxs-lookup"><span data-stu-id="d0499-185">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="d0499-186">Para ofertas cobradas anualmente:</span><span class="sxs-lookup"><span data-stu-id="d0499-186">For offers billed annually:</span></span>

- <span data-ttu-id="d0499-187">Se você cancelar menos de 14 dias depois de fazer o pedido, receberá um crédito completo na próxima fatura.</span><span class="sxs-lookup"><span data-stu-id="d0499-187">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="d0499-188">Se você cancelar depois de 14 dias depois de fazer o pedido, o cancelamento será agendado para ocorrer na renovação.</span><span class="sxs-lookup"><span data-stu-id="d0499-188">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="d0499-189">Depois que esses períodos terminarem, você não verá mais a opção de cancelar a assinatura.</span><span class="sxs-lookup"><span data-stu-id="d0499-189">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="d0499-190">Os serviços ISV de terceiros baseados em uso e limitados (que usam máquinas virtuais ou contêineres, por exemplo) não são elegíveis para retorno.</span><span class="sxs-lookup"><span data-stu-id="d0499-190">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="d0499-191">Os serviços baseados em uso podem ser desprovisionados como um método de cancelamento.</span><span class="sxs-lookup"><span data-stu-id="d0499-191">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="d0499-192">Como os encargos são cobrados após o uso, esses serviços não são elegíveis para reembolso.</span><span class="sxs-lookup"><span data-stu-id="d0499-192">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="d0499-193">Para cancelar uma assinatura de SaaS baseada em licença de um publicador ISV, faça o seguinte:</span><span class="sxs-lookup"><span data-stu-id="d0499-193">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="d0499-194">Entre no [painel](https://partner.microsoft.com/dashboard) do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="d0499-194">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="d0499-195">No menu do centro de parceiros, **selecione** clientes e, em seguida, escolha um cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="d0499-195">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="d0499-196">Localize a assinatura que você deseja cancelar.</span><span class="sxs-lookup"><span data-stu-id="d0499-196">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="d0499-197">Na coluna **status** , selecione **Cancelar**.</span><span class="sxs-lookup"><span data-stu-id="d0499-197">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="d0499-198">**Envie** suas alterações.</span><span class="sxs-lookup"><span data-stu-id="d0499-198">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="d0499-199">Se uma caixa de diálogo for exibida, preencha todos os detalhes relevantes e selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="d0499-199">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="d0499-200">Para confirmar o cancelamento, selecione **Sim, cancelar**.</span><span class="sxs-lookup"><span data-stu-id="d0499-200">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="d0499-201">Você também pode optar por cancelar uma assinatura do Azure Marketplace usando APIs.</span><span class="sxs-lookup"><span data-stu-id="d0499-201">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="d0499-202">Para fazer isso, consulte [cancelar uma assinatura do Azure Marketplace](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span><span class="sxs-lookup"><span data-stu-id="d0499-202">To do so, see [Cancel an Azure Marketplace subscription](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="d0499-203">Escolha se deseja renovar automaticamente uma assinatura do Marketplace comercial</span><span class="sxs-lookup"><span data-stu-id="d0499-203">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="d0499-204">Por padrão, as assinaturas ativas são definidas para serem renovadas automaticamente ao término do período de assinatura.</span><span class="sxs-lookup"><span data-stu-id="d0499-204">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="d0499-205">Para [assinaturas para produtos do Marketplace comercial](csp-commercial-marketplace-overview.md), opcionalmente, você pode optar por não renovar automaticamente a assinatura.</span><span class="sxs-lookup"><span data-stu-id="d0499-205">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="d0499-206">Para interromper uma assinatura do Marketplace comercial ativa de renovar automaticamente:</span><span class="sxs-lookup"><span data-stu-id="d0499-206">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="d0499-207">Entre no [painel](https://partner.microsoft.com/dashboard) do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="d0499-207">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="d0499-208">No menu do centro de parceiros, **selecione** clientes e, em seguida, escolha um cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="d0499-208">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="d0499-209">Selecione **Assinaturas**.</span><span class="sxs-lookup"><span data-stu-id="d0499-209">Select **Subscriptions**.</span></span> <span data-ttu-id="d0499-210">Isso lista todas as assinaturas baseadas em licença que você comprou para o cliente.</span><span class="sxs-lookup"><span data-stu-id="d0499-210">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="d0499-211">Na coluna **assinatura** , selecione a assinatura que você deseja modificar.</span><span class="sxs-lookup"><span data-stu-id="d0499-211">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="d0499-212">Na página detalhes da assinatura, localize a seção **status** e desmarque a caixa **renovação automática** .</span><span class="sxs-lookup"><span data-stu-id="d0499-212">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="d0499-213">Selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="d0499-213">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d0499-214">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="d0499-214">Next steps</span></span>

- [<span data-ttu-id="d0499-215">Comprar produtos do Marketplace comercial para seus clientes</span><span class="sxs-lookup"><span data-stu-id="d0499-215">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="d0499-216">Gerenciar produtos do Marketplace comercial para seus clientes</span><span class="sxs-lookup"><span data-stu-id="d0499-216">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="d0499-217">Visão geral do marketplace comercial</span><span class="sxs-lookup"><span data-stu-id="d0499-217">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)