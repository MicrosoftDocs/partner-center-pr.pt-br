---
title: Relatar problemas em nome de um cliente
ms.topic: how-to
ms.date: 02/26/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba quando escalonar um problema de atendimento ao cliente para a Microsoft e como arquivar um tíquete de suporte para diferentes tipos de serviços da Microsoft.
author: Kim-Davis
ms.author: kimnich
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0cf8769bcf45ba90a714231a7c9db7660efce0b0
ms.sourcegitcommit: 700150044ea4f1a0b96cb4caeb97d7197da29ef6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "105549049"
---
# <a name="report-a-service-problem-on-behalf-of-a-customer---including-when-and-how-to-do-so"></a>Relatar um problema de serviço em nome de um cliente, incluindo quando e como fazer isso

**Aplica-se a**

- Partner Center para nuvem do Microsoft governamental

**Funções apropriadas**

- Provedor indireto

Se o seu cliente estiver enfrentando um problema de serviço que você não pode resolver e que atenda aos critérios descritos em [escalonar problemas para a Microsoft](escalate-problems-to-microsoft.md), seu provedor indireto poderá arquivar um tíquete de suporte para eles. Esse processo também é útil para encaminhar problemas ou controvérsias relativos a cobrança e preocupações com fraude.

## <a name="submit-a-service-request-for-a-customer"></a>Envie uma solicitação de serviço por um cliente

1. No menu do centro de parceiros, em CSP, selecione **clientes**

2. Na página clientes, selecione ou pesquise o cliente desejado
    
3. No menu cliente, selecione **solicitações de serviço**

4. Do menu suspenso **Nova solicitação**, selecione **Azure** ou **Office 365, Dynamics 365, Enterprise Mobility Suite**. Você será redirecionado para o portal do Microsoft Azure ou para o centro de administração do Office 365.

>[!NOTE]
>Os parceiros de operações de suporte que transportam o Dynamics 365 no CSP são necessários para manter um contrato de suporte de plano de suporte avançado para parceiro (ASfP) ou superior. Esse contrato de suporte é necessário para enviar incidentes do Dynamics 365 em nome de um cliente CSP. [Saiba mais](https://partner.microsoft.com/support/partnersupport) sobre as opções do contrato de suporte.

### <a name="microsoft-azure"></a>Microsoft Azure

> [!IMPORTANT]
> Quando você precisar criar uma solicitação de serviço para seu cliente no Azure, esteja ciente do seguinte:
>
>- Para você, como o revendedor indireto, para criar solicitações de serviço para seu cliente no Azure, seu provedor indireto deve conceder a você acesso à conta do Azure do cliente. Isso é diferente de administrar em nome dos clientes para o Office 365.
>
>- Embora o administrador de assistência técnica no Partner Center não possa criar solicitações de serviço no portal de serviço do Azure, o que eles podem fazer é criar um grupo de suporte no portal de serviço do Azure e conceder a esse grupo permissões para registrar solicitações de suporte.

1. Selecione **Nova solicitação de suporte**.

2. Preencha a solicitação de suporte com as informações apropriadas e, em seguida, selecione **Criar**:

   - Na seção **Noções básicas** da solicitação de suporte, certifique-se de selecionar **Provedor de Soluções na Nuvem** no campo **Plano de suporte**.

   - Na seção de informações **Contato** da solicitação de suporte, insira suas informações, não as informações do cliente.

3. Posteriormente, revise as solicitações de serviço do seu cliente no portal do Microsoft Azure selecionando **Gerenciar solicitações de suporte**.

Talvez seja necessário criar uma solicitação de suporte para um cliente quando você não tiver permissões de administrador para esse cliente. Isso poderia ocorrer em um dos seguintes dois cenários:

- Você não solicitou privilégios de administrador quando estabeleceu pela primeira vez a relação.
- Você só gerencia as assinaturas do Azure de um cliente, portanto, você não tem permissões administrativas.
 
Em qualquer um desses casos, você pode usar o procedimento a seguir para criar uma solicitação de suporte. 

1. Copie o nome de domínio do cliente da página conta no centro de parceiros.

2. Vá para https://portal.azure.com/[customerdomainname]. 

3. Selecione a assinatura do Azure que requer suporte.

4. Selecione **nova solicitação de suporte** e siga os prompts para criar a solicitação. 

 
### <a name="office-365-microsoft-dynamics-crm-online-enterprise-mobility-suite"></a>Office 365, Microsoft Dynamics CRM Online, Enterprise Mobility Suite

1. Na seção **criar uma solicitação de serviço** , escolha a categoria de suporte apropriada. Talvez seja necessário selecionar **mais..** . para exibir artigos adicionais.

2. Preencha o formulário de solicitação de serviço e selecione **Enviar**.

   > [!TIP]
   > Certifique-se de incluir suas informações de contato, não o seu cliente.

3. Posteriormente, examine as solicitações de serviço do seu cliente acessando o centro de administração do Office 365 e selecionando **Ver todos os tíquetes de suporte**.

### <a name="support-for-commercial-marketplace-products"></a>Suporte para produtos do Marketplace comercial

A Microsoft não oferece suporte ao produto para produtos do Marketplace comercial. Você precisará entrar em contato com o ISV (fornecedor independente de software) que publicou o produto para obter suporte.

Para localizar as informações de contato do ISV:

1.  Na página do **Marketplace**, selecione o produto com o qual você precisa de ajuda.

2.  Na página do produto, você encontrará informações de contato de suporte. Isso pode ser uma ou mais das seguintes opções:

    - Um link para um ponto de entrada de suporte no site do ISV
    - Um e-mail de suporte
    - Um número de telefone de contato de suporte

## <a name="faq"></a>Perguntas frequentes

Consulte as perguntas frequentes a seguir sobre as solicitações de serviço que você pode enviar em nome de um cliente. 

### <a name="what-is-included-as-part-of-the-support-entitlement"></a>O que é incluído como parte do direito a suporte?

As solicitações de serviço devem ser arquivadas por meio do Partner Center. Eles estão disponíveis para o Azure, Microsoft Office 365, Microsoft Dynamics CRM Online e Enterprise Mobility Suite. Como um parceiro que participa do programa de provedor de soluções na nuvem, você pode esperar o tempo de resposta de prioridade para seus principais problemas.

O suporte para seu próprio locatário de parceiro não está incluído como parte do benefício de suporte do CSP. No entanto, o Office 365, o Microsoft Dynamics CRM Online e o Enterprise Mobility Suite não cobram uma taxa de assinatura de suporte separada para parceiros ou clientes. O Azure cobra uma taxa, mas se você tiver direito à assinatura de suporte de nuvem ou a outros benefícios de Microsoft Partner Network (MPN), poderá usá-los para pagar essa taxa.

Esse benefício se aplica a todos os parceiros que participam do programa do provedor de soluções na nuvem, sejam pagos ou em um período de avaliação. O suporte ao gerenciamento de assinatura e cobrança também está incluído como um componente gratuito desse pacote.

### <a name="how-quickly-will-i-get-an-initial-response"></a>Com que rapidez obterei uma resposta inicial?

Nossos tempos de resposta iniciais dependem da gravidade do incidente enviado. A gravidade do problema é determinada por sua indicação de impacto de negócios quando você envia uma solicitação de serviço.

Tempos de resposta iniciais para **incidentes de consertos técnicos**:

- Impacto crítico (severidade A): duas horas (perda significativa ou degradação dos serviços. Serviços de produção inativos).
- Impacto moderado (severidade B): quatro horas (perda moderada ou degradação de serviços. Serviços de produção afetados parcialmente.)
- Impacto mínimo (severidade C): oito horas (perda mínima ou degradação dos serviços. Serviços ainda disponíveis ou serviços de não produção afetados.)

Os tempos de resposta iniciais são apenas para suporte em inglês. É fornecido suporte no idioma local durante o horário comercial.
Para incidentes que se enquadram nos limites do direito de suporte, mas não são considerados incidentes de conserto de conserto, o tempo de resposta inicial pode ser de até um dia útil.

### <a name="can-i-submit-a-service-request-by-phone"></a>Posso enviar uma solicitação de serviço por telefone?

Não, o suporte ao telefone não é oferecido para este programa.

### <a name="what-happens-if-i-sign-into-the-azure-portal-and-bypass-partner-center"></a>O que acontece se eu fizer logon no portal do Azure e ignorar o Partner Center?

Se você entrar no portal do Microsoft Azure diretamente, você está visualizando o centro em seu próprio contexto, não no contexto de um cliente. É por isso que você só deve entrar diretamente no portal do Microsoft Azure ao criar uma solicitação de serviço para suas próprias assinaturas.

O direito de suporte do programa CSP não fornece suporte para sua própria assinatura de parceiro. Por isso, você precisa fornecer seu direito de plano de suporte válido ao criar uma solicitação de serviço que se preocupa com sua própria assinatura de parceiro. Os exemplos incluem ID do contrato MPN, Premier ou um plano de suporte do Azure. Para obter mais informações, consulte as [perguntas frequentes sobre o suporte do Azure](https://go.microsoft.com/fwlink/?LinkId=717532).

### <a name="what-happens-if-i-sign-into-the-office-365-admin-center-portal-and-bypass-partner-center"></a>O que acontece se eu entrar no portal do centro de administração do Office 365 e ignorar o Partner Center?

Se você entrar no centro de administração do Office 365 diretamente, você está exibindo o centro em seu próprio contexto, não no contexto de um cliente. É por isso que você só deve assinar diretamente no centro de administração do Office 365 ao criar uma solicitação de serviço para suas próprias assinaturas.

### <a name="how-do-i-get-additional-dynamics-365-support"></a>Como obter suporte adicional ao Dynamics 365?

Se você estiver enfrentando problemas relacionados a: assinaturas do plano do Dynamics 365, licenciamento, cobrança, finanças & operações, licenças de produto do Dynamics 365 ou precisar de mais suporte técnico:
 
Contate o [Suporte do Dynamics](/dynamics365/customer-engagement/admin/contact-technical-support)

## <a name="next-steps"></a>Próximas etapas

- [Fornecer suporte aos seus clientes](customer-support.md)
- [Verificar a integridade do serviço](check-service-health.md)
