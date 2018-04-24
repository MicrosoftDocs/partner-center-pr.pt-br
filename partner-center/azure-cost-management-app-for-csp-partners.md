---
title: Azure Cost Management by Cloudyn para parceiros CSP | Partner Center
description: Azure Cost Management by Cloudyn requer acesso provisionado à API do Partner Center.
author: Janet
Keywords: Azure cost management app, manage costs, web apps
robots: ''
ms.openlocfilehash: 01553b850d5839d721de5406c3f1c63094f76bd6
ms.sourcegitcommit: 32f34476cbcae58651baab15d3f5591d6ef70d27
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2018
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a>Aplicativo de gerenciamento de custos do Azure para parceiros CSP do Azure  

**Aplicável a**

-  Partner Center

[Obtenha mais informações sobre o Azure Cost Management](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a>Antes de começar
Antes de usar o Azure Cost Management, certifique-se de atender aos seguintes requisitos:
- Você é um parceiro do programa Provedor de Soluções na Nuvem.
- Você pode criar um aplicativo Web com a API do Painel de Parceiros.

## <a name="overview"></a>Visão geral

Azure Cost Management by Cloudyn é um aplicativo web que permite controlar e gerenciar o quanto os clientes estão usando o Azure e os custos desse uso. Você pode usá-lo por meio da API do Painel de Parceiros.

## <a name="register-your-web-app-in-the-partner-dashboard"></a>Registre seu aplicativo Web no Painel de Parceiros
Ao registrar um aplicativo Web do Azure Active Directory no Painel de Parceiros, você habilita o acesso à API do Painel de Parceiros. 
1.  Entre no [Painel de Parceiros](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview) usando uma [conta de administrador global ou de agente administrador](create-user-accounts-and-set-permissions.md).
2.  No menu **Painel**, selecione **Configurações da conta** &gt; **[Gerenciamento de aplicativos](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)**.
3.  Na seção **Aplicativo Web**, clique em **Adicionar novo aplicativo web**.
<br> **Observação**: se você tiver criado anteriormente um aplicativo web, pode pular a etapa 3.
4.  Copie e salve o GUID da **ID do Comércio** e o GUID da **ID do Aplicativo** para seu aplicativo web. Você precisará das duas IDs para usar o versão de avaliação gratuita de 30 dias do aplicativo Azure Cost Management.

## <a name="add-a-secret-key-to-your-app"></a>Adicione uma chave secreta ao seu aplicativo
1.  No menu suspenso ao lado do botão **Adicionar chave**, selecione uma duração de 1 ou 2 anos.
2.  Clique em **Adicionar chave**. 
3.  Copie e salve o valor da chave secreta. Você precisará disso para a versão de avaliação gratuita de 30 dias.
<br>**Observação**: as chaves secretas do aplicativo são como senhas com datas de vencimento mais longas. Salve o valor da chave em um local seguro para uso futuro.

## <a name="next-steps"></a>Próximas etapas
Inicie uma [avaliação gratuita de 30 dias](https://go.microsoft.com/fwlink/?linkid=857895).
Você precisa dos seguintes detalhes para iniciar a avaliação:
- Credenciais para entrar no Painel de Parceiros
- GUID da ID do Comércio
- GUID da ID do Aplicativo
- Valor da chave secreta do aplicativo
