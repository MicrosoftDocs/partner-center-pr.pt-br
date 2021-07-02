---
title: Como comprar uma oferta de SaaS no portal do Azure
description: Saiba como encontrar e comprar uma oferta de SaaS portal do Azure.
author: mingshen-ms
ms.author: mingshen
ms.reviewer: dannyevers
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: how-to
ms.date: 06/29/2021
ms.openlocfilehash: a124e4c5bb31a1fbb744bf2c5e1ea65a356bdd54
ms.sourcegitcommit: 1d09ccaaa54f167b0c63e99761172ebe84e89f2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2021
ms.locfileid: "113221433"
---
# <a name="purchase-a-saas-offer-in-azure-portal"></a>Comprar uma oferta de SaaS portal do Azure

Este artigo explica as diferentes opções e requisitos para pesquisar, tentar e comprar uma oferta de SaaS (software como serviço) da portal do Azure.

## <a name="create-a-saas-subscription"></a>Criar uma assinatura de SaaS

Para comprar uma assinatura de SaaS, você precisa de uma conta de usuário do Azure com acesso a uma assinatura apropriada do Azure. Essa assinatura será usada para cobrança, bem como para compartimentalização de seus recursos de nuvem comprados. Para saber mais sobre assinaturas do Azure, confira [Criar uma assinatura adicional do Azure.](/azure/cost-management-billing/manage/create-subscription)

Na seção portal do Azure, selecione a oferta de SaaS desejada na **seção Marketplace.**

Uma assinatura software como serviço fornece o direito de usar um serviço por um determinado período de tempo por meio de uma assinatura online, em vez de instalação local em computadores individuais. Uma assinatura é um contrato para usar uma ou mais plataformas de nuvem ou serviços, para os quais os encargos se acumulam com base em um valor de licença por usuário ou no consumo de recursos baseados em nuvem. Uma organização pode ter várias assinaturas de SaaS.

As restrições nas assinaturas de SaaS incluem:

- Nenhuma assinatura de aluno.
- Nenhuma Visual Studio Enterprise assinatura.
- Nenhuma assinatura de crédito gratuito.
- Para ofertas pagas, é necessário um meio de pagamento.

## <a name="saas-offers-discovery-in-azure-portal"></a>Descoberta de ofertas de SaaS portal do Azure

Quando você está no portal do Azure, há algumas maneiras de restringir sua pesquisa para se concentrar em ofertas de SaaS.

### <a name="narrowing-your-search"></a>Restringindo sua pesquisa

Na home page, em Serviços **do Azure,** **selecione + Criar um recurso** ou **Marketplace.** Ou use o atalho **G + N em** qualquer lugar da plataforma.

- Restrina os resultados para ofertas de SaaS usando o filtro **Tipo de** Oferta e, em seguida, selecionando **SaaS**.
- Use a pesquisa global na área de navegação superior para encontrar uma oferta de SaaS específica.

Encontre uma [oferta de SaaS](/marketplace/private-offers) privado selecionando a faixa na parte superior da home page do **Marketplace.** Nem todas as ofertas ou planos estão disponíveis em todas as geografias e algumas podem aparecer apenas para determinados locatários.

A exibição filtrada mostra cada oferta de SaaS disponível representada por um título. Selecione um para ver a página de detalhes do produto. O que inclui as seguintes seções:

- Visão geral – detalhes sobre os materiais de serviço, marketing e aprendizado
- Planos + Preços – cada oferta incluirá pelo menos um plano com preços e termos de cobrança diferentes
- Informações de uso + suporte – inclui Publisher ID, ID da oferta e ID do plano
- Classificação e revisões da oferta específica de SaaS

## <a name="available-billing-models-plansskus-for-saas-offers"></a>Modelos de cobrança disponíveis (planos/SKUs) para ofertas de SaaS

Cada oferta de SaaS terá um ou mais planos. Cada oferta tem um modelo de preços associado a ela: taxa fixa ou por usuário. Cada preço de plano é uma taxa recorrente, que pode ser zero dólares (os preços listados são apenas para fins de exemplo e não se destinam a refletir os custos reais). Esse valor é uma taxa fixa ou um preço por usuário. Tipos de planos disponíveis:

- **Planos mensais** – taxa mensal recorrente; valor mensal simples ou por usuário que é pago em uma recorrência mensal. Quando o termo terminar, o plano será renovado automaticamente.
- **Planos anuais** – taxa anual recorrente; valor anual simples ou por usuário que é pago em uma recorrência anual. Quando o termo terminar, o plano será renovado automaticamente.
- **Medidores personalizados** – juntamente com os valores recorrentes, um plano de taxa fixa também pode incluir dimensões personalizadas opcionais para o uso de excesso não incluído na taxa fixa. Cada dimensão representa uma unidade de cobrança. Esse é um custo variável que muda de acordo com o uso de unidades limitadas, como: largura de banda, tíquetes ou email processado. Você será cobrado de acordo com o consumo dessas dimensões mensalmente. Observe que o consumo excessivo é iniciado somente quando você usou todas as unidades medida incluídas na taxa fixa.
- **Avaliação** gratuita – em alguns casos, o plano inclui um período de avaliação de um mês, durante o qual você pode usar o software gratuitamente.  Depois que o período de avaliação for final, você será cobrado de acordo com seu plano. As ofertas de avaliação não são compatíveis com medidores personalizados.

Esses modelos de preços estão disponíveis para planos públicos e privados.

## <a name="saas-purchase-experience"></a>Experiência de compra de SaaS

1. Na página do produto, selecione um plano que atenda às suas necessidades e continue **a configurar + assinar**
2. Como parte do processo de compra, você  será redirecionado para a guia Básico e será necessário:
    1. Defina *qual assinatura* você gostaria de usar para cobrança. A assinatura do Azure que você usa deve ter um método de compra válido definido para ela. Você deve ter o nível certo de permissão ou ter um grupo de recursos nessa assinatura com o nível certo de permissões. Além disso, seu país de cobrança deve ser um país em que a oferta está disponível para compra. As assinaturas do Azure sem uma forma de pagamento válida (por exemplo, uma assinatura MSDN) só podem ser usadas para comprar planos gratuitos
    1. Escolha ou crie um **Grupo de Recursos* ao qual o recurso SaaS pertence.
    1. Digite um *Nome para* a assinatura de SaaS para identificá-la facilmente mais tarde. Depois de comprado, você não pode alterar o nome.
    1. Em **Plano**, você verá o plano selecionado na página detalhada do produto (PDP). Se você ainda não tiver feito uma seleção ativa no PDP, verá o plano padrão. Você pode alterar sua seleção selecionando o link **Alterar plano.** Selecione o termo de cobrança relevante e escolha outro plano. Você poderá alterar o plano após a compra, se o editor dá suporte a ele. No entanto, você não poderá alterar o termo de mensal para anual ou anual para mensal.
    1. Nos casos em que o modelo de preços é *por usuário,* talvez seja necessário especificar o número de *Usuários*. O preço que você vê mudará com base na assinatura, no plano e no termo que você selecionou.
3. Vá para **a guia** Marcas – *As marcas* são pares chave/valor definidos pelo usuário, que podem ser colocados diretamente em um recurso ou em um grupo de recursos. Você pode usar marcas para encontrar facilmente o recurso de SaaS posteriormente. Atualmente, o Azure permite até 50 marcas por recurso e grupo de recursos. As marcas podem ser colocadas em um recurso no momento da criação ou adicionadas a um recurso existente.
4. Continue a **Revisar + Assinar** para ver os detalhes da oferta e do plano.
    1. Revise *Termos de uso* *política* de privacidade,  de alterações e do publicador e também para Azure Marketplace
    1. Talvez você seja solicitado a adicionar seus detalhes de contato
    1. Revisar *noções básicas* e *detalhes de* marcas
5. Após a confirmação, selecione **Assinar**.

## <a name="saas-subscription-and-configuration"></a>Assinatura e configuração de SaaS

Quando você seleciona assinar, uma mensagem informa " Sua assinatura de SaaS está em andamento". Esse processo deve levar alguns minutos, não feche a janela até que ela seja concluída.

Depois que a assinatura for concluída, uma mensagem informa que sua assinatura de SaaS foi concluída e você deve configurar a conta para começar a aproveitar sua compra. Você também receberá um email solicitando que você ative a nova assinatura. Se você não for aquele que vai configurar a conta de SaaS, encaminhe este email para a pessoa relevante.

Para concluir o processo e começar a usar o SaaS, você precisa começar a configurar sua assinatura. Ao selecionar o **botão Configurar conta agora,** ele redireciona você para o site do editor.

Você também pode verificar o status da assinatura selecionando o ícone "sino" no canto superior direito do header.

Se você não concluir o processo de configuração dentro *de 30* dias, essa assinatura de SaaS será *excluída automaticamente.* A cobrança será iniciada depois que sua conta estiver configurada no site do editor.

Mensagens de erro que você pode encontrar durante o processo:

- O nome *do plano selecionado não pode* ser comprado em uma assinatura gratuita
  - Atualize sua conta, https://aka.ms/UpgradeFreeSub consulte para obter mais detalhes.

- A compra falhou porque não foi possível encontrar um cartão de crédito válido nem uma forma de pagamento associada à sua assinatura do Azure.
  - Use uma assinatura diferente do Azure ou adicione\atualize o cartão de crédito atual ou a forma de pagamento para essa assinatura e tentar novamente.

- O *nome do plano selecionado do*  nome da oferta pelo editor da oferta não está disponível para compra de acordo com as regras definidas pelo administrador de TI. 
  - Entre em contato com o administrador de IT.

- O *nome do* plano  selecionado do  plano de oferta selecionado pelo editor da oferta não está disponível para compra devido às configurações do marketplace privado feitas pelo Administrador de TI do locatário.
  - Entre em contato com o administrador de IT

- Falha na compra porque o prazo de cobrança solicitado está vazio ou inválido.
  - Tente comprar um termo de plano/cobrança diferente.

- A compra falhou porque não foi possível verificar sua assinatura no contrato legal.
  - Repetir. Se o erro persistir, tente fazer a compra usando uma assinatura diferente do Azure ou contate o suporte.

- Falha na compra da *oferta OfferId pelo* Publicador *PublisherID* . Atualmente, esta oferta não está disponível para compra.
  - Tente novamente depois. Se depois de uma hora você continuar recebendo essa mensagem de erro, entre em contato com o suporte.  

- Falha na compra da oferta *do plano de plano da oferta* *OfferId* pelo editor *PublisherID* . No momento, este plano não está disponível para compra.
  - Tente novamente depois. Se depois de uma hora você continuar recebendo essa mensagem de erro, entre em contato com o suporte. 

- O *endereço de email* do cliente com *ObjectID* de ID de objeto não tem autorização para executar a ação *DeploymentValidationAction* sobre o resourcegroup de escopo *; DeploymentScope* ou o escopo é inválido.  
  - Você receberá essa mensagem se não tiver as permissões corretas no grupo de recursos/assinatura do Azure.  
    Se o acesso foi concedido recentemente, atualize suas credenciais.  
    Para implantar recursos em um grupo de recursos, você deve ter pelo menos acesso de colaborador. Verifique seu status de acesso em **grupos de recursos** e, em seguida, controle de **acesso**. Isso mostra quem é o ' proprietário ', quem você pode pedir para atribuí-lo como um ' colaborador '.

- A assinatura usada para esta compra não permite compras do Marketplace.  
  - Use uma assinatura diferente ou peça ao administrador para alterar a definição dessa assinatura e tente novamente.

## <a name="next-steps"></a>Próximas etapas

- Se você já comprou uma oferta no Marketplace, vá para [cobrança e faturamento](/marketplace/billing-invoicing)
- Você também pode aprender mais sobre as opções de [planos particulares](/marketplace/private-offers) .
