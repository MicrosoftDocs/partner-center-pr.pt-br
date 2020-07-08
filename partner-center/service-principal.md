---
title: Principal de serviço do Azure AD
ms.topic: article
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Descubra como adicionar uma entidade de serviço ao seu inquilino do Azure AD. Fazer isso significa adicionar um aplicativo do Azure AD (principal de serviço) no Partner Center.
author: dhirajgandhi
ms.author: dhgandhi
Keywords: Azure, plano do Azure, entidade de serviço, aplicativo do Azure AD
robots: ''
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: bd2880f57d1ccb3c3675fef4fae7499f7ac02f4b
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/03/2020
ms.locfileid: "85949626"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>Adicionar um aplicativo do Azure AD (entidade de serviço) no Partner Center

No programa Marketplace Comercial no Partner Center agora é possível adicionar um aplicativo do Azure AD (entidade de serviço) como um usuário em sua conta do Partner Center. (Você conseguiu fazer isso anteriormente em sua conta do Cloud Partner Portal ou CPP. Agora que você migrou para o Partner Center, a conta do CPP é somente leitura.)
 
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
