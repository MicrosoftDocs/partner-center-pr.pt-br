---
title: Gerenciar locais na sua conta de parceiro
ms.topic: how-to
ms.date: 11/23/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Saiba como adicionar um novo local e como a ID do MPN do local é usada em programas de incentivo, negócios do CSP, assinaturas e outras transações.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 03c4fb5a4adeb49602fe3736971e140ac6da6f4f
ms.sourcegitcommit: 245b4792e8221468f781f6effd1c9b23be05499a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/24/2020
ms.locfileid: "95514785"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a>Gerenciar os locais de sua conta do MPN e adicionar um novo local

**Aplica-se a**

- Partner Center

**Funções apropriadas**

- Administrador global
- Administrador de conta

A ID de MPN do local identifica cada local específico de sua empresa. Você usa a ID de MPN de local para se registrar em programas de incentivo, para fazer transações com empresas do CSP (Provedor de Soluções na Nuvem) e para fazer outras transações de negócios. A ID de MPN global é usada para atividades não transacionais, como solicitações de suporte.

## <a name="the-following-is-a-typical-scenario"></a>O seguinte é um cenário típico:

A Contoso tem sua PGA (Conta global de parceiro) no Reino Unido. Trata-se de seus negócios jurídicos registrados e sua ID de MPN global é usada para gerenciar todos os negócios não transacionais. A Contoso também tem PLAs (Contas de local de parceiro) equivalentes a subsidiárias ou a divisões em outros locais do Reino Unido, da França e dos EUA. Na estrutura de Conta do MPN, essas PLAs são representadas como IDs de MPN de local exclusivas. As PLAs são usadas para negócios transacionais, como programas de CSP ou de incentivos. Os pagamentos são vinculados a locais específicos. 

>[!NOTE]
>Há uma relação um-para-um entre um locatário do CSP e uma ID de local do MPN.

:::image type="content" source="images/locations/locations1.png" alt-text="Estrutura dos locais do MPN":::

## <a name="prerequisites-in-order-to-add-a-new-location-for-a-csp-business"></a>Pré-requisitos para adicionar um novo local para um negócio do CSP

Para adicionar um novo local para um negócio do CSP, há vários pré-requisitos:

1. Você precisa ter uma ID de MPN de local no país em que deseja fazer negócios.

1. Você precisa de um novo locatário do Azure AD na [região de negócios](regional-authorization-overview.md) que ainda não esteja inscrito no CSP. Crie-o ao se registrar no CSP.
 
3. Use o novo locatário do AAD para se registrar no programa CSP na região.
Fornecer detalhes legais da empresa, incluindo o nome jurídico da empresa, o endereço e os detalhes do contato principal. Essa conta passará por verificação, portanto, certifique-se de adicionar informações válidas.

>[!NOTE] 
 >Lembre-se de entrar usando as **novas** credenciais do **novo** locatário do Azure AD. Não use suas credenciais existentes, pois o Partner Center reconhecerá que você já tem uma conta.

4. Aceite o Contrato de Parceiro da Microsoft e ative a conta.

## <a name="add-an-mpn-location"></a>Adicionar um local do MPN

1. Entre usando a conta do MPN no Partner Center. A conta MPN deve ter privilégios de administrador global ou de administrador de conta. 

1. No **ícone Configuração**, selecione as **Configurações da organização**.

2. Selecione **Jurídico** e **Locais.**

3. Selecione **Adicionar um local** e insira os detalhes do endereço do local que você deseja adicionar à sua empresa, bem como um contato principal para o local.

> [!NOTE]
> Depois que um local for adicionado no Partner Center, ele não poderá ser removido. Você verá **MPN** no menu à esquerda do Partner Center se tiver usado a ID de MPN correta para entrar.

## <a name="change-global-partner-account-location"></a>Alterar o local da Conta de parceiro global

1. Em **[Local da empresa](https://partner.microsoft.com/dashboard/account/v3/organization/legalinfo#mpn)** , confira a lista de locais para garantir que o local que você quer como pessoa jurídica esteja listado. Se não estiver, adicione-o.

   :::image type="content" source="images/accountsettings/location1.png" alt-text="Captura de tela da página Locais da Conta do Partner Center com a lista de todos os locais atuais.":::

2. Selecione **Jurídico** e depois **Atualizar perfil de negócios jurídico**
  
3. Selecione a região e a pessoa jurídica e **Envie-a**.

  
## <a name="next-steps"></a>Próximas etapas

- Saiba mais sobre o [processo de verificação](verification-responses.md).
