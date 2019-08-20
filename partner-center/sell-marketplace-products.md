---
title: Vender assinaturas de produtos do Azure Marketplace | Partner Center
ms.topic: article
ms.date: 08/07/2019
description: Você pode usar o Partner Center para vender suas assinaturas de clientes para produtos de software como serviço (SaaS) publicados no Azure Marketplace por fornecedores independentes de software (ISVs).
author: JnHs
ms.author: jenhayes
keywords: assinaturas, Marketplace, terceiros, ISV
ms.localizationpriority: medium
ms.openlocfilehash: 204a0638399034c753474bb0ce92434ca318f5bb
ms.sourcegitcommit: ea68a16c2ed386cca983dd3fa85032450eacf871
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/09/2019
ms.locfileid: "68860954"
---
# <a name="sell-subscriptions-to-azure-marketplace-products"></a>Vender assinaturas de produtos do Azure Marketplace

**Aplica-se a**

- Partner Center

Você pode usar o Partner Center para vender suas assinaturas de clientes para produtos de software como serviço (SaaS) publicados no [Azure Marketplace](https://azuremarketplace.microsoft.com/marketplace) por fornecedores independentes de software (ISVs). Isso pode ajudar a diferenciar sua empresa das demais e fornecer aos clientes pacotes de softwares que atendam a necessidades específicas. Você gerencia licenças e assinaturas para esses produtos SaaS do Azure Marketplace da mesma forma como faz para produtos da Microsoft.

Para obter mais informações sobre o Azure Marketplace , consulte as [perguntas frequentes](https://docs.microsoft.com/azure/marketplace/marketplace-faq-publisher-guide) do Azure Marketplace.

## <a name="view-marketplace-offers-and-pricing"></a>Exibir ofertas e preços do Marketplace

Para exibir todas as ofertas disponíveis, selecione **Marketplace** no menu de navegação à esquerda. Por padrão, você verá produtos de todos os tipos e categorias. Você pode filtrar por tipo e/ou categoria ou usar a caixa de pesquisa para procurar palavras-chave específicas. Selecione um produto para ver informações sobre o editor e as SKUs disponíveis, incluindo se um período de avaliação gratuita é oferecido ou não.

> [!NOTE]
> Alguns produtos que estão disponíveis no Azure Marketplace podem não ser mostrados aqui. Os ISVs podem decidir se devem ou não oferecer seus produtos aos parceiros do CSP (provedor de soluções na nuvem) no Partner Center. Se você vir um produto no Azure Marketplace que deseja oferecer aos seus clientes pelo Partner Center, encontre as informações de contato do editor no Azure Marketplace e expresse seu interesse.

Os preços dos produtos do Azure Marketplace podem ser alterados com frequência. Para obter informações de preços atuais para todos os produtos do Marketplace, selecione **Exportar lista de preço** no canto superior direito da página do **Marketplace**. Isso gerará uma planilha com todos os dados de preço. As informações de preço são atualizadas todos os dias, para que você possa verificá-las sempre que desejar obter os preços atuais.

> [!TIP]
> Se um produto desta lista oferecer uma avaliação gratuita, a planilha incluirá duas linhas para esse produto. Uma linha mostrará um preço zerado, indicando que uma avaliação gratuita está disponível. A outra linha incluirá o preço e o termo que serão aplicados após o término do período de avaliação.
>
> Se um produto nesta lista usar [cobrança limitada](https://docs.microsoft.com/azure/marketplace/partner-center-portal/saas-metered-billing), o campo de prazo ficará em branco.

## <a name="purchase-marketplace-products-for-your-customers"></a>Comprar produtos do Marketplace para seus clientes

A compra de assinaturas para produtos SaaS do Azure Marketplace segue o mesmo processo que a compra de assinaturas para produtos da Microsoft. Ao adicionar uma assinatura para um cliente, você pode optar por ver apenas as ofertas de ISVs do Marketplace selecionando **Parceiro** no filtro **Editor**. Para obter mais informações, consulte [Criar uma nova assinatura](create-a-new-subscription.md).

> [!IMPORTANT]
> Você só pode adquirir assinaturas de produtos SaaS (software como serviço) no Partner Center. Outros tipos de oferta (como aplicativos, contêineres ou VMs do Azure) são gerenciados com o portal do Azure e cobrados de acordo com o consumo. Uma assinatura do Azure existente é necessária para habilitar as soluções pré-pagas com o portal do Azure.

Observe que algumas ofertas que você vê na página **Marketplace** podem não estar disponíveis para um cliente específico. A disponibilidade pode ser afetada por vários fatores, incluindo se o ISV dá suporte ao país/região de cobrança do cliente.

> [!TIP]
> Você também pode usar [as APIs do Partner Center](https://docs.microsoft.com/partner-center/develop/)para criar assinaturas do Azure Marketplace para seus clientes. Para obter mais informações, consulte [Criar uma assinatura para produtos do Azure Marketplace](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products).

Com assinaturas para produtos do Azure Marketplace, você tem a opção de [cancelar a assinatura](https://docs.microsoft.com/partner-center/create-a-new-subscription#cancel-a-subscription) no período de cancelamento (24 horas para assinaturas mensais ou 14 dias para assinaturas anuais). Você também [pode escolher se deseja ou não renovar automaticamente a assinatura](https://docs.microsoft.com/partner-center/create-a-new-subscription#choose-whether-to-automatically-renew-an-azure-marketplace-subscription).

## <a name="license-activation-for-marketplace-products"></a>Ativação de licença para produtos do Marketplace

Para tipos de oferta de SaaS (software como serviço), a atribuição e a ativação de licenças são gerenciadas por meio do ISV (fornecedor independente de software) que publicou o produto. Para concluir esse processo, você precisará acessar o site do editor, usando um link personalizado com um código de autorização que permite que o editor identifique sua compra específica. Você pode encontrar esse link na página de confirmação que aparece depois de comprar uma oferta de SaaS e na página **Assinaturas** (na linha dessa oferta). Você também pode [usar as APIs do Partner Center para recuperar esse link](https://docs.microsoft.com/partner-center/develop/get-activation-link-by-order-line-item).

Ao visitar o site do Editor usando este link, você verá quais informações ou ações adicionais são necessárias para provisionar e atribuir licenças ou concluir o processo de instalação. As etapas necessárias podem variar dependendo do Editor e da oferta. Você é responsável por enviar todas as informações necessárias (ou enviar a URL para o cliente para fornecer essas informações diretamente). Depois que as informações necessárias forem fornecidas, o Editor provisionará e atribuirá as licenças apropriadas. A cobrança da assinatura será iniciada somente depois que as licenças tiverem sido atribuídas com êxito.

## <a name="access-billing-info-for-marketplace-products"></a>Acessar informações de cobrança para produtos do Marketplace

Para produtos do Marketplace, o período de cobrança começa no primeiro dia do mês e termina no último dia do mês. Disponibilizaremos sua fatura no oitavo dia do mês seguinte. Você pode acessar essas notas fiscais no Partner Center ou usando as APIs do Partner Center.

Para obter mais informações, consulte [Entendendo os tipos de cobrança no Partner Center](https://docs.microsoft.com/partner-center/billing-different-types#billing-for-one-time-and-select-recurring-charges).

## <a name="provide-support-for-customers-using-marketplace-products"></a>Fornecer suporte para clientes que usam produtos do Marketplace

Você permanecerá como o primeiro ponto de contato do seu cliente em caso de dúvidas sobre cobranças e gerenciamento de assinaturas. Para obter suporte técnico, você precisará entrar em contato com o Editor. A Microsoft não fornece suporte para produtos do Marketplace, mas fornecerá as informações de contato de suporte do editor para você.

Para obter mais informações, consulte o [Suporte para produtos do Azure Marketplace](https://docs.microsoft.com/partner-center/report-problems-on-behalf-of-a-customer#support-for-azure-marketplace-products) e [Fornecendo suporte aos seus clientes](https://docs.microsoft.com/partner-center/customer-support).

## <a name="manage-subscriptions-using-partner-center-apis"></a>Gerenciar assinaturas usando APIs do Partner Center

Você pode criar uma assinatura para produtos do Azure Marketplace usando as APIs do Partner Center, ao obter uma lista de ofertas para um mercado, criar e enviar um pedido para uma assinatura do Azure Marketplace e, em seguida, recuperar um link de ativação. Você também pode usar as APIs do Partner Center para executar o gerenciamento do ciclo de vida e gerenciar faturas para essas assinaturas.

Para obter mais informações, consulte [Criar uma assinatura para produtos do Azure Marketplace](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products).