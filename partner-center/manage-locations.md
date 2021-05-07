---
title: Gerenciar locais na sua conta de parceiro
ms.topic: how-to
ms.date: 05/01/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Saiba como adicionar um novo local e como a ID do MPN do local é usada em programas de incentivo, negócios do CSP, assinaturas e outras transações.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8a2b4fa8b204b10d5d45c0e1409ab4bc463e272f
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702885"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a>Gerenciar os locais da sua conta do MPN e adicionar (ou excluir) um local


**Funções apropriadas**

- Administrador global
- Administrador de conta

A ID de MPN do local identifica cada local específico de sua empresa. Você usa a ID de MPN de local para se registrar em programas de incentivo, para fazer transações com empresas do CSP (Provedor de Soluções na Nuvem) e para fazer outras transações de negócios. A ID de MPN global é usada para atividades não transacionais, como solicitações de suporte.

## <a name="the-following-scenario-is-typical"></a>O seguinte cenário é típico:

A Contoso tem sua PGA (Conta global de parceiro) no Reino Unido. A PGA é o negócio jurídico registrado deles e a ID global do MPN da empresa é usada para gerenciar todos os negócios não transacionais. A Contoso também tem PLAs (Contas de local de parceiro) equivalentes a subsidiárias ou a divisões em outros locais do Reino Unido, da França e dos EUA. Na estrutura de Conta do MPN, essas PLAs são representadas como IDs de MPN de local exclusivas. As PLAs são usadas para negócios transacionais, como programas de CSP ou de incentivos. Os pagamentos são vinculados a locais específicos. 

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

## <a name="view-and-update-your-mpn-locations"></a>Exibir e atualizar seus locais do MPN

1. Entre no [painel](https://partner.microsoft.com/dashboard/home) do Partner Center com suas credenciais da conta do MPN. (Suas credenciais do MPN podem ser diferentes das credenciais do CSP) 
 
1. No ícone **Configurações**, selecione **Configurações da conta**, **Perfil da organização**, **Legal**. 

1. Na guia **Parceiro**, verifique se não há uma mensagem de erro de banner solicitando que você corrija os locais migrados do PMC.  Se os locais não tiverem sido configurados corretamente no PMC e ainda não tiverem sido transferidos para o PC, será necessário atualizar esses locais.

:::image type="content" source="images/locations/location-two.png" alt-text="A captura de tela mostra como atualizar o local.":::
 
4.  Na tela **Examinar locais do PMC**, selecione **Atualizar**.
Atualize os seguintes campos:

- **Campo Nome**: verifique se o nome do local da empresa está correto. Se for exibido um erro de duplicação, tente mudar, por exemplo, de Contoso para Contoso, Inc.

- **Campo Pessoa jurídica**: verifique se você escolheu a pessoa jurídica à qual o local está vinculado

- **Campos Linhas 1 e 2 de endereço**: verifique se o endereço está correto

- **Campos Cidade e Estado/Província**: verifique se a combinação entre cidade e estado/província está correta. Para alguns países, será fornecido um menu suspenso para escolha de estado/província; para outros países, esse campo deverá ser preenchido manualmente.

- **Campo CEP/Código postal**: verifique se o campo CEP corresponde ao país, à região, à cidade ou ao endereço indicado.

- **Campos de Informações de contato principal**: verifique se os campos Nome e Sobrenome estão preenchidos e se o endereço de email indicado é de trabalho e não pessoal (por exemplo: @outlook.com, @live.com etc.)

- **Campo Número de telefone**: verifique se o número de telefone NÃO contém caracteres especiais, espaços ou o código do país. O valor inserido no campo Número de telefone deverá conter sempre o máximo de 10 caracteres.

5. Se não houver uma mensagem de erro, em **Configurações**, selecione **Configurações da Conta**, **Perfil da organização**, **Identificadores**.

6. Localize a ID do MPN com o tipo "Local" que corresponde ao país dessa conta do CSP e use-a para concluir a associação.

7. Se você não encontrar a ID do MPN do local que corresponda à conta do CSP que você deseja usar, será possível adicionar um local, que criará uma ID do MPN. Confira **Adicionar um local do MPN** abaixo.

## <a name="add-an-mpn-location"></a>Adicionar um local do MPN

1. Entre usando a conta do MPN no Partner Center. (Suas credenciais do MPN podem ser diferentes das credenciais do CSP). A conta MPN deve ter privilégios de administrador global ou de administrador de conta. 

1. No **ícone Configurações**, selecione as **Configurações da conta** e o **Perfil da organização**.

2. Selecione **Legal** e, em seguida, na guia **Parceiro**, escolha **Localizações da empresa** e clique em **Adicionar um local**.

3. Insira as informações necessárias, como nome da empresa, endereço e contato do local que você quer adicionar à empresa.
 
1. Clique em **Adicionar local**. Isso criará uma nova ID de MPN para o novo local que você pode usar para transações e incentivos do CSP.

:::image type="content" source="images/legal-biz.png" alt-text="Adicionar uma nova pessoa jurídica":::

> [!NOTE]
> Depois que um local for adicionado no Partner Center, você não poderá removê-lo. Você verá **MPN** no menu à esquerda do Partner Center se tiver usado a ID de MPN correta para entrar.

## <a name="add-the-registration-number-id"></a>Adicionar a ID do número de registro

Se você for um provedor indireto, parceiro de cobrança direto ou revendedor indireto e estiver fazendo negócios com clientes novos ou existentes nos países a seguir, será necessário fornecer números de ID de registro para sua empresa. Se o país onde você está fazendo negócios não estiver listado abaixo, a ID de registro será opcional.

- Armênia 
- Azerbaijão 
- Bielorrússia 
- Brasil 
- Hungria 
- Índia 
- Iraque 
- Cazaquistão 
- Quirguistão 
- Moldova 
- Myanmar 
- Polônia 
- Rússia 
- Arábia Saudita 
- África do Sul 
- Sudão do Sul  
- Tadjiquistão 
- Tailândia
- Turquia 
- Ucrânia 
- Emirados Árabes Unidos 
- Uzbequistão 
- Venezuela
- Vietnã 


Para obter mais informações, leia [Informações do número da ID de registro](reg-number-id.md)

## <a name="delete-a-location"></a>Excluir um local

Para excluir um local da sua conta, será necessário entrar em contato com o [Suporte a Parceiros](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b). Verifique se você entendeu o impacto que essa ação tem. Os locais excluídos não podem ser recuperados e qualquer coisa associada a essa ID de MPN específica não será mais reconhecida nem estará ativa para sua empresa.

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
