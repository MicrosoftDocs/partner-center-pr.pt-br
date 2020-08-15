---
title: Análises de Microsoft Learn do Partner Center
ms.topic: article
ms.date: 08/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Acompanhe os aprendizes em sua empresa aproveitando os dados em treinamento individual, módulos concluídos, caminhos de aprendizado concluídos e muito mais.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 42c7af80ab49cee6e7043587207e553d2ffaa3ac
ms.sourcegitcommit: 735593129d1a009854a4ed0b03b11035211dbb25
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/14/2020
ms.locfileid: "88239446"
---
# <a name="the-microsoft-learn-analytics-report-shows-the-status-of-learners-in-your-company"></a>O relatório de análise de Microsoft Learn mostra o status dos aprendizes em sua empresa

**Funções apropriadas**
-   Administrador global
-   Administrador de parceiros do MPN

O relatório de Microsoft Learn fornece informações sobre os aprendizes em sua empresa, incluindo os módulos que eles concluíram e os caminhos de aprendizado em que estão. O relatório exibe o status de cada aprendiz individual. O administrador global e o administrador do MPN para sua empresa podem exibir os dados.

## <a name="how-to-read-the-report"></a>Como ler o relatório

### <a name="summary-charts"></a>Gráficos de resumo

Esses gráficos resumem a contagem e as tendências cumulativas mensais para indivíduos treinados, preenchimentos de módulo e roteiros de aprendizagem.


**Contagem de indivíduos treinados**: uma contagem de todos os aprendizes distintos que concluíram pelo menos um módulo durante o intervalo de datas selecionado 

A **pessoa treinada Trend mini Chart**: Contagem cumulativa mês a mês dos aprendizes ativos 

**Contagem de preenchimentos de módulo**: contagem de preenchimentos de módulo pelos aprendizes na empresa do parceiro durante o intervalo de datas selecionado.
Por exemplo, se "módulo 1" for concluído por 15 indivíduos e o "módulo 2" tiver sido concluído pelos mesmos 15 indivíduos, a contagem de preenchimentos de módulo será 30. A data de conclusão do módulo deve estar no intervalo de datas selecionado.

**Trimódulo de tendências de preenchimentos de módulos**: mês acima do mês Contagem cumulativa das conclusões do módulo 

**Contagem de conclusões de roteiros de aprendizagem**: contagem de conclusões de caminho de aprendizagem pelos aprendizes na empresa do parceiro durante o intervalo de datas selecionado.
Por exemplo, se o roteiro de aprendizagem "caminho 1" for concluído por 20 indivíduos e o roteiro de aprendizagem "caminho 2" tiver sido concluído pelos mesmos 20 indivíduos, a contagem de conclusão do roteiro de aprendizagem será de 40. A data de conclusão do roteiro de aprendizagem deve estar dentro do intervalo de datas selecionado.

A **tendência de conclusão do roteiro de aprendizagem**é o gráfico de tendências: mês acima do mês Contagem cumulativa das conclusões do roteiro de aprendizagem 

### <a name="trained-individuals-monthly-trend"></a>Tendência mensal de pessoas treinadas

Esses dados são a tendência dos usuários de sua empresa que concluíram um módulo pela primeira vez nesse mês. 

**Eixo X** é mês para o filtro de tempo selecionado. 

O **eixo Y** é a contagem de aprendizes ativos que se registraram (conclusão inicial de um módulo) durante esse mês. Isso não é cumulativo.

### <a name="module-completions-monthly-trend"></a>Tendência mensal de preenchimentos de módulo

Esses dados são a tendência dos módulos concluídos por todos os usuários da sua empresa durante esse mês. (não cumulativo) 

**Eixo X** é mês para o filtro de tempo selecionado. 

O **eixo Y** é a contagem das conclusões do módulo durante esse mês. Isso não é cumulativo.

### <a name="learning-path-completions-monthly-trend"></a>Tendência mensal de conclusões do roteiro de aprendizagem

Esses dados são a tendência de caminhos de aprendizado concluídos pelos usuários da sua empresa durante esse mês. (não cumulativo) 

**Eixo X** é mês para o filtro de tempo selecionado. 

O **eixo Y** é a contagem de preenchimentos de módulo nesse mês. Isso não é cumulativo.

### <a name="learning-path-completion-tabs"></a>Guias de conclusão do roteiro de aprendizagem 

**Guia módulo**

Esta guia inclui a divisão dos módulos concluídos em sua empresa pelos 5 principais nomes de módulo; o produto ao qual o módulo está associado; e a função de usuário pertinente ao módulo.  

- Gráfico de rosca de preenchimentos de módulo: divisão das conclusões do módulo (contagem exibida na seção de resumo) pelos nomes de módulo.

O número exibido no centro do gráfico é o total de módulos concluídos

- Conclusões por função: divisão das conclusões do módulo pela função do módulo. Se um módulo estiver associado a várias funções, cada uma das funções será adicionada à contagem de preenchimentos de módulo.

O número exibido no centro do gráfico é o número de funções distintas para as conclusões do módulo. 

- Conclusões por produto: divisão das conclusões do módulo pelo produto ao qual o módulo está mapeado. Se um módulo estiver associado a vários produtos, cada um dos produtos será adicionado à contagem de preenchimentos de módulo.    

O número exibido no centro do gráfico é o número de produtos distintos para as conclusões do módulo.  

**Guia caminho de aprendizagem**   

Esta guia inclui uma análise dos caminhos de aprendizado concluídos em sua empresa pelos 5 principais nomes de módulo; o produto ao qual o roteiro de aprendizagem está mapeado; e a função pertinente a este roteiro de aprendizagem.  

- Gráfico de rosca de conclusões de roteiros de aprendizado: análise das conclusões do roteiro de aprendizagem (contagem exibida na seção Resumo) por nome.

- Conclusões por função *: a divisão dos caminhos de aprendizado é concluída pela função. Se um módulo estiver associado a várias funções, cada uma das funções será adicionada à contagem de preenchimentos de módulo.

- Conclusões por produto: a divisão dos caminhos de aprendizado é concluída pelo produto ao qual o roteiro de aprendizagem está mapeado. Se um módulo estiver associado a vários produtos, cada um dos produtos será adicionado à contagem de preenchimentos de módulo.

### <a name="completions-by-learning-individuals"></a>Conclusões por indivíduos de aprendizagem

Isso lista os usuários treinados em sua empresa e os detalhes de seus módulos e roteiros de aprendizado concluídos.

Microsoft Learn identifica os aprendizes com uma ID de objeto de usuário. Na **guia módulos**, todos os aprendizes são classificados pelos módulos concluídos. Eles são exibidos com seus Microsoft Learn nome de usuário, ID de objeto e contagem de módulos. Você pode pesquisar usando o nome de usuário. 

Na **guia caminhos de aprendizado** , todos os aprendizes classificados por caminhos de aprendizado concluídos são exibidos com o nome de exibição do aprendiz, a ID do objeto e a contagem de módulos.

Para obter detalhes de um aprendiz usando a ID de objeto de usuário: 

1. Entre no [Gerenciador de gráficos](https://developer.microsoft.com/graph/graph-explorer ). (Você deve ser o administrador global do locatário do Azure AD da sua empresa.)

2. Copie a ID de objeto de usuário para a [área realçada](https://graph.microsoft.com/v1.0/users/a9633ad7-c8dc-4587-b119-0bc286b0711f) no Gerenciador de gráficos. 

## <a name="faq"></a>Perguntas frequentes

1. Não consigo ver os detalhes de aprendizado da minha empresa.

Esse relatório está disponível para parceiros que têm uma conta no Partner Center. Se ainda estiver no centro de associação de parceiro, você não poderá ver esse relatório.

2.  Quem em nossa empresa pode exibir este relatório? 

O administrador global e o administrador do MPN podem exibir o relatório.

3. Como garantir que todos os usuários associem suas contas de Microsoft Learn à sua conta do Partner Center?

Depois que o administrador global adicionar um novo usuário, esse usuário precisará acessar o **meu perfil** para associar sua conta de Microsoft learn.

- Selecione o ícone de **sua conta** no canto direito do painel e, em seguida, selecione **meu perfil**. 

-  Em **seu aprendizado** , um usuário poderá associar sua conta do Microsoft Learning e conectar seu conta Microsoft à University Partner.

3. Posso ver todos os usuários da empresa que entram no Microsoft Learn com uma conta MSA neste relatório?

Atualmente, a melhor maneira de fazer isso é adicionar esses usuários ao seu locatário do Azure AD e adicioná-los ao Partner Center para que eles possam associar sua conta de Microsoft Learn por meio do **meu perfil** no Partner Center. 

Para os usuários que usam apenas sua conta MSA para treinamento, em um futuro próximo, a equipe de Microsoft Learn permitirá que eles associem seus emails de trabalho ao seu perfil de Microsoft Learn. 

## <a name="next-steps"></a>Próximas etapas

Para obter mais relatórios, consulte os [insights do Partner Center](partner-center-insights.md).

>[!NOTE] 
> Você pode baixar os dados brutos, capacitando esse relatório na seção baixar relatórios no painel do insights. [Saiba mais](pci-download-reports.md) 