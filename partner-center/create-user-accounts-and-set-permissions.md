---
title: Criar contas de usuário e atribuir funções
description: Cada funcionário deve ser atribuído a uma função antes que possa acessar o Partner Center. Saiba como criar contas de usuário, atribuir funções e definir permissões.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
ms.custom: contperfq2
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.date: 10/12/2020
ms.openlocfilehash: 41f7f68c61630daf30595e28bd5de52f5a5787c8
ms.sourcegitcommit: 940dad4527f51781f6f966e196b3aa08389613a2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/13/2020
ms.locfileid: "92006771"
---
# <a name="create-user-accounts"></a><span data-ttu-id="34a4a-104">Criar contas de usuário</span><span class="sxs-lookup"><span data-stu-id="34a4a-104">Create user accounts</span></span>  

<span data-ttu-id="34a4a-105">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="34a4a-105">**Appropriate roles**</span></span>

- <span data-ttu-id="34a4a-106">Administrador de conta</span><span class="sxs-lookup"><span data-stu-id="34a4a-106">Account admin</span></span>
- <span data-ttu-id="34a4a-107">Administrador global</span><span class="sxs-lookup"><span data-stu-id="34a4a-107">Global admin</span></span>
- <span data-ttu-id="34a4a-108">Administrador de gerenciamento de usuário</span><span class="sxs-lookup"><span data-stu-id="34a4a-108">User management admin</span></span>

<span data-ttu-id="34a4a-109">Crie contas de usuário para os funcionários que precisam acessar o Partner Center.</span><span class="sxs-lookup"><span data-stu-id="34a4a-109">Create user accounts for employees who need access to the Partner Center.</span></span> <span data-ttu-id="34a4a-110">Essas tarefas precisam ser realizadas pelo administrador de gerenciamento de usuários, pelo administrador de contas ou pelo administrador global. O usuário que realiza essas tarefas também deve receber as funções do AAD (Azure Active Directory) do administrador de usuários ou do administrador global.</span><span class="sxs-lookup"><span data-stu-id="34a4a-110">These tasks must be done by the user management admin, accounts admin, or the global admin. The user performing these tasks must also be assigned the Azure Active Directory (AAD) roles of User administrator or Global administrator.</span></span> <span data-ttu-id="34a4a-111">Para saber mais sobre as funções do AAD, confira [Permissões de função de administrador no Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span><span class="sxs-lookup"><span data-stu-id="34a4a-111">For more information about AAD roles, see [Administrator role permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>

## <a name="add-a-new-user"></a><span data-ttu-id="34a4a-112">Adicionar um novo usuário</span><span class="sxs-lookup"><span data-stu-id="34a4a-112">Add a new user</span></span>

1. <span data-ttu-id="34a4a-113">No ícone **Configurações**, localizado no canto superior direito do Partner Center, selecione **Configurações de conta** e, em seguida, selecione **Gerenciamento de usuário**.</span><span class="sxs-lookup"><span data-stu-id="34a4a-113">From the **Settings** icon at the top right of the Partner Center, select **Account settings** and then select **User management**.</span></span>

2. <span data-ttu-id="34a4a-114">Selecione **Adicionar usuário**.</span><span class="sxs-lookup"><span data-stu-id="34a4a-114">Select **Add user**.</span></span>

3. <span data-ttu-id="34a4a-115">Insira o nome completo e endereço de email exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="34a4a-115">Enter the user's full name and unique email address.</span></span>

4. <span data-ttu-id="34a4a-116">Selecione o tipo de agente e/ou o tipo de administrador que deseja atribuir ao usuário.</span><span class="sxs-lookup"><span data-stu-id="34a4a-116">Select the type of agent and/or the type of admin you want to assign to the user.</span></span> <span data-ttu-id="34a4a-117">O acesso do Partner Center é baseado em função, portanto, você pode atribuir permissões para personalizar o modo de exibição do usuário e mostrar somente os recursos que o usuário precisa para completar tarefas específicas.</span><span class="sxs-lookup"><span data-stu-id="34a4a-117">Partner Center access is role-based, so you can assign permissions to customize the user's view to show only the features the user needs to complete specific tasks.</span></span>  <span data-ttu-id="34a4a-118">Se os usuários quiserem obter uma atribuição de função, eles poderão encontrar administradores globais para contato acessando **Gerenciamento de usuários** e filtrando por administrador global.</span><span class="sxs-lookup"><span data-stu-id="34a4a-118">If users want a role assignment, they can find global admins to contact by going to **User management** and filtering on global admin.</span></span>

5. <span data-ttu-id="34a4a-119">Selecione **Adicionar** para criar a conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="34a4a-119">Select **Add** to create the user account.</span></span> <span data-ttu-id="34a4a-120">Confirme os detalhes do usuário na próxima página.</span><span class="sxs-lookup"><span data-stu-id="34a4a-120">Confirm the user's details on the next page.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="34a4a-121">Anote as novas informações de login do usuário exibidas nessa página.</span><span class="sxs-lookup"><span data-stu-id="34a4a-121">Make a note of the new user's sign-in information displayed on this page.</span></span> <span data-ttu-id="34a4a-122">Certifique-se de copiar e enviar essas informações para o novo usuário, pois você não conseguirá acessá-las novamente mais tarde.</span><span class="sxs-lookup"><span data-stu-id="34a4a-122">Be sure to copy and send this information to the new user as you will not be able to access it again later.</span></span> 

<span data-ttu-id="34a4a-123">O usuário precisará entrar no Partner Center com seu nome de usuário e senha temporária.</span><span class="sxs-lookup"><span data-stu-id="34a4a-123">The user will need to sign in to the Partner Center with their user name and temporary password.</span></span> <span data-ttu-id="34a4a-124">Quando o usuário entrar no Partner Center pela primeira vez, ele precisará alterar sua senha.</span><span class="sxs-lookup"><span data-stu-id="34a4a-124">When the user signs in to the Partner Center for the first time, they are prompted to change their password.</span></span>

## <a name="assign-user-roles"></a><span data-ttu-id="34a4a-125">Atribuir funções de usuário</span><span class="sxs-lookup"><span data-stu-id="34a4a-125">Assign user roles</span></span>

<span data-ttu-id="34a4a-126">Para trabalhar no Partner Center, você precisará ter uma função atribuída.</span><span class="sxs-lookup"><span data-stu-id="34a4a-126">To work in the Partner Center, you must have an assigned role.</span></span>  <span data-ttu-id="34a4a-127">Atualmente, as funções incluem funções de locatário do Azure Active Directory, funções de CSP (Provedor de Soluções na Nuvem) e funções de empresa não AAD.</span><span class="sxs-lookup"><span data-stu-id="34a4a-127">Currently, roles include Azure Active Directory tenant roles, Cloud Solution Provider (CSP) roles, and non-AAD company roles.</span></span> <span data-ttu-id="34a4a-128">Uma empresa individual pode ter a necessidade de todas essas funções.</span><span class="sxs-lookup"><span data-stu-id="34a4a-128">An individual company can have a need for all of these roles.</span></span>

>[!Important]
><span data-ttu-id="34a4a-129">Os indivíduos precisam estar listados em seu locatário para acessar o Partner Center.</span><span class="sxs-lookup"><span data-stu-id="34a4a-129">Individuals must be listed in your tenant to access Partner Center.</span></span> <span data-ttu-id="34a4a-130">As atribuições de função fornecem acesso adicional.</span><span class="sxs-lookup"><span data-stu-id="34a4a-130">Role assignments provide additional access.</span></span>

## <a name="next-steps"></a><span data-ttu-id="34a4a-131">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="34a4a-131">Next steps</span></span>

- [<span data-ttu-id="34a4a-132">Atribuir funções e permissões de usuários para funcionários que precisam trabalhar no Partner Center</span><span class="sxs-lookup"><span data-stu-id="34a4a-132">Assign users roles and permissions for employees needing to work in Partner Center</span></span>](permissions-overview.md)
