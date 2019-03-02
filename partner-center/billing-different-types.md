---
title: Noções básicas sobre os tipos de cobrança no Partner Center | Partner Center
ms.topic: article
ms.date: 03/01/2019
Description: Informações sobre os diferentes tipos de cobrança, períodos de cobrança e datas de cobrança
author: labrenne
ms.author: labrenne
keywords: cobrança, pagamentos, pedidos, arquivos de reconciliação, arquivo de reconciliação
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 777a98f8780eb036b4bac99eca9a5621d61da66b
ms.sourcegitcommit: 8bfd1358a0ef86e46bee2a1097d86de3c9e969e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/02/2019
ms.locfileid: "9122284"
---
# <a name="understanding-the-types-of-billing-in-partner-center"></a>Noções básicas sobre os tipos de cobrança no Partner Center

**Aplica-se ao**

-  Partner Center
-  Parceiros no programa CSP

Dependendo dos tipos de produtos que você comprar para seus clientes, você pode ter diferentes períodos de cobrança e cobrado em dias diferentes do mesmo mês. Este artigo explica o que está mudando a partir de 1º de março de 2019, e como as alterações afetarão você.

## <a name="billing-for-recurring-charges"></a>Cobrança para encargos recorrentes

A experiência de cobrança para encargos recorrentes das assinaturas baseadas em licença e em uso não está mudando. Continuaremos cobrar você no dia do mês selecionado como sua data de cobrança e o período de cobrança continuará a ser o mês antes da data. Se você selecionou o 15º dia do mês para sua data de cobrança, você será cobrado pela toda a atividade do dia 15 de um mês de calendário no dia 14 do mês seguinte. Faturas e arquivos de reconciliação são estará disponíveis 2 a 4 dias após a data de cobrança.

Como antes, será cobrado para esses produtos na moeda para o país/região que você está localizado nos, independentemente do local do cliente você vendeu o produto.

## <a name="billing-for-one-time-and-select-recurring-charges"></a>Cobrança únicas e selecionados encargos recorrentes

A partir de 1º de março de 2019, apresentamos uma nova experiência de cobrança para encargos recorrentes e únicas para produtos da Microsoft e de terceiros ISV.

Para esses produtos, o período de cobrança começa no primeiro dia do mês do calendário e termina no último dia do mês do calendário. Faremos sua fatura disponíveis no 8 de dia do mês seguinte. 

Em outras palavras, todas as transações feitas entre 1º de maio e 31 de maio de 2019 aparecerão em sua fatura de 8 de junho. Todas as transações feitas entre 1º de junho e 30 de junho de 2019 aparecerão em sua fatura de 8 de julho. Você pode obter cobrado por compras únicas e recorrentes na mesma fatura. 

Você também pode verificar sua fatura da proporção de conta sempre que você deseja (por exemplo, entre 1 de maio e 7 de junho) e ver a atividade mais recente da conta sem precisar aguardar fatura. Observe que quando sua fatura, lança a 8, ele incluirá impostos e quaisquer outros encargos aplicáveis e créditos, portanto, o valor final pode ser diferente do que você vê durante o período de cobrança. 

Você vai acessar suas faturas da mesma maneira que você faça agora, no Partner Center ou pela API. Eles aparecerão antes da meia-noite UTC em 8 de dia do mês. 

|**Experiência de cobrança**|**Tipos de produto**|**Data da cobrança**|**Período de cobrança**|**Moeda de cobrança**|**Atividade atual disponível?**|
|:----------------|:--------------|:--------------|:--------------|:--------------|:--------------|
|Encargos recorrentes para assinaturas baseadas em licença e baseadas em uso |Todos os produtos no [Catálogo de serviços online](https://partner.microsoft.com/commerce/preferredoffers/list). Exemplos incluem o Office 365, Microsoft 365, Azure Active Directory, Azure (pagamento conforme o uso), Dynamics 365, PowerBI Pro |A data em que você selecionou quando você criou sua conta do Partner Center |O mês antes da sua data de cobrança. |A moeda do país/região que você está localizado em. Por exemplo, se sua empresa está localizada no Reino Unido, será cobrado em libras esterlinas (GBP). Se sua empresa está localizada na Índia, será cobrado na Índia rúpias (INR).  |Não |
|Encargos recorrentes e únicos para produtos da Microsoft e de terceiros ISVs |Todos os SaaS assinaturas, reservas do Azure e produtos de software (permanente e baseado em assinatura) oferecidos pela Microsoft e os ISVs de terceiros. Veja os produtos disponíveis no [mercado](https://partner.microsoft.com/commerce/sales?type=Any&category=Any). Exemplos incluem software SUSE Linux (assinatura de software), Windows Server 2019 Essentials (software permanente), a assinatura do Azure ISV SaaS produto. |8 de dia de cada mês |Desde o primeiro dia para o último dia de cada mês do calendário |A moeda do país/região que seu cliente está localizado na. Isso significa que você receberá faturas separadas e arquivos de reconciliação na moeda do país/região cada cliente que você vendeu para no período de cobrança. |Sim |
