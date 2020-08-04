---
title: Campos para o arquivo. csv para importar vários usuários para uma conta de cliente
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Para adicionar vários usuários a uma conta de cliente, crie um arquivo de valores separados por vírgulas (. csv) com os campos apropriados.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 07a28e5310716f3df11caa36e51339e877e65627
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/03/2020
ms.locfileid: "87528173"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a>Adicionar vários usuários a uma conta de cliente criando um arquivo. csv

**Aplica-se a**

- Partner Center

**Funções apropriadas**

- Administrador global

Adicione vários usuários à conta de um cliente de uma só vez, carregando um arquivo de dados no formato de arquivo de valores separados por vírgula (. csv) no Partner Center. Você pode baixar um arquivo de dados de exemplo do centro de parceiros e, em seguida, editá-lo para seu uso ou pode criar um novo arquivo de dados usando o modelo de dados definido abaixo.

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a>Requisitos de arquivo de dados:

Para adicionar vários usuários à conta de um cliente usando o processo de carregamento em massa, você precisará atender aos seguintes requisitos:

- Você deve ter permissões de administrador global para a conta de cliente;
- Cada usuário deve ter um endereço de email exclusivo, adicionado ao(s) domínio(s) de email do cliente;
- Você pode carregar até 100 registros por vez. Se você precisar adicionar mais de 100 usuários, crie e carregue arquivos de dados adicionais.
- Todos os usuários devem estar na mesma **localização** geográfica.
- Insira apenas os dados descritos abaixo. Dados irrelevantes causarão a falha do upload.

Insira os seguintes dados no arquivo de dados:

| **Nome da coluna** | **Descrição**  | **Limitação**  |
|:-------- |:------  |:----- |
| Nome  | Nome do usuário (campo opcional)  | limite de 50 caracteres  |
| Sobrenome  | Sobrenome do usuário (campo opcional)  | limite de 50 caracteres  |
| Nome de exibição    | Nome exibido no Partner Center (campo obrigatório)                            | limite de 50 caracteres                         |
| Email   | Endereço de email comercial do usuário na empresa do cliente (campo obrigatório)           | Cada usuário deve ter um endereço de e-mail exclusivo |
| Atualização de status   | Usado para indicar se o novo registro de usuário foi ou não criado com êxito | \*\*Deixar vazio\*\*                        |

## <a name="next-steps"></a>Próximas etapas

- [Como adicionar vários usuários a um cliente](adding-multiple-users-to-a-customer-account.md)