---
title: Migrar o Dynamics 365 Business Edition
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como migrar ofertas do Dynamics 365 Business Edition qualificadas para versões mais recentes antes que elas expirem.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
Keywords: O Dynamics 365 oferece, renovar ofertas, novas SKUs do Dynamics 365
ms.openlocfilehash: 9675f607d183c5d427371de4f09f088fd267c573
ms.sourcegitcommit: e0a1b4506840486f4bb82620051e0f6a5e81662a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "84992084"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a>Migrar as ofertas do Dynamics 365 Business Edition para versões mais recentes

**Aplica-se a**

- Partner Center

**Funções apropriadas**
- Administrador global
- Administrador de usuários
- Agente administrativo
- Agente de vendas

A partir de 1º de janeiro de 2019, os clientes com as assinaturas do Dynamics 365 Business Edition não podem mais renovar essas ofertas herdadas; as assinaturas existentes não serão renovadas automaticamente quando expirarem. Na página de detalhes da assinatura, o status da assinatura será alterado para "expira em [data]" de "renovações automáticas em [data]".

Para garantir a continuidade dos clientes, você deve fazer a transição deles com assinaturas expirando para uma opção com suporte, listada abaixo. É recomendável mover os clientes para novas assinaturas antes da data de término anual da assinatura para evitar qualquer interrupção de serviço para os clientes.

Se você usar a API (CREST ou o Partner Center), poderá encontrar assinaturas expirando, avaliando a data de término da assinatura junto com a propriedade renovação automática = falso. As assinaturas em questão serão definidas para renovação automática = falso em 1º de janeiro de 2019. Você pode mover os clientes para um novo plano a qualquer momento. 

## <a name="the-dynamics-365-business-editions-being-retired"></a>As edições Business do Dynamics 365 estão sendo desativadas

- Dynamics 365 for Finance and Operations, Business Edition
- Dynamics 365 para Team Members, Business Edition

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a>Dynamics Business Central-as novas ofertas do Dynamics 365 Business Edition

Com as novas ofertas do Dynamics Business central, seus clientes podem conectar suas finanças, vendas, serviços e operações para simplificar os processos de negócios, melhorar as interações com o cliente e tomar decisões melhores. O Dynamics 365 Business central é baseado em nuvem e está disponível somente por meio de parceiros do programa CSP (provedor de soluções na nuvem).
Os clientes do Dynamics 365 Business Edition estão qualificados a receber preços de transição com desconto para as novas ofertas do Business central até 30 de junho de 2020.

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
