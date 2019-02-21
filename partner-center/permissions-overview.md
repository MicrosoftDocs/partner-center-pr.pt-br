---
title: Atribuir funções de usuários e permissões | Partner Center
ms.topic: article
ms.date: 10/29/2018
description: Todos os funcionários que precisam trabalhar no Partner Center devem ser atribuído a uma função.
author: labrenne
ms.author: labrenne
keywords: funções, permissões, administrador, agente
ms.localizationpriority: medium
ms.openlocfilehash: d811cb76b03b1784eaf926052e6a00151b2fc347
ms.sourcegitcommit: bfbb5b5edb381e219134be5a3e4a97bfe232288f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "9086724"
---
# <a name="assign-users-roles-and-permissions"></a>Atribuir funções e permissões de usuário


Você configurou seu perfil de parceiro, incluindo o nome legal e endereço, detalhes de suporte, isenções de impostos, informações bancárias e o contato principal para sua empresa. Próxima etapa: obter os usuários configurado com senhas e funções, portanto, eles podem começar a trabalhar no Partner Center com você.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Configurar seus funcionários para trabalhar no Partner Center

Determinar os tipos de acesso que os usuários tenham Partner Center, as funções e permissões que dar a eles. Funções estão relacionadas à programas em que sua empresa está envolvida em. Por exemplo, se sua empresa é uma empresa de provedor de soluções na nuvem (CSP), você não terá apenas o Azure AD padrão funções de gerenciamento, como o administrador global do locatário, mas será necessário funções específicas ao programa CSP. Cada programa tem funções específicas a ela.

>[!Note]
> Funções de locatário do Azure Active Directory (AAD) incluem o administrador global, administrador de usuários e funções do CSP. Funções do AAD não incluem administrador MPN, administrador de perfil de negócios, administrador de indicações, administrador de incentivos e usuário de incentivos. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Gerenciar transações comerciais no Partner Center (Azure AD e funções do CSP)

|**Função**|**O que eles podem fazer**|
|----------------------------------|:---------------------------------|
|Administração global|• Pode acessar todas as contas/serviços da Microsoft com todos os privilégios
|      |• Criar tíquetes de suporte para o Partner Center
||• Exibir contratos, listas de preços e ofertas
||• Exibir, criar e gerenciar usuários de parceiros|
|Administrador de usuários   | • Exibir, criar e gerenciar usuários
||• Exibir todos os perfis de parceiros
||• Exibir, criar e gerenciar usuários de parceiros  |
|Usuário padrão|  Exibir meu perfil   |
|Agente administrativo | • Gerenciamento de cliente
||• Adicionar lista de dispositivos para o Center< de parceiro
||• Criar e aplicar perfis aos dispositivos
||• Gerenciamento de assinaturas
||• Serviço solicitações de integridade e para clientes
||• Solicitar privilégios de administrador
||• Exibir preços e ofertas
||• A cobrança
||• Administrar em nome do cliente
||• Registrar um valor bom revendedor|
|Agente de vendas | • Gerenciamento de cliente
||• Adicionar lista de dispositivos ao Partner Center
||• Gerenciamento de assinaturas
||• Exibir tíquetes de suporte
||• Solicitar um relacionamento com um cliente
||• Gerenciar as oportunidades de cliente
||• Exibir o contrato do cliente
||• Registrar um revendedor|
|Agente de suporte técnico| • Pesquisar e exibir um cliente
||• Editar detalhes do cliente
||• Ajudam a resolver problemas do cliente com o gerenciamento de cobrança ou assinatura
||• Solicitação de suporte em nome dos clientes (Observação: você deve ser um agente administrador para concluir essa tarefa para assinaturas do Office 365)
||• Gerenciar assinaturas e serviços em nome dos clientes (Observação: você deve ser um agente administrador para concluir essa tarefa para assinaturas do Office 365)|
|
### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a>Fornecedor do painel de controle (CPV). (Funções de CSP e não AAD)
CPVs desenvolver aplicativos para uso por parceiros de provedor de soluções na nuvem (CSP) para habilitá-los integrar seus sistemas com APIs do Partner Center. 

|**Função**   |**Você pode fazer**|
|------------------------------|:----------------------------|
|Administração global| Exibir e gerenciar seu perfil CPV|
||Exibir e gerenciar qualquer um dos seus usuários que precisam de acesso a recursos CPV|

## <a name="manage-mpn-membership-and-your-company-non-aad-roles"></a>Gerenciar a associação à MPN e a sua empresa (funções não AAD)

|**Função** | **Você pode fazer**|
|----------------------------|:----------------------------|
|Administrador do MPN|•CAN adicionar usuários não locatário
||• Exibir, criar e gerenciar solicitações de serviço do parceiro
||• Exibição legal, organização, empresas e perfis do MPN
||• Exibir detalhes do usuário e seus dados de habilidades
||• Exibir competências
||• Exibir e gerenciar benefícios
||• Exibição e compra de ofertas do MPN
||• Exibição MPN histórico de pedidos e faturas de ofertas
||• Pode exibir dados de contribuição de parceiros
||• Podem funcionar na ferramenta de validação de comprovantes|
|Conta de administrador| • Pode adicionar usuários não locatário
||• Adicionar ou excluir locais
||-Gerenciar perfis relacionados às contas de que administrador para você são 
||• Atribuir funções para os usuários de locatário às funções não AAD 
||• Se inscrever locais em programas

## <a name="manage-referrals-non-aad-roles"></a>Gerenciar indicações (funções não AAD)

|**Função**|**Você pode fazer**|
|-----------------------------|:------------------------|
|Administrador de indicações       |• Exibir, criar e gerenciar perfis de negócios
||• Receber e gerenciar indicações
||• Exibir, criar e gerenciar solicitações de serviço do parceiro|
|Administrador de perfis de negócios   |•View, criar e gerenciar perfil de negócios 
||• Exibir, criar e gerenciar solicitações de serviço do parceiro|

## <a name="manage-incentives--non-aad-roles"></a>Gerencie incentivos (funções não AAD)

|**Função** | **Você pode fazer**|
|------------------------------|:-------------------------|
|Administrador de incentivos|• Inicia e gerencia incentivos 
||• Pode exibir e editar todos os aspectos de programas de incentivos
||• Pode exibir e editar detalhes bancários e fiscais
||• Lucros de reembolso e cooperação do modo de exibição
||• Suporte de acesso
||Pagamentos de incentivos disputa •|
|Usuário de incentivos|• Pode exibir programas de incentivos
||• Pode exibir e iniciar declarações de incentivos
||• Lucros de reembolso e cooperação do modo de exibição
||• Lucros de reembolso e cooperação do modo de exibição
||• Suporte de acesso












