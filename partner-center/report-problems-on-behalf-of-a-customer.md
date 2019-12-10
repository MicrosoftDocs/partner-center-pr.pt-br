---
title: Relatar problemas em nome de um cliente | Partner Center
ms.topic: article
ms.date: 08/16/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Se o seu cliente estiver enfrentando um problema de serviço que você não pode resolver, e que atenda aos critérios descritos em escalar problemas para a Microsoft, forneça um tíquete de suporte para eles.
ms.assetid: 417E8EE3-EBD2-41DA-BF6E-DD935BE78EF5
author: MaggiePucciEvans
ms.author: evansma
Keywords: solicitação de serviço, tíquete de serviço, suporte, direito de suporte, Aobo, AOBO do Azure
ms.localizationpriority: medium
ms.openlocfilehash: 28f5be859d8c949eb0135f3096c320cc160b835a
ms.sourcegitcommit: 9a628b8fc73d4db995b7cb42faaf4d6c3b573e45
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2019
ms.locfileid: "74943209"
---
# <a name="report-problems-on-behalf-of-a-customer"></a>Relatar problemas em nome de um cliente

**Aplica-se a**

-  Partner Center
-  Partner Center do Microsoft Cloud for US Government


Se o cliente está tendo um problema de serviço que você não consegue resolver e que atende aos critérios descritos em [Encaminhar problemas para a Microsoft](escalate-problems-to-microsoft.md), abra um tíquete de suporte para ele. Esse processo também é útil para encaminhar problemas ou controvérsias relativos a cobrança e preocupações com fraude.

## <a name="submit-a-service-request-for-a-customer"></a>Envie uma solicitação de serviço por um cliente

1.  Do menu **Centro de Parceiros**, selecione **Solicitações de serviço** e então **Solicitação do cliente**. 

2.  Na página Solicitações do cliente, pesquise o cliente desejado.

3.  Do menu suspenso **Nova solicitação**, selecione **Azure** ou **Office 365, Dynamics 365, Enterprise Mobility Suite**. Você será redirecionado para o portal do Microsoft Azure ou o Centro de Administração do Office 365.

### <a name="microsoft-azure"></a>Microsoft Azure

> [!IMPORTANT]
> Quando você precisar criar uma solicitação de serviço para seu cliente no Azure, esteja ciente do seguinte:
>
>- Para criar solicitações de serviço para o cliente no Azure, seu provedor indireto deve conceder acesso à conta do Azure do cliente. Isso é diferente de administrar em nome dos clientes para o Office 365. 
>
>- Embora o administrador de assistência técnica no Partner Center não possa criar solicitações de serviço no portal de serviço do Azure, o que eles podem fazer é criar um grupo de suporte no portal de serviço do Azure e conceder a esse grupo permissões para registrar solicitações de suporte.

1. Selecione **Nova solicitação de suporte**.
2. Preencha a solicitação de suporte com as informações apropriadas e, em seguida, selecione **Criar**:
-   Na seção **Noções básicas** da solicitação de suporte, certifique-se de selecionar **Provedor de Soluções na Nuvem** no campo **Plano de suporte**.
-   Na seção de informações **Contato** da solicitação de suporte, insira suas informações, não as informações do cliente.

3. Mais tarde, revise as solicitações de serviço do cliente no portal do Microsoft Azure selecionando **Gerenciar solicitações de suporte**.

Talvez seja necessário criar uma solicitação de suporte para um cliente quando você não tiver permissões de administrador para esse cliente. Isso poderia ocorrer em um dos seguintes dois cenários: 
 
-   Você não solicitou privilégios de administrador quando estabeleceu pela primeira vez a relação.
-   Você gerencia as assinaturas do Azure de um cliente e não outras, o que não exige que você tenha permissões administrativas.
 
Em qualquer um desses casos, você pode usar o procedimento a seguir para criar uma solicitação de suporte. 

1. Copie o nome de domínio do cliente da página conta no centro de parceiros.

2. Vá para https://portal.azure.com/ [customerdomainname]. 

3. Selecione a assinatura do Azure que requer suporte.

4. Selecione **nova solicitação de suporte** e siga os prompts para criar a solicitação. 

 
### <a name="office-365-microsoft-dynamics-crm-online-enterprise-mobility-suite"></a>Office 365, Microsoft Dynamics CRM Online, Enterprise Mobility Suite

1. Na seção **Criar uma solicitação de serviço**, escolha a categoria de tópico de suporte apropriada. Talvez seja necessário selecionar **mais..** . para exibir tópicos adicionais.    
2. Preencha o formulário de solicitação de serviço e selecione **Enviar**.

   > [!TIP]
   > Certifique-se de incluir suas informações de contato, não as do cliente.

3. Mais tarde, examine as solicitações de serviço do cliente indo para o Centro de Administração do Office 365 e selecionando **Ver todos os tíquetes de suporte**.

### <a name="support-for-commercial-marketplace-products"></a>Suporte para produtos do Marketplace comercial

A Microsoft não oferece suporte ao produto para produtos do Marketplace comercial. Você precisará entrar em contato com o ISV (fornecedor independente de software) que publicou o produto para obter suporte.

Para localizar as informações de contato do ISV:

1.  Na página do **Marketplace**, selecione o produto com o qual você precisa de ajuda.
2.  Na página do produto, você encontrará informações de contato de suporte. Isso pode ser um ou mais dos seguintes:
    - Um link para um ponto de entrada de suporte no site do ISV
    - Um e-mail de suporte 
    - Um número de telefone de contato de suporte

## <a name="faq"></a>Perguntas frequentes

**O que é incluído como parte do direito a suporte?**

As solicitações de serviço devem ser feitas por meio do Partner Center e estão disponíveis para Azure, Microsoft Office 365, Microsoft Dynamics CRM Online e Enterprise Mobility Suite. Como um parceiro que participa do programa de provedor de soluções na nuvem, você pode esperar o tempo de resposta de prioridade para seus principais problemas.

O suporte para seu próprio locatário parceiro não está incluído como parte do benefício de suporte CSP. No entanto, o Office 365, o Microsoft Dynamics CRM Online e o Enterprise Mobility Suite não cobram uma taxa de assinatura de suporte separada para parceiros ou clientes. O Azure cobra uma taxa, mas caso tenha direito ao suporte à nuvem de assinatura ou outros benefícios de MPN (Rede de Parceiros Microsoft), você poderá usá-los para pagar essa taxa.

Esse benefício se aplica a todos os parceiros que participam do programa do provedor de soluções na nuvem, sejam pagos ou em um período de avaliação. O suporte ao gerenciamento de assinatura e cobrança também está incluído como um componente gratuito desse pacote.

**Com que rapidez obterei uma resposta inicial?**

Nossos tempos de resposta iniciais dependem da gravidade do incidente enviado. A gravidade do problema é determinada por sua indicação de impacto de negócios quando você envia uma solicitação de serviço.

Os tempos de resposta iniciais para **incidentes de suporte técnico** são:

-   Impacto crítico (gravidade A): 2 horas (perda significativa ou degradação de serviços. Serviços de produção inativos).
-   Impacto moderado (gravidade B): 4 horas (Perda moderada ou degradação de serviços. Serviços de produção parcialmente afetados.)
-   Impacto mínimo (gravidade C): 8 horas (Perda mínima ou degradação de serviços. Serviços ainda disponíveis ou nenhum serviço de produção afetado).

Os tempos de resposta iniciais são apenas para suporte em inglês. É fornecido suporte no idioma local durante o horário comercial.
Para incidentes que ficam dentro dos limites da qualificação de suporte, mas não são considerados incidentes de interrupção-correção, o tempo de resposta inicial pode ser até um dia útil.

**Posso enviar uma solicitação de serviço por telefone?**

Não, o suporte por telefone não é oferecido neste programa.

**O que acontece se eu fizer logon no portal do Azure e ignorar o Partner Center?**

Caso entre no portal do Microsoft Azure diretamente, você verá o centro em seu próprio contexto, não no contexto do cliente. Portanto, você só deve entrar diretamente no portal do Microsoft Azure quando estiver criando uma solicitação de serviço para suas próprias assinaturas.

O direito de suporte do programa CSP não fornece suporte em sua própria assinatura de parceiro. portanto, ao criar uma solicitação de serviço que se preocupa com sua própria assinatura de parceiro, você deve fornecer seu direito de plano de suporte válido. Exemplos incluem ID de contrato MPN, Premier ou um plano de suporte do Azure. Consulte as [Perguntas frequentes sobre o suporte do Azure](https://go.microsoft.com/fwlink/?LinkId=717532).

**O que acontece se eu entrar no portal do centro de administração do Office 365 e ignorar o Partner Center?**

Caso entre diretamente no Centro de Administração do Office 365, você verá o centro em seu próprio contexto, não no contexto do cliente. Portanto, você só deve entrar diretamente no Centro de Administração do Office 365 quando estiver criando uma solicitação de serviço para suas próprias assinaturas.

**Como obter suporte adicional ao Dynamics 365?**

Se você estiver tendo problemas relacionados a: assinaturas do plano do Dynamics 365, licenciamento, cobrança, Finanças & operações, licenças de produto do Dynamics 365 ou precisar de mais suporte técnico:
 
Contate o [Suporte do Dynamics](https://docs.microsoft.com/dynamics365/customer-engagement/admin/contact-technical-support)

Leia [Suporte do Microsoft Dynamics](https://support.microsoft.com/help/4052881/faq-microsoft-dynamics-365-for-unified-operations-iur)



