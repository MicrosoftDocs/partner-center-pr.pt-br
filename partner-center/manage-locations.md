---
title: Gerenciar locais na sua conta de parceiro
ms.topic: how-to
ms.date: 01/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Saiba como adicionar um novo local e como a ID do MPN do local é usada em programas de incentivo, negócios do CSP, assinaturas e outras transações.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 38ea8a451f51d80998643e2a023420ea3efaa6ba
ms.sourcegitcommit: e99882e9b6c9b1a0f7427fb133693b1d977be76b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "98773422"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="afd6a-103">Gerenciar os locais de sua conta do MPN e adicionar um novo local</span><span class="sxs-lookup"><span data-stu-id="afd6a-103">Manage your MPN account locations and add a new location</span></span>


<span data-ttu-id="afd6a-104">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="afd6a-104">**Appropriate roles**</span></span>

- <span data-ttu-id="afd6a-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="afd6a-105">Global admin</span></span>
- <span data-ttu-id="afd6a-106">Administrador de conta</span><span class="sxs-lookup"><span data-stu-id="afd6a-106">Account admin</span></span>

<span data-ttu-id="afd6a-107">A ID de MPN do local identifica cada local específico de sua empresa.</span><span class="sxs-lookup"><span data-stu-id="afd6a-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="afd6a-108">Você usa a ID de MPN de local para se registrar em programas de incentivo, para fazer transações com empresas do CSP (Provedor de Soluções na Nuvem) e para fazer outras transações de negócios.</span><span class="sxs-lookup"><span data-stu-id="afd6a-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="afd6a-109">A ID de MPN global é usada para atividades não transacionais, como solicitações de suporte.</span><span class="sxs-lookup"><span data-stu-id="afd6a-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="afd6a-110">O seguinte é um cenário típico:</span><span class="sxs-lookup"><span data-stu-id="afd6a-110">The following is a typical scenario:</span></span>

<span data-ttu-id="afd6a-111">A Contoso tem sua PGA (Conta global de parceiro) no Reino Unido.</span><span class="sxs-lookup"><span data-stu-id="afd6a-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="afd6a-112">Trata-se de seus negócios jurídicos registrados e sua ID de MPN global é usada para gerenciar todos os negócios não transacionais.</span><span class="sxs-lookup"><span data-stu-id="afd6a-112">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="afd6a-113">A Contoso também tem PLAs (Contas de local de parceiro) equivalentes a subsidiárias ou a divisões em outros locais do Reino Unido, da França e dos EUA.</span><span class="sxs-lookup"><span data-stu-id="afd6a-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="afd6a-114">Na estrutura de Conta do MPN, essas PLAs são representadas como IDs de MPN de local exclusivas.</span><span class="sxs-lookup"><span data-stu-id="afd6a-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="afd6a-115">As PLAs são usadas para negócios transacionais, como programas de CSP ou de incentivos.</span><span class="sxs-lookup"><span data-stu-id="afd6a-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="afd6a-116">Os pagamentos são vinculados a locais específicos.</span><span class="sxs-lookup"><span data-stu-id="afd6a-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="afd6a-117">Há uma relação um-para-um entre um locatário do CSP e uma ID de local do MPN.</span><span class="sxs-lookup"><span data-stu-id="afd6a-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Estrutura dos locais do MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-location-for-a-csp-business"></a><span data-ttu-id="afd6a-119">Pré-requisitos para adicionar um novo local de conta para um negócio do CSP</span><span class="sxs-lookup"><span data-stu-id="afd6a-119">Prerequisites in order to add a new account location for a CSP business</span></span>

<span data-ttu-id="afd6a-120">Para adicionar um novo local para um negócio do CSP, há vários pré-requisitos:</span><span class="sxs-lookup"><span data-stu-id="afd6a-120">To add a new CSP business location, there are several prerequisites:</span></span>

1. <span data-ttu-id="afd6a-121">Você precisa ter uma ID de MPN de local no país em que deseja fazer negócios.</span><span class="sxs-lookup"><span data-stu-id="afd6a-121">You must have a location MPN ID in the country where you want to do business.</span></span>

1. <span data-ttu-id="afd6a-122">Você precisa de um novo locatário do Azure AD na [região de negócios](regional-authorization-overview.md) que ainda não esteja inscrito no CSP.</span><span class="sxs-lookup"><span data-stu-id="afd6a-122">You need a new Azure AD tenant in the [region of business](regional-authorization-overview.md) which is not already enrolled into CSP.</span></span> <span data-ttu-id="afd6a-123">Crie-o ao se registrar no CSP.</span><span class="sxs-lookup"><span data-stu-id="afd6a-123">Create this when you enroll in CSP.</span></span>
 
3. <span data-ttu-id="afd6a-124">Use o novo locatário do AAD para se registrar no programa CSP na região.</span><span class="sxs-lookup"><span data-stu-id="afd6a-124">Use the new AAD tenant to enroll into CSP program in the region.</span></span>
<span data-ttu-id="afd6a-125">Fornecer detalhes legais da empresa, incluindo o nome jurídico da empresa, o endereço e os detalhes do contato principal.</span><span class="sxs-lookup"><span data-stu-id="afd6a-125">Providing legal company details including the legal company name, address, primary contact details.</span></span> <span data-ttu-id="afd6a-126">Essa conta passará por verificação, portanto, certifique-se de adicionar informações válidas.</span><span class="sxs-lookup"><span data-stu-id="afd6a-126">This account will undergo verification, so make sure to add valid information.</span></span>

>[!NOTE] 
 ><span data-ttu-id="afd6a-127">Lembre-se de entrar usando as **novas** credenciais do **novo** locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="afd6a-127">Remember to sign in with the **new** credentials for the **new** Azure AD tenant.</span></span> <span data-ttu-id="afd6a-128">Não use suas credenciais existentes, pois o Partner Center reconhecerá que você já tem uma conta.</span><span class="sxs-lookup"><span data-stu-id="afd6a-128">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

4. <span data-ttu-id="afd6a-129">Aceite o Contrato de Parceiro da Microsoft e ative a conta.</span><span class="sxs-lookup"><span data-stu-id="afd6a-129">Accept the Microsoft Partner Agreement and activate the account.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="afd6a-130">Adicionar um local do MPN</span><span class="sxs-lookup"><span data-stu-id="afd6a-130">Add an MPN location</span></span>

1. <span data-ttu-id="afd6a-131">Entre usando a conta do MPN no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="afd6a-131">Sign in using the MPN account in Partner Center .</span></span> <span data-ttu-id="afd6a-132">A conta MPN deve ter privilégios de administrador global ou de administrador de conta.</span><span class="sxs-lookup"><span data-stu-id="afd6a-132">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="afd6a-133">No **ícone Configuração**, selecione as **Configurações da organização**.</span><span class="sxs-lookup"><span data-stu-id="afd6a-133">From the **Setting icon**, select the **Organization settings**.</span></span>

2. <span data-ttu-id="afd6a-134">Selecione **Jurídico** e **Locais.**</span><span class="sxs-lookup"><span data-stu-id="afd6a-134">Select **Legal** and then select **Locations.**</span></span>

3. <span data-ttu-id="afd6a-135">Selecione **Adicionar um local** e insira os detalhes do endereço do local que você deseja adicionar à sua empresa, bem como um contato principal para o local.</span><span class="sxs-lookup"><span data-stu-id="afd6a-135">Select **Add a location**, and insert the address details of the location that you want to add to your company as well as a primary contact for the location.</span></span>

> [!NOTE]
> <span data-ttu-id="afd6a-136">Depois que um local for adicionado no Partner Center, ele não poderá ser removido.</span><span class="sxs-lookup"><span data-stu-id="afd6a-136">Once a location is added in Partner Center, it cannot be removed.</span></span> <span data-ttu-id="afd6a-137">Você verá **MPN** no menu à esquerda do Partner Center se tiver usado a ID de MPN correta para entrar.</span><span class="sxs-lookup"><span data-stu-id="afd6a-137">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="change-global-partner-account-location"></a><span data-ttu-id="afd6a-138">Alterar o local da Conta de parceiro global</span><span class="sxs-lookup"><span data-stu-id="afd6a-138">Change Global partner account location</span></span>

1. <span data-ttu-id="afd6a-139">Em **[Local da empresa](https://partner.microsoft.com/dashboard/account/v3/organization/legalinfo#mpn)** , confira a lista de locais para garantir que o local que você quer como pessoa jurídica esteja listado.</span><span class="sxs-lookup"><span data-stu-id="afd6a-139">On **[Business locations](https://partner.microsoft.com/dashboard/account/v3/organization/legalinfo#mpn)**, check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> <span data-ttu-id="afd6a-140">Se não estiver, adicione-o.</span><span class="sxs-lookup"><span data-stu-id="afd6a-140">If it isn't, add it.</span></span>

   :::image type="content" source="images/accountsettings/location1.png" alt-text="Captura de tela da página Locais da Conta do Partner Center com a lista de todos os locais atuais.":::

2. <span data-ttu-id="afd6a-142">Selecione **Jurídico** e depois **Atualizar perfil de negócios jurídico**</span><span class="sxs-lookup"><span data-stu-id="afd6a-142">Select **Legal** and then select **Update legal business profile**</span></span>
  
3. <span data-ttu-id="afd6a-143">Selecione a região e a pessoa jurídica e **Envie-a**.</span><span class="sxs-lookup"><span data-stu-id="afd6a-143">Select the region and legal entity and **Submit** it.</span></span>

  
## <a name="next-steps"></a><span data-ttu-id="afd6a-144">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="afd6a-144">Next steps</span></span>

- <span data-ttu-id="afd6a-145">Saiba mais sobre o [processo de verificação](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="afd6a-145">Learn about the [verification process](verification-responses.md).</span></span>
