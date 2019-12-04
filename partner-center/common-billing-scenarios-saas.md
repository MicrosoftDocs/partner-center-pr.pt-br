---
title: Cenários de cobrança comuns para transações SaaS baseadas em licença | Centro de parceiros
ms.topic: article
ms.date: 11/25/2019
description: Saiba mais sobre cenários de cobrança comuns no Partner Center para transações de SaaS baseadas em licença.
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
Keywords: cobrança, pagamentos, compra única, compra recorrente, assinaturas, estações
ms.localizationpriority: medium
ms.openlocfilehash: 5d86210ce52280b73846de56dafb5909081b6524
ms.sourcegitcommit: c793c1b61f50fc0b0a12c95cedd9f57b31703093
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2019
ms.locfileid: "74722515"
---
# <a name="billing-scenarios-for-license-based-saas-transactions"></a>Cenários de cobrança para transações SaaS baseadas em licença

**Funções apropriadas**

- Agente administrativo
- Administrador de cobrança
- Agente de suporte técnico
- Agente de vendas


Esses [cenários de cobrança comuns](common-billing-scenarios.md) de exemplo são aplicáveis a assinaturas SaaS (software como serviço) baseadas em licença no Partner Center.

## <a name="convert-a-free-trial-saas-subscription-to-a-paid-subscription"></a>Converter uma assinatura SaaS de avaliação gratuita em uma assinatura paga

Este cenário descreve a cobrança para a renovação de uma assinatura SaaS de avaliação gratuita baseada em licença. A renovação converte a avaliação gratuita em uma assinatura paga no final do período de avaliação gratuita.

Neste exemplo, você comprou uma avaliação gratuita de uma assinatura SaaS (software como serviço) baseada em licença em 10 de junho. Essa avaliação gratuita é renovada automaticamente como uma assinatura paga quando o período de avaliação gratuita termina.

Os arquivos reconhecimento incluirão os seguintes encargos:

| Data de compra | Data de início do encargo | Data de término do encargo | Preço unitário | Quantidade de unidades | Valor total | Tipo de cobrança | Descrição da assinatura |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | US$ 0 | 1 | US$ 0 | Novo | Avaliação gratuita |
| 07/10/2019 | 07/10/2019 | 08/09/2019 | US$ 2 | 1 | US$ 2 | Renovar | Assinatura paga |

## <a name="cancel-a-free-trial-saas-subscription"></a>Cancelar uma assinatura de SaaS de avaliação gratuita

> [!TIP]
> Você pode cancelar uma assinatura SaaS de avaliação gratuita baseada em licença a qualquer momento, mesmo durante o período de avaliação gratuita.

Nesse cenário, você comprou uma assinatura SaaS de avaliação gratuita baseada em licença em 1º de julho e, em seguida, a cancelou imediatamente no Partner Center.

O arquivo reconhecimento incluirá os seguintes encargos:

| Data de compra | Data de início do encargo | Data de término do encargo | Preço unitário | Quantidade de unidades | Valor total | Tipo de cobrança | Descrição da assinatura |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | US$ 0 | 11 | US$ 0 | Novo | Avaliação gratuita |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | US$ 0 | 11 | US$ 0 | Cancelar | Avaliação gratuita |

## <a name="convert-custom-meter-saas-subscription-to-another-sku"></a>Converter a assinatura SaaS do medidor personalizado em outra SKU

Este cenário descreve como converter uma assinatura de SaaS de medidor personalizado de uma SKU (unidade de manutenção de estoque) para outra SKU para o mesmo produto, na mesma data.

Nesse cenário, você comprou um SKU (prata) em um produto e o converteu em outro SKU (bronze) disponível sob este produto na mesma data.

O arquivo reconhecimento incluirá os seguintes encargos:

| Data de compra | Data de início do encargo | Data de término do encargo | Preço unitário | Quantidade de unidades | Valor total | Tipo de cobrança | Descrição da assinatura |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | Prata | 06/10/2019 | 06/10/2019 | US$ 20 | 1 | US$ 20 | Novo | Assinatura de SaaS do medidor personalizado |
| 06/10/2019 | Prata | 06/10/2019 | 06/10/2019 | US$ 20 | 1 | -$20 | Converter | Fatura rateada para assinatura de SaaS de medidor personalizado |
| 06/10/2019 | Bronze | 06/10/2019 | 06/10/2019 | US$ 10 | 1 | US$ 10 | Converter | Assinatura de SaaS do medidor personalizado |

## <a name="purchase-and-cancel-a-customer-meter-saas-subscription-on-same-date"></a>Comprar e cancelar uma assinatura de SaaS do medidor do cliente na mesma data

Este cenário descreve a cobrança de uma assinatura de SaaS do medidor do cliente que você comprou e cancelou por meio do portal do Azure na mesma data.

Nesse cenário, você comprou uma assinatura de SaaS de medidor personalizado no portal do Azure. Em seguida, você cancelou a assinatura na mesma data.

| Data de compra | Data de início do encargo | Data de término do encargo | Preço unitário | Quantidade de unidades | Valor total | Tipo de cobrança | Descrição da assinatura |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | Bronze | 06/10/2019 | 06/10/2019 | US$ 10 | 1 | US$ 10 | Novo | Assinatura de SaaS do medidor personalizado |
| 06/10/2019 | Bronze | 06/10/2019 | 06/10/2019 | US$ 10 | 1 | -$10 | CancelImmediate | Assinatura de SaaS do medidor personalizado |
