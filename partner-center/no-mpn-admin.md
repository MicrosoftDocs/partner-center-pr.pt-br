---
title: O que fazer se o único administrador de seu programa MPN tiver deixado a empresa?
ms.topic: how-to
ms.date: 09/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba o que fazer para encontrar um novo administrador do MPN ou obter ajuda do administrador global da sua empresa. Além disso, saiba como adicionar um novo administrador global do Partner Center.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1ff6252ce36e68f2f17115460a97fa4928daf029
ms.sourcegitcommit: 3a9318d0de7a159215cb454295125532134ff8de
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/09/2020
ms.locfileid: "89570616"
---
# <a name="what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company"></a>O que fazer se o único administrador de seu programa MPN tiver deixado a empresa?

**Aplica-se a**

- Partner Center

O artigo a seguir orienta você por três cenários típicos sobre o que fazer se o administrador do MPN tiver deixado a empresa.

## <a name="scenario-1-mpn-partner-adminaccount-admin-has-left-the-company-but-there-are-still-global-admins-in-the-account"></a>Cenário 1: administrador do parceiro MPN/administrador da conta saiu da empresa, mas ainda há administradores globais na conta

Nesse caso, outra pessoa na empresa pode receber a função de administrador do parceiro MPN. Para receber a função da função de administrador de conta/Administrador de parceiro MPN específica:

1. Entre em sua conta do Partner Center com sua conta corporativa (por exemplo, tom@contoso.com ).
1. Na página de **Gerenciamento de usuário** , filtre o administrador global para ver quem são os administradores globais da sua empresa. 
1. Contate um dos administradores globais e peça que eles atribuam a você a função específica de MPN de que você precisa. 

## <a name="scenario-2-mpn-partner-adminaccount-admin-has-left-the-company-and-there-are-no-global-admins-in-the-account"></a>Cenário 2: administrador do parceiro MPN/administrador da conta saiu da empresa e não há administradores globais na conta 

Se você acessar a página de **Gerenciamento de usuários** e filtrar o administrador global, mas achar que não há nenhum administrador global em sua empresa que possa ajudá-lo a obter a função específica do MPN, siga estas etapas:

1. Acesse [Portal.Azure.com](https://ms.portal.azure.com/), entre com sua conta corporativa (por exemplo, tom@contoso.com ). 
1. Selecione a opção **ajuda + suporte** na barra de navegação do menu à esquerda.
1. Na página seguinte, selecione **novo solicitação de suporte** e tipo de **problema técnico** no menu suspenso, insira os detalhes adicionais e clique em **Avançar: soluções.**

:::image type="content" source="images/accountsettings/adminfinder.png" alt-text="Localizar administrador no portal do Azure":::

4. Depois de examinar as soluções recomendadas na próxima página, selecione **Avançar: detalhes** e conclua os campos necessários.
1. Examine e crie a solicitação de suporte.


## <a name="scenario-3-mpn-partner-adminaccount-adminglobal-admin-has-left-the-company-and-there-are-no-other-users-who-can-access-the-companys-azure-ad-this-is-a-complete-loss-of-access"></a>Cenário 3: o administrador do parceiro MPN/administrador da conta/Administrador Global saiu da empresa e não há outros usuários que possam acessar o Azure AD da empresa. Essa é uma perda completa de acesso.

Siga as etapas de [tomada do administrador](https://docs.microsoft.com/azure/active-directory/users-groups-roles/domains-admin-takeover#internal-admin-takeover) para assumir um diretório não gerenciado como administrador Azure Active Directory.

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>Não tem certeza se a sua empresa já tem uma conta corporativa?

Se você não tiver certeza se a empresa tem uma conta corporativa, siga estas etapas para verificar.

1. Entre no portal de [Administração do Azure](https://ms.portal.azure.com).
2. Selecione **Azure Active Directory** no menu à esquerda e, em seguida, selecione **nomes de domínio**.
Caso você já tenha uma conta corporativa, seu nome de domínio estará listado.

>[!Note]
>Se você tiver uma assinatura ativa para o Microsoft Azure ou o Office 365, você já tem uma conta corporativa e suas credenciais de entrada devem ser as mesmas que as usadas para acessar esses serviços.