---
title: Adicionar locatários à sua Partner Center de dados
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como adicionar, consolidar ou gerenciar vários locatários do Azure AD em sua conta do Partner Center e saiba por que você pode querer fazer isso.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: caea2002b5edc2958c0af316762408e309bcf14a
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151195"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Adicionar e gerenciar vários locatários em sua Partner Center de gerenciamento


**Funções apropriadas:** administrador global | Administrador da conta

Este artigo discute como consolidar vários locatários Azure Active Directory (Azure AD) para sua empresa e, em seguida, adicioná-los e gerenciá-los em sua Partner Center conta. Há muitos motivos para fazer isso. Por exemplo:

- Digamos que sua empresa, Contoso, adquiriu outra empresa, Fabrikam. Você deseja que as duas empresas permaneçam separadas, mas deseja que os novos funcionários sejam capazes de usar Partner Center. Nesse caso, você associa o locatário do Azure AD da nova empresa à sua PGA (conta global de parceiro). Essa associação permite que os usuários em ambas as empresas trabalhem em Partner Center.

- Se você executar sua empresa com mais de um locatário (por exemplo, *contoso.com*, *contoso.uk* e contoso.in ), poderá usar *a* multitenuidade para a groupá-los na mesma conta de PC.

- Se as diretrizes de fusões e aquisições exigirem que você trabalhe  com locatários de ambas as empresas, você usaria os locatários constoso.com e *fabrikam.com* locatários.

- Os usuários de qualquer um dos locatários precisam ser capazes de:
    * Acesso Partner Center para treinamento, downloads digitais ou associação MCP (Microsoft Certified Professional).
    * Sejam atribuídas Partner Center funções como administrador Microsoft Partner Network (MPN) ou administrador de incentivos.

## <a name="add-an-azure-ad-tenant-to-your-account"></a>Adicionar um locatário do Azure AD à sua conta

1. Entre como administrador global no [Microsoft Partner Center](https://partner.microsoft.com/dashboard).

1. No canto superior direito, selecione **Configurações,** selecione **Configurações da conta** e, em seguida, **locatários.**
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Captura de tela do botão Associar no painel Perfil do Azure AD."::: 

1. Selecione **Associar** e, em seguida, indique o locatário que você deseja associar.

1. No prompt, entre como administrador global para o locatário que você deseja associar e, em seguida, selecione **confirmar**. 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Captura de tela do botão confirmar no painel confirmar nova associação do Azure AD."::: 

   Depois de confirmar a associação, será exibida uma mensagem de **todos os conjuntos** . Para exibir o locatário recém-adicionado, selecione **retornar ao gerenciamento de locatário**. 
 
>[!NOTE]
>Você não poderá associar um locatário a uma conta se ela já estiver associada a outra conta do centro do parceiro.


## <a name="remove-a-tenant-from-your-account"></a>Remover um locatário de sua conta
 
1. Entre como administrador global no [Microsoft Partner Center](https://partner.microsoft.com/dashboard).

1. No canto superior direito, selecione o ícone **configurações** e, em seguida, selecione **configurações de conta**.

1. No painel esquerdo, selecione **locatários**. Em **gerenciar locatários do Azure ad**, selecione a guia **parceiro** .
 
1. Selecione **remover** ao lado do locatário cuja associação você deseja remover.

   :::image type="content" source="images/disassociate.png" alt-text="Captura de tela das associações de locatário atuais e seus links de remoção.":::

   Conforme mostrado na captura de tela anterior, os links de **remoção** são habilitados para todos os locatários associados, exceto para o locatário primário e o locatário ao qual você está conectado no momento. 

   > [!NOTE]   
   > Quando você remove um locatário, os usuários nesse locatário não têm mais acesso à conta do Partner Center e a remoção pode ter um impacto sobre suas competências. 

## <a name="next-steps"></a>Próximas etapas

- [Criar contas de usuário](create-user-accounts-and-set-permissions.md)






