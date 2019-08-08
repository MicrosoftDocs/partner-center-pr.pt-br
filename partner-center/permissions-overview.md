---
title: Atribuir funções e permissões de usuários | Partner Center
ms.topic: article
ms.date: 3/5/2019
description: Cada funcionário que precisa trabalhar no Partner Center deve ser atribuído a uma função.
author: LauraBrenner
ms.author: labrenne
keywords: funções, permissões, administrador, agente
ms.localizationpriority: medium
ms.openlocfilehash: 744ce84c47d3adaf21d8f7b790001737d6489cdb
ms.sourcegitcommit: 9d01fb30eafc523784ecc3568c05da9bbe9a1e8c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/01/2019
ms.locfileid: "68708865"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="8fdb1-104">Atribuir funções e permissões de usuário</span><span class="sxs-lookup"><span data-stu-id="8fdb1-104">Assign users roles and permissions</span></span>


<span data-ttu-id="8fdb1-105">Você configurou seu perfil de parceiro, incluindo nome legal e endereço, detalhes de suporte, isenções de imposto sobre o arquivo, informações bancárias e o contato principal para sua empresa.</span><span class="sxs-lookup"><span data-stu-id="8fdb1-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="8fdb1-106">Próxima etapa: Configure seus usuários com senhas e funções para que eles possam começar a trabalhar no Partner Center com você.</span><span class="sxs-lookup"><span data-stu-id="8fdb1-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="8fdb1-107">Configurar seus funcionários para trabalhar no Partner Center</span><span class="sxs-lookup"><span data-stu-id="8fdb1-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="8fdb1-108">Você determina os tipos de acesso que os usuários têm ao Partner Center pelas funções e permissões que você lhes dá.</span><span class="sxs-lookup"><span data-stu-id="8fdb1-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="8fdb1-109">As funções estão relacionadas aos programas nos quais sua empresa está envolvida.</span><span class="sxs-lookup"><span data-stu-id="8fdb1-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="8fdb1-110">Por exemplo, se sua empresa for um negócio CSP (provedor de soluções na nuvem), você não terá apenas as funções de gerenciamento de locatário padrão do Azure AD, como o administrador global, mas precisará de funções específicas para o programa CSP.</span><span class="sxs-lookup"><span data-stu-id="8fdb1-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="8fdb1-111">Cada programa tem funções específicas para ele.</span><span class="sxs-lookup"><span data-stu-id="8fdb1-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="8fdb1-112">As funções de locatário do Azure Active Directory (AAD) incluem administrador global, administrador de usuário e funções de CSP.</span><span class="sxs-lookup"><span data-stu-id="8fdb1-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="8fdb1-113">As funções que não são do AAD são aquelas que não gerenciam o locatário e incluem administrador de MPN, administrador de perfil de negócios, administrador de referência, administrador de incentivos e usuário de incentivo.</span><span class="sxs-lookup"><span data-stu-id="8fdb1-113">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="8fdb1-114">Gerenciar transações comerciais no Partner Center (funções do Azure AD e CSP)</span><span class="sxs-lookup"><span data-stu-id="8fdb1-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="8fdb1-115">**Cargo**</span><span class="sxs-lookup"><span data-stu-id="8fdb1-115">**Role**</span></span>|<span data-ttu-id="8fdb1-116">**O que eles podem fazer**</span><span class="sxs-lookup"><span data-stu-id="8fdb1-116">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="8fdb1-117">Administração global</span><span class="sxs-lookup"><span data-stu-id="8fdb1-117">Global admin</span></span>|<span data-ttu-id="8fdb1-118">• Pode acessar todos os conta Microsoft/serviços com privilégios totais</span><span class="sxs-lookup"><span data-stu-id="8fdb1-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="8fdb1-119">• Criar tíquetes de suporte para o Partner Center</span><span class="sxs-lookup"><span data-stu-id="8fdb1-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="8fdb1-120">• Exibir contratos, listas de preços e ofertas</span><span class="sxs-lookup"><span data-stu-id="8fdb1-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="8fdb1-121">• Exibir, criar e gerenciar usuários parceiros</span><span class="sxs-lookup"><span data-stu-id="8fdb1-121">• View, create, and manage partner users</span></span>|
||  <span data-ttu-id="8fdb1-122">Exibir, criar e gerenciar a cobrança, as notas fiscais e os arquivos reconhecimento</span><span class="sxs-lookup"><span data-stu-id="8fdb1-122">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="8fdb1-123">Administrador de gerenciamento de usuário</span><span class="sxs-lookup"><span data-stu-id="8fdb1-123">User management admin</span></span>   | <span data-ttu-id="8fdb1-124">• Exibir, criar e gerenciar usuários</span><span class="sxs-lookup"><span data-stu-id="8fdb1-124">•    View, create, and manage users</span></span>
||<span data-ttu-id="8fdb1-125">• Exibir todos os perfis de parceiro</span><span class="sxs-lookup"><span data-stu-id="8fdb1-125">• View all partner profiles</span></span>
||<span data-ttu-id="8fdb1-126">• Exibir, criar e gerenciar usuários parceiros</span><span class="sxs-lookup"><span data-stu-id="8fdb1-126">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="8fdb1-127">Administrador de cobrança</span><span class="sxs-lookup"><span data-stu-id="8fdb1-127">Billing admin</span></span> | <span data-ttu-id="8fdb1-128">-Exibir, criar e gerenciar a cobrança, as notas fiscais e os arquivos reconhecimento</span><span class="sxs-lookup"><span data-stu-id="8fdb1-128">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="8fdb1-129">Usuário padrão</span><span class="sxs-lookup"><span data-stu-id="8fdb1-129">Default user</span></span>|  <span data-ttu-id="8fdb1-130">Exibir meu perfil</span><span class="sxs-lookup"><span data-stu-id="8fdb1-130">View My profile</span></span>   |
|<span data-ttu-id="8fdb1-131">Agente administrador</span><span class="sxs-lookup"><span data-stu-id="8fdb1-131">Admin agent</span></span> | <span data-ttu-id="8fdb1-132">• Gerenciamento de clientes</span><span class="sxs-lookup"><span data-stu-id="8fdb1-132">•    Customer management</span></span>
||<span data-ttu-id="8fdb1-133">• Adicionar a lista de dispositivos ao Partner Center</span><span class="sxs-lookup"><span data-stu-id="8fdb1-133">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="8fdb1-134">• Criar e aplicar perfis a dispositivos</span><span class="sxs-lookup"><span data-stu-id="8fdb1-134">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="8fdb1-135">• Gerenciamento de assinatura</span><span class="sxs-lookup"><span data-stu-id="8fdb1-135">• Subscription management</span></span>
||<span data-ttu-id="8fdb1-136">• Serviço de integridade e solicitações de serviço para clientes</span><span class="sxs-lookup"><span data-stu-id="8fdb1-136">• Service health and service requests for customers</span></span>
||<span data-ttu-id="8fdb1-137">• Solicitar privilégios de administrador delegado</span><span class="sxs-lookup"><span data-stu-id="8fdb1-137">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="8fdb1-138">• Exibir preços e ofertas</span><span class="sxs-lookup"><span data-stu-id="8fdb1-138">• View pricing and offers</span></span>
||<span data-ttu-id="8fdb1-139">• Cobrança</span><span class="sxs-lookup"><span data-stu-id="8fdb1-139">• Billing</span></span>
||<span data-ttu-id="8fdb1-140">• Administrar em nome de um cliente</span><span class="sxs-lookup"><span data-stu-id="8fdb1-140">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="8fdb1-141">• Registrar um revendedor de valor agregado</span><span class="sxs-lookup"><span data-stu-id="8fdb1-141">• Register a value added reseller</span></span>|
|<span data-ttu-id="8fdb1-142">Agente de vendas</span><span class="sxs-lookup"><span data-stu-id="8fdb1-142">Sales agent</span></span> | <span data-ttu-id="8fdb1-143">• Gerenciamento de clientes</span><span class="sxs-lookup"><span data-stu-id="8fdb1-143">•    Customer management</span></span>
||<span data-ttu-id="8fdb1-144">• Adicionar a lista de dispositivos ao Partner Center</span><span class="sxs-lookup"><span data-stu-id="8fdb1-144">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="8fdb1-145">• Gerenciamento de assinatura</span><span class="sxs-lookup"><span data-stu-id="8fdb1-145">• Subscription management</span></span>
||<span data-ttu-id="8fdb1-146">• Exibir listas de preços e ofertas</span><span class="sxs-lookup"><span data-stu-id="8fdb1-146">• View price lists and offers</span></span>
||<span data-ttu-id="8fdb1-147">• Exibir tíquetes de suporte</span><span class="sxs-lookup"><span data-stu-id="8fdb1-147">• View support tickets</span></span>
||<span data-ttu-id="8fdb1-148">• Solicitar uma relação com um cliente</span><span class="sxs-lookup"><span data-stu-id="8fdb1-148">• Request a relationship with a customer</span></span>
||<span data-ttu-id="8fdb1-149">• Gerenciar clientes potenciais do cliente</span><span class="sxs-lookup"><span data-stu-id="8fdb1-149">• Manage customer leads</span></span>
||<span data-ttu-id="8fdb1-150">• Exibir o contrato do cliente</span><span class="sxs-lookup"><span data-stu-id="8fdb1-150">• View the customer agreement</span></span>
||<span data-ttu-id="8fdb1-151">• Registrar um revendedor de valor agregado</span><span class="sxs-lookup"><span data-stu-id="8fdb1-151">• Register a value-added reseller</span></span>|
|<span data-ttu-id="8fdb1-152">Agente de suporte técnico</span><span class="sxs-lookup"><span data-stu-id="8fdb1-152">Helpdesk agent</span></span>| <span data-ttu-id="8fdb1-153">• Pesquisar e exibir um cliente</span><span class="sxs-lookup"><span data-stu-id="8fdb1-153">•  Search for and view a customer</span></span>
||<span data-ttu-id="8fdb1-154">• Editar detalhes do cliente</span><span class="sxs-lookup"><span data-stu-id="8fdb1-154">• Edit customer details</span></span>
||<span data-ttu-id="8fdb1-155">• Ajudar a resolver problemas do cliente com gerenciamento de assinaturas ou cobrança</span><span class="sxs-lookup"><span data-stu-id="8fdb1-155">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="8fdb1-156">• Solicitar suporte em nome dos clientes (Observação: Você deve ser um agente de administração para concluir esta tarefa para assinaturas do Office 365)</span><span class="sxs-lookup"><span data-stu-id="8fdb1-156">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="8fdb1-157">• Gerenciar assinaturas e problemas de cobrança em nome dos clientes (Observação: Você deve ser um agente de administração para concluir esta tarefa para assinaturas do Office 365)</span><span class="sxs-lookup"><span data-stu-id="8fdb1-157">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="8fdb1-158">Fornecedor do painel de controle (CPV).</span><span class="sxs-lookup"><span data-stu-id="8fdb1-158">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="8fdb1-159">(Função CSP e função não AAD)</span><span class="sxs-lookup"><span data-stu-id="8fdb1-159">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="8fdb1-160">CPVs desenvolva aplicativos para uso por parceiros do CSP (provedor de soluções na nuvem) para permitir que eles integrem seus sistemas com as APIs do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="8fdb1-160">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="8fdb1-161">**Cargo**</span><span class="sxs-lookup"><span data-stu-id="8fdb1-161">**Role**</span></span>   |<span data-ttu-id="8fdb1-162">**O que você pode fazer**</span><span class="sxs-lookup"><span data-stu-id="8fdb1-162">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="8fdb1-163">Administração global</span><span class="sxs-lookup"><span data-stu-id="8fdb1-163">Global admin</span></span>| <span data-ttu-id="8fdb1-164">Exibir e gerenciar seu perfil do CPV</span><span class="sxs-lookup"><span data-stu-id="8fdb1-164">View and manage your CPV profile</span></span>|
||<span data-ttu-id="8fdb1-165">Exibir e gerenciar qualquer um dos seus usuários que precisam de acesso aos recursos do CPV</span><span class="sxs-lookup"><span data-stu-id="8fdb1-165">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="8fdb1-166">Usuário convidado (deve ser adicionado ao locatário do AAD)</span><span class="sxs-lookup"><span data-stu-id="8fdb1-166">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="8fdb1-167">**Usuário convidado**</span><span class="sxs-lookup"><span data-stu-id="8fdb1-167">**Guest user**</span></span>   | <span data-ttu-id="8fdb1-168">**Papéis**</span><span class="sxs-lookup"><span data-stu-id="8fdb1-168">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="8fdb1-169">Administrador de parceiros do MPN</span><span class="sxs-lookup"><span data-stu-id="8fdb1-169">MPN partner admin</span></span>|
||<span data-ttu-id="8fdb1-170">Administrador de contas</span><span class="sxs-lookup"><span data-stu-id="8fdb1-170">Accounts admin</span></span>|
||<span data-ttu-id="8fdb1-171">Administrador de incentivos</span><span class="sxs-lookup"><span data-stu-id="8fdb1-171">Incentives admin</span></span>|
||<span data-ttu-id="8fdb1-172">Administrador de perfis de negócios</span><span class="sxs-lookup"><span data-stu-id="8fdb1-172">Business profile admin</span></span>|
||<span data-ttu-id="8fdb1-173">Administrador de referências</span><span class="sxs-lookup"><span data-stu-id="8fdb1-173">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="8fdb1-174">Gerenciar associação do MPN e sua empresa (funções não AAD: essas funções gerenciam o negócio da empresa em vez do locatário)</span><span class="sxs-lookup"><span data-stu-id="8fdb1-174">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="8fdb1-175">**Cargo**</span><span class="sxs-lookup"><span data-stu-id="8fdb1-175">**Role**</span></span> | <span data-ttu-id="8fdb1-176">**O que você pode fazer**</span><span class="sxs-lookup"><span data-stu-id="8fdb1-176">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="8fdb1-177">Administrador de parceiros do MPN</span><span class="sxs-lookup"><span data-stu-id="8fdb1-177">MPN partner admin</span></span>|<span data-ttu-id="8fdb1-178">• Exibir, criar e gerenciar solicitações de serviço de parceiro</span><span class="sxs-lookup"><span data-stu-id="8fdb1-178">•    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="8fdb1-179">• Exibir perfis legais, de empresa, de negócios e de MPN</span><span class="sxs-lookup"><span data-stu-id="8fdb1-179">• View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="8fdb1-180">• Exibir detalhes do usuário e seus dados de habilidades</span><span class="sxs-lookup"><span data-stu-id="8fdb1-180">• View user details and their skills data</span></span>
||<span data-ttu-id="8fdb1-181">• Exibir competências</span><span class="sxs-lookup"><span data-stu-id="8fdb1-181">• View competencies</span></span>
||<span data-ttu-id="8fdb1-182">• Exibir e gerenciar benefícios</span><span class="sxs-lookup"><span data-stu-id="8fdb1-182">• View and manage benefits</span></span>
||<span data-ttu-id="8fdb1-183">• Exibir e adquirir ofertas de MPN</span><span class="sxs-lookup"><span data-stu-id="8fdb1-183">• View and purchase MPN offers</span></span>
||<span data-ttu-id="8fdb1-184">• Exibir MPN oferece histórico de pedidos e faturas</span><span class="sxs-lookup"><span data-stu-id="8fdb1-184">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="8fdb1-185">• Exibir dados do indicador de contribuição de parceiro</span><span class="sxs-lookup"><span data-stu-id="8fdb1-185">• View partner contribution indicator data</span></span>
||<span data-ttu-id="8fdb1-186">• Pode funcionar na ferramenta de validação de comprovante</span><span class="sxs-lookup"><span data-stu-id="8fdb1-186">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="8fdb1-187">-Exibir análise de dados do cliente</span><span class="sxs-lookup"><span data-stu-id="8fdb1-187">- View customer data analytics</span></span>
|| <span data-ttu-id="8fdb1-188">Exibir outras funções de usuário na empresa, mas não pode atribuir funções</span><span class="sxs-lookup"><span data-stu-id="8fdb1-188">View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="8fdb1-189">Administrador da conta</span><span class="sxs-lookup"><span data-stu-id="8fdb1-189">Account admin</span></span>| <span data-ttu-id="8fdb1-190">Adicionar locais</span><span class="sxs-lookup"><span data-stu-id="8fdb1-190">Add locations</span></span>
|| <span data-ttu-id="8fdb1-191">Gerenciar perfis relacionados às contas para as quais você é administrador</span><span class="sxs-lookup"><span data-stu-id="8fdb1-191">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="8fdb1-192">• Atribuir funções para usuários no locatário a funções não AAD</span><span class="sxs-lookup"><span data-stu-id="8fdb1-192">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="8fdb1-193">• Registrar locais em programas</span><span class="sxs-lookup"><span data-stu-id="8fdb1-193">• Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="8fdb1-194">Gerenciar referências</span><span class="sxs-lookup"><span data-stu-id="8fdb1-194">Manage referrals</span></span> 

|<span data-ttu-id="8fdb1-195">**Cargo**</span><span class="sxs-lookup"><span data-stu-id="8fdb1-195">**Role**</span></span>|<span data-ttu-id="8fdb1-196">**O que você pode fazer**</span><span class="sxs-lookup"><span data-stu-id="8fdb1-196">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="8fdb1-197">Administrador de referências</span><span class="sxs-lookup"><span data-stu-id="8fdb1-197">Referrals admin</span></span>       |<span data-ttu-id="8fdb1-198">• Exibir, criar e gerenciar perfis de negócios</span><span class="sxs-lookup"><span data-stu-id="8fdb1-198">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="8fdb1-199">• Receber e gerenciar referências</span><span class="sxs-lookup"><span data-stu-id="8fdb1-199">• Receive and manage referrals</span></span>
||<span data-ttu-id="8fdb1-200">• Exibir, criar e gerenciar as referências de venda conjunta</span><span class="sxs-lookup"><span data-stu-id="8fdb1-200">• View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="8fdb1-201">• Exibir, criar e gerenciar solicitações de serviço de parceiro</span><span class="sxs-lookup"><span data-stu-id="8fdb1-201">• View, create, and manage partner service requests</span></span>
|<span data-ttu-id="8fdb1-202">Administrador de perfis de negócios</span><span class="sxs-lookup"><span data-stu-id="8fdb1-202">Business profile admin</span></span>   |<span data-ttu-id="8fdb1-203">• Exibir, criar e gerenciar perfil de negócios</span><span class="sxs-lookup"><span data-stu-id="8fdb1-203">• View, create, and manage business profile</span></span> 
||<span data-ttu-id="8fdb1-204">• Exibir, criar e gerenciar solicitações de serviço de parceiro</span><span class="sxs-lookup"><span data-stu-id="8fdb1-204">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="8fdb1-205">Gerenciar incentivos</span><span class="sxs-lookup"><span data-stu-id="8fdb1-205">Manage incentives</span></span> 

|<span data-ttu-id="8fdb1-206">**Cargo**</span><span class="sxs-lookup"><span data-stu-id="8fdb1-206">**Role**</span></span> | <span data-ttu-id="8fdb1-207">**O que você pode fazer**</span><span class="sxs-lookup"><span data-stu-id="8fdb1-207">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="8fdb1-208">Administrador de incentivos</span><span class="sxs-lookup"><span data-stu-id="8fdb1-208">Incentives admin</span></span>|<span data-ttu-id="8fdb1-209">• Inicia e gerencia incentivos</span><span class="sxs-lookup"><span data-stu-id="8fdb1-209">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="8fdb1-210">• Pode exibir e editar todos os aspectos dos programas de incentivos</span><span class="sxs-lookup"><span data-stu-id="8fdb1-210">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="8fdb1-211">• Pode exibir e editar os detalhes do banco e do imposto</span><span class="sxs-lookup"><span data-stu-id="8fdb1-211">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="8fdb1-212">• Exibir descontos e ganhos de cooperação</span><span class="sxs-lookup"><span data-stu-id="8fdb1-212">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="8fdb1-213">• Suporte ao Access</span><span class="sxs-lookup"><span data-stu-id="8fdb1-213">• Access support</span></span>
||<span data-ttu-id="8fdb1-214">• Testar os pagamentos de incentivos</span><span class="sxs-lookup"><span data-stu-id="8fdb1-214">• Dispute incentives payments</span></span>|
|<span data-ttu-id="8fdb1-215">Usuário de incentivos</span><span class="sxs-lookup"><span data-stu-id="8fdb1-215">Incentives user</span></span>|<span data-ttu-id="8fdb1-216">• Pode exibir programas de incentivos</span><span class="sxs-lookup"><span data-stu-id="8fdb1-216">•  Can view incentives programs</span></span>
||<span data-ttu-id="8fdb1-217">• Pode exibir e iniciar declarações de incentivos</span><span class="sxs-lookup"><span data-stu-id="8fdb1-217">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="8fdb1-218">• Exibir descontos e ganhos de cooperação</span><span class="sxs-lookup"><span data-stu-id="8fdb1-218">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="8fdb1-219">• Suporte ao Access</span><span class="sxs-lookup"><span data-stu-id="8fdb1-219">• Access support</span></span>












