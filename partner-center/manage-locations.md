---
title: Gerenciar locais na sua conta de parceiro
ms.topic: article
ms.date: 10/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Saiba como adicionar um novo local e como a ID do MPN do local é usada em programas de incentivo, negócios do CSP, assinaturas e outras transações.
author: vinayks
ms.author: vinayks
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: c9bc3ffc09b657ab6e3e7e2dcda576898c96803d
ms.sourcegitcommit: d9c7890520ecd37a7651e976d540cfe65c51be54
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2020
ms.locfileid: "91663887"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="41381-103">Gerenciar os locais de sua conta do MPN e adicionar um novo local</span><span class="sxs-lookup"><span data-stu-id="41381-103">Manage your MPN account locations and add a new location</span></span>

<span data-ttu-id="41381-104">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="41381-104">**Applies to**</span></span>

- <span data-ttu-id="41381-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="41381-105">Partner Center</span></span>

<span data-ttu-id="41381-106">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="41381-106">**Appropriate roles**</span></span>

- <span data-ttu-id="41381-107">Administrador global</span><span class="sxs-lookup"><span data-stu-id="41381-107">Global admin</span></span>
- <span data-ttu-id="41381-108">Administrador de conta</span><span class="sxs-lookup"><span data-stu-id="41381-108">Account admin</span></span>

<span data-ttu-id="41381-109">A ID de MPN do local identifica cada local específico de sua empresa.</span><span class="sxs-lookup"><span data-stu-id="41381-109">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="41381-110">Você usa a ID de MPN de local para se registrar em programas de incentivo, para fazer transações com empresas do CSP (Provedor de Soluções na Nuvem) e para fazer outras transações de negócios.</span><span class="sxs-lookup"><span data-stu-id="41381-110">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="41381-111">A ID de MPN global é usada para atividades não transacionais, como solicitações de suporte.</span><span class="sxs-lookup"><span data-stu-id="41381-111">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="41381-112">O seguinte é um cenário típico:</span><span class="sxs-lookup"><span data-stu-id="41381-112">The following is a typical scenario:</span></span>

<span data-ttu-id="41381-113">O local da PGA (Conta global de parceiro) da Contoso é no Reino Unido.</span><span class="sxs-lookup"><span data-stu-id="41381-113">Contoso has its Partner global account (PGA) location in the UK.</span></span> <span data-ttu-id="41381-114">Trata-se da empresa com registro jurídico, que tem uma ID de MPN usada para gerenciar todos os negócios não transacionais.</span><span class="sxs-lookup"><span data-stu-id="41381-114">This is their registered legal business, and it has one MPN ID used for managing all non-transactional business.</span></span> <span data-ttu-id="41381-115">A Contoso também tem PLAs (Contas de local de parceiro) equivalentes a subsidiárias ou a divisões em outros locais do Reino Unido, da França e dos EUA.</span><span class="sxs-lookup"><span data-stu-id="41381-115">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="41381-116">Na estrutura de Conta do MPN, essas PLAs são representadas como IDs de MPN de local exclusivas.</span><span class="sxs-lookup"><span data-stu-id="41381-116">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="41381-117">As PLAs são usadas para negócios transacionais, como programas de CSP ou de incentivos.</span><span class="sxs-lookup"><span data-stu-id="41381-117">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="41381-118">Os pagamentos são vinculados a locais específicos.</span><span class="sxs-lookup"><span data-stu-id="41381-118">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="41381-119">Há uma relação um-para-um entre um locatário do CSP e uma ID de local do MPN.</span><span class="sxs-lookup"><span data-stu-id="41381-119">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/accountsettings/accountstructure.png" alt-text="Estrutura dos locais do MPN":::

## <a name="prerequisites-in-order-to-add-a-new-location-for-a-csp-business"></a><span data-ttu-id="41381-121">Pré-requisitos para adicionar um novo local para um negócio do CSP</span><span class="sxs-lookup"><span data-stu-id="41381-121">Prerequisites in order to add a new location for a CSP business</span></span>

<span data-ttu-id="41381-122">Para adicionar um novo local para um negócio do CSP, há vários pré-requisitos:</span><span class="sxs-lookup"><span data-stu-id="41381-122">To add a new CSP business location, there are several prerequisites:</span></span>

1. <span data-ttu-id="41381-123">Você precisa ter uma ID de MPN de local no país em que deseja fazer negócios.</span><span class="sxs-lookup"><span data-stu-id="41381-123">You must have a location MPN ID in the country where you want to do business.</span></span>

1. <span data-ttu-id="41381-124">Você precisa de um novo locatário do Azure AD na região de negócios que ainda não esteja inscrito no CSP.</span><span class="sxs-lookup"><span data-stu-id="41381-124">You need a new Azure AD tenant in the region of business which is not already enrolled into CSP.</span></span> <span data-ttu-id="41381-125">Crie-o ao se registrar no CSP.</span><span class="sxs-lookup"><span data-stu-id="41381-125">Create this when you enroll in CSP.</span></span>
 
3. <span data-ttu-id="41381-126">Use o novo locatário do AAD para se registrar no programa CSP na região.</span><span class="sxs-lookup"><span data-stu-id="41381-126">Use the new AAD tenant to enroll into CSP program in the region.</span></span>
<span data-ttu-id="41381-127">Fornecer detalhes legais da empresa, incluindo o nome jurídico da empresa, o endereço e os detalhes do contato principal.</span><span class="sxs-lookup"><span data-stu-id="41381-127">Providing legal company details including the legal company name, address, primary contact details.</span></span> <span data-ttu-id="41381-128">Essa conta passará por verificação, portanto, certifique-se de adicionar informações válidas.</span><span class="sxs-lookup"><span data-stu-id="41381-128">This account will undergo verification, so make sure to add valid information.</span></span>

>[!NOTE] 
 ><span data-ttu-id="41381-129">Lembre-se de entrar usando as **novas** credenciais do **novo** locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="41381-129">Remember to sign in with the **new** credentials for the **new** Azure AD tenant.</span></span> <span data-ttu-id="41381-130">Não use suas credenciais existentes, pois o Partner Center reconhecerá que você já tem uma conta.</span><span class="sxs-lookup"><span data-stu-id="41381-130">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

4. <span data-ttu-id="41381-131">Aceite o Contrato de Parceiro da Microsoft e ative a conta.</span><span class="sxs-lookup"><span data-stu-id="41381-131">Accept the Microsoft Partner Agreement and activate the account.</span></span>

## <a name="add-a-location"></a><span data-ttu-id="41381-132">Adicionar um local</span><span class="sxs-lookup"><span data-stu-id="41381-132">Add a location</span></span>

1. <span data-ttu-id="41381-133">No **ícone Configuração**, selecione as **Configurações do parceiro**.</span><span class="sxs-lookup"><span data-stu-id="41381-133">From the **Setting icon**, select the **Partner settings**.</span></span>

2. <span data-ttu-id="41381-134">Selecione **Locais.**</span><span class="sxs-lookup"><span data-stu-id="41381-134">Select **Locations.**</span></span>

3. <span data-ttu-id="41381-135">Selecione **Adicionar um local**.</span><span class="sxs-lookup"><span data-stu-id="41381-135">Select **Add a location**.</span></span>  

4. <span data-ttu-id="41381-136">Na página **Adicionar um local**, insira os detalhes do endereço do local que você deseja adicionar à sua empresa, bem como um contato principal para o local.</span><span class="sxs-lookup"><span data-stu-id="41381-136">In the **Add a location** page, insert the address details of the location that you want to add to your company as well as a primary contact for the location.</span></span>

> [!NOTE]
> <span data-ttu-id="41381-137">Depois que um local for adicionado no Partner Center, ele não poderá ser removido.</span><span class="sxs-lookup"><span data-stu-id="41381-137">Once a location is added in Partner Center, it cannot be removed.</span></span>

## <a name="change-global-partner-account-location"></a><span data-ttu-id="41381-138">Alterar o local da Conta de parceiro global</span><span class="sxs-lookup"><span data-stu-id="41381-138">Change Global partner account location</span></span>

1. <span data-ttu-id="41381-139">Na página **Locais**, confira a lista de locais para verificar se o local que você deseja como pessoa jurídica está listado.</span><span class="sxs-lookup"><span data-stu-id="41381-139">On the **Locations** page, check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> <span data-ttu-id="41381-140">Se não estiver, adicione-o.</span><span class="sxs-lookup"><span data-stu-id="41381-140">If it isn't, add it.</span></span>

   :::image type="content" source="images/updatepartnerprofile2.png" alt-text="Estrutura dos locais do MPN":::

2. <span data-ttu-id="41381-142">Selecione **Perfil do parceiro** e, em seguida, **Atualizar perfil de negócios jurídico**</span><span class="sxs-lookup"><span data-stu-id="41381-142">Select **Partner profile** and then select **Update legal business profile**</span></span>

   :::image type="content" source="images/updatepartnerprofile1.png" alt-text="Estrutura dos locais do MPN":::

3. <span data-ttu-id="41381-144">Selecione a região e a pessoa jurídica e **Envie-a**.</span><span class="sxs-lookup"><span data-stu-id="41381-144">Select the region and legal entity and **Submit** it.</span></span>

   :::image type="content" source="images/updatepartnerprofile3.png" alt-text="Estrutura dos locais do MPN":::

## <a name="next-steps"></a><span data-ttu-id="41381-146">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="41381-146">Next steps</span></span>

- <span data-ttu-id="41381-147">Saiba mais sobre o [processo de verificação](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="41381-147">Learn about the [verification process](verification-responses.md).</span></span>
