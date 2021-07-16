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
# <a name="prerequisites-to-programmatically-access-analytics-data"></a><span data-ttu-id="f256a-103">Pré-requisitos para acessar dados de análise programaticamente</span><span class="sxs-lookup"><span data-stu-id="f256a-103">Prerequisites to programmatically access analytics data</span></span>

<span data-ttu-id="f256a-104">**Funções apropriadas:** Administrador global | Administrador do MPN</span><span class="sxs-lookup"><span data-stu-id="f256a-104">**Appropriate roles:** Global admin | MPN admin</span></span>

<span data-ttu-id="f256a-105">Antes de poder acessar de forma programática os dados de análise do Revisions do parceiro, você precisa atender aos seguintes requisitos.</span><span class="sxs-lookup"><span data-stu-id="f256a-105">Before you can programmatically access partner insights analytics data, you need to meet the following requirements.</span></span>

## <a name="mpn-program-enrollment"></a><span data-ttu-id="f256a-106">Registro do programa MPN</span><span class="sxs-lookup"><span data-stu-id="f256a-106">MPN Program enrollment</span></span>

<span data-ttu-id="f256a-107">Para acessar dados de análise de parceiros de informações programaticamente, você precisa estar registrado no programa MPN e ter uma conta do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="f256a-107">To access partner insights analytics data programmatically, you need to be enrolled in the MPN program and have a Partner Center account.</span></span> <span data-ttu-id="f256a-108">Para saber como, consulte [criar uma conta do MPN no Partner Center](mpn-create-a-partner-center-account.md)</span><span class="sxs-lookup"><span data-stu-id="f256a-108">To learn how, see [Create an MPN account in Partner Center](mpn-create-a-partner-center-account.md)</span></span>

## <a name="create-azure-active-directory-aad-application"></a><span data-ttu-id="f256a-109">criar aplicativo Azure Active Directory (AAD)</span><span class="sxs-lookup"><span data-stu-id="f256a-109">Create Azure Active Directory (AAD) application</span></span>

<span data-ttu-id="f256a-110">as credenciais de usuário regulares não podem ser usadas para acesso programático de dados de análise de Insights de parceiros.</span><span class="sxs-lookup"><span data-stu-id="f256a-110">Regular user credentials cannot be used for programmatic access of Partner Insights Analytics data.</span></span> <span data-ttu-id="f256a-111">um aplicativo Azure Active Directory (AAD) precisa ser criado junto com um segredo (aplicativo + acesso de usuário) para acessar as APIs de acesso programáticos.</span><span class="sxs-lookup"><span data-stu-id="f256a-111">An Azure Active Directory (AAD) application needs to be created along with a secret (application + user access) to access the programmatic access APIs.</span></span> <span data-ttu-id="f256a-112">para saber como criar um aplicativo e um segredo do AAD, consulte [início rápido: registrar um aplicativo com o plataforma de identidade da Microsoft.](/azure/active-directory/develop/quickstart-register-app)   A permissão é necessária para acessar a API de parceiro da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f256a-112">To learn how to create an AAD application and secret, see [Quickstart: Register an application with the Microsoft identity platform.](/azure/active-directory/develop/quickstart-register-app) Permission is required to access Microsoft Partner API.</span></span> <span data-ttu-id="f256a-113">Para saber como adicionar permissão, consulte [autenticação de API de parceiro-parceiro](/partner/develop/api-authentication#application-and-user-access)</span><span class="sxs-lookup"><span data-stu-id="f256a-113">To learn how to add permission, see [Partner API authentication - Partner](/partner/develop/api-authentication#application-and-user-access)</span></span>

## <a name="assign-executive-report-viewer-erv-role-to-the-user"></a><span data-ttu-id="f256a-114">Atribuir função ERV (Executive Report Viewer) ao usuário</span><span class="sxs-lookup"><span data-stu-id="f256a-114">Assign Executive Report Viewer (ERV) role to the user</span></span>

<span data-ttu-id="f256a-115">Para acessar dados de análise do parceiro insights programaticamente, você deve ter o ERV (Executive Report Viewer).</span><span class="sxs-lookup"><span data-stu-id="f256a-115">To access partner insights analytics data programmatically, you should have Executive Report Viewer (ERV).</span></span> <span data-ttu-id="f256a-116">para saber como atribuir a função ERV ao usuário, consulte o [partner center Insights acesso baseado em função-partner center](insights-roles.md)</span><span class="sxs-lookup"><span data-stu-id="f256a-116">To learn how to assign ERV role to the user, see [Partner Center Insights role-based access - Partner Center](insights-roles.md)</span></span>

## <a name="generate-an-aad-token"></a><span data-ttu-id="f256a-117">Gerar um token do AAD</span><span class="sxs-lookup"><span data-stu-id="f256a-117">Generate an AAD token</span></span>

<span data-ttu-id="f256a-118">Você precisa gerar um token do AAD usando a ID do aplicativo (cliente), o segredo do cliente, sua ID de usuário e senha.   [Verifique aqui](insights-programmatic-first-api-call.md#token-generation) as etapas para gerar o token do AAD.</span><span class="sxs-lookup"><span data-stu-id="f256a-118">You need to Generate an AAD token using the Application (client) ID, client secret, your user ID and password.  [Check here](insights-programmatic-first-api-call.md#token-generation) for steps to generate AAD token.</span></span>

> [!Note]
> <span data-ttu-id="f256a-119">O token é válido por uma hora.</span><span class="sxs-lookup"><span data-stu-id="f256a-119">The token is valid for one hour.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f256a-120">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="f256a-120">Next steps</span></span>
[<span data-ttu-id="f256a-121">Paradigma do acesso programático</span><span class="sxs-lookup"><span data-stu-id="f256a-121">Programmatic access paradigm</span></span>](insights-programmatic-access-paradigm.md)