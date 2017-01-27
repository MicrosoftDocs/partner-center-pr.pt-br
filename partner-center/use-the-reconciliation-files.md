---
title: "Usar os arquivos de reconciliação | Partner Center"
description: "Para obter uma exibição detalhada em itens de linha de cada encargo em um ciclo de cobrança, baixe os arquivos de reconciliação do painel do Partner Center."
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: MaggiePucciEvans
translationtype: Human Translation
ms.sourcegitcommit: cb3523dffbd017aa5c40e6899e1cb37be1f2a726
ms.openlocfilehash: 362cc5c1f40034355f9899a79ae4bb6c948ec622

---

# Usar os arquivos de reconciliação

**Aplicável a**

-  Partner Center
-  Partner Center do Microsoft Cloud Germany

Para obter uma exibição detalhada em itens de linha de cada encargo em um ciclo de cobrança, baixe os arquivos de reconciliação do painel do Partner Center. Os detalhes incluem encargos por assinaturas de cada cliente e eventos detalhados (como a adição de assentos a uma assinatura no meio do período).

## Nesta seção


-   [Discriminar por parceiro](#itemizebypartner)
-   [Arquivos de reconciliação baseados em licença](#licencebasedfiles)
-   [Arquivos de reconciliação baseados em uso](#usagebasedfiles)

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
<td><p>A ID do MPN do parceiro CSP (direto ou indireto).</p></td>
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
<td>CustomerNumber</td>
<td><p>Identificador exclusivo do cliente na plataforma de cobrança da Microsoft. Pode ser útil para identificar o cliente ao entrar em contato com o suporte, mas não para reconciliação.</p></td>
<td>123456789</td>
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
<td><p>ID exclusivo da oferta. ID padrão da oferta de acordo com a lista de preços.</p></td>
<td>306855</td>
</tr>
<tr class="even">
<td>DurableOfferID</td>
<td><p>ID exclusivo da oferta durável, conforme definido na tabela de preços.</p></td>
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
<td><p>O tipo de encargo ou ajuste.</p>
<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td>Encargos:</td>
<td><ul>
<li>PURCHASE_FEE: encargo inicial de uma assinatura</li>
<li>CYCLE_FEE: encargos periódicos de uma assinatura</li>
</ul></td>
</tr>
<tr class="even">
<td>ConvertResources</td>
<td><ul>
<li>CANCEL_USAGEFEE: taxa de uso de acesso com o cancelamento para uso não pago durante o período de cobrança atual</li>
<li>CYCLE_USAGEFEE: taxa de uso de acesso para o período atual de cobrança</li>
</ul></td>
</tr>
<tr class="odd">
<td>Proporcionais:</td>
<td><ul>
<li>PURCHASE_PRORATE: taxas proporcionais após a compra</li>
<li>CANCEL_PRORATE: reembolso proporcional para a parte não utilizada do serviço após o cancelamento</li>
<li>ACTIVATION_PRORATE: taxas proporcionais da ativação até o final do período de cobrança</li>
<li>RENEW_PRORATE: taxas proporcionais após a renovação da assinatura</li>
</ul></td>
</tr>
<tr class="even">
<td>InstanceProrates:</td>
<td><ul>
<li>CANCEL_INSTANCEPRORATE: encargos proporcionais reembolsados para o cliente quando os assentos associados são alterados</li>
<li>CYCLE_INSTANCEPRORATE: encargos proporcionais cobrados do cliente quando os assentos associados são alterados</li>
</ul></td>
</tr>
<tr class="odd">
<td>Créditos:</td>
<td><ul>
<li>CREDIT: crédito aplicado a um método de pagamento</li>
</ul></td>
</tr>
<tr class="even">
<td>Deslocamentos:</td>
<td><ul>
<li>OFFSET_LINEITEM: reembolso parcial ou integral para um item de linha</li>
<li>ONE_TIME_REFUND: reembolso único processado para o cliente</li>
<li>TAX_REFUND: reembolso devido para a validação do certificado de isenção de imposto</li>
</ul></td>
</tr>
<tr class="odd">
<td>Descontos:</td>
<td><ul>
<li>ACTIVATION_DISCOUNT: desconto aplicado quando a assinatura é ativada</li>
<li>CYCLE_DISCOUNT: desconto aplicado em encargos periódicos</li>
<li>RENEW_DISCOUNT: desconto aplicado quando a assinatura é renovada</li>
<li>CANCEL_DISCOUNT: encargos aplicados quando os descontos são cancelados</li>
</ul></td>
</tr>
</tbody>
</table>
<p> </p></td>
<td></td>
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
<td><p>Nome da oferta do serviço</p></td>
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
<td><p>Descrição do tipo de item de linha.</p></td>
<td>TAXA DE USO DE ACESSO PARA O CICLO ATUAL</td>
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
</tbody>
</table>

 

 

 






<!--HONumber=Jan17_HO2-->


