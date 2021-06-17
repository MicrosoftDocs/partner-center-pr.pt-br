---
title: O conector de venda co-venda para o Salesforce CRM Partner Center
ms.topic: how-to
ms.date: 01/06/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Sincronizar suas indicações no Partner Center com o Salesforce CRM. Em seguida, os vendedores podem fazer a venda em cooperação com a Microsoft de dentro de seus sistemas crm.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 74894671966ac0409f6366f33c91ddadfae1ba4c
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276970"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Conector de venda conjunta para o Salesforce CRM – visão geral

**Funções apropriadas:** indicações de administrador | Administrador do sistema ou personalizador de sistema no CRM

Partner Center conector de venda co-venda permite que os vendedores vendam com a Microsoft de dentro de seus sistemas CRM. Eles não precisam ser treinados para usar o Partner Center gerenciar acordos de venda em cooperação. Usando os conectores de venda de co-venda, você pode criar uma nova indicação de venda co-venda para envolver um vendedor da Microsoft, receber indicações do vendedor da Microsoft, aceitar/recusar indicações, modificar dados de negociação, como valor da oferta e data de fechamento.  Você também pode receber atualizações dos vendedores da Microsoft nesses acordos de venda em cooperação. Você pode fazer todas as suas indicações funcionarem enquanto trabalham dentro do CRM de sua escolha em vez de em Partner Center. 

A solução baseia-se na solução microsoft Power Automate e usa apIs Partner Center aplicativo.

## <a name="before-you-install---pre-requisites"></a>Antes de instalar – pré-requisitos

|**Tópicos**   |**Detalhes**   |**Links**   |
|--------------|--------------------|------|
|Microsoft Partner Network ID |Você precisa de uma ID de MPN válida|Para ingressar no [MPN](https://partner.microsoft.com/)|
|Pronto para venda conjunta|Sua solução de IP/Serviços deve estar pronta para venda em cooperação.|[Vender com a Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Conta do Partner Center|A ID do MPN associada ao locatário Partner Center deve ser igual à ID do MPN associada à sua solução de venda co-venda. Verifique se você pode ver suas indicações de venda em Partner Center portal antes de implantar os conectores.|[Gerenciar sua conta](create-user-accounts-and-set-permissions.md)|
|Funções de usuário da Central de parceiros|O funcionário que instalará e usará os conectores deve ser um administrador de indicações|[Atribuir permissões e funções de usuários](create-user-accounts-and-set-permissions.md)|
|Salesforce CRM|A função de usuário crm é Administrador do sistema ou Personalizador do sistema|[Atribuir funções no Salesforce CRM](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|Power Automate Flow Account|Uma conta [Power Automate](https://flow.microsoft.com) ativa para o administrador do sistema crm ou personalizador do sistema. Esse usuário deve entrar no [Power Automate](https://flow.microsoft.com) pelo menos uma vez antes da instalação.|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a>Instalação do pacote salesforce para campos personalizados da Microsoft 

Para sincronizar as indicações entre Partner Center e Salesforce CRM, Power Automate solução precisa identificar claramente os campos de indicação específicos da Microsoft. Essa demarcação fornece às equipes de vendedores parceiros a capacidade de decidir quais indicações elas querem compartilhar com a Microsoft para venda em parceria.

1. No Salesforce, ative **as Notas** e adicione-as à lista de oportunidades relacionadas. 
[Referência](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. Ative **as equipes de** oportunidade seguindo as etapas: 
    - Em Instalação, use a **caixa Localização Rápida** para localizar as Configurações da Equipe de Oportunidade.
    - Defina as configurações conforme necessário.
[Referência](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. No Salesforce, instale objetos e campos personalizados usando o [instalador de pacote](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV). Use isso para instalar o pacote em qualquer empresa.

>[!NOTE]
>Se você estiver instalando em uma área sandbox, deverá substituir a parte inicial da URL por http://test.salesforce.com

4. No Salesforce, adicione Soluções da Microsoft à **lista relacionada** à oportunidade. Depois de adicionado, selecione o ícone **de chave inglesa** e atualize as propriedades

## <a name="best-practice-test-before-you-go-live"></a>Melhor prática: testar antes de entrar no ar

Antes de instalar, configurar e personalizar a solução Power Automate no ambiente de produção, teste a solução em uma instância de CRM de preparação.

- Instale a solução microsoft Power Automate em um ambiente de preparação/instância crm.

- Faça uma cópia da solução e execute sua configuração e Power Automate personalizações de fluxo no ambiente de preparação.

- Teste a solução em uma instância de preparação/CRM.

- Em caso de sucesso, importe como uma solução gerenciada para a instância de produção.

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>Instalar Partner Center sincronização de indicações do Salesforce CRM

1. Vá para [Power Automate](https://flow.microsoft.com) e selecione **Ambientes** no canto superior direito. Isso mostrará as instâncias de CRM disponíveis.

2. Selecione a instância de CRM apropriada na lista inferior no canto superior direito.

3. Selecione **Soluções** na barra de navegação à esquerda.

4. Selecione o link **Abrir AppSource** no menu superior.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Abra AppSource.":::

5. **Pesquise Partner Center conectores de indicações para Salesforce** na tela pop-up.  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce.":::

6. Selecione o **botão Obter agora e,** em seguida, **Continuar.**

7. Isso abre a página em que você pode selecionar o ambiente do Salesforce CRM para instalar o aplicativo.  Concorde com os termos e condições.

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="CRMS disponíveis.":::

8. Em seguida, você será direcionado para a **página Gerenciar suas soluções.**  Navegue até "Partner Center indicações" usando os botões de seta na parte inferior da página. **A instalação agendada** deve aparecer ao lado Partner Center de indicações. A instalação levará de 10 a 15 minutos.

9. Depois que a instalação for concluída, navegue de [volta para Power Automate](https://flow.microsoft.com) e selecione **Soluções** na área de navegação à esquerda. Observe que **Partner Center sincronização de indicações para Salesforce** está disponível na lista Soluções.

10. Selecione **Partner Center sincronização de indicações para o Salesforce.** As seguintes Power Automate fluxos e entidades estão disponíveis:

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Fluxos do Salesforce.":::



## <a name="configure-the-solution"></a>Configurar a solução

1. Depois de instalar a solução em sua instância do CRM, navegue de volta para [Power Automate](https://flow.microsoft.com/).

2. Na lista **de ambientes** no canto superior direito, selecione a instância do CRM em que você instalou a solução Power Automate aplicativo.
3. Você precisará criar conexões que associem as três contas de usuário:
    - Partner Center usuário com credenciais de administrador de indicações
    - Eventos do Partner Center
    - Administrador de CRM com Power Automate fluxos na solução.
4. Selecione **Conexões** na barra de navegação à esquerda e selecione a solução "Partner Center Indicações" na lista.

5. Crie uma conexão clicando em **Criar uma conexão**.

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Criar conexão.":::

- Pesquise Partner Center Indicações (versão prévia) na barra de pesquisa no canto superior direito.

- Crie uma conexão para seu Partner Center usuário com a função de credenciais do administrador de indicações.

-  Em seguida, crie uma conexão Partner Center eventos para seu Partner Center com as credenciais de administrador de indicações.

- Crie uma conexão para o Salesforce para o usuário administrador do CRM.

-  Depois de adicionar todas as Conexões, você deverá ver as seguintes Conexões em seu ambiente:

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Observe as conexões.":::

### <a name="edit-the-connections"></a>Editar as conexões

1. Retorne à página Soluções e selecione **Solução Padrão.**  Selecione **Referência de Conexão (versão prévia)** clicando em **Todos.**
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Inicie a edição do conector.":::

2. Edite cada uma das Conexões individualmente selecionando o ícone de três pontos. Adicione as conexões relevantes.

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Editar conectores.":::

3. A ligar os fluxos na sequência a seguir:

- Partner Center de webhook (visualização do insider)
- Criar indicação de venda co-venda – Salesforce para Partner Center (Visualização do Insider)
- Partner Center atualizações de indicação de venda co-venda da Microsoft para o Salesforce (Visualização do Insider)
- Partner Center ao Salesforce (Visualização do Insider)
- Salesforce para Partner Center (Insider Preview)
- Salesforce Opportunity to Partner Center (Insider Preview)
- Salesforce Microsoft Solutions to Partner Center (Insider Preview)

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Usar APIs de webhook para se registrar para eventos de alteração de recursos

As APIs Partner Center Webhook permitem que você se registre para eventos de alteração de recursos. Esses eventos de alteração são enviados para sua URL como postagens HTTP.

1. Para registrar sua URL, selecione Partner Center **registro de webhook (visualização do insider)** Power Automate fluxo.

2. Adicione conexões para (a.) Partner Center usuário com credenciais de administrador de indicações (b.) Partner Center Eventos conforme realçada abaixo

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Gatilho.":::

3. Ao fazer essas atualizações, você verá

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks.":::

4. Salve suas alterações e selecione **Ativar**.

   Para habilitar Partner Center webhooks para escutar alterações de evento, execute as seguintes etapas:

5. Selecione **Partner Center para Salesforce CRM (Insider Preview)**.

6. Selecione o **ícone Editar** e selecione Quando **uma solicitação HTTP é recebida.**

7. Selecione o **ícone Copiar** para copiar a URL HTTP POST fornecida.

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Copiar URL.":::

8. Agora selecione o fluxo de Partner Center de webhook (Visualização do Power Automate Insider)" e selecione **Executar**.

9. Verifique se a janela "Executar Fluxo" é aberta no painel direito e selecione **Continuar.**

10. Insira os seguintes detalhes:

    1. **Ponto de extremidade de gatilho HTTP:** URL copiada da etapa anterior

    2. **Eventos a registrar:**"criado por indicação" e "atualizado por indicação"

    3. **Substituir pontos de extremidade de gatilho existentes se estiver** presente: Sim (isso substitui todos os pontos de extremidade existentes.)

11. Selecione **Executar** e, em seguida, **selecione Feito.**

O webhook agora pode escutar para criar e atualizar eventos.

## <a name="customize-synchronization-steps"></a>Personalizar etapas de sincronização

Quando as indicações de venda co-venda são sincronizadas entre o Partner Center e o sistema CRM, os campos sincronizados no computador Partner Center são listados aqui.

Geralmente, os sistemas CRM são altamente personalizados. Você pode personalizar os fluxos Power Automate dados. Siga o guia de mapeamento de campo e, se necessário, faça as alterações apropriadas nas etapas dos Power Automate fluxos.  Os mapeamentos do Microsoft Partner Centers para CRM são fornecidos, mas com base em seu ambiente crm, você pode optar por personalizar ainda mais os campos.

Várias etapas de cada um dos fluxos Power Automate podem ser personalizados de acordo com suas necessidades. Veja a seguir exemplos de personalizações disponíveis:

1. Para personalizar os campos para os eventos de criação ou atualização no Partner Center sincronização de indicação do CRM:

   1. Selecione Partner Center Salesforce CRM (Insider Preview).

   2. Selecione **Editar** para editar/personalizar o Power Automate fluxo.

   3. Selecione **(Escopo) Sincronizar o lead ou a oportunidade**.

2. Para personalizar mapeamentos de campo crm para criar eventos, selecione **Se for uma nova oportunidade compartilhada, em seguida,**. Selecione a sub-etapa **se sim e,** em seguida, expanda **Criando uma nova oportunidade no CRM.** Você pode editar os mapeamentos nesta seção usando o Guia de Mapeamento de Campo.

   1. Para personalizar mapeamentos de campo crm para eventos de atualização, selecione a etapa "(Escopo) Sincronizar o cliente ou a oportunidade".

   2. Selecione **Se for uma atualização para uma oportunidade, em seguida,**. Selecione a sub-etapa **se sim e** expanda Se diferença entre os objetos de oportunidade no Partner Center e **CRM, em seguida,**.  

   3. Selecione **Se sim seguido** de Atualizar oportunidade **existente**

3. Para personalizar os campos para a sincronização de indicação de CRM para PC para eventos de atualização:

   1. Selecione **Editar**  para editar/personalizar o Power Automate fluxo.

   2. Selecione **(Escopo) Sincronizar a oportunidade.**

   3. Para personalizar mapeamentos de campo crm (com base no guia de mapeamentos de campo) para eventos de atualização, selecione Se houver diferença entre os objetos de cliente Partner Center e **CRM, em seguida,**.

   4. Selecione a sub-etapa se **sim e** expanda a etapa Atualizar **uma indicação com dados de oportunidade**.

   Você pode editar os mapeamentos nesta seção com base no Guia de Mapeamento de Campo.

4. Para personalizar os campos para a sincronização de indicação de CRM para PC para criar eventos?

   1. Selecione **Editar**  para editar/personalizar o Power Automate fluxo.

   2. Selecione **(Escopo) Sincronizando Indicações.**

   3. Para personalizar mapeamentos de campo crm (com base no guia de mapeamentos de campo) para criar eventos, **selecione Criar Referência da Microsoft**.

Você pode editar os mapeamentos nesta seção com base no Guia de Mapeamento de Campo.


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>Sincronização de indicação de venda co-direcional de ponta a ponta

Depois de instalar, configurar e personalizar a solução Power Automate, você poderá testar a sincronização de indicações de venda co-venda entre o Salesforce CRM e Partner Center.

### <a name="pre-requisites"></a>Pré-requisitos

Para sincronizar as indicações entre Partner Center e Salesforce CRM, a solução Power Automate precisa demarcar claramente os campos de indicação específicos da Microsoft. Essa identificação fornece às equipes de vendedores a capacidade de decidir quais indicações eles querem compartilhar com a Microsoft para venda em cooperação.

Um conjunto de campos personalizados está disponível como parte da Partner Center  sincronização de indicações para a entidade de oportunidade da solução Salesforce CRM. Um usuário administrador do CRM precisará criar uma seção crm separada com os **campos personalizados oportunidade.**

Os seguintes campos personalizados devem fazer parte da seção CRM:

- **Sincronizar com Partner Center:** se a oportunidade deve ser sincronizada com o Microsoft Partner Center

- **Identificador de Indicação:** um campo de identificador somente leitura para a indicação Partner Center Microsoft

- **Link de** indicação: um link somente leitura para a indicação no Microsoft Partner Center

- **Como a Microsoft pode ajudar:** Ajuda necessária da Microsoft para a indicação

- **Produtos**: lista de produtos associados a essa oportunidade

- **Auditoria:** uma trilha de auditoria somente leitura para sincronização com Partner Center indicações

### <a name="scenarios"></a>Cenários:

1. Sincronização de indicação quando a indicação é criada ou atualizada no CRM e sincronizada Partner Center:

   1. Entre em seu ambiente do Salesforce CRM com o usuário que tenha visibilidade na **seção Oportunidade** do CRM.

   2. Verifique se a seção a seguir está presente quando você cria uma "Nova Oportunidade" no ambiente do Salesforce CRM

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Ambiente do Salesforce.":::

   3. Para sincronizar essa oportunidade com o Microsoft Partner Center, certifique-se de definir os seguintes campos na exibição de cartão:

       - "Sincronizar com Partner Center": Sim
       - "Como a Microsoft pode ajudar?": selecione uma das seguintes opções:
       - Produtos: IDs de solução do produto

   4. Depois de definir a opção  **Sincronizar** com Partner Center oportunidade como **Sim,** aguarde 10 minutos, entre em sua conta Partner Center. Suas indicações serão sincronizadas com o Salesforce CRM.

   5. Quando a opção "Sincronizar com Partner Center" estiver definida como "Sim", se você atualizar a oportunidade no Salesforce CRM, as alterações serão sincronizadas com sua Partner Center cliente.

   6. As oportunidades sincronizadas com êxito com Partner Center serão identificadas com ✔icon no Salesforce CRM.

2. Sincronização de indicação quando a indicação é criada ou atualizada no Microsoft Partner Center sincronizada no ambiente salesforce CRM:

    1. Entre em seu painel Partner Center [.](https://partner.microsoft.com/dashboard/home)

    2. Selecione **Indicações** no menu à esquerda.

    3. Crie uma nova indicação de venda de Partner Center clicando na opção "Nova oferta".

    4. Entre em seu ambiente do Salesforce CRM.

    5. Navegue até **Abrir Oportunidades**. A indicação criada no Microsoft Partner Center agora está sincronizada no Salesforce CRM.

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Tela de oportunidade do Salesforce.":::

    6. Quando você seleciona uma indicação sincronizada, os detalhes da exibição de cartão são preenchidos.

## <a name="next-steps"></a>Próximas etapas

- [Gerenciar clientes potenciais](manage-leads.md)

- [Gerenciar oportunidades de venda conjunta](manage-co-sell-opportunities.md)

- [Webhooks do Partner Center](/partner-center/develop/partner-center-webhooks)
