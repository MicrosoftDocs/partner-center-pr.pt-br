---
title: Cobrança – transações de SaaS baseadas em licença
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba mais sobre cenários comuns de cobrança Partner Center para transações SaaS (software como serviço) baseadas em licença.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 764d5a3cb0dc6f409e5272d4119424396caff53b
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148628"
---
# <a name="common-billing-scenarios-for-license-based-saas-transactions-in-partner-center"></a>Cenários comuns de cobrança para transações saaS baseadas em licença em Partner Center

**Funções apropriadas:** agente administrador | Administrador de cobrança | Agente de ajuda | Agente de vendas


Esses [exemplos de cenários comuns](common-billing-scenarios.md) de cobrança são aplicáveis a assinaturas de SaaS (software como serviço) baseadas em licença Partner Center.

## <a name="convert-a-free-trial-saas-subscription-to-a-paid-subscription"></a>Converter uma assinatura saaS de avaliação gratuita em uma assinatura paga

Este cenário descreve a cobrança pela renovação de uma assinatura saaS de avaliação gratuita baseada em licença. A renovação converte a avaliação gratuita em uma assinatura paga no final do período de avaliação gratuita.

Neste exemplo, você comprou uma avaliação gratuita de uma assinatura de SaaS (software como serviço) baseada em licença em 10 de junho. Essa avaliação gratuita é renovada automaticamente como uma assinatura paga quando o período de avaliação gratuita termina.

Os arquivos de reconhecimento incluirão os seguintes encargos:

| Data de compra | Data de início da cobrança | Data de término da cobrança | Preço unitário | Quantidade de unidade | Valor total | Tipo de cobrança | Descrição da assinatura |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | U$0 | 1 | U$0 | Novo | Avaliação gratuita |
| 07/10/2019 | 07/10/2019 | 09/08/2019 | U$2 | 1 | U$2 | Renew | Assinatura paga |

## <a name="cancel-a-free-trial-saas-subscription"></a>Cancelar uma assinatura de SaaS de avaliação gratuita

> [!TIP]
> Você pode cancelar uma assinatura SaaS de avaliação gratuita baseada em licença a qualquer momento, mesmo durante o período de avaliação gratuita.

Nesse cenário, você comprou uma assinatura SaaS de avaliação gratuita baseada em licença em 1º de julho e a cancelou imediatamente no Partner Center.

O arquivo reconhecimento incluirá os seguintes encargos:

| Data de compra | Data de início do encargo | Data de término do encargo | Preço unitário | Quantidade de unidades | Valor total | Tipo de cobrança | Descrição da assinatura |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | U$0 | 11 | U$0 | Novo | Avaliação gratuita |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | U$0 | 11 | U$0 | Cancelar | Avaliação gratuita |

## <a name="convert-custom-meter-saas-subscription-to-another-sku"></a>Converter a assinatura SaaS do medidor personalizado em outra SKU

Este cenário descreve como converter uma assinatura de SaaS de medidor personalizado de uma SKU (unidade de manutenção de estoque) para outra SKU para o mesmo produto, na mesma data.

Nesse cenário, você comprou um SKU (prata) em um produto e o converteu em outro SKU (bronze) disponível sob este produto na mesma data.

O arquivo reconhecimento incluirá os seguintes encargos:

| Data de compra | SKU | Data de início do encargo | Data de término do encargo | Preço unitário | Quantidade de unidades | Valor total | Tipo de cobrança | Descrição da assinatura |
| ------------- | ----------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | Prata | 06/10/2019 | 06/10/2019 | U$20 | 1 | U$20 | Novo | Assinatura de SaaS do medidor personalizado |
| 06/10/2019 | Prata | 06/10/2019 | 06/10/2019 | U$20 | 1 | -$20 | Converter | Fatura rateada para assinatura de SaaS de medidor personalizado |
| 06/10/2019 | Bronze | 06/10/2019 | 06/10/2019 | US$ 10 | 1 | US$ 10 | Converter | Assinatura de SaaS de medidor personalizado |

## <a name="purchase-and-cancel-a-customer-meter-saas-subscription-on-same-date"></a>Comprar e cancelar uma assinatura saaS de medidor de cliente na mesma data

Este cenário descreve a cobrança de uma assinatura saaS do medidor de cliente que você comprou e cancelou por meio do portal do Azure na mesma data.

Nesse cenário, você comprou uma assinatura de SaaS de medidor personalizado no portal do Azure. Em seguida, você cancelou a assinatura na mesma data.

| Data de compra | SKU | Data de início da cobrança | Data de término da cobrança | Preço unitário | Quantidade de unidade | Valor total | Tipo de cobrança | Descrição da assinatura |
| ------------- | ------------- |----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | Bronze | 06/10/2019 | 06/10/2019 | US$ 10 | 1 | US$ 10 | Novo | Assinatura de SaaS de medidor personalizado |
| 06/10/2019 | Bronze | 06/10/2019 | 06/10/2019 | US$ 10 | 1 | -$10 | CancelImmediate | Assinatura de SaaS de medidor personalizado |
