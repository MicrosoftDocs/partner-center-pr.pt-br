---
title: Adicionar vários usuários para uma conta de cliente
ms.topic: article
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como adicionar vários usuários à conta de um cliente de uma só vez. Carregue um arquivo de dados no Partner Center usando o formato de arquivo. csv (valores separados por vírgulas).
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: upload em massa, adicionar vários usuários a uma conta do cliente, adicionar usuários do cliente, upload em massa de usuários do cliente, conta do cliente, usuários do cliente, usuários
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1929eb7eee7f23de6ae6e8dcd343d38fe2414f6f
ms.sourcegitcommit: 2a980b50cf177753c15ebfd7770e14cf6d486cf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2020
ms.locfileid: "83794899"
---
# <a name="add-multiple-users-to-a-customer-account---upload-a-data-file-to-partner-center"></a>Adicionar vários usuários a uma conta de cliente – carregar um arquivo de dados no Partner Center

**Aplica-se a**

- Partner Center

**Funções apropriadas**

- Administrador global

Você pode adicionar vários usuários à conta de um cliente de uma só vez, carregando um arquivo de dados no formato de arquivo de valores separados por vírgula (. csv) no Partner Center. Você pode baixar um arquivo de dados de exemplo do centro de parceiros e, em seguida, editá-lo para seu uso ou pode criar um novo arquivo de dados usando o modelo de dados definido abaixo.

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a>Requisitos de arquivo de dados:

Para adicionar vários usuários à conta de um cliente usando o processo de carregamento em massa, você precisará atender aos seguintes requisitos:

- Você deve ter permissões de administrador global para a conta de cliente;
- Cada usuário deve ter um endereço de email exclusivo, adicionado ao(s) domínio(s) de email do cliente;
- Você pode carregar até 100 registros por vez. Se você precisar adicionar mais de 100 usuários, crie e carregue arquivos de dados adicionais.
- Todos os usuários devem estar na mesma **localização** geográfica.
- Insira apenas os dados descritos abaixo. Dados irrelevantes causarão a falha do upload.

Insira os seguintes dados no arquivo de dados:

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| **Nome da coluna** | **Descrição**                                                              | **Limitações**                             |
| Nome      | Nome do usuário (campo opcional)                                           | limite de 50 caracteres                         |
| Sobrenome       | Sobrenome do usuário (campo opcional)                                            | limite de 50 caracteres                         |
| Nome de exibição    | Nome exibido no Partner Center (campo obrigatório)                            | limite de 50 caracteres                         |
| Email           | Endereço de email comercial do usuário na empresa do cliente (campo obrigatório)           | Cada usuário deve ter um endereço de e-mail exclusivo |
| Atualização de status   | Usado para indicar se o novo registro de usuário foi ou não criado com êxito | \*\*Deixar vazio\*\*                        |

### <a name="to-create-multiple-user-accounts"></a><a href="" id="createmultipleuseraccounts"></a>Para criar várias contas de usuário

<a href="" id="creatingtheaccounts"></a>

1. Crie um arquivo de valores separados por vírgula (.csv) com os dados descritos acima. Salve o arquivo para que você possa usá-lo em uma etapa posterior.

2. Entre no [painel](https://partner.microsoft.com/dashboard) do Partner Center.

3. No menu do centro de parceiros, **selecione**clientes e, em seguida, escolha um cliente na lista.

4. Selecione a guia **usuários e licenças** do cliente e, em seguida, selecione **carregar usuários**.

5. Em **Carregar informações do usuário**, selecione **Procurar**.

6. No seletor de arquivo, selecione seu arquivo de dados e, em seguida, selecione **Abrir**.

7. Selecione **Validar**.

    **Observação**    A maioria dos erros de criação de conta é causada por problemas de arquivo de dados, incluindo informações ausentes, endereços de email malformados ou duplicados ou muitos registros no arquivo.

8. Depois que o Partner Center validar o arquivo, selecione o **local** geográfico para os novos usuários.
9. Selecione **Salvar**.
10. Baixe as informações de senha temporária para os usuários.

**IMPORTANTE:** Certifique-se de baixar o arquivo com as senhas temporárias agora, pois não será possível fazer isso mais tarde. Os novos usuários devem fazer logon em suas novas contas usando a respectiva senha temporária.

10. Os novos usuários recebem automaticamente permissões de **Pode usar licenças e serviços**. 

 

 



