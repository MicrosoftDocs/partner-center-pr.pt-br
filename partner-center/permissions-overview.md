---
title: Atribuir funções e permissões de usuários | Partner Center
ms.topic: article
ms.date: 3/5/19
description: Todos os funcionários que precisam para trabalhar no Partner Center devem ser atribuído a uma função.
author: LauraBrenner
ms.author: labrenne
keywords: funções, permissões, administrador, agente
ms.localizationpriority: medium
ms.openlocfilehash: 66923c8a5d4912d178ef483a883f08f40ed8378b
ms.sourcegitcommit: 9a2bda49446030e60251c9c913259472ff2eed9a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2019
ms.locfileid: "57682484"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="fdcae-104">Atribuir funções e permissões de usuário</span><span class="sxs-lookup"><span data-stu-id="fdcae-104">Assign users roles and permissions</span></span>


<span data-ttu-id="fdcae-105">Você configurou o perfil de parceiro, incluindo nome legal e endereço, detalhes de suporte, isenções de imposto sobre arquivos, informações bancárias e o contato principal para a sua empresa.</span><span class="sxs-lookup"><span data-stu-id="fdcae-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="fdcae-106">Próxima etapa: configurar os usuários configurados com senhas e funções, para que eles possam começar a trabalhar no Partner Center com você.</span><span class="sxs-lookup"><span data-stu-id="fdcae-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="fdcae-107">Configurar seus funcionários para trabalhar no Partner Center</span><span class="sxs-lookup"><span data-stu-id="fdcae-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="fdcae-108">Os tipos de acesso que os usuários têm Partner Center, as funções e permissões que você conceda a você determinar.</span><span class="sxs-lookup"><span data-stu-id="fdcae-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="fdcae-109">As funções estão relacionadas aos programas de que sua empresa está envolvida no.</span><span class="sxs-lookup"><span data-stu-id="fdcae-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="fdcae-110">Por exemplo, se sua empresa é uma empresa de provedor de solução de nuvem (CSP), você não somente terá o Azure AD padrão funções de gerenciamento como administrador global do locatário, mas será necessário a funções específicas para o programa CSP.</span><span class="sxs-lookup"><span data-stu-id="fdcae-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="fdcae-111">Cada programa tem funções específicas a ela.</span><span class="sxs-lookup"><span data-stu-id="fdcae-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="fdcae-112">As funções de locatário do Azure Active Directory (AAD) incluem administrador global, administrador de usuários e funções CSP.</span><span class="sxs-lookup"><span data-stu-id="fdcae-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="fdcae-113">Funções do AAD não incluem MPN admin, administrador de perfil de negócios, administração de indicação, incentivo administrador e usuário incentivo.</span><span class="sxs-lookup"><span data-stu-id="fdcae-113">Non-AAD roles include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="fdcae-114">Gerenciar transações comerciais no Partner Center (Azure AD e as funções do CSP)</span><span class="sxs-lookup"><span data-stu-id="fdcae-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="fdcae-115">**Função**</span><span class="sxs-lookup"><span data-stu-id="fdcae-115">**Role**</span></span>|<span data-ttu-id="fdcae-116">**O que pode fazer**</span><span class="sxs-lookup"><span data-stu-id="fdcae-116">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="fdcae-117">Administração global</span><span class="sxs-lookup"><span data-stu-id="fdcae-117">Global admin</span></span>|<span data-ttu-id="fdcae-118">• Podem acessar todos os Microsoft/serviços de conta com privilégios totais</span><span class="sxs-lookup"><span data-stu-id="fdcae-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="fdcae-119">• Criar tíquetes de suporte para o Centro de parceiros</span><span class="sxs-lookup"><span data-stu-id="fdcae-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="fdcae-120">• Exibir contratos, listas de preços e ofertas</span><span class="sxs-lookup"><span data-stu-id="fdcae-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="fdcae-121">• Exibir, criar e gerenciar os usuários do parceiro</span><span class="sxs-lookup"><span data-stu-id="fdcae-121">• View, create, and manage partner users</span></span>|
|<span data-ttu-id="fdcae-122">Usuário administrador</span><span class="sxs-lookup"><span data-stu-id="fdcae-122">User Admin</span></span>   | <span data-ttu-id="fdcae-123">• Exibir, criar e gerenciar usuários</span><span class="sxs-lookup"><span data-stu-id="fdcae-123">•   View, create, and manage users</span></span>
||<span data-ttu-id="fdcae-124">• Exibir todos os perfis de parceiros</span><span class="sxs-lookup"><span data-stu-id="fdcae-124">• View all partner profiles</span></span>
||<span data-ttu-id="fdcae-125">• Exibir, criar e gerenciar os usuários do parceiro</span><span class="sxs-lookup"><span data-stu-id="fdcae-125">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="fdcae-126">Administrador de cobrança</span><span class="sxs-lookup"><span data-stu-id="fdcae-126">Billing admin</span></span> | <span data-ttu-id="fdcae-127">-Exibir, criar e gerenciar arquivos recon, faturas e cobrança</span><span class="sxs-lookup"><span data-stu-id="fdcae-127">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="fdcae-128">Usuário padrão</span><span class="sxs-lookup"><span data-stu-id="fdcae-128">Default user</span></span>|  <span data-ttu-id="fdcae-129">Exibir meu perfil</span><span class="sxs-lookup"><span data-stu-id="fdcae-129">View My profile</span></span>   |
|<span data-ttu-id="fdcae-130">Agente administrador</span><span class="sxs-lookup"><span data-stu-id="fdcae-130">Admin agent</span></span> | <span data-ttu-id="fdcae-131">• Gerenciamento de cliente</span><span class="sxs-lookup"><span data-stu-id="fdcae-131">•    Customer management</span></span>
||<span data-ttu-id="fdcae-132">• Adicionar lista de dispositivos para o Centro de parceiros <</span><span class="sxs-lookup"><span data-stu-id="fdcae-132">• Add device list to the Partner Center<</span></span>
||<span data-ttu-id="fdcae-133">• Criar e aplicar perfis de dispositivos</span><span class="sxs-lookup"><span data-stu-id="fdcae-133">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="fdcae-134">• Gerenciamento de assinatura</span><span class="sxs-lookup"><span data-stu-id="fdcae-134">• Subscription management</span></span>
||<span data-ttu-id="fdcae-135">• Integridade e o serviço de solicitações de clientes</span><span class="sxs-lookup"><span data-stu-id="fdcae-135">• Service health and service requests for customers</span></span>
||<span data-ttu-id="fdcae-136">• Solicitação delegada privilégios de administrador</span><span class="sxs-lookup"><span data-stu-id="fdcae-136">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="fdcae-137">• Exibir preço e ofertas</span><span class="sxs-lookup"><span data-stu-id="fdcae-137">• View pricing and offers</span></span>
||<span data-ttu-id="fdcae-138">• Cobrança</span><span class="sxs-lookup"><span data-stu-id="fdcae-138">• Billing</span></span>
||<span data-ttu-id="fdcae-139">• Administrar em nome de um cliente</span><span class="sxs-lookup"><span data-stu-id="fdcae-139">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="fdcae-140">• Registre-se um valor adicionado revendedor</span><span class="sxs-lookup"><span data-stu-id="fdcae-140">• Register a value added reseller</span></span>|
|<span data-ttu-id="fdcae-141">Agente de vendas</span><span class="sxs-lookup"><span data-stu-id="fdcae-141">Sales agent</span></span> | <span data-ttu-id="fdcae-142">• Gerenciamento de cliente</span><span class="sxs-lookup"><span data-stu-id="fdcae-142">•    Customer management</span></span>
||<span data-ttu-id="fdcae-143">• Adicionar lista de dispositivos para o Centro de parceiros</span><span class="sxs-lookup"><span data-stu-id="fdcae-143">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="fdcae-144">• Gerenciamento de assinatura</span><span class="sxs-lookup"><span data-stu-id="fdcae-144">• Subscription management</span></span>
||<span data-ttu-id="fdcae-145">• Tíquetes de suporte de modo de exibição</span><span class="sxs-lookup"><span data-stu-id="fdcae-145">• View support tickets</span></span>
||<span data-ttu-id="fdcae-146">• Solicitação uma relação com um cliente</span><span class="sxs-lookup"><span data-stu-id="fdcae-146">• Request a relationship with a customer</span></span>
||<span data-ttu-id="fdcae-147">• Gerenciar clientes potenciais</span><span class="sxs-lookup"><span data-stu-id="fdcae-147">• Manage customer leads</span></span>
||<span data-ttu-id="fdcae-148">• Exibir o contrato do cliente</span><span class="sxs-lookup"><span data-stu-id="fdcae-148">• View the customer agreement</span></span>
||<span data-ttu-id="fdcae-149">• Registre-se um revendedor de valor agregado</span><span class="sxs-lookup"><span data-stu-id="fdcae-149">• Register a value-added reseller</span></span>|
|<span data-ttu-id="fdcae-150">Agente de suporte técnico</span><span class="sxs-lookup"><span data-stu-id="fdcae-150">Helpdesk agent</span></span>| <span data-ttu-id="fdcae-151">• Pesquisar e exibir um cliente</span><span class="sxs-lookup"><span data-stu-id="fdcae-151">•  Search for and view a customer</span></span>
||<span data-ttu-id="fdcae-152">• Editar detalhes do cliente</span><span class="sxs-lookup"><span data-stu-id="fdcae-152">• Edit customer details</span></span>
||<span data-ttu-id="fdcae-153">• Ajuda resolver problemas de cliente com o gerenciamento de cobrança ou assinatura</span><span class="sxs-lookup"><span data-stu-id="fdcae-153">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="fdcae-154">• Suporte a solicitação em nome dos clientes (Observação: Você deve ser um agente de administrador para concluir essa tarefa para assinaturas do Office 365)</span><span class="sxs-lookup"><span data-stu-id="fdcae-154">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="fdcae-155">• Gerenciar assinaturas e cobrança problemas em nome dos clientes (Observação: Você deve ser um agente de administrador para concluir essa tarefa para assinaturas do Office 365)</span><span class="sxs-lookup"><span data-stu-id="fdcae-155">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="fdcae-156">Fornecedor do painel de controle (CPV).</span><span class="sxs-lookup"><span data-stu-id="fdcae-156">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="fdcae-157">(Função do CSP e função de não-AAD)</span><span class="sxs-lookup"><span data-stu-id="fdcae-157">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="fdcae-158">CPVs desenvolver aplicativos para uso pelos parceiros de provedor de solução de nuvem (CSP) para que eles possam integrar seus sistemas com APIs do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="fdcae-158">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="fdcae-159">**Função**</span><span class="sxs-lookup"><span data-stu-id="fdcae-159">**Role**</span></span>   |<span data-ttu-id="fdcae-160">**O que você pode fazer**</span><span class="sxs-lookup"><span data-stu-id="fdcae-160">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="fdcae-161">Administração global</span><span class="sxs-lookup"><span data-stu-id="fdcae-161">Global admin</span></span>| <span data-ttu-id="fdcae-162">Exibir e gerenciar seu perfil CPV</span><span class="sxs-lookup"><span data-stu-id="fdcae-162">View and manage your CPV profile</span></span>|
||<span data-ttu-id="fdcae-163">Exibir e gerenciar qualquer um dos seus usuários que precisam de acesso aos recursos de CPV</span><span class="sxs-lookup"><span data-stu-id="fdcae-163">View and manage any of your users who need access to CPV capabilities</span></span>|

## <a name="manage-mpn-membership-and-your-company-non-aad-roles"></a><span data-ttu-id="fdcae-164">Gerenciar a associação da MPN e sua empresa (funções de não-AAD)</span><span class="sxs-lookup"><span data-stu-id="fdcae-164">Manage MPN membership and your company (non-AAD roles)</span></span>

|<span data-ttu-id="fdcae-165">**Função**</span><span class="sxs-lookup"><span data-stu-id="fdcae-165">**Role**</span></span> | <span data-ttu-id="fdcae-166">**O que você pode fazer**</span><span class="sxs-lookup"><span data-stu-id="fdcae-166">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="fdcae-167">Administrador de parceiros do MPN</span><span class="sxs-lookup"><span data-stu-id="fdcae-167">MPN partner admin</span></span>|<span data-ttu-id="fdcae-168">•CAN adicionar usuários de locatário não</span><span class="sxs-lookup"><span data-stu-id="fdcae-168">•Can add non-tenant users</span></span>
||<span data-ttu-id="fdcae-169">• Exibir, criar e gerenciar solicitações de serviço do parceiro</span><span class="sxs-lookup"><span data-stu-id="fdcae-169">• View, create, and manage partner service requests</span></span>
||<span data-ttu-id="fdcae-170">• Exibir legal, organização, negócios e perfis do MPN</span><span class="sxs-lookup"><span data-stu-id="fdcae-170">• View legal, organization, business, and MPN profiles</span></span>
||<span data-ttu-id="fdcae-171">• Exibir detalhes do usuário e seus dados de habilidades</span><span class="sxs-lookup"><span data-stu-id="fdcae-171">• View user details and their skills data</span></span>
||<span data-ttu-id="fdcae-172">• Exibir competências</span><span class="sxs-lookup"><span data-stu-id="fdcae-172">• View competencies</span></span>
||<span data-ttu-id="fdcae-173">• Exibir e gerenciar os benefícios</span><span class="sxs-lookup"><span data-stu-id="fdcae-173">• View and manage benefits</span></span>
||<span data-ttu-id="fdcae-174">Compra e o modo de exibição • o MPN oferece</span><span class="sxs-lookup"><span data-stu-id="fdcae-174">• View and purchase MPN offers</span></span>
||<span data-ttu-id="fdcae-175">• Exibir MPN oferece notas fiscais e histórico de pedidos</span><span class="sxs-lookup"><span data-stu-id="fdcae-175">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="fdcae-176">• Exibir dados de contribuição de parceiro</span><span class="sxs-lookup"><span data-stu-id="fdcae-176">• View partner contribution data</span></span>
||<span data-ttu-id="fdcae-177">• Podem trabalhar na ferramenta de validação de comprovante</span><span class="sxs-lookup"><span data-stu-id="fdcae-177">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="fdcae-178">-Exibir a análise de dados do cliente</span><span class="sxs-lookup"><span data-stu-id="fdcae-178">- View customer data analytics</span></span>
|<span data-ttu-id="fdcae-179">Administrador da conta</span><span class="sxs-lookup"><span data-stu-id="fdcae-179">Account admin</span></span>| <span data-ttu-id="fdcae-180">• Pode adicionar usuários de locatário não</span><span class="sxs-lookup"><span data-stu-id="fdcae-180">•   Can add non-tenant users</span></span>
||<span data-ttu-id="fdcae-181">• Adicionar ou excluir locais</span><span class="sxs-lookup"><span data-stu-id="fdcae-181">• Add or delete locations</span></span>
||<span data-ttu-id="fdcae-182">-Gerenciar perfis relacionados às contas que você é administrador</span><span class="sxs-lookup"><span data-stu-id="fdcae-182">- Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="fdcae-183">• Atribuir funções para usuários no locatário para funções do AAD não</span><span class="sxs-lookup"><span data-stu-id="fdcae-183">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="fdcae-184">• Registrar locais em programas</span><span class="sxs-lookup"><span data-stu-id="fdcae-184">• Enroll locations into programs</span></span>

## <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="fdcae-185">Usuário convidado (deve ser adicionado ao locatário do AAD)</span><span class="sxs-lookup"><span data-stu-id="fdcae-185">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="fdcae-186">**Usuário convidado**</span><span class="sxs-lookup"><span data-stu-id="fdcae-186">**Guest user**</span></span>   | <span data-ttu-id="fdcae-187">**Funções**</span><span class="sxs-lookup"><span data-stu-id="fdcae-187">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="fdcae-188">Administrador de parceiros do MPN</span><span class="sxs-lookup"><span data-stu-id="fdcae-188">MPN partner admin</span></span>|
||<span data-ttu-id="fdcae-189">Contas de administrador</span><span class="sxs-lookup"><span data-stu-id="fdcae-189">Accounts admin</span></span>|
||<span data-ttu-id="fdcae-190">Administrador de incentivos</span><span class="sxs-lookup"><span data-stu-id="fdcae-190">Incentives admin</span></span>|
||<span data-ttu-id="fdcae-191">Administrador de perfis de negócios</span><span class="sxs-lookup"><span data-stu-id="fdcae-191">Business profile admin</span></span>|
||<span data-ttu-id="fdcae-192">Administrador de referências</span><span class="sxs-lookup"><span data-stu-id="fdcae-192">Referrals admin</span></span>|


## <a name="manage-referrals-non-aad-roles"></a><span data-ttu-id="fdcae-193">Gerenciar as referências (funções de não-AAD)</span><span class="sxs-lookup"><span data-stu-id="fdcae-193">Manage referrals (non-AAD roles)</span></span>

|<span data-ttu-id="fdcae-194">**Função**</span><span class="sxs-lookup"><span data-stu-id="fdcae-194">**Role**</span></span>|<span data-ttu-id="fdcae-195">**O que você pode fazer**</span><span class="sxs-lookup"><span data-stu-id="fdcae-195">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="fdcae-196">Administrador de referências</span><span class="sxs-lookup"><span data-stu-id="fdcae-196">Referrals admin</span></span>       |<span data-ttu-id="fdcae-197">• Exibir, criar e gerenciar perfis de negócios</span><span class="sxs-lookup"><span data-stu-id="fdcae-197">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="fdcae-198">• Receber e gerenciar as referências</span><span class="sxs-lookup"><span data-stu-id="fdcae-198">• Receive and manage referrals</span></span>
||<span data-ttu-id="fdcae-199">• Exibir, criar e gerenciar solicitações de serviço do parceiro</span><span class="sxs-lookup"><span data-stu-id="fdcae-199">• View, create, and manage partner service requests</span></span>|
|<span data-ttu-id="fdcae-200">Administrador de perfis de negócios</span><span class="sxs-lookup"><span data-stu-id="fdcae-200">Business profile admin</span></span>   |<span data-ttu-id="fdcae-201">•View, criar e gerenciar um perfil comercial</span><span class="sxs-lookup"><span data-stu-id="fdcae-201">•View, create, and manage business profile</span></span> 
||<span data-ttu-id="fdcae-202">• Exibir, criar e gerenciar solicitações de serviço do parceiro</span><span class="sxs-lookup"><span data-stu-id="fdcae-202">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives--non-aad-roles"></a><span data-ttu-id="fdcae-203">Gerenciar incentivos (funções de não-AAD)</span><span class="sxs-lookup"><span data-stu-id="fdcae-203">Manage Incentives  (non-AAD roles)</span></span>

|<span data-ttu-id="fdcae-204">**Função**</span><span class="sxs-lookup"><span data-stu-id="fdcae-204">**Role**</span></span> | <span data-ttu-id="fdcae-205">**O que você pode fazer**</span><span class="sxs-lookup"><span data-stu-id="fdcae-205">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="fdcae-206">Administrador de incentivos</span><span class="sxs-lookup"><span data-stu-id="fdcae-206">Incentives admin</span></span>|<span data-ttu-id="fdcae-207">• Inicia e gerencia incentivos</span><span class="sxs-lookup"><span data-stu-id="fdcae-207">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="fdcae-208">• Pode exibir e editar todos os aspectos de programas de incentivos</span><span class="sxs-lookup"><span data-stu-id="fdcae-208">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="fdcae-209">• Pode exibir e editar os detalhes do banco e imposto</span><span class="sxs-lookup"><span data-stu-id="fdcae-209">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="fdcae-210">• Ganhos de reembolso e cooperação do modo de exibição</span><span class="sxs-lookup"><span data-stu-id="fdcae-210">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="fdcae-211">• Suporte a acesso</span><span class="sxs-lookup"><span data-stu-id="fdcae-211">• Access support</span></span>
||<span data-ttu-id="fdcae-212">• Os pagamentos incentivos de controvérsias</span><span class="sxs-lookup"><span data-stu-id="fdcae-212">• Dispute incentives payments</span></span>|
|<span data-ttu-id="fdcae-213">Usuário de incentivos</span><span class="sxs-lookup"><span data-stu-id="fdcae-213">Incentives user</span></span>|<span data-ttu-id="fdcae-214">• Podem exibir programas incentivos</span><span class="sxs-lookup"><span data-stu-id="fdcae-214">•  Can view incentives programs</span></span>
||<span data-ttu-id="fdcae-215">• Pode exibir e iniciar as declarações de incentivos</span><span class="sxs-lookup"><span data-stu-id="fdcae-215">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="fdcae-216">• Ganhos de reembolso e cooperação do modo de exibição</span><span class="sxs-lookup"><span data-stu-id="fdcae-216">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="fdcae-217">• Ganhos de reembolso e cooperação do modo de exibição</span><span class="sxs-lookup"><span data-stu-id="fdcae-217">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="fdcae-218">• Suporte a acesso</span><span class="sxs-lookup"><span data-stu-id="fdcae-218">• Access support</span></span>












