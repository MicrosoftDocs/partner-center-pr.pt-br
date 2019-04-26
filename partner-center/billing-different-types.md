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
ms.openlocfilehash: 4b2b42c0d9bbb2654bbd486f987e3d5da9c562a2
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2019
ms.locfileid: "62135376"
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
