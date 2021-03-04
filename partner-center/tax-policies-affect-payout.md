---
title: Como as políticas de impostos afetam o pagamento do Azure Marketplace
description: Saiba como as políticas de impostos afetam o pagamento do Azure Marketplace.
ms.topic: conceptual
ms.service: partner-dashboard
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: 3630824c839ccd9f54f3e8e5199a573b5824bb91
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/03/2021
ms.locfileid: "101758418"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a>Como as políticas de impostos afetam o pagamento do Azure Marketplace

**Funções apropriadas**
-    Administrador global
-    Administrador de usuários
-    Agente administrativo

## <a name="introduction"></a>Introdução

O Microsoft Commercial Marketplace tem alcance global. As transações ocorrem entre as bordas e, dependendo de onde o ISV e o cliente estão localizados, as implicações de impostos podem variar. Microsoft AppSource e o Azure Marketplace usam as informações do perfil de impostos do Partner Center para determinar o país do ISV. Para determinar o país do cliente, use as informações de cobrança do cliente ou, se o cliente estiver na UE, usaremos duas partes diferentes de informações.

Para entender melhor os cenários a seguir, consulte a tabela [detalhes do imposto](tax-details-marketplace.md) , que mostra se a Microsoft coleta e paga impostos em nome do Publicador ou se essa responsabilidade pertence ao Publicador.

> [!NOTE]
> Todos os exemplos de valores de venda e percentuais de imposto neste tópico são apenas para fins ilustrativos, não valores exatos.

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a>O Publicador reage no país de imposto gerenciado pela Microsoft

**Cenário A** – transações que ocorrem entre um Publicador e um cliente em um [país de imposto gerenciado pela Microsoft](tax-details-marketplace.md#microsoft-managed-countries). Essas transações terão imposto aplicável adicionado no momento da venda e a Microsoft enviará esse imposto para o país aplicável. Nenhum imposto é retido do pagamento e os cálculos de pagamento são exclusivos de impostos.

Consulte [cenário D](#foreign-publisher-transacts-with-us-customer) para transações entre um Publicador não-EUA e um cliente dos EUA.

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Mostra o fluxo de trabalho para o cenário de processo de pagamento A.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a>O Publicador reage no país de imposto gerenciado pela Microsoft em que a taxa do Marketplace é um serviço tributável

**Cenário B** – transações que ocorrem entre um Publicador baseado nos EUA (conforme definido pelas informações do perfil de impostos do Partner Center) para um cliente em um país de imposto gerenciado pela Microsoft onde o país impõe um imposto sobre a taxa do Marketplace (um serviço tributável). Nesse cenário, o imposto sobre a taxa do serviço de loja é subtraído do pagamento do editor.

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Mostra o fluxo de trabalho para o cenário de processo de pagamento B.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a>Publicador transatos no Publicador-país do imposto gerenciado

**Cenário C** – transações que ocorrem entre um Publicador e um cliente em um país de imposto gerenciado pelo Publicador que não impõe uma retenção de imposto sobre os clientes. Os clientes não pagam nenhum imposto no ponto de venda e é a obrigação do editor pagar todos os impostos aplicáveis.

Para obter mais informações sobre preços específicos do país (por exemplo, para deslocar a tributação futura), consulte [planos e preços para ofertas do Marketplace comercial](https://docs.microsoft.com/azure/marketplace/plans-pricing#custom-prices).

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Mostra o fluxo de trabalho para o cenário de processo de pagamento C.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a>Publicador externo interage com o cliente dos EUA

**Cenário D** – todos os Publicadores estrangeiros (conforme definido por suas informações de perfil de impostos do Partner Center) em países sem um Tratado de US (consulte o [cenário E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) fazendo uma venda para um cliente baseado nos EUA (conforme definido pelo endereço de sua conta de cliente). O governo dos EUA requer que a retenção de imposto da Microsoft seja em nome do Publicador. O imposto retido do pagamento para o Publicador é calculado com base no preço da oferta.

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Mostra o fluxo de trabalho para o cenário de processo de pagamento D.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a>Publicador estrangeiro com um tratado transatos com o cliente dos EUA

**Cenário E** – todos os Publicadores estrangeiros (conforme definido por suas informações de perfil de impostos do Partner Center) em países com um Tratado dos EUA fazendo uma venda para um cliente baseado nos EUA (conforme definido pelo endereço de sua conta de cliente). O governo dos EUA não exige que a Microsoft reponha impostos em nome do Publicador.

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Mostra o fluxo de trabalho para o cenário do processo de pagamento E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a>O Publicador estrangeiro vende para um cliente registrado por IVA da UE em um país gerenciado pela Microsoft (fora da Irlanda)

**Cenário F** – todas as transações entre Publicadores estrangeiros e clientes registrados no IVA da UE (fora da Irlanda) em um país Microsoft-Managed. O cliente não paga o imposto sobre a venda.

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Mostra o fluxo de trabalho para o cenário do processo de pagamento F.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a>O Publicador estrangeiro vende para um cliente registrado por IVA da UE em um país gerenciado pela Microsoft (na Irlanda)

**Cenário G** – todas as transações entre Publicadores estrangeiros e clientes registrados no IVA da UE (dentro da Irlanda) em um país Microsoft-Managed. O cliente paga o IVA da irlandês e a Microsoft paga esse imposto ao governo da irlandês.

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Mostra o fluxo de trabalho para o cenário de processo de pagamento G.":::

## <a name="next-steps"></a>Próximas etapas

- [Perguntas frequentes do Publicador](https://docs.microsoft.com/azure/marketplace/marketplace-faq-publisher-guide)
- [Instruções para criar perfis de pagamento e de impostos](https://docs.microsoft.com/partner-center/set-up-your-payout-account?context=/azure/marketplace/context/context#create-a-payment-profile)
