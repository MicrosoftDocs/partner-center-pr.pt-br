---
title: Inscrever-se no programa CSP
titleSuffix: Microsoft Cloud for US Government - Partner Center
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba mais sobre os requisitos do programa CSP para parceiros que desejam se registrar no programa do provedor de soluções na nuvem para Microsoft Cloud para o governo dos EUA.
author: mowrim
ms.author: mowrim
ms.localizationpriority: medium
ms.custom: SEOJUNE.20
ms.date: 10/05/2020
ms.openlocfilehash: e2b206b049050efa520099d74230d8535ac93793
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147166"
---
# <a name="enroll-in-the-cloud-solution-provider-program-for-microsoft-cloud-for-us-government"></a>Inscrever-se no programa Provedor de Soluções na Nuvem do Microsoft Cloud for US Government

**Aplica-se a**: Partner Center para Microsoft Cloud do governo dos EUA

**Funções apropriadas**: administrador global

Os parceiros da Microsoft agora podem vender soluções de nuvem da Microsoft e serviços para entidades federais, estaduais, locais e tribais dos EUA por meio do programa CSP (Provedor de Soluções na Nuvem) para Microsoft Cloud for US Government.

A Microsoft Cloud for US Government fornece uma instância privada, dedicada e isolada do Microsoft Azure para atender às necessidades dos requisitos de segurança, privacidade e conformidade do governo dos EUA. Sua empresa deve atender aos requisitos de qualificação da Microsoft para participar do programa CSP para Microsoft Cloud for US Government. Para obter mais informações, consulte [Partner Center do Microsoft Cloud for US Government](partner-center-for-microsoft-us-govt-cloud.md).

## <a name="before-you-begin"></a>Antes de começar

Antes de você poder se inscrever no programa CSP da Microsoft Cloud for US Government, precisamos verificar se sua empresa atende aos requisitos de venda para entidades do governo dos Estados Unidos. Antes de você iniciar o processo de inscrição, preencha o [formulário de Validação da Microsoft Government Cloud](https://azuregov.microsoft.com/csp) para que possamos verificar a qualificação da empresa. Depois de verificar a qualificação da empresa, forneceremos um locatário do Azure Active Directory (Azure AD) específico para a Microsoft Cloud for US Government.  

Para criar uma conta do Partner Center e se inscrever no CSP do Microsoft Cloud for US Government, você precisará fornecer as seguintes informações (talvez você queira coletar essas informações antes de iniciar o processo de inscrição):

- Credenciais de administrador global para o novo locatário do Azure AD da empresa para Microsoft Cloud for US Government.
- ID do MPN (Microsoft Partner Network) da sua empresa
- Um endereço comercial nos Estados Unidos

> [!IMPORTANT]  
> Caso tenha uma conta existente no Partner Center e deseje se registrar no CSP do Microsoft Cloud for US Government, você deve criar uma nova conta separada especificamente para o mercado do governo dos EUA.

## <a name="how-to-enroll"></a>Como se registrar

### <a name="step-1---create-a-partner-center-account-for-microsoft-cloud-for-us-government"></a>Etapa 1 - Criar uma conta do Partner Center para Microsoft Cloud for US Government

1. Inicie o processo de inscrição [aqui](https://partnercenter.microsoft.com/register/resellerusgjoinnow).

2. Entre com as credenciais de administrador global de locatário do Azure AD da organização para Microsoft Cloud for US Government. Se sua organização não tiver uma conta para esse portal, você pode solicitar uma ao preencher o [Formulário da Microsoft Government Cloud Validation](https://azuregov.microsoft.com/csp).

### <a name="step-2---apply-to-participate-in-the-cloud-solution-provider-program-for-microsoft-cloud-for-us-government"></a>Etapa 2 - Inscrever-se para participar do programa de Provedor de Soluções na Nuvem para Microsoft Cloud for US Government

1. Preencha as informações ausentes no formulário de inscrição, inclusive sua ID do Microsoft Partner Network e os detalhes de suporte de cliente da sua empresa.

2. Selecione **Aceitar e continuar**. Pode levar vários dias para que possamos analisar seu aplicativo. Enviaremos um email para você quando concluirmos nossa análise.

   > [!IMPORTANT]
   > Selecionando **Aceitar e continuar**, você estará confirmando que está autorizado a agir em nome da empresa, e está concordando em permitir que a Microsoft execute uma verificação de crédito em segundo plano antes de analisar o aplicativo de Provedor de Soluções na Nuvem da sua empresa.

### <a name="step-3---sign-the-reseller-agreement-for-microsoft-cloud-for-us-government"></a>Etapa 3 - Assinar o contrato de revendedor do Microsoft Cloud for US Government

1. Entre no Partner Center do Microsoft Cloud for US Government usando o link fornecido no email de aprovação do aplicativo.

2. Na página **contrato** , leia os termos e, se você concordar, selecione **aceitar e continuar** para assinar digitalmente o contrato de revendedor para Microsoft Cloud para o governo dos EUA. A criação da sua conta pode levar várias horas. Você pode sair do Partner Center para Microsoft Cloud para o governo dos EUA e, em seguida, entrar novamente mais tarde.

### <a name="step-4---assign-users-to-the-admin-agent-role-in-the-microsoft-azure-admin-portal-for-microsoft-cloud-for-us-government"></a>Etapa 4 - Atribua os usuários à função de agente administrador no portal do administrador do Microsoft Azure para Microsoft Cloud for US Government

O Microsoft Cloud for US Government fornece uma instância separada do Microsoft Azure que atende aos padrões de privacidade, segurança e conformidade do governo. Para permitir que os administradores gerenciem usuários e licenças no portal do Microsoft Azure, você precisará atribuir manualmente a função de agente administrador a eles.

> [!NOTE]
> Depois de atribuir os usuários a função de Agente administrador, elas poderão acessar a lista de clientes na página **Clientes** e [adicionar novos clientes](add-a-new-customer.md).

1. Entre no portal de administração do Microsoft Azure em [https://portal.azure.us/](https://portal.azure.us/) .

2. Atribua a função de Agente Administrador para os usuários apropriados em sua organização. Para fazer isso, você precisará adicioná-los ao grupo integrado **AdminAgent**. Consulte [Gerenciar os membros de um grupo no Azure Active Directory](/azure/active-directory/active-directory-groups-members-azure-portal) para obter informações sobre como fazer isso.

## <a name="connect-with-us"></a>Conecte-se conosco

- Perguntas? Envie o email para azgovcsp@microsoft.com

- Junte-se a nós no [Yammer](https://www.yammer.com/cloudpartnercommunity/#/threads/inGroup?type=in_group&feedId=11509777).

## <a name="next-steps"></a>Próximas etapas

- [Partner Center do Microsoft Cloud for US Government](partner-center-for-microsoft-us-govt-cloud.md)

- [Gerenciamento de usuários e licenças no Partner Center do Microsoft Cloud for US Government](user-management-in-partner-center-for-microsoft-us-govt-cloud.md)