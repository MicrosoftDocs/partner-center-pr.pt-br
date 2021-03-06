---
title: Oferecer avaliações de produtos da Microsoft aos clientes
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Permitir que os clientes experimentem produtos de assinatura da Microsoft por 30 dias. Inscreva-se para essas avaliação gratuitas no catálogo, assim como muitas outras serviços online.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1d6fda82464b9abc30714798a2ee3999d8f93db5
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151127"
---
# <a name="give-customers-30-day-free-trials-of-microsoft-products"></a>Dar aos clientes 30 dias de avaliação gratuita de produtos da Microsoft

**Funções apropriadas:** administrador global | Administrador de gerenciamento de usuários | Agente de vendas

Uma boa maneira de apresentar os clientes a novos produtos da Microsoft é oferecendo avaliações gratuitas de 30 dias. Você pode se inscrever para as avaliações no catálogo da mesma forma que se inscreve em muitos outros serviços online. Todos os parceiros podem participar.

## <a name="available-trial-offers"></a>Ofertas de avaliação disponíveis

Você pode encontrar todas as suas ofertas de avaliação pendentes na **página** Cliente. Esta página lista todas as assinaturas, incluindo avaliação gratuita e assinaturas pagas. (Esse recurso não está disponível atualmente na China.)

Cada cliente tem direito a uma avaliação gratuita para cada oferta disponível. Por exemplo, eles podem obter uma avaliação gratuita para Microsoft 365 Business Standard e uma avaliação gratuita para o Office 365 E3. No entanto, se o cliente já tiver a oferta, ele não poderá usar uma avaliação gratuita para essa oferta.

### <a name="available-products"></a>Produtos disponíveis

As avaliação gratuitas estão disponíveis para as ofertas mais abrangentes e populares baseadas em licesen. Novas ofertas de avaliação podem ser introduzidas mensalmente.

Os parceiros podem encontrar avaliação na lista de preços mensal na página **de preços e ofertas** Partner Center. As ofertas de avaliação terão "TRIAL" listado na lista de preços **Tipo de Licença** Secundária coluna.

Atualmente, não há **nenhuma avaliação gratuita para ofertas** governamentais, ofertas de educação ou ofertas de complemento.

## <a name="licenses-for-free-trial-offers"></a>Licenças para ofertas de avaliação gratuita

Todas as avaliação gratuitas fornecem 25 licenças. Você não pode alterar esse número durante a avaliação. Você não pode adicionar ou remover licenças na avaliação gratuita. Depois que a avaliação for convertida em uma assinatura paga, você poderá adicionar mais licenças à assinatura.

As licenças de avaliação devem ser atribuídas aos usuários da mesma forma que a licença de serviços pagos são atribuídas.

## <a name="sign-customers-up-for-trials"></a>Conectar os clientes para avaliações

Obtenha uma avaliação para seu cliente no Partner Center:

1. Em **vender** no Partner Center, acesse **Catálogo**. 
2. No catálogo, da **frequência de cobrança**, selecione **oferta de avaliação**. Isso exibe apenas as avaliações gratuitas e oculta ofertas que não são gratuitas. Avaliações aparecem na guia **Avaliações** no catálogo.
3. Selecione a avaliação gratuita que você deseja oferecer e, em seguida, selecione **enviar**. Todas as avaliações são válidas por um período de 30 dias durante o qual você não será cobrado. Você também pode convertê-la para uma assinatura paga a qualquer momento durante a avaliação.

## <a name="converting-trials-to-paid-subscriptions"></a>Convertendo avaliações em assinaturas pagas

Uma avaliação gratuita não é convertida automaticamente em uma assinatura paga. Após 30 dias, uma avaliação gratuita deverá ser convertida em uma assinatura paga ou ela [expirará](#expiring-offers). As avaliações gratuitas não podem ser estendidas.

Você precisará converter a avaliação em uma assinatura paga por conta própria. Você pode fazer isso [usando o Partner Center](#convert-trials-using-partner-center) ou [por meio das APIs do Partner Center](#convert-trials-using-apis).

> [!NOTE]
> As avaliações gratuitas do cliente para o programa CSP (provedor de soluções na nuvem) não podem ser convertidas em outro locatário do programa (como EA, Open ou MOSP).

### <a name="convert-trials-using-partner-center"></a>Converter avaliações usando o Partner Center

Você pode converter Avaliações para assinaturas pagas usando o Partner Center:

1. Acesse a página de assinatura do cliente e selecione a avaliação gratuita.
2. Selecione **Converter uma assinatura de avaliação em paga**.
3. Insira a quantidade de licenças desejada e a frequência de cobrança e selecione **Aplicar**.
4. A cobrança da assinatura paga começa na data de conversão e a assinatura é renovada por 12 meses a partir da data de conversão. 

### <a name="convert-trials-using-apis"></a>Converter avaliações usando APIs

Talvez seja necessário alterar suas APIs para acomodar a conversão de uma avaliação gratuita em uma assinatura paga. Para obter mais informações, consulte a seguinte documentação do desenvolvedor:

- [Converter uma assinatura de avaliação em paga](/partner-center/develop/convert-a-trial-subscription-to-paid)
- [Obter uma lista de ofertas de conversão de avaliação](/partner-center/develop/get-a-list-of-trial-conversion-offers)

### <a name="trials-without-conversions"></a>Avaliações sem conversões

Nem todas as avaliações podem ser convertidas em assinaturas pagas. Os parceiros podem usar uma avaliação que não tem conversões até a data de validade. Os parceiros podem adquirir ofertas compatíveis que dão suporte aos mesmos serviços da oferta de avaliação.  Isso deve ser feito antes de a avaliação expirar para garantir que os serviços de ofertas recentemente adquiridos se alinhem aos serviços da avaliação. 

|**Avaliação**   |**Ofertas de pequenas empresas compatíveis**   |**Ofertas corporativas compatíveis**   |
|----------------------------|:---------------------------------|:------------------------------------------|
|Avaliação de nuvem comercial do Microsoft Teams (iniciada pelo usuário)   |Microsoft 365 Business Basic, Microsoft 365 Business Standard, Microsoft 365 Business Premium   | F3 (anteriormente F1), Office 365 para empresas (E1, E3 e E5), Microsoft 365 F1/F3, Microsoft 365 Enterprise (E3)   |

>[!NOTE]
>As ofertas acima têm planos de serviço semelhantes com funcionalidade semelhante, no entanto, pode haver algumas diferenças entre as ofertas.

### <a name="expiring-offers"></a>Ofertas expirando

Você não será notificado de ofertas expiradas. Você pode acompanhar datas de expiração futuras usando a exibição de cliente no Partner Center ou consultando a API. É recomendável monitorar essas datas com frequência para que você possa executar as ações de acompanhamento apropriadas quando os clientes tomarem uma decisão.

Após a expiração de uma avaliação, um cliente que tentar fazer logon nessa avaliação verá uma mensagem de expiração. No entanto, os dados são armazenados em linha com os padrões de retenção de dados. Depois de comprar uma nova assinatura com os mesmos planos de serviço, as informações do cliente poderão ser acessadas novamente da assinatura que acabou de ser ativada.

## <a name="billing"></a>Cobrança

A cobrança anual e as avaliações gratuitas são as mesmas em nuvens soberanass e na nuvem pública. A única diferença são os SKUs de avaliação disponíveis no momento do lançamento.

## <a name="billing-for-free-trials"></a>Cobrança de avaliações gratuitas

As avaliações gratuitas podem ser usadas para assinaturas mensais e anuais cobradas. Você pode selecionar a frequência de cobrança ao converter a avaliação em uma assinatura paga.

A data de início da assinatura é baseada na data de conversão. Se a avaliação gratuita for convertida em uma oferta paga com cobrança anual, a data de renovação da assinatura será de 12 meses a partir da data de conversão. Se a avaliação gratuita for convertida em uma oferta paga com cobrança mensal, a data de renovação da assinatura será 12 meses a partir da data de cobrança após a data de conversão.

### <a name="invoices"></a>Faturas

Você não verá avaliações gratuitas listadas em seu arquivo de reconciliação baseado em licença ou fatura. As avaliações gratuitas só serão exibidas em seu arquivo de reconciliação baseado em licença e fatura depois que você converter uma avaliação gratuita em uma assinatura paga. A assinatura convertida será exibida da mesma maneira que qualquer nova assinatura.

### <a name="incentives"></a>Incentivos

As avaliações gratuitas não têm impacto sobre os incentivos.

## <a name="support"></a>Suporte

Para obter suporte em avaliações gratuitas, envie uma solicitação de serviço por meio do Partner Center.