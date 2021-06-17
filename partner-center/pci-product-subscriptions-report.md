---
title: Partner Center de assinaturas do Partner Center Insights
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Veja o que você está fazendo bem e onde pode melhorar em relação às assinaturas de nuvem que você vende ou gerencia para seus clientes.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bf2663122ca95e8d610c8be792a26682ae1718bf
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276307"
---
# <a name="product-subscriptions-report-available-from-the-partner-center-insights-dashboard"></a>Relatório de Assinaturas de Produto disponível no painel Partner Center Insights

**Funções apropriadas:** administrador global | Agente administrador | Visualizador de | Visualizador de relatório executivo

O relatório Assinaturas de Produto apresenta análises sobre assinaturas de nuvem que você vende ou que você gerencia para seus clientes. Este é um relatório específico do produto que inclui o desempenho de assinaturas associadas a produtos de nuvem, como Office 365, Azure, Dynamics e outros.

Você pode exibir as seções a seguir no relatório Assinaturas de Produto.

- Resumo
- Distribuição geográfica de assinaturas
- Tendência de adoção/variação de assinaturas
- Distribuição de assinatura por locais de parceiros, canal de vendas, SKUs, tipo de anexação de parceiro, segmento
- Tendência por estados de assinatura
- Tendência de produtos

 > [!NOTE]
 > Este relatório está disponível no painel insights. Para exibir esse relatório, você deve ter uma função específica no Partner Center, como Administrador Global, Administrador da Conta, Visualizador de Relatório ou Visualizador de Relatório Executivo. Para obter mais informações, consulte Administrador Global da sua empresa. Tipos específicos de dados neste relatório também podem estar disponíveis somente para usuários com privilégios de Visualizador de Relatório Executivo.

## <a name="summary"></a>Resumo

A seção de resumo apresenta uma exibição de instantâneo dos KPIs (indicadores chave de desempenho) relacionados a assinaturas vendidas ou gerenciadas por você para seus clientes.  

:::image type="content" source="images/pci/pci-sub-report-summary-1.png" alt-text="resumo do relatório de assinaturas.":::

Para obter mais informações sobre cada seção do resumo, consulte abaixo:

- Assinaturas:
  - Contagem atual das assinaturas de produto de nuvem vendidas ou gerenciadas por você.
  - Percentual de crescimento ou redução de assinaturas durante o intervalo de datas selecionado.
  - O micro gráfico apresenta uma tendência mensal da contagem de assinaturas durante o intervalo de datas selecionado.

- Assinaturas ativas:
  - Contagem atual de assinaturas de produtos de nuvem com Uso ativo medido com base na telemetria do produto. Isso exclui todas as assinaturas de avaliação no caso de assinaturas do Azure.
  - Percentual de crescimento ou redução de assinaturas ativas durante o período selecionado.
  - O micro gráfico apresenta uma tendência mensal de assinaturas ativas durante o intervalo de datas selecionado.

- Assinaturas adicionadas:
  - Total de assinaturas do cliente adicionadas (vendidas ou gerenciadas) por você durante o intervalo de datas selecionado. Novas assinaturas com **estado Ativo** **ou Renovado** são contadas como Assinaturas adicionadas.
  - Percentual de crescimento ou redução de assinaturas adicionadas no último mês completo em comparação com o primeiro mês completo.
  - O micro gráfico apresenta uma tendência mensal de assinaturas adicionadas durante o intervalo de datas selecionado.

- Assinaturas rotativas:
  - Total de assinaturas de cliente rotatividade durante o intervalo de datas selecionado. As assinaturas com estado **Desprovisionado** **ou Suspenso** nesse mês são contadas como uma assinatura rotatividade.  
  - Percentual de assinaturas rotativas durante o intervalo de datas selecionado.
  - O micro gráfico apresenta uma tendência mensal de assinaturas rotativas ao longo do intervalo de datas selecionado.

- Assinaturas por produtos: detalhamento da contagem de assinaturas atual por produtos de nuvem.

## <a name="geographical-spread-of-subscriptions"></a>Distribuição geográfica de assinaturas

A **exibição Assinaturas por** geografia mostra a distribuição geográfica do total de assinaturas por mercados de clientes. O valor total da assinatura inclui assinaturas vendidas e assinaturas ativas.

A **tabela Número de países/regiões** apresenta o total de países/regiões em que você tem assinaturas e a quantidade por país de assinaturas totais e ativas.

Você pode pesquisar e selecionar um país na grade para ampliar o local no mapa. Pressione a **opção** Página Inicial no mapa para reverter para a exibição original. Passe o mouse sobre o mapa para exibir todas as assinaturas e assinaturas ativas por país. Ambos os campos na grade são sortíveis.

:::image type="content" source="images/pci/pci-sub-report-sub-by-geography-2.png" alt-text="assinaturas por geografia.":::

## <a name="subscription-addschurns"></a>Adicionações/rotatividades de assinatura

Essa exibição apresenta uma tendência de assinaturas. Eles são divididos em categorias diferentes (Novo, Existente, Rotatividade) para o intervalo de datas selecionado. O eixo X representa meses do intervalo de datas selecionado. O eixo Y representa a contagem de assinaturas. As assinaturas rotativas são representadas na escala negativa do eixo Y. 

O gráfico de colunas empilhadas apresenta um detalhamento de assinaturas novas, existentes e rotativas para o mês. Você pode recriar o gráfico de colunas, dividido com itens de pilha específicos. Para fazer isso, selecione esses itens específicos na legenda. Você também pode usar o controle deslizante na parte superior do gráfico para ampliar um período específico.

:::image type="content" source="images/pci/pci-sub-report-sub-adds-churns-3.png" alt-text="A assinatura adiciona e rotatividade.":::

## <a name="subscription-distribution"></a>Distribuição de assinatura

Essa exibição apresenta um detalhamento de suas assinaturas atuais por seus locais de MPN, segmentos de clientes, modelo de preços do canal de vendas/Azure e o tipo de atribuição (por exemplo, DPOR, DAP e outros). Selecione as respectivas guias para exibir o detalhamento por essas categorias. Para criar o gráfico de pizza com um detalhamento de categorias de item específicas, selecione essas categorias de item na legenda.

:::image type="content" source="images/pci/pci-sub-report-distribution-4.png" alt-text="distribuição de assinatura.":::

## <a name="subscription-state-distribution"></a>Distribuição de estado da assinatura

Essa exibição mostra a distribuição das assinaturas atuais do cliente por estado ou status da assinatura. Isso inclui os seguintes estados de assinatura: **Ativo,** Desabilitado, **Desprovisionado,** **Abrir**, **InGracePeriod,** **Fechado** e **Outros.**

:::image type="content" source="images/pci/pci-sub-report-sub-states-5.png" alt-text="distribuição de estado da assinatura.":::

## <a name="products-trend"></a>Tendência de produtos

Esta exibição mostra um gráfico de barras e dois gráficos de pizza. O gráfico de barras apresenta uma tendência mensal de assinaturas divididas por produtos comerciais, como Azure, Office, Dynamics etc.

Os dois gráficos de pizza mostram um detalhamento das assinaturas atuais do cliente. O primeiro gráfico de pizza divide as assinaturas por produtos. O segundo gráfico de pizza divide as assinaturas por SKUs ou planos. Quando você seleciona um  produto no gráfico de pizza detalhamento por Produtos, o gráfico de pizza adjacente mostrará um detalhamento das assinaturas desse produto por SKUs.

:::image type="content" source="images/pci/pci-sub-report-prods-trend-6.png" alt-text="tendência de produtos.":::

> [!NOTE]
 > A contagem de assinaturas dividida por SKUs nem sempre pode corresponder à contagem total de assinaturas desse produto. Isso poderá ocorrer se um cliente tiver comprado vários SKUs na mesma assinatura do produto.

## <a name="next-steps"></a>Próximas etapas

- Para obter mais relatórios, [consulte Partner Center Insights.](partner-center-insights.md)

>[!NOTE] 
> Você pode baixar os dados brutos que agem neste relatório na seção Baixar Relatórios no painel Insights. [Saiba mais](pci-download-reports.md) 
