---
title: Mesclar sua conta de parceiro com outra conta de parceiro
description: Saiba como mesclar sua conta de parceiro com outra conta de parceiro no Partner Center-para empresas que estão ativas parceiros da Microsoft no Partner Center.
ms.topic: article
author: parthpandyaMSFT
ms.author: parthp
ms.custom: seodec18
ms.date: 06/12/2020
ms.openlocfilehash: 47827b6aa3bb9853355a6e2fa4f8816e1dd701a1
ms.sourcegitcommit: 7f595faf952bf2d6cdc229da38bd67ee701b2083
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2020
ms.locfileid: "93189740"
---
# <a name="merge-your-partner-account-with-another-partner-account"></a>Mesclar sua conta de parceiro com outra conta de parceiro

**Funções aplicáveis**

- Administrador de conta

Duas ou mais empresas que estão ativas parceiros da Microsoft e que têm contas no Partner Center podem optar por mesclar suas contas.

## <a name="what-happens-when-two-partners-elect-to-merge-their-partner-center-accounts"></a>O que acontece quando dois parceiros optam por mesclar suas contas do Partner Center

- A organização parceira que inicia a mesclagem será a conta global do parceiro (PGA).

- O PGA da organização convidada se torna um local da empresa inicial.

- Todos os locais da conta de mesclagem se tornam locais sob o PGA.

- Depois que a fusão de contas for concluída, você verá os detalhes da conta, como locais e usuários no perfil do PGA. Não é possível reverter esse processo.

- Todas as IDs de MPN para locais são preservadas durante essa consolidação.

- As funções do usuário são trazidas. Por exemplo, se um usuário tivesse sido o administrador de incentivos para um local específico, ele ainda teria essa função após a fusão e poderá ver os incentivos vistos antes da fusão.

- Os locatários e as contas do CSP do Azure AD não são mesclados e não têm impacto.

- As ofertas publicadas e os dados de pipeline de venda conjunta associados a ambas as empresas são preservados

### <a name="view-of-merged-accounts"></a>Exibição de contas mescladas

:::image type="content" source="images/merge-accounts/account-merge.png" alt-text="Fusão de contas":::

## <a name="what-to-expect-if-you-have-been-invited-to-merge-your-partner-center-account-with-another-partner-center-account"></a>O que esperar se você tiver sido convidado para mesclar sua conta do Partner Center com outra conta do Partner Center

Se você decidir aceitar o convite para mesclar contas: · Suas IDs e locais de MPN serão mescladas no PGA da conta de parceiro que o convidou.

- Os usuários serão trazidos para a conta mesclada com suas funções intactas.

- Os benefícios e as competências existentes serão preservadas para ambas as empresas após a refusão até a renovação. Na renovação, as contas serão tratadas como uma empresa e as regras de renovação padrão serão aplicadas.

## <a name="understand-the-impacts-to-programs-and-benefits-when-partners-elect-to-merge-accounts"></a>Entenda os impactos nos programas e nos benefícios quando os parceiros optam por mesclar contas

- Todas as competências existentes (Gold/prata), compras (como o Microsoft Action Pack) e benefícios associados são preservadas durante a consolidação. Se ambas as empresas têm a mesma competência, mas uma é ouro e outra prata, a competência com mais alto nível de proficiência será concedida e os parceiros terão um conjunto de benefícios prata e um conjunto de benefícios dourados para essa competência até a próxima renovação. 

- A data de aniversário mais alta para o Microsoft Action Pack será mantida após a fusão. Por exemplo, se a data de aniversário da empresa 1 for de junho de 2020 para renovação de Action Pack e a data de aniversário para Action Pack renovação para a empresa 2 for de outubro de 2020, a Microsoft usará a data de outubro de 2020 como a nova data de aniversário da empresa mesclada.

- Durante a fusão de contas e até sua próxima renovação, cada conta reterá seus benefícios de Action Pack e/ou competência. Nas regras de renovação, Action Pack padrão e renovação de competência se aplicam.

- Após a renovação, os benefícios incluídos com a obtenção de competência e Action Pack são implementados para a conta global do parceiro da empresa parceira:

  - Microsoft Action Pack: a empresa parceira poderá comprar uma Action Pack por conta global de parceiro.

  - Competência: a empresa parceira receberá um pacote de principais benefícios, associado à sua maior realização, além de benefícios específicos da competência que o parceiro está qualificado para cada conta global do parceiro.

- Todos os benefícios estão sujeitos ao [Guia de uso de Microsoft Partner Network benefícios](https://aka.ms/partner-benefits-use-guide). Por exemplo: um token do O365 E3 ativado é funcional por doze (12) meses após a ativação. Depois que um token tiver sido ativado para licenças em um locatário, essas licenças não poderão ser movidas para outro locatário.

- As associações de ID do MCP para ambas as empresas serão retidas e associadas à ID do PGA MPN.

- As vantagens para o mercado e os benefícios técnicos são oferecidas como um benefício principal de competência. Após a mesclagem, é recomendável que você verifique suas informações bancárias e fiscais para garantir a exatidão.

- Se sua empresa estiver no programa MSP do especialista do Azure, os benefícios serão mantidos até a renovação.

- Se a sua empresa ganhou especializações avançadas, elas são mantidas em ambas as contas são mantidas.

- Os comprovantes do Software Assurance são mantidos em ambas as contas. 

## <a name="invite-a-company-to-merge-their-partner-center-account-with-your-partner-center-account"></a>Convide uma empresa para mesclar sua conta do Partner Center com sua conta do Partner Center

>[!Note]
>Para executar a fusão de contas, você deve ser o **administrador da conta** da sua empresa.

1. Selecione **configurações** no painel do Partner Center. 

2. Selecione **mesclagem de conta** .

3. Adicione a ID de MPN localizada no **perfil de parceiro** da conta que você deseja convidar para mesclar com você. Você deve usar sua ID de MPN global do parceiro. Você não pode usar uma ID de MPN de local.

4. Quando você seleciona **mesclar** , um convite é enviado para a empresa parceira. Ao aceitar sua solicitação, você pode iniciar a mesclagem de conta no Partner Center. Se a empresa rejeitar sua solicitação para mesclar contas, poderá explicar por que ela rejeitou a solicitação. Uma lista de todas as mesclagens de sua conta está disponível para você no **histórico de mesclagem** .
 
### <a name="example-of-two-companies-merging-accounts"></a>Exemplo de duas empresas que mesclam contas

1. A contoso tem 

    a. uma [ID de MPN global de 1111111](https://partner.microsoft.com/pcv/accountsettings/connectedpartnerprofile) e um [local subordinado MPN IDs de 2222222](https://partner.microsoft.com/pcv/accountsettings/locationsprofile).
  
    b. um locatário do Azure AD = @contoso.com
 
    c. uma competência Gold que expira em 1º de outubro de 2020
2. Fabricam tem
 
    a.  uma ID de MPN global de 3333333 e duas IDs de MPN de local subordinado de 4444444 e 5555555

    b.  um locatário do Azure AD = @fabricam.com

    c.  duas competências Gold que expiram em 1º de dezembro de 2020
3.  A contoso compra fabricam e vai [aqui](https://partner.microsoft.com/dashboard/account/merger) para iniciar uma solicitação de mesclagem.
4.  Fabricam entra no Partner Center e vai para a mesma página que a contoso fez na etapa #3, para aprovar a solicitação da contoso.
5.  A contoso revisa os detalhes da mesclagem na mesma página e fornece confirmação para prosseguir com a fusão de contas.
6.  Após a fusão, a conta da empresa será exibida como:

    a.  Uma empresa chamada contoso com uma ID de MPN global de 1111111 e 4 IDs de MPN de local subordinado de 2222222, 3333333, 4444444 e 5555555
    
    b.  Ele terá dois locatários do Azure AD ( @contoso.com + @fabricam.com ) que têm acesso à mesma conta do Partner Center
    
    c.  Ele terá dois pacotes de benefícios de competência, um que expira em 1º de outubro de 2020 e outro que expira em 1º de dezembro de 2020. Eles poderão ser renovados como um pacote de benefícios de competência única em 1º de dezembro de 2020. Quando eles forem renovados, a contoso manterá todas as três competências, mesmo que elas possam manter apenas um único pacote de benefícios.
    
7.  Os administradores da Contoso continuarão a gerenciar as funções do Partner Center para @contoso.com os usuários. Os administradores do fabricam continuarão a gerenciar as funções do Partner Center para @fabricam.com os usuários. Os administradores da Contoso só poderão administrar os usuários do fabricam se forem convidados como convidados no locatário do fabricam.
8.  A Contoso pode decidir ignorar o @fabricam.com locatário e reemitir as novas credenciais dos funcionários fabricam @contoso.com com novas funções e permissões.

## <a name="next-steps"></a>Próximas etapas

- [Atribuir permissões e funções de usuários](permissions-overview.md)

- [Verifique suas informações de perfil do parceiro](update-your-partner-profile.md)

- [Adicionar serviços compartilhados de parceiros do Azure para que os parceiros possam comprar assinaturas do Azure para seu próprio uso](shared-services.md)
