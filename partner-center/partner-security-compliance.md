---
title: Status dos requisitos de segurança do parceiro
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Conheça os requisitos obrigatórios que aumentam a segurança para Consultores, Fornecedores do Painel de Controle e parceiros no programa de Provedor de Soluções na Nuvem.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.topic: conceptual
ms.custom: SEOMAY.20
ms.openlocfilehash: 79fd61827f64a060da2b1ecd8f7eeceedb2fcdc5
ms.sourcegitcommit: 5f31146f50e01dc4c1922e0a5bc369f0a3cd8162
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/01/2020
ms.locfileid: "89220194"
---
# <a name="partner-security-requirements-status---get-answers-and-check-reports-about-current-status"></a>Status de requisitos de segurança do parceiro – obter respostas e verificar os relatórios sobre o status atual

**Aplica-se a**

- Todos os parceiros no programa Provedor de Soluções na Nuvem
  - Fatura direta
  - Provedor indireto
  - Revendedor indireto
- Todos os Fornecedores do Painel de Controle
- Todos os consultores

**Usuários apropriados**
- Todos os usuários habilitados, incluindo usuários convidados

As maiores proteções de privacidade e segurança estão entre nossas principais prioridades. Sabemos que a melhor defesa é a prevenção e que somos tão fortes quanto nosso vínculo mais fraco. É por isso que precisamos de todos em nosso ecossistema, para agir e garantir que eles tenham proteções de segurança adequadas implantadas. Para ajudar a proteger parceiros e clientes, estamos introduzindo um conjunto de requisitos de segurança obrigatórios para consultores, fornecedores do painel de controle e parceiros que participam do programa de Provedor de Soluções na Nuvem.

A partir de 1º de agosto de 2019, todos os parceiros são obrigados a impor a autenticação multifator a todos os usuários, incluindo as contas de serviço, em seu locatário de parceiro. Para obter informações mais detalhadas sobre as novas políticas de segurança, leia [Requisitos de Segurança do Parceiro](partner-security-requirements.md).

Queremos garantir que cada usuário tenha um desafio de MFA para toda autenticação única. Para que isso seja alcançado, devemos adotar uma das seguintes opções:

- Implementar o Azure AD Premium e garantir que a MFA seja imposta para cada usuário
- Implementar os [padrões de segurança do Azure AD](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)
- Implementar uma solução de terceiros para garantir que a MFA seja imposta para cada usuário

## <a name="partner-security-requirements-status"></a>Status dos requisitos de segurança do parceiro

Este relatório pode ajudá-lo a verificar o status dos requisitos de segurança, fornecendo uma maneira de enxergar claramente os pontos a serem melhorados. O acompanhamento é atualizado regularmente.

>[!NOTE]
>O relatório de status dos requisitos de segurança do parceiro é compatível apenas com o Partner Center. Ele não está disponível no Microsoft Cloud for US Government nem no Microsoft Cloud Alemanha. É altamente recomendável que todos os parceiros que negociam em uma nuvem soberana (21Vianet, governo dos EUA e Alemanha) adotem esses novos requisitos de segurança imediatamente. No entanto, esses parceiros não precisam atender aos novos requisitos de segurança em vigor em 1º de agosto de 2019. Futuramente, a Microsoft fornecerá detalhes adicionais sobre a imposição desses requisitos de segurança para nuvens soberanas.

## <a name="multi-factor-authentication-mfa-report"></a>Relatório de MFA (autenticação multifator)

O relatório de MFA do Partner Center oferece insights sobre a implementação de MFA do parceiro ao fornecer dois tipos de métricas com base na configuração de MFA e nas atividades do Partner Center do locatário de CSP: 

### <a name="mfa-configuration-on-a-csp-tenant"></a>Configuração de MFA em um locatário de CSP

Essa métrica está relacionada à configuração de MFA em um locatário de CSP que é capturado e relatado diariamente. Ele mede o percentual de contas de usuário habilitadas com a MFA imposta usando qualquer uma das [opções de MFA](https://aka.ms/partner-mfa-get-started). Por exemplo:

- A Contoso é um parceiro CSP com 110 contas de usuário no locatário, das quais 10 estão desabilitadas. 
- Das 100 contas de usuário restantes, 90 têm o uso de MFA imposto pelas [opções de MFA](https://aka.ms/partner-mfa-get-started) fornecidas. Portanto, a métrica mostra 90%. 

### <a name="partner-center-activities-with-mfa"></a>Atividades do Partner Center com MFA

Cada vez que seus funcionários entram no Partner Center para trabalhar ou, por meio de APIs, obter ou enviar dados por meio do Partner Center, seu status de segurança é desafiado e acompanhado. Também estão incluídos no acompanhamento de status de segurança os seus aplicativos e todos os aplicativos de fornecedor do painel de controle. O status exibido é referente aos sete dias anteriores.

#### <a name="mfa-verification-completed-by-users"></a>Verificação de MFA concluída pelos usuários

Essa métrica está relacionada às atividades no Painel do Partner Center. Ela mede o percentual de operações realizadas por usuários que concluíram a verificação da MFA. Por exemplo:

- a Contoso é um parceiro CSP com dois agentes administradores: Jane e João.
- No primeiro dia, Jane se conectou ao Painel do Partner Center sem a verificação da MFA e fez três operações.
- No segundo dia, John se conectou ao Painel do Partner Center sem a verificação da MFA e fez cinco operações.
- No terceiro dia, Jane se conectou ao Painel do Partner Center com a verificação da MFA e fez duas operações.
- Nenhuma outra operação foi realizada pelos agentes nos quatro dias restantes.
- Das dez operações feitas na janela de sete dias, duas foram feitas pelo usuário com a verificação de MFA. Portanto, a métrica mostrará 20%.

Use o arquivo **Solicitações do portal sem MFA** para entender qual usuário fez logon no Painel do Partner Center sem ter a verificação de MFA e a hora da última visita durante a janela de relatório.

#### <a name="appuser-authentication"></a>Autenticação aplicativo + usuário

Essa métrica está relacionada ao uso de solicitações de API do Partner Center feitas usando a Autenticação aplicativo + usuário. Ela mede o percentual de solicitações de API feitas usando um token de acesso com a declaração da MFA. Por exemplo:

- a Fabrikam é um parceiro CSP e tem um aplicativo CSP que usa uma combinação de autenticação aplicativo + usuário e métodos de autenticação somente por aplicativo.
- No primeiro dia, o aplicativo fez três solicitações de API que foram apoiadas por um token de acesso obtido por meio do método de autenticação Usuário + Aplicativo, sem a verificação da MFA.
- No segundo dia, o aplicativo fez cinco solicitações de API, que foram apoiadas por um token de acesso obtido usando a autenticação somente por aplicativo.
- No terceiro dia, o aplicativo fez duas solicitações de API, que foram apoiadas por um token de acesso obtido por meio do método de autenticação Usuário + Aplicativo, com a verificação da MFA.
- Nenhuma outra operação foi realizada pelos agentes nos quatro dias restantes.
- As cinco solicitações de API no segundo dia, que foram apoiadas por um token de acesso obtido por meio da autenticação somente por aplicativo, são omitidas da métrica, pois não fazem uso de credenciais de usuário. Das cinco operações restantes, duas foram apoiadas por um token de acesso obtido com a verificação da MFA. Portanto, a métrica mostrará 40%.

Se você quiser entender quais atividades de aplicativo + usuário resultam em menos que 100% nessa métrica, use os arquivos:

- **Resumo de solicitações de API** para entender o status geral da MFA por aplicativo.
- **Todas as solicitações de API** para entender os detalhes de cada solicitação de API feita pelos usuários do seu locatário; o resultado é limitado às 10.000 solicitações mais recentes, para uma melhor experiência de download.

## <a name="what-should-i-do-if-the-metrics-under-mfa-report-arent-100"></a>O que devo fazer se as métricas do relatório da MFA não forem iguais a 100%

É possível que as métricas do relatório da MFA do Partner Center não sejam iguais a 100% para parceiros que implementaram a MFA. Para entender o porquê, aqui estão alguns fatores a serem considerados.

> [!NOTE]
> Será necessário trabalhar com alguém da sua organização que esteja familiarizado com o gerenciamento de identidades e a implementação da MFA para o seu locatário de parceiros.

### <a name="have-you-implemented-mfa-for-your-partner-tenant"></a>Você implementou a MFA para o seu locatário de parceiros?

Caso contrário, primeiro você precisará implementar a MFA para o seu locatário de parceiros. Para obter detalhes sobre como implementar a MFA, consulte o artigo [Requisitos de Segurança do Parceiro](partner-security-requirements.md).

### <a name="have-you-only-recently-completed-mfa-implementation"></a>Você concluiu recentemente a implementação da MFA?

As métricas são calculadas diariamente e levam em conta as operações executadas nos últimos sete dias. Se você concluiu recentemente a implementação da MFA para o seu locatário de parceiros, as métricas podem não ser iguais a 100%.

### <a name="have-some-user-accounts-been-excluded-from-mfa-implementation"></a>Algumas contas de usuário foram excluídas da implementação da MFA?

Entenda se a sua implementação atual da MFA abrange todas as contas de usuário ou apenas algumas. Algumas soluções de MFA são baseadas em políticas e compatíveis com a exclusão de usuários, ao passo que outras podem exigir que você habilite explicitamente a MFA para cada usuário. Verifique se você não excluiu nenhum usuário da sua implementação de MFA atual. Toda conta de usuário excluída e que faça logon no Partner Center para executar qualquer atividade relacionada ao CSP poderá fazer com que as métricas sejam diferentes de 100%.

### <a name="is-mfa-only-required-when-certain-conditions-are-met"></a>A MFA é necessária somente quando determinadas condições são atendidas?

Entenda se a implementação atual só impõe a MFA em condições específicas. Algumas soluções de MFA fornecem a flexibilidade de impor a MFA somente quando determinadas condições são atendidas. Por exemplo, quando o usuário está acessando de um dispositivo desconhecido ou de um local desconhecido. Um usuário que está habilitado para a MFA, mas que não precisa concluir a verificação de MFA ao acessar o Partner Center poderá fazer com que as métricas sejam diferentes de 100%.

>[!NOTE]
>Para parceiros que implementaram a MFA usando os padrões de segurança do Azure AD é importante observar que para as contas de usuário não administrador, a autenticação multifator será imposta com base em risco. Os usuários deverão realizar a MFA somente durante tentativas de entrada suspeitas (por exemplo, quando o usuário estiver entrando de um local diferente). Além disso, os usuários terão até 14 dias para se registrarem para a MFA. Os usuários que não concluíram o registro da MFA não serão desafiados pela verificação de MFA durante esse período de 14 dias. Portanto, espera-se que as métricas não sejam iguais a 100% para parceiros que implementaram a MFA usando os padrões de segurança do Azure AD.

### <a name="are-you-using-third-party-mfa-solution"></a>Você está usando uma solução de MFA de terceiros?

Se estiver usando uma solução de MFA de terceiros, identifique como você a está integrando ao Azure AD. Em geral, há dois métodos, incluindo a federação e controles personalizados:

* **Federação de identidade** – Quando o Azure AD receber uma solicitação de autenticação, ele redirecionará o usuário para o provedor de identidade federada para autenticação. Após a autenticação bem-sucedida, o provedor de identidade federada redirecionará o usuário de volta ao Azure AD juntamente com um token SAML. Para que o Azure AD reconheça que o usuário concluiu a verificação de MFA ao autenticar no provedor de identidade federada, o token SAML deve incluir a declaração *authenticationmethodsreferences* (com o valor *multipleauthn*). Verifique se o provedor de identidade federada é compatível com a emissão de tal declaração. Em caso afirmativo, verifique se o provedor de identidade federada foi configurado para fazer isso. Se a declaração estiver ausente, o Azure AD (e, portanto, a Central de Parceiros) não saberá que o usuário concluiu a verificação da MFA e a declaração ausente poderá fazer com que a métrica não seja igual a 100%.

* **Controle Personalizado** – O Controle Personalizado do Azure AD não pode ser usado para identificar se um usuário concluiu a verificação da MFA por meio de uma solução de MFA de terceiros. Como resultado, todo usuário que tenha concluído a verificação da MFA por meio de um controle personalizado sempre aparecerá no Azure AD (e, em seguida, no Partner Center) como se não houvesse concluído a verificação da MFA. Sempre que possível, é recomendável que você alterne para o uso da Federação de Identidade em vez do Controle Personalizado ao se integrar com o Azure AD.

### <a name="identify-which-users-have-logged-into-partner-center-without-mfa"></a>Identificar quais usuários fizeram logon no Partner Center sem a MFA

Pode ser útil identificar quais usuários estão fazendo logon no Partner Center sem a verificação da MFA e verificá-los com sua implementação de MFA atual. Você poderá usar o [relatório de entrada do Azure AD](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins) para descobrir se um usuário concluiu ou não a verificação da MFA. O relatório de conexão do Azure AD está disponível apenas para parceiros que se inscreveram no Azure AD Premium ou em qualquer SKU do O365, o que inclui o Azure AD Premium (por exemplo, EMS).

## <a name="next-steps"></a>Próximas etapas

- [Comunidade do grupo de diretrizes de segurança do Partner Center](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)
- [Requisitos de segurança do Partner Center](partner-security-requirements.md)
- [Perguntas Frequentes sobre os requisitos de segurança do Partner Center](partner-security-requirements-faq.md)
