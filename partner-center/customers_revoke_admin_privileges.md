---
title: Os clientes delegam privilégios administrativos para parceiros | Partner Center
ms.topic: article
ms.date: 12/18/2018
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Como parceiro revendedor, seu cliente pode delegá-lo como administrador. Eles também podem remover privilégios.
author: LauraBrenner
ms.author: labrenne
keywords: privilégios de administrador delegados, admin em nome de, remover privilégios, DAP, AOBO
ms.localizationpriority: medium
ms.openlocfilehash: 35777dbdaa8ce77f4a1e7154447b37cd62772bc6
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "73653431"
---
# <a name="customers-delegate-administration-privileges-to-partners"></a>Os clientes delegam privilégios administrativos para parceiros

**Aplica-se a**

-  Partner Center

Para gerenciar um serviço ou inscrição de cliente em seu nome, o cliente deve conceder suas permissões de administrador para aquele serviço. Para receber permissões de administrador de um cliente, mande um e-mail para eles com uma solicitação de relação de revendedor. Depois do cliente aprovar sua solicitação, você será capaz de entrar no portal de admin do serviço e gerenciar o serviço em nome do cliente. 

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>Convide um cliente para estabelecer uma relação de revendedor com você

1.  Selecione **clientes** e, em seguida, selecione **solicitar uma relação de revendedor**.

2.  Na próxima página, reveja o rascunho da mensagem de email. Você pode abrir a mensagem rascunho em seu aplicativo de e-mail padrão ou pode copiar a mensagem para sua área de transferência e colá-lo no e-mail. 

    >[!IMPORTANT]
    >Você pode editar o texto no email, mas certifique-se de incluir o link, pois ele é personalizado, para vincular o cliente diretamente à sua conta. 
    
3.  Selecione **concluído** quando você concluiu esta etapa.

4.  Envie o email para seu cliente.

5.  Depois do cliente aceitar seu convite, eles aparecerão em sua página **Clientes**, e você poderá provisionar e gerenciar o serviço para o cliente a partir daí.

6.  Para gerenciar a conta, os serviços, os usuários e as licenças do cliente, expanda o registro do cliente selecionando a seta para baixo próximo ao nome e, em seguida, selecione o portal de administração para o serviço que você deseja gerenciar.

>[!IMPORTANT]  
>Os clientes podem reatribuir ou remover permissões de administrador no portal de administração de um serviço. No entanto, a menos e até que você renegocie seu contrato com o cliente, você continua a ser responsável por fornecer suporte ao cliente e por aderir aos termos do Contrato de revendedor de soluções de Nuvem da Microsoft, mesmo depois de um cliente reatribuir ou remover permissões de administrador. Nessa situação, se o cliente precisar de ajuda, entre em contato com o suporte da Microsoft para abrir uma solicitação de serviço em nome do cliente.

Seus clientes podem descobrir quais de seus parceiros têm privilégios de administrador para seus locatários no portal de administração do Office 365. Para fazer isso:

1. O cliente precisa entrar no portal de administração do Office 365 como um administrador global.

2. Selecione **configurações** > **relações de parceiro**.

3. Na página **relações de parceiro** , o cliente verá uma lista dos parceiros com os quais eles trabalham e os que receberam privilégios de administração delegada para seu locatário.

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>Os clientes podem gerenciar os privilégios de administrador delegado de um parceiro 

O cliente pode decidir remover os privilégios de administrador delegado do seu locatário, mas manter a relação com você para fins de renovação de assinatura e licença. Os clientes gerenciam direitos e permissões para suas contas do Office 365 na página **Relações de parceiro** no centro de administração do Office 365. Nessa página, os clientes podem:

- Ver com quais parceiros eles têm uma relação e quais parceiros têm privilégios de administrador

- Remover os privilégios de administração delegada de um parceiro do locatário

Para remover os privilégios de administrador delegado de um parceiro:

1. Na página **Relações de parceiro**, selecione o parceiro de interesse.
2. No painel de detalhes, selecione **Remover administrador delegado**.
3. No painel de confirmação, selecione **Remover**.

>[!IMPORTANT]  
>As atribuições de função do Azure AD para o parceiro são implícitas. Se você tentar listar os membros das funções do Azure AD usando o Portal do Azure AD/PowerShell/Graph, o parceiro não será retornado. Para descobrir se os parceiros estão atribuídos a funções do Azure AD, você deve consultar a página Relações de parceiro no Portal de Administração do Office 365 para saber se privilégios de administração delegada foram concedidos ao parceiro ou não.

## <a name="delegated-admin-privileges-in-azure-ad"></a>Privilégios de administração delegada no Azure AD 

Há dois grupos de segurança, agentes de administração e agentes de assistência técnica, no locatário do Azure AD do parceiro que são usados para administração delegada. Quando um cliente concede privilégios de administração delegada a um parceiro:

- O grupo de agente de administração é atribuído à função de administrador global no locatário do Azure AD do cliente.

- O grupo de agente de assistência técnica é atribuído à função de administrador de assistência técnica no locatário do Azure AD do cliente.

Com base nas funções de diretório atribuídas, os membros de ambos os grupos podem entrar no locatário do Azure AD do cliente e nos serviços do O365 usando suas credenciais de parceiro e administrador em nome do cliente.

Se o cliente remover privilégios de administrador delegado, as atribuições de função do Azure AD serão removidas e você não poderá mais gerenciar o locatário do Azure AD do cliente.

### <a name="azure-subscriptions-and-resource-management"></a>Assinaturas do Azure e gerenciamento de recursos

Cada assinatura do Azure tem seu próprio conjunto de funções de gerenciamento de recursos. Antes que um parceiro CSP possa gerenciar a assinatura do Azure de um cliente, o parceiro deve ser atribuído a uma ou mais funções na assinatura do Azure. Especificamente:

- Quando um cliente aceita um convite de revendedor e concede privilégios de administração delegada a um parceiro, o parceiro não obtém automaticamente acesso a assinaturas do Azure existentes no locatário do cliente.

- Quando o parceiro CSP provisiona uma nova assinatura do Azure para o cliente, o grupo Agentes de Administrador sob o locatário do parceiro CSP é automaticamente atribuído para a função Proprietário na assinatura. Com base nessa atribuição de função, os membros do grupo podem acessar e gerenciar recursos na assinatura.

- Quando um cliente remove privilégios de administração delegada de um parceiro usando o portal do Office 365, o parceiro ainda pode gerenciar a assinatura do Azure do cliente, desde que o parceiro ainda esteja atribuído a uma ou mais funções na assinatura. Para impedir o parceiro de gerenciar a assinatura do Azure, o cliente deve remover a atribuição de função.

## <a name="windows-autopilot"></a>Windows Autopilot

<!--Maggie, 12/5/18 - Removed table showing what different CSP partner types can and can't do because all partner types are now in parity. As per Bhavya Chopra in bug 19841770.-->

No Partner Center, os parceiros CSP podem gerenciar perfis de AutoPilot para seus clientes sem privilégios de administrador delegados sob estas circunstâncias: 

- Se um cliente remover privilégios de administração delegada, mas mantiver uma relação de revendedor com você, você poderá continuar a gerenciar perfis do AutoPilot para eles.

- Você pode gerenciar os dispositivos de clientes que você ou outro parceiro adicionou. 

- Você não pode gerenciar dispositivos que seu cliente adicionou por meio do Microsoft Store for Business, Microsoft Store for Education ou portal do Microsoft Intune.

Para obter mais informações sobre o piloto automático, consulte [simplificar a configuração do dispositivo com o Windows AutoPilot](https://docs.microsoft.com/partner-center/autopilot).

>[!IMPORTANT]  
>A experiência atual de gerenciamento de piloto automático no Partner Center pode continuar a mudar. No momento em que este artigo foi publicado, as seguintes alterações estão sendo consideradas:

- O parceiro deve receber privilégios de administração delegada do cliente para que o parceiro possa adicionar ou atualizar/remover perfis e aplicar/remover o perfil de qualquer dispositivo no locatário do cliente.

- O parceiro deve receber o privilégio de administração delegada pelo cliente para que o parceiro possa remover dispositivos adicionados por outros parceiros ou pelo cliente no locatário do cliente. Caso contrário, o parceiro poderá remover somente os dispositivos adicionados anteriormente pelo mesmo parceiro.
