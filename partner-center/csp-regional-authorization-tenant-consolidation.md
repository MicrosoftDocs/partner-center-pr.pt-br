---
title: Consolidação de locatários de autorização regional do CSP
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Use estas instruções para consolidar locatários para países/regiões diferentes. Isso inclui etapas para migrar contas de cliente e assinaturas de cliente.
author: LauraBrenner
ms.author: labrenne
keywords: migrar provedores, provisionamento, conta de locatário, consolidar locatários
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: 2e3c0bd9b50e91e02952a690cc7cbfe1601ad550
ms.sourcegitcommit: e0a1b4506840486f4bb82620051e0f6a5e81662a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "84991466"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="93180-105">Instruções para a consolidação de locatários de autorização regional do CSP</span><span class="sxs-lookup"><span data-stu-id="93180-105">Instructions for CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="93180-106">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="93180-106">**Applies to**</span></span>

-  <span data-ttu-id="93180-107">Partner Center</span><span class="sxs-lookup"><span data-stu-id="93180-107">Partner Center</span></span>
-  <span data-ttu-id="93180-108">Partner Center do Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="93180-108">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="93180-109">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="93180-109">**Appropriate roles**</span></span>

- <span data-ttu-id="93180-110">Administrador global</span><span class="sxs-lookup"><span data-stu-id="93180-110">Global admin</span></span>
- <span data-ttu-id="93180-111">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="93180-111">Admin agent</span></span>

<span data-ttu-id="93180-112">\[Algumas informações estão relacionadas ao produto de pré-lançamento que pode ser substancialmente modificado antes de ser lançado comercialmente.</span><span class="sxs-lookup"><span data-stu-id="93180-112">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="93180-113">A Microsoft não oferece garantias, expressas ou implícitas, quanto às informações fornecidas aqui.\]</span><span class="sxs-lookup"><span data-stu-id="93180-113">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="93180-114">Use estas instruções para consolidar locatários para países/regiões diferentes.</span><span class="sxs-lookup"><span data-stu-id="93180-114">Use these instructions to consolidate tenants for different country/regions.</span></span>

>[!NOTE]  
><span data-ttu-id="93180-115">Você deve estar atento a todas as assinaturas e contagens de assentos para seus clientes provisionados a partir das contas de transição.</span><span class="sxs-lookup"><span data-stu-id="93180-115">You must be aware of all of the subscriptions and seat counts for your customers provisioned from the transition accounts.</span></span> <span data-ttu-id="93180-116">Você reprovisionará exatamente as mesmas assinaturas com o mesmo número de estações sob a nova conta de CSP Central como parte do processo de migração.</span><span class="sxs-lookup"><span data-stu-id="93180-116">You will be re-provisioning those same exact subscriptions with the same seat counts under the new Central CSP account as part of the migration process.</span></span> <span data-ttu-id="93180-117">Use o recurso de lista de exportação para ajudar a criar uma lista de clientes para mover para o locatário centralizado.</span><span class="sxs-lookup"><span data-stu-id="93180-117">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span> <span data-ttu-id="93180-118">Os parceiros optam por consolidar seus locatários.</span><span class="sxs-lookup"><span data-stu-id="93180-118">Partners choose to consolidate their tenants.</span></span> <span data-ttu-id="93180-119">Quando consolidação for concluída, os parceiros não poderão reverter para seu estado anterior.</span><span class="sxs-lookup"><span data-stu-id="93180-119">Once consolidation is complete, Partners cannot revert to their previous state.</span></span> <span data-ttu-id="93180-120">A ação do cliente também pode ser necessária.</span><span class="sxs-lookup"><span data-stu-id="93180-120">Customer action may also be required.</span></span>

## <a name="prepare-for-migration"></a><span data-ttu-id="93180-121">Preparar para a migração</span><span class="sxs-lookup"><span data-stu-id="93180-121">Prepare for migration</span></span>

- <span data-ttu-id="93180-122">Entre no **Partner Center** com a conta de **transição** (existente) (aquela que você fará a transição) e examine todos os clientes e todos os serviços provisionados para esses clientes.</span><span class="sxs-lookup"><span data-stu-id="93180-122">Sign in to **Partner Center**  with the **Transitioning** (existing) account (the one you will transition) and review of all customers and all of the services provisioned for those customers.</span></span>

   :::image type="content" source="images/regionalcustomer1.png" alt-text="lista de clientes regionais":::

## <a name="migrate-customer-accounts"></a><span data-ttu-id="93180-124">Migrar contas de clientes</span><span class="sxs-lookup"><span data-stu-id="93180-124">Migrate customer accounts</span></span>

1. <span data-ttu-id="93180-125">Entre no **Partner Center** com a conta de **transição** (nova) (a que você está fazendo a transição) e navegue até a lista de clientes de **clientes**.</span><span class="sxs-lookup"><span data-stu-id="93180-125">Sign in to your **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning into) and navigate to the Customers list from **Customers**.</span></span>

2. <span data-ttu-id="93180-126">Selecione Clientes.</span><span class="sxs-lookup"><span data-stu-id="93180-126">Select Customers.</span></span>

3. <span data-ttu-id="93180-127">Clique em **Solicitar uma relação de revendedor**.</span><span class="sxs-lookup"><span data-stu-id="93180-127">Click **Request a reseller relationship**.</span></span> <span data-ttu-id="93180-128">Será exibida uma mensagem de email padrão para apresentar aos seus clientes.</span><span class="sxs-lookup"><span data-stu-id="93180-128">You are presented with a default email message to present to your customers.</span></span> <span data-ttu-id="93180-129">Essa mensagem contém uma URL com a ID da organização exclusiva para sua nova conta do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="93180-129">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4. <span data-ttu-id="93180-130">**Ação do cliente:** Certifique-se de que cada um dos clientes ativos que você deseja migrar visite essa URL.</span><span class="sxs-lookup"><span data-stu-id="93180-130">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="93180-131">Ao abrir a URL, o cliente será solicitado a entrar no portal do Office 365.</span><span class="sxs-lookup"><span data-stu-id="93180-131">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="93180-132">O cliente entra usando a mesma ID da organização que ele usa para acessar os portais de administrador do Azure e do Office 365.</span><span class="sxs-lookup"><span data-stu-id="93180-132">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5. <span data-ttu-id="93180-133">Ao entrar, o Administrador Global da conta do cliente será solicitado a enviar um contrato para conceder privilégios de administrador delegado à nova conta CSP.</span><span class="sxs-lookup"><span data-stu-id="93180-133">After signing in, the Global Admin for the customer account is prompted to submit an agreement to give delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="93180-134">Se concordar, o cliente marca a caixa de seleção e concorda em autorizar o relacionamento.</span><span class="sxs-lookup"><span data-stu-id="93180-134">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="93180-135">Os clientes serão exibidos na lista de clientes do parceiro depois que tiverem enviado o contrato, um por um.</span><span class="sxs-lookup"><span data-stu-id="93180-135">The customers will appear in the partner's customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="93180-136">Migrando assinaturas baseadas em uso do Office 365 e não Azure</span><span class="sxs-lookup"><span data-stu-id="93180-136">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>

1. <span data-ttu-id="93180-137">Depois que o cliente assinar o contrato, você poderá recriar as assinaturas dele em seu locatário parceiro centralizado.</span><span class="sxs-lookup"><span data-stu-id="93180-137">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2. <span data-ttu-id="93180-138">No **Partner Center** , selecione **clientes**.</span><span class="sxs-lookup"><span data-stu-id="93180-138">From **Partner Center** select **Customers**.</span></span>

3. <span data-ttu-id="93180-139">Abra o nome da empresa do cliente que você deseja migrar.</span><span class="sxs-lookup"><span data-stu-id="93180-139">Open the company name for the customer you want to migrate.</span></span>

4. <span data-ttu-id="93180-140">Selecione **Adicionar assinatura**.</span><span class="sxs-lookup"><span data-stu-id="93180-140">Select **Add subscription**.</span></span>

5. <span data-ttu-id="93180-141">Adicione as assinaturas corretas e os números de estações do catálogo.</span><span class="sxs-lookup"><span data-stu-id="93180-141">Add the correct subscriptions and seat counts from the catalog.</span></span> <span data-ttu-id="93180-142">Verificar com as informações fornecidas nas contas de parceiro de **origem da transição**.</span><span class="sxs-lookup"><span data-stu-id="93180-142">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

   :::image type="content" source="images/regionalcustomer2.png" alt-text="lista de clientes":::

6. <span data-ttu-id="93180-144">Clique em **Enviar.**</span><span class="sxs-lookup"><span data-stu-id="93180-144">Click **Submit.**</span></span>

   <span data-ttu-id="93180-145">Agora os serviços serão fornecidos para o cliente da conta de parceiro de **destino da transição**.</span><span class="sxs-lookup"><span data-stu-id="93180-145">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

7. <span data-ttu-id="93180-146">Repita essas etapas para migrar assinaturas para todos os outros clientes.</span><span class="sxs-lookup"><span data-stu-id="93180-146">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="93180-147">Antes de prosseguir para a próxima seção, certifique-se de que todas as assinaturas de cliente existentes nas contas de parceiros de **origem da transição** sejam reprovisionadas sob a conta de parceiro de **destino da transição**.</span><span class="sxs-lookup"><span data-stu-id="93180-147">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

> [!NOTE]
> <span data-ttu-id="93180-148">Os parceiros devem suspender as assinaturas na **transição da conta de locatário do** parceiro no centro de parceiros no mesmo dia em que essas assinaturas são transferidas e configuradas na **transição para** a conta de locatário do parceiro no Partner Center para garantir que a cobrança dupla não ocorra.</span><span class="sxs-lookup"><span data-stu-id="93180-148">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="93180-149">As solicitações de suporte serão negadas para créditos decorrentes de alguma sobreposição de cobranças que ocorra devido à não configuração das assinaturas de **origem da transição** como desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="93180-149">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to disabled.</span></span>

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="93180-150">Desabilitando as assinaturas do Office 365 na conta de parceiro de origem da transição</span><span class="sxs-lookup"><span data-stu-id="93180-150">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>

<span data-ttu-id="93180-151">Desabilitar a assinatura de CSP sob as contas de parceiros de **destino da transição** impede qualquer cobrança futura.</span><span class="sxs-lookup"><span data-stu-id="93180-151">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="93180-152">Você não precisa desabilitar manualmente as assinaturas do Azure, elas são desativadas automaticamente durante o processo de migração.</span><span class="sxs-lookup"><span data-stu-id="93180-152">You do not have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1. <span data-ttu-id="93180-153">Entre no **Partner Center** com a **transição da conta do** CSP e navegue até a lista de clientes.</span><span class="sxs-lookup"><span data-stu-id="93180-153">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2. <span data-ttu-id="93180-154">Abra o cliente com assinaturas para desabilitar e, em seguida, selecione a primeira oferta a ser desabilitada.</span><span class="sxs-lookup"><span data-stu-id="93180-154">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>

3. <span data-ttu-id="93180-155">Defina a assinatura como **suspensa** e clique em **enviar**.</span><span class="sxs-lookup"><span data-stu-id="93180-155">Set the subscription to **suspended**, and then click **submit**.</span></span>

   >[!Note]
   ><span data-ttu-id="93180-156">A suspensão da assinatura garante que a cobrança dupla não ocorra.</span><span class="sxs-lookup"><span data-stu-id="93180-156">Suspending the subscription ensures double billing does not occur.</span></span>

   <span data-ttu-id="93180-157">A assinatura é exibida como **suspensa** na lista de assinaturas.</span><span class="sxs-lookup"><span data-stu-id="93180-157">The Subscription shows **suspended** on the subscriptions list.</span></span>

4. <span data-ttu-id="93180-158">Repita essas etapas para todas as assinaturas sob o cliente.</span><span class="sxs-lookup"><span data-stu-id="93180-158">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="93180-159">Verifique se todas são exibidas como **suspensas**.</span><span class="sxs-lookup"><span data-stu-id="93180-159">Verify all show **suspended.**</span></span>

5. <span data-ttu-id="93180-160">Selecione o próximo cliente na lista e repita o processo para desabilitar todas as assinaturas.</span><span class="sxs-lookup"><span data-stu-id="93180-160">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="93180-161">Migrando assinaturas baseadas em uso do Azure</span><span class="sxs-lookup"><span data-stu-id="93180-161">Migrating Azure usage-based subscriptions</span></span>

<span data-ttu-id="93180-162">O Azure, as assinaturas do CSP com base no uso não precisam ser migradas manualmente, como é o caso das assinaturas do CSP do Office 365.</span><span class="sxs-lookup"><span data-stu-id="93180-162">Azure, usage-based CSP subscriptions do not need to be migrated manually as is the case with Office 365 CSP subscriptions.</span></span> <span data-ttu-id="93180-163">O suporte do Microsoft Azure pode migrar as assinaturas do Azure, bem como todos os serviços ou recursos implantados, das contas de revendedor CSP de **origem da transição** para a conta de revendedor CSP de **destino da transição**.</span><span class="sxs-lookup"><span data-stu-id="93180-163">Microsoft Azure Support can migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="93180-164">Não haverá qualquer interrupção do serviço para o cliente durante a transição.</span><span class="sxs-lookup"><span data-stu-id="93180-164">There will be no disruption of service to the customer during this transition.</span></span>

1. <span data-ttu-id="93180-165">Certifique-se de que as contas de clientes que precisam de assinaturas do Azure migradas aceitem o contrato para serem associadas à nova conta CSP de **destino da transição**.</span><span class="sxs-lookup"><span data-stu-id="93180-165">Ensure that the customer accounts that need Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>

2. <span data-ttu-id="93180-166">Os parceiros notificam a Microsoft quais contas de clientes que têm assinaturas do Azure estão prontas para serem migradas e fornece os nomes de empresa do cliente.</span><span class="sxs-lookup"><span data-stu-id="93180-166">Partners notify Microsoft which customer accounts that have Azure subscriptions are ready to migrate, and provides those customer's company names.</span></span>

3. <span data-ttu-id="93180-167">A Microsoft migra as assinaturas baseadas em uso do Azure e notifica o parceiro quando a migração é concluída.</span><span class="sxs-lookup"><span data-stu-id="93180-167">Microsoft migrates the Azure usage-based subscriptions and notifies the partner when the migration is complete.</span></span>

4. <span data-ttu-id="93180-168">O parceiro confirma se agora a assinatura do Azure sob a conta de revendedor CSP de **origem da transição** é exibida como suspensa no Partner Center, na seção de assinaturas de cliente.</span><span class="sxs-lookup"><span data-stu-id="93180-168">The partner confirms that the Azure subscription under the **Transitioning From** CSP reseller accounts now shows suspended in the Partner Center under the customer subscriptions section.</span></span>

5. <span data-ttu-id="93180-169">O parceiro confirma se agora a assinatura do Azure sob a conta de revendedor CSP de **destino da transição** mostra o status de **ativa** no Partner Center, na seção de assinaturas de cliente.</span><span class="sxs-lookup"><span data-stu-id="93180-169">The partner confirms that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in the Partner Center under the customer subscriptions section.</span></span>

   >[!Note]
   > <span data-ttu-id="93180-170">Desabilitar as assinaturas no cliente não altera a aparência do cliente na lista de clientes.</span><span class="sxs-lookup"><span data-stu-id="93180-170">Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="93180-171">Atualmente, não há uma opção para remover clientes da lista.</span><span class="sxs-lookup"><span data-stu-id="93180-171">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="93180-172">Os parceiros devem evitar readicionar assinaturas para esses clientes a partir da conta de **destino da transição** no futuro.</span><span class="sxs-lookup"><span data-stu-id="93180-172">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

6. <span data-ttu-id="93180-173">Repita essas etapas para todas as assinaturas em todos os seus clientes para impedir encargos futuros nas contas de **origem da transição**.</span><span class="sxs-lookup"><span data-stu-id="93180-173">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="93180-174">O parceiro receberá uma fatura final com um crédito pelo número de dias não utilizados entre o dia de cancelamento e o último dia do período de cobrança.</span><span class="sxs-lookup"><span data-stu-id="93180-174">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="93180-175">Nenhuma fatura futura será gerada após esse período de cobrança final.</span><span class="sxs-lookup"><span data-stu-id="93180-175">No future invoices will generate after that final billing period.</span></span>

### <a name="additional-information"></a><span data-ttu-id="93180-176">Informações adicionais</span><span class="sxs-lookup"><span data-stu-id="93180-176">Additional information</span></span>

- <span data-ttu-id="93180-177">A desabilitação da assinatura da conta do CSP em **transição** não afeta o serviço do cliente final, desde que o serviço tenha sido provisionado da **transição para** a conta do CSP antes de desabilitar a assinatura.</span><span class="sxs-lookup"><span data-stu-id="93180-177">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer's service as long as the service was provisioned from the **Transitioning To** CSP account prior to disabling the subscription.</span></span>

- <span data-ttu-id="93180-178">As assinaturas não podem ser usadas pelo cliente e não geram encargos quando suspensos ou cancelados.</span><span class="sxs-lookup"><span data-stu-id="93180-178">Subscriptions cannot be used by the customer and do not generate charges when suspended or canceled.</span></span>

- <span data-ttu-id="93180-179">Atualmente, não há uma maneira de remover completamente um cliente da Lista de clientes.</span><span class="sxs-lookup"><span data-stu-id="93180-179">There is currently no way to remove a customer from the Customers list completely.</span></span>

    >[!Note]
    > <span data-ttu-id="93180-180">Os parceiros devem suspender as assinaturas na **transição da conta de locatário do** parceiro no centro de parceiros no mesmo dia em que essas assinaturas são transferidas e configuradas na **transição para** a conta de locatário do parceiro no Partner Center para garantir que a cobrança dupla não ocorra.</span><span class="sxs-lookup"><span data-stu-id="93180-180">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned to and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="93180-181">A Microsoft não dará suporte a solicitações de créditos devido a qualquer sobreposição na cobrança que ocorre de não definir corretamente a **transição de** assinaturas para suspensa.</span><span class="sxs-lookup"><span data-stu-id="93180-181">Microsoft will not support requests for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

### <a name="simplify-migration-using-export"></a><span data-ttu-id="93180-182">Simplificar a migração usando Exportar</span><span class="sxs-lookup"><span data-stu-id="93180-182">Simplify migration using Export</span></span>

<span data-ttu-id="93180-183">Usando a **função Exportar**, você pode capturar as assinaturas que serão usadas em sua nova estrutura consolidada:</span><span class="sxs-lookup"><span data-stu-id="93180-183">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1. <span data-ttu-id="93180-184">Clique em **clientes** no Partner Center para ver a lista de clientes em sua estrutura existente.</span><span class="sxs-lookup"><span data-stu-id="93180-184">Click **Customers** on Partner Center to see the list of customers in your existing structure.</span></span>

2. <span data-ttu-id="93180-185">Abra o nome do cliente desejado.</span><span class="sxs-lookup"><span data-stu-id="93180-185">Open the desired customer name.</span></span>

3. <span data-ttu-id="93180-186">Na página **Assinaturas**, clique em **Exportar Assinaturas** para exportar os detalhes das assinaturas para um arquivo do Excel.</span><span class="sxs-lookup"><span data-stu-id="93180-186">On the **Subscriptions** page, click **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4. <span data-ttu-id="93180-187">Use essa lista para recriar as assinaturas em seu novo locatário consolidado.</span><span class="sxs-lookup"><span data-stu-id="93180-187">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="93180-188">Registro de API</span><span class="sxs-lookup"><span data-stu-id="93180-188">API registration</span></span>

<span data-ttu-id="93180-189">Para obter mais informações sobre o registro de API, consulte [Configurar o acesso à API no Partner Center](https://go.microsoft.com/fwlink/?linkid=847990).</span><span class="sxs-lookup"><span data-stu-id="93180-189">For more information about API registration, see [Set up API access in Partner Center](https://go.microsoft.com/fwlink/?linkid=847990).</span></span>
