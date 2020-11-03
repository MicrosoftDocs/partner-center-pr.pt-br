---
title: Exigir MFA de seu locatário parceiro
ms.topic: article
ms.date: 10/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como obrigar a MFA para seus locatários parceiros ajudará a proteger o acesso aos recursos do cliente. Inclui cenários de exemplo.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 01122e81254a8e63f9bbf8d6bc3d3271accac74a
ms.sourcegitcommit: 2847efac28d3bff24ed37cdfaa88ff4be06705c8
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/27/2020
ms.locfileid: "92680410"
---
# <a name="mandating-multi-factor-authentication-mfa-for-your-partner-tenant"></a>Obrigar a MFA (Autenticação Multifator) para seu locatário parceiro

**Aplica-se a**

- Todos os parceiros no programa Provedor de Soluções na Nuvem
  - Fatura direta
  - Provedor indireto
  - Revendedor indireto
- Todos os consultores

**Funções afetadas**

- Agente administrativo
- Agente de vendas
- Agente de suporte técnico
- Administrador de cobrança
- Administrador global

A intenção desse recurso é ajudar os parceiros a proteger o acesso aos recursos do cliente contra o comprometimento das credenciais.
Os parceiros são obrigados a impor a MFA (Autenticação Multifator) a todas as contas de usuário nos respectivos locatários de parceiro, incluindo o usuário convidado. Com esse recurso, essas funções de parceiros serão obrigadas a concluir a verificação da MFA nas seguintes áreas:

- [Painel do Partner Center](#partner-center-dashboard)
- [API do Partner Center](#partner-center-api)
- [Administração Delegada do Parceiro](#partner-delegated-administration)

Garantias de segurança e privacidade maiores e contínuas estão entre as nossas principais prioridades, e continuamos ajudando os parceiros a proteger os clientes e os locatários. Todos os parceiros que participam do programa CSP (Provedor de Soluções na Nuvem), CPVs (fornecedores de painel de controle) e consultores devem implementar os [Requisitos de segurança do parceiro](partner-security-requirements.md) para manter a conformidade.

A fim de ajudar os parceiros a proteger os negócios e os clientes contra incidentes relacionados ao roubo de identidade, ativamos as proteções de segurança adicionais para locatários de parceiro que podem ajudar os parceiros a garantir o uso pelos locatários e pelos clientes, obrigando a verificação da MFA (autenticação multifator) para impedir o acesso não autorizado. 

Esta documentação fornece aos parceiros experiência e diretrizes detalhadas sobre a ativação de garantias de segurança.

## <a name="partner-center-dashboard"></a>Painel do Partner Center

Determinadas páginas no painel do Partner Center serão protegidas por MFA, incluindo:

- Todas as páginas na guia **Clientes** , por exemplo, todas as páginas que podem ser acessadas por meio da seguinte URL: https://partner.microsoft.com/commerce/*
- Todas as páginas na guia **Suporte > Solicitações do cliente** , por exemplo, a página acessada em https://partner.microsoft.com/dashboard/support/csp/customers/*
- Página de cobrança

Se você tentar acessar qualquer uma dessas páginas e não tiver concluído a verificação de MFA anteriormente, você precisará fazer isso.

> [!NOTE]
> Outras páginas da Central de Parceiros, como Visão Geral e Verificação do Status de Integridade do Serviço, não serão protegidas por MFA.

Os tipos de usuários a seguir estão autorizados a acessar estas páginas protegidas por MFA e, portanto, são afetados por esse recurso


| Páginas protegidas por MFA       | Agentes administrativos      |  Agente de vendas     |   Agentes de assistência técnica     | Administrador global      |  Administrador de cobrança     | 
|---    |---    |---    |---    |---    |---    |
| Todas as páginas na guia Clientes      |   x    |    x   |  x     |       |       |
| Todas as páginas na guia Suporte > Solicitações do cliente     | x      |       |    x   |       |       |
| Página de cobrança     |   x    |       |       |    x   |   x    |

## <a name="examples-showing-how-verification-works"></a>Exemplos mostrando como a verificação funciona

Para ilustrar como a verificação funciona, considere os dois exemplos a seguir.

### <a name="example-1-partner-has-implemented-azure-ad-mfa"></a>Exemplo 1: o parceiro implementou o Azure AD MFA

1. Jane trabalha para o CSP Contoso. A Contoso implementou a MFA para todos os usuários no locatário de parceiro da Contoso usando a MFA do Azure AD (Azure Active Directory).

2. Jane inicia uma nova sessão do navegador e navega até a página de visão geral do painel do Partner Center (que não é protegida por MFA). A Central de Parceiros redireciona Leila ao Azure AD para entrada.

3. Devido à configuração existente do Azure AD MFA pela Contoso, Jane deve concluir a verificação da MFA. Após a entrada e a verificação de MFA bem-sucedidas, Leila é redirecionada novamente à página de visão geral do Painel da Central de Parceiros.

4. Jane tenta acessar uma das páginas protegidas por MFA no Partner Center. Como Jane já concluiu a verificação de MFA durante a entrada anterior, ela pode acessar a página protegida por MFA sem precisar passar pela verificação de MFA novamente.

### <a name="example-2-partner-has-implemented-third-party-mfa-using-identity-federation"></a>Exemplo 2: o parceiro implementou a MFA de terceiros usando a federação de identidades

1. Trent trabalha para o CSP Wingtip. A Wingtip implementou a MFA para todos os usuários no locatário de parceiro da Wingtip usando a MFA de terceiros, que está integrada ao Azure AD por meio da federação de identidades.

2. Trent inicia uma nova sessão do navegador e navega até a página de visão geral do painel do Partner Center (que não é protegida por MFA). A Central de Parceiros redireciona Matheus ao Azure AD para entrada.

3. Como a Wingtip configurou a federação de identidades, o Azure AD redireciona Trent para o provedor de identidade federada para concluir a entrada e a verificação de MFA. Após a entrada e a verificação da MFA bem-sucedidas, Matheus é redirecionado novamente ao Azure AD e, em seguida, à página de visão geral do Painel da Central de Parceiros.

4. Trent tenta acessar uma das páginas protegidas por MFA no Partner Center. Como Trent já concluiu a verificação de MFA durante a entrada anterior, ele pode acessar a página protegida por MFA sem precisar passar pela verificação de MFA novamente.

### <a name="example-3-partner-hasnt-implemented-mfa"></a>Exemplo 3: o parceiro não implementou a MFA

1. John trabalha para o CSP Fabrikam. A Fabrikam não implementou a MFA para nenhum usuário no locatário parceiro da Fabrikam.

2. John inicia uma nova sessão do navegador e navega até a página de visão geral do painel do Partner Center (que não é protegida por MFA). A Central de Parceiros redireciona Paulo ao Azure AD para entrada.

3. Como a Fabrikam não implementou a MFA, John não precisa concluir a verificação de MFA. Após a entrada bem-sucedida, Paulo é redirecionado novamente à página de visão geral do Painel da Central de Parceiros.

4. John tenta acessar uma das páginas protegidas por MFA no Partner Center. Como John não concluiu a verificação de MFA, o Partner Center o redireciona ao Azure AD para concluí-la. Como essa é a primeira vez que Paulo precisa concluir a MFA, também é solicitado que ele se [registre na MFA](#mfa-registration-experience). Após o registro e a verificação de MFA bem-sucedidos, John agora pode acessar a página protegida por MFA.

5. Outro dia, antes da Fabrikam implementar a MFA para qualquer usuário, Paulo iniciou uma nova sessão do navegador e navegou até a página de visão geral do Painel da Central de Parceiros (que não é protegida por MFA). A Central de Parceiros redireciona Paulo ao Azure AD para entrada sem o aviso de MFA. 

6. John tenta acessar uma das páginas protegidas por MFA no Partner Center. Como John não concluiu a verificação de MFA, o Partner Center o redireciona ao Azure AD para concluí-la. Como Paulo registrou a MFA, desta vez, ele só precisa concluir a verificação de MFA.

> [!NOTE]
>Ação: O Administrador da empresa deve implementar a MFA agora por meio de uma destas [opções](partner-security-requirements.md#actions-that-you-need-to-take) sugeridas pela Central de Parceiros.

## <a name="partner-center-api"></a>API do Partner Center

A API do Partner Center dá suporte à autenticação somente de aplicativo e à autenticação aplicativo+usuário. 

Quando a autenticação aplicativo+usuário for usada, o Partner Center exigirá a verificação de MFA. Mais especificamente, quando um aplicativo parceiro deseja enviar uma solicitação de API ao Partner Center, ele deve incluir um token de acesso no cabeçalho de autorização da solicitação. 

> [!NOTE]
>O [Modelo de Aplicativo Seguro](/partner-center/develop/enable-secure-app-model) é uma estrutura segura e escalonável para autenticar parceiros CSP e CPVs por meio da arquitetura da MFA do Microsoft Azure. Ao chamar a API da Central de Parceiros, você precisará implementá-la antes de habilitar a MFA no seu locatário. 

Quando a Central de Parceiros receber uma solicitação de API com um token de acesso obtido usando a autenticação aplicativo + usuário, a API da Central de Parceiros verificará se o valor da *MFA* está presente na declaração de *AMR (Referência do Método de Autenticação)* . Você pode usar um decodificador JWT para validar se um token de acesso contém o valor de AMR (referência de método de autenticação) esperado ou não:

``` csharp
{
  "aud": "https://api.partnercenter.microsoft.com",
  "iss": "https://sts.windows.net/df845f1a-7b35-40a2-ba78-6481de91f8ae/",
  "iat": 1549088552,
  "nbf": 1549088552,
  "exp": 1549092452,
  "acr": "1",
  "amr": [
    "pwd",
    "mfa"
  ],
  "appid": "23ec45a3-5127-4185-9eff-c8887839e6ab",
  "appidacr": "0",
  "family_name": "Adminagent",
  "given_name": "CSP",
  "ipaddr": "127.0.0.1",
  "name": "Adminagent CSP",
  "oid": "4988e250-5aee-482a-9136-6d269cb755c0",
  "scp": "user_impersonation",
  "tenant_region_scope": "NA",
  "tid": "df845f1a-7b35-40a2-ba78-6481de91f8ae",
  "unique_name": "Adminagent.csp@testtestpartner.onmicrosoft.com",
  "upn": "Adminagent.csp@testtestpartner.onmicrosoft.com",
  "ver": "1.0"
}
```

Se o valor estiver presente, o Partner Center concluirá que a verificação de MFA foi concluída e processará a solicitação de API. Se o valor não estiver presente, a API do Partner Center rejeitará a solicitação com a seguinte resposta:

``` csharp
HTTP/1.1 401 Unauthorized - MFA required
Transfer-Encoding: chunked
Request-Context: appId=cid-v1:03ce8ca8-8373-4021-8f25-d5dd45c7b12f
WWW-Authenticate: Bearer error="invalid_token"
Date: Thu, 14 Feb 2019 21:54:58 GMT
```

Quando a autenticação somente por aplicativo for usada, as APIs que dão suporte à autenticação somente por aplicativo trabalharão continuamente sem exigir a MFA.

## <a name="partner-delegated-administration"></a>Administração Delegada por Parceiro

### <a name="using-service-portals"></a>Usar portais de serviço

As contas de parceiros, incluindo Agentes Administrativos e Agentes de Assistência Técnica, podem usar os Privilégios de Administrador Delegado do Parceiro para gerenciar recursos do cliente por meio dos Portais do Microsoft Online Services, da CLI (interface de linha de comando) e das APIs (usando a autenticação aplicativo + usuário).

Ao acessar os Portais do Microsoft Online Services usando os Privilégios de Administrador Delegado do Parceiro (Administrador em nome de) para gerenciar recursos do cliente, muitos desses portais exigem que a conta do parceiro seja autenticada de maneira interativa, com o locatário do Azure Active Directory do cliente definido como o contexto de autenticação: a conta do parceiro é necessária para entrar no locatário do cliente.

Quando o Azure Active Directory receber essas solicitações de autenticação, ele exigirá que a conta do parceiro conclua a verificação de MFA. Há duas experiências de usuário possíveis, dependendo se a conta do parceiro é uma identidade gerenciada ou federada:

- Se a conta do parceiro for uma identidade **gerenciada** , o Azure Active Directory solicitará diretamente que o usuário conclua a verificação de MFA. Se a conta de parceiro não tiver sido registrada na MFA com o Azure Active Directory antes, o usuário deverá [concluir o registro da MFA](#mfa-registration-experience) primeiro.

- Se a conta do parceiro for uma identidade **federada** , a experiência dependerá de como o administrador de parceiro configurou a Federação no Azure Active Directory. Ao configurar a federação no Azure Active Directory, o administrador de parceiro pode indicar para o Azure Active Directory se o provedor de identidade federada dá suporte à MFA ou não. Em caso afirmativo, o Azure Active Directory redirecionará o usuário para o provedor de identidade federada para concluir a verificação de MFA. Caso contrário, o Azure Active Directory solicitará diretamente que o usuário conclua a verificação de MFA. Se a conta de parceiro não tiver sido registrada na MFA com o Azure Active Directory antes, o usuário deverá [concluir o registro da MFA](#mfa-registration-experience) primeiro.

A experiência geral é semelhante ao cenário em que um locatário do cliente final implementou a MFA para os administradores dele. Por exemplo, o locatário do cliente habilitou os [padrões de segurança do Azure AD](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), o que exige que todas as contas com direitos administrativos entrem no locatário do cliente com verificação de MFA, incluindo Agentes Administrativos e Agentes de Suporte Técnico. Para fins de teste, os parceiros podem habilitar os [padrões de segurança do Azure AD](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) no locatário do cliente e, em seguida, tentar usar Privilégios de Administração Delegada do Parceiro para acessar o locatário do cliente.

> [!NOTE]
> Nem todos os Portais do Microsoft Online Service exigem que as contas do parceiro entrem no locatário do cliente ao acessar os recursos do cliente usando Privilégios de Administração Delegada do Parceiro. Em vez disso, eles exigem apenas que as contas do parceiro entrem no locatário parceiro. Um exemplo é o Centro de Administração do Exchange. Ao longo do tempo, esperamos que esses portais exijam que as contas do parceiro entrem no locatário do cliente ao usar Privilégios de Administração Delegada do Parceiro.

### <a name="using-service-apis"></a>Usar APIs de serviço

Algumas APIs do Microsoft Online Services (como o Azure Resource Manager, o Azure AD Graph, o Microsoft Graph etc.) dão suporte a parceiros que usam Privilégios de Administração Delegada do Parceiro para gerenciar programaticamente os recursos do cliente. Para aproveitar os Privilégios de Administração Delegada do Parceiro com essas APIs, o aplicativo do parceiro deve incluir um token de acesso no cabeçalho de Autorização de solicitação da API, em que o token de acesso é obtido tendo uma conta de usuário parceiro para autenticar com o Azure AD, com o cliente do Azure AD definido como o contexto de autenticação. O aplicativo do parceiro precisa ter credenciais da conta do usuário parceiro no locatário do cliente.

Quando o Azure AD receber essa solicitação de autenticação, ele exigirá que a conta do usuário parceiro conclua a verificação da MFA. Se a conta do usuário parceiro ainda não tiver sido registrada na MFA, ela deverá concluir o registro de MFA primeiro.

Todos os aplicativos do parceiro integrados a essas APIs que usam os Privilégios de Administração Delegada do Parceiro são afetados por esse recurso. Para verificar se os aplicativos do parceiro podem continuar trabalhando com essas APIs sem interrupção:

- O parceiro deve evitar usar o método de autenticação do usuário não interativo com o Azure AD para obter o token de acesso. Ao usar o método de autenticação do usuário não interativo como o [Fluxo de Senha](https://github.com/AzureAD/azure-activedirectory-library-for-dotnet/wiki/Acquiring-tokens-with-username-and-password), o Azure AD não poderá solicitar que o usuário conclua a verificação de MFA. Em vez disso, o parceiro deve alternar para usar o método de autenticação do usuário interativo como o [fluxo do OpenID Connect](/azure/active-directory/develop/v1-protocols-openid-connect-code).

- Durante o método de autenticação do usuário interativo, o parceiro deve usar uma conta do usuário parceiro que já esteja habilitada para MFA. Ou, quando solicitado pelo Azure AD, o parceiro pode concluir o registro e a verificação de MFA durante a entrada.

- Isso é semelhante ao cenário em que um locatário do cliente final implementou a MFA para os administradores dele. Por exemplo, o locatário do cliente habilitou os [padrões de segurança do Azure AD](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), que exige que todas as contas de usuário com direitos administrativos entrem no locatário do cliente com verificação de MFA, incluindo Agentes Administrativos e Agentes de Suporte Técnico. Para fins de teste, os parceiros podem habilitar os [padrões de segurança do Azure AD](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) no locatário do cliente e, em seguida, tentar usar Privilégios de Administração Delegada do Parceiro para acessar programaticamente o locatário do cliente.

### <a name="mfa-registration-experience"></a>Experiência de registro de MFA

Durante a verificação de MFA, se a conta do usuário parceiro ainda não tiver sido registrada na MFA, o Azure AD solicitará que o usuário conclua o registro de MFA primeiro:

:::image type="content" source="images/MfaRegistration1.png" alt-text="Etapa 1 do registro de MFA":::

Depois de clicar em **Avançar** , o usuário precisará escolher uma opção em uma lista de métodos de verificação.

:::image type="content" source="images/MfaRegistration2.png" alt-text="Etapa 1 do registro de MFA":::

Após o registro bem-sucedido, o usuário precisará concluir a verificação de MFA com base na verificação escolhida pelo usuário.

## <a name="request-for-technical-exception"></a>Solicitação de exceção técnica

Os parceiros poderão se candidatar para uma exceção técnica a fim de suprimir a verificação de MFA se estiverem encontrando problemas técnicos com o Microsoft Online Services e não houver uma solução viável ou alternativa. Antes de fazer isso, examine as seguintes seções:

- [Lista de problemas comuns relatados por parceiros](#list-of-common-issues-reported-by-partners)
- [Como enviar uma solicitação de exceção técnica](#how-to-submit-a-request-for-technical-exception)
 
### <a name="list-of-common-issues-reported-by-partners"></a>Lista de problemas comuns relatados por parceiros
Antes de se candidatar para uma exceção técnica, examine a lista de problemas comuns relatados por outros parceiros para entender se são motivos válidos para exceção técnica ou não.

#### <a name="issue-1-partner-needs-more-time-to-implement-mfa-for-their-partner-agents"></a>Problema 1: o parceiro precisa de mais tempo para implementar a MFA para os agentes do parceiro dele
Um parceiro não iniciou ou ainda está no processo de implementação da MFA para os agentes do parceiro dele que precisam acessar os Portais do Microsoft Online Services usando Privilégios de Administração Delegada do Parceiro para gerenciar os recursos do cliente. O parceiro precisa de mais tempo para concluir a implementação da MFA. Esse problema é um motivo válido para exceção técnica?

**Resposta** : Não. O parceiro precisa fazer planos para implementar a MFA para os usuários dele para evitar interrupções.

> [!NOTE]
> Embora o parceiro não tenha implementado a MFA para os agentes parceiros dele, os agentes do parceiro ainda poderão acessar os Portais de Serviço Online da Microsoft usando os Privilégios de Administração Delegada do Parceiro, desde que possam concluir o registro e a verificação da MFA quando solicitado durante a entrada no locatário do cliente. Concluir o registro da MFA não habilita automaticamente o usuário para a MFA.

##### <a name="issue-2-partner-has-not-implemented-mfa-for-user-accounts-not-using-delegated-admin-privileges"></a>Problema 2: o parceiro não implementou a MFA para contas de usuário que não usam Privilégios de Administração Delegada
Um parceiro tem alguns usuários nos locatários dele que não precisam de acesso aos Portais do Microsoft Online Services para gerenciar os recursos do cliente usando os Privilégios de Administração Delegada do Parceiro. O parceiro está no processo de implementação da MFA para esses usuários e precisa de mais tempo para concluí-lo. Esse problema é um motivo válido para exceção técnica?

**Resposta** : Não. Como essas contas de usuário não estão usando Privilégios de Administrador Delegado do Parceiro para gerenciar recursos do cliente, elas não precisarão entrar no locatário do cliente. Elas não serão afetadas pelo Azure AD que exige verificação de MFA durante a entrada no locatário do cliente.

##### <a name="issue-3-partner-has-not-implemented-mfa-for-user-service-accounts"></a>Problema 3: o parceiro não implementou a MFA para contas de serviço de usuário
Um parceiro tem algumas contas de usuário nos locatários parceiros dele, que estão sendo usadas por dispositivos como contas de serviço. Essas são contas com poucos privilégios que não exigem acesso ao Partner Center nem aos Portais do Microsoft Online Services para gerenciar recursos do cliente usando Privilégios de Administração Delegada do Parceiro. Esse problema é um motivo válido para exceção técnica?

**Resposta** : Não. Como essas contas de usuário não estão usando Privilégios de Administrador Delegado do Parceiro para gerenciar recursos do cliente, elas não precisarão entrar no locatário do cliente. Elas não serão afetadas pelo Azure AD que exige verificação de MFA durante a entrada no locatário do cliente.

##### <a name="issue-4-partner-cannot-implement-mfa-using-ms-authenticator-app"></a>Problema 4: o parceiro não consegue implementar a MFA usando o aplicativo MS Authenticator
Um parceiro tem uma política de “clean desk”, que não permite que funcionários levem dispositivos móveis pessoais para a área de trabalho deles. Sem acesso aos respectivos dispositivos móveis pessoais, os funcionários não podem instalar o aplicativo MS Authenticator, que é a única verificação de MFA compatível com os padrões de segurança do Azure AD. Esse problema é um motivo válido para exceção técnica?

**Resposta** : Não, esse não é um motivo válido para exceção técnica. O parceiro deve considerar as seguintes alternativas para que os funcionários dele ainda possam concluir a verificação de MFA ao acessar o Partner Center:
- O parceiro também pode se inscrever no Azure AD Premium ou em soluções de MFA de terceiros (compatíveis com o Azure AD) que possam fornecer métodos de verificação adicional.

##### <a name="issue-5-partner-cannot-implement-mfa-due-to-the-use-of-legacy-authentication-protocols"></a>Problema 5: o parceiro não pode implementar a MFA devido ao uso de protocolos de autenticação herdados
Um parceiro tem alguns agentes do parceiro que ainda estão usando protocolos de autenticação herdados, que não são compatíveis com MFA. Por exemplo, os usuários ainda estão usando o Outlook 2010, que é baseado em protocolos de autenticação herdados. Habilitar a MFA para esses agentes do parceiro interromperá o uso de protocolos de autenticação herdados.

**Resposta** : Não, esse não é um motivo válido para exceção técnica. Os parceiros são incentivados a não usar protocolos de autenticação herdados devido a eventuais implicações de segurança, pois esses protocolos não podem ser protegidos com verificação de MFA e são muito mais suscetíveis ao comprometimento de credenciais. Se o não uso de protocolos de autenticação herdados não for uma opção, os parceiros deverão considerar inscrever-se no Azure AD Premium, que dá suporte ao uso de Senhas de Aplicativo. As Senhas de Aplicativo são senhas avulsas geradas pelo sistema e geralmente são mais fortes do que as senhas geradas por humanos. Usando Senhas de Aplicativo, os parceiros podem implementar a MFA para os usuários deles enquanto retornam para Senhas de Aplicativo apenas para protocolos de autenticação herdados.

Leia a postagem sobre [Autenticação básica e Exchange Online](https://techcommunity.microsoft.com/t5/exchange-team-blog/basic-auth-and-exchange-online-february-2020-update/ba-p/1191282) para conhecer o plano mais recente de suporte à autenticação herdada para o Outlook e siga o [blog da equipe do Exchange](https://techcommunity.microsoft.com/t5/exchange-team-blog/bg-p/Exchange) para receber as próximas notícias. 

> [!NOTE]
> Embora o parceiro não tenha implementado a MFA para os agentes parceiros dele, os agentes do parceiro ainda poderão acessar os Portais de Serviço Online da Microsoft usando os Privilégios de Administração Delegada do Parceiro desde que possam concluir o registro e a verificação da MFA quando solicitado durante a entrada no locatário do cliente. Concluir o registro da MFA não habilita automaticamente o usuário para a MFA.

##### <a name="issue-6-partner-has-implemented-third-party-mfa-that-isnt-recognized-by-azure-ad"></a>Problema 6: o parceiro implementou uma MFA de terceiros que não é reconhecida pelo Azure AD
Um parceiro implementou a MFA para os usuários dele usando uma solução de MFA de terceiros. No entanto, o parceiro não consegue configurar corretamente a solução de MFA de terceiros para retransmitir ao Azure AD que a verificação de MFA foi concluída durante a autenticação do usuário. Esse é um motivo válido para exceção técnica?

**Resposta** : Sim, esse problema pode ser considerado um motivo válido para exceção técnica. Antes de enviar uma solicitação de exceção técnica, confirme com o provedor de soluções de MFA de terceiros que a solução de MFA não pode ser configurada para fluir a declaração *authenticationmethodsreferences* (com o valor *multipleauthn* ) para o Azure AD, a fim de indicar que a verificação de MFA foi concluída durante a autenticação do usuário. Ao enviar uma solicitação de exceção técnica, você precisará fornecer detalhes da solução de MFA de terceiros usada e indicar o método de integração (por exemplo, por meio da federação de identidades ou do uso do controle personalizado do Azure AD) e fornecer as seguintes informações na solicitação de exceção técnica como os documentos de suporte:

- As configurações de MFA de terceiros.

- O resultado de [Testar os Requisitos de Segurança do Parceiro](/powershell/partnercenter/test-partner-security-requirements) em execução pela conta habilitada para MFA de terceiros.

- A ordem de compra da solução de MFA de terceiros que você está usando ou pretende usar.

### <a name="how-to-submit-a-request-for-technical-exception"></a>Como enviar uma solicitação de exceção técnica

Para enviar uma solicitação de exceção técnica:

1. Faça logon no Partner Center como Administrador Global ou Agente Administrativo.

2. Crie uma solicitação de serviço de parceiro navegando até **Suporte** > **Solicitações de suporte do parceiro** e clicando em **Nova solicitação** .

3. Procure **MFA – Solicitação de exceção** na caixa de pesquisa ou selecione **CSP** em Categoria, **Contas, Integração, Acesso** em Tópico, **MFA – Solicitação de exceção** em Subtópico e, em seguida, escolha **Próxima etapa** .

4. Forneça os detalhes solicitados para enviar uma solicitação de serviço de exceção técnica e clique em **Enviar** .

A Microsoft pode levar até três dias úteis para fornecer uma resposta a uma solicitação de exceção técnica.