---
title: Solucionar problemas de conectores de referências de venda conjunta
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba mais sobre as respostas a perguntas comuns sobre como usar conectores de venda conjunta. Leia estas perguntas frequentes sobre como solucionar problemas de conectores de televenda.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 988a696a8a0a0abb4d37e3915c76f905ec5b35b0
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "92031259"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a>Solucionar problemas de conectores de referências de venda conjunta

**Aplica-se a:**

- Partner Center
- CRM do Dynamics 365
- CRM do Salesforce

**Funções apropriadas**

- Administrador de indicações
- Administrador do sistema ou personalizador do sistema no CRM

 ## <a name="questions-and-answers-about-pre-requisites"></a>Perguntas e respostas sobre os pré-requisitos

1. É possível usar uma solução de avaliação de conectores de indicações para o seu ambiente?

Se você estiver no ambiente de teste/preparo, poderá optar pela solução de avaliação. A versão paga dos conectores está disponível em AppSource a US $15/mês. Com a conexão paga, você receberá chamadas de API de 10K por dia. Os conectores são wrappers sobre as APIs de referência do Partner Center. Sempre que as soluções de conector são executadas para um evento de **criação** ou **atualização** nas oportunidades no lado do parceiro ou do CRM, é feita uma chamada à API.

2. Que função você precisa para criar seções no ambiente CRM?

Os usuários que são administradores de sistema ou personalizadores de sistema podem aplicar alterações para todos. No entanto, todos os usuários do aplicativo podem personalizar o sistema e até compartilhar algumas de suas personalizações com outras pessoas. 

3. Os vendedores de parceiros precisam de funções especiais para trabalhar no Partner Center?
 
Os vendedores do parceiro devem ser atribuídos à função "administrador de referências". Para obter mais informações, consulte o seguinte [Visão geral de permissões) (Create-User-Accounts-and-Set-Permissions).

4. Quais campos precisam ser configurados primeiro em seu ambiente de CRM? 

• Verifique se sua moeda é apropriada para seu local e se está em seu ambiente CRM com precisão. • Sua equipe de vendas deve estar listada em seu ambiente de CRM como usuários do CRM.

5. Quais pré-requisitos são necessários para a criação do ambiente de automatização de energia?

Para usar o ambiente de automatização de energia, você precisa:

- Uma licença de automatização de energia é necessária.
- É necessário um mínimo de armazenamento de 1 GB.

6.  Você precisa de uma assinatura do Dynamics 365 para usar a solução de conectores do Salesforce?

A solução do conector do Salesforce é do tipo "fluxo do Dynamics" que dá suporte à sincronização com outros sistemas de CRM. A solução não exige que você tenha uma instância ou assinatura do Dynamics 365. Ao instalar a solução Salesforce, uma lista suspensa com um ambiente de CDS existente em sua empresa pode ser exibida. Você precisa selecionar esse ambiente. Além disso, se você receber o erro "não foi possível encontrar uma organização do Dynamics 365 conectada ao usuário conectado", será necessário criar um novo ambiente para o conector.

## <a name="questions-and-answers-about-configuration"></a>Perguntas e respostas sobre a configuração

1. O que você deve fazer se enfrentar o seguinte erro ao ativar fluxos na plataforma Power Automate?

Erro: a solicitação para Azure Resource Manager falhou com o erro: ' {"erro": {"código": "WorkflowTriggerNotFound", "Message": "não foi possível encontrar o gatilho ' manual ' do fluxo de trabalho ' e14d00f1-1fdf-4b1b-AAAC-54a5064093d3 '."}} '. 

Siga estas etapas de solução de problemas:

- Exclua a conexão de CDS e recrie as conexões de CDS.
- Desativar e ativar o fluxo filho 
- Exclua a solução e reinstale a solução. 

2.  O que você deve fazer se enfrentar o erro "entrar" ao adicionar um conector do Partner Center na plataforma Power Automate?

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Mensagem de erro que requer entrada":::

Siga esta etapa de solução de problemas:

- Use suas credenciais do Partner Center para entrar no ambiente de fluxo uma vez (flow.microsoft.com).


3. O que você deve fazer se receber o seguinte erro ao ativar o Partner Center para o fluxo do CRM na plataforma de energia automatizada?
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Mensagem de erro que requer entrada":::

Siga estas etapas de solução de problemas:

- Ative primeiro os dois fluxos filho a seguir antes de ativar o Partner Center para o fluxo do CRM.
      - Partner Center para CRM-Helper (insider Preview)
      - Partner Center Microsoft co-vender atualizações de referência para CRM (insider Preview)

4. O que você deve fazer quando não é possível adicionar conexões ao fluxo ao tentar editar o fluxo?

Você adiciona conexões ao fluxo enquanto o fluxo está em execução e adiciona a cada fluxo separadamente.  Se a caixa de diálogo para adicionar conexões não abrir automaticamente ao editar o fluxo, você poderá editar cada uma das etapas e as subetapas dos fluxos individualmente.

- Selecione cada fluxo e edite-os individualmente.
- Expandir todas as etapas no fluxo 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Mensagem de erro que requer entrada":::

- Selecione as etapas em que você verá um ícone de aviso solicitando a associação de conexões e adicionar conexões. 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Mensagem de erro que requer entrada":::


5. O que você deve fazer se os fluxos da solução covenda de conectores de referências não estiverem ativados?

a. Na energia automatizada, você precisará editar os fluxos na seguinte ordem e atualizá-los para usar as conexões corretas:

- Registro do webhook do Partner Center (insider Preview)
- Criar referência de co-venda-Salesforce para o Partner Center (insider Preview)
- Partner Center Microsoft co-vender atualizações de referência para o Salesforce (insider Preview)
- Partner Center para Salesforce (insider Preview)
- Salesforce para o Partner Center (insider Preview)
- Oportunidade do Salesforce para o Partner Center (insider Preview)
- Salesforce Microsoft Solutions para Partner Center (insider Preview)

 B. Para cada fluxo, selecione a opção **executar somente usuários** . Selecione **usar conexão** em vez de **fornecido pelo usuário somente execução**.  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Mensagem de erro que requer entrada":::


C. Ative-os abaixo dos fluxos mencionados:

 - Partner Center Microsoft co-vender atualizações de referência para o Salesforce (insider Preview)

- Salesforce para o Partner Center (insider Preview)

    
D. Ative todos os fluxos restantes.

E. Em registro de webhook do Flow Center de fluxo, selecione **executar**. Forneça a **URL http** da primeira ação no **Partner Center para** o fluxo do Salesforce. Selecione todas as quatro opções em **eventos para registrar** e selecione **Sim** para substituir.

## <a name="questions-and-answers-about-runmaintenance"></a>Perguntas e respostas sobre a execução/manutenção

1. Como solucionar problemas em caso de falhas durante a execução do fluxo de energia automatizada?

Para garantir que seus fluxos de energia automatizada sejam executados conforme esperado e para solucionar falhas durante a execução, consulte [corrigir falhas de fluxo](/power-automate/fix-flow-failures).

2. O que você deve fazer se vir as referências que não estão sincronizadas corretamente no ambiente do Partner Center ou CRM?
 
Para determinar o status da sincronização de referência, selecione **auditoria**. 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Mensagem de erro que requer entrada":::

Certifique-se de que as seguintes condições sejam atendidas:

- A ID da solução é fornecida como parte da oportunidade.

- O código do país de duas letras é necessário.

- Quando a ajuda da Microsoft é selecionada para a oportunidade, as informações de contato do cliente são necessárias.

3. Como garantir que uma referência seja sincronizada bidirecionalmente?

Execute as seguintes etapas:

- Os vendedores do parceiro precisam garantir que tenham habilitado a opção **sincronizar com o Partner Center** na seção CRM.

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Mensagem de erro que requer entrada" no Partner Center.

## <a name="next-steps"></a>Próximas etapas

- [Gerenciar clientes potenciais](manage-leads.md)
 
- [Gerenciar oportunidades de venda conjunta](manage-co-sell-opportunities.md)