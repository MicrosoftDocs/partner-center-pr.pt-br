---
title: Encontrar ID do locatário, nome de domínio, ID de objeto de usuário
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como encontrar IDs no portal do Azure – ID de locatário do Azure AD de uma organização, nome de domínio ou ID de objeto de usuário específica. Algumas tarefas precisam dessa informação.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 5da41cdbfa7aa1780b31e170a2398e8e7c65df27
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150855"
---
# <a name="locate-important-ids-for-a-user"></a><span data-ttu-id="9c0be-104">Localizar IDs importantes para um usuário</span><span class="sxs-lookup"><span data-stu-id="9c0be-104">Locate important IDs for a user</span></span>

<span data-ttu-id="9c0be-105">**Funções apropriadas**: administrador global</span><span class="sxs-lookup"><span data-stu-id="9c0be-105">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="9c0be-106">Este artigo descreve como usar o portal do Azure [para](https://portal.azure.com/) localizar as seguintes informações para um usuário:</span><span class="sxs-lookup"><span data-stu-id="9c0be-106">This article describes how to use the [Azure portal](https://portal.azure.com/) to locate the following information for a user:</span></span>

- <span data-ttu-id="9c0be-107">A Microsoft Azure Active Directory do locatário do Azure AD (Azure) da organização ou da empresa do usuário</span><span class="sxs-lookup"><span data-stu-id="9c0be-107">The Microsoft Azure Active Directory (Azure AD) tenant ID of the user's organization or company</span></span>

- <span data-ttu-id="9c0be-108">O nome de domínio primário da organização ou da empresa associada ao locatário do Azure AD</span><span class="sxs-lookup"><span data-stu-id="9c0be-108">The primary domain name of the organization or company associated with the Azure AD tenant</span></span>

- <span data-ttu-id="9c0be-109">A ID do objeto de usuário</span><span class="sxs-lookup"><span data-stu-id="9c0be-109">The user object ID</span></span>

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a><span data-ttu-id="9c0be-110">Encontre a ID Microsoft Azure AD locatário e o nome de domínio primário</span><span class="sxs-lookup"><span data-stu-id="9c0be-110">Find the Microsoft Azure AD tenant ID and primary domain name</span></span>

<span data-ttu-id="9c0be-111">Siga estas etapas para localizar a ID do locatário do Azure AD ou o nome de domínio primário no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="9c0be-111">Follow these steps to locate the Azure AD tenant ID or primary domain name within the Azure portal.</span></span> <span data-ttu-id="9c0be-112">(Se você quiser encontrar uma ID de locatário programaticamente, consulte Encontrar a ID do locatário com [o PowerShell ou a CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell).)</span><span class="sxs-lookup"><span data-stu-id="9c0be-112">(If you'd like to find a tenant ID programmatically, see [Find tenant ID with PowerShell or CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell).)</span></span>

> [!NOTE]
> <span data-ttu-id="9c0be-113">A ID do locatário pode ser chamada de nomes diferentes em diferentes aplicativos ou recursos.</span><span class="sxs-lookup"><span data-stu-id="9c0be-113">The tenant ID may be called different names in different applications or resources.</span></span> <span data-ttu-id="9c0be-114">Por exemplo, a ID do locatário pode ser conhecida como a ID do diretório, o locatário do Azure Active Directory (Azure AD), a ID da Microsoft ou para determinados relatórios, até mesmo o *tenantguid*.</span><span class="sxs-lookup"><span data-stu-id="9c0be-114">For example, the tenant ID may be referred to as the directory ID, the Azure Active Directory (Azure AD) tenant, Microsoft ID, or for certain reports, even the *tenantguid*.</span></span>

1. <span data-ttu-id="9c0be-115">Entre no [portal do Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="9c0be-115">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="9c0be-116">Selecione **Azure Active Directory** no menu.</span><span class="sxs-lookup"><span data-stu-id="9c0be-116">Select **Azure Active Directory** from the menu.</span></span>

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Mostra portal do Azure selecionando a Azure Active Directory no menu.":::

3. <span data-ttu-id="9c0be-118">Uma página Azure Active Directory **Visão geral** é exibida.</span><span class="sxs-lookup"><span data-stu-id="9c0be-118">An Azure Active Directory **Overview** page appears.</span></span> <span data-ttu-id="9c0be-119">Para encontrar a ID do locatário do Azure AD ou o nome de domínio primário, procure o campo **ID** do locatário e o **campo Domínio** primário.</span><span class="sxs-lookup"><span data-stu-id="9c0be-119">To find the Azure AD tenant ID or primary domain name, look for the **Tenant ID** field and the **Primary domain** field.</span></span> <span data-ttu-id="9c0be-120">Esses campos aparecem na seção Informações do locatário.</span><span class="sxs-lookup"><span data-stu-id="9c0be-120">These fields appear in the Tenant information section.</span></span>

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Mostra a página Visão geral com dois campos realçadas, ID do locatário e nome de domínio primário.":::

4. <span data-ttu-id="9c0be-122">Você pode encontrar a ID do locatário no portal do Azure de algumas outras maneiras.</span><span class="sxs-lookup"><span data-stu-id="9c0be-122">You can find the tenant ID in the Azure portal in a few other ways.</span></span> <span data-ttu-id="9c0be-123">Selecione **Azure Active Directory** no menu.</span><span class="sxs-lookup"><span data-stu-id="9c0be-123">Select **Azure Active Directory** from the menu.</span></span> <span data-ttu-id="9c0be-124">Em seguida, **localize a seção** Gerenciar no menu e selecione **Propriedades**.</span><span class="sxs-lookup"><span data-stu-id="9c0be-124">Then, locate the **Manage** section on the menu and select **Properties**.</span></span>

   <span data-ttu-id="9c0be-125">A página Propriedades também exibe a ID de locatário associada do usuário.</span><span class="sxs-lookup"><span data-stu-id="9c0be-125">The Properties page also displays the user's associated Tenant ID.</span></span>

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Mostra a página de propriedades com o campo ID de locatário realçado.":::

## <a name="find-the-user-object-id"></a><span data-ttu-id="9c0be-127">Localizar a ID de objeto de usuário</span><span class="sxs-lookup"><span data-stu-id="9c0be-127">Find the user object ID</span></span>

<span data-ttu-id="9c0be-128">Apenas encontrar o nome de domínio e a ID de locatário nem sempre pode ser suficiente.</span><span class="sxs-lookup"><span data-stu-id="9c0be-128">Just finding the domain name and tenant ID may not always be enough.</span></span> <span data-ttu-id="9c0be-129">Talvez você também precise localizar a ID de objeto específica atribuída a um usuário.</span><span class="sxs-lookup"><span data-stu-id="9c0be-129">You may also need to locate the specific object ID assigned to a user.</span></span> <span data-ttu-id="9c0be-130">Siga estas etapas para localizar a ID de objeto de um usuário no portal do Azure:</span><span class="sxs-lookup"><span data-stu-id="9c0be-130">Follow these steps to find a user's object ID in the Azure portal:</span></span>

1. <span data-ttu-id="9c0be-131">Entre no [portal do Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="9c0be-131">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="9c0be-132">Selecione **Azure Active Directory** no menu.</span><span class="sxs-lookup"><span data-stu-id="9c0be-132">Select **Azure Active Directory** from the menu.</span></span>

3. <span data-ttu-id="9c0be-133">Localize a seção **gerenciar** no menu e, em seguida, selecione **usuários**.</span><span class="sxs-lookup"><span data-stu-id="9c0be-133">Locate the **Manage** section on the menu, then select **Users**.</span></span>

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Mostra Azure Active Directory menu com a opção Users realçada.":::

4. <span data-ttu-id="9c0be-135">Na página usuários, digite o nome do usuário na caixa de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="9c0be-135">From the Users page, type the user's name in the search box.</span></span>

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Mostra a página de usuários com a caixa de pesquisa para procurar um usuário específico.":::

5. <span data-ttu-id="9c0be-137">Selecione o nome do usuário onde ele aparece na lista.</span><span class="sxs-lookup"><span data-stu-id="9c0be-137">Select the user's name where it appears on the list.</span></span>  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Mostra a página do usuário exibindo uma linha para o usuário pesquisado.":::

6. <span data-ttu-id="9c0be-139">Localize a seção identidade na página de perfil do usuário.</span><span class="sxs-lookup"><span data-stu-id="9c0be-139">Locate the Identity section on the user's Profile page.</span></span> <span data-ttu-id="9c0be-140">O campo ID de objeto aparece aqui com a ID de objeto exclusiva do usuário.</span><span class="sxs-lookup"><span data-stu-id="9c0be-140">The Object ID field appears here with the user's unique object ID.</span></span>

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Mostra a página de perfil do usuário com a seção de identidade e um campo realçado para a ID de objeto.":::

## <a name="next-steps"></a><span data-ttu-id="9c0be-142">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="9c0be-142">Next steps</span></span>

- [<span data-ttu-id="9c0be-143">Localize sua ID de locatário programaticamente com o PowerShell ou a CLI</span><span class="sxs-lookup"><span data-stu-id="9c0be-143">Find your tenant ID programmatically with PowerShell or CLI</span></span>](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [<span data-ttu-id="9c0be-144">Saiba mais sobre perfis de usuário no Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="9c0be-144">Learn more about user profiles in Azure Active Directory</span></span>](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [<span data-ttu-id="9c0be-145">Descubra como os parceiros podem ver ou exportar detalhes do cliente no Partner Center</span><span class="sxs-lookup"><span data-stu-id="9c0be-145">Find out how partners can see or export customer details in Partner Center</span></span>](see-your-customer-list.md)

