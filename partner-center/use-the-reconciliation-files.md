---
title: Usar os arquivos de reconciliação | Partner Center
ms.topic: article
ms.date: 07/08/2019
description: Para obter uma exibição detalhada de item de linha de cada encargo em um ciclo de cobrança, baixe os arquivos de reconciliação do Partner Center.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 8fae84790aa84b3c5a006d65a632668a33ac24a7
ms.sourcegitcommit: bae29ab191c72e15259d99c40c69a9e7c3f2b502
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/06/2019
ms.locfileid: "68820560"
---
# <a name="use-the-reconciliation-files"></a>Usar os arquivos de reconciliação

**Aplica-se a**

-  Partner Center
-  Partner Center para Microsoft Cloud for US Government


Para obter uma exibição detalhada de item de linha de cada encargo em um ciclo de cobrança, baixe os arquivos de reconciliação do Partner Center. Os detalhes incluem encargos por assinaturas de cada cliente e eventos detalhados (como a adição de assentos a uma assinatura no meio do período).

## <a name="formatting-issues"></a>Problemas de formatação

Ocasionalmente, seu arquivo reconhecimento pode ter problemas de formatação. (Isso pode acontecer, por exemplo, se a localidade EN-US não for usada.) Siga as etapas abaixo para corrigir esses problemas. 

<ol>
<li>Abra o arquivo. csv no Excel e selecione a primeira coluna. Na faixa de opções, selecione <strong>dados</strong>e, em seguida, selecione <strong>texto para colunas</strong>.</li>

<li>No assistente converter texto em colunas, selecione <strong>tipo de arquivo delimitado</strong>e, em seguida, selecione <strong>Avançar</strong>.</li> 

<li>No campo delimitadores, selecione <strong>vírgula</strong>. Se a <strong>guia</strong> já estiver selecionada, você poderá deixá-la. Selecione <strong>Avançar</strong>.</li>

<li>No campo formato de dados da coluna, <strong>selecione Data: MDY</strong>e, em seguida, selecione <strong>Avançar</strong>.</li> 

<li>No campo formato de dados da coluna, selecione <strong>texto</strong> para todas as colunas de valor e, em seguida, selecione <strong>concluir</strong>.</li>
</ol>

## <a name="downloading-a-large-recon-file"></a>Baixando um arquivo reconhecimento grande

Os arquivos reconhecimento podem crescer muito e, às vezes, são difíceis de baixar. Para obter um script do PowerShell para ajudar a baixar arquivos grandes do reconhecimento, consulte [obter itens de linha da fatura](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).

## <a href="" id="itemizebypartner"></a>Discriminar por parceiro


Os parceiros no modelo indireto podem usar esses campos adicionais nos arquivos de reconciliação baseados em uso e em licença para discriminar por revendedor.

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>ID do MPN</th>
<th>Descrição</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>ID do MPN</td>
<td><p>A ID do Microsoft Partner Network (MPN) do parceiro CSP (direta ou indireta).</p></td>
</tr>
<tr class="even">
<td>ID do MPN do revendedor</td>
<td><p>Só aparece em arquivos de reconciliação para parceiros no modelo indireto.</p>
<p>A ID do MPN do revendedor de registro da assinatura. Isso corresponde à ID de revendedor listada para a assinatura específica no Partner Center.</p>
<p>eTo exibir ou atualizar o revendedor, no menu do centro de parceiros, selecione <strong>clientes</strong>e, em seguida, escolha o cliente na lista. No menu do cliente, selecione <strong>Assinaturas</strong>, escolha a assinatura na lista. Selecione <strong>Atualizar</strong> para alterar o <strong>Revendedor (ID do MPN)</strong>.</p>
<p>Se um parceiro CSP vendeu a assinatura diretamente para o cliente, sua ID do MPN estará listada duas vezes, como a ID do MPN e a ID do MPN do revendedor.</p>
<p>Se um parceiro CSP tiver um revendedor sem ID do MPN, esse valor será definido como a ID do MPN do parceiro.</p>
<p>Se o parceiro CSP remover uma ID de revendedor, esse valor será definido como -1.</p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a>Campos de arquivo com base em licença


Para reconciliar seus encargos com os pedidos de seu cliente, compare o campo Syndication\_Partner\_Subscription\_Number do arquivo de reconciliação com a ID de Assinatura do Partner Center.

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>Coluna</strong></td>
<td><strong>Descrição</strong></td>
<td><strong>Valor de exemplo</strong></td>
</tr>
<tr class="even">
<td>PartnerID</td>
<td><p>Identificador exclusivo de uma entidade de cobrança específica, em formato GUID. Não é necessário para reconciliação, mas pode ser uma informação útil. O mesmo em todas as linhas.</p></td>
<td>8ddd03642-test-test-test-46b58d356b4e</td>
</tr>
<tr class="odd">
<td>CustomerID</td>
<td><p>ID exclusiva da Microsoft, no formato GUID, usada para identificar o cliente.</p></td>
<td>12ABCD34-001A-BCD2-987C-3210ABCD5678</td>
</tr>
<tr class="even">
<td>OrderID</td>
<td><p>Identificador exclusivo para um pedido na plataforma de cobrança da Microsoft. Pode ser útil para identificar o pedido ao entrar em contato com o suporte, mas não para reconciliação.</p></td>
<td>566890604832738111</td>
</tr>
<tr class="odd">
<td>SubscriptionID</td>
<td><p>Identificador exclusivo de uma assinatura na plataforma de cobrança da Microsoft. Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</p>
<p>Esse não é o mesmo que o ID da assinatura no Partner Admin Console. Consulte Número_Assinatura_Parceiro_Sindicalização.</p></td>
<td>usCBMgAAAAAAAAIA</td>
</tr>
<tr class="even">
<td>SyndicationPartnerSubscriptionNumber</td>
<td><p>Identificador exclusivo para assinaturas. Target: Um cliente pode ter várias assinaturas para o mesmo plano, portanto, isso é importante para análise de arquivo de reconciliação.</p>
<p>Esse campo é mapeado para a ID da assinatura no Partner Admin Console.</p></td>
<td>fb977ab5-test-test-test-24c8d9591708</td>
</tr>
<tr class="odd">
<td>OfferID</td>
<td><p>ID exclusivo da oferta. ID padrão da oferta de acordo com a lista de preços.</p>
<p><b>Observação</b>: Esse valor não corresponde à ID da oferta da lista de preços. Veja DurableOfferID abaixo.</p></td>
<td>FE616D64-E9A8-40EF-843F-152E9BBEF3D1</td>
</tr>
<tr class="even">
<td>DurableOfferID</td>
<td><p>ID exclusivo da oferta durável, conforme definido na tabela de preços.</p>
<p><b>Observação</b>: Esse valor corresponde à ID da oferta da lista de preços.</p></td>
<td>1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</td>
</tr>
<tr class="odd">
<td>OfferName</td>
<td><p>O nome da oferta de serviço comprada pelo cliente, conforme definido na tabela de preços.</p></td>
<td>Microsoft Office 365 (plano E3)</td>
</tr>
<tr class="even">
<td>SubscriptionStartDate</td>
<td><p>A data de início da assinatura, definida como um dia após o pedido ser enviado. Verificando a data de início da assinatura em conjunto com a data de término, você pode determinar se o cliente está dentro do primeiro ano da assinatura ou se a assinatura foi renovada para o ano seguinte.</p>
<p>A hora é sempre o início do dia, 0:00.</p></td>
<td>1/2/2015 0:00</td>
</tr>
<tr class="odd">
<td>SubscriptionEndDate</td>
<td><p>A data de término da assinatura: 12 meses + x dias após a data de início (para alinhar com a data de cobrança do parceiro) ou 12 meses a partir da data de renovação.</p>
<p>Na renovação, os preços são atualizados com a tabela de preços atual. Um comunicado ao cliente pode ser necessário antes da renovação automática.</p>
<p>A hora é sempre o início do dia, 0:00.</p></td>
<td>1/2/2015 0:00</td>
</tr>
<tr class="even">
<td>ChargeStartDate</td>
<td><p>Dia de início dos encargos.</p>
<p>Quando o cliente muda o número de assentos, esse número é usado para calcular os encargos por dia (pro-rata).</p>
<p>A hora é sempre o início do dia, 0:00.</p></td>
<td>1/2/2015 0:00</td>
</tr>
<tr class="odd">
<td>ChargeEndDate</td>
<td><p>Dia do término dos encargos.</p>
<p>Quando o cliente muda o número de assentos, esse número é usado para calcular os encargos por dia (pro-rata).</p>
<p>A hora é sempre o fim do dia, 23:59.</p></td>
<td>28/2/2015 23:59</td>
</tr>
<tr class="even">
<td>ChargeType</td>
<td><p>O tipo de encargo ou ajuste. Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></p></td>
<td><p>Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></p></td>
</tr>
<tr class="odd">
<td>UnitPrice</td>
<td><p>Preço por estação, conforme publicado na lista de preços no momento da compra. Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</p></td>
<td>6.82</td>
</tr>
<tr class="even">
<td>Quantidade</td>
<td><p>Número de assentos. Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</p></td>
<td>2</td>
</tr>
<tr class="odd">
<td>Valor</td>
<td><p>Preço total por quantidade. Útil para verificar se o cálculo do valor coincide com a forma como você calcula isso para seus clientes.</p></td>
<td>13.32</td>
</tr>
<tr class="even">
<td>TotalOtherDiscount</td>
<td><p>Valor de desconto aplicado a esses encargos. As licenças de produto incluídas com uma competência ou mapas ou novas assinaturas qualificadas para um incentivo também conterão um valor de desconto nesta coluna.</p></td>
<td>2.32</td>
</tr>
<tr class="odd">
<td>Subtotal</td>
<td><p>Total sem imposto. Verifica se seu subtotal corresponde ao total esperado, em caso de desconto.</p></td>
<td>11</td>
</tr>
<tr class="even">
<td>Tax</td>
<td><p>Valor do imposto, com base nas regras&#39;de imposto de s do mercado e em circunstâncias específicas.</p></td>
<td>0</td>
</tr>
<tr class="odd">
<td>TotalForCustomer</td>
<td><p>Total com imposto. Verifica se o imposto é cobrado na fatura.</p></td>
<td>11</td>
</tr>
<tr class="even">
<td>Currency</td>
<td><p>Tipo de moeda. Cada entidade de cobrança tem somente uma moeda. Verifique se isso coincide com a primeira fatura e faça o mesmo após grandes atualizações na plataforma de cobrança.</p></td>
<td>EUR</td>
</tr>
<tr class="odd">
<td>CustomerName</td>
<td><p>Nome&#39;da organização do cliente como relatado no Partner Center. Isso é muito importante para reconciliar a fatura com as informações de seu sistema.</p></td>
<td>Cliente de teste A</td>
</tr>
<tr class="even">
<td>ID do MPN</td>
<td><p>ID do MPN do parceiro CSP</p></td>
<td>4390934</td>
</tr>
<tr class="odd">
<td>ResellerMPNID</td>
<td><p>ID do MPN do revendedor de registro da assinatura. Consulte <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Discriminar por parceiro</a>.</p></td>
<td>4390934</td>
</tr>
<tr class="even">
<td>DomainName</td>
<td><p>Nome&#39;de domínio do cliente, usado para ajudar a identificar o cliente. Isso não deve ser usado para identificar exclusivamente o cliente, pois o cliente/parceiro pode atualizar o domínio intuitivo/padrão por meio do portal do O365. Este campo pode aparecer em branco até o segundo ciclo de cobrança.</p></td>
<td>example.onmicrosoft.com</td>
</tr>
<tr class="odd">
<td>SubscriptionName</td>
<td><p>Apelido da Inscrição. Se nenhum apelido for especificado, o Partner Center usa o OfferName.</p></td>
<td>PROJETO ONLINE</td>
</tr>
<tr class="even">
<td>SubscriptionDescription</td>
<td><p>O nome da oferta de serviço comprada pelo cliente, conforme definido na tabela de preços. (Este é um campo idêntico ao nome da oferta).</p></td>
<td>PROJETO ONLINE PREMIUM SEM PROJETO CLIENTE</td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a>Campos de arquivo com base no uso


Para reconciliar seus encargos com o uso de seu cliente, compare ResellerID/ResellerName/ResellerBillableAccount do arquivo de reconciliação com o nome do cliente e a ID da assinatura do Partner Center.

Os campos a seguir explicam quais serviços foram usados e a taxa.

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>Coluna</strong></td>
<td><strong>Descrição</strong></td>
<td><strong>Valor de exemplo</strong></td>
</tr>
<tr class="even">
<td>PartnerID</td>
<td><p>ID do parceiro, no formato GUID.</p></td>
<td>DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</td>
</tr>
<tr class="odd">
<td>PartnerName</td>
<td><p>Nome do parceiro.</p></td>
<td>Acme incorporado</td>
</tr>
<tr class="even">
<td>PartnerBillableAccountID</td>
<td><p>ID da conta do parceiro.</p></td>
<td>1010578050</td>
</tr>
<tr class="odd">
<td>CustomerName</td>
<td><p>Nome&#39;da organização do cliente como relatado no Partner Center. Isso é muito importante para reconciliar a fatura com as informações de seu sistema.</p></td>
<td>Cliente de teste A</td>
</tr>
<tr class="even">
<td>ID do MPN</td>
<td><p>ID do MPN do parceiro CSP.</p></td>
<td>4390934</td>
</tr>
<tr class="odd">
<td>ResellerMPNID</td>
<td><p>ID do MPN do revendedor de registro da assinatura. Consulte <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Discriminar por parceiro</a>.</p></td>
<td>4390934</td>
</tr>
<tr class="even">
<td>InvoiceNumber</td>
<td><p>Número da fatura na qual a transação especificada é exibida.</p></td>
<td>D020001IVK</td>
</tr>
<tr class="odd">
<td>ChargeStartDate</td>
<td><p>Data de início do ciclo de cobrança exceto quando apresentadas as datas de dados de uso latentes anteriormente não cobradas (do ciclo de cobrança anterior).</p>
<p>A hora é sempre o início do dia, 0:00.</p></td>
<td>1/2/2014 0:00</td>
</tr>
<tr class="even">
<td>ChargeEndDate</td>
<td><p>Data de término do ciclo de cobrança exceto quando apresentadas as datas de dados de uso latentes anteriormente não cobradas (do ciclo de cobrança anterior).</p>
<p>A hora é sempre o fim do dia, 23:59.</p></td>
<td>28/2/2014 23:59</td>
</tr>
<tr class="odd">
<td>SubscriptionID</td>
<td><p>Identificador exclusivo de uma assinatura na plataforma de cobrança da Microsoft. Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</p>
<p>Esse não é o mesmo que o ID da assinatura no Partner Admin Console.</p></td>
<td>usCBMgAAAAAAAAIA</td>
</tr>
<tr class="even">
<td>SubscriptionName</td>
<td><p>Apelido da oferta do serviço.</p></td>
<td>Microsoft Azure</td>
</tr>
<tr class="odd">
<td>SubscriptionDescription</td>
<td><p>Linha de negócios da oferta do serviço</p></td>
<td>Microsoft Azure</td>
</tr>
<tr class="even">
<td>OrderID</td>
<td><p>Identificador exclusivo para um pedido na plataforma de cobrança da Microsoft. Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação.</p></td>
<td>566890604832738111</td>
</tr>
<tr class="odd">
<td>ServiceName</td>
<td><p>O nome do serviço do Azure em questão.</p></td>
<td>MÁQUINAS VIRTUAIS</td>
</tr>
<tr class="even">
<td>ServiceType</td>
<td><p>O tipo específico de serviço do Windows Azure.</p></td>
<td><ul>
<li>Service Bus – Individual ou pacote</li>
<li>Banco de dados SQL Azure – Edição empresa ou Web</li>
</ul></td>
</tr>
<tr class="odd">
<td>ResourceGUID</td>
<td><p>Identificador exclusivo específico de toda a estrutura de serviço de dados e preço.</p></td>
<td>DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</td>
</tr>
<tr class="even">
<td>Nome do recurso</td>
<td><p>O nome do recurso do Azure.</p></td>
<td><ul>
<li>Dados de entrada transferidos (GB)</li>
<li>Dados de saída transferidos (GB)</li>
</ul></td>
</tr>
<tr class="odd">
<td>Região</td>
<td><p>A região a qual o uso se aplica. Usado principalmente para atribuir as taxas de transferências de dados, já que as taxas variam de acordo com a região.</p></td>
<td>Pacífico Asiático, Europa, América Latina e América do Norte</td>
</tr>
<tr class="even">
<td>SKU</td>
<td><p>Identificador exclusivo MSFT da oferta</p></td>
<td>7UD-00001</td>
</tr>
<tr class="odd">
<td><p>DetailLineItemId</p></td>
<td><p>Uma ID e a quantidade para discriminar as taxas diferentes de um serviço ou recurso em um determinado período de cobrança. Para a classificação em camadas do Azure, pode haver uma taxa para uma determinada quantidade de unidades faturáveis e uma taxa diferente depois disso.</p></td>
<td>1</td>
</tr>
<tr class="even">
<td>ConsumedQuantity</td>
<td><p>A quantidade de serviço consumida (horas, GB etc.) durante o período de relatório.</p>
<p>Também inclui qualquer uso não cobrado de períodos de relatório anteriores.</p></td>
<td>11</td>
</tr>
<tr class="odd">
<td>IncludedQuantity</td>
<td><p>Unidades incluídas como parte da oferta. Normalmente não está presente no CSP.</p></td>
<td>0</td>
</tr>
<tr class="even">
<td><p>OverageQuantity</p></td>
<td><p>Unidades não incluídas como parte da oferta devem ser pagas pelo parceiro.</p>
<p>Igual a ConsumedQuantity - IncludedQuantity.</p></td>
<td>11</td>
</tr>
<tr class="odd">
<td>ListPrice</td>
<td><p>Preço da oferta em vigor na data de início da assinatura.</p></td>
<td>U$ 0,0808</td>
</tr>
<tr class="even">
<td>PretaxCharges</td>
<td><p>ListPrist vezes OverageQuantity, arredondado para o centavo mais próximo.</p></td>
<td>U$ 0,085</td>
</tr>
<tr class="odd">
<td>TaxAmount</td>
<td><p>Valor do imposto, com base nas regras&#39;de imposto de s do mercado e em circunstâncias específicas.</p></td>
<td>U$ 0,08</td>
</tr>
<tr class="even">
<td>PostTaxTotal</td>
<td><p>Total após imposto, quando o imposto é aplicável.</p></td>
<td>U$ 0,93</td>
</tr>
<tr class="odd">
<td>Currency</td>
<td><p>Tipo de moeda. Cada entidade de cobrança tem somente uma moeda. Verifique se isso coincide com a primeira fatura e faça o mesmo após grandes atualizações na plataforma de cobrança.</p></td>
<td>EUR</td>
</tr>
<tr class="even">
<td>PretaxEffectiveRate</td>
<td><p>Preço por unidade sem imposto. Igual a PretaxCharges / OverageQuantity, arredondado para o centavo mais próximo.</p></td>
<td>U$ 0,08</td>
</tr>
<tr class="odd">
<td>PostTaxEffectiveRate</td>
<td><p>Preço pós-imposto por unidade. Igual a PostTaxTotal / OverageQuantity, ou PretaxEffectiveRate + taxa de imposto por valor de unidade, arredondado para o centavo mais próximo.</p></td>
<td>U$ 0,08</td>
</tr>
<tr class="even">
<td>ChargeType</td>
<td><p>O tipo de encargo ou ajuste. Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></p></td>
<td><p>Consulte <a href="#charge_types">mapeando encargos entre uma fatura e o arquivo de reconciliação</a></p></td>
</tr>
<tr class="odd">
<td>CustomerBillableAccount</td>
<td><p>ID exclusiva da conta na plataforma de cobrança da MSFT.</p></td>
<td>1280018095</td>
</tr>
<tr class="even">
<td>UsageDate</td>
<td><p>Data da implantação do serviço.</p></td>
<td>1/2/2014 0:00</td>
</tr>
<tr class="odd">
<td>MeteredRegion</td>
<td><p>Essa coluna identifica a localização de um data center dentro da região para serviços onde isso é aplicável e preenchido.</p></td>
<td>Leste da Ásia, Sudeste da Ásia, Norte da Europa, Europa Ocidental, Centro Norte e Centro Sul dos EUA</td>
</tr>
<tr class="even">
<td>MeteredService</td>
<td><p>Essa coluna é utilizada para rastrear o serviço do Microsoft Azure individual que não pode ser identificado especificamente na coluna Nome do Serviço. Por exemplo, transferências de dados são relatadas como &quot;Microsoft Azure – Todos os Serviços&quot; na coluna Nome do Serviço. Essa coluna MeteredService indicará ao qual serviço específico o uso pertence.</p></td>
<td>AccessControl, CDN, Computação, Banco de dados, ServiceBus, Armazenamento</td>
</tr>
<tr class="odd">
<td>MeteredServiceType</td>
<td><p>Um subcabeçalho que esclarece ainda mais o serviço Microsoft Azure individual além do nível fornecido pelo campo MeteredService.</p></td>
<td>EXTERNO</td>
</tr>
<tr class="even">
<td>Projeto</td>
<td><p>Nome definido pelo cliente para a instância do serviço</p></td>
<td>ORDDC52E52FDEF405786F0642DD0108BE4</td>
</tr>
<tr class="odd">
<td>ServiceInfo</td>
<td><p>O número de conexões ServiceBus que foram provisionados e utilizados em um dia específico.</p></td>
<td>Por exemplo: se você tivesse uma conexão individualmente provisionada durante um mês de 30 dias, a coluna Informação do Serviço 1 lerá "1,000000 conexões/30 dias". Se você tiver um pacote de 25 pacotes de conexões do ServiceBus provisionado e tiver utilizado 1 durante esse dia, sua instrução de uso diário para esse dia indicaria "25 conexões/30 dias – usado: 1, 0 ".</td>
</tr>
<tr class="even">
<td>CustomerID</td>
<td><p>ID exclusiva da Microsoft, no formato GUID, usada para identificar o cliente.</p></td>
<td>ORDDC52E52FDEF405786F0642DD0108BE4</td>
</tr>
<tr class="odd">
<td>DomainName</td>
<td><p>Nome&#39;de domínio do cliente, usado para ajudar a identificar o cliente. Este campo pode aparecer em branco até o segundo ciclo de cobrança.</p></td>
<td>example.onmicrosoft.com</td></tr>
</tr>
<tr class="even">
<td>Unidade</td>
<td><p>A unidade do nome do recurso</p></td>
<td>GB ou HORAS</td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a>Campos de arquivo de uso único e recorrente

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Column</th>
<th>Descrição</th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td>PartnerID</td>
<td><p>Identificador de locatário de Microsoft Azure Active Directory exclusivo para uma entidade de cobrança específica, no formato GUID. Não é necessário para reconciliação, mas pode ser uma informação útil. O mesmo em todas as linhas.</p></td>
</tr>

<tr class="even">
<td>ID do cliente</td>
<td><p>ID de locatário de Microsoft Azure Active Directory exclusiva, no formato GUID, usada para identificar o cliente.</p></td>
</tr>

<tr class="odd">
<td>Nome do cliente</td>
<td><p>Nome da organização do cliente como informado no Partner Center.</p></td>
</tr>

<tr class="even">
<td>CustomerDomainName</td>
<td><p>Nome de domínio do cliente, usado para ajudar a identificar o cliente. Isso não deve ser usado para identificar exclusivamente o cliente, pois o cliente/parceiro pode atualizar o domínio intuitivo/padrão por meio do portal do O365. Este campo pode aparecer em branco até o segundo ciclo de cobrança.</p></td>
</tr>

<tr class="odd">
<td>País do cliente</td>
<td><p>O país em que o cliente está localizado.</p></td>
</tr>

<tr class="even">
<td>Número da fatura</td>
<td><p>Número da fatura na qual a transação especificada é exibida.</p></td>
</tr>

<tr class="odd">
<td>MpnID</td>
<td><p>ID do MPN do parceiro CSP.</p></td>
</tr>

<tr class="even">
<td>MpnId do revendedor</td>
<td><p>ID do MPN do revendedor de registro da assinatura.</p></td>
</tr>

<tr class="odd">
<td>ID do Pedido</td>
<td><p>Identificador exclusivo de um pedido na plataforma Microsoft Commerce. Pode ser útil para identificar o pedido ao entrar em contato com o suporte, mas não para reconciliação.</p></td>
</tr>

<tr class="even">
<td>Data do pedido</td>
<td><p>A data em que o pedido foi feito.</p></td>
</tr>

<tr class="odd">
<td>ProductId</td>
<td><p>A ID do produto.</p></td>
</tr>

<tr class="even">
<td>SkuId</td>
<td><p>A ID de uma SKU em particular.</p></td>
</tr>

<tr class="odd">
<td>AvailabilityId</td>
<td><p>A ID de uma Disponibilidade em particular. "Disponibilidade" refere-se a se uma SKU em particular está disponível ou não para compra para determinado país, moeda, segmento do setor etc.</p></td>
</tr>

<tr class="even">
<td>Nome do SKU</td>
<td><p>O título de uma SKU em particular.</p></td>
</tr>

<tr class="odd">
<td>Nome do produto</td>
<td><p>O nome do produto.</p></td>
</tr>

<tr class="even">
<td>PublisherName</td>
<td><p>O nome do editor do produto.</p></td>
</tr>

<tr class="odd">
<td>PublisherID</td>
<td><p>ID exclusiva para este Publicador.</p></td>
</tr>

<tr class="even">
<td>Descrição da assinatura</td>
<td><p>Nome amigável de uma assinatura.</p></td>
</tr>

<tr class="odd">
<td>ID da assinatura</td>
<td><p>Identificador exclusivo de uma assinatura na plataforma Microsoft Commerce. Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação. Esse não é o mesmo que o ID da assinatura no Partner Admin Console.</p></td>
</tr>

<tr class="even">
<td>ChargeStartDate</td>
<td><p>Dia de início dos encargos. A hora é sempre o início do dia, 0:00.</p></td>
</tr>

<tr class="odd">
<td>ChargeEndDate</td>
<td><p>Dia do término dos encargos. A hora é sempre o fim do dia, 23:59.</p></td>
</tr>

<tr class="even">
<td>Termo e Billingcycle</td>
<td><p>O tamanho do termo e o ciclo de cobrança da compra. Por exemplo, "1 ano, mensalmente."</p></td>
</tr>

<tr class="odd">
<td>Tipo de Cobrança</td>
<td><p>O tipo de encargo ou ajuste.</p></td>
</tr>

<tr class="even">
<td>Preço unitário</td>
<td><p>O preço como publicado na tabela de preços no momento da compra. Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</p></td>
</tr>

<tr class="odd">
<td>Preço unitário efetivo</td>
<td><p>O preço unitário após os ajustes terem sido feitos.</p></td>
</tr>

<tr class="even">
<td>Quantidade</td>
<td><p>Número de unidades. Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</p></td>
</tr>

<tr class="odd">
<td>Tipo de unidade</td>
<td><p>O tipo de unidade que está sendo adquirida.</p></td>
</tr>

<tr class="even">
<td>DiscountDetails</td>
<td><p>Uma explicação de qualquer desconto aplicável.</p></td>
</tr>

<tr class="odd">
<td>Subtotal</td>
<td><p>Total sem imposto. Verifica se seu subtotal corresponde ao total esperado, em caso de desconto.</p></td>
</tr>

<tr class="even">
<td>Total do imposto</td>
<td><p>Valor do imposto cobrado, com base nas regras fiscais do mercado e em circunstâncias específicas.</p></td>
</tr>

<tr class="odd">
<td>Total</td>
<td><p>Total com imposto. Verifica se o imposto é cobrado na fatura.</p></td>
</tr>

<tr class="even">
<td>Currency</td>
<td><p>Tipo de moeda. Cada entidade de cobrança tem somente uma moeda. Verifique se isso coincide com a primeira fatura e faça o mesmo após grandes atualizações na plataforma de cobrança.</p></td>
</tr>

<tr class="odd">
<td>Uma alternateid</td>
<td><p>Um identificador alternativo para uma ID de pedido.</p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a>Campos de arquivo de uso com classificação diária


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Column</th>
<th>Descrição</th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td>PartnerID</td>
<td><p>ID do parceiro, no formato GUID.</p></td>
</tr>

<tr class="even">
<td>PartnerName</td>
<td><p>Nome do parceiro.</p></td>
</tr>

<tr class="odd">
<td>CustomerID</td>
<td><p>ID exclusiva da Microsoft, no formato GUID, usada para identificar o cliente.</p></td>
</tr>

<tr class="even">
<td>CustomerCompanyName</td>
<td><p>Nome da organização do cliente como informado no Partner Center. Isso é muito importante para reconciliar a fatura com as informações de seu sistema.</p></td>
</tr>

<tr class="odd">
<td>CustomerDomainName</td>
<td><p>O nome de domínio do cliente. Não disponível para a atividade atual.</p></td>
</tr>

<tr class="even">
<td>País do cliente</td>
<td><p>O país em que o cliente está localizado.</p></td>
</tr>

<tr class="odd">
<td>ID do MPN</td>
<td><p>ID do MPN do parceiro CSP.</p></td>
</tr>

<tr class="even">
<td>MPNID do revendedor</td>
<td><p>ID do MPN do revendedor de registro da assinatura. Não disponível para a atividade atual.</p></td>
</tr>

<tr class="odd">
<td>InvoiceNumber</td>
<td><p>Número da fatura na qual a transação especificada é exibida. Não disponível para a atividade atual.</p></td>
</tr>

<tr class="even">
<td>ProductId</td>
<td><p>A ID do produto.</p></td>
</tr>

<tr class="odd">
<td>SkuId</td>
<td><p>A ID de uma SKU em particular.</p></td>
</tr>

<tr class="even">
<td>AvailabilityId</td>
<td><p>A ID de uma Disponibilidade em particular. "Disponibilidade" refere-se a se uma SKU em particular está disponível ou não para compra para determinado país, moeda, segmento do setor etc.</p></td>
</tr>

<tr class="odd">
<td>Nome do SKU</td>
<td><p>O título de uma SKU em particular.</p></td>
</tr>

<tr class="even">
<td>PublisherName</td>
<td><p>O nome do Publicador.</p></td>
</tr>

<tr class="odd">
<td>PublisherID</td>
<td><p>A ID do Publicador, no formato GUID. Não disponível para a atividade atual.</p></td>
</tr>

<tr class=”even">
<td>Descrição da assinatura</td>
<td><p>O nome da oferta de serviço comprada pelo cliente, conforme definido na tabela de preços. (Este é um campo idêntico ao nome da oferta).</p></td>
</tr>

<tr class="odd">
<td>ID da assinatura</td>
<td><p>Identificador exclusivo de uma assinatura na plataforma de cobrança da Microsoft. Pode ser útil para identificar a assinatura ao entrar em contato com o suporte, mas não para reconciliação. Esse não é o mesmo que o ID da assinatura no Partner Admin Console.</p></td>
</tr>

<tr class="even">
<td>ChargeStartDate</td>
<td><p>Data de início do ciclo de cobrança exceto quando apresentadas as datas de dados de uso latentes anteriormente não cobradas (do ciclo de cobrança anterior). A hora é sempre o início do dia, 0:00.</p></td>
</tr>

<tr class="odd">
<td>ChargeEndDate</td>
<td><p>Data de término do ciclo de cobrança exceto quando apresentadas as datas de dados de uso latentes anteriormente não cobradas (do ciclo de cobrança anterior). A hora é sempre o fim do dia, 23:59.</p></td>
</tr>

<tr class="even">
<td>Data de uso</td>
<td><p>Data de uso do serviço.</p></td>
</tr>

<tr class="odd">
<td>Tipo de medidor</td>
<td><p>O tipo de medidor.</p></td>
</tr>

<tr class="even">
<td>Categoria do medidor</td>
<td><p>O serviço de nível superior para o uso.</p></td>
</tr>

<tr class="odd">
<td>ID do medidor</td>
<td><p>A ID do medidor que está sendo usado.</p></td>
</tr>

<tr class="even">
<td>Subcategoria do medidor</td>
<td><p>O tipo de serviço do Azure que pode afetar a taxa.</p></td>
</tr>

<tr class="odd">
<td>Nome do medidor</td>
<td><p>A unidade de medida para o medidor que está sendo consumido.</p></td>
</tr>

<tr class="even">
<td>Região do medidor</td>
<td><p>Essa coluna identifica a localização de um data center dentro da região para serviços onde isso é aplicável e preenchido.</p></td>
</tr>

<tr class="odd">
<td>Unidade</td>
<td><p>A unidade do nome do recurso.</p></td>
</tr>

<tr class="even">
<td>Quantidade consumida</td>
<td><p>A quantidade de serviço consumida (horas, GB etc.) durante o período de relatório. Também inclui qualquer uso não cobrado de períodos de relatório anteriores.</p></td>
</tr>

<tr class="odd">
<td>Local do recurso</td>
<td><p>O datacenter em que o medidor está em execução.</p></td>
</tr>

<tr class="even">
<td>Serviço consumido</td>
<td><p>O serviço da plataforma do Azure que você usou.</p></td>
</tr>


<tr class="even">
<td>URI de recurso</td>
<td><p>O URI do recurso que está sendo usado.</p></td>
</tr>

<tr class="odd">
<td>Tipo de cobrança</td>
<td><p>O tipo de encargo ou ajuste. Não disponível para a atividade atual.</p></td>
</tr>

<tr class="even">
<td>Preço unitário</td>
<td><p>Preço por licença, conforme publicado na tabela de preços no momento da compra. Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</p></td>
</tr>

<tr class="odd">
<td>Quantidade</td>
<td><p>Número de licenças. Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</p></td>
</tr>

<tr class="even">
<td>Tipo de unidade</td>
<td><p>O tipo de unidade em que o medidor é cobrado. Não disponível para a atividade atual.</p></td>
</tr>

<tr class="odd">
<td>Pré-imposto de cobrança</td>
<td><p>Valor total antes dos impostos.</p></td>
</tr>

<tr class="even">
<td>Moeda de cobrança</td>
<td><p>A moeda na região geográfica do cliente</p></td>
</tr>

<tr class="odd">
<td>Preço custo total</td>
<td><p>O preço antes da adição de impostos.</p></td>
</tr>

<tr class="even">
<td>Moeda de preços</td>
<td><p>A moeda na tabela de preços.</p></td>
</tr>

<tr class="odd">
<td>Informações de serviço 1</td>
<td><p>O número de conexões ServiceBus que foram provisionados e utilizados em um dia específico.</p></td>
</tr>

<tr class="even">
<td>Informações de serviço 2</td>
<td><p>Um campo herdado que captura metadados específicos do serviço opcionais.</p></td>
</tr>

<tr class="even">
<td>Informações adicionais</td>
<td><p>Quaisquer informações adicionais não abordadas em outras colunas.</p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a>Mapeando cobranças entre uma fatura e o arquivo de reconciliação

Sua fatura fornece um resumo dos encargos, enquanto seu arquivo de reconciliação fornece uma divisão detalhada das transações de item de linha, incluindo os tipos de carga.

Para fazer referência cruzada das quantidades de carga entre o arquivo de reconciliação e fatura, você pode usar opções de filtro do Microsoft Excel para filtrar por tipos de cobrança no arquivo de reconciliação para mapear os encargos de fatura em um conjunto de detalhamentos de cobrança no arquivo de reconciliação.

Os arquivos de reconciliação, tanto os baseados em licença quanto os baseados em uso, mostram apenas encargos e transações relacionadas ao uso (unidades consumidas e encargos relacionados). Créditos únicos, descontos ou reembolsos que aparecem na fatura como "Ajustes" não são mostrados no arquivo de reconciliação.

A tabela a seguir mostra os mapeamentos entre uma seção da fatura e os tipos de encargo associados que podem aparecer nos arquivos de reconciliação. 

<table>
<tbody>
<tr>
<td>
<p><strong>Descrição da cobrança da fatura</strong></p>
</td>
<td>
<p><strong>Descrição do encargo do arquivo de reconciliação (coluna Chargetype)</strong></p>
</td>
<td>
<p><strong>Qual é essa cobrança?</strong></p>
</td>
<td>
<p><strong>Como fazer mapear esses ChargeTypes para a fatura?</strong></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><strong>Encargos baseados em licença</strong></p>
</td>
<td>
<p>Taxa de ativação</p>
</td>
<td>
<p>O valor cobrado do cliente quando ele usa a assinatura depois de comprá-la.</p>
</td>
<td rowspan="10">
<p>No arquivo baseado em licença, some a coluna <strong>Quantidade</strong></p>
</td>
</tr>
<tr>
<td>
<p>Taxa de cancelamento</p>
</td>
<td>
<p>Os encargos proporcionais reembolsados para o cliente quando os assentos associados são alterados</p>
</td>
</tr>
<tr>
<td>
<p>Taxa do ciclo</p>
</td>
<td>
<p>Encargos periódicos de uma assinatura</p>
</td>
</tr>
<tr>
<td>
<p>Proporcional à instância do ciclo</p>
</td>
<td>
<p>Os encargos proporcionais cobrados do cliente quando os assentos associados são alterados</p>
</td>
</tr>
<tr>
<td>
<p>Taxas proporcionais durante o cancelamento</p>
</td>
<td>
<p>Reembolso proporcional para a parte não utilizada do serviço após o cancelamento</p>
</td>
</tr>
<tr>
<td>
<p>Taxas proporcionais durante a compra</p>
</td>
<td>
<p>O tipo de encargo para uma assinatura ao usar a cobrança anual</p>
</td>
</tr>
<tr>
<td>
<p>Valor de compra</p>
</td>
<td>
<p>O tipo de encargo para uma assinatura ao usar a cobrança mensal</p>
</td>
</tr>
<tr>
<td>
<p>Taxa proporcional ao renovar</p>
</td>
<td>
<p>Taxas proporcionais após a renovação da assinatura</p>
</td>
</tr>
<tr>

<td>
<p>Taxa de renovação</p>
</td>
<td>
<p>Cobrança para renovação de uma assinatura</p>
</td>
</tr>
<tr>
<td>
<p>Taxas proporcionais ao ativar</p>
</td>
<td>
<p>Taxas proporcionais da ativação até o final do período de cobrança</p>
</td>
</tr>



<tr>
<td rowspan="5">
<p><strong>Encargos de uso único</strong></p>

</td>
<td>
<p>Novo</p>
</td>
<td>
<p>Usado quando uma nova compra é criada</p>
</td>

<p></p>
</td>
</tr>
<tr>
<td>
<p>addquantity</p>
</td>
<td>
<p>Usado tanto no reembolso da compra original quanto na nova quantidade após o aumento</p>
</td>
</tr>

</tr>
<tr>
<td>
<p>removeQuantity</p>
</td>
<td>
<p>Usado tanto no reembolso da compra original quanto na nova quantidade após a diminuição</p>
</td>
</tr>

</tr>
<tr>
<td>
<p>Cancel</p>
</td>
<td>
<p>Usado quando uma assinatura é cancelada</p>
</td>
</tr>

</tr>
<tr>
<td>
<p>Converter</p>
</td>
<td>
<p>Usado quando uma licença é atualizada, mas o número de estações permanece inalterado</p>
</td>
</tr>

<tr>
<td rowspan="2">
<p><strong>Encargos de uso</strong></p>
</td>
<td>
<p>Avaliar a taxa de uso ao cancelar</p>
</td>
<td>
<p>Taxa de uso de acesso com o cancelamento para uso não pago durante o período de cobrança atual</p>
</td>
<td rowspan="2">
<p>No arquivo baseado em uso, some a coluna <strong>PretaxCharges</strong></p>
</td>
</tr>
<tr>
<td>
<p>Avalie a taxa de uso para o ciclo atual</p>
</td>
<td>
<p>Taxa de uso de acesso para o período atual de cobrança</p>
</td>
</tr>

<tr>
<td>
<p><strong>Crédito</strong></p>
</td>
<td>
<p>Deslocando um item de linha</p>
</td>
<td>
<p>Reembolso parcial ou integral para um item de linha, incluindo os impostos</p>
</td>
<td>
<p>No arquivo baseado em licença, some a coluna <strong>TotalForCustomer</strong></p>
<p>No arquivo baseado em uso, some a coluna <strong>PostTaxTotal</strong></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><strong>Descontos com base no uso</strong></p>
</td>
<td>
<p>Desconto de ativação</p>
</td>
<td>
<p>Desconto aplicado quando a assinatura é ativada</p>
</td>

<td rowspan="4">
<p>No arquivo baseado em uso, some a coluna <strong>PretaxCharges</strong></p>
</td>
</tr>
<tr>
<td>
<p>Desconto de ciclo</p>
</td>
<td>
<p>Desconto aplicado em cobranças periódicas</p>
</td>
</tr>
<tr>
<td>
<p>Desconto de renovação</p>
</td>
<td>
<p>Desconto aplicado quando a assinatura é renovada</p>
</td>
</tr>
<tr>
<td>
<p>Desconto de cancelamento</p>
</td>
<td>
<p>Encargos aplicados quando descontos são cancelados</p>
</td>
</tr>


<tr>
<td>
<p><strong>Descontos baseados em licença</strong></p>
</td>
<td>
<p><em>Pode ser aplicado a vários tipos de cobrança</em></p>
</td>
<td>
<p></p>
</td>
<td>
<p>No arquivo baseado em licença, some a coluna <strong>TotalOtherDiscount</strong></p>
</td>
</tr>
<tr>
<td>
<p><strong>Impostos</strong>&nbsp;ou&nbsp;<strong>IVA</strong></p>
</td>
<td>
<p><em>Pode ser aplicado a vários tipos de cobrança</em></p>
<p><em>Exception &quot;Deslocar um item&quot; de linha já inclui impostos. Consulte créditos, acima.</em></p>
</td>
<td>
<p>Impostos ou impostos sobre valor agregado (IVA)</p>
</td>
<td>
<p>No arquivo baseado em licença, some a coluna <strong>Imposto</strong></p>
<p>No arquivo baseado em uso, some a coluna <strong>TaxAmount</strong></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
