---
title: Gerenciar o licenciamento em ofertas do Marketplace
ms.topic: how-to
ms.date: 04/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como configurar e gerenciar o licenciamento para suas ofertas de Marketplace comercial de ISV.
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f049ffda4c3d9476c09257fc814e5acac393cb54
ms.sourcegitcommit: 6c20c3cc4a226cada70c56df295966696affcec8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/30/2021
ms.locfileid: "108328008"
---
# <a name="manage-licensing-in-marketplace-offers"></a>Gerenciar o licenciamento em ofertas do Marketplace

**Funções apropriadas**

- Administrador global
- Administrador de conta

Este artigo orienta você pelo processo de configuração de uma oferta no Partner Center, disponibilizando-o em Microsoft AppSource e, em seguida, gerenciando licenças para essa oferta.  

>[!IMPORTANT]
>Os recursos neste artigo estão atualmente em visualização pública.

## <a name="before-you-begin"></a>Antes de começar

### <a name="commercial-marketplace-basics"></a>Noções básicas do Marketplace comercial

Antes de começar esse processo, você deve se familiarizar com os conceitos básicos do Marketplace comercial. Os artigos na tabela a seguir ajudarão você a começar. 

| Tópico  | Artigo  |
|-------|--------|
|Planos do Marketplace comercial | [Planos e preços para ofertas de Marketplace comercial](/azure/marketplace/plans-pricing)    |
|Ofertas do Marketplace comercial  | [Tipos de listagem](/azure/marketplace/determine-your-listing-type)    |
|Contas do Marketplace comercial |  [Criar uma conta do Marketplace comercial no Partner Center](/azure/marketplace/create-account) |

### <a name="determine-your-offer-id"></a>Determinar sua ID de oferta

Nos procedimentos abaixo, você será solicitado a inserir uma ID de oferta. Reserve algum tempo agora para criar uma ID de oferta adequada, tendo em mente os seguintes pontos:

- Essa ID é visível para os clientes no endereço da Web para a oferta do Marketplace e nos modelos do Azure Resource Manager, se aplicável.
- A ID da oferta combinada com a ID do Publicador deve ter menos de 40 caracteres de comprimento.
- Use apenas letras minúsculas e números. A ID da oferta pode incluir hifens e sublinhados, mas sem espaços. Por exemplo, se sua ID de editor for `testpublisherid` e você inserir `test-offer-1` , o endereço Web da oferta será `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1` .
- Essa ID não pode ser alterada depois que você seleciona **criar**.

### <a name="determine-your-offer-alias"></a>Determinar seu alias de oferta

O alias da oferta é o nome usado para a oferta no Partner Center. Você também precisará de um alias de oferta apropriado que siga as diretrizes abaixo:

- Esse nome não é usado no Marketplace e é diferente do nome da oferta e de outros valores mostrados aos clientes.
- Esse nome não pode ser alterado depois que você seleciona criar.

## <a name="create-your-offer"></a>Criar sua oferta

A primeira etapa do processo de licenciamento é criar sua oferta do Marketplace comercial. 

1. Entre no painel [Partner Center](https://partner.microsoft.com/dashboard/).
2. No menu de navegação à esquerda, selecione **Marketplace comercial/visão geral**.
3. Na parte superior da página Visão geral, selecione **nova oferta** e, em seguida, selecione **Dynamics 365 para compromisso com o cliente & PowerApps**.
4. Insira a **ID da oferta** e o **alias da oferta** que você criou anteriormente.
5. Selecione **Criar** para gerar a oferta e continuar.
6. Escolha suas opções de licenciamento.

    - Para habilitar o gerenciamento de licenças para sua oferta, selecione **habilitar o gerenciamento de licenças de aplicativos por meio da Microsoft**. Essa é uma configuração única, e você não poderá alterá-la depois que sua oferta for publicada.

    - Você também pode permitir que os clientes executem a funcionalidade base do aplicativo sem uma licença e executem recursos premium depois de adquirirem uma licença. Para fazer isso, selecione **permitir que os clientes instalem meu aplicativo mesmo se as licenças não forem atribuídas**.

    - Se você não quiser que sua oferta tenha o gerenciamento de licenças habilitado, selecione **obtê-lo agora (gratuito)**, **avaliação gratuita** ou **entre em contato comigo**.

## <a name="create-your-plan"></a>Criar o plano

Nestas etapas, você definirá o plano ou planos que deseja habilitar para sua oferta.

1. No menu de navegação à esquerda, selecione **visão geral do plano** e, em seguida, selecione **criar novo plano**.
2. Insira uma **ID do plano** e o **nome do plano** e, em seguida, selecione **criar**.
3. Na página de **listagem do plano** , insira a descrição do **plano**.
4. Para salvar a descrição e concluir mais tarde, selecione **salvar rascunho**.

5. Quando tiver terminado, selecione **revisar e publicar**. As informações do plano agora serão exibidas em appsource.microsoft.com Em listagem de oferta (seção planos).

6. Depois de criar todos os planos para esta oferta, você precisará copiar a ID de serviço de cada plano. Selecione **visão geral do plano** na parte superior da página de listagem do plano. Copie a ID de serviço de cada plano para um local seguro.

## <a name="add-service-ids-to-your-solution"></a>Adicionar IDs de serviço à sua solução

A próxima etapa é atualizar sua solução adicionando as IDs de serviço para cada plano que você acabou de copiar. Para obter diretrizes sobre isso, consulte [criar um pacote AppSource para sua solução](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource).

## <a name="upload-your-package-and-publish-your-offer"></a>Carregue seu pacote e publique sua oferta

1. No painel de navegação esquerdo, selecione **Marketplace comercial** e, em seguida, selecione **configuração técnica**.
2. Em **modelo de licença base**, selecione **usuário**.
3. Em **pacote do CRM**, insira a URL do local do pacote.
4. Use as outras guias no painel de navegação esquerdo para inserir outras informações necessárias. Quando terminar, selecione **revisar e publicar**.

Depois de publicar a oferta, vamos revisar e verificar suas informações. Se houver algum problema com esse processo, você será notificado. Quando todos os problemas forem resolvidos, você receberá uma notificação de que sua oferta está disponível no AppSource. Nesse ponto, você pode torná-lo dinâmico.

## <a name="make-your-offer-live-in-partner-center"></a>Torne sua oferta ativa no Partner Center

O procedimento a seguir orienta você pelo processo de tornar sua oferta ativa no AppSource. Para saber mais sobre esse processo, consulte [introdução às opções de listagem](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type).

>[!NOTE]
>Depois de publicar sua oferta, levará 4-6 horas para entrar em tempo real.

1. Entre no painel [Partner Center](https://partner.microsoft.com/dashboard/).
2. No menu de navegação à esquerda, selecione **Marketplace comercial/visão geral**.
3. Na página **visão geral** , localize a oferta que você está procurando. As ofertas prontas para serem publicadas terão um status de versão **prévia**. Selecione a oferta.
4. Na página **visão geral da oferta** , selecione **entrar em tempo real**.
A oferta será ativa em 4-6 horas.
5. Para ver sua listagem de ofertas em AppSource, selecione o link **AppSource** na parte inferior da página **visão geral da oferta** .

    - **Para ofertas habilitadas para licença**: se sua oferta exigir uma verificação de licença, os usuários só poderão inserir um cliente potencial clicando **em entrar em contato comigo**, para que você possa se comunicar com eles.

    - **Para ofertas com licença habilitada com a opção de instalação gratuita**: se sua oferta não exigir uma verificação de licença, os usuários administradores verão um botão **obter agora** , além de **entrar em contato comigo**. Os usuários que desejam experimentar sua opção de instalação gratuita devem clicar em **obter agora**, o que os levará para instalar a oferta no centro de administração do Power Platform. Os usuários ainda poderão usar **entrar em contato comigo** se tiverem alguma dúvida ou se quiserem atualizar para um plano pago.

## <a name="register-isv-connect-deal-in-deal-registration"></a>Registrar o contrato do ISV Connect no registro de negociações

Antes de poder atribuir licenças a um cliente, cada venda precisa ser registrada no Partner Center. Para fazer isso, consulte [registrar suas negociações](register-deals.md).

## <a name="invite-the-customer"></a>Convidar o cliente

Use o procedimento a seguir para convidar o cliente a participar desse negócio.  

1. Entre no painel [Partner Center](https://partner.microsoft.com/dashboard/).
2. No menu de navegação à esquerda, selecione **Marketplace comercial/visão geral**.
3. No menu de navegação à esquerda, selecione **referências** e, em seguida, selecione **registro de negociações**.
4. Filtrar para negociações **enviadas** , selecione a guia **em andamento** e, em seguida, selecione o negócio desejado.
5. Na página Visão geral desse negócio, selecione **gerenciar licenças**.
6. Na janela **gerenciar licenças** , selecione o cliente na lista suspensa **detalhes do cliente** . Se a relação do cliente ainda não existir, selecione **+ convidar um novo cliente para consentir**.
7. Copie o link que é exibido.
8. Envie este link por email para o administrador de cobrança ou administrador global do seu cliente e faça com que eles usem esse link para acessar o admin.microsoft.com e aceitar e autorizar a relação que você está estabelecendo.

    >[!NOTE]
    >A relação não será estabelecida até que o cliente execute esta etapa.

## <a name="activate-manage-and-remove-your-licenses"></a>Ativar, gerenciar e remover suas licenças

Depois que o cliente tiver autorizado a relação com você, você poderá começar a adicionar planos de sua oferta e atribuir licenças a cada plano.

1. Na janela Gerenciar licenças para esse negócio, selecione **+ Adicionar um plano**.
2. Preencha os **planos para esta solução** e **número de campos de licenças** e, em seguida, selecione **Atualizar licenças**. As licenças estarão disponíveis em admin.microsoft.com para que os clientes gerenciem e atribuam a funcionários.

    - Para alterar o número de licenças de um plano existente, insira o novo número no campo **número de licenças** e, em seguida, selecione **Atualizar licenças**.

    - Para desativar ou remover licenças de um negócio, selecione o ícone de lixeira no campo **ações** e, em seguida, selecione **Atualizar licenças**.

## <a name="next-steps"></a>Próximas etapas

[Recursos de licenciamento](support-resources-licensing.md)
