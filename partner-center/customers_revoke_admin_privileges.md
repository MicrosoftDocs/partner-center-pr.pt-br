---
title: Os clientes delegam privilégios administrativos para parceiros | Partner Center
description: Como um parceiro revendedor, seu cliente pode delegar você para ser seu administrador. Ele também pode remover privilégios.
author: labrenne
keywords: privilégios de administrador delegado, administrador em nome de, remover privilégios
ms.openlocfilehash: 7f1bd81f40892f851e1582a7a842a64c55e4ff63
ms.sourcegitcommit: 93968695897114a68d5e948d13a36127a4079b6f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2018
ms.locfileid: "1913939"
---
# <a name="customers-delegate-administration-privileges-to-partners"></a>Os clientes delegam privilégios administrativos para parceiros

**Aplica-se ao**

-  Partner Center

Como parceiro CSP e consultor confiável para seus clientes, eles podem delegar você para ser o administrador para seu locatário do Azure AD e do Office 365. Você pode iniciar esse relacionamento por meio do Painel de Parceiros enviando-lhes um convite. 

1. No **Painel**, selecione **Clientes** e **Solicitar uma relação de revenda**.
2. Será exibido um email de formulário que contém sua url. Você pode copiar e colar o formulário em um email para enviar ao cliente. Fique à vontade para incluir informações adicionais, mas não se esqueça de que incluir a url. O cliente usará essa url para responder à sua solicitação.  
3. Quando o cliente aceitar o convite, você se tornará o administrador para seus serviços.

Os clientes podem saber quais de seus parceiros têm privilégios de administrador para seu locatário no portal de serviço do Office 365. Para fazer isso:

1. Entre no [portal de Administração do Office 365](https://portal.office.com/adminportal) como Administrador Global.
2. Selecione **Configurações** → **Relações de parceiro**.
3. Na página **Relações de parceiro**, eles verão uma lista de parceiros com quem trabalham e aqueles que receberam privilégios de administração para seu locatário.

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>Os clientes podem gerenciar os privilégios de administrador delegado de um parceiro 

Seu cliente pode optar por remover seus privilégios de administrador do locatário, mas manter o relacionamento com você, para fins de renovação de licença e de assinatura. Os clientes gerenciam direitos e permissões para suas contas do Office 365 na página **Relações de parceiro** no centro de administração do Office 365. Nessa página, os clientes podem:

- Ver com quais parceiros eles têm uma relação e quais parceiros têm privilégios de administrador

- Remover os privilégios de administrador delegado de um parceiro do locatário

Para remover os privilégios de administrador delegado de um parceiro:

1. Na página **Relações de parceiro**, selecione o parceiro de interesse.
2. No painel de detalhes, selecione **Remover administrador delegado**.
3. No painel de confirmação, selecione **Remover**.

>**Importante**<br>
As atribuições de função do Azure AD para o parceiro são implícitas. Se você tentar listar os membros das funções do Azure AD usando o Portal do Azure AD/PowerShell/Graph, o parceiro não será retornado. Para descobrir se os parceiros estão atribuídos a funções do Azure AD, você deve consultar a página Relações de parceiro no Portal de Administração do Office 365 para saber se privilégios de administração delegada foram concedidos ao parceiro ou não.

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

## <a name="windows-autopilot"></a>Windows AutoPilot 

No Painel de Parceiros, os parceiros CSP podem gerenciar a configuração AutoPilot para seus clientes mesmo sem privilégios de administrador. Saiba como [Simplificar a configuração dos dispositivos com o Windows Autopilot.](https://docs.microsoft.com/partner-center/autopilot)

O que você pode fazer depende de você ser um revendedor direto ou indireto.

|**Operação**   |**Revendedor direto ou indireto**   |**Revendedor indireto**   |
|-----------------|-----------------------------------| -----------------------------|
|Adicionar dispositivos (usando um arquivo csv)  |Sim      |Não|
|Remover dispositivos   |Sim   |Não|
|Adicionar perfil   |Sim   | Sim   |
|Atualizar perfil   |Sim    |Sim   |
|Remover perfil   |Sim   |Sim   |
|Aplicar perfil a dispositivos   |Sim   |Sim   |
|Remover perfil de dispositivos   |Sim   |Sim   | 

- Os parceiros CSP podem continuar a gerenciar a configuração AutoPilot para clientes existentes com a relação de Revendedor, mesmo que os clientes tenham removido o privilégio de administração delegada de seus parceiros.

- Você pode gerenciar dispositivos existentes para seus clientes que foram adicionados por você ou por outro parceiro CSP.

- Você não pode gerenciar dispositivos que seu cliente carregou (via Microsoft Store para Empresas ou Portal do Microsoft Intune).

>**Importante** A experiência de gerenciamento AutoPilot atual no Microsoft Partner Center não é final e está sujeita a mudanças no futuro. No momento da elaboração deste artigo, as seguintes alterações estão sendo consideradas:

  - O parceiro deve receber privilégios de administração delegada do cliente para que o parceiro possa adicionar ou atualizar/remover perfis e aplicar/remover o perfil de qualquer dispositivo no locatário do cliente.

- O parceiro deve receber privilégios de administração delegada do cliente para que possa remover dispositivos carregados por outros parceiros ou pelo cliente no locatário do cliente. Caso contrário, o parceiro só poderá remover dispositivos adicionados anteriormente pelo mesmo parceiro.
