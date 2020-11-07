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
ms.openlocfilehash: b88d6e11c7f4d56cf58d136a91b530688b3e5413
ms.sourcegitcommit: fdc32c0afce88f8266f75746ec15bf04745590ad
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/07/2020
ms.locfileid: "94360064"
---
# <a name="locate-important-ids-for-a-user"></a>Localizar IDs importantes para um usuário

Este artigo descreve como usar o [portal do Azure](https://portal.azure.com/) para localizar as seguintes informações para um usuário:

- A ID de locatário do Microsoft Azure Active Directory (Azure AD) da organização ou empresa do usuário

- O nome de domínio primário da organização ou da empresa associada ao locatário do Azure AD

- A ID do objeto de usuário

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a>Localizar a ID de locatário Microsoft Azure AD e o nome de domínio primário

Siga estas etapas para localizar a ID de locatário do Azure AD ou o nome de domínio primário dentro do portal do Azure. (Se você quiser encontrar uma ID de locatário programaticamente, consulte [Localizar ID de locatário com PowerShell ou CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell).)

> [!NOTE]
> A ID do locatário pode ser chamada de nomes diferentes em aplicativos ou recursos diferentes. Por exemplo, a ID do locatário pode ser referida como a ID do diretório, o locatário do Azure Active Directory (Azure AD), a ID da Microsoft ou para determinados relatórios, até mesmo o *tenantguid*.

1. Entre no [portal do Azure](https://portal.azure.com/).

2. Selecione **Azure Active Directory** no menu.

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Mostra portal do Azure selecionando a opção Azure Active Directory no menu.":::

3. Uma página de **visão geral** do Azure Active Directory é exibida. Para localizar a ID de locatário do Azure AD ou o nome de domínio primário, procure o campo **ID do locatário** e o campo **domínio primário** . Esses campos aparecem na seção informações do locatário.

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Mostra a página de visão geral com dois campos realçados, ID de locatário e nome de domínio primário.":::

4. Você pode encontrar a ID do locatário na portal do Azure de algumas outras maneiras. Selecione **Azure Active Directory** no menu. Em seguida, localize a seção **gerenciar** no menu e selecione **Propriedades**.

   A página Propriedades também exibe a ID de locatário associada do usuário.

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Mostra a página de propriedades com o campo ID de locatário realçado.":::

## <a name="find-the-user-object-id"></a>Localizar a ID de objeto de usuário

Apenas encontrar o nome de domínio e a ID de locatário nem sempre pode ser suficiente. Talvez você também precise localizar a ID de objeto específica atribuída a um usuário. Siga estas etapas para localizar a ID de objeto de um usuário no portal do Azure:

1. Entre no [portal do Azure](https://portal.azure.com/).

2. Selecione **Azure Active Directory** no menu.

3. Localize a seção **gerenciar** no menu e, em seguida, selecione **usuários**.

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Mostra Azure Active Directory menu com a opção Users realçada.":::

4. Na página usuários, digite o nome do usuário na caixa de pesquisa.

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Mostra a página de usuários com a caixa de pesquisa para procurar um usuário específico.":::

5. Selecione o nome do usuário onde ele aparece na lista.  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Mostra a página do usuário exibindo uma linha para o usuário pesquisado.":::

6. Localize a seção identidade na página de perfil do usuário. O campo ID de objeto aparece aqui com a ID de objeto exclusiva do usuário.

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Mostra a página de perfil do usuário com a seção de identidade e um campo realçado para a ID de objeto.":::

## <a name="next-steps"></a>Próximas etapas

- [Localize sua ID de locatário programaticamente com o PowerShell ou a CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [Saiba mais sobre perfis de usuário no Azure Active Directory](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [Descubra como os parceiros podem ver ou exportar detalhes do cliente no Partner Center](see-your-customer-list.md)
