---
title: Análises do Partner Center – relatórios de CloudAscent propensation
description: Saiba mais sobre os relatórios de CloudAscent propensation no Partner Center. Inclui informações sobre as propensações de um cliente para comprar produtos da Microsoft.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 04/27/2021
ms.openlocfilehash: 430aea81964d1b75514b6e1377bd2ba1af41b538
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110153031"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a>Relatórios de CloudAscent propensation disponíveis no painel do Partner Center

**Funções apropriadas**: Visualizador de relatórios executivos | Visualizador de relatórios

O painel do Partner Center fornece dados de propensação baixáveis do programa CloudAscent. Os dados mostram a probabilidade dos clientes de comprar produtos da Microsoft.  Este artigo descreve a divisão desses dados, como usar a pontuação e o que isso significa.

## <a name="summary-definitions"></a>Definições de resumo

- **Clientes do SMC**– este é o número total de clientes nos downloads de propensação.  Os clientes são identificados pelo parceiro do registro.
- **Contratos de expiração**– dentro do ano fiscal atual, estamos fornecendo o número de contratos expirando.
- **Abrir receita de expiração**– a receita associada aos contratos expirados abertos.

:::image type="content" source="images/pci/cust-oppor-11.png" alt-text="Captura de tela do painel de Resumo de oportunidades de clientes.":::

## <a name="cloudascent-smb-segmentation"></a>Segmentação SMB do CloudAscent

O segmento SMB (Small to Medium Business) é dividido em três subsegmentos distintos.

1. A **parte superior não gerenciada** inclui os maiores clientes SMB com mais oportunidade para a Microsoft. Os principais clientes não gerenciados compartilham características semelhantes às contas gerenciadas, com grande número de funcionários, grandes orçamentos de ti e gastos e grandes quantidades de receitas potenciais para a Microsoft.

   Definimos Top não gerenciado de duas maneiras:

   - **Com base em principais usuários não gerenciados**– inclui contas com 300 ou mais funcionários. User-Based contas são ótimos destinos para compra pela primeira vez ou expansão de produtos de assinatura baseados no usuário, como Microsoft 365, Dynamics 365 ou Surface.
   - **Top Unmanaged Compute Based** – inclui contas com potencial do Azure maior que US$ 10 mil. Contas baseadas em computação incluem o Azure existente. contas com potencial futuro significativo e contas que ainda não compraram o Azure, mas têm potencial para o Azure maior que US$ 10 mil.

2. **O Medium Business** inclui clientes e contas potenciais existentes com 25 a 300 funcionários.

3. **O Small Business** inclui empresas com 10 a 25 funcionários.

4. **A Very Small Business** inclui empresas com 1 a 9 funcionários.

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="Cliente por tipo SMC.":::

**Os principais subsegmentos** de Negócios Médios e Não Planejados representam clientes ltV (alto valor de tempo de vida) para a Microsoft e parceiros da Microsoft.  Por isso, eles são as principais áreas de foco para impulsionar o crescimento nesse segmento. Nesses dois subsegmentos, estamos mais bem posicionados para adquirir o soquete com o Microsoft 365, monetizar ainda mais com aplicativos DE LOB (linha de negócios) do Azure/D365 e realizar um LTV alto para a Microsoft.

Hoje, temos duas áreas principais de oportunidade – 1. nosso cliente adiciona crescimento; 2. enquanto adquirimos bem os soquetes de nuvem à Microsoft 365, temos uma grande oportunidade no Dynamics 365 e no Azure.

A captura de tela a seguir representa os quatro Subseções SMB. A CloudAscent prioriza a criação de perfil, a pontuação e a modelagem de todas as principais contas de negócios médias e nãomanutivas.

:::image type="content" source="images/pci/cust-oppor-32.png" alt-text="Captura de tela de subseções SMB.":::

## <a name="cloudascent-machine-learning"></a>CloudAscent Machine Learning

O SMB usa a tecnologia de aprendizado de máquina para impulsionar as previsões de clientes de vendas e marketing nos principais segmentos de Negócios NãoManagedos e Médios. Como os sinais são coletados e transformados em recomendações de propensão?

- **Coleta de dados**: os rastreadores da Web examinam e coletam bilhões de sinais de clientes ao executar ping nos domínios da empresa e monitorar postagens em Blogs, Press Releases, fluxos sociais e fóruns técnicos.  Além dos sinais coletados, as informações de firmographics são coletadas de fontes internas e externas, como D&B, assinatura interna da Microsoft e dados transacionais.

- **Machine Learning**: os sinais são inseridos no modelo de aprendizado de máquina que gera um conjunto de dados estruturado de previsões de vendas e marketing para cada cliente por produto e cluster de nuvem.  Cada cliente é pontuado usando um modelo semelhante ao principal SMB da Microsoft que determina o ajuste do cliente e os algoritmos de aprendizado de máquina que integram o comportamento online do cliente, defina como intenção. A pontuação é mesclada em clusters que mostram a propensão de um cliente para comprar Microsoft Cloud produtos.

- **Otimização**: o sistema de Machine Learning otimiza os modelos consumindo os dados de transação mensalmente e os dados de assinatura trimestral.  Usando os dados de ganho/perda, o Machine Learning ajusta os algoritmos e valida que os modelos estão funcionando conforme o esperado, comparando as recomendações de cluster às oportunidades trabalhadas no MSX.

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="Captura de tela do aprendizado de máquina SMB.":::

## <a name="cloudascent-propensity"></a>CloudAscent propensaity

Como as recomendações de propensação são criadas?

Usando sinais coletados por meio de rastreadores da Web e dados fornecidos de várias fontes, consolidamos os dados de firmographics e os sinais de mídia social do cliente.  A pontuação usa esses sinais e dados em modelos de comparação para os modelos de ajuste e pontuação para a intenção.

1. Ajuste de conta do cliente

   - Pontos de dados internos e externos que definem firmographics.

   - Ajustar a pontuação usa um modelo semelhante ao nosso melhor SMB para comparar os clientes e ver se eles são um ajuste potencial para Microsoft Cloud produtos.

   - Ajustar Pontuação é atualizado trimestral

2. Intenção de conta de cliente

   - Os sinais relacionados à mídia social e ao comportamento online de um cliente definem a intenção.

   - A pontuação da intenção é sobressprovida de ajuste para definir os clusters.

   - A pontuação da intenção é atualizada mensalmente.

   :::image type="content" source="images/pci/cust-oppor-5.png" alt-text="Modelos de previsão do CloudAscent SMB.":::

3. Clustering

   Os Sinais para ajuste e intenção são consolidados em uma pontuação de clustering. CloudAscent tem quatro clusters:

      - Agir agora – clientes prontos para vendas
      - Avaliar – clientes prontos para marketing
      - Incentivar – impulsionar campanhas de reconhecimento
      - Instrua – instrua e monitore a intenção

   O clustering permite aos usuários direcionar clientes específicos para iniciativas de vendas e marketing com base em fatores de segmento, por exemplo: produto, área geográfica, setor e vertical.

   A **guia Modelo de propensão** nas Workbooks CloudAscent compartilha a propensão e a receita estimada de espaço em branco. Para definir o clustering de Ajuste e Intenção, vamos passar pelas seguintes etapas:

      1. Usando modelos de ML, primeiro calculamos a Pontuação de Ajuste do Cliente e a Pontuação da intenção em uma escala de 100.  As pontuações exatas variam de acordo com os modelos de ML.  Pontuações de exemplo abaixo:

         |**Classificação**|**Pontuação**|
         |---------|:---------|
         |Alto|75 - 100|
         |Médio|55 - 74|
         |Baixo|30 - 54|
         |Muito baixo|0 - 29|

      2. Usando a regra acima, classificamos as empresas para serem altas, médias, baixas e muito baixas entre os sinais de ajuste do cliente e de intenção.

      3. Nós plotamos os sinais de ajuste do cliente e de intenção em uma matriz 2D com cada interseção que representa a propensação. Por exemplo, alto ajuste + alta tentativa = a1, representando a mais alta propensação.

      4. Por fim, esses segmentos agrupam-se para formar clusters.  Por exemplo, a1, a2, a3, A4 forma o cluster Act Now.

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="Modelos de CloudAscent.":::

   Para esses clientes, é recomendável direcionar o Act agora e avaliar os clientes.

## <a name="cloudascent-products--models"></a>CloudAscent produtos & modelos

O gráfico a seguir fornece uma exibição de cada modelo de propensação dentro de CloudAscent:

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="Modelo de CloudAscent propensation.":::

Os modelos de espaço em branco são compostos de previsões para clientes da Microsoft existentes onde não têm um produto e/ou são clientes novos de cliente potencial.

Os modelos de venda cruzada usam dados de transação para prever o potencial de venda no Azure e Microsoft 365 SKUs.

Esses clientes já terão o Azure ou o Microsoft 365 e o modelo de venda mostrará que é provável que eles comprem mais de sua SKU existente.

EOS compartilha os clientes de fim de serviço (EOS) para o Win 7, o Office 2010, o SQL Server e o Windows Server. Os dados de EOS são extraídos da MS Sales e sobrepostos com a modelagem de propensão CloudAscent, quando disponível. Os dados de EOS residem no trabalho moderno e nas atividades de vendas do Azure.
