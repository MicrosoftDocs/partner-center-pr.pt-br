---
title: Gerenciamento de Custos do Azure licenciado pela Cloudyn para CSPs
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como registrar o aplicativo Web Cloudyn e usar uma chave secreta para ele no Partner Center para que você possa usar o aplicativo para acompanhar o uso do cliente e os custos do Azure.
author: aparnagkrishnan
ms.author: aparnag
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: defa691a3bc70cbda45f01cb447d89364a49e3b8
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534974"
---
# <a name="track-customer-azure-usage-and-costs-with-the-azure-cost-management-app-for-csp-partners"></a>Acompanhe o uso e os custos do Azure para clientes com o aplicativo de gerenciamento de custos do Azure para parceiros CSP  

**Funções apropriadas**

- Administrador global
- Agente administrativo

[Obtenha mais informações sobre o Azure Cost Management](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a>Antes de começar
Antes de usar o Azure Cost Management, certifique-se de atender aos seguintes requisitos:

- Você é um parceiro do programa Provedor de Soluções na Nuvem.
- Você pode criar um aplicativo web com a API do Partner Center.

## <a name="overview"></a>Visão geral

O Cloudyn é um aplicativo Web que permite que você acompanhe e gerencie quanto seus clientes estão usando o Azure e os custos desse uso. Você pode usá-lo por meio da API do Partner Center.

## <a name="register-your-web-app-in-the-partner-center"></a>Registre seu aplicativo Web no Partner Center
Ao registrar um aplicativo web do Azure Active Directory no Partner Center, você habilita o acesso à API do Partner Center. 
1.  Entre no [Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) usando uma [conta de administrador global ou de agente administrador](create-user-accounts-and-set-permissions.md).
2.  No **Partner Center**, selecione **configurações de conta** &gt; **[Gerenciamento de aplicativos](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.
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
