---
title: Localizar ID de locatário, nome de domínio, ID de objeto de usuário
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como localizar IDs no portal do Azure-ID de locatário do Azure AD, nome de domínio ou ID de objeto de usuário específico de uma organização. Algumas tarefas precisam dessas informações.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 643b1eeb96a47ee4c438f733efe3be22234d02ff
ms.sourcegitcommit: e462f562e7f26b7d6870c22638a2a841499109d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2021
ms.locfileid: "109740277"
---
# <a name="locate-important-ids-for-a-user"></a><span data-ttu-id="3241d-104">Localizar IDs importantes para um usuário</span><span class="sxs-lookup"><span data-stu-id="3241d-104">Locate important IDs for a user</span></span>

<span data-ttu-id="3241d-105">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="3241d-105">**Appropriate roles**</span></span>

- <span data-ttu-id="3241d-106">Administrador global</span><span class="sxs-lookup"><span data-stu-id="3241d-106">Global admin</span></span>

<span data-ttu-id="3241d-107">Este artigo descreve como usar o [portal do Azure](https://portal.azure.com/) para localizar as seguintes informações para um usuário:</span><span class="sxs-lookup"><span data-stu-id="3241d-107">This article describes how to use the [Azure portal](https://portal.azure.com/) to locate the following information for a user:</span></span>

- <span data-ttu-id="3241d-108">A ID de locatário do Microsoft Azure Active Directory (Azure AD) da organização ou empresa do usuário</span><span class="sxs-lookup"><span data-stu-id="3241d-108">The Microsoft Azure Active Directory (Azure AD) tenant ID of the user's organization or company</span></span>

- <span data-ttu-id="3241d-109">O nome de domínio primário da organização ou da empresa associada ao locatário do Azure AD</span><span class="sxs-lookup"><span data-stu-id="3241d-109">The primary domain name of the organization or company associated with the Azure AD tenant</span></span>

- <span data-ttu-id="3241d-110">A ID do objeto de usuário</span><span class="sxs-lookup"><span data-stu-id="3241d-110">The user object ID</span></span>

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a><span data-ttu-id="3241d-111">Localizar a ID de locatário Microsoft Azure AD e o nome de domínio primário</span><span class="sxs-lookup"><span data-stu-id="3241d-111">Find the Microsoft Azure AD tenant ID and primary domain name</span></span>

<span data-ttu-id="3241d-112">Siga estas etapas para localizar a ID de locatário do Azure AD ou o nome de domínio primário dentro do portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="3241d-112">Follow these steps to locate the Azure AD tenant ID or primary domain name within the Azure portal.</span></span> <span data-ttu-id="3241d-113">(Se você quiser encontrar uma ID de locatário programaticamente, consulte [Localizar ID de locatário com PowerShell ou CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell).)</span><span class="sxs-lookup"><span data-stu-id="3241d-113">(If you'd like to find a tenant ID programmatically, see [Find tenant ID with PowerShell or CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell).)</span></span>

> [!NOTE]
> <span data-ttu-id="3241d-114">A ID do locatário pode ser chamada de nomes diferentes em aplicativos ou recursos diferentes.</span><span class="sxs-lookup"><span data-stu-id="3241d-114">The tenant ID may be called different names in different applications or resources.</span></span> <span data-ttu-id="3241d-115">Por exemplo, a ID do locatário pode ser referida como a ID do diretório, o locatário do Azure Active Directory (Azure AD), a ID da Microsoft ou para determinados relatórios, até mesmo o *tenantguid*.</span><span class="sxs-lookup"><span data-stu-id="3241d-115">For example, the tenant ID may be referred to as the directory ID, the Azure Active Directory (Azure AD) tenant, Microsoft ID, or for certain reports, even the *tenantguid*.</span></span>

1. <span data-ttu-id="3241d-116">Entre no [portal do Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="3241d-116">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="3241d-117">Selecione **Azure Active Directory** no menu.</span><span class="sxs-lookup"><span data-stu-id="3241d-117">Select **Azure Active Directory** from the menu.</span></span>

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Mostra portal do Azure selecionando a opção Azure Active Directory no menu.":::

3. <span data-ttu-id="3241d-119">Uma página de **visão geral** do Azure Active Directory é exibida.</span><span class="sxs-lookup"><span data-stu-id="3241d-119">An Azure Active Directory **Overview** page appears.</span></span> <span data-ttu-id="3241d-120">Para localizar a ID de locatário do Azure AD ou o nome de domínio primário, procure o campo **ID do locatário** e o campo **domínio primário** .</span><span class="sxs-lookup"><span data-stu-id="3241d-120">To find the Azure AD tenant ID or primary domain name, look for the **Tenant ID** field and the **Primary domain** field.</span></span> <span data-ttu-id="3241d-121">Esses campos aparecem na seção informações do locatário.</span><span class="sxs-lookup"><span data-stu-id="3241d-121">These fields appear in the Tenant information section.</span></span>

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Mostra a página de visão geral com dois campos realçados, ID de locatário e nome de domínio primário.":::

4. <span data-ttu-id="3241d-123">Você pode encontrar a ID do locatário na portal do Azure de algumas outras maneiras.</span><span class="sxs-lookup"><span data-stu-id="3241d-123">You can find the tenant ID in the Azure portal in a few other ways.</span></span> <span data-ttu-id="3241d-124">Selecione **Azure Active Directory** no menu.</span><span class="sxs-lookup"><span data-stu-id="3241d-124">Select **Azure Active Directory** from the menu.</span></span> <span data-ttu-id="3241d-125">Em seguida, localize a seção **gerenciar** no menu e selecione **Propriedades**.</span><span class="sxs-lookup"><span data-stu-id="3241d-125">Then, locate the **Manage** section on the menu and select **Properties**.</span></span>

   <span data-ttu-id="3241d-126">A página Propriedades também exibe a ID de Locatário associada do usuário.</span><span class="sxs-lookup"><span data-stu-id="3241d-126">The Properties page also displays the user's associated Tenant ID.</span></span>

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Mostra a página Propriedades com o campo ID do Locatário realçada.":::

## <a name="find-the-user-object-id"></a><span data-ttu-id="3241d-128">Encontrar a ID do objeto de usuário</span><span class="sxs-lookup"><span data-stu-id="3241d-128">Find the user object ID</span></span>

<span data-ttu-id="3241d-129">Encontrar apenas o nome de domínio e a ID do locatário pode nem sempre ser suficiente.</span><span class="sxs-lookup"><span data-stu-id="3241d-129">Just finding the domain name and tenant ID may not always be enough.</span></span> <span data-ttu-id="3241d-130">Talvez você também precise localizar a ID de objeto específica atribuída a um usuário.</span><span class="sxs-lookup"><span data-stu-id="3241d-130">You may also need to locate the specific object ID assigned to a user.</span></span> <span data-ttu-id="3241d-131">Siga estas etapas para encontrar a ID de objeto de um usuário no portal do Azure:</span><span class="sxs-lookup"><span data-stu-id="3241d-131">Follow these steps to find a user's object ID in the Azure portal:</span></span>

1. <span data-ttu-id="3241d-132">Entre no [portal do Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="3241d-132">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="3241d-133">Selecione **Azure Active Directory** no menu.</span><span class="sxs-lookup"><span data-stu-id="3241d-133">Select **Azure Active Directory** from the menu.</span></span>

3. <span data-ttu-id="3241d-134">Localize **a seção** Gerenciar no menu e, em seguida, selecione **Usuários**.</span><span class="sxs-lookup"><span data-stu-id="3241d-134">Locate the **Manage** section on the menu, then select **Users**.</span></span>

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Mostra Azure Active Directory menu com realçada, opção Usuários.":::

4. <span data-ttu-id="3241d-136">Na página Usuários, digite o nome do usuário na caixa de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="3241d-136">From the Users page, type the user's name in the search box.</span></span>

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Mostra a página Usuários com a caixa de pesquisa para pesquisar um usuário específico.":::

5. <span data-ttu-id="3241d-138">Selecione o nome do usuário em que ele aparece na lista.</span><span class="sxs-lookup"><span data-stu-id="3241d-138">Select the user's name where it appears on the list.</span></span>  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Mostra a página Usuário exibindo uma linha para o usuário pesquisado.":::

6. <span data-ttu-id="3241d-140">Localize a seção Identidade na página Perfil do usuário.</span><span class="sxs-lookup"><span data-stu-id="3241d-140">Locate the Identity section on the user's Profile page.</span></span> <span data-ttu-id="3241d-141">O campo ID do objeto aparece aqui com a ID de objeto exclusiva do usuário.</span><span class="sxs-lookup"><span data-stu-id="3241d-141">The Object ID field appears here with the user's unique object ID.</span></span>

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Mostra a página Perfil do Usuário com a seção Identidade e um campo realçado para A ID do Objeto.":::

## <a name="next-steps"></a><span data-ttu-id="3241d-143">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="3241d-143">Next steps</span></span>

- [<span data-ttu-id="3241d-144">Encontrar sua ID de locatário programaticamente com o PowerShell ou a CLI</span><span class="sxs-lookup"><span data-stu-id="3241d-144">Find your tenant ID programmatically with PowerShell or CLI</span></span>](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [<span data-ttu-id="3241d-145">Saiba mais sobre perfis de usuário no Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="3241d-145">Learn more about user profiles in Azure Active Directory</span></span>](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [<span data-ttu-id="3241d-146">Descubra como os parceiros podem ver ou exportar detalhes do cliente Partner Center</span><span class="sxs-lookup"><span data-stu-id="3241d-146">Find out how partners can see or export customer details in Partner Center</span></span>](see-your-customer-list.md)

