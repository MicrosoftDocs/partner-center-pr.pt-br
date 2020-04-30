---
title: Dê permissão aos clientes para comprar seus próprios serviços
ms.topic: article
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como os parceiros do programa CSP podem permitir que os clientes comprem seus próprios serviços, como reservas do Azure, para uma assinatura adquirida para eles.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
Keywords: assinatura, compra de autoatendimento, RI de autoatendimento, habilitar RI, desabilitar RI, autoatendimento, compra de cliente, permissões de cliente, instância reservada de compra de cliente, reservas do Azure para comprar, ativar autoatendimento, desligar o autoatendimento
ms.localizationpriority: medium
ms.openlocfilehash: ee8f1221344ce2375aff63c52bbfd42350a29839
ms.sourcegitcommit: 8359f618426e341180b0380367dd9d16dfd6623c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2020
ms.locfileid: "82255462"
---
# <a name="learn-how-to-give-customers-permission-to-buy-their-own-products-or-services"></a>Saiba como dar aos clientes permissão para comprar seus próprios produtos ou serviços

**Aplica-se a**

- Partner Center
- Parceiros no programa CSP

**Funções apropriadas**

- Agente administrativo
- Agente de vendas

Este artigo mostra como um parceiro no programa CSP (provedor de soluções na nuvem) pode conceder a um cliente permissão para comprar alguns de seus próprios serviços ou recursos.

Os parceiros no programa CSP geralmente usam o Partner Center e seu mercado comercial para comprar soluções e serviços para seus clientes. Os parceiros permitem que alguns clientes provisionem esses serviços diretamente do portal do Azure.

Veja um exemplo. Digamos que você compre uma assinatura do plano do Azure para um cliente no Partner Center. Em seguida, você decide adicionar outros recursos ou serviços a essa assinatura em nome do cliente. Nesse caso, você pode adicionar reservas do Azure à assinatura do cliente (como adicionar instâncias de máquina virtual reservadas). Em seguida, você pode permitir que o cliente provisione ainda mais os recursos de reserva do Azure no portal do Azure.

Agora, com o recurso de **permissões de cliente** , você fornece aos clientes mais opções de autoatendimento com os recursos do Azure. Ao ativar as permissões para o cliente, você permite que os clientes comprem seus próprios recursos (como, por exemplo, comprando suas próprias reservas do Azure).  

## <a name="overview-of-customer-permissions-in-partner-center"></a>Visão geral das permissões do cliente no Partner Center

Use a página **conta** do cliente para ativar (ou desativar) as permissões do cliente. Atualmente, esse recurso dá suporte a:

- **Reservas do Azure:** Ativar essa permissão permite que o cliente compre suas próprias reservas do Azure para uma assinatura específica do Azure que você comprou para elas.

Antes de ativar as permissões do cliente, observe estes pontos importantes:

- Por padrão, as permissões do cliente são desabilitadas automaticamente (desativadas) no Partner Center.
- Antes de ativar (ou desativar) as permissões para um cliente, você deve receber a função de agente de administração no Partner Center.
  Os parceiros que atribuiram a função de agente de vendas ou agente de suporte técnico têm acesso somente leitura e não podem ativar ou desativar as permissões do cliente.
- Você pode ativar (habilitar) permissões para qualquer cliente que escolher.
- Você pode ativar (ou desativar) as permissões do cliente usando o painel do Partner Center ou as [APIs do Partner Center](https://docs.microsoft.com/partner-center/develop/manage-customers).
- Depois de ativar (habilitar) as permissões para um cliente específico, você será responsável por pagar por quaisquer compras subsequentes feitas por esse cliente. Se os clientes desejarem trocar, cancelar ou renovar uma compra que eles fizeram, eles não poderão fazer isso por conta própria. Eles precisam pedir a você, como parceiro, para ajudá-los a trocar, cancelar ou renovar essas compras.
- Depois de ativar as permissões para um cliente específico, você **não** será notificado sobre nenhuma compra posterior feita pelo cliente.
- As compras posteriores feitas pelo cliente serão exibidas no Partner Center junto com as compras feitas por você. Você pode encontrar essas compras na página histórico do **pedido** do cliente, na página **reservas** ou no log de [**atividades**](activity-logs.md).

## <a name="give-customers-permission-to-buy-their-own-azure-reservations"></a>Dê permissão aos clientes para comprar suas próprias reservas do Azure

As reservas do Azure são uma ótima maneira de comprar os serviços do Azure com uma taxa com desconto. Para saber mais sobre os benefícios das reservas do Azure, confira [o que são as reservas do Azure?](https://docs.microsoft.com/azure/cost-management-billing/reservations/save-compute-costs-reservations)

Agora você tem a opção de comprar reservas do Azure em nome de seus clientes, pois talvez já tenha feito isso. Ou você pode conceder aos clientes permissão para comprar suas próprias reservas do Azure.

>[!NOTE]
> Depois de conceder aos clientes permissão para comprar suas próprias reservas do Azure, você pode ajudá-los a entender como gerenciar as reservas que comprarem. Por exemplo, os clientes talvez queiram saber como otimizar o uso de uma reserva ou como alterar o escopo de uma reserva. Para obter mais informações sobre esses tópicos, peça aos clientes para ler as [reservas de gerenciamento de recursos do Azure]( https://docs.microsoft.com/azure/cost-management-billing/reservations/manage-reserved-vm-instance).

### <a name="to-enable-customers-to-buy-their-own-azure-reservations"></a>Para permitir que os clientes comprem suas próprias reservas do Azure

1. Verifique se o cliente tem um plano do Azure existente ou uma assinatura global do Azure que você comprou em seu nome.

2. Verifique se a função de **proprietário** foi atribuída ao cliente para esta assinatura.

3. Habilitar permissões de cliente (ativar este **recurso)** para comprar suas próprias reservas do Azure.

Cada etapa aparece abaixo.

### <a name="verify-the-customer-has-an-existing-azure-subscription"></a>Verificar se o cliente tem uma assinatura do Azure existente

Antes de conceder aos clientes permissão para comprar suas próprias reservas do Azure, você deve verificar se o cliente tem um plano do Azure ou uma assinatura global do Azure existente. Se o cliente não mostrar nenhuma assinatura do Azure atual no Partner Center, você deverá comprar uma assinatura para eles antes de ativar suas permissões de cliente.

- Para ver se um cliente já tem uma assinatura do Azure, entre no painel do Partner Center e selecione **CSP** seguido pelos **clientes**. Selecione o cliente específico na lista. Em seguida, selecione **assinaturas** e procure por qualquer assinatura baseada em uso para o plano do Azure ou para o Azure global.

- Se um cliente não tiver uma assinatura do Azure existente, você poderá comprar uma assinatura para elas. Consulte [comprar o plano do Azure](purchase-azure-plan.md).

### <a name="verify-the-customer-has-been-assigned-the-correct-role-in-azure"></a>Verifique se a função correta foi atribuída ao cliente no Azure

Depois de verificar se o cliente tem uma assinatura do Azure existente, você também precisa verificar se os principais usuários associados ao cliente receberam a função de **proprietário** correta para essa assinatura do Azure. Esse é o RBAC (acesso baseado em função) que o cliente precisa para comprar reservas do Azure para uma assinatura do Azure que você comprou.

Alguns parceiros podem já ter atribuído a função de **proprietário** aos clientes que desejam gerenciar e provisionar ativamente seus próprios recursos do Azure. Se você já tiver atribuído o status de **proprietário** a um cliente para gerenciar as assinaturas anteriores que comprou para eles, poderá ignorar esta etapa.  

> [!IMPORTANT]
> Se um cliente não tiver sido atribuído à função de **proprietário** , ele receberá um erro no portal do Azure impedindo que eles comprem reservas do Azure.

Para verificar se o cliente recebeu a função de **proprietário** de uma assinatura do Azure:

1. Entre no [painel](https://partner.microsoft.com/dashboard) do Partner Center.

2. Selecione **CSP**, em seguida, **clientes** e selecione o cliente específico.

3. Selecione **assinaturas** para esse cliente e localize a assinatura específica do Azure.

4. Selecione o botão **gerenciar** ao lado da assinatura do cliente. Isso abre a [portal do Azure](https://portal.azure.com/).

5. Para atribuir a função de **proprietário** a um usuário específico, siga estas etapas [para atribuir um usuário como administrador](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator).

### <a name="turn-on-or-turn-off-customer-permissions-to-purchase-their-own-azure-reservations"></a>Ativar ou desativar as permissões do cliente para comprar suas próprias reservas do Azure

Depois de verificar se o cliente tem uma assinatura do Azure existente e os usuários recebem a função de **proprietário** para essa assinatura, você estará pronto para ativar (habilitar) permissões de cliente. Você também pode usar estas etapas para desativar (desabilitar) permissões de cliente. Você pode habilitar ou desabilitar as permissões do cliente usando o painel do Partner Center ou as [APIs do Partner Center](https://docs.microsoft.com/partner-center/develop/manage-customers).

Para ativar (ou desativar) as permissões de cliente no Partner Center:

1. Entre no [painel](https://partner.microsoft.com/dashboard) do Partner Center.

2. No menu de navegação à esquerda, selecione **CSP**e, em seguida, **clientes**. Uma lista de clientes é exibida.

3. Selecione um nome de cliente específico.

4. Selecione **conta** no menu do cliente. A página **conta** do cliente é exibida.

5. Localize a área **permissões do cliente** na parte inferior da página.

   ![Permissões de cliente na página conta](images/give-customers-permission-reservations.png)

6. Em **reservas do Azure**, localize a opção **permitir que o cliente adquira** .

7. Para ativar as permissões do cliente, mova a opção ao lado dessa opção para a posição **ligado** . Para desativar as permissões do cliente, mova a mudança para a posição **desativado** .

>[!NOTE]
> Para saber o que mais acontece quando você ativa as permissões de um cliente para comprar suas próprias reservas do Azure, consulte [visão geral das permissões do cliente no Partner Center](give-customers-permission.md#overview-of-customer-permissions-in-partner-center). Quando você ativa (ou desativa) as permissões de cliente, o log de atividades registra cada ação. (Esse log é acessível quando você seleciona o ícone de engrenagem na parte superior do painel do Partner Center). Quando você ativar ou desativar as permissões do cliente, a ação será exibida como **criar permissões de compra do cliente** ou **excluir permissões de compra do cliente** no log de atividades.

## <a name="see-also"></a>Confira também

- [Comprar reservas do Azure em nome de seus clientes](azure-reservations-buying.md)
- [Partner Center – vender reservas da Microsoft](azure-reservations.md)
- [Gerenciar reservas do Azure em nome dos seus clientes](azure-reservations-manage.md) 