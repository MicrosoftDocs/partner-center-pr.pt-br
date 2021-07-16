---
title: Aplicativo de exemplo
ms.topic: article
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Use o aplicativo de exemplo para criar seu próprio aplicativo para acessar programaticamente os dados do Partner Insights.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.openlocfilehash: 6f334b9047c38e8b7763a4ba96d21d987c252682
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114374782"
---
# <a name="sample-application"></a><span data-ttu-id="ed989-103">Aplicativo de exemplo</span><span class="sxs-lookup"><span data-stu-id="ed989-103">Sample Application</span></span>

<span data-ttu-id="ed989-104">Os aplicativos de exemplo são criados em linguagens C# e JAVA e estão disponíveis [GitHub](https://github.com/partneranalytics)</span><span class="sxs-lookup"><span data-stu-id="ed989-104">Sample applications are created in C# and JAVA languages and are available on [GitHub](https://github.com/partneranalytics)</span></span>

- [<span data-ttu-id="ed989-105">Aplicativo de exemplo C#</span><span class="sxs-lookup"><span data-stu-id="ed989-105">C# Sample Application</span></span>](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN)
- [<span data-ttu-id="ed989-106">Aplicativo de exemplo JAVA</span><span class="sxs-lookup"><span data-stu-id="ed989-106">JAVA Sample Application</span></span>](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)

<span data-ttu-id="ed989-107">Você pode optar por se inspirar no aplicativo de exemplo e criar seu próprio aplicativo em qualquer idioma.</span><span class="sxs-lookup"><span data-stu-id="ed989-107">You can choose to take inspiration from the sample application and build your own application in any language.</span></span>

<span data-ttu-id="ed989-108">O aplicativo de exemplo atinge os seguintes objetivos:</span><span class="sxs-lookup"><span data-stu-id="ed989-108">The sample application achieves the following objectives:</span></span>

- <span data-ttu-id="ed989-109">Gera um token Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="ed989-109">Generates an Azure Active Directory (Azure AD) Token.</span></span>
- <span data-ttu-id="ed989-110">Obtém conjuntos de dados disponíveis.</span><span class="sxs-lookup"><span data-stu-id="ed989-110">Gets available datasets.</span></span>
- <span data-ttu-id="ed989-111">Cria consultas definidas pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="ed989-111">Creates user defined queries.</span></span>
- <span data-ttu-id="ed989-112">Obtém as consultas definidas pelo usuário e pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="ed989-112">Gets user defined and system queries.</span></span>
- <span data-ttu-id="ed989-113">Agenda um relatório.</span><span class="sxs-lookup"><span data-stu-id="ed989-113">Schedules a report.</span></span>

<span data-ttu-id="ed989-114">O aplicativo de exemplo não abrange o método de chamada de APIs para outras funcionalidades.</span><span class="sxs-lookup"><span data-stu-id="ed989-114">The sample application doesn't cover the method of calling APIs for other functionalities.</span></span> <span data-ttu-id="ed989-115">No entanto, o processo de chamar outras APIs permanece o mesmo descrito acima.</span><span class="sxs-lookup"><span data-stu-id="ed989-115">However, the process of calling other APIs remains the same as outlined above.</span></span>

## <a name="how-to-run-the-application"></a><span data-ttu-id="ed989-116">Como executar o aplicativo</span><span class="sxs-lookup"><span data-stu-id="ed989-116">How to run the application</span></span>

- <span data-ttu-id="ed989-117">Clone o repositório em um sistema local usando este comando:</span><span class="sxs-lookup"><span data-stu-id="ed989-117">Clone the repository to a local system using this command:</span></span>

```cli
git clone https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN.git
```

> [!Note]
> <span data-ttu-id="ed989-118">Para obter mais instruções, consulte o arquivo ProgrammaticExportSampleAppMPN/README.md no repositório GitHub [.](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)</span><span class="sxs-lookup"><span data-stu-id="ed989-118">For more instructions, refer to the ProgrammaticExportSampleAppMPN/README.md file in the GitHub [repository](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java).</span></span>

- <span data-ttu-id="ed989-119">Para executar rapidamente o aplicativo, atualize a ID do cliente e o segredo do cliente **noappsettings.Development.jsem**</span><span class="sxs-lookup"><span data-stu-id="ed989-119">To quickly run the app, update the client id and client secret in the **appsettings.Development.json**</span></span>

:::image type="content" source="images/insights/prog-acc-appsetting-development.png" alt-text="Ilustrando appsetting development json":::

<span data-ttu-id="ed989-121">A execução do aplicativo iniciará um servidor Web local e uma página será aberta (`https://localhost:44365/ProgrammaticExportSampleApp/sample`).</span><span class="sxs-lookup"><span data-stu-id="ed989-121">Running the app will start a local web server and a page will open (`https://localhost:44365/ProgrammaticExportSampleApp/sample`).</span></span>
  
:::image type="content" source="images/insights/prog-acc-sample-application.png" alt-text="Ilustrando a interface do usuário do aplicativo de exemplo":::

<span data-ttu-id="ed989-123">Esta página fará chamadas de API para o servidor Web em execução no computador local, o que, por sua vez, fará as chamadas de API de acesso programático real.</span><span class="sxs-lookup"><span data-stu-id="ed989-123">This page will make API calls to the webserver running on the local machine, which in turn will make the actual programmatic access API calls.</span></span>

## <a name="code-snippets"></a><span data-ttu-id="ed989-124">Snippets de código</span><span class="sxs-lookup"><span data-stu-id="ed989-124">Code Snippets</span></span>

<span data-ttu-id="ed989-125">A estrutura básica do código C# para fazer as chamadas de API de acesso programático é a seguinte:</span><span class="sxs-lookup"><span data-stu-id="ed989-125">The basic structure of the C# code for doing the programmatic access API calls is as follows:</span></span>
 
:::image type="content" source="images/insights/prog-acc-code-snippet.png" alt-text="Ilustrando o snippet de código":::

## <a name="next-steps"></a><span data-ttu-id="ed989-127">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="ed989-127">Next steps</span></span>

[<span data-ttu-id="ed989-128">APIs para acessar dados de análise do Partner Insights</span><span class="sxs-lookup"><span data-stu-id="ed989-128">APIs for accessing partner insights analytics data</span></span>](insights-programmatic-analytics-available-api.md)
