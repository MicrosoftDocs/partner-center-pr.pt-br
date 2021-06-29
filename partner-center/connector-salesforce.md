---
title: O conector de televenda para o centro de parceiros do Salesforce CRM
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Sincronize suas referências no Partner Center com seu Salesforce CRM. Os vendedores podem, então, vender com a Microsoft de dentro de seus sistemas de CRM.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 06/28/2021
ms.openlocfilehash: f8cb4cd2488e55ab64cf7b7cdce4a3e950b266de
ms.sourcegitcommit: 6a6e8f9af0a58b32770c7fce9f567dd4795b9797
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2021
ms.locfileid: "113029033"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Conector de venda conjunta para o Salesforce CRM – visão geral

**Funções apropriadas**: administrador de referências | Administrador do sistema ou personalizador do sistema no CRM

O conector de televenda do Partner Center permite que seus vendedores covendam-se com a Microsoft de dentro de seus sistemas de CRM. Eles não precisarão ser treinados para usar o Partner Center para gerenciar acordos de venda. Usando os conectores de venda conjunta, você pode criar uma nova referência de covenda para envolver um vendedor da Microsoft, receber referências do vendedor da Microsoft, aceitar/recusar referências, modificar dados de negociações, como valor de negócio e data de fechamento.  Você também pode receber todas as atualizações dos vendedores da Microsoft sobre esses acordos de venda conjunta. Você pode fazer todas as suas referências funcionarem enquanto trabalha no CRM de sua escolha em vez de no Partner Center.

A solução baseia-se na solução de automatização de energia da Microsoft e usa as APIs do Partner Center.

## <a name="before-you-install---pre-requisites"></a>Antes de instalar-pré-requisitos

|**Tópicos**|**Detalhes**|**Links**|
|--------------|--------------------|------|
|ID de Microsoft Partner Network |Você precisa de uma ID de MPN válida|Para ingressar no [MPN](https://partner.microsoft.com/)|
|Pronto para venda conjunta|Sua solução de IP/serviços deve estar pronta para venda.|[Venda com a Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)|
|Conta do Partner Center|A ID de MPN associada ao locatário do Partner Center deve ser a mesma que a ID do MPN associada à sua solução de venda conjunta. Verifique se você pode ver suas referências de venda conjunta no portal do Partner Center antes de implantar os conectores.|[Gerenciar sua conta](create-user-accounts-and-set-permissions.md)|
|Funções de usuário da Central de parceiros|O funcionário que irá instalar e usar os conectores deve ser um administrador de referências|[Atribuir permissões e funções de usuários](create-user-accounts-and-set-permissions.md)|
|CRM do Salesforce|A função de usuário CRM é administrador do sistema ou personalizador do sistema|[Atribuir funções no Salesforce CRM](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|Conta de fluxo de automatização de energia|Crie um novo ambiente de produção com um banco de dados para teste, preparo e produção. Se você tiver um ambiente de produção existente com um banco de dados, ele poderá ser reutilizado. O usuário que vai instalar a solução de conector deve ter uma licença automatizada de energia e acesso a esse ambiente. Você pode monitorar o progresso e obter mais informações na [automatização de energia](https://flow.microsoft.com/) se a instalação falhar. Selecione **Ver histórico** em **soluções**.|[Criar ou gerenciar ambiente](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a>Instalação do pacote do Salesforce para campos personalizados da Microsoft

Para sincronizar as referências no Partner Center e no Salesforce CRM, a solução de automatização de energia precisa identificar claramente os campos de referência específicos da Microsoft. Essa demarcação fornece às equipes do vendedor do parceiro a capacidade de decidir quais referências eles desejam compartilhar com a Microsoft para venda.

1. No Salesforce, ative as **anotações** e adicione-as à lista de oportunidades relacionadas. [Referência](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

1. Ative as **equipes de oportunidades** seguindo as etapas:
    - Na instalação, use a caixa **localização rápida** para localizar as configurações da equipe de oportunidade.
    - Defina as configurações conforme necessário. [Referência](https://help.salesforce.com/articleView?id=sf.opp_team_manage.htm&type=5)

1. No Salesforce, instale campos personalizados e objetos usando o [instalador de pacote](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV). Use este instalador para instalar o pacote em qualquer empresa.

    >[!NOTE]
    >Se você estiver instalando em uma área restrita, deverá substituir a parte inicial da URL por `http://test.salesforce.com` .

1. No Salesforce, adicione soluções da Microsoft à lista de **oportunidades** relacionadas. Depois de adicionado, selecione o ícone de **chave inglesa** e atualize as propriedades

## <a name="best-practice-test-before-you-go-live"></a>Prática recomendada: teste antes de entrar no ar

Antes de instalar, configurar e personalizar a solução de automatização de energia no ambiente de produção, certifique-se de testar a solução em uma instância de CRM de preparo.

- Instale a solução de automatização de energia da Microsoft em uma instância de ambiente de preparo/CRM.

- Faça uma cópia da solução e execute sua configuração e automatize as personalizações de fluxo no ambiente de preparo.

- Teste a solução em uma instância de preparo/CRM.

- Em caso de sucesso, importe como uma solução gerenciada para a instância de produção.

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>Instalar a sincronização de referências do Partner Center para o Salesforce CRM

1. Vá para [energia automatizada](https://flow.microsoft.com) e selecione **ambientes** no canto superior direito. Isso mostrará as instâncias do CRM disponíveis.

1. Selecione a instância apropriada do CRM na lista suspensa no canto superior direito.

1. Selecione **soluções** na barra de navegação à esquerda.

1. Selecione o link **abrir AppSource** no menu superior.

   :::image type="content" source="images/cosellconnectors/open-appsource.png" alt-text="Abrir AppSource":::

1. Procure **conectores de referências do Partner Center para Salesforce** na tela pop-up.  

   :::image type="content" source="images/salesforce/salesforce-get-it-now.png" alt-text="Captura de tela de obter agora.":::

1. Selecione o botão **obter agora** e, em seguida, selecione **continuar**.

1. Na página seguinte, selecione o ambiente do Salesforce CRM para instalar o aplicativo. Concorde com os termos e condições.

1. Em seguida, você será direcionado para a página **gerenciar suas soluções** .  Navegue até "referências do Partner Center" usando os botões de seta na parte inferior da página. A **instalação agendada** deve aparecer ao lado da solução de referências do Partner Center. A instalação levará 10-15 minutos.

1. Após a conclusão da instalação, navegue de volta para [Power Automate](https://flow.microsoft.com) e selecione **soluções** na área de navegação à esquerda. Observe que a **sincronização de referências do Partner Center para Salesforce** agora está disponível na lista de soluções.

1. Selecione **sincronização de referências do Partner Center para Salesforce**. Os fluxos e as entidades automatizados de energia a seguir estão disponíveis:

   :::image type="content" source="images/cosellconnectors/partner-center-referrals-synchronization.png" alt-text="Fluxos do Salesforce":::

## <a name="configure-the-solution"></a>Configurar a solução

1. Depois de instalar a solução em sua instância do CRM, navegue de volta para o [Power Automate](https://flow.microsoft.com/).

1. Na lista suspensa **ambientes** no canto superior direito, selecione a instância de CRM na qual você instalou a solução de energia automatizada.

1. Você precisará criar conexões que associem as três contas de usuário:

   - Usuário do Partner Center com credenciais de administrador de referências
   - Eventos do Partner Center
   - Administrador de CRM com os fluxos de energia automatizada na solução

   1. Selecione **conexões** na barra de navegação à esquerda e selecione a solução de **referências do Partner Center** na lista.

   1. Crie uma conexão selecionando **criar uma conexão**.

        :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Captura de tela que mostra criar uma conexão.":::

   1. Procure por **referências do Partner Center (versão prévia)** na barra de pesquisa no canto superior direito.

   1. Crie uma conexão para o usuário do Partner Center com a função de credenciais do administrador de referências.

   1. Em seguida, crie uma conexão de eventos do Partner Center para o usuário do Partner Center com as credenciais do administrador de referências.

   1. Crie uma conexão para o Salesforce para o usuário administrador do CRM.
  
   1. Crie uma conexão para o Microsoft dataverso para o usuário administrador do CRM.

   1. Depois de adicionar todas as conexões, você deverá ver as seguintes conexões em seu ambiente:

        :::image type="content" source="images/cosellconnectors/salesforce-connections.png" alt-text="Captura de tela que mostra como observar conexões.":::

### <a name="edit-the-connections"></a>Editar as conexões

1. Volte para a página **soluções** e selecione **solução padrão**. Selecione **referência de conexão (versão prévia)** clicando em **tudo**.

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

Depois de instalar, configurar e personalizar a solução de Power Automate, você poderá testar a sincronização de indicações de venda em cooperação entre o Salesforce CRM e Partner Center.

### <a name="pre-requisites"></a>Pré-requisitos

Para sincronizar as indicações entre Partner Center e Salesforce CRM, a solução Power Automate precisa demarcar claramente os campos de indicação específicos da Microsoft. Essa identificação fornece às equipes de vendedores a capacidade de decidir quais indicações eles querem compartilhar com a Microsoft para venda em cooperação.

Um conjunto de campos personalizados está disponível como parte da Partner Center  sincronização de indicações para a entidade de oportunidade da solução Salesforce CRM. Um usuário administrador do CRM precisará criar uma seção crm separada com os **campos personalizados oportunidade.**

Os seguintes campos personalizados devem fazer parte da seção CRM:

- **Sincronizar com Partner Center**: se a oportunidade deve ser sincronizada com Partner Center. Por padrão, o valor desse campo é Não e precisa ser definido explicitamente como Sim pelo vendedor para compartilhar uma oportunidade com a Microsoft. Novas indicações compartilhadas de Partner Center crm terão esse valor de campo definido como Sim.

- **Identificador de Indicação:** um campo de identificador somente leitura para a indicação Partner Center Microsoft.

- **Link de** indicação: um link somente leitura para a indicação no Microsoft Partner Center.

- **Como a Microsoft pode ajudar:** ajuda necessária da Microsoft para a indicação. Para criar uma indicação de venda em cooperação, selecione a ajuda apropriada necessária da Microsoft. Um contato do cliente deve estar associado à oportunidade de criar uma indicação de venda em cooperação. Para criar uma indicação de não venda co-venda, não selecione este campo. Uma indicação de não venda co-venda pode ser convertida em uma indicação de venda em co-venda a qualquer momento selecionando a opção apropriada de ajuda necessária.

- **Visibilidade Partner Center referência** da Microsoft: selecione visibilidade para a Partner Center referência. Tornando-o visível para os vendedores da Microsoft, uma referência de não-venda pode ser convertida em uma venda conjunta. Quando a ajuda da Microsoft é necessária, a referência é visível para os vendedores da Microsoft por padrão. Depois que esse campo é marcado como visível, ele não pode ser revertido.

- **Identificador do Microsoft CRM**: quando uma referência de parceria de venda é criada e aceita pela Microsoft, esse campo será preenchido com o identificador CRM da Microsoft.

- **Soluções do Microsoft Partner Center**: um objeto personalizado para associar soluções prontas para venda ou soluções da Microsoft com a oportunidade. Uma ou mais soluções podem ser adicionadas ou removidas da oportunidade. É obrigatório adicionar pelo menos uma solução de revenda pronta ou da Microsoft à oportunidade antes de compartilhá-la com a Microsoft. Para associar esse objeto à oportunidade, atualize o formulário **oportunidade** no CRM.

- **Auditoria**: uma trilha de auditoria somente leitura para sincronização com as referências do Partner Center

### <a name="scenarios"></a>EXEMPLOS

1. Sincronização de referência quando a referência é criada ou atualizada no CRM e sincronizada no Partner Center:

   1. Entre no ambiente do Salesforce CRM com o usuário que tem visibilidade na seção **oportunidade** do CRM.

   1. Verifique se a seção **Microsoft Partner Center** está presente quando você cria uma **nova oportunidade** no ambiente do Salesforce CRM.

   1. As oportunidades sincronizadas com êxito com o Partner Center serão identificadas com ✔ ícone no Salesforce CRM.
      :::image type="content" source="images/salesforce/salesforce-environment.png" alt-text="Captura de tela do ambiente do Salesforce.":::

   1. Para sincronizar essa oportunidade com o Microsoft Partner Center, certifique-se de definir os seguintes campos no modo de exibição de cartão:

      - **Como a Microsoft pode ajudar?**: para criar uma referência de covenda, selecione uma opção de ajuda apropriada.

        :::image type="content" source="images/salesforce/salesforce-help-option.png" alt-text="Captura de tela que mostra como obter os campos apropriados no modo de exibição de cartão.":::

      - **Sincronizar com o Partner Center**: Sim
      - **Contato do cliente**: para criar uma referência de venda conjunta, adicione um contato do cliente à oportunidade.
      - **Soluções da Microsoft**: para compartilhar uma referência à Microsoft, adicione uma solução válida de covenda pronta ou Microsoft à oportunidade.

   1. Depois de definir a opção sincronização de oportunidade **com o Partner Center** como **Sim**, aguarde 10 minutos e entre em sua conta do Partner Center. Suas referências serão sincronizadas com o Salesforce CRM e o link de referência será preenchido. Se houver uma falha, o campo de auditoria será preenchido com informações de erro.

   1. Da mesma forma, quando a opção **sincronizar com o Partner Center** for definida como **Sim**, se você atualizar a oportunidade no Salesforce CRM, as alterações serão sincronizadas com sua conta do Partner Center.

2. Sincronização de referência quando a referência é criada ou atualizada no Microsoft Partner Center e sincronizada no ambiente do Salesforce CRM:

    1. Entre no [painel](https://partner.microsoft.com/dashboard/home)do Partner Center.

    1. Selecione **referências** no menu à esquerda.

    1. Crie uma nova referência de revenda do Partner Center clicando na opção "novo negócio".

    1. Entre no ambiente do Salesforce CRM.

    1. Navegue até **oportunidades abertas**. A referência criada no Microsoft Partner Center agora está sincronizada no Salesforce CRM.

    1. Quando você seleciona uma referência sincronizada, os detalhes da exibição do cartão são preenchidos.

       :::image type="content" source="images/salesforce/salesforce-casino.png" alt-text="Captura de tela da página de oportunidade do Salesforce.":::

>[!NOTE]
>**Precisa de ajuda com a implantação?**
>Para obter assistência com a implantação do conector de referência de sua venda, você pode participar de um consultor técnico do parceiro. Eles podem fornecer assistência de implantação e práticas recomendadas para uma implementação bem-sucedida.
>
>Para obter mais informações, consulte [como enviar uma solicitação de pré-vendas técnica e serviços de implantação](technical-benefits.md)

## <a name="next-steps"></a>Próximas etapas

- [Gerenciar clientes potenciais](manage-leads.md)

- [Gerenciar oportunidades de venda conjunta](manage-co-sell-opportunities.md)

- [Webhooks do Partner Center](/partner-center/develop/partner-center-webhooks)
