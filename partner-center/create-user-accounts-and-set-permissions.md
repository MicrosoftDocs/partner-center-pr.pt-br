---
title: Criar contas de usuário e atribuir funções
description: Cada funcionário deve ser atribuído a uma função antes que possa acessar o Partner Center. Saiba como criar contas de usuário, atribuir funções e definir permissões.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.date: 02/26/2020
ms.openlocfilehash: c7d04307be7a81cf3501e1b50e278cf1a012afcd
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2020
ms.locfileid: "86435185"
---
# <a name="create-user-accounts-and-assign-roles-and-permissions"></a><span data-ttu-id="cd1ba-104">Criar contas de usuário e atribuir funções e permissões</span><span class="sxs-lookup"><span data-stu-id="cd1ba-104">Create user accounts and assign roles and permissions</span></span>

<span data-ttu-id="cd1ba-105">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="cd1ba-105">**Appropriate roles**</span></span>

- <span data-ttu-id="cd1ba-106">Administrador de conta</span><span class="sxs-lookup"><span data-stu-id="cd1ba-106">Account admin</span></span>
- <span data-ttu-id="cd1ba-107">Administrador global</span><span class="sxs-lookup"><span data-stu-id="cd1ba-107">Global admin</span></span>
- <span data-ttu-id="cd1ba-108">Administrador de gerenciamento de usuário</span><span class="sxs-lookup"><span data-stu-id="cd1ba-108">User management admin</span></span>

<span data-ttu-id="cd1ba-109">Crie contas de usuário para os funcionários que precisam acessar o Partner Center.</span><span class="sxs-lookup"><span data-stu-id="cd1ba-109">Create user accounts for employees who need access to the Partner Center.</span></span> <span data-ttu-id="cd1ba-110">Essas tarefas precisam ser realizadas pelo administrador de gerenciamento de usuários, pelo administrador de contas ou pelo administrador global. O usuário que realiza essas tarefas também deve receber as funções do AAD (Azure Active Directory) do administrador de usuários ou do administrador global.</span><span class="sxs-lookup"><span data-stu-id="cd1ba-110">These tasks must be done by the user management admin, accounts admin, or the global admin. The user performing these tasks must also be assigned the Azure Active Directory (AAD) roles of User administrator or Global administrator.</span></span> <span data-ttu-id="cd1ba-111">Para saber mais sobre as funções do AAD, confira [Permissões de função de administrador no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span><span class="sxs-lookup"><span data-stu-id="cd1ba-111">For more information about AAD roles, see [Administrator role permissions in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>


## <a name="add-a-new-user"></a><span data-ttu-id="cd1ba-112">Adicionar um novo usuário</span><span class="sxs-lookup"><span data-stu-id="cd1ba-112">Add a new user</span></span>

1. <span data-ttu-id="cd1ba-113">No ícone **Configurações** no canto superior direito do Partner Center, selecione **Gerenciamento de usuários**.</span><span class="sxs-lookup"><span data-stu-id="cd1ba-113">From the **Settings** icon at the top right of the Partner Center, select **User management**.</span></span>

2. <span data-ttu-id="cd1ba-114">Selecione **Adicionar usuário**.</span><span class="sxs-lookup"><span data-stu-id="cd1ba-114">Select **Add user**.</span></span>

3. <span data-ttu-id="cd1ba-115">Insira o nome completo e endereço de email exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="cd1ba-115">Enter the user's full name and unique email address.</span></span>

4. <span data-ttu-id="cd1ba-116">Selecione o tipo de agente e/ou o tipo de administrador que deseja atribuir ao usuário.</span><span class="sxs-lookup"><span data-stu-id="cd1ba-116">Select the type of agent and/or the type of admin you want to assign to the user.</span></span> <span data-ttu-id="cd1ba-117">O acesso do Partner Center é baseado em função, portanto, você pode atribuir permissões para personalizar o modo de exibição do usuário e mostrar somente os recursos que o usuário precisa para completar tarefas específicas.</span><span class="sxs-lookup"><span data-stu-id="cd1ba-117">Partner Center access is role-based, so you can assign permissions to customize the user's view to show only the features the user needs to complete specific tasks.</span></span>  <span data-ttu-id="cd1ba-118">Se os usuários quiserem obter uma atribuição de função, eles poderão encontrar administradores globais para contato acessando **Gerenciamento de usuários** e filtrando por administrador global.</span><span class="sxs-lookup"><span data-stu-id="cd1ba-118">If users want a role assignment, they can find global admins to contact by going to **User management** and filtering on global admin.</span></span>

5. <span data-ttu-id="cd1ba-119">Selecione **Adicionar** para criar a conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="cd1ba-119">Select **Add** to create the user account.</span></span> <span data-ttu-id="cd1ba-120">Confirme os detalhes do usuário na próxima página.</span><span class="sxs-lookup"><span data-stu-id="cd1ba-120">Confirm the user's details on the next page.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="cd1ba-121">Anote as novas informações de login do usuário exibidas nessa página.</span><span class="sxs-lookup"><span data-stu-id="cd1ba-121">Make a note of the new user's sign-in information displayed on this page.</span></span> <span data-ttu-id="cd1ba-122">Certifique-se de copiar e enviar essas informações para o novo usuário, pois você não conseguirá acessá-las novamente mais tarde.</span><span class="sxs-lookup"><span data-stu-id="cd1ba-122">Be sure to copy and send this information to the new user as you will not be able to access it again later.</span></span> 


<span data-ttu-id="cd1ba-123">O usuário precisará entrar no Partner Center com seu nome de usuário e senha temporária.</span><span class="sxs-lookup"><span data-stu-id="cd1ba-123">The user will need to sign in to the Partner Center with their user name and temporary password.</span></span> <span data-ttu-id="cd1ba-124">Quando o usuário entrar no Partner Center pela primeira vez, ele precisará alterar sua senha.</span><span class="sxs-lookup"><span data-stu-id="cd1ba-124">When the user signs in to the Partner Center for the first time, they are prompted to change their password.</span></span> 


### <a name="find-your-global-admin"></a><span data-ttu-id="cd1ba-125">Encontrar seu administrador global</span><span class="sxs-lookup"><span data-stu-id="cd1ba-125">Find your global admin</span></span>

<span data-ttu-id="cd1ba-126">Às vezes, um usuário pode precisar mudar de função ou um novo usuário pode desejar obter uma atribuição de função específica.</span><span class="sxs-lookup"><span data-stu-id="cd1ba-126">Sometimes a user might need to have their role changed or a new user may want a specific role assignment.</span></span>  
<span data-ttu-id="cd1ba-127">Para encontrar um administrador global que possa fazer alterações de função ou atribuir funções a um novo usuário, no **ícone de Configurações** no canto superior direito do Partner Center, selecione **Gerenciamento de usuários** e filtre por administrador global.</span><span class="sxs-lookup"><span data-stu-id="cd1ba-127">To find a global admin who can make role changes or assign roles to a new user, from the **Settings icon** at the top right of the Partner Center, select **User management** and filter on global admin.</span></span> 


### <a name="new-global-admin"></a><span data-ttu-id="cd1ba-128">Novo administrador global</span><span class="sxs-lookup"><span data-stu-id="cd1ba-128">New global admin</span></span>

<span data-ttu-id="cd1ba-129">Se o seu administrador global deixar a organização e outra pessoa precisar preencher essa função, você poderá enviar um tíquete para a equipe do Azure ou do Office 365.</span><span class="sxs-lookup"><span data-stu-id="cd1ba-129">If your global admin leaves the organization and someone else needs to fill this role, you can submit a ticket to either the Azure or Office 365 team.</span></span> <span data-ttu-id="cd1ba-130">Para obter informações sobre como fazer isso, selecione uma das opções abaixo.</span><span class="sxs-lookup"><span data-stu-id="cd1ba-130">For information on how to do this, select one of the options below.</span></span>

[<span data-ttu-id="cd1ba-131">Novo administrador global do Azure</span><span class="sxs-lookup"><span data-stu-id="cd1ba-131">New global admin for Azure</span></span>](https://support.microsoft.com/help/4505981/what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company)

[<span data-ttu-id="cd1ba-132">Novo administrador global do Office 365</span><span class="sxs-lookup"><span data-stu-id="cd1ba-132">New global admin for Office 365</span></span>](https://admin.microsoft.com/)


## <a name="assign-user-roles"></a><span data-ttu-id="cd1ba-133">Atribuir funções de usuário</span><span class="sxs-lookup"><span data-stu-id="cd1ba-133">Assign user roles</span></span>

<span data-ttu-id="cd1ba-134">Para trabalhar no Partner Center, você precisará ter uma função atribuída.</span><span class="sxs-lookup"><span data-stu-id="cd1ba-134">To work in the Partner Center, you must have an assigned role.</span></span>  <span data-ttu-id="cd1ba-135">Atualmente, as funções incluem funções de locatário do Azure Active Directory, funções de CSP (Provedor de Soluções na Nuvem) e funções de empresa não AAD.</span><span class="sxs-lookup"><span data-stu-id="cd1ba-135">Currently, roles include Azure Active Directory tenant roles, Cloud Solution Provider (CSP) roles, and non-AAD company roles.</span></span> <span data-ttu-id="cd1ba-136">Uma empresa individual pode ter a necessidade de todas essas funções.</span><span class="sxs-lookup"><span data-stu-id="cd1ba-136">An individual company can have a need for all of these roles.</span></span>

>[!Important]
><span data-ttu-id="cd1ba-137">Os indivíduos precisam estar listados em seu locatário para acessar o Partner Center.</span><span class="sxs-lookup"><span data-stu-id="cd1ba-137">Individuals must be listed in your tenant to access Partner Center.</span></span> <span data-ttu-id="cd1ba-138">As atribuições de função fornecem acesso adicional.</span><span class="sxs-lookup"><span data-stu-id="cd1ba-138">Role assignments provide additional access.</span></span>


<span data-ttu-id="cd1ba-139">**As funções de locatário do AAD incluem**:</span><span class="sxs-lookup"><span data-stu-id="cd1ba-139">**AAD tenant roles include**:</span></span>
- <span data-ttu-id="cd1ba-140">Administrador global</span><span class="sxs-lookup"><span data-stu-id="cd1ba-140">Global admin</span></span>
- <span data-ttu-id="cd1ba-141">Administrador de usuários</span><span class="sxs-lookup"><span data-stu-id="cd1ba-141">User admin</span></span>

<span data-ttu-id="cd1ba-142">**As funções do CSP incluem**:</span><span class="sxs-lookup"><span data-stu-id="cd1ba-142">**CSP roles include**:</span></span>
- <span data-ttu-id="cd1ba-143">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="cd1ba-143">Admin agent</span></span>
- <span data-ttu-id="cd1ba-144">Administrador de cobrança</span><span class="sxs-lookup"><span data-stu-id="cd1ba-144">Billing admin</span></span>
- <span data-ttu-id="cd1ba-145">Agente de vendas</span><span class="sxs-lookup"><span data-stu-id="cd1ba-145">Sales agent</span></span>
- <span data-ttu-id="cd1ba-146">Agente de suporte técnico</span><span class="sxs-lookup"><span data-stu-id="cd1ba-146">Helpdesk agent</span></span>

<span data-ttu-id="cd1ba-147">**Funções que gerenciam a associação do MPN e a empresa (não AAD)**</span><span class="sxs-lookup"><span data-stu-id="cd1ba-147">**Roles that manage the MPN membership and the company (Non-AAD)**</span></span>
- <span data-ttu-id="cd1ba-148">Administrador de parceiros do MPN</span><span class="sxs-lookup"><span data-stu-id="cd1ba-148">MPN partner admin</span></span>
- <span data-ttu-id="cd1ba-149">Administrador de conta</span><span class="sxs-lookup"><span data-stu-id="cd1ba-149">Account admin</span></span>
- <span data-ttu-id="cd1ba-150">Administrador de indicações</span><span class="sxs-lookup"><span data-stu-id="cd1ba-150">Referral admin</span></span>
- <span data-ttu-id="cd1ba-151">Administrador de perfis de negócios</span><span class="sxs-lookup"><span data-stu-id="cd1ba-151">Business profile admin</span></span>
- <span data-ttu-id="cd1ba-152">Administrador e usuário de incentivos</span><span class="sxs-lookup"><span data-stu-id="cd1ba-152">Incentives admin and user</span></span>

<span data-ttu-id="cd1ba-153">**O fornecedor de painel de controle é uma função de CSP e não AAD**.</span><span class="sxs-lookup"><span data-stu-id="cd1ba-153">**Control Panel Vendor is a CSP and non-AAD role**.</span></span>
- <span data-ttu-id="cd1ba-154">Administrador global</span><span class="sxs-lookup"><span data-stu-id="cd1ba-154">Global admin</span></span>

<span data-ttu-id="cd1ba-155">O **usuário convidado** precisa fazer parte do locatário do AAD e pode ter qualquer função que não seja do AAD.</span><span class="sxs-lookup"><span data-stu-id="cd1ba-155">**Guest user** must be part of the AAD tenant and can have any non-AAD role.</span></span>

<span data-ttu-id="cd1ba-156">Para obter informações específicas sobre as funções e o que cada uma pode fazer, confira [Atribuir permissões de usuário](permissions-overview.md).</span><span class="sxs-lookup"><span data-stu-id="cd1ba-156">For specific information on the roles and what each role can do, see [Assign user permissions](permissions-overview.md).</span></span>

## <a name="associate-a-users-microsoft-learn-account-in-partner-center"></a><span data-ttu-id="cd1ba-157">Associar a conta do Microsoft Learn de um usuário no Partner Center</span><span class="sxs-lookup"><span data-stu-id="cd1ba-157">Associate a user's Microsoft Learn account in Partner Center</span></span>

<span data-ttu-id="cd1ba-158">Para ver os roteiros de aprendizagem e treinamento que os usuários estão seguindo em relação às competências, eles precisam associar a ID do MCP às suas respectivas contas do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="cd1ba-158">In order to be able to see the training and learning paths your users are taking towards competencies, they need to associate their MCP ID to their Partner Center account.</span></span> <span data-ttu-id="cd1ba-159">Como o administrador global, ao adicionar novos usuários, lembre-os de associar a ID do MCP às suas respectivas contas.</span><span class="sxs-lookup"><span data-stu-id="cd1ba-159">As the global admin, when you add new users, be sure to remind them to associate their MCP ID to their account.</span></span> 

### <a name="how-to-associate-your-mcp-id-to-your-partner-center-account"></a><span data-ttu-id="cd1ba-160">Como associar sua ID do MCP à sua conta do Partner Center</span><span class="sxs-lookup"><span data-stu-id="cd1ba-160">How to associate your MCP ID to your Partner Center account</span></span>

1. <span data-ttu-id="cd1ba-161">No painel do Partner Center, selecione o ícone **Sua conta** no canto direito do painel e, em seguida, selecione **Meu perfil**.</span><span class="sxs-lookup"><span data-stu-id="cd1ba-161">From the Partner Center dashboard, select the **Your account** icon in the right corner of the dashboard, and then select **My profile**.</span></span>

2. <span data-ttu-id="cd1ba-162">Em **Seu aprendizado**, será possível associar sua conta do Microsoft Learning e também conectar sua conta Microsoft à Partner University.</span><span class="sxs-lookup"><span data-stu-id="cd1ba-162">Under **Your learning** you will be able to associate your Microsoft Learning account and also connect your Microsoft account to Partner University.</span></span>
