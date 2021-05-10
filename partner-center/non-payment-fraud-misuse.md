---
title: Gerenciamento de não pagamento, fraude ou uso indevido
description: Saiba mais sobre os diversos riscos envolvidos em transações online e as práticas recomendadas para gerenciar e atenuar esses riscos no Partner Center.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 07/14/2020
ms.openlocfilehash: c3b7db95bbbd039f8328ddd2785579bb533197cc
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686289"
---
# <a name="managing-non-payment-fraud-or-misuse-in-partner-center"></a>Gerenciamento de não pagamento, fraude ou uso indevido no Partner Center

**Aplica-se a**

- Partner Center do Microsoft Cloud for US Government

**Funções apropriadas**

- Administrador global
- Administrador de gerenciamento de usuário
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

Você pode usar as recomendações a seguir para ajudá-lo a desenvolver políticas e práticas para reduzir sua exposição a riscos de transação online no ciclo de vida de suas relações com o cliente.

### <a name="onboarding-new-customers"></a>Integração de novos clientes

As sugestões para reduzir os riscos online durante a integração de novos clientes incluem:

- Estabelecer relações pessoais com os clientes quando possível (por exemplo, entrar em contato com os clientes por telefone).
- Verifique as credenciais e a experiência dos clientes por meio de métodos melhores (como usar agências de crédito ou agências de relatório comerciais).
- Use a autenticação multifa factor (como verificação por SMS) durante a assinatura para minimizar a exposição à criação e à compra de contas robóticas.
- Gerenciar e rastrear identidades usando serviços (como serviços de identidade digital).
- Avaliar a força financeira do cliente por meio de rigorosos sistemas de detecção de fraudes de cartão de crédito.
- Estabeleça uma política clara de coleções. Detalhar o processo de suas coleções e quando o acesso às assinaturas será afetado por não pagamento. (Você pode desabilitar o acesso [ou suspender as assinaturas de](create-a-new-subscription.md#suspend-a-subscription) um cliente por não pagamento.)

### <a name="managing-customer-accounts"></a>Gerenciar contas de clientes

As sugestões para gerenciar contas de clientes após a compra incluem:

- Implemente um processo para receber, revisar, agir e responder rapidamente às notificações da Microsoft.
- Trabalhe com os clientes para entender suas necessidades de negócios de uso de nuvem enquanto configura os limites de monitoramento apropriados. (Por exemplo, você pode definir um orçamento mensal de gastos do [Azure](set-an-azure-spending-budget-for-your-customers.md) em Partner Center. Essa compreensão permite que você monitore o uso do cliente durante o mês e seja notificado quando os clientes estão próximos do orçamento.)
- Monitore [os logs de atividades do](activity-logs.md) cliente regularmente para ajudar a detectar fraudes no início.
- Tome uma ação rápida quando atividades suspeitas são detectadas.
- Evite dar aos clientes acesso administrativo completo às assinaturas sem primeiro implementar controles de mitigação de risco.

### <a name="managing-customer-billing"></a>Gerenciando cobrança de clientes

As sugestões para gerenciar a cobrança de cliente após a compra incluem:

- Solicite pagamentos antecipados antes das transações iniciais e da cobrança.
- Não aceite instrumentos de pagamento de alto risco (como cartões pré-pagos ou cartões de valores armazenados).
- Monitore pagamentos de clientes e contas a receber de vencimento. Impor agressivamente processos cobrança padronizados para pagamentos atrasados ou não de pagamento.

Para mais estratégias mais detalhadas de atenuação de risco online, consulte o [Guia de gerenciamento de risco de transação online.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4Bhtt)
