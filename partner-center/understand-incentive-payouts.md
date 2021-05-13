---
title: Exibir os detalhes do incentivo e do programa
ms.topic: article
ms.date: 11/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: Use essas páginas para exibir e gerenciar Programa de incentivos status
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 798fde02b87e8f8105dad6d00c32b050fb90097e
ms.sourcegitcommit: dc9438475ccc6298bec6a698bf5fc9bd5cf2aa81
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/12/2021
ms.locfileid: "109818738"
---
# <a name="view-your-incentives-program-details"></a>Exibir os detalhes do programa de incentivos

**Funções apropriadas:** incentivos de administrador | Incentivos do usuário | Administrador global | Administrador de parceiro do MPN

Este artigo explica a página Visão geral Meus **incentivos,** que mostra o status geral de seus programas de incentivo, bem como o status de cada programa em cada local. Ele também fornece os diferentes status de registro.

>[!NOTE]
>Para obter mais informações sobre incentivos e recursos de incentivos no Partner Center, consulte Investimentos e [incentivos](https://partner.microsoft.com/membership/partner-incentives) de parceiros (é necessário entrar).

## <a name="access-the-incentives-overview-page"></a>Acessar a página de visão geral de incentivos

1. Entre no [Painel do Partner Center](https://partner.microsoft.com/dashboard).
1. Selecione **Incentivos** e, em **seguida, Visão** geral no menu.
1. Veja o resumo de ganhos e pagamentos na parte superior da página e mais detalhes na tabela a seguir. Você também pode classificar, agrupar e expandir a tabela que o acompanha:

   - Para classificar por coluna, selecione o nome da coluna.
   - Para agrupar por programa, selecione **a guia Por programa** acima da tabela.
   - Para agrupar por local, selecione **a guia Por local** acima da tabela.
   - Para exibir mais detalhes sobre os registro em um grupo específico, selecione o símbolo de divisa no final de uma determinada linha. Essa divisa expande sua exibição.
1. Se for necessária uma ação adicional para se inscrever em um programa, essas informações aparecerão na coluna **Status**. Nesse caso, selecione o símbolo de divisa para saber mais sobre as próximas etapas que você precisa realizar.

## <a name="enrollment-status"></a>Status do registro

A tabela a seguir explica os diferentes estados de registro mostrados na **coluna Status.**

| **Status**         | **Aparece quando** |
|:------------------------------------|:------------------|
| Ação requerida  | O parceiro aceitou um convite para se inscrever em um programa de incentivos, mas pode precisar atualizar informações bancárias ou fiscais. Consulte a **coluna Ações necessárias para** obter as próximas etapas ou links para atualizar suas informações bancárias ou fiscais Partner Center. |
| Descontinuado  | O programa de incentivo específico não é mais oferecido no sistema de incentivos. |
| Inscrito  | Todas as informações de impostos e bancos foram validadas. Nenhuma ação de registro adicional é exigida pelo parceiro. |
| Registrando  | O usuário não é um administrador de incentivos e o registro está na **ação necessária** ou **Validando** os Estados de registro.|
| Inativo/inelegível | O programa de incentivos pode não estar aberto para registro no momento ou o parceiro não atende à qualificação atual para registro ou reinscrição. <br><br> Se o status for **inelegível**, o parceiro não atenderá aos requisitos de qualificação atuais para o programa; a seleção do link **ver requisitos de qualificação** abaixo do status do registro mostrará os requisitos para elegibilidade e quais desses requisitos foram atendidos. <br><br> Você também pode ver um status **inativo** para os registros da Vorg (organização virtual) ou do PGA (conta global do parceiro) que não estão mais ativos no programa de incentivo.  |
| Convidado  | Um novo convite de registro de programa de incentivo foi enviado para o parceiro, mas o parceiro ainda não iniciou o processo de registro. A coluna adjacente **ações necessárias** mostra as próximas etapas e todos os links relacionados.  |
| Validando o registro  | O parceiro já concluiu ou atualizou as informações bancárias e fiscais para um registro novo ou existente e está aguardando que a Microsoft valide essas informações. Durante o processo de validação, a **validação do registro** pode aparecer por até 48 horas.  |

## <a name="see-your-payment-information"></a>Ver suas informações de pagamento

Selecione o ícone de pagamento no canto superior direito da tela para acessar esses resumos diferentes:

- Histórico de transação
- Pagamentos
- Exportar dados

:::image type="content" source="images/payouts/payout-overview.png" alt-text="Ilustra o ícone de pagamento no canto superior direito do portal do Partner Center":::

Essas informações incluem ganhos de incentivos e pagamentos totais desde que você se inscreveu em programas de incentivo. Também estão incluídas nesta página os ganhos e os pagamentos por local ou programa, bem como outras ações que talvez você precise executar para se registrar em um programa em um local específico. 

Você também pode usar a [API](https://apidocs.microsoft.com/services/partnerpayouts) de pagamento de parceiro para conectar-se e obter dados de transação e pagamentos diretamente. Consulte as [instruções de pagamento](payout-statement.md) para saber mais.

## <a name="next-steps"></a>Próximas etapas

- [Demonstrativos de pagamento](payout-statement.md)
