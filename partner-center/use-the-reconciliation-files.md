---
title: "Usar os arquivos de reconciliação | Partner Center"
description: "Para obter uma exibição detalhada em itens de linha de cada encargo em um ciclo de cobrança, baixe os arquivos de reconciliação do painel do Partner Center."
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: KPacquer
ms.openlocfilehash: 61e71d4207d9e8ac68ee4fcfc1f0d04282474032
ms.sourcegitcommit: c2a12d6a18b9631916f6dd8301a4752ecc03296b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2017
---
# <a name="use-the-reconciliation-files"></a>Usar os arquivos de reconciliação

**Aplicável a**

-  Partner Center
-  Partner Center for Microsoft Cloud for US Government
-  Partner Center for Microsoft Cloud Germany

Para obter uma exibição detalhada em itens de linha de cada encargo em um ciclo de cobrança, baixe os arquivos de reconciliação do painel do Partner Center. Os detalhes incluem encargos por assinaturas de cada cliente e eventos detalhados (como a adição de assentos a uma assinatura no meio do período).

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
<p>Para exibir ou atualizar o revendedor, no menu Partner Center, selecione <strong>Clientes</strong>, em seguida, escolha o cliente na lista. No menu do cliente, selecione <strong>Assinaturas</strong>, escolha a assinatura na lista. Selecione <strong>Atualizar</strong> para alterar o <strong>Revendedor (ID do MPN)</strong>.</p>
<p>Se um parceiro CSP vendeu a assinatura diretamente para o cliente, sua ID do MPN estará listada duas vezes, como a ID do MPN e a ID do MPN do revendedor.</p>
<p>Se um parceiro CSP tiver um revendedor sem ID do MPN, esse valor será definido como a ID do MPN do parceiro.</p>
<p>Se o parceiro CSP remover uma ID de revendedor, esse valor será definido como -1.</p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licencebasedfiles"></a> Campos de arquivos baseado em licença


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
<td>OperatingUnit</td>
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
<p><b>Observação</b>: esse valor não coincide com a ID de oferta da lista de preços. Veja DurableOfferID abaixo.</p></td>
<td>FE616D64-E9A8-40EF-843F-152E9BBEF3D1</td>
</tr>
<tr class="even">
<td>DurableOfferID</td>
<td><p>ID exclusiva da oferta durável, conforme definido na tabela de preços.</p>
<p><b>Observação</b>: esse valor corresponde à ID de oferta da lista de preços.</p></td>
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
<td><p>A data do término da assinatura: 12 meses + x dias após a data de início (para se alinhar com a data de cobrança do parceiro) ou 12 meses a partir da data de renovação.</p>
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
<td><p>Preço por assento. Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</p></td>
<td>6.82</td>
</tr>
<tr class="even">
<td>Quantity</td>
<td><p>Número de assentos. Isso deve coincidir com a informação armazenada em seu sistema de cobrança durante a reconciliação.</p></td>
<td>2</td>
</tr>
<tr class="odd">
<td>Quantidade</td>
<td><p>Preço total por quantidade. Útil para verificar se o cálculo do valor coincide com a forma como você calcula isso para seus clientes.</p></td>
<td>13.32</td>
</tr>
<tr class="even">
<td>TotalOtherDiscount</td>
<td><p>Valor de desconto aplicado a esses encargos. IUR ou novas assinaturas qualificadas para incentivo também conterão um valor de desconto nessa coluna.</p></td>
<td>2.32</td>
</tr>
<tr class="odd">
<td>Subtotal</td>
<td><p>Total sem imposto. Verifica se seu subtotal corresponde ao total esperado, em caso de desconto.</p></td>
<td>11</td>
</tr>
<tr class="even">
<td>Imposto</td>
<td><p>Valor do imposto cobrado, com base nas regras fiscais do mercado e em circunstâncias específicas.</p></td>
<td>0</td>
</tr>
<tr class="odd">
<td>TotalForCustomer</td>
<td><p>Total com imposto. Verifica se o imposto é cobrado na fatura.</p></td>
<td>11</td>
</tr>
<tr class="even">
<td>Moeda</td>
<td><p>Tipo de moeda. Cada entidade de cobrança tem somente uma moeda. Verifique se isso coincide com a primeira fatura e faça o mesmo após grandes atualizações na plataforma de cobrança.</p></td>
<td>Euro</td>
</tr>
<tr class="odd">
<td>CustomerName</td>
<td><p>Nome da organização do cliente como informado no Partner Center. Isso é muito importante para reconciliar a fatura com as informações de seu sistema.</p></td>
<td>Cliente de teste A</td>
</tr>
<tr class="even">
<td>ID do MPN</td>
<td><p>ID do MPN do parceiro CSP</p></td>
<td>4390934</td>
</tr>
<tr class="odd">
<td>ResellerMPNID</td>
<td><p>ID do MPN do revendedor de registro da assinatura. Consulte [Discriminar por parceiro](#itemizebypartner).</p></td>
<td>4390934</td>
</tr>
<tr class="even">
<td>DomainName</td>
<td><p>Nome de domínio do cliente, usado para ajudar a identificar o cliente.</p></td>
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


## <a href="" id="usagebasedfiles"></a>Campos de arquivo baseado em uso


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
<td><p>Nome da organização do cliente como informado no Partner Center. Isso é muito importante para reconciliar a fatura com as informações de seu sistema.</p></td>
<td>Cliente de teste A</td>
</tr>
<tr class="even">
<td>ID do MPN</td>
<td><p>ID do MPN do parceiro CSP.</p></td>
<td>4390934</td>
</tr>
<tr class="odd">
<td>ResellerMPNID</td>
<td><p>ID do MPN do revendedor de registro da assinatura. Consulte [Discriminar por parceiro](#itemizebypartner).</p></td>
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
<p>Esse não é o mesmo que a ID da assinatura no Partner Admin Console.</p></td>
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
<td><p>Valor do imposto cobrado, com base nas regras fiscais do mercado e em circunstâncias específicas.</p></td>
<td>U$ 0,08</td>
</tr>
<tr class="even">
<td>PostTaxTotal</td>
<td><p>Total após imposto, quando o imposto é aplicável.</p></td>
<td>U$ 0,93</td>
</tr>
<tr class="odd">
<td>Moeda</td>
<td><p>Tipo de moeda. Cada entidade de cobrança tem somente uma moeda. Verifique se isso coincide com a primeira fatura e faça o mesmo após grandes atualizações na plataforma de cobrança.</p></td>
<td>Euro</td>
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
<td>Por exemplo: se você tivesse uma conexão individualmente provisionada durante um mês de 30 dias, a coluna Informação do Serviço 1 lerá "1,000000 conexões/30 dias". Se você tinha um pacote de 25 conexões ServiceBus provisionadas e você utilizou 1 durante o dia, sua declaração de uso diário para esse dia indicaria "25 conexões/30 dias – Usado: 1,000000".</td>
</tr>
<tr class="even">
<td>CustomerID</td>
<td><p>ID exclusiva da Microsoft, no formato GUID, usada para identificar o cliente.</p></td>
<td>ORDDC52E52FDEF405786F0642DD0108BE4</td>
</tr>
<tr class="odd">
<td>DomainName</td>
<td><p>Nome de domínio do cliente, usado para ajudar a identificar o cliente.</p></td>
<td>example.onmicrosoft.com</td></tr>
</tbody>
</table>



## <a href="" id="charge_types"></a>Mapeando encargos entre uma fatura e o arquivo de reconciliação

Sua fatura fornece um resumo dos encargos, enquanto seu arquivo de reconciliação fornece uma divisão detalhada das transações de item de linha, incluindo os tipos de carga.

Para fazer referência cruzada das quantidades de carga entre o arquivo de reconciliação e fatura, você pode usar opções de filtro do Microsoft Excel para filtrar por tipos de cobrança no arquivo de reconciliação para mapear os encargos de fatura em um conjunto de detalhamentos de cobrança no arquivo de reconciliação.

A tabela a seguir mostra os mapeamentos entre uma seção da fatura e os tipos de encargo associados que podem aparecer nos arquivos de reconciliação. 

<table>
<tbody>
<tr>
<td>
<p><strong>Descrição do encargo da fatura</strong></p>
</td>
<td>
<p><strong>Descrição do encargo do arquivo de reconciliação (coluna ChargeType)</strong></p>
</td>
<td>
<p><strong>O que é este encargo?</strong></p>
</td>
<td>
<p><strong>Como é possível mapear esses tipos de encargo na fatura?</strong></p>
</td>
</tr>
<tr>
<td rowspan="8">
<p><strong>Encargos recorrentes</strong></p>
</td>
<td>
<p>Cancelar ocorrência proporcional</p>
</td>
<td>
<p>Os encargos proporcionais reembolsados para o cliente quando os assentos associados são alterados</p>
</td>
<td rowspan="8">
<p>No arquivo baseado em licença, some a coluna <strong>Quantidade</strong></p>
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
<p>Percorrer ocorrência proporcional</p>
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
<p>Taxas proporcionais após a compra</p>
</td>
</tr>
<tr>
<td>
<p>Taxa de compra</p>
</td>
<td>
<p>Encargo inicial de uma assinatura</p>
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
<p><strong>Outros produtos e serviços</strong></p>
</td>
<td>
<p>Taxas proporcionais ao ativar</p>
</td>
<td>
<p>Taxas proporcionais da ativação até o final do período de cobrança</p>
</td>
<td>
<p>No arquivo baseado em licença, some a coluna <strong>Quantidade</strong></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong>Tarifas de uso</strong></p>
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
<p><strong>Créditos &amp; Ajustes</strong></p>
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
<p><strong>Outros descontos</strong></br>
<em>(com base em uso)</em></p>
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
</tr><tr>
<td>
<p>Desconto de renovação</p>
</td>
<td>
<p>Desconto aplicado quando a assinatura é renovada</p>
</td>
</tr><tr>
<td>
<p>Desconto de cancelamento</p>
</td>
<td>
<p>Encargos aplicados quando descontos são cancelados</p>
</td>
</tr>
<tr>
<td>
<p><strong>Outros descontos</strong></br>
<em>(com base em licença)</em></p>
</td>
<td>
<p><em>Podem ser aplicados a vários tipos de cobrança</em></p>
</td>
<td>
<p>&nbsp;</p>
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
<p><em>Podem ser aplicados a vários tipos de cobrança</em></p>
<p><em>Exceção: "Deslocamento de um item de linha" já inclui impostos. Consulte Créditos &amp;Ajustes, acima.</em></p>
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
