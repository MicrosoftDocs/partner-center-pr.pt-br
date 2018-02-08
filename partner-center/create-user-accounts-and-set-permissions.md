---
title: "Criar contas de usuário e definir permissões | Partner Center"
description: "O administrador cria uma conta de usuário para cada funcionário de parceiro que precise acessar o Partner Center."
ms.assetid: 75D805AE-9922-4CFD-9427-196047D70963
author: MaggiePucciEvans
Keywords: roles, permissions,add user, assign role, admin, agent,
ms.openlocfilehash: 809641e488595e59beb63b0867b4758f3912106e
ms.sourcegitcommit: fc49a5e334ed37db4ff4c594ecf89a1527a3bd1d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2018
---
# <a name="create-user-accounts-and-assign-permissions"></a>Criar contas de usuário e atribuir permissões

**Aplicável a**

-  Partner Center

Criar contas de usuário para os funcionários que precisam acessar o Partner Center. Essas tarefas devem ser realizadas por um administrador com permissões de administrador do gerenciamento de usuário. 

>**Observação**<br> Agora você tem a capacidade de atribuir os usuários a três novas funções no Partner Center que ajudarão você a gerenciar seu negócio, Administrador do MPN, Administrador de perfil de negócios e Administrador de indicações. Consulte Atribuir permissões de usuário, a seguir, para obter os detalhes sobre cada função.


## <a name="add-a-new-user"></a>Adicionar um novo usuário

1. No menu **Painel**, selecione **Configurações da conta > Gerenciamento de usuário**.

2.  Selecione **Adicionar usuário**.

3.  Insira o nome completo e endereço de email exclusivo do usuário.

4.  Selecione o tipo de agente e/ou o tipo de administrador que deseja atribuir ao usuário. O acesso do Partner Center é baseado em função, portanto, você pode atribuir permissões para personalizar o modo de exibição do usuário e mostrar somente os recursos que o usuário precisa para completar tarefas específicas. Para obter mais informações sobre o que cada função pode fazer, consulte Atribuir permissões de usuário abaixo.

5.  Selecione **Adicionar** para criar a conta de usuário. Confirme os detalhes do usuário na próxima página.

>**Importante**<br>
Anote as novas informações de login do usuário exibidas nessa página. Certifique-se de copiar e enviar essas informações para o novo usuário, pois você não conseguirá acessá-las novamente mais tarde. 

O usuário precisará entrar no Partner Center com seu nome de usuário e senha temporária. Quando o usuário entrar no Partner Center pela primeira vez, ele precisará alterar sua senha. 

>**Observação**<br> Se o seu administrador global deixou a organização ou mudou de função e houver a necessidade de adicionar um novo administrador global, você terá que fazer uma solicitação de serviço no [portal MPN](https://partner.microsoft.com/support). O agente de suporte poderá solicitar a promoção de um usuário a administrador global se seu solicitante for capaz de fornecer as informações de identidade pessoal requisitadas e informações adicionais sobre a sua organização.

## <a name="assign-user-permissions"></a>Atribuir permissões de usuário

O acesso do Partner Center é baseado em função. As permissões que você atribuir a um usuário personalizam o modo de exibição do usuário para mostrar somente os recursos de que o usuário precisa para concluir suas tarefas específicas. 

Para cada usuário, você deve atribuir pelo menos um nível de permissão. Um desses níveis pode ser o nível padrão, que é **Gerencia a conta da sua organização como**. Se você não atribuir uma função a um usuário, ele não poderá trabalhar no Partner Center.

-   As permissões de agente controlam quais tipos de dados de cliente e informações de conta que o usuário pode ver e alterar.

-   Permissões de administrador controlam o nível de acesso do usuário aos recursos do Partner Center. Essa configuração tem impacto fora do Partner Center, pois um Administrador de cobrança poderá acessar as listas de todos os serviços Microsoft (mesmo aqueles não relacionados a CSP) e um Administrador global poderá acessar contas de usuário e contas de clientes além do CSP.

As categorias gerais de funções são: 

- Funções de administrador
- Funções de agente
- Funções de incentivos
- Funções de indicação e marketing

Dentro de cada uma dessas categorias gerais, um usuário pode ter apenas uma função, mas o mesmo usuário também pode ter funções nas outras categorias gerais. 

>**Importante** Se um usuário não precisar de uma função específica, deixe a designação na configuração padrão - **Gerencia a conta da sua organização como**. Os usuários devem ter atribuída pelo menos uma função para trabalhar no Partner Center.

A tabela a seguir explica o que cada função pode fazer no Partner Center. Ao pensar sobre a forma como você deseja atribuir funções, considere o trabalho que um usuário faz em sua organização. Você pode, por exemplo, desejar que o administrador global também seja o agente administrativo. A pessoa que lida com seu marketing também pode ser a pessoa que deve gerenciar o perfil de negócios.

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Função no Partner Center</strong></p></td>
<td><p><strong>O que eles podem fazer</strong></p></td>
</tr>
<tr class="odd">
<td><p><strong>Administração global</strong></p></td>
<td><ul>
<li><p>Pode acessar todas as contas/serviços da Microsoft com todos os privilégios</p></li>
<li><p>Criar tíquetes de suporte para o Partner Center</p></li>
<li><p>Exibir contratos, listas de preços e ofertas</p></li>
<li><p>Cobrança</p></li>
<li><p>Exibir, criar e gerenciar usuários de parceiros</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p><strong>Administrador de cobrança</strong></p></td>
<td><ul>
<li><p>Pode acessar todas as contas da Microsoft com todos os privilégios</p></li>
<li><p>Exibir contratos, listas de preços e ofertas</p></li>
<li><p>Cobrança</p></li>
</ul></td>
</tr>
<tr class="odd">
<td><p><strong>Administrador de gerenciamento de usuário</strong></p></td>
<td><ul>
<li><p>Exibir, criar e gerenciar usuários</p></li>
<li><p>Exibir todos os perfis de parceiros</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p><strong>Administrador de perfis de negócios</strong></p></td>
<td><ul>
<li><p>Exibir, criar e gerenciar perfil de negócios </p></li>
<li><p>Exibir, criar e gerenciar solicitações de serviço de parceiros</p></li>
</ul></td>
<tr class="odd">
<td><p><strong>Administrador de indicações </strong></p></td>
<td><ul>
<li><p>Exibir, criar e gerenciar perfis de negócios</p></li>
<li><p>Receber e gerenciar indicações</p></li>
<li><p>Exibir, criar e gerenciar solicitações de serviço de parceiros</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p><strong>Administrador de parceiros do MPN</strong></p></td>
<td><ul>
<li><p>Exibir, criar e gerenciar solicitações de serviço de parceiros</p></li>
<li><p>Exibir perfis legal, da organização, de negócios e do MPN</p></li>
<li><p>Exibir detalhes de usuário e seus dados de habilidades</p></li>
<li><p>Exibir competências</p></li>
<li><p>Exibir e gerenciar benefícios</p></li>
<li><p>Exibir e comprar ofertas do MPN</p></li>
<li><p>Exibir histórico de pedidos e faturas de ofertas do MPN</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p><strong>Agente administrativo</strong></p></td>
<td><ul>
<li><p>Gerenciamento de clientes</p></li>
<li><p>Adicionar lista de dispositivos ao Partner Center</p></li>
<p><li>Criar e aplicar perfis aos dispositivos</p></li>
<li><p>Gerenciamento de assinaturas</p></li>
<li><p>Solicitações de integridade e serviços para clientes</p></li>
<li><p>Solicitar privilégios de administrador</p></li>
<li><p>Exibir preços e ofertas</p></li>
<li><p>Cobrança</p></li>
<li><p>Administrar em nome de um cliente</p></li>
<li><p>Registrar um revendedor de valor agregado</p></li>
</ul></td>
</tr>
<tr class="odd">
<td><p><strong>Agente de vendas</strong></p></td>
<td><ul>
<li><p>Gerenciamento de clientes</p></li>
<li><p>Adicionar lista de dispositivos ao Partner Center</p></li>
<li><p>Gerenciamento de assinaturas</p></li>
<li><p>Exibir tíquetes de suporte</p></li>
<li><p>Solicitar uma relação com um cliente</p></li>
<li><p>Gerenciar clientes em potencial dos clientes</p></li>
<li><p>Exibir o contrato do cliente</p></li>
<li><p>Registrar um revendedor de valor agregado</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p><strong>Agente de suporte técnico</strong></p></td>
<td><ul>
<li><p>Pesquisar e exibir um cliente</p></li>
<li><p>Editar detalhes do cliente</p></li>
<li><p>Ajuda a resolver problemas do cliente com o gerenciamento de cobrança ou assinatura</p></li>
<li><p>Solicitação de suporte em nome dos clientes (Observação: você deve ser um agente administrador para concluir essa tarefa para assinaturas do Office 365)</p></li>
<li><p>Gerenciar assinaturas e serviços em nome dos clientes (Observação: você deve ser um agente administrador para concluir essa tarefa para assinaturas do Office 365)</p></li>
</ul></td>
</tr>
 

 

 



