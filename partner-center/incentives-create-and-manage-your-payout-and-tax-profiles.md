---
title: Criar e gerenciar perfis fiscais e de pagamento no Partner Center
ms.topic: article
ms.date: 06/29/2020
description: Antes que você possa ser pago pelo trabalho de seus incentivos, você precisa criar seus perfis de pagamento e de impostos.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.openlocfilehash: ed8820065c8c009e64419e58fa11758a27f95d7e
ms.sourcegitcommit: c4f2561fb7f224554c31e3af491de4ad65644158
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/23/2020
ms.locfileid: "87114089"
---
# <a name="payout-and-tax-profiles-in-partner-center"></a>Perfis de pagamento e impostos no Partner Center

Aplica-se a:

- Partner Center

Para receber o pagamento de seus programas de incentivo para um local de MPN específico, conclua o registro associando um perfil de pagamento e imposto válido ao programa e ao local de MPN. A Microsoft usará este perfil de pagamento e imposto para emitir pagamentos. Você pode usar transferência bancária eletrônica ou uma nota de crédito para pagamento, dependendo das regras do programa de incentivo. 

Funções apropriadas:

- Administrador de incentivos
- Administrador de cobrança
- Administrador global

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a>Criar e gerenciar perfis fiscais e de pagamento no Partner Center

As seções abaixo guiarão você pelo processo de criação e gerenciamento de perfis de pagamento e impostos no Partner Center.

>[!IMPORTANT]
>Você deve ser um administrador de incentivos para criar ou gerenciar perfis de pagamento no Partner Center. As funções de incentivo devem ser atribuídas a cada local MPN em cada programa de incentivo. Para obter mais informações sobre como adicionar administradores de incentivos no Partner Center, consulte [como adicionar usuários de incentivo ou administradores no Partner Center](https://support.microsoft.com/help/3011450/how-to-add-incentive-users-or-admins-in-partner-center).

## <a name="access-the-payout-and-tax-section-in-partner-center"></a>Acessar a seção pagamento e impostos no Partner Center

1. Faça logon no Partner Center usando sua conta do AAD (conta da empresa) ou o endereço de email apropriado, se um tiver sido atribuído. 

   - Vários domínios podem ser registrados em uma conta do AAD. Entre em contato com seu administrador global para determinar quais domínios estão associados.
   - Se você só puder fazer logon com **@onmicrosoft.com** o domínio, entre em contato com o administrador da conta para adicionar outros domínios à conta do AAD.
   - Se for solicitado que você selecione conta **corporativa ou de estudante** ou **conta pessoal**, selecione **conta corporativa ou de estudante**.

2. Selecione o ícone de engrenagem para abrir o menu **configurações** e, em seguida, selecione **configurações de parceiro**.

3. No menu **configurações de conta** , selecione **pagamento e imposto**. 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a>Atribuir pagamentos e perfis de impostos a programas individuais

1. No Partner Center, selecione o ícone de engrenagem para abrir o menu **configurações** . 

2. Selecione **configurações de parceiro**, expanda a **seção pagamento e imposto**e selecione **atribuição de perfil de pagamento e imposto**. 
   
   Será exibida uma lista de seus programas. Selecione a seta ao lado de um programa para ver os detalhes do perfil. 

3. No menu suspenso **perfil de imposto** , selecione o perfil de imposto desejado ou selecione a opção para criar um novo perfil. Ao selecionar a opção para criar um novo perfil, você será redirecionado adequadamente.  Selecione continuar na janela pop-up. O processo para criar um novo perfil de imposto foi fornecido abaixo.

4. Selecione o **método de pagamento**.

   - Se você tiver selecionado **transferência bancária eletrônica** como método de pagamento, em seguida, no menu suspenso perfil de pagamento, selecione o perfil de pagamento desejado ou selecione a opção para criar um novo perfil. Ao selecionar a opção para criar um novo perfil, você será redirecionado adequadamente.  Selecione continuar na janela pop-up. O processo para criar um novo perfil de pagamento foi fornecido abaixo.

   - Se você tiver selecionado **Nota de crédito** como o método de pagamento, conclua a verificação para confirmar se o número SAP referenciado pertence à sua organização.

    >[!NOTE]
    >Se houver várias entidades comerciais da Microsoft listadas, você deverá selecionar um perfil de pagamento para cada entidade.

    >[!NOTE]
    >A disponibilidade do método de pagamento depende das regras do programa de incentivo.
    
5. Selecione a **moeda**.

6. Quando você tiver concluído todos os campos de pagamento, selecione **Enviar**.

## <a name="create-your-bank-profile"></a>Criar seu perfil bancário

Os perfis bancários são criados em um nível de organização, o que permite que o mesmo perfil de banco seja atribuído a vários programas de incentivo e ID de MPN em uma organização. Pode haver exceções ao aplicar o perfil bancário a diferentes países, já que regras de imposto e de bancos diferentes podem ser aplicadas.

>[!NOTE]
>Nas páginas a seguir, são necessários campos com um asterisco. Se você não souber o que é um campo, selecione o ícone de informações. 

1. Na página **detalhes** , preencha os seguintes campos: **nome do perfil:** Insira um nome exclusivo para identificar este perfil de pagamento.
    **Local da conta bancária:** O país no qual o banco da sua empresa está localizado.
    **Método de pagamento:** O método de pagamento preferido é para o Partner Center ser transferência bancária eletrônica.

2. Selecione **Avançar**.

3. Na página **conta bancária** , insira suas informações. Os campos mostrados nesta página variam de acordo com o país. 

4. Selecione **Avançar**.

5. Na página do **beneficiário** , insira as informações apropriadas. O beneficiário é a pessoa em sua empresa que o banco deve contatar se precisar discutir sua conta.

6. Quando os campos forem concluídos, selecione **concluir**e, em seguida, selecione **confirmar** para criar seu perfil bancário.

Você será redirecionado para a página de **perfis de pagamento e impostos** . O status do seu novo perfil refletirá a **validação pendente da Microsoft** até que a validação tenha sido concluída. Isso pode levar até 48 horas. Após a conclusão da validação, o status do perfil refletirá **aprovado** ou **ação necessária**. Se a **ação for necessária**, repita as etapas acima fornecendo as informações necessárias. 

## <a name="create-your-tax-profile"></a>Criar seu perfil de imposto

Use o procedimento a seguir para fornecer à Microsoft as informações de impostos necessárias para sua organização. As páginas nesta seção são dinâmicas e variam de acordo com seu país ou região. Se você precisar de ajuda para identificar as informações de imposto corretas, entre em contato com as fontes governamentais apropriadas em seu país.

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

## <a name="payout-and-tax-profile-faqs"></a>Perguntas frequentes sobre pagamento e perfil fiscal

### <a name="why-do-i-need-to-provide-my-payout-andor-tax-details"></a>Por que preciso fornecer meus detalhes de pagamento e/ou imposto?

Para receber pagamentos para programas de incentivo da Microsoft, você precisa concluir o registro fornecendo detalhes válidos de pagamento e imposto. Um registro é considerado completo somente quando o pagamento e o perfil de impostos que você fornece são validados pela Microsoft.

### <a name="how-do-i-know-that-i-need-to-provideupdate-my-payout-andor-tax-details"></a>Como fazer saber que preciso fornecer/atualizar meus detalhes de pagamento e/ou imposto?

Todos os parceiros registrados em um novo programa de incentivo devem fornecer pagamento e detalhes de impostos válidos para concluir o registro.

Talvez você também precise fornecer informações atualizadas se as regras do seu programa de incentivos forem alteradas ou se os aspectos do perfil expirarem ou ficarem desatualizados. Se isso acontecer, sua página de visão geral mostrará um status de **ação necessária – atualizar banco e/ou perfil de imposto**.

### <a name="how-do-i-provide-update-my-payout-and-or-tax-details"></a>Como posso fornecer/atualizar meus detalhes de pagamento e/ou imposto?

Para obter informações detalhadas sobre como atualizar os detalhes de pagamento e impostos no Partner Center, consulte [como criar e gerenciar perfis bancários e de impostos no Partner Center](https://support.microsoft.com/help/4524534/how-to-create-and-manage-bank-and-tax-profiles-in-partner-center)

### <a name="why-dont-i-see-my-enrollments-when-i-go-to-assign-my-payout-and-tax-profile"></a>Por que não vejo meus registros ao atribuir meu perfil de pagamento e imposto?

Somente os administradores de incentivos do seu local de MPN podem criar ou gerenciar os perfis de pagamento e imposto. Pode ser que você não tenha as permissões adequadas ou que esteja conectado com uma conta que não possui essas permissões. Entre em contato com o administrador da organização para gerenciar as permissões bancárias e fiscais.

### <a name="where-can-i-see-the-payout-and-tax-profiles-for-my-organization-that-i-can-use"></a>Onde posso ver os perfis de pagamento e de impostos da minha organização que posso usar?

Use o procedimento a seguir para ver os perfis de pagamento e de impostos:

1. Entre no Partner Center.

2. Selecione o ícone de engrenagem para abrir o menu de **Configurações**.

3. Selecione **configurações de parceiro**.

4. Em **Configurações da conta**, selecione **Pagamento e taxa**, em seguida, selecione **Perfil de Pagamento e fiscal**. Você verá todos os perfis de pagamento e fiscais existentes junto com o status e a capacidade de editar.

### <a name="my-organization-is-participating-in-multiple-incentive-programs-do-i-need-to-provide-my-payment-and-tax-profile-multiple-times"></a>Minha organização está participando de vários programas de incentivos. Preciso fornecer meu pagamento e perfil de impostos várias vezes?

Com os perfis de pagamento, geralmente é opção sua. Os perfis de pagamento são criados em um nível de organização, o que permite que o mesmo perfil de banco seja atribuído a vários programas de incentivo e ID de MPN em uma organização. Na maioria dos casos, você pode reutilizar um perfil existente ou criar um novo.

No entanto, pode haver exceções ao aplicar seu perfil bancário a diferentes países ou regiões, já que as regras fiscais ou de banco local podem ser aplicadas.

Os perfis fiscais criados para um MPN local são reutilizados e preenchidos automaticamente, quando o mesmo local MPN participa de outro programa de incentivo. Mas pode haver exceções. Por exemplo, as regras de pagamento de um novo programa de incentivo podem exigir detalhes adicionais para o perfil fiscal.  

### <a name="i-am-only-able-to-log-in-with-my-onmicrosoftcom-domain-what-should-i-do"></a>Só posso fazer logon com meu @onmicrosoft.com domínio. O que devo fazer?

Contate o administrador da conta para adicionar outros domínios à conta do AAD.
