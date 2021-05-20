---
title: Adicionar vários usuários para uma conta de cliente
ms.topic: how-to
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Para adicionar vários usuários à conta de um cliente, carregue um arquivo de dados no Partner Center usando o formato de arquivo de valor separado por vírgula (.csv).
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 268cc9cb42bc72a444da6aec99425c2b29b71cb4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150464"
---
# <a name="upload-a-csv-file-of-users-to-a-customers-account"></a>Carregar um arquivo .csv de usuários na conta de um cliente


**Funções apropriadas**: administrador global

Adicione vários usuários à conta de um cliente de uma só vez carregando um arquivo de dados no formato de arquivo de valor separado por vírgula (.csv) para o Partner Center. 

## <a name="create-the-file-of-customer-users-and-upload-to-customer-account"></a>Criar o arquivo de usuários do cliente e carregar na conta do cliente

1. Crie um arquivo de valores separados por vírgula (.csv) com os dados descritos acima. Salve o arquivo para que você possa usá-lo em uma etapa posterior. Consulte [Campos para o arquivo .csv para importar vários usuários para uma conta de cliente](file-customer-users.md). 

2. Entre no [painel](https://partner.microsoft.com/dashboard) do Partner Center.

3. No menu do centro de parceiros, **selecione** clientes e, em seguida, escolha um cliente na lista.

4. Selecione a guia Usuários **e Licenças do** cliente e, em seguida, **selecione Carregar usuários**.

5. Em **Carregar informações do usuário**, selecione **Procurar**.

6. No seletor de arquivo, selecione seu arquivo de dados e, em seguida, selecione **Abrir**.

7. Selecione **Validar**.

    **Observação**  A maioria dos erros de criação de conta é causada por problemas no arquivo de dados, como falta de informações, endereços de email incorretos ou duplicados ou número excessivo de registros no arquivo.

8. Depois que Partner Center validar o arquivo, selecione a **Localização geográfica** para os novos usuários.
9. Selecione **Salvar**.
10. Baixe as informações de senha temporária para os usuários.

    >[!IMPORTANT]
    > Certifique-se de baixar o arquivo com as senhas temporárias agora, pois você não poderá fazer isso mais tarde. Os novos usuários devem fazer logon em suas novas contas usando a respectiva senha temporária.

11. Novos usuários são atribuídos automaticamente a permissões de **Pode usar licenças e serviços**. 

## <a name="next-steps"></a>Próximas etapas

- [Dar aos clientes permissão Partner Center para comprar seus próprios produtos ou serviços](give-customers-permission.md)
