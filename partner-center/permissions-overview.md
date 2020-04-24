---
title: Atribuir funções e permissões de usuários | Partner Center
ms.topic: article
ms.date: 03/23/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba quais funções são melhores para os seus usuários que estão gerenciando transações comerciais, indicações, incentivos ou associações MPN de sua empresa.
author: LauraBrenner
ms.author: labrenne
keywords: funções, permissões, administrador, agente
ms.localizationpriority: high
ms.openlocfilehash: fbff7f353a0055aa645467fccaa049b598b4c880
ms.sourcegitcommit: 449cb8c32880217ad7543712b02a84ae69869289
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2020
ms.locfileid: "80296394"
---
# <a name="assign-users-roles-and-permissions"></a>Atribuir permissões e funções de usuários

**Funções apropriadas**
-    Administrador global
-    Administrador de usuários
-    Administrador de parceiros do MPN

Você configurou seu perfil de parceiro, incluindo a razão social, o endereço, os detalhes de suporte, as isenções de imposto sobre arquivos, as informações bancárias e o contato principal da empresa. Próxima etapa: configure as senhas e funções de seus usuários para que eles possam começar a trabalhar no Partner Center com você.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Configurar seus funcionários para trabalhar no Partner Center

Você determinará os tipos de acesso que os usuários terão ao Partner Center por meio das funções e permissões a eles atribuídas. As funções estão relacionadas aos programas com os quais a sua empresa está envolvida. Por exemplo, se a sua empresa for um CSP (Provedor de Soluções na Nuvem), você não apenas terá as funções de gerenciamento de locatário padrão do Azure AD, como o administrador global, mas também precisará de funções específicas para o programa CSP. Cada programa tem funções específicas para ele.

>[!Note]
> As funções de locatário do Azure Active Directory (AAD) incluem administrador global, administrador de usuários e funções de CSP. As funções não pertencentes ao AAD são aquelas que não gerenciam o locatário e incluem administrador do MPN, administrador de perfil de negócios, administrador de indicações, administrador de incentivos e usuário de incentivos. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Gerenciar transações comerciais no Partner Center (funções Azure AD e CSP)

|**Função**|**O que eles podem fazer**|
|----------------------------------|:---------------------------------|
|Administrador global|*    Pode acessar todas as contas/os serviços da Microsoft com todos os privilégios
|      |*    Criar tíquetes de suporte para o Partner Center
||*    Ver contratos, listas de preços e ofertas
||*    Ver, criar e gerenciar usuários parceiros|
||  • Exibir, criar e gerenciar a cobrança, as faturas e os arquivos reconhecimento
|Administrador de gerenciamento de usuário   | *    Ver, criar e gerenciar usuários
||*    Ver todos os perfis de parceiros
||*    Ver, criar e gerenciar usuários parceiros  |
|Administrador de cobrança | – Exibir, criar e gerenciar a cobrança, as faturas e os arquivos reconhecimento|
|Usuário padrão|  Exibir meu perfil   |
|Agente administrativo | *    Gerenciamento de clientes
||*    Adicionar lista de dispositivos ao Partner Center
||*    Criar e aplicar perfis aos dispositivos
||*    Gerenciamento de assinaturas
||*    Solicitações de integridade e de serviços para os clientes
||*    Solicitar privilégios de administrador delegado
||*    Ver preços e ofertas
||*    Cobrança
||*    Administrar em nome de um cliente
||*    Registrar um revendedor com valor agregado|
|Agente de vendas | *    Gerenciamento de clientes
||*    Adicionar lista de dispositivos ao Partner Center
||*    Gerenciamento de assinaturas
||*    Ver tíquetes de suporte
||*    Solicitar um relacionamento com um cliente
||*    Gerenciar clientes potenciais
||*    Ver o contrato do cliente
||*    Registrar um revendedor com valor agregado|
|Agente de suporte técnico| *    Pesquisar e ver um cliente
||*    Editar detalhes do cliente
||*    Ajudar a resolver problemas dos clientes com o gerenciamento de cobrança ou assinaturas
||*    Solicitar suporte em nome dos clientes 
||*    Gerenciar problemas de assinaturas e cobrança em nome dos clientes| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a>CPV (Fornecedor de Painel de Controle). (Função CSP e função não pertencente ao AAD)
Os CPVs desenvolvem aplicativos para uso por parceiros CSP (Provedor de Soluções na Nuvem) a fim de permitir que eles integrem seus sistemas com as APIs do Partner Center. 

|**Função**   |**O que você pode fazer**|
|------------------------------|:----------------------------|
|Administrador global| Exibir e gerenciar seu perfil de CPV|
||Exibir e gerenciar todos os seus usuários que precisam de acesso aos recursos de CPV|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a>Usuário convidado (deve ser adicionado ao locatário do AAD)

|**Usuário convidado**   | **Funções**|
|---------------------------|:--------------------|
||Administrador de parceiros do MPN|
||Administrador de contas|
||Administrador de incentivos|
||Administrador de perfis de negócios|
||Administrador de indicações|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a>Gerenciar associação do MPN e sua empresa (funções não pertencentes ao AAD: essas funções gerenciam os negócios da empresa em vez do locatário)

|**Função** | **O que você pode fazer**|
|----------------------------|:----------------------------|
|Administrador de parceiros do MPN|*    Ver, criar e gerenciar solicitações de serviço de parceiros||
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
|Administrador de conta| Adicionar locais
|| Gerenciar perfis relacionados às contas para as quais você é administrador 
||*    Atribuir funções aos usuários do locatário para funções não pertencentes ao AAD 
||*    Registrar locais em programas


## <a name="manage-referrals"></a>Gerenciar indicações 

|**Função**|**O que você pode fazer**|
|-----------------------------|:------------------------|
|Administrador de indicações       |* Ver, criar e gerenciar perfis de negócios
||*    Receber e gerenciar indicações
||* Ver, criar e gerenciar as indicações de venda conjunta|
||*    Ver, criar e gerenciar solicitações de serviço de parceiros
|Administrador de perfis de negócios   |* Ver, criar e gerenciar perfis de negócios 
||*    Ver, criar e gerenciar solicitações de serviço de parceiros|

## <a name="manage-incentives"></a>Gerenciar incentivos 

|**Função** | **O que você pode fazer**|
|------------------------------|:-------------------------|
|Administrador de incentivos|*    Iniciar e gerenciar incentivos 
||*    Ver e editar todos os aspectos dos programas de incentivos
||*    Ver e editar detalhes bancários e fiscais
||*    Ver lucros de reembolso e de cooperação
||*    Acessar suporte
||*    Disputar pagamentos de incentivos|
|Usuário de incentivos|*    Ver programas de incentivos
||*    Ver e iniciar reivindicações de incentivos
||*    Ver lucros de reembolso e de cooperação
||*    Acessar suporte

## <a name="view-partner-center-insights-data"></a>Exibir dados de Insights do Partner Center

|**Função** | **O que você pode fazer**|
|------------------------------|:-------------------------|
|Visualizador de relatórios executivos|Acesso a todos os conjuntos de dados de relatórios|
|Visualizador de relatórios|Acesso a relatórios de dados com exceção de receita e dados pessoais de clientes e funcionários|












                                    