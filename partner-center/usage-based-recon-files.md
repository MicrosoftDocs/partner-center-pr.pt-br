---
title: Arquivos de reconciliação baseados em uso
ms.topic: article
ms.date: 06/08/2020
description: Saiba mais sobre todos os itens em seu arquivo de reconciliação baseado em uso no Partner Center. Inclui alguns exemplos.
author: sodeb
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6c486d4866b0a2a912801d2648a1822418687078
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431711"
---
# <a name="understand-usage-based-reconciliation-files-and-their-specific-fields-in-partner-center"></a>Entender os arquivos de reconciliação baseados em uso e seus campos específicos Partner Center

**Funções apropriadas:** conta de administrador | Administrador de cobrança

Para reconciliar seus encargos com relação ao uso de um cliente, compare **ResellerID,** **ResellerName** e  **ResellerBillableAccount** do arquivo de reconciliação com o Nome do cliente e a **ID** da assinatura do Partner Center.

## <a name="fields-in-usage-based-reconciliation-files"></a>Campos em arquivos de reconciliação baseados em uso

Os campos a seguir explicam quais serviços foram usados e a taxa.

| Coluna | Descrição | Valores de exemplo |
| ------ | ----------- | ------------ |
| PartnerId | Identificador de parceiro, no formato GUID. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| PartnerName | Nome do parceiro. | *Contoso, Ltd.* |
| PartnerBillableAccountId | Identificador de conta de parceiro. | *1010578050* |
| CustomerCompanyName | Nome da organização do cliente, conforme relatado Partner Center. *Isso é muito importante para reconciliar a fatura com as informações do seu sistema.* | *Testar cliente* |
| MpnId | Microsoft Partner Network (MPN) do parceiro Provedor de Soluções na Nuvem (CSP). | *4390934* |
| ResellerMpnId | Identificador MPN do revendedor de registro para a assinatura.  |
| Número da Fatura | Número da fatura em que a transação especificada é exibida. | *D020001IVK* |
| ChargeStartDate | Data de início do ciclo de faturamento, exceto ao apresentar datas de dados de uso latente anteriormente não cobertos (do ciclo de faturamento anterior). A hora sempre é o início do dia, 0h00. | *2/1/2019 0:00* |
| Data final da cobrança | Data final do ciclo de faturamento, exceto ao apresentar datas de dados de uso latente anteriormente não cobertos (do ciclo de faturamento anterior). A hora é sempre o fim do dia, 23:59. | *2/28/2019 23:59* |
| SubscriptionId | Identificador exclusivo de uma assinatura na plataforma de faturamento da Microsoft. Pode ser útil identificar a assinatura ao entrar em contato com o suporte. Não usado para reconciliação. *Isso não é o mesmo que a **ID da Assinatura** no Console de Administração do Parceiro.* | *usCBMgAAAAAAAAIA* |
| SubscriptionName | Apelido para a oferta de serviço. | *Microsoft Azure* |
| Descrição da assinatura | Linha de negócios da oferta de serviço. | *Microsoft Azure* |
| OrderID | Identificador exclusivo para um pedido na plataforma de cobrança do Microsoft. Pode ser útil identificar a assinatura ao entrar em contato com o suporte. Não usado para reconciliação. | *566890604832738111* |
| ServiceName | O nome do serviço do Azure em questão. | *MÁQUINAS VIRTUAIS* |
| ServiceType | O tipo específico do serviço do Azure. | *Barramento de Serviço – Individual ou Pack*, Banco de Dados SQL do *Azure – Business ou Web Edition* |
| ResourceGuid | Identificador exclusivo específico para todos os dados de serviço e estrutura de preços. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| ResourceName | O nome do recurso do Azure. | *Transferência de dados em (GB)*, *transferência de dados (GB)* |
| Região | A região à qual o uso se aplica. Usado principalmente para atribuir taxas a transferências de dados, pois as taxas variam de acordo com a região. | *Pacífico Asiático,* *Europa,* *América Latina,* *América do Norte* |
| Sku | Identificador exclusivo da Microsoft para uma oferta. | *7UD-00001* |
| DetailLineItemId | Um identificador e uma quantidade para listar taxas diferentes para um serviço ou recurso em um determinado período de cobrança. Para preços em camadas do Azure, pode haver uma taxa para até uma determinada quantidade de unidades de cobrança e, em seguida, uma taxa diferente após essa quantidade. | *1* |
| ConsumedQuantity | A quantidade de serviço consumido (como horas ou GB) durante o período de relatório. Também inclui qualquer uso não faturado de períodos de relatório anteriores. | *11* |
| IncludedQuantity | Unidades incluídas como parte da oferta. Normalmente, não está presente no CSP. | *0* |
| OverageQuantity | Unidades não incluídas como parte da oferta. Eles devem ser pagos pelo parceiro. Igual a **ConsumedQuantity** menos **IncludedQuantity.** | *11* |
| ListPrice | Preço da oferta em vigor na data de início da assinatura. | *$0.0808* |
| PretaxCharges | Igual a **ListPrist** multiplicado por **OverageQuantity**, arredondado para o cent mais próximo. | *U$ 0,085* |
| TaxAmount | Valor do imposto cobrado. Com base nas regras fiscais do seu mercado e em circunstâncias específicas. | *US$ 0,08* |
| PostTaxTotal | Total após impostos, quando o imposto é aplicável. | *US$ 0,93* |
| Moeda | Tipo de moeda. Cada entidade de cobrança tem apenas uma moeda. Verifique se ele corresponde à sua primeira fatura e, em seguida, após as atualizações da plataforma de cobrança principal. | *EUR* |
| PretaxEffectiveRate | Pretax preço por unidade. Igual a **PretaxCharges** dividido por **OverageQuantity**, arredondado para o cent mais próximo. | *US$ 0,08* |
| PostTaxEffectiveRate | Preço de imposto de POST por unidade. Igual a **PostTaxTotal** dividido por **OverageQuantity**, arredondado para o cent mais próximo. Ou, igual a **PretaxEffectiveRate mais** a taxa de imposto por valor unitário, arredondado para o cent mais próximo. | *US$ 0,08* |
| ChargeType | O [tipo de cobrança](recon-file-charge-types.md) ou ajuste. | Consulte [tipos de cobrança](recon-file-charge-types.md). |
| CustomerId | Identificador exclusivo da Microsoft para o cliente, no formato GUID. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| DomainName | Nome de domínio do cliente. Este campo pode aparecer em branco até o segundo ciclo de cobrança. | *example.onmicrosoft.com* |
| BillingCycleType | Frequência de cobrança de tempo.| **Mensalmente**  |
| Unidade | A unidade do nome do **recurso.** | *GB* ou *HOURS* |
| CustomerBillableAccount | Identificador de conta exclusivo na plataforma de cobrança da Microsoft. | *1280018095* |
| UsageDate | Data de implantação do serviço. | *2/1/2019 0:00* |
| MeteredRegion | Identifica o local de um data center dentro da região (para serviços em que esse valor é aplicável e populado). | *Leste da Ásia*, Sudeste da Ásia *,* Norte *da Europa,* *Europa Ocidental,* *Centro-Norte dos EUA,* *Centro-Sul dos EUA* |
| MeteredService | Identifica o uso individual do serviço do Azure quando ele não é especificamente identificado na **coluna ServiceName.** Por exemplo, as transferências de dados são *relatadas como Microsoft Azure - Todos os Serviços* na coluna **ServiceName.** | *AccessControl,* *CDN,* *Computação,* Banco *de Dados,* *ServiceBus,* *Armazenamento* |
| MeteredServiceType | Subposição para **o campo MeteredService** que fornece esclarecimento adicional sobre o uso do serviço do Azure. | *EXTERNAL* |
| Project | Nome definido pelo cliente para sua instância de serviço. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| ServiceInfo | O número de Barramento de Serviço do Azure que foram provisionadas e utilizadas em um determinado dia. | *1.00000 Conexões/30* dias (se você tiver uma conexão provisionada individualmente durante um mês de 30 dias), *25 Conexões/30 Dias – Usado: 1,0000000* (se você tivesse um pacote de 25 conexões do Barramento de Serviço provisionado e utilizado 1 durante esse dia) |

## <a name="next-steps"></a>Próximas etapas

- [Entender os campos nos Partner Center de reconciliação baseados em licença](license-based-recon-files.md)