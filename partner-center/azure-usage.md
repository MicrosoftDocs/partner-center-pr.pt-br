---
title: Dimensionamento da VM do Azure para uso máximo de reserva
description: Saiba como dimensionar uma VM (máquina virtual) para as necessidades de computação de seus clientes ao comprar Microsoft Azure reservas para elas.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 08/06/2020
ms.openlocfilehash: 14d488091227e30909b3d41af0684494a8b55de7
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149444"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>Dimensionamento de VM do Microsoft Azure para uso máximo de reserva do Azure

**Funções apropriadas**: agente de administração | Agente de vendas

Este artigo explica como dimensionar uma VM (máquina virtual) para as necessidades de computação de seus clientes ao comprar Microsoft Azure reservas para elas.
 
> [!NOTE]
> Este artigo se aplica somente a parceiros no programa CSP (provedor de soluções na nuvem). Os clientes que usam outros tipos de assinaturas (como pagamento conforme o uso, individuais, contrato de cliente da Microsoft ou assinaturas de Contrato Enterprise) devem ler [essa documentação de reservas do Azure](/azure/cost-management-billing/reservations).

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>Determinar o tamanho da VM para a reserva do Azure de um cliente

Ao comprar Microsoft Azure reservas em nome de seus clientes, você precisará escolher uma VM (máquina virtual) dimensionada para atender às necessidades de computação do cliente. Você pode encontrar essas informações usando um destes métodos:

- API de utilização do Azure
- O Portal do Azure
- Azure PowerShell
- A API do Azure Resource Manager (ARM)

As instruções para o uso de cada um desses métodos estão listadas a seguir. Depois que você comprar uma reserva, o desconto da reserva será aplicado automaticamente em máquinas virtuais que correspondam aos atributos e à quantidade da reserva. Você não precisa atribuir a reserva a uma VM.

>[!NOTE]
>Os descontos de reserva não se aplicam às VMs clássicas ou promocionais.

>[!IMPORTANT]
>Para identificar o tipo e o tamanho da VM a ser comprada em nome de seu cliente, você deverá usar um dos métodos descritos abaixo já que o tipo de série de VM não é exibido corretamente nos arquivos de reconciliação do Partner Center.

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a>Obter informações de dimensionamento de VM usando a API de utilização do Azure

1. Use o valor do atributo ServiceType desde additionalInfo na resposta da API para identificar o tamanho da VM a ser comprada.

2. Para obter mais informações, consulte [obter os registros de utilização do cliente para o Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) na API do [Partner Center](/partner-center/develop/).

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a>Obter informações de dimensionamento de VM usando o portal do Microsoft Azure

1. No Partner Center, vá para a página de seus **clientes** .

2. Localize o cliente que deseja comprar as reservas de VM do Azure e, em seguida, selecione a seta para baixo para expandir as informações do cliente. Selecione **portal de gerenciamento do Microsoft Azure** para abrir o registro do cliente no portal do Azure.

3. Selecione **Máquinas virtuais** no menu do portal e então selecione a VM para a qual você deseja comprar uma reserva.

4. Na página de detalhes da VM, localize as informações de tamanho e região, conforme ilustrado abaixo, e use essas informações para comprar a reserva no Partner Center.  

   :::image type="content" source="images/usage1.png" alt-text="Informações de tamanho e região na página de detalhes":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a>Obter informações de dimensionamento de VM usando o Microsoft Azure PowerShell

Use as informações na imagem abaixo para obter a localização e o tamanho da VM para a qual você deseja comprar uma reserva. 

:::image type="content" source="images/usage2.png" alt-text="Local e tamanho da VM":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a>Obter informações de dimensionamento de VM usando a API do Azure Resource Manager (ARM)

1. Usando o ARMClient ou as APIs ARM, chame o cliente ARM para a VM para a qual você deseja comprar uma reserva.

2. /subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01

3. A chamada retorna os valores de **vmSize** e **location**, como ilustrado abaixo.

    :::image type="content" source="images/usage3.png" alt-text="valor de vmSize":::
    :::image type="content" source="images/usage4.png" alt-text="valor da localização":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>Verificar o desconto de uso e de reserva de VM do Azure

Depois de comprar uma instância de VM reservada do Azure em nome de um cliente, o desconto para pagar pelo espaço da VM com antecedência é aplicado automaticamente às máquinas virtuais que correspondem aos atributos e à quantidade da reserva do cliente.

Você pode verificar o uso de reserva do cliente e ver a quais máquinas virtuais os descontos de reserva são aplicados usando um dos seguintes métodos:

- O portal do Azure
- API de utilização do Azure

As instruções para o uso de cada um desses métodos estão listadas a seguir.

>[!NOTE]
>Somente a API de utilização do Azure mostra a qual máquina virtual o desconto está sendo aplicado.  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>Verifique o uso de reserva do cliente no portal do Microsoft Azure

1. No Partner Center, vá para a **página Clientes.**

2. Encontre o cliente cujo desconto de reserva e uso você deseja verificar e, em seguida, selecione a seta para baixo para expandir as informações do cliente. Selecione **Portal de Gerenciamento do Microsoft Azure** para abrir o registro do cliente no portal do Azure.
3. Selecione **Reservas** no menu do portal e então selecione a reserva cujo uso você deseja verificar.
4. Na página **Visão** geral, verifique o grafo de utilização da reserva, que mostra quanto da reserva foi aplicada às máquinas virtuais.

    >[!NOTE]
    >Os dados de utilização podem ser atrasados em até 8 horas.

    a. Se a utilização da reserva for de 100%, seu cliente está recebendo todas as economias possíveis que a compra de reserva pode fornecer.
    b. Se o uso da reserva for 0%, o desconto não será aplicado a nenhuma máquina virtual.
    c. Se o uso da reserva estiver entre 1% e 99%, haverá benefícios não usuários.

5. Para evitar essa situação, determine o tamanho correto da VM para dar suporte às necessidades de computação do cliente antes de fazer a compra.

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>Verificar o uso de reserva do cliente com a API de utilização do Azure

>[!NOTE]
>Somente a API de utilização do Azure mostra a qual máquina virtual o desconto está sendo aplicado.  

Você pode obter dados de uso da reserva com a API de utilização do Azure para verificar se o cliente está recebendo o desconto da reserva e para ver a quais VMs (máquinas virtuais) o desconto é aplicado. Compare o Exemplo A com o Exemplo B para ver como verificar o uso de reserva de um cliente.

:::image type="content" source="images/usage5.png" alt-text="Exemplos de uso de reserva":::

- A reservationId identifica a reserva do Azure que foi usada para aplicar o desconto à VM.
- consumptionMeter é a MeterId para a VM que tem o desconto da reserva aplicado a ela.
- O ReservationMeter mostra o custo de US$ 0 desde que o desconto da reserva foi aplicado.

Para obter mais informações, consulte Obter registros de utilização de um cliente para [o Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) na [API Partner Center .](/partner-center/develop/)

>[!IMPORTANT]
>Os custos de software, como o Microsoft Windows Server, não estão incluídos no preço de uma reserva de VM e aparecerão como itens de linha separados no registro do pedido e em sua fatura. No entanto, se um cliente tiver o Benefício de Uso Híbrido do Azure, os custos de software não serão aplicados. Para obter mais informações, consulte [Custos de software do Windows não incluídos com Instâncias Reservadas](/azure/billing/billing-reserved-instance-windows-software-costs).  

## <a name="next-steps"></a>Próximas etapas

|**Para obter informações sobre**   |**Leia isto**    |
|:-----------------------------|:-----------------|
|Reservas do Azure na visão geral do CSP  | [Vender Instâncias de VM Reservadas do Microsoft Azure](azure-reservations.md)
|Comprar reservas do Azure para seus clientes no Partner Center   | [Comprar reservas do Azure](azure-reservations-buying.md)
|Gerenciando reservas do Azure no Partner Center | [Gerenciando reservas do Azure no Partner Center](azure-reservations-manage.md)
|Como comprar reservas do Azure no portal do Azure | [Pagar antecipadamente por máquinas virtuais com Instâncias de VM Reservadas do Azure](/azure/virtual-machines/windows/prepay-reserved-vm-instances) na Ajuda do Azure |
|Como gerenciar reservas do Azure no portal do Azure   | [Gerenciar instâncias de VM reservadas](/azure/billing/billing-manage-reserved-vm-instance) na Ajuda do Azure  |
|Como comprar reservas do Azure usando a API do Partner Center | [Comprar Instâncias de VM Reservadas do Azure](/partner-center/develop/purchase-azure-reservations) na documentação do desenvolvedor do Partner Center   |
|Dando aos clientes permissão para comprar suas próprias reservas do Azure de uma assinatura que você comprou para eles. | [Dar aos clientes permissão para comprar suas próprias reservas do Azure](give-customers-permission.md)   |