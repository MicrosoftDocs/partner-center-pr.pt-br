---
title: Principal de serviço do Azure AD
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Descubra como adicionar uma entidade de serviço ao seu inquilino do Azure AD. Fazer isso significa adicionar um aplicativo do Azure AD (principal de serviço) no Partner Center.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 3698032a632384e8416664c9564819d7c4da9c38
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551547"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>Adicionar um aplicativo do Azure AD (entidade de serviço) no Partner Center

**Funções apropriadas**: administrador global

No programa Marketplace Comercial no Partner Center, agora você pode adicionar um aplicativo do Microsoft Azure AD (Active Directory) (entidade de serviço) como usuário na sua conta do Partner Center. (Você podia fazer isso anteriormente em sua conta do CPP (Portal do Cloud Partner)). Agora que você migrou para o Partner Center, a conta do CPP é somente leitura.)
 
>[!Note] 
>A entidade de serviço equivale ao aplicativo do Azure AD.

## <a name="add-an-azure-ad-application-service-principal"></a>Adicionar um aplicativo do Azure AD (entidade de serviço)

1. No painel do Partner Center, selecione **Configurações** e, em seguida, selecione **Configurações do desenvolvedor**.

2. Selecione **Usuários** e, em seguida, selecione **Adicionar Aplicativos do Azure AD**.

3. Crie um aplicativo do Azure AD ou selecione um existente.

4. Se você criar um aplicativo do Azure AD, inclua as seguintes informações:  

   - **URL de resposta**: A URL em que os usuários podem entrar para usar seu aplicativo Azure AD.

   - **URI da ID do aplicativo**: Um identificador lógico do aplicativo Azure AD que é apresentado quando ele envia uma solicitação de logon único para o Azure AD.

   - **Funções de segurança**: As funções de **Gerente** (equivalente à função de 'Proprietário' no CPP) e de **Desenvolvedor** (equivalente à função 'Colaborador' no CPP) se aplicam ao programa Marketplace Comercial no Partner Center e podem ser associadas a este aplicativo do Azure AD.  

## <a name="next-steps"></a>Próximas etapas

- [Visão geral do marketplace comercial no Partner Center](csp-commercial-marketplace-overview.md)