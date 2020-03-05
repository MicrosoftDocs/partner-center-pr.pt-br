---
title: Criar contas de usuário e definir permissões | Partner Center
ms.topic: article
ms.date: 02/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como criar contas de usuário e atribuir funções no Partner Center para cada funcionário que precisar de acesso. Usuários com diferentes privilégios de administrador podem fazer isso.
ms.assetid: 75D805AE-9922-4CFD-9427-196047D70963
author: MaggiePucciEvans
ms.author: evansma
Keywords: funções, permissões, adicionar usuário, atribuir função, administrador, agente,
ms.localizationpriority: high
ms.openlocfilehash: 6bbae5b8bcd2882c7ba32a8b660fc256dec4e49a
ms.sourcegitcommit: 717ef04f5c0040611af3ba9e5a324ab67e99ba14
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/03/2020
ms.locfileid: "78240203"
---
# <a name="create-user-accounts-and-assign-permissions"></a>Criar contas de usuário e atribuir permissões

**Funções apropriadas**

- Administrador de conta
- Administrador global
- Administrador de gerenciamento de usuário

Crie contas de usuário para os funcionários que precisam acessar o Partner Center. Essas tarefas precisam ser realizadas pelo administrador de gerenciamento de usuários, pelo administrador de contas ou pelo administrador global. O usuário que realiza essas tarefas também deve receber as funções do AAD (Azure Active Directory) do administrador de usuários ou do administrador global. Para saber mais sobre as funções do AAD, confira [Permissões de função de administrador no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles).


## <a name="add-a-new-user"></a>Adicionar um novo usuário

1. No ícone **Configurações** no canto superior direito do Partner Center, selecione **Gerenciamento de usuários**.

2. Selecione **Adicionar usuário**.

3. Insira o nome completo e endereço de email exclusivo do usuário.

4. Selecione o tipo de agente e/ou o tipo de administrador que deseja atribuir ao usuário. O acesso do Partner Center é baseado em função, portanto, você pode atribuir permissões para personalizar o modo de exibição do usuário e mostrar somente os recursos que o usuário precisa para completar tarefas específicas.  Se os usuários quiserem obter uma atribuição de função, eles poderão encontrar administradores globais para contato acessando **Gerenciamento de usuários** e filtrando por administrador global.

5. Selecione **Adicionar** para criar a conta de usuário. Confirme os detalhes do usuário na próxima página.

> [!IMPORTANT]  
> Anote as novas informações de login do usuário exibidas nessa página. Certifique-se de copiar e enviar essas informações para o novo usuário, pois você não conseguirá acessá-las novamente mais tarde. 

O usuário precisará entrar no Partner Center com seu nome de usuário e senha temporária. Quando o usuário entrar no Partner Center pela primeira vez, ele precisará alterar sua senha. 

> [!NOTE]  
>  Caso o administrador global tenha saído da organização ou mudado de função e você precise adicionar um novo administrador global, registre uma solicitação de serviço em log no [portal do MPN](https://partner.microsoft.com/support). O agente de suporte poderá solicitar a elevação de um usuário a administrador global se o solicitante puder fornecer as informações de identidade pessoal requisitadas e informações adicionais sobre a sua organização.

### <a name="find-your-global-admin"></a>Encontrar seu administrador global

Às vezes, um usuário pode precisar mudar de função ou um novo usuário pode desejar obter uma atribuição de função específica.  
Para encontrar um administrador global que possa fazer alterações de função ou atribuir funções a um novo usuário, no **ícone de Configurações** no canto superior direito do Partner Center, selecione **Gerenciamento de usuários** e filtre por administrador global. 

## <a name="assign-user-roles"></a>Atribuir funções de usuário

Para trabalhar no Partner Center, você precisará ter uma função atribuída.  Atualmente, as funções incluem funções de locatário do Azure Active Directory, funções de CSP (Provedor de Soluções na Nuvem) e funções de empresa não AAD. Uma empresa individual pode ter a necessidade de todas essas funções.

>[!Important]
>Os indivíduos precisam estar listados em seu locatário para acessar o Partner Center. As atribuições de função fornecem acesso adicional.


**As funções de locatário do AAD incluem**:
- Administrador global
- Administrador de usuários

**As funções do CSP incluem**:
- Agente administrativo
- Administrador de cobrança
- Agente de vendas
- Agente de suporte técnico

**Funções que gerenciam a associação do MPN e a empresa (não AAD)**
- Administrador de parceiros do MPN
- Administrador de conta
- Administrador de indicações
- Administrador de perfis de negócios
- Administrador e usuário de incentivos

**O fornecedor de painel de controle é uma função de CSP e não AAD**.
- Administrador global

O **usuário convidado** precisa fazer parte do locatário do AAD e pode ter qualquer função que não seja do AAD.

Para obter informações específicas sobre as funções e o que cada uma pode fazer, confira [Atribuir permissões de usuário](permissions-overview.md).

## <a name="associate-a-users-microsoft-learn-account-in-partner-center"></a>Associar a conta do Microsoft Learn de um usuário no Partner Center

Para ver os roteiros de aprendizagem e treinamento que os usuários estão seguindo em relação às competências, eles precisam associar a ID do MCP às suas respectivas contas do Partner Center. Como o administrador global, ao adicionar novos usuários, lembre-os de associar a ID do MCP às suas respectivas contas. 

### <a name="how-to-associate-your-mcp-id-to-your-partner-center-account"></a>Como associar sua ID do MCP à sua conta do Partner Center

1. No painel do Partner Center, selecione o ícone **Sua conta** no canto direito do painel e, em seguida, selecione **Meu perfil**.

2. Em **Seu aprendizado**, será possível associar sua conta do Microsoft Learning e também conectar sua conta Microsoft à Partner University.








