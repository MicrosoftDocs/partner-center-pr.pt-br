---
title: Relatório de status dos requisitos de segurança
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como verificar a conformidade dos requisitos de segurança com o relatório de status dos requisitos de segurança e o relatório de MFA do Partner Center
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.topic: conceptual
ms.custom: SEOMAY.20
ms.openlocfilehash: 673728ad03d6617fa60ba4119f0ebbbaaa4ce328
ms.sourcegitcommit: 98f5eebe7d08ba214ed5a078f1ac770439e41eb7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/31/2020
ms.locfileid: "93132956"
---
# <a name="security-requirements-status-report"></a>Relatório de status dos requisitos de segurança

**Aplica-se a**

- Todos os parceiros no programa Provedor de Soluções na Nuvem
- Todos os Fornecedores do Painel de Controle
- Todos os consultores

**Usuários apropriados**
- Todos os usuários habilitados, incluindo usuários convidados

Este artigo explica o relatório de status dos requisitos de segurança no Partner Center. Este relatório fornece métricas de conformidade nos [requisitos de segurança de parceiro](partner-security-requirements.md) para MFA (autenticação multifator) dos usuários no seu locatário do parceiro.

Para acessar esse relatório no [Partner Center](https://partner.microsoft.com/dashboard), acesse **Configurações** > **Configurações de parceiro** > **Status de requisitos de segurança**. O relatório é atualizado diariamente e reflete os dados de logon dos últimos sete dias.

>[!NOTE]
>O relatório de status dos requisitos de segurança é compatível apenas com o Partner Center. Ele não está disponível no Microsoft Cloud for US Government nem no Microsoft Cloud Alemanha. É altamente recomendável que todos os parceiros que negociam em uma nuvem soberana (governo dos EUA e Alemanha) adotem esses novos requisitos de segurança imediatamente. No entanto, esses parceiros não precisam atender aos novos requisitos de segurança no momento. Futuramente, a Microsoft fornecerá detalhes adicionais sobre a imposição desses requisitos de segurança para nuvens soberanas.

## <a name="security-status-metrics"></a>Métricas de status de segurança

O relatório de status de requisitos de segurança oferece insights sobre a implementação de MFA do parceiro e fornece métricas sobre a configuração de MFA e as atividades do Partner Center nos locatários do parceiro. As seções a seguir explicam essas métricas em mais detalhes.

### <a name="mfa-configuration-on-a-partner-tenant"></a>Configuração de MFA em um locatário do parceiro

A métrica **Percentual de contas de usuário habilitadas com MFA imposta usando opções listadas aqui:** mostra o percentual de contas de usuário habilitadas no seu locatário do parceiro que têm a MFA imposta. Você pode usar uma dessas [opções de MFA](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started) para obter conformidade. Esses dados são capturados e relatados diariamente. Por exemplo:

- A Contoso é um parceiro CSP com 110 contas de usuário no locatário, das quais 10 estão desabilitadas. 
- Das 100 contas de usuário restantes, 90 têm o uso de MFA imposto pelas [opções de MFA](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started) fornecidas. Portanto, a métrica mostra 90%. 

### <a name="partner-center-requests-with-mfa"></a>Solicitações do Partner Center com MFA

Cada vez que seus funcionários entram no Partner Center para trabalhar ou, por meio de APIs, obter ou enviar dados por meio do Partner Center, seu status de segurança é desafiado e acompanhado. Também estão incluídos no acompanhamento de status de segurança os seus aplicativos e todos os aplicativos de fornecedor de painel de controle. Esses dados são mostrados em métricas sob **Percentual de solicitações para o Partner Center com MFA** e refletem os últimos sete dias.

#### <a name="dashboard-mfa-verification"></a>Verificação de MFA do painel

A métrica **Por meio do portal do Partner Center** está relacionada às atividades no painel do Partner Center. Ela mede o percentual de operações realizadas por usuários que concluíram a verificação da MFA. Por exemplo:

- a Contoso é um parceiro CSP com dois agentes administradores: Jane e João.
- No primeiro dia, Jane se conectou ao Painel do Partner Center sem a verificação da MFA e fez três operações.
- No segundo dia, John se conectou ao Painel do Partner Center sem a verificação da MFA e fez cinco operações.
- No terceiro dia, Jane se conectou ao Painel do Partner Center com a verificação da MFA e fez duas operações.
- Nenhuma outra operação foi realizada pelos agentes nos quatro dias restantes.
- Das dez operações feitas na janela de sete dias, duas foram feitas pelo usuário com a verificação de MFA. Portanto, a métrica mostrará 20%.

Use o arquivo **Solicitações do portal sem MFA** para entender qual usuário fez logon no Painel do Partner Center sem ter a verificação de MFA e a hora da última visita durante a janela de relatório.

#### <a name="appuser-mfa-verification"></a>Verificação de MFA do Aplicativo + Usuário

A métrica **Por meio da API ou do SDK** está relacionada à autenticação de Aplicativo + Usuário realizada por meio de solicitações de API do Partner Center. Ela mede o percentual de solicitações de API feitas usando um token de acesso com a declaração da MFA. Por exemplo:

- a Fabrikam é um parceiro CSP e tem um aplicativo CSP que usa uma combinação de autenticação aplicativo + usuário e métodos de autenticação somente por aplicativo.
- No primeiro dia, o aplicativo fez três solicitações de API que foram apoiadas por um token de acesso obtido por meio do método de autenticação Usuário + Aplicativo, sem a verificação da MFA.
- No segundo dia, o aplicativo fez cinco solicitações de API, que foram apoiadas por um token de acesso obtido usando a autenticação somente por aplicativo.
- No terceiro dia, o aplicativo fez duas solicitações de API, que foram apoiadas por um token de acesso obtido por meio do método de autenticação Usuário + Aplicativo, com a verificação da MFA.
- Nenhuma outra operação foi realizada pelos agentes nos quatro dias restantes.
- As cinco solicitações de API no segundo dia, que foram apoiadas por um token de acesso obtido por meio da autenticação somente por aplicativo, são omitidas da métrica, pois não fazem uso de credenciais de usuário. Das cinco operações restantes, duas foram apoiadas por um token de acesso obtido com a verificação da MFA. Portanto, a métrica mostrará 40%.

Se você quiser entender quais atividades de aplicativo + usuário resultam em menos que 100% nessa métrica, use os arquivos:

- **Resumo de solicitações de API** para entender o status geral da MFA por aplicativo.
- **Todas as solicitações de API** para entender os detalhes de cada solicitação de API feita pelos usuários do seu locatário; o resultado é limitado às 10.000 solicitações mais recentes, para uma melhor experiência de download.

## <a name="actions-for-mfa-status-below-100"></a>Ações para o status de MFA abaixo de 100%

Alguns parceiros que implementaram o MFA podem ver as métricas de relatório abaixo de 100%. Para entender o porquê, aqui estão alguns fatores a serem considerados.

> [!NOTE]
> Será necessário trabalhar com alguém da sua organização que esteja familiarizado com o gerenciamento de identidades e a implementação da MFA para o seu locatário de parceiros.

### <a name="implemented-mfa-for-your-partner-tenant"></a>MFA implementada para o seu locatário do parceiro

Você precisará implementar a MFA para o seu locatário do parceiro para atingir a conformidade. Para obter detalhes sobre como implementar o MFA, confira [Requisitos de segurança para usar o Partner Center ou as APIs do Partner Center](partner-security-requirements.md).

>[!NOTE]
> As métricas de MFA são calculadas diariamente e levam em conta as operações executadas nos últimos sete dias. Se você concluiu recentemente a implementação da MFA no seu locatário do parceiro, as métricas talvez ainda não mostrem 100%.

### <a name="verify-mfa-on-all-user-accounts"></a>Verificar a MFA em todas as contas de usuário

Entenda se a sua implementação atual da MFA abrange todas as contas de usuário ou apenas algumas. Algumas soluções de MFA são baseadas em políticas e compatíveis com a exclusão de usuários, ao passo que outras podem exigir que você habilite explicitamente a MFA para cada usuário. Verifique se você não excluiu nenhum usuário da sua implementação de MFA atual. Toda conta de usuário excluída e que faça logon no Partner Center para executar qualquer atividade relacionada ao CSP, ao CPV ou ao Assistente poderá fazer com que as métricas sejam diferentes de 100%.

### <a name="review-your-mfa-conditions"></a>Examinar as condições de MFA

Entenda se a implementação atual só impõe a MFA em condições específicas. Algumas soluções de MFA fornecem a flexibilidade de impor a MFA somente quando determinadas condições são atendidas. Por exemplo, quando o usuário está acessando de um dispositivo desconhecido ou de um local desconhecido. Um usuário que está habilitado para a MFA, mas que não precisa concluir a verificação de MFA ao acessar o Partner Center poderá fazer com que as métricas sejam diferentes de 100%.

>[!NOTE]
>Para parceiros que implementaram a MFA usando os padrões de segurança do Azure AD é importante observar que para as contas de usuário não administrador, a autenticação multifator será imposta com base em risco. Os usuários deverão realizar a MFA somente durante tentativas de entrada suspeitas (por exemplo, quando o usuário estiver entrando de um local diferente). Além disso, os usuários terão até 14 dias para se registrarem para a MFA. Os usuários que não concluíram o registro da MFA não serão desafiados pela verificação de MFA durante esse período de 14 dias. Portanto, espera-se que as métricas não sejam iguais a 100% para parceiros que implementaram a MFA usando os padrões de segurança do Azure AD.

### <a name="review-third-party-mfa-configurations"></a>Examine as configurações de MFA de terceiros

Se estiver usando uma solução de MFA de terceiros, identifique como você a está integrando ao Azure AD. Em geral, há dois métodos, incluindo a federação e controles personalizados:

* **Federação de identidade** – Quando o Azure AD receber uma solicitação de autenticação, ele redirecionará o usuário para o provedor de identidade federada para autenticação. Após a autenticação bem-sucedida, o provedor de identidade federada redirecionará o usuário de volta ao Azure AD juntamente com um token SAML. Para que o Azure AD reconheça que o usuário concluiu a verificação de MFA ao autenticar no provedor de identidade federada, o token SAML deve incluir a declaração *authenticationmethodsreferences* (com o valor *multipleauthn* ). Verifique se o provedor de identidade federada é compatível com a emissão de tal declaração. Em caso afirmativo, verifique se o provedor de identidade federada foi configurado para fazer isso. Se a declaração estiver ausente, o Azure AD (e, portanto, a Central de Parceiros) não saberá que o usuário concluiu a verificação da MFA e a declaração ausente poderá fazer com que a métrica não seja igual a 100%.

* **Controle Personalizado** – O Controle Personalizado do Azure AD não pode ser usado para identificar se um usuário concluiu a verificação da MFA por meio de uma solução de MFA de terceiros. Como resultado, todo usuário que tenha concluído a verificação da MFA por meio de um controle personalizado sempre aparecerá no Azure AD (e, em seguida, no Partner Center) como se não houvesse concluído a verificação da MFA. Sempre que possível, é recomendável que você alterne para o uso da Federação de Identidade em vez do Controle Personalizado ao se integrar com o Azure AD.

### <a name="identify-which-users-have-signed-in-to-partner-center-without-mfa"></a>Identificar quais usuários entraram no Partner Center sem a MFA

Pode ser útil identificar quais usuários estão fazendo logon no Partner Center sem a verificação da MFA e verificá-los com sua implementação de MFA atual. Você poderá usar o [relatório de entrada do Azure AD](/azure/active-directory/reports-monitoring/concept-sign-ins) para descobrir se um usuário concluiu ou não a verificação da MFA. O relatório de conexão do Azure AD está disponível apenas para parceiros que se inscreveram no Azure AD Premium ou em qualquer SKU do O365, o que inclui o Azure AD Premium (por exemplo, EMS).

## <a name="next-steps"></a>Próximas etapas

- [Comunidade do grupo de diretrizes de segurança do Partner Center](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)
- [Requisitos de segurança do Partner Center](partner-security-requirements.md)
- [Perguntas Frequentes sobre os requisitos de segurança do Partner Center](partner-security-requirements-faq.md)