---
title: Oferecer avaliações de produtos da Microsoft aos clientes | Partner Center
ms.topic: article
ms.date: 11/21/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Seus clientes podem testar produtos de assinatura da Microsoft durante 30 dias. Você pode se inscrever para essas avaliações no catálogo, assim como muitos outros serviços online.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: ca774233fa6d5314e57f1ab2eb2a73b6037223e5
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/22/2019
ms.locfileid: "74384837"
---
# <a name="offer-your-customers-trials-of-microsoft-products"></a>Oferecer aos clientes avaliações de produtos da Microsoft

Aplica-se a:

- Partner Center

Uma boa maneira de apresentar novos produtos da Microsoft aos clientes é oferecendo avaliações gratuitas de 30 dias. Você pode se inscrever para as avaliações no catálogo da mesma forma que se inscreve em muitos outros serviços online. Todos os parceiros podem participar.

## <a name="available-trial-offers"></a>Ofertas de avaliação disponíveis

Você pode encontrar todas as suas ofertas de avaliação pendentes na página do **cliente** . Esta página lista todas as assinaturas, incluindo avaliações gratuitas e assinaturas pagas. (Esse recurso não está disponível atualmente na China.)

Cada cliente tem direito a uma avaliação gratuita para cada oferta disponível. Por exemplo, eles podem obter uma avaliação gratuita do Office 365 Business Premium e uma avaliação gratuita do Office 365 E3. No entanto, se o cliente já possuir a oferta, ele não poderá usar uma avaliação gratuita para essa oferta.

### <a name="available-products"></a>Produtos disponíveis

As avaliações gratuitas estão disponíveis para os seguintes produtos:

- Office 365 Business Premium
- Office 365 E3
- Office 365 E5 com PSTN
- Office 365 E5 sem PSTN
- Enterprise Mobility & Security E5
- Dynamics 365 Customer Engagement Plan 1
- Dynamics 365 for Financials
- Microsoft 365 Business

Nós fornecemos avaliações gratuitas para esses produtos porque eles são as ofertas de negócios mais abrangentes e populares. É possível que adicionemos outras ofertas de avaliação gratuita no futuro.

Atualmente, não existem **avaliações gratuitas** para ofertas governamentais, ofertas de treinamento ou ofertas complementares.

## <a name="licenses-for-free-trial-offers"></a>Licenças para ofertas de avaliação gratuita

Todas as avaliações gratuitas fornecem 25 licenças. Não é possível alterar esse número durante a avaliação. Você não pode adicionar ou remover estações na avaliação gratuita. Depois que a avaliação for convertida em uma assinatura paga, você poderá adicionar licenças adicionais à assinatura.

Você deve atribuir licenças de avaliação e estações da mesma forma como faria com um serviço pago no Partner Center.

## <a name="sign-customers-up-for-trials"></a>Conectar os clientes para avaliações

Para conectar seu cliente para uma avaliação por meio do Partner Center:

1. Em **vender** no Partner Center, acesse **Catálogo**. 
2. No catálogo, em **Frequência da cobrança**, clique em **Trial offer**. Isso exibe apenas as avaliações gratuitas e oculta ofertas que não são gratuitas. Avaliações aparecem na guia **Avaliações** no catálogo.
3. Selecione a avaliação gratuita que você deseja oferecer e, em seguida, selecione **enviar**. Todas as avaliações são válidas por um período de 30 dias durante o qual você não será cobrado. Você também pode convertê-la para uma assinatura paga a qualquer momento durante a avaliação.

## <a name="converting-trials-to-paid-subscriptions"></a>Convertendo avaliações em assinaturas pagas

Uma avaliação gratuita não é convertida automaticamente em uma assinatura paga. Após trinta dias, uma avaliação gratuita deverá ser convertida em uma assinatura paga ou ela [expirará](#expiring-offers). As avaliações gratuitas não podem ser estendidas.

Você precisará converter a avaliação em uma assinatura paga por conta própria. Você pode fazer isso [usando o Partner Center](#convert-trials-using-partner-center) ou [por meio das APIs do Partner Center](#convert-trials-using-apis).

> [!NOTE]
> As avaliações gratuitas do cliente para o programa CSP (provedor de soluções na nuvem) não podem ser convertidas em outro locatário do programa (como EA, Open ou MOSP).

### <a name="convert-trials-using-partner-center"></a>Converter avaliações usando o Partner Center

Você pode converter avaliações em assinaturas pagas usando o painel do Partner Center da seguinte maneira:

1. Acesse a página de assinatura do cliente e selecione a avaliação gratuita.
2. Selecione **Converter uma assinatura de avaliação em paga**.
3. Insira a quantidade de licenças desejada e a frequência de cobrança e selecione **Aplicar**.
4. A cobrança para a assinatura paga começa na data de conversão, e a inscrição será renovada automaticamente 12 meses a partir da data de conversão. 

### <a name="convert-trials-using-apis"></a>Converter avaliações usando APIs

Talvez seja necessário alterar suas APIs para acomodar a conversão de uma avaliação gratuita em uma assinatura paga. Para obter mais informações, consulte a seguinte documentação do desenvolvedor:

- [Converter uma assinatura de avaliação em paga](https://docs.microsoft.com/partner-center/develop/convert-a-trial-subscription-to-paid)
- [Obter uma lista de ofertas de conversão de avaliação](https://docs.microsoft.com/partner-center/develop/get-a-list-of-trial-conversion-offers)

### <a name="expiring-offers"></a>Ofertas expirando

Você não será notificado de ofertas expiradas. Você pode acompanhar datas de expiração futuras usando a exibição de cliente no Partner Center ou consultando a API. É recomendável monitorar essas datas com frequência para que você possa executar as ações de acompanhamento apropriadas quando os clientes tomarem uma decisão.

Após a expiração de uma avaliação, um cliente que tentar fazer logon nessa avaliação verá uma mensagem de expiração. No entanto, os dados são armazenados em linha com os padrões de retenção de dados. Depois de comprar uma nova assinatura com os mesmos planos de serviço, as informações do cliente poderão ser acessadas novamente da assinatura que acabou de ser ativada.

## <a name="billing"></a>Cobrança

A cobrança anual e as avaliações gratuitas são as mesmas em nuvens soberanass e na nuvem pública. A única diferença são os SKUs de avaliação disponíveis no momento do lançamento.

## <a name="billing-for-free-trials"></a>Cobrança de avaliações gratuitas

As avaliações gratuitas podem ser usadas para assinaturas mensais e anuais cobradas. Você pode selecionar a frequência de cobrança ao converter a avaliação em uma assinatura paga.

A data de início da assinatura é baseada na data de conversão. Se a avaliação gratuita for convertida em uma oferta paga com cobrança anual, a data de renovação da assinatura será de doze meses a partir da data de conversão. Se a avaliação gratuita for convertida em uma oferta paga com cobrança mensal, a data de renovação da assinatura será 12 meses a partir da data de cobrança após a data de conversão.

### <a name="invoices"></a>Faturas

Você não verá avaliações gratuitas listadas em seu arquivo de reconciliação baseado em licença ou fatura. As avaliações gratuitas só serão exibidas em seu arquivo de reconciliação baseado em licença e fatura depois que você converter uma avaliação gratuita em uma assinatura paga. A assinatura convertida será exibida da mesma maneira que qualquer nova assinatura.

### <a name="incentives"></a>Incentivos

As avaliações gratuitas não têm impacto sobre os incentivos.

## <a name="support"></a>Suporte

Para obter suporte em avaliações gratuitas, envie uma solicitação de serviço por meio do Partner Center.
