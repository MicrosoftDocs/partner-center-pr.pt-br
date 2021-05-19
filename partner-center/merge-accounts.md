---
title: Mesclar sua conta de parceiro com outra conta de parceiro
description: Saiba como mesclar sua conta de parceiro com outra conta de parceiro no Partner Center-para empresas que estão ativas parceiros da Microsoft no Partner Center.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: parthpandyaMSFT
ms.author: parthp
ms.custom: seodec18
ms.date: 06/12/2020
ms.openlocfilehash: 8c47204d54cf05113eae73cede4afedf106ac121
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146503"
---
# <a name="merge-your-partner-account-with-another-partner-account"></a>Mesclar sua conta de parceiro com outra conta de parceiro

**Funções apropriadas**: administrador da conta

Duas ou mais empresas que estão ativas parceiros da Microsoft e que têm contas no Partner Center podem optar por mesclar suas contas.

## <a name="what-happens-when-two-partners-elect-to-merge-their-partner-center-accounts"></a>O que acontece quando dois parceiros optam por mesclar suas contas do Partner Center

- A organização parceira que inicia a mesclagem será a conta global do parceiro (PGA).

- O PGA da organização convidada se torna um local da empresa inicial.

- Todos os locais da conta de mesclagem se tornam locais sob o PGA.

- Depois que a fusão de contas for concluída, você verá os detalhes da conta, como locais e usuários no perfil do PGA. Não é possível reverter esse processo.

- Todas as IDs de MPN para locais são preservadas durante essa consolidação.

- As funções do usuário são trazidas. Por exemplo, se um usuário tivesse sido o administrador de incentivos para um local específico, ele ainda teria essa função após a fusão e poderá ver os incentivos vistos antes da fusão.

- Os locatários e as contas do CSP do Azure AD não são mesclados e não têm nenhum efeito.

- As ofertas publicadas e os dados de pipeline de venda conjunta associados a ambas as empresas são preservados

### <a name="view-of-merged-accounts"></a>Exibição de contas mescladas

:::image type="content" source="images/merge-accounts/account-merge.png" alt-text="Fusão de contas":::

## <a name="what-to-expect-if-you-have-been-invited-to-merge-your-partner-center-account-with-another-partner-center-account"></a>O que esperar se você tiver sido convidado para mesclar sua conta do Partner Center com outra conta do Partner Center

Se você decidir aceitar o convite para mesclar contas: · Suas IDs e locais de MPN serão mescladas no PGA da conta de parceiro que o convidou.

- Os usuários serão trazidos para a conta mesclada com suas funções intactas.

- Os benefícios e as competências existentes serão preservadas para ambas as empresas após a refusão até a renovação. Na renovação, as contas serão tratadas como uma empresa e as regras de renovação padrão serão aplicadas.

## <a name="understand-the-impacts-to-programs-and-benefits-when-partners-elect-to-merge-accounts"></a>Entender os impactos em programas e benefícios quando os parceiros optam por mesclar contas

- Todas as competências existentes (Gold/Silver), compras (como Microsoft Action Pack) e benefícios associados são preservados durante a consolidação. Se ambas as empresas têm a mesma competência, mas uma é ouro e a outra prata, a competência com o nível de proficiência mais alto será concedida e os parceiros terão um conjunto de benefícios pratas e um conjunto de benefícios ouro para essa competência até a próxima renovação. 

- A data de aniversário mais alta para o Microsoft Action Pack será mantida após a fusão. Por exemplo, se a data de aniversário da empresa 1 for junho de 2020 para renovação do Action Pack e a data de aniversário da renovação do Action Pack para a empresa 2 for outubro de 2020, a Microsoft usará a data de outubro de 2020 como a nova data de aniversário para a empresa mesclada.

- Durante a fusão da conta e até a próxima renovação, cada conta manterá seus Action Pack e/ou benefícios de competência. Na renovação, as regras de Action Pack padrão e de renovação de competência se aplicam.

- Após a renovação, os benefícios que estão incluídos com a Action Pack de competência são implementados para a conta global de parceiro da empresa parceira:

  - Microsoft Action Pack: a empresa parceira poderá comprar uma conta Action Pack por parceiro global.

  - Competência: a empresa parceira receberá um pacote de principais benefícios, associados à sua maior realização, além de benefícios específicos de competência que o parceiro está qualificado para cada conta global de parceiro.

- Todos os benefícios estão sujeitos ao guia [de uso Microsoft Partner Network benefícios.](https://aka.ms/partner-benefits-use-guide) Por exemplo: um token O365 E3 ativado é funcional por 12 meses após a ativação. Depois que um token tiver sido ativado para licenças em um locatário, essas licenças poderão não ser movidas para outro locatário.

- As associações de ID do MCP para ambas as empresas serão mantidas e associadas à ID do MPN do PGA.

- As vantagens para o mercado e os benefícios técnicos são oferecidas como um benefício principal de competência. Após a mesclagem, é recomendável que você verifique suas informações bancárias e fiscais para garantir a exatidão.

- Se sua empresa estiver no programa MSP do especialista do Azure, os benefícios serão mantidos até a renovação.

- Se a sua empresa ganhou especializações avançadas, elas são mantidas em ambas as contas são mantidas.

- Os comprovantes do Software Assurance são mantidos em ambas as contas. 

- Não há nenhum efeito para a associação DPOR ou PAL. Todas as contribuições de receita associadas começarão a fluir para a nova conta global do parceiro

## <a name="invite-a-company-to-merge-their-partner-center-account-with-your-partner-center-account"></a>Convide uma empresa para mesclar sua conta do Partner Center com sua conta do Partner Center

>[!Note]
>Para executar a fusão de contas, você deve ser o **administrador da conta** da sua empresa.

1. Selecione **configurações** no painel do Partner Center. 

2. Selecione **mesclagem de conta**.

3. Adicione a ID de MPN localizada no **perfil de parceiro** da conta que você deseja convidar para mesclar com você. Você deve usar sua ID de MPN global do parceiro. Você não pode usar uma ID de MPN de local.

4. Quando você seleciona **mesclar**, um convite é enviado para a empresa parceira. Ao aceitar sua solicitação, você pode iniciar a mesclagem de conta no Partner Center. Se a empresa rejeitar sua solicitação para mesclar contas, poderá explicar por que ela rejeitou a solicitação. Uma lista de todas as mesclagens de sua conta está disponível para você no **histórico de mesclagem**.
 
### <a name="example-of-two-companies-merging-accounts"></a>Exemplo de duas empresas que mesclam contas

1. A contoso, Ltd. tem 

    a. uma [ID de MPN global de 1111111](https://partner.microsoft.com/pcv/accountsettings/connectedpartnerprofile) e um [local subordinado MPN IDs de 2222222](https://partner.microsoft.com/pcv/accountsettings/locationsprofile).
  
    b. um locatário do Azure AD = @contoso.com
 
    c. uma competência Gold que expira em 1º de outubro de 2020
2. A Fabrikam, Inc. tem
 
    a.  uma ID de MPN global de 3333333 e duas IDs de MPN de local subordinado de 4444444 e 5555555

    b.  um locatário do Azure AD = @fabrikam.com

    c.  duas competências Gold que expiram em 1º de dezembro de 2020
3.  A contoso compra a Fabrikam e vai [aqui](https://partner.microsoft.com/dashboard/account/merger) para iniciar uma solicitação de mesclagem.
4.  A Fabrikam entra no Partner Center e vai para a mesma página que a contoso fez na etapa #3, para aprovar a solicitação da contoso.
5.  A contoso revisa os detalhes da mesclagem na mesma página e fornece confirmação para prosseguir com a fusão de contas.
6.  Após a fusão, a conta da empresa será exibida como:

    a.  Uma empresa chamada contoso com uma ID de MPN global de 1111111 e 4 IDs de MPN de local subordinado de 2222222, 3333333, 4444444 e 5555555
    
    b.  Ele terá dois locatários do Azure AD ( @contoso.com + @fabrikam.com ) que têm acesso à mesma conta do Partner Center
    
    c.  Ele terá dois pacotes de benefícios de competência, um que expira em 1º de outubro de 2020 e outro que expira em 1º de dezembro de 2020. Eles poderão ser renovados como um pacote de benefícios de competência única em 1º de dezembro de 2020. Quando eles forem renovados, a contoso manterá todas as três competências, mesmo que elas possam manter apenas um único pacote de benefícios.
    
7.  Os administradores da Contoso continuarão a gerenciar as funções do Partner Center para @contoso.com os usuários. Os administradores da Fabrikam continuarão a gerenciar as funções do Partner Center para @fabrikam.com os usuários. Os administradores da Contoso só poderão administrar os usuários da Fabrikam se forem convidados como convidados no locatário da Fabrikam.
8.  A Contoso pode decidir ignorar o @fabrikam.com locatário e reemitir as novas credenciais da Fabrikam Employees @contoso.com com novas funções e permissões.

## <a name="next-steps"></a>Próximas etapas

- [Atribuir permissões e funções de usuários](permissions-overview.md)

- [Verifique suas informações de perfil do parceiro](update-your-partner-profile.md)

- [Adicione Serviços Compartilhados com Parceiros do Azure para que os parceiros possam comprar assinaturas do Azure para uso próprio](shared-services.md)
