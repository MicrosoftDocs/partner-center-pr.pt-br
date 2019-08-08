---
title: Prepare-se para sua mudança do Partner Membership Center para o Partner Center | Centro de parceiros
ms.topic: article
ms.date: 06/13/2019
description: O que pensar antes de mover seus negócios do PMC para o Partner Center
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: d6db2dcb5ac53e29d907c09ca2b16d123b21c07f
ms.sourcegitcommit: bae29ab191c72e15259d99c40c69a9e7c3f2b502
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/06/2019
ms.locfileid: "68820575"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a>Prepare-se para a migração do Partner Membership Center (PMC) para o Partner Center

Estamos movendo o gerenciamento de associação do Partner Membership Center (PMC) para o Partner Center – o único destino para gerenciar seu relacionamento de negócios com a Microsoft. Queremos que sua mudança para o Partner Center seja a mais eficiente e fácil possível. Identificamos algumas áreas em que o Partner Center difere da PMC e achamos que você desejará entender e se preparar para elas antes de fazer a movimentação.

## <a name="account-and-identity-setup"></a>Configuração de conta e identidade

**O que é uma conta de trabalho do Azure Active Directory (AD do Azure)?**

Uma conta corporativa do Azure é uma representação virtual dedicada e isolada da sua empresa na nuvem pública do Azure, criada quando você assina um serviço em nuvem da Microsoft, como o Azure, o Microsoft Intune ou o Office 365.

Sua conta de trabalho hospeda seus usuários do Azure AD e as informações sobre eles-seus emails, senhas, dados de perfil, permissões e assim por diante. A conta corporativa também contém grupos, aplicativos e outras informações pertencentes a uma empresa e sua segurança. Para obter mais informações, consulte...

No Partner Center, você usará seu email de trabalho para entrar em sua conta, não seu email pessoal.
- Sua conta corporativa:john@contoso.com
- Sua conta pessoal:John@outlook.com

Seu email de trabalho faz parte do seu locatário do Azure Active Directory. Para ter uma conta no Partner Center, você precisa ter um locatário do AAD. Para obter mais informações sobre Azure Active Directory, leia [criar seu diretório no Azure ad](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad).

**Quando você passa para o Partner Center da PMC, qual conta você deve entrar no Partner Center com se você tiver um locatário do AAD com a Microsoft (para o Office 365, por exemplo) e também tiver um locatário para seu negócio CSP?**

Você pode entrar no Partner Center com a conta do CSP ou sua conta de email do MPN work. Se você optar por entrar usando seu email de trabalho do CSP, a navegação à esquerda no painel exibirá as informações do programa MPN e do CSP. Se você entrar com seu email de locatário do Azure AD MPN, verá apenas as informações do programa MPN. As funções de usuário diferem entre MPN e CSP, portanto, se você usar a mesma conta para os negócios do MPN e do CSP, certifique-se de atribuir funções de usuário de forma adequada. Para obter informações sobre funções de usuário, leia [atribuir funções de usuário e permissões](permissions-overview.md).

**Qual é a diferença entre a função de administrador global do AAD e a função de administrador global do PMC MPN?**

Essas são duas funções completamente diferentes com permissões diferentes. O administrador global do locatário do AAD no Partner Center administra o locatário – adiciona ou remove usuários, fornece e gerencia senhas, funções e permissões e tem acesso a todos os programas da empresa no Partner Center. 

A função de administrador global MPN no PMC pode fazer o seguinte:

- Exibir e editar todos os dados associados à empresa e a todos os locais da empresa

-  Adicione administradores no nível global ou local.  Além disso, os administradores globais podem atribuir qualquer pessoa em qualquer local acesso de administrador global que concede a eles acesso global, independentemente de qual local eles estão associados.
-  Execute qualquer função de interface do usuário voltada para o parceiro, incluindo: 

-  Adicionar/remover usuários

 - Atribuir/remover funções 

 - Adicionar/remover/atualizar locais 

 - Competência/mapas de compra 

-  Exibir benefícios

Quando o administrador global do MPN passa para o Partner Center, a função é chamada de administrador do parceiro MPN que tem permissões e tarefas diferentes do administrador global do Partner Center. Para obter mais informações sobre funções e permissões no Partner Center, leia [atribuir funções e permissões de usuários](permissions-overview.md).

**Funções de usuário, incluindo funções de usuário convidado no Partner Center**

O Partner Center tem diferentes tipos de funções, dependendo dos tipos de trabalho necessários para a realização. Há funções como administrador global que são funções do Azure AD. Algumas das funções são específicas para programas como o programa do provedor de serviços de nuvem ou incentivos, e há funções específicas para MPN. Para descobrir quais são todas as funções do Partner Center, leia [atribuir funções e permissões de usuários](permissions-overview.md).



**O que acontece com as funções dos meus usuários quando elas se movem do PMC para o Partner Center?**

Exceto para o administrador global do MPN ou o contato do programa principal que realiza a migração, todos os usuários no PMC perderão suas funções de administrador. O indivíduo que conclui a migração precisará atribuir funções no Partner Center. As funções no Partner Center diferem das do PMC. Leia [atribuir funções e permissões de usuários] (permissões-overview.md e [migrando do PMC para o Partner Center](https://docs.microsoft.com/partner-center/move-pmc-pc-map#user-roles) para obter mais informações sobre as funções de usuário no Partner Center.


**Qual é a diferença entre meu perfil de empresa e meu perfil comercial?**

Seu perfil de empresa é a informação sobre sua empresa que inclui endereço, locais, contato primário, banco e detalhes de impostos.

Seu perfil comercial é como você se apresenta aos clientes e é uma página de marketing que exibe seu logotipo, detalhes sobre seu foco comercial, sua experiência etc.

**O que significa consolidação de conta para minha conta?**

Se você usar o mesmo locatário do Azure AD para migrar várias contas do MPN para o Partner Center, o sistema o reconhecerá automaticamente e solicitará que você consolide suas contas. Isso é verdadeiro mesmo se você tiver vários domínios associados ao mesmo locatário do Azure AD. 

Você ainda pode decidir migrar para o Partner Center usando locatários separados do AAD, mas observe que isso resulta em uma avaliação isolada de suas competências e custos de compra extras. 

**Se eu tiver vários locatários do AAD e uma única conta do MPN, será possível vinculá-los no Partner Center?**

Sim, no Partner Center, você pode vincular vários locatários do Azure AD à conta do centro de parceiros único.
Saiba mais aqui. 

**Há restrições para adicionar vários locatários do Azure AD a uma única conta do Partner Center?**

Se o locatário do Azure AD já estiver associado a uma conta existente do Partner Center, ele não poderá ser associado a novas contas do Partner Center usando o recurso multilocação. Outra maneira de considerar isso é que um locatário do Azure AD só pode ser associado a uma conta do Partner Center, mas uma conta do Partner Center pode ter vários locatários associados a ele.

## <a name="microsoft-partner-network-mpn-membership-migration"></a>Migração de associação de Microsoft Partner Network (MPN) 

**Quem pode realizar a mudança de PMC para o Partner Center?**

O administrador global da empresa MPN ou o contato do programa principal (essas duas funções geralmente são mantidos pela mesma pessoa) pode iniciar e executar a movimentação.

**A pessoa que estiver concluindo a migração se tornará o contato principal do perfil legal da empresa no Partner Center?**

No entanto, não necessariamente, o contato principal precisa ser alguém que tenha autorização para assinar contratos.

**A Microsoft pode migrar minha associação do MPN para mim?**

Não. A Microsoft não pode ajudá-lo a mover sua conta de associação para o Partner Center. Você precisará mover sua conta entrando no PMC com sua conta corporativa (credenciais de entrada) para iniciar o processo de migração. Depois de concluir as etapas para mover sua conta, você pode começar a gerenciar sua associação e atribuir funções e permissões de usuário à sua equipe para que eles possam acessar os benefícios e ajudar a gerenciar a associação. A Microsoft migrará automaticamente as competências, os benefícios, as informações de local, as informações bancárias/de impostos para incentivos e as associações do MCP, incluindo o acesso do Partner University.

A Microsoft migrará automaticamente as competências, os benefícios, as informações de local, as informações bancárias/de impostos para incentivos e as associações do MCP, incluindo o acesso do Partner University.

**Como a política de renovação será alterada?**

 No Partner Center, a janela de renovação é de sua data de aniversário nos 30 dias seguintes.

**Nossas competências permanecerão inalteradas depois de mudarmos para o Partner Center?**

Sim, o compentencies não será afetado pela mudança para o Partner Center. Se você perceber discrepâncias, contate o [suporte](https://partner.microsoft.com/support).


 **Meus benefícios (incluindo benefícios na nuvem, suporte técnico, benefícios de software, Visual Studio) mudam depois de mudarmos?**

 Seus benefícios qualificados não serão alterados. Se você perceber discrepâncias, contate o [suporte](https://partner.microsoft.com/support).

 **As nossas contas da Microsoft que têm as alocações de benefícios do Visual Studio serão respeitadas?**


 Sim. Os benefícios do Visual Studio alocados para o MSAs serão respeitados e mantidos. Eles também serão preservados após a renovação no Partner Center. No entanto, se você remover uma alocação de MSA uma vez migrada no Partner Center, ela não poderá ser adicionada novamente ao Partner Center.

No Partner Center, um parceiro pode adicionar contas de trabalho e contas de usuário convidado que são MSA do mesmo locatário em que o parceiro é MPN admin no locatário do Azure AD. Se o parceiro for um administrador global em vários locatários do Azure AD e todos esses locatários estiverem associados à mesma conta do Partner Center, o parceiro poderá adicionar usuários em todos esses locatários aos benefícios do Visual Studio e às alocações baseadas no uso do Azure.

Embora os usuários convidados possam receber assinaturas baseadas em uso do Visual Studio pelo administrador do MPN ou pelo administrador global, os usuários convidados não podem entrar no Partner Center usando o MSA. No entanto, os usuários convidados podem entrar no Azure e no Visual Studio para validar e usar seus benefícios atribuídos.


 **Como devemos gerenciar nossas associações do MCP e nosso acesso do Partner University?**

 Não há alterações nas associações do MCP que se movem do PMC. No entanto, novos novos funcionários após a mudança para o Partner Center precisarão ser associados no Partner Center. Todas as permissões da Universidade de parceiros para usuários existentes permanecerão, mas os novos funcionários deverão ir para [o centro de treinamento](https://partner.microsoft.com/training) para obter informações sobre como obter acesso ao Partner University.

 **Como fazer exibir informações do MCP quando eu mudar para o Partner Center?**

Selecione **competências** na barra de navegação à esquerda no painel. Na página **competências** , você pode baixar o relatório de habilidades. O relatório de habilidades listará seus usuários que adquiriram habilidades relevantes para as competências e os programas no Partner Center. Se os usuários obtiverem habilidades, mas essas habilidades não forem relevantes para as competências nas quais você está trabalhando, elas não serão listadas no relatório.


 **As referências do cliente são usadas no Partner Center?**

 Não, você não precisa de referências de clientes para atender aos requisitos de competência no Partner Center.

 **O parceiro de associações de registro será movido para o Partner Center?**

 Sim, não há nenhuma alteração no parceiro do registro. Saiba mais sobre como [vincular sua ID de parceiro aos seus clientes](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started).

**Há um impacto nos incentivos devido à mudança para o Partner Center?**

Não, não haverá impacto em incentivos se você tiver movido sua conta sem consolidar locais. Se sua empresa tiver várias contas na PMC e, quando você mudar para o Partner Center, você decide consolidar em uma conta global, não haverá perda para os incentivos, mas pode haver um atraso no pagamento de incentivos. Se você não mover todas as suas contas do PMC envolvidas em aplicativos de incentivos, poderá parar de ganhar incentivos vinculados a essas contas.


**Quais são as funções de usuário de incentivos no Partner Center?** 

As funções de incentivos no Partner Center são baseadas no local e incluem incentivos de administrador e incentivos. Para obter mais informações sobre o que essas funções podem fazer, consulte [atribuir funções e permissões de usuários](permissions-overview.md).

**Os incentivos podem ser atribuídos aos usuários no nível global e local?**

 Sim. Você pode atribuir um administrador de incentivos para ser o administrador de incentivos para todos os locais ou cada local pode ter seu próprio administrador de incentivos.

 **Os incentivos podem ser pagos no nível global ou de local?**

 Os incentivos são pagos apenas no nível do local.

**Sobre referências, quantos perfis de negócios podemos criar?**

Sua empresa pode criar quantos perfis de negócios forem necessários para representar totalmente os interesses da sua empresa. Em cada perfil comercial, você pode listar até cinco locais, um local por país. Cada um dos perfis de negócios pode receber referências para cada um de seus locais.

**Como as referências serão atribuídas, quais alterações posso esperar? Por exemplo, se eu tiver uma empresa global em um mercado e locais em outros mercados, como as referências serão atribuídas?**

As referências são atribuídas com base nos parâmetros de pesquisa definidos pelo cliente. Portanto, independentemente de você ter um local ou muitos, se os clientes especificarem um local desejado e você tiver uma empresa que atenda aos outros parâmetros, a referência irá para esse local.








