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
ms.openlocfilehash: 5ba6992eff64031aed0dafeb5a5010983396ab63
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151637"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>Migrar o Dynamics 365 e o Customer Engagement Plan de Basic (ofertas qualificadas) para versões mais recentes

**Funções apropriadas**: Administração Global | Administrador de gerenciamento de usuários | Agente de administração | Agente de vendas

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
- Dynamics 365 para sales Enterprise Edition Add-On para CRM Basic (oferta qualificada)
- Dynamics 365 for Sales Edição Enterprise Add-On for CRM Basic (Oferta Qualificada) para Docentes
- Dynamics 365 for Sales Edição Enterprise Add-On for CRM Basic (Oferta Qualificada) para Alunos
- Dynamics 365 for Sales Edição Enterprise (Preços governamentais) Add-On para CRM Basic (oferta qualificada)
- Plano de Participação do Cliente do Dynamics 365 Edição Enterprise CRMOL Basic (oferta qualificada)
- Plano de participação do cliente do Dynamics 365 Edição Enterprise (preços governamentais) CRMOL Basic (oferta qualificada)
- Plano de Participação do Cliente do Dynamics 365 Edição Enterprise CRMOL Basic (oferta qualificada) para alunos
- Plano de Participação do Cliente do Dynamics 365 Edição Enterprise CRMOL Basic (oferta qualificada) para docentes
- Plano de Participação do Cliente do Dynamics 365 Edição Enterprise do SA para CRM Basic (oferta qualificada)
- Plano de participação do cliente do Dynamics 365 Edição Enterprise (preços governamentais) do SA para CRM Basic (oferta qualificada)
- Plano de Participação do Cliente do Dynamics 365 Edição Enterprise do SA para CRM Basic (oferta qualificada) para alunos
- Plano de Participação do Cliente do Dynamics 365 Edição Enterprise do SA para CRM Basic (oferta qualificada) para docentes
- Plano de participação do cliente do Dynamics 365 Edição Enterprise Add-On para CRM Basic (oferta qualificada)
- Plano de participação do cliente do Dynamics 365 Edição Enterprise (preços governamentais) Add-On para CRM Basic (oferta qualificada)
- Plano de participação do cliente do Dynamics 365 Edição Enterprise Add-On para CRM Basic (oferta qualificada) para alunos
- Plano de participação do cliente do Dynamics 365 Edição Enterprise Add-On para CRM Basic (oferta qualificada) para docentes



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>Dynamics 365 for Sales/Customer Engagement Plan from Basic (Qualified Offers) replacement plans (Qualified Offers)

**Ofertas retiradas**   

- Dynamics 365 for Sales do CRM Basic ou CRMOL Basic (oferta qualificada)
- Plano de Participação do Cliente do Dynamics 365 do CRM Basic ou CRMOL Basic (oferta qualificada)

**Opções de substituição**
- Dynamics 365 for Sales Professional (NOVO)
- Dynamics 365 for Sales Professional (NOVO)
- Dynamics 365 for Customer Service
- Plano de Participação do Cliente do Dynamics 365 ou
- Membros da equipe do Dynamics 365



## <a name="transition-customers-to-new-product-plans"></a>Transição dos clientes para novos planos do produto

Mover os clientes de SKUs antigos para os mais novos requer as seguintes etapas nesta ordem:

- Comprar a nova assinatura
- Reatribuir as licenças de usuário atuais
- Cancelar a assinatura antiga

## <a name="purchase-the-new-plan-for-your-customer"></a>Comprar o novo plano para seu cliente

1. Selecione **Clientes** no nav à esquerda e, em seguida, selecione o cliente que você deseja mover para a nova assinatura.
2. Selecione **Adicionar Assinatura**.
3. Selecione a assinatura que deseja comprar no catálogo (nesse caso, uma das opções acima), insira o número de licenças e selecione **Enviar**. 

Seu cliente agora terá a assinatura antiga e a nova. A próxima etapa é reatribuir licenças aos usuários do cliente.

1. Selecione **Clientes** no nav à esquerda e, em seguida, selecione o cliente que você está movendo.
2. Selecione **Usuários e licenças**.
3. Para reatribuir uma licença a um usuário, selecione o usuário e, em seguida, **selecione Gerenciar licenças**. 
4. Na página Gerenciar **licenças, des** marque a caixa de seleção Dynamics 365 for Sales/Customer Engagement Plan da licença Básica (Oferta Qualificada) e selecione um novo plano de serviço para a assinatura para a qual o cliente está mudando. 
5. Selecione **Enviar**. Você fará isso para cada usuário que precisa da nova licença. 

Depois de ter movido as licenças para a nova assinatura, você pode cancelar a assinatura antiga. 

1. Selecione **Clientes** no nav à esquerda e, em seguida, selecione o cliente que você está movendo.
2. Na página de detalhes da assinatura, de definir a assinatura antiga como **Suspensa** e selecione **Enviar**.

A assinatura antiga agora está suspensa e a nova assinatura está ativa. A assinatura suspensa será desprovisionada automaticamente após 120 dias. Seu cliente não incorre em custos adicionais para a assinatura antiga.
 

 



