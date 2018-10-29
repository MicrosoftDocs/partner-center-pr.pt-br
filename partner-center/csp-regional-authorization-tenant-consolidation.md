---
title: Consolidação de locatários de autorização regional do CSP | Partner Center
ms.topic: article
ms.date: 10/29/2018
description: Use estas instruções para consolidar locatários para países/regiões diferentes.
ms.assetid: 749B4C6A-26BE-4942-BDA8-F08C40DF048A
author: MaggiePucciEvans
ms.author: evansma
keywords: migrar provedores, provisionamento, conta de locatário, consolidar locatários
ms.localizationpriority: medium
ms.openlocfilehash: 6285b9dfe88052939a50d6675a190f3e5419cdbb
ms.sourcegitcommit: ed22f6825d3af1d19385198b4d511e4b39d5e353
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/29/2018
ms.locfileid: "5797279"
---
# <a name="csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="da9c0-104">Consolidação de locatários de autorização regional do CSP</span><span class="sxs-lookup"><span data-stu-id="da9c0-104">CSP regional authorization tenant consolidation</span></span>

**<span data-ttu-id="da9c0-105">Aplicável a</span><span class="sxs-lookup"><span data-stu-id="da9c0-105">Applies to</span></span>**

-  <span data-ttu-id="da9c0-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="da9c0-106">Partner Center</span></span>
-  <span data-ttu-id="da9c0-107">Partner Center for Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="da9c0-107">Partner Center for Microsoft Cloud for US Government</span></span>
-  <span data-ttu-id="da9c0-108">Partner Center for Microsoft Cloud Germany</span><span class="sxs-lookup"><span data-stu-id="da9c0-108">Partner Center for Microsoft Cloud Germany</span></span>

<span data-ttu-id="da9c0-109">\[Algumas informações dizem respeito a produtos de pré-lançamento que poderão ser substancialmente modificados antes do lançamento comercial.</span><span class="sxs-lookup"><span data-stu-id="da9c0-109">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="da9c0-110">A Microsoft não fornece nenhuma garantia, expressa ou implícita, com relação às informações fornecidas aqui.\]</span><span class="sxs-lookup"><span data-stu-id="da9c0-110">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="da9c0-111">Use estas instruções para consolidar locatários para países/regiões diferentes.</span><span class="sxs-lookup"><span data-stu-id="da9c0-111">Use these instructions to consolidate tenants for different country/regions.</span></span>

<span data-ttu-id="da9c0-112">**Observação**você deve estar ciente de todas as assinaturas e estações para seus clientes provisionados das contas de transição.</span><span class="sxs-lookup"><span data-stu-id="da9c0-112">**Note**You must be aware of all of the subscriptions and seat counts for your customers provisioned from the transition accounts.</span></span> <span data-ttu-id="da9c0-113">Você reprovisionará exatamente as mesmas assinaturas com o mesmo número de estações sob a nova conta de CSP Central como parte do processo de migração.</span><span class="sxs-lookup"><span data-stu-id="da9c0-113">You will be re-provisioning those same exact subscriptions with the same seat counts under the new Central CSP account as part of the migration process.</span></span> <span data-ttu-id="da9c0-114">Use o recurso de lista de exportação para ajudar a criar uma lista de clientes para mover para o locatário centralizado.</span><span class="sxs-lookup"><span data-stu-id="da9c0-114">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span> <span data-ttu-id="da9c0-115">Os parceiros optam por consolidar seus locatários.</span><span class="sxs-lookup"><span data-stu-id="da9c0-115">Partners choose to consolidate their tenants.</span></span> <span data-ttu-id="da9c0-116">Quando consolidação for concluída, os parceiros não poderão reverter para seu estado anterior.</span><span class="sxs-lookup"><span data-stu-id="da9c0-116">Once consolidation is complete, Partners cannot revert to their previous state.</span></span> <span data-ttu-id="da9c0-117">Observe que a ação do cliente talvez seja necessária.</span><span class="sxs-lookup"><span data-stu-id="da9c0-117">Note that customer action may also be required.</span></span>

 

## <a name="prepare-for-migration"></a><span data-ttu-id="da9c0-118">Preparar para a migração</span><span class="sxs-lookup"><span data-stu-id="da9c0-118">Prepare for migration</span></span>


-   <span data-ttu-id="da9c0-119">Entre no seu **Partner Center** com a conta de **transição** (existente) (da qual será feita a transição) e anote todos os clientes e todos os serviços provisionados para esses clientes.</span><span class="sxs-lookup"><span data-stu-id="da9c0-119">Sign in to your **Partner Center**  with the **Transitioning** (existing) account (the one you will transition)  and take note of all customers and all of the services provisioned for those customers.</span></span>

![lista de clientes regionais](images/regionalcustomer1.png)

## <a name="migrate-customer-accounts"></a><span data-ttu-id="da9c0-121">Migrar contas de clientes</span><span class="sxs-lookup"><span data-stu-id="da9c0-121">Migrate customer accounts</span></span>


1.  <span data-ttu-id="da9c0-122">Entre no seu **Partner Center** com a **transição** (nova) conta (aquela estão fazendo a transição em) e navegue até a lista de clientes de **clientes**.</span><span class="sxs-lookup"><span data-stu-id="da9c0-122">Sign in to your **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning into) and navigate to the Customers list from **Customers**.</span></span>

2.  <span data-ttu-id="da9c0-123">Selecione Clientes.</span><span class="sxs-lookup"><span data-stu-id="da9c0-123">Select Customers.</span></span>

3.  <span data-ttu-id="da9c0-124">Clique em **Solicitar uma relação de revendedor**.</span><span class="sxs-lookup"><span data-stu-id="da9c0-124">Click **Request a reseller relationship**.</span></span> <span data-ttu-id="da9c0-125">Será exibida uma mensagem de email padrão para apresentar aos seus clientes.</span><span class="sxs-lookup"><span data-stu-id="da9c0-125">You are presented with a default email message to present to your customers.</span></span> <span data-ttu-id="da9c0-126">Essa mensagem contém uma URL com a ID da organização exclusiva para sua nova conta do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="da9c0-126">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4.  <span data-ttu-id="da9c0-127">**Ação do cliente:** Certifique-se de que cada um dos clientes ativos que você deseja migrar visite essa URL.</span><span class="sxs-lookup"><span data-stu-id="da9c0-127">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="da9c0-128">Ao abrir a URL, o cliente será solicitado a entrar no portal do Office 365.</span><span class="sxs-lookup"><span data-stu-id="da9c0-128">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="da9c0-129">O cliente entra usando a mesma ID da organização que ele usa para acessar os portais de administrador do Azure e do Office 365.</span><span class="sxs-lookup"><span data-stu-id="da9c0-129">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5.  <span data-ttu-id="da9c0-130">Ao entrar, o Administrador Global da conta do cliente será solicitado a enviar um contrato para conceder privilégios de administrador delegado à nova conta CSP.</span><span class="sxs-lookup"><span data-stu-id="da9c0-130">After signing in, the Global Admin for the customer account is prompted to submit an agreement to give delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="da9c0-131">Se concordar, o cliente marca a caixa de seleção e concorda em autorizar o relacionamento.</span><span class="sxs-lookup"><span data-stu-id="da9c0-131">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="da9c0-132">Os clientes aparecerão na lista de clientes do parceiro após o envio do contrato, um por um.</span><span class="sxs-lookup"><span data-stu-id="da9c0-132">The customers will appear in the partner’s customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="da9c0-133">Migrando assinaturas baseadas em uso do Office 365 e não Azure</span><span class="sxs-lookup"><span data-stu-id="da9c0-133">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>


1.  <span data-ttu-id="da9c0-134">Depois que o cliente assinar o contrato, você poderá recriar as assinaturas dele em seu locatário parceiro centralizado.</span><span class="sxs-lookup"><span data-stu-id="da9c0-134">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2.  <span data-ttu-id="da9c0-135">No **Partner Center** , selecione **os clientes**.</span><span class="sxs-lookup"><span data-stu-id="da9c0-135">From the **Partner Center** select **Customers**.</span></span>

3.  <span data-ttu-id="da9c0-136">Abra o nome da empresa do cliente que você deseja migrar.</span><span class="sxs-lookup"><span data-stu-id="da9c0-136">Open the company name for the customer you want to migrate.</span></span>

4.  <span data-ttu-id="da9c0-137">Clique em **Adicionar assinatura**.</span><span class="sxs-lookup"><span data-stu-id="da9c0-137">Click **Add subscription**.</span></span>

5.  <span data-ttu-id="da9c0-138">Adicione as assinaturas corretas e os números de estações do catálogo.</span><span class="sxs-lookup"><span data-stu-id="da9c0-138">Add the correct subscriptions and seat counts from the catalog.</span></span> <span data-ttu-id="da9c0-139">Verificar com as informações fornecidas nas contas de parceiro de **origem da transição**.</span><span class="sxs-lookup"><span data-stu-id="da9c0-139">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

    ![captura de tela da lista de clientes](images/regionalcustomer2.png)

6.  <span data-ttu-id="da9c0-141">Clique em **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="da9c0-141">Click **Submit.**</span></span>

<span data-ttu-id="da9c0-142">Agora os serviços serão fornecidos para o cliente da conta de parceiro de **destino da transição**.</span><span class="sxs-lookup"><span data-stu-id="da9c0-142">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

<span data-ttu-id="da9c0-143">Repita essas etapas para migrar assinaturas para todos os outros clientes.</span><span class="sxs-lookup"><span data-stu-id="da9c0-143">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="da9c0-144">Antes de prosseguir para a próxima seção, certifique-se de que todas as assinaturas de cliente existentes nas contas de parceiros de **origem da transição** sejam reprovisionadas sob a conta de parceiro de **destino da transição**.</span><span class="sxs-lookup"><span data-stu-id="da9c0-144">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

<span data-ttu-id="da9c0-145">**Observação**os parceiros devem suspender as assinaturas na **Origem da transição** locatário parceiro conta no Partner Center no mesmo dia que essas assinaturas são transmitidas e configuradas na conta de locatário parceiro **Destino da transição** no o Partner Center para garantir que a cobrança dupla não ocorre.</span><span class="sxs-lookup"><span data-stu-id="da9c0-145">**Note**Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="da9c0-146">As solicitações de suporte serão negadas para créditos decorrentes de alguma sobreposição de cobranças que ocorra devido à não configuração das assinaturas de **origem da transição** como desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="da9c0-146">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to disabled.</span></span>

 

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="da9c0-147">Desabilitando as assinaturas do Office 365 na conta de parceiro de origem da transição</span><span class="sxs-lookup"><span data-stu-id="da9c0-147">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>


<span data-ttu-id="da9c0-148">Desabilitar a assinatura de CSP sob as contas de parceiros de **destino da transição** impede qualquer cobrança futura.</span><span class="sxs-lookup"><span data-stu-id="da9c0-148">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="da9c0-149">Você não precisa desabilitar manualmente as assinaturas do Azure, elas são desativadas automaticamente durante o processo de migração.</span><span class="sxs-lookup"><span data-stu-id="da9c0-149">You do not have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1.  <span data-ttu-id="da9c0-150">Entrar no **Partner Center** com a conta CSP **Origem da transição** e navegue até a lista de clientes.</span><span class="sxs-lookup"><span data-stu-id="da9c0-150">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2.  <span data-ttu-id="da9c0-151">Abra o cliente com assinaturas para desabilitar e, em seguida, selecione a primeira oferta a ser desabilitada.</span><span class="sxs-lookup"><span data-stu-id="da9c0-151">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>
3.  <span data-ttu-id="da9c0-152">Defina a assinatura como **suspensa** e clique em **enviar**.</span><span class="sxs-lookup"><span data-stu-id="da9c0-152">Set the subscription to **suspended**, and then click **submit**.</span></span>

    <span data-ttu-id="da9c0-153">**Observação**suspender a assinatura garante que não haja cobrança dupla.</span><span class="sxs-lookup"><span data-stu-id="da9c0-153">**Note**Suspending the subscription ensures double billing does not occur.</span></span>

     

    <span data-ttu-id="da9c0-154">A assinatura é exibida como **suspensa** na lista de assinaturas.</span><span class="sxs-lookup"><span data-stu-id="da9c0-154">The Subscription shows **suspended** on the subscriptions list.</span></span>

4.  <span data-ttu-id="da9c0-155">Repita essas etapas para todas as assinaturas sob o cliente.</span><span class="sxs-lookup"><span data-stu-id="da9c0-155">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="da9c0-156">Verifique se todas são exibidas como **suspensas**.</span><span class="sxs-lookup"><span data-stu-id="da9c0-156">Verify all show **suspended.**</span></span>

5.  <span data-ttu-id="da9c0-157">Selecione o próximo cliente na lista e repita o processo para desabilitar todas as assinaturas.</span><span class="sxs-lookup"><span data-stu-id="da9c0-157">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="da9c0-158">Migrando assinaturas baseadas em uso do Azure</span><span class="sxs-lookup"><span data-stu-id="da9c0-158">Migrating Azure usage-based subscriptions</span></span>


<span data-ttu-id="da9c0-159">Observe que assinaturas de CSP baseadas em uso do Azure não precisam ser migradas manualmente como no caso das assinaturas de CSP do Office 365.</span><span class="sxs-lookup"><span data-stu-id="da9c0-159">Note that Azure usage-based CSP subscriptions do not need to be migrated manually as in the case with Office 365 CSP subscriptions.</span></span> <span data-ttu-id="da9c0-160">O suporte do Microsoft Azure pode migrar as assinaturas do Azure, bem como todos os serviços ou recursos implantados, das contas de revendedor CSP de **origem da transição** para a conta de revendedor CSP de **destino da transição**.</span><span class="sxs-lookup"><span data-stu-id="da9c0-160">Microsoft Azure Support can migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="da9c0-161">Não haverá qualquer interrupção do serviço para o cliente durante a transição.</span><span class="sxs-lookup"><span data-stu-id="da9c0-161">There will be no disruption of service to the customer during this transition.</span></span>

1.  <span data-ttu-id="da9c0-162">Certifique-se de que as contas de clientes que precisam de assinaturas do Azure migradas aceitem o contrato para serem associadas à nova conta CSP de **destino da transição**.</span><span class="sxs-lookup"><span data-stu-id="da9c0-162">Ensure that the customer accounts that need Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>
2.  <span data-ttu-id="da9c0-163">Os parceiros notificam a Microsoft quais contas de clientes que têm assinaturas do Azure estão prontas para migrar, fornecendo também os nomes de empresa do cliente.</span><span class="sxs-lookup"><span data-stu-id="da9c0-163">Partners notify Microsoft which customer accounts that have Azure subscriptions are ready to migrate, and provides those customer’s company names.</span></span>
3.  <span data-ttu-id="da9c0-164">A Microsoft migra as assinaturas baseadas em uso do Azure e notifica o parceiro quando a migração é concluída.</span><span class="sxs-lookup"><span data-stu-id="da9c0-164">Microsoft migrates the Azure usage-based subscriptions and notifies the partner when the migration is complete.</span></span>
4.  <span data-ttu-id="da9c0-165">O parceiro confirma se agora a assinatura do Azure sob a conta de revendedor CSP de **origem da transição** é exibida como suspensa no Partner Center, na seção de assinaturas de cliente.</span><span class="sxs-lookup"><span data-stu-id="da9c0-165">The partner confirms that the Azure subscription under the **Transitioning From** CSP reseller accounts now shows suspended in the Partner Center under the customer subscriptions section.</span></span>
5.  <span data-ttu-id="da9c0-166">O parceiro confirma se agora a assinatura do Azure sob a conta de revendedor CSP de **destino da transição** mostra o status de **ativa** no Partner Center, na seção de assinaturas de cliente.</span><span class="sxs-lookup"><span data-stu-id="da9c0-166">The partner confirms that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in the Partner Center under the customer subscriptions section.</span></span>

    <span data-ttu-id="da9c0-167">**Observação**desabilitar as assinaturas sob o cliente não altera a aparência do cliente na lista de clientes.</span><span class="sxs-lookup"><span data-stu-id="da9c0-167">**Note**Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="da9c0-168">Atualmente, não há uma opção para remover clientes da lista.</span><span class="sxs-lookup"><span data-stu-id="da9c0-168">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="da9c0-169">Os parceiros devem evitar readicionar assinaturas para esses clientes a partir da conta de **destino da transição** no futuro.</span><span class="sxs-lookup"><span data-stu-id="da9c0-169">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

     

6.  <span data-ttu-id="da9c0-170">Repita essas etapas para todas as assinaturas em todos os seus clientes para impedir encargos futuros nas contas de **origem da transição**.</span><span class="sxs-lookup"><span data-stu-id="da9c0-170">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="da9c0-171">O parceiro receberá uma fatura final com um crédito pelo número de dias não utilizados entre o dia de cancelamento e o último dia do período de cobrança.</span><span class="sxs-lookup"><span data-stu-id="da9c0-171">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="da9c0-172">Nenhuma fatura futura será gerada após esse período de cobrança final.</span><span class="sxs-lookup"><span data-stu-id="da9c0-172">No future invoices will generate after that final billing period.</span></span>

### <a name="notes"></a><span data-ttu-id="da9c0-173">Observações</span><span class="sxs-lookup"><span data-stu-id="da9c0-173">Notes</span></span>

-   <span data-ttu-id="da9c0-174">Desabilitar a assinatura da conta CSP de **origem da transição** não afeta o serviço do cliente final contanto que o serviço tenha sido provisionado pela conta CSP de **destino da transição** antes de desabilitar.</span><span class="sxs-lookup"><span data-stu-id="da9c0-174">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer’s service provided the service was provisioned from the **Transitioning To** CSP account prior to the disable.</span></span>

-   <span data-ttu-id="da9c0-175">A assinaturas não podem ser usadas pelo cliente e não geram encargos quando são suspensas ou canceladas.</span><span class="sxs-lookup"><span data-stu-id="da9c0-175">Subscriptions cannot be used by the customer and do not generate charges when suspended or cancelled.</span></span>

-   <span data-ttu-id="da9c0-176">Atualmente, não há uma maneira de remover completamente um cliente da Lista de clientes.</span><span class="sxs-lookup"><span data-stu-id="da9c0-176">There is currently no way to remove a customer from the Customers list completely.</span></span>

-   <span data-ttu-id="da9c0-177">**Observação**os parceiros devem suspender as assinaturas na **Origem da transição** locatário parceiro conta no Partner Center no mesmo dia que essas assinaturas são transmitidas e configuradas na conta **Destino da transição** locatário parceiro no Partner Center para garantir que não haja cobrança dupla.</span><span class="sxs-lookup"><span data-stu-id="da9c0-177">**Note**Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned to and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="da9c0-178">A Microsoft não dará suporte para solicitações de créditos decorrentes de alguma sobreposição de cobranças que ocorra devido à não configuração das assinaturas de **origem da transição** como suspensas.</span><span class="sxs-lookup"><span data-stu-id="da9c0-178">Microsoft will not support requests for credits due to any overlap in billing which occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

     

### <a name="simplify-migration-using-export"></a><span data-ttu-id="da9c0-179">Simplificar a migração usando Exportar</span><span class="sxs-lookup"><span data-stu-id="da9c0-179">Simplify migration using Export</span></span>

<span data-ttu-id="da9c0-180">Usando a **função Exportar**, você pode capturar as assinaturas que serão usadas em sua nova estrutura consolidada:</span><span class="sxs-lookup"><span data-stu-id="da9c0-180">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1.  <span data-ttu-id="da9c0-181">Clique em **clientes** no Partner Center para ver a lista de clientes em sua estrutura existente.</span><span class="sxs-lookup"><span data-stu-id="da9c0-181">Click **Customers** on Partner Center to see the list of customers in your existing structure.</span></span>

2.  <span data-ttu-id="da9c0-182">Abra o nome do cliente desejado.</span><span class="sxs-lookup"><span data-stu-id="da9c0-182">Open the desired customer name.</span></span>

3.  <span data-ttu-id="da9c0-183">Na página **Assinaturas**, clique em **Exportar Assinaturas** para exportar os detalhes das assinaturas para um arquivo do Excel.</span><span class="sxs-lookup"><span data-stu-id="da9c0-183">On the **Subscriptions** page, click **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4.  <span data-ttu-id="da9c0-184">Use essa lista para recriar as assinaturas em seu novo locatário consolidado.</span><span class="sxs-lookup"><span data-stu-id="da9c0-184">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="da9c0-185">Registro de API</span><span class="sxs-lookup"><span data-stu-id="da9c0-185">API registration</span></span>

<span data-ttu-id="da9c0-186">Para obter mais informações sobre o registro de API [consulte esta página](https://go.microsoft.com/fwlink/?linkid=847990).</span><span class="sxs-lookup"><span data-stu-id="da9c0-186">For more information about API registration, [see this page](https://go.microsoft.com/fwlink/?linkid=847990).</span></span>


 

 



