---
title: Migrar do Dynamics 365 e plano de envolvimento de cliente de Basic (ofertas qualificadas) para versões mais recentes | Partner Center
ms.topic: article
ms.date: 12/12/2018
description: Dynamics 365 for Sales / plano de envolvimento de cliente de assinaturas Basic (oferece qualificado) não pode ser renovada.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: labrenne
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 offers, renew offers, new Dynamics 365 SKUs
ms.openlocfilehash: b4b25dd80a684c9060b28461a9e6f594651ae224
ms.sourcegitcommit: 23adf424dd43ed0281473f97d535d73c59c92b01
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/13/2018
ms.locfileid: "8968266"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>Migrar do Dynamics 365 e plano de envolvimento de cliente de Basic (ofertas qualificadas) para versões mais recentes

**Aplica-se ao**

-  Partner Center

Clientes de 1º de janeiro de 2019, eficazes com Dynamics 365 for Sales / plano de envolvimento de cliente de assinaturas Basic (oferece qualificado) não pode renovar essas ofertas herdadas; as assinaturas existentes não serão renovadas automaticamente quando expirarem. Na página de detalhes da assinatura, o status da assinatura será alterado para "Expira em [Data]" de "Renovação automática em [Data]". 


Para garantir a continuidade dos clientes, você deve fazer a transição aqueles com assinaturas E4 vencidas para uma opção com suporte, listada abaixo. É recomendável mover os clientes para as novas assinaturas antes da data de término da assinatura anual, para evitar possíveis interrupções de serviço.

Se você usar a API (CREST ou Partner Center), você pode encontrar assinaturas vencidas avaliando a data de término da assinatura juntamente com automática = falsa propriedade. As assinaturas em questão serão definidas como automático renovar = falso em 1º de janeiro de 2019. Você pode mover os clientes para um novo plano a qualquer momento. 

### <a name="the-dynamics-365-offers-being-retired"></a>O Dynamics 365 oferece sendo desativado

- Dynamics 365 para venda Enterprise Edition CRMOL Basic (oferta qualificada)
- Dynamics 365 para venda Enterprise Edition CRMOL Basic (oferta qualificada) para professores
- Dynamics 365 para venda Enterprise Edition CRMOL Basic (oferta qualificada) para estudantes
- Dynamics 365 para venda Enterprise Edition (preço do governo dos Estados Unidos) CRMOL Basic (oferta qualificada)
- Dynamics 365 para a edição Enterprise vendas do SA para CRM Basic (oferta qualificada)
- Dynamics 365 para a edição Enterprise vendas do SA para CRM Basic (oferta qualificada) para professores
- Dynamics 365 para a edição Enterprise vendas do SA para CRM Basic (oferta qualificada) para estudantes
- Dynamics 365 para venda Enterprise Edition (preço do governo dos Estados Unidos) do SA para CRM Basic (oferta qualificada)
- Dynamics 365 para venda Enterprise Edition complemento para o CRM Basic (oferta qualificada)
- Dynamics 365 para venda Enterprise Edition complemento para o CRM Basic (oferta qualificada) para professores
- Dynamics 365 para venda Enterprise Edition complemento para o CRM Basic (oferta qualificada) para estudantes
- Dynamics 365 para venda Enterprise Edition (preço do governo dos Estados Unidos) complemento para o CRM Basic (oferta qualificada)
- Dynamics 365 Customer envolvimento plano Enterprise Edition CRMOL Basic (oferta qualificada)
- Dynamics 365 Customer envolvimento plano Enterprise Edition (preço do governo dos Estados Unidos) CRMOL Basic (oferta qualificada)
- Dynamics 365 cliente envolvimento plano Enterprise Edition CRMOL Basic (oferta qualificada) para estudantes
- Dynamics 365 Customer envolvimento plano Enterprise Edition CRMOL Basic (oferta qualificada) para professores
- Dynamics 365 Customer envolvimento plano Enterprise Edition do SA para CRM Basic (oferta qualificada)
- Dynamics 365 Customer envolvimento plano edição Enterprise (preço do governo dos Estados Unidos) do SA para CRM Basic (oferta qualificada)
- Dynamics 365 Customer envolvimento plano Enterprise Edition do SA para CRM Basic (oferta qualificada) para estudantes
- Envolvimento do cliente de Dynamics 365 plano edição Enterprise do SA para CRM Basic (oferta qualificada) para professores
- Dynamics 365 cliente envolvimento plano Enterprise Edition complemento para CRM Basic (oferta qualificada)
- Dynamics 365 cliente envolvimento plano Enterprise Edition (preço do governo dos Estados Unidos) complemento para CRM Basic (oferta qualificada)
- Dynamics 365 cliente envolvimento plano Enterprise Edition complemento para CRM Basic (oferta qualificada) para estudantes
- Dynamics 365 Customer envolvimento plano Enterprise Edition complemento para CRM Basic (oferta qualificada) para professores



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>Dynamics 365 for Sales / planos de plano de envolvimento de cliente de substituição Basic (oferece qualificado)

**Ofertas desativadas**   

- Dynamics 365 para vendas do CRM Basic ou CRMOL Basic (oferta qualificada)
- Dynamics 365 Customer Engagement Plan do CRM Basic ou CRMOL Basic (oferta qualificada)

**Opções de substituição**
- Dynamics 365 para venda Professional (novo)
- Dynamics 365 para venda Professional (novo)
- Dynamics 365 for Customer Service
- Dynamics 365 Customer Engagement Plan ou
- Membros da equipe do Dynamics 365



## <a name="transition-customers-to-new-product-plans"></a>Transição dos clientes para novos planos do produto

Mover os clientes de SKUs desativadas para as mais recentes requer as etapas a seguir nesta ordem:

- Comprar a nova assinatura
- Reatribuir as licenças de usuário atuais
- Cancelar a assinatura antiga

## <a name="purchase-the-new-plan-for-your-customer"></a>O novo plano de compra para seu cliente

1. Selecione **os clientes** no painel de navegação esquerdo e, em seguida, selecione o cliente que você deseja mover para a nova assinatura.
2. Selecione **Adicionar assinatura**.
3. Selecione a assinatura que deseja comprar no catálogo (nesse caso, uma das opções acima), insira o número de licenças e selecione **Enviar**. 

Seu cliente agora terá a assinatura antiga e uma nova. A próxima etapa é reatribuir as licenças para os usuários do cliente.

1. Selecione **os clientes** no painel de navegação esquerdo e, em seguida, selecione o cliente que você está movendo.
2. Selecione **Usuários e licenças**.
3. Para reatribuir uma licença para um usuário, selecione o usuário e, em seguida, selecione **Gerenciar licenças**. 
4. Na página **Gerenciar licenças** , desmarque o Dynamics 365 for Sales / plano de envolvimento de cliente do Basic (oferecer qualificado) a caixa de seleção da licença e selecione um novo plano de serviço para a assinatura que o cliente está mudando. 
5. Selecione **Enviar**. Você fará isso para cada usuário que precisa a nova licença. 

Quando você tiver movido as licenças para a nova assinatura, você pode cancelar a assinatura antiga. 

1. Selecione **os clientes** no painel de navegação esquerdo e, em seguida, selecione o cliente que você está movendo.
2. Na página de detalhes de assinatura, defina a assinatura antiga como **suspensa** e selecione **Enviar**.

A assinatura antiga agora é suspenso, e a nova assinatura está ativa. A assinatura suspensa será desprovisionada automaticamente após 120 dias. Seu cliente provocará sem custos adicionais para a assinatura antiga.
 

 



