---
title: Os clientes delegam privilégios administrativos para parceiros | Partner Center
ms.topic: article
ms.date: 12/7/2018
description: Como um parceiro revendedor, seu cliente pode delegar você para ser seu administrador. Eles também podem remover privilégios.
author: labrenne
ms.author: labrenne
keywords: privilégios de administrador, administrador em nome de, remover privilégios, DAP, AOBO
ms.localizationpriority: medium
ms.openlocfilehash: bb92bca26c3b6c73750a5bc02f2833172006d0ff
ms.sourcegitcommit: 777225c8bf16e4a8811a9d88aceb45fcba1cd959
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2018
ms.locfileid: "8917498"
---
# <a name="customers-delegate-administration-privileges-to-partners"></a>Os clientes delegam privilégios administrativos para parceiros

**Aplica-se ao**

-  Partner Center

Para gerenciar um serviço ou inscrição de cliente em seu nome, o cliente deve conceder suas permissões de administrador para aquele serviço. Para receber permissões de administrador de um cliente, mande um e-mail para eles com uma solicitação de relação de revendedor. Depois do cliente aprovar sua solicitação, você será capaz de entrar no portal de admin do serviço e gerenciar o serviço em nome do cliente. 

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>Convide um cliente para estabelecer uma relação de revendedor com você

1.  Selecione **os clientes** e, em seguida, selecione **solicitar uma relação de revendedor**.

2.  Na página seguinte, reveja o rascunho da mensagem de e-mail. Você pode abrir a mensagem rascunho em seu aplicativo de e-mail padrão ou pode copiar a mensagem para sua área de transferência e colá-lo no e-mail. 

    >[!IMPORTANT]
    >Você pode editar o texto no e-mail, mas certifique-se de incluir o link, pois ele é personalizado, para vincular o cliente diretamente a sua conta. 
    
3.  Selecione **Concluído** quando tiver completado essa tarefa.

4.  Envie o e-mail para seu cliente.

5.  Depois do cliente aceitar seu convite, eles aparecerão em sua página **Clientes**, e você poderá provisionar e gerenciar o serviço para o cliente a partir daí.

6.  Para gerenciar a conta do cliente, serviços, usuários e licenças, expanda o registro do cliente, selecionando a seta para baixo perto de seu nome e, em seguida, selecione o portal do administrador para o serviço que você deseja gerenciar.

>[!IMPORTANT]  
>Os clientes podem reatribuir ou remover permissões de administrador no portal do administrador do serviço. No entanto, a menos e até que você renegocie seu contrato com o cliente, você continua a ser responsável por fornecer suporte ao cliente e por aderir aos termos do Contrato de revendedor de soluções de Nuvem da Microsoft, mesmo depois de um cliente reatribuir ou remover permissões de administrador. Nessa situação, se o cliente precisar de Ajuda, contate o suporte da Microsoft para abrir uma solicitação de serviço em nome do cliente.

Os clientes podem saber quais de seus parceiros têm privilégios de administrador para seu locatário no portal de administração do Office 365. Para fazer isso:

1. O cliente precisa fazer logon no portal de administração do Office 365, como um Administrador Global.

2. Selecione **Configurações** → **Relações de parceiro**.

3. Na página **relações de parceiro** , o cliente verá uma lista de parceiros com quem eles funcionam e aqueles que receberam privilégios de administração para seu locatário.

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>Os clientes podem gerenciar os privilégios de administrador delegado de um parceiro 

Seu cliente pode optar por remover seus privilégios de administrador delegado do locatário, mas manter o relacionamento com você para fins de renovação de licença e assinatura. Os clientes gerenciam direitos e permissões para suas contas do Office 365 na página **Relações de parceiro** no centro de administração do Office 365. Nessa página, os clientes podem:

- Ver com quais parceiros eles têm uma relação e quais parceiros têm privilégios de administrador

- Remover os privilégios de administrador delegado de um parceiro do locatário

Para remover os privilégios de administrador delegado de um parceiro:

1. Na página **Relações de parceiro**, selecione o parceiro de interesse.
2. No painel de detalhes, selecione **Remover administrador delegado**.
3. No painel de confirmação, selecione **Remover**.

>[!IMPORTANT]  
>As atribuições de função do Azure AD para o parceiro são implícitas. Se você tentar listar os membros das funções do Azure AD usando o Portal do Azure AD/PowerShell/Graph, o parceiro não será retornado. Para descobrir se os parceiros estão atribuídos a funções do Azure AD, você deve consultar a página Relações de parceiro no Portal de Administração do Office 365 para saber se privilégios de administração delegada foram concedidos ao parceiro ou não.

## <a name="delegated-admin-privileges-in-azure-ad"></a>Privilégios de administração delegada no Azure AD 

Há dois grupos de segurança, Agentes de Administração e Agentes de Suporte Técnico, no locatário do Azure AD do parceiro, que são usados para administração delegada. Quando um cliente concede privilégios de administração delegada a um parceiro:

- O grupo Agente Administrador é atribuído à função Administrador Global no locatário do Azure AD do cliente.

- O grupo Agente de Suporte Técnico é atribuído à função Administrador de Suporte Técnico no locatário do Azure AD do cliente.

Com base nas funções do diretório atribuídas, membros de ambos os grupos podem entrar no locatário do Azure AD e nos serviços do O365 do cliente usando suas credenciais de parceiros e administrador em nome do cliente.

Se o cliente remover privilégios de administrador, as atribuições de função do Azure AD serão removidas, e você não poderá gerenciar o locatário do Azure AD do cliente.

### <a name="azure-subscriptions-and-resource-management"></a>Assinaturas do Azure e gerenciamento de recursos

Cada assinatura do Azure tem seu próprio conjunto de funções de gerenciamento de recursos. Para que um parceiro CSP possa gerenciar a assinatura do Azure do cliente, o parceiro deve ser atribuído a uma ou mais funções na assinatura do Azure. Especificamente:

- Quando um cliente aceita um convite de revendedor e concede privilégios de administração delegada a um parceiro, o parceiro não obtém automaticamente acesso a assinaturas do Azure existentes no locatário do cliente.

- Quando o parceiro CSP provisiona uma nova assinatura do Azure para o cliente, o grupo Agentes de Administrador sob o locatário do parceiro CSP é automaticamente atribuído para a função Proprietário na assinatura. Com base nessa atribuição de função, os membros do grupo podem acessar e gerenciar recursos na assinatura.

- Quando um cliente remove privilégios de administração delegada de um parceiro usando o Portal do Office 365, o parceiro ainda pode gerenciar a assinatura do Azure do cliente, contanto que o parceiro ainda esteja atribuído a uma ou mais funções na assinatura. Para impedir o parceiro de gerenciar a assinatura do Azure, o cliente deve remover a atribuição de função.

## <a name="windows-autopilot"></a>Windows Autopilot

<!--Maggie, 12/5/18 - Removed table showing what different CSP partner types can and can't do because all partner types are now in parity. As per Bhavya Chopra in bug 19841770.-->

Do Partner Center, os parceiros CSP podem gerenciar perfis Autopilot para seus clientes sem privilégios de administrador seguintes circunstâncias: 

- Se um cliente remove privilégios de administração, mas mantém uma relação de revendedor com você, você pode continuar a gerenciar perfis Autopilot para eles.

- Você pode gerenciar dispositivos de cliente que você ou outro parceiro adicionados. 

- Você não pode gerenciar dispositivos que seu cliente tiver adicionado por meio do Microsoft Store para empresas, a Microsoft Store para educação ou o Portal do Microsoft Intune.

Para obter mais informações sobre o Autopilot, consulte [Simplifique a instalação de dispositivo com o Windows Autopilot](https://docs.microsoft.com/partner-center/autopilot).

>[!IMPORTANT]  
>A experiência de gerenciamento Autopilot atual no Partner Center pode continuar a alterar. No momento em que este artigo foi publicado, as seguintes alterações estão sendo consideradas:

- O parceiro deve receber privilégios de administração delegada do cliente para que o parceiro possa adicionar ou atualizar/remover perfis e aplicar/remover o perfil de qualquer dispositivo no locatário do cliente.

- Parceiro deve receber privilégios de administração delegada do cliente que o parceiro possa remover dispositivos adicionados por outros parceiros ou pelo cliente no locatário do cliente. Caso contrário, o parceiro pode remover somente dispositivos adicionados anteriormente pelo mesmo parceiro.
