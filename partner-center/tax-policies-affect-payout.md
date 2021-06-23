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
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a><span data-ttu-id="083b0-103">Como as políticas fiscais afetam o pagamento de Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="083b0-103">How tax policies affect payout for Azure Marketplace</span></span>

<span data-ttu-id="083b0-104">**Funções apropriadas:** administrador global | Administrador de gerenciamento de usuários | Agente administrador</span><span class="sxs-lookup"><span data-stu-id="083b0-104">**Appropriate roles**: Global admin | User management admin | Admin agent</span></span>

## <a name="introduction"></a><span data-ttu-id="083b0-105">Introdução</span><span class="sxs-lookup"><span data-stu-id="083b0-105">Introduction</span></span>

<span data-ttu-id="083b0-106">O marketplace comercial da Microsoft tem alcance global.</span><span class="sxs-lookup"><span data-stu-id="083b0-106">The Microsoft commercial marketplace has global reach.</span></span> <span data-ttu-id="083b0-107">As transações ocorrem entre bordas e, dependendo de onde o ISV (fornecedor independente de software) e o cliente estão localizados, as implicações fiscais podem variar.</span><span class="sxs-lookup"><span data-stu-id="083b0-107">Transactions occur across borders and depending on where the independent software vendor (ISV) and the customer are located, tax implications can vary.</span></span> <span data-ttu-id="083b0-108">Microsoft AppSource e Azure Marketplace o Partner Center informações de perfil de imposto para determinar o país do ISV.</span><span class="sxs-lookup"><span data-stu-id="083b0-108">Microsoft AppSource and Azure Marketplace use the Partner Center Tax Profile Information to determine the ISV's country.</span></span> <span data-ttu-id="083b0-109">Para determinar o país do cliente, use as informações de cobrança do cliente ou, se o cliente estiver na UE, usamos duas informações diferentes.</span><span class="sxs-lookup"><span data-stu-id="083b0-109">To determine the customer's country, either use the customer's billing information or, if the customer is in the EU, we use two different pieces of information.</span></span>

<span data-ttu-id="083b0-110">Para entender melhor os cenários [](tax-details-marketplace.md) a seguir, consulte a tabela Detalhes do imposto, que mostra se a Microsoft coleta e paga impostos em nome do editor ou se essa responsabilidade pertence ao editor.</span><span class="sxs-lookup"><span data-stu-id="083b0-110">To better understand the following scenarios, refer to the [Tax details](tax-details-marketplace.md) table, which shows whether Microsoft collects and pays taxes on behalf of the publisher or if that responsibility belongs to the publisher.</span></span>

> [!NOTE]
> <span data-ttu-id="083b0-111">Todos os exemplos de valores de venda e percentuais de imposto neste tópico são apenas para fins ilustrativos, não para números exatos.</span><span class="sxs-lookup"><span data-stu-id="083b0-111">All examples sale values and tax percentages in this topic are for illustrative purposes only, not exact figures.</span></span>

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a><span data-ttu-id="083b0-112">Transações do Publicador no País de Imposto gerenciado pela Microsoft</span><span class="sxs-lookup"><span data-stu-id="083b0-112">Publisher Transacts in Microsoft-managed Tax Country</span></span>

<span data-ttu-id="083b0-113">**Cenário A** – transações que ocorrem entre um editor e um cliente em um [país fiscal gerenciado pela Microsoft.](tax-details-marketplace.md#microsoft-managed-countries)</span><span class="sxs-lookup"><span data-stu-id="083b0-113">**Scenario A** – Transactions that take place between a publisher and a customer in a [Microsoft-managed tax country](tax-details-marketplace.md#microsoft-managed-countries).</span></span> <span data-ttu-id="083b0-114">Essas transações terão o imposto aplicável adicionado no momento da venda e a Microsoft enviará esse imposto para o país aplicável.</span><span class="sxs-lookup"><span data-stu-id="083b0-114">These transactions will have applicable tax added at the time of sale and Microsoft sends that tax to the applicable country.</span></span> <span data-ttu-id="083b0-115">Nenhum imposto é retido dos cálculos de pagamento e pagamento são exclusivos do imposto.</span><span class="sxs-lookup"><span data-stu-id="083b0-115">No taxes are withheld from payout and payout calculations are tax exclusive.</span></span>

<span data-ttu-id="083b0-116">Consulte [Cenário D](#foreign-publisher-transacts-with-us-customer) para transações entre um publicador não eua e um cliente dos EUA.</span><span class="sxs-lookup"><span data-stu-id="083b0-116">See [Scenario D](#foreign-publisher-transacts-with-us-customer) for transactions between a non-US publisher and a US customer.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Mostra o fluxo de trabalho para o cenário de processo de pagamento A.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a><span data-ttu-id="083b0-118">Transações do Publicador no País de Imposto gerenciado pela Microsoft em que o Valor do Marketplace é Um Serviço Taxável</span><span class="sxs-lookup"><span data-stu-id="083b0-118">Publisher Transacts in Microsoft-managed Tax Country where Marketplace Fee is Taxable Service</span></span>

<span data-ttu-id="083b0-119">Cenário **B** – Transações que ocorrem entre um publicador baseado nos EUA (conforme definido por suas informações de perfil fiscal do Partner Center) para um cliente em um país fiscal gerenciado pela Microsoft em que o país impõe um imposto sobre o Valor do Marketplace (um serviço taxável).</span><span class="sxs-lookup"><span data-stu-id="083b0-119">**Scenario B** – Transactions that take place between a US-based publisher (as defined by their Partner Center Tax Profile Information) to a customer in a Microsoft-managed tax country where the country imposes a tax on the Marketplace Fee (a taxable service).</span></span> <span data-ttu-id="083b0-120">Nesse cenário, o imposto sobre o valor do serviço da loja é subtraído do pagamento do editor.</span><span class="sxs-lookup"><span data-stu-id="083b0-120">In this scenario, the tax on the store service fee is subtracted from the publisher's payout.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Mostra o fluxo de trabalho para o cenário B do processo de pagamento.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a><span data-ttu-id="083b0-122">Transações do publicador no país de imposto gerenciado pelo editor</span><span class="sxs-lookup"><span data-stu-id="083b0-122">Publisher Transacts in Publisher-managed Tax Country</span></span>

<span data-ttu-id="083b0-123">**Cenário C** – transações que ocorrem entre um editor e um cliente em um país fiscal gerenciado pelo editor que não impõe um imposto retido nos clientes.</span><span class="sxs-lookup"><span data-stu-id="083b0-123">**Scenario C** – Transactions that take place between a publisher and a customer in a publisher-managed tax country that does not impose a withholding tax on customers.</span></span> <span data-ttu-id="083b0-124">Os clientes não pagam nenhum imposto no ponto de venda e é a obrigação do editor pagar todos os impostos aplicáveis.</span><span class="sxs-lookup"><span data-stu-id="083b0-124">Customers pay no tax at the point of sale and it is the publisher's obligation to pay all applicable taxes.</span></span>

<span data-ttu-id="083b0-125">Para obter mais informações sobre preços específicos do país (por exemplo, para compensar a futura taxação), consulte Planos e preços para ofertas [do marketplace comercial.](/azure/marketplace/plans-pricing#custom-prices)</span><span class="sxs-lookup"><span data-stu-id="083b0-125">For more information on country-specific pricing (for example, to offset upcoming taxation) see [Plans and pricing for commercial marketplace offers](/azure/marketplace/plans-pricing#custom-prices).</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Mostra o fluxo de trabalho para o cenário de processo de pagamento C.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a><span data-ttu-id="083b0-127">Transações do Publicador Externo com o Cliente dos EUA</span><span class="sxs-lookup"><span data-stu-id="083b0-127">Foreign Publisher Transacts with US Customer</span></span>

<span data-ttu-id="083b0-128">Cenário **D** – Todos os editores externos (conforme definido por suas informações de perfil de imposto do Partner Center) em países sem um governo dos EUA (consulte Cenário [E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) fazendo uma venda para um cliente baseado nos EUA (conforme definido pelo endereço da conta do cliente).</span><span class="sxs-lookup"><span data-stu-id="083b0-128">**Scenario D** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries without a US treaty (see [Scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="083b0-129">O governo dos EUA exige que a Microsoft reter os impostos em nome do editor.</span><span class="sxs-lookup"><span data-stu-id="083b0-129">US government requires that Microsoft withhold tax on behalf of the publisher.</span></span> <span data-ttu-id="083b0-130">O imposto retido do pagamento para o publicador é calculado com base no preço da oferta.</span><span class="sxs-lookup"><span data-stu-id="083b0-130">Tax withheld from payout to publisher is calculated based on offer price.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Mostra o fluxo de trabalho para o cenário de processo de pagamento D.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a><span data-ttu-id="083b0-132">Publicador externo com uma Transacts Desodorização com o cliente dos EUA</span><span class="sxs-lookup"><span data-stu-id="083b0-132">Foreign publisher with a Treaty Transacts with US customer</span></span>

<span data-ttu-id="083b0-133">**Cenário E** – todos os editores externos (conforme definido por suas informações de perfil de imposto do Partner Center) em países com uma oferta dos EUA fazendo uma venda para um cliente baseado nos EUA (conforme definido pelo endereço da conta do cliente).</span><span class="sxs-lookup"><span data-stu-id="083b0-133">**Scenario E** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries with a US treaty making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="083b0-134">O governo dos EUA não exige que a Microsoft reter impostos em nome do editor.</span><span class="sxs-lookup"><span data-stu-id="083b0-134">US government does not require Microsoft to withhold tax on behalf of the publisher.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Mostra o fluxo de trabalho para o cenário de processo de pagamento E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a><span data-ttu-id="083b0-136">O publicador externo vende para um cliente registrado no IVA da UE em um país gerenciado pela Microsoft (fora da Irlanda)</span><span class="sxs-lookup"><span data-stu-id="083b0-136">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (outside Ireland)</span></span>

<span data-ttu-id="083b0-137">**Cenário F** – todas as transações entre publicações estrangeiras e clientes registrados no IVA (imposto sobre valor agregado) da UE (fora da Irlanda) em um Microsoft-Managed país.</span><span class="sxs-lookup"><span data-stu-id="083b0-137">**Scenario F** – All transactions between foreign publishers and EU value-added tax (VAT)-registered customers (outside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="083b0-138">O cliente não paga imposto sobre a venda.</span><span class="sxs-lookup"><span data-stu-id="083b0-138">The customer does not pay tax on the sale.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Mostra o fluxo de trabalho para o cenário de processo de pagamento F.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a><span data-ttu-id="083b0-140">O publicador externo vende para um cliente registrado no IVA da UE em um país gerenciado pela Microsoft (na Irlanda)</span><span class="sxs-lookup"><span data-stu-id="083b0-140">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (in Ireland)</span></span>

<span data-ttu-id="083b0-141">**Cenário G** – todas as transações entre publicações estrangeiras e clientes registrados no IVA da UE (dentro da Irlanda) em um Microsoft-Managed país.</span><span class="sxs-lookup"><span data-stu-id="083b0-141">**Scenario G** – All transactions between foreign publishers and EU VAT-registered customers (inside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="083b0-142">O cliente paga o IVA da Irlanda e a Microsoft paga esse imposto ao governo da Irlanda.</span><span class="sxs-lookup"><span data-stu-id="083b0-142">The customer pays Irish VAT and Microsoft pays this tax to the Irish government.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Mostra o fluxo de trabalho para o cenário de processo de pagamento G.":::

## <a name="next-steps"></a><span data-ttu-id="083b0-144">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="083b0-144">Next steps</span></span>

- [<span data-ttu-id="083b0-145">Perguntas frequentes sobre o publicador</span><span class="sxs-lookup"><span data-stu-id="083b0-145">Publisher FAQ</span></span>](/azure/marketplace/marketplace-faq-publisher-guide)
- [<span data-ttu-id="083b0-146">Instruções para criar perfis de pagamento e imposto</span><span class="sxs-lookup"><span data-stu-id="083b0-146">Instructions to create payment and tax profiles</span></span>](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)