---
title: Gerenciar reservas do Azure em nome dos seus clientes | Partner Center
Description: Purchasing and managing Azure reservations on behalf of your customers.
author: v-petand
keywords: Azure, reservas, gerenciar, cobrança, compra
ms.localizationpriority: medium
ms.openlocfilehash: 6b3fb1aed57b39976556851c007590743a805671
ms.sourcegitcommit: 1321f23b1a5be48a0a5dae6d52fd123ec9bacee2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/12/2018
ms.locfileid: "4562268"
---
# <a name="manage-microsoft-azure-reservations-on-behalf-of-your-customers"></a>Gerenciar reservas do Microsoft Azure em nome dos seus clientes

**Aplica-se a**

-  Partner Center
-  Portal do Microsoft Azure
-  Parceiros no CSP

Para gerenciar o pós-compra de reservas do Azure dos seus clientes, você vai selecionará o cliente e a reserva que você deseja gerenciar no Partner Center e, em seguida, faça alterações na reserva no portal do Azure. 

1. Para começar, selecione **os clientes** do seu menu Partner Center e, em seguida, selecione o cliente cujas reservas você deseja gerenciar. 

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
Quando os negócios dos seus clientes precisarem mudar, eles podem querer cancelar o valor de reembolso proporcional de uma reserva ou de uma troca a ser usado em relação ao preço de uma nova reserva. 

**Como funcionam os cancelamentos**

Os clientes podem cancelar uma reserva a qualquer momento (até US$50.000 por ano). O cancelamento permite que o cliente devolva os meses restantes de uma reserva do Azure para a Microsoft por uma taxa de término antecipado. O saldo restante proporcional, menos a taxa, será reembolsado à compra original do cliente. 

Veja a seguir para obter detalhes de cancelamento e taxas.

|**Data de cancelamento**<br> (dias)   |**Utilização**    |**Crédito**  |**Encerramento**<br> taxa    |**Limite de reembolso** | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|Menos de 5                       | Não          | 100%       | Não                              | US $ 50.000   |
|Menos de 5                       | Sim         | Proporcional  | Não                              | US $ 50.000   |
|Mais de 5                        | Não          | Proporcional  | 12%                             | US $ 50.000   |
|Mais de 5                        | Sim         | Proporcional  | 12%                             | US $ 50.000   |


**Como funcionam as trocas** 

Uma troca permite que um cliente receba um reembolso proporcional com base no tempo restante da reserva e aplique o valor do reembolso a uma nova reserva.   

## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>Solicitar um reembolso ou uma troca em nome de um cliente 

Para enviar uma solicitação de suporte para um reembolso ou uma troca em nome dos seus clientes, você selecionará o cliente e a reserva no Partner Center e, em seguida, criar a solicitação de suporte no portal do Azure. 

>[!NOTE]
>Os agentes do Suporte da Microsoft para fornecer a ID da reserva e a ID do pedido da reserva. Você pode encontrar essas informações na página **Propriedades** no portal do Azure. 

1. Para começar, selecione **os clientes** no menu Partner Center e, em seguida, selecione o cliente que deseja um reembolso. 

2. Na página de detalhes do cliente, selecione **Reservas do Azure** e, em seguida, selecione a reserva específica para a o cliente quer reembolso.  

3. Em **ações**, selecione **reembolso** para ir para registro de reserva do cliente no portal do Azure e iniciar uma solicitação de suporte.  

4. Na página **Nova solicitação de suporte**, siga as etapas abaixo para solicitar um reembolso. Selecione **Avançar** depois de cada etapa. 

|**Etapa**   |**Seleções**    |
|:-----------------------------|:-----------------|
|**1 Noções básicas**   |Tipo de problema: Cobrança.  |
|**2 Problema**   |Tipo de problema: Gerenciamento de reserva. Categoria: Trocas e reembolsos. |
|**3 Informações de contato**   |Selecione suas preferências e insira as informações necessárias. Selecione **Criar** ao terminar.   |

## <a name="azure-reservations-resources"></a>Recursos de reservas do Azure
|**Para obter informações sobre**   |**Leia isto**    |
|:-----------------------------|:-----------------|
|Reservas do Azure na visão geral do CSP  | [Vender instâncias reservadas do Microsoft Azure](azure-reservations.md) |
|Como comprar reservas do Azure para seus clientes no Partner Center   |[Comprar reservas do Azure](azure-reservations-buying.md) |
|Determinar o tamanho correto da VM e verificar o uso da VM do cliente   |[Dimensionamento de VM para uso máximo de reserva do Azure](azure-usage.md)   |
|Como comprar reservas do Azure usando a API do Partner Center | [Comprar Instâncias de VM Reservadas do Azure](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) na documentação do desenvolvedor do Partner Center

