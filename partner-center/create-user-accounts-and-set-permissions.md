---
title: "Criar contas de usuário e definir permissões | Partner Center"
description: "O administrador cria uma conta de usuário para cada funcionário de parceiro que precise acessar o Partner Center."
ms.assetid: 75D805AE-9922-4CFD-9427-196047D70963
author: MaggiePucciEvans
ms.openlocfilehash: bc699214c7919c7cff9788144d472063ba60ad10
ms.sourcegitcommit: 4a1cd51e5986f47badcde9412a7c7b22718500f0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2017
---
# <a name="create-user-accounts-and-assign-permissions"></a>Criar contas de usuário e atribuir permissões

**Aplicável a**

-  Partner Center

Criar contas de usuário para os funcionários que precisam acessar o Partner Center. Essas tarefas devem ser realizadas por um administrador com permissões de administrador do gerenciamento de usuário. 

## <a name="add-a-new-user"></a>Adicionar um novo usuário

1. No menu **Painel**, selecione **Configurações da conta > Gerenciamento de usuário**.

2.  Selecione **Adicionar usuário**.

3.  Insira o nome completo e endereço de e-mail exclusivo do usuário.

4.  Selecione o tipo de agente e o tipo de administrador. O acesso do Partner Center é baseado em função, portanto, você pode atribuir permissões para personalizar o modo de exibição do usuário e mostrar somente os recursos que o usuário precisa para completar tarefas específicas. Para obter mais informações sobre o que cada função pode fazer, consulte [Atribuir permissões de usuário](#assignuserpermissions).

5.  Selecione **Adicionar** para criar a conta de usuário. Confirme os detalhes do usuário na próxima página.

>**Importante**<br>
Anote as novas informações de login do usuário exibidas nessa página. Certifique-se de copiar e enviar essas informações para o novo usuário, pois você não conseguirá acessá-las novamente mais tarde. <br>

>O usuário precisará entrar no Partner Center com seu nome de usuário e senha temporária. Quando o usuário entrar no Partner Center pela primeira vez, ele precisará alterar sua senha.    


### <a href="" id="assignuserpermissions"></a>Atribuir permissões de usuário

O acesso do Partner Center é baseado em função, portanto, você pode atribuir permissões para personalizar o modo de exibição do usuário e mostrar somente os recursos que o usuário precisa para completar tarefas específicas. 

Para cada usuário, você deve selecionar dois níveis de permissão:

-   Permissões de agente controlam que tipo de dados de cliente e informações de conta o usuário pode ver e alterar.

-   Permissões de administrador controlam o nível de acesso do usuário aos recursos do Partner Center. Essa configuração tem impacto fora do Partner Center, pois um Administrador de cobrança poderá acessar as listas de todos os serviços Microsoft (mesmo aqueles não relacionados a CSP) e um Administrador global poderá acessar contas de usuário e contas de clientes além do CSP.

##<a name="assign-permissions-for-incentives-users"></a>Atribuir permissões para os usuários de incentivos
Quando você configura seus usuários de incentivos, você pode oferecer a eles a função de administrador de incentivos ou de usuário de incentivos.  O administrador de incentivos pode editar informações bancárias e fiscais, fazer requerimentos de pagamento à Microsoft, bem como gerenciar usuários de incentivos. Os usuários de incentivos podem examinar programas, informações bancárias e fiscais, mas não podem editá-las. Muitas vezes, eles oferecem os programas de incentivos aos clientes. Os usuários e administradores de incentivos podem ter outras funções no Partner Center para a sua organização, mas para trabalhar em programas de incentivos, um usuário deve ser administrador ou usuário de incentivos.

>**Importante** A configuração padrão deve ser sempre **Nenhum administrador**, a menos que a função do usuário exija acesso adicional para concluir as tarefas e dar suporte aos clientes.

A tabela a seguir explica o que cada função pode fazer no Partner Center.

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Função no Partner Center</strong></p></td>
<td><p><strong>O que eles podem fazer</strong></p></td>
<td><p><strong>O que eles não podem fazer</strong></p></td>
</tr>
<tr class="even">
<td><p><strong>Agente administrador</strong></p></td>
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
<li><p>Registrar um bom revendedor</p></li>
</ul></td>
<td><ul>
<li><p>Gerenciamento de usuários</p></li>
<li><p>Solicitações de serviço para o Partner Center</p></li>
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
<li><p>Registrar um bom revendedor</p></li>
</ul></td>
<td><ul>
<li><p>Criar solicitações de serviço para problemas com o Partner Center</p></li>
<li><p>Resolver tíquetes de suporte</p></li>
<li><p>Exibir integridade do serviço</p></li>
<li><p>Exibir preços e ofertas</p></li>
<li><p>Cobrança</p></li>
<li><p>Administrar em nome de um cliente</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p><strong>Agente de suporte técnico</strong></p></td>
<td><ul>
<li><p>Pesquisar e exibir um cliente</p></li>
<li><p>Editar detalhes do cliente</p></li>
<li><p>Integridade do serviço</p></li>
<li><p>Solicitação de suporte em nome dos clientes (Observação: você deve ser um agente administrador para concluir essa tarefa para assinaturas do Office 365)</p></li>
<li><p>Gerenciar assinaturas e serviços em nome dos clientes (Observação: você deve ser um agente administrador para concluir essa tarefa para assinaturas do Office 365)</p></li>
</ul></td>
<td><ul>
<li><p>Exibir perfis de parceiros</p></li>
<li><p>Criar uma nova conta de cliente</p></li>
<li><p>Editar informações de cobrança do cliente</p></li>
<li><p>Gerenciar assinaturas</p></li>
<li><p>Solicitar uma relação com um cliente</p></li>
<li><p>Gerenciar clientes em potencial</p></li>
<li><p>Exibir preços e ofertas</p></li>
<li><p>Exibir o contrato do cliente</p></li>
<li><p>Cobrança</p></li>
<li><p>Registrar um bom revendedor</p></li>
</ul></td>
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
<td></td>
</tr>
<tr class="even">
<td><p><strong>Administrador de cobrança</strong></p></td>
<td><ul>
<li><p>Pode acessar todas as contas da Microsoft com todos os privilégios</p></li>
<li><p>Exibir contratos, listas de preços e ofertas</p></li>
<li><p>Cobrança</p></li>
</ul></td>
<td></td>
</tr>
<tr class="odd">
<td><p><strong>Administrador de gerenciamento de usuário</strong></p></td>
<td><ul>
<li><p>Exibir, criar e gerenciar usuários</p></li>
<li><p>Exibir todos os perfis de parceiros</p></li>
</ul></td>
<td></td>
</tr>
<tr class="even">
<td><p><strong>Administrador de incentivos</strong></p></td>
<td><ul>
<li><p>Exibir e gerenciar todos os programas de incentivos</p></li>
<li><p>Editar perfis bancários e fiscais para programas de incentivos</p></li>
<LI><p>Gerenciar usuários de incentivos</p></li>
</ul></td>
<td></td>
</tr>
<tr class="odd">
<td><p><strong>Usuário de incentivos</strong></p></td>
<td><ul>
<li><p>Exibir programas de incentivos</p></li>
<li><p>Exibir perfis bancários e fiscais</p></li>
</ul></td>
<td></td>
</tr>
</tbody>
</table>

 

 

 



