---
title: Alternar parceiro de cobrança direta para revendedor indireto
ms.topic: how-to
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como um parceiro do programa CSP pode usar o Partner Center para fazer a transição do parceiro Direct-Bill para o revendedor indireto.
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0e7676df62aa6ea91492f9904ac810397fb0e5aa
ms.sourcegitcommit: 35fe0fdc41886f6f5af71ec74e4a4ebd245dfe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2021
ms.locfileid: "104768747"
---
# <a name="transition-from-cloud-solution-provider-csp-direct-bill-partner-to-csp-indirect-reseller"></a><span data-ttu-id="ae892-103">Transição do parceiro de fatura direto do CSP (Provedor de Soluções na Nuvem) para o revendedor indireto do CSP</span><span class="sxs-lookup"><span data-stu-id="ae892-103">Transition from Cloud Solution Provider (CSP) direct bill partner to CSP indirect reseller</span></span>

<span data-ttu-id="ae892-104">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="ae892-104">**Appropriate roles**</span></span>

- <span data-ttu-id="ae892-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="ae892-105">Global admin</span></span>

>[!Note]
><span data-ttu-id="ae892-106">Este artigo destina-se a parceiros de cobrança direto que decidiram fazer a transição para revendedores indiretos.</span><span class="sxs-lookup"><span data-stu-id="ae892-106">This article is intended for direct bill partners who have decided to transition to indirect resellers.</span></span> <span data-ttu-id="ae892-107">No entanto, mesmo que você ainda não tenha feito uma decisão explícita para se registrar como um revendedor indireto, os parceiros de cobrança diretos que não atendem aos novos [requisitos](direct-partner-new-requirements.md) para o programa de parceiro de cobrança direto do CSP serão informados pela Microsoft quando seus [recursos de fatura direta serão restritos](restricted-direct-bill-capabilities.md).</span><span class="sxs-lookup"><span data-stu-id="ae892-107">However, even if you have not made an explicit decision yet to enroll as an indirect reseller, direct bill partners who do not meet the new [requirements](direct-partner-new-requirements.md) for the CSP direct bill partner program will be informed by Microsoft when their [direct bill capabilities will be restricted](restricted-direct-bill-capabilities.md).</span></span>
<br><span data-ttu-id="ae892-108">A partir de janeiro de 2021, um novo requisito de receita será adicionado.</span><span class="sxs-lookup"><span data-stu-id="ae892-108">As of January 2021, a new revenue requirement will be added.</span></span> <span data-ttu-id="ae892-109">Os parceiros registrados como um parceiro de cobrança direto precisarão ter transacionado pelo menos USD $300 mil na receita do programa do provedor de soluções na nuvem em um nível de conta global do parceiro nos 12 meses anteriores.</span><span class="sxs-lookup"><span data-stu-id="ae892-109">Partners enrolled as a direct bill partner will need to have transacted at least USD$300K in Cloud Solution Provider program revenue at a Partner Global Account level over the previous 12 months.</span></span>

<span data-ttu-id="ae892-110">Você poderá se registrar no programa revendedor indireto usando seu locatário de fatura direta existente.</span><span class="sxs-lookup"><span data-stu-id="ae892-110">You will be able to enroll in the indirect reseller program using your existing direct bill tenant.</span></span>

## <a name="get-started"></a><span data-ttu-id="ae892-111">Introdução</span><span class="sxs-lookup"><span data-stu-id="ae892-111">Get started</span></span>

1. <span data-ttu-id="ae892-112">Verifique se seu perfil de parceiro no Partner Center e na ID do MPN são atuais.</span><span class="sxs-lookup"><span data-stu-id="ae892-112">Make sure your partner profile in Partner Center and MPN ID are current.</span></span>

2. <span data-ttu-id="ae892-113">Entre no Partner Center como o administrador global do locatário de fatura direta que você está fazendo a transição para o revendedor indireto.</span><span class="sxs-lookup"><span data-stu-id="ae892-113">Sign in to Partner Center as the global admin for the direct bill tenant you are transitioning to indirect reseller.</span></span>

   :::image type="content" source="images/direct/direct1.png" alt-text="Visão geral":::

3. <span data-ttu-id="ae892-115">Examine os detalhes do parceiro no formulário de registro.</span><span class="sxs-lookup"><span data-stu-id="ae892-115">Review your partner details on the enrollment form.</span></span>

   :::image type="content" source="images/direct/direct2a.png" alt-text="Registre-se agora":::

4. <span data-ttu-id="ae892-117">Selecione Registrar agora.</span><span class="sxs-lookup"><span data-stu-id="ae892-117">Select Enroll now.</span></span> <span data-ttu-id="ae892-118">Seus negócios indiretos do revendedor usarão o mesmo locatário do AAD que você usa para seus negócios diretos.</span><span class="sxs-lookup"><span data-stu-id="ae892-118">Your indirect reseller business will use the same AAD tenant you use for your direct business.</span></span>

    > [!NOTE]
    > <span data-ttu-id="ae892-119">Inicialmente, esse novo recurso de transição estará disponível para parceiros com datas de setembro a dezembro.</span><span class="sxs-lookup"><span data-stu-id="ae892-119">Initially, this new transition capability will be available for partners with September to December anniversary dates.</span></span> <span data-ttu-id="ae892-120">Se você não tiver uma data de aniversário entre setembro e dezembro, você não verá a capacidade no momento.</span><span class="sxs-lookup"><span data-stu-id="ae892-120">If you don"t have an anniversary date between September and December, you won't see the capability at this time.</span></span> <span data-ttu-id="ae892-121">Os parceiros com datas de aniversário depois de dezembro de 2018 serão notificados mais tarde assim que o recurso for habilitado para os parceiros.</span><span class="sxs-lookup"><span data-stu-id="ae892-121">Partners with anniversary dates after December 2018 will be notified later once the feature is enabled for the partners.</span></span>

5. <span data-ttu-id="ae892-122">Quando seu registro for aprovado, entre no Partner Center novamente.</span><span class="sxs-lookup"><span data-stu-id="ae892-122">When your enrollment is approved, sign in to Partner Center again.</span></span>

    > [!NOTE]
    > <span data-ttu-id="ae892-123">Embora a aprovação seja normalmente imediata, pode levar até cinco dias úteis.</span><span class="sxs-lookup"><span data-stu-id="ae892-123">While approval is usually immediate, it can take up to five business days.</span></span> <span data-ttu-id="ae892-124">Depois de aprovado, você receberá uma notificação para o endereço de email especificado em contato principal no formulário de registro.</span><span class="sxs-lookup"><span data-stu-id="ae892-124">Once approved, you will receive a notification to the email address you have specified under primary contact in the enrollment form.</span></span> <span data-ttu-id="ae892-125">Você também pode verificar o status do registro em **configurações**  >  **conta configurações de contas**  >  **perfil do parceiro** > informações do programa.</span><span class="sxs-lookup"><span data-stu-id="ae892-125">You can also check your enrollment status under **Settings** > **Account Settings** > **Partner Profile** > Program info.</span></span>

6. <span data-ttu-id="ae892-126">Na página de **visão geral** , você verá o contrato de revendedor indireto.</span><span class="sxs-lookup"><span data-stu-id="ae892-126">On your **Overview** page, you will see the indirect reseller agreement.</span></span> <span data-ttu-id="ae892-127">Selecione **Aceitar e continuar**.</span><span class="sxs-lookup"><span data-stu-id="ae892-127">Select **Accept and continue**.</span></span> <span data-ttu-id="ae892-128">Essa ação habilita os recursos indiretos do revendedor.</span><span class="sxs-lookup"><span data-stu-id="ae892-128">This action enables the indirect reseller capabilities.</span></span>

<span data-ttu-id="ae892-129">Quando você tiver aceitado o contrato de revendedor indireto, observe que seu perfil **de parceiro identifica você como uma** fatura direta e um revendedor indireto.</span><span class="sxs-lookup"><span data-stu-id="ae892-129">When you have accepted the indirect reseller agreement, notice that your Partner profile identifies you as **both** a direct bill and indirect reseller.</span></span>

:::image type="content" source="images/direct/direct3.png" alt-text="Contrato de revendedor indireto":::

> [!IMPORTANT]
> <span data-ttu-id="ae892-131">Depois de se registrar como um revendedor indireto usando a nova funcionalidade, não há nenhuma opção para reverter para um locatário direto somente de cobrança.</span><span class="sxs-lookup"><span data-stu-id="ae892-131">Once you enroll as an indirect reseller using the new capability, there is no option to roll back to a direct bill- only tenant.</span></span> <span data-ttu-id="ae892-132">Certifique-se de avaliar totalmente suas necessidades de negócios antes de inscrever-se como um revendedor indireto.</span><span class="sxs-lookup"><span data-stu-id="ae892-132">Please make sure that you fully evaluate your business needs before enrolling as an indirect reseller.</span></span>

## <a name="while-you-transition-from-direct-to-indirect-reseller"></a><span data-ttu-id="ae892-133">Enquanto você faz a transição do revendedor direto para o indireto</span><span class="sxs-lookup"><span data-stu-id="ae892-133">While you transition from direct to indirect reseller</span></span>

<span data-ttu-id="ae892-134">Durante essa fase, você continuará a gerenciar as necessidades de assinatura direta de seus clientes, incluindo o processo de cobrança.</span><span class="sxs-lookup"><span data-stu-id="ae892-134">During this phase, you will continue to manage your direct customers' subscription needs including the billing process.</span></span> <span data-ttu-id="ae892-135">Você também pode começar a aceitar clientes do seu provedor indireto e operar como um revendedor indireto.</span><span class="sxs-lookup"><span data-stu-id="ae892-135">You can also begin accepting customers from your Indirect provider and operating as an indirect reseller.</span></span>

:::image type="content" source="images/direct/direct4.png" alt-text="Você é uma fatura direta e um revendedor indireto":::

## <a name="find-an-indirect-provider"></a><span data-ttu-id="ae892-137">Localizar um provedor indireto</span><span class="sxs-lookup"><span data-stu-id="ae892-137">Find an indirect provider</span></span>

<span data-ttu-id="ae892-138">Após o registro, um link para provedores indiretos será exibido na sua barra de navegação à esquerda.</span><span class="sxs-lookup"><span data-stu-id="ae892-138">After enrolling, a link to Indirect providers will appear in your left nav.</span></span> <span data-ttu-id="ae892-139">Como um revendedor indireto, você estabelecerá uma relação com um provedor indireto que pode manipular sua cobrança, comprar produtos para seus clientes e oferecer suporte à infraestrutura.</span><span class="sxs-lookup"><span data-stu-id="ae892-139">As an indirect reseller you will establish a relationship with an indirect provider who then can handle your billing, purchase products for your customers, and support infrastructure.</span></span>

<span data-ttu-id="ae892-140">Diferentes provedores indiretos oferecem suporte e serviços diferentes, portanto, você deve avaliar os provedores na sua região para determinar quais deles atendem melhor às suas necessidades.</span><span class="sxs-lookup"><span data-stu-id="ae892-140">Different indirect providers offer different support and services, so you should evaluate the providers in your area to determine which ones best meet your needs.</span></span> <span data-ttu-id="ae892-141">Em geral, a maioria dos provedores irá:</span><span class="sxs-lookup"><span data-stu-id="ae892-141">Generally, most providers will:</span></span>

- <span data-ttu-id="ae892-142">Fornecer treinamento e assistência técnica</span><span class="sxs-lookup"><span data-stu-id="ae892-142">Provide you with technical training and assistance</span></span>
- <span data-ttu-id="ae892-143">Ajudar a comercializar seus produtos e serviços</span><span class="sxs-lookup"><span data-stu-id="ae892-143">Help you market your products and services</span></span>
- <span data-ttu-id="ae892-144">Gerenciar seus termos de financiamento e crédito</span><span class="sxs-lookup"><span data-stu-id="ae892-144">Manage your financing and credit terms</span></span>

<span data-ttu-id="ae892-145">Pesquise a lista de [provedores indiretos](https://partnercenter.microsoft.com/partner/find-a-provider)oficiais da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ae892-145">Search the list of official [Microsoft indirect providers](https://partnercenter.microsoft.com/partner/find-a-provider).</span></span>

<span data-ttu-id="ae892-146">Saiba mais,  [parceiro de leitura com provedores indiretos](indirect-reseller-tasks-in-partner-center.md)</span><span class="sxs-lookup"><span data-stu-id="ae892-146">Learn more, read  [Partner with indirect providers](indirect-reseller-tasks-in-partner-center.md)</span></span>

## <a name="accept-a-partnership-invitation-from-your-indirect-provider"></a><span data-ttu-id="ae892-147">Aceitar um convite de parceria do seu provedor indireto</span><span class="sxs-lookup"><span data-stu-id="ae892-147">Accept a partnership invitation from your indirect provider</span></span>

<span data-ttu-id="ae892-148">Quando você encontrar um provedor indireto para parceria com o, estabeleça uma parceria com o provedor indireto no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="ae892-148">When you find an indirect provider to partner with, establish a partnership with the indirect provider in Partner Center.</span></span>

<span data-ttu-id="ae892-149">O provedor indireto que você selecionar enviará por email um link de convite de parceria que levará você ao seu convite no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="ae892-149">The indirect provider you select will send you in email a partnership invitation link that will take you to their invitation in Partner Center.</span></span> <span data-ttu-id="ae892-150">Verifique se o administrador global entra no Partner Center e segue o link de convite.</span><span class="sxs-lookup"><span data-stu-id="ae892-150">Be sure your global admin signs in to Partner Center and follows the invitation link.</span></span> <span data-ttu-id="ae892-151">Quando você aceitar o convite, o nome do provedor será exibido na sua lista de provedores indiretos.</span><span class="sxs-lookup"><span data-stu-id="ae892-151">When you accept the invitation, the provider's name will appear in your indirect provider list.</span></span>

## <a name="acquire-new-customers-as-indirect-reseller"></a><span data-ttu-id="ae892-152">Adquirir novos clientes como revendedor indireto</span><span class="sxs-lookup"><span data-stu-id="ae892-152">Acquire new customers as indirect reseller</span></span>

<span data-ttu-id="ae892-153">Você e seu provedor indireto precisam ter relações com os revendedores com os clientes.</span><span class="sxs-lookup"><span data-stu-id="ae892-153">Both you and your indirect provider need to have reseller relationships with customers.</span></span> <span data-ttu-id="ae892-154">Essas relações de revendedor permitem que você gerencie assinaturas e serviços de um cliente em seu nome.</span><span class="sxs-lookup"><span data-stu-id="ae892-154">These reseller relationships enable you to manage a customer's subscriptions and services on their behalf.</span></span> <span data-ttu-id="ae892-155">Para adquirir um novo cliente que tenha um locatário existente do Azure AD, você pode convidar o cliente para estabelecer uma relação de revendedor com você e seu provedor ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="ae892-155">To acquire a new customer who has an existing Azure AD tenant, you can invite the customer to establish a reseller relationship with both you and your provider at the same time.</span></span>

<span data-ttu-id="ae892-156">Para criar um convite de revendedor indireto:</span><span class="sxs-lookup"><span data-stu-id="ae892-156">To create an indirect reseller invitation:</span></span>

1. <span data-ttu-id="ae892-157">Selecione **provedores indiretos** na barra de navegação à esquerda do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="ae892-157">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="ae892-158">Selecione **Convidar novos clientes** para convidar um cliente a estabelecer uma relação de revendedor com você e a provedor indireto ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="ae892-158">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="ae892-159">O provedor precisa ter uma relação de revendedor com seu cliente, para que possa enviar pedidos em nome do seu cliente quando o cliente quiser comprar novas assinaturas ou adicionar novas licenças a assinaturas existentes.</span><span class="sxs-lookup"><span data-stu-id="ae892-159">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

3. <span data-ttu-id="ae892-160">Na próxima página, reveja o rascunho da mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="ae892-160">On the next page, review the draft email message.</span></span> <span data-ttu-id="ae892-161">Você pode abrir a mensagem de rascunho no email ou pode copiar a mensagem para a área de transferência e colá-la em um email.</span><span class="sxs-lookup"><span data-stu-id="ae892-161">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="ae892-162">Edite o texto no email para dizer o que você precisa, mas certifique-se de incluir o link como ele é personalizado para conectar o cliente diretamente à sua conta e à conta do provedor.</span><span class="sxs-lookup"><span data-stu-id="ae892-162">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="ae892-163">Em seguida, selecione **Concluído**.</span><span class="sxs-lookup"><span data-stu-id="ae892-163">Then select **Done**.</span></span>

5. <span data-ttu-id="ae892-164">Depois que o cliente autorizar você e seu provedor a ser seus revendedores de registro, você terá permissões de administrador para gerenciar as assinaturas, as licenças e os usuários em nome dele e seu provedor indireto será capaz de enviar pedidos em nome dele.</span><span class="sxs-lookup"><span data-stu-id="ae892-164">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>
6. <span data-ttu-id="ae892-165">Para gerenciar a conta, os serviços, os usuários e as licenças do cliente, expanda o registro do cliente selecionando a seta para baixo perto do nome dele.</span><span class="sxs-lookup"><span data-stu-id="ae892-165">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

<span data-ttu-id="ae892-166">Ao contrário dos parceiros de cobrança direto, os revendedores indiretos não podem criar locatários do Azure AD para seus novos clientes no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="ae892-166">Unlike direct bill partners, indirect resellers can't create Azure AD tenants for their new customers in Partner Center.</span></span> <span data-ttu-id="ae892-167">Seu provedor criará o locatário e especificará você como o revendedor indireto para esse cliente.</span><span class="sxs-lookup"><span data-stu-id="ae892-167">Your provider will create the tenant and will specify you as the indirect reseller for this customer.</span></span> <span data-ttu-id="ae892-168">Isso garante que o cliente será exibido na sua lista de clientes no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="ae892-168">This ensures that the customer will appear in your customer list in Partner Center.</span></span>

>[!Note]
><span data-ttu-id="ae892-169">Você não poderá usar sua capacidade de fatura direta para criar compras para os clientes adquiridos como um revendedor indireto.</span><span class="sxs-lookup"><span data-stu-id="ae892-169">You will not be able to use your direct bill capability to create purchases for customers you acquire as an indirect reseller.</span></span>

## <a name="managing-your-direct-bill-customers-and-your-indirect-reseller-customers"></a><span data-ttu-id="ae892-170">Gerenciando seus clientes de cobrança direta e seus clientes indiretos do revendedor</span><span class="sxs-lookup"><span data-stu-id="ae892-170">Managing your direct bill customers and your indirect reseller customers</span></span>

<span data-ttu-id="ae892-171">Você gerencia seus clientes de fatura direta e seus clientes de revendedores indiretos de forma diferente.</span><span class="sxs-lookup"><span data-stu-id="ae892-171">You manage your direct bill customers and your indirect reseller customers differently.</span></span>

### <a name="direct-bill-customers-things-you-wont-do-as-an-indirect-reseller"></a><span data-ttu-id="ae892-172">Clientes diretos de cobrança (coisas que você não fará como um revendedor indireto)</span><span class="sxs-lookup"><span data-stu-id="ae892-172">Direct bill customers (things you won't do as an indirect reseller)</span></span>

- <span data-ttu-id="ae892-173">Criar pedidos para produtos</span><span class="sxs-lookup"><span data-stu-id="ae892-173">Create orders for products</span></span>
- <span data-ttu-id="ae892-174">Gerenciar reservas do Azure</span><span class="sxs-lookup"><span data-stu-id="ae892-174">Manage Azure reservations</span></span>
- <span data-ttu-id="ae892-175">Gerenciar o histórico de pedidos</span><span class="sxs-lookup"><span data-stu-id="ae892-175">Manage their order history</span></span>
- <span data-ttu-id="ae892-176">Comprar software</span><span class="sxs-lookup"><span data-stu-id="ae892-176">Purchase software</span></span>
- <span data-ttu-id="ae892-177">Cobrar os clientes diretamente</span><span class="sxs-lookup"><span data-stu-id="ae892-177">Bill customers directly</span></span>

### <a name="indirect-reseller-customers"></a><span data-ttu-id="ae892-178">Clientes indiretos do revendedor</span><span class="sxs-lookup"><span data-stu-id="ae892-178">Indirect reseller customers</span></span>

- <span data-ttu-id="ae892-179">Seu provedor indireto solicita produtos para seus clientes</span><span class="sxs-lookup"><span data-stu-id="ae892-179">Your indirect provider orders products for your customers</span></span>
- <span data-ttu-id="ae892-180">Gerenciar licenças e usuários dos clientes</span><span class="sxs-lookup"><span data-stu-id="ae892-180">Manage customers' licenses and users</span></span>
- <span data-ttu-id="ae892-181">Manipular renovações de assinatura</span><span class="sxs-lookup"><span data-stu-id="ae892-181">Handle subscription renewals</span></span>

### <a name="to-identify-customers-that-you-acquired-as-a-direct-bill-partner"></a><span data-ttu-id="ae892-182">Para identificar os clientes adquiridos como um parceiro de cobrança direto</span><span class="sxs-lookup"><span data-stu-id="ae892-182">To identify customers that you acquired as a direct bill partner</span></span>

1. <span data-ttu-id="ae892-183">Selecione **Clientes**.</span><span class="sxs-lookup"><span data-stu-id="ae892-183">Select **Customers**.</span></span>

2. <span data-ttu-id="ae892-184">Selecione um cliente para exibir seus detalhes.</span><span class="sxs-lookup"><span data-stu-id="ae892-184">Select a customer to view their details.</span></span>

3. <span data-ttu-id="ae892-185">Se esse cliente for um adquirido como parceiro de cobrança direto, você verá opções para **Adicionar** ou **Exibir produtos** e verá suas assinaturas.</span><span class="sxs-lookup"><span data-stu-id="ae892-185">If this customer is one you acquired as a direct bill partner, you will see options to **add** or **view products** and you will see their subscriptions.</span></span>

4. <span data-ttu-id="ae892-186">Se o cliente tiver uma relação de revendedor indireta com você, essas opções não estarão disponíveis.</span><span class="sxs-lookup"><span data-stu-id="ae892-186">If the customer has an indirect reseller relationship with you, those options will not be available.</span></span>

## <a name="move-your-direct-bill-customers-to-your-indirect-provider"></a><span data-ttu-id="ae892-187">Mover seus clientes de fatura direta para seu provedor indireto</span><span class="sxs-lookup"><span data-stu-id="ae892-187">Move your direct bill customers to your indirect provider</span></span>

<span data-ttu-id="ae892-188">Seu provedor indireto não pode enviar pedidos ou transferências de assinatura existentes para seus clientes de fatura direta existentes até que eles tenham uma relação de revendedor com eles.</span><span class="sxs-lookup"><span data-stu-id="ae892-188">Your indirect provider cannot submit orders or existing subscription transfers for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="ae892-189">Para estabelecer a relação de revendedor entre seu provedor indireto e seu cliente de fatura direta existente, você pode usar um dos seguintes métodos:</span><span class="sxs-lookup"><span data-stu-id="ae892-189">To establish the reseller relationship between your indirect provider and your existing direct bill customer, you can use one of the following methods:</span></span>

- [<span data-ttu-id="ae892-190">Extensão de relacionamento do revendedor</span><span class="sxs-lookup"><span data-stu-id="ae892-190">Reseller relationship extension</span></span>](#reseller-relationship-extension)

- [<span data-ttu-id="ae892-191">Enviar um convite de revendedor indireto para o cliente</span><span class="sxs-lookup"><span data-stu-id="ae892-191">Send an indirect reseller invitation to the customer</span></span>](#send-an-indirect-reseller-invitation-to-the-customer)

<span data-ttu-id="ae892-192">Você pode encontrar uma visão geral detalhada do processo passo a passo no [documento de transição direto para indireta](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/)</span><span class="sxs-lookup"><span data-stu-id="ae892-192">You can find a detailed overview of the step-by-step process in the [Direct to indirect transition document](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/)</span></span>

### <a name="reseller-relationship-extension"></a><span data-ttu-id="ae892-193">Extensão de relacionamento do revendedor</span><span class="sxs-lookup"><span data-stu-id="ae892-193">Reseller relationship extension</span></span>

<span data-ttu-id="ae892-194">Você pode usar o recurso de extensão de relacionamento de revendedor para estabelecer a relação de revendedor entre seus clientes de fatura direta existentes e seu provedor indireto usando o painel do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="ae892-194">You can use the reseller relationship extension feature to establish reseller relationship between your existing direct bill customers and your indirect provider using Partner Center Dashboard.</span></span> <span data-ttu-id="ae892-195">Antes de usar o recurso, observe o seguinte:</span><span class="sxs-lookup"><span data-stu-id="ae892-195">Before using the feature, note the following:</span></span>

- <span data-ttu-id="ae892-196">Esse recurso está disponível apenas para os parceiros de cobrança diretos que estão em transição para se tornarem um revendedor indireto que concluiu o [registro indireto do revendedor](#get-started).</span><span class="sxs-lookup"><span data-stu-id="ae892-196">This feature is only available to direct bill partners who are transitioning to become an indirect reseller have completed the [indirect reseller enrollment](#get-started).</span></span>

- <span data-ttu-id="ae892-197">Você só pode aplicar esse recurso a clientes de fatura direta existentes.</span><span class="sxs-lookup"><span data-stu-id="ae892-197">You can only apply this feature to existing direct bill customers.</span></span> <span data-ttu-id="ae892-198">Ele não é aplicável a [clientes indiretos do revendedor](#acquire-new-customers-as-indirect-reseller).</span><span class="sxs-lookup"><span data-stu-id="ae892-198">It is not applicable to [indirect reseller customers](#acquire-new-customers-as-indirect-reseller).</span></span>

- <span data-ttu-id="ae892-199">Você só pode selecionar um provedor indireto para o qual [aceitou um convite de parceiro do seu provedor indireto](#accept-a-partnership-invitation-from-your-indirect-provider).</span><span class="sxs-lookup"><span data-stu-id="ae892-199">You can only select an indirect provider for which you have [accepted a partner invitation from your indirect provider](#accept-a-partnership-invitation-from-your-indirect-provider).</span></span>

- <span data-ttu-id="ae892-200">Uma cópia das informações de cobrança para esse cliente será disponibilizada para o provedor indireto.</span><span class="sxs-lookup"><span data-stu-id="ae892-200">A copy of the bill-to info you have for this customer will be made available to the indirect provider.</span></span> <span data-ttu-id="ae892-201">Você pode acessar as informações da fatura acessando a página conta para este cliente no painel do centro de parceiros.</span><span class="sxs-lookup"><span data-stu-id="ae892-201">You can access the bill-to info by accessing the Account page for this customer in Partner Center Dashboard.</span></span>

    > [!NOTE]
    > <span data-ttu-id="ae892-202">Usando o recurso de extensão de relacionamento de revendedor, você concorda em compartilhar as informações de cobrança para esse cliente com o provedor indireto.</span><span class="sxs-lookup"><span data-stu-id="ae892-202">By using the reseller relationship extension feature, you consent to sharing the bill-to info you have for this customer with the indirect provider.</span></span>

- <span data-ttu-id="ae892-203">Seu provedor indireto não será fornecido com [privilégios de administração delegados](customers-revoke-admin-privileges.md) para o locatário do cliente.</span><span class="sxs-lookup"><span data-stu-id="ae892-203">Your indirect provider will not be provided with [delegated administration privileges](customers-revoke-admin-privileges.md) to the customer tenant.</span></span> <span data-ttu-id="ae892-204">Se o seu provedor indireto exigir privilégios de administração delegada, você deverá enviar um convite de revendedor indireto para o cliente em vez disso.</span><span class="sxs-lookup"><span data-stu-id="ae892-204">If your indirect provider requires delegated administration privileges, you must send an indirect reseller invitation to the customer instead.</span></span>

- <span data-ttu-id="ae892-205">Depois que a relação do revendedor for estabelecida, o provedor indireto será exibido como um parceiro CSP para o cliente na página relações de parceiro no [centro de administração Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/partners) e [Microsoft Store para empresas](/microsoft-store/work-with-partner-microsoft-store-business).</span><span class="sxs-lookup"><span data-stu-id="ae892-205">Once the reseller relationship is established, the indirect provider will appear as a CSP partner to the customer under the Partner Relationships page in [Microsoft 365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/partners) and [Microsoft Store for Business](/microsoft-store/work-with-partner-microsoft-store-business).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="ae892-206">Para evitar confusão e mal-entendido, você está contratualmente obrigado pelo seu contrato de parceiro para informar e obter consentimento do cliente de fatura direta antes de usar o recurso de extensão de relacionamento para estabelecer a relação de revendedor entre um cliente de fatura direto existente e um provedor indireto.</span><span class="sxs-lookup"><span data-stu-id="ae892-206">To avoid confusion and misunderstanding, you are contractually obliged by your partner agreement to inform and obtain consent from the direct bill customer before you use the relationship extension feature to establish reseller relationship between an existing direct bill customer and an indirect provider.</span></span>

<span data-ttu-id="ae892-207">Para usar esse recurso em um locatário do cliente existente:</span><span class="sxs-lookup"><span data-stu-id="ae892-207">To use this feature on an existing customer tenant:</span></span>

1. <span data-ttu-id="ae892-208">Faça logon no Partner Center como um **agente de administração**.</span><span class="sxs-lookup"><span data-stu-id="ae892-208">Log in to Partner Center as an **Admin Agent**.</span></span>

2. <span data-ttu-id="ae892-209">Na **página clientes**, selecione um cliente existente e clique no ícone **links rápidos** para expandir a exibição de resumo do cliente.</span><span class="sxs-lookup"><span data-stu-id="ae892-209">In the **Customers page**, select an existing customer and click on its **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="ae892-210">Em **provedor (es) indireto (s)**, clique em **transferir cliente em um provedor indireto**.</span><span class="sxs-lookup"><span data-stu-id="ae892-210">Under **Indirect provider(s)**, click **Transfer customer on an indirect provider**.</span></span>

    :::image type="content" source="images/direct/direct5-1.png" alt-text="Transferir cliente para um provedor indireto":::

4. <span data-ttu-id="ae892-212">Na caixa de diálogo pop-up, selecione o **provedor indireto** que você gostaria de ter uma relação de revendedor com o cliente.</span><span class="sxs-lookup"><span data-stu-id="ae892-212">In the pop-up dialog, select the **Indirect Provider** you would like to have reseller relationship with the customer.</span></span>

5. <span data-ttu-id="ae892-213">Clique em **Salvar e continuar**.</span><span class="sxs-lookup"><span data-stu-id="ae892-213">Click **Save and continue**.</span></span>

6. <span data-ttu-id="ae892-214">Verifique se o provedor indireto selecionado aparece em **provedor (es) indireto (s)**.</span><span class="sxs-lookup"><span data-stu-id="ae892-214">Verify the selected indirect provider shows up under **Indirect provider(s)**.</span></span>

    :::image type="content" source="images/direct/direct5-2.png" alt-text="Provedor indireto listado":::

### <a name="send-an-indirect-reseller-invitation-to-the-customer"></a><span data-ttu-id="ae892-216">Enviar um convite de revendedor indireto para o cliente</span><span class="sxs-lookup"><span data-stu-id="ae892-216">Send an indirect reseller invitation to the customer</span></span>

<span data-ttu-id="ae892-217">Seu provedor indireto não pode enviar pedidos para seus clientes de fatura direta existentes até que eles tenham uma relação de revendedor com eles.</span><span class="sxs-lookup"><span data-stu-id="ae892-217">Your indirect provider cannot submit orders for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="ae892-218">Para estabelecer a relação de revendedor entre seus clientes existentes e seu provedor indireto, convide o cliente usando um convite de revendedor indireto.</span><span class="sxs-lookup"><span data-stu-id="ae892-218">To establish the reseller relationship between your existing customers and your indirect provider, invite the customer using an indirect reseller invitation.</span></span>

1. <span data-ttu-id="ae892-219">Selecione **provedores indiretos** na barra de navegação à esquerda do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="ae892-219">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="ae892-220">Selecione **Convidar novos clientes** para convidar um cliente a estabelecer uma relação de revendedor com você e a provedor indireto ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="ae892-220">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="ae892-221">O provedor precisa ter uma relação de revendedor com seu cliente, para que possa enviar pedidos em nome do seu cliente quando o cliente quiser comprar novas assinaturas ou adicionar novas licenças a assinaturas existentes.</span><span class="sxs-lookup"><span data-stu-id="ae892-221">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

    :::image type="content" source="images/direct/direct6.png" alt-text="Convide novos clientes":::

3. <span data-ttu-id="ae892-223">Na próxima página, reveja o rascunho da mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="ae892-223">On the next page, review the draft email message.</span></span> <span data-ttu-id="ae892-224">Você pode abrir a mensagem de rascunho no email ou pode copiar a mensagem para a área de transferência e colá-la em um email.</span><span class="sxs-lookup"><span data-stu-id="ae892-224">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="ae892-225">Edite o texto no email para dizer o que você precisa, mas certifique-se de incluir o link como ele é personalizado para conectar o cliente diretamente à sua conta e à conta do provedor.</span><span class="sxs-lookup"><span data-stu-id="ae892-225">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="ae892-226">Em seguida, selecione **Concluído**.</span><span class="sxs-lookup"><span data-stu-id="ae892-226">Then select **Done**.</span></span>

5. <span data-ttu-id="ae892-227">Depois que o cliente autorizar você e seu provedor a ser seus revendedores de registro, você terá permissões de administrador para gerenciar as assinaturas, as licenças e os usuários em nome dele e seu provedor indireto será capaz de enviar pedidos em nome dele.</span><span class="sxs-lookup"><span data-stu-id="ae892-227">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>

6. <span data-ttu-id="ae892-228">Para gerenciar a conta, os serviços, os usuários e as licenças do cliente, expanda o registro do cliente selecionando a seta para baixo perto do nome dele.</span><span class="sxs-lookup"><span data-stu-id="ae892-228">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

### <a name="microsoft-customer-agreement-acceptance"></a><span data-ttu-id="ae892-229">Aceitação do contrato com o cliente da Microsoft</span><span class="sxs-lookup"><span data-stu-id="ae892-229">Microsoft Customer Agreement acceptance</span></span>

<span data-ttu-id="ae892-230">Microsoft Cloud contrato é válido até 31 de janeiro de 2020.</span><span class="sxs-lookup"><span data-stu-id="ae892-230">Microsoft Cloud Agreement is valid until January 31, 2020.</span></span> <span data-ttu-id="ae892-231">Após essa data, todos os clientes, existentes e novos, devem assinar o novo [contrato do cliente da Microsoft](confirm-customer-agreement.md).</span><span class="sxs-lookup"><span data-stu-id="ae892-231">After that date, all customers, existing and new, must sign the new [Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span> <span data-ttu-id="ae892-232">Para a transição de clientes, se:</span><span class="sxs-lookup"><span data-stu-id="ae892-232">For transitioning customers, if:</span></span>

- <span data-ttu-id="ae892-233">**O cliente ainda não aceitou o contrato com o cliente da Microsoft**</span><span class="sxs-lookup"><span data-stu-id="ae892-233">**Customer has not accepted Microsoft Customer Agreement yet**</span></span>

   <span data-ttu-id="ae892-234">Trabalhe com o provedor indireto para que [o cliente aceite o contrato do cliente da Microsoft](confirm-customer-agreement.md).</span><span class="sxs-lookup"><span data-stu-id="ae892-234">Please work with Indirect Provider to have customer [accept the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

- <span data-ttu-id="ae892-235">**O cliente aceitou o contrato de clientes da Microsoft com você por meio do centro de administração Microsoft 365**</span><span class="sxs-lookup"><span data-stu-id="ae892-235">**Customer has accepted Microsoft Customer Agreement with you through the Microsoft 365 Admin Center**</span></span>

   <span data-ttu-id="ae892-236">A aceitação será retida quando a relação do revendedor for estabelecida com o provedor indireto.</span><span class="sxs-lookup"><span data-stu-id="ae892-236">The acceptance will be retained once the reseller relationship is established with the Indirect Provider.</span></span> <span data-ttu-id="ae892-237">Não há nada que você precise fazer.</span><span class="sxs-lookup"><span data-stu-id="ae892-237">There is nothing you need to do.</span></span>

- <span data-ttu-id="ae892-238">**O cliente aceitou o contrato de clientes da Microsoft com você por meio de atestado de parceiro**</span><span class="sxs-lookup"><span data-stu-id="ae892-238">**Customer has accepted Microsoft Customer Agreement with you through partner attestation**</span></span>

   <span data-ttu-id="ae892-239">A aceitação não será retida.</span><span class="sxs-lookup"><span data-stu-id="ae892-239">The acceptance will not be retained.</span></span> <span data-ttu-id="ae892-240">Trabalhe com o provedor indireto para [atualizar a aceitação do cliente no Partner Center](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers).</span><span class="sxs-lookup"><span data-stu-id="ae892-240">Please work with Indirect Provider to [update the customer's acceptance in Partner Center](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers).</span></span>

## <a name="transfer-existing-direct-bill-subscriptions-to-indirect-provider"></a><span data-ttu-id="ae892-241">Transferir inscrições de fatura direta existentes para o provedor indireto</span><span class="sxs-lookup"><span data-stu-id="ae892-241">Transfer existing direct bill subscriptions to indirect provider</span></span>

<span data-ttu-id="ae892-242">Em modelo indireto do CSP, revendedores indiretos não têm relações de cobrança com a Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ae892-242">Under CSP indirect model, indirect resellers do not have billing relationships with Microsoft.</span></span> <span data-ttu-id="ae892-243">Em vez disso, revendedores indiretos obtêm assinaturas para seus clientes por meio de seus provedores indiretos.</span><span class="sxs-lookup"><span data-stu-id="ae892-243">Instead, indirect resellers obtain subscriptions for their customers through their indirect providers.</span></span> <span data-ttu-id="ae892-244">Ao fazer a transição de um parceiro de cobrança direto para o revendedor indireto, você precisa transferir as assinaturas existentes que você tem como parceiro de cobrança direto para seu provedor indireto.</span><span class="sxs-lookup"><span data-stu-id="ae892-244">While transitioning from direct bill partner to indirect reseller, you need to transfer the existing subscriptions you have as the direct bill partner to your indirect provider.</span></span> <span data-ttu-id="ae892-245">Você pode usar o recurso de transferência de assinatura autoservido no painel do Partner Center para fazer isso.</span><span class="sxs-lookup"><span data-stu-id="ae892-245">You can use the self-served subscription transfer feature in Partner Center Dashboard to do so.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="ae892-246">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ae892-246">Prerequisites</span></span>

- <span data-ttu-id="ae892-247">Esse recurso só está disponível para a transição de parceiros que concluíram o registro indireto do revendedor usando seus locatários de parceiro de conta direta existentes.</span><span class="sxs-lookup"><span data-stu-id="ae892-247">This feature is only available to transitioning partners who have completed the indirect reseller enrollment using their existing direct bill partner tenants.</span></span>

- <span data-ttu-id="ae892-248">Antes de transferir assinaturas associadas a um determinado cliente, o parceiro de transição deve mover o cliente para um provedor indireto.</span><span class="sxs-lookup"><span data-stu-id="ae892-248">Before transferring subscriptions associated with a given customer, the transitioning partner must move the customer to an indirect provider.</span></span>

- <span data-ttu-id="ae892-249">O cliente deve ter [aceito o contrato com o cliente da Microsoft por meio do provedor indireto](#microsoft-customer-agreement-acceptance).</span><span class="sxs-lookup"><span data-stu-id="ae892-249">Customer must have [accepted Microsoft Customer Agreement through the Indirect Provider](#microsoft-customer-agreement-acceptance).</span></span>

### <a name="how-to-transition-to-indirect-reseller-status"></a><span data-ttu-id="ae892-250">Como fazer a transição para o status indireto do revendedor</span><span class="sxs-lookup"><span data-stu-id="ae892-250">How to transition to indirect reseller status</span></span>

<span data-ttu-id="ae892-251">O recurso é um processo de 4 etapas, em que:</span><span class="sxs-lookup"><span data-stu-id="ae892-251">The feature is a 4-step process, where:</span></span>

- <span data-ttu-id="ae892-252">O parceiro de transição cria uma solicitação de transferência de assinatura.</span><span class="sxs-lookup"><span data-stu-id="ae892-252">The transitioning partner creates a subscription transfer request.</span></span> <span data-ttu-id="ae892-253">A solicitação contém uma ou mais assinaturas existentes associadas ao mesmo cliente e é endereçada a um provedor indireto.</span><span class="sxs-lookup"><span data-stu-id="ae892-253">The request contains one or more existing subscriptions associated with the same customer and is addressed to an indirect provider.</span></span>

- <span data-ttu-id="ae892-254">O provedor indireto revisa e aceita (ou rejeita) a solicitação de transferência.</span><span class="sxs-lookup"><span data-stu-id="ae892-254">The indirect provider reviews and accepts (or reject) the transfer request.</span></span>

- <span data-ttu-id="ae892-255">O provedor indireto verifica se a solicitação de transferência foi concluída.</span><span class="sxs-lookup"><span data-stu-id="ae892-255">The indirect provider verifies that the transfer request is complete.</span></span>

- <span data-ttu-id="ae892-256">O parceiro de transição verifica se a solicitação de transferência foi concluída.</span><span class="sxs-lookup"><span data-stu-id="ae892-256">The transitioning partner verifies that the transfer request is complete.</span></span>

### <a name="transitioning-partner"></a><span data-ttu-id="ae892-257">Parceiro de transição</span><span class="sxs-lookup"><span data-stu-id="ae892-257">Transitioning partner</span></span>

> [!NOTE]
> <span data-ttu-id="ae892-258">Você também pode usar a [API/SDK do Partner Center](/partner-center/develop/manage-customers) para transferir as assinaturas existentes para seu provedor indireto.</span><span class="sxs-lookup"><span data-stu-id="ae892-258">You can also use [Partner Center API/SDK](/partner-center/develop/manage-customers) to transfer the existing subscriptions to your indirect provider.</span></span>
>
> - [<span data-ttu-id="ae892-259">Obter a qualificação de transferência de assinaturas de um cliente</span><span class="sxs-lookup"><span data-stu-id="ae892-259">Get a customer's subscriptions transfer eligibility</span></span>](/partner-center/develop/get-customer-s-subscriptions-transfer-eligibility)
> - [<span data-ttu-id="ae892-260">Criar a transferência de um cliente</span><span class="sxs-lookup"><span data-stu-id="ae892-260">Create a customer's transfer</span></span>](/partner-center/develop/create-a-transfer)
> - [<span data-ttu-id="ae892-261">Retirar a transferência de um cliente</span><span class="sxs-lookup"><span data-stu-id="ae892-261">Withdraw a customer's transfer</span></span>](/partner-center/develop/withdraw-a-transfer)
> - [<span data-ttu-id="ae892-262">Aceitar a transferência de um cliente</span><span class="sxs-lookup"><span data-stu-id="ae892-262">Accept a customer's transfer</span></span>](/partner-center/develop/accept-a-transfer)
> - [<span data-ttu-id="ae892-263">Rejeitar a transferência de um cliente</span><span class="sxs-lookup"><span data-stu-id="ae892-263">Reject a Customer's transfer</span></span>](/partner-center/develop/reject-a-transfer)
> - [<span data-ttu-id="ae892-264">Obter as transferências de um cliente</span><span class="sxs-lookup"><span data-stu-id="ae892-264">Get a customer's transfers</span></span>](/partner-center/develop/get-all-of-a-customer-s-transfers)
> - [<span data-ttu-id="ae892-265">Obter detalhes da transferência por ID</span><span class="sxs-lookup"><span data-stu-id="ae892-265">Get transfer details by id</span></span>](/partner-center/develop/get-transfer-by-id)

### <a name="transitioning-partner---create-transfer-request"></a><span data-ttu-id="ae892-266">Parceiro de transição – criar solicitação de transferência</span><span class="sxs-lookup"><span data-stu-id="ae892-266">Transitioning partner - create transfer request</span></span>

<span data-ttu-id="ae892-267">Para criar uma solicitação de transferência como o parceiro de transição:</span><span class="sxs-lookup"><span data-stu-id="ae892-267">To create a transfer request as the transitioning partner:</span></span>

1. <span data-ttu-id="ae892-268">Faça logon no Partner Center como um **agente de administração**.</span><span class="sxs-lookup"><span data-stu-id="ae892-268">Log in to Partner Center as an **Admin Agent**.</span></span>

2. <span data-ttu-id="ae892-269">Na página **clientes** , selecione o cliente desejado e clique no ícone links rápidos para expandir a exibição de resumo do cliente.</span><span class="sxs-lookup"><span data-stu-id="ae892-269">In the **Customers** page, select the intended customer and click on the Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="ae892-270">Em **provedor (es) indireto (s)**, confirme se o provedor indireto pretendido está listado.</span><span class="sxs-lookup"><span data-stu-id="ae892-270">Under **Indirect provider(s)**, confirm that the intended indirect provider is listed.</span></span>

4. <span data-ttu-id="ae892-271">Clique em **Exibir assinaturas**.</span><span class="sxs-lookup"><span data-stu-id="ae892-271">Click **View Subscriptions**.</span></span>

5. <span data-ttu-id="ae892-272">Na página **assinaturas** , procure **transferência de assinatura**.</span><span class="sxs-lookup"><span data-stu-id="ae892-272">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

6. <span data-ttu-id="ae892-273">Em **transferência de assinatura**, clique em **solicitar transferência de assinatura**.</span><span class="sxs-lookup"><span data-stu-id="ae892-273">Under **Subscription Transfer**, click **Request subscription transfer**.</span></span>

    :::image type="content" source="images/direct/direct8.png" alt-text="Solicitar transferência de assinatura":::

7. <span data-ttu-id="ae892-275">Na caixa de diálogo solicitação de transferência, selecione uma ou mais assinaturas a serem transferidas.</span><span class="sxs-lookup"><span data-stu-id="ae892-275">In the transfer request dialog, select one or more subscriptions to be transferred.</span></span>

    :::image type="content" source="images/direct/direct9.png" alt-text="Criar solicitação de transferência":::

8. <span data-ttu-id="ae892-277">Clique em **Criar**.</span><span class="sxs-lookup"><span data-stu-id="ae892-277">Click **Create**.</span></span>

9. <span data-ttu-id="ae892-278">Uma solicitação de transferência de assinatura ativa será exibida sob **transferência de assinatura**.</span><span class="sxs-lookup"><span data-stu-id="ae892-278">An active subscription transfer request will appear under **Subscription Transfer**.</span></span>

    :::image type="content" source="images/direct/direct10.png" alt-text="Transferir lista de solicitações":::

10. <span data-ttu-id="ae892-280">Informe ao seu provedor indireto que você criou uma solicitação de transferência de assinatura para eles.</span><span class="sxs-lookup"><span data-stu-id="ae892-280">Inform your indirect provider that you have created a subscription transfer request to them.</span></span>

### <a name="indirect-provider---accept-transfer-request"></a><span data-ttu-id="ae892-281">Provedor indireto-aceitar solicitação de transferência</span><span class="sxs-lookup"><span data-stu-id="ae892-281">Indirect provider - accept transfer request</span></span>

<span data-ttu-id="ae892-282">Para examinar e aceitar uma solicitação de transferência como o provedor indireto:</span><span class="sxs-lookup"><span data-stu-id="ae892-282">To review and accept a transfer request as the indirect provider:</span></span>

1. <span data-ttu-id="ae892-283">Faça logon no Partner Center como um agente de **Administração** ou **agente de vendas**.</span><span class="sxs-lookup"><span data-stu-id="ae892-283">Log in to Partner Center as an **Admin** Agent or **Sales Agent**.</span></span>

2. <span data-ttu-id="ae892-284">Na página **clientes** , selecione o cliente desejado e clique no ícone links rápidos para expandir a exibição de resumo do cliente.</span><span class="sxs-lookup"><span data-stu-id="ae892-284">In the **Customers** page, select the intended customer and click on its Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="ae892-285">Em **revendedor (es) indireto (s)**, confirme se o parceiro de transição está listado.</span><span class="sxs-lookup"><span data-stu-id="ae892-285">Under **Indirect reseller(s)**, confirm the transitioning partner is listed.</span></span>

4. <span data-ttu-id="ae892-286">Clique em **Exibir assinaturas**.</span><span class="sxs-lookup"><span data-stu-id="ae892-286">Click **View Subscriptions**.</span></span>

5. <span data-ttu-id="ae892-287">Na página **assinaturas** , procure **transferência de assinatura**.</span><span class="sxs-lookup"><span data-stu-id="ae892-287">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

    :::image type="content" source="images/direct/direct11.png" alt-text="Exibir solicitação de transferência":::

6. <span data-ttu-id="ae892-289">Em **transferência de assinatura**, clique na solicitação de transferência para revisar.</span><span class="sxs-lookup"><span data-stu-id="ae892-289">Under **Subscription Transfer**, click on the transfer request to review.</span></span>

7. <span data-ttu-id="ae892-290">Clique em **aceitar** (ou **rejeitar**) conforme apropriado.</span><span class="sxs-lookup"><span data-stu-id="ae892-290">Click **Accept** (or **Reject**) as appropriate.</span></span>

    :::image type="content" source="images/direct/direct12.png" alt-text="Aceitar solicitação de transferência":::

8. <span data-ttu-id="ae892-292">Aguarde a conclusão da solicitação de transferência.</span><span class="sxs-lookup"><span data-stu-id="ae892-292">Wait for the transfer request to complete.</span></span>

### <a name="indirect-provider---verify-transfer-request-is-complete"></a><span data-ttu-id="ae892-293">Provedor indireto-verificação de solicitação de transferência concluída</span><span class="sxs-lookup"><span data-stu-id="ae892-293">Indirect provider - verify transfer request is complete</span></span>

1. <span data-ttu-id="ae892-294">Depois que a solicitação de transferência for concluída com êxito, verifique se você pode ver que as assinaturas aparecem em **assinaturas**.</span><span class="sxs-lookup"><span data-stu-id="ae892-294">After the transfer request is completed successfully, verify that you can see the subscriptions appear under **Subscriptions**.</span></span>

2. <span data-ttu-id="ae892-295">Informe o parceiro de transição.</span><span class="sxs-lookup"><span data-stu-id="ae892-295">Inform the transitioning partner.</span></span>

### <a name="transitioning-partner---verify-transfer-request-is-complete"></a><span data-ttu-id="ae892-296">Parceiro em transição-a solicitação de transferência de verificação foi concluída</span><span class="sxs-lookup"><span data-stu-id="ae892-296">Transitioning partner - verify transfer request is complete</span></span>

<span data-ttu-id="ae892-297">O parceiro de transição deve fazer o seguinte:</span><span class="sxs-lookup"><span data-stu-id="ae892-297">The transitioning partner should do the following:</span></span>

1. <span data-ttu-id="ae892-298">Entre no Partner Center como um **agente de administração** ou **agente de vendas**.</span><span class="sxs-lookup"><span data-stu-id="ae892-298">Sign into Partner Center as an **Admin Agent** or **Sales Agent**.</span></span>

2. <span data-ttu-id="ae892-299">Na página **clientes** , selecione o cliente desejado e clique no ícone **links rápidos** para expandir a exibição de resumo do cliente.</span><span class="sxs-lookup"><span data-stu-id="ae892-299">In the **Customers** page, select the intended customer and click on the **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="ae892-300">Clique em **Exibir assinaturas**.</span><span class="sxs-lookup"><span data-stu-id="ae892-300">Click **View Subscriptions**.</span></span>

4. <span data-ttu-id="ae892-301">Na página **assinaturas** , procure **transferência de assinatura**.</span><span class="sxs-lookup"><span data-stu-id="ae892-301">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

5. <span data-ttu-id="ae892-302">Verifique se a solicitação de transferência está marcada como **concluída**.</span><span class="sxs-lookup"><span data-stu-id="ae892-302">Verify that the transfer request is marked as **Complete**.</span></span>

6. <span data-ttu-id="ae892-303">Verifique se as assinaturas não aparecem mais como ativas na página **assinaturas** :</span><span class="sxs-lookup"><span data-stu-id="ae892-303">Verify that the subscription(s) no longer appear as active in the **Subscriptions** page:</span></span>

   1. <span data-ttu-id="ae892-304">Se esta for uma assinatura do Azure (MS-AZR-0145P), ela não será mais listada.</span><span class="sxs-lookup"><span data-stu-id="ae892-304">If this is an Azure subscription (MS-AZR-0145P), it will no longer be listed.</span></span>

   2. <span data-ttu-id="ae892-305">Se esta for uma assinatura baseada em licença (Office 365, Dynamics, Intune), ela será listada com o estado como **suspenso**.</span><span class="sxs-lookup"><span data-stu-id="ae892-305">If this is a license-based subscription (Office 365, Dynamics, Intune), it will be listed with state as **Suspended**.</span></span>

   :::image type="content" source="images/direct/direct13.png" alt-text="Assinatura suspensa":::

### <a name="considerations"></a><span data-ttu-id="ae892-307">Considerações</span><span class="sxs-lookup"><span data-stu-id="ae892-307">Considerations</span></span>

- <span data-ttu-id="ae892-308">**A ID da assinatura será diferente após a transferência.**</span><span class="sxs-lookup"><span data-stu-id="ae892-308">**Subscription ID will be different after transfer.**</span></span> <span data-ttu-id="ae892-309">Se for uma assinatura do Azure (MS-AZR-0145P), além disso, ela terá uma ID de assinatura do Azure, que é retida do proprietário anterior e aparecerá no portal de gerenciamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="ae892-309">If it is an Azure subscription (MS-AZR-0145P), additionally, it will have an Azure Subscription ID, which is retained from the previous owner, and will appear in the Azure management portal.</span></span>

- <span data-ttu-id="ae892-310">**A mesma assinatura não pode ser referenciada por várias solicitações de transferência.**</span><span class="sxs-lookup"><span data-stu-id="ae892-310">**The same subscription cannot be referenced by multiple transfer requests.**</span></span> <span data-ttu-id="ae892-311">Depois de criar uma solicitação de transferência, que inclui uma assinatura existente, você não poderá criar solicitações de transferência adicionais, incluindo a mesma assinatura, até que a primeira solicitação de transferência seja cancelada.</span><span class="sxs-lookup"><span data-stu-id="ae892-311">After you have created a transfer request, which includes an existing subscription, you cannot create additional transfer requests including the same subscription, until the first transfer request is canceled.</span></span>

- <span data-ttu-id="ae892-312">**Os Complementos para assinaturas baseadas em licença devem ser transferidos junto com sua assinatura base.**</span><span class="sxs-lookup"><span data-stu-id="ae892-312">**Add-ons for license-based subscriptions must be transferred along with their base subscription.**</span></span> <span data-ttu-id="ae892-313">Ao criar uma solicitação de transferência, se você escolher uma assinatura existente com um ou mais Complementos, os complementos serão incluídos automaticamente na solicitação de transferência.</span><span class="sxs-lookup"><span data-stu-id="ae892-313">When creating a transfer request, if you pick an existing subscription with one or more add-ons, the add-ons will automatically be included in the transfer request.</span></span>

- <span data-ttu-id="ae892-314">**As alterações de contagem de licenças em uma assinatura não serão refletidas na solicitação de transferência existente.**</span><span class="sxs-lookup"><span data-stu-id="ae892-314">**License count changes to a subscription will not be reflected in existing transfer request.**</span></span> <span data-ttu-id="ae892-315">Depois de criar uma solicitação de transferência que inclui uma assinatura existente, você deve evitar atualizar a quantidade de licenças da assinatura (ou Complementos associados).</span><span class="sxs-lookup"><span data-stu-id="ae892-315">After you have created a transfer request which includes an existing subscription, you should avoid updating the license quantity of the subscription (or associated addons).</span></span> <span data-ttu-id="ae892-316">Se você fizer isso, a nova quantidade não será refletida na solicitação de transferência.</span><span class="sxs-lookup"><span data-stu-id="ae892-316">If you do so, the new quantity will not be reflected in the transfer request.</span></span> <span data-ttu-id="ae892-317">Depois que o provedor indireto aceitar a solicitação de transferência, a assinatura resultante terá a quantidade antiga.</span><span class="sxs-lookup"><span data-stu-id="ae892-317">After the indirect provider accepts the transfer request, the resultant subscription will have the old quantity.</span></span> <span data-ttu-id="ae892-318">Se desejar que a nova quantidade seja transferida para o provedor indireto, você deverá cancelar a solicitação de transferência existente e recriar uma nova.</span><span class="sxs-lookup"><span data-stu-id="ae892-318">If you wish for the new quantity to be transferred to the indirect provider, you must cancel the existing transfer request and recreate a new one.</span></span>

- <span data-ttu-id="ae892-319">**Nem todas as compras podem ser transferidas usando a transferência de assinatura autoatendida.**</span><span class="sxs-lookup"><span data-stu-id="ae892-319">**Not all purchases can be transferred using self-served subscription transfer.**</span></span> <span data-ttu-id="ae892-320">No momento, você só pode transferir assinaturas do O365 e assinaturas do Azure PAYG (MS-AZR-0145P) usando esse recurso.</span><span class="sxs-lookup"><span data-stu-id="ae892-320">Currently, you can only transfer O365 subscriptions and Azure PAYG subscriptions (MS-AZR-0145P) using this feature.</span></span> <span data-ttu-id="ae892-321">Não há suporte para outras compras, incluindo planos do Azure, instâncias reservadas do Azure, assinaturas baseadas em termos e assinaturas de SaaS para o Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="ae892-321">Other purchases including Azure Plans, Azure Reserved Instances, Term-based Subscriptions and SaaS subscriptions for Azure Marketplace are not supported.</span></span> <span data-ttu-id="ae892-322">Você verá um motivo pelo qual uma assinatura não pode ser transferida na página Enviar solicitação de transferência.</span><span class="sxs-lookup"><span data-stu-id="ae892-322">You will see a reason why a subscription cannot be transferred in the submit transfer request page.</span></span> <span data-ttu-id="ae892-323">Para transferir essas assinaturas, você precisará [cancelar a assinatura existente](create-a-new-subscription.md#suspend-or-cancel-a-subscription) e adquirir uma nova oferta para o cliente por meio do provedor indireto.</span><span class="sxs-lookup"><span data-stu-id="ae892-323">To transfer these subscriptions, you will need to [cancel the existing subscription](create-a-new-subscription.md#suspend-or-cancel-a-subscription) and purchase new offer for customer through Indirect Provider.</span></span>

- <span data-ttu-id="ae892-324">**Não é possível testar usando o ambiente de área restrita.**</span><span class="sxs-lookup"><span data-stu-id="ae892-324">**Cannot be tested using sandbox environment.**</span></span>

## <a name="enroll-for-indirect-reseller-incentives"></a><span data-ttu-id="ae892-325">Registrar-se para incentivos de revendedor indireto</span><span class="sxs-lookup"><span data-stu-id="ae892-325">Enroll for indirect reseller incentives</span></span>

<span data-ttu-id="ae892-326">Depois de ter registrado com êxito como um revendedor indireto em seu locatário de parceiro de cobrança direto existente, você receberá um convite para inscrever-se para o incentivo indireto do revendedor dentro de 30 dias.</span><span class="sxs-lookup"><span data-stu-id="ae892-326">After you have successfully enrolled as an indirect reseller on your existing direct bill partner tenant, you will receive an invitation to enroll for indirect reseller incentive within 30 days.</span></span> <span data-ttu-id="ae892-327">O convite é baseado na conta do Partner MPN que está associada no momento ao seu locatário do parceiro CSP.</span><span class="sxs-lookup"><span data-stu-id="ae892-327">The invitation is based on the partner MPN account that is currently associated with your CSP partner tenant.</span></span> <span data-ttu-id="ae892-328">O convite será enviado para o endereço de email associado à conta do parceiro MPN.</span><span class="sxs-lookup"><span data-stu-id="ae892-328">The invitation will be sent to the email address associated with the partner MPN account.</span></span>

<span data-ttu-id="ae892-329">Você também está qualificado para se inscrever em programas de incentivo de fatura direta com o mesmo locatário do parceiro.</span><span class="sxs-lookup"><span data-stu-id="ae892-329">You are also eligible to enroll for direct bill incentive programs with that same partner tenant.</span></span> <span data-ttu-id="ae892-330">Você deve gerenciar os programas separadamente.</span><span class="sxs-lookup"><span data-stu-id="ae892-330">You must manage the programs separately.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ae892-331">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="ae892-331">Next steps</span></span>

- [<span data-ttu-id="ae892-332">Mais informações sobre como se tornar um revendedor indireto</span><span class="sxs-lookup"><span data-stu-id="ae892-332">Additional information on becoming an indirect reseller</span></span>](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)
- [<span data-ttu-id="ae892-333">Novos requisitos do parceiro direto do CSP</span><span class="sxs-lookup"><span data-stu-id="ae892-333">CSP direct partner new requirements</span></span>](direct-partner-new-requirements.md)
- [<span data-ttu-id="ae892-334">Funcionalidades de fatura direta restritas</span><span class="sxs-lookup"><span data-stu-id="ae892-334">Restricted direct bill capabilities</span></span>](restricted-direct-bill-capabilities.md)
