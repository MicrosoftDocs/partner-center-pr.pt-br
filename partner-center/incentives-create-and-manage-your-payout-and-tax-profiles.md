---
title: Perfis de pagamento e impostos no Partner Center
ms.topic: how-to
ms.date: 11/12/2020
description: Crie e gerencie seu pagamento e seu perfil de impostos para que você possa ser pago pelo trabalho de seus incentivos. Inclui a criação, o gerenciamento e o uso de perfis diferentes.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: 66177c6e3cd0091081866e1508d28346f49ec713
ms.sourcegitcommit: bfc9e6f6476766cf10ba714f03ca2e96560003b1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/14/2020
ms.locfileid: "94626024"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="8ae0c-104">Criar e gerenciar o pagamento de incentivos e perfis de impostos no Partner Center</span><span class="sxs-lookup"><span data-stu-id="8ae0c-104">Create and manage incentives payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="8ae0c-105">**Aplica-se a:**</span><span class="sxs-lookup"><span data-stu-id="8ae0c-105">**Applies to:**</span></span>

- <span data-ttu-id="8ae0c-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="8ae0c-106">Partner Center</span></span>

<span data-ttu-id="8ae0c-107">**Funções apropriadas:**</span><span class="sxs-lookup"><span data-stu-id="8ae0c-107">**Appropriate roles:**</span></span>

- <span data-ttu-id="8ae0c-108">Administrador de incentivos</span><span class="sxs-lookup"><span data-stu-id="8ae0c-108">Incentives admin</span></span>
- <span data-ttu-id="8ae0c-109">Administrador de conta</span><span class="sxs-lookup"><span data-stu-id="8ae0c-109">Account admin</span></span>
- <span data-ttu-id="8ae0c-110">Administrador global</span><span class="sxs-lookup"><span data-stu-id="8ae0c-110">Global admin</span></span>

<span data-ttu-id="8ae0c-111">Para receber o pagamento de seus programas de incentivo para um local de MPN específico, conclua o registro associando um perfil de pagamento e imposto válido ao programa e ao local de MPN.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-111">Before you can receive payment for your incentive programs for a particular MPN location, you must complete your enrollment by associating a valid payout and tax profile with the program and MPN location.</span></span> <span data-ttu-id="8ae0c-112">A Microsoft usará este perfil de pagamento e imposto para emitir pagamentos.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-112">Microsoft will use this payout and tax profile to issue payments.</span></span> <span data-ttu-id="8ae0c-113">Você pode usar transferência bancária eletrônica ou uma nota de crédito para pagamento, dependendo das regras do programa de incentivo.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-113">You may be allowed to use electronic bank transfer or a credit note for payment, depending on the rules of the incentive program.</span></span> 

## <a name="roles-currencies-and-other-microsoft-programs"></a><span data-ttu-id="8ae0c-114">Funções, moedas e outros programas da Microsoft</span><span class="sxs-lookup"><span data-stu-id="8ae0c-114">Roles, currencies, and other Microsoft programs</span></span>

<span data-ttu-id="8ae0c-115">É importante entender as informações abaixo antes de começar com o pagamento e o perfil de impostos.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-115">It's important to understand the information below before you get started with your payout and tax profile.</span></span>

### <a name="roles-and-permissions"></a><span data-ttu-id="8ae0c-116">Funções e permissões</span><span class="sxs-lookup"><span data-stu-id="8ae0c-116">Roles and permissions</span></span>

<span data-ttu-id="8ae0c-117">Você deve ser um administrador de incentivos para inserir informações bancárias e de impostos para pagamentos de incentivos.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-117">You must be an Incentives Admin to enter bank and tax information for incentive payments.</span></span> <span data-ttu-id="8ae0c-118">Se você for um administrador de MPN/conta, você pode atribuir a si mesmo e/ou um colega para ser o administrador de incentivos.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-118">If you're an MPN/Account Admin, you can assign yourself and/or a colleague to be the Incentives Admin.</span></span>

<span data-ttu-id="8ae0c-119">Se você precisar solicitar as permissões de administrador de incentivos, entre em contato com o administrador do MPN ou com o administrador global. Você pode descobrir quem em sua empresa tem essas funções entrando no [painel do Partner Center](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="8ae0c-119">If you need to request Incentives Admin permissions, contact your MPN Admin or Global Admin. You can find out who in your company has these roles by signing into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span> <span data-ttu-id="8ae0c-120">No ícone de **configurações** no canto superior direito, selecione **Gerenciamento de usuários** e filtre o administrador global.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-120">From the **Settings** icon at the top right, select **User Management** and then filter on Global Admin.</span></span>

<span data-ttu-id="8ae0c-121">Os incentivos podem exibir os ganhos de incentivos e os detalhes e relatórios de pagamento, mas não podem editar os detalhes bancários e de imposto.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-121">Incentives Users can view Incentive earnings and payment details and reports, but can’t edit bank and tax details.</span></span>

### <a name="choose-your-disbursement-currency"></a><span data-ttu-id="8ae0c-122">Escolha sua moeda de pagamento</span><span class="sxs-lookup"><span data-stu-id="8ae0c-122">Choose your disbursement currency</span></span>

<span data-ttu-id="8ae0c-123">Os pagamentos de incentivo são feitos na moeda que você selecionou ao configurar seu perfil de pagamento.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-123">Incentive payments are made in the currency you selected when you set up your payment profile.</span></span> <span data-ttu-id="8ae0c-124">Os pagamentos serão calculados usando uma taxa de câmbio como definido mensalmente pela Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-124">Payments will be calculated using an exchange rate as set monthly by Microsoft.</span></span> <span data-ttu-id="8ae0c-125">Você será responsável por qualquer alteração no valor devido à moeda selecionada.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-125">You’ll be responsible for any changes in value due to the currency selected.</span></span>

### <a name="using-different-profiles-for-different-microsoft-programs"></a><span data-ttu-id="8ae0c-126">Usando perfis diferentes para programas diferentes da Microsoft</span><span class="sxs-lookup"><span data-stu-id="8ae0c-126">Using different profiles for different Microsoft programs</span></span>

<span data-ttu-id="8ae0c-127">Se sua empresa estiver inscrita em vários programas de incentivo, você poderá usar a mesma conta de pagamento para todos eles ou optar por usar contas de pagamento diferentes para programas diferentes.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-127">If your company is enrolled in multiple incentive programs, you can use the same payment account for all of them, or choose to use different payment accounts for different programs.</span></span>

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="8ae0c-128">Criar e gerenciar perfis fiscais e de pagamento no Partner Center</span><span class="sxs-lookup"><span data-stu-id="8ae0c-128">Create and manage payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="8ae0c-129">As seções abaixo guiarão você pelo processo de criação e gerenciamento de perfis de pagamento e impostos no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-129">The sections below will walk you through the process of creating and managing payment and tax profiles in Partner Center.</span></span>

>[!IMPORTANT]
><span data-ttu-id="8ae0c-130">Você deve ser um administrador de incentivos para criar ou gerenciar perfis de pagamento no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-130">You must be an Incentive admin to create or manage payment profiles in Partner Center.</span></span> <span data-ttu-id="8ae0c-131">As funções de incentivo devem ser atribuídas a cada local MPN em cada programa de incentivo.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-131">Incentive roles must be assigned to each MPN location under each incentive program.</span></span> <span data-ttu-id="8ae0c-132">Para obter mais informações sobre como adicionar administradores de incentivos no Partner Center, consulte [criar contas de usuário](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="8ae0c-132">For more information on how to add Incentive admins in Partner Center, see [Create user accounts](create-user-accounts-and-set-permissions.md).</span></span>

## <a name="access-the-payout-and-tax-section-in-partner-center"></a><span data-ttu-id="8ae0c-133">Acessar a seção pagamento e impostos no Partner Center</span><span class="sxs-lookup"><span data-stu-id="8ae0c-133">Access the payout and tax section in Partner Center</span></span>

1. <span data-ttu-id="8ae0c-134">Entre no [painel do Partner Center](https://partner.microsoft.com/dashboard/) usando sua conta do Azure Active Directory (Azure AD) (conta da empresa) ou o endereço de email apropriado, se um tiver sido atribuído.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-134">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/) using your Azure Active Directory (Azure AD) account (company account), or the appropriate email address if one was assigned.</span></span>

   - <span data-ttu-id="8ae0c-135">Vários domínios podem ser registrados em uma conta do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-135">Multiple domains can be registered within one Azure AD account.</span></span> <span data-ttu-id="8ae0c-136">Entre em contato com seu administrador global para determinar quais domínios estão associados.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-136">Contact your Global admin to determine which domains are associated.</span></span>
   - <span data-ttu-id="8ae0c-137">Se você só puder fazer logon com o @onmicrosoft.com domínio, entre em contato com o administrador da conta para adicionar outros domínios à conta do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-137">If you're only able to log in with the @onmicrosoft.com domain, contact your Account admin to add additional domains to the Azure AD account.</span></span>
   - <span data-ttu-id="8ae0c-138">Se for solicitado que você selecione conta **corporativa ou de estudante** ou **conta pessoal** , selecione **conta corporativa ou de estudante**.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-138">If you're prompted to select **Work or school account** or **Personal Account** , select **Work or school account**.</span></span>

2. <span data-ttu-id="8ae0c-139">Selecione o ícone de engrenagem para abrir o menu **configurações** e, em seguida, selecione **configurações de parceiro**.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-139">Select the gear icon to open the **Settings** menu, and then select **Partner settings**.</span></span>

3. <span data-ttu-id="8ae0c-140">No menu **configurações de conta** , selecione **pagamento e imposto**.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-140">In the **Account settings** menu, select **Payout and tax**.</span></span> 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a><span data-ttu-id="8ae0c-141">Atribuir pagamentos e perfis de impostos a programas individuais</span><span class="sxs-lookup"><span data-stu-id="8ae0c-141">Assign payout and tax profiles to individual programs</span></span>

1. <span data-ttu-id="8ae0c-142">Entre no [painel do Partner Center](https://partner.microsoft.com/dashboard/)e selecione o ícone de engrenagem para abrir o menu **configurações** .</span><span class="sxs-lookup"><span data-stu-id="8ae0c-142">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/), and then select the gear icon to open the **Settings** menu.</span></span> 

2. <span data-ttu-id="8ae0c-143">Selecione **configurações de parceiro** , expanda a **seção pagamento e imposto** e selecione **atribuição de perfil de pagamento e imposto**.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-143">Select **Partner settings** , expand the **Payout and tax section** , and then select **Payout and tax profile assignment**.</span></span> 
   
   <span data-ttu-id="8ae0c-144">Será exibida uma lista de seus programas.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-144">A list of your programs will be displayed.</span></span> <span data-ttu-id="8ae0c-145">Selecione a seta ao lado de um programa para ver os detalhes do perfil.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-145">Select the arrow next to a program to see profile details.</span></span> 

3. <span data-ttu-id="8ae0c-146">No menu suspenso **perfil de imposto** , selecione o perfil de imposto desejado ou selecione a opção para criar um novo perfil.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-146">In the **Tax Profile** dropdown menu, select the tax profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="8ae0c-147">Ao selecionar a opção para criar um novo perfil, você será redirecionado adequadamente.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-147">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="8ae0c-148">Selecione continuar na janela pop-up.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-148">Select Continue in the pop-up window.</span></span> <span data-ttu-id="8ae0c-149">O processo para criar um novo perfil de imposto foi fornecido abaixo.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-149">The process for creating a new tax profile has been provided below.</span></span>

4. <span data-ttu-id="8ae0c-150">Selecione o **método de pagamento**.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-150">Select **Payment method**.</span></span>

   - <span data-ttu-id="8ae0c-151">Se você selecionou **transferência bancária eletrônica** como seu método de pagamento, selecione o perfil de pagamento desejado ou selecione a opção para criar um novo perfil.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-151">If you have selected **Electronic bank transfer** as your payment method, select the payment profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="8ae0c-152">Ao selecionar a opção para criar um novo perfil, você será redirecionado adequadamente.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-152">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span> <span data-ttu-id="8ae0c-153">Selecione continuar na janela pop-up.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-153">Select Continue in the pop-up window.</span></span> <span data-ttu-id="8ae0c-154">O processo para criar um novo perfil de pagamento foi fornecido abaixo.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-154">The process for creating a new payment profile has been provided below.</span></span>

   - <span data-ttu-id="8ae0c-155">Se você tiver selecionado **Nota de crédito** como seu método de pagamento, conclua a verificação.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-155">If you have selected **Credit Note** as your payment method, then complete the verification.</span></span> <span data-ttu-id="8ae0c-156">Isso confirma que o número SAP referenciado pertence à sua organização.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-156">This confirms that the referenced SAP number belongs to your organization.</span></span>

    >[!NOTE]
    ><span data-ttu-id="8ae0c-157">Se houver várias entidades comerciais da Microsoft listadas, você deverá selecionar um perfil de pagamento para cada entidade.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-157">If there are multiple Microsoft business entities listed, you must select a payment profile for each entity.</span></span>

    >[!NOTE]
    ><span data-ttu-id="8ae0c-158">A disponibilidade do método de pagamento depende das regras do programa de incentivo.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-158">The payment method availability is dependent on the rules of the incentive program.</span></span>
    
5. <span data-ttu-id="8ae0c-159">Selecione a **moeda**.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-159">Select the **Currency**.</span></span>

6. <span data-ttu-id="8ae0c-160">Quando você tiver concluído todos os campos de pagamento, selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-160">When you’ve completed all of the payment fields, select **Submit**.</span></span>

## <a name="create-your-bank-profile"></a><span data-ttu-id="8ae0c-161">Criar seu perfil bancário</span><span class="sxs-lookup"><span data-stu-id="8ae0c-161">Create your bank profile</span></span>

<span data-ttu-id="8ae0c-162">Os perfis bancários são criados em um nível de organização.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-162">Bank profiles are created at an organization level.</span></span> <span data-ttu-id="8ae0c-163">Isso permite que um perfil de banco seja atribuído a vários programas de incentivo e IDs de MPN em uma organização.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-163">This allows one bank profile to be assigned across multiple MPN ID’s and incentive programs within an organization.</span></span> <span data-ttu-id="8ae0c-164">Pode haver exceções ao aplicar o perfil bancário a diferentes países, já que regras de imposto e de bancos diferentes podem ser aplicadas.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-164">There may be exceptions when applying the banking profile to different countries, as different banking and tax rules may apply.</span></span>

>[!NOTE]
><span data-ttu-id="8ae0c-165">Nas páginas a seguir, são necessários campos com um asterisco.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-165">On the following pages, fields with an asterisk are required.</span></span> <span data-ttu-id="8ae0c-166">Se você não souber o que é um campo, selecione o ícone de informações.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-166">If you don’t know what a field is, select the information icon.</span></span> 

1. <span data-ttu-id="8ae0c-167">Na página **detalhes** , preencha os seguintes campos: **nome do perfil:** Insira um nome exclusivo para identificar este perfil de pagamento.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-167">On the **Details** page, complete the following fields: **Profile name:** Enter a unique name to identify this payment profile.</span></span>
    <span data-ttu-id="8ae0c-168">**Local da conta bancária:** O país no qual o banco da sua empresa está localizado.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-168">**Bank account location:** The country in which your company’s bank is located.</span></span>
    <span data-ttu-id="8ae0c-169">**Método de pagamento:** O método de pagamento preferencial para o Partner Center é a transferência bancária eletrônica.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-169">**Payment method:** The preferred payment method for Partner Center is electronic bank transfer.</span></span>

2. <span data-ttu-id="8ae0c-170">Selecione **Avançar**.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-170">Select **Next**.</span></span>

3. <span data-ttu-id="8ae0c-171">Na página **conta bancária** , insira suas informações.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-171">On the **Bank account** page, enter your information.</span></span> <span data-ttu-id="8ae0c-172">Os campos mostrados nesta página variam de acordo com o país.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-172">Fields shown on this page will vary by country.</span></span> 

4. <span data-ttu-id="8ae0c-173">Selecione **Avançar**.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-173">Select **Next**.</span></span>

5. <span data-ttu-id="8ae0c-174">Na página do **beneficiário** , insira as informações apropriadas.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-174">On the **Beneficiary** page, enter the appropriate information.</span></span> <span data-ttu-id="8ae0c-175">O beneficiário é a pessoa em sua empresa que o banco deve contatar se precisar discutir sua conta.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-175">The beneficiary is the person in your company that the bank would contact if they need to discuss your account.</span></span>

6. <span data-ttu-id="8ae0c-176">Quando os campos forem concluídos, selecione **concluir** e, em seguida, selecione **confirmar** para criar seu perfil bancário.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-176">When the fields are completed, select **Finish** , and then select **Confirm** to create your bank profile.</span></span>

<span data-ttu-id="8ae0c-177">Você será redirecionado para a página de **perfis de pagamento e impostos** .</span><span class="sxs-lookup"><span data-stu-id="8ae0c-177">You’ll be redirected to the **Payout and tax profiles** page.</span></span> <span data-ttu-id="8ae0c-178">O status do seu novo perfil refletirá a **validação pendente da Microsoft** até que a validação tenha sido concluída.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-178">The status of your new profile will reflect **Pending Microsoft validation** until the validation has been completed.</span></span> <span data-ttu-id="8ae0c-179">Esse processo pode levar até 48 horas.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-179">This process may take up to 48 hours.</span></span> <span data-ttu-id="8ae0c-180">Após a conclusão da validação, o status do perfil refletirá **aprovado** ou **ação necessária**.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-180">Once validation has been completed, your profile status will reflect either **Approved** or **Action required**.</span></span> <span data-ttu-id="8ae0c-181">Se a **ação for necessária** , repita as etapas acima fornecendo as informações necessárias.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-181">If **Action Required** , repeat the steps above providing the necessary information.</span></span> 

## <a name="create-your-tax-profile"></a><span data-ttu-id="8ae0c-182">Criar seu perfil de imposto</span><span class="sxs-lookup"><span data-stu-id="8ae0c-182">Create your tax profile</span></span>

<span data-ttu-id="8ae0c-183">Use o procedimento a seguir para fornecer à Microsoft as informações de impostos necessárias para sua organização.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-183">Use the following procedure to provide Microsoft with the tax information required for your organization.</span></span> <span data-ttu-id="8ae0c-184">As páginas nesta seção são dinâmicas e variam de acordo com seu país ou região.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-184">The pages in this section are dynamic and will vary according to your country or region.</span></span> <span data-ttu-id="8ae0c-185">Se precisar de ajuda para identificar as informações de imposto corretas, entre em contato com as fontes governamentais apropriadas em seu país.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-185">If you need help with identifying the correct tax information, contact the appropriate government sources in your country.</span></span>

<span data-ttu-id="8ae0c-186">Para empresas parceiras nas Américas, se você precisar de informações sobre como concluir os formulários W8 ou W9, os seguintes endereços levarão você para o site IRS:</span><span class="sxs-lookup"><span data-stu-id="8ae0c-186">For partner companies in the Americas, if you require information on completing the W8 or W9 forms, the following addresses take you to the IRS site:</span></span>

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> <span data-ttu-id="8ae0c-187">Insira apenas os detalhes de sua empresa.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-187">Enter only details for your company.</span></span> <span data-ttu-id="8ae0c-188">Nunca insira detalhes pessoais.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-188">Never enter personal details.</span></span>

1. <span data-ttu-id="8ae0c-189">Na página **perfil de negócios** , preencha os campos obrigatórios e, em seguida, selecione **Avançar**.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-189">On the **Business Profile** page, complete the required fields and then select **Next**.</span></span> 

2. <span data-ttu-id="8ae0c-190">Na página **instalação** , selecione a opção que se aplica à sua empresa.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-190">On the **Setup** page, select the option that applies to your company.</span></span>

   - <span data-ttu-id="8ae0c-191">Selecione a opção à esquerda se sua empresa estiver incorporada somente no Estados Unidos ou se esse perfil for um indivíduo.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-191">Select the option on the left if your company is incorporated in the United States only, or if this profile is for an individual.</span></span>
   - <span data-ttu-id="8ae0c-192">Selecione a opção à direita se sua empresa estiver incorporada fora do Estados Unidos e, em seguida, selecione seu país/região na lista.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-192">Select the option on the right if your company is incorporated outside of the United States, and then select your country/region from the list.</span></span>

3. <span data-ttu-id="8ae0c-193">Selecione **Avançar**.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-193">Select **Next**.</span></span> 

4. <span data-ttu-id="8ae0c-194">Na página **status do imposto** , insira as informações necessárias e, em seguida, selecione **Avançar**.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-194">On the **Tax status** page, enter the required information, and then select **Next**.</span></span> <span data-ttu-id="8ae0c-195">Os campos nesta página variam de acordo com o país.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-195">Fields on this page will vary by country.</span></span> <span data-ttu-id="8ae0c-196">seus detalhes.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-196">your details.</span></span> 

5. <span data-ttu-id="8ae0c-197">Na página de **documentação adicional** , os campos obrigatórios e selecione **Avançar**.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-197">On the **Additional documentation** page, the required fields and select **Next**.</span></span> 

6. <span data-ttu-id="8ae0c-198">Selecione **procurar** para carregar todos os documentos exigidos por seu país ou região.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-198">Select **Browse** to upload any documents required by your country or region.</span></span> <span data-ttu-id="8ae0c-199">Quando o nome do documento for mostrado, selecione **carregar**.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-199">When the document name is shown, select **Upload**.</span></span> 

7. <span data-ttu-id="8ae0c-200">Se você precisar remover o documento, selecione **remover**.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-200">If you need to remove the document, select **Remove**.</span></span>

8. <span data-ttu-id="8ae0c-201">Para salvar e continuar, selecione **concluir**.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-201">To save and continue, select **Finish**.</span></span>

9. <span data-ttu-id="8ae0c-202">Selecione **confirmar** na mensagem pop-up.</span><span class="sxs-lookup"><span data-stu-id="8ae0c-202">Select **Confirm** on the pop-up message.</span></span> <span data-ttu-id="8ae0c-203">Você será levado de volta à página de **configuração de pagamento e imposto** .</span><span class="sxs-lookup"><span data-stu-id="8ae0c-203">You’ll be taken back to the **Payout and tax setup** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8ae0c-204">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="8ae0c-204">Next steps</span></span>

- [<span data-ttu-id="8ae0c-205">Perguntas frequentes sobre o pagamento de incentivos e o perfil fiscal</span><span class="sxs-lookup"><span data-stu-id="8ae0c-205">Incentives payout and tax profile FAQs</span></span>](incentives-payout-tax-profile-faqs.md)
