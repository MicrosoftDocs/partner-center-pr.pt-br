---
title: Perguntas Frequentes sobre os novos recursos de cobrança | Partner Center
ms.topic: article
ms.date: 03/15/2019
Description: Veja a seguir perguntas frequentes sobre os recursos de cobrança anual e avaliação gratuita do Partner Center.
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
ms.localizationpriority: medium
ms.openlocfilehash: fd95787a87a1b70a0b2f31114b22dde7ca0f837c
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2019
ms.locfileid: "62135686"
---
# <a name="faq-about-new-billing-features"></a>Perguntas frequentes sobre os novos recursos de cobrança

**Aplica-se a**

-  Partner Center
-  Partner Center para Microsoft Cloud for US Government


Veja a seguir perguntas frequentes sobre os recursos de cobrança anual e avaliação gratuita do Partner Center. 

## <a name="in-this-section"></a>Nesta seção

-   [Perguntas frequentes sobre cobrança anual](#annualbillingfaq)

-   [Perguntas Frequentes de avaliações gratuitas](#freetrialsfaq)

-   [Perguntas frequentes sobre o alinhamento de cobrança](#billingalignmentfaq)


## <a href="" id="annualbillingfaq"></a>Perguntas frequentes sobre cobrança anual

Seções:

[Visão geral e os benefícios de faturamento anual](#overviewandbenefits)

[Seu pedido e cenários de cobrança](#placingyourorder)

[Alterar sua assinatura](#changingyoursubscription)

[Cálculo de preços](#pricingcalculation)

[Emissão de relatórios](#reporting)

[Incentivos](#incentives)


<a href="" id="overviewandbenefits"></a>**Visão geral e os benefícios de faturamento anual**

**P:** O que mudou?

-   **R:** Em resposta às solicitações, introduzimos a opção de pagamento para determinadas assinaturas de CSP em anualmente ou mensalmente. Essa nova opção foi disponibilizada em 17 de outubro de 2017.

**P:** Quem pode participar?

-   **R:** Todos os tipos de parceiros e parceiros podem se beneficiar da cobrança anual. A Cobrança Anual está disponível em todos os mercados onde o CSP está disponível no momento. 

**P:** O que é necessário levar em consideração ao pensar sobre a cobrança anual?    

-   **R:** Você deve considerar como seu movimento de vendas será afetado. Aqui estão algumas dicas para ajudá-lo a usar efetivamente a cobrança anual. 
    - Atualize as APIs para se preparar para o recurso de cobrança anual, se aplicável. 
    - Examine as alterações feitas na fatura e no arquivo de reconciliação baseado em licença.
    - Informe a sua equipe.
    - Atualize seus processos internos conforme o necessário.

**P:** Quais são os benefícios de faturamento anual? 

-   **R:** Cobranças anuais tem os seguintes benefícios:

    - Maior flexibilidade nas opções de pagamento.

    - Melhor alinhamento com o faturamento dos seus clientes.

    - Impacto reduzido nas flutuações de moeda.

    - Custos operacionais de cobrança reduzidos.

**P:** Quais ofertas terão a opção de cobrança anual?

-   **R:** Com base em licenciado assinaturas mais tem a opção para a opção de cobrança mensal ou anual. As assinaturas baseadas em uso só apresentam a opção de cobrança mensal. Você poderá identificar as frequências de cobrança disponíveis para cada oferta usando a coluna J da matriz de ofertas. Você pode encontrar a matriz de ofertas na seção 'Consulte as ofertas e os preços' no Partner Center. .

**P:** É anual de cobrança por assinatura ou licença?       

-   **R:** A cobrança anual e mensal são por assinatura.

**P:** Há alterações necessárias para as APIs para dar suporte à cobrança anual?    

-   **R:** Para aproveitar a cobrança anual lá está algumas alterações necessárias para suas APIs. Você pode encontrar informações mais detalhadas nos seguintes artigos:

    - https://partnercenter.microsoft.com/en-us/partner/developer

    - https://msdn.microsoft.com/en-us/library/partnercenter/microsoft.store.partnercenter.models.orders.order.billingcycle.aspx 

    - Código de exemplo: https://msdn.microsoft.com/en-us/library/partnercenter/mt634667.aspx 

<a href="" id="placingyourorder"></a>**Seu pedido e cenários de cobrança**

**P:** Haverá uma oferta exclusiva especificamente para pedidos com cobrança anual?   

-   **R:** Não. Todas as frequências de cobrança, incluindo a opção de cobrança anual, são atribuídas à Oferta como um atributo. Entretanto, você pode renomear uma oferta usando um nome de cliente mais amigável para permitir a diferenciação.

**P:** Como seleciono o faturamento anual

-   **R:** Ao adicionar uma nova assinatura, que você será solicitado a escolher a frequência de cobrança. Você pode escolher a opção de cobrança anual nesse ponto. Assim que a cobrança anual for selecionada, todas as ofertas disponíveis serão exibidas.

**P:** Se eu escolher cobranças anuais quando serão faturadas?    

-   **R:** Você será cobrado em sua próxima data de cobrança. Por exemplo, se a data de cobrança for o dia 1º e você comprar uma assinatura com cobrança anual no dia 29 de outubro de 2017, você será cobrado no dia 1º de novembro de 2017. Supondo que você não faça nenhuma alteração na licença, você será cobrado no dia 1º de novembro de 2018. Se você fizer uma alteração na licença, você receberá um crédito e uma nova cobrança na data de cobrança seguinte. 

**P:** Posso dividir uma assinatura para que uma parte é cobrada mensalmente e a outra é cobrada por ano?  

-   **R:** Não. A assinatura inteira deve ter a mesma frequência de cobrança. A assinatura inteira deve ter uma cobrança mensal ou anual.

**P:** Quando é a renovação da assinatura al com faturamento anual?     

-   **R:** A data de renovação será doze meses após a data de início do serviço. O período de serviço começa na data em que a assinatura é criada.  Por exemplo, uma assinatura criada em 10 de janeiro de 2018 será renovada em 10 de janeiro de 2019.

**P:** Quando serão faturadas a renovação de uma assinatura com a cobrança anual? 

-   **R:** Você será cobrado na próxima data de cobrança após a data de renovação de assinatura. Por exemplo, se você comprar uma assinatura com cobrança anual em 15 de janeiro de 2018 e se a sua data de cobrança for 20 de janeiro, sua assinatura será renovada em 15 de janeiro de 2019. Você será cobrado pela renovação em 20 de janeiro de 2019.

**P:** Fazer inscrições com faturamento anual receber um período gratuito?

-   **R:** Não, as assinaturas com frequência da cobrança anual não recebem um período gratuito. O período pago de 12 meses começa na data da compra. Isso é diferente de assinaturas com frequência de cobrança mensal que recebem um período gratuito entre a data da compra e a próxima data de cobrança.

**P:** Um cliente pode ter várias assinaturas da mesma oferta cada com frequências diferentes de cobrança?    

-   **R:** Isso depende da oferta. Há algumas ofertas restritas a uma assinatura por cliente. Se a oferta não estiver restrita, o cliente poderá ter várias assinaturas da mesma oferta com diferentes frequências de cobrança. Você pode encontrar os detalhes de todos os limites e restrições de oferta na coluna I da matriz de ofertas. Você pode encontrar a matriz de ofertas na seção 'Consulte as ofertas e os preços' no Partner Center.

<a href="" id="changingyoursubscription"></a>**Alterar sua assinatura**

**P:** Pode adicionar uma nova licença a uma assinatura existente que tem cobrança anual?    

-   **R:** Sim. Você pode alterar a quantidade de licenças das suas assinaturas a qualquer momento. A adição de outras licenças não afetará a frequência de cobrança. 

**P:** Posso adicionar licenças que têm a cobrança mensal para uma assinatura existente que tem cobrança anual? 

-   **R:** Depois que você comprar uma assinatura com a cobrança anual, as licenças adicionais seguirão a mesma frequência de cobrança. Se então você precisar comprar licenças com cobrança mensal, precisará comprar uma nova assinatura.

**P:** Posso mudar a frequência de cobrança para uma assinatura de mensal, anual e vice-versa? 

-   **R:** Sim. Ver **para alterar a frequência de cobrança de um serviço online** na [Noções básicas de cobrança](https://docs.microsoft.com/en-us/partner-center/billing-basics).

**P:** Cobranças anuais está disponível para as ofertas de complemento?   

-   **R:** Sim. A assinatura complementar terá automaticamente a mesma frequência de cobrança da assinatura principal.

**P:** Como cobranças anuais funcionará quando adicionar ou remover licenças? 

-   **R:** Você pode adicionar ou remover licenças a qualquer momento. alteração Você receberá um crédito e será cobrado novamente proporcionalmente em sua próxima data de cobrança depois de alterar o número de licenças. 

**P:** O que acontece se eu cancelar uma assinatura com faturamento anual de trabalho?    

-   **R:** A política de cancelamento é o mesmo para todas as frequências de cobrança. Se a assinatura for cancelada nos 30 primeiros dias do período de 12 meses pago, você receberá um crédito de 100% em sua próxima data de cobrança. Se a assinatura for cancelada após 30 dias do período pago de 12 meses, você receberá um crédito pro-rata em sua próxima data de cobrança.

**P:** Um cliente pode mudar uma assinatura com faturamento anual de um parceiro para o outro parceiro?  

-   **R:** Não. As assinaturas não podem ser movidas entre parceiros. O novo parceiro deve comprar uma nova assinatura em nome do cliente. Isso se aplica a assinaturas cobradas mensal e anualmente.

**P:** Eu reativar uma assinatura com a cobrança anual?

-   **R:** Sim, você pode reativar a assinatura por 90 dias a partir da data de suspensão. Você receberá uma cobrança proporcional na data de cobrança seguinte. A data de renovação da assinatura permanece a mesma.

<a href="" id="pricingcalculation"></a>**Cálculo de preços**

**P:** O que acontece se um preço da oferta é alterado parte durante o período de 12 meses de uma assinatura anual cobrado?    

-   **R:** O preço da oferta no momento da compra é garantido que o termo de assinatura de 12 meses completos. 

**P:** O preço de uma assinatura será quando ele renovação automática após um período de assinatura de 12 meses?    

-   **R:** Quando uma assinatura seja renovada, o preço se baseará na lista de preços atual na data de renovação. O novo preço é garantido pelo próximo período de 12 meses de assinatura.

**P:** Como o crédito para uma licença foi cancelada ou a assinatura é calculado? Ele é calculado pelo dia ou pelo mês?   

-   **R:** Crédito de cancelamento é calculado da seguinte maneira:

    - Crédito de cancelamento = ((preço mensal*12)/365) * dias restantes no período de 12 meses * número de licenças canceladas.

**P:** O que acontece se uma parte de reduções de preço oferta durante o período de 12 meses de uma assinatura anual cobrado? 

-   **R:** Não há nenhuma alteração. O preço é definido para o período total de 12 meses. Isso também acontece com a cobrança mensal.


<a href="" id="reporting"></a>**Emissão de relatórios**

**P:** Onde posso encontrar out se uma assinatura é cobrada anualmente ou mensalmente?   

-   **R:** O arquivo de reconciliação de licença baseada incluirá as informações sobre a frequência de cobrança. Você pode descobrir isso na coluna AA

**P:** As alterações que haverá no arquivo de reconciliação de licença com base em quando a assinatura com a cobrança anual é adquirida ou renovada?  

-   **R:** A primeira alteração será uma nova linha no arquivo de reconciliação de licença baseada na primeira data de cobrança após a compra ou uma nova assinatura. ativado. Se nenhuma alteração for feita na assinatura, não haverá linhas nos arquivos de reconciliação para o segundo mês até o décimo-segundo do período da assinatura. a próxima alteração no arquivo de reconciliação aparecerá quando a assinatura for renovada. Isso será exibido na data da primeira cobrança após a renovação. Se for feita uma alteração na assinatura durante o período de 12 meses, um crédito e uma nova cobrança proporcional serão exibidos no próximo arquivo de reconciliação depois que a alteração for feita.

**P:** Como a compra de, alteração ou cancelamento de uma assinatura anual aparece na coluna P dos arquivos de uso?

-   **R:** Os encargos da compra inicial aparece como "taxas de Prorate quando comprar." As alterações de licença que resultam em crédito e nova cobrança aparecem como "Proporcional à instância do ciclo". Os créditos de cancelamento aparecem como "Taxa de cancelamento".

**P:** Quando uma assinatura anual é cancelada, como isso aparecem no arquivo de reconciliação?   

-   **R:** O arquivo de reconciliação conterá um item de linha para um crédito de cancelamento. Se o cancelamento ocorrer nos 30 primeiros dias do período de 12 meses, a assinatura será creditada em 100%. Se o cancelamento ocorrer após os primeiros 30 dias, a assinatura será creditada de forma proporcional.

**P:** Como-aparecem no arquivo de reconciliação se licenças são adicionadas a uma assinatura que tem cobrança anual?  

-   **R:** O arquivo de reconciliação conterá um crédito e rebill proporcional. Isso também acontecerá para uma assinatura com cobrança mensal.

**P:** Como ela será exibida lion o arquivo de reconciliação se licenças são removidas de uma assinatura com a cobrança anual? 

-   **R:** O arquivo de reconciliação conterá um crédito e rebill proporcional.  Isso também acontecerá para uma assinatura com cobrança mensal.

**P:** O preço anual é mostrado na lista de preços? 

-   **R:** Não. A lista de preços mostra o preço mensal. Você pode calcular o preço anual multiplicando o preço mensal por doze.

**P:** A matriz de oferta tem entradas diferentes para as ofertas que podem ser cobradas por ano.?   

-   **R:**  Não. As IDs da oferta são iguais para todas as frequências de cobrança. Não há IDs da oferta exclusivas para a cobrança anual.


<a href="" id="incentives"></a>**Incentivos**

**P:** A frequência com que os incentivos em assinaturas anuais são calculados? 

-   **R:** Calculamos receita cobrada. Os pagamentos de incentivos ganhos serão efetuados de acordo com nossa política encontrada nos nossos guias de incentivos do CSP. 

**P:** Como os incentivos nas assinaturas cobradas por ano são pago?  

-   **R:** Atualmente, todos os pagamentos incentivos são feitos duas vezes por ano. Esses pagamentos são feitos 45 dias após o fim do semestre.

**P:** Quando uma assinatura anual cobrada é vendida, como receita dessa assinatura é reconhecida para o cálculo de incentivos. Ele se baseará na receita cobrada ou ajustada? 

-   **R:** Incentivos cálculos baseiam-se na receita cobrada.

**P:**, Como são calculados os ganhos de incentivos sobre a assinatura cobrada anualmente qualificada entre as diversas taxas de incentivo do CSP (taxas de incentivo globais, taxas de acelerador local e campanhas locais)?

-   **R:** Independentemente de como uma assinatura é cobrada, se mensal ou anualmente, parceiros receber incentivos em todas as transações qualificadas. Isso inclui a taxa global de incentivos, aplicada à receita cobrada para o período, o acelerador local para todas as regiões em que existem aceleradores locais e todas as campanhas globais onde aplicável.

**P:** Quem você contata se você tiver dúvidas sobre incentivos?

- **R:** Entre em contato com a equipe de suporte apropriado de incentivos regionais:

  - América do Norte: ocina@microsoft.com

  - América Latina e Brasil: ocilatam@microsoft.com

  - EMEA: ociemea@microsoft.com

  - APOAC (exceto o Japão): ociapgc@microsoft.com

  - Japão: ocijp@microsoft.com


**P:** O que acontece se eu suspender minha assinatura? 

-   **R:** Se você suspender uma assinatura, no Partner Center ou por meio da API, dentro de 30 dias da compra, você receberá um crédito de 100%, independentemente da frequência de cobrança. 

    Com a cobrança anual, isso seria parecido com:

    - O parceiro compra uma assinatura em 1º de janeiro = linha de cobrança criada para o período de serviço de 01/01 – 31/12.
    - Suspende a assinatura em 25 de janeiro = linha de cobrança de crédito criada para o período de serviço de 01/01 – 31/12.
    - Reativa em 29 de janeiro = linha de cobrança criada para o período de serviço de 01/01 – 31/12.

    Com a cobrança mensal, isso seria parecido com:

    - O parceiro compra uma assinatura em 1º de janeiro = linha de cobrança criada para o período de serviço de 01/01 – 31/01.
    - Suspende a assinatura em 25 de janeiro = linha de cobrança de crédito criada para o período de serviço de 01/01 – 31/01.
    - Reativa em 29 de janeiro = linha de cobrança criada para o período de serviço de 29/01 – 31/01.



## <a href="" id="freetrialsfaq"></a>Perguntas Frequentes de avaliações gratuitas

**Q1:** Quais são as avaliações gratuitas?

-   **R:** Você pode oferecer uma avaliação gratuita de 30 dias de determinados produtos para seus clientes. Isso permite que seus clientes avaliem o produto antes de comprá-lo. As avaliações gratuitas estão disponíveis para os seguintes produtos: 

    - Office 365 Business Premium (a partir de 17 de outubro de 2017)
    - Office 365 E3 (a partir de 17 de outubro de 2017)
    - Office 365 E5 com PSTN (a partir de 17 de outubro de 2017)
    - Office 365 E5 sem PSTN (a partir de 17 de outubro de 2017)
    - Enterprise Mobility & Security E5 (a partir de 17 de outubro de 2017)
    - Dynamics 365 Customer Engagement Plan 1 (a partir de 17 de outubro de 2017)
    - Dynamics 365 for Financials (a partir de 17 de outubro de 2017)
    - Microsoft 365 Business (a partir de 1º de março de 2018)
    
**Q2:** São as cobranças anuais e livres avaliações diferentes em uma nuvem soberana vs. nuvem pública?

-   **R:** Não. São iguais. A única diferença serão nas SKUs de avaliação que estão disponíveis no momento da inicialização.

**Q3:** Quem pode participar?

-   **R:** Todos os parceiros podem participar. No entanto, atualmente não está disponível na China. 

**Q4:** As ações que deve levar para habilitar me beneficiar essas avaliações gratuitas??

-   **R:** Considere como a avaliação gratuita pode ser incorporada em seu movimento mais vendido e o impacto sobre os processos internos. Talvez também seja necessário alterar suas APIs para acomodar a conversão de uma avaliação gratuita em uma assinatura paga. Há especificações técnicas detalhadas para as alterações de API na exibição Anúncios no Partner Center.

**Q5:** Será exibida a avaliação gratuita no meu arquivo de nota fiscal e reconciliação?

-   **R:** Não, as avaliações gratuitas não aparecerão na sua fatura ou no arquivo de reconciliação de licença baseada. Elas aparecerão em sua fatura ou no arquivo de reconciliação baseado em licença depois que você converter uma avaliação gratuita em uma assinatura paga. A assinatura convertida aparecerá na sua fatura e no arquivo de reconciliação baseado em licença da mesma maneira que qualquer outra assinatura nova.

**Q6:** As avaliações gratuitas tem um impacto sobre incentivos?

-   **R:** Não. A versão de avaliação gratuita não tem impacto nos incentivos.

**Q7:** As avaliações gratuitas ficará disponíveis para outros produtos do Office no futuro?

-   **R:** Nós fornecemos avaliações gratuitas para esses produtos porque eles são as ofertas de negócios mais abrangentes e populares. É possível que adicionemos outras ofertas de avaliação gratuita no futuro.

**Q8:** Um cliente tenha mais de uma avaliação gratuita?

-   **R:** Cada cliente tem direito a uma avaliação gratuita por oferta disponível.

**Q9:** Há limites para uma avaliação gratuita?

-   **R:** Sim. A avaliação contempla até 25 licenças. A contagem de licenças não pode ser alterada durante o período de avaliação. Depois que a avaliação for convertida em uma assinatura paga, você poderá adicionar outras licenças à assinatura.

**Q10:** Uma avaliação gratuita é automaticamente convertida em uma assinatura paga?

-   **R:** Não. Será necessário converter a assinatura por conta própria, no Partner Center ou por meio da API.

**Q11:** As avaliações gratuitas podem ser usadas para assinaturas cobradas mensais e anuais?

-   **R:** Sim. Você poderá escolher a frequência de cobrança quando estiver convertendo a avaliação em uma assinatura paga.

**Q12:** A data de início da assinatura se basearão na data que o inicia de avaliação gratuito ou a data em que ele é convertido em uma assinatura paga? 

-   **R:** A data de início se baseia na data de conversão. Se a avaliação gratuita for convertida em uma oferta paga com cobrança anual, a data de renovação da assinatura será de doze meses a partir da data de conversão. Se a avaliação gratuita for convertida em uma oferta paga com cobrança mensal, a data de renovação da assinatura será 12 meses a partir da data de cobrança após a data de conversão.

**Q13:** É possível adicionar ou remover estações durante a avaliação gratuita?

-   **R:** Não. As avaliações gratuitas assumirão como padrão 25 licenças e não poderão ser atualizadas.

**Q14:** Há avaliações para ofertas de complemento, como o ATP e PSTN?

-   **R:** Não há nenhum avaliações gratuitas para qualquer oferta de complemento no momento.

**Q15:** Para fornecer uma avaliação gratuita para uma oferta que já possui um cliente?

-   **R:** Não. Se o cliente já tiver a oferta, ela não poderá ser usada em uma avaliação gratuita.

**Q16:** Será capaz de ver todas as minhas ofertas de avaliação pendentes?

-   **R:** Sim. A página de cliente lista todas as assinaturas. Isso inclui as assinaturas de avaliação gratuita e as assinaturas pagas.

**Q17:** Será que posso ser notificado sobre avaliações gratuitas prestes a expirar?

-   **R:** Não. Você pode acompanhar as datas de validade usando a exibição do cliente no Partner Center ou consultando a API. É recomendável monitorar essas datas com frequência para que você possa executar as ações de acompanhamento apropriadas quando os clientes tomarem uma decisão.

**Q18:** Se um cliente teve uma avaliação gratuita para uma oferta pode também usarem outra avaliação para uma oferta diferente? 

-   **R:** Sim. Os clientes podem se inscrever em uma avaliação por oferta. Por exemplo, eles podem obter uma avaliação gratuita do Office 365 Business Premium e uma avaliação gratuita do Office 365 E3.

**Q19:** O que acontece quando a versão de avaliação termina? Eu ou o meu cliente receberemos uma notificação? Quais notificações são exibidas quando tento entrar em uma avaliação expirada?

-   **R:** Depois que uma versão de avaliação expirar, um cliente tentar fazer logon em que a avaliação será exibida uma mensagem indicando que a versão de avaliação expirou. Não haverá notificações para sinalizar que uma avaliação está prestes a expirar; no entanto, como parceiro, você pode controlar isso por meio da exibição do cliente ou por meio de consultas de API.

**Q20:** Uma versão de avaliação pode ser estendido?

-   **R:** Não. Depois de 30 dias, a avaliação deverá ser convertida ou expirará.

**Q21:** Quando uma versão de avaliação expira, podem as informações de avaliação de ser acessadas?

-   **R:** Sim. Os dados são armazenados em linha com os padrões de retenção de dados. Depois que você comprar uma nova assinatura com os mesmos planos de serviço, os dados do cliente poderão ser acessados da assinatura recém-ativada.

**Q22:** São as avaliações gratuitas disponíveis para o governo e Education oferece?

-   **R:** Não há nenhum avaliações gratuitas para o governo e educação oferece no momento.

**Q23:** As avaliações gratuitas de cliente para o programa de provedor de solução de nuvem (CSP) podem ser convertidas para outros locatários do programa como EA, Open ou MOSP? 

-   **R:** Não. As assinaturas não podem ser transferidas do CSP para outro programa.

**Q24:** Como posso obter suporte em versões de avaliação gratuitas? 

-   **R:** Envie uma solicitação de serviço por meio do Partner Center.

## <a href="" id="billingalignmentfaq"></a>Alinhamento - livre de final de período de cobrança

A partir do dia 21 de fevereiro de 2018, o Provedor de Soluções na Nuvem (CSP) começará a implementar o “alinhamento da data de cobrança” para novas assinaturas com cobrança mensal. Esse "alinhamento da data de cobrança" fornecerá aos parceiros mais flexibilidade e previsibilidade das vendas e da cobrança, bem do provisionamento e do gerenciamento de assinaturas de clientes. 

**23 DE FEVEREIRO DE ATUALIZAÇÃO:**  Anteriormente anunciamos uma data de implementação de 20 de fevereiro, mas nossa implementação real foi um pouco atrasada e escalonada por categoria de produto.  Analise o catálogo em destaque abaixo em relação à data de implementação por Categoria de Produto. 

|**Categoria de produto**   |**Dia de implementação**   |
|-----------------|:-------------|
|Office  |21 de fevereiro   |
|Windows, Minecraft   |22 de fevereiro   |
|Office 365 China   |23 de fevereiro   |
|Dynamics/Intune   |23 de fevereiro   |

As assinaturas adquiridas antes da data de implementação (consulte o catálogo em destaque acima) obtêm um período gratuito a partir da data da compra até a data de cobrança do parceiro. As assinaturas adquiridas após a data da implementação não receberão mais um período gratuito. O período pago de 12 meses será iniciado (alinhado) na data da compra em relação ao parceiro de cobrança. Os parceiros não verão mais uma 'linha de cobrança $0' que representa o período gratuito no arquivo de reconciliação. Não há nenhuma alteração nas APIs, no faturamento ou nos incentivos.  Os parceiros devem informar suas equipes de vendas e estatísticas sobre essa nova lógica de cobrança e garantir que as operações sejam ajustadas conforme o necessário.  

Antes de implementar o alinhamento da data de cobrança, nós faturamos e cobramos na data de aniversário de cobrança de um parceiro, a data em que o parceiro assinou o programa CSP, e não na data de aniversário da assinatura do cliente, a data em que o cliente comprou a assinatura. Após a data de implementação, os parceiros serão cobrados na data de aniversário da assinatura, eliminando esse período gratuito.  Os parceiros continuarão a receber as faturas em sua data de aniversário de cobrança, mas a data de efetivação da fatura será a data de aniversário de assinatura do cliente. 

As assinaturas que estiverem no período gratuito na data de implementação não serão cobradas entre a data da compra até a data de cobrança do parceiro. Além disso, eles não serão cobrados pelo primeiro mês do período pago de 12 meses. Se você usar um arquivo de reconciliação para verificação, lembre-se de que essa cobrança do primeiro mês não estará mais visível no arquivo de reconciliação.  

**Q1:** O que está mudando com a data de cobrança?

-   **R:** Assinaturas de licença deixarão de ter um período gratuito. Atualmente, há um período gratuito da data da compra até a data de cobrança do parceiro.

**Q2:** Quando o período de gratuita será removido?

- **R:** Começando na data de implementação listada no gráfico a seguir, novas assinaturas não receberão um período gratuito.

|**Categoria de produto**   |**Dia de implementação**   |
|-----------------|:-------------|
|Office  |21 de fevereiro   |
|Windows, Minecraft   |22 de fevereiro   |
|Office 365 China   |23 de fevereiro   |
|Dynamics/Intune   |23 de fevereiro   |

**Q3:** Qual será o impacto sobre as assinaturas no período na data de implementação gratuito?

- **R:** As assinaturas que estão no período gratuito na data de implementação ainda receberá um período de gratuito a partir da data de compra para a data de cobrança do parceiro. Essas licenças também receberão um "período gratuito estendido" e não serão cobradas pelo primeiro mês do período pago de 12 meses. O "período gratuito estendido" não será aplicável a licenças adicionadas no primeiro mês. Se aumentar a quantidade de licenças no primeiro mês, você será cobrado por essas licenças adicionadas na próxima fatura/reconciliação. Se o arquivo de reconciliação for usado para verificação, esteja ciente de que essa cobrança do primeiro mês poderá estar ausente do arquivo de reconciliação. Veja os cenários abaixo para obter uma explicação mais detalhada.

**Q4:** Quando o período de 12 meses pago será iniciada uma nova assinatura?

- **R:** Atualmente, o período pago começa no parceiro seguindo a data da compra de data de cobrança. A partir da data de implementação, o período pago de novas assinaturas começará na data da compra.

**Q5:** Quando serão assinaturas de renovação automática?

- **R:** Assinaturas de renovação automática 12 meses após a primeira data de cobrança. Atualmente, isso significa que a renovação automática das assinaturas ocorrerá 12 meses após a primeira data de cobrança do parceiro seguinte à data da compra. A partir da data de implementação, as novas assinaturas serão renovadas automaticamente 12 meses após a data da compra.

**Q6:** E se eu comprar a assinatura no dia 29, 30 ou 31 do mês?

- **R:** A assinatura estará disponível a partir da data de compra, mas o termo pago de 12 meses não serão iniciados até o primeiro dia do mês seguinte.

**Q7:** Quais ofertas são afetadas?

- **R:** A remoção de período gratuita se aplica a todas as assinaturas de CSP baseados em licença.

**Q8:** Como isso afeta o arquivo da nota fiscal e reconciliação? 

- **R:** Você não verá mais "linha cobrança de US $0" a nota fiscal ou o arquivo de reconciliação. Atualmente, a linha de cobrança $0 representa o período gratuito.

**Q9:** Data minha cobrança mudará?

- **R:** Não, você continuará a receber o arquivo de nota fiscal e reconciliação no sua data de cobrança existente.

**Q10:** Será o custo mensal começar e terminar a alteração de datas para as assinaturas existentes?

- **R:** Não, existente de assinatura mensal custo inicial e final datas continuarão a se alinhar com a data de cobrança. No entanto, as novas assinaturas serão alinhadas à data da compra. Veja exemplos abaixo.

**Q11:** Cálculo de incentivos mudará?

- **R:** Não, não há nenhuma alteração nos cálculos de incentivos.

**Q12:** Haverá uma alteração para as APIs?

- **R:** Não, não há nenhuma alteração para as APIs.

### <a name="common-scenarios"></a>Cenários comuns


|**Cenários**   |**Cenário 1: Período de assinatura gratuita termina antes da data de implementação**   |**Cenário 2: Assinatura está dentro do período gratuito na data de implementação**  | **Cenário 3: Assinatura adquirida em ou após a data de implementação**   |
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

|**Custo inicial**   |**Final de encargo**   |**Preço unitário**   |**quantidade**   |**Quantidade**   |**Tipo de encargo** |
|-----------------|:-------------|:----------------|:------------|:------|--------------|
|01/06/2018   |30/06/2018   |US$ 30   |1   |US$ 30   |Taxas proporcionais durante a compra |

### <a name="scenario-5a-suspend-and-reactivate-before-billing-date"></a>Cenário 5a: Suspender e reativar antes da data de cobrança

A data de cobrança do parceiro é no dia 15 do mês. Em 1º de junho de 2018, o parceiro compra uma nova assinatura. A assinatura custa US$ 30 por licença por mês. Em 5 de junho de 2018, o parceiro suspende a assinatura. Em 10 de junho de 2018, o parceiro reativa a assinatura. O arquivo de reconciliação de 15 de junho conterá as seguintes linhas de cobrança:

- Cobrança de US$ 30 pelo período de serviço de 1º de junho – 30 de junho. 
- Crédito de cancelamento de -US$ 30 pelo período de serviço de 5 de junho - 30 de junho. O crédito não é proporcional porque a assinatura foi suspensa nos primeiros 30 dias. 
- Cobrança de US$ 30 pelo período de serviço de 10 de junho - 30 de junho. A cobrança não é proporcional porque a assinatura foi reativada nos primeiros 30 dias. 

|**Custo inicial**   |**Final de encargo**   |**Preço unitário**   |**quantidade**   |**Quantidade**   |**Tipo de encargo** |
|-----------------|:-------------|:----------------|:------------|:------|:------ |--------|
|01/06/2018   |30/06/2018   |US$ 30   |1   |US$ 30   |Taxas proporcionais durante a compra |
|05/06/2018   |30/06/2018   |-US$ 30   |1   |US$ 30   |Taxa de cancelamento |
|10/06/2018   |30/06/2018   |US$ 30   |1   |US$ 30   |Taxa de ativação |

Observe que, quando uma assinatura é suspensa e reativada, a data de renovação automática permanecerá sendo 12 meses da data da compra original.

### <a name="scenario-5b-suspend-and-reactivate-after-billing-date-but-less-than-30-days-from-purchase-date"></a>Cenário 5b: Suspender e reativar após a data de cobrança, mas menos de 30 dias a partir da data de compra

A data de cobrança do parceiro é no dia 15 do mês. Em 1º de junho de 2018, o parceiro compra uma nova assinatura. A assinatura custa US$ 30 por licença por mês. Em 20 de junho de 2018, o parceiro suspende a assinatura. Em 25 de junho de 2018, o parceiro reativa a assinatura. O arquivo de reconciliação de 15 de junho conterá as seguintes linhas de cobrança:

- Cobrança de US$ 30 pelo período de serviço de 1º de junho – 30 de junho. 

|**Custo inicial**   |**Final de encargo**   |**Preço unitário**   |**quantidade**   |**Quantidade**   |**Tipo de encargo** |
|-----------------|:-------------|:----------------|:------------|:------|:------ |--------|
|01/06/2018   |30/06/2018   |US$ 30   |1   |US$ 30   |Taxas proporcionais durante a compra |

O arquivo de reconciliação de 15 de julho conterá as seguintes linhas de cobrança:
- Crédito de cancelamento de -US$ 30 pelo período de serviço de 20 de junho – 30 de junho. O crédito não é proporcional porque a assinatura foi suspensa nos primeiros 30 dias.
- Cobrança de US$ 30 pelo período de serviço de 25 de junho – 30 de junho. A cobrança não é proporcional porque a assinatura foi reativada nos primeiros 30 dias.
- Cobrança de US$ 30 pelo período de serviço de 1º de julho – 31 de julho.

|**Custo inicial**   |**Final de encargo**   |**Preço unitário**   |**quantidade**   |**Quantidade**   |**Tipo de encargo** |
|-----------------|:-------------|:----------------|:------------|:------|:------ |--------|
|20/06/2018   |30/06/2018   |-US$ 30   |1   |-US$ 30   |Taxa de cancelamento |
|25/06/2018   |30/06/2018   |US$ 30   |1   |US$ 30   |Taxa de ativação |
|01/07/2018   |31/7/2018   |US$ 30   |1   |US$ 30   |Taxa do ciclo |

### <a name="scenario-5c-suspend-and-reactivate-different-license-quantity-after-billing-date-but-less-than-30-days-from-purchase-date"></a>Cenário 5c: Suspender e reativar (quantidade de licenças diferente) após a data de cobrança, mas menos de 30 dias a partir da data de compra

A data de cobrança do parceiro é no dia 15 do mês. Em 1º de junho de 2018, o parceiro compra uma nova assinatura. A assinatura custa US$ 30 por licença por mês. Em 20 de junho de 2018, o parceiro suspende a assinatura. Em 25 de junho de 2018, o parceiro reativa a assinatura com duas licenças. O arquivo de reconciliação de 15 de junho conterá as seguintes linhas de cobrança:

- Cobrança de US$ 30 pelo período de serviço de 1º de junho – 30 de junho. 

|**Custo inicial**   |**Final de encargo**   |**Preço unitário**   |**quantidade**   |**Quantidade**   |**Tipo de encargo** |
|-----------------|:-------------|:----------------|:------------|:------|:------ |--------|
|01/06/2018   |30/06/2018   |US$ 30   |1   |US$ 30   |Taxas proporcionais durante a compra |

O arquivo de reconciliação de 15 de julho conterá as seguintes linhas de cobrança:
- Crédito de cancelamento de -US$ 30 pelo período de serviço de 20 de junho – 30 de junho. O crédito não é proporcional porque a assinatura foi suspensa nos primeiros 30 dias.
- Cobrança de US$ 30 pelo período de serviço de 25 de junho – 30 de junho. A cobrança de reativação não é proporcional porque a assinatura foi reativada nos primeiros 30 dias. A cobrança também é baseada na quantidade de licenças originais de 1.
- Crédito de -US$ 6 pelo período de serviço de 25 de junho – 30 de junho. A cobrança de reativação só é feita por 1 licença durante o período de serviço de 25 de junho – 30 de junho quando você tinha 2 licenças. O crédito de -US$ 6 reverte a cobrança incorreta pelo período de serviço de 25 de junho – 30 de junho.
- Nova cobrança proporcional de US$ 12 pelo período de serviço de 25 de junho – 30 de junho. O parceiro tinha 2 licenças durante esse período de serviço. O preço unitário é calculado como (30/30)*6*2 = US$ 12.
- Cobrança de US$ 60 pelo período de serviço de 1º de julho – 31 de julho.

|**Custo inicial**   |**Final de encargo**   |**Preço unitário**   |**quantidade**   |**Quantidade**   |**Tipo de encargo** |
|-----------------|:-------------|:----------------|:------------|:------|:------ |--------|
|20/06/2018   |30/06/2018   |-US$ 30   |1   |-US$ 30   |Taxa de cancelamento |
|25/06/2018   |30/06/2018   |US$ 30   |1   |US$ 30   |Taxa de ativação |
|25/06/2018   |30/06/2018   |-US$ 6   |1   |-US$ 6   |Proporcional à instância do ciclo |
|25/06/2018   |30/06/2018   |US$ 6   |2   |US$ 12   |Proporcional à instância do ciclo |
|01/07/2018   |31/7/2018   |US$ 30   |2   |US$ 60   |Taxa do ciclo |

### <a name="scenario-6-subscription-suspension-less-than-30-days-after-purchase-and-reactivation-more-than-30-days-after-purchase"></a>Cenário 6: Menos de 30 dias após a compra e reativação mais de 30 dias após a compra de suspensão da assinatura 

A data de cobrança do parceiro é no dia 15 do mês. Em 1º de junho, o parceiro compra uma nova assinatura de uma licença por US$ 30 por mês. Em 5 de junho, o parceiro suspende a assinatura. O arquivo de reconciliação de 15 de junho conterá as seguintes linhas de cobrança:

- Cobrança de US$ 30 pelo período de serviço de 1º de junho - 30 de junho
- Crédito de cancelamento de -US$ 30 pelo período de serviço de 5 de junho - 30 de junho. O crédito não é proporcional porque a assinatura foi suspensa nos primeiros 30 dias.

|**Custo inicial**   |**Final de encargo**   |**Preço unitário**   |**quantidade**   |**Quantidade**   |**Tipo de encargo** |
|-----------------|:-------------|:----------------|:------------|:------|---------|
|01/06/2018   |30/06/2018   |US$ 30   |1   |US$ 30   |Taxas proporcionais durante a compra
|05/06/2018   |30/06/2018   |-US$ 30   |1   |-US$ 30   |Taxa de cancelamento

Em 10 de julho, o parceiro reativa a assinatura. O arquivo de reconciliação de 15 de julho conterá as seguintes linhas de cobrança:

- Cobrança de reativação de US$ 21,30 pelo período de serviço de 10 de julho - 31 de julho. Reativações após 30 dias da data da compra resultam em uma cobrança proporcional. 

|**Custo inicial**   |**Final de encargo**   |**Preço unitário**   |**quantidade**   |**Quantidade**   |**Tipo de encargo** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|10/07/2018   |31/7/2018   |US$ 21,30   |1   |US$ 21,30   |Taxa de ativação |

O arquivo de reconciliação de 15 de agosto conterá as seguintes linhas de cobrança:
- Cobrança de US$ 30 pelo período de serviço de 1º de agosto – 31 de agosto.

|**Custo inicial**   |**Final de encargo**   |**Preço unitário**   |**quantidade**   |**Quantidade**   |**Tipo de encargo** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|01/08/2018   |31/8/2018   |US$ 30   |1   |US$ 30   |Taxa do ciclo |

Observe que, quando uma assinatura é suspensa e reativada, a data de renovação automática permanecerá sendo 12 meses da data da compra original. 

### <a name="scenario-7-subscription-suspension-and-reactivation-more-than-30-days-after-purchase"></a>Cenário 7: Suspensão e reativação da assinatura com mais de 30 dias após a compra 
A data de cobrança do parceiro é no dia 15 do mês. Em 1º de junho, o parceiro compra uma nova assinatura de uma licença por US$ 30 por mês. 

O arquivo de reconciliação de 15 de junho conterá somente as seguintes linhas de cobrança:

- Cobrança de US$ 30 pelo período de serviço de 1º de junho – 30 de junho.

|**Custo inicial**   |**Final de encargo**   |**Preço unitário**   |**quantidade**   |**Quantidade**   |**Tipo de encargo** |
|-----------------|:-------------|:----------------|:------------|:------|---------|
|01/06/2018   |30/06/2018   |US$ 30   |1   |US$ 30   |Taxas proporcionais durante a compra |

O parceiro suspende a assinatura em 5 de julho, mas a reativa em 15 de julho. O arquivo de reconciliação de 15 de julho conterá as seguintes linhas de cobrança:

- Cobrança de US$ 30 pelo período de serviço de 1º de julho - 31 de julho.
- Crédito de cancelamento de -US$ 26,14 pelo período de serviço de 5 de julho – 31 de julho. Cancelamentos após 30 dias da data da compra resultam em um crédito proporcional. Cálculo = (preço mensal/dias no período de serviço total) x dias no período de serviço proporcional x quantidade de licenças x (-1) = (30/31) x 27 x 1 x (-1) = -26,14.
- Cobrança de reativação de US$ 21,30 pelo período de serviço de 10 de julho - 31 de julho. Reativações após 30 dias da data da compra resultam em uma cobrança proporcional. Cálculo = (30/31) x 22 x 1 = 21,30.

|**Custo inicial**   |**Final de encargo**   |**Preço unitário**   |**quantidade**   |**Quantidade**   |**Tipo de encargo** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|01/07/2018   |31/7/2018   |US$ 30  |1   |US$ 30   |Taxa do ciclo |
|05/07/2018   |31/7/2018   |   -US$ 26,14   |1   |-US$ 26,14|Taxa de cancelamento |
|10/07/2018   |31/7/2018   |-US$ 21,30   |1   |US$ 21,30|Taxa de ativação |

O arquivo de reconciliação de 15 de agosto conterá o seguinte:
- Cobrança de US$ 30 pelo período de serviço de 1º de agosto – 31 de agosto.

|**Custo inicial**   |**Final de encargo**   |**Preço unitário**   |**quantidade**   |**Quantidade**   |**Tipo de encargo** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|01/08/2018   |31/8/2018   |US$ 30  |1   |US$ 30   |Taxa do ciclo |

### <a name="scenario-8-change-of-license-quantity"></a>Cenário 8: Alteração da quantidade de licenças 

A data de cobrança do parceiro é no dia 15. Em 1º de junho, o parceiro compra uma nova assinatura por US$ 30 por mês. Em 10 de junho, o parceiro aumenta a quantidade de licenças de uma para duas licenças. O arquivo de reconciliação de 15 de junho conterá as seguintes linhas de cobrança:

- Cobrança de US$ 30 pelo período de serviço de 1º de junho – 30 de junho. Mesmo que o parceiro tenha aumentado a quantidade de licenças antes da data de cobrança de 15 de junho, o sistema de cobrança da Microsoft não reconhece a alteração até o dia de aniversário da assinatura, em 1º de julho.

|**Custo inicial**   |**Final de encargo**   |**Preço unitário**   |**quantidade**   |**Quantidade**   |**Tipo de encargo** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|01/06/2018   |30/06/2018   |US$ 30   |1   |US$ 30   |Taxas proporcionais durante a compra |

Em 1º de julho, o dia do aniversário da assinatura, o sistema de cobrança da Microsoft reconhecerá que a quantidade de licenças foi alterada de uma para duas em 10 de junho. O sistema de cobrança gerará um crédito e novas cobranças proporcionais para o período de serviço de 1º de junho - 9 de junho e 10 de junho - 30 de junho. 

O arquivo de reconciliação de 15 de julho conterá o seguinte:

- Crédito de -US$ 30 pelo período de serviço de 1º de junho - 30 de junho.
- Nova cobrança proporcional de US$ 9 pelo período de serviço de 1º de junho – 9 de junho. Nesse período o cliente tinha 1 licença. Cálculo = (preço mensal/total de dias no período de serviço) x dias no período de serviço proporcional x número de licenças = (30/30) x 9 x 1 = 9.
- Nova cobrança proporcional de US$ 42 pelo período de serviço de 10 de junho - 30 de junho. Nesse período o cliente tinha 2 licenças. Cálculo = (30/30) x 21 x 2 = 42.
- Cobrança de US$ 60 pelo período de serviço de 1º de julho – 31 de julho.

|**Custo inicial**   |**Final de encargo**   |**Preço unitário**   |**quantidade**   |**Quantidade**   |**Tipo de encargo** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|01/06/2018   |30/06/2018   |-US$ 30   |1   |-US$ 30|Proporcional à instância do ciclo |
|01/06/2018   |09/06/2018   |US$ 9   |1   |US$ 9|Proporcional à instância do ciclo |
|10/06/2018   |30/06/2018   |US$ 21   |2   |US$ 42|Proporcional à instância do ciclo |
|01/07/2018   |31/7/2018   |US$ 30   |2   |US$ 60   |Taxa do ciclo |

### <a name="scenario-9-add-on-subscriptions"></a>Cenário 9: Assinaturas de complemento

A data de cobrança do parceiro é no dia 15 do mês. Em 1º de junho, o parceiro compra uma nova assinatura de uma licença por US$ 30 por mês. Em 10 de junho, o parceiro compra uma nova assinatura de complemento por US$ 5 por mês. A data de renovação da assinatura de complemento será alinhada à data de renovação da assinatura base, que é 1º de junho. 

Em 10 de junho, o parceiro compra uma assinatura de complemento de uma licença por US$ 5 por mês. 

O arquivo de reconciliação de 15 de junho conterá as seguintes linhas de cobrança:

- Cobrança de US$ 30 pelo período de serviço de 1º de junho – 30 de junho. Isso é para a assinatura base.
- Cobrança proporcional de US$ 3,50 pelo período de serviço de 10 de junho – 30 de junho. Isso é para a assinatura de complemento. 

|**Custo inicial**   |**Final de encargo**   |**Preço unitário**   |**quantidade**   |**Quantidade**   |**Tipo de encargo** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|01/06/2018   |30/06/2018   |US$ 30   |1   |US$ 30   |Taxas proporcionais durante a compra |
|10/06/2018   |30/06/2018   |$3,50   |1   |$3,50   |Taxas proporcionais durante a compra |

O arquivo de reconciliação de 15 de julho conterá as seguintes linhas de cobrança:

- Cobrança de US$ 30 pelo período de serviço de 1º de julho – 31 de julho. Isso é para a assinatura base.
- Cobrança de US$ 5 pelo período de serviço de 1º de julho – 31 de julho. Isso é para a assinatura de complemento.

|**Custo inicial**   |**Final de encargo**   |**Preço unitário**   |**quantidade**   |**Quantidade**   |**Tipo de encargo** |
|-----------------|:-------------|:----------------|:------------|:------|-------|
|01/07/2018   |31/7/2018   |US$ 30   |1   |US$ 30   |Taxa do ciclo |
|01/07/2018   |31/7/2018   |US$ 5   |1   |US$ 5   |Taxa do ciclo |

Observe que a data de renovação automática da assinatura de complemento será 1º de junho de 2019, que se alinha à assinatura base.

### <a name="scenario-10-new-purchase-on-the-29th-30th-or-31st"></a>Cenário 10: Nova compra sobre o dia 29, 30 ou 31 

A data de cobrança do parceiro é no dia 15 do mês. Em 29 de maio, o parceiro compra uma nova assinatura de uma licença por US$ 30 por mês. As assinaturas compradas nos dias 29, 30 ou 31 terão um período gratuito da data da compra até o dia 1º do mês seguinte. O aniversário da assinatura padrão será no dia 1º. Nesse cenário, a assinatura receberá um período gratuito de 29 de maio até 31 de maio, e o período pago de 12 meses começará em 1º de junho. 

O arquivo de reconciliação de 15 de junho conterá as seguintes linhas de cobrança:

- Cobrança de US$ 30 pelo período de serviço de 1º de junho - 30 de junho.

|**Custo inicial**   |**Final de encargo**   |**Preço unitário**   |**quantidade**   |**Quantidade**   |**Tipo de encargo** |
|-----------------|:-------------|:----------------|:------------|:------|------|
|29/05/2018   | 30/06/2018   |US$ 30   |1   |US$ 30  |Taxas proporcionais durante a compra |

Observe que a assinatura será renovada automaticamente em 1º de junho de 2019.
