---
title: Demonstrativos de pagamento
description: Saiba mais sobre demonstrativos e resumos de pagamentos e como exibir e exportar seus dados de pagamento do Microsoft Partner Center
ms.subservice: partnercenter-marketplace-publisher
ms.service: marketplace
ms.topic: article
author: eunjkim520
ms.author: eunjkim
ms.date: 3/22/2021
ms.openlocfilehash: b905d422b10e0b82225966fa5379283ea0b83a69
ms.sourcegitcommit: a09a5f893e876de23a8aa5c0d637e50c5be84941
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "113684008"
---
# <a name="payout-statements"></a>Demonstrativos de pagamento

**Funções apropriadas**: administrador da conta | Administrador global

A **instrução pagamento** apresenta uma visão geral de seus pagamentos de ofertas vendidas por meio do Marketplace comercial. Ele mostra o histórico transacional de seus ganhos, estima seu próximo pagamento e mostra as tendências de pagamento. Você também pode baixar o histórico de transações e os demonstrativos de pagamento. Este artigo explica como acessar sua declaração de pagamento e as diferentes páginas de pagamento e downloads acessíveis para você no Partner Center.

>[!NOTE]
>Você só verá dados para IDs e programas MPN aos quais está associado. Se você quiser ver dados adicionais, trabalhe com o administrador da conta para obter permissões. 

## <a name="roles-and-permissions"></a>Funções e permissões

Para acessar uma instrução de pagamento, você precisa receber a função de **proprietário de conta** ou **colaborador financeiro** .

| Relatórios/páginas | Proprietário da conta | Gerente | Desenvolvedor | Colaborador comercial | Colaborador financeiro | Marketer |
| --- | --- | --- | --- | --- | --- | --- |
| Relatório de aquisição (incluindo dados quase em tempo real) | Pode exibir | Pode exibir | Sem acesso | Sem acesso | Pode exibir | Sem acesso |
| Relatório/respostas de comentários | Pode exibir e enviar comentários | Pode exibir e enviar comentários | Pode exibir e enviar comentários | Sem acesso | Sem acesso | Pode exibir e enviar comentários |
| Relatório de integridade (incluindo dados quase em tempo real) | Pode exibir | Pode exibir | Pode exibir | Pode exibir | Sem acesso | Sem acesso |
| Relatório de uso | Pode exibir | Pode exibir | Pode exibir | Pode exibir | Sem acesso | Sem acesso |
| Conta de pagamento | Pode atualizar | Sem acesso | Sem acesso | Sem acesso | Pode atualizar | Sem acesso |
| Perfil fiscal | Pode atualizar | Sem acesso | Sem acesso | Sem acesso | Pode atualizar | Sem acesso |
| Resumo do pagamento | Pode exibir | Sem acesso | Sem acesso | Sem acesso | Pode exibir | Sem acesso |
|

## <a name="access-your-payout-statement"></a>Acessar sua instrução de pagamento

Entre no [Partner Center](https://partner.microsoft.com/dashboard/home) e selecione o ícone de pagamento no canto superior direito da tela para acessar esses resumos diferentes:

- Histórico de transação
- Pagamentos
- Exportar dados

:::image type="content" source="images/payouts/payout-overview.png" alt-text="Ilustra o ícone de Pagamento no canto superior direito do portal do Partner Center.":::

Você também pode usar a [API](/rest/api/partner-center/partner-payouts) de pagamento de parceiro para conectar-se e obter dados de transação e pagamentos diretamente. Saiba mais em [gerenciar pagamentos usando a API do serviço de pagamento](/partner-center/develop/manage-payouts).


## <a name="transaction-history"></a>Histórico de transação

A página **histórico de transações** mostra o resumo dos seus ganhos, o próximo pagamento estimado e sua tendência de ganhos e pagamentos nos últimos 36 meses. Você também pode baixar os detalhes da transação nesta seção.<br><br>Este relatório mostra todos os ganhos qualificados para pagamento, incluindo pagamentos ainda não enviados. Os ganhos são qualificados para pagamento quando um ISV concluiu todas as informações bancárias e de impostos no Partner Center, ganhou >$50, a conta ISV está ativa e o cliente foi cobrado (para transações EA) ou o pagamento foi recebido (para transações não EA).

:::image type="content" source="images/payouts/transaction-overview.png" alt-text="Visão geral da transação.":::

- **Ganhos enviados neste ano** – total de ganhos e divisão de ganhos que foram pagos e serão pagos no próximo mês.
- **Mês de pagamento estimado** – ganhos totais esperados nos próximos meses.
- **Lucros e tendência de pagamento** – valores mensais de conquista e pagamento nos últimos 36 meses.
- **Baixar** – baixar detalhes da transação no formato .csv ou. TSV.

Use a seleção de intervalo de datas no canto superior direito da página para filtrar a saída da página para mostrar os últimos 3, 6, 12 ou 36 meses. Ou então, selecione um intervalo de datas personalizado de até 36 meses. O intervalo de datas padrão é de 12 meses. Você também pode filtrar por ID de registro, programa, ID de pagamento, tipo de conquista, alavanca e status. Os dados estão disponíveis para o ano fiscal atual (1º de julho a 30 de junho) e os dois anos fiscais anteriores.

:::image type="content" source="images/payouts/search-filter.png" alt-text="O filtro de pesquisa na parte superior direita da página.":::

Para ver mais detalhes sobre um ganho, selecione a seta para baixo no lado direito da página. Isso exibirá a alavanca, o valor da receita, o produto e o cliente. Se, por algum motivo, algum desses dados estiver indisponível, mas você precisar acessá-lo, entre em contato com o suporte. Se a conquista for o resultado de um ajuste, e não de uma transação, os campos Product e Customer não serão exibidos.

### <a name="transaction-history-summary"></a>Resumo do histórico de transações

Esta exibição mostra a obtenção de detalhes, incluindo a origem da conquista do produto vendido vendas, status e mês de pagamento estimado.

:::image type="content" source="images/payouts/transaction-history.png" alt-text="Histórico de transações.":::

- **Data** de aquisição – a data de compra.
- **Tipo de** ganho – o tipo de ganho, como Vendas, Lucro ou Cooperação.
- **Valor total** – o valor de ganho líquido. No marketplace comercial, isso significa depois de deduzir o valor padrão do marketplace.
- **Status** – tem três opções:
    - **Futuro –** os ganhos estão no período de resfriamento pendente.
    - **Processado** – os ganhos estão preparados para o próximo pagamento.
    - **Enviado** – Os ganhos foram pagos.
- **Mês de pagamento estimado** – o mês em que os ganhos devem ser pagos. Consulte a [próxima seção para](#estimated-payment-month) obter mais informações.

As transações de ganho são mostradas depois que a transação atende à qualificação de pagamento. Para entender por que você pode ter ganhos ausentes ou inesperados, consulte [Perguntas comuns sobre pagamentos do marketplace comercial.](payout-faq.yml#why-are-my-earnings-missing-)

#### <a name="estimated-payment-month"></a>Mês de pagamento estimado

A página Histórico de Transações agora inclui uma tabela mostrando os valores de pagamento estimados para os próximos meses. Você também pode exibir e baixar essas informações no Histórico de transações e exportações de relatório de resumo. Essas informações facilitam as reconciliaçãos e as projeções de pagamento.

O Mês de pagamento estimado é calculado com base nas regras e linhas do tempo de configuração do programa e é processado no próximo/próximo ciclo de pagamento.

O mês de pagamento estimado está disponível atualmente para todos os tipos de ganho, exceto cooperação, que será exibido **como Não aplicável.** Para ganhos antes de 1º de julho de 2020, o Mês de pagamento estimado será exibido **como Não disponível.**

A tabela a seguir mostra um exemplo de mês de pagamento estimado.

| Mês | Valor |
| ------ | :-----------: |
|  Setembro de 2020 |  US$ 7.273,99   |
|  Outubro de 2020 | US$ 8.692,30  |
|  Novembro de 2020 | US$ 107,89  |

O valor estimado pode variar da quantidade real por vários motivos:

- Recalculação de ganho: se os ganhos são recalculados, o valor real será diferente
- Ajustes: o valor real varia dependendo dos ajustes que ocorreram ou foram enviados.
- Alteração de regras: uma alteração nas regras pode refletir o recálculo no valor real pago
- A pagar: se ocorrer falha no pagamento, o valor real poderá ser diferente

Observe que o pagamento só será liberado no mês projetado se as regras de qualificação de pagamento e limite do programa são atendidas. Essas regras incluem, mas não estão limitadas à lista abaixo:

- Seu perfil de imposto deve estar atualizado
- Seus ganhos devem atender ou exceder o limite mínimo de ganho definido no guia do programa.
- Pagamento em espera: se você selecionar a opção "Manter meu Pagamento" na página de atribuição de perfis.
- Instrumento de pagamento não disponível: o perfil de pagamento ou/e Imposto não foi concluído.

### <a name="transaction-history-download"></a>Download do histórico de transações

Para ver mais detalhes sobre um ganho, selecione **Baixar** na parte superior da página. A tabela a seguir explica cada coluna no relatório.

>[!NOTE]
>A exportação de download do histórico de transações tem dois novos campos a partir de agosto de 2020:
>
>- **lastPaymentCurrency**  A moeda na qual o pagamento mais recente foi recebido, em todos os MPNs aos quais o parceiro que está conectado no momento tem acesso. Se nenhum pagamento for recebido, a última moeda de pagamento será dólares americanos.
>- **earningAmountInLastPaymentCurrency**  O valor do ganho na última moeda de pagamento.

| Nome da coluna | Descrição | Aplicabilidade para programas de incentivo/marketplaces |
| --- | --- | --- |
| agreementEndDate | Data de término do contrato | Incentivos – apenas alguns programas |
| agreementNumber | Número do contrato | Incentivos – apenas alguns programas |
| agreementStartDate | Data de início do contrato | Incentivos – apenas alguns programas |
| calculationDate | Data em que o ganho foi calculado no sistema | Todos |
| claimId | Um identificador exclusivo para a declaração | Incentivos – apenas alguns programas |
| customerCountry | País/região do cliente | marketplaces |
| customerEmail |  |  |
| customerName | Pode estar em branco | Somente programas de incentivo (exceção: OEM) e marketplaces. Para transações CSP, os marketplaces mostrarão o nome do CSP |
| customerTenantId |  |  |
| distributorId | Identificador do distribuidor | Incentivos – apenas alguns programas |
| distributorName | Nome do distribuidor | Incentivos – apenas alguns programas |
| earningAmount | Valor do ganho na moeda da transação original | Todos |
| earningAmountInLastPaymentCurrency | Valor do ganho na moeda do último pagamento (o campo fica vazio se não houver pagamento anterior) |  |
| earningAmountUSD | Valor do ganho em US$ | Todos |
| earningDate | Data do ganho | Todos |
| earningExchangeRate | Taxa de câmbio usada para mostrar o valor em US$ correspondente | Todos |
| earningId | Identificador exclusivo de cada ganho | Todos |
| earningRate | Taxa de incentivos aplicada no valor da transação para gerar um ganho | Todos |
| earningType | Indica se é valor, desconto, cooperação, venda e assim por diante | Todos |
| exchangeRateDate | Data da taxa de câmbio usada para calcular EarningAmount US$ | Todos |
| externalReferenceId | Identificador exclusivo do programa | Programas de pagamento direto (incentivos e Marketplaces) |
| externalReferenceIdLabel | Rótulo de identificador exclusivo | Programas de pagamento direto (incentivos e Marketplaces) |
| instantRebateAmount |  |  |
| invoiceDate |  |  |
| invoiceNumber | Número da nota fiscal (aplicável somente para empresas) | Incentivos e Marketplaces – apenas alguns programas |
| lastPaymentCurrency | Moeda do último pagamento (o campo fica vazio se não houver pagamento anterior) |  |
| alavanca | Indica a regra de negócios para o ganho | Todos |
| LicensingProgramName | Nome do programa de licenciamento |  |
| LineItemId | Linha individual na fatura de um cliente |  |
| localProviderSeller | Provedor/vendedor local do registro |  |
| Mês de maturidade | O mês de pagamento estimado | Tudo |
| OrderId | Está relacionado à fatura de um cliente  | marketplaces |
| parentProductId | Identificador exclusivo do produto pai. Se não houver um produto pai na transação, ID do produto pai = ID do produto. | marketplaces |
| parentProductName | O nome do produto pai. Se não houver um produto pai na transação, Nome do produto pai = Nome do produto. | marketplaces |
| participantId | A identidade principal do parceiro que ganha com o programa | Todos |
| participantIdType | Principalmente a ID do programa para programas de incentivo e vendedor se for Marketplace | Todos |
| participantName | Nome do parceiro de ganho | Todos |
| partnerCountryCode | Localização/país/região do parceiro de ganho | Todos |
| partNumber | Está sempre em branco | Alguns programas de incentivo e Marketplaces |
| paymentId | Identificador exclusivo para correlacionar todas as transações no relatório de transações com um pagamento específico no relatório de pagamento | Tudo |
| paymentStatus | Status de pagamento | Todos |
| paymentStatusDescription | Descrição amigável do status de pagamento | Todos |
| productId | Identificador exclusivo do produto | marketplaces |
| productName | Nome do produto vinculado à transação | Tudo |
| productType | Tipo de produto, como aplicativo, complemento ou jogo | marketplaces |
| Código do programa | Cadeia de caracteres para mapear com o nome do programa |  |
| programName | Nome do programa de incentivo/loja | Todos |
| purchaseOrderCoverageEndDate | Está sempre em branco | Programa de incentivo – CRI |
| purchaseOrderCoverageStartDate | Está sempre em branco | Programa de incentivo – CRI |
| purchaseOrderType | Está sempre em branco | Programa de incentivo – CRI |
| purchaseTypeCode | Está sempre em branco | Programa de incentivo – CRI |
| quantidade | Varia de acordo com o programa. Indica a quantidade cobrada para programas de transação | Todos |
| reasonCode |  |  |
| resellerCountry |  |  |
| resellerId | Identificador do revendedor | Incentivos – apenas alguns programas |
| resellerName | Nome do revendedor |  |
| SkuId | ID do SKU definido durante a publicação. Uma oferta pode ter muitos SKUs, mas um SKU só pode estar associado a uma única oferta. Incentivos – apenas alguns programas |  |
| storeFee | O valor retido pela Microsoft como taxa pela disponibilização do aplicativo ou complemento na loja | marketplaces |
| subscriptionEndDate | Data de término da assinatura | Incentivos – apenas alguns programas |
| subscriptionId | Identificador de assinatura associado ao cliente | Incentivos – apenas alguns programas |
| subscriptionStartDate | Data de início da assinatura | Incentivos – apenas alguns programas |
| taxCity |  |  |
| taxCountry |  |  |
| taxRemitModel | Parte responsável pelo pagamento de impostos (vendas, uso ou impostos sobre IVA/GST) | marketplaces |
| taxRemitted | Valor do imposto remetido (vendas, uso ou impostos sobre IVA/GST) | marketplaces |
| taxState | Estado do cliente |  |
| taxZipCode | CEP/código postal do cliente |  |
| tpan | Indica a rede de anúncios de terceiros | somente anúncios do Marketplaces |
| transactionAmount | Valor da transação na moeda da transação original, com base em qual o ganho é gerado | Todos |
| transactionAmountUSD | Valor da transação em US$ | Todos |
| transactionCountryCode | Código do país/região em que a transação ocorreu |  |
| transactionCurrency | Moeda em que a transação original do cliente ocorreu (não é a moeda da localização do parceiro) | Todos |
| transactionDate | Data da transação. Útil para programas em que muitas transações contribuem para um ganho | Todos |
| transactionExchangeRate | Data da taxa de câmbio usada para mostrar o valor em US$ da transação correspondente | Todos |
| transactionId | Um identificador exclusivo da transação | Todos |
| transactionPaymentMethod | Meio de pagamento do cliente usado na transação, como cartão, cobrança de operadora móvel ou PayPal | marketplaces |
| transactionType | Tipo de transação, como compra, reembolso, inversão ou estorno | marketplaces |
| workload | Carga de trabalho | Incentivos – apenas alguns programas |
|

### <a name="transaction-adjustment-codes"></a>Códigos de ajuste de transação

A tabela a seguir lista os códigos de motivo para ajustes e suas descrições.

|**Código de motivo**   |**Descrição**   |
|------------------|:-------------------------------------|
| Conformidade com o AR | Ajuste que reduz os ganhos quando as faturas da Microsoft não são pagas no tempo pelo parceiro. |
| Substituição de cooperação | Ajuste que transfere os ganhos de cooperação para outro período ou converte os ganhos de cooperação no reembolso. |
| Ajuste de Ops | Ajuste que corrige erros de cálculo do sistema da Microsoft. |
| Cálculo incorreto do Microsoft ajuste de Ops | Ajuste que corrige os incorretos de cálculos. |
| Registro incorreto do Microsoft ajuste de Ops | Ajuste para os inscrições relacionados ao registro. |
| MCI/CSP de mapeamento de parceiro (assinatura) | Ajuste que corrige o desalinhamento da assinatura. |
| Exceção de política | Ajuste que substitui uma regra de programa.  |
| Ganhos do período anterior | Ajuste para ganhos fora do período de conquista atual. |

## <a name="payments"></a>Pagamentos

A página de **pagamentos** fornece detalhes sobre o dinheiro que você ganhou com a Microsoft. Ele também mostra quando e quanto você será pago.

>[!Note]
> Para se qualificar para o pagamento, suas receitas devem alcançar o [limite de pagamento](payment-thresholds-methods-timeframes.md) de US$ 50. para obter mais informações, consulte o [contrato de Microsoft Publisher](/legal/marketplace/msft-publisher-agreement).

:::image type="content" source="images/payouts/payments-overview.png" alt-text="Tela de visão geral de pagamentos.":::

- **Total pago neste ano** – o total combinado pago a você neste ano, em dólares americanos, para todos os seus programas.
- **Próximo pagamento estimado** – o próximo pagamento seguinte chegando a você (mesmo se houver outros em breve), em dólares americanos.
- **Último pagamento** – a quantidade (em dólares americanos), nome do programa e programa do seu pagamento mais recente.
- **Pagamento por origem** – valor de pagamentos (em dólares americanos), por programa, nos últimos 12 meses.

### <a name="payments-list"></a>Lista de pagamentos

A tabela **lista de pagamentos** mostra pagamentos pagos e pendentes. Você pode baixar informações de imposto sobre taxas de serviço no formato PDF e exibir os detalhes de um determinado pagamento.

:::image type="content" source="images/payouts/list-of-payments.png" alt-text="Exportar histórico de transações.":::

- **Pago** – todos os pagamentos enviados com êxito. Escolha o ano no menu suspenso para filtrar os pagamentos liberados nesse ano.
- **Pendente** – pagamentos futuros.
- **Imposto sobre a taxa de serviço (formulário PDF)** – disponível para os pagamentos sujeitos ao imposto sobre tarifa de serviço. Os impostos sobre tarifas de serviço são mostrados em **outros impostos**.
- **Exibir** – redireciona para o histórico de transações com uma lista de ganhos incluídos no pagamento.

Para entender por que você pode ter ganhos ausentes ou inesperados, consulte [perguntas comuns sobre pagamentos do Marketplace comercial](payout-faq.yml#why-are-my-earnings-missing-).

### <a name="payment-status"></a>Status de pagamento

A tabela a seguir explica os diferentes status de conquista.

| Status do ganho | Motivo | É necessária uma ação do parceiro? |
| --- | --- | --- |
| Não processado | O ganho está qualificado para pagamento. Ele permanece nesse estado por um período de resfriamento, conforme definido no guia do programa para o programa de incentivos. | Não |
| Futuros | A ordem de pagamento gerou revisões internas pendentes antes de o pagamento ser processado. | Não |
| Fatura de imposto pendente | Sua fatura de imposto está incompleta ou inválida. | Atualize sua fatura de imposto para ser pago |
| Rejeitado durante a revisão | O pagamento foi rejeitado durante a revisão. | Entre em contato com o Suporte da Microsoft para detalhes |
| Com falha | O pagamento falhou devido a um erro do sistema da Microsoft. | Contate o suporte da Microsoft para obter detalhes |
| Em Andamento | O pagamento está em andamento. | Não |
| Pagamento incorreto | A revitóriação de pagamento está em andamento. | Não |
| Enviado | O pagamento foi enviado ao seu banco. | Não |
| Em reprocessamento | O pagamento encontrou um erro de sistema da Microsoft e está sendo reprocessado. | Não |
| Reversed | O pagamento foi revertido pelo seu banco e será enviado novamente no próximo ciclo de pagamento. | Não |
| Fatura de imposto rejeitada | Sua fatura de imposto foi rejeitada durante a análise. Todos os pagamentos pendentes estarão em espera até que a análise da fatura de imposto seja concluída. | Contate o suporte da Microsoft para obter detalhes |
| Fatura de imposto em análise | Sua fatura de imposto está sendo examinada. Seu pagamento será liberado depois que a fatura de imposto tiver sido aprovada. | Não |
| Rejeitado | O pagamento foi rejeitado pelo seu banco. | Entre em contato com seu banco para obter detalhes. |
|

### <a name="payments-download"></a>Download de pagamentos

 A tabela a seguir explica cada coluna no relatório. Para ver mais detalhes sobre seus pagamentos, selecione **baixar** na parte superior da página de pagamentos.

| Nome da coluna | Descrição |
| --- | --- |
| participantID | A identidade principal do parceiro que ganha com o programa |
| participantIDType | Normalmente a ID do programa para os programas de incentivos e a ID do vendedor para programas da loja |
| participantName | Nome do parceiro de ganho |
| programName | Incentivos/nome do programa de armazenamento |
| ganho | Valor ganho na moeda de pagamento para o programa/participantID |
| earnedUSD | Valor ganho para a ID do programa/participante, em US$ |
| withheldTax | Valor de imposto retido na moeda de pagamento para o programa/participantID |
| salesTax | Valor total do imposto sobre vendas na moeda de pagamento para o programa/participanteid (aplicável somente a programas de incentivos) |
| serviceFeeTax | Valor total de serviceFeeTax na moeda de pagamento para o programa/participantID (aplicável somente a programas da loja e do Azure Marketplace) |
| totalPayment | Pagamento total na moeda local, excluindo a retenção de imposto e incluindo o imposto sobre as vendas (se aplicável) para o programa/participantID |
| currencyCode | Código da moeda de pagamento |
| paymentMethod | O método usado para pagar o parceiro, por exemplo, transferência bancária eletrônica, nota de crédito |
| paymentID | Identificador exclusivo do pagamento. Esse número geralmente é visível em seu extrato bancário (aplicável somente a pagamentos SAP). |
| paymentStatus | Status de pagamento |
| paymentStatusDescription | Descrição amigável do status de pagamento |
| paymentDate | A data de pagamento foi enviada da Microsoft |
|

## <a name="export-data"></a>Exportar dados

A página **exportar dados** não é atualizada por conta própria. Talvez seja necessário atualizar a página manualmente para ver os dados mais recentes. Selecione entre as três guias para exportar o **histórico de transações**, os **pagamentos**, o **Resumo da transação** ou a **instrução histórica**.

O filtro pode resultar em um erro de **nenhum dado disponível** . Isso pode acontecer se você saiu do período de tempo padrão selecionado em três meses e, em seguida, selecionou uma ID de pagamento de uma conquista que está fora desse período. Se isso acontecer, expanda seu período de tempo e tente novamente.

Aqui está um exemplo de exportação de pagamentos:

:::image type="content" source="images/payouts/pc-export-payments.png" alt-text="Relatório de pagamentos de exportação.":::

### <a name="historical-statements"></a>Demonstrativo do histórico

O resumo dos **dados de exportação** também fornece acesso a instruções históricas.

> [!NOTE]
> Uma instrução histórica é um instantâneo e não é atualizada. Entre em contato [com o suporte](https://partner.microsoft.com/support/v2/?stage=1) e solicite os dados mais recentes, se necessário.

:::image type="content" source="images/payouts/pc-export-statements.png" alt-text="Exportar instruções históricas.":::

- O histórico de transações de antes de 1º de julho de 2019 é tratado separadamente e usa campos diferentes de relatórios de histórico posteriores.
- O histórico de transações herdadas tem uma coluna chamada "Reservado" que corresponde à coluna "Ganhos" no histórico moderno, exceto que exclui todos os ganhos com status igual a "Pagamento Enviado".
- Filtros como 3M, 6M ou 12M não serão aplicados à seção Demonstrativos do histórico.

### <a name="historical-statement-downloads"></a>Downloads de instrução histórica

A tabela a seguir explica cada coluna em uma instrução histórica.

| Nome do campo | Descrição |
| --- | --- |
| Origem da receita | A origem de sua receita com base no local no qual a transação ocorreu, como Microsoft Store, Windows Phone Store, Windows Store 8 ou publicidade |
| ID do pedido | Identificador exclusivo do pedido. Essa ID permite que você identifique as transações de compra com suas respectivas transações de não compra, como reembolsos ou estornos. Ambas terão a mesma ID de pedido. Além disso, se houver uma cobrança de divisão em que várias formas de pagamento foram usadas para uma única compra, ela permitirá vincular as transações de compra. |
| ID da transação | Identificador exclusivo da transação. |
| Data e hora da transação | A data e hora em que a transação ocorreu (UTC). |
| ID do produto pai | Identificador exclusivo do produto pai. Se não houver um produto pai na transação, ID do produto pai = ID do produto. |
| Produto ID | Identificador exclusivo do produto. |
| Nome do produto pai | O nome do produto pai. Se não houver um produto pai na transação, Nome do produto pai = Nome do produto. |
| Nome do Produto | O nome do produto |
| Tipo de produto | Tipo de produto, como aplicativo, complemento ou jogo |
| Quantidade | Quando a origem da receita é Microsoft Store para Empresas, a quantidade representa o número de licenças adquiridas. Para todas as outras origens de receita, a quantidade será sempre 1. Mesmo quando uma transação é dividida em dois itens de linha porque dois métodos de pagamento diferentes foram usados, cada item de linha mostrará uma quantidade de 1. |
| Tipo de transação | Tipo de transação, como compra, reembolso, inversão ou estorno |
| Forma de pagamento | Meio de pagamento do cliente usado na transação, como cartão, cobrança de operadora móvel ou PayPal |
| País/região | País/região em que a transação ocorreu |
| Provedor/vendedor local | Provedor/vendedor local do registro |
| Moeda da transação | Moeda da transação |
| Valor da transação | Valor da transação |
| Imposto remetido | Valor do imposto remetido (vendas, uso ou impostos sobre IVA/GST) |
| Recebimentos líquidos | Valor da transação menos o imposto remetido |
| Valor de armazenamento | O percentual dos recebimentos líquidos retidos pela Microsoft como valor pela disponibilização do aplicativo ou complemento na loja |
| Lucros do aplicativo | Recebimentos líquidos menos o valor de armazenamento |
| Impostos retidos | Valor do imposto de renda retido (ou seja, incluído no arquivo CSV **Reservado**) |
| Pagamento | Os lucros do aplicativo menos qualquer retenção de imposto sobre renda aplicável (valor mostrado na moeda da transação). Não incluído no arquivo CSV **Reservado**. |
| Taxa de FX | Taxa de câmbio estrangeira usada para converter a moeda da transação na moeda de pagamento |
| Moeda de pagamento | Moeda na qual seu pagamento é feito |
| Pagamento convertido | Valor de pagamento convertido na moeda de pagamento usando a taxa de FX |
| Modelo de pagamento de imposto | Parte responsável pelo pagamento de impostos (vendas, uso ou impostos sobre IVA/GST) |
| Data e hora da qualificação | A data e a hora em que os lucros da transação se tornam qualificados para pagamento (UTC). Quando um pagamento é criado, ele inclui os lucros da transação com uma data e hora de qualificação antes da data de criação do pagamento (incluída apenas no arquivo CSV **Reservado**). |
| Charges | Mostra uma divisão de todo o detalhamento de preço agregado na coluna Valor da transação (incluído apenas para o Azure Marketplace; não incluído no arquivo CSV **Reservado**). |
|||

## <a name="next-steps"></a>Próximas etapas

- [API de pagamento de parceiro](https://apidocs.microsoft.com/services/partnerpayouts)
- [Detalhes da política de pagamento](payout-policy-details.md)
- Para obter suporte à cobrança, entre em contato com o [suporte do editor do marketplace comercial](https://partner.microsoft.com/support/v2/?stage=1).
