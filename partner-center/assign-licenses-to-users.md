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
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a>Gerenciar usuários e licenças de usuário para contas de clientes 

**Funções apropriadas:** administrador global | Administrador de gerenciamento de usuários | Agente administrador


Você pode criar e excluir novos usuários na conta de um cliente. Você também pode restaurar uma ou mais contas de usuário que você excluiu anteriormente dentro de 30 dias após a exclusão. As atribuições de assinatura anteriores do usuário também serão restauradas (supondo que suas alocações anteriores estejam disponíveis).

Quando você compra novas assinaturas para um cliente, o cliente deve lhe dar uma lista de todos os usuários que precisarão de contas, suas permissões de usuário e quais serviços cada usuário precisa.  

>[!NOTE]
>A seção Usuários e  licenças da guia Cliente mostra todos os usuários criados no locatário de um cliente específico, incluindo usuários que têm licenças **adquiridas** de outro parceiro CSP ou de outro canal de compra.

Você pode [atribuir assinaturas a vários usuários](bulk-license-provisioning-for-multiple-users.md) ao mesmo tempo. Basta importar os nomes usando um [arquivo de planilha .csv compatível com o Excel](adding-multiple-users-to-a-customer-account.md).

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a>Criar contas de usuário para um cliente

1. Entre no [painel](https://partner.microsoft.com/dashboard) do Partner Center.

2. No menu do centro de parceiros, **selecione** clientes e, em seguida, escolha um cliente na lista.

3. No menu do cliente, selecione **Usuários e licenças.**

4. Para cada usuário, selecione **Adicionar usuário** e preencha as informações, incluindo permissões e licenças. **Salve** suas alterações.

5. Grave o nome de usuário e a senha temporária para enviar para o usuário.

6. Se você estiver adicionando vários usuários individualmente, use **Adicionar outro usuário**.

7. Você também pode adicionar vários usuários simultaneamente. Basta [importar um arquivo de planilha .csv compatível com o Excel](adding-multiple-users-to-a-customer-account.md). Se estiver adicionando vários usuários simultaneamente usando a opção Adicionar outro usuário ou importando um arquivo de planilha .csv compatível com o Excel, você poderá esperar até concluir todo o conjunto antes de enviar por email ou imprimir os nomes e senhas a partir da tela de confirmação.

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a>Adicionar ou remover licenças de usuário para um cliente

As etapas a seguir se aplicam à adição ou remoção de licenças de usuário para produtos da Microsoft. Para adicionar ou remover licenças de usuário para assinaturas SaaS baseadas em licença no marketplace comercial, consulte Adicionar ou remover licenças para [uma assinatura de SaaS](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).

1. Entre no [painel](https://partner.microsoft.com/dashboard) do Partner Center.

2. No menu do centro de parceiros, **selecione** clientes e, em seguida, escolha um cliente na lista.

3. No menu do cliente, selecione **Usuários e licenças.**

4. Escolha um ou mais usuários da lista. Se, por exemplo, o cliente acabou de comprar novas licenças e você quiser atribuí-las a pessoas que ainda não as têm, você poderá usar a opção Filtrar usuários **por...** para encontrar o grupo certo.

5. Selecione **Gerenciar licenças**. Faça suas alterações e, em **seguida, salve**.

> [!NOTE]
> Para [Azure Marketplace , a](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)atribuição de licença e a ativação são gerenciadas por meio do ISV (Fornecedor Independente de Software) que publicou o produto.

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a>Redefinir a senha do usuário para um cliente

1. Entre no [Painel](https://partner.microsoft.com/dashboard) do Partner Center.

2. No menu do centro de parceiros, **selecione** clientes e, em seguida, escolha um cliente na lista.

3. No menu do cliente, selecione **Usuários e licenças.** Escolha o usuário na lista.

4. Na parte inferior da tela, selecione **Redefinir senha**. 

5. Envie a nova senha temporária ao usuário.

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a>Excluir contas de usuário para um cliente

1. No menu **Partner Center,** selecione **Clientes**. Escolha o cliente na lista.

2. No menu do cliente, selecione **Usuários e licenças.** Escolha o usuário na lista.

3. Na parte inferior da tela, selecione **Excluir conta de usuário**.

Se precisar restaurar essa conta, você pode encontrá-la na guia **Usuários excluídos** da lista **Usuários e licenças** do cliente. Você tem 30 dias para restaurar um usuário excluído.

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a>Restaurar contas de usuário excluídas

1. No menu **Partner Center,** selecione **Clientes** e escolha o cliente na lista.

2. Selecione **Usuários e licenças**.

3. Selecione a guia **Usuários excluídos ( )**. Ela deve mostrar **(1)** ou mais quando houver usuários excluídos que possam ser restaurados.

4. Marque uma ou mais caixas de seleção dos usuários excluídos e selecione **Restaurar**.

    Todas as contas de usuário selecionadas reaparecerão na página **Usuários e licenças**.

## <a name="next-steps"></a>Próximas etapas

- [Atribuir ou revogar licenças de vários usuários](bulk-license-provisioning-for-multiple-users.md)

- [Criar vários usuários para uma conta de cliente](adding-multiple-users-to-a-customer-account.md)