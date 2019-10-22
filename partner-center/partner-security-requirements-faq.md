---
title: Perguntas frequentes sobre os requisitos de segurança de parceiros | Partner Center
ms.topic: article
ms.date: 09/27/2019
description: Perguntas frequentes sobre os requisitos de segurança de parceiros
author: isaiahwilliams
ms.author: iswillia
keywords: O Azure Active Directory, provedor de soluções na nuvem, programa de provedor de soluções na nuvem, CSP, fornecedor do painel de controle, CPV, autenticação multifator, MFA, modelo de aplicativo seguro, modelo de aplicativo seguro, segurança
ms.localizationpriority: high
ms.openlocfilehash: e9471ae8dd0e478540e30a879d010ffb0c1f1bc0
ms.sourcegitcommit: c388fae97437b727edeb0de3712bd2822010ecd6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2019
ms.locfileid: "71678300"
---
# <a name="frequently-asked-questions-about-the-partner-security-requirements"></a>Perguntas frequentes sobre os requisitos de segurança de parceiros

Este artigo contém algumas perguntas frequentes sobre os [requisitos de segurança de parceiros](partner-security-requirements.md).

## <a name="partner-security-requirements"></a>Requisitos de segurança de parceiros

### <a name="what-are-the-new-partner-security-requirements"></a>Quais são os novos requisitos de segurança de parceiros?

Para proteger nossos parceiros e seus clientes, estamos exigindo que os parceiros executem as seguintes ações imediatamente:  

1. **Habilite a MFA (Autenticação Multifator) para todos os usuários em locatários de parceiros**. Todos os usuários em locatários de parceiros devem usar a MFA (Autenticação Multifator) ao entrar nos serviços de nuvem comercial da Microsoft ou para transações no CSP por meio do Partner Center ou de APIs. Por meio da habilitação das políticas de proteção de linha de base, a MFA está disponível sem nenhum custo para todos os usuários de locatários de parceiros.

2. **Adote a estrutura do Modelo de Aplicativo Seguro**. Todos os parceiros que se integrarem com uma API da Microsoft – como as APIs do Azure Resource Manager, do Microsoft Graph e do Partner Center – deverão adotar a estrutura do Modelo de Aplicativo Seguro para evitar qualquer interrupção em sua integração quando as políticas de linha de base estiverem habilitadas.

Habilitar a MFA (Autenticação Multifator) e adotar a estrutura do Modelo de Aplicativo Seguro ajudará a proteger a sua infraestrutura e os dados do cliente contra possíveis riscos de segurança, identificando roubos e outros incidentes de fraude.  

### <a name="which-partners-need-to-meet-the-requirements"></a>Quais parceiros precisam atender aos requisitos?

Esses requisitos são destinados aos seguintes grupos de parceiros:

- Todas as organizações parceiras que participam do programa CSP (Provedor de Soluções na Nuvem) e que estão realizando transações por meio dos serviços de nuvem comercial da Microsoft
  - Parceiros de fatura direta
  - Provedores indiretos
  - Revendedores indiretos
- Todos os Fornecedores do Painel de Controle
- Todos os parceiros do programa Advisor  

Todos os parceiros que realizam transações por meio de uma nuvem soberana (21Vianet, governo dos EUA e Alemanha) não são obrigados a cumprir os novos requisitos de segurança, em vigor a partir de 1º de agosto. No entanto, é altamente recomendável que todos os parceiros que usam uma nuvem soberana atuem e adotem esses novos requisitos de segurança imediatamente. Futuramente, a Microsoft fornecerá detalhes adicionais sobre a imposição desses requisitos de segurança para nuvens soberanas.

### <a name="what-are-the-key-timelines-and-milestones"></a>Quais são as principais linhas do tempo e marcos?

Os termos associados a esses requisitos de segurança serão adicionados imediatamente ao [Guia do Programa Provedor de Soluções na Nuvem](https://go.microsoft.com/fwlink/p/?LinkId=617100). Você precisará implementar esses requisitos de segurança para estar em conformidade com a sua participação no programa CSP, em vigor a partir de 1º de agosto de 2019.

### <a name="what-will-happen-if-i-do-not-take-any-actions"></a>O que acontecerá se eu não executar nenhuma ação?

Os parceiros que não cumprirem essas obrigações e práticas de segurança não poderão realizar transações no programa Provedor de Soluções na Nuvem, nem gerenciar locatários de clientes que aproveitam os direitos de administrador delegado, uma vez que esses requisitos de segurança de parceiros serão impostos. Estamos no processo de estabelecer uma data de imposição para os requisitos e notificaremos a data aos parceiros com informações detalhadas.

### <a name="what-will-happen-if-i-dont-implement-mfa-as-per-this-new-security-requirement-by-august-1-2019"></a>O que acontecerá se eu não implementar a MFA de acordo com esses novos requisitos de segurança até 1º de agosto de 2019?

A partir de 1º de agosto de 2019, entraram em vigor os termos associados a esses requisitos de segurança no [Guia do Programa do Provedor de Soluções na Nuvem](https://go.microsoft.com/fwlink/p/?LinkId=617100). Todos os parceiros que participam do programa CSP devem atender aos requisitos para estar em conformidade com os termos e proteger seus negócios. Os parceiros que não obedecerem a essas práticas de segurança poderão perder sua capacidade de realizar transações no programa CSP ou de gerenciar locatários de clientes que aproveitam os direitos de administrador delegado, uma vez que iniciaremos a imposição técnica dos requisitos de segurança de parceiros em um futuro próximo. Estamos estabelecendo uma data de imposição e notificaremos os parceiros sobre esse assunto em breve.

### <a name="why-is-microsoft-enforcing-these-new-requirements"></a>Por que a Microsoft está impondo esses novos requisitos?

A segurança e a privacidade de clientes e parceiros são a principal prioridade da Microsoft. Continuamos a ver uma escalada no número e na sofisticação dos ataques de segurança, principalmente aqueles relacionados a incidentes de comprometimento da identidade. Como os controles de prevenção desempenham uma função fundamental na estratégia global de defesa para frustrar os ataques de segurança, passaremos a impor um conjunto de requisitos de segurança obrigatórios para ajudar a proteger os parceiros e seus clientes.

### <a name="does-this-apply-to-all-geographies"></a>Isso se aplica a todas as geografias?

Sim, isso se aplica a todas as geografias. É altamente recomendável que todos os parceiros que negociam em uma nuvem soberana (21Vianet, governo dos EUA e Alemanha) atuem e adotem esses novos requisitos de segurança imediatamente. No entanto, esses parceiros não precisam atender aos novos requisitos de segurança, em vigor a partir de 1º de agosto. Futuramente, a Microsoft fornecerá detalhes adicionais sobre a imposição desses requisitos de segurança para nuvens soberanas.

### <a name="is-it-possible-to-get-an-exclusion-for-an-account"></a>É possível abrir exceção para uma conta?

Não, não é possível isentar nenhuma conta do requisito de ter a MFA imposta. Considerando a natureza altamente privilegiada de ser um parceiro, o [Guia do Programa Provedor de Soluções na Nuvem](https://go.microsoft.com/fwlink/p/?LinkId=617100) exige que a MFA seja imposta para todas as contas do seu locatário de parceiro.

## <a name="required-actions"></a>Ações necessárias

### <a name="what-are-the-key-actions-i-need-to-take-to-meet-the-requirements"></a>Quais são as principais ações que preciso executar para atender aos requisitos?

Todos os parceiros do programa CSP (conta direta, provedor indireto e revendedor indireto), assistentes e fornecedores de painel de controle devem atender aos requisitos.

1. **Impor a MFA para todos os usuários**

    Todos os parceiros do programa CSP, assistentes e fornecedores de painel de controle são obrigados a impor a MFA para todos os usuários do locatário de parceiro. Isso pode ser feito habilitando as políticas de linha de base [Exigir MFA para administradores](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) e [Proteção do usuário final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users), bem como todas as políticas de linha de base futuras. A funcionalidade fornecida pelas políticas de linha de base continuará a evoluir para garantir que parceiros e clientes estejam protegidos contra as ameaças de segurança em constante alteração. Portanto, é importante que você examine a [documentação das políticas de linha de base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) para saber mais.

    - Confira a [Política de linha de base: exigir MFA para administradores](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) a fim de obter detalhes sobre como habilitar essa política de linha de base.
    - Confira a [Política de linha de base: proteção do usuário final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) para obter detalhes sobre como habilitar essa política de linha de base.
    - Entenda o conceito das [políticas de proteção de linha de base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection).

    Considerações adicionais:

    - os provedores indiretos precisarão trabalhar com os revendedores indiretos para se integrar ao Partner Center, caso ainda não o tenham feito, além de encorajar seus revendedores a atender aos requisitos.
    - O Azure MFA está sendo disponibilizado sem custo para todos os usuários do locatário de parceiro por meio das políticas de linha de base, tendo como único método de verificação o uso do [Aplicativo Microsoft Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview).
    - Há métodos de verificação adicional disponíveis por meio das SKUs do [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium), caso outros métodos – uma chamada telefônica ou mensagem e texto – sejam necessários.
    - Os parceiros também podem aproveitar uma solução de MFA de terceiros para cada conta ao acessar os serviços de nuvem comercial da Microsoft.

2. **Adotar a estrutura do Modelo de Aplicativo Seguro**

    Todos os parceiros que desenvolveram uma integração personalizada usando qualquer API (como as APIs do Azure Resource Manager, do Microsoft Graph, do Partner Center, etc.) ou que implementaram uma automação personalizada usando ferramentas como o PowerShell, precisarão adotar a [estrutura do Modelo de Aplicativo Seguro](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) para se integrar com os serviços em nuvem da Microsoft. Deixar de fazer isso pode resultar em uma interrupção devido à implantação da MFA. Os recursos a seguir fornecem uma visão geral e orientações a respeito de como adotar o modelo.

    - [Visão geral do Modelo de Aplicativo Seguro](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
    - [Partner Center: guia do Modelo de Aplicativo Seguro](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
    - [Parceiros no programa CSP: código de exemplo em .NET para habilitar o Modelo de Aplicativo Seguro](https://docs.microsoft.com/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
    - [Parceiros no programa CSP: código de exemplo em Java para habilitar o Modelo de Aplicativo Seguro](https://docs.microsoft.com/samples/microsoft/partner-center-java-samples/secure-app-model/)
    - [Documento de autenticação do Partner Center](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
    - [Documento de MFA (Autenticação Multifator) do PowerShell do Partner Center](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth)

    Se você estiver usando um painel de controle, será necessário consultar o fornecedor a respeito da adoção da estrutura do Modelo de Aplicativo Seguro.

    Os fornecedores de painel de controle são obrigados a se [integrar](https://docs.microsoft.com/partner-center/enroll-as-cpv) com o Partner Center como fornecedores de painel de controle e começar a implementar esses requisitos imediatamente. Confira [Partner Center: estrutura do Modelo de Aplicativo Seguro](http://assetsprod.microsoft.com/secure-application-model-guide.pdf). Os fornecedores de painel de controle devem aceitar e gerenciar o consentimento dos parceiros do CSP em vez de credenciais e limpar todas as credenciais de parceiros do CSP existentes.

## <a name="multi-factor-authentication"></a>Autenticação Multifator

### <a name="what-is-multi-factor-authentication-mfa"></a>O que é a MFA (Autenticação Multifator)?

A MFA é um mecanismo de segurança por meio do qual os indivíduos são autenticados por mais de um procedimento obrigatório de validação e segurança. Ela funciona exigindo dois ou mais dos seguintes métodos de autenticação:

- Algo que você sabe (geralmente uma senha)
- Algo que você tem (um dispositivo confiável que não é duplicado facilmente, como um telefone)
- Algo que você é (biometria)

### <a name="what-are-baseline-protection-policies"></a>O que são as políticas de proteção de linha de base?

As [políticas de proteção de linha de base da Microsoft](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) (atualmente em versão prévia) são um conjunto de políticas predefinidas que ajudam a proteger as organizações contra inúmeros ataques comuns. Esses ataques comuns podem incluir pulverização, reprodução e phishing de senha. As políticas de linha de base estão disponíveis em todas as edições do Azure Active Directory. A Microsoft está disponibilizando essas políticas de proteção de linha de base para todos, pois o volume de ataques baseados em identidade vem aumentando nos últimos anos. O objetivo dessas políticas é permitir que todas as organizações tenham um nível de segurança de linha de base habilitado sem custo adicional.

> [!NOTE]
> As políticas de linha de base da Microsoft e as funcionalidades relacionadas continuarão a evoluir para proteger melhor os parceiros e clientes contra as ameaças de segurança em constante alteração. Pode haver algumas alterações de nomenclatura e taxonomia nas políticas de linha de base em breve. É altamente recomendável que você visite as páginas das políticas de linha de base diretamente para conferir as informações mais recentes.

### <a name="what-baseline-policies-must-i-enable"></a>Quais políticas de linha de base eu devo habilitar?

Se você estiver planejando utilizar as políticas de proteção de linha de base atuais a fim de fornecer MFA para cada conta no locatário de parceiro, será necessário habilitar as políticas de linha de base [Exigir MFA para administradores](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) e [Proteção do usuário final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users). Essas políticas de proteção de linha de base atenderão ao requisito de MFA para cada usuário no locatário de parceiro sem custo apenas para os parceiros que estão usando o Aplicativo Microsoft Authenticator por meio de dispositivos móveis.

A política de linha de base [Exigir MFA para administradores](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) é aproveitada para usuários administrativos no diretório de parceiros, ao passo que a política de linha de base [Proteção do usuário final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) é aproveitada para proteger usuários não administrativos no locatário de parceiro. Habilitar essas políticas exigirá que os usuários se registrem na MFA. Depois que o usuário for registrado com sucesso, será solicitada a MFA em cada tentativa de conexão com base nos critérios da política. A funcionalidade fornecida pelas políticas de linha de base continuará a evoluir para garantir que parceiros e clientes estejam protegidos contra as ameaças de segurança em constante alteração. Portanto, é importante que você examine a [documentação das políticas de linha de base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) para saber mais.

### <a name="how-do-i-enable-the-require-mfa-for-admins-policy"></a>Como faço para habilitar a política Exigir MFA para administradores?

A política de linha de base Exigir MFA para administradores pode ser habilitada por meio do portal de gerenciamento do Azure. Confira a [Política de linha de base: exigir MFA para administradores](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) a fim de obter detalhes sobre como habilitar essa política de linha de base.

### <a name="how-do-i-enable-the-end-user-protection-policy"></a>Como faço para habilitar a política de Proteção do usuário final?

A política de linha de base Proteção do usuário final pode ser habilitada por meio do portal de gerenciamento do Azure. Confira a [Política de linha de base: proteção do usuário final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) para obter detalhes sobre como habilitar essa política de linha de base.

### <a name="will-the-baseline-policies-be-automatically-enabled"></a>As políticas de linha de base serão habilitadas automaticamente?

Não. Para habilitar essas políticas, um usuário que seja membro das funções de administrador global, administrador de segurança ou administrador de acesso condicional precisará configurar as políticas para Usar a política imediatamente.

### <a name="what-is-the-cost-of-enabling-mfa"></a>Qual é o custo para habilitar a MFA?

A Microsoft fornece a MFA sem nenhum custo por meio da implementação das políticas de proteção de linha de base [Exigir MFA para administradores](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) e [Proteção do usuário final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users). A única opção de verificação disponível por meio desta versão da MFA é o [Aplicativo Microsoft Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview). Se for necessário realizar uma chamada telefônica ou enviar uma mensagem SMS, será preciso comprar uma licença do [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium). Como alternativa, você pode utilizar uma solução de terceiros para fornecer MFA a cada usuário em seu locatário de parceiro – nesse caso, é sua responsabilidade garantir que a solução de MFA esteja sendo imposta e que você permaneça em conformidade.

### <a name="if-i-already-have-an-mfa-solution-what-actions-do-i-need-to-take"></a>Se eu já tiver uma solução de MFA, quais ações precisarei executar?

Por meio desses requisitos de segurança, será exigido que os usuários de um locatário de parceiro sejam autenticados usando a MFA ao acessar os serviços de nuvem comercial da Microsoft. Uma solução de terceiros pode ser usada para atender a esses requisitos. A Microsoft não fornece mais testes de validação a provedores de identidade independentes para compatibilidade com o Azure Active Directory. Se você quiser testar seu produto quanto à interoperabilidade, consulte estas [orientações](https://www.microsoft.com/download/details.aspx?id=56843).

> [!IMPORTANT]
> Se você estiver usando uma solução de terceiros, será importante verificar se a solução está emitindo a declaração da AMR (referência de método de autenticação) que inclui o valor da MFA. Confira [Teste dos Requisitos de Segurança do Parceiro](https://docs.microsoft.com/powershell/partnercenter/test-partner-security-requirements) para obter detalhes sobre como validar sua solução de terceiros que está emitindo a declaração esperada.

### <a name="what-verification-method-can-i-use-to-authenticate-mfa"></a>Qual método de verificação eu posso usar para autenticar com a MFA?

A Microsoft fornece a MFA sem nenhum custo por meio da implementação das políticas de proteção de linha de base [Exigir MFA para administradores](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) e [Proteção do usuário final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users). A única opção de verificação disponível por meio desta versão da MFA é o [Aplicativo Microsoft Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview). Se for necessário realizar uma chamada telefônica ou enviar uma mensagem SMS, será preciso comprar uma licença do [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium). Como alternativa, você pode utilizar uma solução de terceiros para fornecer MFA a cada usuário em seu locatário de parceiro – nesse caso, é sua responsabilidade garantir que a solução de MFA esteja sendo imposta e que você permaneça em conformidade.

### <a name="i-use-multiple-partner-tenants-to-transact-do-i-need-to-implement-mfa-on-them-all"></a>Eu uso vários locatários de parceiros para realizar transações. É necessário implementar a MFA em todos eles?

Sim, será necessário impor a MFA para cada locatário do Azure Active Directory associado ao programa CSP ou ao programa Advisor. Se você planeja comprar uma licença do Azure Active Directory Premium, então uma licença deverá ser adquirida para o usuário em cada locatário do Azure Active Directory.

### <a name="does-each-user-in-my-partner-tenant-need-to-have-mfa-enforced"></a>É necessário impor a MFA a todos os usuários do meu locatário de parceiro?*

As políticas de proteção de linha de base [Exigir MFA para administradores](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) e [Proteção do usuário final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) imporão a MFA para cada usuário do seu locatário de parceiro. Se você estiver aproveitando essas políticas para fornecer a MFA e estiver usando o aplicativo [Microsoft Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview), não será necessário comprar nenhuma licença adicional. Caso contrário, será necessário comprar uma solução apropriada para fornecer a MFA a cada usuário do seu locatário de parceiro.

### <a name="i-am-a-direct-bill-partner-with-microsoft-what-do-i-need-to-do"></a>Sou um parceiro de cobrança direta da Microsoft. O que preciso fazer?

Parceiros de cobrança direta do Provedor de Soluções na Nuvem devem impor a MFA para cada usuário do seu locatário de parceiro.

### <a name="i-am-an-indirect-reseller-and-only-transact-though-a-distributor-do-i-still-have-to-do-this"></a>Sou um revendedor indireto e realizo transações apenas por meio de um distribuidor. Mesmo assim tenho que fazer isso?

Todos os revendedores indiretos precisam impor a MFA para cada usuário do seu locatário de parceiro. Essa é uma ação que o revendedor indireto deve executar.

### <a name="i-do-not-use-the-partner-center-api-do-i-still-need-to-implement-mfa"></a>Eu não uso a API do Partner Center. Mesmo assim preciso implementar a MFA?

Sim, esse requisito de segurança é para todos os usuários, inclusive usuários administradores de parceiros e usuários finais do locatário de parceiro.

### <a name="which-third-party-vendors-provide-mfa-solutions-compatible-with-azure-active-directory"></a>Quais fornecedores de terceiros oferecem soluções de MFA compatíveis com o Azure Active Directory?

Há muitas avaliações independentes de soluções de MFA online, como os relatórios da [Gartner](https://www.gartner.com/en/webinars/3881781). Ao examinar os fornecedores e as soluções de MFA, os parceiros devem garantir que a solução escolhida seja compatível com o Azure Active Directory.

A Microsoft não fornece mais testes de validação a provedores de identidade independentes para compatibilidade com o Azure Active Directory. Se você quiser testar seu produto quanto à interoperabilidade, consulte estas [orientações](https://www.microsoft.com/download/details.aspx?id=56843).

Para obter mais informações, confira a [lista de compatibilidade da federação do Azure AD](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-compatibility).

### <a name="how-can-i-test-mfa-in-our-integration-sandbox"></a>Como posso testar a MFA em nossa área restrita de integração?

As políticas de proteção de linha de base [Exigir MFA para administradores](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) e [Proteção do usuário final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) devem ser habilitadas para o locatário da área restrita de integração. Por meio dessa política, cada usuário do locatário será obrigado a se autenticar usando a MFA.

### <a name="will-enabling-mfa-effect-how-i-interact-with-my-customers-tenant"></a>Habilitar a MFA afetará a forma como eu interajo com o locatário do meu cliente?

Não. O cumprimento desses requisitos de segurança não afetará a maneira como você gerencia seus clientes. Sua capacidade de executar operações administrativas delegadas não será interrompida.

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a>Meus clientes estão sujeitos aos requisitos de segurança de parceiros?

Não, não é necessário impor a MFA para cada usuário nos locatários do Azure AD do seu cliente. No entanto, é recomendável que você trabalhe com cada cliente para determinar a melhor maneira de proteger os usuários de cada um deles.

### <a name="can-app-passwords-be-used-with-the-baseline-protection-policies"></a>As senhas de aplicativo podem ser usadas com as políticas de proteção de linha de base?

Sim, as [senhas de aplicativo](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) podem ser usadas. Você deve examinar as considerações de uso de senhas de aplicativo documentadas [aqui](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) a fim de determinar se elas são compatíveis com suas necessidades.

### <a name="can-any-user-be-excluded-from-this-requirement"></a>Algum usuário pode ser excluído deste requisito?

Não, todos os usuários do seu locatário de parceiro, inclusive as contas de serviço, serão obrigados a se autenticar usando a MFA.

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a>Os requisitos de segurança de parceiros se aplicam à área restrita de integração?

Sim, os requisitos de segurança de parceiros se aplicam à área restrita de integração. Isso significa que você precisará implementar a solução de MFA apropriada para os usuários do locatário da área restrita de integração. É recomendável que você implemente as políticas de proteção de linha de base para fornecer a MFA.

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a>Como faço para configurar uma conta de acesso de emergência?

É considerada uma melhor prática criar uma ou duas contas de acesso de emergência para evitar o bloqueio inadvertido do seu locatário do Azure AD. Em relação aos requisitos de segurança de parceiros, é necessário que cada usuário seja autenticado usando a MFA. Portanto, isso significa que você precisará modificar a definição da conta de acesso de emergência. Pode ser uma conta que esteja aproveitando uma solução de MFA de terceiros.

### <a name="how-will-guest-users-be-impacted-by-the-partner-security-requirements"></a>Como os usuários convidados serão afetados pelos requisitos de segurança de parceiros?

Será exigido que os usuários convidados sejam autenticados usando a MFA ao acessar recursos em seu locatário de parceiro. Os requisitos de segurança de parceiros não terão impacto sobre usuários convidados que acessarem recursos de seu próprio locatário.

### <a name="if-i-am-using-a-third-party-solution-is-active-directory-federation-service-adfs-required"></a>Se eu estiver usando uma solução de terceiros, o ADFS (Serviço de Federação do Active Directory) será necessário?

Não, não será necessário ter o ADFS (Serviço de Federação do Active Directory) se você estiver usando uma solução de terceiros. É recomendável que você trabalhe com o fornecedor da solução para determinar quais são os requisitos da solução dele.

### <a name="is-it-a-requirement-to-enable-the-baseline-protection-policies"></a>É um requisito obrigatório habilitar as políticas de proteção de linha de base?

Não, não é um requisito obrigatório habilitar as políticas de proteção de linha de base. O único requisito obrigatório é que você imponha a MFA para cada usuário do seu locatário de parceiro, inclusive das contas de serviço.

### <a name="can-conditional-access-be-used-to-meet-the-mfa-requirement"></a>O acesso condicional pode ser usado para atender ao requisito de MFA?

Sim, você pode usar o acesso condicional para impor a MFA para cada usuário do seu locatário de parceiro, inclusive das contas de serviço. Contudo, considerando a natureza altamente privilegiada de um parceiro, precisamos garantir que cada usuário tenha um desafio de MFA a cada autenticação realizada. Isso significa que você não poderá aproveitar o recurso de acesso condicional que contorna o requisito de MFA.

### <a name="what-verification-options-are-provided-through-the-implementation-of-the-baseline-protection-policies"></a>Quais opções de verificação são fornecidas por meio da implementação das políticas de proteção de linha de base?

Em relação à versão da MFA que está disponível por meio da implementação das políticas de proteção de linha de base, a única opção de verificação disponível é um aplicativo autenticador. O uso de uma chamada telefônica e uma mensagem de texto é considerado menos seguro. Portanto, essas opções não estão disponíveis por meio desta versão da MFA.

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>A conta de serviço usada pelo Azure AD Connect será afetada pelos requisitos de segurança de parceiros?

Não, a conta de serviço usada pelo Azure AD Connect não será afetada pelos requisitos de segurança de parceiros. Se você tiver um problema com o Azure AD Connect em virtude da imposição da MFA, abra uma solicitação de suporte técnico junto ao suporte da Microsoft.

## <a name="secure-application-model"></a>Modelo de Aplicativo Seguro

### <a name="who-should-adopt-the-secure-application-model-to-meet-the-requirements"></a>Quem deve adotar o modelo de aplicativo seguro para atender aos requisitos?

A Microsoft está introduzindo uma estrutura segura e escalonável para autenticar parceiros do CSP (Provedor de Soluções na Nuvem) e CPVs (Fornecedores de Painel de Controle) que aproveitam a Autenticação Multifator. Consulte o [guia do Modelo de Aplicativo Seguro](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) para obter mais informações. Todos os parceiros que desenvolveram uma integração personalizada usando qualquer API (como as APIs do Azure Resource Manager, do Microsoft Graph, do Partner Center, etc.) ou que implementaram uma automação personalizada usando ferramentas como o PowerShell, precisarão adotar a [estrutura do Modelo de Aplicativo Seguro](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) para se integrar com os serviços em nuvem da Microsoft.

### <a name="what-is-the-secure-application-model"></a>O que é o Modelo de Aplicativo Seguro?

A Microsoft está introduzindo uma estrutura segura e escalonável para autenticar parceiros do CSP (Provedor de Soluções na Nuvem) e CPVs (Fornecedores de Painel de Controle) que aproveitam a Autenticação Multifator. Consulte o [guia do Modelo de Aplicativo Seguro](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) para obter mais informações.  

### <a name="how-do-i-implement-the-secure-application-model"></a>Como faço para implementar o Modelo de Aplicativo Seguro?

Todos os parceiros que desenvolveram uma integração personalizada usando qualquer API (como as APIs do Azure Resource Manager, do Microsoft Graph, do Partner Center, etc.) ou que implementaram uma automação personalizada usando ferramentas como o PowerShell, precisarão adotar a [estrutura do Modelo de Aplicativo Seguro](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) para se integrar com os serviços em nuvem da Microsoft. Deixar de fazer isso pode resultar em uma interrupção devido à implantação da MFA. Os recursos a seguir fornecem uma visão geral e orientações a respeito de como adotar o modelo.

- [Visão geral do Modelo de Aplicativo Seguro](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [Partner Center: guia do Modelo de Aplicativo Seguro](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Parceiros no programa CSP: código de exemplo em .NET para habilitar o Modelo de Aplicativo Seguro](https://docs.microsoft.com/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [Parceiros no programa CSP: código de exemplo em Java para habilitar o Modelo de Aplicativo Seguro](https://docs.microsoft.com/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [Documento de autenticação do Partner Center](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
- [Documento de MFA (Autenticação Multifator) do PowerShell do Partner Center](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth)

Se você estiver usando um painel de controle, será necessário consultar o fornecedor a respeito da adoção da estrutura do Modelo de Aplicativo Seguro.

Os fornecedores de painel de controle são obrigados a se [integrar](https://docs.microsoft.com/partner-center/enroll-as-cpv) com o Partner Center como fornecedores de painel de controle e começar a implementar esses requisitos imediatamente. Confira [Partner Center: estrutura do Modelo de Aplicativo Seguro](http://assetsprod.microsoft.com/secure-application-model-guide.pdf). Os fornecedores de painel de controle devem aceitar e gerenciar o consentimento dos parceiros do CSP em vez de credenciais e limpar todas as credenciais de parceiros do CSP existentes.

### <a name="who-is-a-control-panel-vendor-cpv"></a>Quem é um CPV (Fornecedor de Painel de Controle)?

Um Fornecedor de Painel de Controle é um fornecedor independente de software que desenvolve aplicativos a serem usados por Parceiros do CSP para integração com as APIs do Partner Center. Um Fornecedor de Painel de Controle não é um Parceiro do CSP com acesso direto às APIs ou ao Painel do Partner Center. Uma descrição detalhada está disponível no guia [Partner Center: Modelo de Aplicativos Seguros](http://assetsprod.microsoft.com/secure-application-model-guide.pdf).

### <a name="does-the-secure-application-model-need-to-be-implemented-for-the-partner-center-apisdk-only"></a>O Modelo de Aplicativo Seguro precisa ser implementado somente para a API/o SDK do Partner Center?

Quando ambas as políticas de linha de base *Exigir MFA para administradores* e *Proteção do usuário final* estiverem habilitadas, será exigido que cada usuário seja autenticado usando a Autenticação Multifator. Isso significa que você precisará implementar o Modelo de Aplicativo Seguro para cada API, CLI e módulo do PowerShell (por exemplo, Azure, Azure AD, MS online, Partner Center etc.) que se destinar à execução não interativa e que depender do uso de credenciais do usuário para autenticação.

### <a name="i-am-using-automation-tools-such-as-powershell-how-do-i-implement-the-secure-application-model"></a>Estou usando ferramentas de automação, como o PowerShell. Como faço para implementar o Modelo de Aplicativo Seguro?

Se a sua automação for destinada à execução não interativa e depender de credenciais do usuário para autenticação, então você precisará implementar o Modelo de Aplicativo Seguro. Confira [Modelo de Aplicativo Seguro | PowerShell do Partner Center](https://docs.microsoft.com/powershell/partnercenter/secure-app-model?view=partnercenterps-1.5) para obter orientação sobre como implementar essa estrutura.  Observe que nem todas as ferramentas de automação fornecem a capacidade de autenticação usando tokens de acesso. Se precisar de ajuda para entender quais alterações são necessárias, poste uma mensagem no grupo [Orientações de Segurança do Partner Center](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance).

### <a name="what-user-credentials-should-the-application-administrator-provide-when-performing-the-consent-process"></a>Quais credenciais de usuário o administrador de aplicativos deve fornecer ao executar o processo de consentimento?

É recomendável que você use uma conta de serviço à qual tenha sido atribuído o menor nível de permissões. Em relação à API do Partner Center, isso significa que você deve usar uma conta à qual tenha sido atribuída a função de Agente de Vendas ou de Agente de Administração.

### <a name="why-should-the-application-administrator-not-provide-global-admin-user-credentials-when-performing-the-consent-process"></a>Por que o administrador de aplicativos não deve fornecer credenciais de usuário administrador global ao executar o processo de consentimento?

É recomendável usar identidades com menos privilégios, assim você estará reduzindo o risco. Não é recomendável usar uma conta que tenha privilégios de administrador global, pois isso fornece mais permissões do que o necessário

### <a name="i-am-a-csp-partner-how-do-i-know-if-my-control-panel-vendor-cpv-is-working-on-implementing-the-solution-or-not"></a>Eu sou um parceiro do CSP. Como faço para saber se o meu CPV (Fornecedor de Painel de Controle) está trabalhando para implementar a solução ou não?

Para parceiros que usam a solução de um CPV (Fornecedor de Painel de Controle) para realizar transações no programa do CSP (Provedor de Soluções na Nuvem), é sua responsabilidade consultar seu CPV.

### <a name="i-am-a-cpv-how-do-i-enroll"></a>Eu sou um CPV. Como faço para me registrar?

Para se registrar como um CPV (Fornecedor de Painel de Controle), siga as orientações fornecidas [aqui](https://docs.microsoft.com/partner-center/enroll-as-cpv).

Para receber o link de registro, o CPV deve entrar em contato com [CPVHelp@microsoft.com](mailto:CPVHelp@microsoft.com) e informar um patrocinador funcionário da Microsoft que tenha uma relação comercial com ele ou que conheça seus negócios. Por exemplo, um PDM (Gerente de Desenvolvimento de Parceiros).

Depois registrar si mesmo e seus aplicativos no Partner Center, você terá acesso às APIs do Partner Center. Se você for um novo CPV, receberá suas informações de área restrita por meio de uma notificação do Partner Center. Depois de concluir o registro como CPV da Microsoft e aceitar o contrato de CPV, você poderá:

1. Gerenciar aplicativos multilocatários (adicionar aplicativos ao portal do Azure e registrar e cancelar o registro de aplicativos no Partner Center). Observação: os CPVs deverão registrar seus aplicativos no Partner Center para serem autorizados a usar as APIs do Partner Center. Apenas adicionar aplicativos ao portal do Azure não autoriza os aplicativos de CPV a usarem as APIs do Partner Center.
2. Exiba e gerencie seu perfil de CPV.
3. Exiba e gerencie seus usuários que precisam de acesso aos recursos de CPV. A única função que um CPV pode ter é a de Administrador Global.

### <a name="i-am-using-the-partner-center-sdk-will-sdk-automatically-adopt-the-secure-application-model"></a>Estou usando o SDK do Partner Center. O SDK adotará automaticamente o Modelo de Aplicativo Seguro?

Não, você terá que seguir as observações fornecidas no [guia do Modelo de Aplicativo Seguro](http://assetsprod.microsoft.com/secure-application-model-guide.pdf).

### <a name="can-i-generate-a-refresh-token-for-the-secure-application-model-with-accounts-that-do-not-have-mfa-enabled"></a>Eu posso gerar um token de atualização para o Modelo de Aplicativo Seguro com contas que não têm a MFA habilitada?

Sim, é possível gerar um token de atualização com uma conta que não imponha a MFA. No entanto, isso não deve ser feito porque todo token gerado usando uma conta que não tenha a MFA habilitada não será capaz de acessar os recursos devido ao requisito de MFA.

### <a name="how-should-my-application-obtain-an-access-token-if-we-enable-mfa"></a>Como o meu aplicativo deverá obter um token de acesso se habilitarmos a MFA?

Será necessário seguir o [guia do Modelo de Aplicativo Seguro](http://assetsprod.microsoft.com/secure-application-model-guide.pdf), que fornece detalhes sobre como fazer isso e, ao mesmo tempo, manter-se em conformidade com os novos requisitos de segurança. Você pode encontrar um código de exemplo em .NET [aqui](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model) e um código de exemplo em Java [aqui](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model).

### <a name="as-a-cpv-do-i-create-an-azure-ad-application-in-our-cpv-tenant-or-the-tenant-of-the-csp-partner"></a>Como um CPV, eu devo criar um aplicativo do Azure AD em nosso locatário do CPV ou no locatário do parceiro do CSP?

O CPV precisará criar o aplicativo do Azure Active Directory no locatário associado ao seu registro como CPV.

### <a name="i-am-a-csp-that-is-using-app-only-authentication-do-i-need-to-make-any-changes"></a>Sou um CSP que está usando a autenticação somente por aplicativo. Eu preciso fazer alguma alteração?

A autenticação somente por aplicativo não é afetada, pois as credenciais de usuário não estão sendo usadas para solicitar token de acesso. Se as credenciais do usuário estiverem sendo compartilhadas, os CPVs (Fornecedores de Painel de Controle) deverão adotar a [estrutura do Modelo de Aplicativo Seguro](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) e limpar todas as credenciais de parceiro existentes que eles tiverem.

### <a name="as-a-cpv-can-i-leverage-the-app-only-authentication-style-to-get-access-tokens"></a>Como um CPV, eu posso aproveitar o estilo de autenticação somente por aplicativo para obter tokens de acesso?

Não, os Fornecedores de Painel de Controle não podem utilizar o estilo de autenticação somente por aplicativo para solicitar tokens de acesso em nome do parceiro. Eles devem implementar o Modelo de Aplicativo Seguro, que utiliza o estilo de autenticação por aplicativo + usuário.

## <a name="enforcement"></a>Imposição

### <a name="i-am-using-a-third-party-mfa-solution-and-i-am-being-blocked-what-should-i-do"></a>Estou usando uma solução de MFA de terceiros e estou sendo bloqueado, o que devo fazer?

Para validar se a conta que está acessando os recursos foi desafiada pela autenticação multifator, verificaremos a declaração da [referência do método de autenticação](https://tools.ietf.org/html/rfc8176) para ver se a MFA está listada. Algumas soluções de terceiros não emitem essa declaração ou não incluem o valor da MFA. Se a declaração estiver ausente ou se o valor da MFA não estiver listado, não haverá como determinar se a conta autenticada foi desafiada pela autenticação multifator. Será necessário trabalhar com o fornecedor da solução de terceiros a fim de determinar quais ações precisam ser adotadas para que a solução emita a declaração da referência do método de autenticação.

Confira [Teste dos Requisitos de Segurança do Parceiro](https://docs.microsoft.com/powershell/partnercenter/test-partner-security-requirements?view=partnercenterps-2.0) caso não tenha certeza se a sua solução de terceiros está – ou não – emitindo a declaração esperada.

### <a name="mfa-is-blocking-me-from-supporting-my-customer-using-aobo-what-should-i-do"></a>A MFA está me impedindo de oferecer suporte ao meu cliente usando o AOBO, o que devo fazer?

A imposição técnica dos requisitos de segurança do parceiro verificará se a conta autenticada foi desafiada pela autenticação multifator. Em caso negativo, você será redirecionado para a página de logon e receberá uma solicitação para autenticar novamente. Se o domínio não for federado, após a autenticação bem-sucedida você será solicitado a configurar a autenticação multifator. Ao concluir essa operação, você poderá gerenciar seus clientes usando o AOBO. Se o domínio for federado, será necessário garantir que a conta está sendo desafiada pela autenticação multifator.

## <a name="key-resources"></a>Principais recursos

### <a name="how-to-get-started"></a>Como começar

- [Requisitos de segurança de parceiros: guia passo a passo](https://docs.microsoft.com/partner-center/partner-security-requirements).
- Encaminhe suas perguntas e seus comentários para este [Grupo de Orientação de Segurança do Partner Center](https://aka.ms/MPCSecurityGuidance).
- Participe dos próximos webinars e horários de escritório do parceiro. Confira [aqui informações detalhadas sobre os recursos e o cronograma](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance).

### <a name="resources-for-enabling-mfa"></a>Recursos para habilitar a MFA

- Entenda o conceito das [políticas de proteção de linha de base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection).
- Confira a [Política de linha de base: exigir MFA para administradores](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) a fim de obter detalhes sobre como habilitar essa política de linha de base.
- Confira a [Política de linha de base: proteção do usuário final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) para obter detalhes sobre como habilitar essa política de linha de base.

### <a name="resources-for-adopting-secure-application-model"></a>Recursos para adotar o Modelo de Aplicativo Seguro

- [Visão geral do Modelo de Aplicativo Seguro](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [Partner Center: guia do Modelo de Aplicativo Seguro](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Parceiros no programa CSP: código de exemplo em .NET para habilitar o Modelo de Aplicativo Seguro](https://docs.microsoft.com/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [Parceiros no programa CSP: código de exemplo em Java para habilitar o Modelo de Aplicativo Seguro](https://docs.microsoft.com/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [Documento de autenticação do Partner Center](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
- [Documento de MFA (Autenticação Multifator) do PowerShell do Partner Center](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth)

## <a name="support"></a>Suporte

### <a name="where-can-i-get-support"></a>Onde posso obter suporte?

Para obter recursos de suporte a fim de atender aos requisitos de segurança, se você tiver o ASfP (Suporte Avançado para Parceiros), entre em contato com seu Gerente de Conta de Serviço; se tiver o contrato de PSfP (Suporte Premier para Parceiros), entre em contato com o Gerente de Conta de Serviço e o Gerente de Conta Técnico.

### <a name="how-can-i-get-help-with-enabling-the-baseline-policies"></a>Como posso obter ajuda para habilitar as políticas de linha de base?

- Os parceiros podem aproveitar as horas de consultoria dos benefícios do MPN para obter orientações mais detalhadas sobre como implementar os requisitos de segurança.
- Há opções de suporte técnico de produto do Azure Active Directory disponíveis por meio dos seus benefícios do MPN. Parceiros com acesso a contratos ativos do ASfP ou do PSfP podem trabalhar com seus Gerentes de Conta associados (SAM/TAM) para entender melhor as opções disponíveis.
- O suporte para a implementação de políticas de linha de base com o Partner Center pode ser acessado por meio da [solicitação de serviço do Partner Center](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp). Selecione *MFA e Modelo de Aplicativo Seguro* como tópico.

### <a name="how-do-i-get-technical-information-and-support-to-help-me-adopt-secure-application-model-framework"></a>Como faço para obter informações técnicas e suporte para me ajudar a adotar a estrutura do Modelo de Aplicativo Seguro?

Há opções de suporte técnico de produto do Azure Active Directory disponíveis por meio dos seus benefícios do MPN. Parceiros com acesso a assinaturas ativas do ASfP ou do PSfP podem trabalhar com seus Gerentes de Conta associados (SAM/TAM) para entender melhor as opções disponíveis.

### <a name="how-do-i-contact-support-when-ive-lost-access-to-partner-center"></a>Como fazer para entrar em contato com o suporte quando eu tiver perdido o acesso ao Partner Center?

Acesse o [Suporte a Parceiros da Microsoft](https://partner.microsoft.com/support) e escolha **Mostrar todas as opções de suporte**. Você verá as opções disponíveis para entrar em contato com o Suporte a Parceiros da Microsoft. Elas incluem um número de telefone para ligar para o suporte e uma opção para entrar em contato com o suporte por chat. 

### <a name="where-can-i-find-more-information-about-technical-common-issues"></a>Onde posso encontrar mais informações sobre problemas técnicos comuns?

Informações sobre problemas técnicos comuns podem ser encontradas [aqui](https://docs.microsoft.com/partner-center/partner-security-requirements#common-issues).
