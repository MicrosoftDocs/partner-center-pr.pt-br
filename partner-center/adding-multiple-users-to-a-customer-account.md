---
title: Adicionar vários usuários para uma conta de cliente
ms.topic: how-to
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Para adicionar vários usuários à conta de um cliente, carregue um arquivo de dados no Partner Center usando o formato de arquivo. csv (valores separados por vírgulas).
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0a9b2ed89b10e43c31d00777054839f3208e5c16
ms.sourcegitcommit: 32516c30e90ee78415e5537d2b8ccf467f56a82d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/03/2020
ms.locfileid: "87535736"
---
# <a name="upload-a-csv-file-of-users-to-a-customers-account"></a>Carregar um arquivo. csv de usuários para a conta de um cliente


**Aplica-se a**

- Partner Center

**Funções apropriadas**

- Administrador global

Adicione vários usuários à conta de um cliente de uma só vez, carregando um arquivo de dados no formato de arquivo de valores separados por vírgula (. csv) no Partner Center. 

## <a name="create-the-file-of-customer-users-and-upload-to-customer-account"></a>Criar o arquivo de usuários do cliente e carregar na conta do cliente

1. Crie um arquivo de valores separados por vírgula (.csv) com os dados descritos acima. Salve o arquivo para que você possa usá-lo em uma etapa posterior. Consulte [os campos do arquivo. csv para importar vários usuários para uma conta de cliente](file-customer-users.md). 

2. Entre no [painel](https://partner.microsoft.com/dashboard) do Partner Center.

3. No menu do centro de parceiros, **selecione**clientes e, em seguida, escolha um cliente na lista.

4. Selecione a guia **usuários e licenças** do cliente e, em seguida, selecione **carregar usuários**.

5. Em **Carregar informações do usuário**, selecione **Procurar**.

6. No seletor de arquivo, selecione seu arquivo de dados e, em seguida, selecione **Abrir**.

7. Selecione **Validar**.

    **Observação**    A maioria dos erros de criação de conta é causada por problemas de arquivo de dados, incluindo informações ausentes, endereços de email malformados ou duplicados ou muitos registros no arquivo.

8. Depois que o Partner Center validar o arquivo, selecione o **local** geográfico para os novos usuários.
9. Clique em **Salvar**.
10. Baixe as informações de senha temporária para os usuários.

    >[!IMPORTANT]
    > Certifique-se de baixar o arquivo com as senhas temporárias agora, pois você não poderá fazer isso mais tarde. Os novos usuários devem fazer logon em suas novas contas usando a respectiva senha temporária.

11. Os novos usuários recebem automaticamente permissões de **Pode usar licenças e serviços**. 

## <a name="next-steps"></a>Próximas etapas

- [Dê permissão aos clientes no Partner Center para comprar seus próprios produtos ou serviços](give-customers-permission.md)
