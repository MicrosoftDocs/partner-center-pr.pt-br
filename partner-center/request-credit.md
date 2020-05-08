---
title: Solicitar um crédito de SLA da Microsoft
ms.topic: article
ms.date: 04/28/2020
description: Conheça os benefícios, as restrições e os procedimentos para solicitar um crédito de SLA (contrato de nível de serviço) da Microsoft se seus clientes sofrerem uma interrupção de serviço.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.assetid: E7F1F68D-25E5-46C5-9C98-1D0A9FAB7993
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 328051d69f2dfd869cca8c80de595b2e27c9a1af
ms.sourcegitcommit: e9b627159745bcce53a8c2b1676f63f5249bba76
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "82907874"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a>Como e quando solicitar um crédito de SLA (contrato de nível de serviço) da Microsoft

Você poderá solicitar créditos de **SLA (contrato de nível de serviço)** da Microsoft se um serviço que você está fornecendo para seus clientes tiver uma interrupção.

## <a name="sla-credit-calculation"></a>Cálculo de crédito de SLA

Os créditos de SLA da Microsoft são determinados com base em quais serviços foram afetados. Por exemplo, se o cliente tiver um pacote do Office 365, mas tiver apenas uma interrupção do SharePoint, o crédito de SLA será aprovado apenas para o SharePoint e não para o plano inteiro do cliente.

*Os créditos são classificados pelo pro com base no serviço afetado e na duração da interrupção.* Para ver os tipos de cenários que se qualificam para créditos de SLA, consulte o [documento SLA consolidado de serviços online](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37). Essas informações também se aplicam a serviços vendidos por meio do programa provedor de soluções na nuvem.

## <a name="request-an-sla-credit"></a>Solicitar um crédito de SLA

*O parceiro CSP (provedor de soluções na nuvem) deve enviar a declaração e todas as informações necessárias ao final do mês do calendário após o mês em que o incidente ocorreu.* Por exemplo, se o incidente ocorreu em 15 de fevereiro, a Microsoft deve receber a declaração e todas as informações necessárias até 31 de março. Clientes finais e revendedores indiretos não podem enviar declarações de crédito de SLA; o provedor indireto ou o parceiro de cobrança direto deve enviar declarações em seu nome.

### <a name="required-information"></a>Informações necessárias

Antes de [Enviar uma solicitação de crédito de SLA](#submit-sla-credit-request) para a Microsoft, você deve coletar as seguintes informações para incluir em seu tíquete de suporte:

- O GUID do locatário do cliente
- O [identificador do incidente de interrupção](#outage-incident-identifier)?
- As assinaturas afetadas foram adquiridas por meio do CSP? (*Sim* ou *não*)

#### <a name="outage-incident-identifier"></a>Identificador de incidente de interrupção

Você pode encontrar o identificador para o incidente de interrupção na página **integridade do serviço** no centro de administração do Microsoft 365. A **ID do incidente de interrupção** é um número precedido por uma abreviação de duas letras que indica o serviço afetado (por exemplo, *EX25194* para uma interrupção do Exchange Online). A tabela a seguir descreve as abreviações de serviço comuns:

| Abreviação de duas letras | Serviço da Microsoft |
| ----------------------- | ----------------- |
| EX | Exchange Online |
| FO | Proteção do Exchange Online |
| SB | Skype for Business online (anteriormente Lync Online) |
| Sistema operacional | Assinatura do Office |
| PB | Power BI para Office 365 |
| SP | SharePoint online |
| YA | Yammer Enterprise |
| MO | Erro do portal |

### <a name="submit-sla-credit-request"></a>Enviar solicitação de crédito de SLA

Para enviar sua solicitação de crédito de SLA para a Microsoft por meio do painel do Partner Center:

1. Entre no Painel do Partner Center.
2. No menu à esquerda, escolha solicitações de **serviço**e, em seguida, selecione **solicitações de suporte do parceiro**.
3. Na página **solicitação do parceiro** , escolha **nova solicitação**.
4. Na página **iniciar a solicitação** , localize a seção **CSP-Customers, Orders e subscriptions**. Nesta seção, escolha **selecionar um tipo de problema**e, em seguida, selecione solicitações de crédito de atendimento **ao cliente**.
5. Na página **soluções recomendadas** , em **você precisa de mais ajuda?**, escolha **Sim**.
6. Na página **detalhes** , preencha a seção **detalhes do problema** . Na caixa de texto **detalhes** , certifique-se de inserir as [informações necessárias](#required-information) que você coletou anteriormente.
7. Escolha **Enviar** para enviar em sua solicitação de crédito de SLA.
