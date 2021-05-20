---
title: Partner Center insights Microsoft Learn análise
ms.topic: article
ms.date: 08/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Acompanhe os alunos em sua empresa aproveitando dados sobre treinamento individual, módulos concluídos, caminhos de aprendizagem concluídos e muito mais.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 132583352e1697a2f9dfa624eb9532692be6d734
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152623"
---
# <a name="the-microsoft-learn-analytics-report-shows-the-status-of-learners-in-your-company"></a>O relatório de análise do Microsoft Learn mostra o status dos estudantes de sua empresa

**Funções apropriadas:** administrador global | Administrador de parceiro do MPN

O Microsoft Learn relatório fornece informações sobre os alunos em sua empresa, incluindo os módulos que eles concluíram e os caminhos de aprendizagem em que estão. O relatório exibe o status de cada aluno individual. O administrador global e o administrador do MPN para sua empresa podem exibir os dados.

## <a name="how-to-read-the-report"></a>Como ler o relatório

### <a name="summary-charts"></a>Gráficos de resumo

Esses gráficos resumem a contagem e as tendências cumulativas mensais para indivíduos treinados, preenchimentos de módulo e caminhos de aprendizagem.


**Contagem de indivíduos treinados:** uma contagem de todos os alunos distintos que concluíram pelo menos um módulo durante o intervalo de datas selecionado 

**Mini gráfico de tendência de indivíduos treinados:** contagem cumulativa de mês a mês dos alunos ativos 

**Contagem de preenchimentos de** módulo: contagem de preenchimentos de módulo pelos alunos na empresa do parceiro durante o intervalo de datas selecionado.
Por exemplo, se "Módulo 1" for concluído por 15 indivíduos e o "Módulo 2" tiver sido concluído pelos mesmos 15 indivíduos, a contagem de preenchimentos do módulo será de 30. A data de conclusão do módulo deve estar no intervalo de datas selecionado.

**Mini gráfico de tendência de preenchimentos de módulo:** contagem cumulativa de mês a mês das conclusão do módulo 

**Contagem de conclusão do caminho de** aprendizagem: contagem de preenchimentos do caminho de aprendizagem pelos alunos na empresa do parceiro durante o intervalo de datas selecionado.
Por exemplo, se o Caminho de Aprendizagem "Caminho 1" for concluído por 20 indivíduos e o Caminho de Aprendizagem "caminho 2" tiver sido concluído pelos mesmos 20 indivíduos, a contagem de conclusão do Caminho de Aprendizagem será de 40. A data de conclusão do caminho de aprendizagem deve estar dentro do intervalo de datas selecionado.

**Mini gráfico de tendência de conclusão do caminho de aprendizagem:** contagem cumulativa de mês a mês das conclusão do caminho de aprendizagem 

### <a name="trained-individuals-monthly-trend"></a>Tendência mensal de indivíduos treinados

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

Essa guia inclui a divisão dos módulos concluídos em sua empresa pelos cinco principais nomes de módulo; o produto ao qual o módulo está associado; e a função de usuário pertinente ao módulo.  

- Gráfico de rosca de preenchimentos de módulo: divisão das conclusões do módulo (contagem exibida na seção de resumo) pelos nomes de módulo.

O número exibido no centro do gráfico é o total de módulos concluídos

- Preenchimentos por função: detalhamento das conclusão do módulo pela função do módulo. Se um módulo estiver associado a várias funções, cada uma das funções será adicionada à contagem de preenchimentos do módulo.

O número exibido no centro do gráfico é o número de funções distintas para as conclusão do módulo. 

- Preenchimentos por produto: detalhamento das conclusão do módulo pelo produto para o que o módulo é mapeado. Se um módulo estiver associado a vários produtos, cada um dos produtos será adicionado à contagem de preenchimentos do módulo.    

O número exibido no centro do gráfico é o número de produtos distintos para as conclusão do módulo.  

**Guia Caminho de aprendizagem**   

Essa guia inclui um detalhamento dos caminhos de aprendizagem concluídos em sua empresa pelos cinco principais nomes de módulo; o produto para o quais o caminho de aprendizagem é mapeado; e a função pertinente a esse caminho de aprendizagem.  

- Gráfico de rosca de preenchimentos de caminhos de aprendizagem: detalhamento das conclusão do caminho de aprendizagem (contagem exibida na seção de resumo) por nome.

- Preenchimentos por função*: detalhamento dos caminhos de aprendizagem concluídos pela função. Se um módulo estiver associado a várias funções, cada uma das funções será adicionada à contagem de preenchimentos do módulo.

- Preenchimentos por produto: detalhamento dos caminhos de aprendizagem concluídos pelo Produto para o qual o caminho de aprendizagem é mapeado. Se um módulo estiver associado a vários produtos, cada um dos produtos será adicionado à contagem de preenchimentos do módulo.

### <a name="completions-by-learning-individuals"></a>Preenchimentos por indivíduos de aprendizado

Isso lista os usuários treinados em sua empresa e os detalhes de seus módulos concluídos e caminhos de aprendizagem.

Microsoft Learn identifica os alunos com uma ID de Objeto de Usuário. Na guia **Módulos ,** todos os alunos são classificação pelos módulos concluídos. Eles são exibidos com sua Microsoft Learn nome de usuário, ID de objeto e contagem de módulos. Você pode pesquisar usando o nome de usuário. 

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

Atualmente, a melhor maneira de fazer isso é adicionar esses usuários ao seu locatário do Azure AD e, em seguida, adicioná-los ao Partner Center para que eles possam associar sua conta de Microsoft Learn por meio do **meu perfil** no Partner Center. 

Para os usuários que usam apenas sua conta MSA para treinamento, em um futuro próximo, a equipe de Microsoft Learn permitirá que eles associem seus emails de trabalho ao seu perfil de Microsoft Learn. 

## <a name="next-steps"></a>Próximas etapas

Para obter mais relatórios, consulte os [insights do Partner Center](partner-center-insights.md).

>[!NOTE] 
> Você pode baixar os dados brutos, capacitando esse relatório na seção baixar relatórios no painel do insights. [Saiba mais](pci-download-reports.md) 