---
title: Perguntas frequentes sobre requisitos de segurança do parceiro | Centro de parceiros
ms.topic: article
ms.date: 07/18/2019
description: Perguntas frequentes sobre os requisitos de segurança do parceiro
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, provedor de soluções na nuvem, programa de provedor de soluções na nuvem, CSP, fornecedor do painel de controle, CPV, autenticação multifator, MFA, modelo de aplicativo seguro, modelo de aplicativo seguro, segurança
ms.localizationpriority: medium
ms.openlocfilehash: 1f2ae0f07888fdabd16b2eb476af7fac975cd71e
ms.sourcegitcommit: bae29ab191c72e15259d99c40c69a9e7c3f2b502
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/06/2019
ms.locfileid: "68820594"
---
# <a name="frequently-asked-questions-about-the-partner-security-requirements"></a>Perguntas frequentes sobre os requisitos de segurança do parceiro

Este artigo contém algumas perguntas frequentes para os [requisitos de segurança do parceiro](partner-security-requirements.md).

## <a name="partner-security-requirements"></a>Requisitos de segurança do parceiro

### <a name="what-are-the-new-partner-security-requirements"></a>Quais são os novos requisitos de segurança do parceiro?

Para proteger nossos parceiros e seus clientes, estamos exigindo que os parceiros executem as seguintes ações imediatamente:  

1. **Habilite a autenticação multifator (MFA) para todos os usuários em locatários de parceiro**. Todos os usuários em locatários de parceiros devem usar a MFA (autenticação multifator) ao entrar nos serviços de nuvem comercial da Microsoft ou para transações no CSP por meio do Partner Center ou por meio de APIs. Por meio da habilitação das políticas de proteção de linha de base, o MFA está disponível sem nenhum custo para todos os usuários de locatários parceiros.

2. **Adote a estrutura do modelo de aplicativo seguro**. Todos os parceiros que se integram com uma API da Microsoft como Azure Resource Manager, Microsoft Graph e a API do Partner Center devem adotar a estrutura do modelo de aplicativo seguro para evitar qualquer interrupção em sua integração quando as políticas de linha de base estão habilitadas. 
 
Habilitar a MFA (autenticação multifator) e adotar a estrutura de modelo de aplicativo seguro ajudará a proteger sua infraestrutura e a proteger os dados do cliente contra possíveis riscos de segurança, como identificar roubo ou outros incidentes de fraude.  

### <a name="which-partners-need-to-meet-the-requirements"></a>Quais parceiros precisam atender aos requisitos?

Esses requisitos são para os seguintes grupos de parceiros:
- Todas as organizações parceiras que participam do programa CSP (provedor de soluções na nuvem) que estão transagindo usando os serviços de nuvem comercial da Microsoft
  - Parceiros de cobrança direto
  - Provedores indiretos
  - Revendedores indiretos
- Todos os fornecedores do painel de controle
- Todos os parceiros do programa Advisor  

Todos os parceiros que transcorrem por uma nuvem do soberanas (21Vianet, governo dos EUA e Alemanha) não são necessários para atender aos novos requisitos de segurança em vigor em 1º de agosto. No entanto, é altamente recomendável que todos os parceiros que usam um ato de nuvem soberanas e adotem esses novos requisitos de segurança imediatamente. A Microsoft fornecerá detalhes adicionais sobre a imposição desses requisitos de segurança para nuvens soberanas no futuro.

### <a name="what-are-the-key-timelines-and-milestones"></a>Quais são as principais linhas do tempo e Marcos?

Os termos associados a esses requisitos de segurança serão adicionados imediatamente ao guia do programa do provedor de soluções na nuvem. Você precisará implementar esses requisitos de segurança para estar em conformidade com sua participação no programa CSP em vigor em 1º de agosto de 2019. 

### <a name="what-will-happen-if-i-do-not-take-any-actions"></a>O que acontecerá se eu não executar nenhuma ação?

Os parceiros que não obedecem a essas práticas e obrigações de segurança não poderão realizar transações no programa provedor de soluções na nuvem nem gerenciar locatários de clientes aproveitando os direitos de administrador delegado, uma vez que esses requisitos de segurança de parceiro são impostos. Estamos no processo de estabelecer uma data de imposição para os requisitos e notificaremos os parceiros da data com informações detalhadas.

### <a name="why-is-microsoft-enforcing-these-new-requirements"></a>Por que a Microsoft está impondo esses novos requisitos?
A segurança e a privacidade de clientes e parceiros são as principais prioridades da Microsoft. Continuamos a ver o maior número de ataques de segurança mais sofisticados, principalmente relacionados a incidentes de comprometimento de identidade. Como os controles preventivos desempenham um papel fundamental em uma estratégia de defesa geral para frustrar os ataques de segurança, começaremos a impor um conjunto de requisitos de segurança obrigatórios para ajudar a proteger os parceiros e seus clientes.

### <a name="does-this-apply-to-all-geographies"></a>Isso se aplica a todas as regiões geográficas?

Sim, isso se aplica a todas as geografias. É altamente recomendável que todos os parceiros transagindo por uma nuvem soberanas (21Vianet, governo dos EUA e Alemanha) atuem e adotem esses novos requisitos de segurança imediatamente. No entanto, esses parceiros não precisam atender aos novos requisitos de segurança a partir de 1º de agosto. A Microsoft fornecerá detalhes adicionais sobre a imposição desses requisitos de segurança para nuvens soberanas no futuro.

## <a name="required-actions"></a>Ações necessárias

### <a name="what-are-the-key-actions-i-need-to-take-to-meet-the-requirements"></a>Quais são as principais ações que preciso tomar para atender aos requisitos?  
Todos os parceiros no programa CSP (conta direta, provedor indireto e revendedor indireto), consultores e fornecedores do painel de controle devem atender aos requisitos.

1. **Impor MFA para todos os usuários**

    Todos os parceiros do programa CSP, consultores e fornecedores do painel de controle são obrigados a impor a MFA para todos os usuários em seu locatário de parceiro. Isso pode ser feito habilitando a [solicitação de MFA para administradores](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators), a [linha de base de proteção do usuário final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)e quaisquer políticas de linha de base futuras. A funcionalidade fornecida pelas políticas de linha de base continuará a evoluir para garantir que parceiros e clientes estejam protegidos contra ameaças de segurança em constante mudança. Portanto, é importante que você examine a [documentação das políticas de linha de base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) para saber mais.

    - Consulte [política de linha de base: Exigir MFA para administradores](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) para obter detalhes sobre como habilitar a política exigir MFA para a linha de base de administrador.
    - Consulte [política de linha de base: Proteção](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) do usuário final para obter detalhes sobre como habilitar a política de linha de base de proteção do usuário final.
    - Entenda o conceito das [políticas de proteção de linha de base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection).

    Considerações adicionais:

    - Os provedores indiretos precisam trabalhar com revendedores indiretos para carregar para o Partner Center se eles ainda não tiverem feito isso e encorajar seus revendedores a atender aos requisitos.
    - O Azure MFA está sendo disponibilizado para todos os usuários no locatário do parceiro sem custo por meio das políticas de linha de base com o único método de verificação de usar o [aplicativo Microsoft Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview).
    - Os métodos de verificação adicionais estão disponíveis por meio dos SKUs [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium) , se outros métodos, como SMS ou email, forem necessários.
    - Os parceiros também podem aproveitar uma solução de MFA de terceiros por cada usuário ao acessar os serviços de nuvem comercial da Microsoft.

2. **Adote a estrutura do modelo de aplicativo seguro**

    Todos os parceiros que desenvolveram integração personalizada usando qualquer API (como Azure Resource Manager, Microsoft Graph, API do Partner Center etc.) ou implementaram a automação personalizada usando ferramentas como o PowerShell precisarão adotar o [modelo de aplicativo seguro estrutura](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) para integração com os serviços de nuvem da Microsoft. A falha em fazer isso pode resultar em uma interrupção devido à implantação de MFA. Os recursos a seguir fornecem uma visão geral e diretrizes sobre como adotar o modelo.

    - [Visão geral do modelo de aplicativo seguro](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
    - [Centro de parceiros: Guia do modelo de aplicativo seguro](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
    - [Parceiros no programa CSP: código de exemplo .NET para habilitar o modelo de aplicativo seguro](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model)
    - [Parceiros no programa CSP: Código de exemplo de Java para habilitar o modelo de aplicativo seguro](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)
    - [Documento de autenticação do Partner Center](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
    - [Documento de autenticação multifator (MFA) do PowerShell do Partner Center](https://docs.microsoft.com/partner-center/develop/multi-factor-auth)

    Se você estiver usando um painel de controle, precisará consultar o fornecedor sobre a adoção da estrutura do modelo de aplicativo seguro.

    Os fornecedores do painel de controle são obrigados a [integrar](https://docs.microsoft.com/partner-center/enroll-as-cpv) o Partner Center como fornecedor do painel de controle e começar a implementar esse requisito imediatamente. Consulte o [Partner Center: Estrutura](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)de modelo de aplicativo seguro. Os fornecedores do painel de controle devem aceitar e gerenciar o consentimento dos parceiros CSP em vez de credenciais e limpar todas as credenciais existentes dos parceiros CSP.

## <a name="multi-factor-authentication"></a>Autenticação Multifator

### <a name="what-is-mfa"></a>O que é MFA?

A autenticação multifator (MFA) é um mecanismo de segurança no qual os indivíduos são autenticados por meio de mais de um procedimento de validação e segurança necessário. Ele funciona exigindo dois ou mais dos seguintes métodos de autenticação:

- Algo que você sabe (geralmente uma senha)
- Algo que você tem (um dispositivo confiável que não é duplicado facilmente, como um telefone)
- Algo que você é (biometria)

### <a name="what-are-baseline-protection-policies"></a>O que são políticas de proteção de linha de base? 

[Políticas de proteção de linha de base da Microsoft](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) (Atualmente visualização) são um conjunto de políticas predefinidas que ajudam a proteger as organizações contra muitos ataques comuns. Esses ataques comuns podem incluir pulverização, reprodução e phishing de senha. As políticas de linha de base estão disponíveis em todas as edições do Azure Active Directory. A Microsoft está tornando essas políticas de proteção de linha de base disponíveis para todos, pois os ataques baseados em identidade estão aumentando os últimos anos. O objetivo dessas políticas é garantir que todas as organizações tenham um nível de linha de base de segurança habilitado sem nenhum custo adicional.

> [!NOTE]
> As políticas de linha de base da Microsoft e funcionalidades relacionadas continuarão a evoluir para proteger melhor os parceiros e clientes contra ameaças de segurança em constante mudança. Pode haver algumas alterações de nomenclatura e taxonomia com as políticas de linha de base em breve. É altamente recomendável que você visite as páginas de políticas de linha de base diretamente para conferir as informações mais recentes.

### <a name="what-baseline-policies-must-i-enable"></a>Quais políticas de linha de base devo habilitar?

Se você estiver planejando utilizar as políticas de proteção de linha de base atuais para fornecer MFA para cada usuário no locatário do parceiro, será necessário habilitar a política [exigir MFA para administradores](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) e as políticas de linha de base de [proteção do usuário final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) . Essas políticas de proteção de linha de base atenderão ao requisito de MFA para cada usuário no locatário do parceiro sem custo apenas para os parceiros que estão usando aplicativos Microsoft Authenticator por meio do dispositivo móvel.

A [política exigir MFA para administradores de linha de base](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) é utilizada para usuários administrativos no diretório de parceiros, e a política de linha de base de [proteção do usuário final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) é usada para proteger usuários não administrativos no locatário do parceiro. Habilitar essas políticas exigirá que os usuários se registrem no MFA. Depois que o usuário for registrado com êxito, será solicitado que ele seja MFA durante as tentativas de entrada com base nos critérios da política. A funcionalidade fornecida pelas políticas de linha de base continuará a evoluir para garantir que parceiros e clientes estejam protegidos contra ameaças de segurança em constante mudança. Portanto, é importante que você examine a [documentação das políticas de linha de base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) para saber mais.

### <a name="how-do-i-enable-the-require-mfa-for-admins-policy"></a>Como fazer habilitar a política exigir MFA para administradores? 

A política exigir MFA para administradores de linha de base pode ser habilitada por meio do portal de gerenciamento do Azure. Consulte [política de linha de base: Exigir MFA para administradores](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) para obter detalhes sobre como habilitar essa política de linha de base.

### <a name="how-do-i-enable-the-end-user-protection-policy"></a>Como fazer habilitar a política de proteção do usuário final?

A política de linha de base de proteção do usuário final pode ser habilitada por meio do portal de gerenciamento do Azure. Consulte [política de linha de base: Proteção](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) do usuário final para obter detalhes sobre como habilitar essa política de linha de base.

### <a name="will-the-baseline-policies-be-automatically-enabled"></a>As políticas de linha de base serão habilitadas automaticamente? 

Não, para habilitar essas políticas, um usuário membro das funções administrador global, administrador de segurança ou administrador de acesso condicional precisará configurar as políticas para usar a política imediatamente.

### <a name="what-is-the-cost-of-enabling-mfa"></a>Qual é o custo de habilitar a MFA?

A Microsoft fornece MFA sem custo por meio da implementação das políticas [exigir MFA para administração](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) e [proteção do usuário final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) . A única opção de verificação disponível por meio desta versão do MFA é o [aplicativo Microsoft Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview). Se uma chamada telefônica ou uma mensagem SMS for necessária, será necessário adquirir uma licença [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium) . Como alternativa, você pode utilizar uma solução de terceiros para fornecer MFA para cada usuário em seu locatário do parceiro – nesse caso, é sua responsabilidade garantir que sua solução de MFA esteja sendo imposta e que você esteja em conformidade.

### <a name="if-i-already-have-an-mfa-solution-what-actions-do-i-need-to-take"></a>Se eu já tenho uma solução MFA, quais ações preciso tomar?

Por meio desses requisitos de segurança, os usuários em um locatário do parceiro serão solicitados a autenticar usando o MFA ao acessar os serviços de nuvem comercial da Microsoft. A solução de terceiros pode ser usada para atender a esses requisitos. A Microsoft não fornece mais testes de validação para provedores de identidade independentes para compatibilidade com Azure Active Directory. Se você quiser testar seu produto para interoperabilidade, consulte estas [diretrizes](https://www.microsoft.com/download/details.aspx?id=56843).

### <a name="what-verification-method-can-i-use-to-authenticate-mfa"></a>Qual método de verificação posso usar para autenticar a MFA?

A Microsoft fornece MFA sem custo por meio da implementação das políticas [exigir MFA para administração](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) e [proteção do usuário final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) . A única opção de verificação disponível por meio desta versão do MFA é o [aplicativo Microsoft Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview). Se uma chamada telefônica ou uma mensagem SMS for necessária, será necessário adquirir uma licença [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium) . Como alternativa, você pode utilizar uma solução de terceiros para fornecer MFA para cada usuário em seu locatário do parceiro – nesse caso, é sua responsabilidade garantir que sua solução de MFA esteja sendo imposta e que você esteja em conformidade.

### <a name="i-use-multiple-partner-tenants-to-transact-do-i-need-to-implement-mfa-on-them-all"></a>Eu uso vários locatários de parceiros para o Transact. É necessário implementar o MFA em todos eles?

Sim, você precisará impor a MFA para cada locatário de Azure Active Directory associado ao programa CSP ou ao programa Advisor. Se você planeja comprar uma licença de Azure Active Directory Premium, uma licença deve ser adquirida para o usuário em cada locatário Azure Active Directory.

### <a name="does-each-user-in-my-partner-tenant-need-to-have-mfa-enforced"></a>Cada usuário em meu locatário do parceiro precisa ter a MFA imposta? 

As políticas de proteção [exigir MFA para administração](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) e [proteção do usuário final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) impedirão a MFA para cada usuário em seu locatário do parceiro. Se você estiver aproveitando essas políticas para fornecer MFA e estiver usando o aplicativo [Microsoft Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview) , não será necessário comprar nenhuma licença adicional. Caso contrário, você precisará comprar uma solução apropriada para fornecer MFA a cada usuário em seu locatário de parceiro.

### <a name="i-am-a-direct-bill-partner-with-microsoft-what-do-i-need-to-do"></a>Sou parceiro de cobrança direto com a Microsoft. O que eu preciso fazer?

Parceiros diretos do provedor de soluções de nuvem de cobrança devem impor a MFA para cada usuário em seu locatário de parceiro.

### <a name="i-am-an-indirect-reseller-and-only-transact-though-a-distributor-do-i-still-have-to-do-this"></a>Sou um revendedor indireto e apenas transacte um distribuidor. Ainda tenho que fazer isso?

Todos os revendedores indiretos são necessários para impor a MFA para cada usuário em seu locatário de parceiro. Essa é uma ação que o revendedor indireto deve executar.

### <a name="i-do-not-use-the-partner-center-api-do-i-still-need-to-implement-mfa"></a>Eu não uso a API do Partner Center. Ainda preciso implementar a MFA?

Sim, esse requisito de segurança é para todos os usuários, incluindo usuários administradores de parceiros e usuários finais em um locatário de parceiro.

### <a name="which-third-party-vendors-provide-mfa-solutions-compatible-with-azure-active-directory"></a>Quais fornecedores de terceiros fornecem soluções de MFA compatíveis com o Azure Active Directory?

Há muitas revisões independentes de soluções de MFA online, como a [Gartner](https://www.gartner.com/en/webinars/3881781). Ao examinar fornecedores e soluções de MFA, os parceiros devem garantir que a solução escolhida seja compatível com Azure Active Directory.

A Microsoft não fornece mais testes de validação para provedores de identidade independentes para compatibilidade com Azure Active Directory. Se você quiser testar seu produto para interoperabilidade, consulte estas [diretrizes](https://www.microsoft.com/download/details.aspx?id=56843).

Para obter mais informações, consulte a [lista de compatibilidade de Federação do Azure ad](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-compatibility).

### <a name="how-can-i-test-mfa-in-our-integration-sandbox"></a>Como posso testar o MFA em nossa área restrita de integração?

As políticas de linha de base [exigir MFA para administrador](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) e [proteção do usuário final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) devem ser habilitadas para seu locatário da área restrita da integração. Por meio dessa política, cada usuário no locatário será solicitado a autenticar usando o MFA.

### <a name="will-enabling-mfa-effect-how-i-interact-with-my-customers-tenant"></a>Habilitará o efeito de MFA como eu interagir com o locatário do meu cliente? 

Não. O cumprimento desses requisitos de segurança não afetará a maneira como você gerencia seus clientes. Sua capacidade de executar operações administrativas delegadas não será interrompida.

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a>Meus clientes estão sujeitos aos requisitos de segurança do parceiro?

Não, não é necessário impor a MFA para cada usuário nos locatários do Azure AD do seu cliente. No entanto, é recomendável que você trabalhe com cada cliente para determinar a melhor maneira de proteger seus usuários.

### <a name="can-app-passwords-be-used-with-the-baseline-protection-policies"></a>As senhas de aplicativo podem ser usadas com as políticas de proteção de linha de base?

Sim, [as senhas de aplicativo](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) podem ser usadas. Você deve examinar as considerações para usar senhas de aplicativo documentadas [aqui](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) para determinar se há suporte para sua necessidade.

### <a name="can-any-user-be-excluded-from-this-requirement"></a>Qualquer usuário pode ser excluído deste requisito? 

Não, cada usuário, incluindo contas de serviço, no seu locatário do parceiro será solicitado a autenticar usando o MFA.

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a>Os requisitos de segurança do parceiro se aplicam à área restrita da integração?

Sim, os requisitos de segurança do parceiro se aplicam à área restrita da integração. Isso significa que você precisará implementar a solução MFA apropriada para usuários no locatário da área restrita da integração. É recomendável que você implemente as políticas de proteção de linha de base para fornecer MFA.

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a>Como fazer configurar uma conta de acesso de emergência (interrupção)?

Ele considerou a prática recomendada criar uma ou duas contas de acesso de emergência para evitar o bloqueio inadvertidamente do seu locatário do Azure AD. Em relação aos requisitos de segurança do parceiro, é necessário que cada usuário seja autenticado usando o MFA. Portanto, isso significa que você precisará modificar a definição de uma conta de acesso de emergência. Pode ser uma conta que esteja aproveitando uma solução de terceiros para MFA.

### <a name="how-will-guest-users-be-impacted-by-the-partner-security-requirements"></a>Como os usuários convidados serão afetados pelos requisitos de segurança do parceiro?

Os usuários convidados serão solicitados a autenticar-se usando o MFA, ao acessar recursos no seu locatário do parceiro. Os requisitos de segurança do parceiro não terão impacto sobre o usuário convidado que acessará os recursos em seu próprio locatário.

### <a name="if-i-am-using-a-third-party-solution-is-active-directory-federation-service-adfs-required"></a>Se eu estiver usando uma solução de terceiros, o ADFS (Active Directory Serviço de Federação) será necessário? 

Não, não é necessário ter Active Directory Serviço de Federação (ADFS) se você estiver usando uma solução de terceiros. É recomendável que você trabalhe com o fornecedor da solução para determinar quais são os requisitos para sua solução.

### <a name="is-it-a-requirement-to-enable-the-baseline-protection-policies"></a>É um requisito para habilitar as políticas de proteção de linha de base?

Não, não é necessário que você habilite as políticas de proteção de linha de base. O único requisito é que você aplique a MFA para cada usuário, incluindo contas de serviço, em seu locatário de parceiro.

### <a name="can-conditional-access-be-used-to-meet-the-mfa-requirement"></a>O acesso condicional pode ser usado para atender ao requisito de MFA?

Sim, você pode usar o acesso condicional para impor a MFA para cada usuário, incluindo contas de serviço, em seu locatário de parceiro. No entanto, considerando a natureza altamente privilegiada de ser um parceiro, precisamos garantir que cada usuário tenha um desafio de MFA para cada autenticação única. Isso significa que você não poderá aproveitar o recurso de acesso condicional que contorne o requisito para MFA.

### <a name="what-verification-options-are-provided-through-the-implementation-of-the-baseline-protection-policies"></a>Quais opções de verificação são fornecidas por meio da implementação das políticas de proteção de linha de base? 

Em relação à versão do MFA que está disponível por meio da implementação das políticas de proteção de linha de base, a única opção de verificação disponível é um aplicativo autenticador. O uso de uma chamada telefônica e mensagem de mensagem de texto é considerado menos seguro. Portanto, essas opções não estão disponíveis por meio desta versão do MFA.

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>A conta de serviço usada pelo Azure AD Connect ser afetada pelos requisitos de segurança do parceiro?

Não, a conta de serviço usada pelo Azure AD Connect não será afetada pelos requisitos de segurança do parceiro. Se você tiver um problema com Azure AD Connect como resultado da imposição da MFA, abra uma solicitação de suporte técnico com o suporte da Microsoft.

## <a name="secure-application-model"></a>Proteger o modelo de aplicativo

### <a name="who-should-adopt-the-secure-application-model-to-meet-the-requirements"></a>Quem deve adotar o modelo de aplicativo seguro para atender aos requisitos?

A Microsoft está introduzindo uma estrutura segura e escalonável para autenticar parceiros do CSP (provedor de soluções de nuvem) e CPV (fornecedores do painel de controle) que aproveitam a autenticação multifator. Consulte o [Guia do modelo de aplicativo seguro](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) para obter mais informações. Todos os parceiros que desenvolveram integração personalizada usando qualquer API (como Azure Resource Manager, Microsoft Graph, API do Partner Center etc.) ou implementaram a automação personalizada usando ferramentas como o PowerShell precisarão adotar o [modelo de aplicativo seguro estrutura](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) para integração com os serviços de nuvem da Microsoft.

### <a name="what-is-the-secure-application-model"></a>O que é o modelo de aplicativo seguro?

A Microsoft está introduzindo uma estrutura segura e escalonável para autenticar parceiros do CSP (provedor de soluções de nuvem) e CPV (fornecedores do painel de controle) que aproveitam a autenticação multifator. Consulte o [Guia do modelo de aplicativo seguro](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) para obter mais informações.  

### <a name="how-do-i-implement-the-secure-application-model"></a>Como fazer implementar o modelo de aplicativo seguro?

Todos os parceiros que desenvolveram integração personalizada usando qualquer API (como Azure Resource Manager, Microsoft Graph, API do Partner Center etc.) ou implementaram a automação personalizada usando ferramentas como o PowerShell precisarão adotar o [modelo de aplicativo seguro estrutura](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) para integração com os serviços de nuvem da Microsoft. A falha em fazer isso pode resultar em uma interrupção devido à implantação de MFA. Os recursos a seguir fornecem uma visão geral e diretrizes sobre como adotar o modelo.

- [Visão geral do modelo de aplicativo seguro](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [Centro de parceiros: Guia do modelo de aplicativo seguro](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Parceiros no programa CSP: código de exemplo .NET para habilitar o modelo de aplicativo seguro](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model)
- [Parceiros no programa CSP: Código de exemplo de Java para habilitar o modelo de aplicativo seguro](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)
- [Documento de autenticação do Partner Center](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
- [Documento de autenticação multifator (MFA) do PowerShell do Partner Center](https://docs.microsoft.com/partner-center/develop/multi-factor-auth)

Se você estiver usando um painel de controle, precisará consultar o fornecedor sobre a adoção da estrutura do modelo de aplicativo seguro.

Os fornecedores do painel de controle são obrigados a [integrar](https://docs.microsoft.com/partner-center/enroll-as-cpv) o Partner Center como fornecedor do painel de controle e começar a implementar esse requisito imediatamente. Consulte o [Partner Center: Estrutura](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)de modelo de aplicativo seguro. Os fornecedores do painel de controle devem aceitar e gerenciar o consentimento dos parceiros CSP em vez de credenciais e limpar todas as credenciais existentes dos parceiros CSP.

### <a name="who-is-a-control-panel-vendor-cpv"></a>Quem é um fornecedor do painel de controle (CPV)? 
Um fornecedor do painel de controle é um fornecedor de software independente que desenvolve aplicativos para uso por parceiros do CSP para integração com as APIs do Partner Center. Um fornecedor do painel de controle não é um parceiro CSP com acesso direto ao painel ou às APIs do Partner Center. Uma descrição detalhada está disponível no [Partner Center: Guia](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)de modelo de aplicativos seguros.

### <a name="does-the-secure-application-model-need-to-be-implemented-for-the-partner-center-apisdk-only"></a>O modelo de aplicativo seguro precisa ser implementado somente para a API/SDK do Partner Center? 

Quando as políticas de linha de base *exigir MFA para administradores* e *proteção do usuário final* estiverem habilitadas, cada usuário será solicitado a autenticar usando a autenticação multifator. Isso significa que você precisará implementar o modelo de aplicativo seguro para cada API, CLI e módulo do PowerShell (por exemplo, Azure, Azure AD, MS online, Partner Center, etc.) que se destina a executar de forma não interativa e que dependa do uso de credenciais do usuário para autenticação.

### <a name="i-am-using-automation-tools-such-as-powershell-how-do-i-implement-the-secure-application-model"></a>Estou usando ferramentas de automação, como o PowerShell. Como fazer implementar o modelo de aplicativo seguro?  

Se a sua automação for destinada a ser executada de forma não interativa e depender de credenciais do usuário para autenticação, você precisará implementar o modelo de aplicativo seguro. Consulte [proteger o modelo de aplicativo | Partner Center PowerShell](https://docs.microsoft.com/powershell/partnercenter/secure-app-model?view=partnercenterps-1.5) para obter orientação sobre como implementar essa estrutura.  Observe que nem todas as ferramentas de automação fornecem a capacidade de autenticar usando tokens de acesso. Se você precisar de ajuda para entender quais alterações precisam ser feitas, poste uma mensagem no grupo de [diretrizes de segurança do Partner Center](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) .

### <a name="what-user-credentials-should-the-application-administrator-provide-when-performing-the-consent-process"></a>Quais credenciais de usuário o administrador de aplicativos deve fornecer ao executar o processo de consentimento? 

É recomendável que você use uma conta de serviço que tenha sido atribuída a permissões menos privilegiadas. Em relação à API do Partner Center, isso significa que você deve usar uma conta que tenha sido atribuída à função agente de vendas ou agentes de administração.

### <a name="why-should-the-application-administrator-not-provide-global-admin-user-credentials-when-performing-the-consent-process"></a>Por que o administrador do aplicativo deve não fornecer credenciais de usuário de administrador global ao executar o processo de consentimento?

É recomendável usar o menos privilegiado identifica como você está reduzindo o risco. Não é recomendável usar uma conta que tenha privilégios de administrador global, pois isso forneceria mais permissões do que o necessário

### <a name="i-am-a-csp-partner-how-do-i-know-if-my-control-panel-vendor-cpv-is-working-on-implementing-the-solution-or-not"></a>Sou um parceiro CSP. Como fazer saber se o meu fornecedor do painel de controle (CPV) está trabalhando para implementar a solução ou não? 

Para parceiros que usam uma solução de fornecedor do painel de controle (CPV) para o Transact no programa CSP (provedor de soluções na nuvem), é sua responsabilidade consultar seu CPV. 

### <a name="i-am-a-cpv-how-do-i-enroll"></a>Sou um CPV. Como fazer registrar? 

Para registrar-se como um fornecedor do painel de controle (CPV), siga as diretrizes fornecidas [aqui](https://docs.microsoft.com/partner-center/enroll-as-cpv).

Para receber o link de registro, o CPVs deve contatar [CPVHelp@microsoft.com](mailto:CPVHelp@microsoft.com) e fornecer um patrocinador de funcionário da Microsoft que tenha uma relação comercial com o CPV ou conheça seus negócios. Por exemplo, um gerente de desenvolvimento de parceiros (PDM).

Depois de se registrar no Partner Center e registrar seus aplicativos, você terá acesso às APIs do Partner Center. Se você for um novo CPV, receberá suas informações de área restrita por meio de uma notificação do Partner Center. Depois de concluir o registro como um Microsoft CPV e aceito o contrato CPV, você pode:

1. Gerenciar aplicativo multilocatário (adicionar aplicativos para portal do Azure, registrar e cancelar o registro de aplicativos no Partner Center). Observação: CPVs deve registrar seus aplicativos no Partner Center para ser autorizado para APIs do Partner Center. Adicionar aplicativos ao portal do Azure sozinho não autoriza aplicativos CPV para APIs do Partner Center.
2. Exiba e gerencie seu perfil do CPV.
3. Exiba e gerencie seus usuários que precisam de acesso aos recursos do CPV. A única função que um CPV pode ter é administrador global.

### <a name="i-am-using-the-partner-center-sdk-will-sdk-automatically-adopt-the-secure-application-model"></a>Estou usando o SDK do Partner Center. O SDK adotará automaticamente o modelo de aplicativo seguro? 

Não, você precisará seguir as diretrizes fornecidas no guia do [modelo de aplicativo seguro](http://assetsprod.microsoft.com/secure-application-model-guide.pdf).

### <a name="can-i-generate-a-refresh-token-for-the-secure-application-model-with-accounts-that-do-not-have-mfa-enabled"></a>Posso gerar um token de atualização para o modelo de aplicativo seguro com contas que não têm a MFA habilitada?

Sim, um token de atualização pode ser gerado usando uma conta que não tem a MFA imposta. No entanto, isso não deve ser feito porque qualquer token gerado usando uma conta que não tenha a MFA habilitada não será capaz de acessar recursos devido ao requisito de MFA.

### <a name="how-should-my-application-obtain-an-access-token-if-we-enable-mfa"></a>Como o meu aplicativo deve obter um token de acesso se habilitarmos a MFA?

Você precisará seguir o [Guia do modelo de aplicativo seguro](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) , que fornece detalhes sobre como fazer isso enquanto estiver em conformidade com os novos requisitos de segurança. Você pode encontrar o código de exemplo .NET [aqui](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model) e o código de exemplo Java [aqui](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model).

### <a name="as-a-cpv-do-i-create-an-azure-ad-application-in-our-cpv-tenant-or-the-tenant-of-the-csp-partner"></a>Como um CPV, crio um aplicativo do Azure AD em nosso locatário do CPV ou o locatário do parceiro CSP?

O CPV precisará criar o aplicativo Azure Active Directory no locatário associado ao seu registro como um CPV.

### <a name="i-am-a-csp-that-is-using-app-only-authentication-do-i-need-to-make-any-changes"></a>Sou um CSP que está usando a autenticação somente do aplicativo. É necessário fazer alterações?

A autenticação somente do aplicativo não é afetada, pois as credenciais do usuário não estão sendo usadas para solicitar um token de acesso. Se as credenciais do usuário estiverem sendo compartilhadas, os fornecedores do painel de controle (CPVs) deverão adotar a [estrutura do modelo de aplicativo seguro](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) e limpar as credenciais de parceiro existentes.

### <a name="as-a-cpv-can-i-leverage-the-app-only-authentication-style-to-get-access-tokens"></a>Como um CPV, posso aproveitar o estilo de autenticação somente do aplicativo para obter tokens de acesso?

Não, os parceiros do fornecedor do painel de controle não podem utilizar o estilo de autenticação somente do aplicativo para solicitar tokens de acesso em nome do parceiro. Eles devem implementar o modelo de aplicativo seguro, que utiliza o estilo de autenticação do aplicativo + usuário.

## <a name="key-resources"></a>Recursos principais

### <a name="how-to-get-started"></a>Como começar

- [Requisitos de segurança do parceiro: guia passo a passo](https://docs.microsoft.com/partner-center/partner-security-requirements).
- Encaminhe suas perguntas e seus comentários para este [grupo de diretrizes de segurança do Partner Center](https://aka.ms/MPCSecurityGuidance).
- Participe do horário do futuro do parceiro e webinars. Verifique a [agenda e os recursos detalhados aqui](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance).

### <a name="resources-for-enabling-mfa"></a>Recursos para habilitar o MFA

- Entenda o conceito das [políticas de proteção de linha de base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection).
- Consulte [política de linha de base: Exigir MFA para administradores](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) para obter detalhes sobre como habilitar a política exigir MFA para a linha de base de administrador.
- Consulte [política de linha de base: Proteção](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) do usuário final para obter detalhes sobre como habilitar a política de linha de base de proteção do usuário final.

### <a name="resources-for-adopting-secure-application-model"></a>Recursos para adotar o modelo de aplicativo seguro

- [Visão geral do modelo de aplicativo seguro](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [Centro de parceiros: Guia do modelo de aplicativo seguro](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Parceiros no programa CSP: código de exemplo .NET para habilitar o modelo de aplicativo seguro](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model)
- [Parceiros no programa CSP: Código de exemplo de Java para habilitar o modelo de aplicativo seguro](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)
- [Documento de autenticação do Partner Center](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
- [Documento de autenticação multifator (MFA) do PowerShell do Partner Center](https://docs.microsoft.com/partner-center/develop/multi-factor-auth)

## <a name="support"></a>Suporte

### <a name="where-can-i-ask-get-support"></a>Onde posso pedir suporte a Get?

Além disso, para obter suporte para o aproveitamento de recursos para atender aos requisitos de segurança, se você tiver ASfP (suporte avançado para parceiros), entre em contato com seu gerente de conta de serviço; para o contrato de Suporte Premier para parceiros (PSfP), contate o gerente de conta de serviço e o gerente técnico de conta.

### <a name="how-can-i-get-help-with-enabling-the-baseline-policies"></a>Como posso obter ajuda para habilitar as políticas de linha de base?

- Os parceiros podem aproveitar as horas de consultoria dos benefícios do MPN para obter diretrizes mais detalhadas sobre como implementar os requisitos de segurança.
- As opções de suporte técnico de produto para Azure Active Directory estão disponíveis por meio de seus benefícios do MPN. Os parceiros com acesso a contratos ativos ASfP ou PSfP podem trabalhar com seu Gerenciador de contas associado (SAM/TAM) para entender melhor as opções disponíveis.
- O suporte para implementação de políticas de linha de base com o Partner Center pode ser acessado via [solicitação de serviço do Partner Center](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp). Selecione *MFA & modelo de aplicativo seguro* como o tópico.

### <a name="how-do-i-get-technical-information-to-adopt-secure-application-model-framework"></a>Como fazer obter informações técnicas para adotar a estrutura do modelo de aplicativo seguro? 

As opções de suporte técnico de produto para Azure Active Directory estão disponíveis por meio de seus benefícios do MPN. Os parceiros com acesso a uma assinatura ativa do ASfP ou do PSfP podem trabalhar com seu Gerenciador de contas associado (SAM/TAM) para entender melhor as opções disponíveis.

### <a name="where-can-i-find-more-information-about-technical-common-issues"></a>Onde posso encontrar mais informações sobre problemas técnicos comuns? 

Informações sobre os problemas técnicos comuns podem ser encontradas [aqui](https://docs.microsoft.com/partner-center/partner-security-requirements#common-issues).
