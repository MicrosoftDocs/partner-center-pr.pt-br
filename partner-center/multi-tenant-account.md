---
title: Adicionar locatários à sua conta do Partner Center
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como adicionar, consolidar ou gerenciar vários locatários do Azure AD em sua conta do Partner Center e saber por que você talvez queira fazer isso.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2f3094489f65b7164b4a55804047f9a4ab5f11cb
ms.sourcegitcommit: 79d2f00c352db61252e523f45abf93fe2a2742a5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "102124798"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Adicionar e gerenciar vários locatários em sua conta do Partner Center


**Funções apropriadas**

- Administrador global
- Administrador de conta

Este artigo discute como consolidar vários locatários do Azure Active Directory (Azure AD) para sua empresa e, em seguida, adicioná-los e gerenciá-los em sua conta do Partner Center. Há muitas razões para fazer isso. Por exemplo: 

- Digamos que sua empresa, contoso, tenha adquirido outra empresa, fabrikam. Você quer que as duas empresas permaneçam separadas, mas você deseja que os novos funcionários possam usar o Partner Center. Nesse caso, você associa o locatário do Azure AD da nova empresa à sua conta global do parceiro (PGA). Essa associação permite que os usuários em ambas as empresas trabalhem no Partner Center.

- Se você executar sua empresa com mais de um locatário (por exemplo, *contoso.com*, *contoso.uk* e *contoso.in*), poderá usar o multilocação para agrupá-los na mesma conta de PC.

- Se as diretrizes de fusões e aquisições exigirem que você trabalhe com locatários de ambas as empresas, você usaria os locatários *constoso.com* e *fabrikam.com* .

- Os usuários de qualquer um dos locatários precisam ser capazes de:
    * Acesse o Partner Center para treinamento, downloads digitais ou a Associação Microsoft Certified Professional (MCP).
    * Ser atribuídas funções do Partner Center como administrador de Microsoft Partner Network (MPN) ou de incentivos.

## <a name="add-an-azure-ad-tenant-to-your-account"></a>Adicionar um locatário do Azure AD à sua conta

1. Entre como administrador global no [Microsoft Partner Center](https://partner.microsoft.com/dashboard).

1. No canto superior direito, selecione **configurações**, selecione **configurações de conta** e, em seguida, selecione **locatários**.
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Captura de tela do botão associar no painel de perfil do Azure AD."::: 

1. Selecione **associar** e, em seguida, indique o locatário que você deseja associar.

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






