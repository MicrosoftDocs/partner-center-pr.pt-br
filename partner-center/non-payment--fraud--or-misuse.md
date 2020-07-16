---
title: Gerenciamento de não pagamento, fraude ou uso indevido
description: É importante saber mais sobre os vários riscos envolvidos em transações online e as práticas recomendadas para gerenciar e atenuar esses riscos.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 07/14/2020
ms.openlocfilehash: ad0ef9c7aa242645ed0ffef0d5bbb07521edbc72
ms.sourcegitcommit: 9dcdd1225f62a9d9019e72ed12324cdba962fd1a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2020
ms.locfileid: "86405557"
---
# <a name="managing-non-payment-fraud-or-misuse-in-partner-center"></a>Gerenciamento de não pagamento, fraude ou uso indevido no Partner Center

Aplica-se a:

- Partner Center
- Partner Center do Microsoft Cloud for US Government

**Funções apropriadas**
- Administrador global
- Administrador de usuários
- Agente administrativo
- Administrador de cobrança

Você permanece financeiramente responsável por compras fraudulentas de seus clientes e/ou falta de pagamento de serviços comprados pelo cliente. Portanto, é *altamente recomendável que você coloque controles de mitigação de risco de detecção e prevenção de fraudes*.

Para evitar e/ou resolver atividade fraudulenta ou uso indevido, é importante entender os riscos em potencial e desenvolver políticas e práticas que possam reduzir a exposição.

## <a name="enforcement-of-microsoft-acceptable-use-policy"></a>Imposição da política de uso aceitável da Microsoft

Se a Microsoft detectar a atividade de parceiro ou de cliente que confirmamos ou suspeita violar a política de uso aceitável, usaremos etapas de imposição. O cliente pode ser suspenso imediatamente. Você será notificado sobre as ações de imposição ou atualizadas sobre suas solicitações pela Microsoft.

## <a name="abuse-of-service-risks"></a>Abuso de riscos de serviço

**Abuso de riscos de serviço** significa clientes que usam serviços de nuvem violando a política de uso aceitável da Microsoft.

### <a name="examples-of-abuse-of-service"></a>Exemplos de abuso de serviço

Exemplos dessas violações da política de uso aceitável da Microsoft podem incluir:

- Spam
- Pirataria
- Ataques de DDoS (negação de serviço distribuído)
- Mineração de bitcoins
- Distribuição de malware
- Revenda de assinaturas pirateadas

## <a name="theft-of-service-risks"></a>Roubo de riscos de serviço

**Roubo de riscos de serviço** significa clientes que não têm intenção de pagar por serviços consumidos. Esse roubo pode envolver o uso de instrumentos de pagamento roubados, fornecendo informações de cobrança falsas e/ou padronizando os saldos pendentes.

### <a name="examples-of-service-theft"></a>Exemplos de roubo de serviço

Exemplos desses riscos de transação online podem incluir:

- Transações que não ocorrem pessoalmente (transações de "cartão de crédito não presente")
- Identidades fraudulentas
- Serviços provisionados e usados antes de o pagamento inicial ser recebido
- Mercados emergentes e/ou regiões de alto risco para fraudes online
- Automatizar a criação e a compra de contas por atores ruins

## <a name="managing-online-risk"></a>Gerenciando riscos online

Você pode usar as seguintes recomendações para ajudá-lo a desenvolver políticas e práticas para reduzir sua exposição a riscos de transações online no ciclo de vida de suas relações com o cliente.

### <a name="onboarding-new-customers"></a>Integração de novos clientes

Sugestões para reduzir riscos online ao integrar novos clientes incluem:

- Estabeleça relações pessoais com os clientes quando possível (por exemplo, contato com clientes por telefone).
- Verifique as credenciais e o plano de fundo dos clientes por meio de métodos melhores (como o uso de centrais de créditos ou agências de relatórios comerciais comerciais).
- Use a autenticação multifator (como verificação de SMS) durante a inscrição para minimizar a exposição à criação e à compra da conta robótica.
- Gerencie e acompanhe identidades usando serviços (como serviços de identidade digital).
- Avalie a força financeira do cliente por meio de sistemas de detecção de fraudes de cartão de crédito.
- Estabeleça uma política de coleções claras. Detalhe o processo de coleções e quando o acesso a assinaturas será afetado por não pagamento. (Você pode desabilitar o acesso ou [suspender as assinaturas de um cliente](suspend-a-subscription.md) para não pagamento.)

### <a name="managing-customer-accounts"></a>Gerenciar contas de clientes

As sugestões para gerenciar contas de clientes após a compra incluem:

- Implemente um processo para receber, revisar, agir e responder às notificações da Microsoft rapidamente.
- Trabalhe com os clientes para entender suas necessidades de negócios de uso de nuvem enquanto configurações limites de monitoramento apropriados. (Por exemplo, você pode [definir um orçamento mensal de gastos do Azure](set-an-azure-spending-budget-for-your-customers.md) no Partner Center. Essa compreensão permite que você monitore o uso do cliente durante o mês e seja notificado quando os clientes estiverem próximos do orçamento.)
- Monitore [os logs de atividade do cliente](activity-logs.md) regularmente para ajudar a detectar fraudes antecipadamente.
- Faça uma ação rápida quando atividades suspeitas forem detectadas.
- Evite dar aos clientes acesso administrativo total a assinaturas sem primeiro implementar os controles de mitigação de risco.

### <a name="managing-customer-billing"></a>Gerenciando cobrança de clientes

As sugestões para gerenciar a cobrança de cliente após a compra incluem:

- Solicite pagamentos antecipados antes das transações iniciais e da cobrança.
- Não aceite instrumentos de pagamento de alto risco (como cartões pré-pagos ou cartões de valores armazenados).
- Monitore pagamentos de clientes e contas a receber de vencimento. Impor agressivamente processos cobrança padronizados para pagamentos atrasados ou não de pagamento.

Para mais estratégias mais detalhadas de atenuação de risco online, consulte o [Guia de gerenciamento de risco de transação online.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4Bhtt)
