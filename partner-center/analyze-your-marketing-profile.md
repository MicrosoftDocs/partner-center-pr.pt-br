---
title: Analisar clientes potenciais
ms.topic: article
ms.date: 06/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como usar a página de informações do leads para ver como você está capturando a atenção dos clientes de destino e gerando referências.
author: vikrambmsft
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOJUNE.20
ms.openlocfilehash: 6ddb9544e0c6f6a29540fe30d03d307318ddfdf8
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150209"
---
# <a name="analyze-your-leads---see-how-well-you-attract-target-customers-and-potential-referrals"></a>Analise seus leads – Veja como você atrai clientes-alvo e indicações potenciais
<!-- 
https://go.microsoft.com/fwlink/?linkid=849120
-->

**Funções apropriadas**: administrador de referências

A página **clientes potenciais** na seção **análise** em referências permite que você veja como suas referências estão sendo executadas. Revise essas métricas regularmente para ajudar a identificar tendências ou áreas que precisam de atenção e comece a direcioná-las para as suas metas de negócios.

Para ver seus dados de informações de clientes potenciais, no menu do Partner Center, acesse **referências > analisar > leads**.

## <a name="apply-filters"></a>Aplicar filtros

Próximo à parte superior da página **clientes potenciais** , você pode selecionar o período de tempo para o qual deseja mostrar os dados. A seleção padrão será **3M** (três meses). No entanto, em vez disso, será possível optar por mostrar dados de um período de seis meses ou um ano. Também será possível selecionar **Personalizado** para conferir os dados de todas as indicações em um período específico.

Será possível clicar no botão Filtros para abrir o painel que permite filtrar todos os dados nesta página por Nome do cliente, País, Tipo de acordo, Direção do acordo, Nome da solução e Status. Veja abaixo mais detalhes sobre esses filtros.

- **Nome do cliente**: o padrão será **Todos**. No entanto, será possível limitar os dados a um ou mais clientes que você selecionar.
- **País**: o padrão será **Todos**. No entanto, será possível limitar os dados a um ou mais países do cliente que você selecionar.
- **Programa de referência**: o padrão é **todos**, mas você pode limitar os dados a um programa de referência específico. Esse filtro só será visível se a sua organização estiver registrada no programa de referência.
- **Status**: o padrão será **Todos**. No entanto, será possível limitar os dados a indicações que contenham um ou mais tipos de status da indicação que você selecionar, como aceito, recusado, expirado, perdido e conquistado.
- **Tipo de qualificação**: o padrão é **todos**, mas você pode optar por limitar os dados a referências que são clientes potenciais do Marketplace ou clientes qualificados.

As informações de todos os gráficos listados abaixo refletem o intervalo de datas e todos os filtros selecionados, exceto pelo que é observado abaixo. Algumas seções também permitem que você aplique filtros adicionais, tais como a filtragem para uma solução específica.

## <a name="referrals-summary"></a>Resumo das indicações

Este cartão mostra uma visão geral de como seus leads estão sendo executados.

O gráfico mostra o número total de visitas à página, o número de chamadas para botão de ação (parceiro de contato) clica, o número de leads gerados após os clientes clicarem na chamada de ação e o total de leads ganhos pelo período de tempo selecionado.

O percentual de métricas de alteração (mostrada em vermelho ou verde com um indicador de seta) indicará a diferença entre o **último mês no intervalo de datas selecionado** e o **primeiro mês nesse intervalo**. Por exemplo, digamos que a data atual seja 15 de junho e você selecionou o filtro **3M** para mostrar dados dos últimos três meses. Nesse caso, essas métricas mostrariam a diferença entre maio (o último mês completo no período de tempo selecionado) e março (o primeiro mês completo no período de tempo selecionado). Se o intervalo de datas selecionado fosse dos últimos **3M**, a comparação seria entre os dados de maio e os de março.

:::image type="content" source="images/referrals/leadsanalyticssummary.png" alt-text="Imagem mostrando o cartão de resumo da análise de leads.":::

## <a name="conversion-funnel"></a>Funil de conversão

Esta seção mostrará um indicador visual de como seus acordos estão mudando de estado por meio do ciclo de vida. Será possível exibir todo o ciclo de vida com base no volume de acordos, no valor deles em USD e na principal tabela dinâmica desta seção. A primeira seção é rotulada com o tipo de negócio para fornecer um indicador visual do volume ou valor por tipo. Também há uma seção, que **leva do passado**, que é usada para indicar as negociações para as quais você executou a ação de aceitá-las ou detectá-las ou marcá-las como ganhas/perdidas no período de tempo selecionado para o relatório. Será possível aplicar filtros para exibir o progresso dos acordos em vários estágios do ciclo de vida.

:::image type="content" source="images/referrals/leadsanalyticsfunnel.png" alt-text="Imagem mostrando um funil de conversão para as indicações.":::

## <a name="leads-by-geography"></a>Clientes potenciais por geografia

Esta seção mostrará os países/as regiões de origem dos acordos, juntamente com detalhes de cada país/região. Há uma exibição de tabela com os detalhes do acordo para cada país, junto com uma exibição de mapa de todos os países. Será possível clicar em um país específico na tabela ou clicar na exibição de mapa para aplicar zoom a um país específico.

:::image type="content" source="images/referrals/leadsanalyticsgeodistribution.png" alt-text="Imagem mostrando a distribuição geográfica das indicações.":::

## <a name="leads-by-program"></a>Clientes potenciais por programa

Essa combinação de tabela e gráfico permite ver qual dos seus leads do programa de referência está orientando a maioria das referências e o maior valor de negócio.
A tabela tem o total de leads, os leads que foram aceitos com no SLA (24 horas) em termos percentuais e absolutos, os leads que expiraram e os leads que entraram no estado ganho junto com o valor total de leads ganho em moeda em USD. Também há um grafo de tendência de leads à direita da tabela que mostra as contagens totais de negociações e o valor da negociação ganho em moeda em USD com base no programa selecionado. A seleção padrão será Todas as soluções.

:::image type="content" source="images/referrals/leadsanalyticsreferralsprogram.png" alt-text="Imagem mostrando o desempenho do programa de indicações qualificado.":::

## <a name="declined--lost-reasons"></a>Motivos de acordos recusados e perdidos

Esta seção ajudará você a analisar os motivos pelos quais os leads estão sendo marcados como **Recusados** ou **Perdidos** por sua empresa. As opções nessas representações são os mesmos motivos pelos quais os vendedores optaram por fechar o lead como recusado ou perdido.

:::image type="content" source="images/referrals/leadsanalyticsreasons.png" alt-text="Imagem mostrando os motivos selecionados pelo parceiro ao declinar ou fazer um lead como perdido.":::

## <a name="comparison-charts"></a>Gráficos de comparação

A seção de comparação ajudará você a comparar os dados relacionados a clientes com base em várias dimensões, tanto no volume quanto no valor ganho de leads em USD pivot.
As três dimensões que você pode escolher para comparar os dados são:

- Tipo de qualificação
- Mercados
- Programa de indicação

Quando o tipo de qualificação é selecionado, você tem a opção de comparar o desempenho de indicações de em relação a leads do marketplace e leads qualificados. Para mercados e programa de indicação, você pode escolher até três opções diferentes para comparar o desempenho. O primeiro grafo, que é um gráfico de barras, terá dados apresentados com uma tendência mês a mês baseada na tabela dinâmica principal, que representa o volume ou o valor de acordos conquistados. Também há um gráfico de pizza à direita do gráfico de barras, que mostrará a distribuição por percentual para obter os mesmos dados.

:::image type="content" source="images/referrals/leadsanalyticscompare.png" alt-text="Imagem mostrando a seção de comparação.":::

## <a name="raw-data-table"></a>Tabela de dados brutos

A tabela abaixo com todos os dados brutos  relacionados aos leads ajudará você a exportar rapidamente os dados para qualquer análise detalhada ou personalizada que você deseja executar.

:::image type="content" source="images/referrals/leadsanalyticsrawdata.png" alt-text="Imagem mostrando a tabela de dados brutos para clientes.":::

## <a name="no-data"></a>Sem dados

Pode haver vários motivos pelos quais você está recebendo um gráfico em branco, como abaixo, ao acessar a análise de leads, conforme descrito abaixo.

- Não há dados para esta conta. Tente criar acordos para que este relatório seja preenchido.
- A conectividade de rede apresentou um problema. Verifique sua conexão com a Internet e tente novamente.
- Não há registros correspondentes aos filtros que você aplicou. Tente redefinir os filtros.
- Há um atraso entre a alteração de estado do líder e para que o mesmo seja atualizado no relatório de análise. Verifique o relatório após 24 horas.

:::image type="content" source="images/referrals/nodata.png" alt-text="Imagem mostrando nenhuma visualização de dados para clientes.":::

> [!TIP]
> Para ver o desempenho de suas oportunidades de venda co-venda, consulte a página [Insights de oportunidades de venda co-venda](referral-insights.md).

## <a name="next-steps"></a>Próximas etapas

- [Gerenciar vendas potenciais](manage-leads.md)
