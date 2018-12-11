---
title: Gerenciar reservas do Azure em nome dos seus clientes | Partner Center
ms.topic: article
ms.date: 10/29/2018
Description: To manage your customers’ Azure reservations post-purchase, you’ll select the customer and reservation you want to manage in Partner Center, and then make changes to the reservation in the Azure portal.
author: v-petand
ms.author: v-petand
keywords: Azure, reservas, gerenciar, cobrança, comprar, cancelar, exchange, taxa de término antecipado
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 7096efb34f8c72d3c8dc724332dd031a180d0636
ms.sourcegitcommit: 777225c8bf16e4a8811a9d88aceb45fcba1cd959
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2018
ms.locfileid: "8917708"
---
# <a name="manage-microsoft-azure-reservations-on-behalf-of-your-customers"></a>Gerenciar reservas do Microsoft Azure em nome dos seus clientes

**Aplica-se a**

-  Partner Center
-  Portal do Microsoft Azure
-  Parceiros no CSP

Para gerenciar o pós-compra de reservas do Azure dos seus clientes, você vai selecionará o cliente e a reserva que você deseja gerenciar no Partner Center e, em seguida, faça alterações na reserva no portal do Azure. 

1. Para começar, selecione **os clientes** no menu Partner Center e, em seguida, selecione o cliente cujas reservas você deseja gerenciar. 

2. No menu de página de detalhes do cliente, selecione **reservas do Azure** e, em seguida, selecione a reserva específica que você deseja gerenciar.  

3. Em **Ações**, selecione **Gerenciar** para ir para registro de reserva do cliente no portal do Azure. Na página de detalhes da reserva, siga as etapas abaixo para concluir tarefas.  

    | **Selecionar**   | **Para**    |
    |:-----------------------------|:-----------------|
    | **Visão geral**   | Exiba detalhes da reserva de um cliente, incluindo data de validade, escopo e dados de utilização. **OBSERVAÇÃO** Selecione **Reembolso** para criar uma solicitação de suporte para obter um reembolso proporcional. Selecione **Trocar** para criar uma solicitação de suporte para trocar a parte não utilizada do seu termo de reserva.  
    | **Controle de Acesso (IAM)**   | Gerencie o acesso às informações de reserva do cliente.|
    | **Configuração**   | Altere o escopo da reserva e/ou a assinatura do Azure a qual a reserva está associada.    |
    | **Propriedades**   | Exiba as propriedades da reserva e copie para a área de transferência a ID da reserva e a ID do pedido da reserva. **OBSERVAÇÃO** O suporte pode solicitar a ID da reserva e a ID do pedido da reserva quando você solicitar suporte em nome de um cliente.    |
    | **Nova solicitação de suporte**    | Solicite ajuda do Suporte da Microsoft.   |
 
## <a name="cancel-or-exchange-a-reservation"></a>Cancelar ou trocar uma reserva 

Se a qualquer momento negócios do cliente mudam, eles podem querer cancelar uma reserva e obter um reembolso ou troca um reembolso proporcional valor a ser usado em relação ao preço de uma nova reserva.

Em ambos os cenários, Microsoft reembolsos a quantidade para você, para que, em seguida, você pode gerenciar as transações financeiras resultantes com seus clientes. Microsoft não entre em contato com os clientes diretamente sobre cobrança, cancelamentos ou reembolsos.   
 

**Como funcionam os cancelamentos**

Os clientes podem solicitar para cancelar uma reserva a qualquer momento (valor do reembolso coberta em US $50.000 por ano). Cancelar uma reserva permite que o cliente devolva a quantidade dos meses restantes de uma reserva do Azure para uma taxa de término antecipado. O saldo restante proporcional, menos a taxa de término antecipado, será reembolsado à sua conta para que você pode reembolsar a conta do cliente. 

Veja a seguir para obter detalhes de cancelamento e taxas.


|**Data de cancelamento**<br> (dias)   |**Utilização**    |**Crédito**  |**Término antecipado**<br> taxa    |**Limite de reembolso** | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|5 ou menos                         | Não          | 100%       | Não                              | US $ 50.000   |
|5 ou menos                         | Sim         | Proporcional  | Não                              | US $ 50.000   |
|Mais de 5                        | Não          | Proporcional  | 12%                             | US $ 50.000   |
|Mais de 5                        | Sim         | Proporcional  | 12%                             | US $ 50.000   |


**Como funcionam as trocas** 

Se um cliente quiser comprar uma reserva diferente daquele que eles compraram originalmente de você, eles podem solicitar uma troca. Trocar uma reserva pode ser uma alternativa atraente para cancelar uma reserva, porque permite que o cliente a usar o valor do reembolso proporcional em relação ao preço da nova reserva. 

O valor do reembolso proporcional será creditado em sua conta para que você pode oferecer ao cliente uma troca.


## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>Solicitar um reembolso ou uma troca em nome de um cliente 

Para enviar uma solicitação de suporte para um reembolso ou uma troca em nome dos seus clientes, você selecionará o cliente e a reserva no Partner Center e, em seguida, criar a solicitação de suporte no portal do Azure. 

>[!NOTE]
>Os agentes do Suporte da Microsoft para fornecer a ID da reserva e a ID do pedido da reserva. Você pode encontrar essas informações na página **Propriedades** no portal do Azure. 

1. Para começar, selecione **os clientes** no menu Partner Center e, em seguida, selecione o cliente que deseja um reembolso. 

2. Na página de detalhes do cliente, selecione **Reservas do Azure** e, em seguida, selecione a reserva específica para a o cliente quer reembolso.  

3. Em **ações**, selecione **reembolso** para ir para registro de reserva do cliente no portal do Azure e iniciar uma solicitação de suporte.  

4. Na página **Nova solicitação de suporte**, siga as etapas abaixo para solicitar um reembolso. Selecione **Avançar** depois de cada etapa. 

    |**Etapa**                    |**Seleções**    |
    |:---------------------------|:-----------------|
    |**1 Noções básicas**                |Tipo de problema: Cobrança.  |
    |**2 Problema**               |Tipo de problema: Gerenciamento de reserva. Categoria: Trocas e reembolsos. |
    |**3 Informações de contato**   |Selecione suas preferências e insira as informações necessárias. 

5.  Selecione **Criar** ao terminar.

## <a name="azure-reservations-resources"></a>Recursos de reservas do Azure
|**Para obter informações sobre**   |**Leia isto**    |
|:-----------------------------|:-----------------|
|Reservas do Azure na visão geral do CSP  | [Vender instâncias reservadas do Microsoft Azure](azure-reservations.md) |
|Como comprar reservas do Azure para seus clientes no Partner Center   |[Comprar reservas do Azure](azure-reservations-buying.md) |
|Determinar o tamanho correto da VM e verificar o uso da VM do cliente   |[Dimensionamento de VM para uso máximo de reserva do Azure](azure-usage.md)   |
|Como comprar reservas do Azure usando a API do Partner Center | [Comprar Instâncias de VM Reservadas do Azure](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) na documentação do desenvolvedor do Partner Center

