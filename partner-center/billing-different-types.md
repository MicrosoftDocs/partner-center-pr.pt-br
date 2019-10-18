---
title: Noções básicas sobre os tipos de cobrança no Partner Center | Partner Center
ms.topic: article
ms.date: 10/04/2019
Description: Informações sobre diferentes tipos de cobrança, períodos de cobrança e datas de cobrança
author: MaggiePucciEvans
ms.author: evansma
keywords: cobrança, pagamentos, pedidos, arquivos de reconciliação, arquivo de reconhecimento
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 28a5405a033061e5665d0f1e5f937cd3951f09b9
ms.sourcegitcommit: dcc2a2077ef17255ecf7a2fa5fae6bbeefaa9eb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/07/2019
ms.locfileid: "71997840"
---
# <a name="understanding-the-types-of-billing-in-partner-center"></a>Entendendo os tipos de cobrança no Partner Center

**Aplica-se a**

-  Partner Center
-  Parceiros no programa CSP

Dependendo dos tipos de produtos que você compra para seus clientes, poderá haver diferentes períodos de cobrança e esta poderá ser efetuada em diferentes dias do mesmo mês. Este artigo explica o que mudou desde 1º de março de 2019 e como as alterações afetarão você.

## <a name="billing-for-recurring-charges"></a>Cobrança por encargos recorrentes

A experiência de cobrança para encargos recorrentes de assinaturas baseadas em licença e em uso não mudará. Continuaremos cobrando você no dia do mês selecionado como sua data de cobrança e seu período de cobrança continuará sendo o mês anterior a essa data. Se você selecionou o 15º dia do mês da sua data de cobrança, você será cobrado por toda a atividade desde o 15º dia de um mês calendário até o 14º dia do mês calendário seguinte. As faturas e os arquivos de reconciliação estão em disponibilidade geral de 2 a 4 dias após sua data de cobrança.

Como antes, cobraremos por esses produtos na moeda do país/região em que você está localizado, independentemente do local do cliente para o qual você vendeu o produto.

## <a name="billing-for-one-time-and-select-recurring-charges"></a>Cobrança única e seleção de encargos recorrentes

A partir de 1º de março de 2019, apresentamos uma nova experiência de cobrança para cobranças recorrentes e únicas de produtos ISV da Microsoft e de terceiros.

Para esses produtos, o período de cobrança começa no primeiro dia do mês calendário e termina no último dia do mês calendário. Disponibilizaremos sua fatura no oitavo dia do mês seguinte. 

Em outras palavras, as transações efetuadas entre 1º e 31 de maio de 2019 serão exibidas em sua fatura no dia 8 de junho. Transações efetuadas entre 1º e 30 de junho de 2019 serão exibidas em sua fatura no dia 8 de julho. Você pode ser cobrado por compras recorrentes e avulsas na mesma fatura. 

Você também pode verificar seu saldo/fatura da conta sempre que desejar (por exemplo, entre 1º de maio e 7 de junho) e ver a atividade de conta mais recente sem precisar aguardar a fatura. Observe que, quando postamos sua fatura no 8º dia, ela incluirá impostos e outros encargos e créditos aplicáveis, para que o valor final possa ser diferente do que você vê durante o período de cobrança. 

Você acessará suas faturas da mesma maneira como faz agora, seja no Partner Center ou pela API. Elas serão exibidas antes da meia-noite UTC e no 8º dia do mês. 

|**Experiência de cobrança**|**Tipos de produto**|**Data de cobrança**|**Período de cobrança**|**Moeda de cobrança**|**Atividade atual disponível?**|
|:----------------|:--------------|:--------------|:--------------|:--------------|:--------------|
|Encargos recorrentes para assinaturas baseadas em licença e em uso |Todos os produtos do [catálogo de serviços online](https://partner.microsoft.com/commerce/preferredoffers/list). Os exemplos incluem Office 365, Microsoft 365, Azure Active Directory, Azure (pago conforme o uso), Dynamics 365, PowerBI Pro |A data selecionada quando você criou sua conta do Partner Center |O mês antes da sua data de cobrança. |A moeda do país/região no qual você está localizado. Por exemplo, se a sua empresa estiver localizada no Reino Unido, cobraremos você em GBP (libras esterlinas britânicas). Se a sua empresa estiver localizada na Índia, cobraremos você em INR (rúpias indianas).  |Não |
|Encargos recorrentes e únicos para produtos ISVs de terceiros e da Microsoft |Todas as assinaturas SaaS, reservas do Azure e produtos de software (perpétua e baseadas em assinatura) oferecidos por ISVs da Microsoft e de terceiros. Confira os produtos disponíveis no [Marketplace](https://partner.microsoft.com/commerce/sales?type=Any&category=Any). Os exemplos incluem software SUSE Linux (assinatura do software), Windows Server 2019 Essentials (software perpétuo), assinatura de produto SaaS do ISV do Azure. |O 8º dia de cada mês |Do primeiro ao último dia de cada mês calendário |A moeda do país/região no qual seu cliente está localizado. Isso significa que você receberá faturas e arquivos de reconciliação separados na moeda do país/região para cada cliente que você vendeu no período de cobrança. |Sim |

## <a name="billing-scenarios-for-one-time-and-recurring-purchases"></a>Cenários de cobrança para compras únicas e recorrentes
### <a name="scenario-1--purchase-a-subscription-and-then-add-a-seat-on-the-same-day"></a>Cenário 1 – Comprar uma assinatura e adicionar um usuário no mesmo dia

No Cenário 1, você compra uma assinatura em 11 de junho a um preço unitário de US$ 4. Mais tarde, no mesmo dia, você compra outra assinatura como a anterior pelo mesmo preço. 

O arquivo de reconhecimento incluirá o seguinte: 
-   Cobrança de US$ 4 pelo período de serviço de 10 de junho – 9 de julho. 
-   Nova cobrança proporcional de US$ -4,00 pelo período de serviço de 11 de junho – 11 de junho. Nesse período, você tinha 1 licença. Cálculo = (preço mensal/total de dias no período de serviço) x dias no período de serviço proporcional x número de licenças = (4/30) x 30 x 1 = 4,00.
-   Nova cobrança proporcional de US$ 8,00 pelo período de serviço de 10 de junho – 9 de julho. Nesse período, você tinha 2 licenças. Cálculo = (4/30) x 30 x 2 = 8,00.

|**Data de compra**   |**Início da cobrança**  |**Término da cobrança**  |**Preço unitário**  |**Quantidade**  |**Valor** |**Tipo de cobrança** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/06/2019      |10/06/2019   |9/07/2019         |US$ 4                |1                 |US$ 4            |Novo         |
|11/06/2019     | 10/06/2019    |9/07/2019        |US$ 4        |1        | -US$ 4       |addQuantity           |
|11/06/2019     | 10/06/2019    |9/07/2019        |US$ 4        | 2      |US$ 8         |addQuantity           |

### <a name="scenario-2--purchase-a-subscription-and-then-add-more-later"></a>Cenário 2 – Comprar uma assinatura e adicionar mais tarde

No Cenário 2, você compra uma assinatura em 11 de junho com um preço unitário de US$ 4 e, em 12 de junho, você compra outra assinatura do mesmo produto pelo mesmo preço. 

O arquivo de reconhecimento incluirá o seguinte: 
-   Cobrança de US$ 4 pelo período de serviço de 10 de junho – 9 de julho. 
-   Nova cobrança proporcional de US$ -3,87 pelo período de serviço de 11 de junho – 12 de junho. Nesse período, você tinha 1 licença. Cálculo = (preço mensal/total de dias no período de serviço) x dias no período de serviço proporcional x número de licenças = (4/30) x 29 x 1 = 3,87.
-   Nova cobrança proporcional de US$ 7,74 pelo período de serviço de 12 de junho – 9 de julho. Nesse período, você tinha 2 licenças. Cálculo = (4/30) x 29 x 2 = 7,74.

|**Data de compra**   |**Início da cobrança**  |**Término da cobrança**  |**Preço unitário**  |**Quantidade**  |**Valor** |**Tipo de cobrança** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/06/2019 (você tem uma licença)     |10/06/2019   |9/07/2019         |US$ 4         |1        |US$ 4            |Novo         |
|12/06/2019     | 10/06/2019    |9/07/2019        |US$ 4        |1        | -US$ 3,87       |addQuantity           |
|12/06/2019     | 10/06/2019    |9/07/2019        |US$ 4        | 2      |US$ 7,74       |addQuantity           |

### <a name="scenario-3--purchase-a-subscription-and-then-remove-a-seat-on-the-same-day"></a>Cenário 3 – Comprar uma assinatura e remover um usuário no mesmo dia

No Cenário 3, você compra duas assinaturas para o mesmo produto em 11 de junho a um preço unitário de US$ 4. Mais tarde, no mesmo dia, você remove um dos usuários.  

O arquivo de reconhecimento incluirá o seguinte: 
-   Cobrança de US$ 8 por duas licenças pelo período de serviço de 10 de junho – 9 de julho. 
-   Nova cobrança proporcional de US$ -8,00 pelo período de serviço de 11 de junho – 11 de junho. Nesse período, você tinha 2 licenças. Cálculo = (preço mensal/total de dias no período de serviço) x dias no período de serviço proporcional x número de licenças = (4/30) x 30 x 2 = 8,00.
-   Nova cobrança proporcional de US$ 4,00 pelo período de serviço de 11 de junho – 9 de julho. Nesse período, você tinha 1 licença. Cálculo = (4/30) x 30 x 1 = 4,00.

|**Data de compra**   |**Início da cobrança**  |**Término da cobrança**  |**Preço unitário**  |**Quantidade**  |**Valor** |**Tipo de cobrança** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/06/2019      |10/06/2019   |9/07/2019         |US$ 4                |2                 |US$ 8            |Novo         |
|11/06/2019     | 10/06/2019    |9/07/2019        |US$ 4        |2        | -US$ 8       |removeQuantity           |
|11/06/2019     | 10/06/2019    |9/07/2019        |US$ 4        | 1      |US$ 4         |removeQuantity           |

### <a name="scenario-4--purchase-a-subscription-and-then-remove-seats-later"></a>Cenário 4 – Comprar uma assinatura e remover usuários mais tarde

No Cenário 4, você compra duas assinaturas em 11 de junho pelo preço unitário de US$ 4 e em 12 de junho você remove um dos usuários. 

O arquivo de reconhecimento incluirá o seguinte: 
-   Cobrança de US$ 8 pelo período de serviço de 10 de junho – 9 de julho. 
-   Nova cobrança proporcional de US$ -7,74 pelo período de serviço de 11 de junho – 12 de junho. Nesse período, você tinha 2 licenças. Cálculo = (preço mensal/total de dias no período de serviço) x dias no período de serviço proporcional x número de licenças = (4/30) x 29 x 2 = 7,74.
-   Nova cobrança proporcional de US$ 3,87 pelo período de serviço de 12 de junho – 9 de julho. Nesse período, você tinha 1 licença. Cálculo = (4/30) x 29 x 1 = 3,87.

|**Data de compra**   |**Início da cobrança**  |**Término da cobrança**  |**Preço unitário**  |**Quantidade**  |**Valor** |**Tipo de cobrança** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/06/2019 (você tem duas licenças)     |10/06/2019   |9/07/2019         |US$ 4         |2        |US$ 8       |Novo       |
|12/06/2019     | 10/06/2019    |9/07/2019        |US$ 4        |2        | -US$ 7,74       |removeQuantity           |
|12/06/2019 (você tem uma licença)    | 10/06/2019    |9/07/2019   |US$ 4    |1      |US$ 3,87    |removeQuantity |

## <a name="billing-scenarios-for-free-trial-license-based-saas-transactions"></a>Cenários de cobrança para transações de SaaS baseadas em licença de avaliação gratuita
### <a name="scenario-5--renew-a-license-based-free-trial-saas-subscription-to-a-paid-subscription-at-the-end-of-the-free-trial-period"></a>Cenário 5 – Renovar uma assinatura de SaaS de avaliação gratuita baseada em licença para uma assinatura paga no final do período de avaliação gratuita

Nesse cenário, você compra uma assinatura de SaaS (software como serviço) baseada em licença de avaliação gratuita em 10 de junho e ela será renovada automaticamente como uma assinatura paga quando o período de avaliação gratuita terminar. 

Os arquivos de reconhecimento incluirá o seguinte: 
- Cobrança de US$ 0 pelo período de serviço de 10 de junho – 9 de julho 
- Cobrança de US$ 2 pelo período de serviço de 10 de julho – 9 de agosto

|**Data de compra**   |**Início da cobrança**  |**Término da cobrança**  |**Preço unitário**  |**Quantidade**  |**Valor** |**Tipo de cobrança** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|10/06/2019 (você tem uma licença)      |10/06/2019   |9/07/2019         |US$ 0                |1                 |US$ 0            |Novo         |
|10/07/2019 (você tem uma licença)     | 10/07/2019    |9/08/2019        |US$ 2        |1        | US$ 2       |renovar           |

### <a name="scenario-6--cancel-a-license-based-free-trial-saas-subscription"></a>Cenário 6 – Cancelar uma assinatura de SaaS de avaliação gratuita baseada em licença

É possível cancelar uma assinatura de SaaS (software como serviço) de avaliação gratuita baseada em licença a qualquer momento, mesmo durante o período da avaliação gratuita. 

Nesse cenário, você compra uma assinatura de SaaS de avaliação gratuita baseada em licença em 1º de julho e a cancela imediatamente no Partner Center. 

O arquivo de reconhecimento incluirá o seguinte: 
- Cobrança de US$ 0 pelo período de serviço de 10 de junho – 9 de julho para a nova compra
- Cobrança de US$ 0 pelo período de serviço de 10 de julho – 9 de julho para o cancelamento

|**Data de compra**   |**Início da cobrança**  |**Término da cobrança**  |**Preço unitário**  |**Quantidade**  |**Valor** |**Tipo de cobrança** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|10/06/2019 (você tem 11 licenças)      |10/06/2019   |9/07/2019         |US$ 0                |11                |US$ 0            |Novo         |
|10/06/2019 (você tem zero licenças)     | 10/06/2019    |9/07/2019        |US$ 0        |11       | US$ 0       |cancelar           |

### <a name="scenario-7--convert-a-custom-meter-saas-subscription-from-one-sku-to-another-for-the-same-product-on-the-same-day"></a>Cenário 7 – Converter uma assinatura de SaaS de medidor personalizado de um SKU em outro para o mesmo produto no mesmo dia

Nesse cenário, você compra um SKU (Prata) em um produto e o converte em outro SKU disponível (Bronze) nesse produto no mesmo dia. 

O arquivo de reconhecimento incluirá o seguinte: 
- Cobrança de US$ 20 do Prata pelo período de serviço de 10 de junho de 2019 – 9 de julho de 2020
- Nova cobrança proporcional de US$ 20 pelo Prata pelo período de serviço de 10 de junho de 2019 – 9 de julho de 2020
- Cobrança de US$ 10 pelo Bronze pelo período de serviço de 10 de junho de 2019 – 9 de julho de 2020

|**Data de compra**   |**SKU**   |**Início da cobrança**   |**Término da cobrança**  |**Preço unitário**  |**Quantidade**  |**Valor** |**Tipo de cobrança** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|:-----:|
|10/06/2019 (você tem uma licença) |Prata     |10/06/2019   |10/06/2019         |US$ 20        |1         |US$ 20            |Novo      |
|10/06/2019 (você tem uma licença) |Prata    | 10/06/2019    |10/06/2019        |US$ 20        |1       | US$ -20       |Converter           |
|10/06/2019 (você tem uma licença) |Bronze    | 10/06/2019    |10/06/2019        |US$ 10        |1       | US$ 10       |Converter           |

### <a name="scenario-8--purchase-and-cancel-a-custom-meter-saas-subscription-from-the-azure-portal-on-the-same-day"></a>Cenário 8 – Comprar e cancelar uma assinatura de SaaS de medidor personalizado no portal do Azure no mesmo dia 

Nesse cenário, você compra uma assinatura do SaaS do medidor personalizado no portal do Azure e a cancela no mesmo dia. 

|**Data de compra**   |**SKU**   |**Início da cobrança**   |**Término da cobrança**  |**Preço unitário**  |**Quantidade**  |**Valor** |**Tipo de cobrança** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|:-----:|
|10/06/2019 (você tem uma licença) |Bronze     |10/06/2019   |10/06/2019         |US$ 10        |1         |US$ 10            |Novo      |
|10/06/2019 (você tem 0 licenças) |Bronze    | 10/06/2019    |10/06/2019        |US$ 10        |1       | US$ -10       |CancelImmediate  |

## <a name="billing-under-the-azure-plan"></a>Cobrança no plano do Azure

- **Data da nota fiscal**: a nota fiscal e o arquivo de reconciliação estarão disponíveis no painel do Partner Center/API pelo oitavo (meia-noite UTC).

- **Período de cobrança da fatura**: o período de cobrança da nota fiscal está alinhado ao mês do calendário, por exemplo, 10/1-10/31, 11/1-11/30).

- **Períodos de serviço de cobrança**: as cobranças serão alinhadas ao mês civil. Por exemplo, se o parceiro cobrado adicionar serviços do Azure por meio de um plano do Azure em 10/15 e o cliente iniciar o consumo de serviços do Azure em 10/15, o parceiro cobrado receberá fatura/reconhecimento em 11/8 para consumo de cliente pelo período de serviço 10/15-10/31. A fatura do próximo mês que será gerada em 12/8 contém todos os encargos para o período de serviço 11/1-11/31.

- **Termo de pagamento de fatura**: net 60 dias.

- **Moeda da nota fiscal**: os parceiros continuarão sendo cobrados na moeda atribuída do country's do cliente. Por exemplo, se o parceiro cobrado estiver na Irlanda com clientes do Reino Unido, da Noruega e da Alemanha, o parceiro cobrado receberá uma nota fiscal/reconhecimento de GBP, NOK e EUR.

- **Incentivos para parceiros**: pago 45 dias a partir do final do mês da nota fiscal.

Para obter informações sobre o plano do Azure, consulte:

- [Plano do Azure-visão geral](azure-plan-get-started.md)

- [Plano do Azure – cobrança](azure-plan-billing.md)