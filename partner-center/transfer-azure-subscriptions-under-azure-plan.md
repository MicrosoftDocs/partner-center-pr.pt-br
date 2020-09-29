---
title: Transferir a assinatura do Azure em um plano do Azure para outro parceiro CSP
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como alterar o parceiro de programa do provedor de soluções na nuvem associado às assinaturas do Azure de um cliente em um plano do Azure.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: e1b70f26dc146507ac3764ae223ca27915162f0c
ms.sourcegitcommit: 3329fd120d8d49a4831412b79e044678ec71b84c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/29/2020
ms.locfileid: "91422538"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a>Transferir as assinaturas do plano do Azure de um cliente para um parceiro diferente

## <a name="applies-to"></a>Aplica-se a

- Parceiros no programa CSP (Provedor de Soluções na Nuvem)

Este artigo descreve como um cliente pode mudar suas assinaturas do Azure em um plano do Azure de um CSP (provedor de soluções de nuvem) para outro.

Para mudar as assinaturas do Azure do cliente de um parceiro diferente, siga estas etapas. O parceiro e o cliente têm as etapas a serem concluídas.

>[!Note]  
>Somente parceiros com uma relação de cobrança direta com a Microsoft podem acessar as ferramentas de transição. Revendedores indiretos devem trabalhar com seus provedores indiretos para aproveitar essa ferramenta de transição.

O cliente deve estar em conversa com os dois parceiros (atuais e futuros) antes da utilização dessa ferramenta. Uma conversa offline precisa ser necessária para evitar confusão e variações. Além disso, os parceiros e os clientes devem entender essas considerações e pré-requisitos antes de iniciar uma transição:

**Principais considerações:**

- As reservas do Azure não serão movidas com a assinatura para o parceiro futuro
- O preço do CSP para serviços do Azure sob o parceiro atual não fará a transição  
- As responsabilidades de suporte para o cliente passarão para o futuro parceiro
- Cobrança e faturamento serão transferidos para o futuro parceiro no momento da transferência
- O RBAC (controle de acesso baseado em função) do Azure não é afetado pela transferência
- O administrador em nome de (AOBO) não será concedido por padrão ao parceiro futuro
- Os produtos do Marketplace de terceiros serão transferidos desde que os produtos passem pela verificação de qualificação do Marketplace.
    - Não há descontos especiais ou restrições regionais
    - Os produtos não são baseados em assinatura
    - O parceiro futuro deve funcionar com o editor para garantir que eles estejam na lista de permissões para implantação do produto
    - Se nem todas essas condições forem atendidas para transferir os produtos do Marketplace devem ser cancelados, as assinaturas do Azure transferidas e, em seguida, adquirir novamente de produtos do Marketplace com o novo parceiro

**Pré-requisitos:**

- O cliente participa do parceiro CSP atual em sua intenção de fazer a transição
- O futuro parceiro CSP trabalha com o cliente para garantir que as necessidades do cliente possam ser atendidas
- O parceiro CSP futuro estabelece uma relação com o cliente antes do início da transição  
- O cliente deve assinar o contrato do cliente da Microsoft com o futuro parceiro CSP
- O parceiro CSP futuro deve ter assinado o Microsoft Partner Agreement para usar essa ferramenta

## <a name="customer-tasks-to-be-completed"></a>Tarefas do cliente a serem concluídas

Para transferir uma assinatura do Azure em um plano do Azure, o cliente deve iniciar o processo entrando em contato com o parceiro atual. Eles devem coletar o nome e o domínio da empresa do seu parceiro atual para que seu parceiro futuro possa concluir o formulário de solicitação de transferência em seu nome.

O cliente também deve identificar as assinaturas que desejam transferir de seu parceiro atual. Você não pode alterar parceiros para as assinaturas do Office 365, Enterprise Mobility Suite ou Microsoft Dynamics CRM.

>[!Note]  
>É responsabilidade do parceiro futuro concluir o formulário de solicitação de transferência que inicia o processo de transferência. A Microsoft não pode intervir em nome do cliente ou do parceiro atual. O cliente deve planejar trabalhar em conjunto com seus parceiros futuros e atuais para fazer a transição funcionar sem problemas.

## <a name="future-partner-tasks-to-be-completed"></a>Tarefas futuras do parceiro a serem concluídas

O parceiro futuro da assinatura precisa concluir um formulário de solicitação de transferência do Partner Center para solicitar uma transferência de assinatura:

1.  No menu do centro de parceiros, selecione **clientes**e selecione o cliente para o qual você deseja concluir um formulário de solicitação de transferência em nome de.
2.  No menu cliente, selecione **assinaturas**.
3.  Selecione a seção **solicitação de transferência** .
4.  Na **seção solicitação de transferência**, selecione **Adicionar nova solicitação**.

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Seção de transferências":::

5.  Preencha o formulário de **nova solicitação de transferência** .

6.  Selecione **Enviar solicitação de transferência**  >  **Enviar**.

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Formulário concluir solicitação de transferência":::

7.  Examinar a confirmação da solicitação de transferência

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Revisar transferência pendente":::

    >[!Note]
    >O parceiro futuro pode cancelar a solicitação de transferência selecionando **Cancelar solicitação** no canto superior direito somente quando o status da solicitação de transferência for "pendente". Depois que o status da solicitação de transferência for "em andamento" ou "concluído", os cancelamentos não serão possíveis.

## <a name="current-partner-tasks-to-be-completed"></a>Tarefas do parceiro atual a serem concluídas

O agente de administrador do parceiro atual do cliente receberá um email informando que o cliente está solicitando uma transferência de suas assinaturas:

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Examinar":::

Examine e aceite o formulário de solicitação de transferência do centro de parceiros para concluir a transferência da assinatura.

>[!Note]  
>Se nenhuma ação for realizada pelo parceiro atual dentro de 30 dias, a solicitação expirará e o parceiro futuro terá um para criar uma nova solicitação de transferência.

1.  Selecione **examinar solicitação de transferência** do email ou
1.  No menu do centro de parceiros, selecione **clientes**e, em seguida, selecione o cliente para o qual uma solicitação de transferência foi enviada em nome de.
2.  No menu cliente, selecione **assinaturas**.
3.  Selecione a seção **solicitação de transferência** .
4.  Expanda informações de transferência selecionando a **ID da solicitação de transferência** escolhida em **solicitações recebidas**

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Solicitação de transferência de revisões de origem":::

5.  Examine a solicitação de transferência. Selecione as assinaturas do Azure solicitadas a serem transferidas.

>[!Note]  
> Antes de continuar, observe: você não terá mais acesso às assinaturas selecionadas.
> Você não será faturado para uso adicional.
> As reservas do Azure não são transferidas com as assinaturas.

6.  Em seguida, selecione **aceitar e transferir** para concluir o processo de transferência.

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Selecione as assinaturas a serem transferidas em seus planos do Azure":::

7.  Exibir confirmação de aceitação da transferência.

   Neste ponto, o parceiro futuro, o cliente e o parceiro atual serão notificados sobre a solicitação de transferência aceita por email.

   Depois, a transição foi aceita, o status da transferência pode permanecer pendente por até 15 minutos enquanto o sistema é atualizado. Se demorar mais, o sistema continuará tentando por três dias. Se o status da transferência ainda permanecer pendente, o parceiro deverá enviar uma solicitação de serviço.

   Depois que a transferência for concluída, as assinaturas incluídas na solicitação aparecerão no plano do Azure do parceiro futuro e não serão mais listadas com você.

>[!Note]  
>Para provedores indiretos: Informe seu revendedor indireto de que a solicitação de transferência foi aceita.

### <a name="managing-your-transferred-customer-subscriptions"></a>Gerenciando suas assinaturas de cliente transferidas
- O acesso a usuários, grupos ou entidades de serviço existentes que foram atribuídos usando o RBAC (controle de acesso baseado em função) do Azure não é afetado durante a transição. O Azure [RBAC (](/azure/role-based-access-control/overview) controle de acesso baseado em função) ajuda seu cliente a gerenciar quem tem acesso aos recursos do Azure, o que eles podem fazer com esses recursos e em quais áreas eles têm acesso. Como o novo parceiro, você não recebe nenhum acesso de RBAC aos recursos do cliente após a transferência da assinatura. O parceiro anterior do seu cliente retém o acesso do RBAC. Trabalhe com seu cliente para entender quem tem informações sobre suas assinaturas e como fazer as alterações desejadas.

- Consequentemente, é importante que o cliente remova o acesso RBAC do Azure para seu parceiro anterior e adicione acesso para o novo parceiro. Para obter mais informações sobre o cliente que oferece acesso novo, consulte [o que é o Azure RBAC (controle de acesso baseado em função)?](/azure/role-based-access-control/overview) Para obter mais informações sobre o cliente que remove o acesso RBAC do parceiro anterior, consulte [remover uma atribuição de função](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).

- Além disso, você não obtém automaticamente o [administrador em nome do (Aobo)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) acesso às suas assinaturas. O AOBO é necessário para que o parceiro gerencie as assinaturas do Azure do cliente em seu nome. Para obter mais informações sobre os privilégios do Azure, consulte [obter permissões para gerenciar o serviço ou a assinatura de um cliente.](/partner-center/customers-revoke-admin-privileges)

## <a name="next-steps"></a>Próximas etapas:

- [(RBAC do Azure)](/azure/role-based-access-control/overview)
- [Obtenha permissões para gerenciar o serviço ou a assinatura de um cliente.](/partner-center/customers-revoke-admin-privileges)