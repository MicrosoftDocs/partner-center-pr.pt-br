---
title: Mesclar sua conta de parceiro com outra conta de parceiro
description: Saiba como mesclar sua conta de parceiro com outra conta de parceiro no Partner Center – para empresas que são parceiros ativos da Microsoft no Partner Center.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: parthpandyaMSFT
ms.author: parthp
ms.custom: seodec18
ms.date: 06/12/2020
ms.openlocfilehash: bcef4c771d748b0e2fbeae8cf1daaf41d7f53b43
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276630"
---
# <a name="merge-your-partner-account-with-another-partner-account"></a>Mesclar sua conta de parceiro com outra conta de parceiro

**Funções apropriadas:** Administrador da conta

Duas ou mais empresas que são parceiros ativas da Microsoft e têm contas Partner Center podem optar por mesclar suas contas.

## <a name="what-happens-when-two-partners-elect-to-merge-their-partner-center-accounts"></a>O que acontece quando dois parceiros optam por mesclar suas contas Partner Center dados

- A organização parceira que inicia a mesclagem será a PGA (conta global do parceiro).

- O PGA da organização convidada se torna um local da empresa que está iniciando.

- Todos os locais da conta mesclada se tornam locais no PGA.

- Depois que a fusão da conta for concluída, você verá os detalhes da conta, como locais e usuários dentro do perfil PGA. Não é possível reverter esse processo.

- Todas as IDs de MPN para locais são preservadas durante essa consolidação.

- As funções do usuário são trazidos. Por exemplo, se um usuário tivesse sido o administrador de incentivos para um local específico, ele ainda teria essa função após a fusão e seria capaz de ver os incentivos que viu antes da fusão.

- Os locatários do Azure AD e as contas do CSP não são mesclados e não têm nenhum efeito.

- Ofertas publicadas e dados de pipeline de venda co-venda associados a ambas as empresas são preservados

### <a name="view-of-merged-accounts"></a>Exibição de contas mescladas

:::image type="content" source="images/merge-accounts/account-merge.png" alt-text="Fusão de conta.":::

## <a name="what-to-expect-if-you-have-been-invited-to-merge-your-partner-center-account-with-another-partner-center-account"></a>O que esperar se você tiver sido convidado para mesclar sua conta Partner Center com outra conta Partner Center conta

Se você decidir aceitar o convite para mesclar contas: · Suas IDs e locais do MPN serão mesclados no PGA da conta de parceiro que o chamou.

- Seus usuários serão trazidos para a conta mesclada com suas funções intactas.

- Os benefícios e competências existentes serão preservados para ambas as empresas após a fusão até a renovação. Na renovação, as contas serão tratadas como uma empresa e as regras de renovação padrão serão aplicadas.

## <a name="understand-the-impacts-to-programs-and-benefits-when-partners-elect-to-merge-accounts"></a>Entender os impactos em programas e benefícios quando os parceiros optam por mesclar contas

- Todas as competências existentes (Gold/Silver), compras (como Microsoft Action Pack) e benefícios associados são preservados durante a consolidação. Se ambas as empresas têm a mesma competência, mas uma é ouro e a outra prata, a competência com o nível de proficiência mais alto será concedida e os parceiros terão um conjunto de benefícios pratas e um conjunto de benefícios ouro para essa competência até a próxima renovação. 

- A data de aniversário mais alta para o Microsoft Action Pack será mantida após a fusão. Por exemplo, se a data de aniversário da empresa 1 for junho de 2020 para renovação do Action Pack e a data de aniversário da renovação do Action Pack para a empresa 2 for outubro de 2020, a Microsoft usará a data de outubro de 2020 como a nova data de aniversário para a empresa mesclada.

- Durante a fusão da conta e até a próxima renovação, cada conta manterá seus Action Pack e/ou benefícios de competência. Na renovação, as regras de Action Pack padrão e de renovação de competência se aplicam.

- Após a renovação, os benefícios que estão incluídos com a Action Pack de competência são implementados para a conta global de parceiro da empresa parceira:

  - Microsoft Action Pack: a empresa parceira poderá comprar uma conta Action Pack por parceiro global.

  - Competência: a empresa parceira receberá um pacote de principais benefícios, associados à sua maior realização, além de benefícios específicos de competência que o parceiro está qualificado para cada conta global de parceiro.

- Todos os benefícios estão sujeitos ao guia [de uso Microsoft Partner Network benefícios.](https://aka.ms/partner-benefits-use-guide) Por exemplo: um token O365 E3 ativado é funcional por 12 meses após a ativação. Depois que um token tiver sido ativado para licenças em um locatário, essas licenças poderão não ser movidas para outro locatário.

- As associações de ID do MCP para ambas as empresas serão mantidas e associadas à ID do MPN do PGA.

- Os benefícios técnicos e de go-to-market são oferecidos como benefício principal de competência. Após a mesclagem, é recomendável que você verifique suas informações bancárias e fiscais para garantir a precisão.

- Se sua empresa estiver no programa MSP Especialista em Azure, os benefícios serão mantidos até a renovação.

- Se sua empresa tiver obtido especializações avançadas, elas serão mantidas em ambas as contas.

- Todos os comprovantes do software assurance são retidos em ambas as contas. 

- Não há nenhum efeito na associação de DPOR ou PAL. Todas as contribuições de receita associadas começarão a fluir para a nova Conta Global do Parceiro

## <a name="invite-a-company-to-merge-their-partner-center-account-with-your-partner-center-account"></a>Convidar uma empresa para mesclar sua conta Partner Center com sua conta Partner Center conta

>[!Note]
>Para executar a fusão de conta, você deve ser o **Administrador da conta** da sua empresa.

1. Selecione **Configurações** no painel Partner Center aplicativo. 

2. Selecione **Mesclagem de conta**.

3. Adicione a ID do MPN localizada no **perfil de Parceiro** da conta que você deseja convidar para mesclar com você. Você deve usar a ID do MPN global do parceiro. Você não pode usar uma ID do MPN de local.

4. Quando você seleciona **Mesclar**, um convite é enviado para a empresa parceira. Quando eles aceitam sua solicitação, você pode iniciar a mesclagem de conta em Partner Center. Se a empresa rejeitar sua solicitação para mesclar contas, ela poderá explicar por que ela rejeitou a solicitação. Uma lista de todas as mesclagem de sua conta está disponível para você em **Histórico de mesclagem.**
 
### <a name="example-of-two-companies-merging-accounts"></a>Exemplo de duas empresas mesclando contas

1. Contoso, Ltd. tem 

    a. uma [ID de MPN global de 1111111 e](https://partner.microsoft.com/pcv/accountsettings/connectedpartnerprofile) uma IDs de MPN de local subordinado [de 22222222](https://partner.microsoft.com/pcv/accountsettings/locationsprofile).
  
    b. um locatário do Azure AD = @contoso.com
 
    c. uma competência gold que expira em 1º de outubro de 2020
2. A Fabrikam, Inc. tem
 
    a.  uma ID de MPN global de 3333333 e duas IDs de MPN de localização subordinada de 4444444 e 55555555

    b.  um locatário do Azure AD = @fabrikam.com

    c.  duas competências gold que expiram em 1º de dezembro de 2020
3.  A Contoso compra a Fabrikam e vem [aqui para](https://partner.microsoft.com/dashboard/account/merger) iniciar uma solicitação de mesclagem.
4.  A Fabrikam entra Partner Center e vai para a mesma página que a Contoso fez na etapa #3, para aprovar a solicitação da Contoso.
5.  A Contoso revisa os detalhes da mesclagem na mesma página e fornece confirmação para prosseguir com a fusão da conta.
6.  Após a fusão, a conta da empresa será exibida como:

    a.  Uma empresa chamada Contoso com uma ID de MPN global de 1111111 e 4 IDs de MPN de localização subordinada de 22222222, 3333333, 44444444 e 5555555
    
    b.  Ele terá dois locatários do Azure AD ( + ) que @contoso.com têm acesso à mesma conta de @fabrikam.com Partner Center
    
    c.  Ele terá dois pacotes de benefícios de competência, um que expira em 1º de outubro de 2020 e outro que expira em 1º de dezembro de 2020. Eles poderão renovar como um pacote de benefícios de competência único em 1º de dezembro de 2020. Quando eles renovarem, a Contoso manterá todas as três competências, embora possam manter apenas um único pacote de benefícios.
    
7.  Os administradores da Contoso continuarão a gerenciar Partner Center funções para @contoso.com os usuários. Os administradores da Fabrikam continuarão a gerenciar Partner Center funções para @fabrikam.com os usuários do . Os administradores da Contoso só poderão administrar os usuários da Fabrikam se eles são convidados como convidados no locatário da Fabrikam.
8.  A Contoso pode decidir ignorar o locatário e emita as novas credenciais dos funcionários da Fabrikam com novas @fabrikam.com @contoso.com funções e permissões.

## <a name="next-steps"></a>Próximas etapas

- [Atribuir permissões e funções de usuários](permissions-overview.md)

- [Verifique suas informações de perfil do parceiro](update-your-partner-profile.md)

- [Adicione Serviços Compartilhados com Parceiros do Azure para que os parceiros possam comprar assinaturas do Azure para uso próprio](shared-services.md)
