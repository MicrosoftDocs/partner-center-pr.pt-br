---
title: Campos para o arquivo .csv para importar vários usuários para uma conta de cliente
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Para adicionar vários usuários a uma conta de cliente, crie um arquivo de valor separado por vírgula (.csv) com campos apropriados.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 152daadde25a9325937797f7a3daa90dfb59a9b4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150974"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a>Adicionar vários usuários a uma conta de cliente criando um arquivo .csv

**Funções apropriadas**: administrador global

Adicione vários usuários à conta de um cliente de uma só vez carregando um arquivo de dados no formato de arquivo de valor separado por vírgula (.csv) para o Partner Center. Você pode baixar um arquivo de dados de exemplo do Partner Center e editá-lo para seu uso ou criar um novo arquivo de dados usando o modelo de dados definido abaixo.

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
| Nome de exibição    | Nome exibido na Partner Center (campo obrigatório)                            | limite de 50 caracteres                         |
| Email   | Endereço de email comercial do usuário na empresa do cliente (campo obrigatório)           | Cada usuário deve ter um endereço de e-mail exclusivo |
| Atualização de status   | Usado para indicar se o novo registro de usuário foi criado com êxito | \*\*Deixe em branco\*\*                        |

## <a name="next-steps"></a>Próximas etapas

- [Como adicionar vários usuários para um cliente](adding-multiple-users-to-a-customer-account.md)