---
title: Instalar a análise do Partner Center para Power BI
ms.topic: article
ms.date: 07/10/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Siga as etapas neste artigo para instalar e visualizar o aplicativo de análise do Partner Center para Power BI (para parceiros diretos no CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ad0c2f3ee7d130c49dea6ba354e6794e29fd9e9f
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633685"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Instale e visualize o aplicativo de análise do Partner Center para Microsoft Power BI


**Funções apropriadas**

- Administrador global
- Administrador de gerenciamento de usuário
- Agente de vendas
- Agente administrativo

## <a name="before-you-begin"></a>Antes de começar

Selecione o aplicativo que é mais relevante para seu negócio na seguinte lista de aplicativos de Power BI disponíveis:

- [Provedor direto](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [Provedor indireto](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [Revendedor indireto](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

Antes de instalar a versão de visualização do aplicativo análises do Partner Center, certifique-se de que você atende aos seguintes requisitos.

- Você escolhe o aplicativo de Power BI correto para sua empresa.

- Você tem uma licença Power BI pro.

- Você tem permissões para instalar aplicativos de modelo em seu locatário.

- Você pode se conectar no Power BI.

- Você pode entrar como um administrador global, agente de administração ou administrador de cobrança para [o locatário do Azure Active Directory (Azure AD) da sua empresa](azure-active-directory-tenants-and-partner-center.md).

## <a name="to-install-the-app"></a>Para instalar o aplicativo

1. Selecione o link de origem do aplicativo fornecido (provedor direto/provedor indireto/revendedor indireto) na seção acima.

2. Selecione **OBTENHA AGORA**. 

3. Concorde com os termos e condições selecionando **continuar**.

4. Em Já tem uma conta?, selecione **Conecte-se**.

5. Na próxima página, digite seu nome de usuário e senha do Partner Power BI e, em seguida, selecione **Conecte-se**.

6. Instale o espaço de trabalho fornecendo o nome do espaço de trabalho.

7. Você pode encontrar os aplicativos de modelo instalados na seção aplicativos.

8. Selecione **aplicativos** e escolha os aplicativos instalados.

9. Introdução à nova tela do aplicativo é aberta.

10. Para se conectar aos dados, selecione **conectar**.

11. Na janela pop-up **conectar ao Partner Center Analytics** , verifique se o **método de autenticação** está definido como **oAuth2** ou selecione **oAuth2** na lista, se não for. 

> [!NOTE]  
>  Esta janela pode demorar alguns minutos para aparecer.

12. Na página **conector de análise do Partner Center** , entre com administrador global, agente de administração ou credenciais de administrador de cobrança para o locatário do Azure ad da sua empresa e selecione **entrar**.
 
13. Quando solicitado para acesso, selecione **Aceitar**. 

Depois que o serviço de análise do Partner Center estiver conectado com o Power BI, os dados começam a ser carregados. Dependendo da quantidade de dados, isso pode levar até 10 minutos. 

Depois que carregamento de dados é concluído, você pode começar a usar o painel do aplicativo de análise do Partner Center e os relatórios no Power BI.

## <a name="next-steps"></a>Próximas etapas

[Visualize seus dados de negócio com o aplicativo de análise do Partner Center para Microsoft Power BI](power-bi-app-for-direct-partners-use.md)
