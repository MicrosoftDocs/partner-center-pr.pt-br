---
title: Atribuir funções e permissões de usuários | Partner Center
ms.topic: article
ms.date: 3/5/19
description: Todos os funcionários que precisam para trabalhar no Partner Center devem ser atribuído a uma função.
author: LauraBrenner
ms.author: labrenne
keywords: funções, permissões, administrador, agente
ms.localizationpriority: medium
ms.openlocfilehash: 65a2f7f373fc57f86cfffa73aafd3b7095fe2c04
ms.sourcegitcommit: be8086534ec73937f2be9bcc495c2627423c50f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2019
ms.locfileid: "67396735"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="4baf0-104">Atribuir funções e permissões de usuário</span><span class="sxs-lookup"><span data-stu-id="4baf0-104">Assign users roles and permissions</span></span>


<span data-ttu-id="4baf0-105">Você configurou o perfil de parceiro, incluindo nome legal e endereço, detalhes de suporte, isenções de imposto sobre arquivos, informações bancárias e o contato principal para a sua empresa.</span><span class="sxs-lookup"><span data-stu-id="4baf0-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="4baf0-106">Próxima etapa: configurar os usuários configurados com senhas e funções, para que eles possam começar a trabalhar no Partner Center com você.</span><span class="sxs-lookup"><span data-stu-id="4baf0-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="4baf0-107">Configurar seus funcionários para trabalhar no Partner Center</span><span class="sxs-lookup"><span data-stu-id="4baf0-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="4baf0-108">Os tipos de acesso que os usuários têm Partner Center, as funções e permissões que você conceda a você determinar.</span><span class="sxs-lookup"><span data-stu-id="4baf0-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="4baf0-109">As funções estão relacionadas aos programas de que sua empresa está envolvida no.</span><span class="sxs-lookup"><span data-stu-id="4baf0-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="4baf0-110">Por exemplo, se sua empresa é uma empresa de provedor de solução de nuvem (CSP), você não somente terá o Azure AD padrão funções de gerenciamento como administrador global do locatário, mas será necessário a funções específicas para o programa CSP.</span><span class="sxs-lookup"><span data-stu-id="4baf0-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="4baf0-111">Cada programa tem funções específicas a ela.</span><span class="sxs-lookup"><span data-stu-id="4baf0-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="4baf0-112">As funções de locatário do Azure Active Directory (AAD) incluem administrador global, administrador de usuários e funções CSP.</span><span class="sxs-lookup"><span data-stu-id="4baf0-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="4baf0-113">Funções do AAD não são essas funções que não gerencia o locatário e elas incluem MPN admin, administrador de perfil de negócios, administração de indicação, incentivo administrador e usuário incentivo.</span><span class="sxs-lookup"><span data-stu-id="4baf0-113">Non-AAD roles are those roles that do not manage the tenant and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="4baf0-114">Gerenciar transações comerciais no Partner Center (Azure AD e as funções do CSP)</span><span class="sxs-lookup"><span data-stu-id="4baf0-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="4baf0-115">**Função**</span><span class="sxs-lookup"><span data-stu-id="4baf0-115">**Role**</span></span>|<span data-ttu-id="4baf0-116">**O que pode fazer**</span><span class="sxs-lookup"><span data-stu-id="4baf0-116">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="4baf0-117">Administração global</span><span class="sxs-lookup"><span data-stu-id="4baf0-117">Global admin</span></span>|<span data-ttu-id="4baf0-118">• Podem acessar todos os Microsoft/serviços de conta com privilégios totais</span><span class="sxs-lookup"><span data-stu-id="4baf0-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="4baf0-119">• Criar tíquetes de suporte para o Centro de parceiros</span><span class="sxs-lookup"><span data-stu-id="4baf0-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="4baf0-120">• Exibir contratos, listas de preços e ofertas</span><span class="sxs-lookup"><span data-stu-id="4baf0-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="4baf0-121">• Exibir, criar e gerenciar os usuários do parceiro</span><span class="sxs-lookup"><span data-stu-id="4baf0-121">• View, create, and manage partner users</span></span>|
|<span data-ttu-id="4baf0-122">Usuário administrador</span><span class="sxs-lookup"><span data-stu-id="4baf0-122">User Admin</span></span>   | <span data-ttu-id="4baf0-123">• Exibir, criar e gerenciar usuários</span><span class="sxs-lookup"><span data-stu-id="4baf0-123">•   View, create, and manage users</span></span>
||<span data-ttu-id="4baf0-124">• Exibir todos os perfis de parceiros</span><span class="sxs-lookup"><span data-stu-id="4baf0-124">• View all partner profiles</span></span>
||<span data-ttu-id="4baf0-125">• Exibir, criar e gerenciar os usuários do parceiro</span><span class="sxs-lookup"><span data-stu-id="4baf0-125">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="4baf0-126">Administrador de cobrança</span><span class="sxs-lookup"><span data-stu-id="4baf0-126">Billing admin</span></span> | <span data-ttu-id="4baf0-127">-Exibir, criar e gerenciar arquivos recon, faturas e cobrança</span><span class="sxs-lookup"><span data-stu-id="4baf0-127">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="4baf0-128">Usuário padrão</span><span class="sxs-lookup"><span data-stu-id="4baf0-128">Default user</span></span>|  <span data-ttu-id="4baf0-129">Exibir meu perfil</span><span class="sxs-lookup"><span data-stu-id="4baf0-129">View My profile</span></span>   |
|<span data-ttu-id="4baf0-130">Agente administrador</span><span class="sxs-lookup"><span data-stu-id="4baf0-130">Admin agent</span></span> | <span data-ttu-id="4baf0-131">• Gerenciamento de cliente</span><span class="sxs-lookup"><span data-stu-id="4baf0-131">•    Customer management</span></span>
||<span data-ttu-id="4baf0-132">• Adicionar lista de dispositivos para o Centro de parceiros <</span><span class="sxs-lookup"><span data-stu-id="4baf0-132">• Add device list to the Partner Center<</span></span>
||<span data-ttu-id="4baf0-133">• Criar e aplicar perfis de dispositivos</span><span class="sxs-lookup"><span data-stu-id="4baf0-133">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="4baf0-134">• Gerenciamento de assinatura</span><span class="sxs-lookup"><span data-stu-id="4baf0-134">• Subscription management</span></span>
||<span data-ttu-id="4baf0-135">• Integridade e o serviço de solicitações de clientes</span><span class="sxs-lookup"><span data-stu-id="4baf0-135">• Service health and service requests for customers</span></span>
||<span data-ttu-id="4baf0-136">• Solicitação delegada privilégios de administrador</span><span class="sxs-lookup"><span data-stu-id="4baf0-136">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="4baf0-137">• Exibir preço e ofertas</span><span class="sxs-lookup"><span data-stu-id="4baf0-137">• View pricing and offers</span></span>
||<span data-ttu-id="4baf0-138">• Cobrança</span><span class="sxs-lookup"><span data-stu-id="4baf0-138">• Billing</span></span>
||<span data-ttu-id="4baf0-139">• Administrar em nome de um cliente</span><span class="sxs-lookup"><span data-stu-id="4baf0-139">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="4baf0-140">• Registre-se um valor adicionado revendedor</span><span class="sxs-lookup"><span data-stu-id="4baf0-140">• Register a value added reseller</span></span>|
|<span data-ttu-id="4baf0-141">Agente de vendas</span><span class="sxs-lookup"><span data-stu-id="4baf0-141">Sales agent</span></span> | <span data-ttu-id="4baf0-142">• Gerenciamento de cliente</span><span class="sxs-lookup"><span data-stu-id="4baf0-142">•    Customer management</span></span>
||<span data-ttu-id="4baf0-143">• Adicionar lista de dispositivos para o Centro de parceiros</span><span class="sxs-lookup"><span data-stu-id="4baf0-143">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="4baf0-144">• Gerenciamento de assinatura</span><span class="sxs-lookup"><span data-stu-id="4baf0-144">• Subscription management</span></span>
||<span data-ttu-id="4baf0-145">• Exibir preço de lista e oferece</span><span class="sxs-lookup"><span data-stu-id="4baf0-145">• View price lists and offers</span></span>
||<span data-ttu-id="4baf0-146">• Tíquetes de suporte de modo de exibição</span><span class="sxs-lookup"><span data-stu-id="4baf0-146">• View support tickets</span></span>
||<span data-ttu-id="4baf0-147">• Solicitação uma relação com um cliente</span><span class="sxs-lookup"><span data-stu-id="4baf0-147">• Request a relationship with a customer</span></span>
||<span data-ttu-id="4baf0-148">• Gerenciar clientes potenciais</span><span class="sxs-lookup"><span data-stu-id="4baf0-148">• Manage customer leads</span></span>
||<span data-ttu-id="4baf0-149">• Exibir o contrato do cliente</span><span class="sxs-lookup"><span data-stu-id="4baf0-149">• View the customer agreement</span></span>
||<span data-ttu-id="4baf0-150">• Registre-se um revendedor de valor agregado</span><span class="sxs-lookup"><span data-stu-id="4baf0-150">• Register a value-added reseller</span></span>|
|<span data-ttu-id="4baf0-151">Agente de suporte técnico</span><span class="sxs-lookup"><span data-stu-id="4baf0-151">Helpdesk agent</span></span>| <span data-ttu-id="4baf0-152">• Pesquisar e exibir um cliente</span><span class="sxs-lookup"><span data-stu-id="4baf0-152">•  Search for and view a customer</span></span>
||<span data-ttu-id="4baf0-153">• Editar detalhes do cliente</span><span class="sxs-lookup"><span data-stu-id="4baf0-153">• Edit customer details</span></span>
||<span data-ttu-id="4baf0-154">• Ajuda resolver problemas de cliente com o gerenciamento de cobrança ou assinatura</span><span class="sxs-lookup"><span data-stu-id="4baf0-154">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="4baf0-155">• Suporte a solicitação em nome dos clientes (Observação: Você deve ser um agente de administrador para concluir essa tarefa para assinaturas do Office 365)</span><span class="sxs-lookup"><span data-stu-id="4baf0-155">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="4baf0-156">• Gerenciar assinaturas e cobrança problemas em nome dos clientes (Observação: Você deve ser um agente de administrador para concluir essa tarefa para assinaturas do Office 365)</span><span class="sxs-lookup"><span data-stu-id="4baf0-156">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="4baf0-157">Fornecedor do painel de controle (CPV).</span><span class="sxs-lookup"><span data-stu-id="4baf0-157">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="4baf0-158">(Função do CSP e função de não-AAD)</span><span class="sxs-lookup"><span data-stu-id="4baf0-158">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="4baf0-159">CPVs desenvolver aplicativos para uso pelos parceiros de provedor de solução de nuvem (CSP) para que eles possam integrar seus sistemas com APIs do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="4baf0-159">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="4baf0-160">**Função**</span><span class="sxs-lookup"><span data-stu-id="4baf0-160">**Role**</span></span>   |<span data-ttu-id="4baf0-161">**O que você pode fazer**</span><span class="sxs-lookup"><span data-stu-id="4baf0-161">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="4baf0-162">Administração global</span><span class="sxs-lookup"><span data-stu-id="4baf0-162">Global admin</span></span>| <span data-ttu-id="4baf0-163">Exibir e gerenciar seu perfil CPV</span><span class="sxs-lookup"><span data-stu-id="4baf0-163">View and manage your CPV profile</span></span>|
||<span data-ttu-id="4baf0-164">Exibir e gerenciar qualquer um dos seus usuários que precisam de acesso aos recursos de CPV</span><span class="sxs-lookup"><span data-stu-id="4baf0-164">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="4baf0-165">Usuário convidado (deve ser adicionado ao locatário do AAD)</span><span class="sxs-lookup"><span data-stu-id="4baf0-165">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="4baf0-166">**Usuário convidado**</span><span class="sxs-lookup"><span data-stu-id="4baf0-166">**Guest user**</span></span>   | <span data-ttu-id="4baf0-167">**Funções**</span><span class="sxs-lookup"><span data-stu-id="4baf0-167">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="4baf0-168">Administrador de parceiros do MPN</span><span class="sxs-lookup"><span data-stu-id="4baf0-168">MPN partner admin</span></span>|
||<span data-ttu-id="4baf0-169">Contas de administrador</span><span class="sxs-lookup"><span data-stu-id="4baf0-169">Accounts admin</span></span>|
||<span data-ttu-id="4baf0-170">Administrador de incentivos</span><span class="sxs-lookup"><span data-stu-id="4baf0-170">Incentives admin</span></span>|
||<span data-ttu-id="4baf0-171">Administrador de perfis de negócios</span><span class="sxs-lookup"><span data-stu-id="4baf0-171">Business profile admin</span></span>|
||<span data-ttu-id="4baf0-172">Administrador de referências</span><span class="sxs-lookup"><span data-stu-id="4baf0-172">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="4baf0-173">Gerenciar a associação da MPN e sua empresa (funções de não-AAD: essas funções de gerenciam os negócios da empresa em vez de locatário)</span><span class="sxs-lookup"><span data-stu-id="4baf0-173">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="4baf0-174">**Função**</span><span class="sxs-lookup"><span data-stu-id="4baf0-174">**Role**</span></span> | <span data-ttu-id="4baf0-175">**O que você pode fazer**</span><span class="sxs-lookup"><span data-stu-id="4baf0-175">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="4baf0-176">Administrador de parceiros do MPN</span><span class="sxs-lookup"><span data-stu-id="4baf0-176">MPN partner admin</span></span>|<span data-ttu-id="4baf0-177">•CAN adicionar usuários de locatário não</span><span class="sxs-lookup"><span data-stu-id="4baf0-177">•Can add non-tenant users</span></span>
||<span data-ttu-id="4baf0-178">• Exibir, criar e gerenciar solicitações de serviço do parceiro</span><span class="sxs-lookup"><span data-stu-id="4baf0-178">• View, create, and manage partner service requests</span></span>
||<span data-ttu-id="4baf0-179">• Exibir legal, organização, negócios e perfis do MPN</span><span class="sxs-lookup"><span data-stu-id="4baf0-179">• View legal, organization, business, and MPN profiles</span></span>
||<span data-ttu-id="4baf0-180">• Exibir detalhes do usuário e seus dados de habilidades</span><span class="sxs-lookup"><span data-stu-id="4baf0-180">• View user details and their skills data</span></span>
||<span data-ttu-id="4baf0-181">• Exibir competências</span><span class="sxs-lookup"><span data-stu-id="4baf0-181">• View competencies</span></span>
||<span data-ttu-id="4baf0-182">• Exibir e gerenciar os benefícios</span><span class="sxs-lookup"><span data-stu-id="4baf0-182">• View and manage benefits</span></span>
||<span data-ttu-id="4baf0-183">Compra e o modo de exibição • o MPN oferece</span><span class="sxs-lookup"><span data-stu-id="4baf0-183">• View and purchase MPN offers</span></span>
||<span data-ttu-id="4baf0-184">• Exibir MPN oferece notas fiscais e histórico de pedidos</span><span class="sxs-lookup"><span data-stu-id="4baf0-184">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="4baf0-185">• Exibir dados de contribuição de parceiro</span><span class="sxs-lookup"><span data-stu-id="4baf0-185">• View partner contribution data</span></span>
||<span data-ttu-id="4baf0-186">• Podem trabalhar na ferramenta de validação de comprovante</span><span class="sxs-lookup"><span data-stu-id="4baf0-186">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="4baf0-187">-Exibir a análise de dados do cliente</span><span class="sxs-lookup"><span data-stu-id="4baf0-187">- View customer data analytics</span></span>
|<span data-ttu-id="4baf0-188">Administrador da conta</span><span class="sxs-lookup"><span data-stu-id="4baf0-188">Account admin</span></span>| <span data-ttu-id="4baf0-189">• Pode adicionar usuários de locatário não</span><span class="sxs-lookup"><span data-stu-id="4baf0-189">•   Can add non-tenant users</span></span>
||<span data-ttu-id="4baf0-190">• Adicionar ou excluir locais</span><span class="sxs-lookup"><span data-stu-id="4baf0-190">• Add or delete locations</span></span>
||<span data-ttu-id="4baf0-191">-Gerenciar perfis relacionados às contas que você é administrador</span><span class="sxs-lookup"><span data-stu-id="4baf0-191">- Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="4baf0-192">• Atribuir funções para usuários no locatário para funções do AAD não</span><span class="sxs-lookup"><span data-stu-id="4baf0-192">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="4baf0-193">• Registrar locais em programas</span><span class="sxs-lookup"><span data-stu-id="4baf0-193">• Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="4baf0-194">Gerenciar indicações</span><span class="sxs-lookup"><span data-stu-id="4baf0-194">Manage referrals</span></span> 

|<span data-ttu-id="4baf0-195">**Função**</span><span class="sxs-lookup"><span data-stu-id="4baf0-195">**Role**</span></span>|<span data-ttu-id="4baf0-196">**O que você pode fazer**</span><span class="sxs-lookup"><span data-stu-id="4baf0-196">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="4baf0-197">Administrador de referências</span><span class="sxs-lookup"><span data-stu-id="4baf0-197">Referrals admin</span></span>       |<span data-ttu-id="4baf0-198">• Exibir, criar e gerenciar perfis de negócios</span><span class="sxs-lookup"><span data-stu-id="4baf0-198">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="4baf0-199">• Receber e gerenciar as referências</span><span class="sxs-lookup"><span data-stu-id="4baf0-199">• Receive and manage referrals</span></span>
||<span data-ttu-id="4baf0-200">• Exibir, criar e gerenciar as referências de venda conjunta</span><span class="sxs-lookup"><span data-stu-id="4baf0-200">• View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="4baf0-201">• Exibir, criar e gerenciar solicitações de serviço do parceiro</span><span class="sxs-lookup"><span data-stu-id="4baf0-201">• View, create, and manage partner service requests</span></span>
|<span data-ttu-id="4baf0-202">Administrador de perfis de negócios</span><span class="sxs-lookup"><span data-stu-id="4baf0-202">Business profile admin</span></span>   |<span data-ttu-id="4baf0-203">• Exibir, criar e gerenciar um perfil comercial</span><span class="sxs-lookup"><span data-stu-id="4baf0-203">• View, create, and manage business profile</span></span> 
||<span data-ttu-id="4baf0-204">• Exibir, criar e gerenciar solicitações de serviço do parceiro</span><span class="sxs-lookup"><span data-stu-id="4baf0-204">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="4baf0-205">Gerenciar incentivos</span><span class="sxs-lookup"><span data-stu-id="4baf0-205">Manage incentives</span></span> 

|<span data-ttu-id="4baf0-206">**Função**</span><span class="sxs-lookup"><span data-stu-id="4baf0-206">**Role**</span></span> | <span data-ttu-id="4baf0-207">**O que você pode fazer**</span><span class="sxs-lookup"><span data-stu-id="4baf0-207">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="4baf0-208">Administrador de incentivos</span><span class="sxs-lookup"><span data-stu-id="4baf0-208">Incentives admin</span></span>|<span data-ttu-id="4baf0-209">• Inicia e gerencia incentivos</span><span class="sxs-lookup"><span data-stu-id="4baf0-209">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="4baf0-210">• Pode exibir e editar todos os aspectos de programas de incentivos</span><span class="sxs-lookup"><span data-stu-id="4baf0-210">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="4baf0-211">• Pode exibir e editar os detalhes do banco e imposto</span><span class="sxs-lookup"><span data-stu-id="4baf0-211">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="4baf0-212">• Ganhos de reembolso e cooperação do modo de exibição</span><span class="sxs-lookup"><span data-stu-id="4baf0-212">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="4baf0-213">• Suporte a acesso</span><span class="sxs-lookup"><span data-stu-id="4baf0-213">• Access support</span></span>
||<span data-ttu-id="4baf0-214">• Os pagamentos incentivos de controvérsias</span><span class="sxs-lookup"><span data-stu-id="4baf0-214">• Dispute incentives payments</span></span>|
|<span data-ttu-id="4baf0-215">Usuário de incentivos</span><span class="sxs-lookup"><span data-stu-id="4baf0-215">Incentives user</span></span>|<span data-ttu-id="4baf0-216">• Podem exibir programas incentivos</span><span class="sxs-lookup"><span data-stu-id="4baf0-216">•  Can view incentives programs</span></span>
||<span data-ttu-id="4baf0-217">• Pode exibir e iniciar as declarações de incentivos</span><span class="sxs-lookup"><span data-stu-id="4baf0-217">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="4baf0-218">• Ganhos de reembolso e cooperação do modo de exibição</span><span class="sxs-lookup"><span data-stu-id="4baf0-218">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="4baf0-219">• Ganhos de reembolso e cooperação do modo de exibição</span><span class="sxs-lookup"><span data-stu-id="4baf0-219">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="4baf0-220">• Suporte a acesso</span><span class="sxs-lookup"><span data-stu-id="4baf0-220">• Access support</span></span>












