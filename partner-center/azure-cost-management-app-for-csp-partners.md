---
title: Azure Cost Management by Cloudyn para parceiros CSP | Partner Center
ms.topic: article
ms.date: 11/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como registrar o aplicativo Web Cloudyn e usar uma chave secreta para ele no Partner Center para que você possa usar o aplicativo para acompanhar o uso do cliente e os custos do Azure.
author: Janet
ms.author: janet
Keywords: Aplicativo de gerenciamento de custos do Azure, gerenciar custos, aplicativos Web
robots: ''
ms.localizationpriority: medium
ms.openlocfilehash: b05f2085aad63f8a0e23fa44de97550d13053f86
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253302"
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a>Aplicativo de gerenciamento de custos do Azure para parceiros CSP do Azure  

**Aplica-se a**

- Partner Center
- Parceiros do programa Provedor de Soluções na Nuvem

**Funções apropriadas**

- Administração global
- Agente administrador

[Obter mais informações sobre o gerenciamento de custos do Azure](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a>Antes de começar
Antes de usar o Azure Cost Management, certifique-se de atender aos seguintes requisitos:

- Você é um parceiro do programa Provedor de Soluções na Nuvem.
- Você pode criar um aplicativo web com a API do Partner Center.

## <a name="overview"></a>Visão geral

O Cloudyn é um aplicativo Web que permite que você acompanhe e gerencie quanto seus clientes estão usando o Azure e os custos desse uso. Você pode usá-lo por meio da API do Partner Center.

## <a name="register-your-web-app-in-the-partner-center"></a>Registre seu aplicativo Web no Partner Center
Ao registrar um aplicativo web do Azure Active Directory no Partner Center, você habilita o acesso à API do Partner Center. 
1.  Entre no [Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) usando uma [conta de administrador global ou de agente administrador](create-user-accounts-and-set-permissions.md).
2.  No **Partner Center**, selecione **configurações de conta** &gt; **[Gerenciamento de aplicativos](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)** .
3.  Na seção **Aplicativo Web**, clique em **Adicionar novo aplicativo web**.
<br> **Observação**: se você tiver criado anteriormente um aplicativo web, pode pular a etapa 3.
4.  Copie e salve o GUID da **ID do Comércio** e o GUID da **ID do Aplicativo** para seu aplicativo web. Você precisará das duas IDs para usar o versão de avaliação gratuita de 30 dias do aplicativo Azure Cost Management.

## <a name="add-a-secret-key-to-your-app"></a>Adicione uma chave secreta ao seu aplicativo
1. No menu suspenso ao lado do botão **Adicionar chave**, selecione uma duração de 1 ou 2 anos.
2. Clique em **Adicionar chave**. 
3. Copie e salve o valor da chave secreta. Você precisará disso para a versão de avaliação gratuita de 30 dias.<br>
   > [!NOTE]  
   > As chaves secretas do aplicativo são como senhas com datas de expiração mais longas. Salve o valor da chave em um local seguro para uso futuro.

## <a name="next-steps"></a>Próximas etapas
Inicie uma [avaliação gratuita de 30 dias](https://go.microsoft.com/fwlink/?linkid=857895).
Você precisa dos seguintes detalhes para iniciar a avaliação:
- Credenciais para entrar no Partner Center
- GUID da ID do Comércio
- GUID da ID do Aplicativo
- Valor da chave secreta do aplicativo
