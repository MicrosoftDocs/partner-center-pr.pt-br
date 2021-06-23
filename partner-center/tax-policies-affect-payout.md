---
title: Como as políticas fiscais afetam o pagamento de Azure Marketplace
description: Saiba como as políticas fiscais afetam o pagamento Azure Marketplace.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: 32c5cda9558aaaeddaf194eb8258ba732e2ac698
ms.sourcegitcommit: 09eabb559aae25518caf3f2a59ef16a3e123c207
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2021
ms.locfileid: "112489961"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a>Como as políticas fiscais afetam o pagamento de Azure Marketplace

**Funções apropriadas:** administrador global | Administrador de gerenciamento de usuários | Agente administrador

## <a name="introduction"></a>Introdução

O marketplace comercial da Microsoft tem alcance global. As transações ocorrem entre bordas e, dependendo de onde o ISV (fornecedor independente de software) e o cliente estão localizados, as implicações fiscais podem variar. Microsoft AppSource e Azure Marketplace o Partner Center informações de perfil de imposto para determinar o país do ISV. Para determinar o país do cliente, use as informações de cobrança do cliente ou, se o cliente estiver na UE, usamos duas informações diferentes.

Para entender melhor os cenários [](tax-details-marketplace.md) a seguir, consulte a tabela Detalhes do imposto, que mostra se a Microsoft coleta e paga impostos em nome do editor ou se essa responsabilidade pertence ao editor.

> [!NOTE]
> Todos os exemplos de valores de venda e percentuais de imposto neste tópico são apenas para fins ilustrativos, não para números exatos.

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a>Transações do Publicador no País de Imposto gerenciado pela Microsoft

**Cenário A** – transações que ocorrem entre um editor e um cliente em um [país fiscal gerenciado pela Microsoft.](tax-details-marketplace.md#microsoft-managed-countries) Essas transações terão o imposto aplicável adicionado no momento da venda e a Microsoft enviará esse imposto para o país aplicável. Nenhum imposto é retido dos cálculos de pagamento e pagamento são exclusivos do imposto.

Consulte [Cenário D](#foreign-publisher-transacts-with-us-customer) para transações entre um publicador não eua e um cliente dos EUA.

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Mostra o fluxo de trabalho para o cenário de processo de pagamento A.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a>Transações do Publicador no País de Imposto gerenciado pela Microsoft em que o Valor do Marketplace é Um Serviço Taxável

Cenário **B** – Transações que ocorrem entre um publicador baseado nos EUA (conforme definido por suas informações de perfil fiscal do Partner Center) para um cliente em um país fiscal gerenciado pela Microsoft em que o país impõe um imposto sobre o Valor do Marketplace (um serviço taxável). Nesse cenário, o imposto sobre o valor do serviço da loja é subtraído do pagamento do editor.

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Mostra o fluxo de trabalho para o cenário B do processo de pagamento.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a>Transações do publicador no país de imposto gerenciado pelo editor

**Cenário C** – transações que ocorrem entre um editor e um cliente em um país fiscal gerenciado pelo editor que não impõe um imposto retido nos clientes. Os clientes não pagam nenhum imposto no ponto de venda e é a obrigação do editor pagar todos os impostos aplicáveis.

Para obter mais informações sobre preços específicos do país (por exemplo, para compensar a futura taxação), consulte Planos e preços para ofertas [do marketplace comercial.](/azure/marketplace/plans-pricing#custom-prices)

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Mostra o fluxo de trabalho para o cenário de processo de pagamento C.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a>Transações do Publicador Externo com o Cliente dos EUA

Cenário **D** – Todos os editores externos (conforme definido por suas informações de perfil de imposto do Partner Center) em países sem um governo dos EUA (consulte Cenário [E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) fazendo uma venda para um cliente baseado nos EUA (conforme definido pelo endereço da conta do cliente). O governo dos EUA exige que a Microsoft reter os impostos em nome do editor. O imposto retido do pagamento para o publicador é calculado com base no preço da oferta.

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Mostra o fluxo de trabalho para o cenário de processo de pagamento D.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a>Publicador externo com uma Transacts Desodorização com o cliente dos EUA

**Cenário E** – todos os editores externos (conforme definido por suas informações de perfil de imposto do Partner Center) em países com uma oferta dos EUA fazendo uma venda para um cliente baseado nos EUA (conforme definido pelo endereço da conta do cliente). O governo dos EUA não exige que a Microsoft reter impostos em nome do editor.

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Mostra o fluxo de trabalho para o cenário de processo de pagamento E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a>O publicador externo vende para um cliente registrado no IVA da UE em um país gerenciado pela Microsoft (fora da Irlanda)

**Cenário F** – todas as transações entre publicações estrangeiras e clientes registrados no IVA (imposto sobre valor agregado) da UE (fora da Irlanda) em um Microsoft-Managed país. O cliente não paga imposto sobre a venda.

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Mostra o fluxo de trabalho para o cenário de processo de pagamento F.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a>O publicador externo vende para um cliente registrado no IVA da UE em um país gerenciado pela Microsoft (na Irlanda)

**Cenário G** – todas as transações entre publicações estrangeiras e clientes registrados no IVA da UE (dentro da Irlanda) em um Microsoft-Managed país. O cliente paga o IVA da Irlanda e a Microsoft paga esse imposto ao governo da Irlanda.

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Mostra o fluxo de trabalho para o cenário de processo de pagamento G.":::

## <a name="next-steps"></a>Próximas etapas

- [Perguntas frequentes sobre o publicador](/azure/marketplace/marketplace-faq-publisher-guide)
- [Instruções para criar perfis de pagamento e imposto](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)