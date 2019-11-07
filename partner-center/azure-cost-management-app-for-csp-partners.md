---
title: Azure Cost Management by Cloudyn para parceiros CSP | Partner Center
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure Cost Management by Cloudyn requer acesso provisionado à API do Partner Center.
author: Janet
ms.author: janet
Keywords: Aplicativo de gerenciamento de custos do Azure, gerenciar custos, aplicativos Web
robots: ''
ms.localizationpriority: medium
ms.openlocfilehash: a746522d3470a8b97b845ed723fae87455e33e5e
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "73653864"
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a>Aplicativo de gerenciamento de custos do Azure para parceiros CSP do Azure  

**Aplica-se a**

-  Partner Center

[Obter mais informações sobre o gerenciamento de custos do Azure](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a>Antes de começar
Antes de usar o Azure Cost Management, certifique-se de atender aos seguintes requisitos:

- Você é um parceiro do programa Provedor de Soluções na Nuvem.
- Você pode criar um aplicativo web com a API do Partner Center.

## <a name="overview"></a>Visão geral

O Cloudyn é um aplicativo Web que permite que você acompanhe e gerencie quanto seus clientes estão usando o Azure e os custos desse uso. Você pode usá-lo por meio da API do Partner Center.

## <a name="register-your-web-app-in-the-partner-center"></a>Registre seu aplicativo Web no Partner Center
Ao registrar um aplicativo Web do Azure Active Directory no Partner Center, você habilita o acesso à API do Partner Center. 
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
