---
title: Painel de visão geral de informações do Partner Center
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Veja um instantâneo de como você está fazendo com vendas e implantação, crescimento do cliente e crescimento da receita com licenças, assinaturas e consumo do Azure.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 14d280a65fa7c72ed382fd8b27e0354a4aa9e190
ms.sourcegitcommit: 078eac1456f68585ff1003b21e5e1fe777af314b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "108120810"
---
# <a name="overview-dashboard-reports-available-in-partner-center-insights"></a>Visão geral dos relatórios do painel disponíveis em Insights do Partner Center
 
**Funções apropriadas**

- Administrador global
- Agente administrativo
- Visualizador de relatórios
- Visualizador de relatórios executivos

O painel Visão geral do insights fornece uma exibição de instantâneo dos principais indicadores de desempenho, como clientes, assinaturas, receita de consumo do Azure e licenças. Você pode visualizar os gráficos a seguir no relatório de visão geral.

- Resumo  
- Distribuição geográfica de seus clientes, assinaturas e licenças  
- Tendência de crescimento dos clientes 
- Tendência de crescimento de assinaturas 
- Tendência de crescimento da receita consumida pelo Azure 
- Tendência de crescimento de licenças 

## <a name="summary"></a>Resumo

O resumo inclui informações sobre clientes, ACR (receita consumida do Azure), assinaturas vendidas, assinaturas ativas e licenças implantadas. 

:::image type="content" source="images/pci/summary.png" alt-text="Licenças de resumo":::

Veja a seguir mais informações sobre cada seção do resumo.

### <a name="customers"></a>Clientes

A área **clientes** inclui:

- A contagem atual de todos os clientes com pelo menos uma assinatura ativa associada à sua empresa por meio de diferentes tipos de atribuição e em todos os produtos de nuvem.
- O percentual de crescimento de clientes durante o intervalo de datas selecionado.
- O micro gráfico apresenta a tendência mês a mês da contagem de clientes dentro do intervalo de datas selecionado.

### <a name="azure-consumed-revenue-acr"></a>Receita consumida do Azure (ACR)

A área de **receita consumida do Azure (ACR)** no resumo inclui:

- A receita total consumida do Azure (em US $) atribuída a você no intervalo de datas selecionado.
- O percentual de crescimento ou declínio no ACR atribuído (em US $) durante o intervalo de datas selecionado.
- O micro Chart apresenta uma tendência mensal de ACR US $ atribuído a você no intervalo de datas selecionado 

> [!NOTE]
> Os dados de receita consumida do Azure (ACR) estão disponíveis para usuários que receberam a função de visualizador de relatórios executivos 
 
### <a name="subscriptions-sold"></a>Assinaturas vendidas

A área de **assinaturas vendidas** no resumo inclui:

- A contagem total atual de assinaturas de produtos de nuvem (ativas e inativas) vendidas ou gerenciadas por você.  
- O percentual de crescimento ou declínio nas assinaturas durante o intervalo de datas selecionado.
- O micro gráfico apresenta a tendência de mês a mês do total de assinaturas no intervalo de datas selecionado.

### <a name="active-subscriptions"></a>Assinaturas ativas

A área de **assinaturas ativas** no resumo inclui:

- A contagem atual de assinaturas de produtos de nuvem com uso ativo medido com base na telemetria do produto. Isso exclui todas as assinaturas de avaliação no caso de assinaturas do Azure.  
- O percentual de crescimento de assinaturas ativas no intervalo de datas selecionado.
- O micro gráfico apresenta a tendência mês a mês das assinaturas ativas no intervalo de datas selecionado.
 
### <a name="licenses-deployed"></a>Licenças implantadas

A área de **licenças implantadas** no resumo inclui:
 
- A contagem de todas as licenças de produtos de nuvem implantadas em suas assinaturas de cliente no período de tempo selecionado. 
- O percentual de crescimento ou declínio dessas licenças durante o intervalo de datas selecionado. 
- O micro Chart mostra a tendência mês a mês dessa contagem de licenças atribuídas no intervalo de datas selecionado.

## <a name="geographical-spread-of-your-customers-subscriptions-and-licenses"></a>Distribuição geográfica de seus clientes, assinaturas e licenças

Essa exibição é uma distribuição geográfica do total de clientes, assinaturas e licenças por país do cliente. Selecione as diferentes guias para exibir cada uma dessas informações no mapa. Você pode pesquisar e selecionar um país na grade para aplicar zoom ao local no mapa. Reverta para a exibição original pressionando o botão página inicial no mapa. Clicar em cada guia (por exemplo, clientes, assinaturas) mostra o valor da métrica para cada país e a porcentagem do total do país.  

:::image type="content" source="images/pci/geosummary.png" alt-text="Resumo geográfico":::

## <a name="customers-growth-trend"></a>Tendência de crescimento dos clientes

Tendência mensal de contagens totais de clientes para o intervalo de datas selecionado. O eixo X representa meses do intervalo de datas selecionado e eixo Y representa a contagem total de clientes para esse mês. 

:::image type="content" source="images/pci/customergrowth.png" alt-text="tendência de crescimento dos clientes":::

## <a name="subscriptions-growth-trend"></a>Tendência de crescimento de assinaturas

Isso indica a tendência de sua contagem de assinaturas de cliente para o intervalo de datas selecionado. Eixo X representa meses do intervalo de datas selecionado e eixo Y representa a contagem de assinaturas do produto selecionado. Percorra o controle deslizante na parte superior do gráfico para aplicar zoom no gráfico para um período de tempo específico. 

:::image type="content" source="images/pci/subscriptiongrowth.png" alt-text="Tendência de crescimento da assinatura":::

## <a name="azure-consumed-revenue-growth-trend"></a>Tendência de crescimento da receita consumida pelo Azure

Tendência mensal de receita consumida pelo Azure US $ atribuída a você no intervalo de datas selecionado. O eixo X representa os meses do intervalo de datas selecionado e o eixo Y representa a receita total consumida do Azure US $ atribuídas a você durante o mês.

> [!NOTE]
> A receita consumida do Azure (ACR) só ficará visível para os usuários aos quais foi atribuída a função de visualizador de relatórios executivos. 

:::image type="content" source="images/pci/azureconsumed.png" alt-text="Consumo do Azure":::

## <a name="licenses-growth-trend"></a>Tendência de crescimento de licenças
 
Tendência de licenças atribuídas por todos os clientes durante o intervalo de datas selecionado. Eixo X representa meses do intervalo de datas selecionado e eixo Y representa a contagem de licenças do produto que você selecionou. Percorra o controle deslizante na parte superior do gráfico para aplicar zoom no gráfico para um período de tempo específico.  

:::image type="content" source="images/pci/licensesgrowth.png" alt-text="licenças":::

## <a name="next-steps"></a>Próximas etapas

Para obter mais relatórios, consulte os [insights do Partner Center](partner-center-insights.md).
