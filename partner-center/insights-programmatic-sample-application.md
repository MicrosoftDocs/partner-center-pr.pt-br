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
# <a name="sample-application"></a>Aplicativo de exemplo

Os aplicativos de exemplo são criados em linguagens C# e JAVA e estão disponíveis [GitHub](https://github.com/partneranalytics)

- [Aplicativo de exemplo C#](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN)
- [Aplicativo de exemplo JAVA](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)

Você pode optar por se inspirar no aplicativo de exemplo e criar seu próprio aplicativo em qualquer idioma.

O aplicativo de exemplo atinge os seguintes objetivos:

- Gera um token Azure Active Directory (Azure AD).
- Obtém conjuntos de dados disponíveis.
- Cria consultas definidas pelo usuário.
- Obtém as consultas definidas pelo usuário e pelo sistema.
- Agenda um relatório.

O aplicativo de exemplo não abrange o método de chamada de APIs para outras funcionalidades. No entanto, o processo de chamar outras APIs permanece o mesmo descrito acima.

## <a name="how-to-run-the-application"></a>Como executar o aplicativo

- Clone o repositório em um sistema local usando este comando:

```cli
git clone https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN.git
```

> [!Note]
> Para obter mais instruções, consulte o arquivo ProgrammaticExportSampleAppMPN/README.md no repositório GitHub [.](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)

- Para executar rapidamente o aplicativo, atualize a ID do cliente e o segredo do cliente **noappsettings.Development.jsem**

:::image type="content" source="images/insights/prog-acc-appsetting-development.png" alt-text="Ilustrando appsetting development json":::

A execução do aplicativo iniciará um servidor Web local e uma página será aberta (`https://localhost:44365/ProgrammaticExportSampleApp/sample`).
  
:::image type="content" source="images/insights/prog-acc-sample-application.png" alt-text="Ilustrando a interface do usuário do aplicativo de exemplo":::

Esta página fará chamadas de API para o servidor Web em execução no computador local, o que, por sua vez, fará as chamadas de API de acesso programático real.

## <a name="code-snippets"></a>Snippets de código

A estrutura básica do código C# para fazer as chamadas de API de acesso programático é a seguinte:
 
:::image type="content" source="images/insights/prog-acc-code-snippet.png" alt-text="Ilustrando o snippet de código":::

## <a name="next-steps"></a>Próximas etapas

[APIs para acessar dados de análise do Partner Insights](insights-programmatic-analytics-available-api.md)
