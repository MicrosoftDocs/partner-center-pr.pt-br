---
title: Análise do Microsoft Learn | Partner Center
ms.topic: article
ms.date: 07/05/2019
description: Obter informações sobre como compreender suas análises de aprendizado
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: e59be88d1e599bbd9d26827ec6a588a23a2f77a4
ms.sourcegitcommit: 1388ca15f359b7cb0a7856974f605f14523a73fb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2019
ms.locfileid: "67674249"
---
# <a name="microsoft-learn-analytics-report"></a>Relatório de análise do Microsoft Learn

O relatório do Microsoft Learn fornece informações sobre os aprendizes em sua empresa, incluindo os módulos a que serem concluídos e os caminhos de aprendizado estão na. O relatório exibe o status de cada aprendiz individual. O administrador global e o administrador do MPN para sua empresa podem exibir os dados.

## <a name="how-to-read-the-report"></a>Como ler o relatório

### <a name="summary-charts"></a>Gráficos de resumo

Esses gráficos resumem contagem e mensalmente tendências cumulativas para indivíduos treinados, conclusões de módulo e planos de aprendizado.


**Treinado indivíduos contagem**: Uma contagem de todos os aprendizes distintos que concluíram a pelo menos um módulo durante o intervalo de datas selecionado 

**Mini gráfico de tendência de indivíduos treinados**: Mês a contagem cumulativa de mês dos aprendizes Active Directory 

**Contagem de conclusões de módulo**: Preenchimentos de contagem do módulo pelos aprendizes de empresa do parceiro durante o intervalo de datas selecionado.
Por exemplo, se o "módulo de 1" é concluído por 15 pessoas e o "módulo 2" foi concluído pelas mesmas 15 pessoas, a contagem de conclusões de módulo será 30. A data de conclusão do módulo deve estar no intervalo de datas selecionado.

**Mini gráfico de tendência de conclusões de módulo**: Mês a contagem cumulativa de mês das conclusões de módulo 

**Contagem de conclusões de caminho de aprendizado**: Preenchimentos de caminho de contagem de aprendizado pelos aprendizes de empresa do parceiro durante o intervalo de datas selecionado.
Por exemplo, se o roteiro de aprendizagem do "caminho de 1" é concluído por 20 indivíduos e o roteiro de aprendizagem "caminho 2" foi concluído pelas mesmas 20 pessoas, a contagem de preenchimento do plano de aprendizado será 40. A data de conclusão de caminho de aprendizado deve estar dentro do intervalo de datas selecionado.

**Mini gráfico de tendência de conclusões de caminho de aprendizado**: Mês a contagem cumulativa de mês de aprendizado preenchimentos de caminho 

### <a name="trained-individuals-monthly-trend"></a>Tendência de pessoas físicas treinado mensal

Esses dados são a tendência de usuários da sua empresa que concluíram um módulo pela primeira vez no mês. 

**Eixo x** é mês para o filtro de tempo selecionado. 

**Eixo y** é contagem de aprendizes Active Directory que se registraram (pela primeira vez o término de um módulo) durante esse mês. Isso não é cumulativo.

### <a name="module-completions-monthly-trend"></a>Tendência mensal de conclusões de módulo

Esses dados são a tendência dos módulos concluídos pelos usuários de todos os da sua empresa durante esse mês. (não cumulativo) 

**Eixo x** é mês para o filtro de tempo selecionado. 

**Eixo y** é a contagem das conclusões de módulo durante esse mês. Isso não é cumulativo.

### <a name="learning-path-completions-monthly-trend"></a>Tendência mensal de conclusões de caminho de aprendizado

Esses dados são a tendência de roteiros concluídos pelos usuários de sua empresa durante esse mês de aprendizagem. (não cumulativo) 

**Eixo x** é mês para o filtro de tempo selecionado. 

**Eixo y** é a contagem de conclusões de módulo no mês. Isso não é cumulativo.

### <a name="learning-path-completion-tabs"></a>Guias de preenchimento do caminho de aprendizado 

**Guia de módulo**

Este guia inclui análise de módulos concluída em sua empresa por nomes de módulo 5 principais; o produto ao qual o módulo está associado; e a função de usuário pertinente para o módulo.  

- Gráfico de rosca de conclusões de módulo: divisão das conclusões de módulo (exibida na seção de resumo de contagem), os nomes do módulo.

Número exibido no centro do gráfico é os módulos total concluídos

- As conclusões por função: divisão das conclusões de módulo da função do módulo. Se um módulo estiver associado a várias funções, cada uma das funções é adicionada à contagem de conclusões de módulo.

Número exibido no centro do gráfico é o número de funções distintas para as conclusões de módulo. 

- As conclusões por produto: divisão das conclusões de módulo pelo produto o módulo é mapeado para. Se um módulo estiver associado a vários produtos, cada um dos produtos é adicionada à contagem de conclusões de módulo.    

Número exibido no centro do gráfico é o número de produtos distintos para as conclusões de módulo.  

**Guia de caminho de aprendizado**   

Este guia inclui uma divisão dos caminhos concluídos em sua empresa por nomes de módulo 5 principais; de aprendizado o produto que o roteiro de aprendizagem é mapeado para; e a função pertinente para este roteiro de aprendizagem.  

- Gráfico de rosca de preenchimentos de caminhos de aprendizado: divisão das conclusões de caminho de aprendizado (exibida na seção de resumo de contagem) por nome.

- As conclusões por função *: divisão da learning preenchimentos de caminhos da função. Se um módulo estiver associado a várias funções, cada uma das funções é adicionada à contagem de conclusões de módulo.

- As conclusões por produto: divisão da learning preenchimentos de caminhos pelo produto ao qual o plano de aprendizado é mapeado. Se um módulo estiver associado a vários produtos, cada um dos produtos é adicionada à contagem de conclusões de módulo.

### <a name="completions-by-learning-individuals"></a>Conclusões por indivíduos de aprendizagem

Isso lista os usuários treinados em sua empresa e os detalhes de seus módulos concluídos e planos de aprendizado.

Microsoft Learn identifica aprendizes com uma ID de objeto de usuário. Sob o **guia de módulos**, todos os aprendizes são classificados pelos módulos concluídos. Eles são exibidos com seu nome de usuário Microsoft Learn, ID de objeto e contagem de módulos. Você pode pesquisar usando nome de usuário. 

Sob o **guia de caminhos de aprendizado** todos os aprendizes classificados por concluído, de caminhos de aprendizado são exibidos com o nome de exibição de aprendiz, a ID de objeto e a contagem de módulo.

Para obter detalhes de um aprendiz usando a ID de objeto de usuário: 

1. Entrar no [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer ). (Você deve ser o administrador global do locatário do Azure AD da sua empresa.)

2. Copie a ID de objeto de usuário para o [área realçada](https://graph.microsoft.com/v1.0/users/a9633ad7-c8dc-4587-b119-0bc286b0711f) no Explorador do Graph. 

## <a name="faq"></a>Perguntas frequentes

1. Não consigo ver os detalhes de aprendizado da minha empresa.

Esse relatório está disponível para os parceiros que tenham uma conta no Partner Center. Se você ainda estiver no Partner Membership Center, você não poderá ver esse relatório.

2.  Quem na nossa empresa pode exibir esse relatório? 

O administrador do MPN e o administrador global podem exibir o relatório.

3. Como posso ter certeza de todos os nossos usuários associar suas contas Microsoft Learn à respectiva conta do Partner Center?

Depois que o administrador global adiciona um novo usuário, que o usuário deve ir para seus **meu perfil** para associar sua conta da Microsoft Learn.

- Selecione o **sua conta** ícone no canto direito do dashboard e, em seguida, selecione **meu perfil**. 

-  Sob **seu aprendizado** um usuário poderá associar sua conta do Microsoft Learning e se conectar a sua conta da Microsoft a Universidade do parceiro.

3. Posso ver todos os usuários da empresa que entrar no Microsoft Learn com uma conta MSA nesse relatório?

Atualmente, a melhor maneira de fazer isso é adicionar esses usuários ao AD do Azure do locatário e adicioná-los ao Partner Center, para que eles podem associar sua conta da Microsoft Learn por meio **meu perfil** no Partner Center. 

Para usuários que só usam suas contas MSA para treinamento em um futuro próximo, a equipe do Microsoft Learn permitirá que a capacidade para que eles possam associar seus emails de trabalho para seu perfil do Microsoft Learn. 

