---
title: Migrar assinaturas do Dynamics 365 qualificadas
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como migrar de assinaturas do Dynamics 365 básicas e qualificadas para uma nova assinatura antes que as assinaturas existentes expirem.
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
Keywords: O Dynamics 365 oferece, renovar ofertas, novas SKUs do Dynamics 365
ms.openlocfilehash: 5225ff60399cd491009ecb16e4c17b4fc05c0052
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/03/2020
ms.locfileid: "85949644"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>Migrar o Dynamics 365 e o Customer Engagement Plan de Basic (ofertas qualificadas) para versões mais recentes

**Aplica-se a**

-  Partner Center

**Funções apropriadas**
-   Administrador global
-   Administrador de usuários
-   Agente administrativo
-   Agente de vendas

A partir de 1º de janeiro de 2019, os clientes com Dynamics 365 para o plano de vendas/envolvimento do cliente das assinaturas básicas (ofertas qualificadas) não podem mais renovar essas ofertas herdadas; as assinaturas existentes não serão renovadas automaticamente quando expirarem. Na página de detalhes da assinatura, o status da assinatura será alterado para "expira em [data]" de "renovações automáticas em [data]". 

Para garantir a continuidade dos clientes, você deve fazer a transição deles com assinaturas expirando para uma opção com suporte, listada abaixo. É recomendável mover os clientes para novas assinaturas antes da data de término anual da assinatura para evitar qualquer interrupção de serviço para os clientes.

Se você usar a API (CREST ou o Partner Center), poderá encontrar assinaturas expirando, avaliando a data de término da assinatura junto com a propriedade renovação automática = falso. As assinaturas em questão serão definidas para renovação automática = falso em 1º de janeiro de 2019. Você pode mover os clientes para um novo plano a qualquer momento. 

### <a name="the-dynamics-365-offers-being-retired"></a>As ofertas do Dynamics 365 estão sendo desativadas

- Dynamics 365 para sales Enterprise Edition CRMOL Basic (oferta qualificada)
- Dynamics 365 para sales Enterprise Edition CRMOL Basic (oferta qualificada) para docentes
- Dynamics 365 para sales Enterprise Edition CRMOL Basic (oferta qualificada) para estudantes
- Dynamics 365 para sales Enterprise Edition (preços do governo) CRMOL básico (oferta qualificada)
- Dynamics 365 para sales Enterprise Edition do SA para CRM básico (oferta qualificada)
- Dynamics 365 para sales Enterprise Edition do SA para CRM básico (oferta qualificada) para docentes
- Dynamics 365 para sales Enterprise Edition do SA para CRM básico (oferta qualificada) para estudantes
- Dynamics 365 para sales Enterprise Edition (preços do governo) do SA para CRM básico (oferta qualificada)
- Complemento do Dynamics 365 para sales Enterprise Edition para CRM básico (oferta qualificada)
- Dynamics 365 for Sales Enterprise Edition complemento para CRM básico (oferta qualificada) para docentes
- Dynamics 365 for Sales Enterprise Edition complemento para CRM básico (oferta qualificada) para estudantes
- Complemento do Dynamics 365 para sales Enterprise Edition (preços do governo) para CRM básico (oferta qualificada)
- Plano de envolvimento do cliente do Dynamics 365 Enterprise Edition CRMOL Basic (oferta qualificada)
- Plano de envolvimento do cliente do Dynamics 365 Enterprise Edition (preços do governo) CRMOL básico (oferta qualificada)
- Plano de envolvimento do cliente do Dynamics 365 Enterprise Edition CRMOL Basic (oferta qualificada) para estudantes
- Plano de envolvimento do cliente do Dynamics 365 Enterprise Edition CRMOL Basic (oferta qualificada) para docentes
- Plano de envolvimento do cliente do Dynamics 365 Enterprise Edition do SA para CRM básico (oferta qualificada)
- Plano de envolvimento do cliente do Dynamics 365 Enterprise Edition (preço governamental) do SA para CRM básico (oferta qualificada)
- Plano de envolvimento do cliente do Dynamics 365 Enterprise Edition do SA para CRM básico (oferta qualificada) para estudantes
- Plano de envolvimento do cliente do Dynamics 365 Enterprise Edition do SA para CRM básico (oferta qualificada) para docentes
- Dynamics 365 plano de envolvimento do cliente Enterprise Edition complemento para CRM básico (oferta qualificada)
- Plano de envolvimento do cliente do Dynamics 365 Enterprise Edition (preço do governo) complemento para CRM básico (oferta qualificada)
- Dynamics 365 plano de envolvimento do cliente Enterprise Edition complemento para CRM básico (oferta qualificada) para estudantes
- Dynamics 365 plano de envolvimento do cliente Enterprise Edition complemento para CRM básico (oferta qualificada) para docentes



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>Dynamics 365 para vendas/plano de envolvimento com o cliente de planos de substituição básicos (ofertas qualificadas)

**Ofertas desativadas**   

- Dynamics 365 para vendas do CRM Basic ou do CRMOL Basic (oferta qualificada)
- Plano de envolvimento do cliente do Dynamics 365 do CRM Basic ou do CRMOL Basic (oferta qualificada)

**Opções de substituição**
- Dynamics 365 for Sales Professional (novo)
- Dynamics 365 for Sales Professional (novo)
- Dynamics 365 for Customer Service
- Plano de envolvimento do cliente do Dynamics 365 ou
- Membros da equipe do Dynamics 365



## <a name="transition-customers-to-new-product-plans"></a>Transição dos clientes para novos planos do produto

Mover clientes de SKUs desativados para os mais recentes requer as seguintes etapas nesta ordem:

- Comprar a nova assinatura
- Reatribuir as licenças de usuário atuais
- Cancelar a assinatura antiga

## <a name="purchase-the-new-plan-for-your-customer"></a>Comprar o novo plano para o cliente

1. Selecione **clientes** na barra de navegação à esquerda e, em seguida, selecione o cliente que você deseja mover para a nova assinatura.
2. Selecione **Adicionar assinatura**.
3. Selecione a assinatura que deseja comprar no catálogo (nesse caso, uma das opções acima), insira o número de licenças e selecione **Enviar**. 

Agora, seu cliente terá a assinatura antiga e a nova. A próxima etapa é reatribuir licenças aos usuários do cliente.

1. Selecione **clientes** na barra de navegação à esquerda e, em seguida, selecione o cliente que você está movendo.
2. Selecione **usuários e licenças**.
3. Para reatribuir uma licença a um usuário, selecione o usuário e, em seguida, selecione **gerenciar licenças**. 
4. Na página **gerenciar licenças** , desmarque a caixa de seleção Dynamics 365 para vendas/plano de envolvimento do cliente da licença básica (oferta qualificada) e selecione um novo plano de serviço para a assinatura à qual o cliente está se movendo. 
5. Selecione **Enviar**. Você fará isso para cada usuário que precisa da nova licença. 

Depois de mover as licenças para a nova assinatura, você poderá cancelar a assinatura antiga. 

1. Selecione **clientes** na barra de navegação à esquerda e, em seguida, selecione o cliente que você está movendo.
2. Na página detalhes da assinatura, defina a assinatura antiga como **suspensa** e selecione **Enviar**.

A assinatura antiga agora está suspensa e a nova assinatura está ativa. A assinatura suspensa será desprovisionada automaticamente após 120 dias. Seu cliente não incorrerá em nenhum custo adicional para a assinatura antiga.
 

 



