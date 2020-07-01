---
title: Criar e gerenciar perfis de pagamento e de impostos no Partner Center
ms.topic: article
ms.date: 06/29/2020
description: Antes que você possa ser pago pelo trabalho de seus incentivos, você precisa criar seus perfis de pagamento e de impostos.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: b7f99ff64b6cdabe8b59607e5820daf0909050f1
ms.sourcegitcommit: bea864212edc90c5f851566505deef6623f79723
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "85719304"
---
# <a name="payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="e6ca3-103">Perfis de pagamento e impostos no Partner Center</span><span class="sxs-lookup"><span data-stu-id="e6ca3-103">Payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="e6ca3-104">Aplica-se a:</span><span class="sxs-lookup"><span data-stu-id="e6ca3-104">Applies to:</span></span>

- <span data-ttu-id="e6ca3-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="e6ca3-105">Partner Center</span></span>

<span data-ttu-id="e6ca3-106">Para receber o pagamento de seus programas de incentivo para um local de MPN específico, conclua o registro associando um perfil de pagamento e imposto válido ao programa e ao local de MPN.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-106">Before you can receive payment for your incentive programs for a particular MPN location, you must complete your enrollment by associating a valid payout and tax profile with the program and MPN location.</span></span> <span data-ttu-id="e6ca3-107">A Microsoft usará este perfil de pagamento e imposto para emitir pagamentos.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-107">Microsoft will use this payout and tax profile to issue payments.</span></span> <span data-ttu-id="e6ca3-108">Você pode usar transferência bancária eletrônica ou uma nota de crédito para pagamento, dependendo das regras do programa de incentivo.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-108">You may be allowed to use electronic bank transfer or a credit note for payment, depending on the rules of the incentive program.</span></span> 

<span data-ttu-id="e6ca3-109">Funções apropriadas:</span><span class="sxs-lookup"><span data-stu-id="e6ca3-109">Appropriate roles:</span></span>

- <span data-ttu-id="e6ca3-110">Administrador de incentivos</span><span class="sxs-lookup"><span data-stu-id="e6ca3-110">Incentives admin</span></span>
- <span data-ttu-id="e6ca3-111">Administrador de cobrança</span><span class="sxs-lookup"><span data-stu-id="e6ca3-111">Billing admin</span></span>
- <span data-ttu-id="e6ca3-112">Administrador global</span><span class="sxs-lookup"><span data-stu-id="e6ca3-112">Global admin</span></span>

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="e6ca3-113">Criar e gerenciar perfis de pagamento e de impostos no Partner Center</span><span class="sxs-lookup"><span data-stu-id="e6ca3-113">Create and manage payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="e6ca3-114">As seções abaixo guiarão você pelo processo de criação e gerenciamento de perfis de pagamento e impostos no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-114">The sections below will walk you through the process of creating and managing payment and tax profiles in Partner Center.</span></span>

>[!IMPORTANT]
><span data-ttu-id="e6ca3-115">Você deve ser um administrador de incentivos para criar ou gerenciar perfis de pagamento no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-115">You must be an Incentive admin to create or manage payment profiles in Partner Center.</span></span> <span data-ttu-id="e6ca3-116">As funções de incentivo devem ser atribuídas a cada local MPN em cada programa de incentivo.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-116">Incentive roles must be assigned to each MPN location under each incentive program.</span></span> <span data-ttu-id="e6ca3-117">Para obter mais informações sobre como adicionar administradores de incentivos no Partner Center, consulte [como adicionar usuários de incentivo ou administradores no Partner Center](https://support.microsoft.com/help/3011450/how-to-add-incentive-users-or-admins-in-partner-center).</span><span class="sxs-lookup"><span data-stu-id="e6ca3-117">For more information on how to add Incentive admins in Partner Center, see [How to add incentive users or admins in Partner Center](https://support.microsoft.com/help/3011450/how-to-add-incentive-users-or-admins-in-partner-center).</span></span>

## <a name="access-the-payout-and-tax-section-in-partner-center"></a><span data-ttu-id="e6ca3-118">Acessar a seção pagamento e impostos no Partner Center</span><span class="sxs-lookup"><span data-stu-id="e6ca3-118">Access the payout and tax section in Partner Center</span></span>

1. <span data-ttu-id="e6ca3-119">Faça logon no Partner Center usando sua conta do AAD (conta da empresa) ou o endereço de email apropriado, se um tiver sido atribuído.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-119">Log into Partner Center using your AAD account (company account), or the appropriate email address if one was assigned.</span></span> 

   - <span data-ttu-id="e6ca3-120">Vários domínios podem ser registrados em uma conta do AAD.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-120">Multiple domains can be registered within one AAD account.</span></span> <span data-ttu-id="e6ca3-121">Entre em contato com seu administrador global para determinar quais domínios estão associados.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-121">Contact your Global admin to determine which domains are associated.</span></span>
   - <span data-ttu-id="e6ca3-122">Se você só puder fazer logon com **@onmicrosoft.com** o domínio, entre em contato com o administrador da conta para adicionar outros domínios à conta do AAD.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-122">If you are only able to login with **@onmicrosoft.com** domain, contact your Account admin to add additional domains to the AAD account.</span></span>
   - <span data-ttu-id="e6ca3-123">Se for solicitado que você selecione conta **corporativa ou de estudante** ou **conta pessoal**, selecione **conta corporativa ou de estudante**.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-123">If prompted to select **Work or school account** or **Personal Account**, select **Work or school account**.</span></span>

2. <span data-ttu-id="e6ca3-124">Selecione o ícone de engrenagem para abrir o menu **configurações** e, em seguida, selecione **configurações de parceiro**.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-124">Select the gear icon to open the **Settings** menu, and then select **Partner settings**.</span></span>

3. <span data-ttu-id="e6ca3-125">No menu **configurações de conta** , selecione **pagamento e imposto**.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-125">In the **Account settings** menu, select **Payout and tax**.</span></span> 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a><span data-ttu-id="e6ca3-126">Atribuir pagamentos e perfis de impostos a programas individuais</span><span class="sxs-lookup"><span data-stu-id="e6ca3-126">Assign payout and tax profiles to individual programs</span></span>

1. <span data-ttu-id="e6ca3-127">No Partner Center, selecione o ícone de engrenagem para abrir o menu **configurações** .</span><span class="sxs-lookup"><span data-stu-id="e6ca3-127">In Partner Center, select the gear icon to open the **Settings** menu.</span></span> 

2. <span data-ttu-id="e6ca3-128">Selecione **configurações de parceiro**, expanda a **seção pagamento e imposto**e selecione **atribuição de perfil de pagamento e imposto**.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-128">Select **Partner settings**, expand the **Payout and tax section**, and then select **Payout and tax profile assignment**.</span></span> 
   
   <span data-ttu-id="e6ca3-129">Será exibida uma lista de seus programas.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-129">A list of your programs will be displayed.</span></span> <span data-ttu-id="e6ca3-130">Selecione a seta ao lado de um programa para ver os detalhes do perfil.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-130">Select the arrow next to a program to see profile details.</span></span> 

3. <span data-ttu-id="e6ca3-131">No menu suspenso **perfil de imposto** , selecione o perfil de imposto desejado ou selecione a opção para criar um novo perfil.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-131">In the **Tax Profile** dropdown menu, select the tax profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="e6ca3-132">Ao selecionar a opção para criar um novo perfil, você será redirecionado adequadamente.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-132">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="e6ca3-133">Selecione continuar na janela pop-up.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-133">Select Continue in the pop-up window.</span></span> <span data-ttu-id="e6ca3-134">O processo para criar um novo perfil de imposto foi fornecido abaixo.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-134">The process for creating a new tax profile has been provided below.</span></span>

4. <span data-ttu-id="e6ca3-135">Selecione o **método de pagamento**.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-135">Select **Payment method**.</span></span>

   - <span data-ttu-id="e6ca3-136">Se você tiver selecionado **transferência bancária eletrônica** como método de pagamento, em seguida, no menu suspenso perfil de pagamento, selecione o perfil de pagamento desejado ou selecione a opção para criar um novo perfil.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-136">If you have selected **Electronic bank transfer** as payment method then in the payment profile dropdown select the payment profile you want or select the option to create a new profile.</span></span> <span data-ttu-id="e6ca3-137">Ao selecionar a opção para criar um novo perfil, você será redirecionado adequadamente.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-137">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="e6ca3-138">Selecione continuar na janela pop-up.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-138">Select Continue in the pop-up window.</span></span> <span data-ttu-id="e6ca3-139">O processo para criar um novo perfil de pagamento foi fornecido abaixo.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-139">The process for creating a new payment profile has been provided below.</span></span>

   - <span data-ttu-id="e6ca3-140">Se você tiver selecionado **Nota de crédito** como o método de pagamento, conclua a verificação para confirmar se o número SAP referenciado pertence à sua organização.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-140">If you have selected **Credit Note** as the payment method then complete the verification to confirm that the referenced SAP number belongs to your organization.</span></span>

    >[!NOTE]
    ><span data-ttu-id="e6ca3-141">Se houver várias entidades comerciais da Microsoft listadas, você deverá selecionar um perfil de pagamento para cada entidade.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-141">If there are multiple Microsoft business entities listed, you must select a payment profile for each entity.</span></span>

    >[!NOTE]
    ><span data-ttu-id="e6ca3-142">A disponibilidade do método de pagamento depende das regras do programa de incentivo.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-142">The payment method availability is dependent on the rules of the incentive program.</span></span>
    
5. <span data-ttu-id="e6ca3-143">Selecione a **moeda**.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-143">Select the **Currency**.</span></span>

6. <span data-ttu-id="e6ca3-144">Quando você tiver concluído todos os campos de pagamento, selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-144">When you’ve completed all of the payment fields, select **Submit**.</span></span>

## <a name="create-your-bank-profile"></a><span data-ttu-id="e6ca3-145">Criar seu perfil bancário</span><span class="sxs-lookup"><span data-stu-id="e6ca3-145">Create your bank profile</span></span>

<span data-ttu-id="e6ca3-146">Os perfis bancários são criados em um nível de organização, o que permite que o mesmo perfil de banco seja atribuído a vários programas de incentivo e ID de MPN em uma organização.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-146">Bank profiles are created at an organization level, which allows for the same bank profile to be assigned across multiple MPN ID’s and incentive programs within an organization.</span></span> <span data-ttu-id="e6ca3-147">Pode haver exceções ao aplicar o perfil bancário a diferentes países, já que regras de imposto e de bancos diferentes podem ser aplicadas.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-147">There may be exceptions when applying the banking profile to different countries, as different banking and tax rules may apply.</span></span>

>[!NOTE]
><span data-ttu-id="e6ca3-148">Nas páginas a seguir, são necessários campos com um asterisco.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-148">On the following pages, fields with an asterisk are required.</span></span> <span data-ttu-id="e6ca3-149">Se você não souber o que é um campo, selecione o ícone de informações.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-149">If you don’t know what a field is, select the information icon.</span></span> 

1. <span data-ttu-id="e6ca3-150">Na página **detalhes** , preencha os seguintes campos: **nome do perfil:** Insira um nome exclusivo para identificar este perfil de pagamento.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-150">On the **Details** page, complete the following fields: **Profile name:** Enter a unique name to identify this payment profile.</span></span>
    <span data-ttu-id="e6ca3-151">**Local da conta bancária:** O país no qual o banco da sua empresa está localizado.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-151">**Bank account location:** The country in which your company’s bank is located.</span></span>
    <span data-ttu-id="e6ca3-152">**Método de pagamento:** O método de pagamento preferido é para o Partner Center ser transferência bancária eletrônica.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-152">**Payment method:** The preferred payment method is for Partner Center is electronic bank transfer.</span></span>

2. <span data-ttu-id="e6ca3-153">Selecione **Avançar**.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-153">Select **Next**.</span></span>

3. <span data-ttu-id="e6ca3-154">Na página **conta bancária** , insira suas informações.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-154">On the **Bank account** page, enter your information.</span></span> <span data-ttu-id="e6ca3-155">Os campos mostrados nesta página variam de acordo com o país.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-155">Fields shown on this page will vary by country.</span></span> 

4. <span data-ttu-id="e6ca3-156">Selecione **Avançar**.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-156">Select **Next**.</span></span>

5. <span data-ttu-id="e6ca3-157">Na página do **beneficiário** , insira as informações apropriadas.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-157">On the **Beneficiary** page, enter the appropriate information.</span></span> <span data-ttu-id="e6ca3-158">O beneficiário é a pessoa em sua empresa que o banco deve contatar se precisar discutir sua conta.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-158">The beneficiary is the person in your company that the bank would contact if they need to discuss your account.</span></span>

6. <span data-ttu-id="e6ca3-159">Quando os campos forem concluídos, selecione **concluir**e, em seguida, selecione **confirmar** para criar seu perfil bancário.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-159">When the fields are completed, select **Finish**, and then select **Confirm** to create your bank profile.</span></span>

<span data-ttu-id="e6ca3-160">Você será redirecionado para a página de **perfis de pagamento e impostos** .</span><span class="sxs-lookup"><span data-stu-id="e6ca3-160">You’ll be redirected to the **Payout and tax profiles** page.</span></span> <span data-ttu-id="e6ca3-161">O status do seu novo perfil refletirá a **validação pendente da Microsoft** até que a validação tenha sido concluída.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-161">The status of your new profile will reflect **Pending Microsoft validation** until the validation has been completed.</span></span> <span data-ttu-id="e6ca3-162">Isso pode levar até 48 horas.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-162">This may take up to 48 hours.</span></span> <span data-ttu-id="e6ca3-163">Após a conclusão da validação, o status do perfil refletirá **aprovado** ou **ação necessária**.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-163">Once validation has been completed, your profile status will reflect either **Approved** or **Action required**.</span></span> <span data-ttu-id="e6ca3-164">Se a **ação for necessária**, repita as etapas acima fornecendo as informações necessárias.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-164">If **Action Required**, repeat the steps above providing the necessary information.</span></span> 

## <a name="create-your-tax-profile"></a><span data-ttu-id="e6ca3-165">Criar seu perfil de imposto</span><span class="sxs-lookup"><span data-stu-id="e6ca3-165">Create your tax profile</span></span>

<span data-ttu-id="e6ca3-166">Use o procedimento a seguir para fornecer à Microsoft as informações de impostos necessárias para sua organização.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-166">Use the following procedure to provide Microsoft with the tax information required for your organization.</span></span> <span data-ttu-id="e6ca3-167">As páginas nesta seção são dinâmicas e variam de acordo com seu país ou região.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-167">The pages in this section are dynamic and will vary according your country or region.</span></span> <span data-ttu-id="e6ca3-168">Se você precisar de ajuda para identificar as informações de imposto corretas, entre em contato com as fontes governamentais apropriadas em seu país.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-168">If you need help identifying the correct tax information, contact the appropriate government sources in your country.</span></span>

<span data-ttu-id="e6ca3-169">Para empresas parceiras nas Américas, se você precisar de informações sobre como concluir os formulários W8 ou W9, os seguintes endereços levarão você para o site IRS:</span><span class="sxs-lookup"><span data-stu-id="e6ca3-169">For partner companies in the Americas, if you require information on completing the W8 or W9 forms, the following addresses take you to the IRS site:</span></span>

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> <span data-ttu-id="e6ca3-170">Insira apenas os detalhes de sua empresa.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-170">Enter only details for your company.</span></span> <span data-ttu-id="e6ca3-171">Nunca insira detalhes pessoais.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-171">Never enter personal details.</span></span>

1. <span data-ttu-id="e6ca3-172">Na página **perfil de negócios** , preencha os campos obrigatórios e, em seguida, selecione **Avançar**.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-172">On the **Business Profile** page, complete the required fields and then select **Next**.</span></span> 

2. <span data-ttu-id="e6ca3-173">Na página **instalação** , selecione a opção que se aplica à sua empresa.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-173">On the **Setup** page, select the option that applies to your company.</span></span>

   - <span data-ttu-id="e6ca3-174">Selecione a opção à esquerda se sua empresa estiver incorporada somente no Estados Unidos ou se esse perfil for um indivíduo.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-174">Select the option on the left if your company is incorporated in the United States only, or if this profile is for an individual.</span></span> 
   - <span data-ttu-id="e6ca3-175">Selecione a opção à direita se sua empresa estiver incorporada fora do Estados Unidos e, em seguida, selecione seu país/região na lista.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-175">Select the option on the right if your company is incorporated outside of the United States, and then select your country/region from the list.</span></span>

3. <span data-ttu-id="e6ca3-176">Selecione **Avançar**.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-176">Select **Next**.</span></span> 

4. <span data-ttu-id="e6ca3-177">Na página **status do imposto** , insira as informações necessárias e, em seguida, selecione **Avançar**.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-177">On the **Tax status** page, enter the required information, and then select **Next**.</span></span> <span data-ttu-id="e6ca3-178">Os campos nesta página variam de acordo com o país.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-178">Fields on this page will vary by country.</span></span> <span data-ttu-id="e6ca3-179">seus detalhes.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-179">your details.</span></span> 

5. <span data-ttu-id="e6ca3-180">Na página de **documentação adicional** , os campos obrigatórios e selecione **Avançar**.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-180">On the **Additional documentation** page, the required fields and select **Next**.</span></span> 

6. <span data-ttu-id="e6ca3-181">Selecione **procurar** para carregar todos os documentos exigidos por seu país ou região.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-181">Select **Browse** to upload any documents required by your country or region.</span></span> <span data-ttu-id="e6ca3-182">Quando o nome do documento for mostrado, selecione **carregar**.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-182">When the document name is shown, select **Upload**.</span></span> 

7. <span data-ttu-id="e6ca3-183">Se você precisar remover o documento, selecione **remover**.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-183">If you need to remove the document, select **Remove**.</span></span>

8. <span data-ttu-id="e6ca3-184">Para salvar e continuar, selecione **concluir**.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-184">To save and continue, select **Finish**.</span></span>

9. <span data-ttu-id="e6ca3-185">Selecione **confirmar** na mensagem pop-up.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-185">Select **Confirm** on the pop-up message.</span></span> <span data-ttu-id="e6ca3-186">Você será levado de volta à página de **configuração de pagamento e imposto** .</span><span class="sxs-lookup"><span data-stu-id="e6ca3-186">You’ll be taken back to the **Payout and tax setup** page.</span></span>

## <a name="payout-and-tax-profile-faqs"></a><span data-ttu-id="e6ca3-187">Perguntas frequentes sobre pagamento e perfil fiscal</span><span class="sxs-lookup"><span data-stu-id="e6ca3-187">Payout and tax profile FAQs</span></span>

### <a name="why-do-i-need-to-provide-my-payout-andor-tax-details"></a><span data-ttu-id="e6ca3-188">Por que preciso fornecer meus detalhes de pagamento e/ou imposto?</span><span class="sxs-lookup"><span data-stu-id="e6ca3-188">Why do I need to provide my payout and/or tax details?</span></span>

<span data-ttu-id="e6ca3-189">Para receber pagamentos para programas de incentivo da Microsoft, você precisa concluir o registro fornecendo detalhes válidos de pagamento e imposto.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-189">In order to receive payouts for Microsoft incentive programs, you need to complete enrollment by providing valid payout and tax details.</span></span> <span data-ttu-id="e6ca3-190">Um registro é considerado completo somente quando o pagamento e o perfil de impostos que você fornece são validados pela Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-190">An enrollment is considered complete only when the payout and tax profile you provide is validated by Microsoft.</span></span>

### <a name="how-do-i-know-that-i-need-to-provideupdate-my-payout-andor-tax-details"></a><span data-ttu-id="e6ca3-191">Como fazer saber que preciso fornecer/atualizar meus detalhes de pagamento e/ou imposto?</span><span class="sxs-lookup"><span data-stu-id="e6ca3-191">How do I know that I need to provide/update my payout and/or tax details?</span></span>

<span data-ttu-id="e6ca3-192">Todos os parceiros registrados em um novo programa de incentivo devem fornecer pagamento e detalhes de impostos válidos para concluir o registro.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-192">All partners enrolling in a new incentive program must provide valid payout and tax details to complete the enrollment.</span></span>

<span data-ttu-id="e6ca3-193">Talvez você também precise fornecer informações atualizadas se as regras do seu programa de incentivos forem alteradas ou se os aspectos do perfil expirarem ou ficarem desatualizados.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-193">You may also need to provide updated information if the rules for your incentive program change, or if aspects of the profile expire or become outdated.</span></span> <span data-ttu-id="e6ca3-194">Se isso acontecer, sua página de visão geral mostrará um status de **ação necessária – atualizar banco e/ou perfil de imposto**.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-194">If this happens, your Overview page will show a status of **Action required – Update bank and/or tax profile**.</span></span>

### <a name="how-do-i-provide-update-my-payout-and-or-tax-details"></a><span data-ttu-id="e6ca3-195">Como posso fornecer/atualizar meus detalhes de pagamento e/ou imposto?</span><span class="sxs-lookup"><span data-stu-id="e6ca3-195">How do I provide/ update my payout and/ or tax details?</span></span>

<span data-ttu-id="e6ca3-196">Para obter informações detalhadas sobre como atualizar os detalhes de pagamento e impostos no Partner Center, consulte [como criar e gerenciar perfis bancários e de impostos no Partner Center](https://support.microsoft.com/help/4524534/how-to-create-and-manage-bank-and-tax-profiles-in-partner-center)</span><span class="sxs-lookup"><span data-stu-id="e6ca3-196">For detailed information on how to on how to update payment and tax details in Partner Center, see [How to create and manage bank and tax profiles in Partner Center](https://support.microsoft.com/help/4524534/how-to-create-and-manage-bank-and-tax-profiles-in-partner-center)</span></span>

### <a name="why-dont-i-see-my-enrollments-when-i-go-to-assign-my-payout-and-tax-profile"></a><span data-ttu-id="e6ca3-197">Por que não vejo meus registros ao atribuir meu perfil de pagamento e imposto?</span><span class="sxs-lookup"><span data-stu-id="e6ca3-197">Why don't I see my enrollments when I go to assign my payout and tax profile?</span></span>

<span data-ttu-id="e6ca3-198">Somente os administradores de incentivos do seu local de MPN podem criar ou gerenciar os perfis de pagamento e imposto.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-198">Only incentive admins for your MPN location can create or manage payout and tax profiles.</span></span> <span data-ttu-id="e6ca3-199">Pode ser que você não tenha as permissões adequadas ou que esteja conectado com uma conta que não possui essas permissões.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-199">It could be that you don’t have the proper permissions, or that you’re logged in with an account that does not have these permissions.</span></span> <span data-ttu-id="e6ca3-200">Entre em contato com o administrador da organização para gerenciar as permissões bancárias e fiscais.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-200">Contact your organization administrator to manage permissions for bank and tax.</span></span>

### <a name="where-can-i-see-the-payout-and-tax-profiles-for-my-organization-that-i-can-use"></a><span data-ttu-id="e6ca3-201">Onde posso ver os perfis de pagamento e de impostos da minha organização que posso usar?</span><span class="sxs-lookup"><span data-stu-id="e6ca3-201">Where can I see the payout and tax profiles for my organization that I can use?</span></span>

<span data-ttu-id="e6ca3-202">Use o procedimento a seguir para ver os perfis de pagamento e de impostos:</span><span class="sxs-lookup"><span data-stu-id="e6ca3-202">Use the following procedure to see payout and tax profiles:</span></span>

1. <span data-ttu-id="e6ca3-203">Entre no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-203">Log into Partner Center.</span></span>

2. <span data-ttu-id="e6ca3-204">Selecione o ícone de engrenagem para abrir o menu de **Configurações**.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-204">Select the gear icon to open the **Settings** menu.</span></span>

3. <span data-ttu-id="e6ca3-205">Selecione **configurações de parceiro**.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-205">Select **Partner settings**.</span></span>

4. <span data-ttu-id="e6ca3-206">Em **Configurações da conta**, selecione **Pagamento e taxa**, em seguida, selecione **Perfil de Pagamento e fiscal**.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-206">Under **Account settings**, select **Payout and tax**, and then select **Payout and tax profile**.</span></span> <span data-ttu-id="e6ca3-207">Você verá todos os perfis de pagamento e fiscais existentes junto com o status e a capacidade de editar.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-207">You’ll see all existing payment and tax profiles along with status and ability to edit.</span></span>

### <a name="my-organization-is-participating-in-multiple-incentive-programs-do-i-need-to-provide-my-payment-and-tax-profile-multiple-times"></a><span data-ttu-id="e6ca3-208">Minha organização está participando de vários programas de incentivos.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-208">My organization is participating in multiple incentive programs.</span></span> <span data-ttu-id="e6ca3-209">Preciso fornecer meu pagamento e perfil de impostos várias vezes?</span><span class="sxs-lookup"><span data-stu-id="e6ca3-209">Do I need to provide my payment and tax profile multiple times?</span></span>

<span data-ttu-id="e6ca3-210">Com os perfis de pagamento, geralmente é opção sua.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-210">With payment profiles, it’s usually up to you.</span></span> <span data-ttu-id="e6ca3-211">Os perfis de pagamento são criados em um nível de organização, o que permite que o mesmo perfil de banco seja atribuído a vários programas de incentivo e ID de MPN em uma organização.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-211">Payment profiles are created at an organization level, which allows for the same bank profile to be assigned across multiple MPN ID’s and incentive programs within an organization.</span></span> <span data-ttu-id="e6ca3-212">Na maioria dos casos, você pode reutilizar um perfil existente ou criar um novo.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-212">In most cases, you can either reuse an existing profile or create a new one.</span></span>

<span data-ttu-id="e6ca3-213">No entanto, pode haver exceções ao aplicar seu perfil bancário a diferentes países ou regiões, já que as regras fiscais ou de banco local podem ser aplicadas.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-213">There may be exceptions, however, when applying your bank profile to different countries or regions, as local bank or tax rules may apply.</span></span>

<span data-ttu-id="e6ca3-214">Os perfis fiscais criados para um MPN local são reutilizados e preenchidos automaticamente, quando o mesmo local MPN participa de outro programa de incentivo.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-214">Tax profiles created for an MPN location get reused and automatically populated when the same MPN location participates in other incentive program.</span></span> <span data-ttu-id="e6ca3-215">Mas pode haver exceções.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-215">But there can be exceptions.</span></span> <span data-ttu-id="e6ca3-216">Por exemplo, as regras de pagamento de um novo programa de incentivo podem exigir detalhes adicionais para o perfil fiscal.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-216">For example, the payout rules of a new incentive program may require additional details for the tax profile.</span></span>  

### <a name="i-am-only-able-to-log-in-with-my-onmicrosoftcom-domain-what-should-i-do"></a><span data-ttu-id="e6ca3-217">Só posso fazer logon com meu @onmicrosoft.com domínio.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-217">I am only able to log in with my @onmicrosoft.com domain.</span></span> <span data-ttu-id="e6ca3-218">O que devo fazer?</span><span class="sxs-lookup"><span data-stu-id="e6ca3-218">What should I do?</span></span>

<span data-ttu-id="e6ca3-219">Contate o administrador da conta para adicionar outros domínios à conta do AAD.</span><span class="sxs-lookup"><span data-stu-id="e6ca3-219">Contact your Account administrator to add additional domains to the AAD account.</span></span>
