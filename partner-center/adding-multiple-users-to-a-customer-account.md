---
title: "Criar vários usuários para uma conta de cliente | Partner Center"
description: "Você pode adicionar vários usuários a uma conta do cliente de uma vez, carregando um arquivo de dados em formato de arquivo de valores separados por vírgula (.csv) no Partner Center."
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: MaggiePucciEvans
translationtype: Human Translation
ms.sourcegitcommit: 14ba85c868e59dd1c77063f5b1b0e9ab8db7f82f
ms.openlocfilehash: d8aa280363bc654170c10ea0497a77bcd1e09e11

---

# Criar vários usuários para uma conta de cliente


Você pode adicionar vários usuários a uma conta do cliente de uma vez, carregando um arquivo de dados em formato de arquivo de valores separados por vírgula (.csv) no Partner Center. Você pode baixar um arquivo de dados de exemplo do Partner Center e editá-lo para seu uso, ou pode criar um novo arquivo de dados usando o modelo de dados definido abaixo.

## <a href="" id="creatingtheimportcsvfile"></a>Requisitos de arquivo de dados:


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
| Nome de exibição    | Nome exibido no Partner Center (campo obrigatório)                            | Limite de 50 caracteres                         |
| Email           | Endereço de email comercial do usuário na empresa do cliente (campo obrigatório)           | Cada usuário deve ter um endereço de email exclusivo |
| Atualização de status   | Usado para indicar se o novo registro de usuário foi ou não criado com êxito | \*\*Deixar em branco\* \ *                        |

 

### <a href="" id="createmultipleuseraccounts"></a>Para criar várias contas de usuário

<a href="" id="creatingtheaccounts"></a>
1.  Crie um arquivo de valores separados por vírgula (.csv) com os dados descritos acima. Salve o arquivo para que você possa usá-lo em uma etapa posterior.
2.  No menu **Painel**, selecione **Clientes** e escolha um cliente da lista.
3.  Selecione **Carregar usuários**.
4.  Em **Carregar informações do usuário**, selecione **Procurar**.
5.  No seletor de arquivo, selecione seu arquivo de dados e, em seguida, selecione **Abrir**.
6.  Selecione **Validar**.

    **Observação**  A maioria dos erros de criação de conta é causada por problemas no arquivo de dados, como falta de informações, endereços de email incorretos ou duplicados ou número excessivo de registros no arquivo.

     

7.  Depois que o Partner Center validar o arquivo, selecione a **localização** geográfica dos novos usuários.
8.  Selecione **Salvar**.
9.  Baixe as informações de senha temporária dos usuários.

**IMPORTANTE:** Certifique-se de baixar o arquivo com as senhas temporárias agora, pois não será possível fazer isso mais tarde. Os novos usuários devem fazer logon em suas novas contas usando a respectiva senha temporária.

O Partner Center atribui automaticamente a permissão **Pode usar licenças e serviços** aos novos usuários.

 

 






<!--HONumber=Nov16_HO4-->


