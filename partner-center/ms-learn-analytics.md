---
title: Partner Center Insights Microsoft Learn análise
ms.topic: article
ms.date: 08/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Acompanhe os alunos em sua empresa aproveitando dados sobre treinamento individual, módulos concluídos, caminhos de aprendizagem concluídos e muito mais.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d9f9ce631fe667030638e1a9167809e3dae69830
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114373870"
---
# <a name="use-microsoft-learn-analytics-reports"></a>Usar Microsoft Learn de análise

**Funções apropriadas:** administrador global | Administrador de parceiro do MPN

O [Microsoft Learn](/learn/) relatório fornece informações sobre os alunos em sua empresa, incluindo os módulos que eles concluíram e os caminhos de aprendizagem em que estão. O relatório exibe o status de cada aluno individual. Administradores globais e administradores do MPN para uma empresa podem exibir os dados.

## <a name="how-to-read-the-report"></a>Como ler o relatório

### <a name="summary-charts"></a>Gráficos de resumo

Esses gráficos resumem a contagem e as tendências cumulativas mensais para indivíduos treinados, preenchimentos de módulo e caminhos de aprendizagem.

**Contagem de indivíduos treinados:** uma contagem de todos os alunos distintos que concluíram pelo menos um módulo durante o intervalo de datas selecionado 

**Mini gráfico de tendência de indivíduos treinados:** contagem cumulativa de mês a mês dos alunos ativos 

**Contagem de preenchimentos de** módulo: contagem de preenchimentos de módulo pelos alunos na empresa do parceiro durante o intervalo de datas selecionado.
Por exemplo, se "Módulo 1" for concluído por 15 indivíduos e o "Módulo 2" tiver sido concluído pelos mesmos 15 indivíduos, a contagem de preenchimentos do módulo será de 30. A data de conclusão do módulo deve estar no intervalo de datas selecionado.

**Mini gráfico de tendência de preenchimentos de módulo:** contagem cumulativa de mês a mês das conclusão do módulo 

**Learning de** conclusão de caminho: contagem de Learning de caminho pelos alunos na empresa do parceiro durante o intervalo de datas selecionado.
Por exemplo, se Learning caminho "Caminho 1" for concluído por 20 indivíduos e o Caminho do Learning "caminho 2" tiver sido concluído pelos mesmos 20 indivíduos, a contagem de conclusão do caminho Learning será de 40. A Learning de conclusão do caminho deve estar dentro do intervalo de datas selecionado.

Learning mini gráfico de tendência **de preenchimentos de** caminho: contagem cumulativa de mês a mês das conclusão do caminho de aprendizagem 

### <a name="trained-individuals-monthly-trend"></a>Tendência mensal de indivíduos treinados

Esses dados são a tendência dos usuários da sua empresa que concluíram um módulo pela primeira vez nesse mês. 

**Eixo X é** o mês do filtro de tempo selecionado. 

**Eixo Y é** a contagem de alunos ativos que registraram (conclusão pela primeira vez de um módulo) durante esse mês. Isso não é cumulativo.

### <a name="module-completions-monthly-trend"></a>Tendência mensal de preenchimentos de módulo

Esses dados são a tendência de módulos concluídos por todos os usuários da sua empresa durante esse mês. (não cumulativo) 

**Eixo X é** o mês do filtro de tempo selecionado. 

**Eixo Y é** a contagem das conclusão do módulo durante esse mês. Isso não é cumulativo.

### <a name="learning-path-completions-monthly-trend"></a>Learning tendência mensal de preenchimentos de caminho

Esses dados são a tendência de caminhos de aprendizagem concluídos pelos usuários da sua empresa durante esse mês. (não cumulativo) 

**Eixo X é** o mês do filtro de tempo selecionado. 

**Eixo Y é** a contagem de preenchimentos de módulo nesse mês. Isso não é cumulativo.

### <a name="learning-path-completion-tabs"></a>Learning de conclusão do caminho

#### <a name="module-tab"></a>Guia Módulo

Essa guia inclui o detalhamento dos módulos concluídos em sua empresa pelos cinco principais nomes de módulo; o produto ao qual o módulo está associado; e a função de usuário pertinente ao módulo.  

- Gráfico de rosca de preenchimentos do módulo: detalhamento das conclusão do módulo (contagem exibida na seção de resumo) pelos nomes do módulo.

O número exibido no centro do gráfico é o total de módulos concluídos

- Preenchimentos por função: detalhamento das conclusão do módulo pela função do módulo. Se um módulo estiver associado a várias funções, cada uma das funções será adicionada à contagem de preenchimentos do módulo.

O número exibido no centro do gráfico é o número de funções distintas para as conclusão do módulo. 

- Preenchimentos por produto: detalhamento das conclusão do módulo pelo produto para o que o módulo é mapeado. Se um módulo estiver associado a vários produtos, cada um dos produtos será adicionado à contagem de preenchimentos do módulo.    

O número exibido no centro do gráfico é o número de produtos distintos para as conclusão do módulo.  

#### <a name="learning-path-tab"></a>Learning de caminho

Essa guia inclui um detalhamento dos caminhos de aprendizagem concluídos em sua empresa pelos cinco principais nomes de módulo; o produto para o quais o caminho de aprendizagem é mapeado; e a função pertinente a esse caminho de aprendizagem.  

- Learning gráfico de rosca de preenchimentos de caminhos: detalhamento das Learning de caminho (contagem exibida na seção de resumo) por nome.

- Preenchimentos por função: detalhamento dos caminhos de aprendizagem concluídos pela função. Se um módulo estiver associado a várias funções, cada uma das funções será adicionada à contagem de preenchimentos do módulo.

- Preenchimentos por produto: detalhamento dos caminhos de aprendizagem concluídos pelo Produto para o qual o caminho de aprendizagem é mapeado. Se um módulo estiver associado a vários produtos, cada um dos produtos será adicionado à contagem de preenchimentos do módulo.

### <a name="completions-by-learning-individuals"></a>Preenchimentos por indivíduos de aprendizado

Isso lista os usuários treinados em sua empresa e os detalhes de seus módulos concluídos e caminhos de aprendizagem.

Microsoft Learn identifica os alunos com uma ID de Objeto de Usuário. Na guia **Módulos ,** todos os alunos são classificação pelos módulos concluídos. Eles são exibidos com sua Microsoft Learn nome de usuário, ID de objeto e contagem de módulos. Você pode pesquisar usando o nome de usuário. 

Na guia **Learning todos** os alunos classificaram por caminhos de aprendizagem concluídos, são exibidos com o nome de exibição do aluno, a ID do objeto e a contagem de módulos.

Para obter os detalhes de um aluno usando a ID de Objeto de Usuário: 

1. Entre no [Graph Explorer.](https://developer.microsoft.com/graph/graph-explorer ) (Você deve ser o administrador global do locatário do Azure AD da sua empresa.)

2. Copie a ID do objeto de usuário para [a área realçada](https://graph.microsoft.com/v1.0/users/a9633ad7-c8dc-4587-b119-0bc286b0711f) no Graph Explorer. 

## <a name="frequently-asked-questions-faq"></a>Perguntas frequentes (FAQ)

1. Não consigo ver os detalhes do Learn da minha empresa.

   Este relatório está disponível para parceiros que têm uma conta no Partner Center. Se você ainda estiver Partner Membership Center, não poderá ver esse relatório.

2. Who minha empresa pode exibir esse relatório? 

   O administrador global e o administrador do MPN podem exibir o relatório.

3. Como posso garantir que todos os nossos usuários associem suas contas Microsoft Learn dados à conta Partner Center usuário?

   *Depois que* o administrador global adiciona um novo usuário , esse usuário deve acessar o [Microsoft Learn](/learn/) para vincular sua conta corporativa do AD (Azure Active Directory) com sua conta do Learn. Isso garante que a Insights Learning guia mostrará os cursos e as habilidades certos.
   
   O usuário precisa:
   
   1. Entre no [Microsoft Learn](/learn/).
   2. Selecione a imagem do perfil e, em **seguida, selecione Meu perfil**.
   3. Selecione **Configurações**.
   4. Em **Gerenciamento de conta,** adicione sua conta de trabalho em **Contas vinculadas.**

4. Posso ver todos os usuários da empresa que entraram no Microsoft Learn com uma conta da MSA neste relatório?

   Atualmente, a melhor maneira de fazer isso é adicionar esses usuários ao seu locatário do Azure AD e, em seguida, adicioná-los ao Partner Center para que eles possam associar sua conta do Microsoft Learn por meio do **Meu perfil** no Partner Center. 

   Para usuários que usam apenas sua conta MSA para treinamento, em um futuro próximo, a equipe do Microsoft Learn permitirá que eles associem seu email de trabalho ao seu perfil Microsoft Learn trabalho. 

## <a name="next-steps"></a>Próximas etapas

Para obter mais relatórios, [consulte Partner Center Insights](partner-center-insights.md).

>[!NOTE] 
> Você pode baixar os dados brutos que agem neste relatório na seção Baixar Relatórios no painel Insights dados. [Saiba mais](insights-download-reports.md) 
