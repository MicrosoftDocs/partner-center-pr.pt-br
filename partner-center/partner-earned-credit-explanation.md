---
title: Crédito ganho pelo parceiro para serviços gerenciados
ms.topic: article
ms.date: 12/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como o PEC (crédito ganho pelo parceiro) da Microsoft para serviços gerenciados é calculado e pago, além de como garantir que você esteja qualificado.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 022e7aabd0d850660f8236dce9a4fab9069af01b
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "106087120"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a><span data-ttu-id="2cade-103">Como o crédito ganho pelo parceiro é calculado e pago</span><span class="sxs-lookup"><span data-stu-id="2cade-103">How the partner earned credit is calculated and paid</span></span>

<span data-ttu-id="2cade-104">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="2cade-104">**Appropriate roles**</span></span>

- <span data-ttu-id="2cade-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="2cade-105">Global admin</span></span>
- <span data-ttu-id="2cade-106">Administrador de gerenciamento de usuário</span><span class="sxs-lookup"><span data-stu-id="2cade-106">User management admin</span></span>
- <span data-ttu-id="2cade-107">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="2cade-107">Admin agent</span></span>
- <span data-ttu-id="2cade-108">Administrador de cobrança</span><span class="sxs-lookup"><span data-stu-id="2cade-108">Billing admin</span></span>
- <span data-ttu-id="2cade-109">Agente de vendas</span><span class="sxs-lookup"><span data-stu-id="2cade-109">Sales agent</span></span>

<span data-ttu-id="2cade-110">O PEC (crédito ganho pelo parceiro para serviços gerenciados) reconhece e recompensa os parceiros que têm o controle operacional de TI 24x7 e o gerenciamento de partes – ou da totalidade – do ambiente do Azure de seus clientes.</span><span class="sxs-lookup"><span data-stu-id="2cade-110">Partner earned credit for managed services (PEC) recognizes and rewards partners that own the 24x7 IT operational control and management of parts of, or the entire, Azure environment of their customers.</span></span> <span data-ttu-id="2cade-111">Por padrão, no CSP, os parceiros recebem os direitos de acesso necessários à assinatura do cliente, permitindo que eles executem o gerenciamento operacional 24x7 e o controle dos recursos na assinatura.</span><span class="sxs-lookup"><span data-stu-id="2cade-111">By default, in CSP, partners are granted the necessary access rights to the customer's subscription allowing them to perform 24 X 7 operational management and control of the resources on the subscription.</span></span> <span data-ttu-id="2cade-112">Outras maneiras pelas quais o cliente pode provisionar acesso aos parceiros das transações estão descritas na seção a seguir.</span><span class="sxs-lookup"><span data-stu-id="2cade-112">Other ways in which customers can provision access for transacting partners is described in the following section.</span></span> <span data-ttu-id="2cade-113">O valor da fatura mensal é o valor líquido do crédito obtido por parceiro.</span><span class="sxs-lookup"><span data-stu-id="2cade-113">The monthly invoice amount is the net of the partner earned credit.</span></span> <span data-ttu-id="2cade-114">Os parceiros podem ver os detalhes do PEC em seu arquivo de reconhecimento mensal.</span><span class="sxs-lookup"><span data-stu-id="2cade-114">Partners can see the PEC details on their monthly recon file.</span></span> <span data-ttu-id="2cade-115">Para ver outras maneiras pelas quais um cliente pode provisionar acesso ao parceiro de transações, leia [Gerenciar assinaturas e recursos no âmbito do plano do Azure](azure-plan-manage.md).</span><span class="sxs-lookup"><span data-stu-id="2cade-115">For additional ways in which a customer can provision access for the transacting partner, read [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md).</span></span>

<span data-ttu-id="2cade-116">Leia também [Restabelecer privilégios de administrador para assinaturas do Azure CSP](revoke-reinstate-csp.md)</span><span class="sxs-lookup"><span data-stu-id="2cade-116">Also read [Reinstate admin privileges for Azure CSP subscriptions](revoke-reinstate-csp.md)</span></span>

## <a name="eligibility"></a><span data-ttu-id="2cade-117">Qualificação</span><span class="sxs-lookup"><span data-stu-id="2cade-117">Eligibility</span></span>

<span data-ttu-id="2cade-118">Para receber o PEC (crédito obtido por parceiro), os seguintes requisitos se aplicam:</span><span class="sxs-lookup"><span data-stu-id="2cade-118">In order to receive the partner earned credit (PEC), the following requirements apply:</span></span> 

- <span data-ttu-id="2cade-119">Você precisa ter um contrato de MPN ativo e uma função RBAC (controle de acesso baseado em função) válida para receber o crédito obtido dos ativos do Azure gerenciados por você.</span><span class="sxs-lookup"><span data-stu-id="2cade-119">You must have an active MPN agreement and valid role-based access control (RBAC) role to receive earned credit for the Azure assets you manage.</span></span>

- <span data-ttu-id="2cade-120">Você precisa ter o controle operacional e o gerenciamento 24 horas por dia, 7 dias por semana dos recursos do Azure do cliente no CSP.</span><span class="sxs-lookup"><span data-stu-id="2cade-120">You must have 24x7 operational control and management of the customer's Azure resources in CSP.</span></span> <span data-ttu-id="2cade-121">Isso significa que você precisa ter privilégios de administrador na assinatura do Azure do cliente, no grupo de recursos do Azure e no recurso do Azure.</span><span class="sxs-lookup"><span data-stu-id="2cade-121">This means you must have admin privileges on the customer’s Azure subscription, Azure resource group, Azure resource.</span></span> <span data-ttu-id="2cade-122">No caso dos provedores indiretos e dos respectivos revendedores indiretos, o provedor indireto será qualificado para o PEC se ele ou o revendedor indireto ou ambos tiverem esse controle operacional.</span><span class="sxs-lookup"><span data-stu-id="2cade-122">In the case of indirect providers and their indirect resellers, the indirect provider will be eligible for PEC if either the indirect provider or the indirect reseller or both have this operational control.</span></span> <span data-ttu-id="2cade-123">Para saber mais sobre isso, confira [Restabelecer privilégios de administrador para assinaturas do CSP do Azure](./revoke-reinstate-csp.md).</span><span class="sxs-lookup"><span data-stu-id="2cade-123">To learn more about this, see [Reinstate admin privileges for Azure CSP subscriptions](./revoke-reinstate-csp.md).</span></span>

- <span data-ttu-id="2cade-124">Além dos requisitos acima, o PEC só é aplicável aos serviços listados no preço de consumo do plano do Azure, que pode ser exportado da página [Preços do plano do Azure](https://partner.microsoft.com/commerce/sales).</span><span class="sxs-lookup"><span data-stu-id="2cade-124">In addition to the requirements above, PEC is only applicable to services listed in the Azure plan consumption pricing, which you can export from the [Azure plan pricing](https://partner.microsoft.com/commerce/sales) page.</span></span>

- <span data-ttu-id="2cade-125">O PEC **não** é aplicável aos seguintes serviços:</span><span class="sxs-lookup"><span data-stu-id="2cade-125">PEC is **not** applicable to the following services:</span></span>
    - <span data-ttu-id="2cade-126">Reservas do plano do Azure</span><span class="sxs-lookup"><span data-stu-id="2cade-126">Azure Plan reservations</span></span>
    - <span data-ttu-id="2cade-127">Produtos de terceiros identificados como Terceiros na coluna Marcas do preço de consumo do plano do Azure</span><span class="sxs-lookup"><span data-stu-id="2cade-127">Third-party products identified as Third Party in the Tags column of the Azure plan consumption price</span></span>
    - <span data-ttu-id="2cade-128">Produtos da lista de preços do Marketplace</span><span class="sxs-lookup"><span data-stu-id="2cade-128">Products in the Marketplace price list</span></span>
    - [<span data-ttu-id="2cade-129">Máquinas Virtuais Spot do Azure</span><span class="sxs-lookup"><span data-stu-id="2cade-129">Azure Spot Virtual Machines</span></span>](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

- <span data-ttu-id="2cade-130">O PEC é obtido no nível de recurso do Azure.</span><span class="sxs-lookup"><span data-stu-id="2cade-130">PEC is earned down to the Azure resource level.</span></span> <span data-ttu-id="2cade-131">Se você tiver acesso válido no nível da assinatura ou do grupo de recursos, todos os recursos acumulados até a entidade mais alta receberão o PEC.</span><span class="sxs-lookup"><span data-stu-id="2cade-131">If you have valid access at either the subscription or resource group level, each resource that rolls up to the higher entity will earn PEC.</span></span>

- <span data-ttu-id="2cade-132">Mais detalhes sobre o PEC também estão disponíveis na página [Gerenciamento de Custos do Azure](/azure/cost-management-billing/costs/get-started-partners).</span><span class="sxs-lookup"><span data-stu-id="2cade-132">Details on PEC are also available on the [Azure Cost management](/azure/cost-management-billing/costs/get-started-partners) page.</span></span>

### <a name="calculation"></a><span data-ttu-id="2cade-133">Cálculo</span><span class="sxs-lookup"><span data-stu-id="2cade-133">Calculation</span></span>

<span data-ttu-id="2cade-134">O PEC é calculado diariamente e pode ser exibido no arquivo de uso diário e no arquivo reconhecimento de fatura mensal.</span><span class="sxs-lookup"><span data-stu-id="2cade-134">PEC is calculated daily and can be viewed in the daily usage file and monthly invoice recon file.</span></span> <span data-ttu-id="2cade-135">Um parceiro (provedor indireto ou revendedor indireto) deve ter acesso ao dia inteiro (24x7) para garantir que eles obtenham o PEC.</span><span class="sxs-lookup"><span data-stu-id="2cade-135">A partner (indirect provider or indirect reseller) must have access for the entire day (24x7) to ensure they earn PEC.</span></span> <span data-ttu-id="2cade-136">O PEC é calculado diariamente nos ativos gerenciados do Azure.</span><span class="sxs-lookup"><span data-stu-id="2cade-136">PEC is calculated on a daily basis on the managed Azure assets.</span></span> <span data-ttu-id="2cade-137">Os parceiros que retêm o acesso privilegiado persistente durante o mês (período de acesso) e para todos os recursos qualificados (escopo de acesso) ganharão o PEC completo.</span><span class="sxs-lookup"><span data-stu-id="2cade-137">Partners retaining persistent privileged access through the month (span of access) and for all the eligible resources (scope of access) will earn full PEC.</span></span> <span data-ttu-id="2cade-138">A redução de escopo e período resultará em uma taxa menor de PEC para o mês.</span><span class="sxs-lookup"><span data-stu-id="2cade-138">Scope and span reduction will result in lower PEC rate for the month.</span></span> <span data-ttu-id="2cade-139">O arquivo de uso com classificação diária é mostrado diariamente em um ativo do Azure, independentemente de o PEC ser aplicado ou não.</span><span class="sxs-lookup"><span data-stu-id="2cade-139">Daily rated usage file shows on a daily basis on an Azure asset, whether PEC is applied or not.</span></span> <span data-ttu-id="2cade-140">Os parceiros também podem se registrar para receber alertas e monitorar se há alterações no acesso privilegiado persistente.</span><span class="sxs-lookup"><span data-stu-id="2cade-140">Partners can also enroll in alerts to monitor changes to persistent privileged access.</span></span>

## <a name="azure-cost-management"></a><span data-ttu-id="2cade-141">Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="2cade-141">Azure Cost Management</span></span>

<span data-ttu-id="2cade-142">O ACM (Gerenciamento de Custos do Azure), pelo uso da análise de custos, permite que você, na condição de parceiro, exiba os custos que receberam o benefício do PEC.</span><span class="sxs-lookup"><span data-stu-id="2cade-142">Azure Cost Management (ACM) using Cost Analysis enables you as a partner to view the costs that have received the benefit of PEC.</span></span>  

1. <span data-ttu-id="2cade-143">No [portal do Azure](https://portal.azure.com), entre no locatário do parceiro e selecione **Cobrança + Gerenciamento de Custos**.</span><span class="sxs-lookup"><span data-stu-id="2cade-143">In the [Azure portal](https://portal.azure.com), sign into your partner tenant and select **Cost Management + Billing**.</span></span>

2. <span data-ttu-id="2cade-144">Selecione **Gerenciamento de custos**</span><span class="sxs-lookup"><span data-stu-id="2cade-144">Select **Cost management**</span></span>

3. <span data-ttu-id="2cade-145">Selecione **Análise de Custo**</span><span class="sxs-lookup"><span data-stu-id="2cade-145">Select **Cost Analysis**</span></span>

   <span data-ttu-id="2cade-146">A exibição de Análise de Custo exibirá os custos da sua conta de cobrança para todos os serviços comprados e consumidos segundo os preços que você paga à Microsoft.</span><span class="sxs-lookup"><span data-stu-id="2cade-146">The Cost Analysis view will display the costs for your billing account, for all the services purchased and consumed at the prices that you pay Microsoft.</span></span>

4. <span data-ttu-id="2cade-147">Selecione **PartnerEarnedCreditApplied** na lista suspensa em um gráfico dinâmico para ver os custos que têm o PEC aplicado.</span><span class="sxs-lookup"><span data-stu-id="2cade-147">Select **PartnerEarnedCreditApplied** in the drop-down list on a pivot chart to see costs that have PEC applied.</span></span> <span data-ttu-id="2cade-148">Quando a propriedade **PartnerEarnedCreditApplied** é True, o custo associado tem o benefício do crédito ganho do parceiro.</span><span class="sxs-lookup"><span data-stu-id="2cade-148">When **PartnerEarnedCreditApplied** property is True, the associated cost has the benefit of the partner earned credit.</span></span> 

   <span data-ttu-id="2cade-149">Quando a propriedade PartnerEarnedCreditApplied é False, o custo associado não atendeu à qualificação necessária para o crédito ou o serviço comprado não é elegível para crédito ganho do parceiro.</span><span class="sxs-lookup"><span data-stu-id="2cade-149">When the PartnerEarnedCreditApplied property is False, the associated cost has not met the required eligibility for the credit or the service purchased is not eligible for partner earned credit.</span></span>

   >[!NOTE] 
   ><span data-ttu-id="2cade-150">Normalmente, o uso de serviços leva de 8 a 24 horas para aparecer no **Gerenciamento de Custos**, e os créditos do PEC aparecerão dentro de 48 horas a partir da hora de acesso no Gerenciamento de Custos do Azure.</span><span class="sxs-lookup"><span data-stu-id="2cade-150">Typically, usage for services takes 8-24 hours to appear in **Cost Management** and the PEC credits will appear within 48 hours from time of access in Azure Cost Management.</span></span>

5. <span data-ttu-id="2cade-151">Você também pode agrupar pela propriedade **PartnerEarnedCreditApplied** e filtrar por ela, usando os recursos de filtro **Agrupar por e Adicionar** para analisar os custos que têm o PEC aplicado e os custos que não têm nenhum PEC aplicado.</span><span class="sxs-lookup"><span data-stu-id="2cade-151">You can also group by, and filter by, the **PartnerEarnedCreditApplied** property using the **Group by and Add** filter features to drill into costs that have PEC and the costs that have no PEC applied.</span></span>

## <a name="next-steps"></a><span data-ttu-id="2cade-152">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="2cade-152">Next steps</span></span>

- [<span data-ttu-id="2cade-153">Crédito ganho pelo parceiro – visão geral</span><span class="sxs-lookup"><span data-stu-id="2cade-153">Partner earned credit - overview</span></span>](partner-earned-credit.md)

- <span data-ttu-id="2cade-154">Exemplos detalhados do cálculo do crédito obtido por parceiro estão localizados na lista de preços que você pode acessar por meio do Painel do Partner Center (requer credenciais).</span><span class="sxs-lookup"><span data-stu-id="2cade-154">Detailed examples of partner earned credit calculations are located on the price list that you can reach through the Partner Center dashboard (sign in required).</span></span>

- [<span data-ttu-id="2cade-155">Migrar para o plano do Azure – introdução</span><span class="sxs-lookup"><span data-stu-id="2cade-155">Move to Azure plan - get started</span></span>](azure-plan-get-started.md)

- [<span data-ttu-id="2cade-156">Gerenciar assinaturas e recursos no âmbito do plano do Azure</span><span class="sxs-lookup"><span data-stu-id="2cade-156">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)

- [<span data-ttu-id="2cade-157">Revogar ou restabelecer privilégios de administrador para assinaturas do CSP do Azure</span><span class="sxs-lookup"><span data-stu-id="2cade-157">Revoke or reinstate admin privileges for Azure CSP subscriptions</span></span>](revoke-reinstate-csp.md)
