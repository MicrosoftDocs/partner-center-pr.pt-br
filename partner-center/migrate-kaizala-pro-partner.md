---
title: Migrar assinaturas do Kaizala Pro para o Microsoft 365
description: Saiba como migrar assinaturas do Kaizala pro para as versões Microsoft 365 ou Office 365. Leia este artigo para obter mais detalhes sobre a transição de seus clientes.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 583e9c40bb8d161c30440f12331dc8dcbf3db417
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146418"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft-365-or-office-365-versions"></a>Migrar assinaturas autônomas do Kaizala pro para as versões Microsoft 365 ou Office 365

**Funções apropriadas**: agente de vendas

A partir de 1º de julho de 2020, a Microsoft está terminando as vendas do serviço autônomo do Kaizala pro. Os clientes não poderão mais comprar novas assinaturas do Kaizala pro após essa data, e as assinaturas existentes do Kaizala pro não serão renovadas automaticamente quando expirarem.

Para garantir a continuidade dos clientes, você deve fazer a transição de clientes com assinaturas do Kaizala pro standalone expiradas para uma opção de SKU com suporte, listada abaixo. É recomendável mover os clientes para novas assinaturas antes da data de término anual da assinatura para evitar qualquer interrupção de serviço para os clientes.

Se você usar a API (CREST ou o Partner Center), poderá descobrir assinaturas expirando avaliando a data de término da assinatura junto com a propriedade de renovação automática definida como false: `auto renew = False` .

As assinaturas do E4 serão definidas `auto renew=False` em 1º de julho de 2020. Você pode mover os clientes para um novo plano a qualquer momento.

## <a name="kaizala-pro-standalone-replacement-plans"></a>Planos de substituição autônomos do Kaizala pro

Com os novos planos, os clientes podem aproveitar os recursos e as funcionalidades mais recentes no Microsoft 365. Detalhes de preço são encontrados na lista de preços e oferecem a matriz de lista no Partner Center.

- [**Microsoft 365 para negócios**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), incluindo:  
   - Microsoft 365 Business Basic
   - Microsoft 365 Business Standard
   - Microsoft 365 Business Premium
    
- [**Microsoft 365 para frente**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), incluindo:
   - Microsoft 365 F3 (antigo Microsoft 365 F1) e Office 365 F3
    
- [**Microsoft 365 para empresas**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), incluindo: 
   - Office 365 E1
   - Microsoft 365 E3 e Office 365 E3
   - Microsoft 365 E5 e Office 365 E5

- [**Microsoft 365 para educação**](https://www.microsoft.com/education/buy-license/microsoft365), incluindo: 
    - Microsoft 365 A1 e Office 365 A1
    - Microsoft 365 A3 e Office 365 A3
    - Microsoft 365 A5 e Office 365 A5

## <a name="transition-customers-to-new-product-plans"></a>Transição dos clientes para novos planos do produto

A Microsoft oferece continuamente novos produtos e serviços para nossos parceiros. Nesses casos, você pode precisar fazer o upgrade dos clientes para novos serviços ou migrar as assinaturas de SKUs que serão encerradas em breve. A migração dos clientes de SKUs desativadas para as mais recentes requer as seguintes etapas:

a. Comprar a nova assinatura

B. Reatribuir as licenças de usuário atuais

C. Cancelar a assinatura antiga


## <a name="migrate-your-customers-to-new-plans"></a>Migrar seus clientes para novos planos

### <a name="a-purchase-the-new-subscription"></a>a. Comprar a nova assinatura

1. Para comprar a nova assinatura, no menu do **Partner Center** , selecione **clientes**, selecione o cliente que você deseja mover e, em seguida, selecione **adicionar assinaturas**.

2. Selecione a assinatura que deseja comprar no catálogo (nesse caso, uma das opções acima), insira o número de licenças e selecione **Enviar**.

Agora, o cliente deve ter assinaturas antigas e novas, a antiga assinatura autônoma do Kaizala pro e a nova assinatura de "destino", por exemplo, a opção 1-Office 365 Enterprise F1.

### <a name="b-reassign-current-user-licenses"></a>B. Reatribuir as licenças de usuário atuais

1. Para reatribuir as licenças dos usuários do cliente, no menu **Partner Center,** selecione Clientes **,** selecione o cliente que você está movendo e, em seguida, selecione Usuários **e licenças**. A página Usuários e Licenças do cliente é aberta.

2. Para reatribuir a licença de usuário, selecione o usuário para reatribuir e, em **seguida, selecione Gerenciar licenças**.

3. Na página **Gerenciar licenças, des** marque a caixa de seleção Licenças autônomas do Kaizala Pro e selecione um novo plano de serviço para a assinatura para a quais o cliente está mudando.

4.  Selecione **Enviar**. Uma página de confirmação lista as novas atribuições de licença. Continue esse mesmo processo para outros usuários que precisam de atribuições de licença.

### <a name="c-cancel-old-subscription"></a>C. Cancelar a assinatura antiga

Depois de migrar a licença do usuário para o novo serviço, você pode cancelar com segurança a assinatura desativada no nível do cliente.

1.  No menu **Partner Center,** selecione **Clientes**. Selecione o cliente cuja assinatura você está cancelando.

2.  Na página de detalhe da assinatura, defina o status da assinatura como **Suspensa**.

3.  Selecione **Enviar**.

A assinatura antiga será suspensa e a nova assinatura será ativada. A assinatura suspensa será desprovisionada automaticamente após 120 dias. O cliente não pagará custos adicionais pela assinatura antiga.
