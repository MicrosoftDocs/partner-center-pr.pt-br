---
title: Qualificação de transferência – diretrizes para transferir uma assinatura entre contas de cobrança, Azure Marketplace
description: Diretrizes para verificações comerciais antes de transferir uma assinatura entre contas de cobrança no portal do Azure.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: 4b235bd462915fc205813ae86e92f98b4fd49fe4
ms.sourcegitcommit: 3a2415ab9833d5c574ad76d462f526a131c24f33
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "103412549"
---
# <a name="transfer-eligibility-for-a-subscription-between-billing-accounts"></a><span data-ttu-id="8095b-103">Qualificação de transferência para uma assinatura entre contas de cobrança</span><span class="sxs-lookup"><span data-stu-id="8095b-103">Transfer eligibility for a subscription between billing accounts</span></span>

<span data-ttu-id="8095b-104">Você pode [transferir uma assinatura](/azure/cost-management-billing/understand/subscription-transfer) de uma conta de cobrança para outra na seção de cobrança do portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="8095b-104">You can [transfer a subscription](/azure/cost-management-billing/understand/subscription-transfer) from one billing account to another in the billing section of the Azure portal.</span></span> <span data-ttu-id="8095b-105">Antes de uma transferência, a assinatura é verificada para produtos de terceiros.</span><span class="sxs-lookup"><span data-stu-id="8095b-105">Prior to a transfer, the subscription is scanned for third-party products.</span></span> <span data-ttu-id="8095b-106">A transferência será permitida somente se *todos os* produtos forem limpos para transferência (consulte os [critérios](#criteria-for-transfer-approval-or-denial) abaixo).</span><span class="sxs-lookup"><span data-stu-id="8095b-106">The transfer is permitted only if *all* products are cleared for transfer (see the [criteria](#criteria-for-transfer-approval-or-denial) below).</span></span> <span data-ttu-id="8095b-107">O sistema irá gerar mensagens de erro relevantes para os aplicativos que não puderam ser desmarcados para ajudá-lo a determinar as próximas etapas.</span><span class="sxs-lookup"><span data-stu-id="8095b-107">The system will generate relevant error messages for the apps that failed to clear to help you determine next steps.</span></span>

> [!NOTE]
> <span data-ttu-id="8095b-108">Este artigo não se aplica a ofertas de SaaS porque os recursos de SaaS são anexados a um locatário, não a uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="8095b-108">This article does not apply to SaaS offers because SaaS resources are attached to a tenant, not a subscription.</span></span> <span data-ttu-id="8095b-109">Os recursos de SaaS podem ser transferidos de uma conta de cobrança para outra, mas isso é feito por recurso e pelo suporte do Azure como uma solicitação de suporte.</span><span class="sxs-lookup"><span data-stu-id="8095b-109">SaaS resources are transferable from one billing account to another, but this is done per resource and by Azure support as a support request.</span></span>

## <a name="criteria-for-transfer-approval-or-denial"></a><span data-ttu-id="8095b-110">Critérios para aprovação de transferência ou negação</span><span class="sxs-lookup"><span data-stu-id="8095b-110">Criteria for transfer approval or denial</span></span>

<span data-ttu-id="8095b-111">Você não poderá transferir uma assinatura se algum de seus aplicativos de terceiros atender a qualquer um dos seguintes critérios:</span><span class="sxs-lookup"><span data-stu-id="8095b-111">You cannot transfer a subscription if any of its third-party apps meet any of the following criteria:</span></span>

- <span data-ttu-id="8095b-112">A conta de destino é comercial e o aplicativo é recusado para ser vendido por meio de parceiros.</span><span class="sxs-lookup"><span data-stu-id="8095b-112">The target account is commercial and the app is opt-out to be sold via partners.</span></span>
- <span data-ttu-id="8095b-113">O aplicativo é opcional para os parceiros selecionados e a conta de destino não está na lista de permissões.</span><span class="sxs-lookup"><span data-stu-id="8095b-113">The app is opt-in for selected partners and the target account is not in the allow list.</span></span>
- <span data-ttu-id="8095b-114">A oferta foi uma oferta de visualização no passado para assinaturas selecionadas ou era uma oferta privada e a assinatura não está mais na lista de permissões.</span><span class="sxs-lookup"><span data-stu-id="8095b-114">The offer was a preview offer in the past for selected subscriptions or was a private offer and the subscription is no longer in the allow list.</span></span>
- <span data-ttu-id="8095b-115">A nova conta de cobrança está em uma região diferente de onde a oferta é vendida e a oferta não é vendida nessa região.</span><span class="sxs-lookup"><span data-stu-id="8095b-115">The new billing account is in a region different from where the offer is sold AND the offer is not to be sold in that region.</span></span>

<span data-ttu-id="8095b-116">Uma transferência bloqueada permanece em vigor até que você remova o recurso da assinatura, após o qual você pode tentar a transferência novamente.</span><span class="sxs-lookup"><span data-stu-id="8095b-116">A blocked transfer remains in effect until you remove the resource from the subscription, after which you can try the transfer again.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8095b-117">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="8095b-117">Next steps</span></span>

[<span data-ttu-id="8095b-118">Obtenha suporte para Microsoft AppSource e Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="8095b-118">Get support for Microsoft AppSource and Azure Marketplace</span></span>](get-support.md)

