---
title: Criar contas de usuário e definir permissões (operado pela 21Vianet do Partner Center)
ms.topic: article
ms.date: 10/29/2018
description: Como criar contas de usuário para os funcionários que precisam de acesso ao Partner Center.
author: MaggiePucciEvans
ms.author: evansma
ms.openlocfilehash: a96c7fedacbb177c93ae19c5ff4f1a241905be4b
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2019
ms.locfileid: "57584439"
---
# <a name="create-user-accounts-and-set-permissions"></a>Criar contas de usuário e definir permissões


**Aplica-se a**

-   Partner Center operado pela 21Vianet


Crie contas de usuário para seus funcionários que precisam para realizar tarefas no Partner Center. Somente globais ou administradores de gerenciamento de usuário podem adicionar usuários e atribuir funções. Na **configurações de conta** &gt; **gerenciamento de usuários**, você pode adicionar contas de usuário e atribuir ou alterar as permissões.

**Adicionar um novo usuário**

1.  No Partner Center, vá até o menu do painel &gt; **configurações de conta** &gt; **gerenciamento de usuário**.

2.  Selecione **Adicionar usuário**.

3.  Digite o nome completo do usuário e o endereço de email exclusivo.

4.  Selecione a função do funcionário e o nível de acesso. Permissões e acesso ao partner Center são baseadas em funções, que lhe permite controlar as tarefas específicas que pode ser executadas por cada funcionário. Para obter mais informações sobre o que cada função pode fazer, consulte [definir permissões de usuário](#setuserpermissions).

5.  Selecione **Adicionar** para criar a conta de usuário. A página de confirmação aparece, exibindo o novo usuário permissões e informações de logon, incluindo uma senha temporária.

    >**Importante**<br>Quando novos usuários entrarem no Partner Center pela primeira vez, eles devem entrar com sua senha temporária. Certifique-se de anotar a nova senha de usuário temporário para que você pode enviá-lo mais tarde. Você não conseguirá acessar essas informações novamente. 

### <a href="" id="setuserpermissions"></a>Definir permissões de usuário

Acesso do Partner Center é baseado em função, que significa que você pode restringir a exibição de usuário para mostrar apenas os recursos e funções que um usuário precisa para concluir tarefas específicas. Para cada usuário, você deve selecionar duas configurações:

-   O **agente** determina que tipo de dados de clientes e da empresa em que o usuário pode ver.

-   O **admin** determina quanto acesso do usuário para dados, funções e recursos do Partner Center. 

    >**Observação**<br>A configuração padrão deve ser **nenhum administrador** na maioria dos casos, a menos que o funcionário requer permissões para concluir tarefas administrativas específicas.

####<a name="partner-center-roles-and-associated-permissions"></a>Funções do Partner Center e permissões associadas

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Função no Partner Center</strong></p></td>
<td><p><strong>O que pode fazer</strong></p></td>
<td><p><strong>O que não é possível fazer</strong></p></td>
</tr>
<tr class="even">
<td><p><strong>Agente de Admin</strong></p></td>
<td><ul>
<li><p>Gerenciamento de clientes</p></li>
<li><p>Gerenciar assinatura</p></li>
<li><p>Integridade do serviço de acesso para clientes</p></li>
<li><p>Privilégios administrativos de delegados de solicitação</p></li>
<li><p>Exibir preços e ofertas</p></li>
<li><p>Exibir e baixar faturas e arquivos de reconciliação</p></li>
<li><p>Administrar em nome de um cliente</p></li>
<li><p>Registrar um bom revendedor</p></li>
</ul></td>
<td><ul>
<li><p>Gerenciar usuário</p></li>
</ul></td>
</tr>
<tr class="odd">
<td><p><strong>Agente de vendas</strong></p></td>
<td><ul>
<li><p>Gerenciamento de clientes</p></li>
<li><p>Gerenciar assinatura</p></li>
<li><p>Solicitar uma relação de revendedor com um cliente</p></li>
<li><p>Exibir o contrato do cliente</p></li>
<li><p>Registrar um bom revendedor</p></li>
</ul></td>
<td><ul>
<li><p>Criar solicitações de suporte com 21Vianet para problemas com os serviços ou o Partner Center</p></li>
<li><p>Exibir integridade do serviço</p></li>
<li><p>Exibir preços e ofertas</p></li>
<li><p>Exibir e baixar faturas e arquivos de reconciliação</p></li>
<li><p>Administrar em nome de um cliente</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p><strong>Agente de suporte técnico</strong></p></td>
<td><ul>
<li><p>Pesquisa de clientes e exibir detalhes do cliente</p></li>
<li><p>Editar detalhes do cliente</p></li>
<li><p>Integridade do serviço de acesso para clientes</p></li>
<li><p>Administrar em nome de um cliente</p></li>
</ul></td>
<td><ul>
<li><p>Exibir perfis de parceiros</p></li>
<li><p>Criar uma nova conta de cliente</p></li>
<li><p>Editar informações de cobrança do cliente</p></li>
<li><p>Gerenciar assinatura</p></li>
<li><p>Solicitar uma relação de revendedor com um cliente</p></li>
<li><p>Exibir preços e ofertas</p></li>
<li><p>Exibir o contrato do cliente</p></li>
<li><p>Exibir e baixar faturas e arquivos de reconciliação</p></li>
<li><p>Registrar um bom revendedor</p></li>
</ul></td>
</tr>
<tr class="odd">
<td><p><strong>Administrador global</strong></p></td>
<td><ul>
<li><p>Pode acessar todas as contas e serviços com privilégios totais</p></li>
<li><p>Criar solicitações de suporte com 21Vianet para problemas do Partner Center</p></li>
<li><p>Exibir contratos, listas de preços e ofertas</p></li>
<li><p>Exibir e baixar faturas e arquivos de reconciliação</p></li>
<li><p>Exibir, criar e gerenciar usuários da sua empresa</p></li>
</ul></td>
<td></td>
</tr>
<tr class="even">
<td><p><strong>Administrador de cobrança</strong></p></td>
<td><ul>
<li><p>Pode acessar todas as faturas e arquivos de reconciliação com privilégios totais</p></li>
<li><p>Exibir contratos, listas de preços e ofertas</p></li>
</ul></td>
<td></td>
</tr>
<tr class="odd">
<td><p><strong>Administrador de gerenciamento de usuário</strong></p></td>
<td><ul>
<li><p>Exibir, criar e gerenciar usuários da sua empresa</p></li>
<li><p>Exibir todos os perfis de parceiros</p></li>
</ul></td>
<td></td>
</tr>
</tbody>
</table>

