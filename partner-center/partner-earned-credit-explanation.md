---
title: Crédito ganho pelo parceiro para serviços gerenciados (versão prévia) | Partner Center
ms.topic: article
ms.date: 10/15/2019
description: Informações importantes sobre o crédito ganho pelo parceiro
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: high
ms.openlocfilehash: a20305b72bd3c72fe9aab21b9b7b48c7ce5104e6
ms.sourcegitcommit: 646536a113584f1572de851e22a212a6f77e64d7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/01/2019
ms.locfileid: "73428423"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a>Como o crédito ganho pelo parceiro é calculado e pago

O PEC (crédito ganho pelo parceiro para serviços gerenciados) reconhece e recompensa os parceiros que têm o controle operacional de TI 24x7 e o gerenciamento de partes – ou da totalidade – do ambiente do Azure de seus clientes. Por padrão, no CSP, os parceiros recebem os direitos de acesso necessários à assinatura do cliente, permitindo que eles executem o gerenciamento operacional 24x7 e o controle dos recursos na assinatura. Outras maneiras pelas quais o cliente pode provisionar acesso aos parceiros das transações estão descritas na seção a seguir. O valor da fatura mensal é líquido de créditos ganhos pelo parceiro. Os parceiros podem ver os detalhes do PEC em seu arquivo de reconhecimento mensal. Para ver outras maneiras pelas quais um cliente pode provisionar acesso ao parceiro de transações, leia [Gerenciar assinaturas e recursos no âmbito do plano do Azure](azure-plan-manage.md).

Leia também [Restabelecer privilégios de administrador para assinaturas do Azure CSP](revoke-reinstate-csp.md)

## <a name="important-eligibility-and-calculation-information"></a>Informações importantes de qualificação e cálculo

- O parceiro deve ter um contrato de MPN ativo e uma função de RBAC válida para receber os créditos ganhos nos ativos do Azure que eles gerenciam. 

- No caso de provedores indiretos e seus revendedores indiretos, o provedor indireto será qualificado para o PEC se ele ou o revendedor indireto (ou os dois) tiverem um controle operacional 24x7 e gerenciamento dos recursos do Azure do cliente no CSP.

- O PEC está associado ao consumo cobrado (passível de cobrança) da propriedade do Azure do cliente no CSP gerenciada pelo parceiro. O PEC é disponibilizado somente para parceiros no CSP cobrados pela Microsoft (provedor indireto e parceiro de cobrança direto). 

- Serviços qualificados: o crédito ganho pelo parceiro é aplicável aos serviços listados nos **preços de consumo do plano do Azure**, que os parceiros podem exportar da página de [preços do plano do Azure](https://partner.microsoft.com/commerce/sales). Observe que há exceções que incluem, mas não se limitam a, produtos de terceiros identificados como **De Terceiros** na coluna **Marcas** da lista de preços de consumo do plano do Azure, reservas do plano do Azure e produtos na lista de preços do Marketplace.

- O PEC é calculado diariamente e pode ser exibido no arquivo de uso diário e no arquivo reconhecimento de fatura mensal. Um parceiro (provedor indireto ou revendedor indireto) deve ter acesso ao dia inteiro (24x7) para garantir que eles obtenham o PEC.  

- O PEC é obtido no nível de recurso do Azure. Se o parceiro tiver acesso válido na assinatura ou no nível do grupo de recursos, cada recurso que role para a entidade mais alta receberá o PEC.  

- Os detalhes do PEC também estarão disponíveis no [Gerenciamento de Custos do Azure](https://go.microsoft.com/fwlink/?linkid=2106482)

## <a name="azure-cost-management"></a>Azure Cost Management

 O ACM (Gerenciamento de Custos do Azure), pelo uso da análise de custos, permite que você, na condição de parceiro, exiba os custos que receberam o benefício do PEC.  

1. No portal do Azure, entre no locatário do parceiro e selecione **Gerenciamento de Custos + Cobrança**.
2.  Selecione **Gerenciamento de custos**
3.  Selecione **Análise de Custo**

A exibição de Análise de Custo exibirá os custos da sua conta de cobrança para todos os serviços comprados e consumidos segundo os preços que você paga à Microsoft.

4.  Selecione **PartnerEarnedCreditApplied** no menu suspenso em um gráfico dinâmico para ver os custos que têm o PEC aplicado. Quando a propriedade **PartnerEarnedCreditApplied** é True, o custo associado tem o benefício do crédito ganho do parceiro. 

Quando a propriedade PartnerEarnedCreditApplied é False, o custo associado não atendeu à qualificação necessária para o crédito ou o serviço comprado não é elegível para crédito ganho do parceiro.

Observação: normalmente, o uso de serviços leva 8-24 horas para aparecer no **Gerenciamento de Custos** e os créditos do PEC aparecerão dentro de 48 horas a partir da hora de acesso no Gerenciamento de Custos do Azure.

5. Você também pode agrupar pela propriedade **PartnerEarnedCreditApplied** e filtrar por ela, usando os recursos de filtro **Agrupar por e Adicionar** para analisar os custos que têm o PEC aplicado e os custos que não têm nenhum PEC aplicado.

 **Para saber mais**

- [Crédito ganho pelo parceiro – visão geral](partner-earned-credit.md)

- Exemplos detalhados do cálculo dos créditos ganhos pelo parceiro estão localizados na lista de preços que você pode acessar por meio do Painel do Partner Center (requer credenciais).

- [Migrar para o plano do Azure – introdução](azure-plan-get-started.md)

- [Gerenciar assinaturas e recursos no âmbito do plano do Azure](azure-plan-manage.md)

- [Revogar ou restabelecer privilégios de administrador para assinaturas do Azure CSP ](revoke-reinstate-csp.md)

