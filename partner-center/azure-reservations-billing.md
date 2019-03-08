---
title: Cobrança para reservas do Azure | Partner Center
ms.topic: article
ms.date: 10/29/2018
Description: Informações sobre a cobrança do Azure reservas.
author: LauraBrenner
ms.author: v-petand
keywords: Azure RI, instâncias reservadas do azure, reservas, vm, gerenciar, cobrança, compra
robots: noindex, nofollow
ms.localizationpriority: medium
ms.openlocfilehash: b32c0da58cefea764f7f0cb3adb6d3a13faa46b5
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2019
ms.locfileid: "57586899"
---
# <a name="microsoft-azure-reserved-vm-instances-billing"></a>Cobrança de Instâncias de VM Reservadas do Microsoft Azure

**Aplica-se a**

-  Partner Center
-  Portal do Microsoft Azure
-  Parceiros no CSP

Os parceiros do programa Cloud Solution Provider (CSP) podem oferecer a seus clientes instâncias reservadas em máquinas virtuais do Microsoft Azure. Os clientes podem reservar máquinas virtuais com antecedência – para termos de um ano ou três anos – e experimentar uma economia significativa no uso do Azure.   

Seus clientes pagam antecipadamente por Instâncias de VM Reservadas do Azure. Quando você comprar Instâncias de VM Reservadas do Azure em nome de um cliente, ,, receberá faturas e arquivos de reconciliação para esses encargos únicos. 

>[!IMPORTANT]
>Se você comprar Instâncias de VM Reservadas do Azure para um cliente em um mercado com uma moeda diferente da sua, a moeda de cobrança padrão se baseará no mercado do cliente, não em sua localização. Se você tiver clientes em vários mercados, receberá faturas separadas e arquivos de reconciliação para cada moeda em que os clientes precisam ser cobrados, permitindo que você envie faturas para seus clientes na moeda apropriada. 

Para acessar arquivos de reconciliação e notas fiscais de encargo único, selecione **cobrança** no Partner Center e selecione **uma vez**. 

Para obter informações mais gerais sobre a cobrança no programa Provedor de Soluções na Nuvem, consulte [Noções básicas de cobrança](billing-basics.md).

## <a name="azure-reserved-vm-instance-invoice-file-definitions"></a>Definições do arquivo de fatura de Instância de VM Reservada do Azure

**Informações gerais de cobrança**

|**Campo** |**Definição**|
|:----------------|:-----------------------------|
|EUA FEIN |O ID do Imposto Federal. |
|Cobrar de |O endereço comercial legal usado para fins fiscais. Para alterar esse endereço, vá para Configurações da conta > Perfil de cobrança do parceiro. |
|Encargos |Todos os encargos atuais. |
|Créditos |Créditos por atividade de reembolso desde a compra inicial. |
|Descontos |Descontos que podem ser aplicáveis a reservas Azure ou a outros itens no pedido do cliente. |
|Impostos |O total de imposto para os encargos atuais como o total no início da seção detalhes na página 2 da fatura. |
|Total dos encargos atuais |O valor devido em moeda de cobrança para o período de faturamento, pago no dia do vencimento. |
|Instruções de pagamento |Descreve quando e como pagar sua fatura, com base em sua região. Inclua o número de sua fatura quando efetuar o pagamento. |
|Nº da Fatura |O número da sua fatura. |
|Data da fatura |A data em que sua fatura foi gerada. |
|Termos de pagamento |Para as compras únicas, sempre será 60 dias. |
|Data do pagamento |Seu pagamento deve ser recebido até essa data. |


**Lista detalhada dos encargos de uso únicos**

|**Campo** |**Definição**|
|:----------------|:-----------------------------|
|Data |Data da compra. |
|Descrição |Nome do produto. |
|Quantidade |O número de produtos (reservas, por exemplo) comprados. |
|Preço unitário |Preço por produto (reserva, por exemplo). |
|Descontos |Qualquer desconto aplicável. |
|Valor pré-taxado |Subtotal das compras antes dos impostos. |
|Imposto sobre vendas |Valor do imposto. |
|Total |Total a ser pago. |


## <a name="azure-reserved-vm-instance-reconciliation-file-descriptions"></a>Descrições de arquivo de reconciliação de Instância de VM Reservada do Azure

|**Campo** |**Definição**|
|:----------------|:-----------------------------|
|PartnerID |ID do parceiro, no formato GUID. |
|CustomerID |ID exclusiva da Microsoft, no formato GUID, usada para identificar o cliente. |
|CustomerName |Nome da organização do cliente como informado no Partner Center. Isso é muito importante para reconciliar a fatura com as informações de seu sistema. |
|CustomerDomainName |O nome de domínio do cliente. |
|CustomerCountry |O país em que o cliente está localizado. |
|InvoiceNumber |Número da fatura na qual a transação especificada é exibida. |
|MpnID |ID do MPN do parceiro CSP (direto ou indireto). |
|ID do MPN do revendedor |Só aparece em arquivos de reconciliação para parceiros no modelo indireto. A ID do MPN do revendedor de registro da reserva. Isso corresponde à ID de revendedor listada para a reserva específica no Partner Center. Se um parceiro CSP vendeu a reserva diretamente para o cliente, sua ID do MPN estará listada duas vezes, como a ID do MPN e a ID do MPN do revendedor. Se um parceiro CSP tiver um revendedor sem ID do MPN, esse valor será definido como a ID do MPN do parceiro. Se o parceiro CSP remover uma ID de revendedor, esse valor será definido como -1. |
|OrderID |Identificador exclusivo para um pedido na plataforma de cobrança da Microsoft. Pode ser útil para identificar a reserva do Azure ao entrar em contato com o suporte, mas não para reconciliação. |
|OrderDate |A data em que o pedido foi feito. |
|ProductId |A ID do produto. |
|SkuId  |A ID de uma SKU em particular. |
|AvailabilityId |A ID de uma Disponibilidade em particular. "Disponibilidade" refere-se a se uma SKU em particular está disponível ou não para compra para determinado país, moeda, segmento do setor etc. |
|SkuName  |O título de uma SKU em particular. |
|ProductName |O nome do produto. |
|ChargeType |O tipo de encargo ou ajuste. |
|UnitPrice |Preço por produto pedido. |
|Quantidade |Número de produtos pedidos. |
|Subtotal |Total sem imposto. Verifica se seu subtotal corresponde ao total esperado, em caso de desconto. |
|TaxTotal |O total de todos os impostos aplicáveis. |
|Total |O valor total desta compra. |
|Currency |Tipo de moeda. Cada entidade de cobrança tem somente uma moeda. Verifique se isso coincide com a primeira fatura e faça o mesmo após grandes atualizações na plataforma de cobrança. |
|DiscountDetails |Lista detalhada dos descontos relevantes. |


## <a name="manage-your-billing"></a>Gerenciar sua cobrança

### <a name="view-your-current-billing-status-invoices-and-recon-files"></a>Exibir o status de cobrança, as faturas e os arquivos de reconhecimento atuais

1.  No Centro de parceiro, selecione **cobrança** e, em seguida **uma vez** para exibir seu status de cobrança. 
2.  Selecione uma fatura ou um arquivo de reconhecimento para exibir informações mais detalhadas. 

### <a name="view-a-customers-order-history"></a>Exibir o histórico de pedidos de um cliente

1.  Selecione **clientes** no menu do Partner Center.
2.  Na sua página **Clientes**, localize o cliente cujo histórico de pedidos você deseja exibir e, em seguida, selecione a seta para baixo para expandir o registro do cliente. 
3.  Selecione **Exibir pedidos** para exibir o histórico de pedidos.

### <a name="create-a-credit-or-void-note"></a>Criar uma nota de crédito ou cancelada

Em algum momento, talvez seja necessário anular uma fatura e então emitir uma nova. Por exemplo, um cliente pode alterar o nome da empresa dele e então receber uma fatura com o nome antigo. 

Para cancelar uma fatura e emitir uma nova, baixe o formulário da página de cobrança, sob ajustes.

## <a name="azure-reservations-resources"></a>Recursos de reservas do Azure
|**Para obter informações sobre**   |**Leia isto**    |
|:-----------------------------|:-----------------|
|Reservas do Azure na visão geral do CSP  | [Vende instâncias VM reservadas do Azure da Microsoft](azure-reservations.md)
|Comprar reservas do Azure para seus clientes no Partner Center   |[Comprar reservas do Azure](azure-reservations-buying.md)
| Gerenciando reservas do Azure no Partner Center | [Gerenciando reservas do Azure no Partner Center](azure-reservations-manage.md)
|Como comprar reservas do Azure no portal do Azure | [Pagar antecipadamente por máquinas virtuais com Instâncias de VM Reservadas do Azure](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) na Ajuda do Azure |
|Como gerenciar reservas do Azure no portal do Azure   |[Gerenciar instâncias de VM reservadas](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) na Ajuda do Azure  |
|Como comprar reservas do Azure usando a API do Partner Center | [Comprar Instâncias de VM Reservadas do Azure](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) na documentação do desenvolvedor do Partner Center

 
