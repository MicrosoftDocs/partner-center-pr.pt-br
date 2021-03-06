---
title: Arquivos de reconciliação de uso com classificação diária
ms.topic: article
ms.date: 06/12/2020
description: Saiba como ler arquivos de reconciliação de uso com classificação diária no Partner Center. Inclui descrições para campos específicos no arquivo reconhecimento.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9b5daf91646324a9d4ace92d25736cfd0361ad6c
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147268"
---
# <a name="learn-how-to-read-daily-rated-usage-reconciliation-files-in-partner-center"></a>Saiba como ler arquivos de reconciliação de uso com classificação diária no Partner Center

**Aplica-se a**: Partner Center | Partner Center para Microsoft Cloud do governo dos EUA

**Funções apropriadas**: agente de administração | Administrador de cobrança | Agente de vendas | Agente de assistência técnica

Este artigo explica como ler arquivos de reconciliação de uso com classificação diária.

>[!NOTE]
>O uso com classificação diária normalmente leva 24 horas para aparecer no Partner Center ou para ser acessado por meio da API.

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>Campos em arquivos de reconciliação de uso com classificação diária

| Coluna | Descrição |
| ------ | ----------- |
| PartnerId | Identificador de parceiro no formato GUID. |
| PartnerName | Nome do parceiro. |
| CustomerId | Identificador exclusivo da Microsoft para o cliente no formato GUID. |
| CustomerName | Nome da organização do cliente, conforme relatado na Central de parceiros. *Essa coluna é importante para reconciliar a fatura com as informações do sistema.* |
| CustomerDomainName | O nome de domínio do cliente. |
| CustomerCountry | O país em que o cliente está localizado. |
| MpnId | Identificador de MPN do parceiro CSP. |
| Tier2MpnId | Identificador MPN do revendedor do registro para a assinatura. |
| Número da Fatura | Número da fatura em que a transação especificada é exibida. |
| ProductId | O identificador do produto. |
| SkuId | O identificador de um SKU específico. |
| AvailabilityId | O identificador para a disponibilidade de um SKU específico. Esta coluna mostra se a SKU está disponível para compra no país, moeda, segmento do setor, etc. |
| SkuName | O título de uma SKU em particular. |
| ProductName | O nome do produto. |
| PublisherName | O nome do publicador. |
| PublisherId | O identificador do publicador no formato GUID. |
| Descrição da assinatura | O nome da oferta de serviço comprada pelo cliente, conforme definido na tabela de preços. (Esta coluna é um campo idêntico a **OfferName**). |
| SubscriptionId | Identificador exclusivo de uma assinatura na plataforma de faturamento da Microsoft. Não usado para reconciliação. *Esse identificador não é o mesmo que a **ID da Assinatura** no console de administração do parceiro.* |
| ChargeStartDate | Data de início do ciclo de cobrança (exceto ao apresentar datas de dados de uso latente não cobrados anteriormente do ciclo de cobrança anterior). A hora sempre é o início do dia, 0h00. |
| Data final da cobrança | Data de término do ciclo de cobrança (exceto ao apresentar datas de dados de uso latente não cobrados anteriormente do ciclo de cobrança anterior). A hora é sempre o fim do dia, 23:59. |
| UsageDate | Data de uso do serviço. |
| MeterType | O tipo de medidor. |
| MeterCategory | O serviço de nível superior para o uso. |
| MeterId | O identificador do medidor que está sendo usado. |
| MeterSubCategory | O tipo de serviço do Azure, que pode afetar a taxa. |
| MeterName | A unidade de medida para o medidor que está sendo consumido. |
| MeterRegion | Essa coluna identifica o local de um data center dentro da região para serviços em que MeterRegion é aplicável e populado. |
| Unidade | A unidade do nome do **recurso.** |
| ResourceLocation | O data center em que o medidor está em execução. |
| ConsumedService | O serviço da plataforma do Azure que você usou. |
| ResourceGroup | Representa um contêiner que contém recursos relacionados para uma solução do Azure. |
| ResourceURI | O URI do recurso que está sendo usado. |
| ChargeType | O tipo de preço ou ajuste.  |
| UnitPrice | Preço por licença, conforme publicado na lista de preços no momento da compra. Certifique-se de que esse preço corresponde às informações armazenadas em seu sistema de cobrança durante a reconciliação. |
| Quantidade | Número de licenças. Certifique-se de que esse preço corresponde às informações armazenadas em seu sistema de cobrança durante a reconciliação. |
| UnitType | O tipo de unidade em que o medidor é cobrado.  |
| BillingPreTaxTotal | Valor total de cobrança antes dos impostos.<br/> _**BillingPreTaxTotal** = Floor (([ @EffectiveUnitPrice ]*[ @Quantity ]*[ @PCToBCExchangeRate ]), 2)_ |
| BillingCurrency | A moeda na região geográfica do cliente. |
| PricingPreTaxTotal | O preço, antes que os impostos sejam adicionados. |
| PricingCurrency | A moeda na lista de preços. |
| ServiceInfo1 | O número de conexões do barramento de serviço que foram provisionadas e usadas em um determinado dia. |
| ServiceInfo2 | Um campo herdado que captura metadados específicos do serviço opcionais. |
| Marcações | Representa uma organização lógica dos recursos do Azure definidos pelo usuário. |
| AdditionalInfo | Informações adicionais não abordadas em outras colunas. |
| EffectiveUnitPrice | O valor real cobrado por unidade, incluindo descontos, crédito acumulado e assim por diante. |
| PCToBCExchangeRate | Taxa de câmbio aplicada para a moeda de preço à moeda de cobrança. |
| PCToBCExchangeRateDate | A data na qual a moeda de preço para a moeda de cobrança é determinada. |
| EntitlementId | Representa a ID da assinatura do Azure. |
| EntitlementDescription | Representa o nome da ID da Assinatura do Azure. |
| PartnerEarnedCreditPercentage | Exibe o PartnerEarnedCredit para o item de linha. O crédito ganho será de 0 ou 15% |
| CreditPercentage | Exibe o Crédito de Consumo do Azure. O crédito ganho será de 0 ou 100%. |
| CreditType | Tipo do crédito. Por exemplo, **Crédito Azure Aplicado.** |
>[!NOTE]
>O uso com classificação diária normalmente leva 24 horas para aparecer no Partner Center ou para ser acessado por meio da API.


