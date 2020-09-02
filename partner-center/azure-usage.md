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
ms.openlocfilehash: ba24376bad1d04fcbc9f02d442f0cba7e6354bd3
ms.sourcegitcommit: c40f826bb1143555bf3a1c2c806c34024f0f6019
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/02/2020
ms.locfileid: "89367090"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="38eb8-103">Dimensionamento de VM do Microsoft Azure para uso máximo de reserva do Azure</span><span class="sxs-lookup"><span data-stu-id="38eb8-103">Microsoft Azure VM sizing for maximum reservation usage</span></span>

<span data-ttu-id="38eb8-104">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="38eb8-104">**Applies to**</span></span>

- <span data-ttu-id="38eb8-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="38eb8-105">Partner Center</span></span>
- <span data-ttu-id="38eb8-106">Portal do Azure</span><span class="sxs-lookup"><span data-stu-id="38eb8-106">Azure portal</span></span>
- <span data-ttu-id="38eb8-107">Parceiros no programa CSP</span><span class="sxs-lookup"><span data-stu-id="38eb8-107">Partners in the CSP program</span></span>
 
> [!NOTE]
> <span data-ttu-id="38eb8-108">Este artigo se aplica somente a parceiros no programa CSP (provedor de soluções na nuvem).</span><span class="sxs-lookup"><span data-stu-id="38eb8-108">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="38eb8-109">Os clientes que usam outros tipos de assinaturas (como pagamento conforme o uso, individuais, contrato de cliente da Microsoft ou assinaturas de Enterprise Agreement) devem ler [essa documentação de reservas do Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations).</span><span class="sxs-lookup"><span data-stu-id="38eb8-109">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](https://docs.microsoft.com/azure/cost-management-billing/reservations).</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="38eb8-110">Determinar o tamanho da VM para a reserva do Azure de um cliente</span><span class="sxs-lookup"><span data-stu-id="38eb8-110">Determine the VM size for a customer's Azure reservation</span></span>

<span data-ttu-id="38eb8-111">Ao comprar Microsoft Azure reservas em nome de seus clientes, você precisará escolher uma VM (máquina virtual) dimensionada para atender às necessidades de computação do cliente.</span><span class="sxs-lookup"><span data-stu-id="38eb8-111">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span></span> <span data-ttu-id="38eb8-112">Você pode encontrar essas informações usando um destes métodos:</span><span class="sxs-lookup"><span data-stu-id="38eb8-112">You can find this information using one of these methods:</span></span>

- <span data-ttu-id="38eb8-113">API de utilização do Azure</span><span class="sxs-lookup"><span data-stu-id="38eb8-113">Azure utilization API</span></span>
- <span data-ttu-id="38eb8-114">O Portal do Azure</span><span class="sxs-lookup"><span data-stu-id="38eb8-114">The Azure portal</span></span>
- <span data-ttu-id="38eb8-115">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="38eb8-115">Azure PowerShell</span></span>
- <span data-ttu-id="38eb8-116">A API do Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="38eb8-116">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="38eb8-117">As instruções para o uso de cada um desses métodos estão listadas a seguir.</span><span class="sxs-lookup"><span data-stu-id="38eb8-117">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="38eb8-118">Depois que você comprar uma reserva, o desconto da reserva será aplicado automaticamente em máquinas virtuais que correspondam aos atributos e à quantidade da reserva.</span><span class="sxs-lookup"><span data-stu-id="38eb8-118">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="38eb8-119">Você não precisa atribuir a reserva a uma VM.</span><span class="sxs-lookup"><span data-stu-id="38eb8-119">You don't need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="38eb8-120">Os descontos de reserva não se aplicam às VMs clássicas ou promocionais.</span><span class="sxs-lookup"><span data-stu-id="38eb8-120">Reservation discounts don't apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="38eb8-121">Para identificar o tipo e o tamanho da VM a ser comprada em nome de seu cliente, você deverá usar um dos métodos descritos abaixo já que o tipo de série de VM não é exibido corretamente nos arquivos de reconciliação do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="38eb8-121">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a><span data-ttu-id="38eb8-122">Obter informações de dimensionamento de VM usando a API de utilização do Azure</span><span class="sxs-lookup"><span data-stu-id="38eb8-122">Get VM sizing information using the Azure utilization API</span></span>

1. <span data-ttu-id="38eb8-123">Use o valor do atributo ServiceType desde additionalInfo na resposta da API para identificar o tamanho da VM a ser comprada.</span><span class="sxs-lookup"><span data-stu-id="38eb8-123">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span>

2. <span data-ttu-id="38eb8-124">Para obter mais informações, consulte [obter os registros de utilização do cliente para o Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) na API do [Partner Center](https://docs.microsoft.com/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="38eb8-124">For more information, see [Get a customer's utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span>

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a><span data-ttu-id="38eb8-125">Obter informações de dimensionamento de VM usando o portal do Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="38eb8-125">Get VM sizing information using the Microsoft Azure portal</span></span>

1. <span data-ttu-id="38eb8-126">No Partner Center, vá para a página de seus **clientes** .</span><span class="sxs-lookup"><span data-stu-id="38eb8-126">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="38eb8-127">Localize o cliente que deseja comprar as reservas de VM do Azure e, em seguida, selecione a seta para baixo para expandir as informações do cliente.</span><span class="sxs-lookup"><span data-stu-id="38eb8-127">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="38eb8-128">Selecione **portal de gerenciamento do Microsoft Azure** para abrir o registro do cliente no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="38eb8-128">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>

3. <span data-ttu-id="38eb8-129">Selecione **Máquinas virtuais** no menu do portal e então selecione a VM para a qual você deseja comprar uma reserva.</span><span class="sxs-lookup"><span data-stu-id="38eb8-129">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span>

4. <span data-ttu-id="38eb8-130">Na página de detalhes da VM, localize as informações de tamanho e região, conforme ilustrado abaixo, e use essas informações para comprar a reserva no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="38eb8-130">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

   :::image type="content" source="images/usage1.png" alt-text="Informações de tamanho e região na página de detalhes":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a><span data-ttu-id="38eb8-132">Obter informações de dimensionamento de VM usando o Microsoft Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="38eb8-132">Get VM sizing information using Microsoft Azure PowerShell</span></span>

<span data-ttu-id="38eb8-133">Use as informações na imagem abaixo para obter a localização e o tamanho da VM para a qual você deseja comprar uma reserva.</span><span class="sxs-lookup"><span data-stu-id="38eb8-133">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

:::image type="content" source="images/usage2.png" alt-text="Local e tamanho da VM":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a><span data-ttu-id="38eb8-135">Obter informações de dimensionamento de VM usando a API do Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="38eb8-135">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>

1. <span data-ttu-id="38eb8-136">Usando o ARMClient ou as APIs ARM, chame o cliente ARM para a VM para a qual você deseja comprar uma reserva.</span><span class="sxs-lookup"><span data-stu-id="38eb8-136">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2. <span data-ttu-id="38eb8-137">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span><span class="sxs-lookup"><span data-stu-id="38eb8-137">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3. <span data-ttu-id="38eb8-138">A chamada retorna os valores de **vmSize** e **location**, como ilustrado abaixo.</span><span class="sxs-lookup"><span data-stu-id="38eb8-138">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    :::image type="content" source="images/usage3.png" alt-text="valor de vmSize":::
    :::image type="content" source="images/usage4.png" alt-text="valor da localização":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="38eb8-141">Verificar o desconto de uso e de reserva de VM do Azure</span><span class="sxs-lookup"><span data-stu-id="38eb8-141">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="38eb8-142">Depois de comprar uma instância de VM reservada do Azure em nome de um cliente, o desconto para pagar pelo espaço da VM com antecedência é aplicado automaticamente às máquinas virtuais que correspondem aos atributos e à quantidade da reserva do cliente.</span><span class="sxs-lookup"><span data-stu-id="38eb8-142">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span></span>

<span data-ttu-id="38eb8-143">Você pode verificar o uso de reserva do cliente e ver em quais máquinas virtuais os descontos de reserva são aplicados usando um dos seguintes métodos:</span><span class="sxs-lookup"><span data-stu-id="38eb8-143">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>

- <span data-ttu-id="38eb8-144">O portal do Azure</span><span class="sxs-lookup"><span data-stu-id="38eb8-144">The Azure portal</span></span>
- <span data-ttu-id="38eb8-145">API de utilização do Azure</span><span class="sxs-lookup"><span data-stu-id="38eb8-145">Azure utilization API</span></span>

<span data-ttu-id="38eb8-146">As instruções para o uso de cada um desses métodos estão listadas a seguir.</span><span class="sxs-lookup"><span data-stu-id="38eb8-146">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="38eb8-147">Somente a API de utilização do Azure mostra a qual máquina virtual o desconto está sendo aplicado.</span><span class="sxs-lookup"><span data-stu-id="38eb8-147">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="38eb8-148">Verificar o uso de reserva do cliente no portal do Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="38eb8-148">Verify the customer's reservation usage in the Microsoft Azure portal</span></span>

1. <span data-ttu-id="38eb8-149">No Partner Center, vá para a página de seus **clientes** .</span><span class="sxs-lookup"><span data-stu-id="38eb8-149">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="38eb8-150">Localize o cliente cujo desconto e uso de reserva você deseja verificar e, em seguida, selecione a seta para baixo para expandir as informações do cliente.</span><span class="sxs-lookup"><span data-stu-id="38eb8-150">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="38eb8-151">Selecione **portal de gerenciamento do Microsoft Azure** para abrir o registro do cliente no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="38eb8-151">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="38eb8-152">Selecione **Reservas** no menu do portal e então selecione a reserva cujo uso você deseja verificar.</span><span class="sxs-lookup"><span data-stu-id="38eb8-152">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span>
4. <span data-ttu-id="38eb8-153">Na página **visão geral** , verifique o grafo de utilização da reserva, que mostra quanto da reserva foi aplicada às máquinas virtuais.</span><span class="sxs-lookup"><span data-stu-id="38eb8-153">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span>

    >[!NOTE]
    ><span data-ttu-id="38eb8-154">Os dados de utilização podem ser atrasados em até 8 horas.</span><span class="sxs-lookup"><span data-stu-id="38eb8-154">Utilization data may be delayed by up to 8 hours.</span></span>

    <span data-ttu-id="38eb8-155">a.</span><span class="sxs-lookup"><span data-stu-id="38eb8-155">a.</span></span> <span data-ttu-id="38eb8-156">Se a utilização da reserva for 100%, o cliente estará obtendo toda a economia possível que a compra da reserva possa fornecer.</span><span class="sxs-lookup"><span data-stu-id="38eb8-156">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span>
    <span data-ttu-id="38eb8-157">b.</span><span class="sxs-lookup"><span data-stu-id="38eb8-157">b.</span></span> <span data-ttu-id="38eb8-158">Se o uso da reserva for 0%, o desconto não será aplicado a nenhuma máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="38eb8-158">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span></span>
    <span data-ttu-id="38eb8-159">c.</span><span class="sxs-lookup"><span data-stu-id="38eb8-159">c.</span></span> <span data-ttu-id="38eb8-160">Se o uso da reserva estiver entre 1% e 99%, haverá benefícios não utilizados.</span><span class="sxs-lookup"><span data-stu-id="38eb8-160">If the reservation's usage is between 1% and 99%, there are unused benefits.</span></span>

5. <span data-ttu-id="38eb8-161">Para evitar essa situação, determine a VM de tamanho correta para dar suporte às necessidades de computação do cliente antes de fazer a compra.</span><span class="sxs-lookup"><span data-stu-id="38eb8-161">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="38eb8-162">Verificar o uso de reserva do cliente com a API de utilização do Azure</span><span class="sxs-lookup"><span data-stu-id="38eb8-162">Verify the customer's reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="38eb8-163">Somente a API de utilização do Azure mostra a qual máquina virtual o desconto está sendo aplicado.</span><span class="sxs-lookup"><span data-stu-id="38eb8-163">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="38eb8-164">Você pode obter dados de uso da reserva com a API de utilização do Azure para verificar se o cliente está recebendo o desconto da reserva e para ver a quais VMs (máquinas virtuais) o desconto é aplicado.</span><span class="sxs-lookup"><span data-stu-id="38eb8-164">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="38eb8-165">Compare o exemplo a para o exemplo B para ver como verificar o uso de reserva de um cliente.</span><span class="sxs-lookup"><span data-stu-id="38eb8-165">Compare Example A to Example B to see how to verify a customer's reservation usage.</span></span>

:::image type="content" source="images/usage5.png" alt-text="Exemplos de uso de reserva":::

- <span data-ttu-id="38eb8-167">A reservationId identifica a reserva do Azure que foi usada para aplicar o desconto à VM.</span><span class="sxs-lookup"><span data-stu-id="38eb8-167">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
- <span data-ttu-id="38eb8-168">consumptionMeter é a MeterId para a VM que tem o desconto da reserva aplicado a ela.</span><span class="sxs-lookup"><span data-stu-id="38eb8-168">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
- <span data-ttu-id="38eb8-169">O ReservationMeter mostra o custo de US$ 0 desde que o desconto da reserva foi aplicado.</span><span class="sxs-lookup"><span data-stu-id="38eb8-169">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span>

<span data-ttu-id="38eb8-170">Para obter mais informações, consulte [obter os registros de utilização do cliente para o Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) na API do [Partner Center](https://docs.microsoft.com/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="38eb8-170">For more information, see [Get a customer's utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="38eb8-171">Os custos de software, como o Microsoft Windows Server, não estão incluídos no preço de uma reserva de VM e aparecerão como itens de linha separados no registro do pedido e em sua fatura.</span><span class="sxs-lookup"><span data-stu-id="38eb8-171">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="38eb8-172">No entanto, se um cliente tiver o Benefício de Uso Híbrido do Azure, os custos de software não serão aplicados.</span><span class="sxs-lookup"><span data-stu-id="38eb8-172">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="38eb8-173">Para obter mais informações, consulte [Custos de software do Windows não incluídos com Instâncias Reservadas](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span><span class="sxs-lookup"><span data-stu-id="38eb8-173">For more information, see [Windows software costs not included with Reserved Instances](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="azure-reservations-resources"></a><span data-ttu-id="38eb8-174">Recursos de reservas do Azure</span><span class="sxs-lookup"><span data-stu-id="38eb8-174">Azure reservations resources</span></span>

|<span data-ttu-id="38eb8-175">**Para obter informações sobre**</span><span class="sxs-lookup"><span data-stu-id="38eb8-175">**For information about**</span></span>   |<span data-ttu-id="38eb8-176">**Leia isto**</span><span class="sxs-lookup"><span data-stu-id="38eb8-176">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="38eb8-177">Reservas do Azure na visão geral do CSP</span><span class="sxs-lookup"><span data-stu-id="38eb8-177">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="38eb8-178">Vender Instâncias de VM Reservadas do Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="38eb8-178">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="38eb8-179">Comprando reservas do Azure para seus clientes no Partner Center</span><span class="sxs-lookup"><span data-stu-id="38eb8-179">Purchasing Azure reservations for your customers in Partner Center</span></span>   | [<span data-ttu-id="38eb8-180">Comprar reservas do Azure</span><span class="sxs-lookup"><span data-stu-id="38eb8-180">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="38eb8-181">Gerenciando reservas do Azure no Partner Center</span><span class="sxs-lookup"><span data-stu-id="38eb8-181">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="38eb8-182">Gerenciando reservas do Azure no Partner Center</span><span class="sxs-lookup"><span data-stu-id="38eb8-182">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="38eb8-183">Como comprar reservas do Azure no portal do Azure</span><span class="sxs-lookup"><span data-stu-id="38eb8-183">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="38eb8-184">[Pagar antecipadamente por máquinas virtuais com Instâncias de VM Reservadas do Azure](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) na Ajuda do Azure</span><span class="sxs-lookup"><span data-stu-id="38eb8-184">[Prepay for virtual machines with Azure Reserved VM Instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="38eb8-185">Como gerenciar reservas do Azure no portal do Azure</span><span class="sxs-lookup"><span data-stu-id="38eb8-185">Managing Azure reservations in the Azure portal</span></span>   | <span data-ttu-id="38eb8-186">[Gerenciar instâncias de VM reservadas](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) na Ajuda do Azure</span><span class="sxs-lookup"><span data-stu-id="38eb8-186">[Manage reserved VM instances](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="38eb8-187">Como comprar reservas do Azure usando a API do Partner Center</span><span class="sxs-lookup"><span data-stu-id="38eb8-187">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="38eb8-188">[Comprar Instâncias de VM Reservadas do Azure](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) na documentação do desenvolvedor do Partner Center</span><span class="sxs-lookup"><span data-stu-id="38eb8-188">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="38eb8-189">Conceder aos clientes permissão para comprar suas próprias reservas do Azure de uma assinatura que você comprou para eles.</span><span class="sxs-lookup"><span data-stu-id="38eb8-189">Giving customers permission to buy their own Azure reservations from a subscription you purchased for them.</span></span> | [<span data-ttu-id="38eb8-190">Dê permissão aos clientes para comprar suas próprias reservas do Azure</span><span class="sxs-lookup"><span data-stu-id="38eb8-190">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |
