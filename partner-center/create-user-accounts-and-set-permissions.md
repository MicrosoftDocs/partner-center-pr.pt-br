---
title: Criar contas de usuário e atribuir funções
description: Cada funcionário deve ser atribuído a uma função antes que possa acessar o Partner Center. Saiba como criar contas de usuário, atribuir funções e definir permissões.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
ms.custom: contperf-fy21q2
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.date: 10/12/2020
ms.openlocfilehash: 9621f0bc3283d7d3b08e2ebac62b4e5d8c95a4d4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148135"
---
# <a name="create-user-accounts"></a>Criar contas de usuário  

**Funções apropriadas**: Administrador da conta | Administrador global | Administrador de gerenciamento de usuários

Crie contas de usuário para os funcionários que precisam acessar o Partner Center. Essas tarefas precisam ser realizadas pelo administrador de gerenciamento de usuários, pelo administrador de contas ou pelo administrador global. O usuário que realiza essas tarefas também deve receber as funções do AAD (Azure Active Directory) do administrador de usuários ou do administrador global. Para saber mais sobre as funções do AAD, confira [Permissões de função de administrador no Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).

## <a name="add-a-new-user"></a>Adicionar um novo usuário

1. No ícone **Configurações**, localizado no canto superior direito do Partner Center, selecione **Configurações de conta** e, em seguida, selecione **Gerenciamento de usuário**.

2. Selecione **Adicionar usuário**.

3. Insira o nome completo e endereço de email exclusivo do usuário.

4. Selecione o tipo de agente e/ou o tipo de administrador que deseja atribuir ao usuário. O acesso do Partner Center é baseado em função, portanto, você pode atribuir permissões para personalizar o modo de exibição do usuário e mostrar somente os recursos que o usuário precisa para completar tarefas específicas.  Se os usuários quiserem obter uma atribuição de função, eles poderão encontrar administradores globais para contato acessando **Gerenciamento de usuários** e filtrando por administrador global.

5. Selecione **Adicionar** para criar a conta de usuário. Confirme os detalhes do usuário na próxima página.

> [!IMPORTANT]  
> Anote as novas informações de login do usuário exibidas nessa página. Certifique-se de copiar e enviar essas informações para o novo usuário, pois você não conseguirá acessá-las novamente mais tarde. 

O usuário precisará entrar no Partner Center com seu nome de usuário e senha temporária. Quando o usuário entrar no Partner Center pela primeira vez, ele precisará alterar sua senha.

## <a name="assign-user-roles"></a>Atribuir funções de usuário

Para trabalhar no Partner Center, você precisará ter uma função atribuída.  Atualmente, as funções incluem funções de locatário do Azure Active Directory, funções de CSP (Provedor de Soluções na Nuvem) e funções de empresa não AAD. Uma empresa individual pode ter a necessidade de todas essas funções.

>[!Important]
>Os indivíduos precisam estar listados em seu locatário para acessar o Partner Center. As atribuições de função fornecem acesso adicional.

## <a name="next-steps"></a>Próximas etapas

- [Atribuir funções e permissões de usuários para funcionários que precisam trabalhar no Partner Center](permissions-overview.md)
