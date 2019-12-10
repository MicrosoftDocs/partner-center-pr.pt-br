---
title: Arquivos de reconciliação com base em licença | Centro de parceiros
ms.topic: article
ms.date: 11/21/2019
description: Entenda os arquivos de reconciliação baseados em licença no Partner Center.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 617b49556851a4d9999e6294d61d79c4fe1befa1
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389814"
---
# <a name="license-based-reconciliation-files"></a>Arquivos de reconciliação baseados em licença

Aplica-se a:

- Partner Center
- Partner Center do Microsoft Cloud for US Government

Para reconciliar as alterações em relação aos pedidos de um cliente, compare o **Syndication_Partner_Subscription_Number** do arquivo de reconciliação com a **ID da assinatura** do Partner Center.

## <a name="fields-in-license-based-reconciliation-files"></a>Campos em arquivos de reconciliação com base em licença

| Column | Descrição | Valor de exemplo |
| ------ | ----------- | ------------ |
| PartnerID | Identificador exclusivo no formato GUID para uma entidade de cobrança específica. Não é necessário para reconciliação. O mesmo em todas as linhas. | *8ddd03642-test-test-test-46b58d356b4e* |
| CustomerID | Identificador exclusivo da Microsoft para o cliente no formato GUID. | *12ABCD34-001A-BCD2-987C-3210ABCD5678* |
| OrderID | Identificador exclusivo para um pedido na plataforma de cobrança da Microsoft. Pode ser útil identificar a ordem ao contatar o suporte. Não usado para reconciliação. | *566890604832738111* |
| SubscriptionID | Identificador exclusivo de uma assinatura na plataforma de cobrança da Microsoft. Pode ser útil identificar a assinatura ao entrar em contato com o suporte. Não usado para reconciliação. *Esse valor não é o mesmo que a **ID da assinatura** no console do administrador do parceiro. Consulte **SyndicationPartnerSubscriptionNumber** em vez disso.* | *usCBMgAAAAAAAAIA* |
| SyndicationPartnerSubscriptionNumber | Identificador exclusivo para assinaturas. Um cliente pode ter várias assinaturas para o mesmo plano. Essa coluna é importante para a análise de arquivo de reconciliação. Esse campo é mapeado para a **ID da assinatura** no console do administrador do parceiro. | *fb977ab5-test-test-test-24c8d9591708* |
| OfferID | Identificador de oferta exclusivo. Identificador de oferta padrão, conforme definido na lista de preços. *Esse valor não corresponde à **ID da oferta** da lista de preços. Consulte **DurableOfferID** em vez disso.* | *FE616D64-E9A8-40EF-843F-152E9BBEF3D1* |
| DurableOfferID | Identificador de oferta durável exclusiva, conforme definido na lista de preços. *Esse valor corresponde à **ID da oferta** da lista de preços.* | *1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C* |
| OfferName | O nome da oferta de serviço comprada pelo cliente, conforme definido na tabela de preços. | *Microsoft Office 365 (plano E3)* |
| SubscriptionStartDate | A data de início da assinatura. A hora é sempre o início do dia, 0:00. Esse campo é definido como o dia após o envio do pedido. Usado em conjunto com o **SubscriptionEndDate** para determinar: se o cliente ainda estiver no primeiro ano da assinatura ou se a assinatura tiver sido renovada para o ano seguinte. | *2/1/2019 0:00* |
| SubscriptionEndDate | A data de término da assinatura. A hora é sempre o início do dia, 0:00. *12 meses mais **x** dias após a data de início* para se alinhar com a data de cobrança do parceiro ou *12 meses a partir da data de renovação*. Na renovação, os preços são atualizados com a tabela de preços atual. Um comunicado ao cliente pode ser necessário antes da renovação automática. | *2/1/2019 0:00* |
| ChargeStartDate | Dia de início dos encargos. A hora é sempre o início do dia, 0:00. Usado para calcular os encargos diários (encargos*pro favorável* ) quando um cliente altera números de estação. | *2/1/2019 0:00* |
| ChargeEndDate | Dia do término dos encargos. A hora é sempre o fim do dia, 23:59. Usado para calcular os encargos diários (encargos*pro favorável* ) quando um cliente altera números de estação. | *2/28/2019 23:59* |
| ChargeType | O [tipo de encargo](recon-file-charge-types.md) ou ajuste. | Consulte [tipos de cobrança](recon-file-charge-types.md). |
| UnitPrice | Preço por estação, conforme publicado na lista de preços no momento da compra. Certifique-se de que isso corresponde às informações armazenadas em seu sistema de cobrança durante a reconciliação. | *6,82* |
| Quantity | Número de assentos. Certifique-se de que isso corresponde às informações armazenadas em seu sistema de cobrança durante a reconciliação. | *2* |
| Amount | Preço total por quantidade. Usado para verificar se o cálculo de valor corresponde à forma como você calcula esse valor para seus clientes. | *13,32* |
| TotalOtherDiscount | Valor de desconto aplicado a esses encargos. As licenças de produto incluídas com uma competência ou mapas, ou novas assinaturas qualificadas para um incentivo, também conterão um valor de desconto nesta coluna. | *2,32* |
| Subtotal | Total sem imposto. Verifica se o SUBTOTAL corresponde ao seu total esperado, no caso de um desconto. | *11* |
| Tax | Encargo do valor do imposto. Com base nas regras de imposto do mercado e em circunstâncias específicas. | *0* |
| TotalForCustomer | Total com imposto. Verifica se o imposto é cobrado na fatura. | *11* |
| Currency | Tipo de moeda. Cada entidade de cobrança tem somente uma moeda. Verifique se ele corresponde à sua primeira fatura. Verifique novamente após as principais atualizações da plataforma de cobrança. | *$* |
| CustomerName | Nome da organização do cliente, conforme relatado no Partner Center. *Campo muito importante para reconciliar a fatura com as informações do sistema.* | *Testar cliente A* |
| ID do MPN | Identificador de MPN do parceiro CSP. Veja [como discriminar por parceiro](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner). | *4390934* |
| ResellerMPNID | Identificador MPN do revendedor do registro para a assinatura. Veja [como discriminar por parceiro](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner). | *4390934* |
| DomainName | Nome de domínio do cliente. Este campo pode aparecer em branco até o segundo ciclo de cobrança. *Não use esse campo como um identificador exclusivo para o cliente. O cliente/parceiro pode atualizar o intuitivo ou o domínio padrão por meio do portal do Office 365.* | *example.onmicrosoft.com* |
| SubscriptionName | Apelido da Inscrição. Se nenhum apelido for especificado, o Partner Center usará o **offername**. | *PROJETO ONLINE* |
| SubscriptionDescription | O nome da oferta de serviço comprada pelo cliente, conforme definido na tabela de preços. (Este é um campo idêntico a **oferecer**.) | *PROJECT ONLINE PREMIUM SEM CLIENTE DO PROJETO* |