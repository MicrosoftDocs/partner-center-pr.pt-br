---
title: Plano do Azure – Cobrança | Partner Center
ms.topic: article
ms.date: 10/04/2019
description: Descreve a estrutura de arquivos de faturamento e reconhecimento
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: High
ms.openlocfilehash: 28e670635ca7fcff60041fcb5c93b3ddd5e4069d
ms.sourcegitcommit: cd90a59ff0ea81197b603abcb7bf462c4fb1edbe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2019
ms.locfileid: "72171297"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a>Nova experiência de comércio no CSP – Cobrança do Azure 

A cobrança no âmbito do plano do Azure é uma experiência de cobrança simplificada usando uma data de cobrança única alinhada e um período de cobrança baseado no mês civil. Para obter informações sobre a plataforma de cobrança, leia [Guia operacional de comércio moderno do Partner Center](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx).

## <a name="summary-of-billing-essentials"></a>Resumo dos conceitos básicos de cobrança

- **Data da fatura**: A fatura e o arquivo de reconciliação estarão disponíveis na API/no Painel do Partner Center até o dia oito (à meia-noite, UTC).

- **Período de cobrança da fatura**: O período de cobrança da fatura é alinhado ao mês civil, por exemplo, 1/10 – 31/10, 1/11 – 30/11.

- **Períodos de serviço de cobrança**: As cobranças serão alinhadas ao mês civil. Por exemplo, se o parceiro cobrado adicionar serviços do Azure por meio de um plano do Azure em 15/10 e o cliente iniciar o consumo de serviços do Azure em 10/15, então o parceiro cobrado receberá a fatura/o reconhecimento em 8/11 para o consumo do cliente referente ao período de serviço 15/10 – 31/10. A fatura do próximo mês, que será gerada em 8/12, conterá todos os encargos referentes ao período de serviço de 1/11 – 31/11.

- **Condição de pagamento da fatura**: Líquido de 60 dias.

- **Moeda da fatura**: Os parceiros continuarão sendo cobrados na moeda atribuída ao país do cliente. Por exemplo, se o parceiro cobrado estiver na Irlanda com clientes no Reino Unido, na Noruega e na Alemanha, ele receberá faturas/reconhecimentos em GBP, NOK e EUR.

- **Incentivos para Parceiros**: pago 45 dias após o final do mês da fatura.

##  <a name="access-your-invoices-and-recon-files"></a>Acessar seus arquivos de fatura e reconhecimento

O administrador global ou de cobrança da sua empresa receberá um email quando a fatura estiver pronta para ser exibida. 

**Para acessar o arquivo de fatura e reconhecimento**

1. Entre no Partner Center.

2. No menu do Partner Center, selecione **Cobrança**.

3. Selecione a guia para **baseado em calendário** e moeda em que você está interessado.

![cobrança](images/azure/billing1.png)

4. Selecione **arquivo de Fatura e Reconhecimento**.  

Para exibir os arquivos históricos de faturas e reconhecimento, expanda a linha do histórico de cobrança, abaixo.

## <a name="read-the-invoice"></a>Leia a fatura

1. A fatura estará disponível até o dia oito de cada mês.

2. Os parceiros têm 60 dias para remeterem o pagamento.

3. O período de cobrança abrangerá um determinado mês civil, por exemplo, de 1/10 – 31/10.

4. As cobranças são líquidas de ajustes (o valor é líquido de "Créditos ganhos pelo parceiro para serviços gerenciados").

5. Examine o arquivo de reconhecimento de fatura e o arquivo de uso de classificação diária para obter detalhes adicionais de cobrança.

![fatura](images/azure/invoice1.png)

## <a name="read-the-recon-file"></a>Ler o arquivo de reconhecimento

1. Cada medidor da assinatura do Azure pode ter até duas linhas de cobrança no arquivo reconhecimento.

2. Se o medidor for qualificado para qualquer tipo de desconto ou crédito (como descontos de nível 1 ou créditos ganhos pelo parceiro para serviços gerenciados) durante todo o mês civil, então o arquivo de reconhecimento conterá apenas uma linha de cobrança. A coluna **PriceAdjusmentDescription** fará referência ao desconto ou ao crédito ganho; o preço unitário efetivo será o preço de varejo menos o crédito ganho pelo parceiro ou outros descontos eventualmente aplicados.

3. Se o medidor não se qualificou para os créditos ganhos pelo parceiro para serviços gerenciados durante todo o mês civil, então o arquivo de reconhecimento conterá apenas uma linha de cobrança e o preço unitário efetivo será o preço de varejo (que é o preço unitário).

4. Se o medidor se qualificou para **Créditos ganhos pelo parceiro para serviços gerenciados** em uma parte do mês, então o arquivo de reconhecimento conterá duas linhas de cobrança. Uma linha representará os dias em que o medidor se qualificou, ao passo que a outra linha representará os dias em que o medidor não se qualificou. 

## <a name="read-the-daily-usage-file"></a>Ler o arquivo de uso diário

- Os medidores de assinatura no âmbito de um plano do Azure são classificados e acumulados diariamente. 

- **O crédito ganho pelo parceiro para serviços gerenciados** é determinado e aplicado diariamente.

- Cada medidor de assinatura terá uma linha para cada dia do mês em que houve consumo.

- No exemplo a seguir:

  - O medidor se qualificou para **Crédito ganho pelo parceiro para serviços gerenciados** de 01/07 – 03/07 (observe que o preço unitário efetivo é o preço de varejo menos os créditos ganhos pelo parceiro).

   - O medidor não se qualificou para **Crédito ganho pelo parceiro para serviços gerenciados** de 04/07 – 07/07 (observe que o preço unitário efetivo é o preço de varejo).

    - O medidor se qualificou para **Crédito ganho pelo parceiro para serviços gerenciados** de 08/07 – 31/07 (observe que o preço unitário efetivo é o preço de varejo menos os créditos ganhos pelo parceiro).

![recon2](images/azure/billing2.png) 

## <a name="invoice-in-customer-currency"></a>Fatura na moeda do cliente 

Os serviços do Azure por meio de um plano do Azure serão precificados em USD e cobrados na moeda atribuída ao país do cliente. Se a moeda de cobrança não for USD, então a taxa de câmbio usada será mostrada na última página da fatura. As taxas de câmbio são determinadas mensalmente e aplicadas à fatura a seguir. Para obter a lista completa das moedas dos países, consulte a [Matriz de moedas do cliente e disponibilidade por país de novas ofertas de comércio](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3Qn1V). 

A Microsoft usará o [Thompson Reuters](https://developers.thomsonreuters.com/content/wm-company) para estabelecer a taxa de câmbio usada para determinar a moeda de preço para a conversão de moeda da fatura. A taxa de câmbio será atualizada e disponibilizada no dia anterior ao primeiro dia de cada mês em que ela será aplicada.

**Exemplo**:  Os encargos de uso do período de serviço de 1º de agosto a 31 de agosto serão cobrados usando a taxa de câmbio publicada no dia 1º de agosto. Esses encargos serão exibidos na fatura de setembro e a taxa de câmbio poderá ser observada na última página da fatura. 

Os usuários do locatário do parceiro continuarão a ver informações relacionadas à função específica sobre todos os clientes e todos os pedidos, independentemente da moeda de cobrança. Além disso, o usuário poderá ver todas as faturas em todas as moedas.  
 
## <a name="azure-reservations"></a>Reservas do Azure 

Ao comprar [Reservas do Azure](https://docs.microsoft.com/partner-center/azure-reservations) por meio de um plano do Azure, inicialmente, só será possível escolher a cobrança única no Partner Center. A cobrança mensal está disponível no portal do Azure. A cobrança mensal será disponibilizada no Partner Center em uma data posterior. 

## <a name="azure-cost-management"></a>Gerenciamento de Custos do Azure 

As ferramentas de Gerenciamento de Custos do Azure ajudarão as organizações a visualizar, gerenciar e otimizar os custos em todo o Microsoft Azure. Esse recurso estará disponível na portal do Azure. Os parceiros terão uma solução sempre ativa e de baixa latência com os seguintes recursos disponíveis: 

- Análise e alertas de orçamento mais abundantes 
- APIs e conectores do Power BI 
- Exibição de vários clientes 
- Gratuito para gerenciar os custos do Azure 
- Expansão de funções/usuários 

Consulte o [Gerenciamento de Custos do Azure](https://azure.microsoft.com/services/cost-management) para obter mais informações sobre esse recurso, que foi disponibilizado para contratos corporativos em fevereiro de 2019. Isso está disponível somente com os serviços do Azure adquiridos como parte dessa nova experiência se comércio do Azure no CSP. 
 
## <a name="azure-spending"></a>Gastos do Azure 

Uma ferramenta de gastos do Azure estará disponível no Partner Center para a nova experiência de comércio no CSP. Quando aplicada, essa funcionalidade permitirá que os parceiros enxerguem:  

- O orçamento total de um cliente 
- O total de gastos estimados em um plano do Azure existente 
- O percentual de uso de clientes em cada período de cobrança 

Como o modelo de cobrança para os serviços do Azure por meio de um plano do Azure é o consumo pós-pago, para evitar uma cobrança maior do que o previsto, os parceiros podem aplicar um orçamento mensal e acompanhar o percentual de uso. Um orçamento pode ser aplicado a um cliente ou a vários clientes ao mesmo tempo. 

![Gastos do Azure](images/azure/azurespend.png)

**Para saber mais**

-  Como o PEC (crédito ganho pelo parceiro) é calculado está localizado na lista de preços disponível por meio do Painel do Partner Center. 
   
-  [Comprar o plano do Azure](purchase-azure-plan.md)

-  [Lista de preços para a nova experiência de comércio no CSP](azure-plan-price-list.md)
