---
title: Entidade de serviço do Azure AD | Partner Center
ms.topic: article
ms.date: 12/11/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Adicionar uma entidade de serviço ao seu locatário do Azure AD
author: LauraBrenner
ms.author: labrenne
Keywords: Azure, plano do Azure, entidade de serviço, aplicativo do Azure AD
robots: ''
ms.localizationpriority: High
ms.openlocfilehash: bd74d09445d9a2f1745c518362b26f243f00a777
ms.sourcegitcommit: 449cb8c32880217ad7543712b02a84ae69869289
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2020
ms.locfileid: "75716887"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>Adicionar um aplicativo do Azure AD (entidade de serviço) no Partner Center

No programa Marketplace Comercial no Partner Center agora é possível adicionar um aplicativo do Azure AD (entidade de serviço) como um usuário em sua conta do Partner Center. (Anteriormente era possível fazer isso em sua conta do CPP (Portal do Cloud Partner), mas agora que você migrou para o Partner Center, a conta do CPP é somente leitura.) Observe que a entidade de serviço equivale ao aplicativo do Azure AD.

## <a name="add-an-azure-ad-application-service-principal"></a>Adicionar um aplicativo do Azure AD (entidade de serviço)

1. No painel do Partner Center, selecione **Configurações** e, em seguida, selecione **Configurações do desenvolvedor**.

2. Selecione **Usuários** e, em seguida, selecione **Adicionar Aplicativos do Azure AD**.

3. Crie um aplicativo do Azure AD ou selecione um existente.

4. Se você criar um aplicativo do Azure AD, inclua as seguintes informações:  

  


**URL de resposta**: É a URL onde é possível que os usuários entrem para usar seu aplicativo do Azure AD. 

**URI da ID do aplicativo**: Ele é um identificador lógico do aplicativo Azure AD que é apresentado quando ele envia uma solicitação de logon único para o Azure AD. 

**Funções de segurança**: As funções de **Gerente** (equivalente à função de 'Proprietário' no CPP) e de **Desenvolvedor** (equivalente à função 'Colaborador' no CPP) se aplicam ao programa Marketplace Comercial no Partner Center e podem ser associadas a este aplicativo do Azure AD.  

  
