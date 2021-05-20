---
title: Permitir que os clientes comprem seus próprios serviços no CSP
description: Saiba como os parceiros do programa CSP podem permitir que os clientes comprem seus próprios serviços, como reservas do Azure, para uma assinatura adquirida para eles Partner Center.
ms.topic: how-to
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9fabd6bd188c9d596128672d9fce3321db9b5432
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150753"
---
# <a name="give-customers-permission-in-partner-center-to-buy-their-own-products-or-services"></a>Dar aos clientes permissão Partner Center para comprar seus próprios produtos ou serviços

**Funções apropriadas:** agente administrador | Agente de vendas

Este artigo mostra como um parceiro no programa CSP (Provedor de Soluções na Nuvem) pode dar a um cliente permissão para comprar alguns de seus próprios serviços ou recursos.

Os parceiros no programa CSP geralmente usam Partner Center e seu marketplace comercial para comprar soluções e serviços para seus clientes. Em seguida, os parceiros permitem que alguns clientes provisionem esses serviços diretamente do portal do Azure.

Aqui está um exemplo. Digamos que você compre uma assinatura do Plano do Azure para um cliente no Partner Center. Em seguida, você decide adicionar outros recursos ou serviços a essa assinatura em nome do cliente. Nesse caso, você pode adicionar reservas do Azure à assinatura do cliente (como adicionar instâncias reservadas de máquina virtual). Em seguida, você pode permitir que o cliente provisione ainda mais os recursos de reserva do Azure no portal do Azure.

Agora, com o **recurso Permissões do** cliente, você dá aos clientes mais opções de autoatendados com recursos do Azure. Ao ligar as permissões para o cliente, você permite que os clientes comprem seus próprios recursos (por exemplo, comprando suas próprias reservas do Azure).  

## <a name="overview-of-customer-permissions-in-partner-center"></a>Visão geral das permissões do cliente Partner Center

Use a página **Conta do** Cliente para ativar (ou desativar) permissões de cliente. Atualmente, esse recurso dá suporte a:

- **Reservas do Azure:** A adoção dessa permissão permite que o cliente compre suas próprias reservas do Azure para uma assinatura específica do Azure que você comprou para elas.

Antes de ativar as permissões do cliente, observe estes pontos importantes:

- Por padrão, as permissões do cliente são desabilitadas automaticamente (desativadas) no Partner Center.

- Antes de ativar (ou desativar) as permissões para um cliente, você deve receber a função de agente de administração no Partner Center.

  Os parceiros que atribuiram a função de agente de vendas ou agente de suporte técnico têm acesso somente leitura e não podem ativar ou desativar as permissões do cliente.

- Você pode ativar (habilitar) permissões para qualquer cliente que escolher.

- Você pode ativar (ou desativar) as permissões do cliente usando o painel do Partner Center ou as [APIs do Partner Center](/partner-center/develop/manage-customers).

- Depois de ativar (habilitar) as permissões para um cliente específico, você será responsável por pagar por quaisquer compras subsequentes feitas por esse cliente. Se os clientes quiserem trocar, cancelar ou renovar uma compra que foram feitas (ou se quiserem alterar o escopo inicial de uma reserva), eles não poderão fazer isso por conta própria. Eles precisam pedir a você, como parceiro, para ajudá-los a trocar, cancelar e renovar compras ou fazer alterações posteriores no escopo de uma reserva.  

- Depois de ativar as permissões para um cliente específico, você **não** será notificado sobre nenhuma compra posterior feita pelo cliente.

- As compras posteriores feitas pelo cliente serão exibidas no Partner Center junto com as compras feitas por você. Você pode encontrar essas compras na página histórico do **pedido** do cliente, na página **reservas** ou no log de [**atividades**](activity-logs.md).

>[!NOTE]
> Para obter informações sobre os preços que o cliente pagará e como ajudar os clientes a gerenciar suas compras, consulte [ajudar os clientes a gerenciar as reservas que comprarem](give-customers-permission.md#help-customers-manage-reservations-they-purchase).

## <a name="give-customers-permission-to-buy-their-own-azure-reservations"></a>Dê permissão aos clientes para comprar suas próprias reservas do Azure

As reservas do Azure são uma ótima maneira de comprar serviços do Azure por uma taxa reduzida. Para saber mais sobre os benefícios das reservas do Azure, confira [o que são as reservas do Azure?](/azure/cost-management-billing/reservations/save-compute-costs-reservations)

Agora você tem a opção de comprar reservas do Azure em nome de seus clientes, pois talvez já tenha feito isso. Ou você pode conceder aos clientes permissão para comprar suas próprias reservas do Azure.

>[!NOTE]
> Depois de conceder aos clientes permissão para comprar suas próprias reservas do Azure, ajude-os a gerenciar as reservas que comprarem. Para obter mais informações, consulte [Ajudar os clientes a gerenciar reservas que compram](give-customers-permission.md#help-customers-manage-reservations-they-purchase).

### <a name="to-enable-customers-to-buy-their-own-azure-reservations"></a>Para permitir que os clientes comprem suas próprias reservas do Azure

1. Verifique se o cliente tem uma assinatura existente do Plano do Azure ou global do Azure que você comprou em seu nome.

2. Verifique se o cliente recebeu a função **Proprietário** para esta assinatura.

3. Habilita permissões de cliente (ative esse **recurso**) para comprar suas próprias reservas do Azure.

Cada etapa é exibida abaixo.

### <a name="verify-the-customer-has-an-existing-azure-subscription"></a>Verifique se o cliente tem uma assinatura existente do Azure

Antes de dar aos clientes permissão para comprar suas próprias reservas do Azure, você deve verificar se o cliente tem um Plano do Azure ou uma assinatura global do Azure existente. Se o cliente não mostrar nenhuma assinatura atual do Azure no Partner Center, você deverá comprar uma assinatura para ele antes de ativar as permissões do cliente.

- Para ver se um cliente já tem uma assinatura do Azure, entre no painel Partner Center e selecione **CSP** seguido por **Clientes**. Selecione o cliente específico na lista. Em **seguida, selecione Assinaturas** e procure assinaturas baseadas em uso para o Plano do Azure ou o Azure Global.

- Se um cliente não tiver uma assinatura existente do Azure, você poderá comprar uma assinatura para ele. Confira [Comprar o Plano do Azure.](purchase-azure-plan.md)

### <a name="verify-the-customer-has-been-assigned-the-correct-role-in-azure"></a>Verifique se o cliente recebeu a função correta no Azure

Depois de verificar se o cliente tem uma assinatura existente do Azure, você também precisa  verificar se os principais usuários associados ao cliente foram atribuídos à função de Proprietário correta para essa assinatura do Azure. Esse é o RBAC (acesso baseado em função) que o cliente precisa para comprar reservas do Azure para uma assinatura do Azure que você comprou.

Alguns parceiros podem já ter atribuído a função **proprietário** aos clientes que querem gerenciar e provisionar ativamente seus próprios recursos do Azure. Se você já **atribuiu** o status de Proprietário a um cliente para gerenciar assinaturas anteriores que comprou para eles, ignore esta etapa.  

> [!IMPORTANT]
> Se um cliente não tiver sido atribuído à função de **proprietário** , ele receberá um erro no portal do Azure impedindo que eles comprem reservas do Azure.

Para verificar se o cliente recebeu a função de **proprietário** de uma assinatura do Azure:

1. Entre no [painel](https://partner.microsoft.com/dashboard) do Partner Center.

2. Selecione **CSP**, em seguida, **clientes** e selecione o cliente específico.

3. Selecione **assinaturas** para esse cliente e localize a assinatura específica do Azure.

4. Selecione o botão **gerenciar** ao lado da assinatura do cliente. Isso abre a [portal do Azure](https://portal.azure.com/).

5. Para atribuir a função de **proprietário** a um usuário específico, siga estas etapas [para atribuir um usuário como administrador](/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator).

### <a name="turn-on-or-turn-off-customer-permissions-to-purchase-their-own-azure-reservations"></a>Ativar ou desativar as permissões do cliente para comprar suas próprias reservas do Azure

Depois de verificar se o cliente tem uma assinatura do Azure existente e os usuários recebem a função de **proprietário** para essa assinatura, você estará pronto para ativar (habilitar) permissões de cliente. Você também pode usar estas etapas para desativar (desabilitar) permissões de cliente. Você pode habilitar ou desabilitar as permissões do cliente usando o painel do Partner Center ou as [APIs do Partner Center](/partner-center/develop/manage-customers).

Para ativar (ou desativar) as permissões de cliente no Partner Center:

1. Entre no [painel](https://partner.microsoft.com/dashboard) do Partner Center.

2. No menu de navegação à esquerda, selecione **CSP** e, em seguida, **clientes**. Uma lista de clientes é exibida.

3. Selecione um nome de cliente específico.

4. Selecione **conta** no menu do cliente. A página **conta** do cliente é exibida.

5. Localize a área **permissões do cliente** na parte inferior da página.

   :::image type="content" source="images/give-customers-permission-reservations.png" alt-text="Permissões de cliente na página conta." border="true":::

6. Em **reservas do Azure**, localize a opção **permitir que o cliente adquira** .

7. Para ativar as permissões do cliente, mova a opção ao lado dessa opção para a posição **ligado** . Para desativar as permissões do cliente, mova a mudança para a posição **desativado** .

>[!NOTE]
> Para saber o que mais acontece quando você ativa as permissões de um cliente para comprar suas próprias reservas do Azure, consulte [visão geral das permissões do cliente no Partner Center](give-customers-permission.md#overview-of-customer-permissions-in-partner-center).
>
>Quando você ativa (ou desativa) as permissões de cliente, o log de atividades registra cada ação. (Esse log é acessível quando você seleciona o ícone de engrenagem na parte superior do painel do Partner Center). Quando você ativar ou desativar as permissões do cliente, a ação será exibida como **criar permissões de compra do cliente** ou **excluir permissões de compra do cliente** no log de atividades.

## <a name="help-customers-manage-reservations-they-purchase"></a>Ajude os clientes a gerenciar as reservas que comprarem

Depois de conceder aos clientes permissão para comprar suas próprias reservas do Azure, você pode ajudá-los a gerenciar melhor os recursos que comprarem. Os clientes podem gerenciar vários aspectos das próprias reservas do Azure diretamente do [portal do Azure](https://portal.azure.com/). Eles precisarão de sua ajuda para gerenciar alguns outros aspectos das reservas do Azure que comprarem em sua assinatura do CSP.  

Ajude os clientes a entender mais sobre o gerenciamento desses aspectos de reservas do Azure:

- Preços que os clientes pagarão pelas reservas do Azure
- Como os clientes podem otimizar o uso de reservas do Azure
- O que acontece quando os clientes compram reservas com um escopo compartilhado?
- O que acontece se os clientes desejarem alterar, cancelar e renovar uma reserva ou alterar seu escopo?

**Os preços que os clientes pagarão por suas reservas.** Seu cliente comprará as reservas do Azure com base em uma assinatura que você comprou anteriormente para elas em sua conta de cobrança do parceiro CSP. O preço do cliente para quaisquer reservas do Azure adquiridas com base nessa assinatura também é definido por você. Esse preço pode ser diferente do preço direto da Web que o cliente vê na portal do Azure.

**Como os clientes podem otimizar o uso de uma reserva.** Alguns clientes podem se beneficiar de aprender mais sobre como otimizar o uso de uma reserva ou como atribuir o escopo inicial de uma reserva durante sua compra. Para obter mais informações, peça aos clientes para ler [Gerenciar reservas para recursos do Azure.](/azure/cost-management-billing/reservations/manage-reserved-vm-instance)

**O que acontece quando um cliente compra uma reserva com um escopo compartilhado?** Quando os clientes comprarem uma reserva com base em uma assinatura anterior do CSP e atribuirem um escopo compartilhado a essa reserva, todos os descontos que o cliente tiver sido dado pelo CSP se aplicarão ao uso correspondente para todas as assinaturas que o parceiro CSP comprou para esse cliente.

**O que os clientes devem fazer se quiserem trocar, cancelar ou renovar uma compra que fizeram ou alterar o escopo inicial de uma reserva?** Os clientes precisam pedir ao parceiro para ajudá-los a alterar o escopo inicial de uma reserva. Eles também precisam da ajuda de um parceiro para trocar, cancelar ou renovar uma reserva. Eles não podem executar essas tarefas por conta própria com reservas com base nas assinaturas adquiridas para elas por um parceiro do CSP.

## <a name="next-steps"></a>Próximas etapas

- [Comprar reservas do Azure em nome de seus clientes](azure-reservations-buying.md)

- [Partner Center - Vender reservas da Microsoft](azure-reservations.md)

- [Gerenciar reservas do Azure em nome dos seus clientes](azure-reservations-manage.md)