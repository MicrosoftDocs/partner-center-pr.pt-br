---
title: Atribuir funções e permissões de usuários | Partner Center
ms.topic: article
ms.date: 10/10/2019
description: É necessário atribuir uma função a todos os funcionários que precisam trabalhar no Partner Center.
author: LauraBrenner
ms.author: labrenne
keywords: funções, permissões, administrador, agente
ms.localizationpriority: high
ms.openlocfilehash: 0bbc9af84b8a1464f255c17147fdc10a7504eb43
ms.sourcegitcommit: 1ccc27092949deb6f6404e64fd6a628fd7b5fd5c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/11/2019
ms.locfileid: "72276096"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="c2a3c-104">Atribuir permissões e funções de usuários</span><span class="sxs-lookup"><span data-stu-id="c2a3c-104">Assign users roles and permissions</span></span>


<span data-ttu-id="c2a3c-105">Você configurou seu perfil de parceiro, incluindo a razão social, o endereço, os detalhes de suporte, as isenções de imposto sobre arquivos, as informações bancárias e o contato principal da empresa.</span><span class="sxs-lookup"><span data-stu-id="c2a3c-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="c2a3c-106">Próxima etapa: configure as senhas e funções de seus usuários para que eles possam começar a trabalhar no Partner Center com você.</span><span class="sxs-lookup"><span data-stu-id="c2a3c-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="c2a3c-107">Configurar seus funcionários para trabalhar no Partner Center</span><span class="sxs-lookup"><span data-stu-id="c2a3c-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="c2a3c-108">Você determinará os tipos de acesso que os usuários terão ao Partner Center por meio das funções e permissões a eles atribuídas.</span><span class="sxs-lookup"><span data-stu-id="c2a3c-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="c2a3c-109">As funções estão relacionadas aos programas com os quais a sua empresa está envolvida.</span><span class="sxs-lookup"><span data-stu-id="c2a3c-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="c2a3c-110">Por exemplo, se a sua empresa for um CSP (Provedor de Soluções na Nuvem), você não apenas terá as funções de gerenciamento de locatário padrão do Azure AD, como o administrador global, mas também precisará de funções específicas para o programa CSP.</span><span class="sxs-lookup"><span data-stu-id="c2a3c-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="c2a3c-111">Cada programa tem funções específicas para ele.</span><span class="sxs-lookup"><span data-stu-id="c2a3c-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="c2a3c-112">As funções de locatário do Azure Active Directory (AAD) incluem administrador global, administrador de usuários e funções de CSP.</span><span class="sxs-lookup"><span data-stu-id="c2a3c-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="c2a3c-113">As funções não pertencentes ao AAD são aquelas que não gerenciam o locatário e incluem administrador do MPN, administrador de perfil de negócios, administrador de indicações, administrador de incentivos e usuário de incentivos.</span><span class="sxs-lookup"><span data-stu-id="c2a3c-113">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="c2a3c-114">Gerenciar transações comerciais no Partner Center (funções Azure AD e CSP)</span><span class="sxs-lookup"><span data-stu-id="c2a3c-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="c2a3c-115">**Função**</span><span class="sxs-lookup"><span data-stu-id="c2a3c-115">**Role**</span></span>|<span data-ttu-id="c2a3c-116">**O que eles podem fazer**</span><span class="sxs-lookup"><span data-stu-id="c2a3c-116">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="c2a3c-117">Administração global</span><span class="sxs-lookup"><span data-stu-id="c2a3c-117">Global admin</span></span>|<span data-ttu-id="c2a3c-118">• Podem acessar todas as contas/os serviços da Microsoft com todos os privilégios</span><span class="sxs-lookup"><span data-stu-id="c2a3c-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="c2a3c-119">• Criar tíquetes de suporte para o Partner Center</span><span class="sxs-lookup"><span data-stu-id="c2a3c-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="c2a3c-120">• Exibir contratos, listas de preços e ofertas</span><span class="sxs-lookup"><span data-stu-id="c2a3c-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="c2a3c-121">• Exibir, criar e gerenciar usuários parceiros</span><span class="sxs-lookup"><span data-stu-id="c2a3c-121">• View, create, and manage partner users</span></span>|
||  <span data-ttu-id="c2a3c-122">• Exibir, criar e gerenciar a cobrança, as faturas e os arquivos reconhecimento</span><span class="sxs-lookup"><span data-stu-id="c2a3c-122">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="c2a3c-123">Administrador de gerenciamento de usuário</span><span class="sxs-lookup"><span data-stu-id="c2a3c-123">User management admin</span></span>   | <span data-ttu-id="c2a3c-124">• Exibir, criar e gerenciar usuários</span><span class="sxs-lookup"><span data-stu-id="c2a3c-124">•    View, create, and manage users</span></span>
||<span data-ttu-id="c2a3c-125">• Exibir todos os perfis de parceiros</span><span class="sxs-lookup"><span data-stu-id="c2a3c-125">• View all partner profiles</span></span>
||<span data-ttu-id="c2a3c-126">• Exibir, criar e gerenciar usuários parceiros</span><span class="sxs-lookup"><span data-stu-id="c2a3c-126">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="c2a3c-127">Administrador de cobrança</span><span class="sxs-lookup"><span data-stu-id="c2a3c-127">Billing admin</span></span> | <span data-ttu-id="c2a3c-128">– Exibir, criar e gerenciar a cobrança, as faturas e os arquivos reconhecimento</span><span class="sxs-lookup"><span data-stu-id="c2a3c-128">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="c2a3c-129">Usuário padrão</span><span class="sxs-lookup"><span data-stu-id="c2a3c-129">Default user</span></span>|  <span data-ttu-id="c2a3c-130">Exibir meu perfil</span><span class="sxs-lookup"><span data-stu-id="c2a3c-130">View My profile</span></span>   |
|<span data-ttu-id="c2a3c-131">Agente administrador</span><span class="sxs-lookup"><span data-stu-id="c2a3c-131">Admin agent</span></span> | <span data-ttu-id="c2a3c-132">• Gerenciamento de clientes</span><span class="sxs-lookup"><span data-stu-id="c2a3c-132">•    Customer management</span></span>
||<span data-ttu-id="c2a3c-133">• Adicionar lista de dispositivos ao Partner Center</span><span class="sxs-lookup"><span data-stu-id="c2a3c-133">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="c2a3c-134">• Criar e aplicar perfis aos dispositivos</span><span class="sxs-lookup"><span data-stu-id="c2a3c-134">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="c2a3c-135">• Gerenciamento de assinaturas</span><span class="sxs-lookup"><span data-stu-id="c2a3c-135">• Subscription management</span></span>
||<span data-ttu-id="c2a3c-136">• Solicitações de integridade e de serviços para os clientes</span><span class="sxs-lookup"><span data-stu-id="c2a3c-136">• Service health and service requests for customers</span></span>
||<span data-ttu-id="c2a3c-137">• Solicitar privilégios de administrador delegado</span><span class="sxs-lookup"><span data-stu-id="c2a3c-137">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="c2a3c-138">• Exibir preços e ofertas</span><span class="sxs-lookup"><span data-stu-id="c2a3c-138">• View pricing and offers</span></span>
||<span data-ttu-id="c2a3c-139">• Cobrança</span><span class="sxs-lookup"><span data-stu-id="c2a3c-139">• Billing</span></span>
||<span data-ttu-id="c2a3c-140">• Administrar em nome de um cliente</span><span class="sxs-lookup"><span data-stu-id="c2a3c-140">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="c2a3c-141">• Registrar um revendedor com alto valor agregado</span><span class="sxs-lookup"><span data-stu-id="c2a3c-141">• Register a value added reseller</span></span>|
|<span data-ttu-id="c2a3c-142">Agente de vendas</span><span class="sxs-lookup"><span data-stu-id="c2a3c-142">Sales agent</span></span> | <span data-ttu-id="c2a3c-143">• Gerenciamento de clientes</span><span class="sxs-lookup"><span data-stu-id="c2a3c-143">•    Customer management</span></span>
||<span data-ttu-id="c2a3c-144">• Adicionar lista de dispositivos ao Partner Center</span><span class="sxs-lookup"><span data-stu-id="c2a3c-144">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="c2a3c-145">• Gerenciamento de assinaturas</span><span class="sxs-lookup"><span data-stu-id="c2a3c-145">• Subscription management</span></span>
||<span data-ttu-id="c2a3c-146">• Exibir tíquetes de suporte</span><span class="sxs-lookup"><span data-stu-id="c2a3c-146">• View support tickets</span></span>
||<span data-ttu-id="c2a3c-147">• Solicitar um relacionamento com um cliente</span><span class="sxs-lookup"><span data-stu-id="c2a3c-147">• Request a relationship with a customer</span></span>
||<span data-ttu-id="c2a3c-148">• Gerenciar clientes em potencial</span><span class="sxs-lookup"><span data-stu-id="c2a3c-148">• Manage customer leads</span></span>
||<span data-ttu-id="c2a3c-149">• Exibir o contrato do cliente</span><span class="sxs-lookup"><span data-stu-id="c2a3c-149">• View the customer agreement</span></span>
||<span data-ttu-id="c2a3c-150">• Registrar um revendedor com alto valor agregado</span><span class="sxs-lookup"><span data-stu-id="c2a3c-150">• Register a value-added reseller</span></span>|
|<span data-ttu-id="c2a3c-151">Agente de suporte técnico</span><span class="sxs-lookup"><span data-stu-id="c2a3c-151">Helpdesk agent</span></span>| <span data-ttu-id="c2a3c-152">• Pesquisar e exibir um cliente</span><span class="sxs-lookup"><span data-stu-id="c2a3c-152">•  Search for and view a customer</span></span>
||<span data-ttu-id="c2a3c-153">• Editar detalhes do cliente</span><span class="sxs-lookup"><span data-stu-id="c2a3c-153">• Edit customer details</span></span>
||<span data-ttu-id="c2a3c-154">• Ajudar a resolver problemas dos clientes com o gerenciamento de cobrança ou assinaturas</span><span class="sxs-lookup"><span data-stu-id="c2a3c-154">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="c2a3c-155">• Solicitar suporte em nome dos clientes (Observação: é necessário ser um agente administrador para concluir esta tarefa para assinaturas do Office 365)</span><span class="sxs-lookup"><span data-stu-id="c2a3c-155">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="c2a3c-156">• Gerenciar assinaturas e problemas de cobrança em nome dos clientes (Observação: é necessário ser um agente administrador para concluir esta tarefa para assinaturas do Office 365)</span><span class="sxs-lookup"><span data-stu-id="c2a3c-156">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="c2a3c-157">CPV (Fornecedor de Painel de Controle).</span><span class="sxs-lookup"><span data-stu-id="c2a3c-157">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="c2a3c-158">(Função CSP e função não pertencente ao AAD)</span><span class="sxs-lookup"><span data-stu-id="c2a3c-158">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="c2a3c-159">Os CPVs desenvolvem aplicativos para uso por parceiros CSP (Provedor de Soluções na Nuvem) a fim de permitir que eles integrem seus sistemas com as APIs do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="c2a3c-159">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="c2a3c-160">**Função**</span><span class="sxs-lookup"><span data-stu-id="c2a3c-160">**Role**</span></span>   |<span data-ttu-id="c2a3c-161">**O que você pode fazer**</span><span class="sxs-lookup"><span data-stu-id="c2a3c-161">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="c2a3c-162">Administração global</span><span class="sxs-lookup"><span data-stu-id="c2a3c-162">Global admin</span></span>| <span data-ttu-id="c2a3c-163">Exibir e gerenciar seu perfil de CPV</span><span class="sxs-lookup"><span data-stu-id="c2a3c-163">View and manage your CPV profile</span></span>|
||<span data-ttu-id="c2a3c-164">Exibir e gerenciar todos os seus usuários que precisam de acesso aos recursos de CPV</span><span class="sxs-lookup"><span data-stu-id="c2a3c-164">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="c2a3c-165">Usuário convidado (deve ser adicionado ao locatário do AAD)</span><span class="sxs-lookup"><span data-stu-id="c2a3c-165">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="c2a3c-166">**Usuário convidado**</span><span class="sxs-lookup"><span data-stu-id="c2a3c-166">**Guest user**</span></span>   | <span data-ttu-id="c2a3c-167">**Funções**</span><span class="sxs-lookup"><span data-stu-id="c2a3c-167">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="c2a3c-168">Administrador de parceiros do MPN</span><span class="sxs-lookup"><span data-stu-id="c2a3c-168">MPN partner admin</span></span>|
||<span data-ttu-id="c2a3c-169">Administrador de contas</span><span class="sxs-lookup"><span data-stu-id="c2a3c-169">Accounts admin</span></span>|
||<span data-ttu-id="c2a3c-170">Administrador de incentivos</span><span class="sxs-lookup"><span data-stu-id="c2a3c-170">Incentives admin</span></span>|
||<span data-ttu-id="c2a3c-171">Administrador de perfis de negócios</span><span class="sxs-lookup"><span data-stu-id="c2a3c-171">Business profile admin</span></span>|
||<span data-ttu-id="c2a3c-172">Administrador de indicações</span><span class="sxs-lookup"><span data-stu-id="c2a3c-172">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="c2a3c-173">Gerenciar associação do MPN e sua empresa (funções não pertencentes ao AAD: essas funções gerenciam os negócios da empresa em vez do locatário)</span><span class="sxs-lookup"><span data-stu-id="c2a3c-173">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="c2a3c-174">**Função**</span><span class="sxs-lookup"><span data-stu-id="c2a3c-174">**Role**</span></span> | <span data-ttu-id="c2a3c-175">**O que você pode fazer**</span><span class="sxs-lookup"><span data-stu-id="c2a3c-175">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="c2a3c-176">Administrador de parceiros do MPN</span><span class="sxs-lookup"><span data-stu-id="c2a3c-176">MPN partner admin</span></span>|<span data-ttu-id="c2a3c-177">• Exibir, criar e gerenciar solicitações de serviço de parceiros</span><span class="sxs-lookup"><span data-stu-id="c2a3c-177">•    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="c2a3c-178">• Exibir perfis jurídico, empresarial, de negócios e do MPN</span><span class="sxs-lookup"><span data-stu-id="c2a3c-178">• View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="c2a3c-179">• Exibir detalhes do usuário e seus dados de habilidades</span><span class="sxs-lookup"><span data-stu-id="c2a3c-179">• View user details and their skills data</span></span>
||<span data-ttu-id="c2a3c-180">• Exibir competências</span><span class="sxs-lookup"><span data-stu-id="c2a3c-180">• View competencies</span></span>
||<span data-ttu-id="c2a3c-181">• Exibir e gerenciar benefícios</span><span class="sxs-lookup"><span data-stu-id="c2a3c-181">• View and manage benefits</span></span>
||<span data-ttu-id="c2a3c-182">• Exibir e comprar ofertas do MPN</span><span class="sxs-lookup"><span data-stu-id="c2a3c-182">• View and purchase MPN offers</span></span>
||<span data-ttu-id="c2a3c-183">• Exibir histórico de pedidos de ofertas e faturas do MPN</span><span class="sxs-lookup"><span data-stu-id="c2a3c-183">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="c2a3c-184">• Exibir dados do indicador de contribuição de parceiros</span><span class="sxs-lookup"><span data-stu-id="c2a3c-184">• View partner contribution indicator data</span></span>
||<span data-ttu-id="c2a3c-185">• Pode funcionar na ferramenta de validação de comprovantes</span><span class="sxs-lookup"><span data-stu-id="c2a3c-185">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="c2a3c-186">– Exibir análise de dados do cliente</span><span class="sxs-lookup"><span data-stu-id="c2a3c-186">- View customer data analytics</span></span>
|| <span data-ttu-id="c2a3c-187">Exibir outras funções de usuário dentro da empresa, mas não pode atribuir funções</span><span class="sxs-lookup"><span data-stu-id="c2a3c-187">View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="c2a3c-188">Administrador de conta</span><span class="sxs-lookup"><span data-stu-id="c2a3c-188">Account admin</span></span>| <span data-ttu-id="c2a3c-189">Adicionar locais</span><span class="sxs-lookup"><span data-stu-id="c2a3c-189">Add locations</span></span>
|| <span data-ttu-id="c2a3c-190">Gerenciar perfis relacionados às contas para as quais você é administrador</span><span class="sxs-lookup"><span data-stu-id="c2a3c-190">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="c2a3c-191">• Atribuir funções aos usuários do locatário para funções não pertencentes ao AAD</span><span class="sxs-lookup"><span data-stu-id="c2a3c-191">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="c2a3c-192">• Registrar locais em programas</span><span class="sxs-lookup"><span data-stu-id="c2a3c-192">• Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="c2a3c-193">Gerenciar indicações</span><span class="sxs-lookup"><span data-stu-id="c2a3c-193">Manage referrals</span></span> 

|<span data-ttu-id="c2a3c-194">**Função**</span><span class="sxs-lookup"><span data-stu-id="c2a3c-194">**Role**</span></span>|<span data-ttu-id="c2a3c-195">**O que você pode fazer**</span><span class="sxs-lookup"><span data-stu-id="c2a3c-195">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="c2a3c-196">Administrador de indicações</span><span class="sxs-lookup"><span data-stu-id="c2a3c-196">Referrals admin</span></span>       |<span data-ttu-id="c2a3c-197">• Exibir, criar e gerenciar perfis de negócios</span><span class="sxs-lookup"><span data-stu-id="c2a3c-197">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="c2a3c-198">• Receber e gerenciar indicações</span><span class="sxs-lookup"><span data-stu-id="c2a3c-198">• Receive and manage referrals</span></span>
||<span data-ttu-id="c2a3c-199">• Exibir, criar e gerenciar as referências indicações de venda conjunta</span><span class="sxs-lookup"><span data-stu-id="c2a3c-199">• View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="c2a3c-200">• Exibir, criar e gerenciar solicitações de serviço de parceiros</span><span class="sxs-lookup"><span data-stu-id="c2a3c-200">• View, create, and manage partner service requests</span></span>
|<span data-ttu-id="c2a3c-201">Administrador de perfis de negócios</span><span class="sxs-lookup"><span data-stu-id="c2a3c-201">Business profile admin</span></span>   |<span data-ttu-id="c2a3c-202">• Exibir, criar e gerenciar perfis de negócios</span><span class="sxs-lookup"><span data-stu-id="c2a3c-202">• View, create, and manage business profile</span></span> 
||<span data-ttu-id="c2a3c-203">• Exibir, criar e gerenciar solicitações de serviço de parceiros</span><span class="sxs-lookup"><span data-stu-id="c2a3c-203">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="c2a3c-204">Gerenciar incentivos</span><span class="sxs-lookup"><span data-stu-id="c2a3c-204">Manage incentives</span></span> 

|<span data-ttu-id="c2a3c-205">**Função**</span><span class="sxs-lookup"><span data-stu-id="c2a3c-205">**Role**</span></span> | <span data-ttu-id="c2a3c-206">**O que você pode fazer**</span><span class="sxs-lookup"><span data-stu-id="c2a3c-206">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="c2a3c-207">Administrador de incentivos</span><span class="sxs-lookup"><span data-stu-id="c2a3c-207">Incentives admin</span></span>|<span data-ttu-id="c2a3c-208">• Iniciar e gerenciar incentivos</span><span class="sxs-lookup"><span data-stu-id="c2a3c-208">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="c2a3c-209">• Poder exibir e editar todos os aspectos dos programas de incentivos</span><span class="sxs-lookup"><span data-stu-id="c2a3c-209">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="c2a3c-210">• Poder exibir e editar detalhes bancários e fiscais</span><span class="sxs-lookup"><span data-stu-id="c2a3c-210">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="c2a3c-211">• Exibir lucros de reembolso e de cooperação</span><span class="sxs-lookup"><span data-stu-id="c2a3c-211">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="c2a3c-212">• Acessar suporte</span><span class="sxs-lookup"><span data-stu-id="c2a3c-212">• Access support</span></span>
||<span data-ttu-id="c2a3c-213">• Disputar pagamentos de incentivos</span><span class="sxs-lookup"><span data-stu-id="c2a3c-213">• Dispute incentives payments</span></span>|
|<span data-ttu-id="c2a3c-214">Usuário de incentivos</span><span class="sxs-lookup"><span data-stu-id="c2a3c-214">Incentives user</span></span>|<span data-ttu-id="c2a3c-215">• Poderá exibir programas de incentivos</span><span class="sxs-lookup"><span data-stu-id="c2a3c-215">•  Can view incentives programs</span></span>
||<span data-ttu-id="c2a3c-216">• Poderá exibir e iniciar reivindicações de incentivos</span><span class="sxs-lookup"><span data-stu-id="c2a3c-216">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="c2a3c-217">• Exibir lucros de reembolso e de cooperação</span><span class="sxs-lookup"><span data-stu-id="c2a3c-217">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="c2a3c-218">• Acessar suporte</span><span class="sxs-lookup"><span data-stu-id="c2a3c-218">• Access support</span></span>












