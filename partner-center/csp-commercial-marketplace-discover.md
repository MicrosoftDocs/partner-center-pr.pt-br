---
title: Ofertas de descoberta – Marketplace comercial
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como os parceiros do CSP podem usar o Partner Center para exibir ou pesquisar o Marketplace para ofertas de SaaS ou preços de ISVs (fornecedores independentes de software).
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e89473cf095be4cc87c96f1c2a6d0da224eccedd
ms.sourcegitcommit: f34f2f69e6df4f260479a205d94010cf47987ff2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/25/2020
ms.locfileid: "96038839"
---
# <a name="discover-offers-and-pricing-in-partner-center-commercial-marketplace"></a>Descubra ofertas e preços no Marketplace comercial do Partner Center

**Aplica-se a**

- Partner Center
- Parceiros no programa CSP

**Funções apropriadas**

- Administrador global
- Agente administrativo

Quando fornecedores independentes de software (ISVs) optam por publicar uma oferta no Marketplace comercial, eles também podem decidir se querem que a oferta seja disponibilizada no programa CSP. Se eles optarem por vender a oferta por meio do programa CSP, os parceiros CSP deverão ver a oferta na área Partner Center Marketplace.

Se uma oferta de ISV não aparecer conforme o esperado no Partner Center, talvez isso ocorra porque:

- O ISV decidiu não vender a oferta por meio do programa CSP. Por exemplo, alguns produtos de ISV podem ter sido disponibilizados em outras áreas do Marketplace comercial (como no [Microsoft AppSource](https://appsource.microsoft.com/) e no [Azure Marketplace](https://azuremarketplace.microsoft.com/)), mas podem não aparecer para parceiros no programa CSP no Partner Center Marketplace.

- O ISV decidiu tornar a oferta exclusiva para apenas um número selecionado de parceiros CSP. Para obter mais informações sobre ofertas exclusivas, consulte mais adiante neste tópico da ajuda.

- O tipo de oferta não pode ser acessado por meio do Partner Center ou portal do Azure (por exemplo, contêineres ou algumas ofertas baseadas em uso).

- O país de cobrança dos clientes associados pode não ter suporte para esta oferta de ISV.

## <a name="view-marketplace-offers-in-partner-center"></a>Exibir ofertas do Marketplace no Partner Center

Para exibir as ofertas do Marketplace comercial disponíveis no programa CSP:

1. Entre no [painel](https://partner.microsoft.com/dashboard)do Partner Center e selecione **CSP** no menu de navegação à esquerda.

2. Selecione **vender**, seguido pelo **Marketplace**. Por padrão, você verá produtos de todos os tipos e categorias.

3. Selecione um filtro por tipo ou categoria. Você também pode usar **Pesquisar** para localizar palavras-chave específicas, nomes de oferta ou os nomes de editores de ISV.

4. Selecione uma oferta de produto específica na lista. Isso levará você a uma guia Visão geral do produto, na qual você pode saber mais sobre a oferta. As informações sobre essa guia podem incluir: 

    - Uma descrição do produto ou da oferta

    - Mais informações sobre o ISV Publisher

    - Links para documentação ou materiais de marketing carregados pelo editor ISV

    - Outros possíveis contatos do ISV para suporte ao cliente, engenharia ou um contato para o programa CSP

5. Para ver mais informações sobre os planos, SKUs ou preços disponíveis de uma oferta, selecione a guia **planos + preços** . Esta guia mostrará:

    - Os mercados em que esta oferta está disponível para você

    - Uma lista de SKUs ou planos disponíveis para a oferta

    - Preço de cada SKU ou plano disponível

## <a name="view-marketplace-offers-via-partner-center-apis"></a>Exibir ofertas do Marketplace por meio de APIs do Partner Center

Os parceiros do programa CSP também podem usar APIs para retornar uma lista de ofertas qualificadas. As ofertas qualificadas serão apenas aquelas disponíveis para o parceiro para venda por meio do Partner Center Marketplace. Para parceiros que usam APIs para identificar ofertas no catálogo, consulte as diretrizes para [obter uma lista de ofertas para um mercado](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market).

## <a name="view-the-latest-marketplace-offer-pricing-in-partner-center"></a>Exibir os preços mais recentes da oferta do Marketplace no Partner Center

Siga estas etapas para obter os detalhes de preços mais recentes associados a uma oferta:

1. Entre no [painel](https://partner.microsoft.com/dashboard)do Partner Center e selecione **CSP** no menu de navegação à esquerda.

2. Selecione **vender**, seguido de **preços e ofertas**.

3. Role para baixo até a seção **Marketplace** , selecione um local e baixe os **preços do Marketplace**. Isso gera uma planilha com os dados de preços mais recentes para SaaS, ofertas baseadas em licença e ofertas limitadas disponíveis em editores de ISV. Alguns preços de aplicativo do Azure também podem aparecer aqui. Essas informações são atualizadas diariamente, para que você possa verificá-las em relação aos preços atuais com a frequência que escolher.

4. Se um produto ISV incluir um período de avaliação gratuita, a planilha exibirá duas linhas para esse produto:

    - Uma linha mostra o preço de avaliação gratuita de zero. Isso significa que um período de avaliação gratuita está disponível.

    - A outra linha mostra o preço e os termos que serão aplicados após o término do período de avaliação gratuita.

Como parceiro do programa CSP, você pode estar qualificado para outros incentivos associados a determinadas ofertas do Marketplace comercial. Para obter mais informações sobre outros incentivos, consulte o [Guia de incentivos do CSP](https://aka.ms/partnerincentives) (requer logon no CSP).

## <a name="learn-about-marketplace-exclusive-offers"></a>Saiba mais sobre ofertas exclusivas do Marketplace

Os ISVs têm a opção de disponibilizar suas ofertas somente para parceiros específicos no programa CSP. Isso é conhecido como uma oferta exclusiva. Todos os parceiros no programa CSP ainda podem exibir todas as ofertas de ISV no Marketplace comercial do Partner Center, incluindo as ofertas marcadas como exclusivas.

Se uma oferta **não** for marcada como exclusiva, todos os parceiros poderão comprar essa oferta (supondo que o país de cobrança do cliente selecionado corresponda à disponibilidade do país da oferta do ISV).

No entanto, para qualquer oferta marcada como exclusiva, somente os parceiros selecionados pelo ISV poderão comprar essa oferta.

> [!NOTE]
> Se você vir uma oferta marcada como exclusiva que gostaria de vender aos seus clientes, acesse o ISV diretamente e solicite permissão para vender a oferta exclusiva. Ao exibir os detalhes de uma oferta exclusiva, você poderá ver um link de **ISV de contato** que você pode selecionar.

Para saber mais sobre a experiência do ISV no Marketplace comercial, leia [provedores de soluções de nuvem](/azure/marketplace/cloud-solution-providers).

Para obter mais informações sobre a experiência do CSP no Marketplace, leia [visão geral do Marketplace comercial](csp-commercial-marketplace-overview.md).

## <a name="next-steps"></a>Próximas etapas

- [Comprar ofertas do Marketplace comercial](csp-commercial-marketplace-purchase.md)