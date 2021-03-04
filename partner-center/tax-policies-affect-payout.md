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
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a><span data-ttu-id="24cff-103">Como as políticas de impostos afetam o pagamento do Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="24cff-103">How tax policies affect payout for Azure Marketplace</span></span>

<span data-ttu-id="24cff-104">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="24cff-104">**Appropriate roles**</span></span>
-    <span data-ttu-id="24cff-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="24cff-105">Global admin</span></span>
-    <span data-ttu-id="24cff-106">Administrador de usuários</span><span class="sxs-lookup"><span data-stu-id="24cff-106">User admin</span></span>
-    <span data-ttu-id="24cff-107">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="24cff-107">Admin agent</span></span>

## <a name="introduction"></a><span data-ttu-id="24cff-108">Introdução</span><span class="sxs-lookup"><span data-stu-id="24cff-108">Introduction</span></span>

<span data-ttu-id="24cff-109">O Microsoft Commercial Marketplace tem alcance global.</span><span class="sxs-lookup"><span data-stu-id="24cff-109">The Microsoft commercial marketplace has global reach.</span></span> <span data-ttu-id="24cff-110">As transações ocorrem entre as bordas e, dependendo de onde o ISV e o cliente estão localizados, as implicações de impostos podem variar.</span><span class="sxs-lookup"><span data-stu-id="24cff-110">Transactions occur across borders and depending on where the ISV and the customer are located, tax implications can vary.</span></span> <span data-ttu-id="24cff-111">Microsoft AppSource e o Azure Marketplace usam as informações do perfil de impostos do Partner Center para determinar o país do ISV.</span><span class="sxs-lookup"><span data-stu-id="24cff-111">Microsoft AppSource and Azure Marketplace use the Partner Center Tax Profile Information to determine the ISV's country.</span></span> <span data-ttu-id="24cff-112">Para determinar o país do cliente, use as informações de cobrança do cliente ou, se o cliente estiver na UE, usaremos duas partes diferentes de informações.</span><span class="sxs-lookup"><span data-stu-id="24cff-112">To determine the customer's country, either use the customer's billing information or, if the customer is in the EU, we use two different pieces of information.</span></span>

<span data-ttu-id="24cff-113">Para entender melhor os cenários a seguir, consulte a tabela [detalhes do imposto](tax-details-marketplace.md) , que mostra se a Microsoft coleta e paga impostos em nome do Publicador ou se essa responsabilidade pertence ao Publicador.</span><span class="sxs-lookup"><span data-stu-id="24cff-113">To better understand the following scenarios, refer to the [Tax details](tax-details-marketplace.md) table, which shows whether Microsoft collects and pays taxes on behalf of the publisher or if that responsibility belongs to the publisher.</span></span>

> [!NOTE]
> <span data-ttu-id="24cff-114">Todos os exemplos de valores de venda e percentuais de imposto neste tópico são apenas para fins ilustrativos, não valores exatos.</span><span class="sxs-lookup"><span data-stu-id="24cff-114">All examples sale values and tax percentages in this topic are for illustrative purposes only, not exact figures.</span></span>

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a><span data-ttu-id="24cff-115">O Publicador reage no país de imposto gerenciado pela Microsoft</span><span class="sxs-lookup"><span data-stu-id="24cff-115">Publisher Transacts in Microsoft-managed Tax Country</span></span>

<span data-ttu-id="24cff-116">**Cenário A** – transações que ocorrem entre um Publicador e um cliente em um [país de imposto gerenciado pela Microsoft](tax-details-marketplace.md#microsoft-managed-countries).</span><span class="sxs-lookup"><span data-stu-id="24cff-116">**Scenario A** – Transactions that take place between a publisher and a customer in a [Microsoft-managed tax country](tax-details-marketplace.md#microsoft-managed-countries).</span></span> <span data-ttu-id="24cff-117">Essas transações terão imposto aplicável adicionado no momento da venda e a Microsoft enviará esse imposto para o país aplicável.</span><span class="sxs-lookup"><span data-stu-id="24cff-117">These transactions will have applicable tax added at the time of sale and Microsoft sends that tax to the applicable country.</span></span> <span data-ttu-id="24cff-118">Nenhum imposto é retido do pagamento e os cálculos de pagamento são exclusivos de impostos.</span><span class="sxs-lookup"><span data-stu-id="24cff-118">No taxes are withheld from payout and payout calculations are tax exclusive.</span></span>

<span data-ttu-id="24cff-119">Consulte [cenário D](#foreign-publisher-transacts-with-us-customer) para transações entre um Publicador não-EUA e um cliente dos EUA.</span><span class="sxs-lookup"><span data-stu-id="24cff-119">See [Scenario D](#foreign-publisher-transacts-with-us-customer) for transactions between a non-US publisher and a US customer.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Mostra o fluxo de trabalho para o cenário de processo de pagamento A.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a><span data-ttu-id="24cff-121">O Publicador reage no país de imposto gerenciado pela Microsoft em que a taxa do Marketplace é um serviço tributável</span><span class="sxs-lookup"><span data-stu-id="24cff-121">Publisher Transacts in Microsoft-managed Tax Country where Marketplace Fee is Taxable Service</span></span>

<span data-ttu-id="24cff-122">**Cenário B** – transações que ocorrem entre um Publicador baseado nos EUA (conforme definido pelas informações do perfil de impostos do Partner Center) para um cliente em um país de imposto gerenciado pela Microsoft onde o país impõe um imposto sobre a taxa do Marketplace (um serviço tributável).</span><span class="sxs-lookup"><span data-stu-id="24cff-122">**Scenario B** – Transactions that take place between a US-based publisher (as defined by their Partner Center Tax Profile Information) to a customer in a Microsoft-managed tax country where the country imposes a tax on the Marketplace Fee (a taxable service).</span></span> <span data-ttu-id="24cff-123">Nesse cenário, o imposto sobre a taxa do serviço de loja é subtraído do pagamento do editor.</span><span class="sxs-lookup"><span data-stu-id="24cff-123">In this scenario, the tax on the store service fee is subtracted from the publisher's payout.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Mostra o fluxo de trabalho para o cenário de processo de pagamento B.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a><span data-ttu-id="24cff-125">Publicador transatos no Publicador-país do imposto gerenciado</span><span class="sxs-lookup"><span data-stu-id="24cff-125">Publisher Transacts in Publisher-managed Tax Country</span></span>

<span data-ttu-id="24cff-126">**Cenário C** – transações que ocorrem entre um Publicador e um cliente em um país de imposto gerenciado pelo Publicador que não impõe uma retenção de imposto sobre os clientes.</span><span class="sxs-lookup"><span data-stu-id="24cff-126">**Scenario C** – Transactions that take place between a publisher and a customer in a publisher-managed tax country that does not impose a withholding tax on customers.</span></span> <span data-ttu-id="24cff-127">Os clientes não pagam nenhum imposto no ponto de venda e é a obrigação do editor pagar todos os impostos aplicáveis.</span><span class="sxs-lookup"><span data-stu-id="24cff-127">Customers pay no tax at the point of sale and it is the publisher's obligation to pay all applicable taxes.</span></span>

<span data-ttu-id="24cff-128">Para obter mais informações sobre preços específicos do país (por exemplo, para deslocar a tributação futura), consulte [planos e preços para ofertas do Marketplace comercial](https://docs.microsoft.com/azure/marketplace/plans-pricing#custom-prices).</span><span class="sxs-lookup"><span data-stu-id="24cff-128">For more information on country-specific pricing (for example, to offset upcoming taxation) see [Plans and pricing for commercial marketplace offers](https://docs.microsoft.com/azure/marketplace/plans-pricing#custom-prices).</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Mostra o fluxo de trabalho para o cenário de processo de pagamento C.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a><span data-ttu-id="24cff-130">Publicador externo interage com o cliente dos EUA</span><span class="sxs-lookup"><span data-stu-id="24cff-130">Foreign Publisher Transacts with US Customer</span></span>

<span data-ttu-id="24cff-131">**Cenário D** – todos os Publicadores estrangeiros (conforme definido por suas informações de perfil de impostos do Partner Center) em países sem um Tratado de US (consulte o [cenário E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) fazendo uma venda para um cliente baseado nos EUA (conforme definido pelo endereço de sua conta de cliente).</span><span class="sxs-lookup"><span data-stu-id="24cff-131">**Scenario D** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries without a US treaty (see [Scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="24cff-132">O governo dos EUA requer que a retenção de imposto da Microsoft seja em nome do Publicador.</span><span class="sxs-lookup"><span data-stu-id="24cff-132">US government requires that Microsoft withhold tax on behalf of the publisher.</span></span> <span data-ttu-id="24cff-133">O imposto retido do pagamento para o Publicador é calculado com base no preço da oferta.</span><span class="sxs-lookup"><span data-stu-id="24cff-133">Tax withheld from payout to publisher is calculated based on offer price.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Mostra o fluxo de trabalho para o cenário de processo de pagamento D.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a><span data-ttu-id="24cff-135">Publicador estrangeiro com um tratado transatos com o cliente dos EUA</span><span class="sxs-lookup"><span data-stu-id="24cff-135">Foreign publisher with a Treaty Transacts with US customer</span></span>

<span data-ttu-id="24cff-136">**Cenário E** – todos os Publicadores estrangeiros (conforme definido por suas informações de perfil de impostos do Partner Center) em países com um Tratado dos EUA fazendo uma venda para um cliente baseado nos EUA (conforme definido pelo endereço de sua conta de cliente).</span><span class="sxs-lookup"><span data-stu-id="24cff-136">**Scenario E** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries with a US treaty making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="24cff-137">O governo dos EUA não exige que a Microsoft reponha impostos em nome do Publicador.</span><span class="sxs-lookup"><span data-stu-id="24cff-137">US government does not require Microsoft to withhold tax on behalf of the publisher.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Mostra o fluxo de trabalho para o cenário do processo de pagamento E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a><span data-ttu-id="24cff-139">O Publicador estrangeiro vende para um cliente registrado por IVA da UE em um país gerenciado pela Microsoft (fora da Irlanda)</span><span class="sxs-lookup"><span data-stu-id="24cff-139">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (outside Ireland)</span></span>

<span data-ttu-id="24cff-140">**Cenário F** – todas as transações entre Publicadores estrangeiros e clientes registrados no IVA da UE (fora da Irlanda) em um país Microsoft-Managed.</span><span class="sxs-lookup"><span data-stu-id="24cff-140">**Scenario F** – All transactions between foreign publishers and EU VAT-registered customers (outside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="24cff-141">O cliente não paga o imposto sobre a venda.</span><span class="sxs-lookup"><span data-stu-id="24cff-141">The customer does not pay tax on the sale.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Mostra o fluxo de trabalho para o cenário do processo de pagamento F.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a><span data-ttu-id="24cff-143">O Publicador estrangeiro vende para um cliente registrado por IVA da UE em um país gerenciado pela Microsoft (na Irlanda)</span><span class="sxs-lookup"><span data-stu-id="24cff-143">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (in Ireland)</span></span>

<span data-ttu-id="24cff-144">**Cenário G** – todas as transações entre Publicadores estrangeiros e clientes registrados no IVA da UE (dentro da Irlanda) em um país Microsoft-Managed.</span><span class="sxs-lookup"><span data-stu-id="24cff-144">**Scenario G** – All transactions between foreign publishers and EU VAT-registered customers (inside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="24cff-145">O cliente paga o IVA da irlandês e a Microsoft paga esse imposto ao governo da irlandês.</span><span class="sxs-lookup"><span data-stu-id="24cff-145">The customer pays Irish VAT and Microsoft pays this tax to the Irish government.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Mostra o fluxo de trabalho para o cenário de processo de pagamento G.":::

## <a name="next-steps"></a><span data-ttu-id="24cff-147">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="24cff-147">Next steps</span></span>

- [<span data-ttu-id="24cff-148">Perguntas frequentes do Publicador</span><span class="sxs-lookup"><span data-stu-id="24cff-148">Publisher FAQ</span></span>](https://docs.microsoft.com/azure/marketplace/marketplace-faq-publisher-guide)
- [<span data-ttu-id="24cff-149">Instruções para criar perfis de pagamento e de impostos</span><span class="sxs-lookup"><span data-stu-id="24cff-149">Instructions to create payment and tax profiles</span></span>](https://docs.microsoft.com/partner-center/set-up-your-payout-account?context=/azure/marketplace/context/context#create-a-payment-profile)
