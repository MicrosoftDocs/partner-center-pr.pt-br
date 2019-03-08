---
title: Gerenciar reservas do Azure em nome dos seus clientes | Partner Center
ms.topic: article
ms.date: 10/29/2018
Description: Para gerenciar a pós-compra de de reservas do Azure dos seus clientes, você vai selecionar o cliente e a reserva que você deseja gerenciar no Partner Center e, em seguida, fazer alterações à reserva no portal do Azure.
author: LauraBrenner
ms.author: v-petand
keywords: Azure, reservas, gerenciar, cobrança, compra, cancelar, exchange, taxa de rescisão antecipada
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: de1846b6259764b40059ece1d311e5f63587a525
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2019
ms.locfileid: "57584499"
---
# <a name="manage-microsoft-azure-reservations-on-behalf-of-your-customers"></a>Gerenciar reservas do Microsoft Azure em nome dos seus clientes

**Aplica-se a**

-  Partner Center
-  Portal do Microsoft Azure
-  Parceiros no CSP

Para gerenciar a pós-compra de de reservas do Azure dos seus clientes, você vai selecionar o cliente e a reserva que você deseja gerenciar no Partner Center e, em seguida, fazer alterações à reserva no portal do Azure. 

1. Para começar, selecione **clientes** no menu do Partner Center e, em seguida, selecione o cliente cujas reservas você deseja gerenciar. 

2. No menu da página de detalhes do cliente, selecione **Reservas do Azure** e, em seguida, selecione a reserva específica que você deseja gerenciar.  

3. Em **Ações**, selecione **Gerenciar** para ir para registro de reserva do cliente no portal do Azure. Na página de detalhes da reserva, siga as etapas abaixo para concluir tarefas.  

    | **Select**   | **Para**    |
    |:-----------------------------|:-----------------|
    | **Visão geral**   | Exiba detalhes da reserva de um cliente, incluindo data de validade, escopo e dados de utilização. **OBSERVAÇÃO** Selecione **Reembolso** para criar uma solicitação de suporte para obter um reembolso proporcional. Selecione **Trocar** para criar uma solicitação de suporte para trocar a parte não utilizada do seu termo de reserva.  
    | **Controle de acesso (IAM)**   | Gerencie o acesso às informações de reserva do cliente.|
    | **Configuração**   | Altere o escopo da reserva e/ou a assinatura do Azure a qual a reserva está associada.    |
    | **Propriedades**   | Exiba as propriedades da reserva e copie para a área de transferência a ID da reserva e a ID do pedido da reserva. **OBSERVAÇÃO** O suporte pode solicitar a ID da reserva e a ID do pedido da reserva quando você solicitar suporte em nome de um cliente.    |
    | **Nova solicitação de suporte**    | Solicite ajuda do Suporte da Microsoft.   |
 
## <a name="cancel-or-exchange-a-reservation"></a>Cancelar ou trocar uma reserva 

Se a qualquer momento as do cliente necessidades comerciais mudarem, eles talvez queira cancelar uma reserva e obter um reembolso ou quantidade de reembolso proporcional de uma reserva a ser usado para o preço de uma nova reserva do exchange.

Em ambos os cenários, o Microsoft reembolsos a quantidade para você, para que, em seguida, você pode gerenciar as transações financeiras resultantes com seus clientes. Microsoft não entre em contato com clientes diretamente sobre cobrança, cancelamentos ou reembolsos.   
 

**Como funcionam os cancelamentos**

Os clientes podem solicitar para cancelar uma reserva a qualquer momento (quantidade de reembolso limitado a US $50.000 por ano). Cancelar uma reserva permite que o cliente retornar o valor dos meses restantes de uma reserva do Azure para uma taxa de rescisão antecipada. O balanço proporcional restante, menos a taxa de rescisão antecipada, será reembolsado em sua conta para que o reembolso de conta do cliente. 

Veja abaixo os detalhes de cancelamento e taxas.


|**Data de cancelamento**<br> (dias)   |**Uso**    |**Crédito**  |**Término antecipado**<br> taxa    |**Limite de reembolso** | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|5 ou menos                         | Não          | 100%       | Não                              | US $50.000   |
|5 ou menos                         | Sim         | Proporcional  | Não                              | US $50.000   |
|Mais de 5                        | Não          | Proporcional  | 12%                             | US $50.000   |
|Mais de 5                        | Sim         | Proporcional  | 12%                             | US $50.000   |


**Como funcionam as trocas de** 

Se um cliente deseja comprar uma reserva diferente daquela que eles compraram originalmente por você, eles podem solicitar uma troca. Troca de uma reserva pode ser uma alternativa atraente para cancelar uma reserva porque ela permite que o cliente usar a quantidade de reembolso proporcional para o preço da nova reserva. 

A quantidade de reembolso proporcional é creditada para sua conta, de modo que você pode oferecer ao cliente uma troca.


## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>Solicitar um reembolso ou uma troca em nome de um cliente 

Para arquivar uma solicitação de suporte para um exchange ou o reembolso em nome de seus clientes, você vai selecionar o cliente e a reserva no Partner Center e, em seguida, criar a solicitação de suporte no portal do Azure. 

>[!NOTE]
>Os agentes do Suporte da Microsoft para fornecer a ID da reserva e a ID do pedido da reserva. Você pode encontrar essas informações na página **Propriedades** no portal do Azure. 

1. Para começar, selecione **clientes** no menu do Partner Center e, em seguida, selecione o cliente que deseja um reembolso. 

2. Na página de detalhes do cliente, selecione **Reservas do Azure** e, em seguida, selecione a reserva específica para a o cliente quer reembolso.  

3. Em **Ações**, selecione **Reembolso** para ir para registro de reserva do cliente no portal do Azure e inicie uma solicitação de suporte.  

4. Na página **Nova solicitação de suporte**, siga as etapas abaixo para solicitar um reembolso. Selecione **Avançar** depois de cada etapa. 

    |**Etapa**                    |**Seleções**    |
    |:---------------------------|:-----------------|
    |**Noções básicas 1**                |Tipo de problema: Cobrança.  |
    |**Problema 2**               |Tipo de problema: Gerenciamento de reserva. Categoria: Trocas e os reembolsos. |
    |**Informações de contato de 3**   |Selecione suas preferências e insira as informações necessárias. 

5.  Selecione **Criar** ao terminar.

## <a name="azure-reservations-resources"></a>Recursos de reservas do Azure
|**Para obter informações sobre**   |**Leia isto**    |
|:-----------------------------|:-----------------|
|Reservas do Azure na visão geral do CSP  | [Vende instâncias reservadas do Microsoft Azure](azure-reservations.md) |
|Comprar reservas do Azure para seus clientes no Partner Center   |[Comprar reservas do Azure](azure-reservations-buying.md) |
|Determinar o tamanho correto da VM e verificar o uso da VM do cliente   |[Dimensionamento da VM para uso de máximo de reserva do Azure](azure-usage.md)   |
|Como comprar reservas do Azure usando a API do Partner Center | [Comprar Instâncias de VM Reservadas do Azure](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) na documentação do desenvolvedor do Partner Center

