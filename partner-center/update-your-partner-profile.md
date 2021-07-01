---
title: Verificar o perfil da sua empresa
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como verificar os detalhes da empresa, como contato principal, endereço e informações do programa. Você também pode atualizar seus endereços jurídico e para cobrança.
author: parthpandyaMSFT
ms.author: parthp
ms.topic: how-to
ms.date: 04/12/2021
ms.localizationpriority: medium
ms.custom: contperf-fy21q4
ms.openlocfilehash: 9f9a055ce3bfbff568287267b74b04e8f9d03ad1
ms.sourcegitcommit: 8235c89e789cdb5115fc1c19151fa8e97c743fe5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "113080615"
---
# <a name="verify-or-update-your-company-profile-information"></a>Verificar ou atualizar as informações de perfil da sua empresa 

**Funções apropriadas**: administrador global | administrador de conta do MPN

Na primeira vez que você entrar no Partner Center como administrador global, deverá confirmar se todos os detalhes da empresa estão corretos. Isso inclui contato principal, razão social, endereço jurídico e informações do programa. Se sua empresa tiver mais de um local, verifique se os dados do local estão corretos. Como o administrador global, o administrador de cobrança ou o agente administrador, você também poderá ver e atualizar as informações de cobrança e imposto.

> [!NOTE]
> Somente o administrador global pode alterar o endereço para cobrança.

Seu perfil de parceiro consiste em informações jurídicas, nome e email do contato principal, programas nas quais a sua empresa participa e, se relevante, suas outras empresas que agora se fundiram no seu negócio jurídico. Verifique se o nome e o endereço da empresa no perfil comercial jurídico não têm erros de ortografia nem abreviações e se correspondem exatamente aos registros comerciais formais da empresa. Se você estiver operando como Proprietário Único, precisará usar o nome da empresa como razão social.


## <a name="locate-the-legal-business-profile"></a>Localizar o perfil comercial jurídico

1. No Partner Center, selecione o ícone **Configurações** e depois **Configurações da conta**.
 
1. Selecione **Perfil da organização**. 

2. Verifique os valores do **Perfil comercial jurídico**, de **Informações do contato principal** e de **Informações do programa**.

Caso tenha fundido suas outras empresas em seu negócio jurídico, examine também essas informações. 

## <a name="update-your-legal-business-profile"></a>Atualizar seu perfil comercial jurídico 

Atualize a razão social ou o endereço no Partner Center.

>[!Important]
>- Para contas do MPN (Microsoft Partner Network), o administrador global e o administrador da conta podem atualizar a razão social da empresa.
>- Para contas de CSP Indirect Reseller, somente o administrador global pode atualizar a razão social da empresa. 
>- Os parceiros do Direct Bill e os provedores do Indirect não poderão alterar a razão social das respectivas empresas se o status de verificação da conta for **Autorizado**. Se você precisar alterar o nome, será necessário criar um [tíquete de suporte](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=eb74583c-61b3-2124-bffc-00920e0ae772).



1. No Partner Center, selecione **Configurações**, **Configurações da conta** e **Perfil da organização**.

2. Selecione **Jurídico** e escolha o perfil comercial jurídico (Parceiro ou Revendedor) que você deseja atualizar.

1. Selecione **Atualizar** ao lado do nome/endereço da empresa e altere os detalhes.
 
1. Quando você selecionar **Enviar**, a identidade jurídica será reavaliada. Reavaliamos apenas o que você alterou.

1. Se a verificação falhar, saiba como [corrigir o problema](verification-responses.md).

>[!Important]
>Os parceiros de CSP não podem alterar o país associado ao endereço jurídico. O país do endereço jurídico está vinculado ao seu locatário e serviços, bem como à moeda com a qual você faz negócios. Para saber mais sobre as atualizações de país do MPN, leia [Atualizações do país do MPN](manage-locations.md#change-country-of-partner-global-account).


### <a name="who-can-update-legal-business-name-and-when"></a>Quem pode atualizar o nome de pessoa jurídica e quando

|**Programa**|**Quem pode atualizar o nome da empresa**|**Quando (status) pode ser atualizado**|**Permitido**|
|---------------------|:-------------------------------|:------------|:-----------------|
MPN|Administrador global; Administrador da conta|Autorizado; pendente; rejeitado| Permitido|
|CSP: revendedor do Indirect|Administrador global|Autorizado; pendente; rejeitado| Permitido|


## <a name="update-your-mpn-global-business-account"></a>Atualizar sua conta comercial global do MPN

Se, durante a migração do Partner Membership Center para o Partner Center, a conta comercial incorreta tiver sido identificada como a pessoa jurídica, você poderá alterá-la para a conta da pessoa jurídica correta.

Para fazer essas atualizações, você precisa ser o administrador global ou administrador da conta. Saiba como [gerenciar as contas de localização global do MPN](manage-locations.md)


## <a name="update-your-mpn-id-associated-with-your-csp-account"></a>Atualizar sua ID do MPN associada à sua conta do CSP

Para atualizar a ID do MPN associada à sua conta do CSP:

1. Entre no [painel](https://partner.microsoft.com/dashboard/home) do Partner Center como administrador global com as credenciais da conta do CSP e selecione **Configurações**. (Suas credenciais do MPN e do CSP podem ser diferentes.)
 
1. Selecione **Identificadores** em **Configurações de conta**.

1. Na seção **CSP**, use o link **Atualizar** para atualizar a ID do MPN associada à sua conta do CSP 


## <a name="update-your-csp-legal-billing-address"></a>Atualizar seu endereço para cobrança legal do CSP

O administrador global pode alterar o endereço que aparece na fatura no **perfil Pagamento e impostos**. Atualmente, não é possível alterar o nome da empresa na fatura devido a uma limitação do sistema de faturas.

:::image type="content" source="images/billing-profile.png" alt-text="Captura de tela da área em que as informações de cobrança são adicionadas.":::

|**Campo**  |**Descrição**|  
|---------------------|:------------------|
|Nome da empresa recebedora da fatura|O nome da empresa que aparece nas informações do recebedor da fatura em sua fatura do CSP.  Não é possível editar essas informações no Partner Center.  Para atualizar, crie um tíquete de suporte.|
|Endereço do recebedor da fatura|O endereço para cobrança mostrado na fatura do CSP. Pode ser alterado no [Perfil de cobrança](https://partner.microsoft.com/dashboard/account/v3/accountsettings/billingprofile#commercial).|
|Contato de cobrança|Os detalhes de contato de cobrança (nome, sobrenome, número principal) para a conta do CSP.  Pode ser alterado no [Perfil de cobrança](https://partner.microsoft.com/dashboard/account/v3/accountsettings/billingprofile#commercial).|
|Número da OC|O número da ordem de compra exibido na fatura do parceiro. Pode ser alterado no [Perfil de cobrança](https://partner.microsoft.com/dashboard/account/v3/accountsettings/billingprofile#commercial).|
|ID do imposto da empresa|As empresas em alguns países podem fornecer os respectivos [números de IVA (imposto sobre valor agregado) ou equivalente local](./organization-tax-info.md). Para atualizar sua ID de imposto/IVA, você deve ser um administrador global, um administrador de cobrança ou um agente de administrador.|
|Moeda de Cobrança|A moeda de cobrança para a conta do CSP é determinada pelo país legal dessa conta.  Não é possível alterar essas informações depois da criação da conta de CSP.|

## <a name="next-steps"></a>Próximas etapas

- [Examinar o status de verificação](verification-responses.md)

- [Gerenciar locais do MPN](manage-locations.md)
