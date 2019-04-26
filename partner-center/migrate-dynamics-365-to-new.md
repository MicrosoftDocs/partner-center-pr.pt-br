---
title: Migrar do Dynamics 365 Business Edition oferece para versões mais recentes | Partner Center
ms.topic: article
ms.date: 12/12/2018
description: As assinaturas do Dynamics 365 Business Edition não podem ser renovadas.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 oferece, renovar ofertas, novas SKUs do Dynamics 365
ms.openlocfilehash: ca1823c4055e2d89edc5c49e900a1c255a94f59a
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2019
ms.locfileid: "62134366"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a>Migrar as ofertas do Dynamics 365 Business Edition para versões mais recentes 

**Aplica-se a**

- Partner Center

Clientes de 1 de janeiro de 2019 efetivos com as assinaturas do Dynamics 365 Business Edition não podem renovar para essas ofertas herdadas; as assinaturas existentes não serão renovadas automaticamente quando eles expiram. Na página de detalhes da assinatura, o status da assinatura será alterado para "Expira em [Data]" de "Automático renova em [Data]".

Para garantir a continuidade para os clientes, você deve fazer a transição aquelas com assinatura prestes a expirar para uma opção com suporte, listados abaixo. É recomendável mover os clientes para as novas assinaturas antes da data de término da assinatura anual, para evitar possíveis interrupções de serviço.

Se você usar a API (CREST ou Partner Center), você pode encontrar a renovação de assinaturas prestes a expirar, avaliando a data de término da assinatura, juntamente com o auto = False propriedade. As assinaturas em questão serão definidas como auto renovar = False em 1 de janeiro de 2019. Você pode mover os clientes para um novo plano a qualquer momento. 

## <a name="the-dynamics-365-business-editions-being-retired"></a>O Dynamics 365 Business Editions sendo desativado

- Dynamics 365 para Finanças e operações do Business edition
- Dynamics 365 para Team Members, Business edition

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a>Central de negócios do Dynamics – novas ofertas do Dynamics 365 Business Edition

Com novas ofertas do Dynamics Business Central, seus clientes podem conectar suas finanças, vendas, serviço e operações para simplificar os processos de negócios, aprimorar as interações de cliente e tomar decisões melhores. Dynamics 365 Business Central é baseado em nuvem e disponível por meio de parceiros do programa provedor de solução de nuvem (CSP) apenas.
Os clientes de Business Edition são elegíveis para receber a transição com desconto de preços para a nova Central de negócios do Dynamics 365 oferece até 30 de junho de 2020.

## <a name="transition-customers-to-new-product-plans"></a>Transição dos clientes para novos planos do produto

 Mover os clientes de SKUs desativados para as mais novas exige as seguintes etapas nesta ordem:

- Comprar a nova assinatura
- Reatribuir as licenças de usuário atuais
- Cancelar a assinatura antiga

## <a name="purchase-the-new-plan-for-your-customer"></a>O novo plano de compra para seu cliente

1. Selecione **clientes** da navegação à esquerda e em seguida, selecione o cliente que você deseja mover para a nova assinatura.
2. Selecione **Adicionar assinatura**.
3. Selecione a assinatura que deseja comprar no catálogo (nesse caso, uma das opções acima), insira o número de licenças e selecione **Enviar**. 

Agora, o cliente terá a assinatura antiga e nova. A próxima etapa é reatribuir licenças aos usuários do cliente.

1. Selecione **clientes** da barra de navegação à esquerda e selecione o cliente estiver movendo.
2. Selecione **Usuários e licenças**.
3. Para reatribuir uma licença a um usuário, selecione o usuário e, em seguida, selecione **gerenciar licenças**. 
4. Sobre o **gerenciar licenças** página, desmarque o Dynamics 365 para vendas / plano de envolvimento do cliente do Basic (oferecer qualificado) caixa de seleção de licença e selecione um novo plano de serviço para a assinatura que o cliente está se movendo para. 
5. Selecione **Enviar**. Você fará isso para cada usuário que precisa da nova licença. 

Depois de mover as licenças ao longo para a nova assinatura, você pode cancelar a assinatura antiga. 

1. Selecione **clientes** da barra de navegação à esquerda e selecione o cliente estiver movendo.
2. Na página de detalhes da assinatura, defina a assinatura antiga **Suspended** e selecione **enviar**.

A assinatura antiga agora está suspenso e a nova assinatura está ativa. A assinatura suspensa será desprovisionada automaticamente após 120 dias. Seu cliente não incorrerá em nenhum custo adicional para a assinatura antiga.