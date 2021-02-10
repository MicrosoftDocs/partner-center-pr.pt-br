---
title: Gerenciar locais na sua conta de parceiro
ms.topic: how-to
ms.date: 02/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Saiba como adicionar um novo local e como a ID do MPN do local é usada em programas de incentivo, negócios do CSP, assinaturas e outras transações.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 41ffaeaf0fb46659142949872295523546bb91c1
ms.sourcegitcommit: 5768f10cd122a20fe3df3062ea34e7096d99f639
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "100005901"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a><span data-ttu-id="9b65a-103">Gerenciar os locais da sua conta do MPN e adicionar (ou excluir) um local</span><span class="sxs-lookup"><span data-stu-id="9b65a-103">Manage your MPN account locations and add (delete) a location</span></span>


<span data-ttu-id="9b65a-104">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="9b65a-104">**Appropriate roles**</span></span>

- <span data-ttu-id="9b65a-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="9b65a-105">Global admin</span></span>
- <span data-ttu-id="9b65a-106">Administrador de conta</span><span class="sxs-lookup"><span data-stu-id="9b65a-106">Account admin</span></span>

<span data-ttu-id="9b65a-107">A ID de MPN do local identifica cada local específico de sua empresa.</span><span class="sxs-lookup"><span data-stu-id="9b65a-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="9b65a-108">Você usa a ID de MPN de local para se registrar em programas de incentivo, para fazer transações com empresas do CSP (Provedor de Soluções na Nuvem) e para fazer outras transações de negócios.</span><span class="sxs-lookup"><span data-stu-id="9b65a-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="9b65a-109">A ID de MPN global é usada para atividades não transacionais, como solicitações de suporte.</span><span class="sxs-lookup"><span data-stu-id="9b65a-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="9b65a-110">O seguinte é um cenário típico:</span><span class="sxs-lookup"><span data-stu-id="9b65a-110">The following is a typical scenario:</span></span>

<span data-ttu-id="9b65a-111">A Contoso tem sua PGA (Conta global de parceiro) no Reino Unido.</span><span class="sxs-lookup"><span data-stu-id="9b65a-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="9b65a-112">Trata-se de seus negócios jurídicos registrados e sua ID de MPN global é usada para gerenciar todos os negócios não transacionais.</span><span class="sxs-lookup"><span data-stu-id="9b65a-112">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="9b65a-113">A Contoso também tem PLAs (Contas de local de parceiro) equivalentes a subsidiárias ou a divisões em outros locais do Reino Unido, da França e dos EUA.</span><span class="sxs-lookup"><span data-stu-id="9b65a-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="9b65a-114">Na estrutura de Conta do MPN, essas PLAs são representadas como IDs de MPN de local exclusivas.</span><span class="sxs-lookup"><span data-stu-id="9b65a-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="9b65a-115">As PLAs são usadas para negócios transacionais, como programas de CSP ou de incentivos.</span><span class="sxs-lookup"><span data-stu-id="9b65a-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="9b65a-116">Os pagamentos são vinculados a locais específicos.</span><span class="sxs-lookup"><span data-stu-id="9b65a-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="9b65a-117">Há uma relação um-para-um entre um locatário do CSP e uma ID de local do MPN.</span><span class="sxs-lookup"><span data-stu-id="9b65a-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Estrutura dos locais do MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="9b65a-119">Pré-requisitos para adicionar uma nova conta para um negócio do CSP</span><span class="sxs-lookup"><span data-stu-id="9b65a-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="9b65a-120">Para adicionar uma nova conta para o negócio do CSP, primeiro verifique se você cumpre os pré-requisitos.</span><span class="sxs-lookup"><span data-stu-id="9b65a-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="9b65a-121">É preciso ter uma ID de MPN de local no país em que deseja fazer negócios com o CSP.</span><span class="sxs-lookup"><span data-stu-id="9b65a-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="9b65a-122">Para criar um novo local de MPN, leia "Adicionar um local de MPN" abaixo.</span><span class="sxs-lookup"><span data-stu-id="9b65a-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="9b65a-123">Para criar um novo registro de CSP Indirect Reseller, leia [Trabalhar com provedores indiretos](indirect-reseller-tasks-in-partner-center.md#get-started)</span><span class="sxs-lookup"><span data-stu-id="9b65a-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="9b65a-124">Lembre-se de entrar usando as **novas** credenciais da **nova** conta do CSP.</span><span class="sxs-lookup"><span data-stu-id="9b65a-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="9b65a-125">Não use suas credenciais existentes, pois o Partner Center reconhecerá que você já tem uma conta.</span><span class="sxs-lookup"><span data-stu-id="9b65a-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="9b65a-126">Aceite o Contrato de Parceiro da Microsoft e ative a conta.</span><span class="sxs-lookup"><span data-stu-id="9b65a-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="9b65a-127">Se você quiser se registrar como parceiro de fatura direta, leia [Requisitos para parceiros de fatura direta](direct-partner-new-requirements.md)</span><span class="sxs-lookup"><span data-stu-id="9b65a-127">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-your-mpn-locations"></a><span data-ttu-id="9b65a-128">Exibir seus locais do MPN</span><span class="sxs-lookup"><span data-stu-id="9b65a-128">View your MPN locations</span></span>

1. <span data-ttu-id="9b65a-129">Entre no [painel](https://partner.microsoft.com/dashboard/home) do Partner Center com suas credenciais da conta do MPN.</span><span class="sxs-lookup"><span data-stu-id="9b65a-129">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="9b65a-130">(Suas credenciais do MPN podem ser diferentes das credenciais do CSP)</span><span class="sxs-lookup"><span data-stu-id="9b65a-130">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="9b65a-131">No ícone **Configurações**, selecione **Configurações da conta**, **Perfil da organização**, **Legal**.</span><span class="sxs-lookup"><span data-stu-id="9b65a-131">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="9b65a-132">Na guia **Parceiro**, verifique se não há uma mensagem de erro de banner solicitando que você corrija os locais migrados do PMC.</span><span class="sxs-lookup"><span data-stu-id="9b65a-132">On the **Partner** tab verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span> <span data-ttu-id="9b65a-133">Se houver, siga as instruções e corrija esses locais.</span><span class="sxs-lookup"><span data-stu-id="9b65a-133">If there is, follow instructions and fix those locations.</span></span> 

3. <span data-ttu-id="9b65a-134">Se não houver uma mensagem de erro, em **Configurações**, selecione **Configurações da Conta**, **Perfil da organização**, **Identificadores**.</span><span class="sxs-lookup"><span data-stu-id="9b65a-134">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

4. <span data-ttu-id="9b65a-135">Localize a ID do MPN com o tipo "local" que corresponde ao país dessa conta do CSP e use-a para pesquisar abaixo e concluir a associação.</span><span class="sxs-lookup"><span data-stu-id="9b65a-135">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to search below and complete association.</span></span>

5. <span data-ttu-id="9b65a-136">Se você não encontrar a ID do MPN do local que corresponde à conta do CSP que deseja usar, será possível adicionar um novo local que criará uma ID do MPN.</span><span class="sxs-lookup"><span data-stu-id="9b65a-136">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location which will create a new MPN ID.</span></span> <span data-ttu-id="9b65a-137">Confira **Adicionar um local do MPN** abaixo.</span><span class="sxs-lookup"><span data-stu-id="9b65a-137">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="9b65a-138">Adicionar um local do MPN</span><span class="sxs-lookup"><span data-stu-id="9b65a-138">Add an MPN location</span></span>

1. <span data-ttu-id="9b65a-139">Entre usando a conta do MPN no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="9b65a-139">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="9b65a-140">(Suas credenciais do MPN podem ser diferentes das credenciais do CSP).</span><span class="sxs-lookup"><span data-stu-id="9b65a-140">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="9b65a-141">A conta MPN deve ter privilégios de administrador global ou de administrador de conta.</span><span class="sxs-lookup"><span data-stu-id="9b65a-141">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="9b65a-142">No **ícone Configurações**, selecione as **Configurações da conta** e o **Perfil da organização**.</span><span class="sxs-lookup"><span data-stu-id="9b65a-142">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="9b65a-143">Selecione **Legal** e, em seguida, na guia **Parceiro**, escolha **Localizações da empresa** e clique em **Adicionar um local**.</span><span class="sxs-lookup"><span data-stu-id="9b65a-143">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="9b65a-144">Insira as informações necessárias, como nome da empresa, endereço e contato do local que você quer adicionar à empresa.</span><span class="sxs-lookup"><span data-stu-id="9b65a-144">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="9b65a-145">Clique em **Adicionar local**.</span><span class="sxs-lookup"><span data-stu-id="9b65a-145">Click **Add location**.</span></span> <span data-ttu-id="9b65a-146">Isso criará uma nova ID de MPN para o novo local que você pode usar para transações e incentivos do CSP.</span><span class="sxs-lookup"><span data-stu-id="9b65a-146">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Adicionar uma nova pessoa jurídica":::

> [!NOTE]
> <span data-ttu-id="9b65a-148">Depois que um local for adicionado no Partner Center, você não poderá removê-lo.</span><span class="sxs-lookup"><span data-stu-id="9b65a-148">Once a location is added in Partner Center, you cannot remove it.</span></span> <span data-ttu-id="9b65a-149">Você verá **MPN** no menu à esquerda do Partner Center se tiver usado a ID de MPN correta para entrar.</span><span class="sxs-lookup"><span data-stu-id="9b65a-149">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="delete-a-location"></a><span data-ttu-id="9b65a-150">Excluir um local</span><span class="sxs-lookup"><span data-stu-id="9b65a-150">Delete a location</span></span>

<span data-ttu-id="9b65a-151">Para excluir um local de sua conta, você precisará entrar em contato com o [Suporte a Parceiros](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span><span class="sxs-lookup"><span data-stu-id="9b65a-151">To delete a location from your account you will need to contact [Partner Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span></span> <span data-ttu-id="9b65a-152">Verifique se você entendeu o impacto que essa ação tem.</span><span class="sxs-lookup"><span data-stu-id="9b65a-152">Make sure that you understand the impact this action has.</span></span> <span data-ttu-id="9b65a-153">Os locais excluídos não podem ser recuperados e qualquer coisa associada a essa ID de MPN específica não será mais reconhecida nem estará ativa para sua empresa.</span><span class="sxs-lookup"><span data-stu-id="9b65a-153">Deleted locations cannot be retrieved and anything tied to that specific MPN id will no longer be recognized or be active for your company.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="9b65a-154">Alterar o país da conta global do parceiro</span><span class="sxs-lookup"><span data-stu-id="9b65a-154">Change country of Partner global account</span></span> 

1. <span data-ttu-id="9b65a-155">Entre usando a conta do MPN no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="9b65a-155">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="9b65a-156">(Suas credenciais do MPN podem ser diferentes das credenciais do CSP).</span><span class="sxs-lookup"><span data-stu-id="9b65a-156">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="9b65a-157">A conta MPN deve ter privilégios de administrador global ou de administrador de conta.</span><span class="sxs-lookup"><span data-stu-id="9b65a-157">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="9b65a-158">Na guia **Parceiro**, acesse **Localizações da empresa** e confira a lista de locais para garantir que o local que você quer como pessoa jurídica esteja listado.</span><span class="sxs-lookup"><span data-stu-id="9b65a-158">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="9b65a-159">Para adicionar um local, clique em **Adicionar um local** e, no submenu, insira as informações necessárias, como nome da empresa, endereço e contato principal do local que você quer adicionar à empresa.</span><span class="sxs-lookup"><span data-stu-id="9b65a-159">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="9b65a-160">Selecione **Alterar seu país** ao lado do menu suspenso **País/região** e siga as etapas.</span><span class="sxs-lookup"><span data-stu-id="9b65a-160">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Submenu de dados do perfil de pessoa jurídica":::

5. <span data-ttu-id="9b65a-162">Clique em **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="9b65a-162">Click **Save**.</span></span>

6. <span data-ttu-id="9b65a-163">O país da conta global MPN será alterado para o novo país legal.</span><span class="sxs-lookup"><span data-stu-id="9b65a-163">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="9b65a-164">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="9b65a-164">Next steps</span></span>

- <span data-ttu-id="9b65a-165">Saiba mais sobre o [processo de verificação](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="9b65a-165">Learn about the [verification process](verification-responses.md).</span></span>
