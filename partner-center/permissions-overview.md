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
ms.openlocfilehash: 3feb4e678381b6fa5398bf3b3d89f6e4286e6ff1
ms.sourcegitcommit: 4feae1ea7fd3077934e3c931a5de801c96a4f995
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2020
ms.locfileid: "89040762"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="39eca-103">Atribuir permissões e funções de usuários para os usuários de uma empresa que precisam trabalhar no Partner Center</span><span class="sxs-lookup"><span data-stu-id="39eca-103">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="39eca-104">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="39eca-104">**Appropriate roles**</span></span>

- <span data-ttu-id="39eca-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="39eca-105">Global admin</span></span>
- <span data-ttu-id="39eca-106">Administrador de usuários</span><span class="sxs-lookup"><span data-stu-id="39eca-106">User admin</span></span>
- <span data-ttu-id="39eca-107">Administrador de parceiros do MPN</span><span class="sxs-lookup"><span data-stu-id="39eca-107">MPN partner admin</span></span>

<span data-ttu-id="39eca-108">Você configurou seu perfil de parceiro, incluindo a razão social, o endereço, os detalhes de suporte, as isenções de imposto sobre arquivos, as informações bancárias e o contato principal da empresa.</span><span class="sxs-lookup"><span data-stu-id="39eca-108">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="39eca-109">Próxima etapa: Configure as senhas e funções dos seus usuários para que eles possam começar a trabalhar no Partner Center com você.</span><span class="sxs-lookup"><span data-stu-id="39eca-109">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="39eca-110">Configurar seus funcionários para trabalhar no Partner Center</span><span class="sxs-lookup"><span data-stu-id="39eca-110">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="39eca-111">Você determinará os tipos de acesso que os usuários terão ao Partner Center por meio das funções e permissões a eles atribuídas.</span><span class="sxs-lookup"><span data-stu-id="39eca-111">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="39eca-112">As funções estão relacionadas aos programas com os quais a sua empresa está envolvida.</span><span class="sxs-lookup"><span data-stu-id="39eca-112">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="39eca-113">Por exemplo, se a sua empresa for um CSP (Provedor de Soluções na Nuvem), você não apenas terá as funções de gerenciamento de locatário padrão do Azure AD, como o administrador global, mas também precisará de funções específicas para o programa CSP.</span><span class="sxs-lookup"><span data-stu-id="39eca-113">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="39eca-114">Cada programa tem funções específicas para ele.</span><span class="sxs-lookup"><span data-stu-id="39eca-114">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="39eca-115">As funções de locatário do Azure Active Directory (AAD) incluem administrador global, administrador de usuários e funções de CSP.</span><span class="sxs-lookup"><span data-stu-id="39eca-115">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="39eca-116">As funções não pertencentes ao AAD são aquelas que não gerenciam o locatário e incluem administrador do MPN, administrador de perfil de negócios, administrador de indicações, administrador de incentivos e usuário de incentivos.</span><span class="sxs-lookup"><span data-stu-id="39eca-116">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="39eca-117">Gerenciar transações comerciais no Partner Center (funções Azure AD e CSP)</span><span class="sxs-lookup"><span data-stu-id="39eca-117">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="39eca-118">**Função**</span><span class="sxs-lookup"><span data-stu-id="39eca-118">**Role**</span></span>|<span data-ttu-id="39eca-119">**O que eles podem fazer**</span><span class="sxs-lookup"><span data-stu-id="39eca-119">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="39eca-120">Administrador global</span><span class="sxs-lookup"><span data-stu-id="39eca-120">Global admin</span></span>|<span data-ttu-id="39eca-121">\*    Pode acessar todas as contas/os serviços da Microsoft com todos os privilégios</span><span class="sxs-lookup"><span data-stu-id="39eca-121">\*    Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="39eca-122">\*    Criar tíquetes de suporte para o Partner Center</span><span class="sxs-lookup"><span data-stu-id="39eca-122">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="39eca-123">\*    Ver os tíquetes de suporte do parceiro que você criar</span><span class="sxs-lookup"><span data-stu-id="39eca-123">\*    View partner support tickets you create</span></span>
||<span data-ttu-id="39eca-124">\*    Ver contratos, listas de preços e ofertas</span><span class="sxs-lookup"><span data-stu-id="39eca-124">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="39eca-125">\*    Ver, criar e gerenciar usuários parceiros</span><span class="sxs-lookup"><span data-stu-id="39eca-125">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="39eca-126">• Exibir, criar e gerenciar a cobrança, as faturas e os arquivos reconhecimento</span><span class="sxs-lookup"><span data-stu-id="39eca-126">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="39eca-127">Administrador de gerenciamento de usuário</span><span class="sxs-lookup"><span data-stu-id="39eca-127">User management admin</span></span>   | <span data-ttu-id="39eca-128">\*    Ver, criar e gerenciar usuários</span><span class="sxs-lookup"><span data-stu-id="39eca-128">\*    View, create, and manage users</span></span>
||<span data-ttu-id="39eca-129">\*    Ver todos os perfis de parceiros</span><span class="sxs-lookup"><span data-stu-id="39eca-129">\*    View all partner profiles</span></span>
||<span data-ttu-id="39eca-130">\*    Ver, criar e gerenciar usuários parceiros</span><span class="sxs-lookup"><span data-stu-id="39eca-130">\*    View, create, and manage partner users</span></span>  |
||<span data-ttu-id="39eca-131">\*    Criar tíquetes de suporte para o Partner Center</span><span class="sxs-lookup"><span data-stu-id="39eca-131">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="39eca-132">\*    Ver os tíquetes de suporte do parceiro que você criar</span><span class="sxs-lookup"><span data-stu-id="39eca-132">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="39eca-133">Administrador de cobrança</span><span class="sxs-lookup"><span data-stu-id="39eca-133">Billing admin</span></span> | <span data-ttu-id="39eca-134">– Exibir, criar e gerenciar a cobrança, as faturas e os arquivos reconhecimento</span><span class="sxs-lookup"><span data-stu-id="39eca-134">- View, create, and manage billing, invoices, and recon files</span></span>|
||<span data-ttu-id="39eca-135">\*    Exibir preço</span><span class="sxs-lookup"><span data-stu-id="39eca-135">\*    View pricing</span></span>
||<span data-ttu-id="39eca-136">\*    Criar tíquetes de suporte para o Partner Center</span><span class="sxs-lookup"><span data-stu-id="39eca-136">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="39eca-137">\*    Ver os tíquetes de suporte do parceiro que você criar</span><span class="sxs-lookup"><span data-stu-id="39eca-137">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="39eca-138">Usuário padrão</span><span class="sxs-lookup"><span data-stu-id="39eca-138">Default user</span></span>|  <span data-ttu-id="39eca-139">Exibir meu perfil</span><span class="sxs-lookup"><span data-stu-id="39eca-139">View My profile</span></span>   |
|<span data-ttu-id="39eca-140">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="39eca-140">Admin agent</span></span> | <span data-ttu-id="39eca-141">\*    Gerenciamento de clientes</span><span class="sxs-lookup"><span data-stu-id="39eca-141">\*    Customer management</span></span>
||<span data-ttu-id="39eca-142">\*    Adicionar lista de dispositivos ao Partner Center</span><span class="sxs-lookup"><span data-stu-id="39eca-142">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="39eca-143">\*    Criar e aplicar perfis aos dispositivos</span><span class="sxs-lookup"><span data-stu-id="39eca-143">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="39eca-144">\*    Gerenciamento de assinaturas</span><span class="sxs-lookup"><span data-stu-id="39eca-144">\*    Subscription management</span></span>
||<span data-ttu-id="39eca-145">\*    Solicitações de integridade e de serviços para os clientes</span><span class="sxs-lookup"><span data-stu-id="39eca-145">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="39eca-146">\*    Solicitar privilégios de administrador delegado</span><span class="sxs-lookup"><span data-stu-id="39eca-146">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="39eca-147">\*    Ver preços e ofertas</span><span class="sxs-lookup"><span data-stu-id="39eca-147">\*    View pricing and offers</span></span>
||<span data-ttu-id="39eca-148">\*    Cobrança</span><span class="sxs-lookup"><span data-stu-id="39eca-148">\*    Billing</span></span>
||<span data-ttu-id="39eca-149">\*    Administrar em nome de um cliente</span><span class="sxs-lookup"><span data-stu-id="39eca-149">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="39eca-150">\*    Registrar um revendedor com valor agregado</span><span class="sxs-lookup"><span data-stu-id="39eca-150">\*    Register a value added reseller</span></span>
||<span data-ttu-id="39eca-151">\*    Criar tíquetes de suporte para o Partner Center</span><span class="sxs-lookup"><span data-stu-id="39eca-151">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="39eca-152">\*    Ver os tíquetes de suporte do parceiro que você criar</span><span class="sxs-lookup"><span data-stu-id="39eca-152">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="39eca-153">Agente de vendas</span><span class="sxs-lookup"><span data-stu-id="39eca-153">Sales agent</span></span> | <span data-ttu-id="39eca-154">\*    Gerenciamento de clientes</span><span class="sxs-lookup"><span data-stu-id="39eca-154">\*    Customer management</span></span>
||<span data-ttu-id="39eca-155">\*    Adicionar lista de dispositivos ao Partner Center</span><span class="sxs-lookup"><span data-stu-id="39eca-155">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="39eca-156">\*    Gerenciamento de assinaturas</span><span class="sxs-lookup"><span data-stu-id="39eca-156">\*    Subscription management</span></span>
||<span data-ttu-id="39eca-157">\*    Ver tíquetes de suporte</span><span class="sxs-lookup"><span data-stu-id="39eca-157">\*    View support tickets</span></span>
||<span data-ttu-id="39eca-158">\*    Solicitar um relacionamento com um cliente</span><span class="sxs-lookup"><span data-stu-id="39eca-158">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="39eca-159">\*    Ver preços e ofertas</span><span class="sxs-lookup"><span data-stu-id="39eca-159">\*    View pricing and offers</span></span>
||<span data-ttu-id="39eca-160">\*    Gerenciar clientes potenciais</span><span class="sxs-lookup"><span data-stu-id="39eca-160">\*    Manage customer leads</span></span>
||<span data-ttu-id="39eca-161">\*    Ver o contrato do cliente</span><span class="sxs-lookup"><span data-stu-id="39eca-161">\*    View the customer agreement</span></span>
||<span data-ttu-id="39eca-162">\*    Registrar um revendedor com valor agregado</span><span class="sxs-lookup"><span data-stu-id="39eca-162">\*    Register a value-added reseller</span></span>
||<span data-ttu-id="39eca-163">\*    Criar tíquetes de suporte para o Partner Center</span><span class="sxs-lookup"><span data-stu-id="39eca-163">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="39eca-164">\*    Ver os tíquetes de suporte do parceiro que você criar</span><span class="sxs-lookup"><span data-stu-id="39eca-164">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="39eca-165">Agente de suporte técnico</span><span class="sxs-lookup"><span data-stu-id="39eca-165">Helpdesk agent</span></span>| <span data-ttu-id="39eca-166">\*    Pesquisar e ver um cliente</span><span class="sxs-lookup"><span data-stu-id="39eca-166">\*    Search for and view a customer</span></span>
||<span data-ttu-id="39eca-167">\*    Editar detalhes do cliente</span><span class="sxs-lookup"><span data-stu-id="39eca-167">\*    Edit customer details</span></span>
||<span data-ttu-id="39eca-168">\*    Ajudar a resolver problemas dos clientes com o gerenciamento de cobrança ou assinaturas</span><span class="sxs-lookup"><span data-stu-id="39eca-168">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="39eca-169">\*    Solicitar suporte em nome dos clientes</span><span class="sxs-lookup"><span data-stu-id="39eca-169">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="39eca-170">\*    Gerenciar problemas de assinaturas e cobrança em nome dos clientes</span><span class="sxs-lookup"><span data-stu-id="39eca-170">\*    Manage subscriptions and billing issues on behalf of customers</span></span>
||<span data-ttu-id="39eca-171">\*    Criar tíquetes de suporte para o Partner Center</span><span class="sxs-lookup"><span data-stu-id="39eca-171">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="39eca-172">\*    Ver os tíquetes de suporte do parceiro que você criar</span><span class="sxs-lookup"><span data-stu-id="39eca-172">\*    View partner support tickets you create</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="39eca-173">CPV (Fornecedor de Painel de Controle).</span><span class="sxs-lookup"><span data-stu-id="39eca-173">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="39eca-174">(Função CSP e função não pertencente ao AAD)</span><span class="sxs-lookup"><span data-stu-id="39eca-174">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="39eca-175">Os CPVs desenvolvem aplicativos para uso por parceiros CSP (Provedor de Soluções na Nuvem) a fim de permitir que eles integrem seus sistemas com as APIs do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="39eca-175">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="39eca-176">**Função**</span><span class="sxs-lookup"><span data-stu-id="39eca-176">**Role**</span></span>   |<span data-ttu-id="39eca-177">**O que você pode fazer**</span><span class="sxs-lookup"><span data-stu-id="39eca-177">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="39eca-178">Administrador global</span><span class="sxs-lookup"><span data-stu-id="39eca-178">Global admin</span></span>| <span data-ttu-id="39eca-179">Exibir e gerenciar seu perfil de CPV</span><span class="sxs-lookup"><span data-stu-id="39eca-179">View and manage your CPV profile</span></span>|
||<span data-ttu-id="39eca-180">Exibir e gerenciar todos os seus usuários que precisam de acesso aos recursos de CPV</span><span class="sxs-lookup"><span data-stu-id="39eca-180">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="39eca-181">Usuário convidado (deve ser adicionado ao locatário do AAD)</span><span class="sxs-lookup"><span data-stu-id="39eca-181">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="39eca-182">**Usuário convidado**</span><span class="sxs-lookup"><span data-stu-id="39eca-182">**Guest user**</span></span>   | <span data-ttu-id="39eca-183">**Funções**</span><span class="sxs-lookup"><span data-stu-id="39eca-183">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="39eca-184">Administrador de parceiros do MPN</span><span class="sxs-lookup"><span data-stu-id="39eca-184">MPN partner admin</span></span>|
||<span data-ttu-id="39eca-185">Administrador de contas</span><span class="sxs-lookup"><span data-stu-id="39eca-185">Accounts admin</span></span>|
||<span data-ttu-id="39eca-186">Administrador de incentivos</span><span class="sxs-lookup"><span data-stu-id="39eca-186">Incentives admin</span></span>|
||<span data-ttu-id="39eca-187">Administrador de perfis de negócios</span><span class="sxs-lookup"><span data-stu-id="39eca-187">Business profile admin</span></span>|
||<span data-ttu-id="39eca-188">Administrador de indicações</span><span class="sxs-lookup"><span data-stu-id="39eca-188">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="39eca-189">Gerenciar associação do MPN e sua empresa (funções não pertencentes ao AAD: essas funções gerenciam os negócios da empresa em vez do locatário)</span><span class="sxs-lookup"><span data-stu-id="39eca-189">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="39eca-190">**Função**</span><span class="sxs-lookup"><span data-stu-id="39eca-190">**Role**</span></span> | <span data-ttu-id="39eca-191">**O que você pode fazer**</span><span class="sxs-lookup"><span data-stu-id="39eca-191">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="39eca-192">Administrador de parceiros do MPN</span><span class="sxs-lookup"><span data-stu-id="39eca-192">MPN partner admin</span></span>|<span data-ttu-id="39eca-193">\*    Ver, criar e gerenciar solicitações de serviço de parceiros</span><span class="sxs-lookup"><span data-stu-id="39eca-193">\*    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="39eca-194">\*    Ver perfis jurídico, empresarial, de negócios e do MPN</span><span class="sxs-lookup"><span data-stu-id="39eca-194">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="39eca-195">\*    Ver detalhes do usuário e seus dados de habilidades</span><span class="sxs-lookup"><span data-stu-id="39eca-195">\*    View user details and their skills data</span></span>
||<span data-ttu-id="39eca-196">\*    Ver competências</span><span class="sxs-lookup"><span data-stu-id="39eca-196">\*    View competencies</span></span>
||<span data-ttu-id="39eca-197">\*    Ver e gerenciar benefícios</span><span class="sxs-lookup"><span data-stu-id="39eca-197">\*    View and manage benefits</span></span>
||<span data-ttu-id="39eca-198">\*    Ver e comprar ofertas do MPN</span><span class="sxs-lookup"><span data-stu-id="39eca-198">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="39eca-199">\*    Ver histórico de pedidos de ofertas e faturas do MPN</span><span class="sxs-lookup"><span data-stu-id="39eca-199">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="39eca-200">\*    Ver dados do indicador de contribuição de parceiros</span><span class="sxs-lookup"><span data-stu-id="39eca-200">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="39eca-201">\*    Pode funcionar na ferramenta de validação de comprovantes</span><span class="sxs-lookup"><span data-stu-id="39eca-201">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="39eca-202">\*    Ver análises de dados do cliente</span><span class="sxs-lookup"><span data-stu-id="39eca-202">\*    View customer data analytics</span></span>
||<span data-ttu-id="39eca-203">\*    Ver outras funções de usuário dentro da empresa, mas não atribuir funções</span><span class="sxs-lookup"><span data-stu-id="39eca-203">\*    View other user roles within company, but can't assign roles</span></span>
||<span data-ttu-id="39eca-204">\*    Criar tíquetes de suporte para o Partner Center</span><span class="sxs-lookup"><span data-stu-id="39eca-204">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="39eca-205">\*    Ver os tíquetes de suporte do parceiro que você criar</span><span class="sxs-lookup"><span data-stu-id="39eca-205">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="39eca-206">Administrador de conta</span><span class="sxs-lookup"><span data-stu-id="39eca-206">Account admin</span></span>| <span data-ttu-id="39eca-207">Adicionar locais</span><span class="sxs-lookup"><span data-stu-id="39eca-207">Add locations</span></span>
|| <span data-ttu-id="39eca-208">Gerenciar perfis relacionados às contas para as quais você é administrador</span><span class="sxs-lookup"><span data-stu-id="39eca-208">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="39eca-209">\*    Atribuir funções aos usuários do locatário para funções não pertencentes ao AAD</span><span class="sxs-lookup"><span data-stu-id="39eca-209">\*    Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="39eca-210">\*    Registrar locais em programas</span><span class="sxs-lookup"><span data-stu-id="39eca-210">\*    Enroll locations into programs</span></span>
||<span data-ttu-id="39eca-211">\*    Criar tíquetes de suporte para o Partner Center</span><span class="sxs-lookup"><span data-stu-id="39eca-211">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="39eca-212">\*    Ver os tíquetes de suporte do parceiro que você criar</span><span class="sxs-lookup"><span data-stu-id="39eca-212">\*    View partner support tickets you create</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="39eca-213">Gerenciar indicações</span><span class="sxs-lookup"><span data-stu-id="39eca-213">Manage referrals</span></span> 

|<span data-ttu-id="39eca-214">**Função**</span><span class="sxs-lookup"><span data-stu-id="39eca-214">**Role**</span></span>|<span data-ttu-id="39eca-215">**O que você pode fazer**</span><span class="sxs-lookup"><span data-stu-id="39eca-215">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="39eca-216">Administrador de indicações</span><span class="sxs-lookup"><span data-stu-id="39eca-216">Referrals admin</span></span>       |<span data-ttu-id="39eca-217">\* Ver, criar e gerenciar perfis de negócios</span><span class="sxs-lookup"><span data-stu-id="39eca-217">\*    View, create, and manage business profiles</span></span>
||<span data-ttu-id="39eca-218">\*    Receber e gerenciar indicações</span><span class="sxs-lookup"><span data-stu-id="39eca-218">\*    Receive and manage referrals</span></span>
||<span data-ttu-id="39eca-219">\* Ver, criar e gerenciar as indicações de venda conjunta</span><span class="sxs-lookup"><span data-stu-id="39eca-219">\* View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="39eca-220">\*    Ver, criar e gerenciar solicitações de serviço de parceiros</span><span class="sxs-lookup"><span data-stu-id="39eca-220">\*    View, create, and manage partner service requests</span></span>
|<span data-ttu-id="39eca-221">Administrador de perfis de negócios</span><span class="sxs-lookup"><span data-stu-id="39eca-221">Business profile admin</span></span>   |<span data-ttu-id="39eca-222">\* Ver, criar e gerenciar perfis de negócios</span><span class="sxs-lookup"><span data-stu-id="39eca-222">\* View, create, and manage business profile</span></span> 
||<span data-ttu-id="39eca-223">\*    Ver, criar e gerenciar solicitações de serviço de parceiros</span><span class="sxs-lookup"><span data-stu-id="39eca-223">\*    View, create, and manage partner service requests</span></span>
||<span data-ttu-id="39eca-224">\*    Criar tíquetes de suporte para o Partner Center</span><span class="sxs-lookup"><span data-stu-id="39eca-224">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="39eca-225">\*    Ver os tíquetes de suporte do parceiro que você criar</span><span class="sxs-lookup"><span data-stu-id="39eca-225">\*    View partner support tickets you create</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="39eca-226">Gerenciar incentivos</span><span class="sxs-lookup"><span data-stu-id="39eca-226">Manage incentives</span></span> 

|<span data-ttu-id="39eca-227">**Função**</span><span class="sxs-lookup"><span data-stu-id="39eca-227">**Role**</span></span> | <span data-ttu-id="39eca-228">**O que você pode fazer**</span><span class="sxs-lookup"><span data-stu-id="39eca-228">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="39eca-229">Administrador de incentivos</span><span class="sxs-lookup"><span data-stu-id="39eca-229">Incentives admin</span></span>|<span data-ttu-id="39eca-230">\*    Iniciar e gerenciar incentivos</span><span class="sxs-lookup"><span data-stu-id="39eca-230">\*    Initiates and manages incentives</span></span> 
||<span data-ttu-id="39eca-231">\*    Ver e editar todos os aspectos dos programas de incentivos</span><span class="sxs-lookup"><span data-stu-id="39eca-231">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="39eca-232">\*    Ver e editar detalhes bancários e fiscais</span><span class="sxs-lookup"><span data-stu-id="39eca-232">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="39eca-233">\*    Ver lucros de reembolso e de cooperação</span><span class="sxs-lookup"><span data-stu-id="39eca-233">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="39eca-234">\*    Acessar suporte</span><span class="sxs-lookup"><span data-stu-id="39eca-234">\*    Access support</span></span>
||<span data-ttu-id="39eca-235">\*    Disputar pagamentos de incentivos</span><span class="sxs-lookup"><span data-stu-id="39eca-235">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="39eca-236">Usuário de incentivos</span><span class="sxs-lookup"><span data-stu-id="39eca-236">Incentives user</span></span>|<span data-ttu-id="39eca-237">\*    Ver programas de incentivos</span><span class="sxs-lookup"><span data-stu-id="39eca-237">\*    Can view incentives programs</span></span>
||<span data-ttu-id="39eca-238">\*    Ver e iniciar reivindicações de incentivos</span><span class="sxs-lookup"><span data-stu-id="39eca-238">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="39eca-239">\*    Ver lucros de reembolso e de cooperação</span><span class="sxs-lookup"><span data-stu-id="39eca-239">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="39eca-240">\*    Criar tíquetes de suporte para o Partner Center</span><span class="sxs-lookup"><span data-stu-id="39eca-240">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="39eca-241">\*    Ver os tíquetes de suporte do parceiro que você criar</span><span class="sxs-lookup"><span data-stu-id="39eca-241">\*    View partner support tickets you create</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="39eca-242">Exibir dados de Insights do Partner Center</span><span class="sxs-lookup"><span data-stu-id="39eca-242">View Partner Center Insights data</span></span>

|<span data-ttu-id="39eca-243">**Função**</span><span class="sxs-lookup"><span data-stu-id="39eca-243">**Role**</span></span> | <span data-ttu-id="39eca-244">**O que você pode fazer**</span><span class="sxs-lookup"><span data-stu-id="39eca-244">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="39eca-245">Visualizador de relatórios executivos</span><span class="sxs-lookup"><span data-stu-id="39eca-245">Executive report viewer</span></span>|<span data-ttu-id="39eca-246">Acessar todos os conjuntos de dados dos relatórios, criar tíquetes de suporte do parceiro, ver os tíquetes de suporte do parceiro que você criar</span><span class="sxs-lookup"><span data-stu-id="39eca-246">Access to all reporting datasets, create partner support tickets, view partner support tickets you create</span></span>|
|<span data-ttu-id="39eca-247">Visualizador de relatórios</span><span class="sxs-lookup"><span data-stu-id="39eca-247">Report viewer</span></span>|<span data-ttu-id="39eca-248">Acessar relatórios de dados com exceção de receita e dados pessoais de clientes e funcionários, criar tíquetes de suporte do parceiro, ver os tíquetes de suporte do parceiro que você criar</span><span class="sxs-lookup"><span data-stu-id="39eca-248">Access to data reports with exception of revenue and customer and employee personal data, create partner support tickets, view partner support tickets you create</span></span>|












                                    
