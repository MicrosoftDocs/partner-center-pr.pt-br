---
title: Gerenciar locais na sua conta de parceiro
ms.topic: how-to
ms.date: 01/26/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Saiba como adicionar um novo local e como a ID do MPN do local é usada em programas de incentivo, negócios do CSP, assinaturas e outras transações.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e39f264485e71c5a96916c224c0ea1a85c17a55b
ms.sourcegitcommit: fc1f9cb5a542bdc92d62d2a7e1ab2f4e69903e49
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2021
ms.locfileid: "98925003"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="37e3c-103">Gerenciar os locais de sua conta do MPN e adicionar um novo local</span><span class="sxs-lookup"><span data-stu-id="37e3c-103">Manage your MPN account locations and add a new location</span></span>


<span data-ttu-id="37e3c-104">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="37e3c-104">**Appropriate roles**</span></span>

- <span data-ttu-id="37e3c-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="37e3c-105">Global admin</span></span>
- <span data-ttu-id="37e3c-106">Administrador de conta</span><span class="sxs-lookup"><span data-stu-id="37e3c-106">Account admin</span></span>

<span data-ttu-id="37e3c-107">A ID de MPN do local identifica cada local específico de sua empresa.</span><span class="sxs-lookup"><span data-stu-id="37e3c-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="37e3c-108">Você usa a ID de MPN de local para se registrar em programas de incentivo, para fazer transações com empresas do CSP (Provedor de Soluções na Nuvem) e para fazer outras transações de negócios.</span><span class="sxs-lookup"><span data-stu-id="37e3c-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="37e3c-109">A ID de MPN global é usada para atividades não transacionais, como solicitações de suporte.</span><span class="sxs-lookup"><span data-stu-id="37e3c-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="37e3c-110">O seguinte é um cenário típico:</span><span class="sxs-lookup"><span data-stu-id="37e3c-110">The following is a typical scenario:</span></span>

<span data-ttu-id="37e3c-111">A Contoso tem sua PGA (Conta global de parceiro) no Reino Unido.</span><span class="sxs-lookup"><span data-stu-id="37e3c-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="37e3c-112">Trata-se de seus negócios jurídicos registrados e sua ID de MPN global é usada para gerenciar todos os negócios não transacionais.</span><span class="sxs-lookup"><span data-stu-id="37e3c-112">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="37e3c-113">A Contoso também tem PLAs (Contas de local de parceiro) equivalentes a subsidiárias ou a divisões em outros locais do Reino Unido, da França e dos EUA.</span><span class="sxs-lookup"><span data-stu-id="37e3c-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="37e3c-114">Na estrutura de Conta do MPN, essas PLAs são representadas como IDs de MPN de local exclusivas.</span><span class="sxs-lookup"><span data-stu-id="37e3c-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="37e3c-115">As PLAs são usadas para negócios transacionais, como programas de CSP ou de incentivos.</span><span class="sxs-lookup"><span data-stu-id="37e3c-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="37e3c-116">Os pagamentos são vinculados a locais específicos.</span><span class="sxs-lookup"><span data-stu-id="37e3c-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="37e3c-117">Há uma relação um-para-um entre um locatário do CSP e uma ID de local do MPN.</span><span class="sxs-lookup"><span data-stu-id="37e3c-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Estrutura dos locais do MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="37e3c-119">Pré-requisitos para adicionar uma nova conta para um negócio do CSP</span><span class="sxs-lookup"><span data-stu-id="37e3c-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="37e3c-120">Para adicionar uma nova conta para o negócio do CSP, primeiro verifique se você cumpre os pré-requisitos.</span><span class="sxs-lookup"><span data-stu-id="37e3c-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="37e3c-121">É preciso ter uma ID de MPN de local no país em que deseja fazer negócios com o CSP.</span><span class="sxs-lookup"><span data-stu-id="37e3c-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="37e3c-122">Para criar um novo local de MPN, leia "Adicionar um local de MPN" abaixo.</span><span class="sxs-lookup"><span data-stu-id="37e3c-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="37e3c-123">Para criar um novo registro de CSP Indirect Reseller, leia [Trabalhar com provedores indiretos](indirect-reseller-tasks-in-partner-center.md#get-started)</span><span class="sxs-lookup"><span data-stu-id="37e3c-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="37e3c-124">Lembre-se de entrar usando as **novas** credenciais da **nova** conta do CSP.</span><span class="sxs-lookup"><span data-stu-id="37e3c-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="37e3c-125">Não use suas credenciais existentes, pois o Partner Center reconhecerá que você já tem uma conta.</span><span class="sxs-lookup"><span data-stu-id="37e3c-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="37e3c-126">Aceite o Contrato de Parceiro da Microsoft e ative a conta.</span><span class="sxs-lookup"><span data-stu-id="37e3c-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="37e3c-127">Adicionar um local do MPN</span><span class="sxs-lookup"><span data-stu-id="37e3c-127">Add an MPN location</span></span>

1. <span data-ttu-id="37e3c-128">Entre usando a conta do MPN no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="37e3c-128">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="37e3c-129">(Suas credenciais do MPN podem ser diferentes das credenciais do CSP).</span><span class="sxs-lookup"><span data-stu-id="37e3c-129">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="37e3c-130">A conta MPN deve ter privilégios de administrador global ou de administrador de conta.</span><span class="sxs-lookup"><span data-stu-id="37e3c-130">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="37e3c-131">No **ícone Configurações**, selecione as **Configurações da conta** e o **Perfil da organização**.</span><span class="sxs-lookup"><span data-stu-id="37e3c-131">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="37e3c-132">Selecione **Legal** e, em seguida, na guia **Parceiro**, escolha **Localizações da empresa** e clique em **Adicionar um local**.</span><span class="sxs-lookup"><span data-stu-id="37e3c-132">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="37e3c-133">Insira as informações necessárias, como nome da empresa, endereço e contato do local que você quer adicionar à empresa.</span><span class="sxs-lookup"><span data-stu-id="37e3c-133">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="37e3c-134">Clique em **Adicionar local**.</span><span class="sxs-lookup"><span data-stu-id="37e3c-134">Click **Add location**.</span></span> <span data-ttu-id="37e3c-135">Isso criará uma nova ID de MPN para o novo local que você pode usar para transações e incentivos do CSP.</span><span class="sxs-lookup"><span data-stu-id="37e3c-135">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Adicionar uma nova pessoa jurídica":::

> [!NOTE]
> <span data-ttu-id="37e3c-137">Depois que um local for adicionado no Partner Center, ele não poderá ser removido.</span><span class="sxs-lookup"><span data-stu-id="37e3c-137">Once a location is added in Partner Center, it cannot be removed.</span></span> <span data-ttu-id="37e3c-138">Você verá **MPN** no menu à esquerda do Partner Center se tiver usado a ID de MPN correta para entrar.</span><span class="sxs-lookup"><span data-stu-id="37e3c-138">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="37e3c-139">Alterar o país da conta global do parceiro</span><span class="sxs-lookup"><span data-stu-id="37e3c-139">Change country of Partner global account</span></span> 

1. <span data-ttu-id="37e3c-140">Entre usando a conta do MPN no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="37e3c-140">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="37e3c-141">(Suas credenciais do MPN podem ser diferentes das credenciais do CSP).</span><span class="sxs-lookup"><span data-stu-id="37e3c-141">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="37e3c-142">A conta MPN deve ter privilégios de administrador global ou de administrador de conta.</span><span class="sxs-lookup"><span data-stu-id="37e3c-142">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="37e3c-143">Na guia **Parceiro**, acesse **Localizações da empresa** e confira a lista de locais para garantir que o local que você quer como pessoa jurídica esteja listado.</span><span class="sxs-lookup"><span data-stu-id="37e3c-143">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="37e3c-144">Para adicionar um local, clique em **Adicionar um local** e, no submenu, insira as informações necessárias, como nome da empresa, endereço e contato principal do local que você quer adicionar à empresa.</span><span class="sxs-lookup"><span data-stu-id="37e3c-144">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="37e3c-145">Selecione **Alterar seu país** ao lado do menu suspenso **País/região** e siga as etapas.</span><span class="sxs-lookup"><span data-stu-id="37e3c-145">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Submenu de dados do perfil de pessoa jurídica":::

5. <span data-ttu-id="37e3c-147">Clique em **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="37e3c-147">Click **Save**.</span></span>

6. <span data-ttu-id="37e3c-148">O país da conta global MPN será alterado para o novo país legal.</span><span class="sxs-lookup"><span data-stu-id="37e3c-148">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="37e3c-149">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="37e3c-149">Next steps</span></span>

- <span data-ttu-id="37e3c-150">Saiba mais sobre o [processo de verificação](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="37e3c-150">Learn about the [verification process](verification-responses.md).</span></span>
