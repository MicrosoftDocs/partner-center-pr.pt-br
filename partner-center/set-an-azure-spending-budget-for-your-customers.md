---
title: Definir um orçamento de gasto do Azure para um cliente
ms.topic: how-to
ms.date: 03/17/2021
description: Saiba como definir ou remover orçamentos mensais de gastos do Azure para seus clientes e também para exibir dados de gastos do Azure e definir notificações relacionadas ao orçamento.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: eaf54898d7a130ca38e5a2aaeba279fb722c9e66
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712742"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a>Definir, verificar ou remover orçamentos mensais de gastos do Azure para clientes no Partner Center

**Funções apropriadas**

- Agente administrativo

Você pode [definir um orçamento de gastos do Azure mensal para seus clientes](#set-azure-spending-budget) no Partner Center. Isso ajuda seus clientes a gerenciar seus gastos com o Azure. Essa opção permite que você compare os gastos do Azure dos clientes com o orçamento durante o mês. Ele também ajuda seus clientes a orçar seus gastos do Azure para que sua fatura mensal não seja maior do que a previsão.

> [!NOTE]  
> Esse recurso não está disponível na área restrita ou no teste em contas de produção (TIP).

Depois [de definir um orçamento de gastos do Azure para seus clientes](#set-azure-spending-budget), você também pode examinar o uso do cliente das seguintes maneiras. Essas opções podem ajudá-lo a identificar serviços mal configurados ou tendências incomuns que podem sugerir fraudes. Em seguida, você pode trabalhar com seus clientes para identificar a causa raiz e gerenciar os custos. Se necessário, você também pode [alterar o orçamento do cliente](#set-azure-spending-budget) para um valor mais alto.

- [Verificar os gastos atuais do Azure](#check-current-azure-spending)

- [Ativar notificações por email para quando o gasto de um cliente estiver se aproximando de seu limite de orçamento](#notifications-for-budget-limits)

- [Exibir custos discriminados por serviço para assinaturas baseadas em uso](#itemized-costs-by-service)

Você também pode [remover um orçamento de gastos do Azure](#remove-azure-spending-budget) para clientes a qualquer momento.

## <a name="azure-spending-data"></a>Dados de gastos do Azure

Os dados de gastos do Azure são uma *estimativa* e *valores de cobrança reais podem variar*. O valor dos dados *não reflete* impostos, créditos, ajustes ou outros encargos que podem ser aplicados.

Os dados de gastos são *atualizados uma vez por dia*. Os clientes podem continuar a usar (e serem cobrados) os serviços e recursos do Azure, a menos que você altere as configurações de conta no portal do Azure.

## <a name="set-azure-spending-budget"></a>Definir orçamento de gastos do Azure

Você pode *definir um orçamento de gastos do Azure mensal* para vários clientes no Partner Center:

1. Entre no [Painel do Partner Center](https://partner.microsoft.com/dashboard/).

2. No menu à esquerda, em **CSP**, escolha **gastos do Azure**.

3. Na página **gastos do Azure** , em **clientes com assinaturas Microsoft Azure**, selecione os clientes para os quais você deseja definir um orçamento.

4. Insira um valor para o **orçamento mensal**.

5. Escolha **aplicar** para salvar as alterações.

Você também pode *definir um orçamento para um cliente individual* em suas configurações de assinatura:

1. Entre no Painel do Partner Center.

2. No menu à esquerda, em **CSP**, escolha **clientes**.

3. Na página **clientes** , selecione o **nome da empresa** do cliente.

4. Na página **assinaturas** do cliente, em **assinatura baseada em uso**, escolha **alterar orçamento**.

5. Insira um valor para o orçamento.

6. Escolha **aplicar** para salvar as alterações.

## <a name="remove-azure-spending-budget"></a>Remover orçamento de gastos do Azure

Você pode *remover um orçamento de gastos do Azure mensal* para seus clientes no Partner Center:

1. Entre no [Painel do Partner Center](https://partner.microsoft.com/dashboard/).

2. No menu à esquerda, em **CSP**, escolha **gastos do Azure**.

3. Na página **gastos do Azure** , em **clientes com assinaturas Microsoft Azure**, selecione os clientes cujo orçamento você deseja remover.

4. Escolha **remover orçamento**.

## <a name="check-current-azure-spending"></a>Verificar os gastos atuais do Azure

Você pode *acompanhar os gastos atuais dos clientes do Azure e os orçamentos mensais* a qualquer momento:

1. Entre no [Painel do Partner Center](https://partner.microsoft.com/dashboard/).

2. No menu à esquerda, em **CSP**, escolha **gastos do Azure**.

3. Na página de **gastos do Azure** , em **clientes com assinaturas Microsoft Azure**, você pode ver uma visão geral dos Orçamentos mensais dos clientes, estimativas de gastos atuais e percentual de orçamento usado.

## <a name="notifications-for-budget-limits"></a>Notificações para limites de orçamento

Você pode *ativar as notificações por email* para quando o gasto mensal do cliente estiver se aproximando de seu limite de orçamento. Ao ativar essa opção, você será notificado quando os clientes usarem 80% ou mais de seu orçamento mensal. Essa opção ajuda você a ficar atento à sua fatura do Azure. Para configurar notificações por email:

1. Conecte-se ao Partner Center.

2. Vá para **Configurações**.

3. Selecione **minhas preferências**.

4. Se você ainda não tiver feito isso, configure um endereço de email preferencial.

5. Configure o idioma preferencial para a notificação.

6. Selecione a guia **CSP** na seção **preferências de notificação** .

7. Marque a opção de email para notificação de **gastos do Azure** e **salve**.


## <a name="itemized-costs-by-service"></a>Custos discriminados por serviço

Você pode *exibir os custos discriminados (e o uso estimado) por serviço para assinaturas baseadas em uso*:

1. Conecte-se ao Partner Center.

2. No menu à esquerda, em **CSP**, escolha **clientes**.

3. Na página **clientes** , selecione o **nome da empresa** do cliente.

4. Na página **assinaturas** do cliente, em **assinaturas baseadas em uso**, selecione o nome da **assinatura**.

5. Na página da assinatura, você pode examinar os **custos discriminados** por serviço e o **uso estimado** para o mês atual.


## <a name="next-steps"></a>Próximas etapas

- [Nova experiência de comércio no CSP – cobrança do Azure](azure-plan-billing.md)
