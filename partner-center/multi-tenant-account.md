---
title: Adicionar locatários adicionais à sua conta do Partner Center
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como adicionar, consolidar ou gerenciar vários locatários do Azure AD em sua conta do Partner Center. Saiba também sobre alguns dos motivos pelos quais você pode querer fazer isso.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f9852b4e1c3997b82f744555db25fe64e1afc8ad
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182419"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Adicionar e gerenciar vários locatários em sua conta do Partner Center


**Funções apropriadas**

- Administrador global
- Administrador de conta

Esse recurso permite que você gerencie vários locatários para sua empresa e consolide-os em sua conta do Partner Center. Há muitas razões pelas quais você pode precisar gerenciar vários locatários do Azure AD em sua conta do Partner Center. Por exemplo:

- Sua empresa pode comprar outra empresa e você deseja que os funcionários da nova empresa possam usar o Partner Center. No entanto, você deseja que as duas empresas permaneçam separadas. Nesse caso, você associaria o locatário do Azure AD da nova empresa à sua conta global do parceiro (PGA). Essa associação permitiria que os usuários em ambas as empresas trabalhassem no Partner Center.

- Se você tiver mais de um locatário para executar seu negócio (por exemplo, contoso.com, contoso.uk, contoso.in), poderá usar multilocação para associá-los à mesma conta do PC.

- Fusões e aquisições exigem que você trabalhe com mais de um locatário (por exemplo, se a contoso adquire a Fabrikam, você precisaria ser capaz de usar os respectivos locatários Constoso.com e Fabrikam.com).

- Os usuários de qualquer um dos locatários precisariam ser capazes de:
    1.  Central de parceiros de acesso para treinamento, downloads digitais, associação MCP
    2.  Receber funções do Partner Center como administrador do MPN, incentivos para o administrador, etc.


## <a name="add-another-azure-ad-tenant-to-your-account"></a>Adicionar outro locatário do Azure AD à sua conta

1. Como administrador global, entre no [painel](https://partner.microsoft.com/dashboard)do Partner Center.
1. No ícone de **configurações** , selecione **configurações de conta** e, em seguida, selecione **locatários**.
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="associar locatários"::: 

3. Selecione **associar outro locatário do AD** e indique o locatário que você deseja associar.

1. Como administrador global, entre no locatário que você deseja associar e confirme a associação. 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="confirmar os locatários associados"::: 

5. Depois de confirmar, você verá um aviso de **tudo definido** .  Selecione **retornar ao gerenciamento de locatário** e você verá o locatário recém-adicionado listado. 
 

>[!NOTE]
>Você não poderá associar um locatário a uma conta se ela já estiver associada a outra conta do Partner Center.


## <a name="remove-a-tenant-from-your-account"></a>Remover um locatário de sua conta
 
1. Como administrador global, entre no [painel](https://partner.microsoft.com/dashboard)do Partner Center.

1. No ícone **configurações** , selecione **configurações da conta** -> locatários e clique na guia **parceiro** .
 
3. Clique em **remover** para o locatário que você deseja dissociar.

4. Dissociar um locatário significa que os usuários nesse locatário não terão mais acesso à conta do Partner Center e isso poderá afetar suas competências. 

O botão **remover** está habilitado para todos os locatários associados, exceto o locatário primário e o locatário ao qual você está conectado no momento.

:::image type="content" source="images/disassociate.png" alt-text="locatários com o botão remover":::
 

## <a name="next-steps"></a>Próximas etapas

- [Adicionar usuários](create-user-accounts-and-set-permissions.md)






