---
title: O conector de venda co-venda para o Salesforce CRM Partner Center
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Sincronizar suas indicações no Partner Center com o Salesforce CRM. Em seguida, os vendedores podem fazer a venda em cooperação com a Microsoft de dentro de seus sistemas crm.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 06/28/2021
ms.openlocfilehash: 726e9071347e1590885b4bf82676f7767311f945
ms.sourcegitcommit: c4601069340445135b551fa96bee6d9923d8aa97
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2021
ms.locfileid: "113173675"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Conector de venda conjunta para o Salesforce CRM – visão geral

**Funções apropriadas:** indicações de administrador | Administrador do sistema ou personalizador de sistema no CRM

Partner Center conector de venda co-venda permite que os vendedores vendam com a Microsoft de dentro de seus sistemas CRM. Eles não precisam ser treinados para usar o Partner Center gerenciar acordos de venda em cooperação. Usando os conectores de venda de co-venda, você pode criar uma nova indicação de venda co-venda para envolver um vendedor da Microsoft, receber indicações do vendedor da Microsoft, aceitar/recusar indicações, modificar dados de negociação, como valor da oferta e data de fechamento.  Você também pode receber atualizações dos vendedores da Microsoft nesses acordos de venda em cooperação. Você pode fazer todas as suas indicações funcionarem enquanto trabalham dentro do CRM de sua escolha em vez de em Partner Center.

A solução é baseada na Solução microsoft Power Automate e usa apIs Partner Center aplicativo.

## <a name="before-you-install---pre-requisites"></a>Antes de instalar – pré-requisitos

|**Tópicos**|**Detalhes**|**Links**|
|--------------|--------------------|------|
|Microsoft Partner Network ID |Você precisa de uma ID de MPN válida|Para ingressar no [MPN](https://partner.microsoft.com/)|
|Pronto para venda conjunta|Sua solução de IP/Serviços deve estar pronta para venda em cooperação.|[Vender com a Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)|
|Conta do Partner Center|A ID do MPN associada ao locatário Partner Center deve ser igual à ID do MPN associada à sua solução de venda co-venda. Verifique se você pode ver suas indicações de venda em Partner Center portal antes de implantar os conectores.|[Gerenciar sua conta](create-user-accounts-and-set-permissions.md)|
|Funções de usuário da Central de parceiros|O funcionário que instalará e usará os conectores deve ser um administrador de indicações|[Atribuir permissões e funções de usuários](create-user-accounts-and-set-permissions.md)|
|Salesforce CRM|A função de usuário crm é Administrador do sistema ou Personalizador do sistema|[Atribuir funções no Salesforce CRM](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|Power Automate Flow conta|Crie um novo ambiente de produção com um banco de dados para teste, preparação e produção. Se você tiver um ambiente de produção existente com um banco de dados, ele poderá ser reutilizado. O usuário que instalará a solução do conector deve ter uma licença Power Automate e acesso a esse ambiente. Você pode monitorar o progresso e obter mais informações em [Power Automate](https://flow.microsoft.com/) se a instalação falhar. Selecione **Ver histórico** em **Soluções.**|[Criar ou gerenciar o ambiente](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a>Instalação do pacote salesforce para campos personalizados da Microsoft

Para sincronizar as indicações entre o Partner Center e o Salesforce CRM, Power Automate solução precisa identificar claramente os campos de indicação específicos da Microsoft. Essa demarcação fornece às equipes de vendedores parceiros a capacidade de decidir quais indicações elas querem compartilhar com a Microsoft para venda em parceria.

1. No Salesforce, ative **as Notas** e adicione-as à lista de oportunidades relacionadas. [Referência](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

1. Ative **as equipes de** oportunidade seguindo as etapas:
    - Em Instalação, use a **caixa Localização Rápida** para localizar a Equipe de Oportunidade Configurações.
    - Defina as configurações conforme necessário. [Referência](https://help.salesforce.com/articleView?id=sf.opp_team_manage.htm&type=5)

1. No Salesforce, instale objetos e campos personalizados usando o [instalador de pacote](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV). Use esse instalador para instalar o pacote em qualquer empresa.

    >[!NOTE]
    >Se você estiver instalando em uma área sandbox, deverá substituir a parte inicial da URL por `http://test.salesforce.com` .

1. No Salesforce, adicione Soluções da Microsoft à **lista relacionada** à oportunidade. Depois de adicionado, selecione o ícone **de chave inglesa** e atualize as propriedades

## <a name="best-practice-test-before-you-go-live"></a>Melhor prática: testar antes de entrar no ar

Antes de instalar, configurar e personalizar a solução Power Automate no ambiente de produção, teste a solução em uma instância de CRM de preparação.

- Instale a solução Power Automate Microsoft em um ambiente de preparação/instância crm.

- Faça uma cópia da solução e execute sua configuração e Power Automate personalizações de fluxo no ambiente de preparação.

- Teste a solução em uma instância de preparação/CRM.

- Em caso de sucesso, importe como uma solução gerenciada para a instância de produção.

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>Instalar Partner Center sincronização de indicações do Salesforce CRM

1. Vá para [Power Automate](https://flow.microsoft.com) e selecione **Ambientes** no canto superior direito. Isso mostrará as instâncias de CRM disponíveis.

1. Selecione a instância de CRM apropriada na listada no canto superior direito.

1. Selecione **Soluções** na barra de navegação à esquerda.

1. Selecione o link **Abrir AppSource** no menu superior.

   :::image type="content" source="images/cosellconnectors/open-appsource.png" alt-text="Abra AppSource.":::

1. **Pesquise Partner Center conectores de indicações para Salesforce** na tela pop-up.  

   :::image type="content" source="images/salesforce/salesforce-get-it-now.png" alt-text="Captura de tela de Obter Agora.":::

1. Selecione o **botão Obter agora** e, em seguida, selecione **Continuar.**

1. Na próxima página, selecione o ambiente salesforce CRM para instalar o aplicativo. Concorde com os termos e condições.

1. Em seguida, você será direcionado para a **página Gerenciar suas soluções.**  Navegue até "Partner Center indicações" usando os botões de seta na parte inferior da página. **A instalação agendada** deve aparecer ao lado Partner Center de indicações. A instalação levará de 10 a 15 minutos.

1. Depois que a instalação for concluída, navegue de [volta para Power Automate](https://flow.microsoft.com) e selecione **Soluções** na área de navegação esquerda. Observe que **Partner Center sincronização de indicações para Salesforce** agora está disponível na lista Soluções.

1. Selecione **Partner Center sincronização de indicações para o Salesforce.** As seguintes Power Automate fluxos e entidades estão disponíveis:

   :::image type="content" source="images/cosellconnectors/partner-center-referrals-synchronization.png" alt-text="Fluxos do Salesforce.":::

## <a name="configure-the-solution"></a>Configurar a solução

1. Depois de instalar a solução em sua instância do CRM, navegue de volta para [Power Automate](https://flow.microsoft.com/).

1. Na lista **de ambientes** no canto superior direito, selecione a instância crm em que você instalou a solução Power Automate aplicativo.

1. Você precisará criar conexões que associem as três contas de usuário:

   - Partner Center usuário com credenciais de administrador de indicações
   - Eventos do Partner Center
   - Administrador de CRM com Power Automate fluxos na solução

   1. Selecione **Conexões** na barra de navegação esquerda e selecione a **solução Partner Center Indicações** na lista.

   1. Crie uma conexão selecionando **Criar uma conexão**.

        :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Captura de tela que mostra Criar uma conexão.":::

   1. **Pesquise Partner Center Indicações (versão prévia)** na barra de pesquisa no canto superior direito.

   1. Crie uma conexão para seu Partner Center usuário com a função de credenciais do administrador de indicações.

   1. Em seguida, crie uma conexão Partner Center eventos para seu Partner Center com as credenciais de administrador de indicações.

   1. Crie uma conexão para o Salesforce para o usuário administrador do CRM.
  
   1. Crie uma conexão para o Microsoft Dataverse para o usuário administrador do CRM.

   1. Depois de adicionar todas as Conexões, você deverá ver as seguintes conexões em seu ambiente:

        :::image type="content" source="images/cosellconnectors/salesforce-connections.png" alt-text="Captura de tela que mostra como observar as conexões.":::

### <a name="edit-the-connections"></a>Editar as conexões

1. Retorne à página **Soluções** e selecione **Solução Padrão.** Selecione **Referência de Conexão (versão prévia)** clicando em **Todos.**

   :::image type="content" source="images/connection-reference-video.gif" alt-text="Captura de tela que mostra a edição das conexões.":::

1. Edite cada uma das Conexões individualmente selecionando o ícone de reellipse. Adicione as conexões relevantes.

   :::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Captura de tela que mostra como editar conectores.":::

1. A ligar os fluxos na sequência a seguir:
   - Partner Center de webhook (visualização do insider)
   - [Personalizar] Criar ou obter detalhes do Salesforce
   - Criar uma venda Referral-Salesforce para Partner Center (Visualização do Insider)
   - Partner Center atualizações de indicação de venda co-venda da Microsoft para o Salesforce (Visualização do Insider)  
   - Partner Center ao Salesforce (Visualização do Insider)
   - Salesforce para Partner Center (Insider Preview)
   - Salesforce Opportunity to Partner Center (Insider Preview)
   - Salesforce Microsoft Solutions to Partner Center (Insider Preview)

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Usar APIs de webhook para se registrar para eventos de alteração de recursos

Você pode usar as APIs Partner Center webhook para se registrar para eventos de alteração de recurso. Esses eventos de alteração são enviados para sua URL como postagens HTTP.

1. Selecione **Partner Center para Salesforce CRM (Insider Preview)**.

1. Selecione o **ícone Editar** e selecione Quando **uma solicitação HTTP é recebida.**

1. Selecione o **ícone Copiar** para copiar a URL HTTP **POST fornecida.**

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Captura de tela que mostra como copiar a URL.":::

1. Selecione o Partner Center do Webhook (Visualização do **Insider)** Power Automate fluxo e, em seguida, selecione **Executar**.

1. Verifique se a **janela Executar fluxo** é aberta no painel direito e selecione **Continuar.**

1. Insira os seguintes detalhes:

   - **Ponto de extremidade de gatilho HTTP:** essa URL foi copiada de uma etapa anterior.
   - **Eventos a registrar:** Select all eventos disponíveis **(** criados por indicação, atualizados por indicação, relacionados **criados** por indicações e **relacionados-referral-updated).**
   - **Substituir pontos de extremidade de gatilho existentes, se presente?**: Sim. Somente uma URL pode ser registrada para um determinado evento de webhook.

1. Selecione **Executar fluxo** e, em seguida, selecione **Feito.**

O webhook agora pode escutar, criar e atualizar eventos.

## <a name="customize-synchronization-steps"></a>Personalizar etapas de sincronização

Os sistemas crm são altamente personalizados e você pode personalizar a solução Power Automate com base em sua configuração de CRM. Quando as indicações de venda co-venda são sincronizadas entre o Partner Center e o sistema CRM, os campos sincronizados no computador Partner Center são listados no Guia de mapeamento de campo [personalizado](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S).

Siga o guia de mapeamento de campo e, se necessário, faça as alterações apropriadas **em [Personalizar]** Criar ou obter detalhes do Salesforce ou das variáveis de ambiente. Não atualize nenhum outro fluxo na solução de Power Automate porque ela pode afetar atualizações futuras da solução.

As seguintes personalizações estão disponíveis:

- **Exibir marca** de seleção no nome da oportunidade: por padrão, uma marca de seleção será exibida ao lado do nome da oportunidade para indicar que a sincronização entre o Partner Center e o Salesforce CRM está ocorrendo com êxito. Da mesma forma, uma marca cruzada será exibida se a sincronização falhar. Para evitar adicionar uma marcação de verificação ou cruz no nome da oportunidade, de definir o valor atual da marca de seleção Exibição na variável de ambiente de **nome** de oportunidade como Não.

- **Nome do estágio:**

  - **Nome do estágio ativo:** esse é o estágio no pipeline de vendas de uma oportunidade no Salesforce.  Ele representa um estágio ativo e é equivalente a uma indicação no estado aceito em Partner Center. Esse pode ser o próximo estágio no pipeline de vendas após o estágio em espera. Mover o estágio de vendas do Opportunity para fora do estágio em espera para o estágio ativo aceitará a indicação no Partner Center e as alterações começarão a ser sincronizadas.

  - **Nome do estágio em espera:** nome do estágio no pipeline de vendas de uma oportunidade no Salesforce. Ele representa um estágio em espera. Novas indicações de venda compartilhadas da Microsoft que ainda não foram aceitas serão definidas para esse estágio no Salesforce. Todas as alterações feitas em uma oportunidade enquanto ela estiver em espera não serão sincronizadas com Partner Center. Mover o estágio de vendas do Opportunity para fora desse estágio em espera aceitará a indicação no Partner Center e as alterações começarão a sincronizar.

- **Código do país** da conta do cliente: é obrigatório fornecer um código de país de duas letras (ISO 3166) ao criar uma nova indicação. Por padrão, o código do país será sincronizado de e para o campo **BillingCountry da** conta no Salesforce. Se você tiver um campo diferente no Salesforce para o código do país a ser sincronizado:

  - Para um campo de código de país sem procura na conta que contém um código de duas letras:

    - Atualize **o nome do campo Código** do País da Conta do Cliente na variável de ambiente Salesforce com o nome de campo do CRM. Certifique-se de fornecer o nome do campo, não seu nome de exibição.

    - Edite **[Personalizar] Criar** ou obter detalhes do Salesforce e vá para Criar ou obter **conta** de cliente na ação **crm** para atribuir um valor de País ao campo correto no CRM. Além disso, remova **a atribuição** de valor Country do **BillingCountry.**

  - Para um campo de código de país baseado em busca na conta:

    - Adicione um novo campo personalizado na conta e preencha-o automaticamente com um código de país de duas letras (ISO 3166) com base no valor selecionado no campo baseado em busca e vice-versa.

    - Siga as etapas anteriores para o campo de código de país não lookup para sincronizar um novo campo personalizado do CRM de e para Partner Center.

- **Valor da** negociação: por padrão, o valor da Partner Center será sincronizado de e para **Valor** no CRM. Se você tiver um campo diferente no CRM para o valor de negociação a ser sincronizado de:

  - Atualize **o nome do campo** Valor da oferta na variável de ambiente Salesforce com o nome do campo do CRM. Certifique-se de fornecer o nome do campo, não seu nome de exibição.

  - Editar **[Personalizar]** Criar ou obter detalhes  do Salesforce e ir para Criar ou  atualizar **oportunidade** no CRM e atualizar as ações Criar uma nova oportunidade e Atualizar oportunidade existentes para atribuir **DealValue** ao campo correto no Salesforce.

- **Código de moeda de valor de negociação:** nome do campo de código de moeda de valor de negociação no Salesforce. Esse nome de API de campo será usado para obter o código de moeda do valor de oferta da Oportunidade ao criar ou atualizar a indicação no Microsoft Partner Center. Se o campo de código de moeda de valor de negociação for diferente do campo **padrão CurrencyIsoCode,** atualize o valor atual dessa variável de ambiente.

  - Atualize **o nome do campo Moeda** do valor da negociação na variável de ambiente Salesforce com o nome do campo do CRM. Certifique-se de fornecer o nome do campo, não seu nome de exibição.

  - Edite **[Personalizar]** Criar ou obter detalhes  do Salesforce e acesse Criar ou  atualizar **oportunidade** no CRM e atualize as ações Criar uma nova oportunidade e Atualizar oportunidade existente para atribuir **DealValueCurrency** ao campo correto no Salesforce.

- **Oportunidade de venda de** sincronização: se definido como **sim,** somente oportunidades de venda e compartilhamento de pipeline serão sincronizadas do Partner Center ao Salesforce. Se definido como **nenhum**, as oportunidades de venda, venda em conjunto e compartilhamento de pipeline serão sincronizadas do Partner Center ao Salesforce. Essa variável não tem nenhum impacto sobre as oportunidades sincronizadas do Salesforce para Partner Center.

## <a name="update-environment-variable"></a>Atualizar variável de ambiente

Para atualizar um valor de variável de ambiente:

1. Vá para a **página Soluções** e selecione **Solução Padrão.** Selecione **Variável de** Ambiente selecionando **Todos.**

1. Selecione a variável de ambiente para o valor que precisa ser atualizado e selecione **Editar** usando o ícone de reellipse.

1. Atualize **o Valor** Atual (não atualize **o Valor Padrão**) usando a opção Novo **valor** e fornecendo o valor . O valor deve corresponder ao tipo de dados da variável. Por exemplo, o tipo de dados Sim ou Não aceitará o valor Sim ou Não.

   :::image type="content" source="images/cosellconnectors/environment-variables-video.gif" alt-text="Captura de tela que mostra Atualizar variáveis ambientais.":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>Sincronização de indicação de venda co-direcional de ponta a ponta

Depois de instalar, configurar e personalizar a solução Power Automate, você poderá testar a sincronização de indicações de venda em cooperação entre o Salesforce CRM e Partner Center.

### <a name="pre-requisites"></a>Pré-requisitos

Para sincronizar as indicações entre Partner Center e Salesforce CRM, a solução Power Automate precisa demarcar claramente os campos de indicação específicos da Microsoft. Essa identificação fornece às equipes de vendedores a capacidade de decidir quais indicações eles querem compartilhar com a Microsoft para venda em cooperação.

Um conjunto de campos personalizados está disponível como parte da Partner Center  sincronização de indicações para a entidade de oportunidade da solução Salesforce CRM. Um usuário administrador do CRM precisará criar uma seção crm separada com os **campos personalizados oportunidade.**

Os seguintes campos personalizados devem fazer parte da seção CRM:

- **Sincronizar com Partner Center**: se a oportunidade deve ser sincronizada com Partner Center. Por padrão, o valor desse campo é Não e precisa ser definido explicitamente como Sim pelo vendedor para compartilhar uma oportunidade com a Microsoft. Novas indicações compartilhadas de Partner Center crm terão esse valor de campo definido como Sim.

- **Identificador de Indicação:** um campo de identificador somente leitura para a indicação Partner Center Microsoft.

- **Link de** indicação: um link somente leitura para a indicação no Microsoft Partner Center.

- **Como a Microsoft pode ajudar:** ajuda necessária da Microsoft para a indicação. Para criar uma indicação de venda em cooperação, selecione a ajuda apropriada necessária da Microsoft. Um contato do cliente deve estar associado à oportunidade de criar uma indicação de venda em cooperação. Para criar uma indicação de não venda co-venda, não selecione este campo. Uma indicação de não venda co-venda pode ser convertida em uma indicação de venda em co-venda a qualquer momento selecionando a opção apropriada de ajuda necessária.

- **Visibilidade Partner Center referência** da Microsoft: selecione visibilidade para a Partner Center referência. Ao tornar-o visível para vendedores da Microsoft, uma indicação de não venda co-venda pode ser convertida em venda em co-venda. Quando a ajuda da Microsoft é necessária, a indicação fica visível para os vendedores da Microsoft por padrão. Depois que esse campo é marcado como visível, ele não pode ser revertido.

- **Microsoft CRM Identificador**: quando uma indicação de venda co-venda é criada e aceita pela Microsoft, esse campo será preenchido com o identificador crm da Microsoft.

- **Soluções Partner Center Microsoft:** um objeto personalizado para associar soluções prontas para venda em comum ou soluções da Microsoft com a oportunidade. Uma ou mais soluções podem ser adicionadas ou removidas da oportunidade. É obrigatório adicionar pelo menos uma solução pronta para venda em cooperação ou da Microsoft à oportunidade antes de compartilhá-la com a Microsoft. Para associar esse objeto à oportunidade, atualize o **formulário Oportunidade** no CRM.

- **Auditoria:** uma trilha de auditoria somente leitura para sincronização com Partner Center indicações

### <a name="scenarios"></a>Cenários

1. Sincronização de indicação quando a indicação é criada ou atualizada no CRM e sincronizada Partner Center:

   1. Entre em seu ambiente do Salesforce CRM com o usuário que tenha visibilidade na **seção Oportunidade** do CRM.

   1. Verifique se a seção Microsoft **Partner Center** está presente quando você cria uma **nova oportunidade** no ambiente do Salesforce CRM.

   1. As oportunidades sincronizadas com êxito com o Partner Center serão identificadas com ✔ ícone no Salesforce CRM.
      :::image type="content" source="images/salesforce/salesforce-environment.png" alt-text="Captura de tela do ambiente do Salesforce.":::

   1. Para sincronizar essa oportunidade com o Microsoft Partner Center, certifique-se de definir os seguintes campos na exibição de cartão:

      - **Como a Microsoft pode ajudar?**: para criar uma indicação de venda em cooperação, selecione uma opção de ajuda apropriada.

        :::image type="content" source="images/salesforce/salesforce-help-option.png" alt-text="Captura de tela que mostra como obter os campos apropriados na exibição de cartão.":::

      - **Sincronizar com Partner Center**: Sim
      - **Contato do** cliente: para criar uma indicação de venda em cooperação, adicione um contato do cliente à oportunidade.
      - **Soluções da Microsoft:** para compartilhar uma indicação com a Microsoft, adicione uma solução válida pronta para venda em comum ou da Microsoft à oportunidade.

   1. Depois de definir a opção **Sincronizar com Partner Center** oportunidade como **Sim,** aguarde 10 minutos, entre em sua Partner Center. Suas indicações serão sincronizadas com o Salesforce CRM e o Link de Indicação será preenchido. Se houver uma falha, o campo Auditoria será preenchido com informações de erro.

   1. Da mesma forma, quando **a** opção Sincronizar com Partner Center estiver definida como **Sim,** se você atualizar a oportunidade no Salesforce CRM, as alterações serão sincronizadas com sua Partner Center cliente.

2. Sincronização de indicação quando a indicação é criada ou atualizada no Microsoft Partner Center sincronizada no ambiente salesforce CRM:

    1. Entre em seu painel Partner Center [.](https://partner.microsoft.com/dashboard/home)

    1. Selecione **Indicações** no menu à esquerda.

    1. Crie uma nova indicação de venda de Partner Center clicando na opção "Nova oferta".

    1. Entre em seu ambiente do Salesforce CRM.

    1. Navegue até **Abrir Oportunidades**. A indicação criada no Microsoft Partner Center agora está sincronizada no Salesforce CRM.

    1. Quando você seleciona uma indicação sincronizada, os detalhes da exibição de cartão são preenchidos.

       :::image type="content" source="images/salesforce/salesforce-casino.png" alt-text="Captura de tela da página de oportunidade do Salesforce.":::

>[!NOTE]
>**Precisa de ajuda com a implantação?**
>Para assistência com a implantação do conector de indicação de venda em cooperação, você pode envolver um Consultor Técnico de Parceiro. Eles podem fornecer assistência de implantação e práticas recomendadas para uma implementação bem-sucedida.
>
>Para obter mais informações, consulte Como enviar uma solicitação técnica de [pré-vendas e serviços de implantação](technical-benefits.md)

## <a name="next-steps"></a>Próximas etapas

- [Gerenciar clientes potenciais](manage-leads.md)

- [Gerenciar oportunidades de venda conjunta](manage-co-sell-opportunities.md)

- [Webhooks do Partner Center](/partner-center/develop/partner-center-webhooks)
