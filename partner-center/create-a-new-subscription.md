---
title: Criar, suspender ou cancelar assinaturas de clientes
ms.topic: article
ms.date: 11/27/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como vender as assinaturas do cliente para os produtos no catálogo depois de ter criado um registro de cliente no Partner Center.
ms.assetid: E95F1538-60E1-464C-B72B-52764BF3A820
author: LauraBrenner
ms.author: labrenne
Keywords: assinatura, criar novo, adicionar assinatura, suspender, cancelar, suspensão, suspender, SaaS, licença, ISV, terceiros
ms.localizationpriority: medium
ms.openlocfilehash: 75cfa546834e0e95dd716492ff822c0d1aa940b7
ms.sourcegitcommit: 3849d49261f4f652bd7c0537ebe31558af427c5c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "83362354"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a>Criar, suspender ou cancelar assinaturas de clientes

**Aplica-se a**

- Partner Center
- Partner Center do Microsoft Cloud for US Government
- Parceiros CSP

**Funções apropriadas**

- Agente administrativo
- Administrador de cobrança
- Administrador global
- Agente de suporte técnico
- Agente de vendas

Depois de criar um registro de seu cliente no Partner Center, você pode vender as assinaturas para os produtos no catálogo. Isso inclui produtos publicados pela Microsoft, bem como produtos SaaS (software como serviço) publicados por ISVs (fornecedores de software independentes) de terceiros no [mercado comercial](https://azuremarketplace.microsoft.com/marketplace).

Algumas ofertas são limitadas a uma assinatura por cliente. Para ver uma lista das ofertas restritas, visite a página Ofertas e Preços do Partner Center.

>[!IMPORTANT]
Como um parceiro no programa CSP, você só pode comprar assinaturas SaaS **baseadas em licença** de editores ISV no Partner Center. Isso significa que você pode comprar qualquer oferta de SaaS **baseada em licença** que o editor ISV disponibilizou para você, incluindo [ofertas exclusivas](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) às quais você tem acesso. Para comprar ou gerenciar outras ofertas de Marketplace comercial de ISVs (como ofertas baseadas em **uso**, limitadas ou de consumo que envolvem aplicativos, contêineres ou VMS do Azure), você deve ir para o [portal de gerenciamento do Azure](https://portal.azure.com/). Para obter mais informações, consulte [comprar produtos comerciais do Marketplace](csp-commercial-marketplace-purchase.md).

## <a name="create-a-new-subscription"></a>Criar uma nova assinatura

1. Entre no [painel](https://partner.microsoft.com/dashboard) do Partner Center.

2. No menu do centro de parceiros, **selecione**clientes e, em seguida, escolha um cliente na lista.

3. Selecione **Adicionar assinatura**. A guia **serviços online** mostrará todas as ofertas de SaaS do Marketplace disponíveis.

4. Para ver apenas determinados tipos de assinaturas, faça seleções nos filtros disponíveis:
   - **Publicador**: escolha a **Microsoft** para ver apenas as ofertas da Microsoft ou o **parceiro** para ver os produtos do Marketplace comercial publicados por ISVs.
   - **Tipo de cobrança**: selecione o tipo de cobrança de assinatura que você deseja usar: **licença** ou **uso**. Consulte [as perguntas frequentes sobre](faq-about-new-billing-features.md) novos recursos de cobrança para obter informações que o ajudarão a decidir entre a frequência de cobrança mensal e anual.
   - **Categoria**: escolha **Enterprise**, **Small Business**ou **Trial**. Para obter informações sobre assinaturas de avaliação, consulte [oferecer a seus clientes avaliações de produtos da Microsoft](offer-your-customers-trials-of-microsoft-products.md).

5. Selecione as assinaturas de produto que você deseja comprar para o cliente. Os produtos que você vê dependem do tipo de segmento de cliente (educação, governo, etc.) e dos filtros que você aplicou. Algumas ofertas mostradas no Marketplace talvez nem sempre estejam disponíveis para um cliente específico ou um parceiro CSP específico. Isso pode ocorrer porque:

    - O cliente já tem uma assinatura para esse produto e só é permitido um

    - A assinatura do cliente pode ter sido suspensa (nesse caso, você pode reativar a assinatura em vez de comprar uma nova).

    - Para ofertas de SaaS de ISV, pode haver alguns motivos pelos quais a oferta não está disponível para compra: o ISV pode não oferecer suporte ao país ou à região de cobrança do cliente; Talvez o ISV tenha optado por não disponibilizar a oferta por meio do programa CSP; ou, o ISV pode ter tornado a oferta [exclusiva](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) para apenas determinados parceiros CSP. A oferta de ISV também pode não ser proficada por meio do Partner Center (por exemplo, contêineres ou algumas ofertas baseadas em uso).  

6. Para cada assinatura que você deseja adicionar, insira o número de licenças (se necessário) e selecione **Adicionar ao carrinho**.

7. Quando terminar de adicionar assinaturas, selecione **revisar** e examine seu pedido.

8. Depois de revisar seus pedidos e estar pronto para comprar essas assinaturas, selecione **comprar**.

9. Depois de comprar uma assinatura para um cliente, ocorrerá o seguinte:

    - Você pode revisar ou editar a assinatura selecionando o nome da assinatura na página de **assinaturas** do cliente. A partir daqui, você pode selecionar licenças de complemento, se houver alguma disponível, alterar a quantidade de licenças ou suspender a assinatura.

    **Para assinaturas do SaaS do ISV (baseadas em licença):**
    - Você receberá um link para o site do fornecedor ISV. Esse link deve ajudá-lo a concluir a configuração de implantação ou conta da assinatura do cliente. (Observe que nem você nem seu cliente receberá um email com instruções para concluir a configuração/provisionamento de conta para esse tipo de assinatura de ISV.)

    - Se sua assinatura vier com uma avaliação gratuita de 30 dias, o período de avaliação gratuita será aplicado automaticamente. Como um parceiro no programa CSP, não é possível renunciar ao período de avaliação gratuita em ofertas que você compra para os clientes. Depois que o período de avaliação gratuita terminar, o prazo da assinatura será iniciado e a assinatura será convertida em status pago. Em seguida, a assinatura será renovada de acordo com a mesma agenda.

## <a name="suspend-or-cancel-a-subscription"></a>Suspender ou cancelar uma assinatura

Os parceiros podem suspender ou cancelar uma assinatura se solicitado pelo cliente ou em casos de fraude ou falta de pagamento.

### <a name="suspend-a-subscription"></a>Suspender uma assinatura

Quando você alterar o status de uma assinatura para **Suspensa**, os usuários não poderão entrar nem acessar os serviços.

1. Entre no [painel](https://partner.microsoft.com/dashboard) do Partner Center.

2. No menu do centro de parceiros, **selecione**clientes e, em seguida, escolha um cliente na lista.

3. Escolha a assinatura que deseja gerenciar.

4. Na seção **Status**, escolha **Suspensa**. **Envie** suas alterações.

5. Todos os dados serão excluídos, a menos que a assinatura seja reativada dentro de 90 dias ou 90 dias mais o número de dias entre a hora em que a conta foi aberta e o primeiro período de cobrança (máximo de 120 dias).

Quando você suspende uma assinatura, a data que você vê abaixo **do** botão suspenso indica quando a assinatura expirará automaticamente se você não a reativar. Para obter mais informações, consulte [perguntas frequentes sobre novos recursos de cobrança](faq-about-new-billing-features.md).

### <a name="cancel-a-subscription"></a>Cancelar uma assinatura

Você tem a opção de cancelar assinaturas de SaaS baseadas em licença de editores de ISVs de terceiros no [Marketplace comercial](csp-commercial-marketplace-overview.md)do Partner Center. Desde que você Cancele dentro do período de cancelamento, você receberá um reembolso total.

Para ofertas de ISV cobradas mensalmente:

- Se você cancelar menos de 24 horas depois de colocar o pedido, receberá um crédito completo na próxima fatura.

- Se você cancelar mais tarde que 24 horas depois de colocar o pedido, o cancelamento será agendado para ocorrer na renovação.

Para ofertas cobradas anualmente:

- Se você cancelar menos de 14 dias depois de fazer o pedido, receberá um crédito completo na próxima fatura.

- Se você cancelar depois de 14 dias depois de fazer o pedido, o cancelamento será agendado para ocorrer na renovação.

Depois que esses períodos terminarem, você não verá mais a opção de cancelar a assinatura.

> [!NOTE]
> Os serviços ISV de terceiros baseados em uso e limitados (que usam máquinas virtuais ou contêineres, por exemplo) não são elegíveis para retorno. Os serviços baseados em uso podem ser desprovisionados como um método de cancelamento. Como os encargos são cobrados após o uso, esses serviços não são elegíveis para reembolso.

Para cancelar uma assinatura de SaaS baseada em licença de um publicador ISV, faça o seguinte:

1. Entre no [painel](https://partner.microsoft.com/dashboard) do Partner Center.

2. No menu do centro de parceiros, **selecione**clientes e, em seguida, escolha um cliente na lista.

3. Localize a assinatura que você deseja cancelar.

4. Na coluna **status** , selecione **Cancelar**. **Envie** suas alterações.

5. Se uma caixa de diálogo for exibida, preencha todos os detalhes relevantes e selecione **Enviar**.

6. Para confirmar o cancelamento, selecione **Sim, cancelar**.

> [!NOTE]
> Você também pode optar por cancelar uma assinatura do Azure Marketplace usando APIs. Para fazer isso, consulte [cancelar uma assinatura do Azure Marketplace](https://docs.microsoft.com/partner-center/develop/cancel-an-azure-marketplace-subscription).

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a>Escolha se deseja renovar automaticamente uma assinatura do Marketplace comercial

Por padrão, as assinaturas ativas são definidas para renovar automaticamente quando o período de assinatura expira. Para [assinaturas para produtos](csp-commercial-marketplace-overview.md)do Marketplace comercial, opcionalmente, você pode optar por não renovar automaticamente a assinatura.

Para interromper uma assinatura do Marketplace comercial ativa de renovar automaticamente:

1. Entre no [painel](https://partner.microsoft.com/dashboard) do Partner Center.

2. No menu do centro de parceiros, **selecione**clientes e, em seguida, escolha um cliente na lista.

3. Selecione **assinaturas**. Isso lista todas as assinaturas baseadas em licença que você comprou para o cliente.

4. Na coluna **assinatura** , selecione a assinatura que você deseja modificar.

5. Na página detalhes da assinatura, localize a seção **status** e desmarque a caixa **renovação automática** .

6. Selecione **Enviar**.

## <a name="next-steps"></a>Próximas etapas

- [Comprar produtos do Marketplace comercial para seus clientes](csp-commercial-marketplace-purchase.md)

- [Gerenciar produtos do Marketplace comercial para seus clientes](csp-commercial-marketplace-manage.md)

- [Visão geral do marketplace comercial](csp-commercial-marketplace-overview.md)
