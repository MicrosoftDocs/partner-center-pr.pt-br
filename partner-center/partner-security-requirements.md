---
title: Requisitos de segurança de parceiros | Partner Center
ms.topic: article
ms.date: 06/25/2019
description: Saiba mais sobre os requisitos de segurança para consultores e parceiros participam do programa de provedor de soluções na nuvem.
author: isaiahwilliams
ms.author: iswillia
keywords: Do Azure Active Directory, o provedor de soluções de nuvem, o provedor de soluções de nuvem do programa, CSP, fornecedor de painel de controle, CPV, a autenticação multifator, MFA, proteja o modelo de aplicativo, o modelo de aplicativo seguro, segurança
ms.localizationpriority: medium
ms.openlocfilehash: 8f513b96619819cd6ba892625e47731170d22130
ms.sourcegitcommit: de88bb4cd994f1a106a5d02242261042958d4300
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/03/2019
ms.locfileid: "67549534"
---
# <a name="partner-security-requirements"></a>Requisitos de segurança de parceiro

**Aplica-se a**

- Todos os parceiros no programa de provedor de soluções de nuvem
  - Bill direto
  - Provedor indireto
  - Revendedor indireto
- Todos os fornecedores de painel de controle
- Todos os supervisores

Segurança e privacidade de clientes e parceiros são as principais prioridades para a Microsoft. Podemos continuar a ver um número crescente de ataques de segurança mais sofisticados, relacionadas principalmente às identidades comprometidas. Como os controles de prevenção desempenham um papel importante em uma estratégia geral de defesa para impedir ataques de segurança, começaremos aplicando um conjunto de requisitos de segurança obrigatórios para ajudar a proteger seus clientes e parceiros.

> [!NOTE]
> É altamente recomendável que todos os parceiros transacionar por meio de uma nuvem soberana (21Vianet, governo dos EUA e Alemanha) agirem e adotam esses novos requisitos de segurança imediatamente. No entanto, esses parceiros não são necessários para atender os novos requisitos de segurança em vigor em 1 de agosto de 2019. A Microsoft fornecerá detalhes adicionais sobre a imposição desses requisitos de segurança para nuvens soberanas no futuro.

## <a name="overview-of-the-requirements"></a>Visão geral dos requisitos

Todos os parceiros que estão participando no programa Cloud Solution Provider, fornecedores de painel de controle e parceiros do Advisor são necessárias para impor a autenticação multifator (MFA) para cada usuário, incluindo contas de serviço em seu locatário do parceiro. Isso pode ser feito habilitando duas [diretivas de linha de base do Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection). Diretivas de linha de base são um conjunto de políticas predefinidas que ajudam a proteger as organizações contra vários ataques comuns. Esses ataques comuns podem incluir phishing, reprodução e spray de senha. Diretivas de linha de base estão disponíveis em todas as edições do Azure Active Directory. Microsoft está disponibilizando essas políticas de proteção de linha de base para todas as pessoas para aumentar ainda mais clientes e parceiros implementar as práticas recomendadas de segurança de ponta.

As políticas de linha de dois base devem ser habilitadas são descritas na tabela a seguir.

|**Política**| |
|-----|-----|
|**Exigir MFA para administradores**|Habilitando a exigir MFA para os administradores política, exigirá que os usuários nas funções de administrador registrar para MFA usando o aplicativo autenticador. Depois que o registro de MFA for concluído, os administradores precisarão executar a MFA toda vez que entrarem no.|
|**Proteção do usuário final**|Proteção do usuário final é uma política de linha de base MFA com base em risco que protege todos os usuários em um diretório. A habilitação dessa política requer que todos os usuários se registrar para MFA usando o aplicativo autenticador. Os usuários podem ignorar o prompt de registro MFA por 14 dias, após o qual eles serão impedidos de entrar até que eles se registrar para MFA. Depois de registrado para MFA, os usuários serão solicitados para o MFA somente durante as tentativas de entrada arriscadas. Contas de usuário comprometidas são bloqueadas até que a senha é redefinida e eventos de risco foram ignorados.|

Quando essas políticas são habilitadas, cada usuário será capaz de utilizar o Azure MFA sem custo adicional. Se você estiver usando uma solução de terceiros, são necessárias para impor o MFA para cada usuário ao acessar serviços de nuvem Commercial da Microsoft.

> [!IMPORTANT]
> Uma vez que a MFA será imposta para todos os usuários no diretório de parceiros, haverá um impacto em qualquer automação ou integração que utiliza as credenciais do usuário. Para resolver esse impacto, você precisará modificar a forma como sua automação ou integração conecta-se aos serviços de nuvem comercial da Microsoft. Se o serviço que você está se conectando ao dá suporte à autenticação baseada em token e, em seguida, é recomendável que você implemente a [estrutura de modelo de aplicativo seguro](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model).

## <a name="what-actions-do-i-need-to-take"></a>As ações que é preciso levar? 

Para garantir que os usuários no locatário do parceiro são protegidos, você deve impor o MFA para cada usuário (incluindo contas de serviço). Isso pode ser feito habilitando o [exigir MFA para que os administradores](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) e [proteção do usuário final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) diretivas de linha de base. Antes de habilitar essas políticas, é importante entender o que eles fazem e como elas afetarão qualquer automação ou integração e seus usuários.

> [!NOTE]
> [Diretivas de linha de base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) continuará a evoluir com o tempo. É recomendável que você examine periodicamente a documentação para saber mais sobre a evolução das políticas.

### <a name="considerations"></a>Considerações

Como os requisitos de segurança se aplicam a todos os usuários em um diretório de parceiro, várias considerações precisam ser feitas para assegurar uma implantação tranquila. Essas considerações incluem a identificação de usuários no Active Directory do Azure que não pode ou não deve realizar a MFA, bem como aplicativos e clientes usados pela sua organização que não dão suporte a autenticação moderna.

#### <a name="self-service-password-reset"></a>Redefinição de Senha com Autoatendimento

Redefinição de senha de autoatendimento (SSPR) é um recurso do Azure Active Directory que permite que os funcionários redefinam suas senhas sem a necessidade de entrar em contato com a equipe de TI. Os funcionários devem se registrar para ou ser registrados para autoatendimento a redefinição de senha antes de usar o serviço. Durante o registro, o funcionário escolhe um ou mais métodos de autenticação habilitados pela sua organização.

SSPR permite que os funcionários rapidamente obter o desbloqueio e continuar trabalhando, independentemente de onde eles estão ou a hora do dia. Permitindo que os usuários desbloquear a mesmos, sua organização pode reduzir o tempo não produtivas e custos de suporte de alta dos problemas mais comuns relacionados à senha.

Quando o [proteção do usuário final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) política de linha de base está habilitada quaisquer contas de usuário comprometidas serão bloqueadas até que a senha é redefinida e eventos de risco foram ignorados. Considerando isso é recomendável que cada usuário, que é um administrador global, execute o seguinte para se registrar no SSPR

1. Navegue até o [página de configuração SSPR](https://aka.ms/ssprsetup)
2. Insira seu nome de usuário e senha
3. Configure pelo menos uma das opções de verificações que serão usadas para verificar quem você é ao redefinir sua senha.  

Quando uma conta tiver sido comprometida, um administrador precisará tomar medidas para restaurar o acesso para o usuário afetado. Consulte a [etapas para desbloquear um usuário](#recovering-compromised-accounts) para obter detalhes sobre o processo para desbloquear o usuário.

#### <a name="legacy-protocols"></a>Protocolos herdados

Protocolos de autenticação herdados (IMAP, SMTP, POP3, etc.) são usados por clientes de email para fazer solicitações de autenticação. Esses protocolos não oferecem suporte a MFA. Com muita frequência os comprometimentos de conta é causadas por atores ruins executar ataques contra protocolos herdados, a tentativa de ignorar o MFA. Para garantir que o MFA é exigido ao fazer logon em uma conta em um diretório de parceiros e atores ruins não são capazes de ignorar o MFA, esses requisitos de segurança bloqueará todas as solicitações de autenticação de protocolos herdados.

### <a name="enabling-the-baseline-policies"></a>Habilitar as diretivas de linha de base

Consulte a [Implementando o tutorial de requisitos de segurança de parceiro](tutorials/partner-security-requirements.yml) para uma experiência guiada sobre a implementação das diretivas de linha de base.  

#### <a name="require-mfa-for-admins"></a>Exigir MFA para administradores

O *exigir MFA para o administrador* política de linha de base exige o MFA para as seguintes funções de diretório, consideradas funções mais privilegiadas do Active Directory do Azure:

- Administrador global
- Administrador do SharePoint
- Administrador do Exchange
- Administrador de acesso condicional
- Administrador de segurança
- Administrador de assistência técnica / administrador de senha
- Administrador de cobrança
- Usuário administrador

Após a habilitação da exigir MFA para os administradores política, as funções de nove administrador acima precisará se registrar para MFA usando o aplicativo autenticador. Depois que o registro de MFA for concluído, os administradores precisarão executar a MFA toda vez que entrar.

Se sua organização tiver essas contas em uso no código ou scripts, considere a possibilidade de substituí-los com [identidades gerenciadas](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview).

Para habilitar essa política e proteger seus administradores:

1. Entrar para o **portal do Azure** como um Administrador Global, administrador de segurança ou administrador de acesso condicional.
2. Navegue até **do Azure Active Directory** > **acesso condicional**.
3. Na lista de políticas, selecione **política de linha de base: Exigir MFA para os administradores**.
4. Definir **habilitar política** à **usar a política imediatamente**.
5. Clique em **salvar**.

    ![Exigir MFA para administradores](images/security/baseline-policy-require-mfa-for-admins.png)

> [!WARNING]
> Antes de habilitar essa política, certifique-se de que os usuários não estiver usando protocolos de autenticação herdados. Consulte o artigo [como: Autenticação herdados do bloco para o Azure Active Directory com acesso condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth#identify-legacy-authentication-use) para obter mais informações.

> [!IMPORTANT]
> Há um problema conhecido, o que afeta a capacidade de se conectar ao Exchange Online PowerShell utilizar privilégios de administrador delegados. Consulte a [Exchange Online PowerShell](#exchange-online-powershell) conhecido problema antes de habilitar essa política se você usar este módulo do PowerShell.

#### <a name="end-user-protection"></a>Proteção do usuário final

A política de linha de base do usuário final proteção protege todos os usuários em um diretório. A habilitação dessa política requer que todos os usuários se registrar para MFA do Azure dentro de 14 dias. Depois de registrado, os usuários serão solicitados para o MFA somente durante as tentativas de entrada arriscadas. Contas de usuário comprometidas serão bloqueadas até que a redefinição de senha e corre o risco de exoneração.

A política **política de linha de base: Proteção do usuário final** vem pré-configurada e aparecerá na parte superior quando você navega até a folha de acesso condicional no portal do Azure.

Para habilitar essa política e proteger os usuários:

1. Entrar para o **portal do Azure** como um Administrador Global, administrador de segurança ou administrador de acesso condicional.
2. Navegue até **do Azure Active Directory** > **acesso condicional**.
3. Na lista de políticas, selecione **política de linha de base: Proteção do usuário final (versão prévia)** .
4. Definir **habilitar política** à **usar a política imediatamente**.
5. Clique em **salvar**.

    ![Proteção do usuário final](images/security/baseline-policy-end-user-protection.png)

> [!WARNING]
> Antes de habilitar essa política, certifique-se de que os usuários não estiver usando protocolos de autenticação herdados. Consulte o artigo [como: Autenticação herdados do bloco para o Azure Active Directory com acesso condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth#identify-legacy-authentication-use) para obter mais informações.

> [!IMPORTANT]
> Há um problema conhecido, que afeta a capacidade de se conectar ao Exchange Online PowerShell utilizar privilégios de administrador delegados. Consulte a [Exchange Online PowerShell](#exchange-online-powershell) conhecido problema antes de habilitar essa política se você usar este módulo do PowerShell.

## <a name="common-issues"></a>Problemas comuns

### <a name="azure-active-directory"></a>Azure Active Directory

#### <a name="aadsts50076"></a>AADSTS50076

Depois de habilitar as diretivas de linha de base, você pode achar que sua automação ou integração está encontrando uma exceção semelhante ao seguinte

    AADSTS50076: Due to a configuration change made by your administrator, or because you moved to a new location, you must use multi-factor authentication to access 'MyApp'.

O motivo para essa exceção é que você estiver autenticando usando credenciais de usuário e MFA agora é necessário. Para resolver essa exceção, você precisa utilizar um token de acesso para autenticação. Consulte a [guia do modelo de aplicativo seguro](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) para obter mais informações.

>[!IMPORTANT]
>Módulos do PowerShell e APIs mais modernos dão suporte a capacidade de utilizar um token de acesso para autenticação. No entanto, há alguns que atualmente não dão suporte a essa funcionalidade. Se você precisar de ajuda para determinar se o módulo do PowerShell ou a API que você está tentando utilizar suporta o uso de um token de acesso para autenticação, em seguida, postar uma mensagem sobre o [grupo de diretrizes de segurança do Partner Center](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) comunidade.

#### <a name="aadsts700082"></a>AADSTS700082

Depois que você tiver implementado a estrutura de modelo de aplicativo seguro é provável que você receberá a seguinte exceção 90 dias depois de gerar o token de atualização inicial

    The refresh token has expired due to inactivity. The token was issued on 2019-01-02T09:19:53.5422744Z and was inactive for 90.00:00:00

Em relação ao Azure Active Directory o tempo de vida máximo para uma atualização de token é de 90 dias. Para resolver esse erro, você precisará gerar e armazenar com segurança um novo token de atualização. Observe que é possível atualizar o token de atualização por meio de programação porque com cada solicitação para o Azure Active Directory para um token de acesso um novo token de atualização é retornado. Você pode implementar a lógica apropriada para atualizar o token de atualização armazenados com segurança antes de expirar.

Ver [tempos de vida de token configuráveis no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) para obter mais informações.

### <a name="recovering-compromised-accounts"></a>Recuperando contas comprometidas

Para ajudar a proteger nossos clientes, o serviço de credenciais vazadas da Microsoft localiza pares de nome de usuário/senha publicamente disponíveis. Se elas corresponderem a um dos nossos usuários, ajudamos a proteger essa conta imediatamente. Usuários identificados como tendo uma credencial vazada forem confirmados comprometida. Esses usuários serão impedidos de entrar até que a senha é redefinida.

Os usuários atribuídos a uma licença do Azure AD Premium podem restaurar o acesso por meio de redefinição de senha de autoatendimento (SSPR) se o recurso estiver habilitado em seu diretório. Os usuários sem uma licença premium que tornam-se bloqueado devem contatar um administrador para executar uma redefinição de senha manual e ignorar o evento de risco do usuário sinalizado.

#### <a name="steps-to-unblock-a-user"></a>Etapas para desbloquear um usuário

Confirme que o usuário foi bloqueado pela política, examinando os logs de entrada do usuário.

1. Um administrador precisa entrar para o **portal do Azure** e navegue até **Azure Active Directory** > **usuários** > clique no nome do usuário e navegar para entradas.
2. Para iniciar a redefinição de senha em um usuário bloqueado, um administrador precisa navegar até **Azure Active Directory** > **usuários sinalizados para risco**
3. Clique no usuário cuja conta está bloqueada para exibir informações sobre a atividade de entrada recentes do usuário.
4. Clique em Redefinir a senha para atribuir uma senha temporária que deve ser alterada após o próximo logon.
5. Clique em Descartar todos os eventos para redefinir a pontuação de risco do usuário.

O usuário agora pode entrar, redefina a senha e acessar o aplicativo.

## <a name="known-issues"></a>Problemas conhecidos

### <a name="exchange-online-powershell"></a>PowerShell do Exchange Online

Quando a MFA está habilitada parceiros não poderá utilizar seus privilégios administrativos delegados com o PowerShell do Exchange Online para executar ações em relação a seus clientes. Ver [conectar-se ao Exchange Online PowerShell usando a autenticação multifator](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell) para obter mais informações sobre essa limitação.

## <a name="resources-and-support"></a>Recursos e suporte

Por meio de [comunidade do grupo de diretrizes de segurança do Partner Center](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) você pode encontrar recursos adicionais e saiba mais sobre eventos futuros, como o horário de expediente técnica. Consulte a [perguntas frequentes](http://assetsprod.microsoft.com/security-requirements-faq.pdf) documento para saber mais sobre os requisitos.

### <a name="developers"></a>Desenvolvedores

- [Habilitando o modelo de aplicativo seguro](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [Exemplos de .NET do Partner Center](https://github.com/microsoft/partner-center-dotnet-samples)
- [Exemplos de Java do Partner Center](https://github.com/microsoft/partner-center-java-samples)
- [PowerShell do Partner Center Implementando o modelo de aplicativo seguro](https://docs.microsoft.com/powershell/partnercenter/secure-app-model)
