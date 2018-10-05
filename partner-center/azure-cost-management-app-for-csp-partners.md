---
title: Azure Cost Management by Cloudyn para parceiros CSP | Partner Center
description: Azure Cost Management by Cloudyn requer acesso provisionado à API do Partner Center.
author: Janet
Keywords: Azure cost management app, manage costs, web apps
robots: ''
ms.localizationpriority: medium
ms.openlocfilehash: b24e69d21a50306cbd9bf3495fc55015d5966b17
ms.sourcegitcommit: 5b720c2ad126ec52564ad5264596ca1cf6a12489
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/05/2018
ms.locfileid: "4377798"
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a>Aplicativo de gerenciamento de custos do Azure para parceiros CSP do Azure  

**Aplicável a**

-  Partner Center

[Obtenha mais informações sobre o Azure Cost Management](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a>Antes de começar
Antes de usar o Azure Cost Management, certifique-se de atender aos seguintes requisitos:

- Você é um parceiro do programa Provedor de Soluções na Nuvem.
- Você pode criar um aplicativo web com a API do Partner Center.

## <a name="overview"></a>Visão geral

Azure Cost Management by Cloudyn é um aplicativo web que permite controlar e gerenciar o quanto os clientes estão usando o Azure e os custos desse uso. Você pode usá-lo por meio da API do Partner Center.

## <a name="register-your-web-app-in-the-partner-center"></a>Registre seu aplicativo Web no Partner Center
Ao registrar um aplicativo Web do Azure Active Directory no Partner Center, você habilita o acesso à API do Partner Center. 
1.  Entre no [Partner Center](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview) usando uma [conta de administrador global ou de agente administrador](create-user-accounts-and-set-permissions.md).
2.  No menu **Painel**, selecione **Configurações da conta** &gt; **[Gerenciamento de aplicativos](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)**.
3.  Na seção **Aplicativo Web**, clique em **Adicionar novo aplicativo web**.
<br> **Observação**: se você tiver criado anteriormente um aplicativo web, pode pular a etapa 3.
4.  Copie e salve o GUID da **ID do Comércio** e o GUID da **ID do Aplicativo** para seu aplicativo web. Você precisará das duas IDs para usar o versão de avaliação gratuita de 30 dias do aplicativo Azure Cost Management.

## <a name="add-a-secret-key-to-your-app"></a>Adicione uma chave secreta ao seu aplicativo
1.  No menu suspenso ao lado do botão **Adicionar chave**, selecione uma duração de 1 ou 2 anos.
2.  Clique em **Adicionar chave**. 
3.  Copie e salve o valor da chave secreta. Você precisará disso para a versão de avaliação gratuita de 30 dias.<br>
> [!NOTE]  
> As chaves secretas do aplicativo são como senhas com datas de vencimento mais. Salve o valor da chave em um local seguro para uso futuro.

## <a name="next-steps"></a>Próximas etapas
Inicie uma [avaliação gratuita de 30 dias](https://go.microsoft.com/fwlink/?linkid=857895).
Você precisa dos seguintes detalhes para iniciar a avaliação:
- Credenciais para entrar no Partner Center
- GUID da ID do Comércio
- GUID da ID do Aplicativo
- Valor da chave secreta do aplicativo
