---
title: Análises do Partner Center – relatórios de CloudAscent propensation
description: Saiba mais sobre os relatórios de CloudAscent propensation no Partner Center. Inclui informações sobre as propensações de um cliente para comprar produtos da Microsoft.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 09/18/2020
ms.openlocfilehash: 2cdb63c8f7e29fc8a56e920b587e47c382c6eacb
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "106086950"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a>Relatórios de CloudAscent propensation disponíveis no painel do Partner Center

**Funções apropriadas**

- Visualizador de relatórios executivos
- Visualizador de relatórios

O painel do Partner Center fornece dados de propensação baixáveis do programa CloudAscent. Os dados mostram a propensão dos clientes para comprar produtos da Microsoft.  Este artigo descreve a divisão desses dados, como usar a pontuação e o que isso significa.

## <a name="summary-definitions"></a>Definições de resumo

- **Clientes do SMC**– este é o número total de clientes nos downloads de propensação.  Os clientes são identificados pelo parceiro do registro.
- **Contratos de expiração**– dentro do ano fiscal atual, estamos fornecendo o número de contratos expirando.
- **Receita de expiração**– a receita associada aos contratos expirados.
- **Abrir receita de expiração**– a receita associada aos contratos expirados abertos.

:::image type="content" source="images/pci/cust-oppor-1.png" alt-text="Captura de tela do painel de Resumo de oportunidades de clientes.":::

## <a name="cloudascent-smb-segmentation"></a>Segmentação SMB do CloudAscent

O segmento SMB (de pequeno a médio porte) é dividido em três subsegmentos distintos.

1. A **parte superior não gerenciada** inclui os maiores clientes SMB com mais oportunidade para a Microsoft. Os principais clientes não gerenciados compartilham características semelhantes às contas gerenciadas, com grande número de funcionários, grandes orçamentos de ti e gastos e grandes quantidades de receitas potenciais para a Microsoft.

   Definimos duas maneiras principais não gerenciadas:

   - **Com base em principais usuários não gerenciados**– inclui contas com 300 ou mais funcionários. User-Based contas são ótimos alvos para compra pela primeira vez ou expansão de produtos de assinatura baseados em usuário, como Microsoft 365, Dynamics 365 ou Surface.
   - **Base de computação não gerenciada superior** – inclui contas com o potencial do Azure maior que $10K. As contas baseadas em computação incluem o Azure existente. Acesse as contas com potencial do ano futuro e contas que ainda não compraram o Azure, mas têm potencial para o Azure com mais de US $10.000.

2. Os **negócios médios** incluem clientes existentes e contas de clientes potenciais com 25 a 300 funcionários.

3. A **pequena empresa** inclui todas as empresas restantes com menos de 25 funcionários.

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="Cliente por tipo SMC.":::

Os principais subsegmentos de negócios **não gerenciados** e **médios** representam clientes LTV (valor de tempo de vida alta) para a Microsoft e parceiros da Microsoft. Por isso, eles são as áreas potenciais de foco para impulsionar o crescimento nesse segmento. Nesses dois subsegmentos, estamos mais bem posicionados para adquirir o soquete com Microsoft 365, monetizar ainda mais com aplicativos de LOB (linha de negócios) D365/Azure e percebem um alto LTV para a Microsoft.

Hoje temos duas áreas-chave de oportunidade – 1. nosso cliente adiciona crescimento; 2. Embora possamos adquirir os soquetes de nuvem que levam com Microsoft 365, temos uma grande oportunidade no D365 e no Azure.

A captura de tela a seguir representa os três subsegmentos SMB e as rotas otimizadas para o mercado. CloudAscent priorize a criação de perfil, a pontuação e a modelagem de todas as principais contas de negócios não gerenciadas e médias.

:::image type="content" source="images/pci/cust-oppor-3.png" alt-text="Captura de tela de subsegmentos SMB.":::

## <a name="cloudascent-machine-learning"></a>Machine Learning CloudAscent

O SMB usa a tecnologia de aprendizado de máquina para orientar as previsões de vendas e marketing dos clientes dentro dos principais segmentos de negócios não gerenciados e médios. Como os sinais são coletados e transformados nas recomendações de propensação?

- **Coleta de dados**: os rastreadores da Web examinam e coletam bilhões de sinais de clientes ao executar ping nos domínios da empresa e monitoramento: Postagens de blog, Press Releases, fluxos sociais e fóruns técnicos.  Além dos sinais coletados, as informações de firmographics são coletadas de fontes internas e externas, como D&B, assinatura interna da Microsoft e dados transacionais.

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

   - A pontuação da intenção é sobreposta sobre ajustar para definir os clusters.

   - A pontuação da intenção é atualizada mensalmente.

   :::image type="content" source="images/pci/cust-oppor-5.png" alt-text="Modelos de previsão do CloudAscent SMB.":::

3. Clustering

   Os sinais para ajuste e intenção são consolidados em uma pontuação de clustering. O CloudAscent tem quatro clusters:

      - Clientes do Act Now-Sales Ready
      - Avaliar-clientes prontos para marketing
      - Campanhas de reconhecimento de incentivá
      - Instrua-instrua e monitore para a intenção

   O clustering permite que os usuários direcionem clientes específicos para iniciativas de vendas e marketing com base em fatores de segmento, por exemplo: produto, geográfico, setor e vertical.

   A guia **modelo** de propensão nas pastas de trabalho CloudAscent compartilha a propensão e a receita de espaço em branco estimada. Para definir o clustering de ajuste e intenção, percorreremos as seguintes etapas:

      1. Usando modelos de ML, primeiro calculamos a pontuação de ajuste do cliente e a pontuação de intenção em uma escala de 100.  As pontuações exatas variarão com base nos modelos de ML.  Pontuação de exemplo abaixo:

         |**Classificação**|**Pontuação**|
         |---------|:---------|
         |Alto|75-100|
         |Médio|55-74|
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

O EOS compartilha o fim dos clientes de serviço para o Windows 7, o Office 2010, o SQL Server e o Windows Server. Os dados de EOS são extraídos da MS Sales e sobrepostos com a modelagem de propensão CloudAscent, quando disponível. Os dados de EOS residem no trabalho moderno e nas atividades de vendas do Azure.
