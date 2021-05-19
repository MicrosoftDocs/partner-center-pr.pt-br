---
title: Perfis de pagamento e impostos no Partner Center
ms.topic: how-to
ms.date: 04/15/2021
description: Crie e gerencie seu pagamento e seu perfil de impostos para que você possa ser pago pelo trabalho de seus incentivos. Inclui a criação, o gerenciamento e o uso de perfis diferentes.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: b167b0e65f3339a29f0227f6135ed70931300d8e
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152147"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a>Criar e gerenciar o pagamento de incentivos e perfis de impostos no Partner Center

**Funções apropriadas**: administrador de incentivos | Administrador da conta | Administrador global

Para receber o pagamento de seus programas de incentivo para um local de MPN específico, conclua o registro associando um perfil de pagamento e imposto válido ao programa e ao local de MPN. A Microsoft usará este perfil de pagamento e imposto para emitir pagamentos. Você pode usar transferência bancária eletrônica ou uma nota de crédito para pagamento, dependendo das regras do programa de incentivo. 

## <a name="roles-currencies-and-multiple-microsoft-incentive-programs"></a>Funções, moedas e vários programas de incentivo da Microsoft

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
>Você deve ser um administrador de incentivos para criar ou gerenciar perfis de pagamento e de impostos no Partner Center. As funções de incentivo devem ser atribuídas a cada local MPN em cada programa de incentivo. Para obter mais informações sobre como adicionar administradores de incentivo no Partner Center, consulte [Criar contas de usuário.](create-user-accounts-and-set-permissions.md)

## <a name="access-the-payout-and-tax-section-in-partner-center"></a>Acesse a seção de pagamento e imposto Partner Center

1. Entre no painel [de Partner Center](https://partner.microsoft.com/dashboard/) usando sua conta do Azure Active Directory (Azure AD) (conta da empresa) ou o endereço de email apropriado se um tiver sido atribuído.

   - Vários domínios podem ser registrados em uma conta do Azure AD. Entre em contato com o administrador global para determinar quais domínios estão associados.
   - Se você só conseguir entrar com o domínio e precisar de domínios adicionais, entre em contato com o administrador da conta para adicionar domínios adicionais à conta @onmicrosoft.com do Azure AD.
   - Se for solicitado que você selecione Conta de trabalho ou **de estudante** ou **Conta Pessoal,** selecione Conta de trabalho ou de **estudante.**

2. Selecione o ícone de engrenagem para abrir o menu **Configurações** e, em seguida, selecione **Configurações da conta**.

3. No menu **Configurações da conta,** selecione **Pagamento e imposto.**

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a>Atribuir perfis de pagamento e imposto a programas individuais

1. Entre no painel [Partner Center e](https://partner.microsoft.com/dashboard/)selecione o ícone de engrenagem para abrir o menu **Configurações.** 

2. Selecione **Configurações da conta**, expanda a seção Pagamento e imposto **e,** em seguida, **selecione Pagamento e atribuição de perfil de imposto**. 
   
   Uma lista de seus programas será exibida. Selecione a seta ao lado de um programa para ver os detalhes do perfil. 

3. No menu **suspenso Perfil Fiscal,** selecione o perfil fiscal desejado ou selecione a opção para criar um novo perfil. Ao selecionar a opção para criar um novo perfil, você será redirecionado adequadamente.  Selecione **Continuar** na janela pop-up. O processo para criar um novo perfil de imposto é fornecido abaixo.

4. Selecione **Forma de pagamento**.

   - Se você selecionou **Transferência bancária eletrônica** como sua forma de pagamento, selecione o perfil de pagamento desejado ou selecione a opção para criar um novo perfil. Ao selecionar a opção para criar um novo perfil, você será redirecionado adequadamente. Selecione continuar na janela pop-up. O processo para criar um novo perfil de pagamento foi fornecido abaixo.

   - Se você tiver selecionado **Nota de crédito** como seu método de pagamento, conclua a verificação. Isso confirma que o número SAP referenciado pertence à sua organização.

    >[!NOTE]
    >Se houver várias entidades comerciais da Microsoft listadas, você deverá selecionar um perfil de pagamento para cada entidade.

    >[!NOTE]
    >A disponibilidade do método de pagamento depende das regras do programa de incentivo.

    - Se a ID de MPN do local for paga por uma subsidiária local da Microsoft para um programa de incentivo específico e permitir o memorando de crédito LRD (distribuidor de risco limitado) como o método de pagamento, o perfil de pagamento será preenchido previamente com o método de pagamento de nota de crédito LRD. Na linha de método de pagamento de nota de crédito LRD para o respectivo programa de incentivo e ID de MPN de local, você verá a **confirmação** ou a **verificação necessária** como o status na seção perfil de pagamento.
    
       Selecione a **verificação necessária** para confirmar e verificar os detalhes da ID do locatário do CSP que estão associados ao local MPN e ao método de pagamento para receber o pagamento da nota de crédito. Na caixa de diálogo **detalhes da nota de crédito** , examine e verifique se a ID do locatário do CSP e os detalhes fornecidos estão corretos. Se você receber mais de uma ID de locatário, selecione cuidadosamente a ID do locatário do CSP na qual você deseja receber pagamentos. Em seguida, selecione **confirmar** para confirmar que os detalhes da empresa estão corretos e que o pagamento de incentivos deve ser feito na ID do locatário do CSP que você selecionou.
 
      Se o status mostrar **confirmado**, a atribuição da ID do locatário do CSP foi concluída e nenhuma ação adicional é necessária. Você ainda pode selecionar confirmado para ver os detalhes da atribuição.
   
      Em países que exigem que os parceiros solicitem explicitamente a aplicação de uma isenção de imposto, haverá uma opção para aplicar a isenção de imposto ao lado do perfil fiscal na seção perfil fiscal do programa de incentivos e local do MPN. A verificação dessa caixa aplicará benefícios de isenção de imposto à sua nota de crédito de incentivo. 
   
      Atualmente, a forma de pagamento de Nota de Crédito LRD está disponível apenas para parceiros da Austrália, Nova Zelândia e Canadá para o programa de Incentivo de Comércio da Microsoft. Se você for um parceiro de cobrança direta ou um provedor indireto nesses três países inscritos no programa MCI e não vir a nota de crédito LRD como a forma de pagamento disponível, confirme se a ID do locatário está associada à conta de local do MPN do parceiro relevante. Para obter mais informações sobre isso, [leia como atualizar o perfil da sua organização.](update-your-partner-profile.md)

    
5. Selecione a **moeda**.

6. Quando você concluir todos os campos de pagamento, selecione **Enviar**.

## <a name="set-up-a-default-bank-profile"></a>Configurar um perfil bancário padrão

Você pode configurar perfis bancários padrão e atribuí-los a locais do MPN. Esses perfis padrão serão usados pela Microsoft para registros subsequentes para esse local do MPN. 

1. Entre no painel [Partner Center e](https://partner.microsoft.com/dashboard/)selecione o ícone de engrenagem para abrir o menu ****   Configurações. 

2. Selecione **Configurações da conta**, expanda a **seção** Pagamento e imposto e, em seguida, **selecione Perfis de pagamento e imposto.** 

3. Selecione **Gerenciar perfis padrão** na seção **Perfis de** pagamento. 

4. Para criar um perfil bancário padrão, selecione **Adicionar um perfil bancário padrão.** 

5. Selecione um perfil bancário na lista de perfis bancários disponíveis da sua empresa, selecione a moeda a ser usada com esse perfil bancário e, em seguida, selecione a lista de locais do MPN para os quais você deseja que esse perfil padrão seja aplicado.

6. Selecione **Concluído** depois de concluir as seleções. O botão Concluído não poderá ser clicado até que todos os campos necessários sejam concluídos. 

>[!NOTE]
>O mesmo emparelhamento bancário e de moeda pode ser aplicado a vários locais. Se o local MPN tiver sido atribuído um perfil padrão e uma combinação de moeda uma vez, ele não aparecerá mais na lista suspensa local para atribuições de perfil padrão futuras. Se a seleção padrão for excluída, o local MPN será exibido novamente para as atribuições de perfil padrão futuras. Cada combinação de perfil e moeda do banco é adicionada como uma linha editável exclusiva.

7. Depois que todas as alterações necessárias tiverem sido adicionadas, selecione **salvar**.  

## <a name="create-your-bank-profile"></a>Criar seu perfil bancário

Os perfis bancários são criados no nível da empresa. Isso permite que um perfil de banco seja atribuído a vários programas de incentivo e ID de MPN dentro de uma empresa. Pode haver exceções ao aplicar o perfil bancário a diferentes países, já que regras de imposto e de bancos diferentes podem ser aplicadas.

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

Você será redirecionado para a página de **perfis de pagamento e impostos** . O status do seu novo perfil refletirá a **validação pendente da Microsoft** até que a validação tenha sido concluída. Esse processo pode levar até 48 horas. Depois que a validação for concluída, o status do perfil refletirá **Aprovado ou** **Ação necessária.** Se **a ação for necessária,** repita as etapas acima fornecendo as informações necessárias. 

## <a name="create-your-tax-profile"></a>Criar seu perfil de imposto

Use o procedimento a seguir para fornecer à Microsoft as informações fiscais necessárias para sua organização. As páginas nesta seção são dinâmicas e variam de acordo com seu país ou região. Se você precisar de ajuda para identificar as informações fiscais corretas, entre em contato com as fontes governamentais apropriadas em seu país.

Para empresas parceiras nas Américas, se você precisar de informações sobre como concluir os formulários W8 ou W9, os seguintes endereços levarão você ao site do IRS:

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> Insira apenas detalhes para sua empresa. Nunca insira detalhes pessoais.

1. Na página **Perfil de Negócios,** preencha os campos necessários e, em seguida, selecione **Próximo.** 

2. Na página **Instalação,** selecione a opção que se aplica à sua empresa.

   - Selecione a opção à esquerda se sua empresa for incorporada somente ao Estados Unidos ou se esse perfil for para um indivíduo.
   - Selecione a opção à direita se sua empresa for incorporada fora do Estados Unidos e, em seguida, selecione seu país/região na lista.

3. Selecione **Avançar**. 

4. Na página **Status do imposto,** insira as informações necessárias e selecione **Próximo.** Os campos nesta página variam de acordo com o país. seus detalhes. 

5. Na página **Documentação adicional,** os campos necessários e selecione **Próximo.** 

6. Selecione **Procurar** para carregar todos os documentos necessários para seu país ou região. Quando o nome do documento for mostrado, selecione **Carregar**. 

7. Se você precisar remover o documento, selecione **remover**.

8. Para salvar e continuar, selecione **concluir**.

9. Selecione **confirmar** na mensagem pop-up. Você será levado de volta à página de **configuração de pagamento e imposto** .
 
## <a name="update-expired-tax-profiles"></a>Atualizar perfis de imposto expirados

1. Entre no [painel do Partner Center](https://partner.microsoft.com/dashboard/)e selecione o ícone de engrenagem para abrir o menu **configurações** .

1. Selecione **configurações de conta**, expanda a seção **pagamento e imposto** e selecione **pagamento e perfil de imposto**.

1. Selecione o **perfil de imposto**.

1. Verifique a **data de expiração** da coluna e navegue até o perfil de imposto expirado ou prestes a expirar.

1. Selecione **Editar**.

1. Na seção formulário de imposto, atualize os formulários de imposto fornecendo os novos detalhes. 

## <a name="next-steps"></a>Próximas etapas

- [Perguntas comuns sobre pagamentos e impostos](payout-faq.md)
