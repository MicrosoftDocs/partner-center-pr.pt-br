---
title: Instalar a análise do Partner Center para Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Siga as etapas neste artigo para instalar e visualizar o aplicativo de análise do Partner Center para Power BI (para parceiros diretos no CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e8a8558bad11f641737507f4d76405e9825df516
ms.sourcegitcommit: 2a980b50cf177753c15ebfd7770e14cf6d486cf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2020
ms.locfileid: "83795868"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Instale e visualize o aplicativo de análise do Partner Center para Microsoft Power BI

**Aplica-se a**

- Partner Center

**Funções apropriadas**
-   Administrador global
-   Administrador de usuários
-   Agente de vendas
-   Agente administrativo

## <a name="before-you-begin"></a>Antes de começar

Selecione o aplicativo que é mais relevante para seu negócio na seguinte lista de aplicativos de Power BI disponíveis:
- [Parceiro direto](https://app.powerbi.com/groups/me/getdata/services/direct-providers-partner-analytics)

- [Parceiro indireto](https://app.powerbi.com/groups/me/getdata/services/indirect-providers-partner-analytics)

- [Revendedor indireto](https://app.powerbi.com/groups/me/getdata/services/indirect-seller-partner-analytics)

Antes de instalar a versão de visualização do aplicativo análises do Partner Center, certifique-se de que você atende aos seguintes requisitos.

- Você escolhe o aplicativo de Power BI correto para sua empresa.

- Você tem uma assinatura ativa Microsoft Power BI Professional ou Microsoft Power BI Premium.

- Você pode se conectar no Power BI.

- Você pode entrar como um administrador global, agente de administração ou administrador de cobrança para [o locatário do Azure Active Directory (Azure AD) da sua empresa](azure-active-directory-tenants-and-partner-center.md).

## <a name="to-install-the-app"></a>Para instalar o aplicativo

1. Inicie o [processo de instalação](https://app.powerbi.com/getdata/services/partneranalytics?cpcode=PartnerCenterAnalytics&getDataForceConnect=true&alwaysPromptForContentProviderCreds=true).

2. Em **Já tem uma conta?**, selecione **Conecte-se**. 

3. Na próxima página, digite seu nome de usuário e senha do Partner Power BI e, em seguida, selecione **Conecte-se**. 

4. Na janela pop-up **conectar ao Partner Center Analytics** , verifique se o **método de autenticação** está definido como **oAuth2** ou selecione **oAuth2** na lista, se não for. 

> [!NOTE]  
>  Esta janela pode demorar alguns minutos para aparecer.

5. Na página **conector de análise do Partner Center** , entre com administrador global, agente de administração ou credenciais de administrador de cobrança para o locatário do Azure ad da sua empresa e selecione **entrar**.
 
6. Quando solicitado para acesso, selecione **Aceitar**. 

Depois que o serviço de análise do Partner Center estiver conectado com o Power BI, os dados começam a ser carregados. Dependendo da quantidade de dados, isso pode levar até 10 minutos. 

Depois que carregamento de dados é concluído, você pode começar a usar o painel do aplicativo de análise do Partner Center e os relatórios no Power BI.

## <a name="next-steps"></a>Próximas etapas

[Visualize seus dados de negócio com o aplicativo de análise do Partner Center para Microsoft Power BI](power-bi-app-for-direct-partners-use.md)
