<a name="-head"></a><<<<<<< HEAD
---
title: Cenários comuns de cobrança | Descrição do Partner Center: Este tópico explica o que você deve esperar ver em sua fatura depois de adicionar novas assinaturas, ajustar o número de licenças em uma assinatura ou cancelar uma assinatura. As assinaturas baseadas em uso e em licença serão afetadas de forma diferente.
ms.assetid: E4BBD3E7-AFE2-4998-950D-0D27D1178160 author: MaggiePucciEvans Keywords: cobrança, pagamentos, pedidos, uso, cobrança baseada em licença, data de aniversário, período gratuito, vigência, cancelamento, renovação, fórmula de preço, arquivo de reconciliação, arquivo de reconhecimento
---

# <a name="common-billing-scenarios"></a>Cenários comuns de cobrança

**Aplicável a**

-  Partner Center
-  Partner Center for Microsoft Cloud for US Government
-  Partner Center do Microsoft Cloud Alemanha

Este tópico explica o que você deve esperar ver em sua fatura depois de adicionar novas assinaturas, ajustar o número de licenças de uma assinatura ou cancelar uma assinatura. As assinaturas baseadas em uso e em licença são afetadas de forma diferente.

## <a name="in-this-section"></a>Nesta seção

-   [Cobrança baseada em uso](#usagebased)

-   [Cobrança baseada em licença](#licensebased)

## <a href="" id="usagebased"></a>Cobrança baseada em uso

Você é cobrado somente pelos serviços usados no período de cobrança anterior. Quaisquer serviços ou aplicativos do Azure habilitados ou usados durante o período de cobrança aparecerão na fatura.

-   As taxas de serviço limitadas podem ser alteradas durante o ciclo de fatura.
    -   Aumentos de preço: é fornecido um aviso prévio de 30 dias.
    -   As reduções de preço são refletidas no dia em que elas entram em vigor.
    -   As assinaturas existentes são cobradas usando-se a taxa em vigor no início do ciclo de cobrança.
    -   As novas assinaturas (aqueles criadas durante o ciclo de cobrança) são cobradas com a taxa em vigor quando foram adicionadas.
-   Se você cancelar uma assinatura durante o primeiro ciclo de cobrança, as cobranças por uso aparecerão no arquivo de reconciliação pelo período em que a assinatura estava ativa.

## <a href="" id="licensebased"></a>Cobrança baseada em licença

**Cobrança:** assinaturas baseadas em licença são cobradas antecipadamente no dia de aniversário de assinatura.

**Dia de Aniversário:** assinaturas com cobrança mensal são alinhadas com a data de cobrança do parceiro e assinaturas com cobrança anual são alinhadas com a data da compra.

**Período Gratuito:** assinaturas com cobrança mensal recebem um período gratuito a partir da data de compra para a próxima data de cobrança do parceiro.

**Período:** todas as assinaturas baseadas em licença têm um período pago de 12 meses. O período pago começa na data da compra para assinaturas de cobranças anuais e na data de cobrança após a data da compra para assinaturas de cobranças mensais.

**Cancelamento:** as assinaturas canceladas nos primeiros 30 dias do período pago serão creditadas 100%. Assinaturas canceladas após 30 dias serão creditadas proporcionalmente.

**Renovação:** todas as assinaturas baseadas em licença serão renovadas automaticamente 12 meses após o período pago começar.

## <a href="" id="licensebasedmonthly"></a>Cenários de cobrança mensais

**Cenário 1: Nova assinatura**

Sua data de cobrança é no 15º dia de cada mês. Em 13 de janeiro, você compra uma nova assinatura com uma licença por US$4/mês e seleciona a cobrança mensal. Em 15 de janeiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/01/2018         | 14/01/2018   |Valor da Compra   |0,00       |1       |0,00    
|15/01/2018         |14/02/2018    |Taxa do ciclo   |4,00       |1        |4,00    

Em 15 de fevereiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|15/02/2018         |14/03/2018    |Taxa do ciclo   |4,00       |1        |4,00    
Você continuará sendo cobrado no dia 15 de cada mês até que a assinatura seja suspensa.

**Cenário 2: Alterar a quantidade de licença**

Sua data de cobrança é no 15º dia de cada mês. Em 13 de janeiro, você compra uma nova assinatura com uma licença por US$4/mês e seleciona a cobrança mensal. Em 15 de janeiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/01/2018         |14/01/2018    |Valor de compra   |0,00       |1        |0,00    
|15/01/2018         |14/02/2018    |Taxa do ciclo   |4,00       |1        |4,00    

Em 1º de fevereiro, você aumentará sua quantidade de licença de uma para duas. Em 15 de fevereiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 15/01/2018        |14/02/2018    |Proporcional à instância do ciclo   |-4,00       |1        |4,00    
|15/01/2018         |31/01/2018    | Proporcional à instância do ciclo   |2,21       |1        |2,21    
|01/02/2018         |14/02/2018    | Proporcional à instância do ciclo   |1,82       |2        |3,64    
|15/02/2018         |14/03/2018    | Proporcional à instância do ciclo   |4,00       |2        |8,00    

**Fórmulas do Preço Unitário:**

O preço mensal é de 4,00 e há 31 dias no período de serviço: 15/01/2018 – 14/02/2018. Isso equivale a um preço diário de 0,13 (4/31).

Há 17 dias no período proporcional de 15/01/2018 – 31/01/2018.

Preço unitário proporcional = 2,21 = 17 x 0,13

Há 14 dias no período proporcional de 01/02/2018 – 14/02/2018.

Preço unitário proporcional = 1,82 = 14 x 0,13

**Cenário 3: Suspender antes de 30 dias**

Sua data de cobrança é no 15º dia de cada mês. Em 13 de janeiro, você compra uma nova assinatura com uma licença por US$4/mês e seleciona a cobrança mensal. Em 15 de janeiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/01/2018         |14/01/2018    |Valor de compra   |0,00       |1        |0,00    
|15/01/2018         |14/02/2018    |Taxa do ciclo   |4,00       |1        |4,00    

Em 1º de fevereiro, você suspende a assinatura. Em 15 de fevereiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
15/01/2018|14/02/2018|Taxa de cancelamento|-4,00|1|4,00

**Cenário 4: Suspender depois de 30 dias**

Sua data de cobrança é no 15º dia de cada mês. Em 13 de janeiro, você compra uma nova assinatura com uma licença por US$4/mês e seleciona a cobrança mensal. Em 15 de janeiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|14/01/2018|Valor da Compra|0,00|1|0,00
15/01/2018|14/02/2018|Taxa do ciclo|4,00|1|4,00

Em 15 de fevereiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
15/02/2018|14/03/2018|Taxa do ciclo|4,00|1|4,00

Em 1º de março, você suspende a assinatura. Em 15 de março, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
01/03/2018|14/03/2018|Taxa de cancelamento|-1,96|1|-1,96

**Fórmulas do Preço Unitário:**

O preço mensal é de 4,00 e há 28 dias no período de serviço: 15/02/2018 – 14/03/2018. Isso equivale a um preço diário de 0,14 (4/28).

Preço unitário = dias no período de serviço x preço diário x número de licenças.

Há 14 dias no período de cancelamento de 01/03/2018 – 14/03/2018. 

Portanto, o preço unitário =-1,96 (14 x 0,14 x(-1)).

## <a name="annual-billing-scenarios"></a>Cenários de Cobrança Anual

**Cenário 1: Nova assinatura**

Sua data de cobrança é no 15º dia de cada mês. Em 13 de janeiro, você compra uma nova assinatura com uma licença por US$4/mês e seleciona a cobrança anual. Em 15 de janeiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Taxas proporcionais durante a compra|48,00|1|48,00

**Cenário 2: Alterar a quantidade de licença**

Sua data de cobrança é no 15º dia de cada mês. Em 13 de janeiro, você compra uma nova assinatura com uma licença por US$4/mês e seleciona a cobrança anual. Em 15 de janeiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Taxas proporcionais durante a compra|48,00|1|48,00

Em 1º de fevereiro, você aumentará sua quantidade de licença de uma para duas. Em 15 de fevereiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  | 
13/01/2018|12/01/2019|Proporcional à instância do ciclo|-48,00|1|-48,00
13/01/2018|31/01/2018|Proporcional à instância do ciclo|2,47|1|2,47
01/02/2018|12/01/2019|Proporcional à instância do ciclo|44,98|2|89,96

**Fórmulas do Preço Unitário:**

O preço anual é 48,00, que equivale ao preço diário de 0,13 (48,00/365).

Preço unitário = dias no período de serviço x preço diário x número de licenças.

Há dias 19 no período de serviço de 13/01/2018 – 31/01/2018. 

Portanto, o preço unitário = 2,47 (19 x 0,13 x 1)

Há dias 346 no período de serviço de 01/02/2018 – 12/01/2019. 

Portanto, o preço unitário = 44,98 (346 x 0,13 x 2)

**Cenário 3: Suspender antes de 30 dias**

Sua data de cobrança é no 15º dia de cada mês. Em 13 de janeiro, você compra uma nova assinatura com uma licença por US$4/mês e seleciona a cobrança anual. Em 15 de janeiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Taxas proporcionais durante a compra|48,00|1|48,00

Em 1º de fevereiro, você suspende sua assinatura. Em 15 de fevereiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Taxa de cancelamento|-48,00|1|-48,00

**Cenário 4: Suspender depois de 30 dias**

Sua data de cobrança é no 15º dia de cada mês. Em 13 de janeiro, você compra uma nova assinatura com uma licença por US$4/mês e seleciona a cobrança anual. Em 15 de janeiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Taxas proporcionais durante a compra|48,00|1|48,00

Em 15 de fevereiro, o arquivo de reconciliação baseado em licenças não conterá nenhuma linha de cobrança para essa assinatura.
Em 1º de março, você suspende sua assinatura. Em 15 de março, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
01/03/2018|12/01/2019|Taxa de cancelamento|-41,34|1|-41,34

**Fórmulas do Preço Unitário:**

O preço anual é 48,00, que equivale ao preço diário de 0,13 (48,00/365).

Preço unitário = dias no período de serviço x preço diário x número de licenças.

Há dias 318 no período de serviço de 01/03/2018 – 12/01/2019. 

Portanto, o preço unitário = 41,34 (318 x 0,13 x 1). Como isso é um crédito, o preço unitário é de -41,34.

**Cenário 5: Suspender e reativar**

Sua data de cobrança é no 15º dia de cada mês. Em 13 de janeiro, você compra uma nova assinatura com uma licença por US$4/mês e seleciona a cobrança anual. Em 15 de janeiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Taxas proporcionais durante a compra|48,00|1|48,00

Em 1º de fevereiro, você suspende sua assinatura. Em 15 de fevereiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Taxa de cancelamento|-48,00|1|-48,00

Em 1º de março, você reativa sua assinatura. Em 15 de março, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
01/03/2018|12/01/2019|Taxas proporcionais durante a compra|41,34|1|41,34

**Fórmulas do Preço Unitário:**

O preço anual é 48,00, que equivale ao preço diário de 0,13 (48,00/365).

Preço unitário = dias no período de serviço x preço diário x número de licenças.

Há dias 318 no período de serviço de 01/03/2018 – 12/01/2019. 

Portanto, o preço unitário = 41,34 (318 x 0,13 x 1).

<a name=""></a>=======
---
title: Cenários comuns de cobrança | Descrição do Partner Center: Este tópico explica o que você deve esperar ver em sua fatura depois de adicionar novas assinaturas, ajustar o número de licenças em uma assinatura ou cancelar uma assinatura. As assinaturas baseadas em uso e em licença serão afetadas de forma diferente.
ms.assetid: E4BBD3E7-AFE2-4998-950D-0D27D1178160 author: MaggiePucciEvans Keywords: cobrança, pagamentos, pedidos, uso, cobrança baseada em licença, data de aniversário, período gratuito, vigência, cancelamento, renovação, fórmula de preço, arquivo de reconciliação, arquivo de reconhecimento
---

# <a name="common-billing-scenarios"></a>Cenários comuns de cobrança

**Aplicável a**

-  Partner Center
-  Partner Center for Microsoft Cloud for US Government
-  Partner Center do Microsoft Cloud Alemanha

Este tópico explica o que você deve esperar ver em sua fatura depois de adicionar novas assinaturas, ajustar o número de licenças de uma assinatura ou cancelar uma assinatura. As assinaturas baseadas em uso e em licença são afetadas de forma diferente.

## <a name="in-this-section"></a>Nesta seção

-   [Cobrança baseada em uso](#usagebased)

-   [Cobrança baseada em licença](#licensebased)

## <a href="" id="usagebased"></a>Cobrança baseada em uso

Você é cobrado somente pelos serviços usados no período de cobrança anterior. Quaisquer serviços ou aplicativos do Azure habilitados ou usados durante o período de cobrança aparecerão na fatura.

-   As taxas de serviço limitadas podem ser alteradas durante o ciclo de fatura.
    -   Aumentos de preço: é fornecido um aviso prévio de 30 dias.
    -   As reduções de preço são refletidas no dia em que elas entram em vigor.
    -   As assinaturas existentes são cobradas usando-se a taxa em vigor no início do ciclo de cobrança.
    -   As novas assinaturas (aqueles criadas durante o ciclo de cobrança) são cobradas com a taxa em vigor quando foram adicionadas.
-   Se você cancelar uma assinatura durante o primeiro ciclo de cobrança, as cobranças por uso aparecerão no arquivo de reconciliação pelo período em que a assinatura estava ativa.

## <a href="" id="licensebased"></a>Cobrança baseada em licença

**Cobrança:** assinaturas baseadas em licença são cobradas antecipadamente no dia de aniversário de assinatura.

**Dia de Aniversário:** assinaturas com cobrança mensal são alinhadas com a data de cobrança do parceiro e assinaturas com cobrança anual são alinhadas com a data da compra.

**Período Gratuito:** assinaturas com cobrança mensal recebem um período gratuito a partir da data de compra para a próxima data de cobrança do parceiro.

**Período:** todas as assinaturas baseadas em licença têm um período pago de 12 meses. O período pago começa na data da compra para assinaturas de cobranças anuais e na data de cobrança após a data da compra para assinaturas de cobranças mensais.

**Cancelamento:** as assinaturas canceladas nos primeiros 30 dias do período pago serão creditadas 100%. Assinaturas canceladas após 30 dias serão creditadas proporcionalmente.

**Renovação:** todas as assinaturas baseadas em licença serão renovadas automaticamente 12 meses após o período pago começar.

## <a href="" id="licensebasedmonthly"></a>Cenários de cobrança mensais

**Cenário 1: Nova assinatura**

Sua data de cobrança é no 15º dia de cada mês. Em 13 de janeiro, você compra uma nova assinatura com uma licença por US$4/mês e seleciona a cobrança mensal. Em 15 de janeiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/01/2018         | 14/01/2018   |Valor da Compra   |0,00       |1       |0,00    
|15/01/2018         |14/02/2018    |Taxa do ciclo   |4,00       |1        |4,00    

Em 15 de fevereiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|15/02/2018         |14/03/2018    |Taxa do ciclo   |4,00       |1        |4,00    
Você continuará sendo cobrado no dia 15 de cada mês até que a assinatura seja suspensa.

**Cenário 2: Alterar a quantidade de licença**

Sua data de cobrança é no 15º dia de cada mês. Em 13 de janeiro, você compra uma nova assinatura com uma licença por US$4/mês e seleciona a cobrança mensal. Em 15 de janeiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/01/2018         |14/01/2018    |Valor de compra   |0,00       |1        |0,00    
|15/01/2018         |14/02/2018    |Taxa do ciclo   |4,00       |1        |4,00    

Em 1º de fevereiro, você aumentará sua quantidade de licença de uma para duas. Em 15 de fevereiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 15/01/2018        |14/02/2018    |Proporcional à instância do ciclo   |-4,00       |1        |4,00    
|15/01/2018         |31/01/2018    | Proporcional à instância do ciclo   |2,21       |1        |2,21    
|01/02/2018         |14/02/2018    | Proporcional à instância do ciclo   |1,82       |2        |3,64    
|15/02/2018         |14/03/2018    | Proporcional à instância do ciclo   |4,00       |2        |8,00    

**Fórmulas do Preço Unitário:**

O preço mensal é de 4,00 e há 31 dias no período de serviço: 15/01/2018 – 14/02/2018. Isso equivale a um preço diário de 0,13 (4/31).

Há 17 dias no período proporcional de 15/01/2018 – 31/01/2018.

Preço unitário proporcional = 2,21 = 17 x 0,13

Há 14 dias no período proporcional de 01/02/2018 – 14/02/2018.

Preço unitário proporcional = 1,82 = 14 x 0,13

**Cenário 3: Suspender antes de 30 dias**

Sua data de cobrança é no 15º dia de cada mês. Em 13 de janeiro, você compra uma nova assinatura com uma licença por US$4/mês e seleciona a cobrança mensal. Em 15 de janeiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/01/2018         |14/01/2018    |Valor de compra   |0,00       |1        |0,00    
|15/01/2018         |14/02/2018    |Taxa do ciclo   |4,00       |1        |4,00    

Em 1º de fevereiro, você suspende a assinatura. Em 15 de fevereiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
15/01/2018|14/02/2018|Taxa de cancelamento|-4,00|1|4,00

**Cenário 4: Suspender depois de 30 dias**

Sua data de cobrança é no 15º dia de cada mês. Em 13 de janeiro, você compra uma nova assinatura com uma licença por US$4/mês e seleciona a cobrança mensal. Em 15 de janeiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|14/01/2018|Valor da Compra|0,00|1|0,00
15/01/2018|14/02/2018|Taxa do ciclo|4,00|1|4,00

Em 15 de fevereiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
15/02/2018|14/03/2018|Taxa do ciclo|4,00|1|4,00

Em 1º de março, você suspende a assinatura. Em 15 de março, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
01/03/2018|14/03/2018|Taxa de cancelamento|-1,96|1|-1,96

**Fórmulas do Preço Unitário:**

O preço mensal é de 4,00 e há 28 dias no período de serviço: 15/02/2018 – 14/03/2018. Isso equivale a um preço diário de 0,14 (4/28).

Preço unitário = dias no período de serviço x preço diário x número de licenças.

Há 14 dias no período de cancelamento de 01/03/2018 – 14/03/2018. 

Portanto, o preço unitário =-1,96 (14 x 0,14 x(-1)).

## <a name="annual-billing-scenarios"></a>Cenários de Cobrança Anual

**Cenário 1: Nova assinatura**

Sua data de cobrança é no 15º dia de cada mês. Em 13 de janeiro, você compra uma nova assinatura com uma licença por US$4/mês e seleciona a cobrança anual. Em 15 de janeiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Taxas proporcionais durante a compra|48,00|1|48,00

**Cenário 2: adicionar uma licença após a data de aniversário da assinatura, mas antes da data de cobrança**

Você compra uma nova assinatura dia 11/02/17 com uma licença por US$211,20/ano. O aniversário da sua assinatura é definido como o dia 11 de cada mês. O sistema de cobrança da Microsoft cria as seguintes linhas de cobrança: 

-   Cobrança de US$211,20 pelo período de 11/02/17 a 10/02/18. 

Em 12/02/17, você compra uma segunda licença. Sua data de cobrança é 14/02/17. Os arquivos de fatura e reconciliação são gerados. O arquivo de reconciliação conterá as seguintes linhas de cobrança: 
|Data de Início da Cobrança  |Data de Término da Cobrança  |Tipo de Cobrança  |Preço unitário |Quantidade | Valor |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11/02/2017 |10/02/2018 |Taxas proporcionais na compra |211,20 |1 | 211,20 |
 
No aniversário da sua assinatura, 11/03/17, o sistema de cobrança da Microsoft cria as seguintes linhas de cobrança para o aumento de licença em 12/02/17: 
-   Crédito de -US$211,20 pelo período de 11/02/17 a 10/02/18. 
-   Cobrança proporcional por licença de US$0,58 por 1 licença pelo período de 11/02/17 a 11/02/17. 
-   Cobrança proporcional por licença de US$15,62 por 2 licenças pelo período de 12/02/17 a 10/03/17. 
-   Cobrança proporcional por licença de US$195,00 por 2 licenças pelo período de 11/03/2017 a 10/02/2018. 
 
Em 11/02/17, você compra um assinatura. Em 12/02/17, você adiciona uma licença. Sua data de cobrança é 14/02/17. Em 11/02/18, sua assinatura é renovada.

A próxima data de cobrança é 14/03/17, e os arquivos de fatura e reconciliação são gerados. O arquivo de reconciliação conterá as seguintes linhas de cobrança: 
|Data de Início da Cobrança  |Data de Término da Cobrança  |Tipo de Cobrança  |Preço unitário |Quantidade | Valor |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11/02/2017 |10/02/2018 |Proporcional à instância do ciclo |-211,20 |1 |-211,20 |
|11/02/2017 |11/02/2017 |Proporcional à instância do ciclo |0,58 |1 |0,58 |
|12/02/2017 |10/03/2017 |Proporcional à instância do ciclo |15,62 |2 |31,25 |
|11/03/2017 |10/02/2018 |Proporcional à instância do ciclo |195,00 |2 |390,00 |
 
Em 11/02/18, a assinatura será renovada por outro período de 12 meses.


**Cenário 3: Alterar a quantidade de licença**

Sua data de cobrança é no 15º dia de cada mês. Em 13 de janeiro, você compra uma nova assinatura com uma licença por US$4/mês e seleciona a cobrança anual. Em 15 de janeiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Taxas proporcionais durante a compra|48,00|1|48,00

Em 1º de fevereiro, você aumentará sua quantidade de licença de uma para duas. Em 15 de fevereiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  | 
13/01/2018|12/01/2019|Proporcional à instância do ciclo|-48,00|1|-48,00
13/01/2018|31/01/2018|Proporcional à instância do ciclo|2,47|1|2,47
01/02/2018|12/01/2019|Proporcional à instância do ciclo|44,98|2|89,96

**Fórmulas do Preço Unitário:**

O preço anual é 48,00, que equivale ao preço diário de 0,13 (48,00/365).

Preço unitário = dias no período de serviço x preço diário x número de licenças.

Há dias 19 no período de serviço de 13/01/2018 – 31/01/2018. 

Portanto, o preço unitário = 2,47 (19 x 0,13 x 1)

Há dias 346 no período de serviço de 01/02/2018 – 12/01/2019. 

Portanto, o preço unitário = 44,98 (346 x 0,13 x 2)

**Cenário 4: Suspender antes de 30 dias**

Sua data de cobrança é no 15º dia de cada mês. Em 13 de janeiro, você compra uma nova assinatura com uma licença por US$4/mês e seleciona a cobrança anual. Em 15 de janeiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Taxas proporcionais durante a compra|48,00|1|48,00

Em 1º de fevereiro, você suspende sua assinatura. Em 15 de fevereiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Taxa de cancelamento|-48,00|1|-48,00

**Cenário 5: Suspender depois de 30 dias**

Sua data de cobrança é no 15º dia de cada mês. Em 13 de janeiro, você compra uma nova assinatura com uma licença por US$4/mês e seleciona a cobrança anual. Em 15 de janeiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Taxas proporcionais durante a compra|48,00|1|48,00

Em 15 de fevereiro, o arquivo de reconciliação baseado em licenças não conterá nenhuma linha de cobrança para essa assinatura.
Em 1º de março, você suspende sua assinatura. Em 15 de março, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
01/03/2018|12/01/2019|Taxa de cancelamento|-41,34|1|-41,34

**Fórmulas do Preço Unitário:**

O preço anual é 48,00, que equivale ao preço diário de 0,13 (48,00/365).

Preço unitário = dias no período de serviço x preço diário x número de licenças.

Há dias 318 no período de serviço de 01/03/2018 – 12/01/2019. 

Portanto, o preço unitário = 41,34 (318 x 0,13 x 1). Como isso é um crédito, o preço unitário é de -41,34.

**Cenário 6: Suspender e reativar**

Sua data de cobrança é no 15º dia de cada mês. Em 13 de janeiro, você compra uma nova assinatura com uma licença por US$4/mês e seleciona a cobrança anual. Em 15 de janeiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Taxas proporcionais durante a compra|48,00|1|48,00

Em 1º de fevereiro, você suspende sua assinatura. Em 15 de fevereiro, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Taxa de cancelamento|-48,00|1|-48,00

Em 1º de março, você reativa sua assinatura. Em 15 de março, o arquivo de reconciliação baseado em licenças conterá as seguintes linhas de cobrança:
|Data de Início da Cobrança |Data de Término da Cobrança |Tipo de Cobrança |Preço unitário |Quantidade |Valor |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
01/03/2018|12/01/2019|Taxas proporcionais durante a compra|41,34|1|41,34

**Fórmulas do Preço Unitário:**

O preço anual é 48,00, que equivale ao preço diário de 0,13 (48,00/365).

Preço unitário = dias no período de serviço x preço diário x número de licenças.

Há dias 318 no período de serviço de 01/03/2018 – 12/01/2019. 

Portanto, o preço unitário = 41,34 (318 x 0,13 x 1).
>>>>>>> e10d68b8029ab91ddbfc67d278575a79639cf269
