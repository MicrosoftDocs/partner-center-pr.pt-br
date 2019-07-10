---
title: Atribuir funções e permissões de usuários | Partner Center
ms.topic: article
ms.date: 3/5/19
description: Todos os funcionários que precisam para trabalhar no Partner Center devem ser atribuído a uma função.
author: LauraBrenner
ms.author: labrenne
keywords: funções, permissões, administrador, agente
ms.localizationpriority: medium
ms.openlocfilehash: 658106548596a5fa7d02d29c0065a23caeacb83d
ms.sourcegitcommit: 59825cb626e12dfe5eb2d28e836b4573368d705e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2019
ms.locfileid: "67690848"
---
# <a name="assign-users-roles-and-permissions"></a>Atribuir funções e permissões de usuário


Você configurou o perfil de parceiro, incluindo nome legal e endereço, detalhes de suporte, isenções de imposto sobre arquivos, informações bancárias e o contato principal para a sua empresa. Próxima etapa: configurar os usuários configurados com senhas e funções, para que eles possam começar a trabalhar no Partner Center com você.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Configurar seus funcionários para trabalhar no Partner Center

Os tipos de acesso que os usuários têm Partner Center, as funções e permissões que você conceda a você determinar. As funções estão relacionadas aos programas de que sua empresa está envolvida no. Por exemplo, se sua empresa é uma empresa de provedor de solução de nuvem (CSP), você não somente terá o Azure AD padrão funções de gerenciamento como administrador global do locatário, mas será necessário a funções específicas para o programa CSP. Cada programa tem funções específicas a ela.

>[!Note]
> As funções de locatário do Azure Active Directory (AAD) incluem administrador global, administrador de usuários e funções CSP. Funções do AAD não são essas funções que não gerencia o locatário e elas incluem MPN admin, administrador de perfil de negócios, administração de indicação, incentivo administrador e usuário incentivo. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Gerenciar transações comerciais no Partner Center (Azure AD e as funções do CSP)

|**Função**|**O que pode fazer**|
|----------------------------------|:---------------------------------|
|Administração global|• Podem acessar todos os Microsoft/serviços de conta com privilégios totais
|      |• Criar tíquetes de suporte para o Centro de parceiros
||• Exibir contratos, listas de preços e ofertas
||• Exibir, criar e gerenciar os usuários do parceiro|
||  Exibir, criar e gerenciar arquivos recon, faturas e cobrança
|Administrador de gerenciamento de usuário   | • Exibir, criar e gerenciar usuários
||• Exibir todos os perfis de parceiros
||• Exibir, criar e gerenciar os usuários do parceiro  |
|Administrador de cobrança | -Exibir, criar e gerenciar arquivos recon, faturas e cobrança|
|Usuário padrão|  Exibir meu perfil   |
|Agente administrador | • Gerenciamento de cliente
||• Adicionar lista de dispositivos para o Centro de parceiros
||• Criar e aplicar perfis de dispositivos
||• Gerenciamento de assinatura
||• Integridade e o serviço de solicitações de clientes
||• Solicitação delegada privilégios de administrador
||• Exibir preço e ofertas
||• Cobrança
||• Administrar em nome de um cliente
||• Registre-se um valor adicionado revendedor|
|Agente de vendas | • Gerenciamento de cliente
||• Adicionar lista de dispositivos para o Centro de parceiros
||• Gerenciamento de assinatura
||• Exibir preço de lista e oferece
||• Tíquetes de suporte de modo de exibição
||• Solicitação uma relação com um cliente
||• Gerenciar clientes potenciais
||• Exibir o contrato do cliente
||• Registre-se um revendedor de valor agregado|
|Agente de suporte técnico| • Pesquisar e exibir um cliente
||• Editar detalhes do cliente
||• Ajuda resolver problemas de cliente com o gerenciamento de cobrança ou assinatura
||• Suporte a solicitação em nome dos clientes (Observação: Você deve ser um agente de administrador para concluir essa tarefa para assinaturas do Office 365)
||• Gerenciar assinaturas e cobrança problemas em nome dos clientes (Observação: Você deve ser um agente de administrador para concluir essa tarefa para assinaturas do Office 365)|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a>Fornecedor do painel de controle (CPV). (Função do CSP e função de não-AAD)
CPVs desenvolver aplicativos para uso pelos parceiros de provedor de solução de nuvem (CSP) para que eles possam integrar seus sistemas com APIs do Partner Center. 

|**Função**   |**O que você pode fazer**|
|------------------------------|:----------------------------|
|Administração global| Exibir e gerenciar seu perfil CPV|
||Exibir e gerenciar qualquer um dos seus usuários que precisam de acesso aos recursos de CPV|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a>Usuário convidado (deve ser adicionado ao locatário do AAD)

|**Usuário convidado**   | **Funções**|
|---------------------------|:--------------------|
||Administrador de parceiros do MPN|
||Contas de administrador|
||Administrador de incentivos|
||Administrador de perfis de negócios|
||Administrador de referências|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a>Gerenciar a associação da MPN e sua empresa (funções de não-AAD: essas funções de gerenciam os negócios da empresa em vez de locatário)

|**Função** | **O que você pode fazer**|
|----------------------------|:----------------------------|
|Administrador de parceiros do MPN|• Exibir, criar e gerenciar solicitações de serviço do parceiro||
||• Exibir legal, da empresa, negócios e perfis do MPN
||• Exibir detalhes do usuário e seus dados de habilidades
||• Exibir competências
||• Exibir e gerenciar os benefícios
||Compra e o modo de exibição • o MPN oferece
||• Exibir MPN oferece notas fiscais e histórico de pedidos
||• Exibir dados de indicador de contribuição de parceiro
||• Podem trabalhar na ferramenta de validação de comprovante|
||-Exibir a análise de dados do cliente
|| Exibir outras funções de usuário dentro da empresa, mas não é possível atribuir funções
|Administrador da conta| Adicionar locais
|| Gerenciar perfis relacionados às contas que você é administrador 
||• Atribuir funções para usuários no locatário para funções do AAD não 
||• Registrar locais em programas


## <a name="manage-referrals"></a>Gerenciar indicações 

|**Função**|**O que você pode fazer**|
|-----------------------------|:------------------------|
|Administrador de referências       |• Exibir, criar e gerenciar perfis de negócios
||• Receber e gerenciar as referências
||• Exibir, criar e gerenciar as referências de venda conjunta|
||• Exibir, criar e gerenciar solicitações de serviço do parceiro
|Administrador de perfis de negócios   |• Exibir, criar e gerenciar um perfil comercial 
||• Exibir, criar e gerenciar solicitações de serviço do parceiro|

## <a name="manage-incentives"></a>Gerenciar incentivos 

|**Função** | **O que você pode fazer**|
|------------------------------|:-------------------------|
|Administrador de incentivos|• Inicia e gerencia incentivos 
||• Pode exibir e editar todos os aspectos de programas de incentivos
||• Pode exibir e editar os detalhes do banco e imposto
||• Ganhos de reembolso e cooperação do modo de exibição
||• Suporte a acesso
||• Os pagamentos incentivos de controvérsias|
|Usuário de incentivos|• Podem exibir programas incentivos
||• Pode exibir e iniciar as declarações de incentivos
||• Ganhos de reembolso e cooperação do modo de exibição
||• Suporte a acesso












