---
title: Atribuir funções e permissões a usuários
ms.topic: article
ms.date: 09/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba quais funções são melhores para os usuários da sua empresa que gerenciam transações comerciais, indicações, incentivos ou associações MPN no Partner Center.
author: hemas
ms.author: hemas
ms.localizationpriority: high
ms.custom: SEOMAY.20, contperfq1
ms.openlocfilehash: 32df86887ccbea5d18d1bd8c7c34add2b1ab60e4
ms.sourcegitcommit: 940dad4527f51781f6f966e196b3aa08389613a2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/13/2020
ms.locfileid: "92006806"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a>Atribuir permissões e funções de usuários para os usuários de uma empresa que precisam trabalhar no Partner Center

**Funções apropriadas**

- Administrador global
- Administrador de usuários
- Administrador de parceiros do MPN

Você configurou seu perfil de parceiro, incluindo a razão social, o endereço, os detalhes de suporte, as isenções de imposto sobre arquivos, as informações bancárias e o contato principal da empresa. Próxima etapa: Configure as senhas e funções dos seus usuários para que eles possam começar a trabalhar no Partner Center com você.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Configurar seus funcionários para trabalhar no Partner Center

Você determinará os tipos de acesso que os usuários terão ao Partner Center por meio das funções e permissões a eles atribuídas. As funções estão relacionadas aos programas com os quais a sua empresa está envolvida. Por exemplo, se a sua empresa for um CSP (Provedor de Soluções na Nuvem), você não apenas terá as funções de gerenciamento de locatário padrão do Azure Active Directory, como o administrador global, mas também precisará de funções específicas para o programa CSP. Cada programa tem funções específicas para ele.

>[!Note]
> As funções de locatário do Azure Active Directory incluem administrador global, administrador de usuários e funções de CSP. As funções não pertencentes ao Azure Active Directory são aquelas que não gerenciam o locatário e incluem administrador do MPN, administrador de perfil de negócios, administrador de indicações, administrador de incentivos e usuário de incentivos. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Gerenciar transações comerciais no Partner Center (funções Azure AD e CSP)

|**Função**|**O que eles podem fazer**|**Saiba mais**|
|----------------------------------|---|:---------------------------------|
|Administrador global|*    Pode acessar todas as contas/os serviços da Microsoft com todos os privilégios|[Gerenciar sua conta do Partner Center](partner-center-account-setup.md)
|      |*    Criar tíquetes de suporte para o Partner Center
||*    Ver os tíquetes de suporte do parceiro que você criar
||*    Ver contratos, listas de preços e ofertas
||*    Ver, criar e gerenciar usuários parceiros|
||  • Exibir, criar e gerenciar a cobrança, as faturas e os arquivos reconhecimento
|Administrador de gerenciamento de usuário   | *    Ver, criar e gerenciar usuários|[Gerenciar as suas ofertas e benefícios de associação ao Microsoft Partner Network no Partner Center](manage-your-partner-network-benefits.md)
||*    Ver todos os perfis de parceiros
||*    Criar tíquetes de suporte para o Partner Center
||*    Ver os tíquetes de suporte do parceiro que você criar
|Administrador de cobrança | – Exibir, criar e gerenciar a cobrança, as faturas e os arquivos reconhecimento|[Ler sua fatura](billing.md)
||*    Exibir preço
||*    Criar tíquetes de suporte para o Partner Center
||*    Ver os tíquetes de suporte do parceiro que você criar
|Usuário padrão|  Exibir meu perfil   |[Redefinir sua senha](reset-my-pasword.md)
|Agente administrativo | *    Gerenciamento de clientes|[Conectar-se com seus clientes](connect-with-your-customers.md)
||*    Adicionar lista de dispositivos ao Partner Center
||*    Criar e aplicar perfis aos dispositivos
||*    Gerenciamento de assinaturas
||*    Solicitações de integridade e de serviços para os clientes
||*    Solicitar privilégios de administrador delegado
||*    Ver preços e ofertas
||*    Cobrança
||*    Administrar em nome de um cliente
||*    Registrar um revendedor com valor agregado
||*    Criar tíquetes de suporte para o Partner Center
||*    Ver os tíquetes de suporte do parceiro que você criar|
|Agente de vendas | *    Gerenciamento de clientes|[Fornecer suporte a cobrança para seus clientes e ajudar a responder às perguntas deles sobre cobrança](provide-billing-support.md)
||*    Adicionar lista de dispositivos ao Partner Center
||*    Gerenciamento de assinaturas
||*    Ver tíquetes de suporte
||*    Solicitar um relacionamento com um cliente
||*    Ver preços e ofertas
||*    Gerenciar clientes potenciais
||*    Ver o contrato do cliente
||*    Registrar um revendedor com valor agregado
||*    Criar tíquetes de suporte para o Partner Center
||*    Ver os tíquetes de suporte do parceiro que você criar|
|Agente de suporte técnico| *    Pesquisar e ver um cliente|[Escale problemas para a Microsoft e saiba quais problemas são mais adequados ao escalonamento para a Microsoft](escalate-problems-to-microsoft.md)
||*    Editar detalhes do cliente
||*    Ajudar a resolver problemas dos clientes com o gerenciamento de cobrança ou assinaturas
||*    Solicitar suporte em nome dos clientes 
||*    Gerenciar problemas de assinaturas e cobrança em nome dos clientes
||*    Criar tíquetes de suporte para o Partner Center
||*    Ver os tíquetes de suporte do parceiro que você criar| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-azure-ad-role"></a>CPV (Fornecedor de Painel de Controle). (Função CSP e função não pertencente ao Azure AD)

Os CPVs desenvolvem aplicativos para uso por parceiros CSP (Provedor de Soluções na Nuvem) a fim de permitir que eles integrem seus sistemas com as APIs do Partner Center. 

|**Função**   |**O que você pode fazer**|**Saiba mais**|
|------------------------------|:----------------------------|----|
|Administrador global| Exibir e gerenciar seu perfil de CPV|[Inscreva-se como um Fornecedor de Painel de Controle para ajudar a integrar sistemas de parceiros CSP com as APIs do Partner Center](enroll-as-cpv.md)
||Exibir e gerenciar todos os seus usuários que precisam de acesso aos recursos de CPV|

### <a name="guest-user-must-be-added-to-the-azure-active-directory-tenant"></a>Usuário convidado (precisa ser adicionado ao locatário do Azure Active Directory)

|**Usuário convidado**   | **Funções**|
|---------------------------|:--------------------|
||Administrador de parceiros do MPN|
||Administrador de contas|
||Administrador de incentivos|
||Administrador de perfis de negócios|
||Administrador de indicações|


## <a name="manage-mpn-membership-and-your-company"></a>Gerenciar a associação do MPN e sua empresa 

Essas funções não são funções do Azure Active Directory. Essas funções gerenciam o negócio da empresa em vez do locatário.

|**Função** | **O que você pode fazer**|**Saiba mais**|
|----------------------------|:----------------------------|-----|
|Administrador de parceiros do MPN|*    Ver, criar e gerenciar solicitações de serviço de parceiros|[Comprar ou renovar uma assinatura do Microsoft Action Pack ou as competências silver e gold](mpn-get-action-pack.md)
||*    Ver perfis jurídico, empresarial, de negócios e do MPN
||*    Ver detalhes do usuário e seus dados de habilidades
||*    Ver competências
||*    Ver e gerenciar benefícios
||*    Ver e comprar ofertas do MPN
||*    Ver histórico de pedidos de ofertas e faturas do MPN
||*    Ver dados do indicador de contribuição de parceiros
||*    Pode funcionar na ferramenta de validação de comprovantes|
||*    Ver análises de dados do cliente
||*    Ver outras funções de usuário dentro da empresa, mas não atribuir funções
||*    Criar tíquetes de suporte para o Partner Center
||*    Ver os tíquetes de suporte do parceiro que você criar
|Administrador de conta| Adicionar locais|[Gerenciar locais](manage-locations.md)
|| Gerenciar perfis relacionados às contas para as quais você é administrador 
||*    Atribuir funções para usuários no locatário a funções não pertencentes ao Azure Active Directory 
||*    Registrar locais em programas
||*    Criar tíquetes de suporte para o Partner Center
||*    Ver os tíquetes de suporte do parceiro que você criar


## <a name="manage-referrals"></a>Gerenciar indicações 

|**Função**|**O que você pode fazer**|**Saiba mais**|
|-----------------------------|:------------------------|---|
|Administrador de indicações       |* Ver, criar e gerenciar perfis de negócios|[Gerenciar vendas potenciais diferentes, como consultas de clientes, clientes potenciais qualificados por marketing e clientes potenciais qualificados por vendas](manage-leads.md)
||*    Receber e gerenciar indicações
||* Ver, criar e gerenciar as indicações de venda conjunta|
||*    Ver, criar e gerenciar solicitações de serviço de parceiros
|Administrador de perfis de negócios   |* Ver, criar e gerenciar perfis de negócios |[Criar um perfil de negócios](create-a-marketing-profile.md)
||*    Ver, criar e gerenciar solicitações de serviço de parceiros
||*    Criar tíquetes de suporte para o Partner Center
||*    Ver os tíquetes de suporte do parceiro que você criar|

## <a name="manage-incentives"></a>Gerenciar incentivos 

|**Função** | **O que você pode fazer**|**Saiba mais**
|------------------------------|:-------------------------|---|
|Administrador de incentivos|*    Iniciar e gerenciar incentivos |[Use estes recursos como incentivos para ajudá-lo a começar](incentives-get-started-intro.md)
||*    Ver e editar todos os aspectos dos programas de incentivos
||*    Ver e editar detalhes bancários e fiscais
||*    Ver lucros de reembolso e de cooperação
||*    Acessar suporte
||*    Disputar pagamentos de incentivos|
|Usuário de incentivos|*    Ver programas de incentivos
||*    Ver e iniciar reivindicações de incentivos
||*    Ver lucros de reembolso e de cooperação
||*    Criar tíquetes de suporte para o Partner Center
||*    Ver os tíquetes de suporte do parceiro que você criar

## <a name="view-partner-center-insights-data"></a>Exibir dados de Insights do Partner Center

|**Função** | **O que você pode fazer**|**Saiba mais**|
|------------------------------|:-------------------------|---|
|Visualizador de relatórios executivos|Acessar todos os conjuntos de dados dos relatórios, criar tíquetes de suporte do parceiro, ver os tíquetes de suporte do parceiro que você criar|[Visão geral dos relatórios do painel disponíveis em Insights do Partner Center](pci-overview-report.md)
|Visualizador de relatórios|Acessar relatórios de dados com exceção de receita e dados pessoais de clientes e funcionários, criar tíquetes de suporte do parceiro, ver os tíquetes de suporte do parceiro que você criar|

## <a name="next-steps"></a>Próximas etapas

- [Criar contas de usuário e atribuir funções e permissões](create-user-accounts-and-set-permissions.md)
- [Verifique as informações da sua conta ao se inscrever em um novo programa do Partner Center](verification-responses.md)
