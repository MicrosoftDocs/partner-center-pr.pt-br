---
title: Gerenciar reservas do Azure em nome dos seus clientes | Partner Center
ms.topic: article
ms.date: 11/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Saiba como gerenciar reservas do Azure em nome de um cliente, incluindo como cancelar uma reserva, trocar uma reserva ou solicitar um reembolso.
author: LauraBrenner
ms.author: labrenne
keywords: Azure, reservas, gerenciar, cobrança, compra, cancelamento, troca, taxa de encerramento antecipado
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: eedfe20cea239918e5ece6f10b2b5f5988da9c50
ms.sourcegitcommit: c793c1b61f50fc0b0a12c95cedd9f57b31703093
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2019
ms.locfileid: "74722276"
---
# <a name="manage-microsoft-azure-reservations-on-behalf-of-your-customers"></a>Gerenciar Reservas do Microsoft Azure em nome de seus clientes

**Aplica-se a**

- Partner Center
- Portal do Microsoft Azure 
- Parceiros no CSP

**Funções apropriadas**

- Agente administrativo
- Administração global
- Agente de suporte técnico
- Agente de vendas
- Administrador de gerenciamento de usuário

Para gerenciar as reservas do Azure de seus clientes após a compra, você selecionará o cliente e a reserva que deseja gerenciar no Partner Center e, em seguida, fará alterações na reserva no portal do Azure.

1. Para começar, selecione **clientes** no menu do centro de parceiros e, em seguida, selecione o cliente cujas reservas você deseja gerenciar. 

2. No menu da página de detalhes do cliente, selecione **reservas do Azure** e, em seguida, selecione a reserva específica que você deseja gerenciar.  

3. Em **ações**, selecione **gerenciar** para ir para o registro de reserva do cliente no portal do Azure. Na página de detalhes da reserva, siga as etapas abaixo para concluir tarefas.  

    | **Não**   | **Para**    |
    |:-----------------------------|:-----------------|
    | **Visão geral**   | Exibir detalhes da reserva de um cliente, incluindo data de expiração, escopo e dados de utilização. **OBSERVAÇÃO** Selecione **Reembolso** para criar uma solicitação de suporte para obter um reembolso proporcional. Selecione **Trocar** para criar uma solicitação de suporte para trocar a parte não utilizada do seu termo de reserva.  
    | **Controle de acesso (IAM)**   | Gerencie o acesso às informações de reserva do cliente.|
    | **Configuração**   | Altere o escopo da reserva e/ou a assinatura do Azure à qual a reserva está associada.    |
    | **Propriedades**   | Exiba as propriedades da reserva e copie para a área de transferência a ID da reserva e a ID do pedido de reserva. **OBSERVAÇÃO** O suporte pode solicitar a ID da reserva e a ID do pedido da reserva quando você solicitar suporte em nome de um cliente.    |
    | **Nova solicitação de suporte**    | Solicite ajuda do Suporte da Microsoft.   |
 
## <a name="cancel-or-exchange-a-reservation"></a>Cancelar ou trocar uma reserva 

Se, a qualquer momento, as necessidades dos negócios de um cliente mudarem, talvez desejam cancelar uma reserva e obter um reembolso ou trocar o valor de reembolso rateado da reserva a ser usado em relação ao preço de uma nova reserva.

Em ambos os cenários, a Microsoft refinancia o valor a você para que você possa gerenciar as transações financeiras resultantes com seus clientes. A Microsoft não entra em contato com os clientes diretamente sobre cobrança, cancelamentos ou reembolsos.


**Como o cancelamento funciona**

Os clientes podem solicitar a cancelamento de uma reserva a qualquer momento (valor de reembolso limitado em $50000 por ano). O cancelamento de uma reserva permite que o cliente retorne o valor dos meses restantes de uma reserva do Azure para uma taxa de término antecipado. O saldo rateado restante, menos a taxa de término antecipado, é reembolsado em sua conta para que você possa reembolsar a conta do cliente. 

Consulte abaixo para obter detalhes e taxas de cancelamento.


|**Data do cancelamento**<br> dias   |**Usos**    |**Crédito**  |**Encerramento antecipado**<br> taxa    |**Limite de reembolso** | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|5 ou menos                         | Não          | 100%       | Não                              | US $ $50000   |
|5 ou menos                         | Sim         | Proporcional  | Não                              | US $ $50000   |
|Mais de 5                        | Não          | Proporcional  | 12                             | US $ $50000   |
|Mais de 5                        | Sim         | Proporcional  | 12                             | US $ $50000   |


**Como as trocas funcionam** 

Se um cliente quiser comprar uma reserva diferente daquela que originalmente comprou, poderá solicitar uma troca. A troca de uma reserva pode ser uma alternativa atraente para cancelar uma reserva, pois permite que o cliente use o valor de reembolso rateado em direção ao preço da nova reserva. 

O valor de reembolso rateado é creditado em sua conta para que você possa oferecer ao cliente uma troca.


## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>Solicitar um reembolso ou uma troca em nome de um cliente 

Para arquivar uma solicitação de suporte para um reembolso ou troca em nome de seus clientes, você selecionará o cliente e a reserva no Partner Center e criará a solicitação de suporte no portal do Azure. 

>[!NOTE]
>Os agentes do Suporte da Microsoft para fornecer a ID da reserva e a ID do pedido da reserva. Você pode encontrar essas informações na página de **Propriedades** da reserva no portal do Azure. 

1. Para começar, selecione **clientes** no menu do centro de parceiros e, em seguida, selecione o cliente que deseja um reembolso. 

2. Na página de detalhes do cliente, selecione **reservas do Azure** e, em seguida, selecione a reserva específica que o cliente deseja reembolsar.  

3. Em **ações**, selecione **reembolso** para ir para o registro de reserva do cliente no portal do Azure e iniciar uma solicitação de suporte.  

4. Na página **Nova solicitação de suporte**, siga as etapas abaixo para solicitar um reembolso. Selecione **Avançar** depois de cada etapa. 

    |**Etapa**                    |**Seleções**    |
    |:---------------------------|:-----------------|
    |**1 noções básicas**                |Tipo de problema: Cobrança.  |
    |**2 problema**               |Tipo de problema: Gerenciamento de reserva. Categoria: Trocas e reembolsos. |
    |**3 informações de contato**   |Selecione suas preferências e insira as informações necessárias. 

5.  Selecione **Criar** ao terminar.

## <a name="azure-reservations-resources"></a>Recursos de reservas do Azure
|**Para obter informações sobre**   |**Leia isto**    |
|:-----------------------------|:-----------------|
|Reservas do Azure na visão geral do CSP  | [Vender Microsoft Azure instâncias reservadas](azure-reservations.md) |
|Comprando reservas do Azure para seus clientes no Partner Center   |[Comprar reservas do Azure](azure-reservations-buying.md) |
|Determinar o tamanho correto da VM e verificar o uso da VM do cliente   |[Dimensionamento de VM para uso máximo de reserva do Azure](azure-usage.md)   |
|Como comprar reservas do Azure usando a API do Partner Center | [Comprar Instâncias de VM Reservadas do Azure](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) na documentação do desenvolvedor do Partner Center

