---
title: Crédito ganho pelo parceiro para serviços gerenciados
ms.topic: article
ms.date: 12/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como o PEC (crédito ganho pelo parceiro) da Microsoft para serviços gerenciados é calculado e pago, além de como garantir que você esteja qualificado.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: f274103feeadfa6fd135f99632f3013c29601972
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182402"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a>Como o crédito ganho pelo parceiro é calculado e pago

**Funções apropriadas**

- Administrador global
- Administrador de usuários
- Agente administrativo
- Administrador de cobrança
- Agente de vendas

O PEC (crédito ganho pelo parceiro para serviços gerenciados) reconhece e recompensa os parceiros que têm o controle operacional de TI 24x7 e o gerenciamento de partes – ou da totalidade – do ambiente do Azure de seus clientes. Por padrão, no CSP, os parceiros recebem os direitos de acesso necessários à assinatura do cliente, permitindo que eles executem o gerenciamento operacional 24x7 e o controle dos recursos na assinatura. Outras maneiras pelas quais o cliente pode provisionar acesso aos parceiros das transações estão descritas na seção a seguir. O valor da fatura mensal é líquido de créditos ganhos pelo parceiro. Os parceiros podem ver os detalhes do PEC em seu arquivo de reconhecimento mensal. Para ver outras maneiras pelas quais um cliente pode provisionar acesso ao parceiro de transações, leia [Gerenciar assinaturas e recursos no âmbito do plano do Azure](azure-plan-manage.md).

Leia também [Restabelecer privilégios de administrador para assinaturas do Azure CSP](revoke-reinstate-csp.md)

## <a name="eligibility"></a>Qualificação

Para receber o PEC (crédito obtido por parceiro), os seguintes requisitos se aplicam: 

- Você precisa ter um contrato de MPN ativo e uma função RBAC (controle de acesso baseado em função) válida para receber o crédito obtido dos ativos do Azure gerenciados por você.

- Você precisa ter o controle operacional e o gerenciamento 24 horas por dia, 7 dias por semana dos recursos do Azure do cliente no CSP. Isso significa que você precisa ter privilégios de administrador na assinatura do Azure do cliente, no grupo de recursos do Azure e no recurso do Azure. No caso dos provedores indiretos e dos respectivos revendedores indiretos, o provedor indireto será qualificado para o PEC se ele ou o revendedor indireto ou ambos tiverem esse controle operacional. Para saber mais sobre isso, confira [Restabelecer privilégios de administrador para assinaturas do CSP do Azure](./revoke-reinstate-csp.md).

- Além dos requisitos acima, o PEC só é aplicável aos serviços listados no preço de consumo do plano do Azure, que pode ser exportado da página [Preços do plano do Azure](https://partner.microsoft.com/commerce/sales).

- O PEC **não** é aplicável aos seguintes serviços:
    - Reservas do plano do Azure
    - Produtos de terceiros identificados como Terceiros na coluna Marcas do preço de consumo do plano do Azure
    - Produtos da lista de preços do Marketplace
    - [Máquinas Virtuais Spot do Azure](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

- O PEC é obtido no nível de recurso do Azure. Se você tiver acesso válido no nível da assinatura ou do grupo de recursos, todos os recursos acumulados até a entidade mais alta receberão o PEC.

- Mais detalhes sobre o PEC também estão disponíveis na página [Gerenciamento de Custos do Azure](/azure/cost-management-billing/costs/get-started-partners).

### <a name="calculation"></a>Cálculo

O PEC é calculado diariamente e pode ser exibido no arquivo de uso diário e no arquivo reconhecimento de fatura mensal. Um parceiro (provedor indireto ou revendedor indireto) deve ter acesso ao dia inteiro (24x7) para garantir que eles obtenham o PEC. O PEC é calculado diariamente nos ativos gerenciados do Azure. O PEC máximo para um determinado período de cobrança (mês) é 15%. Os parceiros que retêm o acesso privilegiado persistente durante o mês (período de acesso) e para todos os recursos qualificados (escopo de acesso) ganharão o PEC completo de 15%. A redução de escopo e período resultará em uma taxa menor de PEC para o mês. O arquivo de uso com classificação diária é mostrado diariamente em um ativo do Azure, independentemente de o PEC ser aplicado ou não. Os parceiros também podem se registrar para receber alertas e monitorar se há alterações no acesso privilegiado persistente.

## <a name="azure-cost-management"></a>Azure Cost Management

O ACM (Gerenciamento de Custos do Azure), pelo uso da análise de custos, permite que você, na condição de parceiro, exiba os custos que receberam o benefício do PEC.  

1. No [portal do Azure](https://portal.azure.com), entre no locatário do parceiro e selecione **Cobrança + Gerenciamento de Custos**.

2. Selecione **Gerenciamento de custos**

3. Selecione **Análise de Custo**

   A exibição de Análise de Custo exibirá os custos da sua conta de cobrança para todos os serviços comprados e consumidos segundo os preços que você paga à Microsoft.

4. Selecione **PartnerEarnedCreditApplied** no menu suspenso em um gráfico dinâmico para ver os custos que têm o PEC aplicado. Quando a propriedade **PartnerEarnedCreditApplied** é True, o custo associado tem o benefício do crédito ganho do parceiro. 

   Quando a propriedade PartnerEarnedCreditApplied é False, o custo associado não atendeu à qualificação necessária para o crédito ou o serviço comprado não é elegível para crédito ganho do parceiro.

   >[!NOTE] 
   >Normalmente, o uso de serviços leva de 8 a 24 horas para aparecer no **Gerenciamento de Custos**, e os créditos do PEC aparecerão dentro de 48 horas a partir da hora de acesso no Gerenciamento de Custos do Azure.

5. Você também pode agrupar pela propriedade **PartnerEarnedCreditApplied** e filtrar por ela, usando os recursos de filtro **Agrupar por e Adicionar** para analisar os custos que têm o PEC aplicado e os custos que não têm nenhum PEC aplicado.

## <a name="next-steps"></a>Próximas etapas

- [Crédito ganho pelo parceiro – visão geral](partner-earned-credit.md)

- Exemplos detalhados do cálculo dos créditos ganhos pelo parceiro estão localizados na lista de preços que você pode acessar por meio do Painel do Partner Center (requer credenciais).

- [Migrar para o plano do Azure – introdução](azure-plan-get-started.md)

- [Gerenciar assinaturas e recursos no âmbito do plano do Azure](azure-plan-manage.md)

- [Revogar ou restabelecer privilégios de administrador para assinaturas do CSP do Azure](revoke-reinstate-csp.md)