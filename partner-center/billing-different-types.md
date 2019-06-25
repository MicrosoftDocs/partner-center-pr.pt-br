---
title: Noções básicas sobre os tipos de cobrança no Partner Center | Partner Center
ms.topic: article
ms.date: 03/01/2019
Description: Informações sobre os diferentes tipos de cobrança, períodos de cobrança e datas de cobrança
author: MaggiePucciEvans
ms.author: evansma
keywords: cobrança, pagamentos, pedidos, os arquivos de reconciliação, reconhecimento de arquivo
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 3e664a8a539125bce21d256c6e6d88d1ab22d14d
ms.sourcegitcommit: 1f9078d422af5f8514d79a6ab9c3444500abfe27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2019
ms.locfileid: "67343452"
---
# <a name="understanding-the-types-of-billing-in-partner-center"></a>Entendendo os tipos de cobrança no Partner Center

**Aplica-se a**

-  Partner Center
-  Parceiros no programa CSP

Dependendo dos tipos de produtos que você compra para seus clientes, você pode ter diferentes períodos de cobrança e cobradas em dias diferentes do mesmo mês. Este artigo explica o que mudou começando em 1 de março de 2019, e como as alterações afetarão você.

## <a name="billing-for-recurring-charges"></a>Cobrança de encargos recorrentes

A experiência de cobrança para os encargos recorrentes de assinaturas com base em licença e baseada em uso não está sendo alterado. Continuaremos a cobrar de você no dia do mês em que você selecionou como a data de cobrança e o período de cobrança continuará o mês antes dessa data. Se você tiver selecionado o 15º dia do mês de sua data de cobrança, você será cobrado por toda a atividade do 15º dia de um mês do calendário no dia 14 do próximo mês do calendário. As faturas e arquivos de reconciliação estão geralmente disponíveis 2 a 4 dias após sua data de cobrança.

Como antes, nós cobraremos você para esses produtos na moeda para o país/região que você está localizado, independentemente do local do cliente você vendeu o produto.

## <a name="billing-for-one-time-and-select-recurring-charges"></a>Cobrança de encargos recorrentes únicos e selecionadas

Começando em 1 de março de 2019, apresentamos uma nova experiência de cobrança de encargos recorrentes e de uso únicos para a Microsoft e produtos de ISVS de terceiros.

Para esses produtos, o período de cobrança começa no primeiro dia do mês do calendário e termina no último dia do mês do calendário. Que disponibilizaremos sua fatura no dia 8 do mês seguinte. 

Em outras palavras, todas as transações feitas entre 1º de maio e 31 de maio de 2019 aparecerá na sua fatura 8 de junho. Todas as transações feitas entre 1º de junho e 30 de junho de 2019 aparecerão na sua fatura 8 de julho. Você pode obter cobrado para compras recorrentes e de uso únicas na mesma nota fiscal. 

Você também pode verificar seu saldo de conta/fatura sempre que você deseja (por exemplo, entre 1º de maio e 7 de junho) e veja a última atividade de conta sem precisar aguardar a nota fiscal. Observe que quando publicarmos sua fatura na 8, ele incluirá os impostos e quaisquer outros encargos aplicáveis e créditos, portanto, o valor final pode diferir da que você vê durante o período de cobrança. 

Você acessará suas faturas da mesma maneira que você faça agora no Partner Center ou pela API. Eles serão exibidos antes da meia-noite UTC em que o 8º dia do mês. 

|**Experiência de cobrança**|**Tipo de produto (s)**|**Data de cobrança**|**Período de cobrança**|**Moeda de cobrança**|**Atividade atual disponível?**|
|:----------------|:--------------|:--------------|:--------------|:--------------|:--------------|
|Encargos recorrentes para assinaturas baseados em uso e licença |Todos os produtos da [catálogo de serviços online](https://partner.microsoft.com/commerce/preferredoffers/list). Exemplos incluem o Office 365, Microsoft 365, Azure Active Directory, Azure (pré-pago), do Dynamics 365, Power BI Pro |A data em que você selecionou quando criou sua conta no Partner Center |O mês antes da sua data de cobrança. |A moeda do país/região que você está localizado. Por exemplo, se sua empresa está localizada no Reino Unido, nós cobraremos você em libras esterlinas (GBP). Se sua empresa está localizada na Índia, nós cobraremos você na Índia rúpias (INR).  |Não |
|Encargos recorrentes e de uso únicos para a Microsoft e produtos de ISVs de terceiros |Todos os SaaS assinaturas, as reservas do Azure e produtos de software (perpétua e baseada em assinatura) oferecidos pela Microsoft e ISVs de terceiros. Consulte produtos disponíveis a [Marketplace](https://partner.microsoft.com/commerce/sales?type=Any&category=Any). Exemplos incluem o software do SUSE Linux (assinatura de software), Windows Server 2019 Essentials (software permanente), assinatura de produtos de SaaS ISV do Azure. |8 de dia de cada mês |Desde o primeiro dia até o último dia de cada mês do calendário |A moeda de país/região ou o cliente está localizado em. Isso significa que você vai receber faturas separadas e arquivos de reconciliação na moeda do país/região cada cliente vendido para no período de cobrança. |Sim |

## <a name="billing-scenarios-for-one-time-and-recurring-purchases"></a>Cenários de cobrança para compras únicos e recorrentes
### <a name="scenario-1--purchase-a-subscription-and-then-add-a-seat-on-the-same-day"></a>Cenário 1 – Compre uma assinatura e, em seguida, adicione um Assento no mesmo dia

No cenário 1, você pode comprar uma assinatura no dia 11 de junho a um preço unitário de US $4. Posteriormente nesse dia mesmo que você comprar outro da mesma assinatura com o mesmo preço. 

O arquivo de recon incluirá o seguinte: 
-   fatura US $4 por período de serviço 10 de junho – 9 de julho. 
-   $4.00 rebill rateada por 11 de junho – 11 de junho de período de serviço. Esse é o período que havia 1 licença. Cálculo = (mensais totais/preço dias no período de serviço) x dias no serviço rateado período x número de licenças = (4/30) x 30 x 1 = 4.00.
-   US $8.00 proporcional rebill para 10 de junho – 9 de julho do período de serviço. Esse é o período que havia 2 licenças. Cálculo = (4/30) x 30 x 2 = 8.00.

|**Data de compra**   |**Custo inicial**  |**Final de encargo**  |**Preço unitário**  |**quantidade**  |**Quantidade** |**Tipo de encargo** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019      |6/10/2019   |7/09/2019         |$4                |1                 |$4            |Novo         |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        |1        | -$4       |addQuantity           |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        | 2      |$8         |addQuantity           |

### <a name="scenario-2--purchase-a-subscription-and-then-add-more-later"></a>Cenário 2 – Compre uma assinatura e, em seguida, adicionar mais posteriormente

No cenário 2, você comprar uma assinatura no dia 11 de junho a um preço unitário de US $4 e, em 12 de junho você compra outra assinatura para o mesmo produto com o mesmo preço. 

O arquivo de recon incluirá o seguinte: 
-   fatura US $4 por período de serviço 10 de junho – 9 de julho. 
-   $3,87 rebill rateada por 11 de junho – 12 de junho de período de serviço. Esse é o período que havia 1 licença. Cálculo = (mensais totais/preço dias no período de serviço) x dias no serviço rateado período x número de licenças = x (30/4) 29 x 1 = 3,87.
-   US $7.74 proporcional rebill para 12 de junho – 9 de julho do período de serviço. Esse é o período que havia 2 licenças. Cálculo = x (30/4) 29 x 2 = 7.74.

|**Data de compra**   |**Custo inicial**  |**Final de encargo**  |**Preço unitário**  |**quantidade**  |**Quantidade** |**Tipo de encargo** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/6/2019 (você tem uma licença)     |6/10/2019   |7/09/2019         |$4         |1        |$4            |Novo         |
|6/12/2019     | 6/10/2019    |7/09/2019        |$4        |1        | -$3.87       |addQuantity           |
|6/12/2019     | 6/10/2019    |7/09/2019        |$4        | 2      |$7.74       |addQuantity           |

### <a name="scenario-3--purchase-a-subscription-and-then-remove-a-seat-on-the-same-day"></a>Cenário 3 – Compre uma assinatura e, em seguida, remover um Assento no mesmo dia

Cenário 3, você comprar duas assinaturas para o mesmo produto no dia 11 de junho a um preço unitário de US $4. Posteriormente nesse dia mesmo que você remova uma das estações.  

O arquivo de recon incluirá o seguinte: 
-   cobrança de US $8 para duas licenças para 10 de junho – 9 de julho do período de serviço. 
-   $8.00 rebill rateada por 11 de junho – 11 de junho de período de serviço. Esse é o período que havia 2 licenças. Cálculo = (mensais totais/preço dias no período de serviço) x dias no serviço rateado período x número de licenças = (4/30) x 30 x 2 = 8.00.
-   US $4.00 proporcional rebill para 11 de junho – 9 de julho do período de serviço. Esse é o período que havia 1 licença. Cálculo = (4/30) x 30 x 1 = 4.00.

|**Data de compra**   |**Custo inicial**  |**Final de encargo**  |**Preço unitário**  |**quantidade**  |**Quantidade** |**Tipo de encargo** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019      |6/10/2019   |7/09/2019         |$4                |2                 |$8            |Novo         |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        |2        | -$8       |removeQuantity           |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        | 1      |$4         |removeQuantity           |

### <a name="scenario-4--purchase-a-subscription-and-then-remove-seats-later"></a>Cenário 4 – adquira uma assinatura e, em seguida, remover estações mais tarde

No cenário 4, você compra 2 assinaturas no dia 11 de junho a um preço unitário de US $4 e, em 12 de junho você remova um das estações. 

O arquivo de recon incluirá o seguinte: 
-   cobrança de US $8 de 10 de junho – 9 de julho do período de serviço. 
-   $7.74 rebill rateada por 11 de junho – 12 de junho de período de serviço. Esse é o período que havia 2 licenças. Cálculo = (mensais totais/preço dias no período de serviço) x dias no serviço rateado período x número de licenças = x (30/4) 29 x 2 = 7.74.
-   US $3,87 proporcional rebill para 12 de junho – 9 de julho do período de serviço. Esse é o período que havia 1 licença. Cálculo = x (30/4) 29 x 1 = 3,87.

|**Data de compra**   |**Custo inicial**  |**Final de encargo**  |**Preço unitário**  |**quantidade**  |**Quantidade** |**Tipo de encargo** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/6/2019 (você tem 2 licenças)     |6/10/2019   |7/09/2019         |$4         |2        |$8       |Novo       |
|6/12/2019     | 6/10/2019    |7/09/2019        |$4        |2        | -$7.74       |removeQuantity           |
|12/6/2019 (você tem 1 licença)    | 6/10/2019    |7/09/2019   |$4    |1      |$3.87    |removeQuantity |
