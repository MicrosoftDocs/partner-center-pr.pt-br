---
title: Criar vários usuários para uma conta de cliente | Partner Center
ms.topic: article
ms.date: 03/15/2019
description: Você pode adicionar vários usuários a uma conta do cliente de uma vez, carregando um arquivo de dados em formato de arquivo de valores separados por vírgula (.csv) no Partner Center.
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: MaggiePucciEvans
ms.author: evansma
keywords: upload em massa, adicionar vários usuários a uma conta do cliente, adicionar usuários do cliente, upload em massa de usuários do cliente, conta do cliente, usuários do cliente, usuários
ms.localizationpriority: medium
ms.openlocfilehash: b113736330b201ed6a4d1c6b8915e844b80fe5d5
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2019
ms.locfileid: "62134526"
---
# <a name="add-multiple-users-to-a-customer-account"></a>Adicionar vários usuários a uma conta de cliente

**Aplica-se a**

-  Partner Center

Você pode adicionar vários usuários para uma conta de cliente ao mesmo tempo, carregando um arquivo de dados no formato de arquivo de valores separados por vírgula (. csv) para o Centro de parceiros. Você pode baixar um arquivo de dados de exemplo do Partner Center e, em seguida, editá-lo para seu uso, ou você pode criar um novo arquivo de dados usando o modelo de dados definido abaixo.

## <a href="" id="creatingtheimportcsvfile"></a>Requisitos do arquivo de dados


Para adicionar vários usuários a uma conta de cliente usando o processo de upload em massa, você precisará atender aos seguintes requisitos:

-   Você deve ter permissões de administrador global para a conta de cliente;
-   Cada usuário deve ter um endereço de email exclusivo, adicionado ao(s) domínio(s) de email do cliente;
-   Você pode carregar até 100 registros por vez. Se você precisar adicionar mais de 100 usuários, crie e carregue arquivos de dados adicionais.
-   Todos os usuários devem estar na mesma **localização** geográfica.
-   Insira apenas os dados descritos abaixo. Dados irrelevantes causarão a falha do upload.

Insira os seguintes dados no arquivo de dados:

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| **Nome da coluna** | **Descrição**                                                              | **Limitação**                             |
| Nome      | Nome do usuário (campo opcional)                                           | Limite de 50 caracteres                         |
| Sobrenome       | Sobrenome do usuário (campo opcional)                                            | Limite de 50 caracteres                         |
| Nome de exibição    | Nome exibido no centro do parceiro (campo obrigatório)                            | Limite de 50 caracteres                         |
| Email           | Endereço de email comercial do usuário na empresa do cliente (campo obrigatório)           | Cada usuário deve ter um endereço de email exclusivo |
| Atualização de status   | Usado para indicar se o novo registro de usuário foi ou não criado com êxito | \*\*Deixe em branco\*\*                        |

 

### <a href="" id="createmultipleuseraccounts"></a>Para criar várias contas de usuário

<a href="" id="creatingtheaccounts"></a>
1.  Crie um arquivo de valores separados por vírgula (.csv) com os dados descritos acima. Salve o arquivo para que você possa usá-lo em uma etapa posterior.
2.  Dos **Partner Center** menu, selecione **clientes**, em seguida, escolha um cliente da lista.
3.  Selecione **Carregar usuários**.
4.  Em **Carregar informações do usuário**, selecione **Procurar**.
5.  No seletor de arquivo, selecione seu arquivo de dados e, em seguida, selecione **Abrir**.
6.  Selecione **Validar**.

    **Observação**  a maioria dos erros de criação de conta são causados por problemas de arquivo de dados, incluindo ausentes informações, endereços de email malformado ou duplicados ou muitos registros no arquivo.

7.  Depois que o Partner Center valida o arquivo, selecione o geográfico **local** para os novos usuários.
8.  Clique em **Salvar**.
9.  Baixe as informações de senha temporária dos usuários.

**IMPORTANTE:** Certifique-se de baixar o arquivo com as senhas temporárias agora você não poderá fazer isso mais tarde. Os novos usuários devem fazer logon em suas novas contas usando a respectiva senha temporária.

10. Os novos usuários recebem automaticamente permissões de **Pode usar licenças e serviços**. 

 

 



