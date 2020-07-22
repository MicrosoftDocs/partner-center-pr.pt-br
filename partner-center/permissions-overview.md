---
title: Atribuir funções e permissões a usuários
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba quais funções são melhores para os usuários da sua empresa que gerenciam transações comerciais, indicações, incentivos ou associações MPN no Partner Center.
author: hemas
ms.author: hemas
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: c0e7aecd7d56e1919c7f142312a9090b8ff40bd3
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2020
ms.locfileid: "86434315"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="1c03d-103">Atribuir permissões e funções de usuários para os usuários de uma empresa que precisam trabalhar no Partner Center</span><span class="sxs-lookup"><span data-stu-id="1c03d-103">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="1c03d-104">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="1c03d-104">**Appropriate roles**</span></span>

- <span data-ttu-id="1c03d-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="1c03d-105">Global admin</span></span>
- <span data-ttu-id="1c03d-106">Administrador de usuários</span><span class="sxs-lookup"><span data-stu-id="1c03d-106">User admin</span></span>
- <span data-ttu-id="1c03d-107">Administrador de parceiros do MPN</span><span class="sxs-lookup"><span data-stu-id="1c03d-107">MPN partner admin</span></span>

<span data-ttu-id="1c03d-108">Você configurou seu perfil de parceiro, incluindo a razão social, o endereço, os detalhes de suporte, as isenções de imposto sobre arquivos, as informações bancárias e o contato principal da empresa.</span><span class="sxs-lookup"><span data-stu-id="1c03d-108">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="1c03d-109">Próxima etapa: Configure as senhas e funções dos seus usuários para que eles possam começar a trabalhar no Partner Center com você.</span><span class="sxs-lookup"><span data-stu-id="1c03d-109">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="1c03d-110">Configurar seus funcionários para trabalhar no Partner Center</span><span class="sxs-lookup"><span data-stu-id="1c03d-110">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="1c03d-111">Você determinará os tipos de acesso que os usuários terão ao Partner Center por meio das funções e permissões a eles atribuídas.</span><span class="sxs-lookup"><span data-stu-id="1c03d-111">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="1c03d-112">As funções estão relacionadas aos programas com os quais a sua empresa está envolvida.</span><span class="sxs-lookup"><span data-stu-id="1c03d-112">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="1c03d-113">Por exemplo, se a sua empresa for um CSP (Provedor de Soluções na Nuvem), você não apenas terá as funções de gerenciamento de locatário padrão do Azure AD, como o administrador global, mas também precisará de funções específicas para o programa CSP.</span><span class="sxs-lookup"><span data-stu-id="1c03d-113">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="1c03d-114">Cada programa tem funções específicas para ele.</span><span class="sxs-lookup"><span data-stu-id="1c03d-114">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="1c03d-115">As funções de locatário do Azure Active Directory (AAD) incluem administrador global, administrador de usuários e funções de CSP.</span><span class="sxs-lookup"><span data-stu-id="1c03d-115">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="1c03d-116">As funções não pertencentes ao AAD são aquelas que não gerenciam o locatário e incluem administrador do MPN, administrador de perfil de negócios, administrador de indicações, administrador de incentivos e usuário de incentivos.</span><span class="sxs-lookup"><span data-stu-id="1c03d-116">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="1c03d-117">Gerenciar transações comerciais no Partner Center (funções Azure AD e CSP)</span><span class="sxs-lookup"><span data-stu-id="1c03d-117">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="1c03d-118">**Função**</span><span class="sxs-lookup"><span data-stu-id="1c03d-118">**Role**</span></span>|<span data-ttu-id="1c03d-119">**O que eles podem fazer**</span><span class="sxs-lookup"><span data-stu-id="1c03d-119">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="1c03d-120">Administrador global</span><span class="sxs-lookup"><span data-stu-id="1c03d-120">Global admin</span></span>|<span data-ttu-id="1c03d-121">\*    Pode acessar todas as contas/os serviços da Microsoft com todos os privilégios</span><span class="sxs-lookup"><span data-stu-id="1c03d-121">\*    Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="1c03d-122">\*    Criar tíquetes de suporte para o Partner Center</span><span class="sxs-lookup"><span data-stu-id="1c03d-122">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="1c03d-123">\*    Ver contratos, listas de preços e ofertas</span><span class="sxs-lookup"><span data-stu-id="1c03d-123">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="1c03d-124">\*    Ver, criar e gerenciar usuários parceiros</span><span class="sxs-lookup"><span data-stu-id="1c03d-124">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="1c03d-125">• Exibir, criar e gerenciar a cobrança, as faturas e os arquivos reconhecimento</span><span class="sxs-lookup"><span data-stu-id="1c03d-125">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="1c03d-126">Administrador de gerenciamento de usuário</span><span class="sxs-lookup"><span data-stu-id="1c03d-126">User management admin</span></span>   | <span data-ttu-id="1c03d-127">\*    Ver, criar e gerenciar usuários</span><span class="sxs-lookup"><span data-stu-id="1c03d-127">\*    View, create, and manage users</span></span>
||<span data-ttu-id="1c03d-128">\*    Ver todos os perfis de parceiros</span><span class="sxs-lookup"><span data-stu-id="1c03d-128">\*    View all partner profiles</span></span>
||<span data-ttu-id="1c03d-129">\*    Ver, criar e gerenciar usuários parceiros</span><span class="sxs-lookup"><span data-stu-id="1c03d-129">\*    View, create, and manage partner users</span></span>  |
|<span data-ttu-id="1c03d-130">Administrador de cobrança</span><span class="sxs-lookup"><span data-stu-id="1c03d-130">Billing admin</span></span> | <span data-ttu-id="1c03d-131">– Exibir, criar e gerenciar a cobrança, as faturas e os arquivos reconhecimento</span><span class="sxs-lookup"><span data-stu-id="1c03d-131">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="1c03d-132">Usuário padrão</span><span class="sxs-lookup"><span data-stu-id="1c03d-132">Default user</span></span>|  <span data-ttu-id="1c03d-133">Exibir meu perfil</span><span class="sxs-lookup"><span data-stu-id="1c03d-133">View My profile</span></span>   |
|<span data-ttu-id="1c03d-134">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="1c03d-134">Admin agent</span></span> | <span data-ttu-id="1c03d-135">\*    Gerenciamento de clientes</span><span class="sxs-lookup"><span data-stu-id="1c03d-135">\*    Customer management</span></span>
||<span data-ttu-id="1c03d-136">\*    Adicionar lista de dispositivos ao Partner Center</span><span class="sxs-lookup"><span data-stu-id="1c03d-136">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="1c03d-137">\*    Criar e aplicar perfis aos dispositivos</span><span class="sxs-lookup"><span data-stu-id="1c03d-137">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="1c03d-138">\*    Gerenciamento de assinaturas</span><span class="sxs-lookup"><span data-stu-id="1c03d-138">\*    Subscription management</span></span>
||<span data-ttu-id="1c03d-139">\*    Solicitações de integridade e de serviços para os clientes</span><span class="sxs-lookup"><span data-stu-id="1c03d-139">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="1c03d-140">\*    Solicitar privilégios de administrador delegado</span><span class="sxs-lookup"><span data-stu-id="1c03d-140">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="1c03d-141">\*    Ver preços e ofertas</span><span class="sxs-lookup"><span data-stu-id="1c03d-141">\*    View pricing and offers</span></span>
||<span data-ttu-id="1c03d-142">\*    Cobrança</span><span class="sxs-lookup"><span data-stu-id="1c03d-142">\*    Billing</span></span>
||<span data-ttu-id="1c03d-143">\*    Administrar em nome de um cliente</span><span class="sxs-lookup"><span data-stu-id="1c03d-143">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="1c03d-144">\*    Registrar um revendedor com valor agregado</span><span class="sxs-lookup"><span data-stu-id="1c03d-144">\*    Register a value added reseller</span></span>|
|<span data-ttu-id="1c03d-145">Agente de vendas</span><span class="sxs-lookup"><span data-stu-id="1c03d-145">Sales agent</span></span> | <span data-ttu-id="1c03d-146">\*    Gerenciamento de clientes</span><span class="sxs-lookup"><span data-stu-id="1c03d-146">\*    Customer management</span></span>
||<span data-ttu-id="1c03d-147">\*    Adicionar lista de dispositivos ao Partner Center</span><span class="sxs-lookup"><span data-stu-id="1c03d-147">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="1c03d-148">\*    Gerenciamento de assinaturas</span><span class="sxs-lookup"><span data-stu-id="1c03d-148">\*    Subscription management</span></span>
||<span data-ttu-id="1c03d-149">\*    Ver tíquetes de suporte</span><span class="sxs-lookup"><span data-stu-id="1c03d-149">\*    View support tickets</span></span>
||<span data-ttu-id="1c03d-150">\*    Solicitar um relacionamento com um cliente</span><span class="sxs-lookup"><span data-stu-id="1c03d-150">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="1c03d-151">\*    Gerenciar clientes potenciais</span><span class="sxs-lookup"><span data-stu-id="1c03d-151">\*    Manage customer leads</span></span>
||<span data-ttu-id="1c03d-152">\*    Ver o contrato do cliente</span><span class="sxs-lookup"><span data-stu-id="1c03d-152">\*    View the customer agreement</span></span>
||<span data-ttu-id="1c03d-153">\*    Registrar um revendedor com valor agregado</span><span class="sxs-lookup"><span data-stu-id="1c03d-153">\*    Register a value-added reseller</span></span>|
|<span data-ttu-id="1c03d-154">Agente de suporte técnico</span><span class="sxs-lookup"><span data-stu-id="1c03d-154">Helpdesk agent</span></span>| <span data-ttu-id="1c03d-155">\*    Pesquisar e ver um cliente</span><span class="sxs-lookup"><span data-stu-id="1c03d-155">\*    Search for and view a customer</span></span>
||<span data-ttu-id="1c03d-156">\*    Editar detalhes do cliente</span><span class="sxs-lookup"><span data-stu-id="1c03d-156">\*    Edit customer details</span></span>
||<span data-ttu-id="1c03d-157">\*    Ajudar a resolver problemas dos clientes com o gerenciamento de cobrança ou assinaturas</span><span class="sxs-lookup"><span data-stu-id="1c03d-157">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="1c03d-158">\*    Solicitar suporte em nome dos clientes</span><span class="sxs-lookup"><span data-stu-id="1c03d-158">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="1c03d-159">\*    Gerenciar problemas de assinaturas e cobrança em nome dos clientes</span><span class="sxs-lookup"><span data-stu-id="1c03d-159">\*    Manage subscriptions and billing issues on behalf of customers</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="1c03d-160">CPV (Fornecedor de Painel de Controle).</span><span class="sxs-lookup"><span data-stu-id="1c03d-160">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="1c03d-161">(Função CSP e função não pertencente ao AAD)</span><span class="sxs-lookup"><span data-stu-id="1c03d-161">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="1c03d-162">Os CPVs desenvolvem aplicativos para uso por parceiros CSP (Provedor de Soluções na Nuvem) a fim de permitir que eles integrem seus sistemas com as APIs do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="1c03d-162">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="1c03d-163">**Função**</span><span class="sxs-lookup"><span data-stu-id="1c03d-163">**Role**</span></span>   |<span data-ttu-id="1c03d-164">**O que você pode fazer**</span><span class="sxs-lookup"><span data-stu-id="1c03d-164">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="1c03d-165">Administrador global</span><span class="sxs-lookup"><span data-stu-id="1c03d-165">Global admin</span></span>| <span data-ttu-id="1c03d-166">Exibir e gerenciar seu perfil de CPV</span><span class="sxs-lookup"><span data-stu-id="1c03d-166">View and manage your CPV profile</span></span>|
||<span data-ttu-id="1c03d-167">Exibir e gerenciar todos os seus usuários que precisam de acesso aos recursos de CPV</span><span class="sxs-lookup"><span data-stu-id="1c03d-167">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="1c03d-168">Usuário convidado (deve ser adicionado ao locatário do AAD)</span><span class="sxs-lookup"><span data-stu-id="1c03d-168">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="1c03d-169">**Usuário convidado**</span><span class="sxs-lookup"><span data-stu-id="1c03d-169">**Guest user**</span></span>   | <span data-ttu-id="1c03d-170">**Funções**</span><span class="sxs-lookup"><span data-stu-id="1c03d-170">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="1c03d-171">Administrador de parceiros do MPN</span><span class="sxs-lookup"><span data-stu-id="1c03d-171">MPN partner admin</span></span>|
||<span data-ttu-id="1c03d-172">Administrador de contas</span><span class="sxs-lookup"><span data-stu-id="1c03d-172">Accounts admin</span></span>|
||<span data-ttu-id="1c03d-173">Administrador de incentivos</span><span class="sxs-lookup"><span data-stu-id="1c03d-173">Incentives admin</span></span>|
||<span data-ttu-id="1c03d-174">Administrador de perfis de negócios</span><span class="sxs-lookup"><span data-stu-id="1c03d-174">Business profile admin</span></span>|
||<span data-ttu-id="1c03d-175">Administrador de indicações</span><span class="sxs-lookup"><span data-stu-id="1c03d-175">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="1c03d-176">Gerenciar associação do MPN e sua empresa (funções não pertencentes ao AAD: essas funções gerenciam os negócios da empresa em vez do locatário)</span><span class="sxs-lookup"><span data-stu-id="1c03d-176">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="1c03d-177">**Função**</span><span class="sxs-lookup"><span data-stu-id="1c03d-177">**Role**</span></span> | <span data-ttu-id="1c03d-178">**O que você pode fazer**</span><span class="sxs-lookup"><span data-stu-id="1c03d-178">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="1c03d-179">Administrador de parceiros do MPN</span><span class="sxs-lookup"><span data-stu-id="1c03d-179">MPN partner admin</span></span>|<span data-ttu-id="1c03d-180">\*    Ver, criar e gerenciar solicitações de serviço de parceiros</span><span class="sxs-lookup"><span data-stu-id="1c03d-180">\*    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="1c03d-181">\*    Ver perfis jurídico, empresarial, de negócios e do MPN</span><span class="sxs-lookup"><span data-stu-id="1c03d-181">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="1c03d-182">\*    Ver detalhes do usuário e seus dados de habilidades</span><span class="sxs-lookup"><span data-stu-id="1c03d-182">\*    View user details and their skills data</span></span>
||<span data-ttu-id="1c03d-183">\*    Ver competências</span><span class="sxs-lookup"><span data-stu-id="1c03d-183">\*    View competencies</span></span>
||<span data-ttu-id="1c03d-184">\*    Ver e gerenciar benefícios</span><span class="sxs-lookup"><span data-stu-id="1c03d-184">\*    View and manage benefits</span></span>
||<span data-ttu-id="1c03d-185">\*    Ver e comprar ofertas do MPN</span><span class="sxs-lookup"><span data-stu-id="1c03d-185">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="1c03d-186">\*    Ver histórico de pedidos de ofertas e faturas do MPN</span><span class="sxs-lookup"><span data-stu-id="1c03d-186">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="1c03d-187">\*    Ver dados do indicador de contribuição de parceiros</span><span class="sxs-lookup"><span data-stu-id="1c03d-187">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="1c03d-188">\*    Pode funcionar na ferramenta de validação de comprovantes</span><span class="sxs-lookup"><span data-stu-id="1c03d-188">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="1c03d-189">\*    Ver análises de dados do cliente</span><span class="sxs-lookup"><span data-stu-id="1c03d-189">\*    View customer data analytics</span></span>
||<span data-ttu-id="1c03d-190">\*    Ver outras funções de usuário dentro da empresa, mas não atribuir funções</span><span class="sxs-lookup"><span data-stu-id="1c03d-190">\*    View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="1c03d-191">Administrador de conta</span><span class="sxs-lookup"><span data-stu-id="1c03d-191">Account admin</span></span>| <span data-ttu-id="1c03d-192">Adicionar locais</span><span class="sxs-lookup"><span data-stu-id="1c03d-192">Add locations</span></span>
|| <span data-ttu-id="1c03d-193">Gerenciar perfis relacionados às contas para as quais você é administrador</span><span class="sxs-lookup"><span data-stu-id="1c03d-193">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="1c03d-194">\*    Atribuir funções aos usuários do locatário para funções não pertencentes ao AAD</span><span class="sxs-lookup"><span data-stu-id="1c03d-194">\*    Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="1c03d-195">\*    Registrar locais em programas</span><span class="sxs-lookup"><span data-stu-id="1c03d-195">\*    Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="1c03d-196">Gerenciar indicações</span><span class="sxs-lookup"><span data-stu-id="1c03d-196">Manage referrals</span></span> 

|<span data-ttu-id="1c03d-197">**Função**</span><span class="sxs-lookup"><span data-stu-id="1c03d-197">**Role**</span></span>|<span data-ttu-id="1c03d-198">**O que você pode fazer**</span><span class="sxs-lookup"><span data-stu-id="1c03d-198">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="1c03d-199">Administrador de indicações</span><span class="sxs-lookup"><span data-stu-id="1c03d-199">Referrals admin</span></span>       |<span data-ttu-id="1c03d-200">\* Ver, criar e gerenciar perfis de negócios</span><span class="sxs-lookup"><span data-stu-id="1c03d-200">\*    View, create, and manage business profiles</span></span>
||<span data-ttu-id="1c03d-201">\*    Receber e gerenciar indicações</span><span class="sxs-lookup"><span data-stu-id="1c03d-201">\*    Receive and manage referrals</span></span>
||<span data-ttu-id="1c03d-202">\* Ver, criar e gerenciar as indicações de venda conjunta</span><span class="sxs-lookup"><span data-stu-id="1c03d-202">\* View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="1c03d-203">\*    Ver, criar e gerenciar solicitações de serviço de parceiros</span><span class="sxs-lookup"><span data-stu-id="1c03d-203">\*    View, create, and manage partner service requests</span></span>
|<span data-ttu-id="1c03d-204">Administrador de perfis de negócios</span><span class="sxs-lookup"><span data-stu-id="1c03d-204">Business profile admin</span></span>   |<span data-ttu-id="1c03d-205">\* Ver, criar e gerenciar perfis de negócios</span><span class="sxs-lookup"><span data-stu-id="1c03d-205">\* View, create, and manage business profile</span></span> 
||<span data-ttu-id="1c03d-206">\*    Ver, criar e gerenciar solicitações de serviço de parceiros</span><span class="sxs-lookup"><span data-stu-id="1c03d-206">\*    View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="1c03d-207">Gerenciar incentivos</span><span class="sxs-lookup"><span data-stu-id="1c03d-207">Manage incentives</span></span> 

|<span data-ttu-id="1c03d-208">**Função**</span><span class="sxs-lookup"><span data-stu-id="1c03d-208">**Role**</span></span> | <span data-ttu-id="1c03d-209">**O que você pode fazer**</span><span class="sxs-lookup"><span data-stu-id="1c03d-209">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="1c03d-210">Administrador de incentivos</span><span class="sxs-lookup"><span data-stu-id="1c03d-210">Incentives admin</span></span>|<span data-ttu-id="1c03d-211">\*    Iniciar e gerenciar incentivos</span><span class="sxs-lookup"><span data-stu-id="1c03d-211">\*    Initiates and manages incentives</span></span> 
||<span data-ttu-id="1c03d-212">\*    Ver e editar todos os aspectos dos programas de incentivos</span><span class="sxs-lookup"><span data-stu-id="1c03d-212">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="1c03d-213">\*    Ver e editar detalhes bancários e fiscais</span><span class="sxs-lookup"><span data-stu-id="1c03d-213">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="1c03d-214">\*    Ver lucros de reembolso e de cooperação</span><span class="sxs-lookup"><span data-stu-id="1c03d-214">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="1c03d-215">\*    Acessar suporte</span><span class="sxs-lookup"><span data-stu-id="1c03d-215">\*    Access support</span></span>
||<span data-ttu-id="1c03d-216">\*    Disputar pagamentos de incentivos</span><span class="sxs-lookup"><span data-stu-id="1c03d-216">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="1c03d-217">Usuário de incentivos</span><span class="sxs-lookup"><span data-stu-id="1c03d-217">Incentives user</span></span>|<span data-ttu-id="1c03d-218">\*    Ver programas de incentivos</span><span class="sxs-lookup"><span data-stu-id="1c03d-218">\*    Can view incentives programs</span></span>
||<span data-ttu-id="1c03d-219">\*    Ver e iniciar reivindicações de incentivos</span><span class="sxs-lookup"><span data-stu-id="1c03d-219">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="1c03d-220">\*    Ver lucros de reembolso e de cooperação</span><span class="sxs-lookup"><span data-stu-id="1c03d-220">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="1c03d-221">\*    Acessar suporte</span><span class="sxs-lookup"><span data-stu-id="1c03d-221">\*    Access support</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="1c03d-222">Exibir dados de Insights do Partner Center</span><span class="sxs-lookup"><span data-stu-id="1c03d-222">View Partner Center Insights data</span></span>

|<span data-ttu-id="1c03d-223">**Função**</span><span class="sxs-lookup"><span data-stu-id="1c03d-223">**Role**</span></span> | <span data-ttu-id="1c03d-224">**O que você pode fazer**</span><span class="sxs-lookup"><span data-stu-id="1c03d-224">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="1c03d-225">Visualizador de relatórios executivos</span><span class="sxs-lookup"><span data-stu-id="1c03d-225">Executive report viewer</span></span>|<span data-ttu-id="1c03d-226">Acesso a todos os conjuntos de dados de relatórios</span><span class="sxs-lookup"><span data-stu-id="1c03d-226">Access to all reporting datasets</span></span>|
|<span data-ttu-id="1c03d-227">Visualizador de relatórios</span><span class="sxs-lookup"><span data-stu-id="1c03d-227">Report viewer</span></span>|<span data-ttu-id="1c03d-228">Acesso a relatórios de dados com exceção de receita e dados pessoais de clientes e funcionários</span><span class="sxs-lookup"><span data-stu-id="1c03d-228">Access to data reports with exception of revenue and customer and employee personal data</span></span>|












                                    