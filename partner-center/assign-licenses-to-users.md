---
title: Gerenciar usuários para contas de clientes
ms.topic: how-to
ms.date: 02/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Gerenciar usuários para seus clientes no Partner Center - criar contas de usuário, adicionar ou remover licenças de usuário, redefinir senhas e excluir ou restaurar contas de usuário.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: dc896ec3ce16ab0f05a8131de14f573ad96a8141
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149886"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a><span data-ttu-id="9da83-103">Gerenciar usuários e licenças de usuário para contas de clientes</span><span class="sxs-lookup"><span data-stu-id="9da83-103">Manage users and user licenses for customer accounts</span></span> 

<span data-ttu-id="9da83-104">**Funções apropriadas:** administrador global | Administrador de gerenciamento de usuários | Agente administrador</span><span class="sxs-lookup"><span data-stu-id="9da83-104">**Appropriate roles**: Global admin | User management admin | Admin agent</span></span>


<span data-ttu-id="9da83-105">Você pode criar e excluir novos usuários na conta de um cliente.</span><span class="sxs-lookup"><span data-stu-id="9da83-105">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="9da83-106">Você também pode restaurar uma ou mais contas de usuário que você excluiu anteriormente dentro de 30 dias após a exclusão.</span><span class="sxs-lookup"><span data-stu-id="9da83-106">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="9da83-107">As atribuições de assinatura anteriores do usuário também serão restauradas (supondo que suas alocações anteriores estejam disponíveis).</span><span class="sxs-lookup"><span data-stu-id="9da83-107">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="9da83-108">Quando você compra novas assinaturas para um cliente, o cliente deve lhe dar uma lista de todos os usuários que precisarão de contas, suas permissões de usuário e quais serviços cada usuário precisa.</span><span class="sxs-lookup"><span data-stu-id="9da83-108">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

>[!NOTE]
><span data-ttu-id="9da83-109">A seção Usuários e  licenças da guia Cliente mostra todos os usuários criados no locatário de um cliente específico, incluindo usuários que têm licenças **adquiridas** de outro parceiro CSP ou de outro canal de compra.</span><span class="sxs-lookup"><span data-stu-id="9da83-109">The **Users and licenses** section of **Customer** tab shows all users created in a specific customer’s tenant, including users that have licenses purchased from another CSP partner or from another purchasing channel.</span></span>

<span data-ttu-id="9da83-110">Você pode [atribuir assinaturas a vários usuários](bulk-license-provisioning-for-multiple-users.md) ao mesmo tempo. Basta importar os nomes usando um [arquivo de planilha .csv compatível com o Excel](adding-multiple-users-to-a-customer-account.md).</span><span class="sxs-lookup"><span data-stu-id="9da83-110">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="9da83-111">Criar contas de usuário para um cliente</span><span class="sxs-lookup"><span data-stu-id="9da83-111">Create user accounts for a customer</span></span>

1. <span data-ttu-id="9da83-112">Entre no [painel](https://partner.microsoft.com/dashboard) do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="9da83-112">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="9da83-113">No menu do centro de parceiros, **selecione** clientes e, em seguida, escolha um cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="9da83-113">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="9da83-114">No menu do cliente, selecione **Usuários e licenças.**</span><span class="sxs-lookup"><span data-stu-id="9da83-114">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="9da83-115">Para cada usuário, selecione **Adicionar usuário** e preencha as informações, incluindo permissões e licenças.</span><span class="sxs-lookup"><span data-stu-id="9da83-115">For each user you add, select **Add subscription**, then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="9da83-116">**Salve** suas alterações.</span><span class="sxs-lookup"><span data-stu-id="9da83-116">**Save** your changes.</span></span>

5. <span data-ttu-id="9da83-117">Grave o nome de usuário e a senha temporária para enviar para o usuário.</span><span class="sxs-lookup"><span data-stu-id="9da83-117">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="9da83-118">Se você estiver adicionando vários usuários individualmente, use **Adicionar outro usuário**.</span><span class="sxs-lookup"><span data-stu-id="9da83-118">If you are adding multiple users one at a time use **Add another user**.</span></span>

7. <span data-ttu-id="9da83-119">Você também pode adicionar vários usuários simultaneamente. Basta [importar um arquivo de planilha .csv compatível com o Excel](adding-multiple-users-to-a-customer-account.md).</span><span class="sxs-lookup"><span data-stu-id="9da83-119">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="9da83-120">Se estiver adicionando vários usuários simultaneamente usando a opção Adicionar outro usuário ou importando um arquivo de planilha .csv compatível com o Excel, você poderá esperar até concluir todo o conjunto antes de enviar por email ou imprimir os nomes e senhas a partir da tela de confirmação.</span><span class="sxs-lookup"><span data-stu-id="9da83-120">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="9da83-121">Adicionar ou remover licenças de usuário para um cliente</span><span class="sxs-lookup"><span data-stu-id="9da83-121">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="9da83-122">As etapas a seguir se aplicam à adição ou remoção de licenças de usuário para produtos da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="9da83-122">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="9da83-123">Para adicionar ou remover licenças de usuário para assinaturas SaaS baseadas em licença no marketplace comercial, consulte Adicionar ou remover licenças para [uma assinatura de SaaS](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span><span class="sxs-lookup"><span data-stu-id="9da83-123">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="9da83-124">Entre no [painel](https://partner.microsoft.com/dashboard) do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="9da83-124">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="9da83-125">No menu do centro de parceiros, **selecione** clientes e, em seguida, escolha um cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="9da83-125">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="9da83-126">No menu do cliente, selecione **Usuários e licenças.**</span><span class="sxs-lookup"><span data-stu-id="9da83-126">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="9da83-127">Escolha um ou mais usuários da lista.</span><span class="sxs-lookup"><span data-stu-id="9da83-127">Choose one or more users from the list.</span></span> <span data-ttu-id="9da83-128">Se, por exemplo, o cliente acabou de comprar novas licenças e você quiser atribuí-las a pessoas que ainda não as têm, você poderá usar a opção Filtrar usuários **por...** para encontrar o grupo certo.</span><span class="sxs-lookup"><span data-stu-id="9da83-128">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="9da83-129">Selecione **Gerenciar licenças**.</span><span class="sxs-lookup"><span data-stu-id="9da83-129">Select **Manage licenses**.</span></span> <span data-ttu-id="9da83-130">Faça suas alterações e, em **seguida, salve**.</span><span class="sxs-lookup"><span data-stu-id="9da83-130">Make your changes, then **Save**.</span></span>

> [!NOTE]
> <span data-ttu-id="9da83-131">Para [Azure Marketplace , a](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)atribuição de licença e a ativação são gerenciadas por meio do ISV (Fornecedor Independente de Software) que publicou o produto.</span><span class="sxs-lookup"><span data-stu-id="9da83-131">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="9da83-132">Redefinir a senha do usuário para um cliente</span><span class="sxs-lookup"><span data-stu-id="9da83-132">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="9da83-133">Entre no [Painel](https://partner.microsoft.com/dashboard) do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="9da83-133">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="9da83-134">No menu do centro de parceiros, **selecione** clientes e, em seguida, escolha um cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="9da83-134">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="9da83-135">No menu do cliente, selecione **Usuários e licenças.**</span><span class="sxs-lookup"><span data-stu-id="9da83-135">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="9da83-136">Escolha o usuário na lista.</span><span class="sxs-lookup"><span data-stu-id="9da83-136">Choose the user from the list.</span></span>

4. <span data-ttu-id="9da83-137">Na parte inferior da tela, selecione **Redefinir senha**.</span><span class="sxs-lookup"><span data-stu-id="9da83-137">At the bottom of the screen, select **Reset password**.</span></span> 

5. <span data-ttu-id="9da83-138">Envie a nova senha temporária ao usuário.</span><span class="sxs-lookup"><span data-stu-id="9da83-138">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="9da83-139">Excluir contas de usuário para um cliente</span><span class="sxs-lookup"><span data-stu-id="9da83-139">Delete user accounts for a customer</span></span>

1. <span data-ttu-id="9da83-140">No menu **Partner Center,** selecione **Clientes**.</span><span class="sxs-lookup"><span data-stu-id="9da83-140">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="9da83-141">Escolha o cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="9da83-141">Choose the customer from the list.</span></span>

2. <span data-ttu-id="9da83-142">No menu do cliente, selecione **Usuários e licenças.**</span><span class="sxs-lookup"><span data-stu-id="9da83-142">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="9da83-143">Escolha o usuário na lista.</span><span class="sxs-lookup"><span data-stu-id="9da83-143">Choose the user from the list.</span></span>

3. <span data-ttu-id="9da83-144">Na parte inferior da tela, selecione **Excluir conta de usuário**.</span><span class="sxs-lookup"><span data-stu-id="9da83-144">At the bottom of the screen, select **Delete user account**.</span></span>

<span data-ttu-id="9da83-145">Se precisar restaurar essa conta, você pode encontrá-la na guia **Usuários excluídos** da lista **Usuários e licenças** do cliente.</span><span class="sxs-lookup"><span data-stu-id="9da83-145">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="9da83-146">Você tem 30 dias para restaurar um usuário excluído.</span><span class="sxs-lookup"><span data-stu-id="9da83-146">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="9da83-147">Restaurar contas de usuário excluídas</span><span class="sxs-lookup"><span data-stu-id="9da83-147">Restore deleted user accounts</span></span>

1. <span data-ttu-id="9da83-148">No menu **Partner Center,** selecione **Clientes** e escolha o cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="9da83-148">From the **Partner Center** menu, select **Customers**, then choose the customer from the list.</span></span>

2. <span data-ttu-id="9da83-149">Selecione **Usuários e licenças**.</span><span class="sxs-lookup"><span data-stu-id="9da83-149">Select **Users and licenses**.</span></span>

3. <span data-ttu-id="9da83-150">Selecione a guia **Usuários excluídos ( )**. Ela deve mostrar **(1)** ou mais quando houver usuários excluídos que possam ser restaurados.</span><span class="sxs-lookup"><span data-stu-id="9da83-150">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4. <span data-ttu-id="9da83-151">Marque uma ou mais caixas de seleção dos usuários excluídos e selecione **Restaurar**.</span><span class="sxs-lookup"><span data-stu-id="9da83-151">Select one or more of the deleted users' checkboxes and then select **Restore**.</span></span>

    <span data-ttu-id="9da83-152">Todas as contas de usuário selecionadas reaparecerão na página **Usuários e licenças**.</span><span class="sxs-lookup"><span data-stu-id="9da83-152">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="9da83-153">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="9da83-153">Next steps</span></span>

- [<span data-ttu-id="9da83-154">Atribuir ou revogar licenças de vários usuários</span><span class="sxs-lookup"><span data-stu-id="9da83-154">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

- [<span data-ttu-id="9da83-155">Criar vários usuários para uma conta de cliente</span><span class="sxs-lookup"><span data-stu-id="9da83-155">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)