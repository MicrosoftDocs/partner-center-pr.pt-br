---
title: Gerenciar o licenciamento em ofertas do Marketplace
ms.topic: how-to
ms.date: 04/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como configurar e gerenciar o licenciamento para suas ofertas do marketplace comercial do ISV.
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c128b99b034564bcaa100ca975253f8b1bad7a42
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147948"
---
# <a name="manage-licensing-in-marketplace-offers"></a>Gerenciar o licenciamento em ofertas do Marketplace

**Funções apropriadas:** administrador global | Administrador da conta

Este artigo orienta você pelo processo de configuração de uma oferta no Partner Center, disponibilizando-a no Microsoft AppSource e, em seguida, gerenciando licenças para essa oferta.  

>[!IMPORTANT]
>Os recursos neste artigo estão atualmente em Visualização Pública.

## <a name="before-you-begin"></a>Antes de começar

### <a name="commercial-marketplace-basics"></a>Noções básicas do marketplace comercial

Antes de começar esse processo, você deve se familiarizar com os conceitos básicos do marketplace comercial. Os artigos na tabela abaixo ajudarão você a começar. 

| Tópico  | Artigo  |
|-------|--------|
|Planos do marketplace comercial | [Planos e preços para ofertas comerciais do marketplace](/azure/marketplace/plans-pricing)    |
|Ofertas do marketplace comercial  | [Tipos de listagem](/azure/marketplace/determine-your-listing-type)    |
|Contas do marketplace comercial |  [Criar uma conta do Marketplace comercial no Partner Center](/azure/marketplace/create-account) |

### <a name="determine-your-offer-id"></a>Determinar sua ID da oferta

Nos procedimentos abaixo, você será solicitado a inserir uma ID da Oferta. Agora, leve algum tempo para ter uma ID de oferta adequada, tendo em mente os seguintes pontos:

- Essa ID é visível para os clientes no endereço da Web para a oferta do Marketplace e nos modelos do Azure Resource Manager, se aplicável.
- A ID da oferta combinada com a ID do distribuidor deve ter menos de 40 caracteres.
- Use apenas letras minúsculas e números. A ID da Oferta pode incluir hifens e sublinhados, mas sem espaços. Por exemplo, se a ID do Publicador for `testpublisherid` e você inserir , o endereço Web da oferta será `test-offer-1` `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1` .
- Essa ID não poderá ser alterada depois que você selecionar **Criar**.

### <a name="determine-your-offer-alias"></a>Determinar o alias da oferta

O alias da oferta é o nome usado para a oferta em Partner Center. Você também precisará de um alias de oferta apropriado que siga as diretrizes abaixo:

- Esse nome não é usado no Marketplace e é diferente do nome da oferta e de outros valores mostrados aos clientes.
- Esse nome não pode ser alterado depois que você selecionar Criar.

## <a name="create-your-offer"></a>Criar sua oferta

A primeira etapa no processo de licenciamento é criar sua oferta do marketplace comercial. 

1. Entre no painel [Partner Center](https://partner.microsoft.com/dashboard/).
2. No menu de navegação à esquerda, selecione **Marketplace Comercial/Visão geral.**
3. Na parte superior da página Visão geral, selecione Nova oferta e, em seguida, selecione **Dynamics 365 for Customer Engagement & PowerApps.**
4. Insira a **ID da oferta** **e o alias da** oferta que você criou anteriormente.
5. Selecione **Criar** para gerar a oferta e continuar.
6. Escolha suas opções de licenciamento.

    - Para habilitar o gerenciamento de licenças para sua oferta, selecione **Habilitar o gerenciamento de licenças de aplicativo por meio do Microsoft**. Essa é uma configuração única e você não poderá alterá-la depois que sua oferta for publicada.

    - Você também pode permitir que os clientes executem a funcionalidade base do aplicativo sem uma licença e executem recursos premium depois que comprarem uma licença. Para fazer isso, selecione Permitir que os clientes instalem meu aplicativo **mesmo que as licenças não sejam atribuídas.**

    - Se você não quiser que sua oferta tenha o gerenciamento de licença habilitado, selecione Obter agora **(Gratuito),** Avaliação **gratuita** ou **Entre em contato comigo.**

## <a name="create-your-plan"></a>Criar o plano

Nestas etapas, você definirá o plano ou os planos que deseja habilitar para sua oferta.

1. No menu de navegação à esquerda, selecione **Visão geral do** plano e, em seguida, selecione Criar novo **plano**.
2. Insira uma **ID do Plano** **e o Nome do plano** e, em seguida, selecione **Criar**.
3. Na página **Listagem de planos,** insira a **descrição do plano**.
4. Para salvar a descrição e concluir mais tarde, selecione **Salvar rascunho.**

5. Quando terminar, selecione Revisar **e publicar**. As informações do plano agora serão exibidas no appsource.microsoft.com lista de ofertas (seção planos).

6. Depois de criar todos os planos para essa oferta, você precisará copiar a ID de serviço de cada plano. Selecione **Visão geral do** plano na parte superior da página Listagem de planos. Copie a ID do Serviço de cada plano para um local seguro.

## <a name="add-service-ids-to-your-solution"></a>Adicionar IDs de serviço à sua solução

A próxima etapa é atualizar sua solução adicionando as IDs de serviço para cada plano que você acabou de copiar. Para obter diretrizes sobre isso, consulte [criar um pacote AppSource para sua solução](/powerapps/developer/data-platform/create-package-app-appsource).

## <a name="upload-your-package-and-publish-your-offer"></a>Carregue seu pacote e publique sua oferta

1. No painel de navegação esquerdo, selecione **Marketplace comercial** e, em seguida, selecione **configuração técnica**.
2. Em **modelo de licença base**, selecione **usuário**.
3. Em **pacote do CRM**, insira a URL do local do pacote.
4. Use as outras guias no painel de navegação esquerdo para inserir outras informações necessárias. Quando terminar, selecione **revisar e publicar**.

Depois de publicar a oferta, vamos revisar e verificar suas informações. Se houver algum problema com esse processo, você será notificado. Quando todos os problemas forem resolvidos, você receberá uma notificação de que sua oferta está disponível no AppSource. Nesse ponto, você pode torná-lo dinâmico.

## <a name="make-your-offer-live-in-partner-center"></a>Torne sua oferta ativa no Partner Center

O procedimento a seguir orienta você pelo processo de tornar sua oferta ativa no AppSource. Para saber mais sobre esse processo, consulte [introdução às opções de listagem](/azure/marketplace/determine-your-listing-type).

>[!NOTE]
>Depois de publicar sua oferta, levará 4-6 horas para entrar em tempo real.

1. Entre no painel [Partner Center](https://partner.microsoft.com/dashboard/).
2. No menu de navegação à esquerda, selecione **Marketplace comercial/visão geral**.
3. Na página **visão geral** , localize a oferta que você está procurando. As ofertas prontas para serem publicadas terão um status de versão **prévia**. Selecione a oferta.
4. Na página **Visão geral da** oferta, selecione Ir ao **vivo.**
A oferta estará em tempo de 4 a 6 horas.
5. Para ver sua listagem de ofertas no AppSource, selecione o link **AppSource** na parte inferior da **página Visão** geral da oferta.

    - **Para ofertas** habilitadas para licença: se sua oferta exigir uma verificação de licença, os usuários só poderão inserir um lead clicando em Entrar em Contato **comigo** para que você possa se comunicar com eles.

    - **Para ofertas** habilitadas para licença com **a** opção de instalação gratuita: se sua oferta não exigir uma verificação de licença, os usuários administradores verão um botão Obter Agora, além de Entrar em **contato comigo.** Os usuários que quiserem experimentar sua opção de instalação gratuita devem clicar em Obter **Agora,** o que os levará para instalar a oferta no Power Platform Admin Center. Os usuários ainda poderão **usar Entrar** em contato comigo se tiver dúvidas ou se quiserem atualizar para um plano pago.

## <a name="register-isv-connect-deal-in-deal-registration"></a>Registrar a oferta do ISV Connect no Registro de Oferta

Antes de atribuir licenças a um cliente, cada venda precisa ser registrada em Partner Center. Para fazer isso, consulte [Registrar suas ofertas.](register-deals.md)

## <a name="invite-the-customer"></a>Convidar o cliente

Use o procedimento a seguir para convidar o cliente para participar dessa oferta.  

1. Entre no painel [Partner Center](https://partner.microsoft.com/dashboard/).
2. No menu de navegação à esquerda, selecione **Marketplace Comercial/Visão geral.**
3. No menu de navegação esquerdo, selecione **Indicações** e, em seguida, selecione **Registro de Negociação.**
4. Filtre **por Ofertas** enviadas, selecione **a guia** Em Andamento e, em seguida, selecione a oferta que você deseja.
5. Na página de visão geral dessa oferta, selecione **Gerenciar licenças.**
6. Na janela **Gerenciar licenças,** selecione o cliente na **lista suspenso Detalhes do** cliente. Se a relação de cliente ainda não existir, selecione **+Convidar um novo cliente para consentir**.
7. Copie o link exibido.
8. Envie este link por email para o administrador de cobrança do cliente ou administrador global e use este link para acessar o admin.microsoft.com e aceite e autorize a relação que você está estabelecendo.

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