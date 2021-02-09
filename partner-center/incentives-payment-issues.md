---
title: Solução de problemas com pagamentos e lucros
ms.topic: article
ms.date: 02/05/2021
description: Saiba como solucionar problemas como ganhos ausentes ou incorretos, problemas de qualificação e como reconciliar seus ganhos de incentivos.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: 971b053119a263ed5c7f8e25fb532b4137e1cb13
ms.sourcegitcommit: 2d1f0d7bc897278ef37af6d43c1a088f5ca14807
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/08/2021
ms.locfileid: "99834876"
---
# <a name="troubleshooting-missing-payments-incorrect-earnings-and-other-issues"></a>Solucionando problemas de pagamentos ausentes, ganhos incorretos e outros problemas

**Aplica-se a**:

- Partner Center

**Funções apropriadas**:

- Administrador de incentivos

Este artigo ajudará você a resolver quaisquer problemas de lucros ou pagamentos em seu programa de incentivos. Os tópicos abordados incluem o tempo de pagamento, a verificação da elegibilidade de seus ganhos e a importância de configurar seus perfis de pagamento e de impostos corretamente.

## <a name="who-can-create-or-update-payout-and-tax-profiles-for-my-organization"></a>Quem pode criar ou atualizar perfis de pagamento e de impostos para minha organização?

Os usuários que têm a função de administrador de incentivos no Partner Center para o programa de incentivo e o local de MPN relevantes podem atualizar e ver os perfis de pagamento e de impostos da organização.

## <a name="how-long-does-it-take-for-microsoft-to-approve-my-pending-payout-andor-tax-profiles"></a>Quanto tempo leva para a Microsoft aprovar meus perfis de pagamento e/ou imposto pendentes?

A validação pode levar até 48 horas. Durante esse tempo, o status do perfil na página Visão geral será exibido como Validando o registro. Quando o processo for concluído, o status será exibido como **registrado** se for bem-sucedido ou **ação necessária – atualizar pagamento e/ou detalhes de impostos** , se necessário.

## <a name="how-do-i-know-if-i-have-completed-my-payout-and-tax-profile-correctly"></a>Como posso saber se preenchi meu perfil de pagamento e imposto corretamente?

O status do registro é exibido na página Visão geral. Quando você terminar de criar seus perfis, seu status estará **Validando o registro**. Depois de validarmos suas informações, seu status será alterado para **registrado**. Esse status indica que o pagamento e o perfil de impostos e seu registro foram concluídos com êxito.

## <a name="why-do-i-need-to-update-my-tax-profile-to-use-it-with-a-new-incentive-program"></a>Por que preciso atualizar meu perfil fiscal para usá-lo com um novo programa de incentivo?

Nós pagamos incentivos de diferentes locais, dependendo do tipo de incentivo. Esses locais diferentes podem exigir informações adicionais sobre impostos, com base nas regras do programa de incentivo, para dar andamento corretamente.

## <a name="how-can-i-delete-a-payment-andor-tax-profile"></a>Como posso excluir um perfil de pagamento e/ou imposto?

Atualmente, a Microsoft não oferece suporte à opção de excluir perfis de pagamento e imposto existentes.

## <a name="my-payment-is-missing-or-incorrect"></a>Meu pagamento está ausente ou incorreto

Pagamentos ausentes ou incorretos geralmente são devidos a uma das seguintes opções:

- **Talvez você não esteja qualificado.**  Os ganhos só estarão disponíveis se você atender aos Requisitos de qualificação operacionais, ou seja, registrados no respectivo período de lucro do programa.
- **Você pode não ter atendido aos requisitos.**  Verifique se você cumpriu as regras de qualificação e de receita qualificada para o incentivo que está procurando.

  **Para verificar sua elegibilidade**

  1. Entre em [incentivos de parceiros](https://partner.microsoft.com/membership/partner-incentives).

  2. Role para baixo até os documentos do seu programa.
  
  3. Selecione o link do documento desejado e examine as seções 

**Qualificação para parceiros** e **regras de receita qualificada**.

- **Seu perfil de pagamento pode estar incompleto.** A data de início dos ganhos de incentivo será o primeiro dia do mês em que você concluiu todos os requisitos de qualificação, incluindo a integração com os detalhes de pagamento e imposto. Os lucros não estarão disponíveis para os meses antes da conclusão do pagamento e do imposto. Por exemplo, se você concluir todos os requisitos durante o mês de abril de 2020, a data de início dos lucros será 1º de abril de 2020.
- **Você pode ter uma ação pendente**.  Pode ser que seus incentivos não estejam sendo processados porque há uma ação pendente.

  **Para exibir suas ações pendentes**

  1. Entre em [incentivos de parceiros](https://partner.microsoft.com/membership/partner-incentives).
  2. Abra a página **histórico de transações** . Examine os campos nesta página para que as ações pendentes sejam concluídas, como **perfil de imposto pendente**, **perfil de pagamento pendente** ou **envio de fatura de imposto pendente**.

Se essas ações não ajudarem e seus pagamentos ainda estiverem ausentes ou incorretos, contate o [suporte](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="how-can-i-reconcile-my-adjustments"></a>Como posso reconciliar meus ajustes?

Você pode localizar e reconciliar seus ajustes baixando seus detalhes de conquista e transação.

1. Entre no painel [Partner Center](https://partner.microsoft.com/dashboard/).
2. Na barra de navegação superior, selecione o ícone de dinheiro e, em seguida, selecione **histórico de transações**.
3. Aplique os filtros apropriados. (Veja a observação **importante** abaixo.)
4. Depois de filtrar os dados, selecione **Iniciar Download** e, em seguida, selecione **exportar dados**. Seus dados serão abertos em um arquivo CSV.
5. No arquivo CSV, navegue até a coluna P, **tipo de conquista**.
6. Filtrar esta coluna para o **ajuste de desconto**. Você pode ver o mês de cada ajuste na coluna S.

>[!IMPORTANT]
>Os ajustes aplicados aos períodos de ganhos anteriores não estarão visíveis nos ganhos do mês em que o ajuste foi aplicado. Os ajustes sempre serão refletidos no relatório de ganhos do mês em que o ajuste foi aplicado.
>
>Por exemplo, um ajuste para os ganhos de janeiro de 2019 que foi processado em setembro de 2019 não refletirá no valor de ganhos para 2019 de setembro. No entanto, quando o pagamento de setembro de 2019 for recebido, ele incluirá o ajuste de janeiro de 2019 que foi aplicado em setembro. Nesse cenário, você precisa baixar os detalhes da transação de janeiro de 2019 para ver o ajuste que foi aplicado.
>
>Tenha isso em mente ao definir os filtros de data. Conforme mencionado acima, os ajustes dos períodos anteriores só estarão visíveis no mês em que o ajuste foi aplicado. Verifique se o intervalo de datas selecionado corresponde ao mês do ajuste que você está tentando localizar. Talvez seja necessário selecionar **limpar tudo** para remover os filtros e, em seguida, aplicar os novos.

## <a name="why-are-my-co-op-claim-payments-made-in-two-different-currencies"></a>Por que meus pagamentos da declaração de cooperação são feitos em duas moedas diferentes?

Quando os fundos de cooperação são obtidos de diferentes entidades da Microsoft, os pagamentos são feitos na moeda local de cada entidade respectiva.  

## <a name="why-was-i-paid-in-a-currency-other-than-my-co-op-claim-currency"></a>Por que fui pago em uma moeda diferente da minha moeda de declaração de cooperação?

Cada programa de incentivos tem um perfil bancário criado durante a instalação. A moeda especificada nesse perfil é a moeda em que você será pago.

## <a name="i-dont-see-earnings-for-a-certain-period"></a>Não vejo os ganhos por um determinado período

Quando você não vir os ganhos por um período em que eles são esperados, isso geralmente ocorre devido a um dos seguintes problemas:

- **Talvez você não esteja qualificado.**  Os ganhos só estarão disponíveis se você atender aos Requisitos de qualificação operacionais, ou seja, registrados no respectivo período de lucro do programa.

- **Seu perfil de pagamento pode estar incompleto.**  A data de início dos ganhos de incentivo será o primeiro dia do mês em que você concluiu todos os requisitos de qualificação, incluindo a integração com os detalhes de pagamento e imposto. Os lucros não estarão disponíveis para os meses antes da conclusão do pagamento e do imposto. Por exemplo, se você concluir todos os requisitos durante o mês de abril de 2020, a data de início dos lucros será 1º de abril de 2020.

Se você tiver concluído os requisitos de qualificação, incluindo a integração com os detalhes de pagamento e imposto sobre o tempo, e os ganhos ainda estiverem ausentes, entre em contato com o [suporte](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="my-earnings-are-missing-or-incorrect"></a>Meus ganhos estão ausentes ou incorretos

Ganhos ausentes ou incorretos podem ser causados por um dos seguintes problemas:

- **Você pode não ter atendido aos requisitos.**  Verifique se você cumpriu as regras de [qualificação](#my-payment-is-missing-or-incorrect) e de receita qualificada para o incentivo que está procurando.

- **Pode haver uma discrepância.**  Se você atender aos requisitos de qualificação do [programa](incentives-determined-your-program-eligibility.md) e à qualificação dos [ganhos](incentives-confirm-your-earnings-eligibility.md) e seus ganhos ainda estiverem incorretos, as informações a seguir poderão ajudá-lo a recuperar seus dados.

Os ganhos são exibidos na página **histórico de transações** e na página de **pagamentos** . Você pode acessar ambas as páginas selecionando o ícone de **pagamento** na barra de navegação no Partner Center.

:::image type="content" source="images/incentives/paymenticon.png" alt-text="Informações sobre a transação":::

Valores mensais de conquista no modo de exibição de histórico de transações podem não ser alinhados com o valor de pagamento recebido para um mês específico. Isso ocorre devido a recálculos e ajustes dos períodos de conquista anteriores que são aplicados aos futuros pagamentos.

Por exemplo, um ajuste para os ganhos de janeiro de 2019 que foi processado em setembro de 2019 não será refletido no valor de ganhos para 2019 de setembro; no entanto, quando o pagamento de setembro de 2019 for recebido, ele incluirá o ajuste de janeiro de 2019 que foi aplicado em setembro.

Nesse cenário, você precisa baixar os detalhes da transação para obter uma exibição completa de todos os ganhos incluídos em seu pagamento.  Além disso, você pode navegar até a exibição de pagamentos para baixar transações para cada pagamento.

### <a name="transaction-history"></a>Histórico de transação

Essa exibição mostra a conquista e as tendências de pagamento por mês, os ganhos por status e os detalhes da transação, juntamente com o status de pagamento de cada transação. Os dados só são visíveis para os programas e IDs de MPN para os quais você é um usuário de incentivo ou administrador.

### <a name="payments"></a>Pagamentos

Essa exibição permite exibir pagamentos para todos os programas e IDs de MPN. Os dados só são visíveis para os programas e IDs de MPN para os quais você é um usuário de incentivo ou administrador. Nessa exibição, você pode baixar a remessa ou exibir detalhes da transação por pagamento.

| Para fazer isso | Clique aqui |
| ------ | :----------- | 
| Exibir suas informações de pagamento por linha, incluindo valores de conquista e pagamento na moeda local  | Consulte o campo **lista de pagamentos**   |
| Baixar uma carta de remessa   |  Selecionar **remessa de pagamento**  |
| Exibir detalhes do nível de transação para um pagamento específico |  Selecionar **exibição**  |
| Exportar detalhes da transação para o Excel  |  Selecione **Iniciar Download** e, em seguida, clique em **exportar dados**. Observe que todos os filtros selecionados serão aplicados aos dados exportados. Depois que o status for alterado para concluído, selecione **baixar** e siga os prompts para exportar o relatório de transações detalhadas. Atualize a página se o status não for atualizado em até cinco minutos.  |

### <a name="missing-or-incorrect-earnings-and-payments"></a>Ganhos e pagamentos incorretos ou ausentes

Se não for possível localizar os detalhes de um pagamento ou de uma transação, verifique se você aplicou os filtros corretos. Observe que, como alguns nomes de programa foram alterados (por exemplo, o CSP Direct 1T Partner agora é parceiro de cobrança direto do CSP), talvez seja necessário usar várias seleções.

Se você ainda não consegue encontrar seus ganhos ou acredita que os ganhos mostrados estão incorretos, contate o [suporte](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="how-do-i-reconcile-my-earnings"></a>Como fazer reconciliar meus ganhos?

Se houver uma discrepância em seus lucros, siga as seguintes etapas:

1. **Verifique se você se qualifica para os lucros.**  Os ganhos estarão disponíveis somente se você atender à qualificação do [programa](incentives-determined-your-program-eligibility.md) e à [elegibilidade dos ganhos](incentives-confirm-your-earnings-eligibility.md).

2. **Verifique se o perfil de pagamento foi preenchido.**  A data de início dos ganhos de incentivo será o primeiro dia do mês em que você concluiu todos os requisitos de qualificação, incluindo a integração com os detalhes de pagamento e imposto. Os lucros não estarão disponíveis para os meses antes da conclusão do pagamento e do imposto. Por exemplo, se você concluir todos os requisitos durante o mês de abril de 2020, a data de início dos lucros será 1º de abril de 2020. 

3. **Verifique se você atendeu aos requisitos.**  Verifique se você atendeu às regras de [qualificação](#my-payment-is-missing-or-incorrect) e de receita qualificada para seu programa de incentivo.

Se essas ações não ajudarem e seus ganhos ainda não estiverem reconciliados, entre em contato com o [suporte](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="where-can-i-find-my-rates"></a>Em que local posso encontrar minhas taxas?

1. Entre em [incentivos de parceiros](https://partner.microsoft.com/membership/partner-incentives).

2. Role para baixo para acessar os documentos do seu programa.

3. Selecione o link do documento para o respectivo programa.

4. No documento, consulte a seção **estrutura e taxas do programa**.

## <a name="next-steps"></a>Próximas etapas

- [Gerenciar declarações de cooperação](incentives-managing-co-op-claims.md)