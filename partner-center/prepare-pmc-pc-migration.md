---
title: Migrando do Partner Membership Center
ms.topic: article
ms.date: 06/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Examine informações úteis e perguntas frequentes antes de migrar o seu negócio do Partner Membership Center para o Partner Center.
author: parthpandyamsft
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 12b5b94194c6ca65b31af08dbf0dafef5c6ef21c
ms.sourcegitcommit: 5f31146f50e01dc4c1922e0a5bc369f0a3cd8162
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/01/2020
ms.locfileid: "89220384"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a>Preparar a migração do PMC (Partner Membership Center) para o Partner Center

**Funções apropriadas**
- Administrador global
- Administrador de usuários
- Agente de vendas
- Agente administrativo

Estamos migrando o gerenciamento de associação do PMC (Partner Membership Center) para o Partner Center, o único local para gerenciar seu relacionamento comercial com a Microsoft. Queremos que a sua migração para o Partner Center seja a mais eficiente e fácil possível. Identificamos algumas áreas em que o Partner Center é distinto do PMC e acreditamos ser útil entendê-las e se preparar para elas antes que você faça a migração.

## <a name="account-and-identity-setup"></a>Configuração de conta e identidade

Confira abaixo as respostas a perguntas comuns sobre a configuração de conta e de identidade.

### <a name="what-is-an-azure-active-directory-azure-ad-work-account"></a>O que é uma conta corporativa do Azure AD (Azure Active Directory)?

Uma conta corporativa do Azure é uma representação virtual dedicada e isolada da sua empresa na nuvem pública do Azure, criada quando você assina um serviço de nuvem da Microsoft, como o Azure, o Microsoft Intune ou o Office 365.

Sua conta corporativa hospeda os usuários do Azure AD e as informações sobre eles: emails, senhas, dados de perfil, permissões etc. A conta corporativa também contém grupos, aplicativos e outras informações pertencentes a uma empresa e à segurança dela. 

Seu email de trabalho faz parte do seu locatário do Azure Active Directory. Para ter uma conta no Partner Center, você precisará ter um locatário do AAD. Para obter mais informações sobre o Azure Active Directory, leia [Criar seu diretório no Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad).

No Partner Center, você usará seu email de trabalho para entrar na conta, não seu email pessoal.

- Sua conta corporativa: john@contoso.com
- Sua conta pessoal: John@outlook.com

### <a name="what-account-should-you-sign-into-partner-center-with-if-you-have-an-aad-tenant-with-microsoft-for-office-365-for-example-and-you-also-have-a-tenant-for-your-csp-business"></a>Com qual conta você deverá entrar no Partner Center se tiver um locatário do AAD com a Microsoft (para o Office 365, por exemplo) e também tiver um locatário para o seu negócio do CSP?

Você pode entrar no Partner Center com a conta do CSP ou a conta de email de trabalho do MPN. Se você optar por se conectar usando seu email de trabalho do CSP, a navegação à esquerda no painel exibirá informações dos programas MPN e CSP. Se você se conectar com o seu email de trabalho do locatário do Azure AD no MPN, verá apenas as informações do programa MPN. 

### <a name="if-you-dont-want-to-use-your-existing-office-365-azure-ad-tenant-for-partner-center-you-can-create-a-new-tenant-prior-to-migrating-from-pmc"></a>Caso não deseje usar seu locatário existente do Azure AD do Office 365 para o Partner Center, crie outro locatário antes da migração do PMC.

Pode haver muitos motivos pelos quais você não deseje usar um locatário existente do Azure AD para configurar sua conta do Partner Center. Antes de começar a migração para o Partner Center, acesse o [portal do Azure](https://ms.portal.azure.com/#home) para criar um locatário do Azure AD. Siga as diretrizes em [Criar um locatário no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/quickstart-create-new-tenant). Use o novo locatário do AAD para configurar sua conta do Partner Center. Você precisa ser um administrador global para criar o locatário. 

### <a name="user-roles-including-guest-user-roles-in-partner-center"></a>Funções de usuário, incluindo funções de usuário convidado no Partner Center

O Partner Center tem diferentes tipos de funções, dependendo dos tipos de trabalho que precisam ser feitos. Há funções como administrador global, que são funções do Azure AD. Algumas das funções são específicas de programa, como o programa Provedor de Serviços de Nuvem ou incentivos, e há funções específicas do MPN. Para descobrir quais são todas as funções do Partner Center, leia [Atribuir funções e permissões de usuários](permissions-overview.md).

### <a name="what-happens-to-my-users-roles-when-they-move-from-pmc-to-partner-center"></a>O que acontece com as funções dos meus usuários quando eles migram do PMC para o Partner Center?

Exceto o administrador global do MPN ou o contato principal do programa que realiza a migração, todos os usuários do PMC perderão as respectivas funções de administrador. O indivíduo que conclui a migração precisará atribuir funções no Partner Center. As funções no Partner Center são diferentes das funções no PMC. Leia [Atribuir funções e permissões de usuários]\(permissões-overview.md) e [Como migrar do PMC para o Partner Center](move-pmc-pc-map.md#user-roles) para obter mais informações sobre as funções de usuário do Partner Center.

### <a name="whats-the-difference-between-my-company-profile-and-my-business-profile"></a>Qual é a diferença entre o meu perfil de empresa e o meu perfil comercial?

Seu perfil de empresa são as informações sobre a sua empresa que incluem endereço, localizações, contato principal, bem como dados bancários e fiscais.

Seu perfil comercial é como você se apresenta aos clientes e é uma página de marketing que exibe seu logotipo, os detalhes sobre seu enfoque empresarial, sua experiência etc.

### <a name="what-does-account-consolidation-mean-for-my-account"></a>O que significa a consolidação de conta para minha conta?

Se você usar o mesmo locatário do Azure AD para migrar várias contas do MPN para o Partner Center, o sistema o reconhecerá automaticamente e solicitará que você consolide suas contas. Isso é verdadeiro mesmo se você tem vários domínios associados ao mesmo locatário do Azure AD. 

Você ainda pode decidir migrar para o Partner Center usando locatários separados do AAD, mas observe que isso resulta em uma avaliação isolada de suas competências e custos de compras extras. Para obter mais informações sobre a consolidação de contas, leia [Consolidar as contas da empresa](consolidate-accounts.md)

### <a name="if-i-have-multiple-aad-tenants-and-a-single-mpn-account-is-it-possible-to-link-them-in-partner-center"></a>Se eu tiver vários locatários do AAD e uma só conta do MPN, será possível vinculá-los no Partner Center?

Sim, no Partner Center, você poderá vincular vários locatários do Azure AD à única conta do Partner Center.
Para obter mais informações sobre a consolidação de contas, leia [Consolidar as contas da empresa](consolidate-accounts.md)

### <a name="are-there-restrictions-to-adding-multiple-azure-ad-tenants-to-a-single-partner-center-account"></a>Há restrições à adição de vários locatários do Azure AD a uma só conta do Partner Center?

Se o locatário do Azure AD já estiver associado a uma conta existente do Partner Center, ele não poderá ser associado a novas contas do Partner Center usando o recurso de multilocatário. Outra maneira de considerar isso é que um locatário do Azure AD só pode ser associado a uma conta do Partner Center, mas uma conta do Partner Center pode ter vários locatários associados a ele.

## <a name="microsoft-partner-network-mpn-membership-migration"></a>Migração de associação do MPN (Microsoft Partner Network) 

Confira as respostas a seguir a perguntas comuns sobre a migração da associação do MPN.

### <a name="who-can-perform-the-move-from-pmc-to-partner-center"></a>Quem pode realizar a migração do PMC para o Partner Center?

O contato principal do programa ou o administrador global da empresa do MPN (essas duas funções geralmente são mantidas pela mesma pessoa) pode iniciar e realizar a migração.

### <a name="will-the-person-completing-the-migration-become-the-primary-contact-on-the-company-legal-profile-in-partner-center"></a>A pessoa que estiver concluindo a migração se tornará o contato principal do perfil legal da empresa no Partner Center?

No entanto, não necessariamente, o contato principal precisa ser alguém que tenha autorização para assinar contratos.

### <a name="can-microsoft-migrate-my-mpn-membership-for-me"></a>A Microsoft pode migrar minha associação do MPN para mim?

Não. A Microsoft não pode ajudar você a migrar sua conta de associação para o Partner Center. Você precisará migrar sua conta entrando no PMC com a conta corporativa (credenciais de entrada) para iniciar o processo de migração. Depois de concluir as etapas para migrar sua conta, inicie o gerenciamento da sua associação e atribua funções e permissões de usuário à sua equipe, de modo que ela possa acessar os benefícios e ajudar a gerenciar a associação. 

A Microsoft migrará automaticamente as competências, os benefícios, as informações de localização, as informações bancárias/fiscais para incentivos e as associações do MCP atuais, incluindo o acesso à Partner University.

### <a name="how-will-the-renewal-policy-change"></a>Como a política de renovação será alterada?

No Partner Center, a janela de renovação começa a ser contada da data de aniversário até os 30 dias seguintes.

### <a name="will-our-competencies-remain-unchanged-after-we-move-to-partner-center"></a>Nossas competências permanecerão inalteradas depois de migrarmos para o Partner Center?

Sim, as competências não serão afetadas pela migração para o Partner Center. Se você observar discrepâncias, entre em contato com o [suporte](https://partner.microsoft.com/support).

### <a name="will-my-benefits-including-cloud-benefits-technical-support-software-benefits-visual-studio-change-after-we-move"></a>Meus benefícios (incluindo benefícios na nuvem, suporte técnico, benefícios de software e Visual Studio) serão alterados após a migração?

Seus benefícios qualificados não serão alterados. Se você observar discrepâncias, entre em contato com o [suporte](https://partner.microsoft.com/support).

### <a name="will-our-microsoft-accounts-that-have-visual-studio-benefits-allocations-be-honored"></a>Nossas contas Microsoft que têm alocações de benefícios do Visual Studio serão respeitadas?

Sim. Os benefícios do Visual Studio alocados para o MSAs serão respeitados e mantidos. Eles também serão preservados após a renovação no Partner Center. No entanto, se você remover uma alocação da MSA depois que ela for migrada no Partner Center, ela não poderá ser adicionada novamente ao Partner Center.

No Partner Center, um parceiro pode adicionar contas corporativas e contas de usuário convidado, que sejam MSA, por meio do mesmo locatário em que o parceiro é o administrador do MPN no locatário do Azure AD. Se o parceiro for um administrador global em vários locatários do Azure AD e todos esses locatários estiverem associados à mesma conta do Partner Center, o parceiro poderá adicionar usuários em todos esses locatários aos benefícios do Visual Studio e às alocações baseadas em uso do Azure.

Embora os usuários convidados possam receber assinaturas baseadas em uso do Visual Studio pelo administrador do MPN ou pelo administrador global, os usuários convidados não podem entrar no Partner Center usando as respectivas MSAs. No entanto, os usuários convidados podem entrar no Azure e no Visual Studio para validar e usar os respectivos benefícios atribuídos.

### <a name="how-should-we-manage-our-mcp-associations-and-our-partner-university-access"></a>Como devemos gerenciar nossas associações do MCP e nosso acesso à Partner University?

Não há alterações nas associações do MCP migradas do PMC. No entanto, após a sua migração para o Partner Center, os novos funcionários precisarão ser associados no Partner Center. Todas as permissões da Partner University para os usuários existentes permanecerão, mas os novos funcionários deverão acessar [o centro de treinamento](https://partner.microsoft.com/training) para obter informações sobre como obter acesso à Partner University.

### <a name="how-do-i-view-mcp-information-once-i-move-to-partner-center"></a>Como ver as informações do MCP após a minha migração para o Partner Center?

Selecione **Competências** na barra de navegação à esquerda no painel. Na página **Competências**, você poderá baixar o relatório de habilidades. O relatório de habilidades listará os usuários que adquiriram habilidades relevantes para as competências e os programas no Partner Center. Se os usuários adquiriram habilidades, mas essas habilidades não são relevantes para as competências para as quais você está trabalhando, elas não são listadas no relatório.

### <a name="are-customer-references-used-in-partner-center"></a>As referências do cliente são usadas no Partner Center?

Não, você não precisa de referências do cliente para atender aos requisitos de competência no Partner Center.

### <a name="will-partner-of-record-associations-move-to-partner-center"></a>As associações do parceiro de registro serão migradas para o Partner Center?

Sim, não haverá nenhuma alteração no parceiro de registro. Saiba mais sobre [como vincular sua ID de Parceiro aos clientes](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started).

### <a name="is-there-an-impact-to-incentives-because-of-the-move-to-partner-center"></a>Há algum impacto nos incentivos devido à migração para o Partner Center?

Não. Não haverá nenhum impacto nos incentivos se você tiver migrado sua conta sem consolidar as localizações. Se a sua empresa tiver várias contas no PMC e, quando você migrar para o Partner Center, você decidir consolidá-las em uma conta global, não haverá perda nos incentivos, mas poderá haver um atraso no pagamento de incentivos. 

Se você não migrar todas as suas contas do PMC envolvidas em programas de incentivos, poderá parar de ganhar incentivos vinculados a essas contas.

### <a name="what-are-the-incentive-roles-in-partner-center"></a>O que são funções de incentivo no Partner Center?

As funções dos incentivos no Partner Center são baseadas na localização e incluem o administrador e o usuário de incentivos. Para obter mais informações sobre o que essas funções podem fazer, confira [Atribuir funções e permissões de usuários](permissions-overview.md).

### <a name="can-incentives-admins-be-assigned-at-the-global-and-location-level"></a>Os administradores de incentivos podem ser atribuídos nos níveis global e da localização?

Sim. Você pode atribuir um administrador de incentivos para ser o administrador de incentivos em todas as localizações ou cada localização pode ter o próprio administrador de incentivos.

### <a name="can-incentives-be-paid-at-the-global-or-location-level"></a>Os incentivos podem ser pagos no nível global ou da localização?

Os incentivos são pagos apenas no nível da localização.

### <a name="regarding-referrals-how-many-business-profiles-can-we-create"></a>Com relação às indicações, quantos perfis comerciais podemos criar?

Sua empresa poderá criar quantos perfis comerciais forem necessários para representar totalmente os interesses dela. Em cada perfil comercial, você pode listar até cinco localizações, uma localização por país/região. Cada um dos perfis comerciais pode receber indicações para cada uma das localizações.

### <a name="how-will-referrals-be-assigned-what-changes-can-i-expect-for-example-if-i-have-a-global-company-in-one-market-and-locations-in-other-markets-how-will-referrals-be-assigned"></a>Como as indicações serão atribuídas e quais alterações eu posso esperar? Por exemplo, se eu tiver uma empresa global em um mercado e localizações em outros mercados, como as indicações serão atribuídas?

As indicações são atribuídas com base nos parâmetros de pesquisa definidos pelo cliente. Independentemente de você ter uma localização ou muitas, se os clientes especificarem uma localização desejada e você tiver uma empresa que atenda aos outros parâmetros, a indicação se deslocará para essa localização.

### <a name="i-am-migrating-to-partner-center-from-within-russia-i-get-an-error-message-about-web-direct-how-do-i-continue-with-the-migration"></a>Estou migrando para o Partner Center de dentro da Rússia. Recebi uma mensagem de erro sobre o Web Direct. Como fazer para continuar com a migração?

Se você receber uma mensagem de erro porque está participando do programa Web Direct, faça o seguinte:

1. Entre no portal.Azure.com e crie um locatário do Azure AD. Para obter mais informações, leia [Criar um locatário do Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-access-create-new-tenant).

2. Depois de criar o locatário do Azure AD, use-o para migrar do Partner Membership Center para o Partner Center ou para se registrar como novo no Partner Center.
