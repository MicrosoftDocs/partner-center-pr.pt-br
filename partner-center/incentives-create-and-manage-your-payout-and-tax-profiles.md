---
title: Perfis de pagamento e impostos no Partner Center
ms.topic: how-to
ms.date: 04/15/2021
description: Crie e gerencie seu perfil de pagamento e imposto para que você possa ser pago pelo trabalho de incentivos. Inclui criar, gerenciar e usar perfis diferentes.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: a6d578c2ad09e1f8bb03f520d659f1a9b1e199a9
ms.sourcegitcommit: a09a5f893e876de23a8aa5c0d637e50c5be84941
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "113684246"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a>Criar e gerenciar perfis de pagamento e imposto de incentivos Partner Center

**Funções apropriadas:** incentivos de administrador | Conta de administrador | Administrador global

Para receber o pagamento de seus programas de incentivo para um local de MPN específico, conclua o registro associando um perfil de pagamento e imposto válido ao programa e ao local de MPN. A Microsoft usará este perfil de pagamento e imposto para emitir pagamentos. Você pode usar transferência bancária eletrônica ou uma nota de crédito para pagamento, dependendo das regras do programa de incentivo. 

## <a name="roles-currencies-and-multiple-microsoft-incentive-programs"></a>Funções, moedas e vários programas de incentivo da Microsoft

É importante entender as informações abaixo antes de começar a trabalhar com seu perfil de pagamento e imposto.

### <a name="roles-and-permissions"></a>Funções e permissões

Você deve ser um Administrador de Incentivos para inserir informações bancárias e fiscais para pagamentos de incentivos. Se você for um administrador do MPN/Conta, poderá atribuir a si mesmo e/ou a um colega para ser o Administrador de Incentivos.

Se você precisar solicitar permissões de Administrador de Incentivos, entre em contato com o Administrador do MPN ou o Administrador Global. Você pode descobrir quem em sua empresa tem essas funções entrando no [painel Partner Center .](https://partner.microsoft.com/dashboard/) No ícone **Configurações** superior direito, **selecione** Gerenciamento de Usuários e, em seguida, filtre por Administrador Global.

Incentivos Os usuários podem exibir ganhos de incentivo e detalhes de pagamento e relatórios, mas não podem editar detalhes bancários e fiscais.

### <a name="choose-your-disbursement-currency"></a>Escolha sua moeda de desembolso

Os pagamentos de incentivo são feitos na moeda selecionada quando você configura seu perfil de pagamento. Os pagamentos serão calculados usando uma taxa de câmbio conforme definido mensalmente pela Microsoft. Você será responsável por todas as alterações no valor devido à moeda selecionada.

### <a name="using-different-profiles-for-different-microsoft-programs"></a>Usando perfis diferentes para diferentes programas da Microsoft

Se sua empresa estiver inscrita em vários programas de incentivo, você poderá usar a mesma conta de pagamento para todos eles ou optar por usar contas de pagamento diferentes para programas diferentes.

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a>Criar e gerenciar perfis fiscais e de pagamento no Partner Center

As seções a seguir explicam o processo de criação e gerenciamento de perfis de pagamento e imposto Partner Center.

>[!IMPORTANT]
>Você deve ser um administrador de incentivos para criar ou gerenciar perfis de pagamento e imposto Partner Center. As funções de incentivo devem ser atribuídas a cada local do MPN em cada programa de incentivo. Para obter mais informações sobre como adicionar administradores de incentivo no Partner Center, consulte [Criar contas de usuário.](create-user-accounts-and-set-permissions.md)

## <a name="access-the-payout-and-tax-section-in-partner-center"></a>Acesse a seção de pagamento e imposto Partner Center

1. Entre no painel [Partner Center usando](https://partner.microsoft.com/dashboard/) sua conta do Azure Active Directory (Azure AD) (conta da empresa) ou o endereço de email apropriado se um tiver sido atribuído.

   - Vários domínios podem ser registrados em uma conta do Azure AD. Entre em contato com o administrador global para determinar quais domínios estão associados.
   - Se você só conseguir entrar com o domínio e precisar de domínios adicionais, entre em contato com o administrador da conta para adicionar domínios adicionais à conta @onmicrosoft.com do Azure AD.
   - Se for solicitado que você selecione Conta de trabalho ou **de estudante** ou **Conta Pessoal,** selecione Conta de trabalho ou de **estudante.**

2. Selecione o ícone de engrenagem para abrir o menu **Configurações** e, em seguida, selecione **Configurações de conta**.

3. No menu **Configurações da conta,** selecione **Pagamento e imposto.**

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a>Atribuir perfis de pagamento e imposto a programas individuais

1. Entre no painel [Partner Center e](https://partner.microsoft.com/dashboard/)selecione o ícone de engrenagem para abrir o menu **Configurações.** 

2. Selecione **Configurações da conta**, expanda a seção Pagamento e imposto **e,** em seguida, **selecione Pagamento e atribuição de perfil de imposto**. 
   
   Uma lista de seus programas será exibida. Selecione a seta ao lado de um programa para ver os detalhes do perfil. 

3. No menu **suspenso Perfil Fiscal,** selecione o perfil fiscal desejado ou selecione a opção para criar um novo perfil. Ao selecionar a opção para criar um novo perfil, você será redirecionado adequadamente.  Selecione **Continuar** na janela pop-up. O processo para criar um novo perfil de imposto é fornecido abaixo.

4. Selecione **Forma de pagamento**.

   - Se você selecionou **Transferência bancária eletrônica** como sua forma de pagamento, selecione o perfil de pagamento desejado ou selecione a opção para criar um novo perfil. Ao selecionar a opção para criar um novo perfil, você será redirecionado adequadamente. Selecione Continuar na janela pop-up. O processo para criar um novo perfil de pagamento foi fornecido abaixo.

   - Se você **selecionou Nota de Crédito** como sua forma de pagamento, conclua a verificação. Isso confirma que o número SAP referenciado pertence à sua organização.

    >[!NOTE]
    >Se houver várias entidades de negócios da Microsoft listadas, você deverá selecionar um perfil de pagamento para cada entidade.

    >[!NOTE]
    >A disponibilidade da forma de pagamento depende das regras do programa de incentivo.

    - Se a ID do MPN de local for paga por uma subsidiária local da Microsoft para um programa de incentivo específico e permitir o memorando de crédito LRD (distribuidor de risco limitado) como a forma de pagamento, seu perfil de pagamento será preenchido previamente com a forma de pagamento da Nota de Crédito LRD. Na linha da forma de pagamento da nota de crédito LRD para  o  respectivo programa de incentivo e a ID do MPN de localização, você verá Confirmado ou Verificação Necessária como o status na seção perfil de pagamento.
    
       Selecione **Verificação necessária para** confirmar e verificar os detalhes da ID do locatário do CSP que estão associados ao MPN local e à forma de pagamento para receber o pagamento da nota de crédito. Na caixa **de diálogo Detalhes da** Nota de Crédito , revise e verifique se a ID do Locatário do CSP e os detalhes fornecidos estão corretos. Se você receber mais de uma ID de locatário, selecione cuidadosamente a ID do locatário do CSP na qual deseja receber pagamentos. Em seguida, **selecione Confirmar** para confirmar se os detalhes da sua empresa estão corretos e se o pagamento de incentivo deve ser feito na ID do locatário do CSP que você selecionou.
 
      Se o status mostrar **Confirmado**, a atribuição da ID do locatário do CSP foi concluída e nenhuma ação mais é necessária. Você ainda pode selecionar Confirmado para ver os detalhes da atribuição.
   
      Em países que exigem que os parceiros solicitem explicitamente a aplicação de uma isenção de imposto, haverá uma opção para aplicar a isenção de imposto ao lado do perfil fiscal na seção perfil fiscal do programa de incentivos e local do MPN. A verificação dessa caixa aplicará benefícios de isenção de imposto à sua nota de crédito de incentivo. 
   
      Atualmente, a forma de pagamento de Nota de Crédito LRD está disponível apenas para parceiros da Austrália, Nova Zelândia e Canadá para o programa de Incentivo de Comércio da Microsoft. Se você for um parceiro de cobrança direta ou um provedor indireto nesses três países inscritos no programa MCI e não vir a nota de crédito LRD como a forma de pagamento disponível, confirme se a ID do locatário está associada à conta de local do MPN do parceiro relevante. Para obter mais informações sobre isso, [leia como atualizar o perfil da sua organização.](update-your-partner-profile.md)

    
5. Selecione o **Conversor de Moedas**.

6. Quando você concluir todos os campos de pagamento, selecione **Enviar**.

## <a name="set-up-a-default-bank-profile"></a>Configurar um perfil bancário padrão

É possível configurar perfis de banco padrão e atribuí-los aos locais MPN. Os perfis padrão serão usados pela Microsoft para registros subsequentes para esse local do MPN. 

1. Entre no painel [Partner Center e](https://partner.microsoft.com/dashboard/)selecione o ícone de engrenagem para abrir o menu **Configurações**   aplicativo. 

2. Selecione **Configurações da conta**, expanda a **seção** Pagamento e imposto e, em seguida, **selecione Perfis de pagamento e imposto.** 

3. Selecione **Gerenciar perfis padrão** na seção **Perfis de** pagamento. 

4. Para criar um perfil bancário padrão, selecione **Adicionar um perfil bancário padrão.** 

5. Selecione um perfil bancário na lista de perfis bancários disponíveis da sua empresa, selecione a moeda a ser usada com esse perfil bancário e, em seguida, selecione a lista de locais do MPN para os quais você deseja que esse perfil padrão seja aplicado.

6. Selecione **Concluído** depois de concluir as seleções. O botão Concluído não poderá ser clicado até que todos os campos necessários sejam concluídos. 

>[!NOTE]
>O mesmo emparelhamento bancário e de moeda pode ser aplicado a vários locais. Se o MPN de local tiver sido atribuído a uma combinação de perfil e moeda padrão uma vez, ele não aparecerá mais na lista de locais para futuras atribuições de perfil padrão. Se a seleção padrão for excluída, o MPN de local reaparecerá para futuras atribuições de perfil padrão. Cada combinação de perfil bancário e moeda é adicionada como uma linha exclusiva e editável.

7. Depois que todas as alterações necessárias foram adicionadas, selecione **Salvar**.  

## <a name="create-your-bank-profile"></a>Criar seu perfil bancário

Os perfis bancários são criados no nível da empresa. Isso permite que um perfil bancário seja atribuído em vários programas de IDs e incentivos do MPN em uma empresa. Pode haver exceções ao aplicar o perfil bancário a diferentes países, pois diferentes regras bancárias e fiscais podem ser aplicadas.

>[!NOTE]
>Nas páginas a seguir, são necessários campos com um asterisco. Se você não sabe o que é um campo, selecione o ícone de informações. 

1. Na página **Detalhes,** preencha os seguintes campos: **Nome do perfil: insira** um nome exclusivo para identificar esse perfil de pagamento.
    **Local da conta bancária:** O país no qual o banco da sua empresa está localizado.
    **Forma de pagamento:** A forma de pagamento preferencial para Partner Center é a transferência bancária eletrônica.

2. Selecione **Avançar**.

3. Na página **Conta bancária,** insira suas informações. Os campos mostrados nesta página variam de acordo com o país. 

4. Selecione **Avançar**.

5. Na página **Beneficiária,** insira as informações apropriadas. O beneficiário é a pessoa em sua empresa que o banco contatará se precisar discutir sua conta.

6. Quando os campos são concluídos, selecione **Concluir** e, em seguida, **selecione Confirmar** para criar seu perfil bancário.

Você será redirecionado para a **página Perfis de pagamento e imposto.** O status do novo perfil refletirá a **validação** pendente da Microsoft até que a validação seja concluída. Esse processo pode levar até 48 horas. Depois que a validação for concluída, o status do perfil refletirá **Aprovado ou** **Ação necessária.** Se **a ação for necessária,** repita as etapas acima fornecendo as informações necessárias. 

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

6. Selecione **Procurar** para carregar todos os documentos necessários para seu país ou região. Quando o nome do documento for mostrado, **selecione Upload**. 

7. Se você precisar remover o documento, selecione **Remover**.

8. Para salvar e continuar, selecione **Concluir**.

9. Selecione **Confirmar** na mensagem pop-up. Você será levado de volta para a **página Configuração de pagamento e imposto.**
 
## <a name="update-expired-tax-profiles"></a>Atualizar perfis de imposto expirados

1. Entre no painel [Partner Center e](https://partner.microsoft.com/dashboard/)selecione o ícone de engrenagem para abrir o menu **Configurações.**

1. Selecione **Configurações da conta**, expanda a **seção** Pagamento e imposto e, em seguida, selecione Pagamento e perfil **de imposto.**

1. Selecione **Perfil de imposto**.

1. Verifique a coluna **Data de Validade** e navegue até o perfil fiscal que expirou ou está prestes a expirar.

1. Selecione **Editar**.

1. Na seção formulário de imposto, atualize os formulários de imposto fornecendo os novos detalhes. 

## <a name="next-steps"></a>Próximas etapas

- [Perguntas comuns sobre pagamentos e impostos](payout-faq.yml)
