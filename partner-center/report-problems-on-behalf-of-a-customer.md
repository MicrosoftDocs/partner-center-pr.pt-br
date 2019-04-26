---
title: Relatar problemas em nome de um cliente | Partner Center
ms.topic: article
ms.date: 03/01/2019
Description: Se o cliente está tendo um problema de serviço que você não consegue resolver e que atende aos critérios descritos em Encaminhar problemas para a Microsoft, abra um tíquete de suporte para ele.
ms.assetid: 417E8EE3-EBD2-41DA-BF6E-DD935BE78EF5
author: MaggiePucciEvans
ms.author: evansma
Keywords: solicitação de serviço, o tíquete de serviço, suporte, suporte de qualificação, administrar em nome, administrar em nome do Azure
ms.localizationpriority: medium
ms.openlocfilehash: af024782202bc2127b76277b29049e3d34f17215
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2019
ms.locfileid: "62134056"
---
# <a name="report-problems-on-behalf-of-a-customer"></a>Relatar problemas em nome de um cliente

**Aplica-se a**

-  Partner Center
-  Partner Center para Microsoft Cloud for US Government


Se o cliente está tendo um problema de serviço que você não consegue resolver e que atende aos critérios descritos em [Encaminhar problemas para a Microsoft](escalate-problems-to-microsoft.md), abra um tíquete de suporte para ele. Esse processo também é útil para encaminhar problemas ou controvérsias relativos a cobrança e preocupações com fraude.

## <a name="submit-a-service-request-for-a-customer"></a>Envie uma solicitação de serviço por um cliente

1.  Dos **Partner Center** menu, selecione **solicitações de serviço** e, em seguida, **solicitação de cliente**. 

2.  Na página Solicitações do cliente, pesquise o cliente desejado.

3.  Do menu suspenso **Nova solicitação**, selecione **Azure** ou **Office 365, Dynamics 365, Enterprise Mobility Suite**. Você será redirecionado para o portal do Microsoft Azure ou o Centro de Administração do Office 365.

### <a name="microsoft-azure"></a>Microsoft Azure

> [!IMPORTANT]
> Quando você precisa criar uma solicitação de serviço para o cliente no Azure, esteja ciente das seguintes opções:
>
>- Em ordem para que você possa criar solicitações de serviço para o cliente no Azure, seu provedor indireto deve conceder que acesso à conta do Azure do cliente. Isso é diferente de administrar em nome dos clientes para o Office 365. 
>
>- Embora o administrador de assistência técnica no Partner Center não é possível criar solicitações de serviço no portal de serviços do Azure, o que pode fazer é criar um grupo de suporte no portal de serviços do Azure e conceder permissões desse grupo para registrar solicitações de suporte.

1. Selecione **Nova solicitação de suporte**.
2. Preencha a solicitação de suporte com as informações apropriadas e, em seguida, selecione **Criar**:
-   Na seção **Noções básicas** da solicitação de suporte, certifique-se de selecionar **Provedor de Soluções na Nuvem** no campo **Plano de suporte**.
-   Na seção de informações **Contato** da solicitação de suporte, insira suas informações, não as informações do cliente.

3. Mais tarde, revise as solicitações de serviço do cliente no portal do Microsoft Azure selecionando **Gerenciar solicitações de suporte**.

Talvez você precise criar uma solicitação de suporte para um cliente quando você não tem permissões de administrador para esse cliente. Isso pode acontecer em dois cenários: 
 
-   Você não solicitou privilégios de administrador ao primeiro estabelecer a relação.
-   Gerenciar assinaturas do Azure de um cliente e não outros, que não exige que você tenha permissões administrativas.
 
Em ambos os casos, você pode usar o procedimento a seguir para criar uma solicitação de suporte. 

1. Copie o nome de domínio do cliente na sua página conta no Partner Center.

2. Vá para https://portal.azure.com/[customerdomainname]. 

3. Selecione a assinatura do Azure que exija suporte.

4. Selecione **nova solicitação de suporte**e, em seguida, siga os prompts para criar a solicitação. 

 
### <a name="office-365-microsoft-dynamics-crm-online-enterprise-mobility-suite"></a>Office 365, Microsoft Dynamics CRM Online, Enterprise Mobility Suite

1. Na seção **Criar uma solicitação de serviço**, escolha a categoria de tópico de suporte apropriada. Talvez seja necessário selecionar **Mais...** para exibir tópicos adicionais.    
2. Preencha o formulário de solicitação de serviço e selecione **Enviar**.

   > [!TIP]
   > Certifique-se de incluir suas informações de contato, não as do cliente.

3. Mais tarde, examine as solicitações de serviço do cliente indo para o Centro de Administração do Office 365 e selecionando **Ver todos os tíquetes de suporte**.

### <a name="support-for-azure-marketplace-products"></a>Suporte para produtos do Azure Marketplace

Microsoft não oferece suporte ao produto para produtos do Azure Marketplace. Você precisará entrar em contato com o Software ISV (fornecedor independente) que publicou o produto para obter suporte.

Para localizar informações de contato do ISV:

1.  Na página do Marketplace, selecione o produto que você precisa de Ajuda.
2.  Na página do produto, você encontrará informações de contato de suporte. Isso pode ser um ou mais das seguintes opções:
    - Um link para um ponto de entrada de suporte no site do ISV
    - Um email de suporte 
    - Um número de telefone de contato de suporte

## <a name="faq"></a>Perguntas frequentes

**O que é incluído como parte do direito de suporte?**

As solicitações de serviço devem ser feitas por meio do Partner Center e estão disponíveis para Azure, Microsoft Office 365, Microsoft Dynamics CRM Online e Enterprise Mobility Suite. Como um parceiro CSP, você pode esperar o tempo de resposta prioritário para os seus principais problemas.

O suporte para seu próprio locatário parceiro não está incluído como parte do benefício de suporte CSP. No entanto, o Office 365, o Microsoft Dynamics CRM Online e o Enterprise Mobility Suite não cobram uma taxa de assinatura de suporte separada para parceiros ou clientes. O Azure cobra uma taxa, mas caso tenha direito ao suporte à nuvem de assinatura ou outros benefícios de MPN (Rede de Parceiros Microsoft), você poderá usá-los para pagar essa taxa.

Esse benefício se aplica a todos os parceiros CSP, sejam pagos ou em um período de avaliação. O suporte ao gerenciamento de assinatura e cobrança também está incluído como um componente gratuito desse pacote.

**Quão rapidamente receberão uma resposta inicial?**

Nossos tempos de resposta iniciais dependem da gravidade do incidente enviado. A gravidade do problema é determinada por sua indicação de impacto de negócios quando você envia uma solicitação de serviço.

Os tempos de resposta iniciais para **incidentes de suporte técnico** são:

-   Impacto crítico (severidade A): 2 horas (uma perda significativa ou degradação de serviços. Serviços de produção inativos).
-   Impacto moderado (gravidade B): 4 horas (perda moderada ou degradação de serviços. Serviços de produção parcialmente afetados.)
-   Impacto mínimo (gravidade C): 8 horas (mínimo de perda ou degradação de serviços. Serviços ainda disponíveis ou nenhum serviço de produção afetado).

Os tempos de resposta iniciais são apenas para suporte em inglês. É fornecido suporte no idioma local durante o horário comercial.
Para incidentes que ficam dentro dos limites da qualificação de suporte, mas não são considerados incidentes de interrupção-correção, o tempo de resposta inicial pode ser até um dia útil.

**Pode enviar uma solicitação de serviço por telefone?**

Não, o suporte por telefone não é oferecido neste programa.

**O que acontece se eu entrar no portal do Azure e ignorar o Partner Center?**

Caso entre no portal do Microsoft Azure diretamente, você verá o centro em seu próprio contexto, não no contexto do cliente. Portanto, você só deve entrar diretamente no portal do Microsoft Azure quando estiver criando uma solicitação de serviço para suas próprias assinaturas.

Seu direito de suporte CSP não abrange sua própria assinatura de parceiro, portanto, ao criar uma solicitação de serviço que diga respeito à sua própria assinatura de parceiro, você deverá informar sua qualificação válida ao plano de suporte. Exemplos incluem ID de contrato MPN, Premier ou um plano de suporte do Azure. Consulte as [Perguntas frequentes sobre o suporte do Azure](https://go.microsoft.com/fwlink/?LinkId=717532).

**O que acontece se eu entrar no portal do Centro de administração do Office 365 e ignorar o Partner Center?**

Caso entre diretamente no Centro de Administração do Office 365, você verá o centro em seu próprio contexto, não no contexto do cliente. Portanto, você só deve entrar diretamente no Centro de Administração do Office 365 quando estiver criando uma solicitação de serviço para suas próprias assinaturas.

**Como posso obter suporte adicional do Dynamics 365?**

Se você estiver tendo problemas relacionados a: Dynamics 365 planejar assinaturas, licenciamento, cobrança, finanças e operações, IURs ou você exige ainda mais o suporte técnico:
 
Contate o [Suporte do Dynamics](https://docs.microsoft.com/dynamics365/customer-engagement/admin/contact-technical-support)

Leia [Suporte do Microsoft Dynamics](https://support.microsoft.com/help/4052881/faq-microsoft-dynamics-365-for-unified-operations-iur)



