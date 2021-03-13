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
# <a name="transfer-eligibility-for-a-subscription-between-billing-accounts"></a>Qualificação de transferência para uma assinatura entre contas de cobrança

Você pode [transferir uma assinatura](/azure/cost-management-billing/understand/subscription-transfer) de uma conta de cobrança para outra na seção de cobrança do portal do Azure. Antes de uma transferência, a assinatura é verificada para produtos de terceiros. A transferência será permitida somente se *todos os* produtos forem limpos para transferência (consulte os [critérios](#criteria-for-transfer-approval-or-denial) abaixo). O sistema irá gerar mensagens de erro relevantes para os aplicativos que não puderam ser desmarcados para ajudá-lo a determinar as próximas etapas.

> [!NOTE]
> Este artigo não se aplica a ofertas de SaaS porque os recursos de SaaS são anexados a um locatário, não a uma assinatura. Os recursos de SaaS podem ser transferidos de uma conta de cobrança para outra, mas isso é feito por recurso e pelo suporte do Azure como uma solicitação de suporte.

## <a name="criteria-for-transfer-approval-or-denial"></a>Critérios para aprovação de transferência ou negação

Você não poderá transferir uma assinatura se algum de seus aplicativos de terceiros atender a qualquer um dos seguintes critérios:

- A conta de destino é comercial e o aplicativo é recusado para ser vendido por meio de parceiros.
- O aplicativo é opcional para os parceiros selecionados e a conta de destino não está na lista de permissões.
- A oferta foi uma oferta de visualização no passado para assinaturas selecionadas ou era uma oferta privada e a assinatura não está mais na lista de permissões.
- A nova conta de cobrança está em uma região diferente de onde a oferta é vendida e a oferta não é vendida nessa região.

Uma transferência bloqueada permanece em vigor até que você remova o recurso da assinatura, após o qual você pode tentar a transferência novamente.

## <a name="next-steps"></a>Próximas etapas

[Obtenha suporte para Microsoft AppSource e Azure Marketplace](get-support.md)

