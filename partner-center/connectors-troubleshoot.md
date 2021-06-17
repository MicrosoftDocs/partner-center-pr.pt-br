---
title: Solucionar problemas de conectores de referências de venda conjunta
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba respostas para perguntas comuns sobre como usar conectores de venda em comum. Leia essas perguntas frequentes sobre como solucionar problemas de conectores de venda em cooperação.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: bb7a227624c548a29046b80d3bd5fa363a4aee2f
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276919"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a>Solucionar problemas de conectores de referências de venda conjunta

**Aplica-se a**: Dynamics 365 CRM | Salesforce CRM

**Funções apropriadas:** indicações de administrador | Administrador do sistema ou personalizador de sistema no CRM

 ## <a name="questions-and-answers-about-pre-requisites"></a>Perguntas e respostas sobre pré-requisitos

1. Você pode usar uma solução de conectores de indicações de venda co-venda de avaliação para seu ambiente?

Se você estiver no ambiente de teste/preparação, poderá optar pela solução de avaliação. A versão paga dos Conectores está disponível no AppSource por US$ 15/mês. Com a conexão paga, você receberá chamadas à API de 10 mil por dia. Os Conectores são wrappers sobre as APIs Partner Center referência. Sempre que as soluções  de conector são executados para um evento Criar ou Atualizar nas oportunidades no lado Partner Center crm, uma chamada à API é feita. 

2. Qual função você precisa para criar seções no ambiente crm?

Os usuários que são administradores do sistema ou personalizadores do sistema podem aplicar alterações a todos. No entanto, todos os usuários do aplicativo podem personalizar o sistema e até mesmo compartilhar algumas de suas personalizações com outras pessoas. 

3. Os vendedores parceiros precisam de funções especiais para trabalhar Partner Center?
 
Os vendedores parceiros devem ser atribuídos à função "Administrador de indicações". Para obter mais informações, consulte [Visão geral de permissões.](create-user-accounts-and-set-permissions.md)

4. Quais campos precisam ser definidos primeiro em seu ambiente crm? 

• Verifique se a moeda é apropriada para sua localização e se está em seu ambiente crm com precisão. • Sua equipe de vendas deve estar listada em seu ambiente de CRM como usuários do CRM.

5. Quais pré-requisitos são necessários para a criação Power Automate ambiente?

Para usar o Power Automate, você precisa:

- Uma Power Automate é necessária.
- Um mínimo de 1 GB de armazenamento é necessário.

6.  Você precisa de uma assinatura do Dynamics 365 para usar a solução Conectores do Salesforce?

A solução conector do Salesforce é do tipo "Dynamics Flow" que dá suporte à sincronização com outros sistemas CRM. A solução não exige que você tenha uma instância do Dynamics 365 ou uma assinatura. Durante a instalação da solução Salesforce, uma lista listada com o ambiente CDS existente em sua empresa pode aparecer. Você precisa selecionar esse ambiente. Além disso, se você receber o erro "Não foi possível encontrar uma organização do Dynamics 365 conectada ao usuário conectado", será necessário criar um novo ambiente para o conector.

## <a name="questions-and-answers-about-configuration"></a>Perguntas e respostas sobre a configuração

1. O que você deve fazer se enfrentar o seguinte erro ao ativar fluxos no Power Automate Platform?

Erro: a solicitação para Azure Resource Manager falhou com o erro: '{"error":{"code":"WorkflowTriggerNotFound","message":"O fluxo de trabalho 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' não pôde ser encontrado."}}'. 

Siga estas etapas de solução de problemas:

- Exclua a conexão CDS e recrie as conexões CDS.
- Ativar e desativar o fluxo filho 
- Exclua a solução e reinstale a solução. 

2.  O que você deve fazer se enfrentar o erro "Entrar" ao adicionar um conector Partner Center na Power Automate Platform?

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Mensagem de erro que exige a login.":::

Siga esta etapa de solução de problemas:

- Use suas Partner Center de usuário para entrar no ambiente de fluxo uma vez (flow.microsoft.com).


3. O que você deve fazer se receber o erro a seguir ao ativar o fluxo Partner Center crm no Power Automate Platform?
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Mensagem de erro que exige atualizações.":::

Siga estas etapas de solução de problemas:

- Primeiro, ative os dois fluxos filho a seguir antes de ativar a Partner Center para o fluxo crm.
      - Partner Center CRM – Auxiliar (Visualização do Insider)
      - Partner Center atualizações de indicação de venda co-venda da Microsoft para CRM (Visualização do Insider)

4. O que você deve fazer quando não é possível adicionar conexões ao fluxo ao tentar editar o fluxo?

Você adiciona conexões ao fluxo enquanto o fluxo está em execução e adiciona a cada fluxo separadamente.  Se a caixa de diálogo para adicionar conexões não for aberta automaticamente durante a edição do fluxo, você poderá editar cada uma das etapas e sub etapas dos fluxos individualmente.

- Selecione cada fluxo e edite-os individualmente.
- Expanda todas as etapas no fluxo 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Etapas que precisam de conexões.":::

- Selecione as etapas em que você vê um ícone de aviso solicitando a associação de conexões e adicione conexões. 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Edite o fluxo passo a passo.":::


5. O que você deve fazer se os fluxos da solução Conectores de Indicações de Venda Co-venda não ativarem?

a. Em Power Automate, você precisará editar fluxos na seguinte ordem e atualizá-los para usar as conexões corretas:

- Partner Center de webhook (visualização do insider)
- Criar indicação de venda co-venda – Salesforce para Partner Center (Visualização do Insider)
- Partner Center atualizações de indicação de venda co-venda da Microsoft para o Salesforce (Visualização do Insider)
- Partner Center ao Salesforce (Visualização do Insider)
- Salesforce para Partner Center (Insider Preview)
- Salesforce Opportunity to Partner Center (Insider Preview)
- Salesforce Microsoft Solutions to Partner Center (Insider Preview)

 B. Para cada fluxo, selecione a **opção Executar somente usuários.** Selecione **Usar conexão** em vez de Fornecido pelo usuário somente de **run.**  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Para ativar um fluxo.":::


C. Ative estes fluxos mencionados abaixo:

 - Partner Center atualizações de indicação de venda co-venda da Microsoft para o Salesforce (Visualização do Insider)

- Salesforce para Partner Center (Insider Preview)

    
D. Ative todos os fluxos restantes.

E. No fluxo Partner Center Registro de Webhook, selecione **Executar**. Forneça a **URL http** da primeira ação no Partner Center ao fluxo **do Salesforce.** Select all quatro opções em **Eventos para registrar** e selecionar **sim** para Substituir.

## <a name="questions-and-answers-about-runmaintenance"></a>Perguntas e respostas sobre a manutenção/a manutenção

1. Como solucionar problemas de falhas durante a execução Power Automate fluxo?

Para garantir que seus fluxos de Power Automate executados conforme o esperado e solucionar falhas durante a execução, consulte Corrigir falhas [de fluxo.](/power-automate/fix-flow-failures)

2. O que você deve fazer se vir indicações que não estão sincronizadas corretamente no Partner Center ou ambiente crm?
 
Para determinar o status da sincronização de indicação, selecione **Auditar**. 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Como sincronizar indicações.":::

Verifique se as seguintes condições foram atendidas:

- A ID da solução é fornecida como parte da oportunidade.

- O código de país de duas letras é necessário.

- Quando a ajuda da Microsoft é selecionada para a oportunidade, as informações de contato do cliente são necessárias.

3. Como garantir que uma indicação seja sincronizada de forma bi-direcional?

Execute as seguintes etapas:

- Os vendedores parceiros precisam garantir que tenham habilitado a opção Sincronizar **com Partner Center** na seção CRM.

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Verifique se você habilitar o Synch.":::

- Os vendedores precisam fornecer a receita e a data de fechamento ao qualificar um lead.

- Se a ID do  CRM  for fornecida no estágio de criação ou atualização da oportunidade de venda co-venda, mas uma oportunidade de venda futura com essa ID não for encontrada no CRM, a atualização ou a criação será ignorada.

- Verifique se o campo moeda de indicação está configurado no ambiente do Salesforce. 

4. O que você deve fazer se o conector for desconectado e você perder uma sincronização de indicação.?

A seguir estão algumas das opções que você pode experimentar:

- Verifique se o nome de usuário ou a senha expirou para o Partner Center usuário com funções de administrador de indicação.

- Você pode ir para a oportunidade não sincronizada, fazer uma atualização secundária e observar se a indicação foi sincronizada.

- Se os fluxos foram executados e falharam, selecione o fluxo e envie a sequência que falhou.

5. O que você deve fazer quando recebe erros de acesso negado?

Certifique-se de que as funções apropriadas existam

- Função administrador de indicação para Partner Center vendedor 
 
- Função administrador do sistema ou personalizador do sistema em sua instância do CRM

- Verifique se o usuário Power Automate conta de fluxo de dados faz logo no https://flow.microsoft.com pelo menos uma vez com antecedência

6. Se você vir que **o código do país** da conta do cliente está ausente durante a criação de uma oportunidade de venda de venda, o que você deve fazer?

Você precisará adicionar o código do país ISO de duas letras à conta do cliente no CRM.

7. O que você deve fazer se vir o erro de que a **ID da Solução é necessária** durante a criação de uma oportunidade de venda co-venda?

Para criar uma indicação de venda em cooperação, você precisa de uma solução pronta para venda em cooperação da Microsoft. 

8. O que você deve fazer quando vir oportunidades de venda de Partner Center criadas no Partner Center que não estão sincronizadas com o CRM, mesmo que não haja erros de fluxo?

Faça o seguinte:

- Depois de criar uma nova oferta de venda em Partner Center, verifique se Partner Center para o fluxo do Dynamics 365 é invocado (ele pode ser invocado várias vezes).

- Se o fluxo for invocado, verifique todos os fluxos invocados e identifique a run de fluxo que atualizaria o CRM. Você pode seguir as ações e verificar se ele atualiza o CRM ou se encontrou um problema.

- Verifique **Nova oferta** no Partner Center para ver se ela é preenchida com a ID do CRM.

- Certifique-se de que o negócio não foi fechado acidentalmente **como Won** ou **Lost** no Partner Center.

## <a name="next-steps"></a>Próximas etapas

- [Gerenciar clientes potenciais](manage-leads.md)
 
- [Gerenciar oportunidades de venda conjunta](manage-co-sell-opportunities.md)
