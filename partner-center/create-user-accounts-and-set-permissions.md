---
title: "Criar contas de usuário e definir permissões | Partner Center"
description: "O administrador cria uma conta de usuário para cada funcionário de parceiro que precise acessar o Partner Center."
ms.assetid: 75D805AE-9922-4CFD-9427-196047D70963
author: MaggiePucciEvans
ms.openlocfilehash: a755c9375c7bd5e61345d7d7e1ab27e00af3fe4d
ms.sourcegitcommit: 772577c0538a5d5b05d45f0e669697209761ab03
translationtype: HT
---
# <a name="create-user-accounts-and-set-permissions"></a>Criar contas de usuário e definir permissões

**Aplicável a**

-  Partner Center

O administrador cria uma conta de usuário para cada funcionário de parceiro que precise acessar o Partner Center. Essas tarefas devem ser realizadas por um administrador com permissões de **Administrador global** ou **Administrador do gerenciamento de usuários**. Em **Configurações da conta** &gt; **Gerenciamento de usuários**, você pode adicionar contas e definir ou atualizar as permissões.

**Adicionar um novo usuário**

1.  No Partner Center, acesse o menu Painel &gt; **Configurações da conta** &gt; **Gerenciamento de usuários**.
2.  Escolha **Adicionar usuário**.

3.  Digite o nome completo do usuário e crie um endereço de email exclusivo para ele.

4.  Selecione o tipo de agente e o tipo de administrador. O acesso ao Partner Center é baseado em funções, para que as seleções feitas nesta etapa personalizem o modo de exibição do usuário para mostrar apenas os recursos necessários. Para obter mais informações sobre o que cada função pode fazer, consulte [Definir permissões de usuário](#setuserpermissions).

5.  Adicionar o usuário. Você verá uma tela de confirmação com uma senha temporária para o novo logon. Você deve copiar e enviá-la para o novo usuário, ela não é acessível depois que você sair da tela. Quando se conectar pela primeira vez, ele será solicitado a atualizar a senha.

### <a href="" id="setuserpermissions"></a>Definir permissões de usuário

O acesso ao Partner Center é baseado em função, o que significa que você pode personalizar o modo de exibição do usuário para mostrar apenas a funcionalidade que um usuário precisará em sua função no trabalho. Para cada usuário, você deve selecionar duas configurações:

-   A configuração de **agente** controla quais tipos de dados do cliente e informações da Microsoft o usuário pode ver.

-   A configuração **administrador** determina qual o controle do usuário sobre o ambiente do Partner Center e todos os outros serviços Microsoft (contas, perfis e tíquetes de suporte). Essa configuração tem impacto fora do Partner Center, um Administrador de cobrança pode acessar todas as listas de todos os serviços Microsoft (mesmo aqueles não relacionados a CSP) e um Administrador global pode acessar contas de usuário e contas de clientes além do CSP também.

    A configuração padrão deve ser sempre **Nenhum administrador**, a menos que a função do usuário exija acesso adicional para concluir as tarefas e dar suporte aos clientes.

A tabela a seguir explica o conjunto completo de atividades que cada função pode realizar no Partner Center.

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
<li><p>Gerenciamento de assinaturas</p></li>
<li><p>Solicitações de integridade e serviços para clientes</p></li>
<li><p>Solicitar privilégios de administrador</p></li>
<li><p>Exibir preços e ofertas</p></li>
<li><p>Cobrança</p></li>
<li><p>Administrar em nome de</p></li>
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
<li><p>Gerenciamento de assinaturas</p></li>
<li><p>Exibir tíquetes de suporte</p></li>
<li><p>Solicitar um relacionamento</p></li>
<li><p>Gerenciar clientes em potencial dos clientes</p></li>
<li><p>Exibir o contrato do cliente</p></li>
<li><p>Registrar um bom revendedor</p></li>
</ul></td>
<td><ul>
<li><p>Criar tíquetes de suporte para serviços ou Partner Center</p></li>
<li><p>Resolver tíquetes de suporte</p></li>
<li><p>Exibir integridade do serviço</p></li>
<li><p>Exibir preços e ofertas</p></li>
<li><p>Cobrança</p></li>
<li><p>Administrar em nome de</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p><strong>Agente de suporte técnico</strong></p></td>
<td><ul>
<li><p>Pesquisar e exibir um cliente</p></li>
<li><p>Editar detalhes do cliente</p></li>
<li><p>Integridade do serviço</p></li>
<li><p>Criar tíquetes de suporte para os clientes</p></li>
<li><p>Administrar serviços em nome dos clientes</p></li>
</ul></td>
<td><ul>
<li><p>Exibir perfis de parceiros</p></li>
<li><p>Criar uma nova lista de clientes</p></li>
<li><p>Editar informações de cobrança do cliente</p></li>
<li><p>Gerenciamento de assinaturas</p></li>
<li><p>Solicitar um relacionamento</p></li>
<li><p>Gerenciar clientes em potencial dos clientes</p></li>
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
</tbody>
</table>

 

 

 



