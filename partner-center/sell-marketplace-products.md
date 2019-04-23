---
title: Vender assinaturas de produtos do Azure Marketplace | Partner Center
ms.topic: article
ms.date: 04/04/2019
description: Você pode usar o Centro de parceiros para vender seus clientes de assinaturas de Software como serviço (SaaS) produtos publicados no Azure Marketplace por fornecedores de Software independentes (ISVs).
author: JnHs
ms.author: jenhayes
keywords: assinaturas, mercado, por terceiros, o ISV
ms.localizationpriority: medium
ms.openlocfilehash: a086ab3a58e926d33c118690e7b171ba4f0fd18b
ms.sourcegitcommit: 41b6e677db10ef8e5d12f9240d3450f085ee6d91
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2019
ms.locfileid: "60124267"
---
# <a name="sell-subscriptions-to-azure-marketplace-products"></a>Vender assinaturas de produtos do Azure Marketplace

**Aplica-se a**

- Partner Center

Você pode usar o Partner Center para vender seus clientes assinaturas de Software como um serviço (SaaS) de produtos publicados [do Azure Marketplace](https://azuremarketplace.microsoft.com/marketplace) por fornecedores de Software independentes (ISVs). Isso pode ajudar a diferenciar sua empresa e fornece aos clientes com pacotes de software que atendem suas necessidades de negócios específicas. Gerenciar licenças e assinaturas para esses produtos de SaaS do Azure Marketplace assim como faria para produtos da Microsoft.

Para obter mais informações sobre o Azure Marketplace, consulte [perguntas frequentes do Azure Marketplace](https://docs.microsoft.com/azure/marketplace/marketplace-faq-publisher-guide).

## <a name="view-marketplace-offers-and-pricing"></a>Preços e ofertas do Marketplace de modo de exibição

Para exibir todas as ofertas disponíveis, selecione **Marketplace** no menu de navegação à esquerda. Por padrão, você verá os produtos de todos os tipos e categorias. Você pode filtrar por tipo e/ou categoria, ou use a caixa de pesquisa para pesquisar palavras-chave específicas. Selecione um produto para ver informações sobre o publicador e os SKUs disponíveis.

> [!NOTE]
> Alguns produtos que estão disponíveis no Azure Marketplace podem não ser exibidos aqui. Os ISVs podem decidir se deseja ou não oferecer seus produtos para os parceiros de provedor de solução de nuvem (CSP) no Partner Center. Se você vir um produto no Azure Marketplace que você deseja oferecer aos seus clientes por meio do Partner Center, encontrar as informações de contato do editor no Marketplace do Azure e informe que você está interessado.

Os preços para produtos do Azure Marketplace podem mudar frequentemente. Para obter informações de preços atual para todos os produtos do Marketplace, selecione **lista de preços de exportação** no canto superior direito da **Marketplace** página. Isso irá gerar uma planilha com todos os dados de preços. Informações de preço é atualizada diariamente, para que você possa verificá-lo sempre que você gostaria de obter os preços atuais.

## <a name="purchase-marketplace-products-for-your-customers"></a>Comprar produtos do Marketplace para seus clientes

Aquisição de assinaturas para produtos de SaaS do Azure Marketplace segue o mesmo processo de aquisição de assinaturas para produtos da Microsoft. Ao adicionar uma assinatura para um cliente, você pode optar por ver apenas o Marketplace oferece de ISVs, selecionando **parceiro** na **Publisher** filtro. Para obter mais informações, consulte [criar uma nova assinatura](create-a-new-subscription.md).

> [!IMPORTANT]
> Você só poderá comprar o Software como um assinaturas de produto do serviço (SaaS) no Partner Center. Outros tipos de oferta (como aplicativos do Azure, contêineres ou VMs) são gerenciados por meio do portal do Azure e cobrados de acordo com o consumo. Uma assinatura do Azure existente é necessária para habilitar soluções pago conforme o uso por meio do portal do Azure.

Observe que alguns oferece o que você vê na **Marketplace** página pode não estar disponível para um cliente específico. Disponibilidade pode ser afetada por uma série de fatores, incluindo se o ISV oferece suporte à cobrança país/região do cliente.

> [!TIP]
> Você também pode usar [APIs do Partner Center](https://docs.microsoft.com/partner-center/develop/) para criar assinaturas do Azure Marketplace para seus clientes. Para obter mais informações, consulte [criar uma assinatura para produtos do Azure Marketplace](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products).

Com as assinaturas para produtos do Azure Marketplace, você tem a opção de [cancelar a assinatura](https://docs.microsoft.com/partner-center/create-a-new-subscription#cancel-a-subscription) dentro do período de cancelamento (24 horas para as assinaturas mensais ou 14 dias para as assinaturas anuais). Você também pode [escolha se deseja ou não automaticamente renovar a assinatura](https://docs.microsoft.com/partner-center/create-a-new-subscription#choose-whether-to-automatically-renew-an-azure-marketplace-subscription).

## <a name="access-billing-info-for-marketplace-products"></a>Acessar informações de cobrança para produtos do Marketplace

Para produtos do Marketplace, o período de cobrança começa no primeiro dia do mês do calendário e termina no último dia do mês do calendário. Que disponibilizaremos sua fatura no dia 8 do mês seguinte. Você pode acessar essas notas fiscais no Partner Center ou por meio de APIs do Partner Center.

Para obter mais informações, consulte [Noções básicas sobre os tipos de cobrança no Partner Center](https://docs.microsoft.com/partner-center/billing-different-types#billing-for-one-time-and-select-recurring-charges).

## <a name="provide-support-for-customers-using-marketplace-products"></a>Fornecer suporte para clientes que usam produtos do Marketplace

Assim como ocorre com produtos da Microsoft, você deve ser o primeiro ponto de contato do seu cliente para perguntas sobre o gerenciamento de cobrança e assinatura. Para obter suporte técnico, você precisará entrar em contato com o publicador. Microsoft não oferece suporte para produtos do Marketplace, mas fornecerá informações de contato de suporte do Editor para você.

Para obter mais informações, consulte [suporte para produtos do Azure Marketplace](https://docs.microsoft.com/partner-center/report-problems-on-behalf-of-a-customer#support-for-azure-marketplace-products) e [fornecer suporte a seus clientes](https://docs.microsoft.com/partner-center/customer-support).

## <a name="manage-subscriptions-using-partner-center-apis"></a>Gerenciar assinaturas usando APIs do Partner Center

Você pode criar uma assinatura para produtos do Azure Marketplace usando APIs do Partner Center, obtendo uma lista de ofertas para um mercado, criar e enviar um pedido para uma assinatura do Azure Marketplace e recuperando um link de ativação. Você também pode usar as APIs do Partner Center para executar o gerenciamento de ciclo de vida e gerenciar as faturas por essas assinaturas.

Para obter mais informações, consulte [criar uma assinatura para produtos do Azure Marketplace](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products).