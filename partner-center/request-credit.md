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
ms.openlocfilehash: 74dd5c2c9457961f07dd0dd8d5a6ead9047c5579
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855549"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a>Como e quando solicitar um crédito de SLA (contrato de nível de serviço) da Microsoft

**Funções apropriadas**: agente de administração | Administrador global

Você pode solicitar **créditos de SLA (contrato de nível de serviço)** da Microsoft se um serviço que você está fornecendo para seus clientes tiver uma interrupção.

## <a name="sla-credit-calculation"></a>Cálculo de crédito de SLA

Os créditos de SLA da Microsoft são determinados com base em quais serviços foram afetados. Por exemplo, se o cliente tiver um pacote do Office 365, mas tiver apenas uma interrupção do SharePoint, o crédito de SLA será aprovado apenas para o SharePoint e não para o plano inteiro do cliente.

*Os créditos são classificados pelo pro com base no serviço afetado e na duração da interrupção.* Para ver os tipos de cenários que se qualificam para créditos de SLA, consulte o [documento SLA consolidado de serviços online](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37). Essas informações também se aplicam a serviços vendidos por meio do programa provedor de soluções na nuvem.


## <a name="request-an-sla-credit"></a>Solicitar um crédito de SLA

*O parceiro CSP (provedor de soluções na nuvem) deve enviar a declaração e todas as informações necessárias ao final do mês do calendário após o mês em que o incidente ocorreu.* Por exemplo, se o incidente ocorreu em 15 de fevereiro, a Microsoft deve receber a declaração e todas as informações necessárias até 31 de março. Clientes finais e revendedores indiretos não podem enviar declarações de crédito de SLA; o provedor indireto ou o parceiro de cobrança direto deve enviar declarações em seu nome.

>[!NOTE]
>Os incidentes de consultoria ([como verificar Microsoft 365 integridade do serviço](https://docs.microsoft.com/microsoft-365/enterprise/view-service-health?&preserve-view=trueo365-worldwide#incidents-and-advisories)) não são elegíveis para créditos de SLA.

### <a name="required-information"></a>Informações necessárias

O nome do cliente, o identificador do locatário, o n º do tíquete de parceiro e o carimbo de data/hora criado pelo tíquete não são suficientes para que uma declaração seja processada.

Antes de [Enviar uma solicitação de crédito de SLA](#submit-sla-credit-request) para a Microsoft, você deve reunir **todas** as seguintes informações para incluir em seu tíquete de suporte:

- O GUID do locatário do cliente
- O [identificador do incidente de interrupção](#outage-incident-identifier)?
- Evidência de que o cliente foi afetado pela paralisação e solicitou um crédito SLA.
- As assinaturas impactadas foram adquiridas por meio do CSP? (*sim* ou *não*)

#### <a name="evidence-that-proves-customer-impact"></a>Evidência que prova o impacto do cliente

- Informações sobre o tempo e a duração do tempo de inatividade
- O número e os locais dos usuários afetados (se aplicável)
- Descrições de suas tentativas de resolver o incidente no momento da ocorrência
- Um email do cliente afetado solicitando suporte e, posteriormente, crédito
- O número do tíquete de suporte e os detalhes do contato do cliente em relação à resolução do impacto no serviço


#### <a name="outage-incident-identifier"></a>Identificador de incidente de falha

Você pode encontrar o identificador do incidente de falha na página **De Saúde** do Serviço no centro Microsoft 365 administrador. A **ID do Incidente** de Paralisação é um número precedido por uma abreviação de duas letras que indica o serviço afetado (por exemplo, *EX25194* para uma paralisação do Exchange Online). A tabela a seguir descreve as abreviações de serviço comuns:

| Abreviação de duas letras | Serviço Microsoft |
| ----------------------- | ----------------- |
| EX | Exchange Online |
| FO | Proteção do Exchange Online |
| SB | Skype for Business Online (anteriormente Lync Online) |
| Sistema operacional | Assinatura do Office |
| PB | Power BI para Office 365 |
| SP | SharePoint online |
| Você | Yammer Enterprise |
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
