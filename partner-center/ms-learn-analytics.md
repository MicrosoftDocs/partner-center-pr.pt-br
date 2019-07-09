---
title: Análise do Microsoft Learn | Partner Center
ms.topic: article
ms.date: 07/05/2019
description: Obter informações sobre como compreender suas análises de aprendizado
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 09d4ca14c1b407e9010ab26bccaf612f9caad732
ms.sourcegitcommit: bd83621eb29fafbda341ad41814a9ae5c1e78b00
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2019
ms.locfileid: "67622524"
---
# <a name="microsoft-learn-analytics-report"></a>Relatório de análise do Microsoft Learn

O relatório do Microsoft Learn fornece informações sobre os aprendizes em sua empresa, incluindo os módulos a que serem concluídos e os caminhos de aprendizado estão na. O relatório exibe o status de cada aprendiz individual. O administrador global e o administrador do MPN para sua empresa podem exibir os dados.

## <a name="how-to-read-the-report"></a>Como ler o relatório

### <a name="summary-charts"></a>Gráficos de resumo

**Treinado indivíduos contagem**: Uma contagem de todos os aprendizes distintos que concluíram a pelo menos um módulo durante o intervalo de datas selecionado 

**Mini gráfico de tendência de indivíduos treinados**: Mês a contagem cumulativa de mês dos aprendizes Active Directory 

**Contagem de conclusões de módulo**: Preenchimentos de contagem do módulo pelos aprendizes de empresa do parceiro durante o intervalo de datas selecionado.
Por exemplo, se o "módulo de 1" é concluído por 15 pessoas e o "módulo 2" foi concluído pelas mesmas 15 pessoas, a contagem de conclusões de módulo será 30. A data de conclusão do módulo deve estar no intervalo de datas selecionado.

**Mini gráfico de tendência de conclusões de módulo**: Mês a contagem cumulativa de mês das conclusões de módulo 

**Contagem de conclusões de caminho de aprendizado**: Preenchimentos de caminho de contagem de aprendizado pelos aprendizes de empresa do parceiro durante o intervalo de datas selecionado.
Por exemplo, se o roteiro de aprendizagem do "caminho de 1" é concluído por 20 indivíduos e o roteiro de aprendizagem "caminho 2" foi concluído pelas mesmas 20 pessoas, a contagem de preenchimento do plano de aprendizado será 40. A data de conclusão de caminho de aprendizado deve estar dentro do intervalo de datas selecionado.

**Mini gráfico de tendência de conclusões de caminho de aprendizado**: Mês a contagem cumulativa de mês de aprendizado preenchimentos de caminho 

### <a name="trained-individuals-monthly-trend"></a>Tendência de pessoas físicas treinado mensal

**Eixo x** é mês para o filtro de tempo selecionado. 

**Eixo y** é contagem de aprendizes Active Directory que se registraram (pela primeira vez o término de um módulo) durante esse mês. Isso não é cumulativo.

### <a name="module-completions-monthly-trend"></a>Tendência mensal de conclusões de módulo

**Eixo x** é mês para o filtro de tempo selecionado. 

**Eixo y** é a contagem das conclusões de módulo durante esse mês. Isso não é cumulativo.

### <a name="learning-path-completions-monthly-trend"></a>Tendência mensal de conclusões de caminho de aprendizado

**Eixo x** é mês para o filtro de tempo selecionado. 

**Eixo y** é a contagem de conclusões de módulo no mês. Isso não é cumulativo.

### <a name="learning-path-completion-tabs"></a>Guias de preenchimento do caminho de aprendizado 

- Guia de módulo

**Gráfico de rosca de conclusões de módulo**: divisão das conclusões de módulo (exibida na seção de resumo de contagem), os nomes do módulo.

Número exibido no centro do gráfico é os módulos total concluídos

**As conclusões por função**: divisão das conclusões de módulo da função do módulo. Se um módulo estiver associado a várias funções, cada uma das funções é adicionada à contagem de conclusões de módulo.

Número exibido no centro do gráfico de rosca é o número de funções distintas para as conclusões de módulo. 

**As conclusões por produto**: divisão das conclusões de módulo pelo produto o módulo é mapeado para. Se um módulo estiver associado a vários produtos, cada um dos produtos é adicionada à contagem de conclusões de módulo.    

Número exibido no meio do gráfico de rosca é o número de produtos distintos para as conclusões de módulo.  

- Guia de caminho de aprendizado    

**Gráfico de rosca de preenchimentos de caminhos de aprendizado**: divisão das conclusões de caminhos de aprendizado (exibida na seção de resumo de contagem) por nome.

**As conclusões por função**: divisão da learning preenchimentos de caminhos da função. Se um módulo estiver associado a várias funções, cada uma das funções é adicionada à contagem de conclusões de módulo.

**As conclusões por produto**: divisão da learning preenchimentos de caminhos pelo produto ao qual o plano de aprendizado é mapeado. Se um módulo estiver associado a vários produtos, cada um dos produtos é adicionada à contagem de conclusões de módulo.

### <a name="completions-by-learning-individuals"></a>Conclusões por indivíduos de aprendizagem

Microsoft Learn identifica aprendizes com uma ID de objeto de usuário. Sob o **guia de módulos**, todos os aprendizes são classificados pelos módulos concluídos. Eles são exibidos com seu nome de usuário Microsoft Learn, ID de objeto e contagem de módulos. Você pode pesquisar usando nome de usuário.

Para obter detalhes de um aprendiz usando a ID de objeto de usuário: 

1. Entrar no [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer ). (Você deve ser o administrador global do locatário do Azure AD da sua empresa.)

2. Copie a ID de objeto de usuário para o [área realçada](https://graph.microsoft.com/v1.0/users/a9633ad7-c8dc-4587-b119-0bc286b0711f) no Explorador do Graph. 

