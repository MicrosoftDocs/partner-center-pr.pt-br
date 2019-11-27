---
title: Arquivos de reconciliação de uso com classificação diária | Centro de parceiros
ms.topic: article
ms.date: 11/21/2019
description: Entenda os arquivos de reconciliação de uso com classificação diária no Partner Center.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 896f81b3a51e234065af7779d287b4023dd7163c
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389694"
---
# <a name="daily-rated-usage-reconciliation-files"></a>Arquivos de reconciliação de uso com classificação diária

Aplica-se a:

- Partner Center
- Partner Center do Microsoft Cloud for US Government

Este tópico explica como ler arquivos de reconciliação de uso com classificação diária.

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>Campos em arquivos de reconciliação de uso com classificação diária

| Column | Descrição |
| ------ | ----------- |
| PartnerID | Identificador de parceiro no formato GUID. |
| PartnerName | Nome do parceiro. |
| CustomerID | Identificador exclusivo da Microsoft para o cliente no formato GUID. |
| CustomerCompanyName | Nome da organização do cliente como informado no Partner Center. *Essa coluna é muito importante para reconciliar a fatura com as informações do sistema.* |
| CustomerDomainName | O nome de domínio do cliente. Não disponível para a atividade atual. |
| País do cliente | O país em que o cliente está localizado. |
| ID do MPN | Identificador de MPN do parceiro CSP. |
| MPNID do revendedor | Identificador MPN do revendedor do registro para a assinatura. Não disponível para a atividade atual. |
| InvoiceNumber | Número da fatura na qual a transação especificada é exibida. Não disponível para a atividade atual. |
| ProductId | O identificador do produto. |
| SkuId | O identificador de um SKU específico. |
| AvailabilityId | O identificador para a disponibilidade de um SKU específico. Isso mostra se o SKU está disponível para compra no país, moeda, segmento do setor, etc. |
| Nome do SKU | O título de uma SKU em particular. |
| PublisherName | O nome do Publicador. |
| PublisherID | O identificador do Publicador no formato GUID. Não disponível para a atividade atual. |
| Descrição da assinatura | O nome da oferta de serviço comprada pelo cliente, conforme definido na tabela de preços. (Este é um campo idêntico a **oferecer**). |
| ID da assinatura | Identificador exclusivo de uma assinatura na plataforma de cobrança da Microsoft. Não usado para reconciliação. *Esse identificador não é o mesmo que a **ID de assinatura** no console de administração do parceiro.* |
| ChargeStartDate | Data de início do ciclo de cobrança (exceto ao apresentar datas de dados de uso latentes anteriormente não cobrados do ciclo de cobrança anterior). A hora é sempre o início do dia, 0:00. |
| ChargeEndDate | Data de término do ciclo de cobrança (exceto ao apresentar datas de dados de uso latentes anteriormente não cobrados do ciclo de biling anterior). A hora é sempre o fim do dia, 23:59. |
| Data de uso | Data de uso do serviço. |
| Tipo de medidor | O tipo de medidor. |
| Categoria do medidor | O serviço de nível superior para o uso. |
| ID do medidor | O identificador do medidor que está sendo usado. |
| Subcategoria do medidor | O tipo de serviço do Azure, que pode afetar a taxa. |
| Nome do medidor | A unidade de medida para o medidor que está sendo consumido. |
| Região do medidor | Essa coluna identifica a localização de um data center dentro da região para serviços onde isso é aplicável e preenchido. |
| Unidade | A unidade do **nome**do recurso. |
| Quantidade consumida | A quantidade de serviço consumida (como *horas* ou *GB*) durante o período de relatório. Inclui qualquer uso não cobrado dos períodos de relatório anteriores. |
| Local do recurso | > o data center onde o medidor está em execução. |
| Serviço consumido | O serviço da plataforma do Azure que você usou. |
| URI de recurso | O URI do recurso que está sendo usado. |
| Tipo de cobrança | O tipo de encargo ou ajuste. Não disponível para a atividade atual. |
| Preço unitário | Preço por licença, conforme publicado na lista de preços no momento da compra. Verifique se esse preço corresponde às informações armazenadas em seu sistema de cobrança durante a reconciliação. |
| Quantity | Número de licenças. Verifique se esse preço corresponde às informações armazenadas em seu sistema de cobrança durante a reconciliação. |
| Tipo de unidade | O tipo de unidade em que o medidor é cobrado. Não disponível para a atividade atual. |
| Pré-imposto de cobrança | Valor total de cobrança antes dos impostos. |
| Moeda de cobrança | A moeda na região geográfica do cliente. |
| Preço custo total | O preço antes da adição de impostos. |
| Moeda de preços | A moeda na lista de preços. |
| Informações de serviço 1 | O número de conexões do barramento de serviço que foram provisionadas e utilizadas em um determinado dia. |
| Informações de serviço 2 | Um campo herdado que captura metadados específicos do serviço opcionais. |
| Informações adicionais | Quaisquer informações adicionais não abordadas em outras colunas. |
