---
title: Arquivos de reconciliação com base no uso | Centro de parceiros
ms.topic: article
ms.date: 01/14/2020
description: Todos os itens em seu arquivo de reconciliação baseado em uso explicado, com exemplos.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: e4ce3427f52ccde8f61fa553f3fa0af79bff0a95
ms.sourcegitcommit: fc43ee25d405ef3dc673edd884c877bfc62ad6aa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2020
ms.locfileid: "76021746"
---
# <a name="usage-based-file-fields"></a>Campos de arquivo baseado em uso

Aplica-se a:

- Partner Center
- Partner Center do Microsoft Cloud for US Government

Para reconciliar seus encargos em relação ao uso de um cliente, compare o **revendedorid**, o **revendedorname**e o **ResellerBillableAccount** do arquivo de reconciliação com o **nome do cliente** e a ID da **assinatura** do Partner Center.

## <a name="fields-in-usage-based-reconciliation-files"></a>Campos em arquivos de reconciliação com base no uso

Os campos a seguir explicam quais serviços foram usados e a taxa.

| Column | Descrição | Valor (es) de exemplo |
| ------ | ----------- | ------------ |
| PartnerID | Identificador de parceiro, no formato GUID. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| PartnerName | Nome do parceiro. | *Contoso, Ltd.* |
| PartnerBillableAccountId | Identificador de conta de parceiro. | *1010578050* |
| CustomerCompanyName | Nome da organização do cliente, conforme relatado no Partner Center. *Muito importante para reconciliar a fatura com as informações do sistema.* | *Cliente de teste* |
| MpnId | Identificador de MPN do parceiro CSP. | *4390934* |
| ResellerMpnId | Identificador MPN do revendedor do registro para a assinatura.  |
| InvoiceNumber | Número da fatura na qual a transação especificada é exibida. | *D020001IVK* |
| ChargeStartDate | Data de início do ciclo de faturamento, exceto ao apresentar datas de dados de uso latente anteriormente não cobertos (do ciclo de faturamento anterior). A hora é sempre o início do dia, 0:00. | *2/1/2019 0:00* |
| ChargeEndDate | Data final do ciclo de faturamento, exceto ao apresentar datas de dados de uso latente anteriormente não cobertos (do ciclo de faturamento anterior). A hora é sempre o fim do dia, 23:59. | *2/28/2019 23:59* |
| SubscriptionID | Identificador exclusivo de uma assinatura na plataforma de cobrança da Microsoft. Pode ser útil identificar a assinatura ao entrar em contato com o suporte. Não usado para reconciliação. *Isso não é o mesmo que a **ID da assinatura** no console do administrador do parceiro.* | *usCBMgAAAAAAAAIA* |
| SubscriptionName | Apelido para a oferta de serviço. | *Microsoft Azure* |
| SubscriptionDescription | Linha de negócios da oferta de serviço. | *Microsoft Azure* |
| OrderID | Identificador exclusivo para um pedido na plataforma de cobrança da Microsoft. Pode ser útil identificar a assinatura ao entrar em contato com o suporte. Não usado para reconciliação. | *566890604832738111* |
| ServiceName | O nome do serviço do Azure em questão. | *MÁQUINAS VIRTUAIS* |
| ServiceType | O tipo específico de serviço do Azure. | *Barramento de serviço – individual ou pacote*, *banco de dados SQL Azure – Business ou Web Edition* |
| ResourceGuid | Identificador exclusivo específico de toda a estrutura de serviço de dados e preço. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| ResourceName | O nome do recurso do Azure. | *Transferência de dados em (GB)* , *transferência de dados de saída (GB)* |
| Region | A região à qual o uso se aplica. Usado principalmente para atribuir taxas às transferências de dados, pois as tarifas variam por região. | *Pacífico Asiático*, *Europa*, *América Latina*, *América do Norte* |
| SKU | Identificador exclusivo da Microsoft para uma oferta. | *7UD-00001* |
| DetailLineItemId | Um identificador e uma quantidade para discriminar taxas diferentes para um serviço ou recurso em um determinado período de cobrança. Para preços em camadas do Azure, pode haver uma taxa de até uma determinada quantidade de unidades faturáveis e, em seguida, uma taxa diferente após essa quantidade. | *1* |
| ConsumedQuantity | A quantidade de serviço consumida (como horas ou GB) durante o período de relatório. Também inclui qualquer uso não cobrado de períodos de relatório anteriores. | *11* |
| IncludedQuantity | Unidades incluídas como parte da oferta. Normalmente não está presente no CSP. | *0* |
| OverageQuantity | Unidades não incluídas como parte da oferta. Eles devem ser pagos pelo parceiro. Igual a **ConsumedQuantity** menos **IncludedQuantity**. | *11* |
| ListPrice | Preço da oferta em vigor na data de início da assinatura. | *$0.808* |
| PretaxCharges | Igual a **ListPrist** multiplicado por **OverageQuantity**, arredondado para a cento mais próxima. | *$0.85* |
| TaxAmount | Valor de imposto cobrado. Com base nas regras de imposto do mercado e em circunstâncias específicas. | *$0.08* |
| PostTaxTotal | Total após imposto, quando o imposto é aplicável. | *$0.93* |
| Currency | Tipo de moeda. Cada entidade de cobrança tem somente uma moeda. Verifique se ele corresponde à sua primeira fatura e depois das principais atualizações da plataforma de cobrança. | *$* |
| PretaxEffectiveRate | Preço por unidade sem imposto. Igual a **PretaxCharges** dividido por **OverageQuantity**, arredondado para a cento mais próxima. | *$0.08* |
| PostTaxEffectiveRate | Preço pós-imposto por unidade. Igual a **PostTaxTotal** dividido por **OverageQuantity**, arredondado para a cento mais próxima. Ou, igual a **PretaxEffectiveRate** mais argumentos taxa de impostos por unidade Amoun, arredondado para a Centa mais próxima. | *$0.08* |
| ChargeType | O [tipo de encargo](recon-file-charge-types.md) ou ajuste. | Consulte [tipos de cobrança](recon-file-charge-types.md). |
| CustomerID | Identificador exclusivo da Microsoft para o cliente, no formato GUID. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| DomainName | Nome de domínio do cliente. Este campo pode aparecer em branco até o segundo ciclo de cobrança. | *example.onmicrosoft.com* |
| BillingCycleType | Frequência de cobrança de tempo.| **Mensalmente**  |
| Unidade | A unidade do **nome**do recurso. | *GB* ou *horas* |
| CustomerBillableAccount | Identificador de conta exclusivo na plataforma de cobrança da Microsoft. | *1280018095* |
| UsageDate | Data da implantação do serviço. | *2/1/2019 0:00* |
| MeteredRegion | Identifica o local de um data center dentro da região (para serviços em que esse valor é aplicável e preenchido). | *Ásia Oriental*, *sul Ásia Oriental*, *Europa Setentrional*, *Europa Ocidental*, *norte EUA Central*, *Sul EUA Central* |
| MeteredService | Identifica o uso individual do serviço do Azure quando ele não está especificamente identificado na coluna **ServiceName** . Por exemplo, as transferências de dados são relatadas como *Microsoft Azure-todos os serviços* na coluna **ServiceName** . | *AccessControl*, *CDN*, *computação*, *banco de dados*, *ServiceBus*, *armazenamento* |
| MeteredServiceType | Subtítulo para o campo **MeteredService** que fornece esclarecimentos adicionais sobre o uso do serviço do Azure. | *EXTERNAL* |
| Projeto | Nome definido pelo cliente para sua instância de serviço. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| ServiceInfo | O número de conexões do barramento de serviço do Azure que foram provisionadas e utilizadas em um determinado dia. | *1, 0 conexões/30 dias* (se você tiver uma conexão provisionada individualmente durante um mês de 30 dias), *25 conexões/30 dias – usado: 1, 0* (se você tiver um pacote de 25 pacotes de conexões de barramento de serviço provisionado e utilizado 1 durante esse dia) |
