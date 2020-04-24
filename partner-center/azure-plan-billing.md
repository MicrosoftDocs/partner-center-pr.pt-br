---
title: Cobrança do plano do Azure | Partner Center
ms.topic: article
ms.date: 02/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como acessar e entender a estrutura do arquivo de reconciliação e da fatura relacionada à cobrança do plano do Azure.
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: High
ms.openlocfilehash: 2184733bbbfb5fa3beede2cb45cb409109f11bad
ms.sourcegitcommit: 449cb8c32880217ad7543712b02a84ae69869289
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2020
ms.locfileid: "78240233"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a>Nova experiência de comércio no CSP – Cobrança do Azure 

**Funções apropriadas:**

- Agente administrativo
- Administrador de cobrança
- Administrador global

A cobrança no âmbito do plano do Azure é uma experiência de cobrança simplificada usando uma data de cobrança única alinhada e um período de cobrança baseado no mês civil.

## <a name="summary-of-billing-essentials"></a>Resumo dos conceitos básicos de cobrança

- **Data da fatura**: A fatura e o arquivo de reconciliação estarão disponíveis na API/no Painel do Partner Center até o dia oito (à meia-noite, UTC).

- **Período de cobrança da fatura**: O período de cobrança da fatura é alinhado ao mês civil, por exemplo, 1/10 – 31/10, 1/11 – 30/11.

- **Períodos de serviço de cobrança**: As cobranças serão alinhadas ao mês civil. Por exemplo, se o parceiro cobrado adicionar serviços do Azure por meio de um plano do Azure em 15/10 e o cliente iniciar o consumo de serviços do Azure em 10/15, então o parceiro cobrado receberá a fatura/o reconhecimento em 8/11 para o consumo do cliente referente ao período de serviço 15/10 – 31/10. A fatura do próximo mês, que será gerada em 08/12, conterá todos os encargos referentes ao período de serviço de 01/11 – 31/11.

- **Condição de pagamento da fatura**: Líquido de 60 dias.

- **Moeda da fatura**: Os parceiros continuarão sendo cobrados na moeda atribuída ao país do cliente. Por exemplo, se o parceiro cobrado estiver na Irlanda com clientes no Reino Unido, na Noruega e na Alemanha, ele receberá faturas/reconhecimentos em GBP, NOK e EUR.

- **Incentivos para Parceiros**: pago 45 dias após o final do mês da fatura.

## <a name="access-your-invoices-and-reconciliation-files"></a>Acessar seus arquivos de fatura e reconciliação

O administrador global ou de cobrança da sua empresa receberá um email quando a fatura estiver pronta para ser exibida. 

**Para acessar o arquivo de fatura e reconciliação**

1. Entre no [Painel](https://partner.microsoft.com/en-us/dashboard/) do Partner Center.

2. No menu do Partner Center, selecione **Cobrança**.

3. Selecione a guia para a **Recorrente** e a **Única** e a moeda em que você está interessado.

![cobrança](images/azure/billing3.png)

4. Selecione **Fatura** ou **Arquivo de reconciliação**.  

Para exibir os arquivos históricos de faturas e reconhecimento, expanda a linha do histórico de cobrança, abaixo.


## <a name="understanding-usage-data"></a>Noções básicas sobre dados de uso 

1. O plano do Azure é o contêiner raiz ou de nível superior para uso. Todo o uso é vinculado de volta a um único plano do Azure. 

2. Em um plano, haverá uma ou mais assinaturas do Azure. Esses são contêineres usados para gerenciamento de recursos e implantação. 

3. Em uma assinatura, os grupos de recursos são adicionados aos recursos de grupo. Cada recurso é implantado em um grupo de recursos. 

4. Exemplos de recursos incluem máquinas virtuais e contas de armazenamento. 

5. Medidores de emissão de recurso: Os medidores são medidas de consumo de um recurso, sendo que um recurso pode emitir o uso de vários medidores. Os medidores são identificados por um ProductId, um SKUId e um AvailabilityId. 

### <a name="heirarchy-of-subscription-resource-groups-and-metering"></a>Hierarquia de grupos de recursos de assinatura e medição

**Conta do Azure (locatário)**

- Assinatura A
    - ResourceGroup 1
        - Máquina virtual (recurso)
            - Medidor de computação
        - Rede virtual (recurso)
            - Sem medidor de cobrança

    - ResourceGroup 2
        - Máquina virtual (recurso)
            - Medidor do computador
        - Disco gerenciado SSD Premium (recurso)
            - Medidor de capacidade de armazenamento
            - Medidor de operações de armazenamento

- Assinatura B   – ResourceGroup 1       – SQL do Azure (recurso)           – medidor DTU       – Gateway de VPN (recurso)           – medidor de Gateway de VPN

    - ResourceGroup 2
        - Adaptador de rede virtual (recurso)
            - Sem medidor de cobrança

## <a name="read-the-invoice"></a>Leia a fatura

1. A fatura estará disponível até o dia oito de cada mês.

2. Os parceiros têm 60 dias para remeterem o pagamento.

3. O período de cobrança abrangerá um determinado mês civil, por exemplo, de 1/10 – 31/10.

4. As cobranças são líquidas de ajustes (o valor é líquido de "Créditos ganhos pelo parceiro para serviços gerenciados").

5. Examine o arquivo de reconhecimento de fatura e o arquivo de uso de classificação diária para obter detalhes adicionais de cobrança.

![fatura](images/azure/invoice1.png)

## <a name="read-the-invoice-reconciliation-file"></a>Ler o arquivo de reconciliação/fatura

1. Cada combinação de plano e medidor do Azure pode ter até duas linhas de cobrança no arquivo de reconciliação.

2. Se o medidor for qualificado para qualquer tipo de desconto ou crédito (como descontos por nível ou créditos ganhos pelo parceiro para serviços gerenciados) durante todo o mês civil, então o arquivo de reconciliação conterá apenas uma linha de cobrança. A coluna **PriceAdjusmentDescription** fará referência ao desconto ou crédito obtido.

3. Se não houver recursos para um medidor específico qualificado para o desconto ou créditos ganhos pelo parceiro, então o arquivo de reconciliação conterá apenas uma linha de cobrança e o preço unitário efetivo será o preço de varejo (que é o preço unitário).

4. Se o medidor ou quaisquer recursos que emitam esse medidor se qualificaram para **Créditos ganhos pelo parceiro para serviços gerenciados** em uma parte do mês, então o arquivo de reconciliação conterá duas linhas de cobrança. Uma linha representará os dias em que o medidor se qualificou, ao passo que a outra linha representará os dias em que o medidor não se qualificou. 

## <a name="read-the-daily-usage-file"></a>Ler o arquivo de uso diário

- Os medidores de assinatura no âmbito de um plano do Azure são classificados e acumulados diariamente. 

- **O crédito ganho pelo parceiro para serviços gerenciados** é determinado e aplicado diariamente.

- Cada medidor de assinatura terá uma linha para cada dia do mês em que houve consumo.

- No exemplo a seguir:

  - O medidor se qualificou para **Crédito ganho pelo parceiro para serviços gerenciados** de 01/07 – 03/07 (observe que o preço unitário efetivo é o preço de varejo menos os créditos ganhos pelo parceiro).

   - O medidor não se qualificou para **Crédito ganho pelo parceiro para serviços gerenciados** de 04/07 – 07/07 (observe que o preço unitário efetivo é o preço de varejo).

    - O medidor se qualificou para **Crédito ganho pelo parceiro para serviços gerenciados** de 08/07 – 31/07 (observe que o preço unitário efetivo é o preço de varejo menos os créditos ganhos pelo parceiro).

![recon2](images/azure/pecfinal.png) 

## <a name="invoice-in-customer-currency"></a>Fatura na moeda do cliente 

Os serviços do Azure por meio de um plano do Azure serão precificados em USD e cobrados na moeda atribuída ao país do cliente. Se a moeda de cobrança não for USD, então a taxa de câmbio usada será mostrada na última página da fatura. As taxas de câmbio são determinadas mensalmente e aplicadas à fatura a seguir. Para obter uma lista completa de moedas por país, exiba a [matriz de moedas do cliente e a disponibilidade por país de novas ofertas de comércio](https://go.microsoft.com/fwlink/?linkid=2112354). 

A Microsoft usará o [Thomson Reuters](https://developers.thomsonreuters.com/content/wm-company) para estabelecer a taxa de câmbio usada para determinar a moeda de preço para a conversão de moeda da cobrança. As taxas de câmbio serão atualizadas e disponibilizadas no dia anterior ao primeiro dia de cada mês em que forem aplicadas.

**Exemplo**:  Os encargos de uso do período de serviço de 1º de agosto a 31 de agosto serão cobrados usando a taxa de câmbio publicada no dia 31 de julho. Esses encargos serão exibidos na fatura de setembro e a taxa de câmbio poderá ser observada na última página da fatura. 

 
## <a name="azure-reservations"></a>Reservas do Azure 

Ao comprar [Reservas do Azure](https://docs.microsoft.com/partner-center/azure-reservations) por meio de um plano do Azure, inicialmente, só será possível escolher a cobrança única no Partner Center. A cobrança mensal está disponível no portal do Azure. A cobrança mensal será disponibilizada no Partner Center em uma data posterior. 

## <a name="azure-spending"></a>Gastos do Azure 

A experiência de gastos do Azure existente é atualizada para dar suporte à nova cobrança do plano do Azure no Partner Center. Isso permite aos parceiros:

- exibir, gerenciar e receber alertas do conjunto de orçamentos em um nível de cliente; 

- exibir o gasto total estimado em um plano do Azure (dividido por recurso e nível de medidor)

Já que o modelo de cobrança para os serviços do Azure por meio de um plano do Azure é o consumo pós-pago, para evitar uma cobrança maior do que o previsto, os parceiros podem aplicar um orçamento mensal e acompanhar o percentual de uso. Um orçamento pode ser aplicado a um cliente ou a vários clientes ao mesmo tempo. 

![Gastos do Azure](images/azure/azurespend.png)

**Para obter mais informações**

-  Como o PEC (crédito ganho pelo parceiro) é calculado está localizado na lista de preços disponível por meio do [Painel](https://partner.microsoft.com/en-us/dashboard/) do Partner Center (é necessário entrar). 
   
-  [Comprar o plano do Azure](purchase-azure-plan.md)

-  [Lista de preços para a nova experiência de comércio no CSP](azure-plan-price-list.md)
