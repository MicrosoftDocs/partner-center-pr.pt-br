---
title: Como adquirir uma oferta de SaaS no portal do Azure
description: Saiba como localizar e comprar uma oferta de SaaS no portal do Azure.
author: mingshen-ms
ms.author: mingshen
ms.reviewer: dannyevers
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: how-to
ms.date: 06/04/2021
ms.openlocfilehash: b73a9acb7b9cf9eee1151de1f8e45f6fd6ef256f
ms.sourcegitcommit: 8511fec63961d8c77a4d1eea3e3f1d37cdea46c6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "112373470"
---
# <a name="purchase-a-saas-offer-in-azure-portal"></a>Comprar uma oferta de SaaS no portal do Azure

Este artigo explica as diferentes opções e requisitos de pesquisa, tentativa e compra de uma oferta de SaaS (software como serviço) da portal do Azure.

## <a name="saas-offers-discovery-in-azure-portal"></a>O SaaS oferece descoberta no portal do Azure

Quando estiver em portal do Azure, há algumas maneiras de restringir sua pesquisa para se concentrar nas ofertas de SaaS.

### <a name="narrowing-your-search"></a>Restringir sua pesquisa

Na página inicial, em **Serviços do Azure** , selecione **+ criar um recurso** ou **Marketplace**. Ou use o atalho **G + N** em qualquer lugar na plataforma.

- Restrinja os resultados às ofertas de SaaS usando o filtro de **tipo de oferta** e, em seguida, selecione **SaaS**.
- Use a barra de pesquisa global na área de navegação superior para encontrar uma oferta de SaaS específica.

Localize uma [oferta de SaaS particular](/marketplace/private-offers) selecionando a faixa na parte superior da página inicial do **Marketplace** . Nem todas as ofertas, ou os planos estão disponíveis em todas as regiões geográficas e algumas podem aparecer apenas para determinados locatários.

A exibição filtrada mostra cada oferta de SaaS disponível representada por um título. Selecione um para ver a página de detalhes do produto. Que inclui as seguintes seções:

- Visão geral – detalhes sobre o serviço, os materiais de marketing e aprendizado
- Planos + preços – cada oferta incluirá pelo menos um plano com preços e termos de cobrança diferentes
- Informações de uso + suporte – inclui ID do editor, ID da oferta e ID do plano
- Classificação e revisões da oferta de SaaS específica

## <a name="available-billing-models-plansskus-for-saas-offers"></a>Modelos de cobrança disponíveis (planos/SKUs) para ofertas de SaaS

Cada oferta de SaaS terá um ou mais planos. Cada oferta tem um modelo de preços associado a ela: taxa fixa ou por usuário. Cada preço do plano é uma taxa recorrente, que pode ter zero dólar (todos os preços listados são apenas para fins de exemplo e não se destinam a refletir os custos reais). Essa taxa é uma taxa fixa ou preço por usuário. Tipos de planos disponíveis:

- **Planos mensais** – taxa mensal recorrente; taxa mensal simples ou por usuário paga em uma recorrência mensal. Quando o termo terminar, o plano será renovado automaticamente.
- **Planos anuais** – taxa anual recorrente; taxa anual fixa ou por usuário paga em uma recorrência anual. Quando o termo terminar, o plano será renovado automaticamente.
- **Medidores personalizados** – juntamente com as tarifas recorrentes, um plano de tarifas simples também pode incluir dimensões limitadas personalizadas opcionais para o uso excedente não incluído na taxa fixa. Cada dimensão representa uma unidade faturável. Esse é um custo variável que muda de acordo com o uso de unidades limitadas, como: largura de banda, tíquetes ou email processados. Você será cobrado de acordo com o consumo dessas dimensões mensalmente. Observe que o consumo excedente começa somente quando você usou todas as unidades limitadas incluídas na taxa fixa.
- **Avaliação gratuita** – em alguns casos, o plano inclui um período de avaliação de um mês, durante o qual você pode usar o software gratuitamente.  Depois que o período de avaliação terminar, você será cobrado de acordo com seu plano. As ofertas de avaliação não são compatíveis com medidores personalizados.

Esses modelos de preços estão disponíveis para planos públicos e privados.

## <a name="saas-purchase-experience"></a>Experiência de compra de SaaS

1. Na página do produto, selecione um plano que atenda às suas necessidades e continue a **Configurar + assinar**
2. Como parte do processo de compra, você será redirecionado para a guia **noções básicas** e será necessário:
    1. Defina qual *assinatura* você gostaria de usar para cobrança. A assinatura do Azure que você usa deve ter um método de compra válido definido para ele. Você deve ter o nível certo de permissão ou ter um grupo de recursos sob essa assinatura com o nível certo de permissões. Além disso, seu país de cobrança deve ser um país onde a oferta está disponível para compra. As assinaturas do Azure sem um método de pagamento válido (por exemplo, uma assinatura do MSDN) só podem ser usadas para comprar planos gratuitos
    1. Escolha ou crie um *grupo de recursos* * ao qual o recurso SaaS pertencerá.
    1. Digite um *nome* para a assinatura de SaaS para identificá-lo facilmente mais tarde. Depois de adquirido, você não pode alterar o nome.
    1. Em **plano**, você verá o plano selecionado na página detalhada do produto (PDP). Se você não tiver feito uma seleção ativa no PDP, verá o plano padrão. Você pode alterar sua seleção selecionando o link **Alterar plano** . Selecione o termo de cobrança relevante e, em seguida, escolha outro plano. Você poderá alterar o plano após a compra, se o editor der suporte a ele. No entanto, você não poderá alterar o termo de mensal para anual ou de anual para mensal.
    1. Nos casos em que o modelo de preços é *por usuário*, talvez seja necessário especificar o número de *usuários*. O preço que você vê será alterado com base na assinatura, no plano e no termo que você selecionou.
3. Vá para a guia **marcas** -as *marcas* são pares de chave/valor definidos pelo usuário, que podem ser colocados diretamente em um recurso ou em um grupo de recursos. Você pode usar marcas para localizar facilmente seu recurso de SaaS posteriormente. Atualmente, o Azure permite até 50 marcas por recurso e grupo de recursos. As marcas podem ser colocadas em um recurso no momento da criação ou adicionadas a um recurso existente.
4. Continue a **examinar + assinar** para passar pelos detalhes da oferta e do plano.
    1. Examine *termos de uso*, as *emendas* e a *política de privacidade* do Publicador e também para o Azure Marketplace
    1. Você pode ser solicitado a adicionar seus detalhes de contato
    1. Examinar detalhes *básicos* e *marcas*
5. Após a confirmação, selecione **assinar**.

## <a name="saas-subscription-and-configuration"></a>Assinatura e configuração de SaaS

Quando você seleciona assinar, uma mensagem informa "sua assinatura de SaaS está em andamento". Esse processo deve levar alguns minutos, não feche a janela até que ela seja concluída.

Após a conclusão da assinatura, uma mensagem informa que sua assinatura de SaaS foi concluída e você deve configurar a conta para começar a aproveitar sua compra. Você também receberá um email solicitando que você ative a nova assinatura. Se você não for aquele que configurará a conta de SaaS, encaminhe esse email para a pessoa relevante.

Para concluir o processo e começar a usar o SaaS, você precisará começar a configurar sua assinatura. Ao selecionar o botão **configurar conta agora** , ele será redirecionado para o site do editor.

Você também pode verificar o status da sua assinatura selecionando o ícone "Bell" no canto superior direito do cabeçalho.

Se você não concluir o processo de configuração dentro de *30 dias*, essa assinatura de SaaS será *excluída* automaticamente. A cobrança será iniciada depois que sua conta estiver configurada no site do editor.

Mensagens de erro que você pode ter ao longo do processo:

- O *nome do plano do plano selecionado* não pode ser comprado em uma assinatura gratuita
  - Atualize sua conta, consulte https://aka.ms/UpgradeFreeSub para obter mais detalhes.

- A compra falhou porque não foi possível encontrar um cartão de crédito válido, nem um método de pagamento associado à sua assinatura do Azure.
  - Use uma assinatura do Azure diferente ou o cartão de crédito ou o método de pagamento atual add\update para esta assinatura e tente novamente.

- *Nome do plano do plano selecionado* de *nome* da oferta da oferta pelo editor do Publicador *da oferta* não está disponível para compra de acordo com as regras definidas pelo administrador de ti.
  - Entre em contato com seu administrador de ti.

- O *nome do plano do plano selecionado* do plano de oferta *selecionado* pelo Publicador *Editor da oferta* não está disponível para compra devido a configurações particulares do Marketplace feitas pelo administrador de ti do seu locatário.
  - Entre em contato com seu administrador de ti

- A compra falhou porque a condição de cobrança solicitada está vazia ou é inválida.
  - Tente comprar um termo de plano/cobrança diferente.

- A compra falhou porque não foi possível verificar sua assinatura no contrato legal.
  - Repetir. Se o erro persistir, tente fazer a compra usando uma assinatura diferente do Azure ou contate o suporte.

- Falha na compra da *oferta OfferId pelo* Publicador *PublisherID* . Atualmente, esta oferta não está disponível para compra.
  - Tente novamente depois. Se depois de uma hora você continuar recebendo essa mensagem de erro, entre em contato com o suporte.  

- Falha na compra da oferta *do plano de plano da oferta* *OfferId* pelo editor *PublisherID* . No momento, este plano não está disponível para compra.
  - Tente novamente depois. Se depois de uma hora você continuar recebendo essa mensagem de erro, entre em contato com o suporte. 

- O *endereço de email* do cliente com *ObjectID* de ID de objeto não tem autorização para executar a ação *DeploymentValidationAction* sobre o resourcegroup de escopo *; DeploymentScope* ou o escopo é inválido.  
  - Você receberá essa mensagem se não tiver as permissões corretas na assinatura/grupo de recursos do Azure.  
    Se o acesso foi concedido recentemente, atualize suas credenciais.  
    Para implantar recursos em um grupo de recursos, você deve ter pelo menos acesso de Colaborador. Verifique o status de acesso em **Grupos de Recursos** e, em seguida, Controle de **Acesso.** Isso mostra quem é o 'Proprietário', a quem você pode pedir para atribuí-lo como um 'Colaborador'.

- A assinatura usada para essa compra não permite compras do Marketplace.  
  - Use uma assinatura diferente ou peça ao administrador para alterar a definição dessa assinatura e tentar novamente.

## <a name="next-steps"></a>Próximas etapas

- Se você estiver vendendo sua oferta pela Microsoft, acesse [Como adicionar um público de pré-visualização para sua oferta de SaaS](/azure/marketplace/create-new-saas-offer-preview).
- Caso contrário, vá para [Como vender sua oferta de SaaS](/azure/marketplace/create-new-saas-offer-marketing).
