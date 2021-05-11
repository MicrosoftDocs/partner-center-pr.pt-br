---
title: Localizar ID de locatário, nome de domínio, ID de objeto de usuário
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como localizar IDs no portal do Azure-ID de locatário do Azure AD, nome de domínio ou ID de objeto de usuário específico de uma organização. Algumas tarefas precisam dessas informações.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 643b1eeb96a47ee4c438f733efe3be22234d02ff
ms.sourcegitcommit: e462f562e7f26b7d6870c22638a2a841499109d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2021
ms.locfileid: "109740277"
---
# <a name="locate-important-ids-for-a-user"></a>Localizar IDs importantes para um usuário

**Funções apropriadas**

- Administrador global

Este artigo descreve como usar o [portal do Azure](https://portal.azure.com/) para localizar as seguintes informações para um usuário:

- A ID de locatário do Microsoft Azure Active Directory (Azure AD) da organização ou empresa do usuário

- O nome de domínio primário da organização ou da empresa associada ao locatário do Azure AD

- A ID do objeto de usuário

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a>Localizar a ID de locatário Microsoft Azure AD e o nome de domínio primário

Siga estas etapas para localizar a ID de locatário do Azure AD ou o nome de domínio primário dentro do portal do Azure. (Se você quiser encontrar uma ID de locatário programaticamente, consulte [Localizar ID de locatário com PowerShell ou CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell).)

> [!NOTE]
> A ID do locatário pode ser chamada de nomes diferentes em aplicativos ou recursos diferentes. Por exemplo, a ID do locatário pode ser referida como a ID do diretório, o locatário do Azure Active Directory (Azure AD), a ID da Microsoft ou para determinados relatórios, até mesmo o *tenantguid*.

1. Entre no [portal do Azure](https://portal.azure.com/).

2. Selecione **Azure Active Directory** no menu.

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Mostra portal do Azure selecionando a opção Azure Active Directory no menu.":::

3. Uma página de **visão geral** do Azure Active Directory é exibida. Para localizar a ID de locatário do Azure AD ou o nome de domínio primário, procure o campo **ID do locatário** e o campo **domínio primário** . Esses campos aparecem na seção informações do locatário.

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Mostra a página de visão geral com dois campos realçados, ID de locatário e nome de domínio primário.":::

4. Você pode encontrar a ID do locatário na portal do Azure de algumas outras maneiras. Selecione **Azure Active Directory** no menu. Em seguida, localize a seção **gerenciar** no menu e selecione **Propriedades**.

   A página Propriedades também exibe a ID de Locatário associada do usuário.

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Mostra a página Propriedades com o campo ID do Locatário realçada.":::

## <a name="find-the-user-object-id"></a>Encontrar a ID do objeto de usuário

Encontrar apenas o nome de domínio e a ID do locatário pode nem sempre ser suficiente. Talvez você também precise localizar a ID de objeto específica atribuída a um usuário. Siga estas etapas para encontrar a ID de objeto de um usuário no portal do Azure:

1. Entre no [portal do Azure](https://portal.azure.com/).

2. Selecione **Azure Active Directory** no menu.

3. Localize **a seção** Gerenciar no menu e, em seguida, selecione **Usuários**.

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Mostra Azure Active Directory menu com realçada, opção Usuários.":::

4. Na página Usuários, digite o nome do usuário na caixa de pesquisa.

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Mostra a página Usuários com a caixa de pesquisa para pesquisar um usuário específico.":::

5. Selecione o nome do usuário em que ele aparece na lista.  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Mostra a página Usuário exibindo uma linha para o usuário pesquisado.":::

6. Localize a seção Identidade na página Perfil do usuário. O campo ID do objeto aparece aqui com a ID de objeto exclusiva do usuário.

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Mostra a página Perfil do Usuário com a seção Identidade e um campo realçado para A ID do Objeto.":::

## <a name="next-steps"></a>Próximas etapas

- [Encontrar sua ID de locatário programaticamente com o PowerShell ou a CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [Saiba mais sobre perfis de usuário no Azure Active Directory](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [Descubra como os parceiros podem ver ou exportar detalhes do cliente Partner Center](see-your-customer-list.md)

