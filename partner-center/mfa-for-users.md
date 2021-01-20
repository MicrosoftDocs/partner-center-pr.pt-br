---
title: Configurar os usuários com a autenticação multifator
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Saiba como fazer a configuração da MFA para seus funcionários
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: f42c97be88a1a505f7e0ae9b8af0d4a9167d8447
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182368"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a>Configurar os usuários com a autenticação multifator

**Funções apropriadas**

- Administrador global

As maiores proteções de privacidade e segurança estão entre nossas principais prioridades. Sabemos que a melhor defesa é a prevenção e que somos tão fortes quanto nosso vínculo mais fraco. É por isso que precisamos de todos em nosso ecossistema, para agir e garantir que as proteções de segurança adequadas estejam em vigor. É altamente recomendável que todos os parceiros habilitem a MFA (autenticação multifator) para seus usuários em seus locatários parceiros. 

## <a name="add-multi-factor-authentication-for-your-users"></a>Adicionar a autenticação multifator aos seus dispositivos

Você precisará ser o administrador global da sua empresa para concluir esta tarefa.

É mais fácil habilitar a MFA para os usuários conforme você os adiciona ao seu locatário do Azure AD.

1. Entre no [portal do Azure](https://portal.azure.com) e acesse **Gerenciamento de usuários**.
1. Selecione **Autenticação multifator**.
1. Escolha o usuário que deseja habilitar e selecione **Habilitar**.

Isso habilitará a MFA para o usuário. A indicação Habilitado significa que o usuário precisará configurar a verificação da MFA quando ele se conectar pela primeira vez. Depois disso, ao entrar, será solicitado que forneça um código enviado a eles por email ou mensagem de texto (dependendo da configuração efetuada).  

:::image type="content" source="images/MFA/securityverification.png" alt-text="Especificar a confirmação":::

>[!NOTE]
>Você pode **Impor** aos usuários o uso da MFA usando as mesmas etapas acima e selecionando **Impor**. Para saber mais, leia [Habilitar a Autenticação Multifator do Azure por usuário para proteger eventos de entrada](/azure/active-directory/authentication/howto-mfa-userstates). 

Todos os usuários começam com o estado **Desabilitado**. Quando você registra os usuários na Autenticação Multifator do Azure por usuário, o estado deles passa a ser **Habilitado**. Quando os usuários habilitados se conectam e concluem o processo de registro, o estado deles passa a ser **Imposto**. 

## <a name="next-steps"></a>Próximas etapas

- [Atribuir funções e permissões a usuários](permissions-overview.md)