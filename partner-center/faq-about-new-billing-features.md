---
title: "Perguntas Frequentes sobre os novos recursos de cobrança | Partner Center"
Description: The following are frequently asked questions about Partner Center's annual billing and free trial features.
ms.assetid: 
author: MaggiePucciEvans
ms.openlocfilehash: ddd10efe487effdd2571869f2a4231118f946b8b
ms.sourcegitcommit: 4b697e2e18426edc95b9165f380b784bb10937ed
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/20/2017
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

    - https://partnercenter.microsoft.com/pt-br/partner/developer

    - https://msdn.microsoft.com/pt-br/library/partnercenter/microsoft.store.partnercenter.models.orders.order.billingcycle.aspx 

    - Código de exemplo: https://msdn.microsoft.com/en-us/library/partnercenter/mt634667.aspx 

<a href="" id="placingyourorder"></a>**Seu pedido e cenários de cobrança**

**P:** Haverá uma oferta exclusiva especificamente para pedidos com cobrança anual?   

-   **R:** Não. Todas as frequências de cobrança, incluindo a opção de cobrança anual, são atribuídas à Oferta como um atributo. Entretanto, você pode renomear uma oferta usando um nome de cliente mais amigável para permitir a diferenciação.

**P:** Como posso selecionar a cobrança anual?

-   **R:** Ao adicionar uma nova assinatura, você deverá escolher a frequência de cobrança. Você pode escolher a opção de cobrança anual nesse ponto. Assim que a cobrança anual for selecionada, todas as ofertas disponíveis serão exibidas.

**P:** Se eu escolher a cobrança anual, quando serei faturado?    

-   **R:** Você será cobrado na seguinte data de cobrança. Por exemplo, se a sua data de cobrança for 1º de fevereiro, você sempre será cobrado em 1º de fevereiro. Portanto, se você comprar uma assinatura com cobrança anual em 29 de outubro de 2017 ou em 15 de janeiro de 2018, será cobrado pela assinatura anual de 1º de fevereiro de 2018 em ambos os casos. 

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

**P:**Posso adicionar licenças com cobrança mensal a uma assinatura existente com cobrança anual? 

-   **R:** Assim que você comprar uma assinatura com cobrança anual, todas as licenças adicionais seguirão a mesma frequência de cobrança. Se então você precisar comprar licenças com cobrança mensal, precisará comprar uma nova assinatura.

**P:** É possível alternar a frequência de cobrança de uma assinatura de mensal para anual e vice-versa? 

-   **R:** Não. Depois de selecionar a frequência de cobrança, você não poderá alterá-la 

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

**P:** O que são avaliações gratuitas?

-   **R:** É possível oferecer a seus clientes uma avaliação gratuita de 30 dias de determinados produtos. Isso permite que seus clientes avaliem o produto antes de comprá-lo. As avaliações gratuitas estão disponíveis para os seguintes produtos: 

    - Office 365 Business Premium  
    - Office 365 E3  
    - Office 365 E5 com PSTN  
    - Office 365 E5 sem PSTN  
    - Enterprise Mobility & Security E5  
    - Dynamics 365 Customer Engagement Plan 1  
    - Dynamics 365 for Financials  
    
**P:** O período gratuito está sendo eliminado com a entrega de avaliações gratuitas?

-   **R:** Não, as assinaturas com cobrança mensal continuarão tendo um período gratuito. No entanto, não haverá nenhum período gratuito para cobrança anual.

**P:** O alinhamento de cobrança foi adiado até CY18 Q1. Como isso afeta o período gratuito e a cobrança em geral?

-   **R:** Novas assinaturas com cobrança mensal continuarão recebendo um período gratuito e sendo alinhadas à data de cobrança do parceiro. As assinaturas com cobrança anual não oferecerão um período gratuito e serão alinhadas com a data de compra. Os parceiros continuarão recebendo seus arquivos de reconciliação e fatura na data de cobrança mensal, o que conterá a atividade de cobrança tanto para assinaturas mensais quanto anuais.

**P:** Quando o período gratuito será removido para assinaturas com frequência de cobrança mensal?

-   **A:** CY18 Q1.

**P:** A cobrança anual e as avaliações gratuitas são diferentes em nuvem soberana versus nuvem pública?

-   **R:** Não. São iguais. A única diferença serão nas SKUs de avaliação que estão disponíveis no momento da inicialização.

**P:** Quando isso estará disponível para as SKUs listadas acima?

-   **R:** 17 de outubro de 2017.

**P:** Quem pode participar?

-   **R:** Todos os parceiros podem participar. No entanto, isso não está disponível na China no momento. As avaliações gratuitas estarão disponíveis para clientes e parceiros chineses antes do final de 2017. 

**P:** Quais ações eu devo realizar para poder me beneficiar dessas avaliações gratuitas??

-   **R:** Considere a forma como a avaliação gratuita pode ser incorporada ao seu movimento de vendas e o impacto em seus processos internos. Talvez também seja necessário alterar suas APIs para acomodar a conversão de uma avaliação gratuita em uma assinatura paga. Há especificações técnicas detalhadas para as alterações de API na exibição Anúncios no Partner Center.

**P:** Eu verei a avaliação gratuita em minha fatura e no arquivo de reconciliação?

-   **R:** Não, as avaliações gratuitas não aparecerão em sua fatura ou no arquivo de reconciliação baseado em licença. Elas aparecerão em sua fatura ou no arquivo de reconciliação baseado em licença depois que você converter uma avaliação gratuita em uma assinatura paga. A assinatura convertida aparecerá na sua fatura e no arquivo de reconciliação baseado em licença da mesma maneira do que qualquer outra assinatura nova. 

**P:** As avaliações gratuitas afetam os incentivos?

-   **R:** Não. A versão de avaliação gratuita não tem impacto nos incentivos.

**P:** As avaliações gratuitas estarão disponíveis para outros produtos do Office e CSP no futuro?

-   **R:** Ainda não sabemos. Nós fornecemos avaliações gratuitas para esses produtos porque eles são as ofertas de negócios mais abrangentes e populares. É possível que adicionemos outras ofertas de avaliação gratuita no futuro.

**P:** Um cliente pode ter mais de uma versão de avaliação gratuita?

-   **R:** Cada cliente está qualificado para uma avaliação gratuita por oferta disponível.

**P:** Há algum limite para uma avaliação gratuita?

-   **R:** Sim. A avaliação contempla até 25 licenças. A contagem de licenças não pode ser alterada durante o período de avaliação. Depois que a avaliação for convertida em uma assinatura paga, você poderá adicionar outras licenças à assinatura.

**P:** A avaliação gratuita é automaticamente convertida em uma assinatura paga?

-   **R:** Não. Será necessário converter a assinatura por conta própria, no Partner Center ou por meio da API.

**P:** As avaliações gratuitas podem ser usadas para assinaturas com cobrança mensal e anual?

-   **R:** Sim. Você poderá escolher a frequência de cobrança quando estiver convertendo a avaliação em uma assinatura paga.

**P:** A data de início da assinatura se baseará na data inicial da avaliação gratuita ou na data de conversão em uma assinatura paga? 

-   **R:** A data de início se baseia na data de conversão. Se a avaliação gratuita for convertida em uma oferta paga com cobrança anual, a data de renovação da assinatura será de doze meses a partir da data de conversão. Se a avaliação gratuita for convertida em uma oferta paga com cobrança mensal, a data de renovação da assinatura será 12 meses a partir da data de cobrança após a data de conversão.

**P:** Posso adicionar ou remover estações durante a avaliação gratuita?

-   **R:** Não. As avaliações gratuitas assumirão como padrão 25 licenças e não poderão ser atualizadas.

**P:** Existem avaliações para ofertas de complementos, como ATP e PSTN?

-   **R:** Não há nenhuma avaliação gratuita para ofertas de complementos.

**P:** Posso fornecer uma avaliação gratuita para uma oferta que um cliente já possui?

-   **R:** Não. Se o cliente já tiver a oferta, ela não poderá ser usada em uma avaliação gratuita.

**P:** Conseguirei ver todas as minhas ofertas de avaliação pendentes?

-   **R:** Sim. A página de cliente lista todas as assinaturas. Isso inclui as assinaturas de avaliação gratuita e as assinaturas pagas.

**P:** Serei notificado sobre a expiração de avaliações gratuitas?

-   **R:** Não. Você pode acompanhar as datas de validade usando a exibição do cliente no Partner Center ou consultando a API. É recomendável monitorar essas datas com frequência para que você possa executar as ações de acompanhamento apropriadas quando os clientes tomarem uma decisão.

**P:** Se um cliente teve uma avaliação gratuita para uma oferta, ele também poderá usar outra avaliação para uma oferta diferente? 

-   **R:** Sim. Os clientes podem se inscrever em uma avaliação por oferta. Por exemplo, eles podem obter uma avaliação gratuita do Office 365 Business Premium e uma avaliação gratuita do Office 365 E3.

**P:** O que acontece quando a avaliação termina? Eu ou o meu cliente receberemos uma notificação? Quais notificações são exibidas quando tento entrar em uma avaliação expirada?

-   **R:** Depois que uma avaliação expira, o cliente que está tentando fazer login nessa avaliação verá uma mensagem indicando que a avaliação expirou. Não haverá notificações para sinalizar que uma avaliação está prestes a expirar; no entanto, como parceiro, você pode controlar isso por meio da exibição do cliente ou por meio de consultas de API.

**P:** Uma avaliação pode ser estendida?

-   **R:** Não. Depois de 30 dias, a avaliação deverá ser convertida ou expirará.

**P:** Quando uma avaliação expira, suas informações podem ser acessadas?

-   **R:** Sim. Os dados são armazenados em linha com os padrões de retenção de dados. Depois que você comprar uma nova assinatura com os mesmos planos de serviço, os dados poderão ser acessados da assinatura recém-ativada.

**P:** Há avaliações gratuitas disponíveis para ofertas governamentais e educacionais?

-   **R:** Não há avaliações gratuitas para ofertas governamentais e educacionais neste momento.

**P:** As avaliações gratuitas do cliente para o programa CSP (Provedor de Soluções na Nuvem) podem ser convertidos em locatários de outros programas, como EA, Open ou MOSP? 

-   **R:** Não. As assinaturas não podem ser transferidas do CSP para outro programa.

**P:** Como posso obter suporte para avaliações gratuitas? 

-   **R:** Envie uma solicitação de serviço por meio do Partner Center.

## <a href="" id="billingalignmentfaq"></a>Alinhamento de cobrança - encerramento do período gratuito

Em 20 de fevereiro, o Programa CSP implementará o "alinhamento da data de cobrança" para novas assinaturas com frequência de cobrança mensal. Esse "alinhamento da data de cobrança" fornecerá aos parceiros mais flexibilidade e previsibilidade das vendas e da cobrança, bem como do provisionamento e do gerenciamento de assinaturas de clientes. As assinaturas adquiridas antes de 20 de fevereiro obtêm um período gratuito a partir da data da compra até a data de cobrança do parceiro. As assinaturas adquiridas depois de 20 de fevereiro não receberão mais um período gratuito. O período pago de 12 meses será iniciado (alinhado) na data da compra versus a cobrança do parceiro. Os parceiros não verão mais uma 'linha de cobrança $0' que representa o período gratuito no arquivo de reconciliação. Não há nenhuma alteração nas APIs, no faturamento ou nos incentivos.  Os parceiros devem informar suas equipes de vendas e estatísticas sobre essa nova lógica de cobrança e garantir que as operações sejam ajustadas conforme o necessário.  

Antes de implementar o alinhamento da data de cobrança, nós faturamos e cobramos na data de aniversário de cobrança de um parceiro, a data em que o parceiro assinou o programa CSP, e não na data de aniversário da assinatura do cliente, a data em que o cliente comprou a assinatura. Após 20 de fevereiro, os parceiros serão cobrados na data de aniversário da assinatura, eliminando esse período gratuito.  Os parceiros continuarão a receber as faturas em sua data de aniversário de cobrança, mas a data de efetivação da fatura será a data de aniversário de assinatura do cliente. 

As assinaturas que estiverem no período gratuito em 20 de fevereiro não serão cobradas entre a data da compra até a data de cobrança do parceiro. Além disso, eles não serão cobrados pelo primeiro mês do período pago de 12 meses. Se você usar um arquivo de reconciliação para verificação, lembre-se de que essa cobrança do primeiro mês não estará mais visível no arquivo de reconciliação.  


**P:** O que está mudando?

-   **R:** As assinaturas baseadas em licença não terão mais um período gratuito entre a data da compra e a data de cobrança do parceiro.

**P:** Quando o período gratuito será removido?

- **R:** A partir de 20 de fevereiro de 2018, novas assinaturas não terão um período gratuito.

**P:** As assinaturas no período gratuito em 20 de fevereiro de 2018 serão afetadas?

- **R:** O período gratuito continuará até a data de cobrança do parceiro para as assinaturas que já estiverem no período gratuito em 20 de fevereiro de 2018. Além disso, eles não serão cobrados pelo primeiro mês do período pago de 12 meses. Se você usar o arquivo de reconciliação para verificação, lembre-se de que essa cobrança do primeiro mês poderá estar ausente do arquivo de reconciliação. Veja os cenários abaixo para obter uma explicação mais detalhada.

**P:** Quando começará o período de 12 meses pago?

- **R:** No momento, o período pago começa na data de cobrança do parceiro após a data da compra. Quando o período gratuito for eliminado, o período pago para novas assinaturas começará na data da compra.

**P:** Quando as assinaturas serão renovadas automaticamente?

- **R:** Atualmente, a renovação automática das assinaturas ocorre 12 meses após a data de cobrança de parceiro seguinte à data da compra. Quando o período gratuito for eliminado, as assinaturas serão renovadas automaticamente 12 meses após a data da compra.

**P:** E se eu comprar a assinatura nos dias 29, 30 ou 31?

- **R:** A assinatura será provisionada na data da compra, mas o período pago de 12 meses não será iniciado até a primeira data do mês seguinte.

**P:** Quais ofertas são afetadas por essa alteração?

- **R:** Todas as assinaturas baseadas em licença do CSP são afetadas.

**P:** Como essa alteração afeta a fatura e o arquivo de reconciliação?

- **R:** Você não verá mais uma 'linha de cobrança $0' que representa o período gratuito.

**P:** A minha data de cobrança será alterada?

- **R:** Não, você continuará a receber a fatura e o arquivo de reconciliação em sua data de cobrança existente.

**P:** As datas de início/fim da cobrança mensal serão alteradas para as assinaturas existentes?

- **R:** Não, as datas de início/fim da cobrança mensal da assinatura continuarão a se alinhar à sua data de cobrança. No entanto, as novas assinaturas serão alinhadas à data da compra. Veja exemplos abaixo.

**P:** O cálculo de incentivos será alterado?

- **R:** Não.

**P:** As APIs serão alteradas?

- **R:** Não.

### <a name="common-scenarios"></a>Cenários comuns


|**Cenários**   |**Cenário 1: O período gratuito da assinatura termina antes de 20 de fevereiro de 2018**   |**Cenário 2: A assinatura está no período gratuito em 20 de fevereiro de 2018**  | **Cenário 3: A assinatura adquirida em 20 de fevereiro de 2018 ou depois disso**   |
|----------|:------------|:--------------------|:------------|
|Data da compra |1º de fev.    | 1º de fev.    | 1º de junho     |
|Data do provisionamento | 1º de fev.   |1º de fev.   |1º de junho   |
|Data da cobrança   | 15   |25   | 15|
|Período gratuito   | 1º de fev. - 15 de fev.|1º de fev. - 24 de fev.   |Sem período gratuito|
|Cobrança do primeiro mês   | 15 de fev. - 14 de março | 25 de fevereiro de 2018 – 24 de março de 2018 Sem cobrança, não aparecerá no arquivo de reconciliação|1º de junho - 30 de junho   |
|Cobrança do segundo mês   | 15 de março - 14 de abril|25 de março - 24 de abril   |1º de julho - 31 de julho|
|Período pago começa   | 15 de fev. de 2018 | 25 de março de 2018| 1 de junho de 2018| 
|Período pago termina | 14 de fev. de 2019   |24 de fev. de 2019   | 31 de maio de 2019  |
|Data da renovação | 15 de fev. de 2019 |25 de fev. de 2019   |1º de junho de 2019|

### <a name="scenario---new-purchase"></a>Cenário - nova compra

A data de cobrança do parceiro é no dia 15. Em 1º de junho, o parceiro compra uma nova assinatura por US$ 30/mês. O arquivo de reconciliação de 15 de junho conterá o seguinte:

- Cobrança de US$ 30 pelo primeiro mês (1º de junho - 30 de junho)

|**Início da cobrança**   |**Encerramento da cobrança**   |**Preço unitário**   |**Quantidade**   |**Valor**   |
|-----------------|:-------------|:----------------|:------------|:------|
|01/06/2018   |30/06/2018   |US$ 30   |1   |US$ 30   |

### <a name="scenario-suspend-and-reactivate-a-subscription-in-less-than-30-days-after-purchase"></a>Cenário: suspender e reativar uma assinatura em menos de 30 dias após a compra

A data de cobrança do parceiro é no dia 15. Em 1º de junho, o parceiro compra uma nova assinatura por US$ 30/mês. Em 5 de junho, o parceiro suspende a assinatura. Em 10 de junho, o parceiro reativa a assinatura. O arquivo de reconciliação de 15 de junho conterá o seguinte:

- Cobrança de US$ 30 pelo primeiro mês (1º de junho – 30 de junho) 
- Crédito de cancelamento de -US$ 30. Observe que a data de início da cobrança é 5 de junho, que é quando o parceiro suspendeu a assinatura. O crédito não é proporcional. O parceiro recebe o crédito de 100% porque suspendeu a assinatura nos primeiros 30 dias.
- Cobrança de reativação de US$ 30. Observe que a data de início da cobrança é 10 de junho, que é quando o parceiro reativou a assinatura. O valor não é proporcional. Nenhum cancelamento e reativação dentro de 30 dias após a data da compra é proporcional.


|**Início da cobrança**   |**Encerramento da cobrança**   |**Preço unitário**   |**Quantidade**   |**Valor**   |
|-----------------|:-------------|:----------------|:------------|:------|
|01/06/2018   |30/06/2018   |US$ 30   |1   |US$ 30   |
|05/06/2018   |30/06/2018   |-US$ 30   |1   |US$ 30   |
|10/06/2018   |30/06/2018   |US$ 30   |1   |US$ 30   |


### <a name="scenario-suspend-a-subscription-in-less-than-30-days-after-purchase-and-reactivate-after-30-days"></a>Cenário: suspender uma assinatura em menos de 30 dias após a compra e reativá-la após os 30 dias

A data de cobrança do parceiro é no dia 15. Em 1º de junho, o parceiro compra uma nova assinatura por US$ 30/mês. Em 5 de junho, o parceiro suspende a assinatura. O arquivo de reconciliação de 15 de junho conterá o seguinte:

|**Início da cobrança**   |**Encerramento da cobrança**   |**Preço unitário**   |**Quantidade**   |**Valor**   |
|-----------------|:-------------|:----------------|:------------|:------|
|01/06/2018   |30/06/2018   |US$ 30   |1   |US$ 30   |
|05/06/2018   |30/06/2018   |-US$ 30   |1   |US$ 30   |

Em 10 de julho, o parceiro reativa a assinatura. O arquivo de reconciliação de 15 de julho conterá a seguinte alteração:

- Cobrança de reativação de US$ 21,29. A data de início da cobrança é 10 de julho, que é quando o parceiro reativou a assinatura, e o valor é proporcional, US$ 21,29. Nenhum cancelamento e reativação após os 30 dias após a data da compra é proporcional. 

|**Início da cobrança**   |**Encerramento da cobrança**   |**Preço unitário**   |**Quantidade**   |**Valor**   |
|-----------------|:-------------|:----------------|:------------|:------|
|10/07/2018   |31/07/2018   |US$ 21,29   |1   |US$ 21,29   |

A data de renovação da assinatura permanece 1º de junho do ano seguinte, que é de 12 meses a partir da data da compra original.

### <a name="scenario-subscription-suspension-and-reactivation-more-than-30-days-after-purchase"></a>Cenário: suspensão e reativação da assinatura com mais de 30 dias após a compra 
A data de cobrança do parceiro é no décimo-quinto dia do mês. Em 1º de junho, o parceiro compra uma nova assinatura de uma licença por US$ 30 por mês. O arquivo de reconciliação de 15 de junho conterá apenas o seguinte: cobrança de US$30 no primeiro mês (1º de junho – 30 de junho).

|**Início da cobrança**   |**Encerramento da cobrança**   |**Preço unitário**   |**Quantidade**   |**Valor**   |
|-----------------|:-------------|:----------------|:------------|:------|
|01/06/2018   |30/06/2018   |US$ 30   |1   |US$ 30   |

O parceiro suspende a assinatura em 5 de julho, mas a reativa em 15 de julho. O arquivo de reconciliação de 15 de julho conterá o seguinte:

- Cobrança de US$ 30 pelo segundo mês (1º de julho – 31 de julho)

- Crédito de cancelamento de -US$ 26,19. Observe que a data de início da cobrança é 5 de julho, que é quando o parceiro suspendeu a assinatura, e o crédito é proporcional. Nenhum cancelamento e reativação após os 30 dias após a data da compra é proporcional.

- Cobrança de reativação de US$ 21,37. Observe que a data de início da cobrança é 10 de julho, que é quando o parceiro reativou a assinatura, e a cobrança é proporcional.

|**Início da cobrança**   |**Encerramento da cobrança**   |**Preço unitário**   |**Quantidade**   |**Valor**   |
|-----------------|:-------------|:----------------|:------------|:------|
|01/07/2018   |31/07/2018   |US$ 30  |1   |US$ 30   |
|05/07/2018   |31/07/2018   |   -US$ 26,19   |1   |-US$ 26,19|
|10/07/2018   |31/07/2018   |-US$ 21,34   |1   |US$ 21,34|

### <a name="scenario-change-license-quantity"></a>Cenário: alterar a quantidade de licenças 

A data de cobrança do parceiro é no dia 15. Em 1º de junho, o parceiro compra uma nova assinatura por US$ 30 por mês. Em 10 de junho, o parceiro aumenta a quantidade de licenças de uma para duas licenças. O arquivo de reconciliação de 15 de junho conterá o seguinte:

- Cobrança de US$ 30 pelo primeiro mês (1º de junho – 30 de junho) Mesmo que o parceiro tenha aumentado a quantidade de licenças antes da data de cobrança de 15 de junho, a cobrança não será reconhecida no sistema de cobrança da Microsoft até o dia de aniversário da assinatura, em 1º de julho.

|**Início da cobrança**   |**Encerramento da cobrança**   |**Preço unitário**   |**Quantidade**   |**Valor**   |
|-----------------|:-------------|:----------------|:------------|:------|
|01/06/2018   |30/06/2018   |US$ 30   |1   |US$ 30   |

Em 1º de julho, o dia do aniversário da assinatura, o sistema de cobrança da Microsoft reconhecerá que a quantidade de licenças foi alterada de uma para duas em 10 de junho. O sistema de cobrança irá gerar um crédito e cobranças proporcionais pelo primeiro mês e uma cobrança pelo segundo mês. O arquivo de reconciliação de 15 de julho conterá o seguinte:

- Crédito de -US$ 30 pelo primeiro mês.
- Cobrança proporcional de US$ 9 pelo primeiro mês (1º de junho – 9 de junho) por uma licença.
- Cobrança proporcional de US$ 42 pelo primeiro mês (10 de junho – 30 de junho) por duas licenças.
- Cobrança de US$ 60 pelo segundo mês (1º de julho – 31 de julho) por 2 licenças.

|**Início da cobrança**   |**Encerramento da cobrança**   |**Preço unitário**   |**Quantidade**   |**Valor**   |
|-----------------|:-------------|:----------------|:------------|:------|
|01/06/2018   |30/06/2018   |-US$ 30   |1   |-US$ 30|
|01/06/2018   |09/06/2018   |US$ 9   |1   |US$ 9|
|10/06/2018   |30/06/2018   |US$ 21   |2   |US$ 42|
|01/07/2018   |31/07/2018   |US$ 30   |2   |US$ 60   |

### <a name="scenario-add-on-subscriptions"></a>Cenário: assinaturas de complementos

A data de cobrança do parceiro é no dia 15. Em 1º de junho, o parceiro compra uma nova assinatura por US$ 30 por mês. Em 10 de junho, o parceiro compra uma nova assinatura de complemento por US$ 5 por mês. A data de renovação da assinatura do complemento será alinhada à data de renovação da assinatura base, que é 1º de junho. 

O arquivo de reconciliação de 15 de junho conterá o seguinte:

- Cobrança de US$ 30 pelo primeiro mês (1º de junho – 30 de junho) Isso é para a assinatura base.
- Cobrança proporcional de US$ 3,50 pelo primeiro mês (10 de junho – 30 de junho) para a assinatura do complemento. A data de início da cobrança é 10 de junho, que é quando a assinatura do complemento foi comprada, e o valor é proporcional.

|**Início da cobrança**   |**Encerramento da cobrança**   |**Preço unitário**   |**Quantidade**   |**Valor**   |
|-----------------|:-------------|:----------------|:------------|:------|
|01/06/2018   |30/06/2018   |US$ 30   |1   |US$ 30   |
|10/06/2018   |30/06/2018   |US$ 5   |1   |US$ 5   |

O arquivo de reconciliação de 15 de julho conterá o seguinte:

- Cobrança de US$ 30 pelo segundo mês (1º de julho – 31 de julho) Isso é para a assinatura base.
- Cobrança de US$ 5 pelo segundo mês (1º de julho – 31 de julho) Isso é para a assinatura do complemento.

|**Início da cobrança**   |**Encerramento da cobrança**   |**Preço unitário**   |**Quantidade**   |**Valor**   |
|-----------------|:-------------|:----------------|:------------|:------|
|01/07/2018   |31/07/2018   |US$ 30   |1   |US$ 30   |
|01/07/2018   |31/07/2018   |US$ 5   |1   |US$ 5   |

### <a name="scenario-new-purchase-on-the-29th-30th-or-31st"></a>Cenário: nova compra nos dias 29, 30 ou 31 

A data de cobrança do parceiro é no dia 15. Em 31 de maio, o parceiro compra uma nova assinatura por US$ 30/mês. As assinaturas adquiridas nos dias 29, 30 ou 31 receberão um período gratuito até o início do mês seguinte. Neste exemplo, o cliente obtêm um período gratuito de um dia; o período pago de 12 meses começa em 1º de junho. 

O arquivo de reconciliação de 15 de junho conterá o seguinte:

- Cobrança de US$ 30 pelo primeiro mês (1º de junho - 30 de junho)

|**Início da cobrança**   |**Encerramento da cobrança**   |**Preço unitário**   |**Quantidade**   |**Valor**   |
|-----------------|:-------------|:----------------|:------------|:------|
|01/06/2018   | 30/06/2018   |US$ 30   |1   |US$ 30  |
