---
title: Solicitar um crédito de SLA da Microsoft
ms.topic: article
ms.date: 03/31/2021
description: Conheça os benefícios, as restrições e os procedimentos para solicitar um crédito de SLA (contrato de nível de serviço) da Microsoft se seus clientes sofrerem uma interrupção de serviço.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 3a0bb85143efe3d4135b56985b9a04e2dbe5e4cc
ms.sourcegitcommit: 57442bbbef15a70bd9a042642140cbf2c8608b09
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2021
ms.locfileid: "113519440"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a>Como e quando solicitar um crédito de SLA (contrato de nível de serviço) da Microsoft

**Funções apropriadas**: agente de administração | Administrador global

Você pode solicitar **créditos de SLA (contrato de nível de serviço)** da Microsoft se um serviço que você está fornecendo para seus clientes tiver uma interrupção.

## <a name="sla-credit-calculation"></a>Cálculo de crédito de SLA

Os créditos de SLA da Microsoft são determinados com base em quais serviços foram afetados. por exemplo, se o cliente tiver um conjunto de Office 365, mas tiver ocorrido apenas uma interrupção de SharePoint, o crédito de SLA será aprovado apenas para SharePoint e não para o plano inteiro do cliente.

*Os créditos são classificados pelo pro com base no serviço afetado e na duração da interrupção.* Para ver os tipos de cenários que se qualificam para créditos de SLA, consulte o [documento SLA consolidado de serviços online](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37). essas informações também se aplicam a serviços vendidos por meio do programa Provedor de Soluções na Nuvem (CSP).


## <a name="request-an-sla-credit"></a>Solicitar um crédito de SLA

*O parceiro CSP deve enviar a declaração e todas as informações necessárias ao final do mês civil após o mês em que o incidente ocorreu.* Por exemplo, se o incidente ocorreu em 15 de fevereiro, a Microsoft deve receber a declaração e todas as informações necessárias até 31 de março. Clientes finais e revendedores indiretos não podem enviar declarações de crédito de SLA; o provedor indireto ou o parceiro de cobrança direto deve enviar declarações em seu nome.

> [!NOTE]
> Incidentes de consultoria geralmente não são elegíveis para créditos de SLA. Um incidente Postado no painel de integridade do serviço indica que um locatário *pode* ser afetado e representa as melhores informações que a Microsoft tem no momento da publicação. Os dados da página de integridade representam a disponibilidade geral de um serviço. O impacto, a mitigação e a resolução do serviço individual podem variar. Você pode examinar a postagem do incidente final e postar a revisão do incidente para obter mais detalhes. consulte [como verificar a integridade do serviço Microsoft 365](/microsoft-365/enterprise/view-service-health#incidents-and-advisories) para obter mais informações.

### <a name="required-information"></a>Informações necessárias

O nome do cliente, o identificador do locatário, o n º do tíquete de parceiro e o carimbo de data/hora criado pelo tíquete não são suficientes para que uma declaração seja processada.

Antes de [Enviar uma solicitação de crédito de SLA](#submit-sla-credit-request) para a Microsoft, você deve reunir **todas** as seguintes informações para incluir em seu tíquete de suporte:

- O GUID do locatário do cliente
- O [identificador do incidente de interrupção](#outage-incident-identifier)?
- Evidências de que o cliente foi afetado pela interrupção e solicitou um crédito de SLA.
- As assinaturas afetadas foram adquiridas por meio do CSP? (*Sim* ou *não*)

#### <a name="evidence-that-proves-customer-impact"></a>Evidência que comprova o impacto sobre o cliente

- Informações sobre a hora e a duração do tempo de inatividade
- O número e o local (s) dos usuários afetados (se aplicável)
- Descrições de suas tentativas de resolver o incidente no momento da ocorrência
- Um email do cliente afetado solicitando suporte e, subsequentemente, crédito
- O número do tíquete de suporte e os detalhes do contato do cliente em relação à resolução do impacto do serviço


#### <a name="outage-incident-identifier"></a>Identificador de incidente de interrupção

você pode encontrar o identificador para o incidente de interrupção na página **integridade do serviço** na Centro de administração do Microsoft 365. a **ID do incidente de interrupção** é um número precedido por uma abreviação de duas letras que indica o serviço afetado (por exemplo, *EX25194* para uma interrupção de Exchange Online). A tabela a seguir descreve as abreviações de serviço comuns:

| Abreviação de duas letras | Serviço da Microsoft |
| ----------------------- | ----------------- |
| EX | Exchange Online |
| FO | Proteção do Exchange Online |
| SB | Skype for Business Online (anteriormente Lync Online) |
| Sistema operacional | Assinatura do Office |
| PB | Power BI para Office 365 |
| SP | SharePoint online |
| YA | Yammer Enterprise |
| MO | Erro do portal |

### <a name="submit-sla-credit-request"></a>Enviar solicitação de crédito de SLA

Para enviar sua solicitação de crédito de SLA para a Microsoft por meio do painel do Partner Center:

1. Entre no Painel do Partner Center.
2. No menu à esquerda, escolha solicitações de **serviço** e, em seguida, selecione **solicitações de suporte do parceiro**.
3. Na página **solicitação do parceiro** , escolha **nova solicitação**.
4. Na página **iniciar a solicitação** , localize a seção **CSP-Customers, Orders e subscriptions**. Nesta seção, escolha **selecionar um tipo de problema** e, em seguida, selecione solicitações de crédito de atendimento **ao cliente**.
5. Na página **soluções recomendadas** , em **você precisa de mais ajuda?**, escolha **Sim**.
6. Na página **detalhes** , preencha a seção **detalhes do problema** . Na caixa de texto **detalhes** , certifique-se de inserir as [informações necessárias](#required-information) que você coletou anteriormente.
7. Escolha **Enviar** para enviar em sua solicitação de crédito de SLA.

## <a name="next-steps"></a>Próximas etapas

- [Relatar problemas em nome do seu cliente](report-problems-on-behalf-of-a-customer.md)
