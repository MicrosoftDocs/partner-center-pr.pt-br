---
title: Consolidação de locatários de autorização regional do CSP
ms.topic: how-to
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Use estas instruções para consolidar locatários para países/regiões diferentes. Isso inclui etapas para migrar contas de cliente e assinaturas de cliente.
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: 0ae107c005eaf6b8ff8a6d99a91075ebc560cf81
ms.sourcegitcommit: 940dad4527f51781f6f966e196b3aa08389613a2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/13/2020
ms.locfileid: "92006779"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="d6eea-104">Instruções para a consolidação de locatários de autorização regional do CSP</span><span class="sxs-lookup"><span data-stu-id="d6eea-104">Instructions for CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="d6eea-105">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="d6eea-105">**Applies to**</span></span>

-  <span data-ttu-id="d6eea-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="d6eea-106">Partner Center</span></span>
-  <span data-ttu-id="d6eea-107">Partner Center do Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="d6eea-107">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="d6eea-108">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="d6eea-108">**Appropriate roles**</span></span>

- <span data-ttu-id="d6eea-109">Administrador global</span><span class="sxs-lookup"><span data-stu-id="d6eea-109">Global admin</span></span>
- <span data-ttu-id="d6eea-110">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="d6eea-110">Admin agent</span></span>

<span data-ttu-id="d6eea-111">\[Algumas informações estão relacionadas ao produto de pré-lançamento que pode ser substancialmente modificado antes de ser lançado comercialmente.</span><span class="sxs-lookup"><span data-stu-id="d6eea-111">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="d6eea-112">A Microsoft não faz nenhuma garantia, expressa ou implícita, com relação às informações fornecidas aqui.\]</span><span class="sxs-lookup"><span data-stu-id="d6eea-112">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="d6eea-113">Você pode consolidar locatários para sua empresa.</span><span class="sxs-lookup"><span data-stu-id="d6eea-113">You can consolidate tenants for your business.</span></span> <span data-ttu-id="d6eea-114">Use estas instruções para consolidar locatários para países/regiões diferentes.</span><span class="sxs-lookup"><span data-stu-id="d6eea-114">Use these instructions to consolidate tenants for different country/regions.</span></span>

>[!NOTE]  
><span data-ttu-id="d6eea-115">Você deve estar ciente de todas as assinaturas e contagens de licenças provisionadas para cada um de seus clientes na conta da qual está fazendo a transição.</span><span class="sxs-lookup"><span data-stu-id="d6eea-115">You must be aware of all of the provisioned subscriptions and license counts for each of your customers in the account you are transitioning from.</span></span> <span data-ttu-id="d6eea-116">Você estará reprovisionando as mesmas assinaturas exatas com as mesmas contagens de licenças na nova conta do CSP central como parte do processo de migração.</span><span class="sxs-lookup"><span data-stu-id="d6eea-116">You will be re-provisioning those same exact subscriptions with the same license counts under the new central CSP account as part of the migration process.</span></span> <span data-ttu-id="d6eea-117">Use o recurso de lista de exportação para ajudar a criar uma lista de clientes para mover para o locatário centralizado.</span><span class="sxs-lookup"><span data-stu-id="d6eea-117">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span>  <span data-ttu-id="d6eea-118">Após a conclusão da consolidação, você não poderá reverter para o estado anterior do locatário.</span><span class="sxs-lookup"><span data-stu-id="d6eea-118">Once consolidation is complete, you can't revert to the previous tenant state.</span></span> <span data-ttu-id="d6eea-119">A ação do cliente também pode ser necessária.</span><span class="sxs-lookup"><span data-stu-id="d6eea-119">Customer action may also be required.</span></span>

## <a name="prepare-for-migration"></a><span data-ttu-id="d6eea-120">Preparar para a migração</span><span class="sxs-lookup"><span data-stu-id="d6eea-120">Prepare for migration</span></span>

- <span data-ttu-id="d6eea-121">Entre no **Partner Center**  usando a conta de **transição** (aquela que você fará a transição para a nova conta) e examine todos os clientes e todos os serviços provisionados para esses clientes.</span><span class="sxs-lookup"><span data-stu-id="d6eea-121">Sign in to **Partner Center**  using the **Transitioning** account (the one you will transition to the new account), and review of all customers and all of the services provisioned for those customers.</span></span>

- <span data-ttu-id="d6eea-122">Saia desta conta.</span><span class="sxs-lookup"><span data-stu-id="d6eea-122">Sign out of this account.</span></span>

## <a name="migrate-customer-accounts"></a><span data-ttu-id="d6eea-123">Migrar contas de clientes</span><span class="sxs-lookup"><span data-stu-id="d6eea-123">Migrate customer accounts</span></span>

1. <span data-ttu-id="d6eea-124">Entre no **Partner Center**  com a conta de **transição** (nova) (aquela na qual você está fazendo a transição de clientes).</span><span class="sxs-lookup"><span data-stu-id="d6eea-124">Sign in to **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning customers into).</span></span>

2. <span data-ttu-id="d6eea-125">Selecione **Clientes**.</span><span class="sxs-lookup"><span data-stu-id="d6eea-125">Select **Customers**.</span></span>

3. <span data-ttu-id="d6eea-126">Clique em **Solicitar uma relação de revendedor**.</span><span class="sxs-lookup"><span data-stu-id="d6eea-126">Click **Request a reseller relationship**.</span></span> <span data-ttu-id="d6eea-127">Você verá uma mensagem de email padrão para enviar aos seus clientes.</span><span class="sxs-lookup"><span data-stu-id="d6eea-127">You are presented with a default email message to send to your customers.</span></span> <span data-ttu-id="d6eea-128">Essa mensagem contém uma URL com a ID da organização exclusiva para sua nova conta do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="d6eea-128">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4. <span data-ttu-id="d6eea-129">**Ação do cliente:** Certifique-se de que cada um dos clientes ativos que você deseja migrar visite essa URL.</span><span class="sxs-lookup"><span data-stu-id="d6eea-129">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="d6eea-130">Ao abrir a URL, o cliente será solicitado a entrar no portal do Office 365.</span><span class="sxs-lookup"><span data-stu-id="d6eea-130">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="d6eea-131">O cliente entra usando a mesma ID da organização que ele usa para acessar os portais de administrador do Azure e do Office 365.</span><span class="sxs-lookup"><span data-stu-id="d6eea-131">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5. <span data-ttu-id="d6eea-132">Depois de entrar, o administrador global da **conta do cliente** é solicitado a enviar um contrato que concede privilégios de administrador delegado à nova conta do CSP.</span><span class="sxs-lookup"><span data-stu-id="d6eea-132">After signing in, the Global Admin for the **customer account** is prompted to submit an agreement that gives delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="d6eea-133">Se concordar, o cliente marca a caixa de seleção e concorda em autorizar o relacionamento.</span><span class="sxs-lookup"><span data-stu-id="d6eea-133">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="d6eea-134">Os clientes serão exibidos na lista de clientes do parceiro depois que tiverem enviado o contrato, um por um.</span><span class="sxs-lookup"><span data-stu-id="d6eea-134">The customers will appear in the partner's customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="d6eea-135">Migrando assinaturas baseadas em uso do Office 365 e não Azure</span><span class="sxs-lookup"><span data-stu-id="d6eea-135">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>

1. <span data-ttu-id="d6eea-136">Depois que o cliente assinar o contrato, você poderá recriar as assinaturas dele em seu locatário parceiro centralizado.</span><span class="sxs-lookup"><span data-stu-id="d6eea-136">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2. <span data-ttu-id="d6eea-137">No **Partner Center** , selecione **clientes**.</span><span class="sxs-lookup"><span data-stu-id="d6eea-137">From **Partner Center** select **Customers**.</span></span>

3. <span data-ttu-id="d6eea-138">Abra o nome da empresa do cliente que você deseja migrar.</span><span class="sxs-lookup"><span data-stu-id="d6eea-138">Open the company name for the customer you want to migrate.</span></span>

4. <span data-ttu-id="d6eea-139">Selecione **Adicionar assinatura**.</span><span class="sxs-lookup"><span data-stu-id="d6eea-139">Select **Add subscription**.</span></span>

5. <span data-ttu-id="d6eea-140">Adicione as assinaturas e contagens de licenças corretas do catálogo.</span><span class="sxs-lookup"><span data-stu-id="d6eea-140">Add the correct subscriptions and license counts from the catalog.</span></span> <span data-ttu-id="d6eea-141">Verificar com as informações fornecidas nas contas de parceiro de **origem da transição**.</span><span class="sxs-lookup"><span data-stu-id="d6eea-141">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

   :::image type="content" source="images/regionalcustomer2.png" alt-text="lista de clientes":::

6. <span data-ttu-id="d6eea-143">Clique em **Enviar.**</span><span class="sxs-lookup"><span data-stu-id="d6eea-143">Click **Submit.**</span></span>

   <span data-ttu-id="d6eea-144">Agora os serviços serão fornecidos para o cliente da conta de parceiro de **destino da transição**.</span><span class="sxs-lookup"><span data-stu-id="d6eea-144">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

7. <span data-ttu-id="d6eea-145">Repita essas etapas para migrar assinaturas para todos os outros clientes.</span><span class="sxs-lookup"><span data-stu-id="d6eea-145">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="d6eea-146">Antes de prosseguir para a próxima seção, certifique-se de que todas as assinaturas de cliente existentes nas contas de parceiros de **origem da transição** sejam reprovisionadas sob a conta de parceiro de **destino da transição**.</span><span class="sxs-lookup"><span data-stu-id="d6eea-146">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

> [!NOTE]
> <span data-ttu-id="d6eea-147">Os parceiros devem suspender as assinaturas na **transição da conta de locatário do** parceiro no centro de parceiros no mesmo dia em que essas assinaturas são transferidas e configuradas na **transição para** a conta de locatário do parceiro no Partner Center para garantir que a cobrança dupla não ocorra.</span><span class="sxs-lookup"><span data-stu-id="d6eea-147">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="d6eea-148">As solicitações de suporte serão negadas para créditos devido a qualquer sobreposição na cobrança que ocorre de não desabilitar corretamente a **transição de** assinaturas.</span><span class="sxs-lookup"><span data-stu-id="d6eea-148">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly disabling the **Transitioning From** subscriptions.</span></span>

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="d6eea-149">Desabilitando as assinaturas do Office 365 na conta de parceiro de origem da transição</span><span class="sxs-lookup"><span data-stu-id="d6eea-149">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>

<span data-ttu-id="d6eea-150">Desabilitar a assinatura de CSP sob as contas de parceiros de **destino da transição** impede qualquer cobrança futura.</span><span class="sxs-lookup"><span data-stu-id="d6eea-150">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="d6eea-151">Você não precisa desabilitar manualmente as assinaturas do Azure, pois as assinaturas do Azure são automaticamente desabilitadas durante o processo de migração.</span><span class="sxs-lookup"><span data-stu-id="d6eea-151">You don't have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1. <span data-ttu-id="d6eea-152">Entre no **Partner Center** com a **transição da conta do** CSP e navegue até a lista de clientes.</span><span class="sxs-lookup"><span data-stu-id="d6eea-152">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2. <span data-ttu-id="d6eea-153">Abra o cliente com assinaturas para desabilitar e, em seguida, selecione a primeira oferta a ser desabilitada.</span><span class="sxs-lookup"><span data-stu-id="d6eea-153">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>

3. <span data-ttu-id="d6eea-154">Defina a assinatura como **suspensa** e clique em **enviar**.</span><span class="sxs-lookup"><span data-stu-id="d6eea-154">Set the subscription to **suspended**, and then click **submit**.</span></span>

   >[!Note]
   ><span data-ttu-id="d6eea-155">A suspensão da assinatura garante que a cobrança dupla não ocorra.</span><span class="sxs-lookup"><span data-stu-id="d6eea-155">Suspending the subscription ensures double billing does not occur.</span></span>

   <span data-ttu-id="d6eea-156">A assinatura mostra **suspensa** na lista de assinaturas.</span><span class="sxs-lookup"><span data-stu-id="d6eea-156">The subscription shows **suspended** on the subscriptions list.</span></span>

4. <span data-ttu-id="d6eea-157">Repita essas etapas para todas as assinaturas sob o cliente.</span><span class="sxs-lookup"><span data-stu-id="d6eea-157">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="d6eea-158">Verifique se todas são exibidas como **suspensas**.</span><span class="sxs-lookup"><span data-stu-id="d6eea-158">Verify all show **suspended.**</span></span>

5. <span data-ttu-id="d6eea-159">Selecione o próximo cliente na lista e repita o processo para desabilitar todas as assinaturas.</span><span class="sxs-lookup"><span data-stu-id="d6eea-159">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="d6eea-160">Migrando assinaturas baseadas em uso do Azure</span><span class="sxs-lookup"><span data-stu-id="d6eea-160">Migrating Azure usage-based subscriptions</span></span>

<span data-ttu-id="d6eea-161">Ao contrário das assinaturas do CSP do Office 365, as assinaturas do CSP com base no uso do Azure não precisam ser migradas manualmente.</span><span class="sxs-lookup"><span data-stu-id="d6eea-161">Unlike the Office 365 CSP subscriptions, Azure, usage-based CSP subscriptions do not need to be migrated manually.</span></span> <span data-ttu-id="d6eea-162">Microsoft Azure suporte migrará as assinaturas do Azure, bem como todos os serviços ou recursos implantados da **transição de contas de** revendedor do CSP para a **transição para** a conta de revendedor do CSP.</span><span class="sxs-lookup"><span data-stu-id="d6eea-162">Microsoft Azure Support will migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="d6eea-163">Não haverá qualquer interrupção do serviço para o cliente durante a transição.</span><span class="sxs-lookup"><span data-stu-id="d6eea-163">There will be no disruption of service to the customer during this transition.</span></span>

1. <span data-ttu-id="d6eea-164">Verifique se as contas de cliente que terão as assinaturas do Azure migradas aceitaram o contrato a ser associado à nova **transição para** a conta do CSP.</span><span class="sxs-lookup"><span data-stu-id="d6eea-164">Ensure that the customer accounts that will have Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>

2. <span data-ttu-id="d6eea-165">Você notificará a Microsoft de quais contas de clientes estão prontas para migrar e fornecerá os nomes de empresa do cliente.</span><span class="sxs-lookup"><span data-stu-id="d6eea-165">You will notify Microsoft of which customer accounts are ready to migrate, and provide those customer's company names.</span></span>

3. <span data-ttu-id="d6eea-166">A Microsoft migra as assinaturas baseadas em uso do Azure e notifica você quando a migração é concluída.</span><span class="sxs-lookup"><span data-stu-id="d6eea-166">Microsoft migrates the Azure usage-based subscriptions and notifies you when the migration is complete.</span></span>

4. <span data-ttu-id="d6eea-167">Você precisa confirmar se a assinatura do Azure na **transição da conta de** revendedor do CSP agora está marcada como **suspensa** no Partner Center na seção assinaturas do cliente.</span><span class="sxs-lookup"><span data-stu-id="d6eea-167">You need to confirm that the Azure subscription under the **Transitioning From** CSP reseller account now is marked **suspended** in Partner Center under the customer subscriptions section.</span></span>

5. <span data-ttu-id="d6eea-168">Confirme se a assinatura do Azure na conta de revendedor do CSP em **transição** agora mostra um status de **ativo** no Partner Center na seção assinaturas do cliente.</span><span class="sxs-lookup"><span data-stu-id="d6eea-168">Confirm that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in Partner Center under the customer subscriptions section.</span></span>

   >[!Note]
   > <span data-ttu-id="d6eea-169">Desabilitar as assinaturas no cliente não altera a aparência do cliente na lista de clientes.</span><span class="sxs-lookup"><span data-stu-id="d6eea-169">Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="d6eea-170">Atualmente, não há uma opção para remover clientes da lista.</span><span class="sxs-lookup"><span data-stu-id="d6eea-170">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="d6eea-171">Os parceiros devem evitar readicionar assinaturas para esses clientes a partir da conta de **destino da transição** no futuro.</span><span class="sxs-lookup"><span data-stu-id="d6eea-171">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

6. <span data-ttu-id="d6eea-172">Repita essas etapas para todas as assinaturas em todos os seus clientes para impedir encargos futuros nas contas de **origem da transição**.</span><span class="sxs-lookup"><span data-stu-id="d6eea-172">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="d6eea-173">O parceiro receberá uma fatura final com um crédito pelo número de dias não utilizados entre o dia de cancelamento e o último dia do período de cobrança.</span><span class="sxs-lookup"><span data-stu-id="d6eea-173">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="d6eea-174">Nenhuma fatura futura será gerada após esse período de cobrança final.</span><span class="sxs-lookup"><span data-stu-id="d6eea-174">No future invoices will generate after that final billing period.</span></span>

### <a name="additional-information"></a><span data-ttu-id="d6eea-175">Informações adicionais</span><span class="sxs-lookup"><span data-stu-id="d6eea-175">Additional information</span></span>

- <span data-ttu-id="d6eea-176">A desabilitação da assinatura da conta do CSP em **transição** não afeta o serviço do cliente final, desde que o serviço tenha sido provisionado da **transição para** a conta do CSP antes de desabilitar a assinatura.</span><span class="sxs-lookup"><span data-stu-id="d6eea-176">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer's service as long as the service was provisioned from the **Transitioning To** CSP account prior to disabling the subscription.</span></span>

- <span data-ttu-id="d6eea-177">As assinaturas não podem ser usadas pelo cliente e não geram encargos quando suspensos ou cancelados.</span><span class="sxs-lookup"><span data-stu-id="d6eea-177">Subscriptions cannot be used by the customer and do not generate charges when suspended or canceled.</span></span>

- <span data-ttu-id="d6eea-178">Atualmente, não há nenhuma maneira de remover completamente um cliente da lista de **clientes** .</span><span class="sxs-lookup"><span data-stu-id="d6eea-178">There is currently no way to remove a customer completely from the **Customers** list.</span></span>
- 
    >[!Note]
    > <span data-ttu-id="d6eea-179">Os parceiros devem suspender as assinaturas na **transição da conta de locatário do** parceiro no centro de parceiros no mesmo dia em que as assinaturas são transferidas e configuradas na **transição para** a conta para garantir que a cobrança dupla não ocorra.</span><span class="sxs-lookup"><span data-stu-id="d6eea-179">Partners must suspend subscriptions on the **Transitioning From** partner tenant account in Partner Center the same day those subscriptions are transitioned to and set up under the **Transitioning To** account to ensure double billing does not occur.</span></span> <span data-ttu-id="d6eea-180">A Microsoft não dará suporte a solicitações de créditos devido a qualquer sobreposição na cobrança que ocorre de não definir corretamente a **transição de** assinaturas para suspensa.</span><span class="sxs-lookup"><span data-stu-id="d6eea-180">Microsoft will not support requests for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

### <a name="simplify-migration-using-export"></a><span data-ttu-id="d6eea-181">Simplificar a migração usando Exportar</span><span class="sxs-lookup"><span data-stu-id="d6eea-181">Simplify migration using Export</span></span>

<span data-ttu-id="d6eea-182">Usando a **função Exportar**, você pode capturar as assinaturas que serão usadas em sua nova estrutura consolidada:</span><span class="sxs-lookup"><span data-stu-id="d6eea-182">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1. <span data-ttu-id="d6eea-183">Clique em **clientes** no Partner Center para ver a lista de clientes.</span><span class="sxs-lookup"><span data-stu-id="d6eea-183">Click **Customers** on Partner Center to see the list of customers.</span></span> 

2. <span data-ttu-id="d6eea-184">Abra o nome do cliente desejado.</span><span class="sxs-lookup"><span data-stu-id="d6eea-184">Open the desired customer name.</span></span>

3. <span data-ttu-id="d6eea-185">Na página **Assinaturas**, clique em **Exportar Assinaturas** para exportar os detalhes das assinaturas para um arquivo do Excel.</span><span class="sxs-lookup"><span data-stu-id="d6eea-185">On the **Subscriptions** page, click **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4. <span data-ttu-id="d6eea-186">Use essa lista para recriar as assinaturas em seu novo locatário consolidado.</span><span class="sxs-lookup"><span data-stu-id="d6eea-186">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="d6eea-187">Registro de API</span><span class="sxs-lookup"><span data-stu-id="d6eea-187">API registration</span></span>

<span data-ttu-id="d6eea-188">Para obter mais informações sobre o registro de API, consulte [Configurar o acesso à API no Partner Center](/partner-center/develop/set-up-api-access-in-partner-center).</span><span class="sxs-lookup"><span data-stu-id="d6eea-188">For more information about API registration, see [Set up API access in Partner Center](/partner-center/develop/set-up-api-access-in-partner-center).</span></span>

## <a name="next-steps"></a><span data-ttu-id="d6eea-189">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="d6eea-189">Next steps</span></span>

- [<span data-ttu-id="d6eea-190">Programa de provedor de soluções na nuvem mercados regionais e moedas em que você pode vender ofertas de CSP</span><span class="sxs-lookup"><span data-stu-id="d6eea-190">Cloud Solution Provider program regional markets and currencies where you can sell CSP offers</span></span>](regional-authorization-overview.md)
