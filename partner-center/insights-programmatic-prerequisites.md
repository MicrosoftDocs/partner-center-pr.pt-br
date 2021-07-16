---
title: Pré-requisitos para acessar dados de análise programaticamente
description: Pré-requisitos para acessar dados de análise programaticamente
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: d4c39025aa3804435dd4d2359b93cd4a2e13ccc4
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114374785"
---
# <a name="prerequisites-to-programmatically-access-analytics-data"></a>Pré-requisitos para acessar dados de análise programaticamente

**Funções apropriadas:** Administrador global | Administrador do MPN

Antes de poder acessar de forma programática os dados de análise do Revisions do parceiro, você precisa atender aos seguintes requisitos.

## <a name="mpn-program-enrollment"></a>Registro do programa MPN

Para acessar dados de análise de parceiros de informações programaticamente, você precisa estar registrado no programa MPN e ter uma conta do Partner Center. Para saber como, consulte [criar uma conta do MPN no Partner Center](mpn-create-a-partner-center-account.md)

## <a name="create-azure-active-directory-aad-application"></a>criar aplicativo Azure Active Directory (AAD)

as credenciais de usuário regulares não podem ser usadas para acesso programático de dados de análise de Insights de parceiros. um aplicativo Azure Active Directory (AAD) precisa ser criado junto com um segredo (aplicativo + acesso de usuário) para acessar as APIs de acesso programáticos. para saber como criar um aplicativo e um segredo do AAD, consulte [início rápido: registrar um aplicativo com o plataforma de identidade da Microsoft.](/azure/active-directory/develop/quickstart-register-app)   A permissão é necessária para acessar a API de parceiro da Microsoft. Para saber como adicionar permissão, consulte [autenticação de API de parceiro-parceiro](/partner/develop/api-authentication#application-and-user-access)

## <a name="assign-executive-report-viewer-erv-role-to-the-user"></a>Atribuir função ERV (Executive Report Viewer) ao usuário

Para acessar dados de análise do parceiro insights programaticamente, você deve ter o ERV (Executive Report Viewer). para saber como atribuir a função ERV ao usuário, consulte o [partner center Insights acesso baseado em função-partner center](insights-roles.md)

## <a name="generate-an-aad-token"></a>Gerar um token do AAD

Você precisa gerar um token do AAD usando a ID do aplicativo (cliente), o segredo do cliente, sua ID de usuário e senha.   [Verifique aqui](insights-programmatic-first-api-call.md#token-generation) as etapas para gerar o token do AAD.

> [!Note]
> O token é válido por uma hora.

## <a name="next-steps"></a>Próximas etapas
[Paradigma do acesso programático](insights-programmatic-access-paradigm.md)