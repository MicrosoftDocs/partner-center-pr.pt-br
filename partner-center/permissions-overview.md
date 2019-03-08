---
title: Atribuir funções e permissões de usuários | Partner Center
ms.topic: article
ms.date: 10/29/2018
description: Todos os funcionários que precisam para trabalhar no Partner Center devem ser atribuído a uma função.
author: LauraBrenner
ms.author: labrenne
keywords: funções, permissões, administrador, agente
ms.localizationpriority: medium
ms.openlocfilehash: 038a2d6f4d58bbd9a71a2b241ee68982e0e7ef0a
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2019
ms.locfileid: "57587739"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="ba7b8-104">Atribuir funções e permissões de usuário</span><span class="sxs-lookup"><span data-stu-id="ba7b8-104">Assign users roles and permissions</span></span>


<span data-ttu-id="ba7b8-105">Você configurou o perfil de parceiro, incluindo nome legal e endereço, detalhes de suporte, isenções de imposto sobre arquivos, informações bancárias e o contato principal para a sua empresa.</span><span class="sxs-lookup"><span data-stu-id="ba7b8-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="ba7b8-106">Próxima etapa: configurar os usuários configurados com senhas e funções, para que eles possam começar a trabalhar no Partner Center com você.</span><span class="sxs-lookup"><span data-stu-id="ba7b8-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="ba7b8-107">Configurar seus funcionários para trabalhar no Partner Center</span><span class="sxs-lookup"><span data-stu-id="ba7b8-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="ba7b8-108">Os tipos de acesso que os usuários têm Partner Center, as funções e permissões que você conceda a você determinar.</span><span class="sxs-lookup"><span data-stu-id="ba7b8-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="ba7b8-109">As funções estão relacionadas aos programas de que sua empresa está envolvida no.</span><span class="sxs-lookup"><span data-stu-id="ba7b8-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="ba7b8-110">Por exemplo, se sua empresa é uma empresa de provedor de solução de nuvem (CSP), você não somente terá o Azure AD padrão funções de gerenciamento como administrador global do locatário, mas será necessário a funções específicas para o programa CSP.</span><span class="sxs-lookup"><span data-stu-id="ba7b8-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="ba7b8-111">Cada programa tem funções específicas a ela.</span><span class="sxs-lookup"><span data-stu-id="ba7b8-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="ba7b8-112">As funções de locatário do Azure Active Directory (AAD) incluem administrador global, administrador de usuários e funções CSP.</span><span class="sxs-lookup"><span data-stu-id="ba7b8-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="ba7b8-113">Funções do AAD não incluem MPN admin, administrador de perfil de negócios, administração de indicação, incentivo administrador e usuário incentivo.</span><span class="sxs-lookup"><span data-stu-id="ba7b8-113">Non-AAD roles include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="ba7b8-114">Gerenciar transações comerciais no Partner Center (Azure AD e as funções do CSP)</span><span class="sxs-lookup"><span data-stu-id="ba7b8-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="ba7b8-115">**Função**</span><span class="sxs-lookup"><span data-stu-id="ba7b8-115">**Role**</span></span>|<span data-ttu-id="ba7b8-116">**O que pode fazer**</span><span class="sxs-lookup"><span data-stu-id="ba7b8-116">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="ba7b8-117">Administração global</span><span class="sxs-lookup"><span data-stu-id="ba7b8-117">Global admin</span></span>|<span data-ttu-id="ba7b8-118">• Podem acessar todos os Microsoft/serviços de conta com privilégios totais</span><span class="sxs-lookup"><span data-stu-id="ba7b8-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="ba7b8-119">• Criar tíquetes de suporte para o Centro de parceiros</span><span class="sxs-lookup"><span data-stu-id="ba7b8-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="ba7b8-120">• Exibir contratos, listas de preços e ofertas</span><span class="sxs-lookup"><span data-stu-id="ba7b8-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="ba7b8-121">• Exibir, criar e gerenciar os usuários do parceiro</span><span class="sxs-lookup"><span data-stu-id="ba7b8-121">• View, create, and manage partner users</span></span>|
|<span data-ttu-id="ba7b8-122">Usuário administrador</span><span class="sxs-lookup"><span data-stu-id="ba7b8-122">User Admin</span></span>   | <span data-ttu-id="ba7b8-123">• Exibir, criar e gerenciar usuários</span><span class="sxs-lookup"><span data-stu-id="ba7b8-123">•   View, create, and manage users</span></span>
||<span data-ttu-id="ba7b8-124">• Exibir todos os perfis de parceiros</span><span class="sxs-lookup"><span data-stu-id="ba7b8-124">• View all partner profiles</span></span>
||<span data-ttu-id="ba7b8-125">• Exibir, criar e gerenciar os usuários do parceiro</span><span class="sxs-lookup"><span data-stu-id="ba7b8-125">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="ba7b8-126">Usuário padrão</span><span class="sxs-lookup"><span data-stu-id="ba7b8-126">Default user</span></span>|  <span data-ttu-id="ba7b8-127">Exibir meu perfil</span><span class="sxs-lookup"><span data-stu-id="ba7b8-127">View My profile</span></span>   |
|<span data-ttu-id="ba7b8-128">Agente administrador</span><span class="sxs-lookup"><span data-stu-id="ba7b8-128">Admin agent</span></span> | <span data-ttu-id="ba7b8-129">• Gerenciamento de cliente</span><span class="sxs-lookup"><span data-stu-id="ba7b8-129">•    Customer management</span></span>
||<span data-ttu-id="ba7b8-130">• Adicionar lista de dispositivos para o Centro de parceiros <</span><span class="sxs-lookup"><span data-stu-id="ba7b8-130">• Add device list to the Partner Center<</span></span>
||<span data-ttu-id="ba7b8-131">• Criar e aplicar perfis de dispositivos</span><span class="sxs-lookup"><span data-stu-id="ba7b8-131">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="ba7b8-132">• Gerenciamento de assinatura</span><span class="sxs-lookup"><span data-stu-id="ba7b8-132">• Subscription management</span></span>
||<span data-ttu-id="ba7b8-133">• Integridade e o serviço de solicitações de clientes</span><span class="sxs-lookup"><span data-stu-id="ba7b8-133">• Service health and service requests for customers</span></span>
||<span data-ttu-id="ba7b8-134">• Solicitação delegada privilégios de administrador</span><span class="sxs-lookup"><span data-stu-id="ba7b8-134">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="ba7b8-135">• Exibir preço e ofertas</span><span class="sxs-lookup"><span data-stu-id="ba7b8-135">• View pricing and offers</span></span>
||<span data-ttu-id="ba7b8-136">• Cobrança</span><span class="sxs-lookup"><span data-stu-id="ba7b8-136">• Billing</span></span>
||<span data-ttu-id="ba7b8-137">• Administrar em nome de um cliente</span><span class="sxs-lookup"><span data-stu-id="ba7b8-137">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="ba7b8-138">• Registre-se um valor adicionado revendedor</span><span class="sxs-lookup"><span data-stu-id="ba7b8-138">• Register a value added reseller</span></span>|
|<span data-ttu-id="ba7b8-139">Agente de vendas</span><span class="sxs-lookup"><span data-stu-id="ba7b8-139">Sales agent</span></span> | <span data-ttu-id="ba7b8-140">• Gerenciamento de cliente</span><span class="sxs-lookup"><span data-stu-id="ba7b8-140">•    Customer management</span></span>
||<span data-ttu-id="ba7b8-141">• Adicionar lista de dispositivos para o Centro de parceiros</span><span class="sxs-lookup"><span data-stu-id="ba7b8-141">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="ba7b8-142">• Gerenciamento de assinatura</span><span class="sxs-lookup"><span data-stu-id="ba7b8-142">• Subscription management</span></span>
||<span data-ttu-id="ba7b8-143">• Tíquetes de suporte de modo de exibição</span><span class="sxs-lookup"><span data-stu-id="ba7b8-143">• View support tickets</span></span>
||<span data-ttu-id="ba7b8-144">• Solicitação uma relação com um cliente</span><span class="sxs-lookup"><span data-stu-id="ba7b8-144">• Request a relationship with a customer</span></span>
||<span data-ttu-id="ba7b8-145">• Gerenciar clientes potenciais</span><span class="sxs-lookup"><span data-stu-id="ba7b8-145">• Manage customer leads</span></span>
||<span data-ttu-id="ba7b8-146">• Exibir o contrato do cliente</span><span class="sxs-lookup"><span data-stu-id="ba7b8-146">• View the customer agreement</span></span>
||<span data-ttu-id="ba7b8-147">• Registre-se um revendedor de valor agregado</span><span class="sxs-lookup"><span data-stu-id="ba7b8-147">• Register a value-added reseller</span></span>|
|<span data-ttu-id="ba7b8-148">Agente de suporte técnico</span><span class="sxs-lookup"><span data-stu-id="ba7b8-148">Helpdesk agent</span></span>| <span data-ttu-id="ba7b8-149">• Pesquisar e exibir um cliente</span><span class="sxs-lookup"><span data-stu-id="ba7b8-149">•  Search for and view a customer</span></span>
||<span data-ttu-id="ba7b8-150">• Editar detalhes do cliente</span><span class="sxs-lookup"><span data-stu-id="ba7b8-150">• Edit customer details</span></span>
||<span data-ttu-id="ba7b8-151">• Ajuda resolver problemas de cliente com o gerenciamento de cobrança ou assinatura</span><span class="sxs-lookup"><span data-stu-id="ba7b8-151">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="ba7b8-152">• Suporte a solicitação em nome dos clientes (Observação: Você deve ser um agente de administrador para concluir essa tarefa para assinaturas do Office 365)</span><span class="sxs-lookup"><span data-stu-id="ba7b8-152">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="ba7b8-153">• Gerenciar assinaturas e cobrança problemas em nome dos clientes (Observação: Você deve ser um agente de administrador para concluir essa tarefa para assinaturas do Office 365)</span><span class="sxs-lookup"><span data-stu-id="ba7b8-153">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|
|
### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="ba7b8-154">Fornecedor do painel de controle (CPV).</span><span class="sxs-lookup"><span data-stu-id="ba7b8-154">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="ba7b8-155">(Função do CSP e função de não-AAD)</span><span class="sxs-lookup"><span data-stu-id="ba7b8-155">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="ba7b8-156">CPVs desenvolver aplicativos para uso pelos parceiros de provedor de solução de nuvem (CSP) para que eles possam integrar seus sistemas com APIs do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="ba7b8-156">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="ba7b8-157">**Função**</span><span class="sxs-lookup"><span data-stu-id="ba7b8-157">**Role**</span></span>   |<span data-ttu-id="ba7b8-158">**O que você pode fazer**</span><span class="sxs-lookup"><span data-stu-id="ba7b8-158">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="ba7b8-159">Administração global</span><span class="sxs-lookup"><span data-stu-id="ba7b8-159">Global admin</span></span>| <span data-ttu-id="ba7b8-160">Exibir e gerenciar seu perfil CPV</span><span class="sxs-lookup"><span data-stu-id="ba7b8-160">View and manage your CPV profile</span></span>|
||<span data-ttu-id="ba7b8-161">Exibir e gerenciar qualquer um dos seus usuários que precisam de acesso aos recursos de CPV</span><span class="sxs-lookup"><span data-stu-id="ba7b8-161">View and manage any of your users who need access to CPV capabilities</span></span>|

## <a name="manage-mpn-membership-and-your-company-non-aad-roles"></a><span data-ttu-id="ba7b8-162">Gerenciar a associação da MPN e sua empresa (funções de não-AAD)</span><span class="sxs-lookup"><span data-stu-id="ba7b8-162">Manage MPN membership and your company (non-AAD roles)</span></span>

|<span data-ttu-id="ba7b8-163">**Função**</span><span class="sxs-lookup"><span data-stu-id="ba7b8-163">**Role**</span></span> | <span data-ttu-id="ba7b8-164">**O que você pode fazer**</span><span class="sxs-lookup"><span data-stu-id="ba7b8-164">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="ba7b8-165">Administrador de parceiros do MPN</span><span class="sxs-lookup"><span data-stu-id="ba7b8-165">MPN partner admin</span></span>|<span data-ttu-id="ba7b8-166">•CAN adicionar usuários de locatário não</span><span class="sxs-lookup"><span data-stu-id="ba7b8-166">•Can add non-tenant users</span></span>
||<span data-ttu-id="ba7b8-167">• Exibir, criar e gerenciar solicitações de serviço do parceiro</span><span class="sxs-lookup"><span data-stu-id="ba7b8-167">• View, create, and manage partner service requests</span></span>
||<span data-ttu-id="ba7b8-168">• Exibir legal, organização, negócios e perfis do MPN</span><span class="sxs-lookup"><span data-stu-id="ba7b8-168">• View legal, organization, business, and MPN profiles</span></span>
||<span data-ttu-id="ba7b8-169">• Exibir detalhes do usuário e seus dados de habilidades</span><span class="sxs-lookup"><span data-stu-id="ba7b8-169">• View user details and their skills data</span></span>
||<span data-ttu-id="ba7b8-170">• Exibir competências</span><span class="sxs-lookup"><span data-stu-id="ba7b8-170">• View competencies</span></span>
||<span data-ttu-id="ba7b8-171">• Exibir e gerenciar os benefícios</span><span class="sxs-lookup"><span data-stu-id="ba7b8-171">• View and manage benefits</span></span>
||<span data-ttu-id="ba7b8-172">Compra e o modo de exibição • o MPN oferece</span><span class="sxs-lookup"><span data-stu-id="ba7b8-172">• View and purchase MPN offers</span></span>
||<span data-ttu-id="ba7b8-173">• Exibir MPN oferece notas fiscais e histórico de pedidos</span><span class="sxs-lookup"><span data-stu-id="ba7b8-173">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="ba7b8-174">• Exibir dados de contribuição de parceiro</span><span class="sxs-lookup"><span data-stu-id="ba7b8-174">• View partner contribution data</span></span>
||<span data-ttu-id="ba7b8-175">• Podem trabalhar na ferramenta de validação de comprovante</span><span class="sxs-lookup"><span data-stu-id="ba7b8-175">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="ba7b8-176">-Exibir a análise de dados do cliente</span><span class="sxs-lookup"><span data-stu-id="ba7b8-176">- View customer data analytics</span></span>
|<span data-ttu-id="ba7b8-177">Administrador da conta</span><span class="sxs-lookup"><span data-stu-id="ba7b8-177">Account admin</span></span>| <span data-ttu-id="ba7b8-178">• Pode adicionar usuários de locatário não</span><span class="sxs-lookup"><span data-stu-id="ba7b8-178">•   Can add non-tenant users</span></span>
||<span data-ttu-id="ba7b8-179">• Adicionar ou excluir locais</span><span class="sxs-lookup"><span data-stu-id="ba7b8-179">• Add or delete locations</span></span>
||<span data-ttu-id="ba7b8-180">-Gerenciar perfis relacionados às contas que você é administrador</span><span class="sxs-lookup"><span data-stu-id="ba7b8-180">- Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="ba7b8-181">• Atribuir funções para usuários no locatário para funções do AAD não</span><span class="sxs-lookup"><span data-stu-id="ba7b8-181">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="ba7b8-182">• Registrar locais em programas</span><span class="sxs-lookup"><span data-stu-id="ba7b8-182">• Enroll locations into programs</span></span>

## <a name="manage-referrals-non-aad-roles"></a><span data-ttu-id="ba7b8-183">Gerenciar as referências (funções de não-AAD)</span><span class="sxs-lookup"><span data-stu-id="ba7b8-183">Manage referrals (non-AAD roles)</span></span>

|<span data-ttu-id="ba7b8-184">**Função**</span><span class="sxs-lookup"><span data-stu-id="ba7b8-184">**Role**</span></span>|<span data-ttu-id="ba7b8-185">**O que você pode fazer**</span><span class="sxs-lookup"><span data-stu-id="ba7b8-185">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="ba7b8-186">Administrador de referências</span><span class="sxs-lookup"><span data-stu-id="ba7b8-186">Referrals admin</span></span>       |<span data-ttu-id="ba7b8-187">• Exibir, criar e gerenciar perfis de negócios</span><span class="sxs-lookup"><span data-stu-id="ba7b8-187">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="ba7b8-188">• Receber e gerenciar as referências</span><span class="sxs-lookup"><span data-stu-id="ba7b8-188">• Receive and manage referrals</span></span>
||<span data-ttu-id="ba7b8-189">• Exibir, criar e gerenciar solicitações de serviço do parceiro</span><span class="sxs-lookup"><span data-stu-id="ba7b8-189">• View, create, and manage partner service requests</span></span>|
|<span data-ttu-id="ba7b8-190">Administrador de perfis de negócios</span><span class="sxs-lookup"><span data-stu-id="ba7b8-190">Business profile admin</span></span>   |<span data-ttu-id="ba7b8-191">•View, criar e gerenciar um perfil comercial</span><span class="sxs-lookup"><span data-stu-id="ba7b8-191">•View, create, and manage business profile</span></span> 
||<span data-ttu-id="ba7b8-192">• Exibir, criar e gerenciar solicitações de serviço do parceiro</span><span class="sxs-lookup"><span data-stu-id="ba7b8-192">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives--non-aad-roles"></a><span data-ttu-id="ba7b8-193">Gerenciar incentivos (funções de não-AAD)</span><span class="sxs-lookup"><span data-stu-id="ba7b8-193">Manage Incentives  (non-AAD roles)</span></span>

|<span data-ttu-id="ba7b8-194">**Função**</span><span class="sxs-lookup"><span data-stu-id="ba7b8-194">**Role**</span></span> | <span data-ttu-id="ba7b8-195">**O que você pode fazer**</span><span class="sxs-lookup"><span data-stu-id="ba7b8-195">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="ba7b8-196">Administrador de incentivos</span><span class="sxs-lookup"><span data-stu-id="ba7b8-196">Incentives admin</span></span>|<span data-ttu-id="ba7b8-197">• Inicia e gerencia incentivos</span><span class="sxs-lookup"><span data-stu-id="ba7b8-197">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="ba7b8-198">• Pode exibir e editar todos os aspectos de programas de incentivos</span><span class="sxs-lookup"><span data-stu-id="ba7b8-198">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="ba7b8-199">• Pode exibir e editar os detalhes do banco e imposto</span><span class="sxs-lookup"><span data-stu-id="ba7b8-199">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="ba7b8-200">• Ganhos de reembolso e cooperação do modo de exibição</span><span class="sxs-lookup"><span data-stu-id="ba7b8-200">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="ba7b8-201">• Suporte a acesso</span><span class="sxs-lookup"><span data-stu-id="ba7b8-201">• Access support</span></span>
||<span data-ttu-id="ba7b8-202">• Os pagamentos incentivos de controvérsias</span><span class="sxs-lookup"><span data-stu-id="ba7b8-202">• Dispute incentives payments</span></span>|
|<span data-ttu-id="ba7b8-203">Usuário de incentivos</span><span class="sxs-lookup"><span data-stu-id="ba7b8-203">Incentives user</span></span>|<span data-ttu-id="ba7b8-204">• Podem exibir programas incentivos</span><span class="sxs-lookup"><span data-stu-id="ba7b8-204">•  Can view incentives programs</span></span>
||<span data-ttu-id="ba7b8-205">• Pode exibir e iniciar as declarações de incentivos</span><span class="sxs-lookup"><span data-stu-id="ba7b8-205">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="ba7b8-206">• Ganhos de reembolso e cooperação do modo de exibição</span><span class="sxs-lookup"><span data-stu-id="ba7b8-206">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="ba7b8-207">• Ganhos de reembolso e cooperação do modo de exibição</span><span class="sxs-lookup"><span data-stu-id="ba7b8-207">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="ba7b8-208">• Suporte a acesso</span><span class="sxs-lookup"><span data-stu-id="ba7b8-208">• Access support</span></span>












