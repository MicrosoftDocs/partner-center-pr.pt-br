---
title: Descobrir ofertas – marketplace comercial
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como os parceiros do CSP podem usar Partner Center para exibir ou pesquisar ofertas de SaaS ou preços no marketplace de ISVs (Fornecedores Independentes de Software).
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ab30f8391df58155c8511dc628b1fefd94c8d768
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147965"
---
# <a name="discover-offers-and-pricing-in-partner-center-commercial-marketplace"></a>Descobrir ofertas e preços no Partner Center marketplace comercial

**Funções apropriadas:** administrador global | Agente administrador

Quando isVs (fornecedores independentes de software) optam por publicar uma oferta no marketplace comercial, eles também podem decidir se querem que a oferta seja disponibilizada no programa CSP. Se eles optarem por vender a oferta por meio do programa CSP, os parceiros do CSP deverão ver a oferta na Partner Center marketplace.

Se uma oferta de ISV não aparecer como você espera no Partner Center, pode ser porque:

- O ISV decidiu não vender a oferta por meio do programa CSP. Por exemplo, alguns produtos ISV podem ter sido disponibilizados em outras áreas do marketplace comercial (como no [Microsoft AppSource](https://appsource.microsoft.com/) e [no Azure Marketplace](https://azuremarketplace.microsoft.com/)), mas podem não aparecer para parceiros no programa CSP no Partner Center marketplace.

- O ISV decidiu tornar a oferta exclusiva apenas para um número selecionado de parceiros CSP. Para obter mais informações sobre ofertas exclusivas, consulte mais adiante neste tópico de ajuda.

- O tipo de oferta pode não ser transactável por meio de Partner Center ou portal do Azure (por exemplo, contêineres ou algumas ofertas baseadas em uso).

- O país de cobrança de seus clientes associados pode não ter suporte para essa oferta de ISV.

## <a name="view-marketplace-offers-in-partner-center"></a>Exibir ofertas do Marketplace Partner Center

Para exibir as ofertas do marketplace comercial disponíveis no programa CSP:

1. Entre no Partner Center [e](https://partner.microsoft.com/dashboard)selecione **CSP** no menu de navegação à esquerda.

2. Selecione **Vender**, seguido por **Marketplace.** Por padrão, você verá produtos de todos os tipos e categorias.

3. Selecione um filtro por tipo ou categoria. Você também pode usar **a Pesquisa** para encontrar palavras-chave específicas, nomes de oferta ou nomes de editores ISV.

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

3. Role para baixo até a seção **Marketplace** , selecione um local e baixe os **preços do Marketplace**. Isso gera uma planilha com os dados de preços mais recentes para SaaS, ofertas baseadas em licença e ofertas medida disponíveis de editores ISV. Alguns preços de aplicativo do Azure também podem aparecer aqui. Essas informações são atualizadas diariamente, para que você possa verificar os preços atuais com a frequência que escolher.

4. Se um produto ISV incluir um período de avaliação gratuita, a planilha exibirá duas linhas para esse produto:

    - Uma linha mostra o preço de avaliação gratuita de zero. Isso significa que um período de avaliação gratuita está disponível.

    - A outra linha mostra o preço e os termos que serão aplicados após o fim do período de avaliação gratuita.

Como parceiro do programa CSP, você pode estar qualificado para outros incentivos associados a determinadas ofertas do marketplace comercial. Para obter mais informações sobre outros incentivos, consulte o guia de incentivo do [CSP](https://aka.ms/partnerincentives) (requer logon do CSP).

## <a name="learn-about-marketplace-exclusive-offers"></a>Saiba mais sobre ofertas exclusivas do marketplace

OS ISVs têm a opção de disponibilizar suas ofertas somente para parceiros específicos no programa CSP. Isso é conhecido como uma oferta exclusiva. Todos os parceiros no programa CSP ainda podem exibir todas as ofertas de ISV Partner Center marketplace comercial, incluindo as ofertas marcadas como Exclusivas.

Se uma oferta não **estiver** marcada como Exclusiva, todos os parceiros poderão comprar essa oferta (supondo que o país de cobrança do cliente selecionado corresponde à disponibilidade do país da oferta do ISV).

No entanto, para qualquer oferta marcada como Exclusiva, somente os parceiros selecionados pelo ISV poderão comprar essa oferta.

> [!NOTE]
> Se você vir uma oferta marcada como Exclusiva que gostaria de vender para seus clientes, entre em contato com o ISV diretamente e peça permissão para vender a oferta Exclusiva. Ao exibir os detalhes de uma oferta Exclusiva, você poderá ver um link **do ISV** de Contato que você pode selecionar.

Para saber mais sobre a experiência de ISV no marketplace comercial, leia [Provedores de Soluções na Nuvem.](/azure/marketplace/cloud-solution-providers)

Para obter mais informações sobre a experiência do CSP no marketplace, leia [Visão geral do marketplace comercial.](csp-commercial-marketplace-overview.md)

## <a name="next-steps"></a>Próximas etapas

- [Comprar ofertas do marketplace comercial](csp-commercial-marketplace-purchase.md)