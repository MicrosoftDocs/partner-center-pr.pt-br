---
title: Requisitos de segurança do parceiro | Partner Center
ms.topic: article
ms.date: 08/30/2019
description: Saiba mais sobre os requisitos de segurança para consultores e parceiros que participam do programa de Provedor de Soluções na Nuvem.
author: isaiahwilliams
ms.author: iswillia
keywords: O Azure Active Directory, provedor de soluções na nuvem, programa de provedor de soluções na nuvem, CSP, fornecedor do painel de controle, CPV, autenticação multifator, MFA, modelo de aplicativo seguro, modelo de aplicativo seguro, segurança
ms.localizationpriority: medium
ms.openlocfilehash: c95ec38f928ca4032ffecebaf25f23e87d10c079
ms.sourcegitcommit: de3cdc792b6b4bbc64d1288d371623d79d535205
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/03/2019
ms.locfileid: "70215645"
---
# <a name="partner-security-requirements"></a>Requisitos de segurança de parceiros

**Aplica-se a**

- Todos os parceiros no programa Provedor de Soluções na Nuvem
  - Fatura direta
  - Provedor indireto
  - Revendedor indireto
- Todos os Fornecedores do Painel de Controle
- Todos os consultores

As maiores proteções de privacidade e segurança estão entre nossas principais prioridades. Sabemos que a melhor defesa é a prevenção e que somos tão fortes quanto nosso vínculo mais fraco. É por isso que precisamos de todos em nosso ecossistema, para agir e garantir que eles tenham proteções de segurança adequadas implantadas. Para ajudar a proteger parceiros e clientes, estamos introduzindo um conjunto de requisitos de segurança obrigatórios para consultores, fornecedores do painel de controle e parceiros que participam do programa de Provedor de Soluções na Nuvem.

A partir de 1º de agosto de 2019, todos os parceiros precisam impor a autenticação multifator para os usuários, incluindo contas de serviço, em seu locatário de parceiro.

> [!NOTE]
> É altamente recomendável que todos os parceiros que negociam em uma nuvem soberana (21Vianet, governo dos EUA e Alemanha) atuem e adotem esses novos requisitos de segurança imediatamente. No entanto, esses parceiros não precisam atender aos novos requisitos de segurança em vigor em 1º de agosto de 2019. Futuramente, a Microsoft fornecerá detalhes adicionais sobre a imposição desses requisitos de segurança para nuvens soberanas.

Os termos associados aos requisitos de segurança do parceiro foram adicionados ao guia [do programa do Provedor de Soluções na Nuvem](https://go.microsoft.com/fwlink/p/?LinkId=617100). A partir de 1º de agosto de 2019, todos os parceiros que participam do programa do Provedor de Soluções na Nuvem devem estar em conformidade com os termos. Como ele é relacionado aos consultores, os mesmos requisitos contratuais estarão em vigor.

Os parceiros que não implementarem os requisitos de segurança obrigatórios não poderão fazer transações no programa de Provedor de Soluções na Nuvem nem gerenciar locatários de clientes que utilizam direitos de administrador delegado, pois esses requisitos são impostos. Estamos no processo de estabelecer uma data de imposição técnica para os requisitos e notificaremos a data aos parceiros com informações detalhadas.

## <a name="what-actions-do-i-need-to-take"></a>Quais ações preciso adotar?

Considerando a natureza altamente privilegiada de um parceiro, precisamos garantir que cada usuário tenha um desafio de MFA para cada autenticação única. Isso pode ser feito por uma das seguintes maneiras

- Implementar Azure AD Premium e garantir que a MFA seja imposta para cada usuário
- Implementar [as políticas de proteção de linha de base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)
- Implementar a solução de terceiros e garantir que a MFA seja imposta para cada usuário

> [!IMPORTANT]
> Depois que esses requisitos são tecnicamente impostos, cada autenticação única deve ter um desafio de MFA. Você não poderá usar recursos de acesso condicional para evitar a autenticação usando a MFA ao acessar os serviços de nuvem comercial da Microsoft.

### <a name="considerations"></a>Considerações

Como esses requisitos se aplicam a todos os usuários, incluindo contas de serviço, em seu locatário do parceiro há várias considerações que precisam ser feitas para garantir uma implantação tranquila. Essas considerações incluem a identificação de usuários no Azure AD que não podem executar a MFA, bem como aplicativos e dispositivos usados pela sua empresa que não dão suporte à autenticação moderna.

Antes de executar qualquer ação, é recomendável que você identifique o seguinte

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-mfa-when-authenticating"></a>Você tem um aplicativo ou dispositivo que não dá suporte ao uso de MFA durante a autenticação?

Quando você impõe a autenticação herdada de MFA, o uso de protocolos como IMAP, POP3, SMTP etc. será bloqueado porque esses protocolos não dão suporte à MFA. Para resolver essa limitação, um recurso conhecido como [senhas de aplicativo](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) pode ser usado para garantir que o aplicativo ou dispositivo ainda possa ser autenticado. Você deve examinar as considerações para usar senhas de aplicativo documentadas [aqui](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) para determinar se elas podem ser usadas em seu ambiente.

#### <a name="do-you-have-users-using-office-365-provided-by-licenses-associated-with-your-partner-tenant"></a>Você tem usuários usando o Office 365 fornecido por licenças associadas ao seu locatário do parceiro?

Antes de implementar qualquer solução, é recomendável que você determine por que a versão do Microsoft Office está sendo usada pelos usuários em seu locatário do parceiro. Analise [o plano de autenticação multifator para implantações do Office 365](https://docs.microsoft.com/office365/admin/security-and-compliance/multi-factor-authentication-plan#enable-mfa) antes de realizar qualquer ação. Há uma chance de que os usuários tenham problemas de conectividade com aplicativos como o Outlook. Antes de impor a MFA, é importante garantir que o Outlook 2013 SP1, ou posterior, esteja sendo usado e que sua empresa tenha a autenticação moderna habilitada. Consulte [Habilitar a autenticação moderna no Exchange Online](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online) para obter mais informações.

Para habilitar a autenticação moderna para todos os dispositivos que executam o Windows, com o Microsoft Office 2013 instalado, será necessário criar duas chaves do registro. Consulte [Habilitar a autenticação moderna para o Office 2013 em](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)dispositivos Windows.

> [!IMPORTANT]
> Se você tiver habilitado seus usuários para a MFA do Azure AD e eles tiverem dispositivos que executam o Office 2013 que não estão habilitados para autenticação moderna, eles precisarão usar senhas de aplicativo nesses dispositivos. Mais informações sobre senhas de aplicativo e quando/onde/como elas devem ser usadas podem ser encontradas aqui: [Senhas de aplicativo com a autenticação multifator do Microsoft Azure](https://go.microsoft.com/fwlink/p/?LinkId=528178).

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>Há uma política que impede que qualquer usuário use seus dispositivos móveis enquanto trabalha?

É importante identificar qualquer política corporativa que impeça que os funcionários usem dispositivos móveis enquanto trabalham, porque isso influenciará a solução de MFA que você implementará. Há soluções de MFA, como a fornecida pela implementação das políticas de [proteção de linha de base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection), que permitem apenas o uso de um aplicativo autenticador para verificação. Caso sua empresa tenha uma política que impeça o uso de dispositivos móveis, você deve considerar uma das seguintes opções

- Implantar um aplicativo com senha TOTP (senha única baseada em tempo) que pode ser executado no sistema seguro
- Implemente uma solução de terceiros que impõe a MFA para cada usuário no locatário do parceiro com a opção de verificação mais apropriada
- Comprar licenças do [Azure AD Premium](https://azure.microsoft.com/pricing/details/active-directory/) para os usuários afetados

O suporte para o uso de chaves de segurança FIDO está no roteiro para as políticas de proteção de linha de base. Depois que o suporte tiver sido adicionado, você poderá aproveitar as chaves de segurança FIDO para o segundo fator de autenticação. Até então, você estará limitado ao uso do aplicativo autenticador.

#### <a name="what-automation-or-integration-do-you-have-that-leverages-user-credentials-for-authentication"></a>Qual automação ou integração você tem para aproveitar as credenciais do usuário para autenticação?

Como o requisito é impor a MFA para cada usuário, incluindo contas de serviço, em seu diretório de parceiro, qualquer automação ou integração que aproveita as credenciais do usuário para autenticação será afetada. Portanto, é importante que você identifique quais contas são usadas nessas situações. Veja a seguir uma lista de exemplos de aplicativos ou serviços que devem ser considerados

- Painel de controle usado para provisionar recursos em nome de seus clientes
- Integração com qualquer plataforma usada para faturamento (pois está relacionada ao programa CSP) e suporte aos seus clientes
- Scripts do PowerShell que utilizam os módulos AZ, AzureRM, Azure AD, MS online etc.

A lista acima não é abrangente. Portanto, é importante que você execute uma avaliação completa de qualquer aplicativo ou serviço em seu ambiente, que aproveite as credenciais do usuário para autenticação. Para lidar com o requisito de MFA, você deve implementar a orientação na [ estrutura de Modelo de Aplicativo Seguro ](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model), sempre que possível. A seguir, estão os recursos adicionais que ajudarão você a entender como a estrutura de Modelo de Aplicativo Seguro pode ser implementada

- [Amostras .NET do Partner Center](https://github.com/microsoft/partner-center-dotnet-samples) - Esse repositório GitHub contém amostras desenvolvidas usando o .NET, que demonstrarão como você pode implementar a estrutura do Modelo de Aplicativo Seguro.
- [Amostras Java do Partner Center](https://github.com/microsoft/partner-center-java-samples) - Esse repositório GitHub contém amostras desenvolvidas usando o Java, que demonstrarão como você pode implementar a estrutura do Modelo de Aplicativo Seguro.
- [PowerShell do Partner Center – Modelo de Aplicativo Seguro](https://docs.microsoft.com/powershell/partnercenter/secure-app-model) – Este é um artigo que fornece detalhes sobre como implementar a estrutura de Modelo de Aplicativo Seguro usando o PowerShell.
- [Comunidade do grupo de orientação de segurança do Partner Center](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)  – Esta é uma comunidade online na qual você pode aprender sobre eventos futuros e tirar dúvidas.

### <a name="enforcing-mfa-for-all-users"></a>Impondo MFA para todos os usuários

Esta seção abordará como você pode usar as [políticas de proteção de linha de base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) para impor a MFA para cada usuário, incluindo contas de serviço, em seu locatário de parceiro. Se você estiver planejando usar o Azure AD Premium, siga as etapas documentadas [aqui.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted)

> [!NOTE]
> Uma solução de terceiros, que é compatível com o Azure AD, pode ser usada para impor a MFA para todos os usuários, incluindo contas de serviço. Consulte a documentação do fornecedor para obter mais detalhes sobre como a solução deve ser implementada.

As políticas de proteção de linha de base são um conjunto de políticas predefinidas que ajudam a proteger as empresas contra muitos ataques comuns. Esses ataques comuns podem incluir pulverização, reprodução e phishing de senha. As políticas de proteção de linha de base estão disponíveis em todas as edições do Azure Active Directory. A Microsoft está disponibilizando essas políticas de proteção de linha de base a todos, para permitir que os clientes e parceiros implementem as melhores práticas de segurança.

As duas políticas de proteção de linha de base que devem ser habilitadas são descritas na tabela a seguir.

|**Política**| |
|-----|-----|
|**Exigir MFA para administradores**|Habilitar a política de Exigir MFA para administradores fará com que os usuários nas funções de administrador se registrem para MFA usando o aplicativo autenticador. Depois que o registro de MFA for concluído, os administradores precisarão executar a MFA sempre que entrarem.|
|**Proteção do usuário final**|A proteção do usuário final é uma política de proteção de linha de base da MFA, baseada em risco, que protege todos os usuários em um diretório. A habilitação dessa política exige que todos os usuários se registrem na MFA usando o aplicativo autenticador. Os usuários podem ignorar o prompt de registro de MFA por 14 dias, após o qual eles serão impedidos de entrar até que se registrem na MFA. Depois de registrado para MFA, os usuários serão solicitados a receber MFA somente durante tentativas de inserção de credenciais arriscadas. As contas de usuário comprometidas são bloqueadas até que a senha seja redefinida e os eventos de risco tenham sido ignorados.|

Quando essas políticas estiverem habilitadas, cada usuário poderá utilizar A MFA do Azure usando o aplicativo autenticador para verificação sem custo adicional.

#### <a name="configure-self-service-password-reset"></a>Configurar a Redefinição de Senha com Autoatendimento

A redefinição de senha de autoatendimento (SSPR) é um recurso do Azure Active Directory que permite que os usuários redefinam suas senhas sem precisar entrar em contato com a equipe de suporte. Os usuários devem se registrar ou ser registrados para redefinição de senha de autoatendimento antes de usar o serviço. Durante o registro, o usuário escolhe um ou mais métodos de autenticação habilitados pela empresa.

Quando a [política de proteção de usuário final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) de linha de base estiver habilitada, todas as contas de usuário comprometidas serão bloqueadas até que sua senha seja redefinida e os eventos de risco tenham sido descartados. Considerando isso, é recomendável que cada usuário administrador global execute o seguinte para se registrar no SSPR para que eles não sejam bloqueados.

1. Navegue até a [página de instalação do SSPR](https://aka.ms/ssprsetup)
2. Digite seu nome de usuário e senha
3. Configure pelo menos uma das opções de verificações que serão usadas para verificar quem é você ao redefinir sua senha.  

Quando uma conta tiver sido comprometida, um administrador precisará tomar medidas para restaurar o acesso ao usuário afetado. Consulte as [etapas para desbloquear um usuário](#recovering-compromised-accounts) para obter detalhes sobre o processo para desbloquear o usuário.

#### <a name="require-mfa-for-admins"></a>Exigir MFA para administradores

A política *Exigir MFA para administrador* requer MFA para as funções de diretório a seguir, consideradas como as funções de Azure Active Directory mais privilegiadas:

- Administrador global
- Administrador do SharePoint
- Administradores do Exchange
- Administrador de acesso condicional
- Administrador de segurança
- Administrador de assistência técnica/administrador de senha
- Administrador de cobrança
- Administrador do usuário

Ao habilitar a política de Exigir MFA para administradores, as nove funções de administrador acima exigirá o registro para MFA usando o aplicativo autenticador. Depois que o registro de MFA for concluído, os administradores precisarão executar a MFA sempre que entrarem.

Se sua empresa tiver essas contas em uso em scripts ou código, considere substituí-las [por identidades gerenciadas](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview).

Para habilitar essa política e proteger seus administradores:

1. Entre no **portal do Azure** como administrador global, administrador de segurança ou administrador de acesso condicional.
2. Navegue até o **Azure Active Directory** > **Acesso Condicional**.
3. Na lista de políticas, selecione a **política de linha de base: Exigir a MFA para Administradores**.
4. Defina **Habilitar política** para **Usar política imediatamente**.
5. Clique em  **Salvar**.

> [!WARNING]
> Antes de habilitar essa política, verifique se os usuários não estão usando protocolos de autenticação herdados. Com a implementação desta política, a autenticação herdada será bloqueada.

> [!IMPORTANT]
> Há um problema conhecido que afeta sua capacidade de se conectar ao PowerShell do Exchange Online usando privilégios administrativos delegados. Consulte o problema conhecido do[PowerShell do Exchange Online](#exchange-online-powershell) antes de habilitar essa política se você estiver usando este módulo do PowerShell.

#### <a name="end-user-protection"></a>Proteção do usuário final

A política de linha de base de proteção do usuário final protege todos os usuários em um diretório. A habilitação dessa política exige que todos os usuários se registrem na MFA do Azure em até 14 dias. Depois de registrados para MFA, os usuários serão solicitados a receber MFA somente durante tentativas de inserção de credenciais arriscadas. Contas de usuário comprometidas são bloqueadas até a redefinição de senha e risco de demissão.

A **Política de linha de base: proteção de usuário final** vem pré-configurado e aparecerá na parte superior quando você navegar para a folha Acesso Condicional no portal do Azure.

Para habilitar essa política e proteger seus usuários:

1. Entre no **portal do Azure** como administrador global, administrador de segurança ou administrador de acesso condicional.
2. Navegue até o **Azure Active Directory** > **Acesso Condicional**.
3. Na lista de políticas, selecione a **política de linha de base: Proteção do usuário final (visualização)** .
4. Defina **Habilitar política** para **Usar política imediatamente**.
5. Clique em  **Salvar**.

> [!WARNING]
> Antes de habilitar essa política, verifique se os usuários não estão usando protocolos de autenticação herdados. Com a implementação desta política, a autenticação herdada será bloqueada.

> [!IMPORTANT]
> Há um problema conhecido que afeta sua capacidade de se conectar ao PowerShell do Exchange Online usando privilégios administrativos delegados. Consulte o problema conhecido do[PowerShell do Exchange Online](#exchange-online-powershell) antes de habilitar essa política se você estiver usando este módulo do PowerShell.

## <a name="assessing-your-environment"></a>Avaliação do seu ambiente

Com um dos requisitos atuais de segurança do parceiro, você precisa ter a MFA aplicada para cada usuário em seu locatário parceiro. Como esse requisito pode ser cumprido com vários métodos diferentes, pode ser difícil avaliar se são necessárias ações adicionais. Você pode aproveitar ferramentas como os logs de auditoria do Azure Active Directory e [ Microsoft Secure Score ](https://docs.microsoft.com/office365/securitycompliance/microsoft-secure-score) para avaliar se são necessárias ações adicionais para proteger seu locatário com a MFA. A Microsoft está trabalhando em uma experiência no Partner Center para fornecer uma verificação rápida de conformidade nos requisitos de MFA e do Modelo de Aplicativo Seguro.

O Microsoft Secure Score oferece visualizações robustas, integração com outros produtos da Microsoft, comparação de sua pontuação com outras empresas, filtragem por categoria e muito mais. Com essa ferramenta, você pode concluir as ações de melhoria de segurança em sua organização e acompanhar o histórico de sua pontuação. A pontuação também pode refletir quando soluções de terceiros tiverem resolvido as ações de aperfeiçoamento recomendadas.

![Classificação de Segurança da Microsoft](images/security/secure-score.png)

> [!NOTE]
> As ações que você pode tomar para melhorar a classificação de segurança da Microsoft podem levar até 24 horas para serem refletidas.

A Classificação de Segurança da Microsoft fornecerá apenas uma representação numérica da sua postura de segurança. Para entender melhor o que ou quem está autenticando sem precisar fornecer a MFA, é recomendável consultar os logs de auditoria do Azure Active Directory. Isso pode ser feito usando o módulo[PowerShell do Azure](https://docs.microsoft.com/powershell/azure/overview) e o script abaixo. Ele gerará um relatório que fornece informações sobre quais tentativas de autenticação ocorreram no último dia que não necessitaram de MFA.

```powershell
Login-AzAccount
$context = Get-AzContext

function Get-SignInEvents
{
    param([string]$userId)

    $content = '{"startDateTime":"' + (Get-Date).AddDays(-1).ToUniversalTime().ToString("yyyy-MM-ddT05:00:00.000Z") + '","endDateTime":"' + (Get-Date).ToUniversalTime().ToString("yyyy-MM-ddTHH:mm:ss.fffZ")  + '","userId":"' + $userId +'","riskState":[],"totalRisk":[],"realtimeRisk":[],"tokenIssuerType":[],"isAdfsEnabled":false}'

    $token = [Microsoft.Azure.Commands.Common.Authentication.AzureSession]::Instance.AuthenticationFactory.Authenticate($context.Account, $context.Environment, $context.Tenant.Id, $null, "Never", $null, "74658136-14ec-4630-ad9b-26e160ff0fc6")

    $headers = @{
    'Authorization' = 'Bearer ' + $token.AccessToken
    'Content-Type' = 'application/json'
        'X-Requested-With'= 'XMLHttpRequest'
        'x-ms-client-request-id'= [guid]::NewGuid()
        'x-ms-correlation-id' = [guid]::NewGuid()
    }

    Invoke-RestMethod -Body $content -Header $headers -Method POST -Uri "https://main.iam.ad.ext.azure.com/api/Reports/SignInEventsV3"
}

$report = $()

Get-AzADUser | foreach {
    $events = Get-SignInEvents $_.Id
    $report += $events.Items
}

$report | Where-Object {$_.mfaRequired -eq $false} | Select-Object userPrincipalName, userDisplayName, createdDateTime, resourceDisplayName, loginSucceeded, failureReason, mfaRequired, mfaAuthMethod, mfaAuthDetail, mfaResult, @{Name='policies'; Expression={[string]::join(',', $($_.conditionalAccessPolicies | Select-Object displayName).displayName )}}, conditionalAccessStatus | Export-Csv report.csv
```

Depois de executar o script acima, os detalhes estarão disponíveis no arquivo Report.csv. Ele conterá uma lista de tentativas de autenticação que ocorreram no último dia em que o usuário não precisou de MFA. Será necessário examinar cada entrada para determinar se esse é o comportamento esperado e agir, se necessário.

![Relatório de avaliação](images/security/assessment-report.png)

## <a name="common-issues"></a>Problemas comuns

### <a name="azure-active-directory"></a>Azure Active Directory

#### <a name="aadsts50076"></a>AADSTS50076

Depois de habilitar as políticas de linha de base, você pode descobrir que há uma exceção abaixo na automação ou integração

    AADSTS50076: Due to a configuration change made by your administrator, or because you moved to a new location, you must use multi-factor authentication to access 'MyApp'.

A razão para essa exceção é que você está autenticando usando credenciais de usuário e a MFA agora é necessária. Para resolver essa exceção, você precisará utilizar um token de acesso para autenticação. Consulte o [guia do Modelo de Aplicativo Seguro](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) para obter mais informações.

>[!IMPORTANT]
>Os módulos de APIs e PowerShell mais modernos utilizam um token de acesso para autenticação. No entanto, alguns ainda não dão suporte a essa funcionalidade. Se você precisar de ajuda para determinar se o módulo da API ou do PowerShell que você está tentando utilizar dá suporte ao uso de um token de acesso para autenticação, publique uma mensagem na Comunidade [Partner Center Security Guidance Group](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance).

#### <a name="aadsts700082"></a>AADSTS700082

Depois de implementar a estrutura de modelo de aplicativo seguro, há uma chance de que você receba a seguinte exceção 90 dias depois de gerar o token de atualização inicial

    The refresh token has expired due to inactivity. The token was issued on 2019-01-02T09:19:53.5422744Z and was inactive for 90.00:00:00

Com relação ao Azure Active Directory, o tempo de vida máximo de um token de atualização é de 90 dias. Para resolver esse erro, será necessário gerar e armazenar com segurança um novo token de atualização. Observe que é possível atualizar o token de atualização programaticamente porque, com cada solicitação de um token de acesso ao Azure Active Directory, um novo token de atualização é retornado. Você pode implementar a lógica apropriada para atualizar o token de atualização armazenado com segurança antes que ele expire.

Consulte [Tempos de vida de tokens configuráveis no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) para obter mais informações.

### <a name="recovering-compromised-accounts"></a>Recuperando contas comprometidas

Para ajudar a proteger nossos clientes, o serviço de credenciamento vazado da Microsoft encontra pares de nome de usuário/senha disponíveis publicamente. Se eles corresponderem a um de nossos usuários, ajudaremos a proteger essa conta imediatamente. Os usuários identificados como tendo uma credencial vazada são confirmados como comprometidos. Esses usuários serão impedidos de entrar até que a senha seja redefinida.

Os usuários com uma licença Azure AD Premium podem restaurar o acesso com a redefinição de senha por autoatendimento (SSPR) se a funcionalidade estiver habilitada em seu diretório. Os usuários bloqueados sem uma licença Premium devem entrar em contato com um administrador para executar uma redefinição manual de senha e ignorar o evento de risco de usuário sinalizado.

#### <a name="steps-to-unblock-a-user"></a>Para desbloquear um usuário

Confirme se o usuário foi bloqueado pela política examinando os logs de entrada do usuário.

1. Um administrador precisa entrar no **portal do Azure** e navegar até **Azure Active Directory** > **Usuários** > clicar no nome do usuário e navegar até as Credenciais.
2. Para iniciar a redefinição de senha em um usuário bloqueado, um administrador precisa navegar até **Azure Active Directory** > **Usuários sinalizados para risco**
3. Clique no usuário, cuja conta está bloqueada, para exibir informações sobre a atividade de entrada recente do usuário.
4. Clique em Redefinir Senha para atribuir uma senha temporária que deve ser alterada no próximo logon.
5. Clique em Ignorar todos os eventos para redefinir a classificação de risco do usuário.

Agora, o usuário pode entrar, redefinir sua senha e acessar o aplicativo.

## <a name="known-issues"></a>Problemas conhecidos

### <a name="exchange-online-powershell"></a>PowerShell do Exchange Online

Quando a MFA é imposta, os parceiros não poderão utilizar seus privilégios administrativos delegados com o PowerShell do Exchange Online para executar ações em seus clientes. Confira [Conectar-se ao PowerShell do Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell) usando a autenticação multifator para obter mais informações sobre essa limitação.

Você pode contornar essa limitação criando uma nova conta e nunca usá-la para executar uma autenticação interativa. É recomendável que você utilize o [PowerShell do Azure AD](https://docs.microsoft.com/powershell/module/azuread/) para criar a nova conta e executar a configuração inicial. O PowerShell a seguir pode ser usado para criar e configurar a conta

```powershell
Import-Module AzureAD
Connect-AzureAD

$PasswordProfile = New-Object -TypeName Microsoft.Open.AzureAD.Model.PasswordProfile

$PasswordProfile.Password = "Password"
$PasswordProfile.ForceChangePasswordNextLogin = $false

$user = New-AzureADUser -DisplayName "New User" -PasswordProfile $PasswordProfile -UserPrincipalName "NewUser@contoso.com" -AccountEnabled $true

# Uncomment the following two lines if you want the account to have Admin Agent privileges
# $adminAgentsGroup = Get-AzureADGroup -Filter "DisplayName eq 'AdminAgents'"
# Add-AzureADGroupMember -ObjectId $adminAgentsGroup.ObjectId -RefObjectId $user.ObjectId
```

Na próxima vez que você se conectar ao Exchange Online com o PowerShell, use essa conta, ela funcionará conforme o esperado.

> [!IMPORTANT]
> A habilidade dos parceiros utilizarem seus privilégios administrativos delegados com o PowerShell do Exchange Online para executar ações em seus clientes, quando a MFA é imposta, estará disponível no futuro. Até lá, você deve aproveitar essa solução alternativa.

## <a name="resources-and-support"></a>Recursos e suporte

Com a Comunidade [Partner Center Security Guidance Group](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance), você poderá encontrar recursos adicionais e aprender sobre eventos futuros, como horas úteis técnicas. Consulte o documento de [perguntas frequentes](partner-security-requirements-faq.md) para saber mais sobre os requisitos.
