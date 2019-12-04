---
title: Diferenças de cobrança mensal e anual | Centro de parceiros
ms.topic: article
ms.date: 11/25/2019
Description: Saiba mais sobre as diferenças entre os ciclos de cobrança mensal e anual no Partner Center.
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
ms.localizationpriority: medium
ms.openlocfilehash: 1b5d9b8175f2d64998efaf2e64e3d1adbdbc2f75
ms.sourcegitcommit: c793c1b61f50fc0b0a12c95cedd9f57b31703093
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2019
ms.locfileid: "74722411"
---
# <a name="monthly-and-annual-billing-differences"></a>Diferenças de cobrança mensal e anual

**Aplica-se a**

- Partner Center
- Partner Center do Microsoft Cloud for US Government

**Funções apropriadas**

- Agente administrativo
- Administrador de cobrança
- Administração global
- Administrador de incentivos
- Usuário de incentivos
- Agente de suporte técnico
- Agente de vendas

Este tópico explica as diferenças entre **cobrança mensal** e **cobrança anual** no Partner Center, incluindo benefícios e casos de uso. Você tem a opção de pagar por determinadas assinaturas do CSP (provedor de soluções na nuvem) de acordo com uma base mensal ou anual.

## <a name="applicability"></a>Aplicabilidade

A maioria das assinaturas baseadas em licenciado tem a opção para a opção de cobrança mensal ou anual. As assinaturas baseadas em uso só apresentam a opção de cobrança mensal.

A cobrança anual e mensal são **por assinatura**,  ***não* por licença**.

### <a name="find-subscription-applicability"></a>Encontrar a aplicabilidade da assinatura

Você pode identificar as frequências de cobrança disponíveis para cada oferta usando a coluna J na matriz de oferta. Você pode encontrar a matriz de ofertas na seção **ver ofertas e preços** no Partner Center.

### <a name="applicable-partners"></a>Parceiros aplicáveis

Todos os parceiros e tipos de parceiros podem escolher cobrança mensal ou anual.

### <a name="applicable-markets"></a>Mercados aplicáveis

A cobrança mensal e anual (para ofertas aplicáveis) está disponível em todos os mercados em que o programa CSP está disponível no momento.

## <a name="change-billing-frequency"></a>Alterar frequência de cobrança

Você pode alternar entre a cobrança mensal e anual a qualquer momento. Talvez você queira alterar sua frequência de cobrança se suas necessidades comerciais mudarem.

Quando você altera a frequência de cobrança para anual, o termo anual é atualizado para refletir a data em que você alterou a frequência de cobrança. Uma nova data de renovação também é estabelecida.

### <a name="monthly-to-annual-billing"></a>Cobrança mensal a anual

Alternar de cobrança mensal para cobrança anual pode ser útil se você tiver várias assinaturas que são cobradas mensalmente. Ao alternar para a cobrança anual, você pode alinhar as assinaturas em uma data de cobrança comum.

### <a name="annual-to-monthly-billing"></a>Cobrança anual para mensal

A mudança de cobrança anual para cobrança mensal pode ser útil se você quiser ajustar suas datas de cobrança para as de seus clientes individuais.

## <a name="annual-billing"></a>Cobrança anual

A cobrança anual tem os seguintes benefícios:

- Maior flexibilidade nas opções de pagamento.
- Melhor alinhamento com o faturamento dos seus clientes.
- Impacto reduzido nas flutuações de moeda.
- Custos operacionais de cobrança reduzidos.

### <a name="configure-annual-billing"></a>Configurar cobrança anual

Se estiver planejando mudar para a cobrança anual no Partner Center, considere como seu movimento de vendas será afetado. Você deve informar sua equipe e atualizar seus processos internos conforme necessário. Você também deve examinar as alterações em seu arquivo de reconciliação baseado em licença e fatura. 

Também será necessário [atualizar suas APIs para cobrança anual](#required-api-changes).

#### <a name="required-api-changes"></a>Alterações de API necessárias

Para aproveitar a cobrança anual, algumas mudanças são necessárias para suas APIs.

- [Propriedade Order. BillingCycle](https://docs.microsoft.com/dotnet/api/microsoft.store.partnercenter.models.orders.order.billingcycle)
- [Criar um pedido](https://docs.microsoft.com/partner-center/develop/create-an-order)

Para obter mais informações sobre as APIs do Partner Center, consulte todos os [recursos e documentação do desenvolvedor do Partner Center](https://docs.microsoft.com/partner-center/develop/).

## <a name="placing-orders"></a>Colocando pedidos

O tipo de frequência de cobrança, incluindo a opção de cobrança anual, é atribuído à **oferta** como um atributo. Não há uma oferta exclusiva especificamente para pedidos com cobrança anual. Entretanto, você pode renomear uma oferta usando um nome de cliente mais amigável para permitir a diferenciação.

### <a name="select-annual-billing"></a>Selecionar cobrança anual

Ao adicionar uma nova assinatura, você será solicitado a escolher a frequência de cobrança. Você pode escolher a opção de cobrança anual nesse ponto. Quando você selecionar cobrança anual, todas as ofertas disponíveis serão exibidas.

### <a name="billing-time"></a>Tempo de cobrança

Você será cobrado na próxima data de cobrança. Por exemplo, se a data de cobrança for a primeira do mês e você comprar uma assinatura anual cobrada em 29 de outubro de 2019, você será cobrado em 1º de novembro de 2019. Supondo que você não faça nenhuma alteração de licença, você será cobrado novamente em 1º de novembro de 2020. Se você fizer uma alteração de licença, receberá um crédito e faturará sua próxima data de cobrança.

### <a name="annual-renewals"></a>Renovações anuais

A data de renovação da sua assinatura será de 12 meses após a data de início do serviço. O período de serviço começa na data em que a assinatura é criada.  Por exemplo, uma assinatura criada em 10 de janeiro de 2019 será renovada em 10 de janeiro de 2020.

Você será cobrado na próxima data de cobrança após a data de renovação da assinatura. Por exemplo, se você comprar uma assinatura com cobrança anual em 15 de janeiro de 2018 e se a sua data de cobrança for 20 de janeiro, sua assinatura será renovada em 15 de janeiro de 2019. Você será cobrado pela renovação em 20 de janeiro de 2019.

### <a name="split-subscription-billing-frequency"></a>Frequência de cobrança da assinatura dividida

Não é possível dividir uma **única assinatura** para que uma delas seja cobrada mensalmente e a outra parte seja cobrada anualmente. A assinatura inteira deve ter a mesma frequência de cobrança (cobrança mensal ou anual).

Para clientes com **várias assinaturas** da mesma oferta, talvez seja possível ter frequências de cobrança diferentes por assinatura. Há algumas ofertas restritas a uma assinatura por cliente. Se a oferta não estiver restrita, o cliente poderá ter várias assinaturas da mesma oferta com diferentes frequências de cobrança. Você pode encontrar os detalhes de todos os limites e restrições de oferta na coluna I da matriz de ofertas. Você pode encontrar a matriz de ofertas na seção **ver ofertas e preços** no Partner Center.

### <a name="free-subscription-period"></a>Período de assinatura livre

As assinaturas com frequência de cobrança anual não recebem um período gratuito. O termo pago por doze meses começa na data de compra. Isso é diferente de assinaturas com frequência de cobrança mensal que recebem um período gratuito entre a data da compra e a próxima data de cobrança.

### <a name="adding-and-removing-licenses"></a>Adicionando e removendo licenças

Você pode alterar a quantidade de licenças das suas assinaturas a qualquer momento. A adição de outras licenças não afetará a frequência de cobrança.

Você pode adicionar ou remover licenças a qualquer momento.  Você receberá um crédito e uma fatura rateada em sua próxima data de cobrança depois de alterar o número de licenças.

Se sua assinatura existente tiver cobrança anual, não será possível adicionar licenças com cobrança mensal a essa assinatura. Assim que você comprar uma assinatura com cobrança anual, todas as licenças adicionais seguirão a mesma frequência de cobrança. Se então você precisar comprar licenças com cobrança mensal, precisará comprar uma nova assinatura.

### <a name="add-on-offers"></a>Ofertas de complemento

A assinatura complementar terá automaticamente a mesma frequência de cobrança da assinatura principal. A cobrança anual está disponível para ofertas de complemento. 

### <a name="cancelling-subscriptions"></a>Cancelando assinaturas

A política de cancelamento é a mesma para todas as frequências de cobrança.

Para cobrança anual, se a assinatura for cancelada nos primeiros 30 dias do termo pago por doze meses, você receberá um crédito de 100% na sua próxima data de cobrança. Se a assinatura for cancelada após 30 dias do termo pago por doze meses, você receberá um crédito rateado na próxima data de cobrança.

### <a name="moving-subscriptions-between-partners"></a>Movendo assinaturas entre parceiros

Os clientes não podem mover assinaturas entre um parceiro para outro. Isso se aplica a assinaturas cobradas mensal e anualmente.

O novo parceiro deve comprar uma nova assinatura em nome do cliente. Não é possível mover assinaturas entre parceiros.

### <a name="reactivating-subscriptions"></a>Reativando assinaturas

Você pode reativar uma assinatura por até 90 dias após a data de suspensão. Você receberá uma cobrança proporcional na data de cobrança seguinte. A data de renovação da assinatura permanece a mesma.

## <a name="pricing"></a>Preço

### <a name="offer-pricing"></a>Preço da oferta

O preço da oferta no momento da compra é garantido para o período de assinatura total cobrado (um mês para cobrança mensal, doze meses para cobrança anual). Quando uma assinatura for renovada, o preço se baseará na lista de preços atual na data de renovação. O novo preço é garantido para o próximo prazo de assinatura.

Se um preço de oferta diminuir durante o período de cobrança, o valor cobrado não será alterado. O preço é definido para o período de cobrança completo no momento da compra. Isso se aplica a cobranças mensais e anuais.

### <a name="cancellation-credits"></a>Créditos de cancelamento

O crédito de uma licença ou assinatura cancelada é calculado da seguinte maneira:

**Crédito de cancelamento** = ((* * preço mensal * * * 12)/365) \* **dias restantes no termo de doze meses** \* número de licenças canceladas.

## <a name="reconciliation-file"></a>Arquivo de reconciliação

### <a name="find-subscriptions-billing-frequency"></a>Localizar a frequência de cobrança da assinatura

Examine seu arquivo de reconciliação baseado em licença para obter informações sobre se sua assinatura é cobrada mensal ou anualmente. Essas informações estão na coluna **AA**.

Para descobrir se você pode alterar uma assinatura mensal para cobrança anual, consulte [encontrar a aplicabilidade da assinatura](#find-subscription-applicability).

### <a name="reconciliation-file-changes-for-annual-billing"></a>Alterações de arquivo de reconciliação para cobrança anual

Quando você comprar ou renovar uma assinatura com cobrança anual, o arquivo de reconciliação baseado em licença será alterado da seguinte maneira.

Uma nova linha no arquivo de reconciliação com base em licença na primeira data de cobrança após a compra ou uma nova assinatura.

Se nenhuma alteração for feita na assinatura, não haverá linhas nos arquivos de reconciliação para o segundo mês até o décimo-segundo do período da assinatura. Se uma alteração for feita na assinatura durante o período de doze meses, um crédito e uma fatura rateada serão exibidos no próximo arquivo de reconciliação depois que a alteração for feita.

A próxima alteração no arquivo de reconciliação será exibida quando a assinatura for renovada. Isso será exibido na data da primeira cobrança após a renovação.

### <a name="usage-file-changes-for-annual-billing"></a>Alterações de arquivo de uso para cobrança anual

As seguintes alterações de assinatura cobradas anualmente aparecem na coluna P do seu arquivo de uso.

- **Taxas de tarifas ao comprar**: a compra inicial de uma assinatura anual.
- **Taxa de classificação da instância do ciclo**: alterações de licença que resultam em crédito e cobrança.
- **Cancelar taxa**: o [cancelamento de uma assinatura anual](#cancellation-of-annual-subscription).

### <a name="cancellation-of-annual-subscription"></a>Cancelamento da assinatura anual

Quando uma assinatura cobrada anualmente for cancelada, o arquivo de reconciliação conterá um item de linha para um crédito de cancelamento.

Se o cancelamento ocorrer nos primeiros 30 dias do período de doze meses, a assinatura será creditada em 100%. Se o cancelamento ocorrer após os 30 primeiros dias, a assinatura será creditada de forma proporcional.

### <a name="adding-licenses-to-annual-subscription"></a>Adicionando licenças à assinatura anual

Quando você adiciona licenças a uma assinatura, o arquivo de reconciliação conterá um crédito e uma fatura rateada. Isso se aplica a assinaturas faturadas mensais e anuais.

### <a name="price-lists-for-annual-billing"></a>Listas de preços para cobrança anual

As listas de preços do Partner Center mostram os preços mensais. Não há nenhum preço anual listado. Você pode calcular o preço anual multiplicando o preço mensal por doze.

### <a name="offer-matrix"></a>Matriz de oferta

As IDs de oferta na matriz de oferta são as mesmas para todas as frequências de cobrança. Não há IDs exclusivas para ofertas que podem ser cobradas anualmente.

## <a name="incentives"></a>Incentivos

### <a name="incentives-calculation"></a>Cálculo de incentivos

Os incentivos são calculados com base na **receita cobrada**,  ***não* na receita ajustada**. Os pagamentos de incentivos ganhos serão efetuados de acordo com nossa política encontrada em nossos guias de incentivos do CSP.

Quando uma assinatura anual cobrada é vendida, a receita da assinatura é reconhecida para o cálculo de incentivos com base na receita cobrada.

### <a name="payout"></a>Pagamento

Atualmente, todos os pagamentos de incentivos são feitos duas vezes por ano. Esses pagamentos são feitos 45 dias após o fim do semestre.

### <a name="rates"></a>Taxas

Os parceiros ganham incentivos em todas as transações qualificadas, independentemente de como uma assinatura é cobrada. Os ganhos de incentivo são calculados com base na taxa de incentivo global (que é aplicada à receita cobrada para o período), o acelerador local (para todas as geografias em que há aceleradores locais) e quaisquer campanhas globais (quando aplicável).

### <a name="contacts"></a>Contatos

Para dúvidas sobre incentivos, entre em contato com a equipe de suporte de incentivos regionais apropriada:

| Region | Endereço de email |
| ------ | ------------- |
| América do Norte | <ocina@microsoft.com> |
|América Latina & Brasil | <ocilatam@microsoft.com> |
| EMEA | <ociemea@microsoft.com> |
| APOAC (exceto Japão) | <ociapgc@microsoft.com> |
| Japão | <ocijp@microsoft.com> |


### <a name="suspension"></a>Suspensões

Se você suspender uma assinatura (no Partner Center ou por meio das APIs) dentro de 30 dias após a compra, receberá um crédito de 100%, independentemente da frequência de cobrança.

Para cobrança anual:

1. O parceiro compra a assinatura em 1º de Janeiro. Uma linha de cobrança de encargo é criada para o período de serviço de 1º de janeiro a 31 de dezembro.
2. O parceiro suspende a assinatura em 25 de Janeiro. Uma linha de cobrança de crédito é criada para o período de serviço de 1º de janeiro a 31 de dezembro.
3. O reativa a assinatura em 29 de Janeiro. Uma linha de cobrança de encargo é criada para o período de serviço em 29 de janeiro a 31 de dezembro.

Para cobrança mensal:

1. O parceiro compra a assinatura em 1º de Janeiro. Uma linha de cobrança de encargo é criada para o período de serviço de 1º de janeiro a 31 de Janeiro.
2. O parceiro suspende a assinatura em 25 de Janeiro. Uma linha de cobrança de crédito é criada para o período de serviço de 1º de janeiro a 31 de Janeiro.
3. O parceiro reativa a assinatura em 29 de Janeiro. Uma linha de cobrança de encargo é criada para o período de serviço em 29 de janeiro a 31 de Janeiro.
