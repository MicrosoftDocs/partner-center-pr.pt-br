---
title: Como o crédito ganho do parceiro é calculado | Centro de parceiros
ms.topic: article
ms.date: 09/17/2019
description: Como o aspecto de crédito obtido pelo parceiro do Azure Plan é calculado
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: eb0dd5ef22632a85ca0227cc9e988a88263e9ddf
ms.sourcegitcommit: 0195355f4526362f4d89f59ea643a5e422b6a9b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/27/2019
ms.locfileid: "71318775"
---
# <a name="how-the-partner-earned-credit-pec-is-calculated"></a><span data-ttu-id="620cf-103">Como o PEC (crédito ganho) do parceiro é calculado</span><span class="sxs-lookup"><span data-stu-id="620cf-103">How the partner earned credit (PEC) is calculated</span></span>


<span data-ttu-id="620cf-104">Os parceiros que possuem o gerenciamento de operações de ti 24x7 de partes ou todo o ambiente do Azure de seus clientes no CSP são recompensados com o PEC.</span><span class="sxs-lookup"><span data-stu-id="620cf-104">Partners who own the 24x7 IT operations management of parts or the entire Azure environment of their customers in CSP are rewarded with PEC.</span></span> <span data-ttu-id="620cf-105">O PEC é fornecido como parte da fatura para o parceiro que tem uma relação de cobrança direta com a Microsoft.</span><span class="sxs-lookup"><span data-stu-id="620cf-105">The PEC is provided as part of the invoice to the partner who has a direct billing relationship with Microsoft.</span></span> <span data-ttu-id="620cf-106">O crédito é calculado diariamente e refletido na nota fiscal mensal.</span><span class="sxs-lookup"><span data-stu-id="620cf-106">The credit is calculated daily and reflected in the monthly invoice.</span></span> <span data-ttu-id="620cf-107">Por padrão, no CSP, os parceiros recebem os direitos de acesso necessários à assinatura do cliente que permite que eles tenham gerenciamento de operações 24X7 e controle dos recursos na assinatura.</span><span class="sxs-lookup"><span data-stu-id="620cf-107">By default, in CSP, partners are granted the necessary access rights to the customer’s subscription that allows them to have 24X7 operations management and control of the resources on the subscription.</span></span> <span data-ttu-id="620cf-108">As maneiras adicionais pelas quais o cliente pode provisionar o acesso para o parceiro de transformação são descritas na seção a seguir.</span><span class="sxs-lookup"><span data-stu-id="620cf-108">Additional ways in which customer can provision access for transacting partner are described in the following section.</span></span>   


## <a name="important-eligibility-and-calculation-requirements"></a><span data-ttu-id="620cf-109">Requisitos importantes de elegibilidade e de cálculo:</span><span class="sxs-lookup"><span data-stu-id="620cf-109">Important eligibility and calculation requirements:</span></span>

- <span data-ttu-id="620cf-110">Um parceiro deve ter um contrato MPN ativo e uma função de conta C (RBAC) válida baseada em regras para receber crédito acumulado para os ativos do Azure que eles gerenciam.</span><span class="sxs-lookup"><span data-stu-id="620cf-110">A partner should have an active MPN agreement and a valid Rules Based Account C (RBAC) role to receive earned credit for the azure assets they manage.</span></span> <span data-ttu-id="620cf-111">Saiba mais sobre [funções RBAC válidas]</span><span class="sxs-lookup"><span data-stu-id="620cf-111">Learn more about [valid RBAC roles]</span></span>

- <span data-ttu-id="620cf-112">O provedor indireto será elegível para o PEC se ele ou seu revendedor indireto tiver um controle operacional e o gerenciamento operacionais 24x7 dos recursos do Azure do cliente no CSP.</span><span class="sxs-lookup"><span data-stu-id="620cf-112">The indirect provider will be eligible for PEC if either they or their indirect reseller or both have 24x7 operational control and management of the customer’s Azure resources in CSP.</span></span>

- <span data-ttu-id="620cf-113">O PEC está associado ao consumo cobrado (passível de cobrança) do espaço do Azure do cliente no CSP gerenciado pelo parceiro.</span><span class="sxs-lookup"><span data-stu-id="620cf-113">PEC is associated to billed (chargeable) consumption of customer’s Azure estate in CSP managed by the partner.</span></span> 

- <span data-ttu-id="620cf-114">O PEC está disponível somente para parceiros no CSP que são cobrados pela Microsoft (provedor indireto e parceiro de cobrança direta).</span><span class="sxs-lookup"><span data-stu-id="620cf-114">PEC is available only to partners in CSP who are billed by Microsoft (indirect provider and direct bill partner).</span></span>

- <span data-ttu-id="620cf-115">Serviços qualificados: o crédito ganho do parceiro é aplicável a todos os consumos do Azure 1PP do Azure fornecidos na lista de preços.</span><span class="sxs-lookup"><span data-stu-id="620cf-115">Eligible Services: Partner earned credit is applicable to all Azure 1PP Azure consumption given on the price list.</span></span> <span data-ttu-id="620cf-116">Há exceções que incluem, mas não se limitando a, 3PP e reservas do Azure.</span><span class="sxs-lookup"><span data-stu-id="620cf-116">There are exceptions including, but not limited to, 3PP and Azure Reservations.</span></span>

- <span data-ttu-id="620cf-117">O PEC é calculado diariamente e pode ser exibido no arquivo reconhecimento diário.</span><span class="sxs-lookup"><span data-stu-id="620cf-117">PEC is calculated daily and can be viewed in the daily recon file.</span></span> <span data-ttu-id="620cf-118">Um parceiro (provedor ou revendedor (por meio de seu provedor) deve ter acesso ao dia inteiro (24x7) para garantir que eles ganhem o PEC.</span><span class="sxs-lookup"><span data-stu-id="620cf-118">A partner (provider or reseller (through their provider) must have access for the entire day (24x7) to ensure they earn PEC.</span></span>

- <span data-ttu-id="620cf-119">O PEC é obtido para o nível de recurso do Azure.</span><span class="sxs-lookup"><span data-stu-id="620cf-119">PEC is earned down to the Azure resource level.</span></span> <span data-ttu-id="620cf-120">Se o parceiro tiver acesso válido na assinatura ou no nível do grupo de recursos, cada recurso que role para a entidade mais alta receberá o PEC.</span><span class="sxs-lookup"><span data-stu-id="620cf-120">If the partner has valid access at the subscription, or resource group level, each resource that role up to the higher entity will earn PEC.</span></span> 

- <span data-ttu-id="620cf-121">O PEC será incluído na nota fiscal mensal do parceiro.</span><span class="sxs-lookup"><span data-stu-id="620cf-121">PEC will be included on the partner's monthly invoice.</span></span> <span data-ttu-id="620cf-122">A nota fiscal é uma rede de encargos.</span><span class="sxs-lookup"><span data-stu-id="620cf-122">The invoice is net of charges.</span></span> <span data-ttu-id="620cf-123">Os detalhes são mostrados no arquivo reconhecimento da nota fiscal.</span><span class="sxs-lookup"><span data-stu-id="620cf-123">The details are shown in the invoice recon file.</span></span>

<span data-ttu-id="620cf-124">Para obter informações sobre como obter acesso para gerenciar assinaturas do Azure e sobre como vincular sua ID do MPN a funções de RBAC, leia [gerenciar assinaturas e recursos no plano do Azure](azure-plan-manage.md).</span><span class="sxs-lookup"><span data-stu-id="620cf-124">For information on gaining access to manage Azure subscriptions and on how to link your MPN ID to RBAC roles, read [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md).</span></span>

<span data-ttu-id="620cf-125">Para obter mais informações</span><span class="sxs-lookup"><span data-stu-id="620cf-125">For more information</span></span>

- [<span data-ttu-id="620cf-126">Plano do Azure – cobrança</span><span class="sxs-lookup"><span data-stu-id="620cf-126">Azure plan - billing</span></span>](azure-plan-billing.md)

- [<span data-ttu-id="620cf-127">Lista de preços para a nova experiência de comércio no CSP</span><span class="sxs-lookup"><span data-stu-id="620cf-127">Price list for the new commerce experience in CSP </span></span>](azure-plan-price-list.md)