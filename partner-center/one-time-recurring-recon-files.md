---
title: Arquivos de reconciliação recorrentes e de uso único | Centro de parceiros
ms.topic: article
ms.date: 11/21/2019
description: Entenda os arquivos de reconciliação recorrentes e de uso único no Partner Center.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 51c37c9ea2110b7666c4d1a9bc92a2b01f92209c
ms.sourcegitcommit: 07eb5eb6c1cfed1c84fad3626b8f989247341e70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2019
ms.locfileid: "75004895"
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
| ID do cliente | Identificador exclusivo do locatário do Azure AD, no formato GUID. Identifica o cliente. |
| Nome do cliente | Nome da organização do cliente, conforme relatado no Partner Center. |
| CustomerDomainName | Nome de domínio do cliente. Este campo pode aparecer em branco até o segundo ciclo de cobrança. *Não use esse campo como um identificador exclusivo para o cliente. O cliente/parceiro pode atualizar o intuitivo ou o domínio padrão por meio do portal do Office 365.* |
| País/Região do cliente | O país em que o cliente está localizado. |
| Número da fatura | Número da fatura na qual a transação especificada é exibida. |
| MpnId | Identificador de MPN do parceiro CSP. |
| MpnId do revendedor | Identificador MPN do revendedor do registro para a assinatura. |
| ID do Pedido | Identificador exclusivo de um pedido na plataforma Microsoft Commerce. Não usado para reconciliação. |
| Data do pedido | A data em que o pedido foi feito. |
| ProductId | O identificador do produto. |
| SkuId | O identificador de um SKU específico (unidade de manutenção de estoque). |
| AvailabilityId | O identificador para a disponibilidade de um SKU específico. Isso mostra se o SKU está disponível para compra no país, moeda, segmento do setor, etc. |
| Nome da SKU | O título de uma SKU em particular. |
| Nome do produto | O nome do produto. |
| PublisherName | O nome do editor do produto.
| PublisherID | Identificador exclusivo de um Publicador específico. |
| Descrição da assinatura | Nome amigável de uma assinatura. |
| ID da assinatura | Identificador exclusivo de uma assinatura na plataforma Microsoft Commerce. Não usado para reconciliação. *Esse identificador não é o mesmo que a **ID de assinatura** no console de administração do parceiro.* |
| ChargeStartDate | Dia de início dos encargos. A hora é sempre o início do dia, 0:00. |
| ChargeEndDate | Dia do término dos encargos. A hora é sempre o fim do dia, 23:59. |
| Termo e Billingcycle | O tamanho do termo e o ciclo de cobrança da compra (por exemplo, *1 ano, mensalmente*). |
| Tipo de Cobrança | O tipo de encargo ou ajuste. |
| Preço unitário | O preço unitário como publicado na lista de preços no momento da compra. *Certifique-se de que isso corresponde às informações armazenadas em seu sistema de cobrança durante a reconciliação.* |
| Preço unitário efetivo | O preço unitário após os ajustes terem sido feitos. |
| Quantity | Número de unidades. *Certifique-se de que isso corresponde às informações armazenadas em seu sistema de cobrança durante a reconciliação.* |
| Tipo de unidade | O tipo de unidade que está sendo adquirida. |
| DiscountDetails | Uma explicação de qualquer desconto aplicável. |
| Subtotal | Total sem imposto. Verifica se o SUBTOTAL corresponde ao seu total esperado, no caso de um desconto. |
| Total do imposto | Encargo do valor do imposto. Com base nas regras de imposto do mercado e em circunstâncias específicas. |
| Total | Total com imposto. Verifica se o imposto é cobrado na fatura. |
| Currency | Tipo de moeda. Cada entidade de cobrança tem somente uma moeda. Verifique se isso corresponde à sua primeira fatura e verifique novamente após as principais atualizações da plataforma de cobrança. |
| Uma alternateid | Um identificador alternativo para uma **ID de pedido**. |
