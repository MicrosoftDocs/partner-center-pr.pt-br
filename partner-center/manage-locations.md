---
title: Gerenciar locais na sua conta de parceiro
ms.topic: article
ms.date: 10/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Saiba como adicionar um novo local e como a ID do MPN do local é usada em programas de incentivo, negócios do CSP, assinaturas e outras transações.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c4435227cdd5d777d11c79bf4adc63471ad925e9
ms.sourcegitcommit: 940dad4527f51781f6f966e196b3aa08389613a2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/13/2020
ms.locfileid: "92006853"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="8cea8-103">Gerenciar os locais de sua conta do MPN e adicionar um novo local</span><span class="sxs-lookup"><span data-stu-id="8cea8-103">Manage your MPN account locations and add a new location</span></span>

<span data-ttu-id="8cea8-104">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="8cea8-104">**Applies to**</span></span>

- <span data-ttu-id="8cea8-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="8cea8-105">Partner Center</span></span>

<span data-ttu-id="8cea8-106">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="8cea8-106">**Appropriate roles**</span></span>

- <span data-ttu-id="8cea8-107">Administrador global</span><span class="sxs-lookup"><span data-stu-id="8cea8-107">Global admin</span></span>
- <span data-ttu-id="8cea8-108">Administrador de conta</span><span class="sxs-lookup"><span data-stu-id="8cea8-108">Account admin</span></span>

<span data-ttu-id="8cea8-109">A ID de MPN do local identifica cada local específico de sua empresa.</span><span class="sxs-lookup"><span data-stu-id="8cea8-109">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="8cea8-110">Você usa a ID de MPN de local para se registrar em programas de incentivo, para fazer transações com empresas do CSP (Provedor de Soluções na Nuvem) e para fazer outras transações de negócios.</span><span class="sxs-lookup"><span data-stu-id="8cea8-110">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="8cea8-111">A ID de MPN global é usada para atividades não transacionais, como solicitações de suporte.</span><span class="sxs-lookup"><span data-stu-id="8cea8-111">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="8cea8-112">O seguinte é um cenário típico:</span><span class="sxs-lookup"><span data-stu-id="8cea8-112">The following is a typical scenario:</span></span>

<span data-ttu-id="8cea8-113">A Contoso tem sua PGA (Conta global de parceiro) no Reino Unido.</span><span class="sxs-lookup"><span data-stu-id="8cea8-113">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="8cea8-114">Trata-se de seus negócios jurídicos registrados e sua ID de MPN global é usada para gerenciar todos os negócios não transacionais.</span><span class="sxs-lookup"><span data-stu-id="8cea8-114">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="8cea8-115">A Contoso também tem PLAs (Contas de local de parceiro) equivalentes a subsidiárias ou a divisões em outros locais do Reino Unido, da França e dos EUA.</span><span class="sxs-lookup"><span data-stu-id="8cea8-115">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="8cea8-116">Na estrutura de Conta do MPN, essas PLAs são representadas como IDs de MPN de local exclusivas.</span><span class="sxs-lookup"><span data-stu-id="8cea8-116">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="8cea8-117">As PLAs são usadas para negócios transacionais, como programas de CSP ou de incentivos.</span><span class="sxs-lookup"><span data-stu-id="8cea8-117">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="8cea8-118">Os pagamentos são vinculados a locais específicos.</span><span class="sxs-lookup"><span data-stu-id="8cea8-118">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="8cea8-119">Há uma relação um-para-um entre um locatário do CSP e uma ID de local do MPN.</span><span class="sxs-lookup"><span data-stu-id="8cea8-119">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Estrutura dos locais do MPN":::

## <a name="prerequisites-in-order-to-add-a-new-location-for-a-csp-business"></a><span data-ttu-id="8cea8-121">Pré-requisitos para adicionar um novo local para um negócio do CSP</span><span class="sxs-lookup"><span data-stu-id="8cea8-121">Prerequisites in order to add a new location for a CSP business</span></span>

<span data-ttu-id="8cea8-122">Para adicionar um novo local para um negócio do CSP, há vários pré-requisitos:</span><span class="sxs-lookup"><span data-stu-id="8cea8-122">To add a new CSP business location, there are several prerequisites:</span></span>

1. <span data-ttu-id="8cea8-123">Você precisa ter uma ID de MPN de local no país em que deseja fazer negócios.</span><span class="sxs-lookup"><span data-stu-id="8cea8-123">You must have a location MPN ID in the country where you want to do business.</span></span>

1. <span data-ttu-id="8cea8-124">Você precisa de um novo locatário do Azure AD na [região de negócios](regional-authorization-overview.md) que ainda não esteja inscrito no CSP.</span><span class="sxs-lookup"><span data-stu-id="8cea8-124">You need a new Azure AD tenant in the [region of business](regional-authorization-overview.md) which is not already enrolled into CSP.</span></span> <span data-ttu-id="8cea8-125">Crie-o ao se registrar no CSP.</span><span class="sxs-lookup"><span data-stu-id="8cea8-125">Create this when you enroll in CSP.</span></span>
 
3. <span data-ttu-id="8cea8-126">Use o novo locatário do AAD para se registrar no programa CSP na região.</span><span class="sxs-lookup"><span data-stu-id="8cea8-126">Use the new AAD tenant to enroll into CSP program in the region.</span></span>
<span data-ttu-id="8cea8-127">Fornecer detalhes legais da empresa, incluindo o nome jurídico da empresa, o endereço e os detalhes do contato principal.</span><span class="sxs-lookup"><span data-stu-id="8cea8-127">Providing legal company details including the legal company name, address, primary contact details.</span></span> <span data-ttu-id="8cea8-128">Essa conta passará por verificação, portanto, certifique-se de adicionar informações válidas.</span><span class="sxs-lookup"><span data-stu-id="8cea8-128">This account will undergo verification, so make sure to add valid information.</span></span>

>[!NOTE] 
 ><span data-ttu-id="8cea8-129">Lembre-se de entrar usando as **novas** credenciais do **novo** locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8cea8-129">Remember to sign in with the **new** credentials for the **new** Azure AD tenant.</span></span> <span data-ttu-id="8cea8-130">Não use suas credenciais existentes, pois o Partner Center reconhecerá que você já tem uma conta.</span><span class="sxs-lookup"><span data-stu-id="8cea8-130">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

4. <span data-ttu-id="8cea8-131">Aceite o Contrato de Parceiro da Microsoft e ative a conta.</span><span class="sxs-lookup"><span data-stu-id="8cea8-131">Accept the Microsoft Partner Agreement and activate the account.</span></span>

## <a name="add-a-location"></a><span data-ttu-id="8cea8-132">Adicionar um local</span><span class="sxs-lookup"><span data-stu-id="8cea8-132">Add a location</span></span>

1. <span data-ttu-id="8cea8-133">Entre usando a conta do MPN no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="8cea8-133">Sign in using the MPN account in Partner Center .</span></span> <span data-ttu-id="8cea8-134">A conta MPN deve ter privilégios de administrador global ou de administrador de conta.</span><span class="sxs-lookup"><span data-stu-id="8cea8-134">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="8cea8-135">No **ícone Configuração**, selecione as **Configurações do parceiro**.</span><span class="sxs-lookup"><span data-stu-id="8cea8-135">From the **Setting icon**, select the **Partner settings**.</span></span>

2. <span data-ttu-id="8cea8-136">Selecione **Locais.**</span><span class="sxs-lookup"><span data-stu-id="8cea8-136">Select **Locations.**</span></span>

3. <span data-ttu-id="8cea8-137">Selecione **Adicionar um local** e insira os detalhes do endereço do local que você deseja adicionar à sua empresa, bem como um contato principal para o local.</span><span class="sxs-lookup"><span data-stu-id="8cea8-137">Select **Add a location**, and insert the address details of the location that you want to add to your company as well as a primary contact for the location.</span></span>

> [!NOTE]
> <span data-ttu-id="8cea8-138">Depois que um local for adicionado no Partner Center, ele não poderá ser removido.</span><span class="sxs-lookup"><span data-stu-id="8cea8-138">Once a location is added in Partner Center, it cannot be removed.</span></span> <span data-ttu-id="8cea8-139">Você verá **MPN** no menu à esquerda do Partner Center se tiver usado a ID de MPN correta para entrar.</span><span class="sxs-lookup"><span data-stu-id="8cea8-139">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="change-global-partner-account-location"></a><span data-ttu-id="8cea8-140">Alterar o local da Conta de parceiro global</span><span class="sxs-lookup"><span data-stu-id="8cea8-140">Change Global partner account location</span></span>

1. <span data-ttu-id="8cea8-141">Na página **[Locais](https://partner.microsoft.com/pcv/accountsettings/locationsprofile)** , confira a lista de locais para verificar se o local que você deseja como pessoa jurídica está listado.</span><span class="sxs-lookup"><span data-stu-id="8cea8-141">On the **[Locations](https://partner.microsoft.com/pcv/accountsettings/locationsprofile)** page, check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> <span data-ttu-id="8cea8-142">Se não estiver, adicione-o.</span><span class="sxs-lookup"><span data-stu-id="8cea8-142">If it isn't, add it.</span></span>

   :::image type="content" source="images/updatepartnerprofile2.png" alt-text="Estrutura dos locais do MPN":::

2. <span data-ttu-id="8cea8-144">Selecione **Perfil do parceiro** e, em seguida, **Atualizar perfil de negócios jurídico**</span><span class="sxs-lookup"><span data-stu-id="8cea8-144">Select **Partner profile** and then select **Update legal business profile**</span></span>

   :::image type="content" source="images/updatepartnerprofile1.png" alt-text="Estrutura dos locais do MPN":::

3. <span data-ttu-id="8cea8-146">Selecione a região e a pessoa jurídica e **Envie-a**.</span><span class="sxs-lookup"><span data-stu-id="8cea8-146">Select the region and legal entity and **Submit** it.</span></span>

   :::image type="content" source="images/updatepartnerprofile3.png" alt-text="Estrutura dos locais do MPN":::

## <a name="next-steps"></a><span data-ttu-id="8cea8-148">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="8cea8-148">Next steps</span></span>

- <span data-ttu-id="8cea8-149">Saiba mais sobre o [processo de verificação](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="8cea8-149">Learn about the [verification process](verification-responses.md).</span></span>
