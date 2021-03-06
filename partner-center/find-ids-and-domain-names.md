---
title: Encontrar ID do locatário, nome de domínio, ID de objeto de usuário
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como encontrar IDs no portal do Azure – ID de locatário do Azure AD de uma organização, nome de domínio ou ID de objeto de usuário específica. Algumas tarefas precisam dessa informação.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 5da41cdbfa7aa1780b31e170a2398e8e7c65df27
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150855"
---
# <a name="locate-important-ids-for-a-user"></a>Localizar IDs importantes para um usuário

**Funções apropriadas**: administrador global

Este artigo descreve como usar o portal do Azure [para](https://portal.azure.com/) localizar as seguintes informações para um usuário:

- A Microsoft Azure Active Directory do locatário do Azure AD (Azure) da organização ou da empresa do usuário

- O nome de domínio primário da organização ou da empresa associada ao locatário do Azure AD

- A ID do objeto de usuário

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a>Encontre a ID Microsoft Azure AD locatário e o nome de domínio primário

Siga estas etapas para localizar a ID do locatário do Azure AD ou o nome de domínio primário no portal do Azure. (Se você quiser encontrar uma ID de locatário programaticamente, consulte Encontrar a ID do locatário com [o PowerShell ou a CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell).)

> [!NOTE]
> A ID do locatário pode ser chamada de nomes diferentes em diferentes aplicativos ou recursos. Por exemplo, a ID do locatário pode ser conhecida como a ID do diretório, o locatário do Azure Active Directory (Azure AD), a ID da Microsoft ou para determinados relatórios, até mesmo o *tenantguid*.

1. Entre no [portal do Azure](https://portal.azure.com/).

2. Selecione **Azure Active Directory** no menu.

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Mostra portal do Azure selecionando a Azure Active Directory no menu.":::

3. Uma página Azure Active Directory **Visão geral** é exibida. Para encontrar a ID do locatário do Azure AD ou o nome de domínio primário, procure o campo **ID** do locatário e o **campo Domínio** primário. Esses campos aparecem na seção Informações do locatário.

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Mostra a página Visão geral com dois campos realçadas, ID do locatário e nome de domínio primário.":::

4. Você pode encontrar a ID do locatário no portal do Azure de algumas outras maneiras. Selecione **Azure Active Directory** no menu. Em seguida, **localize a seção** Gerenciar no menu e selecione **Propriedades**.

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

