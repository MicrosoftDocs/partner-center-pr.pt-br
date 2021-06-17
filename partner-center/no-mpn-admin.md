---
title: O que fazer se o único administrador do programa MPN tiver deixado a empresa?
ms.topic: how-to
ms.date: 09/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba o que fazer para encontrar um novo administrador do MPN ou obter ajuda do administrador global da sua empresa. Além disso, saiba como adicionar um novo Partner Center Administrador global.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 21042169a33d9a413f17f951c4daad0c5fc86a17
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277667"
---
# <a name="what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company"></a>O que fazer se o único administrador do programa MPN tiver deixado a empresa?

**Funções apropriadas:** administrador de parceiros do MPN | Conta de administrador | Administrador global

O artigo a seguir explica três cenários típicos sobre o que fazer se o administrador do MPN tiver deixado a empresa.

## <a name="scenario-1-mpn-partner-adminaccount-admin-has-left-the-company-but-there-are-still-global-admins-in-the-account"></a>Cenário 1: Administrador/Administrador da Conta do Parceiro MPN saiu da empresa, mas ainda há Administradores Globais na conta

Nesse caso, outra pessoa na empresa pode ser atribuída à função de administrador do Parceiro mpn. Para ser atribuída a função de administrador/administrador de conta do parceiro MPN específico:

1. Entre em sua Partner Center com sua conta de trabalho (por exemplo, tom@contoso.com ).
1. Na página **Gerenciamento de Usuários,** filtre administrador global para ver quem são os Administradores Globais da sua empresa. 
1. Entre em contato com um dos administradores globais e peça que ele atribua a função específica do MPN de que você precisa. 

## <a name="scenario-2-mpn-partner-adminaccount-admin-has-left-the-company-and-there-are-no-global-admins-in-the-account"></a>Cenário 2: O administrador/administrador da conta do parceiro mpn saiu da empresa e não há administradores globais na conta 

Se você acessar  a página Gerenciamento de Usuários e filtrar para Administrador global, mas descobrir que não há nenhum Administrador Global em sua empresa que possa ajudá-lo a obter a função específica do MPN, siga estas etapas:

1. Vá para [portal.azure.com](https://ms.portal.azure.com/), entre com sua conta de trabalho (por exemplo, tom@contoso.com ). 
1. Selecione a **opção Ajuda +** Suporte na barra de navegação do menu à esquerda.
1. Na próxima página, selecione Novo **Solicitação de suporte** e Tipo de Problema Técnico no menu suspenso, insira quaisquer detalhes adicionais e clique em  **Próximo: Soluções.**

:::image type="content" source="images/accountsettings/adminfinder.png" alt-text="Localize o administrador portal do Azure.":::

4. Depois de revisar as Soluções recomendadas na próxima página, selecione **Próximo: Detalhes** e preencha os campos necessários.
1. Revise e crie a solicitação de suporte.


## <a name="scenario-3-mpn-partner-adminaccount-adminglobal-admin-has-left-the-company-and-there-are-no-other-users-who-can-access-the-companys-azure-ad-this-is-a-complete-loss-of-access"></a>Cenário 3: o administrador/administrador da conta/administrador da conta do MPN saiu da empresa e não há outros usuários que possam acessar o Azure AD da empresa. Essa é uma perda completa de acesso.

Siga as [etapas de Tomada de controle](/azure/active-directory/users-groups-roles/domains-admin-takeover#internal-admin-takeover) do administrador para assumir um diretório não Azure Active Directory administrador.

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>Não tem certeza se a sua empresa já tem uma conta corporativa?

Se você não tiver certeza se a empresa tem uma conta corporativa, siga estas etapas para verificar.

1. Entre no [portal de administração do Azure.](https://ms.portal.azure.com)
2. Selecione **Azure Active Directory** no menu à esquerda e, em seguida, selecione **Nomes de domínio**.
Caso você já tenha uma conta corporativa, seu nome de domínio estará listado.

>[!Note]
>Se você tiver uma assinatura ativa para Microsoft Azure ou Office 365, você já tem uma conta de trabalho e suas credenciais de entrada devem ser as mesmas usadas para acessar esses serviços.