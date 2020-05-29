---
title: Usar WebHooks para obter eventos de alteração de recurso
ms.topic: article
ms.date: 05/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Usar as APIs de webhook para descobrir quando as alterações de recursos de referências ocorrem
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: referências, API de webhook, eventos de alteração de recursos
ms.localizationpriority: medium
ms.openlocfilehash: 4e1eb2e9bd8ceb4f8c4bf43684305504c8594e5c
ms.sourcegitcommit: c13723216761e60d2b37596efc71f5fdecb30be1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/28/2020
ms.locfileid: "84145080"
---
# <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Usar APIs de webhook para registrar eventos de alteração de recurso

### <a name="appropriate-roles"></a>Funções apropriadas

- Administrador de indicações
- Administrador do sistema ou personalizador do sistema para Dynamics 365 CRM ou Salesforce CRM


As APIs de webhook do Partner Center permitem que você se registre em eventos de alteração de recursos. Esses eventos de alteração são enviados para a URL como postagens HTTP.

>[!NOTE]
>Este tópico explica as APIs de webhook para o Dynamics 365 CRM e o Salesforce CRM.

1. Para registrar sua URL, selecione o **registro do webhook do Partner Center (insider Preview)** fluxo automatizado de energia.

2. Adicionar conexões para (a) Usuário do Partner Center com as referências credenciais de administrador (b.) Eventos do Partner Center conforme realçado abaixo

![Gatilho](images/cosellconnectors/triggerflow.png)

3. Ao fazer essas atualizações, você verá

![Webhooks](images/cosellconnectors/webhook1.png)

4. Salve as alterações e selecione **Ativar**. 

Para permitir que os WebHooks do Partner Center escutem as alterações de evento nos objetos de referência de covenda/independente de IP no Partner Center e em sistemas de CRM, execute as seguintes etapas:

5. Selecione **Partner Center para Dynamics 365 (insider Preview)** ou **Partner Center para Salesforce (insider Preview)**.

6. Selecione o ícone **Editar** e selecione **quando uma solicitação HTTP é recebida**.

7. Selecione o ícone de **cópia** para copiar a URL de postagem http fornecida.

![Copiar URL](images/cosellconnectors/copyurl.png)

8. Agora, selecione o fluxo "registro do webhook do Partner Center (insider Preview)" automatizar fluxos de energia e selecione **executar**.

9. Verifique se a janela "executar fluxo" é aberta no painel direito e clique em **continuar**.

10. Insira os seguintes detalhes: 

    a. **Ponto de extremidade de gatilho http**: URL copiada da etapa anterior

    b. **Eventos a serem registrados**: "referência criada" e "referência atualizada"

    c. **Substituir pontos de extremidade de gatilho existentes, se presente**: Sim (isso substitui todos os pontos de extremidade existentes.)

O webhook agora pode escutar alterações (criar e atualizar eventos). 

11. Selecione **executar** e, em seguida, selecione **concluído.**

 ## <a name="customize-synchronization-steps"></a>Personalizar etapas de sincronização

Quando as referências de venda cruzada são sincronizadas entre o Partner Center e o sistema CRM, os campos sincronizados no PC do Partner Center são listados aqui.

Geralmente, os sistemas CRM são altamente personalizados. Você pode personalizar os fluxos de energia automatizada. Siga o guia de mapeamento de campo e, se necessário, faça as alterações apropriadas nas etapas de fluxos de energia automatizar.  Os mapeamentos do Microsoft Partner Center para CRM são fornecidos, mas com base no seu ambiente de CRM, você pode optar por personalizar ainda mais os campos.

Várias etapas de cada um dos fluxos de energia automatizada podem ser personalizadas com base em suas necessidades. Veja a seguir exemplos de personalizações disponíveis:

1. Para personalizar os campos de criação ou atualização de eventos no Partner Center para a sincronização de referência do CRM: 

    a. Selecione Partner Center para Dynamics 365 (insider Preview) ou Partner Center para Salesforce (insider Preview).

    b. Selecione **Editar** para editar/personalizar o fluxo de automatização de energia.

    c. Selecione **(escopo) sincronizar o cliente potencial ou a oportunidade**.

2. Para personalizar mapeamentos de campo de CRM (com base no guia mapeamentos de campo) para criar eventos, selecione **se for nova oportunidade compartilhada e, em seguida,**. Selecione a subetapa **se sim** e, em seguida, expanda **criando uma nova oportunidade no CRM**. Você pode editar os mapeamentos nesta seção usando o guia de mapeamento de campos.

    d. Para personalizar os mapeamentos de campo do CRM (com base no guia mapeamentos de campo) para eventos de atualização, clique na etapa "(escopo) sincronizar o cliente potencial ou a oportunidade".

    e. Selecione **se for uma atualização para uma oportunidade e, em seguida,**. Selecione a subetapa **se sim** e, em seguida, expanda **se a diferença entre os objetos de oportunidade no Partner Center e no CRM, em seguida**.  

    f. Selecione **se sim** seguido de **Atualizar oportunidade existente**
       
3. Para personalizar os campos de sincronização de referência do CRM para PC para eventos de atualização:

    a. Selecione **Editar** para editar/personalizar o fluxo de automatização de energia.

    b. Selecione **(escopo) sincronizar a oportunidade**.

    c. Para personalizar os mapeamentos de campo do CRM (com base no guia mapeamentos de campo) para eventos de atualização, selecione **se houver diferença entre os objetos Lead no Partner Center e CRM, em seguida**. 

    d. Selecione a subetapa **se sim** e, em seguida, expanda a etapa **atualizar uma referência com dados de oportunidade**.

Você pode editar os mapeamentos nesta seção com base no guia de mapeamento de campos.

4. Para personalizar os campos para a sincronização de referência do CRM para PC para criar eventos?

   a. Selecione **Editar** para editar/personalizar o fluxo de automatização de energia.

   b. Selecione **(escopo) sincronizando referências.**

   c. Para personalizar mapeamentos de campo de CRM (com base no guia mapeamentos de campo) para criar eventos, selecione **criar referência da Microsoft**. 

Você pode editar os mapeamentos nesta seção com base no guia de mapeamento de campos.

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>Sincronização de referência de cooperação bidirecional de ponta a ponta

Depois de instalar, configurar e personalizar a solução de automatização de energia, você pode testar a sincronização de referências de venda entre o Dynamics 365 ou o Salesforce e o Partner Center.

### <a name="pre-requisites"></a>Pré-requisitos

Para sincronizar as referências no Partner Center e no Dynamics 365 CRM ou no Partner Center e no Salesforce CRM, a solução de automatização de energia precisa demarcar claramente os campos de referência específicos da Microsoft. Isso fornece às suas equipes do vendedor a capacidade de decidir quais referências eles desejam compartilhar com a Microsoft para fazer a venda.

Um conjunto de campos personalizados está disponível como parte da sincronização de referências do Partner Center para a entidade **oportunidade** de solução do Dynamics 365. Um usuário administrador de CRM precisará criar uma seção de CRM separada com os campos personalizados de **oportunidade** .

Os campos personalizados a seguir devem fazer parte da seção CRM:

- **Sincronizar com o Partner Center**: se deseja sincronizar a oportunidade com o Microsoft Partner Center

- **Identificador de referência**: um campo de identificador somente leitura para a referência do Microsoft Partner Center

- **Link de referência**: um link somente leitura para a referência no Microsoft Partner Center

- **Como a Microsoft pode ajudar?**: ajuda necessária da Microsoft para a referência

- **Produtos**: lista de produtos associados a esta oportunidade

- **Auditoria**: uma trilha de auditoria somente leitura para sincronização com as referências do Partner Center

### <a name="scenarios"></a>EXEMPLOS

1. Sincronização de referência quando a referência é criada ou atualizada no CRM e sincronizada no Partner Center:

    a. Entre no ambiente do Dynamics 365 CRM com o usuário que tem visibilidade na seção **oportunidade** do CRM.

    b. Verifique se a seção a seguir está presente quando você cria uma "nova oportunidade" no ambiente do Dynamics 365

   ![Oportunidade](images/cosellconnectors/opportunity.png)

    c. Para sincronizar essa oportunidade com o Microsoft Partner Center, certifique-se de definir os seguintes campos no modo de exibição de cartão:

    - "Sincronizar com o Partner Center": Sim

    - "Como a Microsoft pode ajudar?": selecione uma das seguintes opções:

    ![Seleções de ajuda](images/cosellconnectors/help.png)

    - Produtos: IDs de solução do produto

    d. Depois que a oportunidade for criada no Dynamics 365 com a opção **sincronizar com o Partner Center** definida como **Sim**, aguarde 10 minutos, entre em sua conta do Partner Center. Suas referências serão sincronizadas com o Dynamics 365.

    e. Consequentemente, para uma oportunidade que tenha a opção "sincronizar com o Partner Center" definida como "Sim", se você atualizar a oportunidade no Dynamics 365 CRM, as alterações serão sincronizadas em sua conta do Partner Center.

    f. As oportunidades sincronizadas com êxito com o Partner Center serão identificadas com ✔ ícone no Dynamics 365.

2. Sincronização de referência quando a referência é criada ou atualizada no Microsoft Partner Center e sincronizada no ambiente do Dynamics 365: 

    a. Entre no [painel](https://partner.microsoft.com/dashboard/home)do Partner Center.

    b. Selecione **referências** no menu à esquerda.

    c. Crie uma nova referência de revenda do Partner Center clicando na opção "novo negócio".

    d. Entre no ambiente do Dynamics 365 CRM. 

    e. Navegue até **oportunidades abertas**. A referência criada no Microsoft Partner Center agora está sincronizada no Dynamics 365 CRM.

    f. Quando você seleciona uma referência sincronizada, os detalhes da exibição do cartão são preenchidos.

 ### <a name="next-steps"></a>Próximas etapas

- [Mais informações sobre a plataforma de automatização de energia da Microsoft?](https://docs.microsoft.com/power-automate/)

- [Eventos de webhook do Partner Center](https://docs.microsoft.com/partner-center/develop/partner-center-webhook-events)

- [Gerenciar clientes potenciais](manage-leads.md)

- [Gerenciar oportunidades de venda conjunta](manage-co-sell-opportunities.md)
