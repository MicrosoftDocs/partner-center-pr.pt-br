---
title: Solicitar um crédito de SLA da Microsoft
ms.topic: article
ms.date: 03/31/2021
description: Conheça os benefícios, restrições e procedimentos para solicitar um crédito SLA (contrato de nível de serviço) da Microsoft se seus clientes experimentarem uma paralisação de serviço.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: f521e55869d60987fb46cd5d570bf206939e0782
ms.sourcegitcommit: 8235c89e789cdb5115fc1c19151fa8e97c743fe5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "113080632"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a>Como e quando solicitar um crédito SLA (contrato de nível de serviço) da Microsoft

**Funções apropriadas:** agente administrador | Administrador global

Você pode solicitar **créditos SLA (Contrato** de Nível de Serviço) da Microsoft se um serviço que você está fornecendo para seus clientes tiver uma paralisação.

## <a name="sla-credit-calculation"></a>Cálculo de crédito SLA

Os créditos SLA da Microsoft são determinados com base em quais serviços foram afetados. Por exemplo, se o cliente tiver um pacote do Office 365, mas tiver apenas uma interrupção do SharePoint, o crédito SLA será aprovado somente para SharePoint e não para todo o plano do cliente.

*Os créditos são proporcionalmente com base no serviço afetado e na duração da paralisação.* Para ver os tipos de cenários qualificados para créditos SLA, consulte o documento [SLA](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37)Consolidado dos Serviços Online . Essas informações também se aplica aos serviços vendidos por meio do programa Provedor de Soluções na Nuvem (CSP).


## <a name="request-an-sla-credit"></a>Solicitar um crédito SLA

*O parceiro CSP deve enviar a declaração e todas as informações necessárias até o final do mês do calendário após o mês em que o incidente ocorreu.* Por exemplo, se o incidente ocorreu em 15 de fevereiro, a Microsoft deve receber a declaração e todas as informações necessárias até 31 de março. Os clientes finais e revendedores indiretos não podem enviar declarações de crédito SLA; O provedor indireto ou o parceiro de cobrança direta deve enviar declarações em seu nome.

> [!NOTE]
> Incidentes de consultoria não são qualificados para créditos SLA. Um incidente postado no Painel de Saúde  do Serviço indica que um locatário pode ser afetado e representa as melhores informações que a Microsoft tem no momento da publicação. Os dados da página de saúde representam a disponibilidade geral de um serviço. O impacto, a mitigação e a resolução de serviço individuais podem variar. Você pode revisar a Postagem de Incidentes final e a Revisão pós-incidente para obter mais detalhes. Confira [Como verificar a Microsoft 365 do serviço](/microsoft-365/enterprise/view-service-health#incidents-and-advisories) para obter mais informações.

### <a name="required-information"></a>Informações necessárias

O nome do cliente, o identificador de locatário, o tíquete do parceiro# e o carimbo de data/hora criados pelo tíquete não são suficientes para que uma declaração seja processada.

Antes de [enviar uma solicitação de crédito SLA](#submit-sla-credit-request) para a Microsoft, você deve reunir **todas** as seguintes informações para incluir no tíquete de suporte:

- GUID do locatário do cliente
- O [identificador de incidente de falha](#outage-incident-identifier)?
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
| SO | Assinatura do Office |
| PB | Power BI para Office 365 |
| SP | SharePoint online |
| Você | Yammer Enterprise |
| MO | Erro do portal |

### <a name="submit-sla-credit-request"></a>Enviar solicitação de crédito SLA

Para enviar sua solicitação de crédito SLA à Microsoft por meio do painel Partner Center:

1. Entre no Painel do Partner Center.
2. No menu à esquerda, escolha Solicitações **de serviço** e, em seguida, selecione **Solicitações de suporte do parceiro**.
3. Na página **Solicitação de** parceiro, escolha **Nova solicitação**.
4. Na página **Iniciar a solicitação,** encontre a seção **CSP – clientes, pedidos e assinaturas**. Nesta seção, escolha Selecionar **um tipo de problema** e, em seguida, selecione **Solicitações de crédito de serviços de clientes**.
5. Na página **Soluções recomendadas,** em **Você precisa de mais ajuda?**, escolha **Sim.**
6. Na página **Detalhes,** preencha a seção **Detalhes do** problema. Na caixa **de** texto Detalhes, insira as [informações](#required-information) necessárias coletadas anteriormente.
7. Escolha **Enviar** para enviar em sua solicitação de crédito SLA.

## <a name="next-steps"></a>Próximas etapas

- [Relatar problemas em nome do cliente](report-problems-on-behalf-of-a-customer.md)
