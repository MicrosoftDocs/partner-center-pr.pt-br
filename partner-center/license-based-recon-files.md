---
title: Arquivos de reconciliação baseados em licença
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como ler arquivos de reconciliação baseados em licença no Partner Center. Este artigo explica o significado de cada campo em seu arquivo reconhecimento baseado em licença.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 117acfa8c50496ddaa75789b2bb3f55c642e4fe6
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702902"
---
# <a name="understand-the-fields-in-partner-center-license-based-reconciliation-files"></a>Entender os campos em arquivos de reconciliação baseados em licença do Partner Center

**Aplica-se a**

- Partner Center do Microsoft Cloud for US Government

**Funções apropriadas**

- Administrador global
- Administrador de gerenciamento de usuário
- Administrador de cobrança
- Agente administrativo

Para reconciliar as alterações em relação aos pedidos de um cliente, compare o **Syndication_Partner_Subscription_Number** do arquivo de reconciliação com a **ID da assinatura** do Partner Center.

## <a name="fields-in-license-based-reconciliation-files"></a>Campos em arquivos de reconciliação com base em licença

| Coluna | Descrição | Valor de exemplo |
| ------ | ----------- | ------------ |
| PartnerId | Identificador exclusivo no formato GUID para uma entidade de cobrança específica. Não é necessário para reconciliação. O mesmo em todas as linhas. | *8ddd03642-test-test-test-46b58d356b4e* |
| CustomerId | Identificador exclusivo da Microsoft para o cliente no formato GUID. | *12ABCD34-001A-BCD2-987C-3210ABCD5678* |
| CustomerName | Nome da organização do cliente, conforme relatado no Partner Center. *Campo muito importante para reconciliar a fatura com as informações do sistema.* | *Testar o cliente A* |
| MpnId | Identificador de MPN do parceiro CSP. Veja [como discriminar por parceiro](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner). | *4390934* |
| ResellerMpnId | Identificador MPN do revendedor do registro para a assinatura.  |
| OrderId | Identificador exclusivo para um pedido na plataforma de cobrança do Microsoft. Pode ser útil identificar a ordem ao contatar o suporte. Não usado para reconciliação. | *566890604832738111* |
| SubscriptionId | Identificador exclusivo de uma assinatura na plataforma de faturamento da Microsoft. Pode ser útil identificar a assinatura ao entrar em contato com o suporte. Não usado para reconciliação. *Esse valor não é o mesmo que a **ID da assinatura** no console do administrador do parceiro. Consulte **SyndicationPartnerSubscriptionNumber** em vez disso.* | *usCBMgAAAAAAAAIA* |
| SyndicationPartnerSubscriptionNumber | Identificador exclusivo para assinaturas. Um cliente pode ter várias assinaturas para o mesmo plano. Essa coluna é importante para a análise de arquivo de reconciliação. Esse campo é mapeado para a **ID da assinatura** no console do administrador do parceiro. | *fb977ab5-test-test-test-24c8d9591708* |
| OfferId | Identificador de oferta exclusivo. Identificador de oferta padrão, conforme definido na lista de preços. *Esse valor não corresponde à **ID da oferta** da lista de preços. Consulte **DurableOfferID** em vez disso.* | *FE616D64-E9A8-40EF-843F-152E9BBEF3D1* |
| DurableOfferId | Identificador de oferta durável exclusiva, conforme definido na lista de preços. *Esse valor corresponde à **ID da oferta** da lista de preços.* | *1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C* |
| OfferName | O nome da oferta de serviço comprada pelo cliente, conforme definido na tabela de preços. | *Microsoft Office 365 (plano E3)* |
| SubscriptionStartDate | A data de início da assinatura em UTC. A hora sempre é o início do dia, 0h00. Esse campo é definido como o dia após o envio do pedido. Usado com o **SubscriptionEndDate** para determinar: se o cliente ainda estiver dentro do primeiro ano da assinatura ou se a assinatura tiver sido renovada para o ano seguinte. | *2/1/2019 0:00* |
| SubscriptionEndDate | A data de término da assinatura em UTC. A hora sempre é o início do dia, 0h00. *12 meses mais **x** dias após a data de início* para se alinhar com a data de cobrança do parceiro ou *12 meses a partir da data de renovação*. Na renovação, os preços são atualizados com a tabela de preços atual. Um comunicado ao cliente pode ser necessário antes da renovação automática. | *2/1/2019 0:00* |
| ChargeStartDate | Dia de início dos encargos. A hora sempre é o início do dia, 0h00. Usado para calcular os encargos diários (encargos *pro favorável* ) quando um cliente altera os números de licença. | *2/1/2019 0:00* |
| Data final da cobrança | Dia do término dos encargos. A hora é sempre o fim do dia, 23:59. Usado para calcular os encargos diários (encargos *pro favorável* ) quando um cliente altera os números de licença. | *2/28/2019 23:59* |
| ChargeType | O [tipo de encargo](recon-file-charge-types.md) ou ajuste. | Consulte [tipos de cobrança](recon-file-charge-types.md). |
| UnitPrice | Preço por licença, conforme publicado na lista de preços no momento da compra. Certifique-se de que isso corresponde às informações armazenadas em seu sistema de cobrança durante a reconciliação. | *6,82* |
| Quantidade | Número de licenças. Certifique-se de que isso corresponde às informações armazenadas em seu sistema de cobrança durante a reconciliação. | *2* |
| Amount | Preço total por quantidade. Usado para verificar se o cálculo de valor corresponde à forma como você calcula esse valor para seus clientes. | *13.32* |
| TotalOtherDiscount | Valor de desconto aplicado a esses encargos. As licenças de produto incluídas com uma competência ou mapas, ou novas assinaturas qualificadas para um incentivo, também conterão um valor de desconto nesta coluna. | *2,32* |
| Subtotal | Total sem imposto. Verifica se o SUBTOTAL corresponde ao seu total esperado, no caso de um desconto. | *11* |
| Imposto | Encargo do valor do imposto. Com base nas regras de imposto do mercado e em circunstâncias específicas. | *0* |
| TotalForCustomer | Total com imposto. Verifica se o imposto é cobrado na fatura. | *11* |
| Moeda | Tipo de moeda. Cada entidade de cobrança tem apenas uma moeda. Verifique se ele corresponde à sua primeira fatura. Verifique novamente após as principais atualizações da plataforma de cobrança. | *EUR* |
| DomainName | Nome de domínio do cliente. Este campo pode aparecer em branco até o segundo ciclo de cobrança. *Não use esse campo como um identificador exclusivo para o cliente. O cliente/parceiro pode atualizar o intuitivo ou o domínio padrão por meio do portal do Office 365.* | *example.onmicrosoft.com* |
| SubscriptionName | Apelido da Inscrição. Se nenhum apelido for especificado, o Partner Center usará o **offername**. | *PROJETO ONLINE* |
| Descrição da assinatura | O nome da oferta de serviço comprada pelo cliente, conforme definido na tabela de preços. (Este é um campo idêntico a **oferecer**.) | *PREMIUM ONLINE DO PROJETO SEM CLIENTE DO PROJECT* |
| BillingCycleType | Frequência de cobrança única.| *Mensalmente* |
