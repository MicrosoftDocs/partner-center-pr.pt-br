---
title: Perguntas Frequentes sobre os novos recursos de cobrança | Partner Center
ms.topic: article
ms.date: 10/29/2018
Description: The following are frequently asked questions about Partner Center's annual billing and free trial features.
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
ms.localizationpriority: medium
ms.openlocfilehash: f0b26856d0fb18062591c2311ef18c68fbbd7498
ms.sourcegitcommit: 757c2e498334322862932068122665846f528b9c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2018
ms.locfileid: "7012599"
---
# <a name="faq-about-new-billing-features"></a>Perguntas Frequentes sobre os novos recursos de cobrança

**Aplicável a**

-  Partner Center
-  Partner Center for Microsoft Cloud for US Government
-  Partner Center for Microsoft Cloud Germany

Veja a seguir perguntas frequentes sobre os recursos de cobrança anual e avaliação gratuita do Partner Center. 

## <a name="in-this-section"></a>Nesta seção

-   [Perguntas frequentes sobre cobrança anual](#annualbillingfaq)

-   [Perguntas frequentes sobre avaliações gratuitas](#freetrialsfaq)

-   [Perguntas frequentes sobre alinhamento de cobrança](#billingalignmentfaq)


## <a href="" id="annualbillingfaq"></a>Perguntas frequentes sobre cobrança anual

Seções:

[Visão geral e benefícios da cobrança anual](#overviewandbenefits)

[Seu pedido e cenários de cobrança](#placingyourorder)

[Alteração da sua assinatura](#changingyoursubscription)

[Cálculo de preço](#pricingcalculation)

[Relatórios](#reporting)

[Incentivos](#incentives)


<a href="" id="overviewandbenefits"></a>**Visão geral e benefícios da cobrança anual**

**P:** O que mudou?

-   **R:** Em resposta às suas solicitações, introduzimos a opção de pagar por determinadas assinaturas CSP de forma anual ou mensal. Essa nova opção foi disponibilizada em 17 de outubro de 2017.

**P:** Quem pode participar?

-   **R:** Todos os parceiros e tipos de parceiro podem utilizar a cobrança anual. A Cobrança Anual está disponível em todos os mercados onde o CSP está disponível no momento. 

**P:** O que é necessário levar em consideração ao pensar em cobrança anual?    

-   **R:** Você deve considerar como o seu movimento de vendas será afetado. Aqui estão algumas dicas para ajudá-lo a usar efetivamente a cobrança anual. 
    - Atualize as APIs para se preparar para o recurso de cobrança anual, se aplicável. 
    - Examine as alterações feitas na fatura e no arquivo de reconciliação baseado em licença.
    - Informe a sua equipe.
    - Atualize seus processos internos conforme o necessário.

**P:** Quais são os benefícios da cobrança anual? 

-   **R:** A cobrança anual tem os seguintes benefícios:

    - Maior flexibilidade nas opções de pagamento.

    - Melhor alinhamento com o faturamento dos seus clientes.

    - Impacto reduzido nas flutuações de moeda.

    - Custos operacionais de cobrança reduzidos.

**P:** Quais ofertas terão a opção de cobrança anual?

-   **R:** A maioria das assinaturas baseadas em licença tem a opção de cobrança mensal ou anual. As assinaturas baseadas em uso só apresentam a opção de cobrança mensal. Você poderá identificar as frequências de cobrança disponíveis para cada oferta usando a coluna J da matriz de ofertas. Você pode encontrar a matriz de ofertas na seção 'Consulte as ofertas e os preços' no Partner Center. .

**P:** A cobrança anual é feita por assinatura ou por licença?       

-   **R:** As cobranças anual e mensal são feitas por assinatura.

**P:** Há alguma alteração necessária para que as APIs deem suporte à cobrança anual?    

-   **R:** Para aproveitar a cobrança anual, há algumas mudanças necessárias para suas APIs. Você pode encontrar informações mais detalhadas nos seguintes artigos:

    - https://partnercenter.microsoft.com/en-us/partner/developer

    - https://msdn.microsoft.com/en-us/library/partnercenter/microsoft.store.partnercenter.models.orders.order.billingcycle.aspx 

    - Código de exemplo: https://msdn.microsoft.com/en-us/library/partnercenter/mt634667.aspx 

<a href="" id="placingyourorder"></a>**Seu pedido e cenários de cobrança**

**P:** Haverá uma oferta exclusiva especificamente para pedidos com cobrança anual?   

-   **R:** Não. Todas as frequências de cobrança, incluindo a opção de cobrança anual, são atribuídas à Oferta como um atributo. Entretanto, você pode renomear uma oferta usando um nome de cliente mais amigável para permitir a diferenciação.

**P:** Como posso selecionar a cobrança anual?

-   **R:** Ao adicionar uma nova assinatura, você deverá escolher a frequência de cobrança. Você pode escolher a opção de cobrança anual nesse ponto. Assim que a cobrança anual for selecionada, todas as ofertas disponíveis serão exibidas.

**P:** Se eu escolher a cobrança anual, quando serei cobrado?    

-   **R:** Você será cobrado na próxima data de cobrança. Por exemplo, se a data de cobrança for o dia 1º e você comprar uma assinatura com cobrança anual no dia 29 de outubro de 2017, você será cobrado no dia 1º de novembro de 2017. Supondo que você não faça nenhuma alteração na licença, você será cobrado no dia 1º de novembro de 2018. Se você fizer uma alteração na licença, você receberá um crédito e uma nova cobrança na data de cobrança seguinte. 

**P:** Posso dividir uma assinatura de forma que uma parte seja cobrada mensalmente e a outra seja cobrada anualmente?  

-   **R:** Não. A assinatura inteira deve ter a mesma frequência de cobrança. A assinatura inteira deve ter uma cobrança mensal ou anual.

**P:** Quando é feita a renovação da assinatura com cobrança anual?     

-   **R:** A data de renovação será doze meses após a data de início do serviço. O período de serviço começa na data em que a assinatura é criada.  Por exemplo, uma assinatura criada em 10 de janeiro de 2018 será renovada em 10 de janeiro de 2019.

**P:** Quando serei cobrado pela renovação de uma assinatura com cobrança anual? 

-   **R:** Você será cobrado na próxima data de cobrança após a data de renovação da assinatura. Por exemplo, se você comprar uma assinatura com cobrança anual em 15 de janeiro de 2018 e se a sua data de cobrança for 20 de janeiro, sua assinatura será renovada em 15 de janeiro de 2019. Você será cobrado pela renovação em 20 de janeiro de 2019.

**P:** As assinaturas com cobrança anual recebem um período gratuito?

-   **R:** Não. As assinaturas com cobrança anual não recebem um período gratuito. O período pago de 12 meses começa na data da compra. Isso é diferente de assinaturas com frequência de cobrança mensal que recebem um período gratuito entre a data da compra e a próxima data de cobrança.

**P:** Um cliente pode ter várias assinaturas da mesma oferta e cada uma com frequências de cobrança diferentes?    

-   **R:** Depende da oferta. Há algumas ofertas restritas a uma assinatura por cliente. Se a oferta não estiver restrita, o cliente poderá ter várias assinaturas da mesma oferta com diferentes frequências de cobrança. Você pode encontrar os detalhes de todos os limites e restrições de oferta na coluna I da matriz de ofertas. Você pode encontrar a matriz de ofertas na seção 'Consulte as ofertas e os preços' no Partner Center.

<a href="" id="changingyoursubscription"></a>**Alteração da sua assinatura**

**P:** Posso adicionar uma nova licença a uma assinatura existente com cobrança anual?    

-   **R:** Sim. Você pode alterar a quantidade de licenças das suas assinaturas a qualquer momento. A adição de outras licenças não afetará a frequência de cobrança. 

**P:** Posso adicionar licenças com cobrança mensal a uma assinatura existente com cobrança anual? 

-   **R:** Assim que você comprar uma assinatura com cobrança anual, todas as licenças adicionais seguirão a mesma frequência de cobrança. Se então você precisar comprar licenças com cobrança mensal, precisará comprar uma nova assinatura.

**P:** É possível alternar a frequência de cobrança de uma assinatura de mensal para anual e vice-versa? 

-   **R:** Sim. Consulte **para alterar a frequência de cobrança de um serviço online** em [Noções básicas de cobrança](https://docs.microsoft.com/en-us/partner-center/billing-basics).

**P:** A cobrança anual está disponível para ofertas complementares?   

-   **R:** Sim. A assinatura complementar terá automaticamente a mesma frequência de cobrança da assinatura principal.

**P:** Como a cobrança anual funcionará quando eu adicionar ou remover licenças? 

-   **R:** Você pode adicionar ou remover licenças a qualquer momento. alteração Você receberá um crédito e será cobrado novamente proporcionalmente em sua próxima data de cobrança depois de alterar o número de licenças. 

**P:** O que acontece se eu cancelar uma assinatura com cobrança anual?    

-   **R:** A política de cancelamento é a mesma para todas as frequências de cobrança. Se a assinatura for cancelada nos 30 primeiros dias do período de 12 meses pago, você receberá um crédito de 100% em sua próxima data de cobrança. Se a assinatura for cancelada após 30 dias do período pago de 12 meses, você receberá um crédito pro-rata em sua próxima data de cobrança.

**P:** Um cliente pode mudar uma assinatura com cobrança anual de um parceiro para outro?  

-   **R:** Não. As assinaturas não podem ser movidas entre parceiros. O novo parceiro deve comprar uma nova assinatura em nome do cliente. Isso se aplica a assinaturas cobradas mensal e anualmente.

**P:** Posso reativar uma assinatura com cobrança anual?

-   **R:** Sim, você pode reativar a assinatura em até 90 dias a partir da data de suspensão. Você receberá uma cobrança proporcional na data de cobrança seguinte. A data de renovação da assinatura permanece a mesma.

<a href="" id="pricingcalculation"></a>**Cálculo de preço**

**P:** O que acontece se o preço de uma oferta for alterado durante o período de 12 meses de uma assinatura com cobrança anual?    

-   **R:** O preço da oferta no momento da compra é garantido pelo período de 12 meses da assinatura. 

**P:** Que preço terá uma assinatura quando ela for automaticamente renovada após um período de 12 meses de assinatura?    

-   **R:** Quando uma assinatura for renovada, o preço se baseará na lista de preços atual na data de renovação. O novo preço é garantido pelo próximo período de 12 meses de assinatura.

**P:** Como é calculado o crédito de uma licença ou assinatura cancelada? Ele é calculado pelo dia ou pelo mês?   

-   **R:** O crédito de cancelamento é calculado da seguinte maneira:

    - Crédito de cancelamento = ((preço mensal*12)/365) * dias restantes no período de 12 meses * número de licenças canceladas.

**P:** O que acontece se o preço de uma oferta diminuir durante o período de 12 meses de uma assinatura com cobrança anual? 

-   **R:** Não há alteração. O preço é definido para o período total de 12 meses. Isso também acontece com a cobrança mensal.


<a href="" id="reporting"></a>**Relatórios**

**P:** Onde posso descobrir se uma assinatura é cobrada anual ou mensalmente?   

-   **R:** O arquivo de reconciliação baseado em licença incluirá as informações sobre a frequência de cobrança. Você pode descobrir isso na coluna AA

**P:** Quais alterações eu verei no arquivo de reconciliação baseado em licença quando a assinatura com cobrança anual for adquirida ou renovada?  

-   **R:** A primeira alteração será uma nova linha no arquivo de reconciliação baseado em licença na data da primeira cobrança após a compra ou uma nova assinatura. ativado. Se nenhuma alteração for feita na assinatura, não haverá linhas nos arquivos de reconciliação para o segundo mês até o décimo-segundo do período da assinatura. a próxima alteração no arquivo de reconciliação aparecerá quando a assinatura for renovada. Isso será exibido na data da primeira cobrança após a renovação. Se for feita uma alteração na assinatura durante o período de 12 meses, um crédito e uma nova cobrança proporcional serão exibidos no próximo arquivo de reconciliação depois que a alteração for feita.

**P:** Como a compra, a alteração ou o cancelamento de uma assinatura anual aparecem na Coluna P dos arquivos de uso?

-   **R:** A cobrança inicial da compra é exibida como "Taxas proporcionais na compra". As alterações de licença que resultam em crédito e nova cobrança aparecem como "Proporcional à instância do ciclo". Os créditos de cancelamento aparecem como "Taxa de cancelamento".

**P:** Quando uma assinatura anual é cancelada, como ela aparece no arquivo de reconciliação?   

-   **R:** O arquivo de reconciliação conterá um item de linha referente a um crédito de cancelamento. Se o cancelamento ocorrer nos 30 primeiros dias do período de 12 meses, a assinatura será creditada em 100%. Se o cancelamento ocorrer após os 30 primeiros dias, a assinatura será creditada de forma proporcional.

**P:** Como isso será exibido no arquivo de reconciliação se as licenças forem adicionadas a uma assinatura com cobrança anual?  

-   **R:** O arquivo de reconciliação conterá um crédito e uma nova cobrança proporcional. Isso também acontecerá para uma assinatura com cobrança mensal.

**P:** Como isso será exibido no arquivo de reconciliação se as licenças forem removidas de uma assinatura com cobrança anual? 

-   **R:** O arquivo de reconciliação conterá um crédito e uma nova cobrança proporcional.  Isso também acontecerá para uma assinatura com cobrança mensal.

**P:** O preço anual é mostrado na lista de preços? 

-   **R:** Não. A lista de preços mostra o preço mensal. Você pode calcular o preço anual multiplicando o preço mensal por doze.

**P:** A matriz de ofertas tem entradas diferentes para ofertas que podem ser cobradas anualmente.?   

-   **R:** Não. As IDs da oferta são iguais para todas as frequências de cobrança. Não há IDs da oferta exclusivas para a cobrança anual.


<a href="" id="incentives"></a>**Incentivos**

**P:** Com que frequência os incentivos são calculados em assinaturas anuais? 

-   **R:** Nós calculamos sobre a receita cobrada. Os pagamentos de incentivos ganhos serão efetuados de acordo com nossa política encontrada em nossos guias de incentivos do CSP. 

**P:** Como são pagos os incentivos em assinaturas cobradas anualmente?  

-   **R:** Atualmente, todos os pagamentos de incentivos são feitos duas vezes por ano. Esses pagamentos são feitos 45 dias após o fim do semestre.

**P:** Quando uma assinatura cobrada anualmente for vendida, como a receita da assinatura será reconhecida para o cálculo de incentivos? Ele se baseará na receita cobrada ou ajustada? 

-   **R:** Os cálculos dos incentivos se baseiam na receita cobrada.

**P:**, Como são calculados os ganhos de incentivos sobre a assinatura cobrada anualmente qualificada entre as diversas taxas de incentivo do CSP (taxas de incentivo globais, taxas de acelerador local e campanhas locais)?

-   **R:** Independentemente da forma como uma assinatura é cobrada, se mensal ou anual, os parceiros ganham incentivos em todas as transações qualificadas. Isso inclui a taxa global de incentivos, aplicada à receita cobrada para o período, o acelerador local para todas as regiões em que existem aceleradores locais e todas as campanhas globais onde aplicável.

**P:** Quem você pode contatar se tiver dúvidas sobre incentivos?

-   **R:** Contate a equipe regional de suporte a incentivos apropriada:

    - América do Norte: ocina@microsoft.com

    - América Latina e Brasil: ocilatam@microsoft.com

    - EMEA: ociemea@microsoft.com

    - APOAC (exceto o Japão): ociapgc@microsoft.com

    - Japão: ocijp@microsoft.com


**P:** O que acontece se eu suspender minha assinatura? 

-   **R:** Se você suspender uma assinatura, seja no Partner Center ou via API, dentro de 30 dias da compra, você receberá um crédito de 100%, independentemente de frequência de cobrança. 

    Com a cobrança anual, isso seria parecido com:

    - O parceiro compra uma assinatura em 1º de janeiro = linha de cobrança criada para o período de serviço de 01/01 – 31/12.
    - Suspende a assinatura em 25 de janeiro = linha de cobrança de crédito criada para o período de serviço de 01/01 – 31/12.
    - Reativa em 29 de janeiro = linha de cobrança criada para o período de serviço de 01/01 – 31/12.

    Com a cobrança mensal, isso seria parecido com:

    - O parceiro compra uma assinatura em 1º de janeiro = linha de cobrança criada para o período de serviço de 01/01 – 31/01.
    - Suspende a assinatura em 25 de janeiro = linha de cobrança de crédito criada para o período de serviço de 01/01 – 31/01.
    - Reativa em 29 de janeiro = linha de cobrança criada para o período de serviço de 29/01 – 31/01.



## <a href="" id="freetrialsfaq"></a>Perguntas frequentes sobre avaliações gratuitas

**P1:** O que são avaliações gratuitas?

-   **R:** É possível oferecer a seus clientes uma avaliação gratuita de 30 dias de determinados produtos. Isso permite que seus clientes avaliem o produto antes de comprá-lo. As avaliações gratuitas estão disponíveis para os seguintes produtos: 

    - Office 365 Business Premium (a partir de 17 de outubro de 2017)
    - Office 365 E3 (a partir de 17 de outubro de 2017)
    - Office 365 E5 com PSTN (a partir de 17 de outubro de 2017)
    - Office 365 E5 sem PSTN (a partir de 17 de outubro de 2017)
    - Enterprise Mobility & Security E5 (a partir de 17 de outubro de 2017)
    - Dynamics 365 Customer Engagement Plan 1 (a partir de 17 de outubro de 2017)
    - Dynamics 365 for Financials (a partir de 17 de outubro de 2017)
    - Microsoft 365 Business (a partir de 1º de março de 2018)
    
**P2:** A cobrança anual e as avaliações gratuitas são diferentes em nuvem soberana em comparação a nuvem pública?

-   **R:** Não. São iguais. A única diferença serão nas SKUs de avaliação que estão disponíveis no momento da inicialização.

**P3:** Quem pode participar?

-   **R:** Todos os parceiros podem participar. No entanto, atualmente não está disponível na China. 

**P4:** Quais ações eu devo realizar para poder me beneficiar dessas avaliações gratuitas?

-   **R:** Considere a forma como a avaliação gratuita pode ser incorporada ao seu movimento de vendas e o impacto em seus processos internos. Talvez também seja necessário alterar suas APIs para acomodar a conversão de uma avaliação gratuita em uma assinatura paga. Há especificações técnicas detalhadas para as alterações de API na exibição Anúncios no Partner Center.

**P5:** Eu verei a avaliação gratuita em minha fatura e no arquivo de reconciliação?

-   **R:** Não, as avaliações gratuitas não aparecerão em sua fatura ou no arquivo de reconciliação baseado em licença. Elas aparecerão em sua fatura ou no arquivo de reconciliação baseado em licença depois que você converter uma avaliação gratuita em uma assinatura paga. A assinatura convertida aparecerá na sua fatura e no arquivo de reconciliação baseado em licença da mesma maneira que qualquer outra assinatura nova.

**P6:** As avaliações gratuitas afetam os incentivos?

-   **R:** Não. A versão de avaliação gratuita não tem impacto nos incentivos.

**P7:** As avaliações gratuitas estarão disponíveis para outros produtos do Office no futuro?

-   **R:** Nós fornecemos avaliações gratuitas para esses produtos porque eles são as ofertas de negócios mais abrangentes e populares. É possível que adicionemos outras ofertas de avaliação gratuita no futuro.

**P8:** Um cliente pode ter mais de uma versão de avaliação gratuita?

-   **R:** Cada cliente está qualificado para receber uma avaliação gratuita por oferta disponível.

**P9:** Há algum limite para uma avaliação gratuita?

-   **R:** Sim. A avaliação contempla até 25 licenças. A contagem de licenças não pode ser alterada durante o período de avaliação. Depois que a avaliação for convertida em uma assinatura paga, você poderá adicionar outras licenças à assinatura.

**P10:** A avaliação gratuita é automaticamente convertida em uma assinatura paga?

-   **R:** Não. Será necessário converter a assinatura por conta própria, no Partner Center ou por meio da API.

**P11:** As avaliações gratuitas podem ser usadas para assinaturas com cobrança mensal e anual?

-   **R:** Sim. Você poderá escolher a frequência de cobrança quando estiver convertendo a avaliação em uma assinatura paga.

**P12:** A data de início da assinatura se baseará na data inicial da avaliação gratuita ou na data de conversão em uma assinatura paga? 

-   **R:** A data de início se baseia na data de conversão. Se a avaliação gratuita for convertida em uma oferta paga com cobrança anual, a data de renovação da assinatura será de doze meses a partir da data de conversão. Se a avaliação gratuita for convertida em uma oferta paga com cobrança mensal, a data de renovação da assinatura será 12 meses a partir da data de cobrança após a data de conversão.

**P13:** Posso adicionar ou remover estações durante a avaliação gratuita?

-   **R:** Não. As avaliações gratuitas assumirão como padrão 25 licenças e não poderão ser atualizadas.

**P14:** Existem avaliações para ofertas de complementos, como ATP e PSTN?

-   **R:** No momento, não há nenhuma avaliação gratuita para ofertas de complementos.

**P15:** Posso fornecer uma avaliação gratuita para uma oferta que um cliente já possui?

-   **R:** Não. Se o cliente já tiver a oferta, ela não poderá ser usada em uma avaliação gratuita.

**P16:** Conseguirei ver todas as minhas ofertas de avaliação pendentes?

-   **R:** Sim. A página de cliente lista todas as assinaturas. Isso inclui as assinaturas de avaliação gratuita e as assinaturas pagas.

**P17:** Serei notificado sobre a expiração de avaliações gratuitas?

-   **R:** Não. Você pode acompanhar as datas de validade usando a exibição do cliente no Partner Center ou consultando a API. É recomendável monitorar essas datas com frequência para que você possa executar as ações de acompanhamento apropriadas quando os clientes tomarem uma decisão.

**P18:** Se um cliente teve uma avaliação gratuita para uma oferta, ele também poderá usar outra avaliação para uma oferta diferente? 

-   **R:** Sim. Os clientes podem se inscrever em uma avaliação por oferta. Por exemplo, eles podem obter uma avaliação gratuita do Office 365 Business Premium e uma avaliação gratuita do Office 365 E3.

**P19:** O que acontece quando a avaliação termina? Eu ou o meu cliente receberemos uma notificação? Quais notificações são exibidas quando tento entrar em uma avaliação expirada?

-   **R:** Depois que uma avaliação expira, o cliente que está tentando fazer login nessa avaliação verá uma mensagem indicando que a avaliação expirou. Não haverá notificações para sinalizar que uma avaliação está prestes a expirar; no entanto, como parceiro, você pode controlar isso por meio da exibição do cliente ou por meio de consultas de API.

**P20:** Uma avaliação pode ser estendida?

-   **R:** Não. Depois de 30 dias, a avaliação deverá ser convertida ou expirará.

**P21:** Quando uma avaliação expira, suas informações podem ser acessadas?

-   **R:** Sim. Os dados são armazenados em linha com os padrões de retenção de dados. Depois que você comprar uma nova assinatura com os mesmos planos de serviço, os dados do cliente poderão ser acessados da assinatura recém-ativada.

**P22:** Há avaliações gratuitas disponíveis para ofertas governamentais e educacionais?

-   **R:** Não há avaliações gratuitas para ofertas governamentais e educacionais no momento.

**P23:** As avaliações gratuitas do cliente para o programa CSP (Provedor de Soluções na Nuvem) podem ser convertidos em locatários de outros programas, como EA, Open ou MOSP? 

-   **R:** Não. As assinaturas não podem ser transferidas do CSP para outro programa.

**P24:** Como posso obter suporte para avaliações gratuitas? 

-   **R:** Envie uma solicitação de serviço por meio do Partner Center.

## <a href="" id="billingalignmentfaq"></a>Alinhamento de cobrança - encerramento do período gratuito

A partir do dia 21 de fevereiro de 2018, o Provedor de Soluções na Nuvem (CSP) começará a implementar o “alinhamento da data de cobrança” para novas assinaturas com cobrança mensal. Esse "alinhamento da data de cobrança" fornecerá aos parceiros mais flexibilidade e previsibilidade das vendas e da cobrança, bem como do provisionamento e do gerenciamento de assinaturas de clientes. 

**ATUALIZAÇÃO DO DIA 23 DE FEVEREIRO:** Anteriormente anunciamos uma data de implementação de 20 de fevereiro, mas nossa implementação real foi um pouco atrasada e escalonada por categoria de produto.  Analise o catálogo em destaque abaixo em relação à data de implementação por Categoria de Produto. 

|**Categoria do Produto**   |**Dia da Implementação**   |
|-----------------|:-------------|
|Office  |21 de fevereiro   |
|Windows, Minecraft   |22 de fevereiro   |
|Office 365 China   |23 de fevereiro   |
|Dynamics/Intune   |23 de fevereiro   |

As assinaturas adquiridas antes da data de implementação (consulte o catálogo em destaque acima) obtêm um período gratuito a partir da data da compra até a data de cobrança do parceiro. As assinaturas adquiridas após a data da implementação não receberão mais um período gratuito. O período pago de 12 meses será iniciado (alinhado) na data da compra em relação ao parceiro de cobrança. Os parceiros não verão mais uma 'linha de cobrança $0' que representa o período gratuito no arquivo de reconciliação. Não há nenhuma alteração nas APIs, no faturamento ou nos incentivos.  Os parceiros devem informar suas equipes de vendas e estatísticas sobre essa nova lógica de cobrança e garantir que as operações sejam ajustadas conforme o necessário.  

Antes de implementar o alinhamento da data de cobrança, nós faturamos e cobramos na data de aniversário de cobrança de um parceiro, a data em que o parceiro assinou o programa CSP, e não na data de aniversário da assinatura do cliente, a data em que o cliente comprou a assinatura. Após a data de implementação, os parceiros serão cobrados na data de aniversário da assinatura, eliminando esse período gratuito.  Os parceiros continuarão a receber as faturas em sua data de aniversário de cobrança, mas a data de efetivação da fatura será a data de aniversário de assinatura do cliente. 

As assinaturas que estiverem no período gratuito na data de implementação não serão cobradas entre a data da compra até a data de cobrança do parceiro. Além disso, eles não serão cobrados pelo primeiro mês do período pago de 12 meses. Se você usar um arquivo de reconciliação para verificação, lembre-se de que essa cobrança do primeiro mês não estará mais visível no arquivo de reconciliação.  

**P1:** O que está mudando com a data de cobrança?

-   **R:** As assinaturas baseadas em licença não terão mais um período gratuito. Atualmente, há um período gratuito da data da compra até a data de cobrança do parceiro.

**P2:** Quando o período gratuito será removido?

- **R:** A partir da data de implementação listada no catálogo em destaque acima, novas assinaturas não receberão um período gratuito.

|**Categoria do Produto**   |**Dia da Implementação**   |
|-----------------|:-------------|
|Office  |21 de fevereiro   |
|Windows, Minecraft   |22 de fevereiro   |
|Office 365 China   |23 de fevereiro   |
|Dynamics/Intune   |23 de fevereiro   |

**P3:** Como as assinaturas que estiverem no período gratuito na data de implementação serão afetadas?

- **R:** As assinaturas que estiverem no período gratuito na data de implementação ainda receberão um período gratuito da data da compra até a data de cobrança do parceiro. Essas licenças também receberão um "período gratuito estendido" e não serão cobradas pelo primeiro mês do período pago de 12 meses. O "período gratuito estendido" não será aplicável a licenças adicionadas no primeiro mês. Se aumentar a quantidade de licenças no primeiro mês, você será cobrado por essas licenças adicionadas na próxima fatura/reconciliação. Se o arquivo de reconciliação for usado para verificação, esteja ciente de que essa cobrança do primeiro mês poderá estar ausente do arquivo de reconciliação. Veja os cenários abaixo para obter uma explicação mais detalhada.

**P4:** Quando começará o período pago de 12 meses de uma nova assinatura?

- **R:** Atualmente, o período pago começa na data de cobrança do parceiro após a data da compra. A partir da data de implementação, o período pago de novas assinaturas começará na data da compra.

**P5:** Quando as assinaturas serão renovadas automaticamente?

- **R:** As assinaturas são renovadas automaticamente 12 meses após a data da primeira cobrança. Atualmente, isso significa que a renovação automática das assinaturas ocorrerá 12 meses após a primeira data de cobrança do parceiro seguinte à data da compra. A partir da data de implementação, as novas assinaturas serão renovadas automaticamente 12 meses após a data da compra.

**P6:** E se eu comprar a assinatura nos dias 29, 30 ou 31 de um mês?

- **R:** A assinatura estará disponível a partir da data da compra, mas o período pago de 12 meses não será iniciado até o primeiro dia do mês seguinte.

**P7:** Quais ofertas são afetadas?

- **R:** A remoção do período gratuito se aplica a todas as assinaturas baseadas em licença do CSP.

**P8:** Como isso afeta a fatura e o arquivo de reconciliação? 

- **R:** Você não verá mais a "linha de cobrança $0" na fatura ou no arquivo de reconciliação. Atualmente, a linha de cobrança $0 representa o período gratuito.

**P9:** A minha data de cobrança será alterada?

- **R:** Não, você continuará recebendo a fatura e o arquivo de reconciliação em sua data de cobrança existente.

**P10:** As datas de início/fim da cobrança mensal serão alteradas para as assinaturas existentes?

- **R:** Não, as datas de início/fim da cobrança mensal das assinaturas existentes continuarão alinhadas à sua data de cobrança. No entanto, as novas assinaturas serão alinhadas à data da compra. Veja exemplos abaixo.

**P11:** O cálculo de incentivos será alterado?

- **R:** Não, não haverá nenhuma alteração nos cálculos de incentivos.

**P12:** Haverá alguma alteração nas APIs?

- **R:** Não, não haverá nenhuma alteração nas APIs.

### <a name="common-scenarios"></a>Cenários comuns


|**Cenários**   |**Cenário 1: O período gratuito de assinatura termina antes da data de implementação**   |**Cenário 2: A assinatura está dentro do período gratuito na data da implementação**  | **Cenário 3: A assinatura foi adquirida na ou depois da data de implementação**   |
|----------|:------------|:--------------------|:------------|
|Data da compra |1º de fev. de 2018    | 1º de fev. de 2018    | 1º de junho de 2018     |
|Data do provisionamento | 1º de fev. de 2018   |1º de fev. de 2018   |1º de junho de 2018   |
|Data da cobrança   | Dia 15 de cada mês   |Dia 25 de cada mês   | Dia 15 de cada mês|
|Período gratuito   | 1º de fevereiro de 2018 - 14 de fevereiro de 2018|1º de fevereiro de 2018 - 24 de fevereiro de 2018   |Sem período gratuito|
|Cobrança do primeiro mês   | 15 de fevereiro de 2018 - 14 de março de 2018 | A quantidade de licenças em 24 de fevereiro de 2018 receberá um período gratuito estendido até 24 de março de 2018. As licenças adicionadas após 24 de fevereiro de 2018 serão cobradas. |1º de junho de 2018 - 30 de junho de 2018   |
|Cobrança do segundo mês   | 15 de março de 2018 - 14 de abril de 2018|25 de março de 2018 - 24 de abril de 2018   |1º de julho de 2018 - 31 de julho de 2018|
|Início do período pago   | 15 de fevereiro de 2018 | 25 de fevereiro de 2018| 1º de junho de 2018| 
|Fim do período pago | 14 de fevereiro de 2019   |24 de fevereiro de 2019   | 31 de maio de 2019  |
|Data da renovação | 15 de fevereiro de 2019 |25 de fevereiro de 2019   |1º de junho de 2019|

### <a name="scenario-4---new-purchase"></a>Cenário 4 - Nova compra

A data de cobrança do parceiro é no dia 15 do mês. Em 1º de junho de 2018, o parceiro compra uma nova assinatura. A assinatura custa US$ 30 por licença por mês. 

O arquivo de reconciliação de 15 de junho conterá somente as seguintes linhas de cobrança:

- Cobrança de US$ 30 pelo período de serviço de 1º de junho - 30 de junho

|**Início da cobrança**   |**Encerramento da cobrança**   |**Preço unitário**   |**Quantidade**   |**Valor**   |**Tipo de cobrança** |
|-----------------|:-------------|:----------------|:------------|:------|--------------|
|01/06/2018   |30/06/2018   |US$ 30   |1   |US$ 30   |Taxas proporcionais durante a compra |

### <a name="scenario-5a-suspend-and-reactivate-before-billing-date"></a>Cenário 5a: Suspensão e reativação antes da data de cobrança

A data de cobrança do parceiro é no dia 15 do mês. Em 1º de junho de 2018, o parceiro compra uma nova assinatura. A assinatura custa US$ 30 por licença por mês. Em 5 de junho de 2018, o parceiro suspende a assinatura. Em 10 de junho de 2018, o parceiro reativa a assinatura. O arquivo de reconciliação de 15 de junho conterá as seguintes linhas de cobrança:

- Cobrança de US$ 30 pelo período de serviço de 1º de junho – 30 de junho. 
- Crédito de cancelamento de -US$ 30 pelo período de serviço de 5 de junho - 30 de junho. O crédito não é proporcional porque a assinatura foi suspensa nos primeiros 30 dias. 
- Cobrança de US$ 30 pelo período de serviço de 10 de junho - 30 de junho. A cobrança não é proporcional porque a assinatura foi reativada nos primeiros 30 dias. 

|**Início da cobrança**   |**Encerramento da cobrança**   |**Preço unitário**   |**Quantidade**   |**Valor**   |**Tipo de cobrança** |
|-----------------|:-------------|:----------------|:------------|:------|:------ |--------|
|01/06/2018   |30/06/2018   |US$ 30   |1   |US$ 30   |Taxas proporcionais durante a compra |
|05/06/2018   |30/06/2018   |-US$ 30   |1   |US$ 30   |Taxa de cancelamento |
|10/06/2018   |30/06/2018   |US$ 30   |1   |US$ 30   |Taxa de ativação |

Observe que, quando uma assinatura é suspensa e reativada, a data de renovação automática permanecerá sendo 12 meses da data da compra original.

### <a name="scenario-5b-suspend-and-reactivate-after-billing-date-but-less-than-30-days-from-purchase-date"></a>Cenário 5b: Suspensão e reativação após a data de cobrança, mas com menos de 30 dias da data da compra

A data de cobrança do parceiro é no dia 15 do mês. Em 1º de junho de 2018, o parceiro compra uma nova assinatura. A assinatura custa US$ 30 por licença por mês. Em 20 de junho de 2018, o parceiro suspende a assinatura. Em 25 de junho de 2018, o parceiro reativa a assinatura. O arquivo de reconciliação de 15 de junho conterá as seguintes linhas de cobrança:

- Cobrança de US$ 30 pelo período de serviço de 1º de junho – 30 de junho. 

|**Início da cobrança**   |**Encerramento da cobrança**   |**Preço unitário**   |**Quantidade**   |**Valor**   |**Tipo de cobrança** |
|-----------------|:-------------|:----------------|:------------|:------|:------ |--------|
|01/06/2018   |30/06/2018   |US$ 30   |1   |US$ 30   |Taxas proporcionais durante a compra |

O arquivo de reconciliação de 15 de julho conterá as seguintes linhas de cobrança:
- Crédito de cancelamento de -US$ 30 pelo período de serviço de 20 de junho – 30 de junho. O crédito não é proporcional porque a assinatura foi suspensa nos primeiros 30 dias.
- Cobrança de US$ 30 pelo período de serviço de 25 de junho – 30 de junho. A cobrança não é proporcional porque a assinatura foi reativada nos primeiros 30 dias.
- Cobrança de US$ 30 pelo período de serviço de 1º de julho – 31 de julho.

|**Início da cobrança**   |**Encerramento da cobrança**   |**Preço unitário**   |**Quantidade**   |**Valor**   |**Tipo de cobrança** |
|-----------------|:-------------|:----------------|:------------|:------|:------ |--------|
|20/06/2018   |30/06/2018   |-US$ 30   |1   |-US$ 30   |Taxa de cancelamento |
|25/06/2018   |30/06/2018   |US$ 30   |1   |US$ 30   |Taxa de ativação |
|01/07/2018   |31/07/2018   |US$ 30   |1   |US$ 30   |Taxa do ciclo |

### <a name="scenario-5c-suspend-and-reactivate-different-license-quantity-after-billing-date-but-less-than-30-days-from-purchase-date"></a>Cenário 5c: Suspensão e reativação (quantidade de licenças diferente) após a data de cobrança, mas com menos de 30 dias da data da compra

A data de cobrança do parceiro é no dia 15 do mês. Em 1º de junho de 2018, o parceiro compra uma nova assinatura. A assinatura custa US$ 30 por licença por mês. Em 20 de junho de 2018, o parceiro suspende a assinatura. Em 25 de junho de 2018, o parceiro reativa a assinatura com duas licenças. O arquivo de reconciliação de 15 de junho conterá as seguintes linhas de cobrança:

- Cobrança de US$ 30 pelo período de serviço de 1º de junho – 30 de junho. 

|**Início da cobrança**   |**Encerramento da cobrança**   |**Preço unitário**   |**Quantidade**   |**Valor**   |**Tipo de cobrança** |
|-----------------|:-------------|:----------------|:------------|:------|:------ |--------|
|01/06/2018   |30/06/2018   |US$ 30   |1   |US$ 30   |Taxas proporcionais durante a compra |

O arquivo de reconciliação de 15 de julho conterá as seguintes linhas de cobrança:
- Crédito de cancelamento de -US$ 30 pelo período de serviço de 20 de junho – 30 de junho. O crédito não é proporcional porque a assinatura foi suspensa nos primeiros 30 dias.
- Cobrança de US$ 30 pelo período de serviço de 25 de junho – 30 de junho. A cobrança de reativação não é proporcional porque a assinatura foi reativada nos primeiros 30 dias. A cobrança também é baseada na quantidade de licenças originais de 1.
- Crédito de -US$ 6 pelo período de serviço de 25 de junho – 30 de junho. A cobrança de reativação só é feita por 1 licença durante o período de serviço de 25 de junho – 30 de junho quando você tinha 2 licenças. O crédito de -US$ 6 reverte a cobrança incorreta pelo período de serviço de 25 de junho – 30 de junho.
- Nova cobrança proporcional de US$ 12 pelo período de serviço de 25 de junho – 30 de junho. O parceiro tinha 2 licenças durante esse período de serviço. O preço unitário é calculado como (30/30)*6*2 = US$ 12.
- Cobrança de US$ 60 pelo período de serviço de 1º de julho – 31 de julho.

|**Início da cobrança**   |**Encerramento da cobrança**   |**Preço unitário**   |**Quantidade**   |**Valor**   |**Tipo de cobrança** |
|-----------------|:-------------|:----------------|:------------|:------|:------ |--------|
|20/06/2018   |30/06/2018   |-US$ 30   |1   |-US$ 30   |Taxa de cancelamento |
|25/06/2018   |30/06/2018   |US$ 30   |1   |US$ 30   |Taxa de ativação |
|25/06/2018   |30/06/2018   |-US$ 6   |1   |-US$ 6   |Proporcional à instância do ciclo |
|25/06/2018   |30/06/2018   |US$ 6   |2   |US$ 12   |Proporcional à instância do ciclo |
|01/07/2018   |31/07/2018   |US$ 30   |2   |US$ 60   |Taxa do ciclo |

### <a name="scenario-6-subscription-suspension-less-than-30-days-after-purchase-and-reactivation-more-than-30-days-after-purchase"></a>Cenário 6: Suspensão da assinatura com menos de 30 dias após a compra e reativação com mais de 30 dias após a compra 

A data de cobrança do parceiro é no dia 15 do mês. Em 1º de junho, o parceiro compra uma nova assinatura de uma licença por US$ 30 por mês. Em 5 de junho, o parceiro suspende a assinatura. O arquivo de reconciliação de 15 de junho conterá as seguintes linhas de cobrança:

- Cobrança de US$ 30 pelo período de serviço de 1º de junho - 30 de junho
- Crédito de cancelamento de -US$ 30 pelo período de serviço de 5 de junho - 30 de junho. O crédito não é proporcional porque a assinatura foi suspensa nos primeiros 30 dias.

|**Início da cobrança**   |**Encerramento da cobrança**   |**Preço unitário**   |**Quantidade**   |**Valor**   |**Tipo de cobrança** |
|-----------------|:-------------|:----------------|:------------|:------|---------|
|01/06/2018   |30/06/2018   |US$ 30   |1   |US$ 30   |Taxas proporcionais durante a compra
|05/06/2018   |30/06/2018   |-US$ 30   |1   |-US$ 30   |Taxa de cancelamento

Em 10 de julho, o parceiro reativa a assinatura. O arquivo de reconciliação de 15 de julho conterá as seguintes linhas de cobrança:

- Cobrança de reativação de US$ 21,30 pelo período de serviço de 10 de julho - 31 de julho. Reativações após 30 dias da data da compra resultam em uma cobrança proporcional. 

|**Início da cobrança**   |**Encerramento da cobrança**   |**Preço unitário**   |**Quantidade**   |**Valor**   |**Tipo de cobrança** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|10/07/2018   |31/07/2018   |US$ 21,30   |1   |US$ 21,30   |Taxa de ativação |

O arquivo de reconciliação de 15 de agosto conterá as seguintes linhas de cobrança:
- Cobrança de US$ 30 pelo período de serviço de 1º de agosto – 31 de agosto.

|**Início da cobrança**   |**Encerramento da cobrança**   |**Preço unitário**   |**Quantidade**   |**Valor**   |**Tipo de cobrança** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|01/08/2018   |31/08/2018   |US$ 30   |1   |US$ 30   |Taxa do ciclo |

Observe que, quando uma assinatura é suspensa e reativada, a data de renovação automática permanecerá sendo 12 meses da data da compra original. 

### <a name="scenario-7-subscription-suspension-and-reactivation-more-than-30-days-after-purchase"></a>Cenário 7: Suspensão e reativação da assinatura com mais de 30 dias após a compra 
A data de cobrança do parceiro é no dia 15 do mês. Em 1º de junho, o parceiro compra uma nova assinatura de uma licença por US$ 30 por mês. 

O arquivo de reconciliação de 15 de junho conterá somente as seguintes linhas de cobrança:

- Cobrança de US$ 30 pelo período de serviço de 1º de junho – 30 de junho.

|**Início da cobrança**   |**Encerramento da cobrança**   |**Preço unitário**   |**Quantidade**   |**Valor**   |**Tipo de cobrança** |
|-----------------|:-------------|:----------------|:------------|:------|---------|
|01/06/2018   |30/06/2018   |US$ 30   |1   |US$ 30   |Taxas proporcionais durante a compra |

O parceiro suspende a assinatura em 5 de julho, mas a reativa em 15 de julho. O arquivo de reconciliação de 15 de julho conterá as seguintes linhas de cobrança:

- Cobrança de US$ 30 pelo período de serviço de 1º de julho - 31 de julho.
- Crédito de cancelamento de -US$ 26,14 pelo período de serviço de 5 de julho – 31 de julho. Cancelamentos após 30 dias da data da compra resultam em um crédito proporcional. Cálculo = (preço mensal/dias no período de serviço total) x dias no período de serviço proporcional x quantidade de licenças x (-1) = (30/31) x 27 x 1 x (-1) = -26,14.
- Cobrança de reativação de US$ 21,30 pelo período de serviço de 10 de julho - 31 de julho. Reativações após 30 dias da data da compra resultam em uma cobrança proporcional. Cálculo = (30/31) x 22 x 1 = 21,30.

|**Início da cobrança**   |**Encerramento da cobrança**   |**Preço unitário**   |**Quantidade**   |**Valor**   |**Tipo de cobrança** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|01/07/2018   |31/07/2018   |US$ 30  |1   |US$ 30   |Taxa do ciclo |
|05/07/2018   |31/07/2018   |   -US$ 26,14   |1   |-US$ 26,14|Taxa de cancelamento |
|10/07/2018   |31/07/2018   |-US$ 21,30   |1   |US$ 21,30|Taxa de ativação |

O arquivo de reconciliação de 15 de agosto conterá o seguinte:
- Cobrança de US$ 30 pelo período de serviço de 1º de agosto – 31 de agosto.

|**Início da cobrança**   |**Encerramento da cobrança**   |**Preço unitário**   |**Quantidade**   |**Valor**   |**Tipo de cobrança** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|01/08/2018   |31/08/2018   |US$ 30  |1   |US$ 30   |Taxa do ciclo |

### <a name="scenario-8-change-of-license-quantity"></a>Cenário 8: Alteração na quantidade de licenças 

A data de cobrança do parceiro é no dia 15. Em 1º de junho, o parceiro compra uma nova assinatura por US$ 30 por mês. Em 10 de junho, o parceiro aumenta a quantidade de licenças de uma para duas licenças. O arquivo de reconciliação de 15 de junho conterá as seguintes linhas de cobrança:

- Cobrança de US$ 30 pelo período de serviço de 1º de junho – 30 de junho. Mesmo que o parceiro tenha aumentado a quantidade de licenças antes da data de cobrança de 15 de junho, o sistema de cobrança da Microsoft não reconhece a alteração até o dia de aniversário da assinatura, em 1º de julho.

|**Início da cobrança**   |**Encerramento da cobrança**   |**Preço unitário**   |**Quantidade**   |**Valor**   |**Tipo de cobrança** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|01/06/2018   |30/06/2018   |US$ 30   |1   |US$ 30   |Taxas proporcionais durante a compra |

Em 1º de julho, o dia do aniversário da assinatura, o sistema de cobrança da Microsoft reconhecerá que a quantidade de licenças foi alterada de uma para duas em 10 de junho. O sistema de cobrança gerará um crédito e novas cobranças proporcionais para o período de serviço de 1º de junho - 9 de junho e 10 de junho - 30 de junho. 

O arquivo de reconciliação de 15 de julho conterá o seguinte:

- Crédito de -US$ 30 pelo período de serviço de 1º de junho - 30 de junho.
- Nova cobrança proporcional de US$ 9 pelo período de serviço de 1º de junho – 9 de junho. Nesse período o cliente tinha 1 licença. Cálculo = (preço mensal/total de dias no período de serviço) x dias no período de serviço proporcional x número de licenças = (30/30) x 9 x 1 = 9.
- Nova cobrança proporcional de US$ 42 pelo período de serviço de 10 de junho - 30 de junho. Nesse período o cliente tinha 2 licenças. Cálculo = (30/30) x 21 x 2 = 42.
- Cobrança de US$ 60 pelo período de serviço de 1º de julho – 31 de julho.

|**Início da cobrança**   |**Encerramento da cobrança**   |**Preço unitário**   |**Quantidade**   |**Valor**   |**Tipo de cobrança** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|01/06/2018   |30/06/2018   |-US$ 30   |1   |-US$ 30|Proporcional à instância do ciclo |
|01/06/2018   |09/06/2018   |US$ 9   |1   |US$ 9|Proporcional à instância do ciclo |
|10/06/2018   |30/06/2018   |US$ 21   |2   |US$ 42|Proporcional à instância do ciclo |
|01/07/2018   |31/07/2018   |US$ 30   |2   |US$ 60   |Taxa do ciclo |

### <a name="scenario-9-add-on-subscriptions"></a>Cenário 9: Assinaturas de complementos

A data de cobrança do parceiro é no dia 15 do mês. Em 1º de junho, o parceiro compra uma nova assinatura de uma licença por US$ 30 por mês. Em 10 de junho, o parceiro compra uma nova assinatura de complemento por US$ 5 por mês. A data de renovação da assinatura de complemento será alinhada à data de renovação da assinatura base, que é 1º de junho. 

Em 10 de junho, o parceiro compra uma assinatura de complemento de uma licença por US$ 5 por mês. 

O arquivo de reconciliação de 15 de junho conterá as seguintes linhas de cobrança:

- Cobrança de US$ 30 pelo período de serviço de 1º de junho – 30 de junho. Isso é para a assinatura base.
- Cobrança proporcional de US$ 3,50 pelo período de serviço de 10 de junho – 30 de junho. Isso é para a assinatura de complemento. 

|**Início da cobrança**   |**Encerramento da cobrança**   |**Preço unitário**   |**Quantidade**   |**Valor**   |**Tipo de cobrança** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|01/06/2018   |30/06/2018   |US$ 30   |1   |US$ 30   |Taxas proporcionais durante a compra |
|10/06/2018   |30/06/2018   |$3,50   |1   |$3,50   |Taxas proporcionais durante a compra |

O arquivo de reconciliação de 15 de julho conterá as seguintes linhas de cobrança:

- Cobrança de US$ 30 pelo período de serviço de 1º de julho – 31 de julho. Isso é para a assinatura base.
- Cobrança de US$ 5 pelo período de serviço de 1º de julho – 31 de julho. Isso é para a assinatura de complemento.

|**Início da cobrança**   |**Encerramento da cobrança**   |**Preço unitário**   |**Quantidade**   |**Valor**   |**Tipo de cobrança** |
|-----------------|:-------------|:----------------|:------------|:------|-------|
|01/07/2018   |31/07/2018   |US$ 30   |1   |US$ 30   |Taxa do ciclo |
|01/07/2018   |31/07/2018   |US$ 5   |1   |US$ 5   |Taxa do ciclo |

Observe que a data de renovação automática da assinatura de complemento será 1º de junho de 2019, que se alinha à assinatura base.

### <a name="scenario-10-new-purchase-on-the-29th-30th-or-31st"></a>Cenário 10: Nova compra nos dias 29, 30 ou 31 

A data de cobrança do parceiro é no dia 15 do mês. Em 29 de maio, o parceiro compra uma nova assinatura de uma licença por US$ 30 por mês. As assinaturas compradas nos dias 29, 30 ou 31 terão um período gratuito da data da compra até o dia 1º do mês seguinte. O aniversário da assinatura padrão será no dia 1º. Nesse cenário, a assinatura receberá um período gratuito de 29 de maio até 31 de maio, e o período pago de 12 meses começará em 1º de junho. 

O arquivo de reconciliação de 15 de junho conterá as seguintes linhas de cobrança:

- Cobrança de US$ 30 pelo período de serviço de 1º de junho - 30 de junho.

|**Início da cobrança**   |**Encerramento da cobrança**   |**Preço unitário**   |**Quantidade**   |**Valor**   |**Tipo de cobrança** |
|-----------------|:-------------|:----------------|:------------|:------|------|
|29/05/2018   | 30/06/2018   |US$ 30   |1   |US$ 30  |Taxas proporcionais durante a compra |

Observe que a assinatura será renovada automaticamente em 1º de junho de 2019.
