---
title: O conector de venda co-venda para o Dynamics 365 CRM Partner Center
description: Sincronizar as indicações Partner Center com seu conector de venda co-venda para o Dynamics 365 CRM. Em seguida, você pode fazer a venda em cooperação com a Microsoft de dentro do seu sistema CRM.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 03/01/2021
ms.openlocfilehash: e656f728789bf5b13dd09732b0b2f5ef30de760a
ms.sourcegitcommit: b7203f1393c3d8f8db4683acdebd09a89e086c3c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/21/2021
ms.locfileid: "112425039"
---
# <a name="co-sell-connector-for-dynamics-365-crm-overview"></a>Visão geral do conector de venda co-venda do Dynamics 365 CRM

**Funções apropriadas:** indicações de administrador | Administrador do sistema ou personalizador de sistema no CRM

Partner Center conectores de venda co-venda permitem que os vendedores vendam com a Microsoft de dentro de seus sistemas CRM. Eles não precisam ser treinados para usar o Partner Center gerenciar acordos de venda em cooperação. Use os conectores de venda co-venda para criar uma nova indicação de venda em cooperação para envolver um vendedor da Microsoft, receber indicações do vendedor da Microsoft, aceitar ou recusar indicações e modificar dados de negociação, como valor da negociação e data de fechamento. Você também pode receber atualizações dos vendedores da Microsoft nessas negociações de venda de venda. Você pode gerenciar todas as suas indicações que funcionam no CRM de sua escolha em vez de em Partner Center.

A solução é baseada em Power Automate e usa Partner Center APIs.

## <a name="prerequisites"></a>Pré-requisitos

Antes de instalar a solução, certifique-se de atender aos pré-requisitos a seguir.

|**Tópicos**   |**Detalhes**   |**Links**   |
|--------------|--------------------|------|
|ID do Microsoft Partner Network (MPN) |Você precisa de uma ID de MPN válida.|[Ingressar na Rede de Parceiros](https://partner.microsoft.com/)|
|Pronto para venda conjunta|Sua solução de IP/Serviços deve estar pronta para venda em cooperação.|[Vender com a Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)|
|Conta do Partner Center|A ID do MPN associada ao locatário Partner Center deve ser igual à ID do MPN associada à sua solução de venda de venda. Verifique se você pode ver suas indicações de venda de venda no portal Partner Center antes de implantar os conectores.|[Gerenciar sua conta](create-user-accounts-and-set-permissions.md)|
|Funções de usuário da Central de parceiros|O funcionário que instalará e usará os conectores deve ser um administrador de indicações.|[Atribuir permissões e funções de usuários](create-user-accounts-and-set-permissions.md)|
|Dynamics 365 CRM|A função de usuário crm é Administrador do sistema ou Personalizador do sistema.|[Atribuir funções no Dynamics 365](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Power Automate de fluxo|Crie um novo ambiente de produção com um banco de dados para teste, preparação e produção. Se você tiver um ambiente de produção existente com um banco de dados, ele poderá ser reutilizado. O usuário que instalará a solução do conector deve ter uma licença Power Automate e acesso a esse ambiente. Você pode monitorar o progresso e obter mais informações em [Power Automate](https://flow.microsoft.com/) se a instalação falhar. Selecione **Ver histórico** em **Soluções.**|[Criar ou gerenciar o ambiente](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Instalar Partner Center sincronização de indicações do Dynamics 365 (Power Automate solução)

1. Vá para [Power Automate](https://flow.microsoft.com)e selecione **Ambientes** no canto superior direito. Esta etapa mostrará as instâncias de CRM disponíveis.

1. Selecione a instância de CRM apropriada na listada no canto superior direito.

1. Selecione **Soluções** à esquerda.

1. Selecione o link **Abrir AppSource** no menu superior.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Captura de tela que mostra Abrir AppSource.":::

1. Pesquise Partner Center conectores de indicações **do Dynamics 365** na tela pop-up.  

1. Selecione o **botão Obter agora** e, em seguida, selecione **Continuar.**

1. É exibida uma página em que você pode selecionar o ambiente crm (Dynamics 365) para instalar o aplicativo. Concorde com os termos e condições.

1. Você pode monitorar o progresso e, se a instalação falhar, poderá obter mais detalhes em Power Automate selecionando Ver histórico **em** **Soluções**.

1. Depois que a instalação for concluída, volte para [Power Automate](https://flow.microsoft.com) e selecione **Soluções** à esquerda. **Partner Center sincronização de indicações para Dynamics 365** agora está disponível na lista **Soluções.**

1. Selecione **Partner Center sincronização de indicações do Dynamics 365.** As seguintes Power Automate fluxos e entidades estão disponíveis.

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Captura de tela que mostra os CRMs disponíveis.":::

## <a name="test-before-you-go-live"></a>Testar antes de entrar no ar

Antes de instalar, configurar e personalizar a solução Power Automate no ambiente de produção, teste a solução em uma instância de CRM de preparação. Você precisará:

- Instale a solução Power Automate em uma instância crm do ambiente de preparação.
- Configure e personalize a Power Automate em um ambiente de preparação.
- Teste a solução em uma instância de CRM de preparação.
- Após um teste bem-sucedido, importe como uma solução gerenciada para a instância de produção.

## <a name="configure-the-solution"></a>Configurar a solução

1. Depois de instalar a solução em sua instância do CRM, volte [para](https://flow.microsoft.com/)Power Automate .

1. Na lista **de listas listadas** em Ambientes no canto superior direito, selecione a instância crm em que você instalou a solução Power Automate aplicativo.

1. Você precisará criar conexões que associem as três contas de usuário:

   - Partner Center usuário com credenciais de administrador de indicações
   - Eventos do Partner Center
   - Administrador de CRM com Power Automate fluxos na solução

   1. Selecione **Conexões** à esquerda e selecione a **solução Partner Center Indicações** na lista.

   1. Crie uma conexão selecionando **Criar uma conexão**.

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Captura de tela que mostra Criar uma conexão.":::

   1. **Pesquise Partner Center Indicações (versão prévia)** na barra de pesquisa no canto superior direito.

   1. Crie uma conexão para seu Partner Center usuário com a função de credenciais do administrador de indicações.

   1. Em seguida, crie uma conexão Partner Center Eventos para seu Partner Center com as credenciais de administrador de indicações.

   1. Crie uma conexão para o Common Data Service (ambiente atual) para o usuário administrador do CRM.
     
   1. Depois de adicionar todas as conexões, você deverá ver as seguintes conexões em seu ambiente.

      :::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="Captura de tela que mostra as conexões.":::

## <a name="edit-the-connections"></a>Editar as conexões

1. Retorne à página **Soluções** e selecione **Solução Padrão.** Selecione **Referência de Conexão (versão prévia)** selecionando **Todos.**

   :::image type="content" source="images/connection-reference-video.gif" alt-text="Captura de tela que mostra a edição das conexões.":::

1. Edite cada uma das conexões individualmente selecionando o ícone de reellipse. Adicione as conexões relevantes.

   :::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="Captura de tela que mostra as conexões listadas.":::

1. Retorne à  página Soluções, selecione Partner Center Sincronização de Indicações para **o Dynamics 365** e a ligue o fluxo selecionando o ícone de reellipse ao lado de cada fluxo na sequência a seguir. Se você encontrar problemas ao ativar o fluxo, confira [Etapas de personalização](connector-dynamics.md#customize-synchronization-steps) e [Etapas de solução de problemas.](connectors-troubleshoot.md)

A ligar os fluxos na sequência a seguir:

- Partner Center de webhook (visualização do insider)
- Criar indicação de venda co-venda – Dynamics 365 para Partner Center (Visualização do Insider)
- [Personalizar] Criar ou obter detalhes do fluxo do Dynamics 365
- Partner Center para o Dynamics 365 – Auxiliar (Visualização do Insider)
- Partner Center atualizações de indicação de venda co-venda da Microsoft para o Dynamics 365 (Versão Prévia do Insider)
- Partner Center ao Dynamics 365 (Insider Preview)
- Dynamics 365 to Partner Center (Insider Preview)
- Oportunidade do Dynamics 365 para Partner Center (Visualização do Insider)
- Dynamics 365 Microsoft Solutions to Partner Center (Insider Preview)
 
## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Usar APIs de webhook para se registrar para eventos de alteração de recursos

Você pode usar as APIs Partner Center webhook para se registrar para eventos de alteração de recurso. Esses eventos de alteração são enviados para a URL como postagens HTTP.

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

  :::image type="content" source="images/cosellconnectors/dynamics-solution-1.png" alt-text="Captura de tela que mostra os novos detalhes da solução Microsoft.":::

### <a name="scenarios"></a>Cenários

1. Sincronização de referência quando a referência é criada ou atualizada no CRM e sincronizada no Partner Center:

   1. Entre no ambiente do Dynamics 365 CRM com o usuário que tem visibilidade na seção **oportunidade** do CRM.

   1. Verifique se a seção **Microsoft Partner Center** está presente quando você cria uma nova oportunidade no ambiente do Dynamics 365.

      :::image type="content" source="images/cosellconnectors/dynamics-solution-2.png" alt-text="Captura de tela que mostra uma nova oportunidade.":::

   1. Para sincronizar essa oportunidade com o Partner Center, certifique-se de definir os seguintes campos no modo de exibição de cartão:

      - **Como a Microsoft pode ajudar?**: para criar uma referência de covenda, selecione uma opção de ajuda apropriada.

         :::image type="content" source="images/cosellconnectors/dynamics-solution-3.png" alt-text="Captura de tela que mostra como obter os campos apropriados no modo de exibição de cartão.":::

      - **Contato do cliente**: para criar uma referência de venda conjunta, adicione um contato do cliente à oportunidade.
      - **Sincronizar com Partner Center:** Sim.
      - **Soluções da Microsoft:** para compartilhar uma indicação com a Microsoft, adicione uma solução válida pronta para venda em comum ou da Microsoft à oportunidade.

        :::image type="content" source="images/cosellconnectors/dynamics-solution-4.png" alt-text="Captura de tela que mostra a ID da solução.":::

   1. Depois que a oportunidade for criada no Dynamics 365 com a opção **Sincronizar** com Partner Center definida como Sim, aguarde 10 minutos. Em seguida, entre em sua Partner Center de dados. Suas indicações serão sincronizadas com o Dynamics 365 e o **Identificador de Indicação.** **O Link de** Indicação será preenchido. Se houver uma falha, o campo **Auditoria** será preenchido com informações de erro.

      1. Da mesma forma, para uma oportunidade que tinha a opção Sincronizar com Partner Center definida como Sim, se você atualizar **a** oportunidade no Dynamics 365 CRM, as alterações serão sincronizadas em sua conta Partner Center cliente.

      1. As oportunidades sincronizadas com êxito com Partner Center serão identificadas com ✔icon no Dynamics 365.

1. Sincronização de indicação quando a indicação é criada ou atualizada Partner Center e sincronizada no ambiente do Dynamics 365:

   1. Entre no painel de Partner Center [.](https://partner.microsoft.com/dashboard/home)

   1. Selecione **Indicações** no menu à esquerda.

   1. Crie uma nova indicação de venda de Partner Center selecionando a **opção Nova** oferta.

   1. Entre em seu ambiente do Dynamics 365 CRM.

   1. Vá para **Abrir Oportunidades**. A indicação criada Partner Center agora está sincronizada no Dynamics 365 CRM.

   1. Quando você seleciona uma indicação sincronizada, os detalhes da exibição de cartão são preenchidos.

## <a name="next-steps"></a>Próximas etapas

- [Gerenciar clientes potenciais](manage-leads.md)
- [Gerenciar oportunidades de venda conjunta](manage-co-sell-opportunities.md)
- [Mais sobre a plataforma microsoft Power Automate](/power-automate/)
- [Webhooks do Partner Center](/partner-center/develop/partner-center-webhooks)
