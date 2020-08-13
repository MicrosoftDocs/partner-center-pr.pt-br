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
ms.openlocfilehash: c87e47efc6c94e4e53a031a983a4a4e528ddc012
ms.sourcegitcommit: 59bdf42f5282262835cb7ee2bd215bbddc7686d7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/06/2020
ms.locfileid: "87839181"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="783ce-103">Atribuir permissões e funções de usuários para os usuários de uma empresa que precisam trabalhar no Partner Center</span><span class="sxs-lookup"><span data-stu-id="783ce-103">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="783ce-104">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="783ce-104">**Appropriate roles**</span></span>

- <span data-ttu-id="783ce-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="783ce-105">Global admin</span></span>
- <span data-ttu-id="783ce-106">Administrador de usuários</span><span class="sxs-lookup"><span data-stu-id="783ce-106">User admin</span></span>
- <span data-ttu-id="783ce-107">Administrador de parceiros do MPN</span><span class="sxs-lookup"><span data-stu-id="783ce-107">MPN partner admin</span></span>

<span data-ttu-id="783ce-108">Você configurou seu perfil de parceiro, incluindo a razão social, o endereço, os detalhes de suporte, as isenções de imposto sobre arquivos, as informações bancárias e o contato principal da empresa.</span><span class="sxs-lookup"><span data-stu-id="783ce-108">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="783ce-109">Próxima etapa: Configure as senhas e funções dos seus usuários para que eles possam começar a trabalhar no Partner Center com você.</span><span class="sxs-lookup"><span data-stu-id="783ce-109">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="783ce-110">Configurar seus funcionários para trabalhar no Partner Center</span><span class="sxs-lookup"><span data-stu-id="783ce-110">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="783ce-111">Você determinará os tipos de acesso que os usuários terão ao Partner Center por meio das funções e permissões a eles atribuídas.</span><span class="sxs-lookup"><span data-stu-id="783ce-111">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="783ce-112">As funções estão relacionadas aos programas com os quais a sua empresa está envolvida.</span><span class="sxs-lookup"><span data-stu-id="783ce-112">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="783ce-113">Por exemplo, se a sua empresa for um CSP (Provedor de Soluções na Nuvem), você não apenas terá as funções de gerenciamento de locatário padrão do Azure AD, como o administrador global, mas também precisará de funções específicas para o programa CSP.</span><span class="sxs-lookup"><span data-stu-id="783ce-113">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="783ce-114">Cada programa tem funções específicas para ele.</span><span class="sxs-lookup"><span data-stu-id="783ce-114">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="783ce-115">As funções de locatário do Azure Active Directory (AAD) incluem administrador global, administrador de usuários e funções de CSP.</span><span class="sxs-lookup"><span data-stu-id="783ce-115">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="783ce-116">As funções não pertencentes ao AAD são aquelas que não gerenciam o locatário e incluem administrador do MPN, administrador de perfil de negócios, administrador de indicações, administrador de incentivos e usuário de incentivos.</span><span class="sxs-lookup"><span data-stu-id="783ce-116">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="783ce-117">Gerenciar transações comerciais no Partner Center (funções Azure AD e CSP)</span><span class="sxs-lookup"><span data-stu-id="783ce-117">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="783ce-118">**Função**</span><span class="sxs-lookup"><span data-stu-id="783ce-118">**Role**</span></span>|<span data-ttu-id="783ce-119">**O que eles podem fazer**</span><span class="sxs-lookup"><span data-stu-id="783ce-119">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="783ce-120">Administrador global</span><span class="sxs-lookup"><span data-stu-id="783ce-120">Global admin</span></span>|<span data-ttu-id="783ce-121">\*    Pode acessar todas as contas/os serviços da Microsoft com todos os privilégios</span><span class="sxs-lookup"><span data-stu-id="783ce-121">\*    Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="783ce-122">\*    Criar tíquetes de suporte para o Partner Center</span><span class="sxs-lookup"><span data-stu-id="783ce-122">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="783ce-123">\*    Ver contratos, listas de preços e ofertas</span><span class="sxs-lookup"><span data-stu-id="783ce-123">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="783ce-124">\*    Ver, criar e gerenciar usuários parceiros</span><span class="sxs-lookup"><span data-stu-id="783ce-124">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="783ce-125">• Exibir, criar e gerenciar a cobrança, as faturas e os arquivos reconhecimento</span><span class="sxs-lookup"><span data-stu-id="783ce-125">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="783ce-126">Administrador de gerenciamento de usuário</span><span class="sxs-lookup"><span data-stu-id="783ce-126">User management admin</span></span>   | <span data-ttu-id="783ce-127">\*    Ver, criar e gerenciar usuários</span><span class="sxs-lookup"><span data-stu-id="783ce-127">\*    View, create, and manage users</span></span>
||<span data-ttu-id="783ce-128">\*    Ver todos os perfis de parceiros</span><span class="sxs-lookup"><span data-stu-id="783ce-128">\*    View all partner profiles</span></span>
||<span data-ttu-id="783ce-129">\*    Ver, criar e gerenciar usuários parceiros</span><span class="sxs-lookup"><span data-stu-id="783ce-129">\*    View, create, and manage partner users</span></span>  |
|<span data-ttu-id="783ce-130">Administrador de cobrança</span><span class="sxs-lookup"><span data-stu-id="783ce-130">Billing admin</span></span> | <span data-ttu-id="783ce-131">– Exibir, criar e gerenciar a cobrança, as faturas e os arquivos reconhecimento</span><span class="sxs-lookup"><span data-stu-id="783ce-131">- View, create, and manage billing, invoices, and recon files</span></span>|
||<span data-ttu-id="783ce-132">\*    Exibir preço</span><span class="sxs-lookup"><span data-stu-id="783ce-132">\*    View pricing</span></span>
|<span data-ttu-id="783ce-133">Usuário padrão</span><span class="sxs-lookup"><span data-stu-id="783ce-133">Default user</span></span>|  <span data-ttu-id="783ce-134">Exibir meu perfil</span><span class="sxs-lookup"><span data-stu-id="783ce-134">View My profile</span></span>   |
|<span data-ttu-id="783ce-135">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="783ce-135">Admin agent</span></span> | <span data-ttu-id="783ce-136">\*    Gerenciamento de clientes</span><span class="sxs-lookup"><span data-stu-id="783ce-136">\*    Customer management</span></span>
||<span data-ttu-id="783ce-137">\*    Adicionar lista de dispositivos ao Partner Center</span><span class="sxs-lookup"><span data-stu-id="783ce-137">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="783ce-138">\*    Criar e aplicar perfis aos dispositivos</span><span class="sxs-lookup"><span data-stu-id="783ce-138">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="783ce-139">\*    Gerenciamento de assinaturas</span><span class="sxs-lookup"><span data-stu-id="783ce-139">\*    Subscription management</span></span>
||<span data-ttu-id="783ce-140">\*    Solicitações de integridade e de serviços para os clientes</span><span class="sxs-lookup"><span data-stu-id="783ce-140">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="783ce-141">\*    Solicitar privilégios de administrador delegado</span><span class="sxs-lookup"><span data-stu-id="783ce-141">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="783ce-142">\*    Ver preços e ofertas</span><span class="sxs-lookup"><span data-stu-id="783ce-142">\*    View pricing and offers</span></span>
||<span data-ttu-id="783ce-143">\*    Cobrança</span><span class="sxs-lookup"><span data-stu-id="783ce-143">\*    Billing</span></span>
||<span data-ttu-id="783ce-144">\*    Administrar em nome de um cliente</span><span class="sxs-lookup"><span data-stu-id="783ce-144">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="783ce-145">\*    Registrar um revendedor com valor agregado</span><span class="sxs-lookup"><span data-stu-id="783ce-145">\*    Register a value added reseller</span></span>|
|<span data-ttu-id="783ce-146">Agente de vendas</span><span class="sxs-lookup"><span data-stu-id="783ce-146">Sales agent</span></span> | <span data-ttu-id="783ce-147">\*    Gerenciamento de clientes</span><span class="sxs-lookup"><span data-stu-id="783ce-147">\*    Customer management</span></span>
||<span data-ttu-id="783ce-148">\*    Adicionar lista de dispositivos ao Partner Center</span><span class="sxs-lookup"><span data-stu-id="783ce-148">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="783ce-149">\*    Gerenciamento de assinaturas</span><span class="sxs-lookup"><span data-stu-id="783ce-149">\*    Subscription management</span></span>
||<span data-ttu-id="783ce-150">\*    Ver tíquetes de suporte</span><span class="sxs-lookup"><span data-stu-id="783ce-150">\*    View support tickets</span></span>
||<span data-ttu-id="783ce-151">\*    Solicitar um relacionamento com um cliente</span><span class="sxs-lookup"><span data-stu-id="783ce-151">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="783ce-152">\*    Ver preços e ofertas</span><span class="sxs-lookup"><span data-stu-id="783ce-152">\*    View pricing and offers</span></span>
||<span data-ttu-id="783ce-153">\*    Gerenciar clientes potenciais</span><span class="sxs-lookup"><span data-stu-id="783ce-153">\*    Manage customer leads</span></span>
||<span data-ttu-id="783ce-154">\*    Ver o contrato do cliente</span><span class="sxs-lookup"><span data-stu-id="783ce-154">\*    View the customer agreement</span></span>
||<span data-ttu-id="783ce-155">\*    Registrar um revendedor com valor agregado</span><span class="sxs-lookup"><span data-stu-id="783ce-155">\*    Register a value-added reseller</span></span>|
|<span data-ttu-id="783ce-156">Agente de suporte técnico</span><span class="sxs-lookup"><span data-stu-id="783ce-156">Helpdesk agent</span></span>| <span data-ttu-id="783ce-157">\*    Pesquisar e ver um cliente</span><span class="sxs-lookup"><span data-stu-id="783ce-157">\*    Search for and view a customer</span></span>
||<span data-ttu-id="783ce-158">\*    Editar detalhes do cliente</span><span class="sxs-lookup"><span data-stu-id="783ce-158">\*    Edit customer details</span></span>
||<span data-ttu-id="783ce-159">\*    Ajudar a resolver problemas dos clientes com o gerenciamento de cobrança ou assinaturas</span><span class="sxs-lookup"><span data-stu-id="783ce-159">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="783ce-160">\*    Solicitar suporte em nome dos clientes</span><span class="sxs-lookup"><span data-stu-id="783ce-160">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="783ce-161">\*    Gerenciar problemas de assinaturas e cobrança em nome dos clientes</span><span class="sxs-lookup"><span data-stu-id="783ce-161">\*    Manage subscriptions and billing issues on behalf of customers</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="783ce-162">CPV (Fornecedor de Painel de Controle).</span><span class="sxs-lookup"><span data-stu-id="783ce-162">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="783ce-163">(Função CSP e função não pertencente ao AAD)</span><span class="sxs-lookup"><span data-stu-id="783ce-163">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="783ce-164">Os CPVs desenvolvem aplicativos para uso por parceiros CSP (Provedor de Soluções na Nuvem) a fim de permitir que eles integrem seus sistemas com as APIs do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="783ce-164">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="783ce-165">**Função**</span><span class="sxs-lookup"><span data-stu-id="783ce-165">**Role**</span></span>   |<span data-ttu-id="783ce-166">**O que você pode fazer**</span><span class="sxs-lookup"><span data-stu-id="783ce-166">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="783ce-167">Administrador global</span><span class="sxs-lookup"><span data-stu-id="783ce-167">Global admin</span></span>| <span data-ttu-id="783ce-168">Exibir e gerenciar seu perfil de CPV</span><span class="sxs-lookup"><span data-stu-id="783ce-168">View and manage your CPV profile</span></span>|
||<span data-ttu-id="783ce-169">Exibir e gerenciar todos os seus usuários que precisam de acesso aos recursos de CPV</span><span class="sxs-lookup"><span data-stu-id="783ce-169">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="783ce-170">Usuário convidado (deve ser adicionado ao locatário do AAD)</span><span class="sxs-lookup"><span data-stu-id="783ce-170">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="783ce-171">**Usuário convidado**</span><span class="sxs-lookup"><span data-stu-id="783ce-171">**Guest user**</span></span>   | <span data-ttu-id="783ce-172">**Funções**</span><span class="sxs-lookup"><span data-stu-id="783ce-172">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="783ce-173">Administrador de parceiros do MPN</span><span class="sxs-lookup"><span data-stu-id="783ce-173">MPN partner admin</span></span>|
||<span data-ttu-id="783ce-174">Administrador de contas</span><span class="sxs-lookup"><span data-stu-id="783ce-174">Accounts admin</span></span>|
||<span data-ttu-id="783ce-175">Administrador de incentivos</span><span class="sxs-lookup"><span data-stu-id="783ce-175">Incentives admin</span></span>|
||<span data-ttu-id="783ce-176">Administrador de perfis de negócios</span><span class="sxs-lookup"><span data-stu-id="783ce-176">Business profile admin</span></span>|
||<span data-ttu-id="783ce-177">Administrador de indicações</span><span class="sxs-lookup"><span data-stu-id="783ce-177">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="783ce-178">Gerenciar associação do MPN e sua empresa (funções não pertencentes ao AAD: essas funções gerenciam os negócios da empresa em vez do locatário)</span><span class="sxs-lookup"><span data-stu-id="783ce-178">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="783ce-179">**Função**</span><span class="sxs-lookup"><span data-stu-id="783ce-179">**Role**</span></span> | <span data-ttu-id="783ce-180">**O que você pode fazer**</span><span class="sxs-lookup"><span data-stu-id="783ce-180">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="783ce-181">Administrador de parceiros do MPN</span><span class="sxs-lookup"><span data-stu-id="783ce-181">MPN partner admin</span></span>|<span data-ttu-id="783ce-182">\*    Ver, criar e gerenciar solicitações de serviço de parceiros</span><span class="sxs-lookup"><span data-stu-id="783ce-182">\*    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="783ce-183">\*    Ver perfis jurídico, empresarial, de negócios e do MPN</span><span class="sxs-lookup"><span data-stu-id="783ce-183">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="783ce-184">\*    Ver detalhes do usuário e seus dados de habilidades</span><span class="sxs-lookup"><span data-stu-id="783ce-184">\*    View user details and their skills data</span></span>
||<span data-ttu-id="783ce-185">\*    Ver competências</span><span class="sxs-lookup"><span data-stu-id="783ce-185">\*    View competencies</span></span>
||<span data-ttu-id="783ce-186">\*    Ver e gerenciar benefícios</span><span class="sxs-lookup"><span data-stu-id="783ce-186">\*    View and manage benefits</span></span>
||<span data-ttu-id="783ce-187">\*    Ver e comprar ofertas do MPN</span><span class="sxs-lookup"><span data-stu-id="783ce-187">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="783ce-188">\*    Ver histórico de pedidos de ofertas e faturas do MPN</span><span class="sxs-lookup"><span data-stu-id="783ce-188">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="783ce-189">\*    Ver dados do indicador de contribuição de parceiros</span><span class="sxs-lookup"><span data-stu-id="783ce-189">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="783ce-190">\*    Pode funcionar na ferramenta de validação de comprovantes</span><span class="sxs-lookup"><span data-stu-id="783ce-190">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="783ce-191">\*    Ver análises de dados do cliente</span><span class="sxs-lookup"><span data-stu-id="783ce-191">\*    View customer data analytics</span></span>
||<span data-ttu-id="783ce-192">\*    Ver outras funções de usuário dentro da empresa, mas não atribuir funções</span><span class="sxs-lookup"><span data-stu-id="783ce-192">\*    View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="783ce-193">Administrador de conta</span><span class="sxs-lookup"><span data-stu-id="783ce-193">Account admin</span></span>| <span data-ttu-id="783ce-194">Adicionar locais</span><span class="sxs-lookup"><span data-stu-id="783ce-194">Add locations</span></span>
|| <span data-ttu-id="783ce-195">Gerenciar perfis relacionados às contas para as quais você é administrador</span><span class="sxs-lookup"><span data-stu-id="783ce-195">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="783ce-196">\*    Atribuir funções aos usuários do locatário para funções não pertencentes ao AAD</span><span class="sxs-lookup"><span data-stu-id="783ce-196">\*    Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="783ce-197">\*    Registrar locais em programas</span><span class="sxs-lookup"><span data-stu-id="783ce-197">\*    Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="783ce-198">Gerenciar indicações</span><span class="sxs-lookup"><span data-stu-id="783ce-198">Manage referrals</span></span> 

|<span data-ttu-id="783ce-199">**Função**</span><span class="sxs-lookup"><span data-stu-id="783ce-199">**Role**</span></span>|<span data-ttu-id="783ce-200">**O que você pode fazer**</span><span class="sxs-lookup"><span data-stu-id="783ce-200">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="783ce-201">Administrador de indicações</span><span class="sxs-lookup"><span data-stu-id="783ce-201">Referrals admin</span></span>       |<span data-ttu-id="783ce-202">\* Ver, criar e gerenciar perfis de negócios</span><span class="sxs-lookup"><span data-stu-id="783ce-202">\*    View, create, and manage business profiles</span></span>
||<span data-ttu-id="783ce-203">\*    Receber e gerenciar indicações</span><span class="sxs-lookup"><span data-stu-id="783ce-203">\*    Receive and manage referrals</span></span>
||<span data-ttu-id="783ce-204">\* Ver, criar e gerenciar as indicações de venda conjunta</span><span class="sxs-lookup"><span data-stu-id="783ce-204">\* View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="783ce-205">\*    Ver, criar e gerenciar solicitações de serviço de parceiros</span><span class="sxs-lookup"><span data-stu-id="783ce-205">\*    View, create, and manage partner service requests</span></span>
|<span data-ttu-id="783ce-206">Administrador de perfis de negócios</span><span class="sxs-lookup"><span data-stu-id="783ce-206">Business profile admin</span></span>   |<span data-ttu-id="783ce-207">\* Ver, criar e gerenciar perfis de negócios</span><span class="sxs-lookup"><span data-stu-id="783ce-207">\* View, create, and manage business profile</span></span> 
||<span data-ttu-id="783ce-208">\*    Ver, criar e gerenciar solicitações de serviço de parceiros</span><span class="sxs-lookup"><span data-stu-id="783ce-208">\*    View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="783ce-209">Gerenciar incentivos</span><span class="sxs-lookup"><span data-stu-id="783ce-209">Manage incentives</span></span> 

|<span data-ttu-id="783ce-210">**Função**</span><span class="sxs-lookup"><span data-stu-id="783ce-210">**Role**</span></span> | <span data-ttu-id="783ce-211">**O que você pode fazer**</span><span class="sxs-lookup"><span data-stu-id="783ce-211">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="783ce-212">Administrador de incentivos</span><span class="sxs-lookup"><span data-stu-id="783ce-212">Incentives admin</span></span>|<span data-ttu-id="783ce-213">\*    Iniciar e gerenciar incentivos</span><span class="sxs-lookup"><span data-stu-id="783ce-213">\*    Initiates and manages incentives</span></span> 
||<span data-ttu-id="783ce-214">\*    Ver e editar todos os aspectos dos programas de incentivos</span><span class="sxs-lookup"><span data-stu-id="783ce-214">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="783ce-215">\*    Ver e editar detalhes bancários e fiscais</span><span class="sxs-lookup"><span data-stu-id="783ce-215">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="783ce-216">\*    Ver lucros de reembolso e de cooperação</span><span class="sxs-lookup"><span data-stu-id="783ce-216">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="783ce-217">\*    Acessar suporte</span><span class="sxs-lookup"><span data-stu-id="783ce-217">\*    Access support</span></span>
||<span data-ttu-id="783ce-218">\*    Disputar pagamentos de incentivos</span><span class="sxs-lookup"><span data-stu-id="783ce-218">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="783ce-219">Usuário de incentivos</span><span class="sxs-lookup"><span data-stu-id="783ce-219">Incentives user</span></span>|<span data-ttu-id="783ce-220">\*    Ver programas de incentivos</span><span class="sxs-lookup"><span data-stu-id="783ce-220">\*    Can view incentives programs</span></span>
||<span data-ttu-id="783ce-221">\*    Ver e iniciar reivindicações de incentivos</span><span class="sxs-lookup"><span data-stu-id="783ce-221">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="783ce-222">\*    Ver lucros de reembolso e de cooperação</span><span class="sxs-lookup"><span data-stu-id="783ce-222">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="783ce-223">\*    Acessar suporte</span><span class="sxs-lookup"><span data-stu-id="783ce-223">\*    Access support</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="783ce-224">Exibir dados de Insights do Partner Center</span><span class="sxs-lookup"><span data-stu-id="783ce-224">View Partner Center Insights data</span></span>

|<span data-ttu-id="783ce-225">**Função**</span><span class="sxs-lookup"><span data-stu-id="783ce-225">**Role**</span></span> | <span data-ttu-id="783ce-226">**O que você pode fazer**</span><span class="sxs-lookup"><span data-stu-id="783ce-226">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="783ce-227">Visualizador de relatórios executivos</span><span class="sxs-lookup"><span data-stu-id="783ce-227">Executive report viewer</span></span>|<span data-ttu-id="783ce-228">Acesso a todos os conjuntos de dados de relatórios</span><span class="sxs-lookup"><span data-stu-id="783ce-228">Access to all reporting datasets</span></span>|
|<span data-ttu-id="783ce-229">Visualizador de relatórios</span><span class="sxs-lookup"><span data-stu-id="783ce-229">Report viewer</span></span>|<span data-ttu-id="783ce-230">Acesso a relatórios de dados com exceção de receita e dados pessoais de clientes e funcionários</span><span class="sxs-lookup"><span data-stu-id="783ce-230">Access to data reports with exception of revenue and customer and employee personal data</span></span>|












                                    
