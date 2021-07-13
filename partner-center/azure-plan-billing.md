---
title: Cobrança do plano do Azure – arquivos de reconciliação e fatura
ms.topic: article
ms.date: 05/19/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como acessar e entender a estrutura do arquivo de reconciliação e da fatura relacionada à cobrança do plano do Azure.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: c7c06f5ed7b147625afb5020f63ead411ef58fa8
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551513"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a>Nova experiência de comércio no CSP – Cobrança do Azure 

**Funções apropriadas**: Agente administrativo | Administrador de cobrança | Administrador global

Este artigo explica como acessar e entender a estrutura do arquivo de reconciliação e da fatura relacionada à cobrança do plano do Azure. A cobrança no âmbito do plano do Azure é uma experiência de cobrança simplificada usando uma data de cobrança única alinhada e um período de cobrança baseado no mês civil.

## <a name="summary-of-billing-essentials"></a>Resumo dos conceitos básicos de cobrança

- **Data da fatura**: A fatura e o arquivo de reconciliação estarão disponíveis na API/no Painel do Partner Center até o dia oito (à meia-noite, UTC).

- **Período de cobrança da fatura**: O período de cobrança da fatura é alinhado ao mês civil, por exemplo, 1/10 – 31/10, 1/11 – 30/11.

- **Períodos de serviço de cobrança**: As cobranças serão alinhadas ao mês civil. Por exemplo, se o parceiro cobrado adicionar serviços do Azure por meio de um plano do Azure em 15/10 e o cliente iniciar o consumo de serviços do Azure em 10/15, então o parceiro cobrado receberá a fatura/o reconhecimento em 8/11 para o consumo do cliente referente ao período de serviço 15/10 – 31/10. A fatura do próximo mês, que será gerada em 08/12, conterá todos os encargos referentes ao período de serviço de 01/11 – 31/11.

- **Condição de pagamento da fatura**: Líquido de 60 dias.

- **Moeda da fatura**: Desde 28 de janeiro de 2021, os parceiros da região da EU/EFTA e do Reino Unido que têm novos clientes e clientes CSP existentes que adquiriram novas ofertas de comércio pela primeira vez cujos locatários foram criados antes de 11 de maio de 2020 estão sendo cobrados por essas compras na moeda da localização do parceiro. Os parceiros localizados fora da região da EU/EFTA e do Reino Unido continuarão sendo cobrados na moeda da localização do parceiro.

- **Incentivos para Parceiros**: pago 45 dias após o final do mês da fatura.

## <a name="access-your-invoices-and-reconciliation-files"></a>Acessar seus arquivos de fatura e reconciliação

O administrador global ou de cobrança da sua empresa receberá um email quando a fatura estiver pronta para ser exibida.

Para acessar o arquivo de fatura e reconciliação:

1. Entre no [Painel](https://partner.microsoft.com/dashboard/) do Partner Center.

2. No menu do Partner Center, selecione **Cobrança**.

3. Selecione a guia para a **Recorrente** e a **Única** e a moeda em que você está interessado.

   :::image type="content" source="images/azure/billing3.png" alt-text="cobrança.":::

4. Selecione **Fatura** ou **Arquivo de reconciliação**.  

   Para exibir os arquivos históricos de faturas e reconhecimento, expanda a linha do histórico de cobrança, abaixo.

## <a name="understanding-usage-data"></a>Noções básicas sobre dados de uso 

1. O plano do Azure é o contêiner raiz ou de nível superior para uso. Todo o uso está vinculado de volta a um único plano do Azure.

2. Em um plano, haverá uma ou mais assinaturas do Azure. Esses são contêineres usados para gerenciamento de recursos e implantação. 

3. Em uma assinatura, os grupos de recursos são adicionados aos recursos de grupo. Cada recurso é implantado em um grupo de recursos. 

4. Exemplos de recursos incluem máquinas virtuais e contas de armazenamento. 

5. Medidores de emissão de recurso: Os medidores são medidas de consumo de um recurso, sendo que um recurso pode emitir o uso de vários medidores. Os medidores são identificados por um ProductId, um SKUId e um AvailabilityId. 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a>Hierarquia de grupos de recursos de assinatura e medição

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
        - Disco gerenciado por SSD Premium (recurso)
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

   :::image type="content" source="images/azure/invoice1.png" alt-text="fatura.":::

## <a name="read-the-invoice-reconciliation-file"></a>Ler o arquivo de reconciliação/fatura

1. Cada combinação de plano e medidor do Azure pode ter até duas linhas de cobrança no arquivo de reconciliação.

2. Se o medidor for qualificado para qualquer tipo de desconto ou crédito (como descontos por nível ou créditos ganhos pelo parceiro para serviços gerenciados) durante todo o mês civil, então o arquivo de reconciliação conterá apenas uma linha de cobrança. A coluna **PriceAdjusmentDescription** fará referência ao desconto ou crédito obtido.

3. Se não houver recursos para um medidor específico qualificado para o desconto ou créditos ganhos pelo parceiro, então o arquivo de reconciliação conterá apenas uma linha de cobrança e o preço unitário efetivo será o preço de varejo (que é o preço unitário).

4. Se o medidor, ou os recursos que emitirem esse medidor, tiver se qualificado para **Créditos ganhos pelo parceiro para serviços gerenciados** em uma parte do mês, então o arquivo de reconciliação conterá duas linhas de cobrança. Uma linha representará os dias em que o medidor se qualificou, ao passo que a outra linha representará os dias em que o medidor não se qualificou.

>[!NOTE]
>Você pode reconciliar o consumo do Azure em seu arquivo único de reconhecimento de compra. Para fazer isso, acesse o arquivo de reconhecimento de uso com classificação diária e pesquise sua SubscriptionID. Isso exibirá todos os custos associados à sua ID do Plano do Azure. Sua SubscriptionID do Azure é mostrada como EntitlementID.

## <a name="read-the-daily-usage-file"></a>Ler o arquivo de uso diário

- Os medidores de assinatura no âmbito de um plano do Azure são classificados e acumulados diariamente.

- **O crédito ganho pelo parceiro para serviços gerenciados** é determinado e aplicado diariamente.

- Cada medidor de assinatura terá uma linha para cada dia do mês em que houve consumo.

- No exemplo a seguir:

  - O medidor se qualificou para **Crédito ganho pelo parceiro para serviços gerenciados** de 01/07 – 03/07 (observe que o preço unitário efetivo é o preço de varejo menos os créditos ganhos pelo parceiro).

  - O medidor não se qualificou para **Crédito ganho pelo parceiro para serviços gerenciados** de 04/07 – 07/07 (observe que o preço unitário efetivo é o preço de varejo).

  - O medidor se qualificou para **Crédito ganho pelo parceiro para serviços gerenciados** de 08/07 – 31/07 (observe que o preço unitário efetivo é o preço de varejo menos os créditos ganhos pelo parceiro).

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2.":::

## <a name="invoice-in-customer-currency"></a>Fatura na moeda do cliente

Os serviços do Azure por meio de um plano do Azure serão precificados em USD e cobrados na moeda atribuída ao país do cliente. Se a moeda de cobrança não for USD, então a taxa de câmbio usada será mostrada na última página da fatura. As taxas de câmbio são determinadas mensalmente e aplicadas à fatura a seguir. Para obter uma lista completa de moedas por país, exiba a [matriz de moedas do cliente e a disponibilidade por país de novas ofertas de comércio](https://go.microsoft.com/fwlink/?linkid=2112354).

A Microsoft aplica uma taxa de câmbio predeterminada aos preços base em USD para chegar aos encargos totais incorridos para serviços do Azure comprados ou consumidos a cada mês calendário. A taxa de câmbio mensal é a taxa média publicada pela Thomson Reuters (normalmente) dois dias úteis antes do fim do mês anterior às 16h GMT. 

**Por exemplo,** a taxa de câmbio de dezembro da Microsoft seria a taxa média da Thomson Reuters no dia 29 de novembro ou perto dessa data para uma determinada moeda. Essa taxa será aplicada a todas as compras nessa moeda de 1º de dezembro a 31 de dezembro. 

## <a name="azure-reservations"></a>Reservas do Azure


Se você estiver comprando [reservas do Azure](azure-reservations.md) por meio de um plano do Azure, escolha a cobrança única ou mensal.


## <a name="azure-spending"></a>Gastos do Azure

A experiência de gastos do Azure existente é atualizada para dar suporte à nova cobrança do plano do Azure no Partner Center. Isso permite aos parceiros:

- exibir, gerenciar e receber alertas do conjunto de orçamentos em um nível de cliente; 

- exibir o gasto total estimado em um plano do Azure (dividido por recurso e nível de medidor)

Já que o modelo de cobrança para os serviços do Azure por meio de um plano do Azure é o consumo pós-pago, para evitar uma cobrança maior do que o previsto, os parceiros podem aplicar um orçamento mensal e acompanhar o percentual de uso. Um orçamento pode ser aplicado a um cliente ou a vários clientes ao mesmo tempo. 

:::image type="content" source="images/azure/azurespend.png" alt-text="Gastos do Azure.":::

## <a name="next-steps"></a>Próximas etapas

- Veja como o PEC (crédito ganho pelo parceiro) é calculado. Entre no [Painel](https://partner.microsoft.com/dashboard/) do Partner Center e localize a lista de preços disponível.

- Saiba mais sobre [como comprar o plano do Azure](purchase-azure-plan.md)

- Veja a [lista de preços para a nova experiência de comércio no CSP](azure-plan-price-list.md)
