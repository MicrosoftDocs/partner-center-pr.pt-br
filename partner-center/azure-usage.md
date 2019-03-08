---
title: Dimensionamento de VM do Microsoft Azure para uso de reserva máximo | Partner Center
ms.topic: article
ms.date: 10/29/2018
Description: Ao comprar reservas do Microsoft Azure em nome dos seus clientes, você precisará escolher uma máquina virtual (VM) dimensionada para atender às necessidades de computação do cliente.
author: LauraBrenner
ms.author: v-petand
keywords: azure, reservas, vm, gerenciar, uso, dimensionamento
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: cbe24b3da0b9cadf1ed9e8d9f06b5b575bf16d22
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2019
ms.locfileid: "57586959"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="5fe1c-104">Dimensionamento de VM do Microsoft Azure para uso máximo de reserva do Azure</span><span class="sxs-lookup"><span data-stu-id="5fe1c-104">Microsoft Azure VM sizing for maximum reservation usage</span></span> 

<span data-ttu-id="5fe1c-105">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="5fe1c-105">**Applies to**</span></span>

-  <span data-ttu-id="5fe1c-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="5fe1c-106">Partner Center</span></span>
-  <span data-ttu-id="5fe1c-107">Portal do Azure</span><span class="sxs-lookup"><span data-stu-id="5fe1c-107">Azure portal</span></span>
-  <span data-ttu-id="5fe1c-108">Parceiros no CSP</span><span class="sxs-lookup"><span data-stu-id="5fe1c-108">Partners in CSP</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="5fe1c-109">Determinar o tamanho da VM para reserva do Azure do cliente</span><span class="sxs-lookup"><span data-stu-id="5fe1c-109">Determine the VM size for a customer’s Azure reservation</span></span> 

<span data-ttu-id="5fe1c-110">Ao comprar reservas do Microsoft Azure em nome dos seus clientes, você precisará escolher uma máquina virtual (VM) dimensionada para atender às necessidades de computação do cliente.</span><span class="sxs-lookup"><span data-stu-id="5fe1c-110">When buying Microsoft Azure reservations on behalf of your customers, you’ll need to choose a virtual machine (VM) sized to meet the customer’s computing needs.</span></span> <span data-ttu-id="5fe1c-111">Você pode encontrar essas informações usando um destes métodos:</span><span class="sxs-lookup"><span data-stu-id="5fe1c-111">You can find this information using one of these methods:</span></span>

-   <span data-ttu-id="5fe1c-112">API de utilização do Azure</span><span class="sxs-lookup"><span data-stu-id="5fe1c-112">Azure utilization API</span></span>
-   <span data-ttu-id="5fe1c-113">O portal do Azure</span><span class="sxs-lookup"><span data-stu-id="5fe1c-113">The Azure portal</span></span>
-   <span data-ttu-id="5fe1c-114">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="5fe1c-114">Azure PowerShell</span></span>
-   <span data-ttu-id="5fe1c-115">A API do Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="5fe1c-115">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="5fe1c-116">As instruções para o uso de cada um desses métodos estão listadas a seguir.</span><span class="sxs-lookup"><span data-stu-id="5fe1c-116">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="5fe1c-117">Depois que você comprar uma reserva, o desconto da reserva será aplicado automaticamente em máquinas virtuais que correspondam aos atributos e à quantidade da reserva.</span><span class="sxs-lookup"><span data-stu-id="5fe1c-117">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="5fe1c-118">Você não precisa atribuir a reserva a uma VM.</span><span class="sxs-lookup"><span data-stu-id="5fe1c-118">You don’t need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="5fe1c-119">Os descontos da reserva não se aplicam a VMs clássicas ou promocionais.</span><span class="sxs-lookup"><span data-stu-id="5fe1c-119">Reservation discounts don’t apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="5fe1c-120">Para identificar o tipo e o tamanho da VM a ser comprada em nome de seu cliente, você deverá usar um dos métodos descritos abaixo já que o tipo de série de VM não é exibido corretamente nos arquivos de reconciliação do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="5fe1c-120">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>


<span data-ttu-id="5fe1c-121">**Obtenha informações usando a API do Azure de utilização de dimensionamento de VM**</span><span class="sxs-lookup"><span data-stu-id="5fe1c-121">**Get VM sizing information using the Azure utilization API**</span></span>

1.  <span data-ttu-id="5fe1c-122">Use o valor do atributo ServiceType desde additionalInfo na resposta da API para identificar o tamanho da VM a ser comprada.</span><span class="sxs-lookup"><span data-stu-id="5fe1c-122">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span> 

2.  <span data-ttu-id="5fe1c-123">Para obter mais informações, consulte [Obter registros de utilização de um cliente do Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) na [API do Partner Center](https://docs.microsoft.com/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="5fe1c-123">For more information, see [Get a customer’s utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span> 

<span data-ttu-id="5fe1c-124">**Obtenha informações usando o portal do Microsoft Azure de dimensionamento de VM**</span><span class="sxs-lookup"><span data-stu-id="5fe1c-124">**Get VM sizing information using the Microsoft Azure portal**</span></span>

1.  <span data-ttu-id="5fe1c-125">No Partner Center, vá para seu **clientes** página.</span><span class="sxs-lookup"><span data-stu-id="5fe1c-125">In Partner Center, go to your **Customers** page.</span></span>

2.  <span data-ttu-id="5fe1c-126">Encontre o cliente que deseja comprar reservas de VM do Azure e então selecione a seta para baixo para expandir as informações do cliente.</span><span class="sxs-lookup"><span data-stu-id="5fe1c-126">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer’s information.</span></span> <span data-ttu-id="5fe1c-127">Selecione **Portal de Gerenciamento do Microsoft Azure** para abrir o registro do cliente no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="5fe1c-127">Select **Microsoft Azure Management Portal** to open the customer’s record in the Azure portal.</span></span> 

3.  <span data-ttu-id="5fe1c-128">Selecione **Máquinas virtuais** no menu do portal e então selecione a VM para a qual você deseja comprar uma reserva.</span><span class="sxs-lookup"><span data-stu-id="5fe1c-128">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span> 

4.  <span data-ttu-id="5fe1c-129">Na página de detalhes da VM, encontre as informações de tamanho e região, como ilustrado abaixo, e use essas informações para comprar a reserva no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="5fe1c-129">On the VM’s detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

    ![Informações de tamanho e a região na página de detalhes](images/usage1.png)

<span data-ttu-id="5fe1c-131">**Obtenha informações usando o Microsoft Azure PowerShell de dimensionamento de VM**</span><span class="sxs-lookup"><span data-stu-id="5fe1c-131">**Get VM sizing information using Microsoft Azure PowerShell**</span></span>

<span data-ttu-id="5fe1c-132">Use as informações na imagem abaixo para obter a localização e o tamanho da VM para a qual você deseja comprar uma reserva.</span><span class="sxs-lookup"><span data-stu-id="5fe1c-132">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

![Tamanho e local da VM](images/usage2.png)

<span data-ttu-id="5fe1c-134">**Obtenha informações usando a API do Azure Resource Manager (ARM) de dimensionamento de VM**</span><span class="sxs-lookup"><span data-stu-id="5fe1c-134">**Get VM sizing information using the Azure Resource Manager (ARM) API**</span></span>

1.  <span data-ttu-id="5fe1c-135">Usando o ARMClient ou as APIs ARM, chame o cliente ARM para a VM para a qual você deseja comprar uma reserva.</span><span class="sxs-lookup"><span data-stu-id="5fe1c-135">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2.  <span data-ttu-id="5fe1c-136">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span><span class="sxs-lookup"><span data-stu-id="5fe1c-136">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3.  <span data-ttu-id="5fe1c-137">A chamada retorna os valores de **vmSize** e **location**, como ilustrado abaixo.</span><span class="sxs-lookup"><span data-stu-id="5fe1c-137">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    <span data-ttu-id="5fe1c-138">![o valor de vmSize](images/usage3.png)
    ![valor local](images/usage4.png)</span><span class="sxs-lookup"><span data-stu-id="5fe1c-138">![vmSize value](images/usage3.png)
![location value](images/usage4.png)</span></span>
 

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="5fe1c-139">Verificar o desconto de uso e de reserva de VM do Azure</span><span class="sxs-lookup"><span data-stu-id="5fe1c-139">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="5fe1c-140">Depois de você comprar uma Instância de VM Reservada do Azure em nome de um cliente, o desconto para pagamento antecipado pelo espaço de VM será automaticamente aplicado às máquinas virtuais que correspondem aos atributos e à quantidade de reservas do cliente.</span><span class="sxs-lookup"><span data-stu-id="5fe1c-140">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer’s reservation.</span></span> 

<span data-ttu-id="5fe1c-141">Você pode verificar o uso de reservas do cliente e ver para quais máquinas virtuais os descontos de reserva são aplicados usando um dos seguintes métodos:</span><span class="sxs-lookup"><span data-stu-id="5fe1c-141">You can verify the customer’s reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>   

-   <span data-ttu-id="5fe1c-142">O portal do Azure</span><span class="sxs-lookup"><span data-stu-id="5fe1c-142">The Azure portal</span></span>
-   <span data-ttu-id="5fe1c-143">API de utilização do Azure</span><span class="sxs-lookup"><span data-stu-id="5fe1c-143">Azure utilization API</span></span>

<span data-ttu-id="5fe1c-144">As instruções para o uso de cada um desses métodos estão listadas a seguir.</span><span class="sxs-lookup"><span data-stu-id="5fe1c-144">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="5fe1c-145">Somente a API de utilização do Azure mostra a qual máquina virtual o desconto está sendo aplicado.</span><span class="sxs-lookup"><span data-stu-id="5fe1c-145">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="5fe1c-146">Verificar o uso de reserva do cliente no portal do Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="5fe1c-146">Verify the customer’s reservation usage in the Microsoft Azure portal</span></span>

1.  <span data-ttu-id="5fe1c-147">No Partner Center, vá para seu **clientes** página.</span><span class="sxs-lookup"><span data-stu-id="5fe1c-147">In Partner Center, go to your **Customers** page.</span></span>

2.  <span data-ttu-id="5fe1c-148">Encontre o cliente cujo desconto e uso de reserva você deseja verificar e então selecione a seta para baixo para expandir as informações do cliente.</span><span class="sxs-lookup"><span data-stu-id="5fe1c-148">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer’s information.</span></span> <span data-ttu-id="5fe1c-149">Selecione **Portal de Gerenciamento do Microsoft Azure** para abrir o registro do cliente no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="5fe1c-149">Select **Microsoft Azure Management Portal** to open the customer’s record in the Azure portal.</span></span> 

3.  <span data-ttu-id="5fe1c-150">Selecione **Reservas** no menu do portal e então selecione a reserva cujo uso você deseja verificar.</span><span class="sxs-lookup"><span data-stu-id="5fe1c-150">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span> 

4.  <span data-ttu-id="5fe1c-151">Na página **Visão geral**, verifique o gráfico de utilização da reserva, que mostra o quanto da reserva foi aplicado às máquinas virtuais.</span><span class="sxs-lookup"><span data-stu-id="5fe1c-151">On the **Overview** page check the reservation’s utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span> 

    >[!NOTE]
    ><span data-ttu-id="5fe1c-152">Os dados de utilização podem ser atrasados em até 8 horas.</span><span class="sxs-lookup"><span data-stu-id="5fe1c-152">Utilization data may be delayed by up to 8 hours.</span></span>
    
    <span data-ttu-id="5fe1c-153">a.</span><span class="sxs-lookup"><span data-stu-id="5fe1c-153">a.</span></span>  <span data-ttu-id="5fe1c-154">Se a utilização da reserva for de 100%, o cliente estará recebendo toda a economia possível que a compra de reserva pode fornecer.</span><span class="sxs-lookup"><span data-stu-id="5fe1c-154">If the reservation’s utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span> 
    
    <span data-ttu-id="5fe1c-155">b.</span><span class="sxs-lookup"><span data-stu-id="5fe1c-155">b.</span></span>  <span data-ttu-id="5fe1c-156">Se o uso da reserva for 0%, o desconto não estará sendo aplicado a nenhuma máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="5fe1c-156">If the reservation’s usage is 0%, the discount is not being applied to any virtual machine.</span></span> 
    
    <span data-ttu-id="5fe1c-157">c.</span><span class="sxs-lookup"><span data-stu-id="5fe1c-157">c.</span></span>  <span data-ttu-id="5fe1c-158">Se o uso da reserva estiver entre 1% e 99%, há benefícios não utilizados.</span><span class="sxs-lookup"><span data-stu-id="5fe1c-158">If the reservation’s usage is between 1% and 99%, there are unused benefits.</span></span> 

5.  <span data-ttu-id="5fe1c-159">Para evitar essa situação, determine a VM de tamanho correto para dar suporte às necessidades de computação do cliente antes de fazer a compra.</span><span class="sxs-lookup"><span data-stu-id="5fe1c-159">To avoid this situation, determine the correct size VM to support the customer’s computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="5fe1c-160">Verificar o uso de reserva do cliente com a API de utilização do Azure</span><span class="sxs-lookup"><span data-stu-id="5fe1c-160">Verify the customer’s reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="5fe1c-161">Somente a API de utilização do Azure mostra a qual máquina virtual o desconto está sendo aplicado.</span><span class="sxs-lookup"><span data-stu-id="5fe1c-161">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="5fe1c-162">Você pode obter dados de uso da reserva com a API de utilização do Azure para verificar se o cliente está recebendo o desconto da reserva e para ver a quais VMs (máquinas virtuais) o desconto é aplicado.</span><span class="sxs-lookup"><span data-stu-id="5fe1c-162">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="5fe1c-163">Compare o Exemplo A ao Exemplo B para saber como verificar o uso da reserva de um cliente.</span><span class="sxs-lookup"><span data-stu-id="5fe1c-163">Compare Example A to Example B to see how to verify a customer’s reservation usage.</span></span> 

![Exemplos de uso de reserva](images/usage5.png)

-   <span data-ttu-id="5fe1c-165">A reservationId identifica a reserva do Azure que foi usada para aplicar o desconto à VM.</span><span class="sxs-lookup"><span data-stu-id="5fe1c-165">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
-   <span data-ttu-id="5fe1c-166">consumptionMeter é a MeterId para a VM que tem o desconto da reserva aplicado a ela.</span><span class="sxs-lookup"><span data-stu-id="5fe1c-166">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
-   <span data-ttu-id="5fe1c-167">O ReservationMeter mostra o custo de US$ 0 desde que o desconto da reserva foi aplicado.</span><span class="sxs-lookup"><span data-stu-id="5fe1c-167">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span> 

<span data-ttu-id="5fe1c-168">Para obter mais informações, consulte [Obter registros de utilização de um cliente do Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) na [API do Partner Center](https://docs.microsoft.com/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="5fe1c-168">For more information, see [Get a customer’s utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="5fe1c-169">Os custos de software, como o Microsoft Windows Server, não estão incluídos no preço de uma reserva de VM e aparecerão como itens de linha separados no registro do pedido e em sua fatura.</span><span class="sxs-lookup"><span data-stu-id="5fe1c-169">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="5fe1c-170">No entanto, se um cliente tiver o Benefício de Uso Híbrido do Azure, os custos de software não serão aplicados.</span><span class="sxs-lookup"><span data-stu-id="5fe1c-170">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="5fe1c-171">Para obter mais informações, consulte [Custos de software do Windows não incluídos com Instâncias Reservadas](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span><span class="sxs-lookup"><span data-stu-id="5fe1c-171">For more information, see [Windows software costs not included with Reserved Instances](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="azure-reservations-resources"></a><span data-ttu-id="5fe1c-172">Recursos de reservas do Azure</span><span class="sxs-lookup"><span data-stu-id="5fe1c-172">Azure reservations resources</span></span>
|<span data-ttu-id="5fe1c-173">**Para obter informações sobre**</span><span class="sxs-lookup"><span data-stu-id="5fe1c-173">**For information about**</span></span>   |<span data-ttu-id="5fe1c-174">**Leia isto**</span><span class="sxs-lookup"><span data-stu-id="5fe1c-174">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="5fe1c-175">Reservas do Azure na visão geral do CSP</span><span class="sxs-lookup"><span data-stu-id="5fe1c-175">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="5fe1c-176">Vende instâncias VM reservadas do Azure da Microsoft</span><span class="sxs-lookup"><span data-stu-id="5fe1c-176">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="5fe1c-177">Comprar reservas do Azure para seus clientes no Partner Center</span><span class="sxs-lookup"><span data-stu-id="5fe1c-177">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="5fe1c-178">Comprar reservas do Azure</span><span class="sxs-lookup"><span data-stu-id="5fe1c-178">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="5fe1c-179">Gerenciando reservas do Azure no Partner Center</span><span class="sxs-lookup"><span data-stu-id="5fe1c-179">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="5fe1c-180">Gerenciando reservas do Azure no Partner Center</span><span class="sxs-lookup"><span data-stu-id="5fe1c-180">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="5fe1c-181">Como comprar reservas do Azure no portal do Azure</span><span class="sxs-lookup"><span data-stu-id="5fe1c-181">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="5fe1c-182">[Pagar antecipadamente por máquinas virtuais com Instâncias de VM Reservadas do Azure](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) na Ajuda do Azure</span><span class="sxs-lookup"><span data-stu-id="5fe1c-182">[Prepay for virtual machines with Azure Reserved VM Instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="5fe1c-183">Como gerenciar reservas do Azure no portal do Azure</span><span class="sxs-lookup"><span data-stu-id="5fe1c-183">Managing Azure reservations in the Azure portal</span></span>   |<span data-ttu-id="5fe1c-184">[Gerenciar instâncias de VM reservadas](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) na Ajuda do Azure</span><span class="sxs-lookup"><span data-stu-id="5fe1c-184">[Manage reserved VM instances](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="5fe1c-185">Como comprar reservas do Azure usando a API do Partner Center</span><span class="sxs-lookup"><span data-stu-id="5fe1c-185">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="5fe1c-186">[Comprar Instâncias de VM Reservadas do Azure](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) na documentação do desenvolvedor do Partner Center</span><span class="sxs-lookup"><span data-stu-id="5fe1c-186">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>



