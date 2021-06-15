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
ms.openlocfilehash: 3264c793dfb2e8592cd059cd84d5bb08769abbcf
ms.sourcegitcommit: c8d1bcf54cdcdc3f827f9210c8abddab02a686fe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2021
ms.locfileid: "112073791"
---
# <a name="csp-one-time-purchase-reconciliation-file-fields"></a>Campos de arquivo de reconciliação de compra única do CSP

**Funções apropriadas**: administrador da conta | Agente de cobrança

## <a name="using-the-recon-file"></a>Usando o arquivo reconhecimento
A tabela a seguir fornece descrições e valores de exemplo para os campos no arquivo de reconciliação para compras unidirecionais do CSP.

Para obter mais informações sobre arquivos de reconciliação, consulte [usar os arquivos de reconciliação](use-the-reconciliation-files.md).

| Coluna | Descrição | Valor de exemplo |
| ------ | ----------- | ------------ |
| PartnerId | Identificador exclusivo no formato GUID para uma entidade de cobrança específica. Não é necessário para reconciliação. O mesmo em todas as linhas. | *0e195b37-4574-4539-bc42-0e539b9684c0* |
| CustomerId | Identificador exclusivo da Microsoft para o cliente no formato GUID. | *196e2273-9651-43a3-ba7e-7cbcd918fc40* |
| CustomerName | Nome da organização do cliente, conforme relatado na Central de parceiros. Essa coluna é importante para reconciliar a fatura com as informações do sistema. | *Johnny de cust DE2 moderno* |
| CustomerDomainName | Nome de domínio do cliente. | *testcustomerdomain.onmicrosoft.com* |
| CustomerCountry | O país onde o cliente está localizado. Consulte a [lista completa de países](./regional-authorization-overview.md) para sua região.  | *DEPRECIA* |
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
| Descrição da assinatura | O nome da oferta de serviço comprada pelo cliente, conforme definido na tabela de preços. Essa coluna é um campo idêntico a OfferName. | *Plano do Azure* |
| SubscriptionId | Identificador exclusivo de uma assinatura na plataforma de faturamento da Microsoft. Não usado para reconciliação. Observe que esse identificador não é o mesmo que a ID da Assinatura no console de administração do parceiro. | *307628f1-d9d2-f09c-ea1f-4183f0cae308* |
| ChargeStartDate | A data em que o período de cobrança de uma assinatura é iniciado. | *9/1/2020* |
| Data final da cobrança | A data em que o período de cobrança de uma assinatura termina. | *30/09/2020* |
| TermAndBillingCycle | O compromisso de duração para continuar a assinatura no momento da compra. | *Dados armazenados (GB/mês)* |
| EffectiveUnitPrice | O preço unitária rateado para calcular o custo do ciclo de cobrança. Descontos, ajustes em dias de cobrança e outros fatores determinam o preço unitário efetivo. Para obter mais informações, consulte [Cálculo de preço unitório efetivo](./effective-unit-price-calculation.md).  | *0.03825* |
| Unittype | O tipo de unidade na qual o medidor é cobrado. | *1 GB/mês* |
| AlternateId | A ID alternativa do item de linha de pedido referenciado. | *6dc5c039750a* |
| BillableQuantity | A quantidade total que está sendo cobrada.  | *0.005001* |
| BillingFrequency | O plano de cobrança selecionado no momento da compra. | *NA*  |
| PricingCurrency | A moeda na lista de preços. | *USD* |
| PCToBCExchangeRate | A taxa de câmbio aplicada à moeda de preços para a moeda de cobrança. | *0.846202666* |
| PCToBCExchangeRateDate | A data em que a moeda de preços para a moeda de cobrança é determinada. | *30/09/2020* |
| MeterDescription | Descrição do medidor.  | *Tabelas – Dados LRS armazenados (GB/Mês)* |
| ReservationOrderId | A ID do Pedido de Reserva. | *E21A6344E398FFC1C4D7...* |
| CreditReasonCode | A Descrição do Crédito. | *Crédito de consumo do Azure* |
| SubscriptionStartDate | A data em que uma assinatura é comprada. | *5/1/2021* |
| SubscriptionEndDate | A data em que uma assinatura expira. | *4/30/2022* |
| ReferenceID | A vinculação a todas as transações que ocorrem durante atualizações. | *025d68a6-1bd6-42ab-9636-15e8d776a30e* |
| ProductQualifiers | O identificador para saber as compras de Complemento ou Avaliação. | *["Complemento"]* |
| PromotionID | O identificador a ser usado para buscar as informações da promoção. | *78bcf906-b945-4210-8818-cfb93caf12a1* |

>[!NOTE]
>Você pode reconciliar o consumo do Azure em seu arquivo de reconhecimento de compra única. Para fazer isso, vá para o arquivo de reconhecimento de uso com classificação diária e pesquise sua SubscriptionID. Isso exibirá todos os custos associados à sua ID do Plano do Azure. Sua SubscriptionID do Azure é mostrada como o EntitlementID.
>

## <a name="how-to-connect-the-base-subscription-with-the-upgraded-subscription"></a>Como conectar a assinatura base à assinatura atualizada?

Você deve usar a ID de assinatura do produto base para encontrar as IDs de referência correspondentes e usá-las para buscar todas as transações associadas. Combinado com a ID da Assinatura e a ID de Referência, você pode conectar todas as atualizações ocorridas em um único evento.

## <a name="next-steps"></a>Próximas etapas

- [Cobrança e impostos](billing.md)
