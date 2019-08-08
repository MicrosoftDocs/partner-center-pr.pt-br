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
# <a name="assign-users-roles-and-permissions"></a>Atribuir funções e permissões de usuário


Você configurou seu perfil de parceiro, incluindo nome legal e endereço, detalhes de suporte, isenções de imposto sobre o arquivo, informações bancárias e o contato principal para sua empresa. Próxima etapa: Configure seus usuários com senhas e funções para que eles possam começar a trabalhar no Partner Center com você.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Configurar seus funcionários para trabalhar no Partner Center

Você determina os tipos de acesso que os usuários têm ao Partner Center pelas funções e permissões que você lhes dá. As funções estão relacionadas aos programas nos quais sua empresa está envolvida. Por exemplo, se sua empresa for um negócio CSP (provedor de soluções na nuvem), você não terá apenas as funções de gerenciamento de locatário padrão do Azure AD, como o administrador global, mas precisará de funções específicas para o programa CSP. Cada programa tem funções específicas para ele.

>[!Note]
> As funções de locatário do Azure Active Directory (AAD) incluem administrador global, administrador de usuário e funções de CSP. As funções que não são do AAD são aquelas que não gerenciam o locatário e incluem administrador de MPN, administrador de perfil de negócios, administrador de referência, administrador de incentivos e usuário de incentivo. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Gerenciar transações comerciais no Partner Center (funções do Azure AD e CSP)

|**Cargo**|**O que eles podem fazer**|
|----------------------------------|:---------------------------------|
|Administração global|• Pode acessar todos os conta Microsoft/serviços com privilégios totais
|      |• Criar tíquetes de suporte para o Partner Center
||• Exibir contratos, listas de preços e ofertas
||• Exibir, criar e gerenciar usuários parceiros|
||  Exibir, criar e gerenciar a cobrança, as notas fiscais e os arquivos reconhecimento
|Administrador de gerenciamento de usuário   | • Exibir, criar e gerenciar usuários
||• Exibir todos os perfis de parceiro
||• Exibir, criar e gerenciar usuários parceiros  |
|Administrador de cobrança | -Exibir, criar e gerenciar a cobrança, as notas fiscais e os arquivos reconhecimento|
|Usuário padrão|  Exibir meu perfil   |
|Agente administrador | • Gerenciamento de clientes
||• Adicionar a lista de dispositivos ao Partner Center
||• Criar e aplicar perfis a dispositivos
||• Gerenciamento de assinatura
||• Serviço de integridade e solicitações de serviço para clientes
||• Solicitar privilégios de administrador delegado
||• Exibir preços e ofertas
||• Cobrança
||• Administrar em nome de um cliente
||• Registrar um revendedor de valor agregado|
|Agente de vendas | • Gerenciamento de clientes
||• Adicionar a lista de dispositivos ao Partner Center
||• Gerenciamento de assinatura
||• Exibir listas de preços e ofertas
||• Exibir tíquetes de suporte
||• Solicitar uma relação com um cliente
||• Gerenciar clientes potenciais do cliente
||• Exibir o contrato do cliente
||• Registrar um revendedor de valor agregado|
|Agente de suporte técnico| • Pesquisar e exibir um cliente
||• Editar detalhes do cliente
||• Ajudar a resolver problemas do cliente com gerenciamento de assinaturas ou cobrança
||• Solicitar suporte em nome dos clientes (Observação: Você deve ser um agente de administração para concluir esta tarefa para assinaturas do Office 365)
||• Gerenciar assinaturas e problemas de cobrança em nome dos clientes (Observação: Você deve ser um agente de administração para concluir esta tarefa para assinaturas do Office 365)|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a>Fornecedor do painel de controle (CPV). (Função CSP e função não AAD)
CPVs desenvolva aplicativos para uso por parceiros do CSP (provedor de soluções na nuvem) para permitir que eles integrem seus sistemas com as APIs do Partner Center. 

|**Cargo**   |**O que você pode fazer**|
|------------------------------|:----------------------------|
|Administração global| Exibir e gerenciar seu perfil do CPV|
||Exibir e gerenciar qualquer um dos seus usuários que precisam de acesso aos recursos do CPV|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a>Usuário convidado (deve ser adicionado ao locatário do AAD)

|**Usuário convidado**   | **Papéis**|
|---------------------------|:--------------------|
||Administrador de parceiros do MPN|
||Administrador de contas|
||Administrador de incentivos|
||Administrador de perfis de negócios|
||Administrador de referências|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a>Gerenciar associação do MPN e sua empresa (funções não AAD: essas funções gerenciam o negócio da empresa em vez do locatário)

|**Cargo** | **O que você pode fazer**|
|----------------------------|:----------------------------|
|Administrador de parceiros do MPN|• Exibir, criar e gerenciar solicitações de serviço de parceiro||
||• Exibir perfis legais, de empresa, de negócios e de MPN
||• Exibir detalhes do usuário e seus dados de habilidades
||• Exibir competências
||• Exibir e gerenciar benefícios
||• Exibir e adquirir ofertas de MPN
||• Exibir MPN oferece histórico de pedidos e faturas
||• Exibir dados do indicador de contribuição de parceiro
||• Pode funcionar na ferramenta de validação de comprovante|
||-Exibir análise de dados do cliente
|| Exibir outras funções de usuário na empresa, mas não pode atribuir funções
|Administrador da conta| Adicionar locais
|| Gerenciar perfis relacionados às contas para as quais você é administrador 
||• Atribuir funções para usuários no locatário a funções não AAD 
||• Registrar locais em programas


## <a name="manage-referrals"></a>Gerenciar referências 

|**Cargo**|**O que você pode fazer**|
|-----------------------------|:------------------------|
|Administrador de referências       |• Exibir, criar e gerenciar perfis de negócios
||• Receber e gerenciar referências
||• Exibir, criar e gerenciar as referências de venda conjunta|
||• Exibir, criar e gerenciar solicitações de serviço de parceiro
|Administrador de perfis de negócios   |• Exibir, criar e gerenciar perfil de negócios 
||• Exibir, criar e gerenciar solicitações de serviço de parceiro|

## <a name="manage-incentives"></a>Gerenciar incentivos 

|**Cargo** | **O que você pode fazer**|
|------------------------------|:-------------------------|
|Administrador de incentivos|• Inicia e gerencia incentivos 
||• Pode exibir e editar todos os aspectos dos programas de incentivos
||• Pode exibir e editar os detalhes do banco e do imposto
||• Exibir descontos e ganhos de cooperação
||• Suporte ao Access
||• Testar os pagamentos de incentivos|
|Usuário de incentivos|• Pode exibir programas de incentivos
||• Pode exibir e iniciar declarações de incentivos
||• Exibir descontos e ganhos de cooperação
||• Suporte ao Access












