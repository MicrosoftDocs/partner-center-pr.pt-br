---
title: Gerenciar usuários para contas de clientes
ms.topic: how-to
ms.date: 02/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Gerenciar usuários para seus clientes no Partner Center – criar contas de usuário, adicionar ou remover licenças de usuário, redefinir senhas e excluir ou restaurar contas de usuário.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0e2bb4ceb146174da83e9c08a9ff030380298bd0
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756082"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a><span data-ttu-id="3cab5-103">Gerenciar usuários e licenças de usuário para contas de clientes</span><span class="sxs-lookup"><span data-stu-id="3cab5-103">Manage users and user licenses for customer accounts</span></span> 

<span data-ttu-id="3cab5-104">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="3cab5-104">**Appropriate roles**</span></span>

- <span data-ttu-id="3cab5-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="3cab5-105">Global admin</span></span>
- <span data-ttu-id="3cab5-106">Administrador de gerenciamento de usuário</span><span class="sxs-lookup"><span data-stu-id="3cab5-106">User management admin</span></span>
- <span data-ttu-id="3cab5-107">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="3cab5-107">Admin agent</span></span>


<span data-ttu-id="3cab5-108">Você pode criar e excluir novos usuários na conta de um cliente.</span><span class="sxs-lookup"><span data-stu-id="3cab5-108">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="3cab5-109">Você também pode restaurar uma ou mais contas de usuário que você excluiu anteriormente dentro de 30 dias da exclusão.</span><span class="sxs-lookup"><span data-stu-id="3cab5-109">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="3cab5-110">As atribuições de assinatura anteriores do usuário também serão restauradas (supondo que suas alocações anteriores estejam disponíveis).</span><span class="sxs-lookup"><span data-stu-id="3cab5-110">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="3cab5-111">Quando você adquire novas assinaturas para um cliente, o cliente deve fornecer uma lista de todos os usuários que precisarão de contas, suas permissões de usuário e os serviços de que cada usuário precisa.</span><span class="sxs-lookup"><span data-stu-id="3cab5-111">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

>[!NOTE]
><span data-ttu-id="3cab5-112">A seção **usuários e licenças** da guia **cliente** mostra todos os usuários criados em um locatário específico do cliente, incluindo usuários que têm licenças adquiridas de outro parceiro CSP ou de outro canal de compra.</span><span class="sxs-lookup"><span data-stu-id="3cab5-112">The **Users and licenses** section of **Customer** tab shows all users created in a specific customer’s tenant, including users that have licenses purchased from another CSP partner or from another purchasing channel.</span></span>

<span data-ttu-id="3cab5-113">Você pode [atribuir assinaturas a vários usuários](bulk-license-provisioning-for-multiple-users.md) ao mesmo tempo. Basta importar os nomes usando um [arquivo de planilha .csv compatível com o Excel](adding-multiple-users-to-a-customer-account.md).</span><span class="sxs-lookup"><span data-stu-id="3cab5-113">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="3cab5-114">Criar contas de usuário para um cliente</span><span class="sxs-lookup"><span data-stu-id="3cab5-114">Create user accounts for a customer</span></span>

1. <span data-ttu-id="3cab5-115">Entre no [painel](https://partner.microsoft.com/dashboard) do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="3cab5-115">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="3cab5-116">No menu do centro de parceiros, **selecione** clientes e, em seguida, escolha um cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="3cab5-116">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="3cab5-117">No menu do cliente, selecione **Usuários e licenças**.</span><span class="sxs-lookup"><span data-stu-id="3cab5-117">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="3cab5-118">Para cada usuário, selecione **Adicionar usuário** e preencha as informações, incluindo permissões e licenças.</span><span class="sxs-lookup"><span data-stu-id="3cab5-118">For each user you add, select **Add subscription**, then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="3cab5-119">**Salve** suas alterações.</span><span class="sxs-lookup"><span data-stu-id="3cab5-119">**Save** your changes.</span></span>

5. <span data-ttu-id="3cab5-120">Grave o nome de usuário e a senha temporária para enviar para o usuário.</span><span class="sxs-lookup"><span data-stu-id="3cab5-120">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="3cab5-121">Se você estiver adicionando vários usuários individualmente, use **Adicionar outro usuário**.</span><span class="sxs-lookup"><span data-stu-id="3cab5-121">If you are adding multiple users one at a time use **Add another user**.</span></span>

7. <span data-ttu-id="3cab5-122">Você também pode adicionar vários usuários simultaneamente. Basta [importar um arquivo de planilha .csv compatível com o Excel](adding-multiple-users-to-a-customer-account.md).</span><span class="sxs-lookup"><span data-stu-id="3cab5-122">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="3cab5-123">Se estiver adicionando vários usuários simultaneamente usando a opção Adicionar outro usuário ou importando um arquivo de planilha .csv compatível com o Excel, você poderá esperar até concluir todo o conjunto antes de enviar por email ou imprimir os nomes e senhas a partir da tela de confirmação.</span><span class="sxs-lookup"><span data-stu-id="3cab5-123">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="3cab5-124">Adicionar ou remover licenças de usuário para um cliente</span><span class="sxs-lookup"><span data-stu-id="3cab5-124">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="3cab5-125">As etapas a seguir se aplicam à adição ou remoção de licenças de usuário para produtos Microsoft.</span><span class="sxs-lookup"><span data-stu-id="3cab5-125">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="3cab5-126">Para adicionar ou remover licenças de usuário para assinaturas SaaS baseadas em licença no Marketplace comercial, consulte [Adicionar ou remover licenças para uma assinatura de SaaS](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span><span class="sxs-lookup"><span data-stu-id="3cab5-126">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="3cab5-127">Entre no [painel](https://partner.microsoft.com/dashboard) do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="3cab5-127">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="3cab5-128">No menu do centro de parceiros, **selecione** clientes e, em seguida, escolha um cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="3cab5-128">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="3cab5-129">No menu do cliente, selecione **Usuários e licenças**.</span><span class="sxs-lookup"><span data-stu-id="3cab5-129">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="3cab5-130">Escolha um ou mais usuários da lista.</span><span class="sxs-lookup"><span data-stu-id="3cab5-130">Choose one or more users from the list.</span></span> <span data-ttu-id="3cab5-131">Se, por exemplo, o cliente acabou de adquirir novas licenças e você quiser atribuí-las às pessoas que não as têm ainda, use a opção **Filtrar usuários por...** para encontrar o grupo correto.</span><span class="sxs-lookup"><span data-stu-id="3cab5-131">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="3cab5-132">Selecione **Gerenciar licenças**.</span><span class="sxs-lookup"><span data-stu-id="3cab5-132">Select **Manage licenses**.</span></span> <span data-ttu-id="3cab5-133">Faça suas alterações e selecione **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="3cab5-133">Make your changes, then **Save**.</span></span>

> [!NOTE]
> <span data-ttu-id="3cab5-134">Para [produtos do Azure Marketplace](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), a atribuição e a ativação de licenças são gerenciadas por meio do ISV (fornecedor independente de software) que publicou o produto.</span><span class="sxs-lookup"><span data-stu-id="3cab5-134">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="3cab5-135">Redefinir a senha do usuário para um cliente</span><span class="sxs-lookup"><span data-stu-id="3cab5-135">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="3cab5-136">Entre no [Painel](https://partner.microsoft.com/dashboard) do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="3cab5-136">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="3cab5-137">No menu do centro de parceiros, **selecione** clientes e, em seguida, escolha um cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="3cab5-137">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="3cab5-138">No menu do cliente, selecione **Usuários e licenças**.</span><span class="sxs-lookup"><span data-stu-id="3cab5-138">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="3cab5-139">Escolha o usuário na lista.</span><span class="sxs-lookup"><span data-stu-id="3cab5-139">Choose the user from the list.</span></span>

4. <span data-ttu-id="3cab5-140">Na parte inferior da tela, selecione **Redefinir senha**.</span><span class="sxs-lookup"><span data-stu-id="3cab5-140">At the bottom of the screen, select **Reset password**.</span></span> 

5. <span data-ttu-id="3cab5-141">Envie a nova senha temporária ao usuário.</span><span class="sxs-lookup"><span data-stu-id="3cab5-141">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="3cab5-142">Excluir contas de usuário para um cliente</span><span class="sxs-lookup"><span data-stu-id="3cab5-142">Delete user accounts for a customer</span></span>

1. <span data-ttu-id="3cab5-143">No menu do **centro de parceiros** , selecione **clientes**.</span><span class="sxs-lookup"><span data-stu-id="3cab5-143">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="3cab5-144">Escolha o cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="3cab5-144">Choose the customer from the list.</span></span>

2. <span data-ttu-id="3cab5-145">No menu do cliente, selecione **Usuários e licenças**.</span><span class="sxs-lookup"><span data-stu-id="3cab5-145">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="3cab5-146">Escolha o usuário na lista.</span><span class="sxs-lookup"><span data-stu-id="3cab5-146">Choose the user from the list.</span></span>

3. <span data-ttu-id="3cab5-147">Na parte inferior da tela, selecione **Excluir conta de usuário**.</span><span class="sxs-lookup"><span data-stu-id="3cab5-147">At the bottom of the screen, select **Delete user account**.</span></span>

<span data-ttu-id="3cab5-148">Se precisar restaurar essa conta, você pode encontrá-la na guia **Usuários excluídos** da lista **Usuários e licenças** do cliente.</span><span class="sxs-lookup"><span data-stu-id="3cab5-148">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="3cab5-149">Você tem 30 dias para restaurar um usuário excluído.</span><span class="sxs-lookup"><span data-stu-id="3cab5-149">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="3cab5-150">Restaurar contas de usuário excluídas</span><span class="sxs-lookup"><span data-stu-id="3cab5-150">Restore deleted user accounts</span></span>

1. <span data-ttu-id="3cab5-151">No menu do **centro de parceiros** , selecione **clientes** e, em seguida, escolha o cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="3cab5-151">From the **Partner Center** menu, select **Customers**, then choose the customer from the list.</span></span>

2. <span data-ttu-id="3cab5-152">Selecione **usuários e licenças**.</span><span class="sxs-lookup"><span data-stu-id="3cab5-152">Select **Users and licenses**.</span></span>

3. <span data-ttu-id="3cab5-153">Selecione a guia **Usuários excluídos ( )**. Ela deve mostrar **(1)** ou mais quando houver usuários excluídos que possam ser restaurados.</span><span class="sxs-lookup"><span data-stu-id="3cab5-153">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4. <span data-ttu-id="3cab5-154">Marque uma ou mais caixas de seleção dos usuários excluídos e selecione **Restaurar**.</span><span class="sxs-lookup"><span data-stu-id="3cab5-154">Select one or more of the deleted users' checkboxes and then select **Restore**.</span></span>

    <span data-ttu-id="3cab5-155">Todas as contas de usuário selecionadas reaparecerão na página **Usuários e licenças**.</span><span class="sxs-lookup"><span data-stu-id="3cab5-155">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="3cab5-156">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="3cab5-156">Next steps</span></span>

- [<span data-ttu-id="3cab5-157">Atribuir ou revogar licenças de vários usuários</span><span class="sxs-lookup"><span data-stu-id="3cab5-157">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

- [<span data-ttu-id="3cab5-158">Criar vários usuários para uma conta de cliente</span><span class="sxs-lookup"><span data-stu-id="3cab5-158">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)