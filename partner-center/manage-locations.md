---
title: Gerenciar locais na sua conta de parceiro
ms.topic: article
ms.date: 10/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Saiba como adicionar um novo local e como a ID do MPN do local é usada em programas de incentivo, negócios do CSP, assinaturas e outras transações.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c4435227cdd5d777d11c79bf4adc63471ad925e9
ms.sourcegitcommit: 940dad4527f51781f6f966e196b3aa08389613a2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/13/2020
ms.locfileid: "92006853"
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

## <a name="add-a-location"></a>Adicionar um local

1. Entre usando a conta do MPN no Partner Center. A conta MPN deve ter privilégios de administrador global ou de administrador de conta. 

1. No **ícone Configuração**, selecione as **Configurações do parceiro**.

2. Selecione **Locais.**

3. Selecione **Adicionar um local** e insira os detalhes do endereço do local que você deseja adicionar à sua empresa, bem como um contato principal para o local.

> [!NOTE]
> Depois que um local for adicionado no Partner Center, ele não poderá ser removido. Você verá **MPN** no menu à esquerda do Partner Center se tiver usado a ID de MPN correta para entrar.

## <a name="change-global-partner-account-location"></a>Alterar o local da Conta de parceiro global

1. Na página **[Locais](https://partner.microsoft.com/pcv/accountsettings/locationsprofile)** , confira a lista de locais para verificar se o local que você deseja como pessoa jurídica está listado. Se não estiver, adicione-o.

   :::image type="content" source="images/updatepartnerprofile2.png" alt-text="Estrutura dos locais do MPN":::

2. Selecione **Perfil do parceiro** e, em seguida, **Atualizar perfil de negócios jurídico**

   :::image type="content" source="images/updatepartnerprofile1.png" alt-text="Estrutura dos locais do MPN":::

3. Selecione a região e a pessoa jurídica e **Envie-a**.

   :::image type="content" source="images/updatepartnerprofile3.png" alt-text="Estrutura dos locais do MPN":::

## <a name="next-steps"></a>Próximas etapas

- Saiba mais sobre o [processo de verificação](verification-responses.md).
