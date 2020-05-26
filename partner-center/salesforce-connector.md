---
title: O conector de televenda para o centro de parceiros do Salesforce CRM
ms.topic: article
ms.date: 05/22/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Usando o conector CRM do Salesforce, obtenha referências da Microsoft
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: ''
ms.localizationpriority: medium
ms.openlocfilehash: ad39bdde92611066d0dd0c56d8b9133f4d9dcaa9
ms.sourcegitcommit: 97f1ff7386562cbb945bdfbcf15c85bc8303cac2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2020
ms.locfileid: "83825693"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Conector de venda conjunta para o Salesforce CRM-visão geral

### <a name="appropriate-roles"></a>Funções apropriadas

- Administrador de indicações
- Administrador do sistema ou personalizador do sistema no CRM

O conector de televenda do Partner Center permite que seus vendedores covendam-se com a Microsoft de dentro de seus sistemas de CRM. Eles não precisarão ser treinados para usar o Partner Center para gerenciar acordos de venda. Usando os conectores de televenda, você poderá criar uma nova referência de cooperação para envolver um vendedor da Microsoft, receber referências do vendedor da Microsoft, aceitar/recusar referências, modificar dados de negociações, como valor de negócio, data de fechamento, etc., além de receber quaisquer atualizações dos vendedores da Microsoft nessas negociações de venda. Você pode fazer tudo isso enquanto trabalha no CRM de sua escolha, em vez de no Partner Center. 

A solução baseia-se na solução de automatização de energia da Microsoft e usa as APIs do Microsoft Partner Center.


## <a name="before-you-install---pre-requisites"></a>Antes de instalar-pré-requisitos

|**Tópicos**   |**Detalhes**   |**Links**   |
|--------------|--------------------|------|
|ID de Microsoft Partner Network |Você precisa de uma ID de MPN válida|Para ingressar no [MPN](https://partner.microsoft.com/)|
|Co-venda pronta|Sua solução de IP/serviços deve estar pronta para venda.|[Venda com a Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Conta do Partner Center|A ID de MPN associada ao locatário do Partner Center deve ser a mesma que a ID do MPN associada à sua solução de venda conjunta. Verifique se você pode ver suas referências de venda conjunta no portal do Partner Center antes de implantar os conectores.|[Gerenciar sua conta](create-user-accounts-and-set-permissions.md)|
|Funções de usuário da Central de parceiros|O funcionário que irá instalar e usar os conectores deve ser um administrador de referências|[Atribuir permissões e funções de usuários](create-user-accounts-and-set-permissions.md)|
|CRM do Salesforce|A função de usuário CRM é administrador do sistema ou personalizador do sistema|[Atribuir funções no Dynamics 365](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Conta de fluxo de automatização de energia|Uma conta de [energia ativa automatizada](https://flow.microsoft.com) para o administrador do sistema do CRM ou o personalizador do sistema. Esse usuário deve entrar no [Power Automate](https://flow.microsoft.com) pelo menos uma vez antes da instalação.|

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>Instalar a sincronização de referências do Partner Center para o Salesforce CRM

1. Vá para [energia automatizada](https://flow.microsoft.com) e selecione **ambientes** no canto superior direito. Isso mostrará as instâncias do CRM disponíveis.

2. Selecione a instância apropriada do CRM na lista suspensa no canto superior direito. 

3. Selecione **soluções** na barra de navegação à esquerda.

4. Clique no link **abrir AppSource** no menu superior.

![Abrir AppSource](images/cosellconnectors/openappsource.png)

5. Procure **conectores de referências do Partner Center para Salesforce** na tela pop-up.  

6. Clique no botão **obter agora** e em **continuar**. 

7. Isso abre a página onde você pode selecionar o ambiente CRM (Dynamics 365) para instalar o aplicativo.  Concorde com os termos e condições. 

8. Em seguida, você será direcionado para a página **gerenciar suas soluções** .  Navegue até "referências do Partner Center" usando os botões de seta na parte inferior da página. A **instalação agendada** deve aparecer ao lado da solução de referências do Partner Center. A instalação levará 10-15 minutos. 

9. Quando a instalação for concluída, navegue de volta para [Power Automate](https://flow.microsoft.com) e selecione **soluções** na área de navegação à esquerda. Observe que a **sincronização de referências do Partner Center para o Salesforce** está disponível na lista de soluções.

10. Selecione **sincronização de referências do Partner Center para o Dynamics 365**. Os fluxos e as entidades automatizados de energia a seguir estão disponíveis:

![CRMS disponíveis](images/cosellconnectors/dynamics-available-crms.png)

## <a name="best-practice-test-before-you-go-live"></a>Prática recomendada: teste antes de entrar no ar

Antes de instalar, configurar e personalizar a solução de automatização de energia no ambiente de produção, certifique-se de testar a solução em uma instância de CRM de preparo.

- Instale a solução de automatização de energia da Microsoft em uma instância de ambiente de preparo/CRM.
- Faça uma cópia da solução e realize suas configurações e automatize as personalizações de fluxo no ambiente de preparo.
- Teste a solução em uma instância de preparo/CRM. 
- Em caso de sucesso, importe como solução gerenciada para a instância de produção. 

## <a name="configure-the-solution"></a>Configurar a solução

1. Depois de instalar a solução em sua instância do CRM, navegue de volta para o [Power Automate](https://flow.microsoft.com/).

2. Na lista suspensa **ambientes** no canto superior direito, selecione a instância de CRM na qual você instalou a solução de automatização de energia.

3. Será necessário criar conexões que associem as três contas de usuário: 

- Usuário do Partner Center com credenciais de administrador de referências 
- Eventos do Partner Center
- Administrador de CRM com os fluxos de energia automatizada na solução. 

    a. Selecione **conexões** na barra de navegação à esquerda e selecione a solução "referências do Partner Center" na lista.
    b. Crie uma conexão clicando em **criar uma conexão**. 

    ![Criar conexão](images/cosellconnectors/createconnection.png)

    c. Procure por **referências do Partner Center (versão prévia)** na barra de pesquisa no canto superior direito.
    d. Crie uma conexão para o usuário do Partner Center com a função de credenciais do administrador de referências. Oriental. Em seguida, crie uma conexão de eventos do Partner Center para o usuário do Partner Center com as credenciais do administrador de referências. fixo. Crie uma conexão para Common Data Service (ambiente atual) para o usuário administrador do CRM.

4. Para associar os fluxos de energia automatizada com as conexões, edite cada um dos fluxos de energia automatizada para se conectar às referências do Common Data Service e do Partner Center. Salve as alterações.

5. **Ative** os fluxos de energia automatizada.

## <a name="next-steps"></a>Próximas etapas

- [Usar WebHooks para obter eventos de alteração de recurso](referral-connector-webhooks.md)

- [Mais informações sobre a plataforma de automatização de energia da Microsoft?](https://docs.microsoft.com/power-automate/)

- [Gerenciar clientes potenciais](manage-leads.md)

- [Gerenciar oportunidades de venda conjunta](manage-co-sell-opportunities.md)
