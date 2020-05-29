---
title: Atribuir funções e permissões a usuários
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba quais funções são melhores para os usuários da sua empresa que gerenciam transações comerciais, indicações, incentivos ou associações MPN no Partner Center.
author: LauraBrenner
ms.author: labrenne
keywords: funções, permissões, administrador, agente
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 0858340c6965ac932f0d4694f6f21be89ca5f817
ms.sourcegitcommit: 2a980b50cf177753c15ebfd7770e14cf6d486cf7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2020
ms.locfileid: "83795883"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="c7950-104">Atribuir permissões e funções de usuários para os usuários de uma empresa que precisam trabalhar no Partner Center</span><span class="sxs-lookup"><span data-stu-id="c7950-104">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="c7950-105">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="c7950-105">**Appropriate roles**</span></span>

- <span data-ttu-id="c7950-106">Administrador global</span><span class="sxs-lookup"><span data-stu-id="c7950-106">Global admin</span></span>
- <span data-ttu-id="c7950-107">Administrador de usuários</span><span class="sxs-lookup"><span data-stu-id="c7950-107">User admin</span></span>
- <span data-ttu-id="c7950-108">Administrador de parceiros do MPN</span><span class="sxs-lookup"><span data-stu-id="c7950-108">MPN partner admin</span></span>

<span data-ttu-id="c7950-109">Você configurou seu perfil de parceiro, incluindo a razão social, o endereço, os detalhes de suporte, as isenções de imposto sobre arquivos, as informações bancárias e o contato principal da empresa.</span><span class="sxs-lookup"><span data-stu-id="c7950-109">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="c7950-110">Próxima etapa: Configure as senhas e funções dos seus usuários para que eles possam começar a trabalhar no Partner Center com você.</span><span class="sxs-lookup"><span data-stu-id="c7950-110">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="c7950-111">Configurar seus funcionários para trabalhar no Partner Center</span><span class="sxs-lookup"><span data-stu-id="c7950-111">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="c7950-112">Você determinará os tipos de acesso que os usuários terão ao Partner Center por meio das funções e permissões a eles atribuídas.</span><span class="sxs-lookup"><span data-stu-id="c7950-112">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="c7950-113">As funções estão relacionadas aos programas com os quais a sua empresa está envolvida.</span><span class="sxs-lookup"><span data-stu-id="c7950-113">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="c7950-114">Por exemplo, se a sua empresa for um CSP (Provedor de Soluções na Nuvem), você não apenas terá as funções de gerenciamento de locatário padrão do Azure AD, como o administrador global, mas também precisará de funções específicas para o programa CSP.</span><span class="sxs-lookup"><span data-stu-id="c7950-114">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="c7950-115">Cada programa tem funções específicas para ele.</span><span class="sxs-lookup"><span data-stu-id="c7950-115">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="c7950-116">As funções de locatário do Azure Active Directory (AAD) incluem administrador global, administrador de usuários e funções de CSP.</span><span class="sxs-lookup"><span data-stu-id="c7950-116">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="c7950-117">As funções não pertencentes ao AAD são aquelas que não gerenciam o locatário e incluem administrador do MPN, administrador de perfil de negócios, administrador de indicações, administrador de incentivos e usuário de incentivos.</span><span class="sxs-lookup"><span data-stu-id="c7950-117">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="c7950-118">Gerenciar transações comerciais no Partner Center (funções Azure AD e CSP)</span><span class="sxs-lookup"><span data-stu-id="c7950-118">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="c7950-119">**Função**</span><span class="sxs-lookup"><span data-stu-id="c7950-119">**Role**</span></span>|<span data-ttu-id="c7950-120">**O que eles podem fazer**</span><span class="sxs-lookup"><span data-stu-id="c7950-120">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="c7950-121">Administrador global</span><span class="sxs-lookup"><span data-stu-id="c7950-121">Global admin</span></span>|<span data-ttu-id="c7950-122">\*    Pode acessar todas as contas/os serviços da Microsoft com todos os privilégios</span><span class="sxs-lookup"><span data-stu-id="c7950-122">\*    Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="c7950-123">\*    Criar tíquetes de suporte para o Partner Center</span><span class="sxs-lookup"><span data-stu-id="c7950-123">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="c7950-124">\*    Ver contratos, listas de preços e ofertas</span><span class="sxs-lookup"><span data-stu-id="c7950-124">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="c7950-125">\*    Ver, criar e gerenciar usuários parceiros</span><span class="sxs-lookup"><span data-stu-id="c7950-125">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="c7950-126">• Exibir, criar e gerenciar a cobrança, as faturas e os arquivos reconhecimento</span><span class="sxs-lookup"><span data-stu-id="c7950-126">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="c7950-127">Administrador de gerenciamento de usuário</span><span class="sxs-lookup"><span data-stu-id="c7950-127">User management admin</span></span>   | <span data-ttu-id="c7950-128">\*    Ver, criar e gerenciar usuários</span><span class="sxs-lookup"><span data-stu-id="c7950-128">\*    View, create, and manage users</span></span>
||<span data-ttu-id="c7950-129">\*    Ver todos os perfis de parceiros</span><span class="sxs-lookup"><span data-stu-id="c7950-129">\*    View all partner profiles</span></span>
||<span data-ttu-id="c7950-130">\*    Ver, criar e gerenciar usuários parceiros</span><span class="sxs-lookup"><span data-stu-id="c7950-130">\*    View, create, and manage partner users</span></span>  |
|<span data-ttu-id="c7950-131">Administrador de cobrança</span><span class="sxs-lookup"><span data-stu-id="c7950-131">Billing admin</span></span> | <span data-ttu-id="c7950-132">– Exibir, criar e gerenciar a cobrança, as faturas e os arquivos reconhecimento</span><span class="sxs-lookup"><span data-stu-id="c7950-132">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="c7950-133">Usuário padrão</span><span class="sxs-lookup"><span data-stu-id="c7950-133">Default user</span></span>|  <span data-ttu-id="c7950-134">Exibir meu perfil</span><span class="sxs-lookup"><span data-stu-id="c7950-134">View My profile</span></span>   |
|<span data-ttu-id="c7950-135">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="c7950-135">Admin agent</span></span> | <span data-ttu-id="c7950-136">\*    Gerenciamento de clientes</span><span class="sxs-lookup"><span data-stu-id="c7950-136">\*    Customer management</span></span>
||<span data-ttu-id="c7950-137">\*    Adicionar lista de dispositivos ao Partner Center</span><span class="sxs-lookup"><span data-stu-id="c7950-137">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="c7950-138">\*    Criar e aplicar perfis aos dispositivos</span><span class="sxs-lookup"><span data-stu-id="c7950-138">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="c7950-139">\*    Gerenciamento de assinaturas</span><span class="sxs-lookup"><span data-stu-id="c7950-139">\*    Subscription management</span></span>
||<span data-ttu-id="c7950-140">\*    Solicitações de integridade e de serviços para os clientes</span><span class="sxs-lookup"><span data-stu-id="c7950-140">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="c7950-141">\*    Solicitar privilégios de administrador delegado</span><span class="sxs-lookup"><span data-stu-id="c7950-141">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="c7950-142">\*    Ver preços e ofertas</span><span class="sxs-lookup"><span data-stu-id="c7950-142">\*    View pricing and offers</span></span>
||<span data-ttu-id="c7950-143">\*    Cobrança</span><span class="sxs-lookup"><span data-stu-id="c7950-143">\*    Billing</span></span>
||<span data-ttu-id="c7950-144">\*    Administrar em nome de um cliente</span><span class="sxs-lookup"><span data-stu-id="c7950-144">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="c7950-145">\*    Registrar um revendedor com valor agregado</span><span class="sxs-lookup"><span data-stu-id="c7950-145">\*    Register a value added reseller</span></span>|
|<span data-ttu-id="c7950-146">Agente de vendas</span><span class="sxs-lookup"><span data-stu-id="c7950-146">Sales agent</span></span> | <span data-ttu-id="c7950-147">\*    Gerenciamento de clientes</span><span class="sxs-lookup"><span data-stu-id="c7950-147">\*    Customer management</span></span>
||<span data-ttu-id="c7950-148">\*    Adicionar lista de dispositivos ao Partner Center</span><span class="sxs-lookup"><span data-stu-id="c7950-148">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="c7950-149">\*    Gerenciamento de assinaturas</span><span class="sxs-lookup"><span data-stu-id="c7950-149">\*    Subscription management</span></span>
||<span data-ttu-id="c7950-150">\*    Ver tíquetes de suporte</span><span class="sxs-lookup"><span data-stu-id="c7950-150">\*    View support tickets</span></span>
||<span data-ttu-id="c7950-151">\*    Solicitar um relacionamento com um cliente</span><span class="sxs-lookup"><span data-stu-id="c7950-151">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="c7950-152">\*    Gerenciar clientes potenciais</span><span class="sxs-lookup"><span data-stu-id="c7950-152">\*    Manage customer leads</span></span>
||<span data-ttu-id="c7950-153">\*    Ver o contrato do cliente</span><span class="sxs-lookup"><span data-stu-id="c7950-153">\*    View the customer agreement</span></span>
||<span data-ttu-id="c7950-154">\*    Registrar um revendedor com valor agregado</span><span class="sxs-lookup"><span data-stu-id="c7950-154">\*    Register a value-added reseller</span></span>|
|<span data-ttu-id="c7950-155">Agente de suporte técnico</span><span class="sxs-lookup"><span data-stu-id="c7950-155">Helpdesk agent</span></span>| <span data-ttu-id="c7950-156">\*    Pesquisar e ver um cliente</span><span class="sxs-lookup"><span data-stu-id="c7950-156">\*    Search for and view a customer</span></span>
||<span data-ttu-id="c7950-157">\*    Editar detalhes do cliente</span><span class="sxs-lookup"><span data-stu-id="c7950-157">\*    Edit customer details</span></span>
||<span data-ttu-id="c7950-158">\*    Ajudar a resolver problemas dos clientes com o gerenciamento de cobrança ou assinaturas</span><span class="sxs-lookup"><span data-stu-id="c7950-158">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="c7950-159">\*    Solicitar suporte em nome dos clientes</span><span class="sxs-lookup"><span data-stu-id="c7950-159">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="c7950-160">\*    Gerenciar problemas de assinaturas e cobrança em nome dos clientes</span><span class="sxs-lookup"><span data-stu-id="c7950-160">\*    Manage subscriptions and billing issues on behalf of customers</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="c7950-161">CPV (Fornecedor de Painel de Controle).</span><span class="sxs-lookup"><span data-stu-id="c7950-161">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="c7950-162">(Função CSP e função não pertencente ao AAD)</span><span class="sxs-lookup"><span data-stu-id="c7950-162">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="c7950-163">Os CPVs desenvolvem aplicativos para uso por parceiros CSP (Provedor de Soluções na Nuvem) a fim de permitir que eles integrem seus sistemas com as APIs do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="c7950-163">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="c7950-164">**Função**</span><span class="sxs-lookup"><span data-stu-id="c7950-164">**Role**</span></span>   |<span data-ttu-id="c7950-165">**O que você pode fazer**</span><span class="sxs-lookup"><span data-stu-id="c7950-165">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="c7950-166">Administrador global</span><span class="sxs-lookup"><span data-stu-id="c7950-166">Global admin</span></span>| <span data-ttu-id="c7950-167">Exibir e gerenciar seu perfil de CPV</span><span class="sxs-lookup"><span data-stu-id="c7950-167">View and manage your CPV profile</span></span>|
||<span data-ttu-id="c7950-168">Exibir e gerenciar todos os seus usuários que precisam de acesso aos recursos de CPV</span><span class="sxs-lookup"><span data-stu-id="c7950-168">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="c7950-169">Usuário convidado (deve ser adicionado ao locatário do AAD)</span><span class="sxs-lookup"><span data-stu-id="c7950-169">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="c7950-170">**Usuário convidado**</span><span class="sxs-lookup"><span data-stu-id="c7950-170">**Guest user**</span></span>   | <span data-ttu-id="c7950-171">**Funções**</span><span class="sxs-lookup"><span data-stu-id="c7950-171">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="c7950-172">Administrador de parceiros do MPN</span><span class="sxs-lookup"><span data-stu-id="c7950-172">MPN partner admin</span></span>|
||<span data-ttu-id="c7950-173">Administrador de contas</span><span class="sxs-lookup"><span data-stu-id="c7950-173">Accounts admin</span></span>|
||<span data-ttu-id="c7950-174">Administrador de incentivos</span><span class="sxs-lookup"><span data-stu-id="c7950-174">Incentives admin</span></span>|
||<span data-ttu-id="c7950-175">Administrador de perfis de negócios</span><span class="sxs-lookup"><span data-stu-id="c7950-175">Business profile admin</span></span>|
||<span data-ttu-id="c7950-176">Administrador de indicações</span><span class="sxs-lookup"><span data-stu-id="c7950-176">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="c7950-177">Gerenciar associação do MPN e sua empresa (funções não pertencentes ao AAD: essas funções gerenciam os negócios da empresa em vez do locatário)</span><span class="sxs-lookup"><span data-stu-id="c7950-177">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="c7950-178">**Função**</span><span class="sxs-lookup"><span data-stu-id="c7950-178">**Role**</span></span> | <span data-ttu-id="c7950-179">**O que você pode fazer**</span><span class="sxs-lookup"><span data-stu-id="c7950-179">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="c7950-180">Administrador de parceiros do MPN</span><span class="sxs-lookup"><span data-stu-id="c7950-180">MPN partner admin</span></span>|<span data-ttu-id="c7950-181">\*    Ver, criar e gerenciar solicitações de serviço de parceiros</span><span class="sxs-lookup"><span data-stu-id="c7950-181">\*    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="c7950-182">\*    Ver perfis jurídico, empresarial, de negócios e do MPN</span><span class="sxs-lookup"><span data-stu-id="c7950-182">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="c7950-183">\*    Ver detalhes do usuário e seus dados de habilidades</span><span class="sxs-lookup"><span data-stu-id="c7950-183">\*    View user details and their skills data</span></span>
||<span data-ttu-id="c7950-184">\*    Ver competências</span><span class="sxs-lookup"><span data-stu-id="c7950-184">\*    View competencies</span></span>
||<span data-ttu-id="c7950-185">\*    Ver e gerenciar benefícios</span><span class="sxs-lookup"><span data-stu-id="c7950-185">\*    View and manage benefits</span></span>
||<span data-ttu-id="c7950-186">\*    Ver e comprar ofertas do MPN</span><span class="sxs-lookup"><span data-stu-id="c7950-186">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="c7950-187">\*    Ver histórico de pedidos de ofertas e faturas do MPN</span><span class="sxs-lookup"><span data-stu-id="c7950-187">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="c7950-188">\*    Ver dados do indicador de contribuição de parceiros</span><span class="sxs-lookup"><span data-stu-id="c7950-188">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="c7950-189">\*    Pode funcionar na ferramenta de validação de comprovantes</span><span class="sxs-lookup"><span data-stu-id="c7950-189">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="c7950-190">\*    Ver análises de dados do cliente</span><span class="sxs-lookup"><span data-stu-id="c7950-190">\*    View customer data analytics</span></span>
||<span data-ttu-id="c7950-191">\*    Ver outras funções de usuário dentro da empresa, mas não atribuir funções</span><span class="sxs-lookup"><span data-stu-id="c7950-191">\*    View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="c7950-192">Administrador de conta</span><span class="sxs-lookup"><span data-stu-id="c7950-192">Account admin</span></span>| <span data-ttu-id="c7950-193">Adicionar locais</span><span class="sxs-lookup"><span data-stu-id="c7950-193">Add locations</span></span>
|| <span data-ttu-id="c7950-194">Gerenciar perfis relacionados às contas para as quais você é administrador</span><span class="sxs-lookup"><span data-stu-id="c7950-194">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="c7950-195">\*    Atribuir funções aos usuários do locatário para funções não pertencentes ao AAD</span><span class="sxs-lookup"><span data-stu-id="c7950-195">\*    Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="c7950-196">\*    Registrar locais em programas</span><span class="sxs-lookup"><span data-stu-id="c7950-196">\*    Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="c7950-197">Gerenciar indicações</span><span class="sxs-lookup"><span data-stu-id="c7950-197">Manage referrals</span></span> 

|<span data-ttu-id="c7950-198">**Função**</span><span class="sxs-lookup"><span data-stu-id="c7950-198">**Role**</span></span>|<span data-ttu-id="c7950-199">**O que você pode fazer**</span><span class="sxs-lookup"><span data-stu-id="c7950-199">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="c7950-200">Administrador de indicações</span><span class="sxs-lookup"><span data-stu-id="c7950-200">Referrals admin</span></span>       |<span data-ttu-id="c7950-201">\* Ver, criar e gerenciar perfis de negócios</span><span class="sxs-lookup"><span data-stu-id="c7950-201">\*    View, create, and manage business profiles</span></span>
||<span data-ttu-id="c7950-202">\*    Receber e gerenciar indicações</span><span class="sxs-lookup"><span data-stu-id="c7950-202">\*    Receive and manage referrals</span></span>
||<span data-ttu-id="c7950-203">\* Ver, criar e gerenciar as indicações de venda conjunta</span><span class="sxs-lookup"><span data-stu-id="c7950-203">\* View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="c7950-204">\*    Ver, criar e gerenciar solicitações de serviço de parceiros</span><span class="sxs-lookup"><span data-stu-id="c7950-204">\*    View, create, and manage partner service requests</span></span>
|<span data-ttu-id="c7950-205">Administrador de perfis de negócios</span><span class="sxs-lookup"><span data-stu-id="c7950-205">Business profile admin</span></span>   |<span data-ttu-id="c7950-206">\* Ver, criar e gerenciar perfis de negócios</span><span class="sxs-lookup"><span data-stu-id="c7950-206">\* View, create, and manage business profile</span></span> 
||<span data-ttu-id="c7950-207">\*    Ver, criar e gerenciar solicitações de serviço de parceiros</span><span class="sxs-lookup"><span data-stu-id="c7950-207">\*    View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="c7950-208">Gerenciar incentivos</span><span class="sxs-lookup"><span data-stu-id="c7950-208">Manage incentives</span></span> 

|<span data-ttu-id="c7950-209">**Função**</span><span class="sxs-lookup"><span data-stu-id="c7950-209">**Role**</span></span> | <span data-ttu-id="c7950-210">**O que você pode fazer**</span><span class="sxs-lookup"><span data-stu-id="c7950-210">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="c7950-211">Administrador de incentivos</span><span class="sxs-lookup"><span data-stu-id="c7950-211">Incentives admin</span></span>|<span data-ttu-id="c7950-212">\*    Iniciar e gerenciar incentivos</span><span class="sxs-lookup"><span data-stu-id="c7950-212">\*    Initiates and manages incentives</span></span> 
||<span data-ttu-id="c7950-213">\*    Ver e editar todos os aspectos dos programas de incentivos</span><span class="sxs-lookup"><span data-stu-id="c7950-213">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="c7950-214">\*    Ver e editar detalhes bancários e fiscais</span><span class="sxs-lookup"><span data-stu-id="c7950-214">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="c7950-215">\*    Ver lucros de reembolso e de cooperação</span><span class="sxs-lookup"><span data-stu-id="c7950-215">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="c7950-216">\*    Acessar suporte</span><span class="sxs-lookup"><span data-stu-id="c7950-216">\*    Access support</span></span>
||<span data-ttu-id="c7950-217">\*    Disputar pagamentos de incentivos</span><span class="sxs-lookup"><span data-stu-id="c7950-217">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="c7950-218">Usuário de incentivos</span><span class="sxs-lookup"><span data-stu-id="c7950-218">Incentives user</span></span>|<span data-ttu-id="c7950-219">\*    Ver programas de incentivos</span><span class="sxs-lookup"><span data-stu-id="c7950-219">\*    Can view incentives programs</span></span>
||<span data-ttu-id="c7950-220">\*    Ver e iniciar reivindicações de incentivos</span><span class="sxs-lookup"><span data-stu-id="c7950-220">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="c7950-221">\*    Ver lucros de reembolso e de cooperação</span><span class="sxs-lookup"><span data-stu-id="c7950-221">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="c7950-222">\*    Acessar suporte</span><span class="sxs-lookup"><span data-stu-id="c7950-222">\*    Access support</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="c7950-223">Exibir dados de Insights do Partner Center</span><span class="sxs-lookup"><span data-stu-id="c7950-223">View Partner Center Insights data</span></span>

|<span data-ttu-id="c7950-224">**Função**</span><span class="sxs-lookup"><span data-stu-id="c7950-224">**Role**</span></span> | <span data-ttu-id="c7950-225">**O que você pode fazer**</span><span class="sxs-lookup"><span data-stu-id="c7950-225">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="c7950-226">Visualizador de relatórios executivos</span><span class="sxs-lookup"><span data-stu-id="c7950-226">Executive report viewer</span></span>|<span data-ttu-id="c7950-227">Acesso a todos os conjuntos de dados de relatórios</span><span class="sxs-lookup"><span data-stu-id="c7950-227">Access to all reporting datasets</span></span>|
|<span data-ttu-id="c7950-228">Visualizador de relatórios</span><span class="sxs-lookup"><span data-stu-id="c7950-228">Report viewer</span></span>|<span data-ttu-id="c7950-229">Acesso a relatórios de dados com exceção de receita e dados pessoais de clientes e funcionários</span><span class="sxs-lookup"><span data-stu-id="c7950-229">Access to data reports with exception of revenue and customer and employee personal data</span></span>|












                                    