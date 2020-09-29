---
title: Solucionar problemas de conectores de referências de venda conjunta
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Perguntas frequentes sobre como solucionar problemas de conectores de televenda.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: d34a13a6789f3bd712d2cec3a594b8e407f7449d
ms.sourcegitcommit: 3329fd120d8d49a4831412b79e044678ec71b84c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/29/2020
ms.locfileid: "91422332"
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

4. Quais são os campos que precisam ser configurados primeiro em seu ambiente de CRM? 

• Verifique se sua moeda é apropriada para seu local e se está em seu ambiente CRM com precisão. • Sua equipe de vendas deve estar listada em seu ambiente de CRM como usuários do CRM.

5.  Quais pré-requisitos são necessários para a criação do ambiente de automatização de energia?

Para usar o ambiente de automatização de energia, você precisa:

- Uma licença de automatização de energia é necessária.
- É necessário um mínimo de armazenamento de 1 GB.

6.  Você precisa de uma assinatura do Dynamics 365 para usar a solução de conectores do Salesforce?

A solução do conector do Salesforce é do tipo "fluxo do Dynamics" que dá suporte à sincronização com outros sistemas de CRM. A solução não exige que você tenha uma instância ou assinatura do Dynamics 365. Ao instalar a solução Salesforce, uma lista suspensa com um ambiente de CDS existente em sua empresa pode ser exibida. Você precisa selecionar esse ambiente. Além disso, se você receber o erro não foi possível encontrar uma organização do Dynamics 365 conectada ao usuário conectado ", será necessário criar um novo ambiente para o conector.

## <a name="questions-and-answers-about-configuration"></a>Perguntas e respostas sobre a configuração

1. O que você deve fazer se enfrentar o seguinte erro ao ativar fluxos na plataforma Power Automate?

Erro: a solicitação para Azure Resource Manager falhou com o erro: ' {"erro": {"código": "WorkflowTriggerNotFound", "Message": "não foi possível encontrar o gatilho ' manual ' do fluxo de trabalho ' e14d00f1-1fdf-4b1b-AAAC-54a5064093d3 '."}} '. 

Siga estas etapas de solução de problemas:

- Exclua a conexão de CDS e recrie as conexões de CDS.
- Desativar e ativar o fluxo filho 
- Exclua a solução e reinstale a solução. 

2.  O que você deve fazer se enfrentar o seguinte erro ao adicionar um conector do Partner Center na plataforma Power Automate?

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Mensagem de erro que requer entrada":::

Siga esta etapa de solução de problemas:

- Use a entrada do Partner Center para entrar no ambiente de fluxo uma vez (flow.microsoft.com).


3. O que você deve fazer se receber o seguinte erro ao ativar o Partner Center para o fluxo do CRM na plataforma de energia automatizada?
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Mensagem de erro que requer atualizações":::

Siga estas etapas de solução de problemas:

- Ative primeiro os dois fluxos filho a seguir antes de ativar o Partner Center para o fluxo do CRM.
      - Partner Center para CRM-Helper (insider Preview)
      - Partner Center Microsoft co-vender atualizações de referência para CRM (insider Preview)

4. O que você deve fazer quando não é possível adicionar conexões ao fluxo ao tentar editar o fluxo?

Você adiciona conexões ao fluxo enquanto o fluxo está em execução e adiciona a cada fluxo separadamente.  Se a caixa de diálogo para adicionar conexões não abrir automaticamente ao editar o fluxo, você poderá editar cada uma das etapas e subetapas dos fluxos para adicionar as conexões.

- Selecione cada fluxo e edite-os individualmente.
- Expandir todas as etapas no fluxo 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Etapas que precisam de conexões":::

- Selecione as etapas em que você verá um ícone de aviso solicitando a associação de conexões e adicionar conexões. 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Editar o fluxo passo a passo":::


5. O que você deve fazer se os fluxos da solução covenda de conectores de indicações não ativarem (ativar)?

a. Na energia automatizada, você precisará editar os fluxos na seguinte ordem e atualizá-los para usar as respectivas conexões:

- Registro do webhook do Partner Center (insider Preview)
- Criar referência de co-venda-Salesforce para o Partner Center (insider Preview)
- Partner Center Microsoft co-vender atualizações de referência para o Salesforce (insider Preview)
- Partner Center para Salesforce (insider Preview)
- Salesforce para o Partner Center (insider Preview)
- Oportunidade do Salesforce para o Partner Center (insider Preview)
- Salesforce Microsoft Solutions para Partner Center (insider Preview)

 B. Para cada fluxo, selecione a opção **executar somente usuários** . Selecione **usar conexão** em vez de **fornecido pelo usuário somente execução**.  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Para ativar um fluxo":::


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

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Como sincronizar referências":::

Certifique-se de que as seguintes condições sejam atendidas:

- A ID da solução é fornecida como parte da oportunidade.

- O código do país de duas letras é necessário.

- Quando a ajuda da Microsoft é selecionada para a oportunidade, as informações de contato do cliente são necessárias.

3. Em quais condições uma referência não sincronizará bidirecionalmente

Verifique o seguinte:

- Os vendedores do parceiro precisam garantir que tenham habilitado a opção **sincronizar com o Partner Center** na seção CRM.

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Verifique se você habilitou a sincronização":::

- Os vendedores precisam fornecer receita e data de fechamento ao qualificar um cliente potencial.

- Se a ID do CRM for fornecida em criar ou atualizar a oportunidade de venda conjunta e se um cliente potencial/oportunidade com essa ID não for encontrado no CRM, a atualização ou criação será ignorada para essa oportunidade.

- Verifique se o campo moeda de referência está configurado no ambiente do Salesforce. 

4. O que você deve fazer se o conector for desconectado e você perder uma sincronização de referência. 

A seguir estão algumas das opções que você pode experimentar:

- Verifique se o nome de usuário ou a senha expiraram para os usuários do Partner Center com funções de administrador de referência.

- Você pode ir para a oportunidade não sincronizada, fazer uma atualização secundária e observar se a referência foi sincronizada.

- Se os fluxos tiverem sido executados e falharem, selecione o fluxo e envie novamente a execução que falhou.

5. O que você deve fazer quando obtiver erros de acesso negado?

Verifique se as funções apropriadas existem

- Função de administrador de referência para o vendedor do Partner Center 
 
- Função Administrador do sistema ou personalizador do sistema na sua instância do CRM

- Verifique se a energia automatizar os logs de usuário da conta de fluxo em https://flow.microsoft.com pelo menos uma vez antes

6. Se você vir que o **código do país da conta do cliente** está ausente durante a criação de uma oportunidade de venda conjunta, o que você deve fazer?

Você precisará adicionar o código do país ISO de duas letras à conta do cliente no CRM.

7. O que você deve fazer se você vir o erro de que a **ID da solução é necessária** ao criar uma oportunidade de venda conjunta?

Para criar uma referência de venda conjunta, você precisa de uma solução de venda pronta da Microsoft. 

8. O que você deve fazer ao ver as oportunidades de venda conjuntas criadas no Partner Center que não são sincronizadas com o CRM, mesmo que não haja nenhum erro de fluxo:

Faça o seguinte:

- Depois de criar um novo negócio de revenda no Partner Center, verifique se o Partner Center para o fluxo do Dynamics 365 é invocado (ele pode ser invocado várias vezes).

- Se o fluxo for invocado, verifique todos os fluxos invocados e identifique a execução do fluxo que atualizará o CRM. Você pode seguir as ações e verificar se ele atualizou o CRM ou encontrou um problema.

- Verifique o *novo negócio** no Partner Center para ver se ele é preenchido com a ID do CRM.

- Certifique-se de que o negócio não seja fechado acidentalmente como "ganho" ou "perdido" no Partner Center.

## <a name="next-steps"></a>Próximas etapas

- [Gerenciar clientes potenciais](manage-leads.md)
 
- [Gerenciar oportunidades de venda conjunta](manage-co-sell-opportunities.md)