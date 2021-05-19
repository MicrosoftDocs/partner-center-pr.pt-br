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
ms.openlocfilehash: 49a2b6e5461dacbe87c34b36805a5c240c2e5fd1
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148339"
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
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Mensagem de erro que requer atualizações":::

Siga estas etapas de solução de problemas:

- Ative primeiro os dois fluxos filho a seguir antes de ativar o Partner Center para o fluxo do CRM.
      - Partner Center para CRM-Helper (insider Preview)
      - Partner Center Microsoft co-vender atualizações de referência para CRM (insider Preview)

4. O que você deve fazer quando não é possível adicionar conexões ao fluxo ao tentar editar o fluxo?

Você adiciona conexões ao fluxo enquanto o fluxo está em execução e adiciona a cada fluxo separadamente.  Se a caixa de diálogo para adicionar conexões não abrir automaticamente ao editar o fluxo, você poderá editar cada uma das etapas e as subetapas dos fluxos individualmente.

- Selecione cada fluxo e edite-os individualmente.
- Expandir todas as etapas no fluxo 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Etapas que precisam de conexões":::

- Selecione as etapas em que você verá um ícone de aviso solicitando a associação de conexões e adicionar conexões. 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Editar o fluxo passo a passo":::


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

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Para ativar um fluxo":::


C. Ative-os abaixo dos fluxos mencionados:

 - Partner Center Microsoft co-vender atualizações de referência para o Salesforce (insider Preview)

- Salesforce para o Partner Center (insider Preview)

    
D. Ative todos os fluxos restantes.

E. Em registro de webhook do Flow Center de fluxo, selecione **executar**. Forneça a **URL http** da primeira ação no **Partner Center para** o fluxo do Salesforce. Selecione todas as quatro opções em **eventos para registrar** e selecione **Sim** para substituir.

## <a name="questions-and-answers-about-runmaintenance"></a>Perguntas e respostas sobre a execução/manutenção

1. Como solucionar problemas de falhas durante a execução do fluxo de energia automatizada?

Para garantir que seus fluxos de energia automatizada sejam executados conforme esperado e para solucionar falhas durante a execução, consulte [corrigir falhas de fluxo](/power-automate/fix-flow-failures).

2. O que você deve fazer se vir as referências que não estão sincronizadas corretamente no ambiente do Partner Center ou CRM?
 
Para determinar o status da sincronização de referência, selecione **auditoria**. 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Como sincronizar referências":::

Certifique-se de que as seguintes condições sejam atendidas:

- A ID da solução é fornecida como parte da oportunidade.

- O código do país de duas letras é necessário.

- Quando a ajuda da Microsoft é selecionada para a oportunidade, as informações de contato do cliente são necessárias.

3. Como garantir que uma referência seja sincronizada bidirecionalmente?

Execute as seguintes etapas:

- Os vendedores do parceiro precisam garantir que tenham habilitado a opção **sincronizar com o Partner Center** na seção CRM.

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Verifique se você habilitou a sincronização":::

- Os vendedores precisam fornecer receita e data de fechamento ao qualificar um cliente potencial.

- Se a ID do CRM for fornecida no estágio **criar** ou **Atualizar** da oportunidade de venda conjunta, mas uma oportunidade de cliente potencial com essa ID não for encontrada no CRM, a atualização ou criação será ignorada.

- Verifique se o campo moeda de referência está configurado no ambiente do Salesforce. 

4. O que você deve fazer se o conector for desconectado e você perder uma sincronização de referência.?

A seguir estão algumas das opções que você pode experimentar:

- Verifique se o nome de usuário ou a senha expiraram para os usuários do Partner Center com funções de administrador de referência.

- Você pode ir para a oportunidade não sincronizada, fazer uma atualização secundária e observar se a referência foi sincronizada.

- Se os fluxos tiverem sido executados e falharem, selecione o fluxo e envie novamente a execução que falhou.

5. O que você deve fazer quando obtiver erros de acesso negado?

Verifique se as funções apropriadas existem

- Função de administrador de referência para o vendedor do Partner Center 
 
- Função Administrador do sistema ou personalizador do sistema na sua instância do CRM

- Verifique se a energia automatizar os logs de usuário da conta de fluxo em https://flow.microsoft.com pelo menos uma vez antes

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
