---
title: Gerenciar locais na sua conta de parceiro
ms.topic: how-to
ms.date: 05/01/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Saiba como adicionar um novo local e como a ID do MPN do local é usada em programas de incentivo, negócios do CSP, assinaturas e outras transações.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8a2b4fa8b204b10d5d45c0e1409ab4bc463e272f
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702885"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a><span data-ttu-id="bd636-103">Gerenciar os locais da sua conta do MPN e adicionar (ou excluir) um local</span><span class="sxs-lookup"><span data-stu-id="bd636-103">Manage your MPN account locations and add (delete) a location</span></span>


<span data-ttu-id="bd636-104">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="bd636-104">**Appropriate roles**</span></span>

- <span data-ttu-id="bd636-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="bd636-105">Global admin</span></span>
- <span data-ttu-id="bd636-106">Administrador de conta</span><span class="sxs-lookup"><span data-stu-id="bd636-106">Account admin</span></span>

<span data-ttu-id="bd636-107">A ID de MPN do local identifica cada local específico de sua empresa.</span><span class="sxs-lookup"><span data-stu-id="bd636-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="bd636-108">Você usa a ID de MPN de local para se registrar em programas de incentivo, para fazer transações com empresas do CSP (Provedor de Soluções na Nuvem) e para fazer outras transações de negócios.</span><span class="sxs-lookup"><span data-stu-id="bd636-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="bd636-109">A ID de MPN global é usada para atividades não transacionais, como solicitações de suporte.</span><span class="sxs-lookup"><span data-stu-id="bd636-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-scenario-is-typical"></a><span data-ttu-id="bd636-110">O seguinte cenário é típico:</span><span class="sxs-lookup"><span data-stu-id="bd636-110">The following scenario is typical:</span></span>

<span data-ttu-id="bd636-111">A Contoso tem sua PGA (Conta global de parceiro) no Reino Unido.</span><span class="sxs-lookup"><span data-stu-id="bd636-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="bd636-112">A PGA é o negócio jurídico registrado deles e a ID global do MPN da empresa é usada para gerenciar todos os negócios não transacionais.</span><span class="sxs-lookup"><span data-stu-id="bd636-112">The PGA is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="bd636-113">A Contoso também tem PLAs (Contas de local de parceiro) equivalentes a subsidiárias ou a divisões em outros locais do Reino Unido, da França e dos EUA.</span><span class="sxs-lookup"><span data-stu-id="bd636-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="bd636-114">Na estrutura de Conta do MPN, essas PLAs são representadas como IDs de MPN de local exclusivas.</span><span class="sxs-lookup"><span data-stu-id="bd636-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="bd636-115">As PLAs são usadas para negócios transacionais, como programas de CSP ou de incentivos.</span><span class="sxs-lookup"><span data-stu-id="bd636-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="bd636-116">Os pagamentos são vinculados a locais específicos.</span><span class="sxs-lookup"><span data-stu-id="bd636-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="bd636-117">Há uma relação um-para-um entre um locatário do CSP e uma ID de local do MPN.</span><span class="sxs-lookup"><span data-stu-id="bd636-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Estrutura dos locais do MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="bd636-119">Pré-requisitos para adicionar uma nova conta para um negócio do CSP</span><span class="sxs-lookup"><span data-stu-id="bd636-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="bd636-120">Para adicionar uma nova conta para o negócio do CSP, primeiro verifique se você cumpre os pré-requisitos.</span><span class="sxs-lookup"><span data-stu-id="bd636-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="bd636-121">É preciso ter uma ID de MPN de local no país em que deseja fazer negócios com o CSP.</span><span class="sxs-lookup"><span data-stu-id="bd636-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="bd636-122">Para criar um novo local de MPN, leia "Adicionar um local de MPN" abaixo.</span><span class="sxs-lookup"><span data-stu-id="bd636-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="bd636-123">Para criar um novo registro de CSP Indirect Reseller, leia [Trabalhar com provedores indiretos](indirect-reseller-tasks-in-partner-center.md#get-started)</span><span class="sxs-lookup"><span data-stu-id="bd636-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="bd636-124">Lembre-se de entrar usando as **novas** credenciais da **nova** conta do CSP.</span><span class="sxs-lookup"><span data-stu-id="bd636-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="bd636-125">Não use suas credenciais existentes, pois o Partner Center reconhecerá que você já tem uma conta.</span><span class="sxs-lookup"><span data-stu-id="bd636-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="bd636-126">Aceite o Contrato de Parceiro da Microsoft e ative a conta.</span><span class="sxs-lookup"><span data-stu-id="bd636-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="bd636-127">Se você quiser se registrar como parceiro de fatura direta, leia [Requisitos para parceiros de fatura direta](direct-partner-new-requirements.md)</span><span class="sxs-lookup"><span data-stu-id="bd636-127">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-and-update-your-mpn-locations"></a><span data-ttu-id="bd636-128">Exibir e atualizar seus locais do MPN</span><span class="sxs-lookup"><span data-stu-id="bd636-128">View and update your MPN locations</span></span>

1. <span data-ttu-id="bd636-129">Entre no [painel](https://partner.microsoft.com/dashboard/home) do Partner Center com suas credenciais da conta do MPN.</span><span class="sxs-lookup"><span data-stu-id="bd636-129">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="bd636-130">(Suas credenciais do MPN podem ser diferentes das credenciais do CSP)</span><span class="sxs-lookup"><span data-stu-id="bd636-130">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="bd636-131">No ícone **Configurações**, selecione **Configurações da conta**, **Perfil da organização**, **Legal**.</span><span class="sxs-lookup"><span data-stu-id="bd636-131">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="bd636-132">Na guia **Parceiro**, verifique se não há uma mensagem de erro de banner solicitando que você corrija os locais migrados do PMC.</span><span class="sxs-lookup"><span data-stu-id="bd636-132">On the **Partner** tab, verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span>  <span data-ttu-id="bd636-133">Se os locais não tiverem sido configurados corretamente no PMC e ainda não tiverem sido transferidos para o PC, será necessário atualizar esses locais.</span><span class="sxs-lookup"><span data-stu-id="bd636-133">If your locations were not set up correctly in PMC, and have not transitioned yet to PC, you need to update those locations.</span></span>

:::image type="content" source="images/locations/location-two.png" alt-text="A captura de tela mostra como atualizar o local.":::
 
4.  <span data-ttu-id="bd636-135">Na tela **Examinar locais do PMC**, selecione **Atualizar**.</span><span class="sxs-lookup"><span data-stu-id="bd636-135">On the **Review PMC locations** screen, select **Update**.</span></span>
<span data-ttu-id="bd636-136">Atualize os seguintes campos:</span><span class="sxs-lookup"><span data-stu-id="bd636-136">Update the following fields:</span></span>

- <span data-ttu-id="bd636-137">**Campo Nome**: verifique se o nome do local da empresa está correto.</span><span class="sxs-lookup"><span data-stu-id="bd636-137">**Name field**: Make sure that the name of the company location is correct.</span></span> <span data-ttu-id="bd636-138">Se for exibido um erro de duplicação, tente mudar, por exemplo, de Contoso para Contoso, Inc.</span><span class="sxs-lookup"><span data-stu-id="bd636-138">If a duplicate error is displayed, try changing from, for example, Contoso to Contoso, Inc.</span></span>

- <span data-ttu-id="bd636-139">**Campo Pessoa jurídica**: verifique se você escolheu a pessoa jurídica à qual o local está vinculado</span><span class="sxs-lookup"><span data-stu-id="bd636-139">**Legal Entity field**: Make sure that you have chosen the legal entity the location is tied to</span></span>

- <span data-ttu-id="bd636-140">**Campos Linhas 1 e 2 de endereço**: verifique se o endereço está correto</span><span class="sxs-lookup"><span data-stu-id="bd636-140">**Address line 1 & 2 fields**: Make sure that the address is correct</span></span>

- <span data-ttu-id="bd636-141">**Campos Cidade e Estado/Província**: verifique se a combinação entre cidade e estado/província está correta.</span><span class="sxs-lookup"><span data-stu-id="bd636-141">**City & State/Province fields**: Make sure the combination between the city and the state/province is correct.</span></span> <span data-ttu-id="bd636-142">Para alguns países, será fornecido um menu suspenso para escolha de estado/província; para outros países, esse campo deverá ser preenchido manualmente.</span><span class="sxs-lookup"><span data-stu-id="bd636-142">There are countries where the dropdown menu for choosing the State/Province will apply, and in other countries that field will need to manually be inserted.</span></span>

- <span data-ttu-id="bd636-143">**Campo CEP/Código postal**: verifique se o campo CEP corresponde ao país, à região, à cidade ou ao endereço indicado.</span><span class="sxs-lookup"><span data-stu-id="bd636-143">**ZIP/ Postal code field**: Make sure the Zip Code field is matching your indicated Country, Region, City, or Address.</span></span>

- <span data-ttu-id="bd636-144">**Campos de Informações de contato principal**: verifique se os campos Nome e Sobrenome estão preenchidos e se o endereço de email indicado é de trabalho e não pessoal (por exemplo: @outlook.com, @live.com etc.)</span><span class="sxs-lookup"><span data-stu-id="bd636-144">**Primary contact information fields**: Make sure the first and last name fields are filled and that the e-mail address indicated is a work e-mail address and not a personal one (for example, @outlook.com, @live.com, etc.)</span></span>

- <span data-ttu-id="bd636-145">**Campo Número de telefone**: verifique se o número de telefone NÃO contém caracteres especiais, espaços ou o código do país.</span><span class="sxs-lookup"><span data-stu-id="bd636-145">**Phone number field**: Make sure that the Phone number does NOT include special characters, spaces, or country code.</span></span> <span data-ttu-id="bd636-146">O valor inserido no campo Número de telefone deverá conter sempre o máximo de 10 caracteres.</span><span class="sxs-lookup"><span data-stu-id="bd636-146">The value entered in the Phone Number field will always contain a maximum of 10 characters.</span></span>

5. <span data-ttu-id="bd636-147">Se não houver uma mensagem de erro, em **Configurações**, selecione **Configurações da Conta**, **Perfil da organização**, **Identificadores**.</span><span class="sxs-lookup"><span data-stu-id="bd636-147">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

6. <span data-ttu-id="bd636-148">Localize a ID do MPN com o tipo "Local" que corresponde ao país dessa conta do CSP e use-a para concluir a associação.</span><span class="sxs-lookup"><span data-stu-id="bd636-148">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to complete the association.</span></span>

7. <span data-ttu-id="bd636-149">Se você não encontrar a ID do MPN do local que corresponda à conta do CSP que você deseja usar, será possível adicionar um local, que criará uma ID do MPN.</span><span class="sxs-lookup"><span data-stu-id="bd636-149">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location, which will create a new MPN ID.</span></span> <span data-ttu-id="bd636-150">Confira **Adicionar um local do MPN** abaixo.</span><span class="sxs-lookup"><span data-stu-id="bd636-150">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="bd636-151">Adicionar um local do MPN</span><span class="sxs-lookup"><span data-stu-id="bd636-151">Add an MPN location</span></span>

1. <span data-ttu-id="bd636-152">Entre usando a conta do MPN no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="bd636-152">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="bd636-153">(Suas credenciais do MPN podem ser diferentes das credenciais do CSP).</span><span class="sxs-lookup"><span data-stu-id="bd636-153">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="bd636-154">A conta MPN deve ter privilégios de administrador global ou de administrador de conta.</span><span class="sxs-lookup"><span data-stu-id="bd636-154">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="bd636-155">No **ícone Configurações**, selecione as **Configurações da conta** e o **Perfil da organização**.</span><span class="sxs-lookup"><span data-stu-id="bd636-155">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="bd636-156">Selecione **Legal** e, em seguida, na guia **Parceiro**, escolha **Localizações da empresa** e clique em **Adicionar um local**.</span><span class="sxs-lookup"><span data-stu-id="bd636-156">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="bd636-157">Insira as informações necessárias, como nome da empresa, endereço e contato do local que você quer adicionar à empresa.</span><span class="sxs-lookup"><span data-stu-id="bd636-157">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="bd636-158">Clique em **Adicionar local**.</span><span class="sxs-lookup"><span data-stu-id="bd636-158">Click **Add location**.</span></span> <span data-ttu-id="bd636-159">Isso criará uma nova ID de MPN para o novo local que você pode usar para transações e incentivos do CSP.</span><span class="sxs-lookup"><span data-stu-id="bd636-159">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Adicionar uma nova pessoa jurídica":::

> [!NOTE]
> <span data-ttu-id="bd636-161">Depois que um local for adicionado no Partner Center, você não poderá removê-lo.</span><span class="sxs-lookup"><span data-stu-id="bd636-161">Once a location is added in Partner Center, you cannot remove it.</span></span> <span data-ttu-id="bd636-162">Você verá **MPN** no menu à esquerda do Partner Center se tiver usado a ID de MPN correta para entrar.</span><span class="sxs-lookup"><span data-stu-id="bd636-162">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="add-the-registration-number-id"></a><span data-ttu-id="bd636-163">Adicionar a ID do número de registro</span><span class="sxs-lookup"><span data-stu-id="bd636-163">Add the registration number ID</span></span>

<span data-ttu-id="bd636-164">Se você for um provedor indireto, parceiro de cobrança direto ou revendedor indireto e estiver fazendo negócios com clientes novos ou existentes nos países a seguir, será necessário fornecer números de ID de registro para sua empresa.</span><span class="sxs-lookup"><span data-stu-id="bd636-164">If you are an Indirect provider, Direct bill partner, or Indirect reseller and you are doing business with new or existing customers in the following countries, you need to provide registration ID numbers for your business.</span></span> <span data-ttu-id="bd636-165">Se o país onde você está fazendo negócios não estiver listado abaixo, a ID de registro será opcional.</span><span class="sxs-lookup"><span data-stu-id="bd636-165">If the country you are doing business in is not listed below, the registration ID is optional.</span></span>

- <span data-ttu-id="bd636-166">Armênia</span><span class="sxs-lookup"><span data-stu-id="bd636-166">Armenia</span></span> 
- <span data-ttu-id="bd636-167">Azerbaijão</span><span class="sxs-lookup"><span data-stu-id="bd636-167">Azerbaijan</span></span> 
- <span data-ttu-id="bd636-168">Bielorrússia</span><span class="sxs-lookup"><span data-stu-id="bd636-168">Belarus</span></span> 
- <span data-ttu-id="bd636-169">Brasil</span><span class="sxs-lookup"><span data-stu-id="bd636-169">Brazil</span></span> 
- <span data-ttu-id="bd636-170">Hungria</span><span class="sxs-lookup"><span data-stu-id="bd636-170">Hungary</span></span> 
- <span data-ttu-id="bd636-171">Índia</span><span class="sxs-lookup"><span data-stu-id="bd636-171">India</span></span> 
- <span data-ttu-id="bd636-172">Iraque</span><span class="sxs-lookup"><span data-stu-id="bd636-172">Iraq</span></span> 
- <span data-ttu-id="bd636-173">Cazaquistão</span><span class="sxs-lookup"><span data-stu-id="bd636-173">Kazakhstan</span></span> 
- <span data-ttu-id="bd636-174">Quirguistão</span><span class="sxs-lookup"><span data-stu-id="bd636-174">Kyrgyzstan</span></span> 
- <span data-ttu-id="bd636-175">Moldova</span><span class="sxs-lookup"><span data-stu-id="bd636-175">Moldova</span></span> 
- <span data-ttu-id="bd636-176">Myanmar</span><span class="sxs-lookup"><span data-stu-id="bd636-176">Myanmar</span></span> 
- <span data-ttu-id="bd636-177">Polônia</span><span class="sxs-lookup"><span data-stu-id="bd636-177">Poland</span></span> 
- <span data-ttu-id="bd636-178">Rússia</span><span class="sxs-lookup"><span data-stu-id="bd636-178">Russia</span></span> 
- <span data-ttu-id="bd636-179">Arábia Saudita</span><span class="sxs-lookup"><span data-stu-id="bd636-179">Saudi Arabia</span></span> 
- <span data-ttu-id="bd636-180">África do Sul</span><span class="sxs-lookup"><span data-stu-id="bd636-180">South Africa</span></span> 
- <span data-ttu-id="bd636-181">Sudão do Sul</span><span class="sxs-lookup"><span data-stu-id="bd636-181">South Sudan</span></span>  
- <span data-ttu-id="bd636-182">Tadjiquistão</span><span class="sxs-lookup"><span data-stu-id="bd636-182">Tajikistan</span></span> 
- <span data-ttu-id="bd636-183">Tailândia</span><span class="sxs-lookup"><span data-stu-id="bd636-183">Thailand</span></span>
- <span data-ttu-id="bd636-184">Turquia</span><span class="sxs-lookup"><span data-stu-id="bd636-184">Turkey</span></span> 
- <span data-ttu-id="bd636-185">Ucrânia</span><span class="sxs-lookup"><span data-stu-id="bd636-185">Ukraine</span></span> 
- <span data-ttu-id="bd636-186">Emirados Árabes Unidos</span><span class="sxs-lookup"><span data-stu-id="bd636-186">United Arab Emirates</span></span> 
- <span data-ttu-id="bd636-187">Uzbequistão</span><span class="sxs-lookup"><span data-stu-id="bd636-187">Uzbekistan</span></span> 
- <span data-ttu-id="bd636-188">Venezuela</span><span class="sxs-lookup"><span data-stu-id="bd636-188">Venezuela</span></span>
- <span data-ttu-id="bd636-189">Vietnã</span><span class="sxs-lookup"><span data-stu-id="bd636-189">Vietnam</span></span> 


<span data-ttu-id="bd636-190">Para obter mais informações, leia [Informações do número da ID de registro](reg-number-id.md)</span><span class="sxs-lookup"><span data-stu-id="bd636-190">For more information, read [Registration ID number information](reg-number-id.md)</span></span>

## <a name="delete-a-location"></a><span data-ttu-id="bd636-191">Excluir um local</span><span class="sxs-lookup"><span data-stu-id="bd636-191">Delete a location</span></span>

<span data-ttu-id="bd636-192">Para excluir um local da sua conta, será necessário entrar em contato com o [Suporte a Parceiros](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span><span class="sxs-lookup"><span data-stu-id="bd636-192">To delete a location from your account, you will need to contact [Partner Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span></span> <span data-ttu-id="bd636-193">Verifique se você entendeu o impacto que essa ação tem.</span><span class="sxs-lookup"><span data-stu-id="bd636-193">Make sure that you understand the impact this action has.</span></span> <span data-ttu-id="bd636-194">Os locais excluídos não podem ser recuperados e qualquer coisa associada a essa ID de MPN específica não será mais reconhecida nem estará ativa para sua empresa.</span><span class="sxs-lookup"><span data-stu-id="bd636-194">Deleted locations cannot be retrieved and anything tied to that specific MPN id will no longer be recognized or be active for your company.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="bd636-195">Alterar o país da conta global do parceiro</span><span class="sxs-lookup"><span data-stu-id="bd636-195">Change country of Partner global account</span></span> 

1. <span data-ttu-id="bd636-196">Entre usando a conta do MPN no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="bd636-196">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="bd636-197">(Suas credenciais do MPN podem ser diferentes das credenciais do CSP).</span><span class="sxs-lookup"><span data-stu-id="bd636-197">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="bd636-198">A conta MPN deve ter privilégios de administrador global ou de administrador de conta.</span><span class="sxs-lookup"><span data-stu-id="bd636-198">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="bd636-199">Na guia **Parceiro**, acesse **Localizações da empresa** e confira a lista de locais para garantir que o local que você quer como pessoa jurídica esteja listado.</span><span class="sxs-lookup"><span data-stu-id="bd636-199">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="bd636-200">Para adicionar um local, clique em **Adicionar um local** e, no submenu, insira as informações necessárias, como nome da empresa, endereço e contato principal do local que você quer adicionar à empresa.</span><span class="sxs-lookup"><span data-stu-id="bd636-200">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="bd636-201">Selecione **Alterar seu país** ao lado do menu suspenso **País/região** e siga as etapas.</span><span class="sxs-lookup"><span data-stu-id="bd636-201">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Submenu de dados do perfil de pessoa jurídica":::

5. <span data-ttu-id="bd636-203">Clique em **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="bd636-203">Click **Save**.</span></span>

6. <span data-ttu-id="bd636-204">O país da conta global MPN será alterado para o novo país legal.</span><span class="sxs-lookup"><span data-stu-id="bd636-204">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="bd636-205">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="bd636-205">Next steps</span></span>

- <span data-ttu-id="bd636-206">Saiba mais sobre o [processo de verificação](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="bd636-206">Learn about the [verification process](verification-responses.md).</span></span>
