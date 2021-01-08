---
title: Gerenciar produtos do Marketplace & ofertas
ms.topic: how-to
ms.date: 07/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Usando o Partner Center, saiba como os provedores de soluções na nuvem podem gerenciar ofertas de ISV de terceiros adquiridas para clientes do mercado comercial.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5e6ca188aeb50cec6f847afb08be4a9d62b36984
ms.sourcegitcommit: a78dd3c532860d01867d116bfb4e2c88b84bcd25
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/08/2021
ms.locfileid: "97979669"
---
# <a name="manage-commercial-marketplace-products-and-offers-for-your-customers"></a>Gerenciar produtos e ofertas do Marketplace comercial para seus clientes


**Funções apropriadas**

- Administrador global
- Agente administrativo

Os parceiros no programa CSP (provedor de soluções de nuvem) podem usar o portal do Partner Center para comprar muitas ofertas ou assinaturas de SaaS de ISV para seus clientes a partir do mercado comercial. Depois de comprar uma oferta, você tem várias maneiras de gerenciá-la.

## <a name="view-or-edit-a-subscription"></a>Exibir ou editar uma assinatura

Depois de comprar uma assinatura de um Publicador ISV de terceiros, você pode revisá-la ou editá-la da seguinte maneira:

1. Entre no [painel](https://partner.microsoft.com/dashboard)do Partner Center e selecione **clientes** no menu de navegação à esquerda.

2. Selecione um cliente apropriado e, em seguida, selecione **assinaturas**. Isso lista todas as assinaturas baseadas em licença que você comprou para o cliente.

3. Na coluna **assinatura** , selecione a assinatura que você deseja exibir ou editar. Isso fornece mais informações para configurar ou provisionar a oferta. (Se mais ações forem necessárias na oferta, você também poderá ver um status "ação necessária" exibido na coluna status. Isso também pode ser acompanhado por um link para o site do editor ISV.)

4. Depois de selecionar a assinatura que você deseja exibir ou editar, a página de detalhes da assinatura permite que você edite a assinatura e faça coisas como:

    - Alterar o apelido da assinatura

    - Adicionar/diminuir o número de licenças na assinatura

    - Cancelar a assinatura

    - Desativar a renovação automática

    - Adicionar uma ID de MPN do revendedor indireta, se aplicável

> [!NOTE]
> Talvez seja necessário concluir determinadas etapas definidas pelo editor ISV antes de executar algumas alterações em uma assinatura, como o cancelamento de uma assinatura.

## <a name="assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer"></a>Atribuir licenças e ativar uma assinatura em nome de um cliente

Quando você adquire uma oferta de SaaS (software como serviço) fornecida por um editor independente de fornecedor de software (ISV) no mercado comercial, o editor ISV ajuda a gerenciar o processo de atribuição de licenças e ativação da assinatura em nome do cliente.

O Publicador deve fornecer um link personalizado e um código de autorização que identifica sua compra específica.

1. Você pode encontrar esse link personalizado do Publicador ISV de algumas maneiras:

   - Você pode ver o link na página de confirmação que aparece depois de comprar uma oferta de SaaS de ISV. Para localizar esse link na página, procure e selecione **ir para o site do Publicador**.

   - Você pode ver o link da página de assinaturas do cliente específico. Este link do Publicador aparece na linha associada à oferta de ISV ou à assinatura adquirida para o cliente.

   - Você pode [recuperar o link usando as APIs do Partner Center](/partner-center/develop/get-activation-link-by-order-line-item).

   > [!NOTE]
   > Para fazer isso em nome do cliente, talvez seja necessário copiar o link personalizado, colá-lo em um navegador privado e inserir as credenciais do cliente.

2. Quando você estiver no site ou no sistema do ISV Publisher, o editor permitirá que você conheça as etapas adicionais que precisa seguir para concluir o processo de configuração do cliente e provisionar ou atribuir licenças.

3. Como um parceiro no programa CSP que está trabalhando em nome de seu cliente, você é responsável por executar as seguintes tarefas:

    - Envie todas as informações necessárias para o Publicador.

    - Enviar qualquer URL necessária diretamente ao cliente (ou, de outra forma, comunicar diretamente os detalhes sobre essa assinatura para o cliente)

4. Depois de fornecer as informações necessárias ao Publicador, o Publicador provisionará e atribuirá as licenças apropriadas. A cobrança da assinatura será iniciada somente depois que os seguintes eventos ocorrerem:

    - O editor ISV atribuiu com êxito as licenças apropriadas

    - O editor ISV confirmou à Microsoft (por meio de uma API de preenchimento de SaaS separada) que a configuração da conta foi concluída com êxito

## <a name="cancel-a-license-based-saas-subscription-from-an-isv-publisher"></a>Cancelar uma assinatura SaaS baseada em licença de um editor ISV

Ao assinar um produto SaaS baseado em licença oferecido por um editor ISV dentro do mercado comercial, você tem a opção de cancelar a assinatura em seu período de cancelamento designado. Esse período de cancelamento é alterado dependendo se você tem uma assinatura mensal ou anual. Você também pode escolher se deseja ou não renovar automaticamente a assinatura.

Para obter mais informações sobre períodos de cancelamento que se aplicam, como cancelar ou como renovar uma assinatura automaticamente, consulte:

- [Cancelar uma assinatura](create-a-new-subscription.md#cancel-a-subscription)

- [Renovar automaticamente uma assinatura do Marketplace comercial](create-a-new-subscription.md#choose-whether-to-automatically-renew-a-commercial-marketplace-subscription)

## <a name="add-or-remove-licenses-for-a-saas-subscription"></a>Adicionar ou remover licenças para uma assinatura de SaaS

Para ofertas de Marketplace comercial de SaaS, você pode adicionar ou remover licenças de usuário para uma assinatura de cliente.

1. Entre no [painel](https://partner.microsoft.com/dashboard)do Partner Center e selecione **clientes** no menu de navegação à esquerda.

2. Selecione um cliente apropriado e, em seguida, selecione **assinaturas**. Isso lista todas as assinaturas baseadas em licença que você comprou para o cliente.

3. Na coluna **assinatura** , selecione a assinatura que você deseja modificar.

4. Na página detalhes da assinatura, localize o campo **quantidade** . É aí que você pode aumentar ou diminuir o número de licenças.

5. Altere a quantidade e, em seguida, selecione **Enviar**.

## <a name="manage-subscriptions-using-partner-center-apis"></a>Gerenciar assinaturas usando APIs do Partner Center

Você também pode usar as APIs do Partner Center para executar o gerenciamento do ciclo de vida e gerenciar faturas para suas assinaturas. Para obter mais informações, consulte [criar uma assinatura para produtos do Marketplace comercial](/partner-center/develop/create-subscription-azure-marketplace-products).

## <a name="next-steps"></a>Próximas etapas

- [Comprar ofertas do Marketplace comercial](csp-commercial-marketplace-purchase.md)
- [Saiba mais sobre cobrança no Marketplace comercial](csp-commercial-marketplace-billing.md)