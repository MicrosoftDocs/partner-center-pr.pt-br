---
title: Criar assinaturas de cliente no Partner Center
ms.topic: how-to
ms.date: 05/19/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como vender assinaturas para seus clientes para produtos publicados pela Microsoft, bem como produtos de SaaS publicados por ISVs de terceiros.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 9052954c81ef55a2bfa06778ace651c9d0f9b26f
ms.sourcegitcommit: e0444145d7720df948b9d02ae2469206db48dba5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110201401"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a>Criar, suspender ou cancelar assinaturas de clientes

**Aplica-se a**: Partner Center | Partner Center para Microsoft Cloud do governo dos EUA

**Funções apropriadas**: agente de administração | Administrador de cobrança | Administrador global | Agente de assistência técnica | Agente de vendas

Depois de criar um registro de seu cliente no Partner Center, você pode vender as assinaturas para os produtos no catálogo. Isso inclui produtos publicados pela Microsoft e por produtos SaaS (software como serviço) publicados por ISVs (fornecedores de software independentes) de terceiros no [mercado comercial](https://azuremarketplace.microsoft.com/marketplace).

Algumas ofertas são limitadas a uma assinatura por cliente. Para ver uma lista das ofertas restritas, visite a página Ofertas e Preços do Partner Center.

>[!IMPORTANT]
> Como um parceiro no programa CSP, você pode comprar assinaturas SaaS **limitadas** ou **baseadas em licença** de editores ISV no Partner Center. Isso significa que você pode comprar qualquer oferta de SaaS **limitada** ou **baseada em licença** que o editor ISV tenha disponibilizado para você, incluindo [ofertas exclusivas](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) às quais você tem acesso. Para comprar ou gerenciar outras ofertas de Marketplace comercial de ISVs (como ofertas baseadas em uso que envolvem aplicativos, contêineres ou VMs do Azure), você deve ir para a [portal do Azure](https://portal.azure.com/).

>[!NOTE]
>Todas as datas e horas no Partner Center são fornecidas no padrão de tempo UTC (tempo Universal Coordenado). Isso pode ser diferente em até 24 horas a partir de sua hora local.

## <a name="create-a-new-subscription"></a>Criar uma nova assinatura

1. Entre no painel [Partner Center](https://partner.microsoft.com/dashboard).

2. No menu do centro de parceiros, **selecione** clientes e, em seguida, escolha um cliente na lista.

3. Selecione **Adicionar assinatura**. A guia **serviços online** mostrará todas as ofertas de SaaS do Marketplace disponíveis.

4. Para ver apenas determinados tipos de assinaturas, faça seleções nos filtros disponíveis:
   - **Publicador**: escolha a **Microsoft** para ver apenas as ofertas da Microsoft ou o **parceiro** para ver os produtos do Marketplace comercial publicados por ISVs.
   - **Tipo de cobrança**: selecione o tipo de cobrança de assinatura que você deseja usar: **licença** ou **uso**. Consulte [cobrança baseada em licença](license-based-billing.md) para obter informações que o ajudarão a decidir entre a frequência de cobrança mensal e anual.
   - **Categoria**: escolha **Enterprise**, **Small Business** ou **Trial**. Para obter informações sobre assinaturas de avaliação, consulte [oferecer a seus clientes avaliações de produtos da Microsoft](offer-your-customers-trials-of-microsoft-products.md).

5. Selecione as assinaturas de produto que você deseja comprar para o cliente. Os produtos que você vê dependem do tipo de segmento de cliente (educação, governo etc.) e dos filtros que você aplicou. Algumas ofertas mostradas no Marketplace nem sempre podem estar disponíveis para um cliente específico ou um parceiro CSP específico. Isso pode ser porque:

   - O cliente já tem uma assinatura para esse produto e só tem permissão para uma

   - A assinatura do cliente pode ter sido suspensa (nesse caso, você pode reativar a assinatura em vez de comprar uma nova.)

   - Para ofertas de SaaS isv, pode haver alguns motivos pelos quais a oferta não está disponível para compra: o ISV pode não dar suporte ao país ou região de cobrança do cliente; O ISV pode ter optado por não disponibilizar a oferta por meio do programa CSP; ou, o ISV pode ter feito a oferta [exclusiva apenas](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) para determinados parceiros do CSP. A oferta isv também pode não ser transactável por meio do Partner Center (por exemplo, contêineres ou algumas ofertas baseadas em uso).  

6. Para cada assinatura que você deseja adicionar, insira o número de licenças (se necessário) e **selecione Adicionar ao carrinho**.

7. Quando terminar de adicionar assinaturas, selecione **Revisar** e revisar seu pedido.

8. Depois de revisar seus pedidos e estiver pronto para comprar essas assinaturas, selecione **Comprar**.

9. Depois de comprar uma assinatura para um cliente, ocorrerá o seguinte:

    - Você pode revisar ou editar a assinatura selecionando o nome da assinatura na página **Assinaturas desse** cliente. A partir daqui, você pode selecionar licenças de complemento, se houver alguma disponível, alterar a quantidade de licenças ou suspender a assinatura.

    **Para assinaturas de SaaS ISV (com base em licença e medição) :**
    - Você receberá um link para o site do publicador ISV. Esse link deve ajudá-lo a concluir a implantação ou a configuração da conta da assinatura do cliente.
      
    >[!NOTE]
    > Nem você nem seu cliente receberão um email com instruções para concluir a configuração/provisionamento da conta para esse tipo de assinatura isv.)

    - Se sua assinatura for fornecidas com uma avaliação gratuita de 30 dias, o período de avaliação gratuita será aplicado automaticamente. Como um parceiro no programa CSP, você não pode abrir mão do período de avaliação gratuita em ofertas que você compra para clientes. Depois que o período de avaliação gratuita terminar, o prazo da assinatura será iniciado e a assinatura será convertida em status pago. A assinatura será renovada automaticamente de acordo com a mesma agenda.
   
## <a name="update-subscriptions-with-add-ons"></a>Atualizar assinaturas com complementos 

Para comprar um complemento, o cliente deve primeiro ter uma assinatura base ativa.  Você não pode comprar complementos pelo catálogo.

1. Entre no [painel](https://partner.microsoft.com/dashboard) do Partner Center.

2. No menu do centro de parceiros, **selecione** clientes e, em seguida, escolha um cliente na lista.

3. Escolha a assinatura que deseja gerenciar.

4. Abaixo da seção **status** , há uma lista de Complementos disponíveis para a assinatura.  

5. Atualize a quantidade de licenças para cada complemento necessário. **Envie** suas alterações.

A capacidade de comprar Complementos por meio do Partner Center só está disponível para provedores diretos de fatura e indiretos.
Somente Complementos qualificados são exibidos com base nos requisitos básicos e na disponibilidade regional. Para obter mais informações sobre preços e ofertas, consulte a matriz de oferta de revendedor de nuvem. Suspender a assinatura base fará com que os complementos associados sejam suspensos.

As datas de início dos complementos estão alinhadas à assinatura base e as cobranças são calculadas da data de início à data de término de cobrança, com taxas proporcionais na primeira fatura. Para obter informações adicionais, consulte [cobrança baseada em licença](license-based-billing.md).


## <a name="suspend-or-cancel-a-subscription"></a>Suspender ou cancelar uma assinatura

Os parceiros podem suspender ou cancelar uma assinatura se solicitado pelo cliente ou em casos de fraude ou falta de pagamento.

### <a name="suspend-a-subscription"></a>Suspender uma assinatura

Quando você alterar o status de uma assinatura para **Suspensa**, os usuários não poderão entrar nem acessar os serviços.

1. Entre no [painel](https://partner.microsoft.com/dashboard) do Partner Center.

2. No menu do centro de parceiros, **selecione** clientes e, em seguida, escolha um cliente na lista.

3. Escolha a assinatura que deseja gerenciar.

4. Na seção **Status**, escolha **Suspensa**. **Envie** suas alterações.

5. Todos os dados serão excluídos, a menos que a assinatura seja reativada dentro de 90 dias ou 90 dias mais o número de dias entre a hora em que a conta foi aberta e o primeiro período de cobrança (máximo de 120 dias).

Quando você suspende uma assinatura, a data que você vê abaixo **do** botão suspenso indica quando a assinatura expirará automaticamente se você não a reativar. 

>[!NOTE]
>As assinaturas do CSP não têm um período expirado (o modo como as assinaturas diretas da Web fazem) durante a qual os serviços ainda estão funcionando, mas a assinatura não gera cobranças. As assinaturas do CSP estão ativas ou suspensas (ou completamente excluídas).

### <a name="cancel-a-subscription"></a>Cancelar uma assinatura

Você pode cancelar assinaturas SaaS baseadas em licenças de editores de ISVs de terceiros no [Marketplace comercial](csp-commercial-marketplace-overview.md)do Partner Center. Desde que você Cancele dentro do período de cancelamento, você receberá um reembolso total.

Para ofertas de ISV cobradas mensalmente:

- Se você cancelar menos de 24 horas depois de colocar o pedido, receberá um crédito completo na próxima fatura.

- Se você cancelar mais tarde que 24 horas depois de colocar o pedido, o cancelamento será agendado para ocorrer na renovação.

Para ofertas cobradas anualmente:

- Se você cancelar menos de 14 dias depois de fazer o pedido, receberá um crédito completo na próxima fatura.

- Se você cancelar depois de 14 dias depois de fazer o pedido, o cancelamento será agendado para ocorrer na renovação.

Depois que esses períodos terminarem, você não verá mais a opção de cancelar a assinatura.

> [!NOTE]
> Serviços ISV de terceiros baseados em uso e monitorados (que usam máquinas virtuais ou contêineres, por exemplo) não são qualificados para retorno. Os serviços baseados em uso podem ser des provisionados como um método de cancelamento. Como os encargos são cobrados após o uso, esses serviços não são qualificados para um reembolso.

Para cancelar uma assinatura de SaaS baseada em licença de um publicador ISV, faça o seguinte:

1. Entre no [painel](https://partner.microsoft.com/dashboard) do Partner Center.

2. No menu do centro de parceiros, **selecione** clientes e, em seguida, escolha um cliente na lista.

3. Localize a assinatura que você deseja cancelar.

4. Na coluna **Status,** selecione **Cancelar**. **Envie** suas alterações.

5. Se uma caixa de diálogo for exibida, preencha todos os detalhes relevantes e selecione **Enviar**.

6. Para confirmar o cancelamento, selecione **Sim, cancele**.

> [!NOTE]
> Você também pode optar por cancelar uma assinatura Azure Marketplace usando APIs. Para fazer isso, consulte [Cancelar uma assinatura Azure Marketplace .](/partner-center/develop/cancel-an-azure-marketplace-subscription)

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a>Escolha se deseja renovar automaticamente uma assinatura do Marketplace comercial

Por padrão, as assinaturas ativas são definidas para serem renovadas automaticamente ao término do período de assinatura. Para [assinaturas de produtos do marketplace comercial,](csp-commercial-marketplace-overview.md)opcionalmente, você pode optar por não renovar automaticamente a assinatura.

Para impedir que uma assinatura ativa do marketplace comercial seja renovada automaticamente:

1. Entre no [painel](https://partner.microsoft.com/dashboard) do Partner Center.

2. No menu do centro de parceiros, **selecione** clientes e, em seguida, escolha um cliente na lista.

3. Selecione **Assinaturas**. Isso lista todas as assinaturas baseadas em licença que você comprou para o cliente.

4. Na coluna **Assinatura,** selecione a assinatura que você deseja modificar.

5. Na página de detalhes da assinatura, localize a **seção Status** e desmarque a **caixa Renovação** automática.

6. Selecione **Enviar**.

## <a name="next-steps"></a>Próximas etapas

- [Comprar produtos do Marketplace comercial para seus clientes](csp-commercial-marketplace-purchase.md)

- [Gerenciar produtos do marketplace comercial para seus clientes](csp-commercial-marketplace-manage.md)

- [Visão geral do marketplace comercial](csp-commercial-marketplace-overview.md)