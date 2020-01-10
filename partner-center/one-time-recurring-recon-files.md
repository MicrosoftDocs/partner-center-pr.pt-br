---
title: Arquivos de reconciliação recorrentes e de uso único | Centro de parceiros
ms.topic: article
ms.date: 01/03/2020
description: Entenda os arquivos de reconciliação recorrentes e de uso único no Partner Center.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 6f381189fc1d8fad692ef248dcdcbf5ab8b0af43
ms.sourcegitcommit: fe1f2730a14ec394caccdbb59b00ef5908acaa29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/09/2020
ms.locfileid: "75757229"
---
# <a name="one-time-and-recurring-reconciliation-files"></a>Arquivos de reconciliação recorrentes e de uso único

**Aplica-se a**

- Partner Center
- Partner Center do Microsoft Cloud for US Government

**Funções apropriadas**
-   Administração global
-   Administrador de usuários
-   Administrador de cobrança
-   Agente administrativo
-   Agente de vendas

Este tópico explica como ler arquivos de reconciliação recorrentes e de uso único no Partner Center.

## <a name="fields-in-one-time-and-recurring-reconciliation-files"></a>Campos em arquivos de reconciliação recorrentes e de uso único

| Column | Descrição |
| ------ | ----------- |
| PartnerID | Identificador de locatário exclusivo do Azure Active Directory (AD do Azure) para uma entidade de cobrança específica, no formato GUID. Não é necessário para reconciliação. O mesmo em todas as linhas. |
| CustomerID | Identificador exclusivo do locatário do Azure AD, no formato GUID. Identifica o cliente. |
| CustomerName | Nome da organização do cliente, conforme relatado no Partner Center. |
| CustomerDomainName | Nome de domínio do cliente. Este campo pode aparecer em branco até o segundo ciclo de cobrança. *Não use esse campo como um identificador exclusivo para o cliente. O cliente/parceiro pode atualizar o intuitivo ou o domínio padrão por meio do portal do Office 365.* |
| CustomerCountry | O país em que o cliente está localizado. |
| InvoiceNumber | Número da fatura na qual a transação especificada é exibida. |
| MpnId | Identificador de MPN do parceiro CSP. |
| OrderID | Identificador exclusivo de um pedido na plataforma Microsoft Commerce. Não usado para reconciliação. |
| OrderDate | A data em que o pedido foi feito. |
| ProductId | O identificador do produto. |
| SkuId | O identificador de um SKU específico (unidade de manutenção de estoque). |
| AvailabilityId | O identificador para a disponibilidade de um SKU específico. Isso mostra se o SKU está disponível para compra no país, moeda, segmento do setor, etc. |
| SkuName | O título de uma SKU em particular. |
| ProductName | O nome do produto. |
| ChargeType | O tipo de encargo ou ajuste. |
| UnitPrice | O preço unitário como publicado na lista de preços no momento da compra. *Certifique-se de que isso corresponde às informações armazenadas em seu sistema de cobrança durante a reconciliação.* |
| Quantity | Número de unidades. *Certifique-se de que isso corresponde às informações armazenadas em seu sistema de cobrança durante a reconciliação.* |
| SubTotal | Total sem imposto. Verifica se o SUBTOTAL corresponde ao seu total esperado, no caso de um desconto. |
| TaxTotal | Encargo do valor do imposto. Com base nas regras de imposto do mercado e em circunstâncias específicas. |
| Total | Total com imposto. Verifica se o imposto é cobrado na fatura. |
| Currency | Tipo de moeda. Cada entidade de cobrança tem somente uma moeda. Verifique se isso corresponde à sua primeira fatura e verifique novamente após as principais atualizações da plataforma de cobrança. |
| PriceAdjustmentDescription | Uma explicação de qualquer desconto aplicável. |
| PublisherName | O nome do editor do produto.
| PublisherId | Identificador exclusivo de um Publicador específico. |
| SubscriptionDescription | Nome amigável de uma assinatura. |
| SubscriptionID | Identificador exclusivo de uma assinatura na plataforma Microsoft Commerce. Não usado para reconciliação. *Esse identificador não é o mesmo que a **ID de assinatura** no console de administração do parceiro.* |
| ChargeStartDate | Dia de início dos encargos. A hora é sempre o início do dia, 0:00. |
| ChargeEndDate | Dia do término dos encargos. A hora é sempre o fim do dia, 23:59. |
| TermAndBillingcycle | O tamanho do termo e o ciclo de cobrança da compra (por exemplo, *1 ano, mensalmente*). |
| EffectiveUnitPrice | O preço unitário após os ajustes terem sido feitos. |
| UnitType | O tipo de unidade que está sendo adquirida. |
| AlternateId | Um identificador alternativo para uma **ID de pedido**. |
| BillableQuantity | Representa o total de unidades adquiridas ou consumidas. |
| BillingFrequency | Descreve se o item de linha é uma frequência de cobrança mensal ou ocasional. *Atualmente, isso tem suporte somente para o Azure RI, com valores com suporte como mensal. Se a RI for comprada com frequência de cobrança única, esse campo no arquivo reconhecimento será exibido em branco.* |
| PricingCurrency | O preço de lista do recurso ou oferta. |
| PCToBCExchangeRate | Taxa de câmbio aplicada para a moeda de preço à moeda de cobrança. |
| PCToBCExchangeRateDate | A data na qual a moeda de preço para a moeda de cobrança é determinada. |
| MeterDescription | A descrição do medidor do item de linha de consumo. |


