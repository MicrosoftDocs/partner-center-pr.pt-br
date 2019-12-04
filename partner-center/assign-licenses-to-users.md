---
title: Tarefas de gerenciamento de usuários para contas de cliente | Partner Center
ms.topic: article
ms.date: 11/25/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como criar contas de usuário para um cliente, adicionar ou remover licenças de usuário, redefinir senhas de usuário, excluir contas de usuário ou restaurá-las.
ms.assetid: 41B06576-8DDD-435D-BABB-697D4AD30213
author: MaggiePucciEvans
ms.author: evansma
Keywords: gerenciamento de clientes, conta, criar conta, licenças, atribuir licença, gerenciamento de usuários, senha, Redefinir senha, alterar senha
ms.localizationpriority: medium
ms.openlocfilehash: cd1b32a0ceb133f9513263f56a7d1e2e98dde3c5
ms.sourcegitcommit: c793c1b61f50fc0b0a12c95cedd9f57b31703093
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2019
ms.locfileid: "74721361"
---
# <a name="user-management-tasks-for-customer-accounts"></a>Tarefas de gerenciamento de usuários para contas de cliente

**Aplica-se a**

- Partner Center

**Funções apropriadas**

- Administração global
- Administrador de gerenciamento de usuário
- Agente administrativo
- Agente de vendas
- Agente de suporte técnico

Você pode criar e excluir novos usuários na conta de um cliente. Você também pode restaurar uma ou mais contas de usuário que você excluiu anteriormente dentro de 30 dias da exclusão. As atribuições de assinatura anteriores do usuário também serão restauradas (supondo que suas alocações anteriores estejam disponíveis).

Quando você adquire novas assinaturas para um cliente, o cliente deve fornecer uma lista de todos os usuários que precisarão de contas, suas permissões de usuário e os serviços de que cada usuário precisa.  

Você pode [atribuir assinaturas a vários usuários](bulk-license-provisioning-for-multiple-users.md) ao mesmo tempo. Basta importar os nomes usando um [arquivo de planilha .csv compatível com o Excel](adding-multiple-users-to-a-customer-account.md).

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a>Criar contas de usuário para um cliente

1. Entre no [painel](https://partner.microsoft.com/dashboard)do Partner Center.

2. No menu do centro de parceiros, **selecione**clientes e, em seguida, escolha um cliente na lista.

3. No menu do cliente, selecione **Usuários e licenças**.

4. Para cada usuário, selecione **Adicionar usuário** e preencha as informações, incluindo permissões e licenças. **Salve** suas alterações.

5. Grave o nome de usuário e a senha temporária para enviar para o usuário.

6. Se você estiver adicionando vários usuários individualmente, use **Adicionar outro usuário**.

7. Você também pode adicionar vários usuários simultaneamente. Basta [importar um arquivo de planilha .csv compatível com o Excel](adding-multiple-users-to-a-customer-account.md). Se estiver adicionando vários usuários simultaneamente usando a opção Adicionar outro usuário ou importando um arquivo de planilha .csv compatível com o Excel, você poderá esperar até concluir todo o conjunto antes de enviar por email ou imprimir os nomes e senhas a partir da tela de confirmação.

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a>Adicionar ou remover licenças de usuário para um cliente

As etapas a seguir se aplicam à adição ou remoção de licenças de usuário para produtos Microsoft. Para adicionar ou remover licenças de usuário para assinaturas SaaS baseadas em licença no Marketplace comercial, consulte [Adicionar ou remover licenças para uma assinatura de SaaS](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).

1. Entre no [painel](https://partner.microsoft.com/dashboard)do Partner Center.

2. No menu do centro de parceiros, **selecione**clientes e, em seguida, escolha um cliente na lista.

3. No menu do cliente, selecione **Usuários e licenças**.

4. Escolha um ou mais usuários da lista. Se, por exemplo, o cliente acabou de adquirir novas licenças e você quiser atribuí-las às pessoas que não as têm ainda, use a opção **Filtrar usuários por...** para encontrar o grupo correto.

5. Selecione **Gerenciar licenças**. Faça suas alterações e selecione **Salvar**.

> [!NOTE]
> Para [produtos do Azure Marketplace](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), a atribuição e a ativação de licenças são gerenciadas por meio do ISV (fornecedor independente de software) que publicou o produto.

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a>Redefinir a senha do usuário para um cliente

1. Entre no [painel](https://partner.microsoft.com/dashboard)do Partner Center.

2. No menu do centro de parceiros, **selecione**clientes e, em seguida, escolha um cliente na lista.

3.  No menu do cliente, selecione **Usuários e licenças**. Escolha o usuário na lista.

4.  Na parte inferior da tela, selecione **Redefinir senha**. 

5.  Envie a nova senha temporária ao usuário.

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a>Excluir contas de usuário para um cliente

1.  No menu do **centro de parceiros** , selecione **clientes**. Escolha o cliente na lista.

2.  No menu do cliente, selecione **Usuários e licenças**. Escolha o usuário na lista.

3.  Na parte inferior da tela, selecione **Excluir conta de usuário**.

Se precisar restaurar essa conta, você pode encontrá-la na guia **Usuários excluídos** da lista **Usuários e licenças** do cliente. Você tem 30 dias para restaurar um usuário excluído.

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a>Restaurar contas de usuário excluídas

1.  No menu do **centro de parceiros** , selecione **clientes**e, em seguida, escolha o cliente na lista.

2.  Selecione **Usuários e licenças**.

3.  Selecione a guia **Usuários excluídos ( )** . Ela deve mostrar **(1)** ou mais quando houver usuários excluídos que possam ser restaurados.

4.  Marque uma ou mais caixas de seleção dos usuários excluídos e selecione **Restaurar**.

    Todas as contas de usuário selecionadas reaparecerão na página **Usuários e licenças**.

## <a name="related-topics"></a>Tópicos relacionados


[Atribuir ou revogar licenças de vários usuários](bulk-license-provisioning-for-multiple-users.md)

[Criar vários usuários para uma conta de cliente](adding-multiple-users-to-a-customer-account.md)