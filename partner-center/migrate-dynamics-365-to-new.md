---
title: Migrar o Dynamics 365 Business Edition oferece para versões mais recentes | Partner Center
ms.topic: article
ms.date: 12/12/2018
description: Assinaturas do Dynamics 365 Business Edition não podem ser renovadas.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: labrenne
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 offers, renew offers, new Dynamics 365 SKUs
ms.openlocfilehash: 11f0d9262856d28adb4d67871503d86f2d4945ac
ms.sourcegitcommit: 23adf424dd43ed0281473f97d535d73c59c92b01
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/13/2018
ms.locfileid: "8968276"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a>Migrar o Dynamics 365 Business Edition oferece para versões mais recentes 

**Aplica-se ao**

- Partner Center

Os clientes de 1º de janeiro de 2019, eficazes com assinaturas do Dynamics 365 Business Edition não podem renovar nessas ofertas herdadas; as assinaturas existentes não serão renovadas automaticamente quando expirarem. Na página de detalhes da assinatura, o status da assinatura será alterado para "Expira em [Data]" de "Renovação automática em [Data]".

Para garantir a continuidade dos clientes, você deve fazer a transição aqueles com assinaturas E4 vencidas para uma opção com suporte, listada abaixo. É recomendável mover os clientes para as novas assinaturas antes da data de término da assinatura anual, para evitar possíveis interrupções de serviço.

Se você usar a API (CREST ou Partner Center), você pode encontrar assinaturas vencidas avaliando a data de término da assinatura juntamente com automática = falsa propriedade. As assinaturas em questão serão definidas como automático renovar = falso em 1º de janeiro de 2019. Você pode mover os clientes para um novo plano a qualquer momento. 

## <a name="the-dynamics-365-business-editions-being-retired"></a>As edições de negócios do Dynamics 365 sendo desativado

- Dynamics 365 para Finanças e operações, edição de negócios
- Dynamics 365 for Team Members, edição de negócios

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a>Central de negócios do Dynamics - as novas ofertas Dynamics 365 Business Edition

Com novas ofertas Dynamics empresas Central, seus clientes podem se conectar suas finanças, vendas, serviço e operações para simplificar processos de negócios, melhorar as interações do cliente e tomar decisões melhores. Central de negócios do Dynamics 365 é baseado em nuvem e disponível por meio de parceiros do programa provedor de soluções na nuvem (CSP) apenas.
Os clientes de Business Edition estão qualificados para receber o preço com desconto de transição para a nova Central de negócios do Dynamics 365 oferece até 30 de junho de 2020.

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