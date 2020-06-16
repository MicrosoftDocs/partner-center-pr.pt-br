---
title: O conector de televenda para o centro de parceiros do Salesforce CRM
ms.topic: article
ms.date: 05/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Sincronize suas referências no Partner Center com seu Salesforce CRM
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: ab70766e0bc20b170a1fb9c12a9bea0e6268b06d
ms.sourcegitcommit: c89ddcf8b366f56dc123936cbda2d0001c9f0d8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2020
ms.locfileid: "84788770"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Conector de venda conjunta para o Salesforce CRM – visão geral

### <a name="appropriate-roles"></a>Funções apropriadas

- Administrador de indicações
- Administrador do sistema ou personalizador do sistema no CRM

O conector de televenda do Partner Center permite que seus vendedores covendam-se com a Microsoft de dentro de seus sistemas de CRM. Eles não precisarão ser treinados para usar o Partner Center para gerenciar acordos de venda. Usando os conectores de venda conjunta, você pode criar uma nova referência de covenda para envolver um vendedor da Microsoft, receber referências do vendedor da Microsoft, aceitar/recusar referências, modificar dados de negociações, como valor de negócio e data de fechamento.  Você também pode receber todas as atualizações dos vendedores da Microsoft sobre esses acordos de venda conjunta. Você pode fazer todas as suas referências funcionarem enquanto trabalha no CRM de sua escolha em vez de no Partner Center. 

A solução baseia-se na solução de automatização de energia da Microsoft e usa as APIs do Partner Center.

## <a name="before-you-install---pre-requisites"></a>Antes de instalar-pré-requisitos

|**Tópicos**   |**Detalhes**   |**Links**   |
|--------------|--------------------|------|
|ID de Microsoft Partner Network |Você precisa de uma ID de MPN válida|Para ingressar no [MPN](https://partner.microsoft.com/)|
|Co-venda pronta|Sua solução de IP/serviços deve estar pronta para venda.|[Venda com a Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Conta do Partner Center|A ID de MPN associada ao locatário do Partner Center deve ser a mesma que a ID do MPN associada à sua solução de venda conjunta. Verifique se você pode ver suas referências de venda conjunta no portal do Partner Center antes de implantar os conectores.|[Gerenciar sua conta](create-user-accounts-and-set-permissions.md)|
|Funções de usuário da Central de parceiros|O funcionário que irá instalar e usar os conectores deve ser um administrador de referências|[Atribuir permissões e funções de usuários](create-user-accounts-and-set-permissions.md)|
|CRM do Salesforce|A função de usuário CRM é administrador do sistema ou personalizador do sistema|[Atribuir funções no Salesforce CRM](https://docs.microsoft.com/SalesforceCRM/customerengagement/on-premises/customize/privileges-required-customization)|
|Conta de fluxo de automatização de energia|Uma conta de [energia ativa automatizada](https://flow.microsoft.com) para o administrador do sistema do CRM ou o personalizador do sistema. Esse usuário deve entrar no [Power Automate](https://flow.microsoft.com) pelo menos uma vez antes da instalação.|

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>Instalar a sincronização de referências do Partner Center para o Salesforce CRM

1. Vá para [energia automatizada](https://flow.microsoft.com) e selecione **ambientes** no canto superior direito. Isso mostrará as instâncias do CRM disponíveis.

2. Selecione a instância apropriada do CRM na lista suspensa no canto superior direito.

3. Selecione **soluções** na barra de navegação à esquerda.

4. Clique no link **abrir AppSource** no menu superior.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Abrir AppSource":::

5. Procure **conectores de referências do Partner Center para Salesforce** na tela pop-up.  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. Clique no botão **obter agora** e em **continuar**.

7. Isso abre a página onde você pode selecionar o ambiente do Salesforce CRM para instalar o aplicativo.  Concorde com os termos e condições.

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="CRMS disponíveis":::

8. Em seguida, você será direcionado para a página **gerenciar suas soluções** .  Navegue até "referências do Partner Center" usando os botões de seta na parte inferior da página. A **instalação agendada** deve aparecer ao lado da solução de referências do Partner Center. A instalação levará 10-15 minutos.

9. Quando a instalação for concluída, navegue de volta para [Power Automate](https://flow.microsoft.com) e selecione **soluções** na área de navegação à esquerda. Observe que a **sincronização de referências do Partner Center para o Salesforce** está disponível na lista de soluções.

10. Selecione **sincronização de referências do Partner Center para Salesforce**. Os fluxos e as entidades automatizados de energia a seguir estão disponíveis:

    :::image type="content" source="images/salesforce/salesforce-flows.png" alt-text="Fluxos do Salesforce":::

## <a name="best-practice-test-before-you-go-live"></a>Prática recomendada: teste antes de entrar no ar

Antes de instalar, configurar e personalizar a solução de automatização de energia no ambiente de produção, certifique-se de testar a solução em uma instância de CRM de preparo.

- Instale a solução de automatização de energia da Microsoft em uma instância de ambiente de preparo/CRM.

- Faça uma cópia da solução e execute sua configuração e automatize as personalizações de fluxo no ambiente de preparo.

- Teste a solução em uma instância de preparo/CRM.

- Em caso de sucesso, importe como solução gerenciada para a instância de produção.

## <a name="configure-the-solution"></a>Configurar a solução

1. Depois de instalar a solução em sua instância do CRM, navegue de volta para o [Power Automate](https://flow.microsoft.com/).

2. Na lista suspensa **ambientes** no canto superior direito, selecione a instância de CRM na qual você instalou a solução de automatização de energia.

3. Será necessário criar conexões que associem as três contas de usuário:

   - Usuário do Partner Center com credenciais de administrador de referências
   - Eventos do Partner Center
   - Administrador de CRM com os fluxos de energia automatizada na solução.

   1. Selecione **conexões** na barra de navegação à esquerda e selecione a solução "referências do Partner Center" na lista.

   2. Crie uma conexão clicando em **criar uma conexão**.

       :::image type="content" source="images/cosellconnectors/createconnection.png" alt-text="Criar conexão":::

   3. Procure por **referências do Partner Center (versão prévia)** na barra de pesquisa no canto superior direito.

   4. Crie uma conexão para o usuário do Partner Center com a função de credenciais do administrador de referências.

   5. Em seguida, crie uma conexão de eventos do Partner Center para o usuário do Partner Center com as credenciais do administrador de referências.

   6. Crie uma conexão para Common Data Service (ambiente atual) para o usuário administrador do CRM.

4. Para associar os fluxos de energia automatizada com as conexões, edite cada um dos fluxos de energia automatizada para se conectar às referências do Common Data Service e do Partner Center. Salve as alterações.

5. **Ative** os fluxos de energia automatizada.

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Usar APIs de webhook para registrar eventos de alteração de recurso

As APIs de webhook do Partner Center permitem que você se registre em eventos de alteração de recursos. Esses eventos de alteração são enviados para a URL como postagens HTTP.

1. Para registrar sua URL, selecione o **registro do webhook do Partner Center (insider Preview)** fluxo automatizado de energia.

2. Adicionar conexões para (a) Usuário do Partner Center com as referências credenciais de administrador (b.) Eventos do Partner Center conforme realçado abaixo

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Gatilho":::

3. Ao fazer essas atualizações, você verá

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks":::

4. Salve as alterações e selecione **Ativar**.

   Para habilitar o parceiro do Partner Center a ouvir as alterações de evento, execute as seguintes etapas:

5. Selecione **Partner Center para SALESFORCE CRM (insider Preview)**.

6. Selecione o ícone **Editar** e selecione **quando uma solicitação HTTP é recebida**.

7. Selecione o ícone de **cópia** para copiar a URL de postagem http fornecida.

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Copiar URL":::

8. Agora, selecione o fluxo "registro do webhook do Partner Center (insider Preview)" automatizar fluxos de energia e selecione **executar**.

9. Verifique se a janela "executar fluxo" é aberta no painel direito e clique em **continuar**.

10. Insira os seguintes detalhes:

    1. **Ponto de extremidade de gatilho http**: URL copiada da etapa anterior

    2. **Eventos a serem registrados**: "referência criada" e "referência atualizada"

    3. **Substituir pontos de extremidade de gatilho existentes, se presente**: Sim (isso substitui todos os pontos de extremidade existentes.)

11. Selecione **executar** e, em seguida, selecione **concluído.**

O webhook agora pode escutar criar e atualizar eventos.

## <a name="customize-synchronization-steps"></a>Personalizar etapas de sincronização

Quando as referências de venda cruzada são sincronizadas entre o Partner Center e o sistema CRM, os campos sincronizados no PC do Partner Center são listados aqui.

Geralmente, os sistemas CRM são altamente personalizados. Você pode personalizar os fluxos de energia automatizada. Siga o guia de mapeamento de campo e, se necessário, faça as alterações apropriadas nas etapas de fluxos de energia automatizar.  Os mapeamentos do Microsoft Partner centers para CRM são fornecidos, mas com base no seu ambiente de CRM, você pode optar por personalizar ainda mais os campos.

Várias etapas de cada um dos fluxos de energia automatizada podem ser personalizadas com base em suas necessidades. Veja a seguir exemplos de personalizações disponíveis:

1. Para personalizar os campos de criação ou atualização de eventos no Partner Center para a sincronização de referência do CRM:

   1. Selecione Partner Center para Salesforce CRM (insider Preview).

   2. Selecione **Editar** para editar/personalizar o fluxo de automatização de energia.

   3. Selecione **(escopo) sincronizar o cliente potencial ou a oportunidade**.

2. Para personalizar mapeamentos de campo de CRM para criar eventos, selecione **se for nova oportunidade compartilhada e, em seguida,**. Selecione a subetapa **se sim** e, em seguida, expanda **criando uma nova oportunidade no CRM**. Você pode editar os mapeamentos nesta seção usando o guia de mapeamento de campos.

   1. Para personalizar mapeamentos de campo de CRM para eventos de atualização, clique na etapa "(escopo) sincronizar o cliente potencial ou a oportunidade".

   2. Selecione **se for uma atualização para uma oportunidade e, em seguida,**. Selecione a subetapa **se sim** e, em seguida, expanda **se a diferença entre os objetos de oportunidade no Partner Center e no CRM, em seguida**.  

   3. Selecione **se sim** seguido de **Atualizar oportunidade existente**

3. Para personalizar os campos de sincronização de referência do CRM para PC para eventos de atualização:

   1. Selecione **Editar** para editar/personalizar o fluxo de automatização de energia.

   2. Selecione **(escopo) sincronizar a oportunidade**.

   3. Para personalizar os mapeamentos de campo do CRM (com base no guia mapeamentos de campo) para eventos de atualização, selecione **se houver diferença entre os objetos Lead no Partner Center e CRM, em seguida**.

   4. Selecione a subetapa **se sim** e, em seguida, expanda a etapa **atualizar uma referência com dados de oportunidade**.

   Você pode editar os mapeamentos nesta seção com base no guia de mapeamento de campos.

4. Para personalizar os campos para a sincronização de referência do CRM para PC para criar eventos?

   1. Selecione **Editar** para editar/personalizar o fluxo de automatização de energia.

   2. Selecione **(escopo) sincronizando referências.**

   3. Para personalizar mapeamentos de campo de CRM (com base no guia mapeamentos de campo) para criar eventos, selecione **criar referência da Microsoft**.

Você pode editar os mapeamentos nesta seção com base no guia de mapeamento de campos.

## <a name="create-separate-section-in-salesforce-crm-opportunity-layout"></a>Criar uma seção separada no layout de oportunidade do CRM Salesforce

Para sincronizar as referências no Partner Center e no Salesforce CRM, a solução de automatização de energia precisa demarcar claramente os campos de referência específicos da Microsoft. Isso fornece às suas equipes do vendedor a capacidade de decidir quais referências eles desejam compartilhar com a Microsoft para fazer a venda.

Um conjunto de campos personalizados está disponível como parte da sincronização de referências do Partner Center para a entidade de **oportunidade** do Salesforce CRM. Um usuário administrador de CRM precisará criar uma seção de CRM separada com os campos personalizados de **oportunidade** .
O usuário administrador do Salesforce CRM precisará criar uma seção de CRM separada.

Os campos personalizados a seguir devem fazer parte da seção CRM:

- **Sincronizar com o Partner Center**: se deseja sincronizar a oportunidade com o Microsoft Partner Center

- **Identificador de referência**: um campo de identificador somente leitura para a referência do Microsoft Partner Center

- **Link de referência**: um link somente leitura para a referência no Microsoft Partner Center

- **Como a Microsoft pode ajudar?** Ajuda necessária da Microsoft para a referência

- **Produtos**: lista de produtos associados a esta oportunidade

- **Auditoria**: uma trilha de auditoria somente leitura para sincronização com a referência do Microsoft Partner Center

### <a name="set-up-fields-and-relationships"></a>Configurar campos e relações

1. Entre em sua conta do Salesforce e vá para **oportunidade**.

2. Clique nas opções **Configurar** e **Editar objeto** para adicionar os campos necessários.

3. Selecionar **campos & relações** no painel de navegação esquerdo

   :::image type="content" source="images/salesforce/fields1.png" alt-text="Fields":::

4. Adicione os campos a seguir nos **campos &** tabela de relações:

   |**Rótulo do campo**   |**Nome do campo**|**Data type**|**Indexa**|
   |---------------------|:-------------------|:--------------|:----------------|
   |Audit| Audit__c|Área de texto longo (100.000) (linha visível 4)||
   |Como a Microsoft pode ajudar?|How_can_Microsoft_help_c|Seleção|
   |Produtos|Products_c|texto (255)||
   |Indicação | Referral_Identfier_c|Texto (100) (ID externa)|sim|
   |Link de referência| Referral_Link_c_|URL (255)||
   |Sincronizar com o Partner Center|sync_with_partner_center_c|Caixa de seleção (padrão desmarcado)||

   * Valores da lista de seleção:

   - Proposta de valor específico da carga de trabalho
   - Arquitetura técnica do cliente
   - Prova de conceito ou demonstração
   - Cotações ou licenciamento
   - Sucesso do cliente do post Sales
   - Geral ou outros

5. Os campos serão criados em **campos & relações**

   :::image type="content" source="images/salesforce/fields2.png" alt-text="Campos criados":::

6. No layout da oportunidade, crie uma seção separada com os campos listados acima.

   - Esta seção deve estar disponível para os vendedores no layout da oportunidade

   :::image type="content" source="images/salesforce/pc-fields-layout.png" alt-text="Layout de campos do Partner Center":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>Sincronização de referência de cooperação bidirecional de ponta a ponta

Depois de instalar, configurar e personalizar a solução de automatização de energia, você pode testar a sincronização de referências de venda entre o Salesforce CRM e o Partner Center.

### <a name="pre-requisites"></a>Pré-requisitos

Para sincronizar as referências no Partner Center e no Salesforce CRM, a solução de automatização de energia precisa demarcar claramente os campos de referência específicos da Microsoft. Essa identificação fornece às suas equipes do vendedor a capacidade de decidir quais referências eles desejam compartilhar com a Microsoft para fazer a venda.

Um conjunto de campos personalizados está disponível como parte da sincronização de referências do Partner Center para a entidade **oportunidade** de solução do Salesforce CRM. Um usuário administrador de CRM precisará criar uma seção de CRM separada com os campos personalizados de **oportunidade** .

Os campos personalizados a seguir devem fazer parte da seção CRM:

- **Sincronizar com o Partner Center**: se deseja sincronizar a oportunidade com o Microsoft Partner Center

- **Identificador de referência**: um campo de identificador somente leitura para a referência do Microsoft Partner Center

- **Link de referência**: um link somente leitura para a referência no Microsoft Partner Center

- **Como a Microsoft pode ajudar**: a ajuda necessária da Microsoft para a referência

- **Produtos**: lista de produtos associados a esta oportunidade

- **Auditoria**: uma trilha de auditoria somente leitura para sincronização com as referências do Partner Center

### <a name="scenarios"></a>EXEMPLOS

1. Sincronização de referência quando a referência é criada ou atualizada no CRM e sincronizada no Partner Center:

   1. Entre no ambiente do Salesforce CRM com o usuário que tem visibilidade na seção **oportunidade** do CRM.

   2. Verifique se a seção a seguir está presente quando você cria uma "nova oportunidade" no ambiente CRM do Salesforce

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Ambiente do Salesforce":::

   3. Para sincronizar essa oportunidade com o Microsoft Partner Center, certifique-se de definir os seguintes campos no modo de exibição de cartão:

       - "Sincronizar com o Partner Center": Sim
       - "Como a Microsoft pode ajudar?": selecione uma das seguintes opções:
       - Produtos: IDs de solução do produto

   4. Depois de definir a opção sincronização de oportunidade **com o Partner Center** como **Sim**, aguarde 10 minutos e entre em sua conta do Partner Center. Suas referências serão sincronizadas com o Salesforce CRM.

   5. Quando a opção "sincronizar com o Partner Center" for definida como "Sim", se você atualizar a oportunidade no Salesforce CRM, as alterações serão sincronizadas com sua conta do Partner Center.

   6. As oportunidades sincronizadas com êxito com o Partner Center serão identificadas com ✔ ícone no Salesforce CRM.

2. Sincronização de referência quando a referência é criada ou atualizada no Microsoft Partner Center e sincronizada no ambiente do Salesforce CRM:

    1. Entre no [painel](https://partner.microsoft.com/dashboard/home)do Partner Center.

    2. Selecione **referências** no menu à esquerda.

    3. Crie uma nova referência de revenda do Partner Center clicando na opção "novo negócio".

    4. Entre no ambiente do Salesforce CRM.

    5. Navegue até **oportunidades abertas**. A referência criada no Microsoft Partner Center agora está sincronizada no Salesforce CRM.

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Tela de oportunidade do Salesforce":::

    6. Quando você seleciona uma referência sincronizada, os detalhes da exibição do cartão são preenchidos.

## <a name="next-steps"></a>Próximas etapas

- [Mais informações sobre a plataforma de automatização de energia da Microsoft?](https://docs.microsoft.com/-automate/)

- [Gerenciar clientes potenciais](manage-leads.md)

- [Gerenciar oportunidades de venda conjunta](manage-co-sell-opportunities.md)

- [Webhooks do Partner Center](https://docs.microsoft.com/partner-center/develop/partner-center-webhooks)