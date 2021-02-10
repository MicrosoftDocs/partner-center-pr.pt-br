---
title: Gerenciar locais na sua conta de parceiro
ms.topic: how-to
ms.date: 02/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Saiba como adicionar um novo local e como a ID do MPN do local é usada em programas de incentivo, negócios do CSP, assinaturas e outras transações.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 41ffaeaf0fb46659142949872295523546bb91c1
ms.sourcegitcommit: 5768f10cd122a20fe3df3062ea34e7096d99f639
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "100005901"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a>Gerenciar os locais da sua conta do MPN e adicionar (ou excluir) um local


**Funções apropriadas**

- Administrador global
- Administrador de conta

A ID de MPN do local identifica cada local específico de sua empresa. Você usa a ID de MPN de local para se registrar em programas de incentivo, para fazer transações com empresas do CSP (Provedor de Soluções na Nuvem) e para fazer outras transações de negócios. A ID de MPN global é usada para atividades não transacionais, como solicitações de suporte.

## <a name="the-following-is-a-typical-scenario"></a>O seguinte é um cenário típico:

A Contoso tem sua PGA (Conta global de parceiro) no Reino Unido. Trata-se de seus negócios jurídicos registrados e sua ID de MPN global é usada para gerenciar todos os negócios não transacionais. A Contoso também tem PLAs (Contas de local de parceiro) equivalentes a subsidiárias ou a divisões em outros locais do Reino Unido, da França e dos EUA. Na estrutura de Conta do MPN, essas PLAs são representadas como IDs de MPN de local exclusivas. As PLAs são usadas para negócios transacionais, como programas de CSP ou de incentivos. Os pagamentos são vinculados a locais específicos. 

>[!NOTE]
>Há uma relação um-para-um entre um locatário do CSP e uma ID de local do MPN.

:::image type="content" source="images/locations/locations1.png" alt-text="Estrutura dos locais do MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a>Pré-requisitos para adicionar uma nova conta para um negócio do CSP

Para adicionar uma nova conta para o negócio do CSP, primeiro verifique se você cumpre os pré-requisitos.

1. É preciso ter uma ID de MPN de local no país em que deseja fazer negócios com o CSP. Para criar um novo local de MPN, leia "Adicionar um local de MPN" abaixo.
  
1. Para criar um novo registro de CSP Indirect Reseller, leia [Trabalhar com provedores indiretos](indirect-reseller-tasks-in-partner-center.md#get-started) 

>[!NOTE] 
 >Lembre-se de entrar usando as **novas** credenciais da **nova** conta do CSP. Não use suas credenciais existentes, pois o Partner Center reconhecerá que você já tem uma conta.

2. Aceite o Contrato de Parceiro da Microsoft e ative a conta.

1. Se você quiser se registrar como parceiro de fatura direta, leia [Requisitos para parceiros de fatura direta](direct-partner-new-requirements.md)

## <a name="view-your-mpn-locations"></a>Exibir seus locais do MPN

1. Entre no [painel](https://partner.microsoft.com/dashboard/home) do Partner Center com suas credenciais da conta do MPN. (Suas credenciais do MPN podem ser diferentes das credenciais do CSP) 
 
1. No ícone **Configurações**, selecione **Configurações da conta**, **Perfil da organização**, **Legal**. 

1. Na guia **Parceiro**, verifique se não há uma mensagem de erro de banner solicitando que você corrija os locais migrados do PMC. Se houver, siga as instruções e corrija esses locais. 

3. Se não houver uma mensagem de erro, em **Configurações**, selecione **Configurações da Conta**, **Perfil da organização**, **Identificadores**.

4. Localize a ID do MPN com o tipo "local" que corresponde ao país dessa conta do CSP e use-a para pesquisar abaixo e concluir a associação.

5. Se você não encontrar a ID do MPN do local que corresponde à conta do CSP que deseja usar, será possível adicionar um novo local que criará uma ID do MPN. Confira **Adicionar um local do MPN** abaixo.

## <a name="add-an-mpn-location"></a>Adicionar um local do MPN

1. Entre usando a conta do MPN no Partner Center. (Suas credenciais do MPN podem ser diferentes das credenciais do CSP). A conta MPN deve ter privilégios de administrador global ou de administrador de conta. 

1. No **ícone Configurações**, selecione as **Configurações da conta** e o **Perfil da organização**.

2. Selecione **Legal** e, em seguida, na guia **Parceiro**, escolha **Localizações da empresa** e clique em **Adicionar um local**.

3. Insira as informações necessárias, como nome da empresa, endereço e contato do local que você quer adicionar à empresa.
 
1. Clique em **Adicionar local**. Isso criará uma nova ID de MPN para o novo local que você pode usar para transações e incentivos do CSP.

:::image type="content" source="images/legal-biz.png" alt-text="Adicionar uma nova pessoa jurídica":::

> [!NOTE]
> Depois que um local for adicionado no Partner Center, você não poderá removê-lo. Você verá **MPN** no menu à esquerda do Partner Center se tiver usado a ID de MPN correta para entrar.

## <a name="delete-a-location"></a>Excluir um local

Para excluir um local de sua conta, você precisará entrar em contato com o [Suporte a Parceiros](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b). Verifique se você entendeu o impacto que essa ação tem. Os locais excluídos não podem ser recuperados e qualquer coisa associada a essa ID de MPN específica não será mais reconhecida nem estará ativa para sua empresa.

## <a name="change-country-of-partner-global-account"></a>Alterar o país da conta global do parceiro 

1. Entre usando a conta do MPN no Partner Center. (Suas credenciais do MPN podem ser diferentes das credenciais do CSP). A conta MPN deve ter privilégios de administrador global ou de administrador de conta. 

2. Na guia **Parceiro**, acesse **Localizações da empresa** e confira a lista de locais para garantir que o local que você quer como pessoa jurídica esteja listado. 
 
1. Para adicionar um local, clique em **Adicionar um local** e, no submenu, insira as informações necessárias, como nome da empresa, endereço e contato principal do local que você quer adicionar à empresa. 
 
1. Selecione **Alterar seu país** ao lado do menu suspenso **País/região** e siga as etapas. 

:::image type="content" source="images/lbp.png" alt-text="Submenu de dados do perfil de pessoa jurídica":::

5. Clique em **Salvar**.

6. O país da conta global MPN será alterado para o novo país legal.
  
## <a name="next-steps"></a>Próximas etapas

- Saiba mais sobre o [processo de verificação](verification-responses.md).
