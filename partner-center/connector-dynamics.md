---
title: O conector de televenda para o centro de parceiros do Dynamics 365 CRM
description: Sincronize as referências no Partner Center com seu conector de televenda para o Dynamics 365 CRM. Você pode, então, vender com a Microsoft de dentro do seu sistema CRM.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 03/01/2021
ms.openlocfilehash: c399e00394208ec29dd59a41afe7cce1b1d07253
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284325"
---
# <a name="co-sell-connector-for-dynamics-365-crm-overview"></a>Visão geral do conector de venda conjunta para o Dynamics 365 CRM

**Funções apropriadas**

- Administrador de indicações
- Administrador do sistema ou personalizador do sistema no CRM

Os conectores da televenda do Partner Center permitem que seus vendedores covendam-se com a Microsoft de dentro de seus sistemas de CRM. Eles não precisarão ser treinados para usar o Partner Center para gerenciar acordos de venda. Use os conectores de venda conjunta para criar uma nova referência de venda conjunta para envolver um vendedor da Microsoft, receber referências do vendedor da Microsoft, aceitar ou recusar referências e modificar dados de negociações, como valor de acordo e data de fechamento. Você também pode receber todas as atualizações dos vendedores da Microsoft sobre esses acordos de venda conjunta. Você pode gerenciar todas as suas referências no CRM de sua escolha, em vez de no Partner Center.

A solução baseia-se na energia automatizada e usa as APIs do Partner Center.

## <a name="prerequisites"></a>Pré-requisitos

Antes de instalar a solução, certifique-se de atender aos seguintes pré-requisitos.

|**Tópicos**   |**Detalhes**   |**Links**   |
|--------------|--------------------|------|
|ID do Microsoft Partner Network (MPN) |Você precisa de uma ID de MPN válida.|[Ingressar na rede do parceiro](https://partner.microsoft.com/)|
|Co-venda pronta|Sua solução de IP/serviços deve estar pronta para venda.|[Venda com a Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)|
|Conta do Partner Center|A ID de MPN associada ao locatário do Partner Center deve ser a mesma que a ID do MPN associada à sua solução de venda conjunta. Verifique se você pode ver suas referências de venda conjunta no portal do Partner Center antes de implantar os conectores.|[Gerenciar sua conta](create-user-accounts-and-set-permissions.md)|
|Funções de usuário da Central de parceiros|O funcionário que irá instalar e usar os conectores deve ser um administrador de referências.|[Atribuir permissões e funções de usuários](create-user-accounts-and-set-permissions.md)|
|CRM do Dynamics 365|A função de usuário CRM é administrador do sistema ou personalizador do sistema.|[Atribuir funções no Dynamics 365](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Conta de fluxo de automatização de energia|Crie um novo ambiente de produção com um banco de dados para teste, preparo e produção. Se você tiver um ambiente de produção existente com um banco de dados, ele poderá ser reutilizado. O usuário que vai instalar a solução de conector deve ter uma licença automatizada de energia e acesso a esse ambiente. Você pode monitorar o progresso e obter mais informações na [automatização de energia](https://flow.microsoft.com/) se a instalação falhar. Selecione **Ver histórico** em **soluções**.|[Criar ou gerenciar ambiente](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Instalar a sincronização de referências do Partner Center para o Dynamics 365 (solução de automatização de energia)

1. Vá para [energia automatizada](https://flow.microsoft.com)e selecione **ambientes** no canto superior direito. Esta etapa mostrará as instâncias do CRM disponíveis.

1. Selecione a instância apropriada do CRM na lista suspensa no canto superior direito.

1. Selecione **soluções** à esquerda.

1. Selecione o link **abrir AppSource** no menu superior.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Captura de tela que mostra o Open AppSource.":::

1. Procure **conectores de referências do Partner Center para o Dynamics 365** na tela pop-up.  

1. Selecione o botão **obter agora** e, em seguida, selecione **continuar**.

1. Uma página é exibida onde você pode selecionar o ambiente CRM (Dynamics 365) para instalar o aplicativo. Concorde com os termos e condições.

1. Você pode monitorar o progresso e, se a instalação falhar, você pode obter mais detalhes na automação de energia selecionando **ver o histórico** em **soluções**.

1. Depois que a instalação for concluída, volte para a [energia automatizada](https://flow.microsoft.com) e selecione **soluções** à esquerda. A **sincronização de referências do Partner Center para o Dynamics 365** agora está disponível na lista de **soluções** .

1. Selecione **sincronização de referências do Partner Center para o Dynamics 365**. Os fluxos e as entidades automatizados de energia a seguir estão disponíveis.

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Captura de tela que mostra o CRMs disponível.":::

## <a name="test-before-you-go-live"></a>Teste antes de entrar no ar

Antes de instalar, configurar e personalizar a solução de automatização de energia no ambiente de produção, certifique-se de testar a solução em uma instância de CRM de preparo. Você precisará:

- Instale a solução de energia automatizada em uma instância de CRM do ambiente de preparo.
- Configurar e personalizar a solução de automatização de energia em um ambiente de preparo.
- Teste a solução em uma instância de CRM de preparo.
- Após um teste bem-sucedido, importe como uma solução gerenciada para a instância de produção.

## <a name="configure-the-solution"></a>Configurar a solução

1. Depois de instalar a solução em sua instância do CRM, volte para o [Power Automate](https://flow.microsoft.com/).

1. Na lista suspensa **ambientes** no canto superior direito, selecione a instância de CRM na qual você instalou a solução de energia automatizada.

1. Você precisará criar conexões que associem as três contas de usuário:

   - Usuário do Partner Center com credenciais de administrador de referências
   - Eventos do Partner Center
   - Administrador de CRM com os fluxos de energia automatizada na solução

   1. Selecione **conexões** à esquerda e selecione a solução de **referências do Partner Center** na lista.

   1. Crie uma conexão selecionando **criar uma conexão**.

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Captura de tela que mostra criar uma conexão.":::

   1. Procure por **referências do Partner Center (versão prévia)** na barra de pesquisa no canto superior direito.

   1. Crie uma conexão para o usuário do Partner Center com a função de credenciais do administrador de referências.

   1. Em seguida, crie uma conexão de eventos do Partner Center para o usuário do Partner Center com as credenciais de administrador de referências.

   1. Crie uma conexão para Common Data Service (ambiente atual) para o usuário administrador do CRM.
     
   1. Depois de adicionar todas as conexões, você deverá ver as seguintes conexões em seu ambiente.

      :::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="Captura de tela que mostra conexões.":::

## <a name="edit-the-connections"></a>Editar as conexões

1. Volte para a página **soluções** e selecione **solução padrão**. Selecione **referência de conexão (versão prévia)** selecionando **tudo**.

   :::image type="content" source="images/connection-reference-video.gif" alt-text="Captura de tela que mostra a edição das conexões.":::

1. Edite cada uma das conexões individualmente selecionando o ícone de reticências. Adicione as conexões relevantes.

   :::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="Captura de tela que mostra as conexões listadas.":::

1.  Retorne à página **soluções** , selecione **sincronização de referências do Partner Center para o Dynamics 365** e ative o fluxo selecionando o ícone de reticências ao lado de cada fluxo na sequência a seguir. Se você encontrar problemas enquanto ativa o fluxo, consulte [etapas de personalização](connector-dynamics.md#customize-synchronization-steps) e etapas de [solução de problemas](connectors-troubleshoot.md).

Ative os fluxos na seguinte sequência:

- Registro do webhook do Partner Center (insider Preview)
- Criar referência de co-venda – Dynamics 365 para o Partner Center (insider Preview)
- Personalizar Criar ou obter detalhes do fluxo do Dynamics 365
- Partner Center para Dynamics 365-auxiliar (insider Preview)
- Partner Center Microsoft co-vender atualizações de referência para o Dynamics 365 (insider Preview)
- Partner Center para Dynamics 365 (insider Preview)
- Dynamics 365 para o Partner Center (insider Preview)
- Oportunidade do Dynamics 365 para o Partner Center (insider Preview)
- Dynamics 365 Microsoft Solutions para Partner Center (insider Preview)
 
## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Usar APIs de webhook para registrar eventos de alteração de recurso

Você pode usar as APIs de webhook do Partner Center para se registrar para eventos de alteração de recursos. Esses eventos de alteração são enviados para a URL como postagens HTTP.

1. Selecione **Partner Center para Dynamics 365 (insider Preview)**.

1. Selecione o ícone **Editar** e selecione **quando uma solicitação HTTP é recebida**.

1. Selecione o ícone de **cópia** para copiar a URL de postagem http fornecida.

   :::image type="content" source="images/webhook-video.gif" alt-text="Captura de tela que mostra o uso de WebHooks para registrar alterações de recursos.":::

1. Selecione o **registro do webhook do Partner Center (insider Preview)** automatizar o fluxo de energia e, em seguida, selecione **executar**.

1. Verifique se a janela **executar fluxo** é aberta no painel direito e selecione **continuar**.

1. Insira os seguintes detalhes:

   - **Ponto de extremidade de gatilho http**: essa URL foi copiada de uma etapa anterior.
   - **Eventos a serem registrados**: selecione todos os eventos disponíveis (**referência criada**, **referência atualizada**, **relacionada à referência criada** e atualizada pela **referência relacionada**).
   - **Substituir pontos de extremidade de gatilho existentes se estiverem presentes?**: Sim. Somente uma URL pode ser registrada para um determinado evento de webhook.

1. Selecione **executar fluxo** e, em seguida, selecione **concluído.**

O webhook agora pode escutar, criar e atualizar eventos.

## <a name="customize-synchronization-steps"></a>Personalizar etapas de sincronização

Os sistemas de CRM são altamente personalizados e você pode personalizar a solução de automatização de energia com base na configuração do CRM. Quando as referências de venda cruzada são sincronizadas entre o Partner Center e o sistema CRM, os campos que são sincronizados no PC do Partner Center são listados no [Guia de mapeamento de campo personalizado](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S).

Siga o guia de mapeamento de campo e, se necessário, faça as alterações apropriadas em **[personalizar] criar ou obter detalhes de variáveis de ambiente ou fluxo do Dynamics 365** . Não atualize nenhum outro fluxo na solução de energia automatizada, pois isso pode afetar futuras atualizações da solução.

As seguintes personalizações estão disponíveis:

- **Exibir marca de seleção no nome da oportunidade**: por padrão, uma marca de seleção será exibida ao lado do nome da oportunidade para indicar que a sincronização entre o Partner Center e o Dynamics 365 CRM está ocorrendo com êxito. Da mesma forma, uma marca cruzada será exibida se a sincronização falhar. Para evitar adicionar uma verificação ou uma marca cruzada no nome da oportunidade, defina o valor atual da marca de seleção de exibição na variável de ambiente **nome da oportunidade** como não.
- **Valor de acordo**: por padrão, o valor de negócio do Partner Center será sincronizado de e para **estimado** no CRM. Se você tiver um campo diferente no CRM para o valor de acordo a ser sincronizado:

  - Atualize o nome do campo de **valor de acordo** na variável de ambiente Dynamics 365 com o nome do campo do CRM. Certifique-se de fornecer o nome do campo, não seu nome de exibição.
  - Edite **[Personalize] Crie ou Obtenha detalhes do fluxo do Dynamics 365** e vá para **criar ou atualizar oportunidade** no CRM e atualizar **criar uma nova oportunidade** e atualizar as ações de **oportunidade existentes** para atribuir o valor de **contrato** ao campo correto no CRM. Além disso, remova a atribuição de **dealvalue** do campo **receita estimada** .

- **Código do país da conta do cliente**: é obrigatório fornecer um código de país de duas letras (ISO 3166) ao criar uma nova referência. Por padrão, o código do país será sincronizado de e para o campo de **address1_country** da conta no CRM. Se você tiver um campo diferente no CRM para o código do país a ser sincronizado:

   - Para um campo de código de país não pesquisado na conta que contém um código de duas letras:
     - Atualize o nome do campo de **código do país da conta do cliente** na variável de ambiente Dynamics 365 com o nome do campo do CRM. Certifique-se de fornecer o nome do campo, não seu nome de exibição.
     - Edite **[Personalize] Crie ou Obtenha detalhes do fluxo do Dynamics 365** e vá para **criar ou obter conta de cliente** na ação CRM para atribuir um valor de **país** ao campo correto no CRM. Além disso, remova a atribuição de valor de **país** do campo **endereço 1: país/região** .

   - Para um campo de código de país baseado em pesquisa na conta:
     - Adicione um novo campo personalizado na conta e preencha-o automaticamente com um código de país de duas letras (ISO 3166) com base no valor selecionado no campo baseado em pesquisa e vice-versa.
     - Siga as etapas anteriores para o campo código de país não pesquisado para sincronizar um novo campo personalizado do CRM para o e do Partner Center.

- **Campos de oportunidade**: se houver campos obrigatórios em **oportunidade** que precisam ser preenchidos, edite **[Personalize] Crie ou Obtenha detalhes do fluxo do Dynamics 365** e vá para **criar ou atualizar oportunidade** no CRM e atualizar **criar uma nova ação de oportunidade** para atribuir valores aos campos obrigatórios com base em seus requisitos de negócios.
- **Campos de Lead**: se houver campos obrigatórios no **cliente potencial** que precisam ser preenchidos, edite **[Personalize] Crie ou Obtenha detalhes do fluxo do Dynamics 365** e vá para **criar ou atualizar cliente potencial** no CRM e atualizar **criar uma nova ação de cliente potencial** para atribuir valores aos campos obrigatórios com base em seus requisitos de negócios.
- **Conta de cliente**: quando uma nova referência é sincronizada do Partner Center para o CRM, a solução de automatização de energia tenta pesquisar uma conta existente no CRM usando o nome da empresa do cliente e o CEP. Se não encontrar uma, uma nova conta de cliente será criada no CRM. Para atualizar os critérios de pesquisa e novos detalhes de criação de conta, edite **[Customize] Create ou Obtenha detalhes do fluxo do Dynamics 365** e vá para **criar ou obter conta de cliente** no CRM e **criar a ação de conta do cliente**.

## <a name="update-environment-variable"></a>Atualizar variável de ambiente

Para atualizar um valor de variável de ambiente:

1. Vá para a página **soluções** e selecione **solução padrão**. Selecione a **variável de ambiente** selecionando **tudo**.

1. Selecione a variável de ambiente para o valor que precisa ser atualizado e selecione **Editar** usando o ícone de reticências.

1. Atualize o **valor atual** (não atualize o **valor padrão**) usando a opção **novo valor** e fornecendo o valor. O valor deve corresponder ao tipo de dados da variável. Por exemplo, o tipo de dados sim ou nenhum aceitará o valor Sim ou não.

   :::image type="content" source="images/environment-variables-video.gif" alt-text="Captura de tela que mostra as variáveis de ambiente de atualização.":::

## <a name="end-to-end-bidirectional-co-sell-referral-synchronization"></a>Sincronização de referência de cooperação bidirecional de ponta a ponta

Depois de instalar, configurar e personalizar a solução de automatização de energia, você pode testar a sincronização de referências de venda entre o Dynamics 365 e o Partner Center.

### <a name="prerequisites"></a>Pré-requisitos

Para sincronizar as referências no Partner Center e no Dynamics 365 CRM, a solução de energia automatizada claramente demarcates os campos de referência específicos da Microsoft. Essa identificação fornece às equipes do vendedor a capacidade de decidir quais referências eles desejam compartilhar com a Microsoft para fazer a venda.

Um conjunto de campos e objetos personalizados será adicionado como parte da instalação da solução. Um usuário administrador de CRM precisará criar uma seção de CRM separada com os campos personalizados de **oportunidade** .

Os campos personalizados a seguir devem fazer parte da seção CRM:

- **Sincronizar com o Partner Center**: se deseja sincronizar a oportunidade com o Partner Center. Por padrão, o valor desse campo é não e precisa ser definido explicitamente como sim pelo seu vendedor para compartilhar uma oportunidade com a Microsoft. As novas referências compartilhadas do Partner Center para o CRM terão esse valor de campo definido como Sim.
- **Identificador de referência**: um campo de identificador somente leitura para a referência do Partner Center.
- **Link de referência**: um link somente leitura para a referência no Partner Center.
- **Como a Microsoft pode ajudar?**: a ajuda necessária da Microsoft para a referência. Para criar uma referência de covenda, selecione a ajuda apropriada necessária da Microsoft. Um contato de cliente deve estar associado à oportunidade de criar uma referência de covenda. Para criar uma referência que não seja de cooperação, não selecione este campo. Uma referência que não é de televenda pode ser convertida em uma referência de covenda a qualquer momento, selecionando a opção apropriada de ajuda necessária.
- **Visibilidade da referência do Microsoft Partner Center**: selecione visibilidade para a referência do Partner Center. Tornando-o visível para os vendedores da Microsoft, uma referência de não-venda pode ser convertida em uma venda conjunta. Quando a ajuda da Microsoft é necessária, a referência é visível para os vendedores da Microsoft por padrão. Depois que esse campo é marcado como visível, ele não pode ser revertido.
- **Identificador do Microsoft CRM**: quando uma referência de parceria de venda é criada e aceita pela Microsoft, esse campo será preenchido com o identificador CRM da Microsoft.
- **Produtos: obsoletos**: não use este campo ou adicione-o à seção CRM. Ele está disponível apenas para compatibilidade com versões anteriores. Em vez disso, use soluções do Partner Center.
- **Auditoria**: uma trilha de auditoria somente leitura para sincronização com as referências do Partner Center.
- **Soluções do Microsoft Partner Center**: um objeto personalizado para associar soluções prontas para venda ou soluções da Microsoft com a oportunidade. Uma ou mais soluções podem ser adicionadas ou removidas da oportunidade. É obrigatório adicionar pelo menos uma solução de revenda pronta ou da Microsoft à oportunidade antes de compartilhá-la com a Microsoft. Para associar esse objeto à oportunidade, atualize o formulário **oportunidade** no CRM.

  Selecione a guia apropriada no formulário **oportunidade** e adicione uma subgrade, conforme mostrado aqui.

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="Captura de tela que mostra o formulário oportunidade.":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="Captura de tela que mostra as soluções da Microsoft.":::

- Depois de adicionar as soluções da Microsoft, você pode preencher previamente os detalhes da solução pronta para a venda para que seus vendedores não precisem adicioná-los. Para adicionar um novo detalhe da solução, vá para o objeto de detalhes da solução da Microsoft no CRM e selecione **adicionar registro** para adicionar uma entrada ou usar o **carregamento do Excel** para adicionar várias entradas.

  :::image type="content" source="images/dynamic-1a.png" alt-text="Captura de tela que mostra os novos detalhes da solução Microsoft.":::

### <a name="scenarios"></a>Cenários

1. Sincronização de referência quando a referência é criada ou atualizada no CRM e sincronizada no Partner Center:

   1. Entre no ambiente do Dynamics 365 CRM com o usuário que tem visibilidade na seção **oportunidade** do CRM.

   1. Verifique se a seção **Microsoft Partner Center** está presente quando você cria uma nova oportunidade no ambiente do Dynamics 365.

      :::image type="content" source="images/dynamic-2a.png" alt-text="Captura de tela que mostra uma nova oportunidade.":::

   1. Para sincronizar essa oportunidade com o Partner Center, certifique-se de definir os seguintes campos no modo de exibição de cartão:

      - **Como a Microsoft pode ajudar?**: para criar uma referência de covenda, selecione uma opção de ajuda apropriada.

         :::image type="content" source="images/dynamic-3a.png" alt-text="Captura de tela que mostra como obter os campos apropriados no modo de exibição de cartão.":::

      - **Contato do cliente**: para criar uma referência de venda conjunta, adicione um contato do cliente à oportunidade.
      - **Sincronizar com o Partner Center**: Sim.
      - **Soluções da Microsoft**: para compartilhar uma referência à Microsoft, adicione uma solução válida de covenda pronta ou Microsoft à oportunidade.
      
        :::image type="content" source="images/dynamic-4a.png" alt-text="Captura de tela que mostra a ID da solução.":::

   1. Depois que a oportunidade for criada no Dynamics 365 com a opção **sincronizar com o Partner Center** definida como Sim, aguarde 10 minutos. Em seguida, entre em sua conta do Partner Center. Suas referências serão sincronizadas com o Dynamics 365 e o **identificador de referência**. O **link de referência** será preenchido. Se houver uma falha, o campo de **auditoria** será preenchido com informações de erro.
     
    1. Da mesma forma, para uma oportunidade que tinha a opção **sincronizar com o Partner Center** definida como Sim, se você atualizar a oportunidade no Dynamics 365 CRM, as alterações serão sincronizadas em sua conta do Partner Center.

    1. As oportunidades sincronizadas com êxito com o Partner Center serão identificadas com ✔ ícone no Dynamics 365.

1. Sincronização de referência quando a referência é criada ou atualizada no Partner Center e sincronizada no ambiente do Dynamics 365:

   1. Entre no [painel](https://partner.microsoft.com/dashboard/home)do Partner Center.

   1. Selecione **referências** no menu à esquerda.

   1. Crie uma nova referência de revenda do Partner Center selecionando a **nova** opção de negócio.

   1. Entre no ambiente do Dynamics 365 CRM.

   1. Acesse **oportunidades abertas**. A referência criada no Partner Center agora está sincronizada no Dynamics 365 CRM.

   1. Quando você seleciona uma referência sincronizada, os detalhes da exibição do cartão são preenchidos.

## <a name="next-steps"></a>Próximas etapas

- [Gerenciar clientes potenciais](manage-leads.md)
- [Gerenciar oportunidades de venda conjunta](manage-co-sell-opportunities.md)
- [Mais informações sobre a plataforma de automatização de energia da Microsoft](/power-automate/)
- [Webhooks do Partner Center](/partner-center/develop/partner-center-webhooks)
