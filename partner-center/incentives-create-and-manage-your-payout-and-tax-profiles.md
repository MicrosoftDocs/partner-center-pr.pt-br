---
title: Perfis de pagamento e impostos no Partner Center
ms.topic: how-to
ms.date: 02/24/2021
description: Crie e gerencie seu pagamento e seu perfil de impostos para que você possa ser pago pelo trabalho de seus incentivos. Inclui a criação, o gerenciamento e o uso de perfis diferentes.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: ba8c1a811d66a5e6233f625c3981283341ea546c
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756599"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a>Criar e gerenciar o pagamento de incentivos e perfis de impostos no Partner Center


**Funções apropriadas:**

- Administrador de incentivos
- Administrador de conta
- Administrador global

Para receber o pagamento de seus programas de incentivo para um local de MPN específico, conclua o registro associando um perfil de pagamento e imposto válido ao programa e ao local de MPN. A Microsoft usará este perfil de pagamento e imposto para emitir pagamentos. Você pode usar transferência bancária eletrônica ou uma nota de crédito para pagamento, dependendo das regras do programa de incentivo. 

## <a name="roles-currencies-and-other-microsoft-programs"></a>Funções, moedas e outros programas da Microsoft

É importante entender as informações abaixo antes de começar com o pagamento e o perfil de impostos.

### <a name="roles-and-permissions"></a>Funções e permissões

Você deve ser um administrador de incentivos para inserir informações bancárias e de impostos para pagamentos de incentivos. Se você for um administrador de MPN/conta, você pode atribuir a si mesmo e/ou um colega para ser o administrador de incentivos.

Se você precisar solicitar as permissões de administrador de incentivos, entre em contato com o administrador do MPN ou com o administrador global. Você pode descobrir quem em sua empresa tem essas funções entrando no [painel do Partner Center](https://partner.microsoft.com/dashboard/). No ícone de **configurações** no canto superior direito, selecione **Gerenciamento de usuários** e filtre o administrador global.

Os incentivos podem exibir os ganhos de incentivos e os detalhes e relatórios de pagamento, mas não podem editar os detalhes bancários e de imposto.

### <a name="choose-your-disbursement-currency"></a>Escolha sua moeda de pagamento

Os pagamentos de incentivo são feitos na moeda que você selecionou ao configurar seu perfil de pagamento. Os pagamentos serão calculados usando uma taxa de câmbio como definido mensalmente pela Microsoft. Você será responsável por qualquer alteração no valor devido à moeda selecionada.

### <a name="using-different-profiles-for-different-microsoft-programs"></a>Usando perfis diferentes para programas diferentes da Microsoft

Se sua empresa estiver inscrita em vários programas de incentivo, você poderá usar a mesma conta de pagamento para todos eles ou optar por usar contas de pagamento diferentes para programas diferentes.

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a>Criar e gerenciar perfis fiscais e de pagamento no Partner Center

As seções abaixo guiarão você pelo processo de criação e gerenciamento de perfis de pagamento e impostos no Partner Center.

>[!IMPORTANT]
>Você deve ser um administrador de incentivos para criar ou gerenciar perfis de pagamento no Partner Center. As funções de incentivo devem ser atribuídas a cada local MPN em cada programa de incentivo. Para obter mais informações sobre como adicionar administradores de incentivos no Partner Center, consulte [criar contas de usuário](create-user-accounts-and-set-permissions.md).

## <a name="access-the-payout-and-tax-section-in-partner-center"></a>Acessar a seção pagamento e impostos no Partner Center

1. Entre no [painel do Partner Center](https://partner.microsoft.com/dashboard/) usando sua conta do Azure Active Directory (Azure AD) (conta da empresa) ou o endereço de email apropriado, se um tiver sido atribuído.

   - Vários domínios podem ser registrados em uma conta do Azure AD. Entre em contato com seu administrador global para determinar quais domínios estão associados.
   - Se você só puder fazer logon com o @onmicrosoft.com domínio, entre em contato com o administrador da conta para adicionar outros domínios à conta do Azure AD.
   - Se for solicitado que você selecione conta **corporativa ou de estudante** ou **conta pessoal**, selecione **conta corporativa ou de estudante**.

2. Selecione o ícone de engrenagem para abrir o menu **configurações** e, em seguida, selecione **configurações de conta**.

3. No menu **configurações de conta** , selecione **pagamento e imposto**. 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a>Atribuir pagamentos e perfis de impostos a programas individuais

1. Entre no [painel do Partner Center](https://partner.microsoft.com/dashboard/)e selecione o ícone de engrenagem para abrir o menu **configurações** . 

2. Selecione **configurações de conta**, expanda a **seção pagamento e imposto** e selecione **atribuição de perfil de pagamento e imposto**. 
   
   Será exibida uma lista de seus programas. Selecione a seta ao lado de um programa para ver os detalhes do perfil. 

3. No menu suspenso **perfil de imposto** , selecione o perfil de imposto desejado ou selecione a opção para criar um novo perfil. Ao selecionar a opção para criar um novo perfil, você será redirecionado adequadamente.  Selecione continuar na janela pop-up. O processo para criar um novo perfil de imposto foi fornecido abaixo.

4. Selecione o **método de pagamento**.

   - Se você selecionou **transferência bancária eletrônica** como seu método de pagamento, selecione o perfil de pagamento desejado ou selecione a opção para criar um novo perfil. Ao selecionar a opção para criar um novo perfil, você será redirecionado adequadamente. Selecione continuar na janela pop-up. O processo para criar um novo perfil de pagamento foi fornecido abaixo.

   - Se você tiver selecionado **Nota de crédito** como seu método de pagamento, conclua a verificação. Isso confirma que o número SAP referenciado pertence à sua organização.

    >[!NOTE]
    >Se houver várias entidades comerciais da Microsoft listadas, você deverá selecionar um perfil de pagamento para cada entidade.

    >[!NOTE]
    >A disponibilidade do método de pagamento depende das regras do programa de incentivo.

    - Se a ID de MPN do local for paga por uma subsidiária local da Microsoft para um programa de incentivo específico e permitir o memorando de crédito LRD (distribuidor de risco limitado) como o método de pagamento, o perfil de pagamento será preenchido previamente com o método de pagamento de nota de crédito LRD. Na linha de método de pagamento de nota de crédito LRD para o respectivo programa de incentivo e ID de MPN de local, você verá a **confirmação** ou a **verificação necessária** como o status na seção perfil de pagamento.
    
       Selecione a **verificação necessária** para confirmar e verificar os detalhes da ID do locatário do CSP que estão associados ao local MPN e ao método de pagamento para receber o pagamento da nota de crédito. Na caixa de diálogo **detalhes da nota de crédito** , examine e verifique se a ID do locatário do CSP e os detalhes fornecidos estão corretos. Se você receber mais de uma ID de locatário, selecione cuidadosamente a ID do locatário do CSP na qual você deseja receber pagamentos. Em seguida, selecione **confirmar** para confirmar que os detalhes da empresa estão corretos e que o pagamento de incentivos deve ser feito na ID do locatário do CSP que você selecionou.
 
      Se o status mostrar **confirmado**, a atribuição da ID do locatário do CSP foi concluída e nenhuma ação adicional é necessária. Você ainda pode selecionar confirmado para ver os detalhes da atribuição.
   
      Em países que exigem que os parceiros solicitem explicitamente a aplicação de uma isenção de imposto, haverá uma opção para aplicar a isenção de imposto ao lado do perfil de imposto na seção perfil de imposto do programa de incentivo e do local MPN. Marcar esta caixa aplicará benefícios de isenção de imposto à sua nota de crédito de incentivo. 
   
      Atualmente, esse método de pagamento está disponível apenas para os parceiros da Austrália, da Nova Zelândia e do Canadá do programa de incentivo do Microsoft Commerce. Se você for um parceiro de cobrança direta ou um provedor indireto nesses três países registrados para o programa MCI e não vir a nota de crédito do LRD como o método de pagamento disponível, confirme se sua ID de locatário está associada à conta de local do parceiro MPN relevante. Para obter mais informações sobre este leia [como atualizar seu perfil de organização](update-your-partner-profile.md).

    
5. Selecione a **moeda**.

6. Quando você tiver concluído todos os campos de pagamento, selecione **Enviar**.


## <a name="create-your-bank-profile"></a>Criar seu perfil bancário

Os perfis bancários são criados em um nível de organização. Isso permite que um perfil de banco seja atribuído a vários programas de incentivo e IDs de MPN em uma organização. Pode haver exceções ao aplicar o perfil bancário a diferentes países, já que regras de imposto e de bancos diferentes podem ser aplicadas.

>[!NOTE]
>Nas páginas a seguir, são necessários campos com um asterisco. Se você não souber o que é um campo, selecione o ícone de informações. 

1. Na página **detalhes** , preencha os seguintes campos: **nome do perfil:** Insira um nome exclusivo para identificar este perfil de pagamento.
    **Local da conta bancária:** O país no qual o banco da sua empresa está localizado.
    **Método de pagamento:** O método de pagamento preferencial para o Partner Center é a transferência bancária eletrônica.

2. Selecione **Avançar**.

3. Na página **conta bancária** , insira suas informações. Os campos mostrados nesta página variam de acordo com o país. 

4. Selecione **Avançar**.

5. Na página do **beneficiário** , insira as informações apropriadas. O beneficiário é a pessoa em sua empresa que o banco deve contatar se precisar discutir sua conta.

6. Quando os campos forem concluídos, selecione **concluir** e, em seguida, selecione **confirmar** para criar seu perfil bancário.

Você será redirecionado para a página de **perfis de pagamento e impostos** . O status do seu novo perfil refletirá a **validação pendente da Microsoft** até que a validação tenha sido concluída. Esse processo pode levar até 48 horas. Após a conclusão da validação, o status do perfil refletirá **aprovado** ou **ação necessária**. Se a **ação for necessária**, repita as etapas acima fornecendo as informações necessárias. 

## <a name="create-your-tax-profile"></a>Criar seu perfil de imposto

Use o procedimento a seguir para fornecer à Microsoft as informações de impostos necessárias para sua organização. As páginas nesta seção são dinâmicas e variam de acordo com seu país ou região. Se precisar de ajuda para identificar as informações de imposto corretas, entre em contato com as fontes governamentais apropriadas em seu país.

Para empresas parceiras nas Américas, se você precisar de informações sobre como concluir os formulários W8 ou W9, os seguintes endereços levarão você para o site IRS:

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> Insira apenas os detalhes de sua empresa. Nunca insira detalhes pessoais.

1. Na página **perfil de negócios** , preencha os campos obrigatórios e, em seguida, selecione **Avançar**. 

2. Na página **instalação** , selecione a opção que se aplica à sua empresa.

   - Selecione a opção à esquerda se sua empresa estiver incorporada somente no Estados Unidos ou se esse perfil for um indivíduo.
   - Selecione a opção à direita se sua empresa estiver incorporada fora do Estados Unidos e, em seguida, selecione seu país/região na lista.

3. Selecione **Avançar**. 

4. Na página **status do imposto** , insira as informações necessárias e, em seguida, selecione **Avançar**. Os campos nesta página variam de acordo com o país. seus detalhes. 

5. Na página de **documentação adicional** , os campos obrigatórios e selecione **Avançar**. 

6. Selecione **procurar** para carregar todos os documentos exigidos por seu país ou região. Quando o nome do documento for mostrado, selecione **carregar**. 

7. Se você precisar remover o documento, selecione **remover**.

8. Para salvar e continuar, selecione **concluir**.

9. Selecione **confirmar** na mensagem pop-up. Você será levado de volta à página de **configuração de pagamento e imposto** .

## <a name="next-steps"></a>Próximas etapas

- [Perguntas comuns sobre pagamentos e impostos](payout-faq.md)
