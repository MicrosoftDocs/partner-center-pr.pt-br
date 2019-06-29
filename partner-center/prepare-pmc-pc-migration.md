---
title: Preparar para migrar de Partner Membership Center Partner Center | Partner Center
ms.topic: article
ms.date: 06/13/2019
description: Coisas a considerar antes de mudar o seu negócio de PMC Partner Center
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 0f1df50c5fa94707ac733a91b0d981b6821de8c0
ms.sourcegitcommit: 7b3847a788365a05628a4cf2938dfd61782d6e4e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2019
ms.locfileid: "67468021"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a>Preparar para a movimentação do Centro de associação de parceiro (PMC) Partner Center

Vamos mudar o gerenciamento de participação do Centro de associação de parceiro (PMC) para o destino único para gerenciar sua relação de negócios com a Microsoft partner center –. Queremos sua migração para o Centro de parceiros para ser o mais eficiente e fácil possível. Nós identificamos algumas áreas onde o Partner Center é diferente do PMC, e acreditamos que você desejará entender e prepará-los antes de fazer a mudança.

## <a name="account-and-identity-setup"></a>Configuração de conta e identidade

**O que é uma conta de trabalho do Azure Active Directory (Azure AD)?**

Uma conta corporativa do Azure é uma representação virtual dedicada e isolada da sua empresa na nuvem pública do Azure, criada quando você assina um serviço em nuvem da Microsoft, como o Azure, o Microsoft Intune ou o Office 365.

Sua conta de trabalho hospeda seus usuários do AD do Azure e as informações sobre eles - suas email, senhas, dados de perfil, permissões e assim por diante. A conta de trabalho também contém grupos, aplicativos e outras informações referentes a uma empresa e sua segurança. Para obter mais informações, consulte...

O Partner Center, você usará seu email de trabalho para entrar na sua conta não seu email pessoal.
- Sua conta de trabalho: john@contoso.com
- Sua conta pessoal: John@outlook.com

Seu email de trabalho faz parte do seu locatário do Azure active directory. Para ter uma conta no Partner Center, você precisa ter um locatário do AAD. Para obter mais informações sobre o Active Directory do Azure, leia [criar seu diretório no Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad).

**Quando você move para o Centro de parceiros de PMC, qual conta deve entrar no Centro de parceiros com se você tiver um locatário do AAD com a Microsoft (para Office 365, por exemplo) e você também tem um locatário para seu negócio CSP?**

Você pode entrar no Centro de parceiros com a conta do CSP ou sua conta de email de trabalho do MPN. Se você optar por entrar usando seu email de trabalho do CSP, no painel de navegação esquerdo exibirá informações sobre o programa MPN e o CSP. Se você entrar com seu email de trabalho de locatário do AD do Azure do MPN, você verá apenas suas informações de programa da MPN. Funções de usuário são diferentes entre a MPN e o CSP então, se você usar a mesma conta para empresas do MPN e o CSP, certifique-se você atribuir funções de usuário adequadamente. Para obter informações sobre funções de usuário, leia [atribuir permissões e funções de usuário](permissions-overview.md).

**Qual é a diferença entre a função de administrador global do AAD e a função de administrador global do PMC MPN?**

Essas são duas funções completamente diferentes com permissões diferentes. O administrador global do locatário AAD no Partner Center administra o locatário – adiciona ou remove usuários, fornece e gerencia as senhas, funções e permissões e tem acesso a programas de todas as suas empresas no Partner Center. 

A função de administrador global do MPN no PMC poderia fazer o seguinte:

- Exibir e editar todos os dados associados com a empresa e todos os locais da empresa

-  Adicione administradores a nível global ou local.  Além disso, os administradores globais podem atribuir qualquer pessoa em qualquer local de acesso de Administrador Global que concede a eles acesso global, independentemente de qual local estão associados.
-  Execute qualquer parceiro voltado para a função de interface do usuário incluindo: 

-  Adicionar/remover usuários

 - Atribuir ou remover funções 

 - Adicionar/remover/atualizar locais 

 - Competência de compra/mapas 

-  Exibir os benefícios

Quando o administrador global do MPN é movida para o Centro de parceiros a função é chamada do administrador de parceiro da MPN que tenha permissões diferentes e tarefas do que o administrador global do Partner Center. Para obter mais informações sobre funções e permissões no Partner Center, leia [atribuir funções de usuários e permissões](permissions-overview.md)

**Funções de usuário, incluindo funções de usuário convidado no Partner Center**

Partner Center tem tipos diferentes de funções de acordo com os tipos de trabalho precisa ser feito. Há funções como administrador global que são funções do Azure AD. Algumas funções são específica para programas como o programa de provedor de serviços de nuvem ou incentivos e há funções que são específicas para MPN. Para descobrir quais são todas as funções do Partner Center, leia [atribuir funções de usuários e permissões](permissions-overview.md).



**O que acontece com as funções de meus usuários quando eles são movidos do PMC Partner Center?**

Exceto o administrador global do MPN ou o contato de programa principal que realiza a migração, todos os usuários no PMC perderão suas funções de administrador. A pessoa que conclui a migração será necessário atribuir funções no Partner Center. As funções no Partner Center diferem no PMC. Leia [atribuir funções de usuários e permissões](permissions-overview) e [movendo do PMC Partner Center](https://docs.microsoft.com/en-us/partner-center/move-pmc-pc-map#user-roles) para obter mais sobre funções de usuário no Partner Center.


**O que é a diferença entre meu perfil da empresa e meu perfil de negócios?**

O perfil da empresa é as informações sobre sua empresa que inclui o endereço, locais, o contato principal, detalhes do banco e imposto.

Seu perfil de negócios é perante aos clientes e uma página de marketing que exibe seu logotipo, detalhes sobre seu negócios a se concentrar, sua experiência, etc.

**O que leva em conta média de consolidação para minha conta?**

Se você usar o mesmo locatário do AD do Azure para migrar várias contas do MPN no Partner Center, o sistema automaticamente reconhecerá que e pedir que você consolide suas contas. Isso é verdadeiro mesmo se você tiver vários domínios associados ao mesmo locatário do Azure AD. 

Você pode decidir migrar para o Centro de parceiros usando locatários separados do AAD, mas observe que isso resulta em avaliação isolada das suas competências e extra de custos de aquisição. 

**Se eu tiver vários locatários do AAD e uma única conta do MPN, é possível vinculá-los no Partner Center?**

Sim, no Partner Center, você pode vincular vários locatários do AD do Azure a única conta no Partner Center.
Saiba mais aqui. 

**Há restrições à adição de vários locatários do AD do Azure para uma única conta do Partner Center?**

Se o locatário do AD do Azure já está associado a uma conta existente do Partner Center, ele não pode ser associado a novas contas do Partner Center usando o recurso de multilocação. Outra maneira de pensar que ele é um locatário do AD do Azure só pode ser associado a uma conta no Partner Center, mas uma conta no Partner Center pode ter vários locatários associados a ele.

## <a name="microsoft-partner-network-mpn-membership-migration"></a>Migração de associação do Microsoft Partner Network (MPN) 

**Quem pode executar a movimentação do PMC Partner Center?**

O administrador global do MPN de empresa ou o contato principal do programa (essas duas funções normalmente são mantidas pela mesma pessoa) pode iniciar e realizar a movimentação.

**A pessoa que concluir a migração se tornará o contato principal no perfil legal da empresa no Partner Center?**

Não necessariamente, no entanto, o contato principal precisará ser alguém que tenha autorização para assinar os contratos.

**Microsoft pode migrar minha associação do MPN para mim?**

Não. Microsoft não pode ajudá-lo a mover sua conta de associação para o Centro de parceiros. Você precisará mover sua conta, entrando no PMC com sua conta corporativa (credenciais de entrada) iniciar o processo de migração. Depois de concluir as etapas para mover sua conta, você pode começar a gerenciar sua associação e atribuir funções de usuário e permissões para a sua equipe para que possam acessar os benefícios e ajudar a gerenciar a associação. Microsoft migrará automaticamente as competências atuais, benefícios, informações de localização, informações bancárias/imposto para incentivos e associações de MCP, incluindo o acesso da Universidade do parceiro.

Microsoft migrará automaticamente as competências atuais, benefícios, informações de localização, informações bancárias/imposto para incentivos e associações de MCP, incluindo o acesso da Universidade do parceiro.

**Como a política de renovação mudará?**

 No Partner Center, a janela de renovação é de sua data de aniversário por meio dos 30 dias a seguir.

**Nosso competências permanecerá inalteradas depois passamos para o Partner Center?**

Sim, competências não serão afetadas pela mudança Partner Center. Se você observar as discrepâncias, entre em contato com [suporte](https://partner.microsoft.com/support).


 **Meus benefícios (incluindo os benefícios da nuvem, suporte técnico, benefícios do software, Visual Studio) serão alterados após passarmos?**

 Seus benefícios qualificados não serão alterado. Se você observar as discrepâncias, entre em contato com [suporte](https://partner.microsoft.com/support).

 **Nossas contas da Microsoft que tenham as alocações de benefícios do Visual Studio ser cumpridas?**


 Sim. Benefícios do Studio Visual alocados para as MSAs serão respeitados e mantidos. Eles também serão preservados após a renovação no Partner Center. No entanto, se você remover uma alocação de MSA uma vez migradas no Partner Center, ele não pode ser adicionado novamente ao Partner Center.

No Partner Center, um parceiro pode adicionar contas de trabalho e contas de usuários convidados que são MSA do mesmo locatário em que o parceiro é MPN administrador no locatário do AD do Azure. Se o parceiro seja um administrador global em vários locatários do AD do Azure e todos esses locatários estão associados à mesma conta do Partner Center, o parceiro é permitido para adicionar usuários em todos os locatários esses para os benefícios do Visual Studio e alocações de baseada no uso do Azure.

Embora podem ser atribuídos a usuários convidados com base no uso de assinaturas do Visual Studio pelo administrador global ou administrador do MPN, os usuários convidados não podem entrar Partner Center usando sua MSA. Usuários convidados podem, no entanto, entrar no Azure e o Visual Studio para validar e usar os benefícios de atribuído.


 **Como podemos gerenciar nossos associações MCP e nosso acesso Universidade do parceiro?**

 Não há nenhuma alteração para as associações de MCP mover do PMC. No entanto, qualquer novo novos funcionários depois de mover para o Partner Center precisará ser associado no Partner Center. Todas as suas permissões de Universidade do parceiro para os usuários existentes permanecerão mas quaisquer novos funcionários devem ir para [o Centro de treinamento](https://partner.microsoft.com/training) para obter informações sobre como obter acesso a Universidade do parceiro.

 **Referências do cliente são usadas no Partner Center?**

 Não, você não precisa referências do cliente para atender aos requisitos de competência no Partner Center.

 **Associações do parceiro de registro serão movido para o Partner Center?**

 Sim, não há nenhuma alteração ao parceiro de registro. Saiba mais sobre [vincular sua ID de parceiro a seus clientes](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started).

**Há um impacto sobre incentivos por causa a mudança para o Partner Center?**

Não há nenhum impacto sobre incentivos se você tiver movido a sua conta sem consolidar locais. Se sua empresa tiver várias contas no PMC e, quando você move Partner Center decidir consolidar em uma conta global, não haverá nenhuma perda de incentivos, mas pode haver um atraso de pagamento de incentivo. Se você não mover todas as suas contas do PMC tem sido envolvidas em programas de incentivos, você pode parar a obtenção de incentivos que estão vinculados a essas contas.


**Quais são as funções de usuário incentivos no Partner Center?** 

Funções incentivos no Partner Center são baseados na localização e incluem incentivos administrador e usuário incentivos. Para obter mais informações sobre o que podem fazer essas funções, consulte [atribuir funções de usuários e permissões](permissions-overview.md).

**Os usuários de incentivos podem ser atribuídos no nível global e local?**

 Sim. Você pode atribuir um administrador incentivos para ser o administrador incentivos para todos os locais ou cada local pode ter seu próprio administrador de incentivos.

 **Incentivos podem ser pagos no nível global ou local?**

 Incentivos são pagos somente no nível do local.

**Sobre as referências, quantos perfis de negócios podemos criar?**

Sua empresa pode criar vários perfis de negócios, como a necessidade de representam totalmente os interesses da sua empresa. Em cada perfil de negócios, você pode listar até cinco locais, um único local por país. Cada um dos perfis de negócios pode receber referências para cada um dos seus locais.

**Como serão as referências atribuídos, as alterações que posso esperar? Por exemplo, se eu tiver uma empresa global em um mercado e locais em outros mercados, como as referências receberá?**

As referências são atribuídas com base em parâmetros de pesquisa que define o cliente. Então, independentemente de você ter um único local ou em várias, se os clientes Especifica um local desejado e você tiver um negócio lá que atenda aos outros parâmetros, e em seguida, a referência deve ir para o local.








