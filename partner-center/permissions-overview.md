---
title: Atribuir funções de usuários e permissões | Partner Center
ms.topic: article
ms.date: 10/29/2018
description: Todos os funcionários que precisam trabalhar no Partner Center devem ser atribuído a uma função.
author: labrenne
ms.author: labrenne
keywords: funções, permissões, administrador, agente
ms.localizationpriority: medium
ms.openlocfilehash: cc0e37601b16033bf31faaf5056ca0389d6f5cf6
ms.sourcegitcommit: 7961476a8fed7cd56a09c6edc8dd1e2dd7f46465
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/27/2019
ms.locfileid: "9117209"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="ae143-104">Atribuir funções e permissões de usuário</span><span class="sxs-lookup"><span data-stu-id="ae143-104">Assign users roles and permissions</span></span>


<span data-ttu-id="ae143-105">Você configurou seu perfil de parceiro, incluindo o nome legal e endereço, detalhes de suporte, isenções de impostos, informações bancárias e o contato principal para sua empresa.</span><span class="sxs-lookup"><span data-stu-id="ae143-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="ae143-106">Próxima etapa: obter os usuários configurado com senhas e funções, portanto, eles podem começar a trabalhar no Partner Center com você.</span><span class="sxs-lookup"><span data-stu-id="ae143-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="ae143-107">Configurar seus funcionários para trabalhar no Partner Center</span><span class="sxs-lookup"><span data-stu-id="ae143-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="ae143-108">Determinar os tipos de acesso que os usuários tenham Partner Center, as funções e permissões que dar a eles.</span><span class="sxs-lookup"><span data-stu-id="ae143-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="ae143-109">Funções estão relacionadas à programas em que sua empresa está envolvida em.</span><span class="sxs-lookup"><span data-stu-id="ae143-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="ae143-110">Por exemplo, se sua empresa é uma empresa de provedor de soluções na nuvem (CSP), você não terá apenas o Azure AD padrão funções de gerenciamento, como o administrador global do locatário, mas será necessário funções específicas ao programa CSP.</span><span class="sxs-lookup"><span data-stu-id="ae143-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="ae143-111">Cada programa tem funções específicas a ela.</span><span class="sxs-lookup"><span data-stu-id="ae143-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="ae143-112">Funções de locatário do Azure Active Directory (AAD) incluem o administrador global, administrador de usuários e funções do CSP.</span><span class="sxs-lookup"><span data-stu-id="ae143-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="ae143-113">Funções do AAD não incluem administrador MPN, administrador de perfil de negócios, administrador de indicações, administrador de incentivos e usuário de incentivos.</span><span class="sxs-lookup"><span data-stu-id="ae143-113">Non-AAD roles include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="ae143-114">Gerenciar transações comerciais no Partner Center (Azure AD e funções do CSP)</span><span class="sxs-lookup"><span data-stu-id="ae143-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|**<span data-ttu-id="ae143-115">Função</span><span class="sxs-lookup"><span data-stu-id="ae143-115">Role</span></span>**|**<span data-ttu-id="ae143-116">O que eles podem fazer</span><span class="sxs-lookup"><span data-stu-id="ae143-116">What they can do</span></span>**|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="ae143-117">Administração global</span><span class="sxs-lookup"><span data-stu-id="ae143-117">Global admin</span></span>|<span data-ttu-id="ae143-118">• Pode acessar todas as contas/serviços da Microsoft com todos os privilégios</span><span class="sxs-lookup"><span data-stu-id="ae143-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="ae143-119">• Criar tíquetes de suporte para o Partner Center</span><span class="sxs-lookup"><span data-stu-id="ae143-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="ae143-120">• Exibir contratos, listas de preços e ofertas</span><span class="sxs-lookup"><span data-stu-id="ae143-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="ae143-121">• Exibir, criar e gerenciar usuários de parceiros</span><span class="sxs-lookup"><span data-stu-id="ae143-121">• View, create, and manage partner users</span></span>|
|<span data-ttu-id="ae143-122">Administrador de usuários</span><span class="sxs-lookup"><span data-stu-id="ae143-122">User Admin</span></span>   | <span data-ttu-id="ae143-123">• Exibir, criar e gerenciar usuários</span><span class="sxs-lookup"><span data-stu-id="ae143-123">•   View, create, and manage users</span></span>
||<span data-ttu-id="ae143-124">• Exibir todos os perfis de parceiros</span><span class="sxs-lookup"><span data-stu-id="ae143-124">• View all partner profiles</span></span>
||<span data-ttu-id="ae143-125">• Exibir, criar e gerenciar usuários de parceiros</span><span class="sxs-lookup"><span data-stu-id="ae143-125">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="ae143-126">Usuário padrão</span><span class="sxs-lookup"><span data-stu-id="ae143-126">Default user</span></span>|  <span data-ttu-id="ae143-127">Exibir meu perfil</span><span class="sxs-lookup"><span data-stu-id="ae143-127">View My profile</span></span>   |
|<span data-ttu-id="ae143-128">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="ae143-128">Admin agent</span></span> | <span data-ttu-id="ae143-129">• Gerenciamento de cliente</span><span class="sxs-lookup"><span data-stu-id="ae143-129">•    Customer management</span></span>
||<span data-ttu-id="ae143-130">• Adicionar lista de dispositivos para o Center< de parceiro</span><span class="sxs-lookup"><span data-stu-id="ae143-130">• Add device list to the Partner Center<</span></span>
||<span data-ttu-id="ae143-131">• Criar e aplicar perfis aos dispositivos</span><span class="sxs-lookup"><span data-stu-id="ae143-131">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="ae143-132">• Gerenciamento de assinaturas</span><span class="sxs-lookup"><span data-stu-id="ae143-132">• Subscription management</span></span>
||<span data-ttu-id="ae143-133">• Serviço solicitações de integridade e para clientes</span><span class="sxs-lookup"><span data-stu-id="ae143-133">• Service health and service requests for customers</span></span>
||<span data-ttu-id="ae143-134">• Solicitar privilégios de administrador</span><span class="sxs-lookup"><span data-stu-id="ae143-134">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="ae143-135">• Exibir preços e ofertas</span><span class="sxs-lookup"><span data-stu-id="ae143-135">• View pricing and offers</span></span>
||<span data-ttu-id="ae143-136">• A cobrança</span><span class="sxs-lookup"><span data-stu-id="ae143-136">• Billing</span></span>
||<span data-ttu-id="ae143-137">• Administrar em nome do cliente</span><span class="sxs-lookup"><span data-stu-id="ae143-137">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="ae143-138">• Registrar um valor bom revendedor</span><span class="sxs-lookup"><span data-stu-id="ae143-138">• Register a value added reseller</span></span>|
|<span data-ttu-id="ae143-139">Agente de vendas</span><span class="sxs-lookup"><span data-stu-id="ae143-139">Sales agent</span></span> | <span data-ttu-id="ae143-140">• Gerenciamento de cliente</span><span class="sxs-lookup"><span data-stu-id="ae143-140">•    Customer management</span></span>
||<span data-ttu-id="ae143-141">• Adicionar lista de dispositivos ao Partner Center</span><span class="sxs-lookup"><span data-stu-id="ae143-141">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="ae143-142">• Gerenciamento de assinaturas</span><span class="sxs-lookup"><span data-stu-id="ae143-142">• Subscription management</span></span>
||<span data-ttu-id="ae143-143">• Exibir tíquetes de suporte</span><span class="sxs-lookup"><span data-stu-id="ae143-143">• View support tickets</span></span>
||<span data-ttu-id="ae143-144">• Solicitar um relacionamento com um cliente</span><span class="sxs-lookup"><span data-stu-id="ae143-144">• Request a relationship with a customer</span></span>
||<span data-ttu-id="ae143-145">• Gerenciar as oportunidades de cliente</span><span class="sxs-lookup"><span data-stu-id="ae143-145">• Manage customer leads</span></span>
||<span data-ttu-id="ae143-146">• Exibir o contrato do cliente</span><span class="sxs-lookup"><span data-stu-id="ae143-146">• View the customer agreement</span></span>
||<span data-ttu-id="ae143-147">• Registrar um revendedor</span><span class="sxs-lookup"><span data-stu-id="ae143-147">• Register a value-added reseller</span></span>|
|<span data-ttu-id="ae143-148">Agente de suporte técnico</span><span class="sxs-lookup"><span data-stu-id="ae143-148">Helpdesk agent</span></span>| <span data-ttu-id="ae143-149">• Pesquisar e exibir um cliente</span><span class="sxs-lookup"><span data-stu-id="ae143-149">•  Search for and view a customer</span></span>
||<span data-ttu-id="ae143-150">• Editar detalhes do cliente</span><span class="sxs-lookup"><span data-stu-id="ae143-150">• Edit customer details</span></span>
||<span data-ttu-id="ae143-151">• Ajudam a resolver problemas do cliente com o gerenciamento de cobrança ou assinatura</span><span class="sxs-lookup"><span data-stu-id="ae143-151">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="ae143-152">• Solicitação de suporte em nome dos clientes (Observação: você deve ser um agente administrador para concluir essa tarefa para assinaturas do Office 365)</span><span class="sxs-lookup"><span data-stu-id="ae143-152">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="ae143-153">• Gerenciar assinaturas e serviços em nome dos clientes (Observação: você deve ser um agente administrador para concluir essa tarefa para assinaturas do Office 365)</span><span class="sxs-lookup"><span data-stu-id="ae143-153">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|
|
### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="ae143-154">Fornecedor do painel de controle (CPV).</span><span class="sxs-lookup"><span data-stu-id="ae143-154">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="ae143-155">(Funções de CSP e não AAD)</span><span class="sxs-lookup"><span data-stu-id="ae143-155">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="ae143-156">CPVs desenvolver aplicativos para uso por parceiros de provedor de soluções na nuvem (CSP) para habilitá-los integrar seus sistemas com APIs do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="ae143-156">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|**<span data-ttu-id="ae143-157">Função</span><span class="sxs-lookup"><span data-stu-id="ae143-157">Role</span></span>**   |**<span data-ttu-id="ae143-158">Você pode fazer</span><span class="sxs-lookup"><span data-stu-id="ae143-158">What you can do</span></span>**|
|------------------------------|:----------------------------|
|<span data-ttu-id="ae143-159">Administração global</span><span class="sxs-lookup"><span data-stu-id="ae143-159">Global admin</span></span>| <span data-ttu-id="ae143-160">Exibir e gerenciar seu perfil CPV</span><span class="sxs-lookup"><span data-stu-id="ae143-160">View and manage your CPV profile</span></span>|
||<span data-ttu-id="ae143-161">Exibir e gerenciar qualquer um dos seus usuários que precisam de acesso a recursos CPV</span><span class="sxs-lookup"><span data-stu-id="ae143-161">View and manage any of your users who need access to CPV capabilities</span></span>|

## <a name="manage-mpn-membership-and-your-company-non-aad-roles"></a><span data-ttu-id="ae143-162">Gerenciar a associação à MPN e a sua empresa (funções não AAD)</span><span class="sxs-lookup"><span data-stu-id="ae143-162">Manage MPN membership and your company (non-AAD roles)</span></span>

|**<span data-ttu-id="ae143-163">Função</span><span class="sxs-lookup"><span data-stu-id="ae143-163">Role</span></span>** | **<span data-ttu-id="ae143-164">Você pode fazer</span><span class="sxs-lookup"><span data-stu-id="ae143-164">What you can do</span></span>**|
|----------------------------|:----------------------------|
|<span data-ttu-id="ae143-165">Administrador de parceiros do MPN</span><span class="sxs-lookup"><span data-stu-id="ae143-165">MPN partner admin</span></span>|<span data-ttu-id="ae143-166">•CAN adicionar usuários não locatário</span><span class="sxs-lookup"><span data-stu-id="ae143-166">•Can add non-tenant users</span></span>
||<span data-ttu-id="ae143-167">• Exibir, criar e gerenciar solicitações de serviço do parceiro</span><span class="sxs-lookup"><span data-stu-id="ae143-167">• View, create, and manage partner service requests</span></span>
||<span data-ttu-id="ae143-168">• Exibição legal, organização, empresas e perfis do MPN</span><span class="sxs-lookup"><span data-stu-id="ae143-168">• View legal, organization, business, and MPN profiles</span></span>
||<span data-ttu-id="ae143-169">• Exibir detalhes do usuário e seus dados de habilidades</span><span class="sxs-lookup"><span data-stu-id="ae143-169">• View user details and their skills data</span></span>
||<span data-ttu-id="ae143-170">• Exibir competências</span><span class="sxs-lookup"><span data-stu-id="ae143-170">• View competencies</span></span>
||<span data-ttu-id="ae143-171">• Exibir e gerenciar benefícios</span><span class="sxs-lookup"><span data-stu-id="ae143-171">• View and manage benefits</span></span>
||<span data-ttu-id="ae143-172">• Exibição e compra de ofertas do MPN</span><span class="sxs-lookup"><span data-stu-id="ae143-172">• View and purchase MPN offers</span></span>
||<span data-ttu-id="ae143-173">• Exibição MPN histórico de pedidos e faturas de ofertas</span><span class="sxs-lookup"><span data-stu-id="ae143-173">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="ae143-174">• Exibir dados de contribuição de parceiros</span><span class="sxs-lookup"><span data-stu-id="ae143-174">• View partner contribution data</span></span>
||<span data-ttu-id="ae143-175">• Podem funcionar na ferramenta de validação de comprovantes</span><span class="sxs-lookup"><span data-stu-id="ae143-175">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="ae143-176">-Exibir a análise de dados do cliente</span><span class="sxs-lookup"><span data-stu-id="ae143-176">- View customer data analytics</span></span>
|<span data-ttu-id="ae143-177">Conta de administrador</span><span class="sxs-lookup"><span data-stu-id="ae143-177">Account admin</span></span>| <span data-ttu-id="ae143-178">• Pode adicionar usuários não locatário</span><span class="sxs-lookup"><span data-stu-id="ae143-178">•   Can add non-tenant users</span></span>
||<span data-ttu-id="ae143-179">• Adicionar ou excluir locais</span><span class="sxs-lookup"><span data-stu-id="ae143-179">• Add or delete locations</span></span>
||<span data-ttu-id="ae143-180">-Gerenciar perfis relacionados às contas de que administrador para você são</span><span class="sxs-lookup"><span data-stu-id="ae143-180">- Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="ae143-181">• Atribuir funções para os usuários de locatário às funções não AAD</span><span class="sxs-lookup"><span data-stu-id="ae143-181">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="ae143-182">• Se inscrever locais em programas</span><span class="sxs-lookup"><span data-stu-id="ae143-182">• Enroll locations into programs</span></span>

## <a name="manage-referrals-non-aad-roles"></a><span data-ttu-id="ae143-183">Gerenciar indicações (funções não AAD)</span><span class="sxs-lookup"><span data-stu-id="ae143-183">Manage referrals (non-AAD roles)</span></span>

|**<span data-ttu-id="ae143-184">Função</span><span class="sxs-lookup"><span data-stu-id="ae143-184">Role</span></span>**|**<span data-ttu-id="ae143-185">Você pode fazer</span><span class="sxs-lookup"><span data-stu-id="ae143-185">What you can do</span></span>**|
|-----------------------------|:------------------------|
|<span data-ttu-id="ae143-186">Administrador de indicações</span><span class="sxs-lookup"><span data-stu-id="ae143-186">Referrals admin</span></span>       |<span data-ttu-id="ae143-187">• Exibir, criar e gerenciar perfis de negócios</span><span class="sxs-lookup"><span data-stu-id="ae143-187">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="ae143-188">• Receber e gerenciar indicações</span><span class="sxs-lookup"><span data-stu-id="ae143-188">• Receive and manage referrals</span></span>
||<span data-ttu-id="ae143-189">• Exibir, criar e gerenciar solicitações de serviço do parceiro</span><span class="sxs-lookup"><span data-stu-id="ae143-189">• View, create, and manage partner service requests</span></span>|
|<span data-ttu-id="ae143-190">Administrador de perfis de negócios</span><span class="sxs-lookup"><span data-stu-id="ae143-190">Business profile admin</span></span>   |<span data-ttu-id="ae143-191">•View, criar e gerenciar perfil de negócios</span><span class="sxs-lookup"><span data-stu-id="ae143-191">•View, create, and manage business profile</span></span> 
||<span data-ttu-id="ae143-192">• Exibir, criar e gerenciar solicitações de serviço do parceiro</span><span class="sxs-lookup"><span data-stu-id="ae143-192">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives--non-aad-roles"></a><span data-ttu-id="ae143-193">Gerencie incentivos (funções não AAD)</span><span class="sxs-lookup"><span data-stu-id="ae143-193">Manage Incentives  (non-AAD roles)</span></span>

|**<span data-ttu-id="ae143-194">Função</span><span class="sxs-lookup"><span data-stu-id="ae143-194">Role</span></span>** | **<span data-ttu-id="ae143-195">Você pode fazer</span><span class="sxs-lookup"><span data-stu-id="ae143-195">What you can do</span></span>**|
|------------------------------|:-------------------------|
|<span data-ttu-id="ae143-196">Administrador de incentivos</span><span class="sxs-lookup"><span data-stu-id="ae143-196">Incentives admin</span></span>|<span data-ttu-id="ae143-197">• Inicia e gerencia incentivos</span><span class="sxs-lookup"><span data-stu-id="ae143-197">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="ae143-198">• Pode exibir e editar todos os aspectos de programas de incentivos</span><span class="sxs-lookup"><span data-stu-id="ae143-198">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="ae143-199">• Pode exibir e editar detalhes bancários e fiscais</span><span class="sxs-lookup"><span data-stu-id="ae143-199">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="ae143-200">• Lucros de reembolso e cooperação do modo de exibição</span><span class="sxs-lookup"><span data-stu-id="ae143-200">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="ae143-201">• Suporte de acesso</span><span class="sxs-lookup"><span data-stu-id="ae143-201">• Access support</span></span>
||<span data-ttu-id="ae143-202">Pagamentos de incentivos disputa •</span><span class="sxs-lookup"><span data-stu-id="ae143-202">• Dispute incentives payments</span></span>|
|<span data-ttu-id="ae143-203">Usuário de incentivos</span><span class="sxs-lookup"><span data-stu-id="ae143-203">Incentives user</span></span>|<span data-ttu-id="ae143-204">• Pode exibir programas de incentivos</span><span class="sxs-lookup"><span data-stu-id="ae143-204">•  Can view incentives programs</span></span>
||<span data-ttu-id="ae143-205">• Pode exibir e iniciar declarações de incentivos</span><span class="sxs-lookup"><span data-stu-id="ae143-205">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="ae143-206">• Lucros de reembolso e cooperação do modo de exibição</span><span class="sxs-lookup"><span data-stu-id="ae143-206">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="ae143-207">• Lucros de reembolso e cooperação do modo de exibição</span><span class="sxs-lookup"><span data-stu-id="ae143-207">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="ae143-208">• Suporte de acesso</span><span class="sxs-lookup"><span data-stu-id="ae143-208">• Access support</span></span>












