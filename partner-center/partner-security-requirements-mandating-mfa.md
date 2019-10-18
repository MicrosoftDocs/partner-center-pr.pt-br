---
title: Obrigando a MFA para seu locatário do parceiro | Centro de parceiros
ms.topic: article
ms.date: 09/25/2019
description: Detalhes sobre a MFA de reobrigar seus requisitos de segurança de locatário do parceiro
author: isaiahwilliams
ms.author: iswillia
keywords: O Azure Active Directory, provedor de soluções na nuvem, programa de provedor de soluções na nuvem, CSP, fornecedor do painel de controle, CPV, autenticação multifator, MFA, modelo de aplicativo seguro, modelo de aplicativo seguro, segurança
ms.localizationpriority: medium
ms.openlocfilehash: 8f68d4628bd6212b800ea926c6c3b9f412e3d5cc
ms.sourcegitcommit: dcc2a2077ef17255ecf7a2fa5fae6bbeefaa9eb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/07/2019
ms.locfileid: "71997785"
---
# <a name="mandating-mfa-for-your-partner-tenant"></a>Obrigando a MFA para seu locatário de parceiro

**Aplica-se a**

- Todos os parceiros no programa Provedor de Soluções na Nuvem
  - Fatura direta
  - Provedor indireto
  - Revendedor indireto
- Todos os consultores

Esses parceiros serão solicitados a concluir a verificação de MFA para as seguintes áreas:

- [Painel do Partner Center](#partner-center-dashboard)
- [API do Partner Center](#partner-center-api)
- [Administração delegada de parceiro](#partner-delegated-administration)

A intenção desse recurso é ajudar os parceiros a proteger o acesso aos recursos do cliente contra o comprometimento de credenciais.

## <a name="partner-center-dashboard"></a>Painel do Partner Center
Determinadas páginas no painel do Partner Center serão protegidas por MFA, incluindo:

* Todas as páginas na guia **clientes** .
* Todas as páginas na guia de **solicitações de clientes do → de suporte** .

Se você tentar acessar qualquer uma dessas páginas e não tiver concluído a verificação de MFA anteriormente, será necessário fazer isso.

Os seguintes tipos de usuário estão autorizados a acessar essas páginas protegidas por MFA e, portanto, são afetados por esse recurso, incluindo:

* Agentes de administração
* Agentes de vendas
* Agentes de assistência técnica

Para ilustrar como isso funciona, considere os dois exemplos a seguir.

**Exemplo 1: o parceiro implementou o Azure AD MFA**
1.  Jane funciona para o CSP contoso. A contoso implementou o MFA para todos os seus usuários no locatário do parceiro contoso usando o Azure AD MFA.
2.  Em sua estação de trabalho, Jane inicia uma nova sessão do navegador e navega para a página de visão geral do painel do Partner Center (que não é protegida por MFA). O Partner Center redireciona Jane para o Azure AD para entrar.
3.  Devido à configuração do Azure AD MFA existente pela contoso, Jane é necessário para concluir a verificação de MFA. Após a entrada bem-sucedida e a verificação de MFA, Jane é Redirecionado de volta para a página de visão geral do painel do Partner Center.
4.  Jane tenta acessar uma das páginas protegidas por MFA no Partner Center. Como Jane já concluiu a verificação de MFA durante a entrada anterior, Jane pode acessar a página protegida por MFA sem precisar passar pela verificação de MFA novamente.

**Exemplo 2: o parceiro implementou o MFA de terceiros usando a Federação de identidades**
1. Trent funciona para o CSP Wingtip. A Wingtip implementou o MFA para todos os seus usuários no locatário do parceiro Wingtip usando o MFA de terceiros, que é integrado ao Azure AD por meio da Federação de identidades.
2. Em sua estação de trabalho, o Trent inicia uma nova sessão do navegador e navega para a página de visão geral do painel do Partner Center (que não é protegida por MFA). O Partner Center redireciona o Justin para o Azure AD para entrar.
3. Como a Wingtip tem a Federação de identidade da instalação, o Azure AD redireciona o Trent para o provedor de identidade federada para concluir a entrada e a verificação de MFA. Após a entrada bem-sucedida e a verificação de MFA, o Trent é Redirecionado de volta para o Azure AD e, em seguida, para a página de visão geral do painel do Partner Center.
4. O Justin tenta acessar uma das páginas protegidas por MFA no Partner Center. Como o Trent já concluiu a verificação de MFA durante a entrada anterior, o Trent pode acessar a página protegida do MFA sem precisar passar pela verificação de MFA novamente.

**Exemplo 3: o parceiro não implementou o MFA**
1. John trabalha para o CSP fabrikam. A Fabrikam não implementou o MFA para nenhum usuário no locatário do parceiro da Fabrikam.
2. Em sua estação de trabalho, João inicia uma nova sessão do navegador e navega para a página de visão geral do painel do Partner Center (que não é protegida por MFA). O Partner Center redireciona John para o Azure AD para entrar.
3. Como a Fabrikam não implementou o MFA, João não precisa concluir a verificação de MFA. Após a entrada bem-sucedida, João é Redirecionado de volta para a página Visão geral do painel do Partner Center.
4. João tenta acessar uma das páginas protegidas por MFA no Partner Center. Como John não concluiu a verificação de MFA, o Partner Center redireciona John para Azure AD para concluir a verificação de MFA. Como essa é a primeira vez que John é necessário para concluir a MFA, John também é solicitado a se registrar para MFA usando Microsoft Authenticator aplicativo. Após o registro de MFA bem-sucedido e a verificação de MFA, John agora pode acessar a página protegida por MFA.

## <a name="partner-center-api"></a>API do Partner Center

A API do Partner Center dá suporte à autenticação somente de aplicativo e ao aplicativo + autenticação de usuário. Quando o aplicativo + a autenticação do usuário for usado, o Partner Center exigirá a verificação de MFA. Mais especificamente, quando um aplicativo de parceiro deseja enviar uma solicitação de API para o Partner Center, ele deve incluir um token de acesso no cabeçalho de autorização da solicitação. Quando o Partner Center recebe uma solicitação de API com um token de acesso obtido usando o aplicativo + autenticação do usuário, a API do Partner Center verificará a presença do valor de *MFA* na declaração da *Amr (referência do método de autenticação)* . Você pode usar um decodificador JWT para validar se um token de acesso contém o valor de AMR (referência de método de autenticação) esperado ou não:

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
  "family_name": "Williams",
  "given_name": "Isaiah",
  "ipaddr": "127.0.0.1",
  "name": "Isaiah Williams",
  "oid": "4988e250-5aee-482a-9136-6d269cb755c0",
  "scp": "user_impersonation",
  "tenant_region_scope": "NA",
  "tid": "df845f1a-7b35-40a2-ba78-6481de91f8ae",
  "unique_name": "Isaiah.Williams@testtestpartner.onmicrosoft.com",
  "upn": "Isaiah.Williams@testtestpartner.onmicrosoft.com",
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

## <a name="partner-delegated-administration"></a>Administração delegada de parceiro

### <a name="using-service-portals"></a>Usando portais de serviço

Contas de parceiros, incluindo agentes de administração e agentes de assistência técnica, podem usar seus privilégios de administrador delegado para parceiros para gerenciar recursos do cliente por meio de portais do Microsoft Online Services, CLI (interface de linha de comando) e APIs (usando o aplicativo + autenticação de usuário).

Ao acessar os portais do Microsoft Online Services usando os privilégios de administrador delegado do parceiro para gerenciar recursos do cliente, muitos desses portais exigem que a conta do parceiro autentique interativamente, com o cliente Azure Active Directory conjunto de locatários como o contexto de autenticação-a conta do parceiro é necessária para entrar no locatário do cliente.

Quando Azure Active Directory receber essas solicitações de autenticação, ela exigirá que a conta do parceiro conclua a verificação de MFA. Há duas experiências de usuário possíveis, dependendo se a conta do parceiro é uma identidade gerenciada ou federada:

- Se a conta do parceiro for uma identidade **gerenciada** , Azure Active Directory solicitará diretamente que o usuário conclua a verificação de MFA. Se a conta de parceiro não tiver sido registrada para MFA com Azure Active Directory antes, o usuário será solicitado a [concluir o registro de MFA](#mfa-registration-experience) primeiro.

- Se a conta do parceiro for uma identidade **federada** , a experiência dependerá de como o administrador do parceiro configurou a federação no Azure Active Directory. Ao configurar a Federação no Azure Active Directory, o administrador do parceiro pode indicar Azure Active Directory se o provedor de identidade federada oferece suporte a MFA ou não. Nesse caso, Azure Active Directory redirecionará o usuário para o provedor de identidade federada para concluir a verificação de MFA. Caso contrário, Azure Active Directory avisará diretamente ao usuário para concluir a verificação de MFA. Se a conta de parceiro não tiver sido registrada para MFA com Azure Active Directory antes, o usuário será solicitado a [concluir o registro de MFA](#mfa-registration-experience) primeiro.

A experiência geral é muito semelhante ao cenário em que um locatário do cliente final implementou o MFA para seus administradores. Por exemplo, o locatário do cliente habilitou a [política de linha de base do Azure ad – MFA para administradores](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators), que exige que todas as contas com direitos administrativos entrem no locatário do cliente com verificação de MFA, incluindo agentes de administração e agentes de assistência técnica. Para fins de teste, os parceiros podem habilitar a [política de MFA para administradores](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) no locatário do cliente e, em seguida, tentar usar privilégios de administração delegada de parceiro para acessar o locatário do cliente.

> [!NOTE]
> Nem todos os portais do Microsoft Online Service exigem que as contas de parceiros entrem no locatário do cliente ao acessar os recursos do cliente usando privilégios de administrador delegado do parceiro. Em vez disso, eles exigem apenas as contas de parceiros para entrar no locatário do parceiro. Um exemplo é o centro de administração do Exchange. Ao longo do tempo, esperamos que esses portais exijam que as contas de parceiros entrem no locatário do cliente ao usar privilégios de administrador delegado para parceiros.

### <a name="using-service-apis"></a>Usando APIs de serviço
Algumas APIs do Microsoft Online Services (por exemplo, Azure Resource Manager, Azure AD Graph, Microsoft Graph, etc.) dão suporte a parceiros que usam privilégios de administrador delegado para gerenciar recursos do cliente programaticamente. Para aproveitar os privilégios de administrador delegado do parceiro com essas APIs, o aplicativo de parceiro deve incluir um token de acesso no cabeçalho de autorização de solicitação da API, em que o token de acesso é obtido com uma conta de usuário do parceiro para autenticar com o Azure AD, com o cliente do Azure AD definido como o contexto de autenticação. O aplicativo parceiro precisa ter uma conta de usuário do parceiro entre no locatário do cliente.

Quando o Azure AD recebe como solicitação de autenticação, o Azure AD exigirá que a conta de usuário do parceiro conclua a verificação de MFA. Se a conta de usuário do parceiro ainda não tiver sido registrada para MFA, a conta de usuário será solicitada a concluir o registro de MFA primeiro.

Todos os aplicativos de parceiros que são integrados a essas APIs usando privilégios de administrador delegados de parceiro são afetados por esse recurso. Para garantir que os aplicativos de parceiros possam continuar a trabalhar com essas APIs sem interrupção:

- O parceiro deve evitar o uso do método de autenticação de usuário não interativo com o Azure AD para obter o token de acesso. Ao usar o método de autenticação de usuário não interativo, como o [fluxo de senha](https://github.com/AzureAD/azure-activedirectory-library-for-dotnet/wiki/Acquiring-tokens-with-username-and-password), o Azure ad não poderá solicitar que o usuário conclua a verificação de MFA. O parceiro deve alternar para o uso do método de autenticação de usuário interativo como, por exemplo, o [fluxo do OpenID Connect](https://docs.microsoft.com/azure/active-directory/develop/v1-protocols-openid-connect-code) .
- Durante o método de autenticação de usuário interativo, o parceiro deve usar uma conta de usuário de parceiro que já esteja habilitada para MFA. Como alternativa, quando solicitado pelo Azure AD, o parceiro pode concluir o registro de MFA e a verificação de MFA durante a entrada.
- Isso é muito semelhante ao cenário em que um locatário do cliente final implementou o MFA para seus administradores. Por exemplo, o locatário do cliente habilitou a [política de linha de base do Azure ad – MFA para administradores](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators), que exige que todas as contas de usuário com direitos administrativos entrem no locatário do cliente com verificação de MFA, incluindo agentes de administração e agentes de assistência técnica. Para fins de teste, os parceiros podem habilitar a [política de MFA para administradores](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) no locatário do cliente e, em seguida, tentar usar privilégios de administração delegada de parceiro para acessar programaticamente o locatário do cliente.

### <a name="mfa-registration-experience"></a>Experiência de registro de MFA
Durante a verificação de MFA, se a conta de parceiro ainda não tiver sido registrada para MFA, o Azure AD solicitará que o usuário conclua o registro de MFA primeiro:

![Etapa 1 do registro de MFA](images/MfaRegistration1.png)

Depois de clicar em **Avançar**, o usuário será solicitado a escolher em uma lista de métodos de verificação (incluindo o telefone, o SMS e o aplicativo autenticador).

![Etapa 2 do registro de MFA](images/MfaRegistration2.png)

Após o registro bem-sucedido, o usuário precisará concluir a verificação de MFA com base na verificação escolhida pelo usuário.



## <a name="request-for-technical-exception"></a>Solicitação de exceção técnica

Os parceiros podem se candidatar para uma exceção técnica a fim de suprimir a verificação de MFA se eles estiverem encontrando problemas técnicos com o Microsoft Online Services e não houver uma solução viável ou uma solução alternativa. Antes de fazer isso, examine as seguintes seções:

 - [Lista de problemas comuns relatados por parceiros](#list-of-common-issues-reported-by-partners)
 - [Como enviar uma solicitação de exceção técnica](#how-to-submit-a-request-for-technical-exception)
 
### <a name="list-of-common-issues-reported-by-partners"></a>Lista de problemas comuns relatados por parceiros
Antes de aplicar uma exceção técnica, examine a lista de problemas comuns relatados por outros parceiros para entender se eles são motivos válidos para a exceção técnica ou não.

#### <a name="issue-1-partner-needs-more-time-to-implement-mfa-for-their-partner-agents"></a>Problema 1: o parceiro precisa de mais tempo para implementar a MFA para seus agentes de parceiro
Um parceiro não foi iniciado ou ainda está no processo de implementação da MFA para seus agentes de parceiro que precisam acessar os portais do Microsoft Online Services usando privilégios de administração delegada de parceiro para gerenciar os recursos do cliente. O parceiro precisa de mais tempo para concluir a implementação da MFA. Esse é um motivo válido para a exceção técnica?

**Resposta**: não. O parceiro precisa fazer planos para implementar a MFA para seus usuários para evitar interrupções.

> [!NOTE]
> Embora o parceiro não tenha implementado o MFA para seus agentes de parceiro, os agentes de parceiro ainda podem acessar portais do Microsoft Online Services usando privilégios de administração delegada de parceiro, desde que possam concluir o registro de MFA e a verificação de MFA Quando solicitado durante a entrada no locatário do cliente. Concluir o registro de MFA não habilita automaticamente o usuário para MFA.

##### <a name="issue-2-partner-has-not-implemented-mfa-for-user-accounts-not-using-delegated-admin-privileges"></a>Problema 2: o parceiro não implementou o MFA para contas de usuário que não usam privilégios de administrador delegado
Um parceiro tem alguns usuários em seus locatários parceiros que não exigem acesso aos portais do Microsoft Online Services para gerenciar recursos do cliente usando privilégios de administração delegada de parceiro. O parceiro está no processo de implementação do MFA para esses usuários e precisa de mais tempo para ser concluído. Esse é um motivo válido para a exceção técnica?

**Resposta**: não. Como essas contas de usuário não estão usando privilégios de administração delegada de parceiro para gerenciar recursos do cliente, elas não serão necessárias para entrar no locatário do cliente. Eles não serão afetados pelo Azure AD exigindo a verificação de MFA durante a entrada no locatário do cliente.

##### <a name="issue-3-partner-has-not-implemented-mfa-for-user-service-accounts"></a>Problema 3: o parceiro não implementou o MFA para contas de serviço de usuário
Um parceiro tem algumas contas de usuário em seus locatários parceiros que estão sendo usados por dispositivos como contas de serviço. Essas são geralmente contas com poucos privilégios que não exigem os portais do Access Center nem do Microsoft Online Services para gerenciar os recursos do cliente usando privilégios de administração delegada de parceiro. Esse é um motivo válido para a exceção técnica?

**Resposta**: não. Como essas contas de usuário não estão usando privilégios de administração delegada de parceiro para gerenciar recursos do cliente, elas não serão necessárias para entrar no locatário do cliente. Eles não serão afetados pelo Azure AD exigindo a verificação de MFA durante a entrada no locatário do cliente.

#### <a name="issue-4-partner-cannot-implement-mfa-using-ms-authenticator-app"></a>Problema 4: o parceiro não pode implementar o MFA usando o aplicativo MS Authenticator
Um parceiro tem uma política de "mesa limpa" que não permite aos funcionários trazer seus dispositivos móveis pessoais para sua área de trabalho. Sem acesso a seus dispositivos móveis pessoais, os funcionários não podem instalar o aplicativo MS Authenticator, que é a única verificação de MFA suportada pelas políticas de linha de base do Azure AD. Esse é um motivo válido para a exceção técnica?

**Resposta**: não, esse não é um motivo válido para a exceção técnica. O parceiro deve considerar as seguintes alternativas, para que seus funcionários ainda possam concluir a verificação de MFA ao acessar o Partner Center:
- Além do aplicativo do MS Authenticator, as políticas de linha de base do Azure AD também podem ser usadas com o aplicativo autenticador compatível de terceiros, que pode ter suporte para computadores Windows que executam o Microsoft Windows.
- O parceiro também pode se inscrever em soluções de MFA de Azure AD Premium ou de terceiros (compatível com o Azure AD), que pode fornecer métodos de verificação adicionais.

#### <a name="issue-5-partner-cannot-implement-mfa-due-to-the-use-of-legacy-authentication-protocols"></a>Problema 5: o parceiro não pode implementar o MFA devido ao uso de protocolos de autenticação herdados
Um parceiro tem alguns agentes de parceiro que ainda estão usando protocolos de autenticação herdados, que não são compatíveis com MFA. Por exemplo, os usuários ainda estão usando o Outlook 2010, que é baseado em protocolos de autenticação herdados. Habilitar a MFA para esses agentes de parceiro irá interromper o uso de protocolos de autenticação herdados.

**Resposta**: não, esse não é um motivo válido para a exceção técnica. Os parceiros são altamente incentivados a se afastar do uso de protocolos de autenticação herdados devido a possíveis implicações de segurança, pois esses protocolos não podem ser protegidos com a verificação de MFA e são muito mais suscetíveis ao comprometimento de credenciais. Se estiver se afastando do uso de protocolos de autenticação herdados não é uma opção, os parceiros devem considerar a inscrição para Azure AD Premium, que oferece suporte ao uso de senhas de aplicativo. As senhas de aplicativo são senhas geradas pelo sistema únicas que geralmente são mais seguras do que as senhas geradas por humanos. Usando senhas de aplicativo, os parceiros podem implementar a MFA para seus usuários, enquanto retornam apenas as senhas de aplicativo para protocolos de autenticação herdados.

> [!NOTE]
> Embora o parceiro não tenha implementado o MFA para seus agentes de parceiro, os agentes de parceiro ainda podem acessar portais do Microsoft Online Services usando privilégios de administração delegada de parceiro, desde que possam concluir o registro de MFA e a verificação de MFA Quando solicitado durante a entrada no locatário do cliente. Concluir o registro de MFA não habilita automaticamente o usuário para MFA.

#### <a name="issue-6-partner-is-using-exchange-online-powershell-which-does-not-support-mfa"></a>Problema 6: o parceiro está usando o PowerShell do Exchange Online que não oferece suporte a MFA
Um parceiro está usando o Exchange Online PowerShell com privilégios de administração delegada de parceiro para gerenciar o serviço Exchange Online em nome de seus clientes. O PowerShell do Exchange Online não oferece suporte a MFA. Se o parceiro implementar a MFA para seus usuários, esses usuários não poderão mais acessar o PowerShell do Exchange Online. Esse é um motivo válido para a exceção técnica?

**Resposta**: Sim, isso pode ser considerado um motivo válido para a exceção técnica. O [módulo do PowerShell do Exchange Online existente que dá suporte à administração delegada de parceiro](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) não exige que o usuário do parceiro entre no locatário do cliente e, portanto, não seja afetado pelo Azure ad exigindo a verificação de MFA. No entanto, não é compatível com MFA. A equipe do Microsoft Exchange Online está desenvolvendo um novo módulo do PowerShell que dá suporte a privilégios de administração delegada de parceiro e MFA. Até que o novo módulo do PowerShell esteja disponível, os parceiros não podem implementar o MFA para usuários que precisam usar o módulo do PowerShell existente. Se esses usuários encontrarem dificuldades para acessar outros serviços online da Microsoft devido ao Azure AD exigir a verificação de MFA durante a entrada entre locatários, os parceiros poderão solicitar uma exceção técnica para suprimir a verificação de MFA.

> [!NOTE]
> Embora o parceiro não consiga implementar o MFA para usuários que precisam acessar o módulo do PowerShell do Exchange Online, esses usuários ainda podem acessar o Microsoft Online Services para gerenciar recursos do cliente usando privilégios de administração delegada de parceiro fornecidos Eles podem concluir o registro de MFA e a verificação de MFA quando solicitado durante a entrada no locatário do cliente. Concluir o registro de MFA não habilita automaticamente o usuário para MFA e, portanto, não afeta o acesso ao módulo do PowerShell do Exchange Online.

#### <a name="issue-7-partner-has-implemented-3rd-party-mfa-which-isnt-recognized-by-azure-ad"></a>Problema 7: o parceiro implementou o MFA de terceiros que não é reconhecido pelo Azure AD
Um parceiro implementou o MFA para seus usuários usando uma solução MFA de terceiros. No entanto, o parceiro não pode configurar corretamente a solução MFA de terceiros para retransmitir ao Azure AD que a verificação de MFA foi concluída durante a autenticação do usuário. Esse é um motivo válido para a exceção técnica?

**Resposta**: Sim, isso pode ser considerado um motivo válido para a exceção técnica. Antes de enviar uma solicitação de exceção técnica, confirme com o provedor de solução MFA de terceiros que a solução MFA não pode ser configurada para fluir a Declaração *authenticationmethodsreferences* (com o valor *multipleauthn*) para o Azure AD para indicar que a verificação de MFA foi concluída durante a autenticação do usuário. Ao enviar uma solicitação de exceção técnica, forneça detalhes da solução de MFA de terceiros usada e indique o método de integração (por exemplo, por meio da Federação de identidade ou uso do controle personalizado do Azure AD).

### <a name="how-to-submit-a-request-for-technical-exception"></a>Como enviar uma solicitação de exceção técnica

Para enviar uma solicitação de exceção técnica:

1. Faça logon no Partner Center como administrador global ou agente de administração.
2. Crie uma nova solicitação de serviço de parceiro navegando para **dar suporte** a **solicitações de suporte de parceiros** → e clicando em **nova solicitação**.
4. No tópico **MFA e modelo de aplicativo seguro** , selec **Enviar solicitação de exceção técnica** como o tipo de problema.
6. Forneça detalhes solicitados para enviar uma solicitação de serviço para exceção técnica e clique em **Enviar**.

A Microsoft pode levar até 3 dias úteis para fornecer uma resposta à solicitação de exceção técnica.
