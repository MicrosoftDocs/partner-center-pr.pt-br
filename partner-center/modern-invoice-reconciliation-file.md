---
title: Campos de arquivo reconhecimento para compras de CSP único
ms.topic: conceptual
ms.date: 01/29/2021
description: Saiba mais sobre todos os itens em seu CSP único arquivo de reconciliação de compra única no Partner Center, incluindo valores de exemplo.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.openlocfilehash: 559b5334eb23ad76fe8cc51fc1beeaa3a86c6fa1
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702783"
---
# <a name="csp-one-time-purchase-reconciliation-file-fields"></a>Campos de arquivo de reconciliação de compra única do CSP

**Funções apropriadas**

- Administrador de conta
- Agente de cobrança

## <a name="using-the-recon-file"></a>Usando o arquivo reconhecimento
A tabela a seguir fornece descrições e valores de exemplo para os campos no arquivo de reconciliação para compras unidirecionais do CSP.

Para obter mais informações sobre arquivos de reconciliação, consulte [usar os arquivos de reconciliação](use-the-reconciliation-files.md).

| Coluna | Descrição | Valor de exemplo |
| ------ | ----------- | ------------ |
| PartnerId | Identificador exclusivo no formato GUID para uma entidade de cobrança específica. Não é necessário para reconciliação. O mesmo em todas as linhas. | *0e195b37-4574-4539-bc42-0e539b9684c0* |
| CustomerId | Identificador exclusivo da Microsoft para o cliente no formato GUID. | *196e2273-9651-43a3-ba7e-7cbcd918fc40* |
| CustomerName | Nome da organização do cliente, conforme relatado na Central de parceiros. Essa coluna é importante para reconciliar a fatura com as informações do sistema. | *Johnny de cust DE2 moderno* |
| CustomerDomainName | Nome de domínio do cliente. | *testcustomerdomain.onmicrosoft.com* |
| CustomerCountry | O país onde o cliente está localizado. Consulte a [lista completa de países](./regional-authorization-overview.md) para sua região.  | *DE* |
| Número da Fatura | O número da nota fiscal associado ao arquivo de reconciliação.  | *G002297372* |
| MpnId | Identificador de MPN do parceiro CSP. Para obter mais informações, consulte [como discriminar por parceiro](./use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner). | *6034453* |
| ResellerMpnId | Identificador MPN do revendedor do registro para a assinatura. | *6048879* |
| OrderId | Identificador exclusivo para um pedido na plataforma de cobrança do Microsoft. Pode ser útil identificar a ordem ao contatar o suporte. Não usado para reconciliação. | *0ET2qaZvJGfF9wgSKnWzR5JLmhp10lOc1* |
| OrderDate | Data em UTC em que a ordem foi colocada. | *10/3/2020* |
| ProductId | O identificador exclusivo do produto. | *DZH318Z0BNZ5* |
| SkuId | O identificador exclusivo do SKU. | *006G* |
| AvailabilityId | O identificador exclusivo de disponibilidade. | *DZH318Z08B80* |
| SkuName | O nome do SKU. | *Tabelas-LRS* |
| ProductName | O Nome do produto. | *Tabelas* |
| ChargeType | O [tipo de encargo](./recon-file-charge-types.md) ou ajuste. | *Novo* |
| UnitPrice | Preço por licença, conforme publicado na lista de preços no momento da compra. Certifique-se de que isso corresponde às informações armazenadas em seu sistema de cobrança durante a reconciliação. | *0, 45* |
| Quantidade | O número de licenças. Certifique-se de que isso corresponde às informações armazenadas em seu sistema de cobrança durante a reconciliação. | *1* |
| Subtotal | Total sem imposto. O SUBTOTAL deve ser igual à quantidade Faturável multiplicada pelo preço unitário efetivo. | *0* |
| TaxTotal | Encargo do valor do imposto. Com base nas regras de imposto do mercado e em circunstâncias específicas. | *0* |
| Total | O valor total é igual ao subtotal mais o valor do imposto. | *0* |
| Moeda | Sua fatura é gerada no contexto da moeda do cliente. Isso significa que, se você for um parceiro que esteja realizando uma transação com clientes de diferentes moedas faturáveis, receberá uma fatura para cada tipo de moeda do cliente.  | *EUR* |
| PriceAdjustmentDescription | Os motivos para os ajustes no preço unitário. Esses são os principais motivos, mas não se limitam à determinação do preço unitário efetivo. | *["15,0% crédito ganho de parceiro para serviços gerenciados"]* |
| PublisherName | Editor do produto.  | *Microsoft* |
| PublisherId | Um identificador exclusivo que o Partner Center usa para identificar o Publicador. | *NA* |
| Descrição da assinatura | O nome da oferta de serviço comprada pelo cliente, conforme definido na tabela de preços. Esta coluna é um campo idêntico a oferecer. | *Plano do Azure* |
| SubscriptionId | Identificador exclusivo de uma assinatura na plataforma de faturamento da Microsoft. Não usado para reconciliação. Observe que esse identificador não é o mesmo que a ID de assinatura no console do administrador do parceiro. | *307628f1-d9d2-f09c-ea1f-4183f0cae308* |
| ChargeStartDate | A data em que o período de cobrança de uma assinatura é iniciado. | *9/1/2020* |
| Data final da cobrança | A data em que o período de cobrança de uma assinatura termina. | *30/09/2020* |
| TermAndBillingCycle | O compromisso de duração para continuar a assinatura no momento da compra. | *Dados armazenados (GB/mês)* |
| EffectiveUnitPrice | O preço unitário rateado para calcular o custo do ciclo de cobrança. Os descontos, os ajustes nos dias de cobrança e outros fatores determinam o preço unitário efetivo. Para obter mais informações, veja [cálculo de preço unitário efetivo](./effective-unit-price-calculation.md).  | *0, 3825* |
| UnitType | O tipo de unidade em que o medidor é cobrado. | *1 GB/mês* |
| Uma alternateid | A ID alternativa do item de linha da ordem referenciada. | *6dc5c039750a* |
| BillableQuantity | A quantidade total sendo cobrada.  | *0, 5001* |
| BillingFrequency | O plano de cobrança selecionado no momento da compra. | *NA*  |
| PricingCurrency | A moeda na lista de preços. | *USD* |
| PCToBCExchangeRate | A taxa de câmbio aplicada para a moeda de preço à moeda de cobrança. | *0,846202666* |
| PCToBCExchangeRateDate | A data na qual a moeda de preço para a moeda de cobrança é determinada. | *30/09/2020* |
| MeterDescription | Descrição do medidor.  | *Tabelas – dados de LRS armazenados (GB/mês)* |
| ReservationOrderId | A ID do pedido de reserva. | *E21A6344E398FFC1C4D7...* |
| CreditReasonCode | A descrição do crédito. | *Crédito de consumo do Azure* |

>[!NOTE]
>Você pode reconciliar seu consumo do Azure em seu arquivo de reconhecimento de compra única. Para fazer isso, acesse o arquivo de reconhecimento de uso com classificação diária e procure sua SubscriptionId. Isso exibirá todos os custos associados à sua ID do plano do Azure. Sua assinatura do Azure é mostrada como o EntitlementID.

## <a name="next-steps"></a>Próximas etapas

- [Cobrança e impostos](billing.md)
