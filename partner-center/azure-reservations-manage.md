---
title: Gerenciar reservas do Azure para clientes
description: Saiba como gerenciar reservas do Azure para um cliente, incluindo como cancelar uma reserva, trocar uma reserva ou solicitar um reembolso.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: 1184b199d6235dd1d16fe981000bae44b797f76a
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149478"
---
# <a name="manage-cancel-exchange-or-refund-microsoft-azure-reservations-for-customers"></a>Gerenciar, cancelar, trocar ou reembolsar reservas de Microsoft Azure para clientes

**Funções apropriadas**: agente de administração | Administrador global | Agente de assistência técnica | Agente de vendas | Administrador de gerenciamento de usuários

Este artigo explica como gerenciar reservas do Azure para um cliente, incluindo como cancelar uma reserva, trocar uma reserva ou solicitar um reembolso.

> [!NOTE]
> Este artigo se aplica somente a parceiros no programa CSP (provedor de soluções na nuvem). Os clientes que usam outros tipos de assinaturas (como pagamento conforme o uso, individuais, contrato de cliente da Microsoft ou assinaturas de Contrato Enterprise) devem ler [essa documentação de reservas do Azure](/azure/cost-management-billing/reservations).

Para gerenciar as reservas do Azure de seus clientes após a compra, você selecionará o cliente e a reserva que deseja gerenciar no Partner Center e, em seguida, fará alterações na reserva no portal do Azure.

1. Para começar, selecione **clientes** no menu do centro de parceiros e, em seguida, selecione o cliente cujas reservas você deseja gerenciar. 

2. No menu da página de detalhes do cliente, selecione **reservas do Azure** e, em seguida, selecione a reserva específica que você deseja gerenciar.  

3. Em **ações**, selecione **gerenciar** para ir para o registro de reserva do cliente no portal do Azure. Na página de detalhes da reserva, siga as etapas abaixo para concluir tarefas.  

    | **Selecionar**   | **Para**    |
    |:-----------------------------|:-----------------|
    | **Visão geral**   | Exibir detalhes da reserva de um cliente, incluindo data de expiração, escopo e dados de utilização. **OBSERVAÇÃO** Selecione **Reembolso** para criar uma solicitação de suporte para obter um reembolso proporcional. Selecione **Trocar** para criar uma solicitação de suporte para trocar a parte não utilizada do seu termo de reserva.  
    | **Controle de acesso (IAM)**   | Gerencie o acesso às informações de reserva do cliente.|
    | **Configuration**   | Altere o escopo da reserva e/ou a assinatura do Azure à qual a reserva está associada.    |
    | **Propriedades**   | Exiba as propriedades da reserva e copie para a área de transferência a ID da reserva e a ID do pedido de reserva. **OBSERVAÇÃO** O suporte pode solicitar a ID da reserva e a ID do pedido da reserva quando você solicitar suporte em nome de um cliente.    |
    | **Nova solicitação de suporte**    | Solicite ajuda do Suporte da Microsoft.   |
 
## <a name="cancel-or-exchange-a-reservation"></a>Cancelar ou trocar uma reserva

Se, a qualquer momento, as necessidades dos negócios de um cliente mudarem, talvez desejam cancelar uma reserva e obter um reembolso ou trocar o valor de reembolso rateado da reserva a ser usado em relação ao preço de uma nova reserva.

Em ambos os cenários, a Microsoft reembolsa o valor para você para que você possa gerenciar as transações financeiras resultantes com seus clientes. A Microsoft não contata os clientes diretamente sobre cobrança, cancelamentos ou reembolsos.

### <a name="how-cancellations-work"></a>Como funcionam os cancelamentos

Os clientes podem solicitar o cancelamento de uma reserva a qualquer momento (valor de reembolso limitado a US$ 50.000 por ano). Cancelar uma reserva permite que o cliente retorne o valor dos meses restantes de uma reserva do Azure por um valor de encerramento antecipado. O saldo rateado restante, menos o valor da rescisão antecipada, é reembolsado à sua conta para que você possa reembolsar a conta do cliente. 

Veja abaixo detalhes e tarifas de cancelamento.


|**Data de cancelamento**<br> (dias)   |**Usage**    |**Crédito**  |**Encerramento antecipado**<br> taxa    |**Limite de reembolso** | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|5 ou menos                         | Não          | 100%       | Não                              | US$ 50.000   |
|5 ou menos                         | Sim         | Pro-rated  | Não                              | US$ 50.000   |
|Mais de 5                        | Não          | Pro-rated  | 12%                             | US$ 50.000   |
|Mais de 5                        | Sim         | Pro-rated  | 12%                             | US$ 50.000   |

### <a name="how-exchanges-work"></a>Como funcionam as trocas 

Se um cliente quiser comprar uma reserva diferente da que comprou originalmente de você, ele poderá solicitar uma troca. A troca de uma reserva pode ser uma alternativa atraente para cancelar uma reserva porque permite que o cliente use o valor de reembolso rateado em relação ao preço da nova reserva. 

O valor do reembolso rateado é creditado em sua conta para que você possa oferecer uma troca ao cliente.

## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>Solicitar um reembolso ou uma troca em nome de um cliente

Para registrar uma solicitação de suporte para reembolso ou troca em nome de seus clientes, você selecionará o cliente e a reserva no Partner Center e, em seguida, criará a solicitação de suporte no portal do Azure. 

>[!NOTE]
>Os agentes do Suporte da Microsoft para fornecer a ID da reserva e a ID do pedido da reserva. Você pode encontrar essas informações na página Propriedades **da** reserva no portal do Azure.

1. Para começar, selecione **Clientes no** menu Partner Center e, em seguida, selecione o cliente que deseja um reembolso. 

2. Na página de detalhes do cliente, selecione Reservas do **Azure** e, em seguida, selecione a reserva específica que o cliente deseja reembolsar.  

3. Em **Ações**, selecione **Reembolso** para ir para o registro de reserva do cliente no portal do Azure e iniciar uma solicitação de suporte.  

4. Na página **Nova solicitação de suporte**, siga as etapas abaixo para solicitar um reembolso. Selecione **Avançar** depois de cada etapa. 

   |**Step**                    |**Seleções**    |
   |:---------------------------|:-----------------|
   |**1 Noções básicas**                |Tipo de problema: Cobrança.  |
   |**2 Problema**               |Tipo de problema: Gerenciamento de reserva. Categoria: Trocas e reembolsos. |
   |**3 Informações de contato**   |Selecione suas preferências e insira as informações necessárias. 

5. Selecione **Criar** ao terminar.

## <a name="azure-reservations-resources"></a>Recursos de reservas do Azure

|**Para obter informações sobre**   |**Leia isto**    |
|:-----------------------------|:-----------------|
|Reservas do Azure na visão geral do CSP  | [Vender Instâncias Reservadas do Microsoft Azure](azure-reservations.md) |
|Comprar reservas do Azure para seus clientes no Partner Center   | [Comprar reservas do Azure](azure-reservations-buying.md) |
|Determinar o tamanho correto da VM e verificar o uso da VM do cliente   | [Dimensionamento de VM para uso máximo de reserva do Azure](azure-usage.md)   |
|Como comprar reservas do Azure usando a API do Partner Center | [Comprar Instâncias de VM Reservadas do Azure](/partner-center/develop/purchase-azure-reservations) na documentação do desenvolvedor do Partner Center   |
|Dando aos clientes permissão para comprar suas próprias reservas do Azure de uma assinatura que você comprou para eles. | [Dar aos clientes permissão para comprar suas próprias reservas do Azure](give-customers-permission.md)   |