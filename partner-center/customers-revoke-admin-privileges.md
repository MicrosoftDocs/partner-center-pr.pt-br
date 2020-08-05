---
title: Obter privilégios de administrador do cliente
ms.topic: how-to
ms.date: 06/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenha as permissões necessárias para gerenciar o serviço ou a assinatura de um cliente em nome dele. Saiba como as permissões são concedidas, revogadas e gerenciadas.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.openlocfilehash: dcfc552016560ecc3167deebf96f7a75a72048bc
ms.sourcegitcommit: 8dc139749916c822c5c438f54a03d2f147697dd5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/04/2020
ms.locfileid: "87545897"
---
# <a name="obtain-permissions-to-manage-a-customers-service-or-subscription"></a>Obter permissões para gerenciar o serviço ou a assinatura de um cliente

**Aplica-se a**

- Partner Center

**Funções apropriadas**

- Agente administrativo
- Agente de vendas

Para gerenciar um serviço ou uma assinatura de um cliente em nome dele, o cliente precisa conceder a você as permissões de administrador nesse serviço. Para receber permissões de administrador de um cliente, envie um email a ele com uma solicitação de relacionamento de revendedor. Depois que o cliente aprovar sua solicitação, você poderá fazer logon no portal de administração do serviço e gerenciar o serviço em nome do cliente. 

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>Convide um cliente para estabelecer uma relação de revendedor com você

1.  Selecione **Clientes** e, em seguida, **Solicitar um relacionamento de revendedor**.

2.  Na próxima página, reveja o rascunho da mensagem de email. Você pode abrir a mensagem de rascunho em seu aplicativo de email padrão ou copiar a mensagem para a área de transferência e colá-la em um email. 

    >[!IMPORTANT]
    >Você pode editar o texto no email, mas certifique-se de incluir o link, pois ele é personalizado, para vincular o cliente diretamente à sua conta. 
    
3.  Selecione **Concluído** quando tiver completado essa etapa.

4.  Envie o email para seu cliente.

5.  Depois que o cliente aceitar seu convite, ele será exibido na página **Clientes**, e você poderá provisionar e gerenciar o serviço para o cliente nela.

6.  Para gerenciar a conta, os serviços, os usuários e as licenças do cliente, expanda o registro do cliente selecionando a seta para baixo próximo ao nome e, em seguida, selecione o portal de administração do serviço que deseja gerenciar.

>[!IMPORTANT]  
>Os clientes podem transferir ou remover as permissões de administrador no portal de administração de um serviço. No entanto, a menos e até que você renegocie seu contrato com o cliente, você continua sendo responsável por fornecer suporte ao cliente e cumprir os termos do Contrato do Revendedor de Soluções de Nuvem, mesmo depois de um cliente transferir ou remover as permissões de administrador. Nessa situação, se o cliente precisar de ajuda, entre em contato com o Suporte da Microsoft para abrir uma solicitação de serviço em nome do cliente.

Os clientes podem descobrir quais dos parceiros têm privilégios de administrador no respectivo locatário no portal de administração do Office 365. Para fazer isso:

1. O cliente precisa entrar no portal de administração do Office 365 como administrador global.

2. Selecione **Configurações** > **Relacionamentos de parceiro**.

3. Na página **Relacionamentos de parceiro**, o cliente verá uma lista dos parceiros com quem ele trabalha e aqueles que receberam privilégios de administração delegada para o respectivo locatário.

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>Os clientes podem gerenciar os privilégios de administrador delegado de um parceiro 

Seu cliente pode optar por remover seus privilégios de administrador delegado por meio do locatário, mas manter o relacionamento com você, para fins de renovação de licença e de assinatura. Os clientes gerenciam direitos e permissões nas respectivas contas do Office 365 na página **Relacionamentos de parceiro** no centro de administração do Office 365. Nessa página, os clientes podem:

- Ver com quais parceiros eles têm um relacionamento e quais parceiros têm privilégios de administrador delegado

- Remover os privilégios de administração delegada de um parceiro por meio do locatário

Para remover os privilégios de administrador delegado de um parceiro:

1. Na página **Relacionamentos de parceiro**, selecione o parceiro de interesse.
2. No painel de detalhes, selecione **Remover administrador delegado**.
3. No painel de confirmação, selecione **Remover**.

>[!IMPORTANT]  
>As atribuições de função do Azure AD para o parceiro são implícitas. Se você tentar listar os membros das funções do Azure AD usando o portal do Azure AD/o PowerShell/o Graph, o parceiro não será retornado. Para descobrir se os parceiros estão atribuídos a funções do Azure AD, você precisará consultar a página Relacionamentos de parceiro no portal de administração do Office 365 para saber se o privilégio de administração delegada foi concedido ao parceiro.

## <a name="delegated-admin-privileges-in-azure-ad"></a>Privilégios de administrador delegado no Azure AD 

Há dois grupos de segurança, Agentes administrativos e Agentes da assistência técnica, no locatário do Azure AD do parceiro, que são usados para administração delegada. Quando um cliente concede o privilégio de administração delegada a um parceiro:

- O grupo Agente administrativo é atribuído à função de administrador global no locatário do Azure AD do cliente.

- O grupo Agentes da assistência técnica é atribuído à função Administrador da assistência técnica no locatário do Azure AD do cliente.

Com base nas funções do diretório atribuídas, os membros dos dois grupos podem entrar no locatário do Azure AD e nos serviços do O365 do cliente usando as respectivas credenciais de parceiro e administrador em nome do cliente.

Se o cliente remover os privilégios de administrador delegado, as atribuições de função do Azure AD serão removidas, e você não poderá mais gerenciar o locatário do Azure AD do cliente.

### <a name="azure-subscriptions-and-resource-management"></a>Assinaturas do Azure e gerenciamento de recursos

Cada assinatura do Azure tem o próprio conjunto de funções de gerenciamento de recursos. Para que um parceiro CSP possa gerenciar a assinatura do Azure de um cliente, ele precisa receber uma ou mais funções na assinatura do Azure. Especificamente:

- Quando um cliente aceita um convite de revendedor e concede o privilégio de administração delegada a um parceiro, o parceiro não obtém automaticamente o acesso às assinaturas do Azure existentes no locatário do cliente.

- Quando o parceiro CSP provisiona uma nova assinatura do Azure para o cliente, o grupo Agentes administrativos no locatário do parceiro CSP recebe automaticamente a função de proprietário na assinatura. Com base nessa atribuição de função, os membros do grupo podem acessar e gerenciar recursos na assinatura.

- Quando um cliente remove os privilégios de administração delegada de um parceiro usando o Portal do Office 365, o parceiro ainda pode gerenciar a assinatura do Azure do cliente, desde que o parceiro ainda esteja atribuído a uma ou mais funções na assinatura. Para impedir o parceiro de gerenciar a assinatura do Azure, o cliente precisará remover a atribuição de função.

## <a name="windows-autopilot"></a>Windows Autopilot

No Partner Center, os parceiros CSP podem gerenciar perfis do Autopilot para os clientes sem privilégios de administrador delegado nestas circunstâncias: 

- Se um cliente remover os privilégios de administração delegada, mas mantiver um relacionamento de revendedor com você, você poderá continuar gerenciando perfis do Autopilot para ele.

- Você pode gerenciar os dispositivos dos clientes adicionados por você ou por outro parceiro. 

- Você não pode gerenciar os dispositivos adicionados pelo cliente por meio da Microsoft Store para Empresas, da Microsoft Store para Educação ou do Portal do Microsoft Intune.

Para obter mais informações sobre o Autopilot, confira [Simplificar a configuração dos dispositivos com o Windows Autopilot](autopilot.md).

>[!IMPORTANT]  
>A experiência atual de gerenciamento do Autopilot no Partner Center poderá continuar sendo alterada. No momento da publicação deste artigo, as seguintes alterações foram consideradas:

- O parceiro precisa receber o privilégio de administração delegada do cliente para adicionar/atualizar/remover perfis e aplicar/remover o perfil de qualquer dispositivo no locatário do cliente.

- O parceiro precisa receber o privilégio de administração delegada do cliente para remover os dispositivos adicionados por outros parceiros ou pelo cliente no locatário do cliente. Caso contrário, o parceiro só poderá remover os dispositivos adicionados anteriormente pelo mesmo parceiro.
