---
title: Arquivos de reconciliação de uso com classificação diária
ms.topic: article
ms.date: 06/12/2020
description: Saiba como ler arquivos de reconciliação de uso com classificação diária no Partner Center.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8b89efd0cb24fb8aa08160bc6b554c5c2823ba2b
ms.sourcegitcommit: b2f389ef0beacd722876e6396eab30b28bdf7e78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/16/2020
ms.locfileid: "84811571"
---
# <a name="learn-how-to-read-daily-rated-usage-reconciliation-files-in-partner-center"></a>Saiba como ler arquivos de reconciliação de uso com classificação diária no Partner Center

**Aplica-se a**

- Partner Center
- Partner Center do Microsoft Cloud for US Government

**Funções apropriadas**

- Agente administrativo
- Administrador de cobrança
- Agente de vendas
- Agente de suporte técnico

Este tópico explica como ler arquivos de reconciliação de uso com classificação diária.

>[!NOTE]
>O uso com classificação diária normalmente leva 24 horas para aparecer no Partner Center ou para ser acessado por meio da API.

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>Campos em arquivos de reconciliação de uso com classificação diária

| Coluna | Descrição |
| ------ | ----------- |
| PartnerId | Identificador de parceiro no formato GUID. |
| PartnerName | Nome do parceiro. |
| CustomerId | Identificador exclusivo da Microsoft para o cliente no formato GUID. |
| CustomerName | Nome da organização do cliente, conforme relatado na Central de parceiros. *Essa coluna é muito importante para reconciliar a fatura com as informações do sistema.* |
| CustomerDomainName | O nome de domínio do cliente. |
| CustomerCountry | O país em que o cliente está localizado. |
| MpnId | Identificador de MPN do parceiro CSP. |
| Tier2MpnId | Identificador MPN do revendedor do registro para a assinatura. |
| Número da Fatura | Número da fatura em que a transação especificada é exibida. |
| ProductId | O identificador do produto. |
| SkuId | O identificador de um SKU específico. |
| AvailabilityId | O identificador para a disponibilidade de um SKU específico. Isso mostra se o SKU está disponível para compra no país, moeda, segmento do setor, etc. |
| SkuName | O título de uma SKU em particular. |
| ProductName | O nome do produto. |
| PublisherName | O nome do publicador. |
| PublisherId | O identificador do Publicador no formato GUID. |
| Descrição da assinatura | O nome da oferta de serviço comprada pelo cliente, conforme definido na tabela de preços. (Este é um campo idêntico a **oferecer**). |
| SubscriptionId | Identificador exclusivo de uma assinatura na plataforma de faturamento da Microsoft. Não usado para reconciliação. *Esse identificador não é o mesmo que a **ID de assinatura** no console de administração do parceiro.* |
| ChargeStartDate | Data de início do ciclo de cobrança (exceto ao apresentar datas de dados de uso latentes anteriormente não cobrados do ciclo de cobrança anterior). A hora sempre é o início do dia, 0h00. |
| Data final da cobrança | Data de término do ciclo de cobrança (exceto ao apresentar datas de dados de uso latentes anteriormente não cobrados do ciclo de cobrança anterior). A hora é sempre o fim do dia, 23:59. |
| UsageDate | Data de uso do serviço. |
| MeterType | O tipo de medidor. |
| MeterCategory | O serviço de nível superior para o uso. |
| MeterId | O identificador do medidor que está sendo usado. |
| MeterSubCategory | O tipo de serviço do Azure, que pode afetar a taxa. |
| MeterName | A unidade de medida para o medidor que está sendo consumido. |
| MeterRegion | Essa coluna identifica a localização de um data center dentro da região para serviços onde isso é aplicável e preenchido. |
| Unidade | A unidade do **nome**do recurso. |
| ResourceLocation | O data center onde o medidor está em execução. |
| ConsumedService | O serviço da plataforma do Azure que você usou. |
| ResourceGroup | Representa um contêiner que mantém recursos relacionados para uma solução do Azure. |
| ResourceURI | O URI do recurso que está sendo usado. |
| ChargeType | O tipo de preço ou ajuste.  |
| UnitPrice | Preço por licença, conforme publicado na lista de preços no momento da compra. Verifique se esse preço corresponde às informações armazenadas em seu sistema de cobrança durante a reconciliação. |
| Quantidade | Número de licenças. Verifique se esse preço corresponde às informações armazenadas em seu sistema de cobrança durante a reconciliação. |
| UnitType | O tipo de unidade em que o medidor é cobrado.  |
| BillingPreTaxTotal | Valor total de cobrança antes dos impostos. |
| BillingCurrency | A moeda na região geográfica do cliente. |
| PricingPreTaxTotal | O preço antes da adição de impostos. |
| PricingCurrency | A moeda na lista de preços. |
| ServiceInfo1 | O número de conexões do barramento de serviço que foram provisionadas e utilizadas em um determinado dia. |
| ServiceInfo2 | Um campo herdado que captura metadados específicos do serviço opcionais. |
| Marcações | Representa uma organização lógica dos recursos do Azure definidos pelo usuário. |
| AdditionalInfo | Informações adicionais não abordadas em outras colunas. |
| EffectiveUnitPrice | O valor real cobrado por unidade, incluindo descontos, crédito acumulado, etc. |
| PCToBCExchangeRate | Taxa de câmbio aplicada para a moeda de preço à moeda de cobrança. |
| PCToBCExchangeRateDate | A data na qual a moeda de preço para a moeda de cobrança é determinada. |
| EntitlementId | Representa a ID da assinatura do Azure. |
| EntitlementDescription | Representa o nome da ID da assinatura do Azure. |
| PartnerEarnedCreditPercentage | Exibe o PartnerEarnedCredit para o item de linha. O crédito acumulado será de 0 ou 15 por cento |

>[!NOTE]
>O uso com classificação diária normalmente leva 24 horas para aparecer no Partner Center ou para ser acessado por meio da API.


