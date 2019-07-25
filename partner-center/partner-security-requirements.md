---
title: Requisitos de segurança do parceiro | Centro de parceiros
ms.topic: article
ms.date: 07/18/2019
description: Saiba mais sobre os requisitos de segurança para consultores e parceiros que participam do programa do provedor de soluções na nuvem.
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, provedor de soluções na nuvem, programa de provedor de soluções na nuvem, CSP, fornecedor do painel de controle, CPV, autenticação multifator, MFA, modelo de aplicativo seguro, modelo de aplicativo seguro, segurança
ms.localizationpriority: medium
ms.openlocfilehash: 0ce8a8dd5a58d1647c8d9e53dec0d0bbf7fe6592
ms.sourcegitcommit: 5c8ac1b6d29d183d85582d6eb32e37b91dd8c6c1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2019
ms.locfileid: "68313932"
---
# <a name="partner-security-requirements"></a>Requisitos de segurança do parceiro

**Aplica-se a**

- Todos os parceiros no programa de provedor de soluções na nuvem
  - Fatura direta
  - Provedor indireto
  - Revendedor indireto
- Todos os fornecedores do painel de controle
- Todos os consultores

As maiores proteções de privacidade e segurança estão entre nossas principais prioridades. Sabemos que a melhor defesa é a prevenção e que somos tão fortes quanto nosso link mais fraco. É por isso que precisamos de todos em nosso ecossistema para agir e garantir que eles tenham proteções de segurança adequadas em vigor. Para ajudar a proteger parceiros e clientes, estamos introduzindo um conjunto de requisitos de segurança obrigatórios para consultores, fornecedores do painel de controle e parceiros que participam do programa do provedor de soluções na nuvem.

A partir de 1º de agosto de 2019, todos os parceiros precisam impor a autenticação multifator para todos os usuários, incluindo contas de serviço, em seu locatário de parceiro.

> [!NOTE]
> É altamente recomendável que todos os parceiros transagindo por uma nuvem soberanas (21Vianet, governo dos EUA e Alemanha) atuem e adotem esses novos requisitos de segurança imediatamente. No entanto, esses parceiros não precisam atender aos novos requisitos de segurança em vigor em 1º de agosto de 2019. A Microsoft fornecerá detalhes adicionais sobre a imposição desses requisitos de segurança para nuvens soberanas no futuro.

Os termos associados aos requisitos de segurança do parceiro foram adicionados ao [Guia do programa do provedor de soluções na nuvem](https://go.microsoft.com/fwlink/p/?LinkId=617100). A partir de 1º de agosto de 2019, todos os parceiros que participam do programa do provedor de soluções na nuvem devem estar em conformidade com os termos. Como ele se relaciona aos consultores, os mesmos requisitos contratuais estarão em vigor.

Os parceiros que não implementam os requisitos de segurança obrigatórios não poderão fazer transações no programa provedor de soluções na nuvem nem gerenciar locatários de clientes que utilizam direitos de administrador delegado, uma vez que esses requisitos são impostos. Estamos no processo de estabelecer uma data de imposição técnica para os requisitos e notificaremos os parceiros da data com informações detalhadas.

## <a name="what-actions-do-i-need-to-take"></a>Quais ações preciso tomar?

Considerando a natureza altamente privilegiada de ser um parceiro, precisamos garantir que cada usuário tenha um desafio de MFA para cada autenticação única. Isso pode ser feito por meio de uma das seguintes maneiras

- Implementar Azure AD Premium e garantir que a MFA seja imposta para cada usuário
- Implementando as [políticas de proteção de linha de base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)
- Implementar uma solução de terceiros e garantir que a MFA seja imposta para cada usuário

> [!IMPORTANT]
> Depois que esses requisitos são tecnicamente impostos, cada autenticação única deve ter um desafio de MFA. Você não poderá usar nenhum recurso de acesso condicional para evitar a autenticação usando o MFA ao acessar os serviços de nuvem comercial da Microsoft.

### <a name="considerations"></a>Considerações

Como esses requisitos se aplicam a todos os usuários, incluindo contas de serviço, em seu locatário do parceiro, há várias considerações que precisam ser feitas para garantir uma implantação tranqüila. Essas considerações incluem a identificação de usuários no Azure AD que não podem executar MFA, bem como aplicativos e dispositivos usados por sua organização que não dão suporte à autenticação moderna.

Antes de executar qualquer ação, é recomendável que você identifique o seguinte

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-mfa-when-authenticating"></a>Você tem um aplicativo ou dispositivo que não dá suporte ao uso de MFA durante a autenticação?

Quando você impõe a autenticação herdada de MFA, o uso de protocolos como IMAP, POP3, SMTP, etc. será bloqueado porque esses protocolos não dão suporte a MFA. Para resolver essa limitação, um recurso conhecido como [senhas de aplicativo](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) pode ser usado para garantir que o aplicativo ou dispositivo ainda possa se autenticar. Você deve examinar as considerações para usar senhas de aplicativo documentadas [aqui](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) para determinar se elas podem ser usadas em seu ambiente.

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>Há uma política que impede que qualquer usuário use seus dispositivos móveis enquanto trabalha?

É importante identificar qualquer política corporativa que impede que os funcionários usem dispositivos móveis enquanto trabalham porque ele influenciará a solução MFA que você implementa. Há soluções de MFA, como a fornecida por meio da implementação das políticas de [linha de base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection), que permitem apenas o uso de um aplicativo autenticador para verificação. Caso sua organização tenha uma política que impede o uso de dispositivos móveis, você deve examinar a compra de [Azure ad Premium](https://azure.microsoft.com/pricing/details/active-directory/) para os usuários afetados ou pode implementar uma solução de terceiros que forneça a verificação mais apropriada Option.

#### <a name="what-automation-or-integration-do-you-have-that-leverages-user-credentials-for-authentication"></a>Qual automação ou integração você tem que aproveita as credenciais do usuário para autenticação?

Como o requisito é impor a MFA para cada usuário, incluindo contas de serviço, em seu diretório de parceiro, qualquer automação ou integração que aproveita as credenciais do usuário para autenticação será afetada. Portanto, é importante que você identifique quais contas estão sendo usadas nessas situações. Veja a seguir uma lista de exemplos de aplicativos ou serviços que devem ser considerados

- Painel de controle usado para provisionar recursos em nome de seus clientes
- Integração com qualquer plataforma usada para faturamento (como está relacionada ao programa CSP) e suporte aos seus clientes
- Scripts do PowerShell que utilizam os módulos AZ, AzureRM, Azure AD, MS online, etc.

A lista acima não é abrangente. Portanto, é importante que você execute uma avaliação completa de qualquer aplicativo ou serviço em seu ambiente que aproveita as credenciais do usuário para autenticação. Para combater o requisito de MFA, você deve implementar as diretrizes na estrutura do [modelo de aplicativo seguro](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) sempre que possível. A seguir estão os recursos adicionais que ajudarão você a entender como a estrutura do modelo de aplicativo seguro pode ser implementada

- [Exemplos de .net do Partner Center](https://github.com/microsoft/partner-center-dotnet-samples) – este repositório GitHub contém exemplos, desenvolvidos usando o .net, que demonstrará como você pode implementar a estrutura do modelo de aplicativo seguro.
- [Exemplos de Java do Partner Center](https://github.com/microsoft/partner-center-java-samples) – este repositório GitHub contém exemplos, desenvolvidos usando Java, que demonstrarão como você pode implementar a estrutura do modelo de aplicativo seguro.
- [Partner Center PowerShell – modelo de aplicativo seguro](https://docs.microsoft.com/powershell/partnercenter/secure-app-model) – este é um artigo que fornece detalhes sobre como implementar a estrutura de modelo de aplicativo seguro usando o PowerShell.
- [Comunidade de grupo de diretrizes de segurança do Partner Center](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) – esta é uma comunidade online na qual você pode aprender sobre eventos futuros e fazer perguntas que você possa ter.

### <a name="enforcing-mfa-for-all-users"></a>Impondo MFA para todos os usuários

Esta seção abordará como você pode usar as [políticas de proteção de linha de base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) para impor a MFA para cada usuário, incluindo contas de serviço, em seu locatário de parceiro. Se você estiver planejando usar Azure AD Premium, siga as etapas documentadas [aqui](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted).

> [!NOTE]
> Uma solução de terceiros, que é compatível com o Azure AD, pode ser usada para impor a MFA para todos os usuários, incluindo contas de serviço. Consulte a documentação do fornecedor para obter mais detalhes sobre como a solução deve ser implementada.

As políticas de proteção de linha de base são um conjunto de políticas predefinidas que ajudam a proteger as organizações contra muitos ataques comuns. Esses ataques comuns podem incluir pulverização, reprodução e phishing de senha. As políticas de proteção de linha de base estão disponíveis em todas as edições do Azure Active Directory. A Microsoft está disponibilizando essas políticas de proteção de linha de base a todos para permitir que os clientes e parceiros implementem as melhores práticas de segurança.

As duas políticas de proteção de linha de base que devem ser habilitadas são descritas na tabela a seguir.

|**Política**| |
|-----|-----|
|**Exigir MFA para administradores**|Habilitar a política exigir MFA para administradores exigirá que os usuários nas funções de administrador se registrem para MFA usando o aplicativo autenticador. Depois que o registro de MFA for concluído, os administradores precisarão executar a MFA sempre que entrarem.|
|**Proteção do usuário final**|A proteção do usuário final é uma política de proteção de linha de base do MFA baseada em risco que protege todos os usuários em um diretório. A habilitação dessa política exige que todos os usuários se registrem no MFA usando o aplicativo autenticador. Os usuários podem ignorar o prompt de registro de MFA por 14 dias, após o qual eles serão impedidos de entrar até que se registrem no MFA. Depois de registrado para MFA, os usuários serão solicitados a receber MFA somente durante tentativas de entrada arriscadas. As contas de usuário comprometidas são bloqueadas até que sua senha seja redefinida e os eventos de risco tenham sido ignorados.|

Quando essas políticas estiverem habilitadas, cada usuário poderá utilizar o Azure MFA usando o aplicativo autenticador para verificação sem custo adicional.

#### <a name="configure-self-service-password-reset"></a>Configurar a redefinição de senha de autoatendimento

A redefinição de senha de autoatendimento (SSPR) é um recurso Azure Active Directory que permite que os usuários redefinam suas senhas sem precisar entrar em contato com a equipe de suporte. Os usuários devem se registrar no ou ser registrados para redefinição de senha de autoatendimento antes de usar o serviço. Durante o registro, o usuário escolhe um ou mais métodos de autenticação habilitados pela organização.

Quando a política de proteção de linha de base de [proteção do usuário final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) estiver habilitada, todas as contas de usuário comprometidas serão bloqueadas até que sua senha seja redefinida e os eventos de risco tenham sido descartados. Considerando que é recomendável que cada usuário, que seja um administrador global, execute o seguinte para se registrar no SSPR para que eles não sejam bloqueados.

1. Navegue até a [página de instalação do SSPR](https://aka.ms/ssprsetup)
2. Insira seu nome de usuário e senha
3. Configure pelo menos uma das opções de verificações que serão usadas para verificar quem você está ao redefinir sua senha.  

Quando uma conta tiver sido comprometida, um administrador precisará tomar medidas para restaurar o acesso ao usuário afetado. Consulte as [etapas para desbloquear um usuário](#recovering-compromised-accounts) para obter detalhes sobre o processo para desbloquear o usuário.

#### <a name="require-mfa-for-admins"></a>Exigir MFA para administradores

A política *exigir MFA para a linha de base de administrador* requer MFA para as seguintes funções de diretório, consideradas como as funções de Azure Active Directory mais privilegiadas:

- Administrador global
- Administrador do SharePoint
- Administrador do Exchange
- Administrador de acesso condicional
- Administrador de segurança
- Administrador de assistência técnica/administrador de senha
- Administrador de cobrança
- Administrador do usuário

Ao habilitar a política exigir MFA para administradores, as nove funções de administrador acima serão necessárias para se registrar no MFA usando o aplicativo autenticador. Depois que o registro de MFA for concluído, os administradores precisarão executar a MFA toda vez que entrarem.

Se sua organização tiver essas contas em uso em scripts ou código, considere substituí-las [](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview)por identidades gerenciadas.

Para habilitar essa política e proteger seus administradores:

1. Entre no **portal do Azure** como administrador global, administrador de segurança ou administrador de acesso condicional.
2. Navegue até **Azure Active Directory** > **acesso condicional**.
3. Na lista de políticas, selecione **política de linha de base: Exigir MFA para administradores**.
4. Defina **habilitar política** para **usar a política imediatamente**.
5. Clique em **salvar**.

> [!WARNING]
> Antes de habilitar essa política, verifique se os usuários não estão usando protocolos de autenticação herdados. Por meio da implementação desta política, a autenticação herdada será bloqueada.

> [!IMPORTANT]
> Há um problema conhecido que afeta sua capacidade de se conectar ao Exchange Online PowerShell usando privilégios administrativos delegados. Consulte o problema conhecido do [PowerShell do Exchange Online](#exchange-online-powershell) antes de habilitar essa política se você estiver usando este módulo do PowerShell.

#### <a name="end-user-protection"></a>Proteção do usuário final

A política de linha de base de proteção do usuário final protege todos os usuários em um diretório. A habilitação dessa política exige que todos os usuários se registrem no Azure MFA dentro de 14 dias. Depois de registrado, os usuários receberão uma solicitação pela MFA somente durante tentativas de entrada arriscadas. As contas de usuário comprometidas são bloqueadas até que a redefinição de senha e o risco sejam ignorados.

A política **de linha de base de política: A proteção** do usuário final vem pré-configurada e aparecerá na parte superior quando você navegar até a folha acesso condicional em portal do Azure.

Para habilitar essa política e proteger seus usuários:

1. Entre no **portal do Azure** como administrador global, administrador de segurança ou administrador de acesso condicional.
2. Navegue até **Azure Active Directory** > **acesso condicional**.
3. Na lista de políticas, selecione **política de linha de base: Proteção do usuário final (versão**prévia).
4. Defina **habilitar política** para **usar a política imediatamente**.
5. Clique em **salvar**.

> [!WARNING]
> Antes de habilitar essa política, verifique se os usuários não estão usando protocolos de autenticação herdados. Por meio da implementação desta política, a autenticação herdada será bloqueada.

> [!IMPORTANT]
> Há problemas conhecidos que afetam sua capacidade de se conectar ao Exchange Online PowerShell usando privilégios administrativos delegados. Consulte o problema conhecido do [PowerShell do Exchange Online](#exchange-online-powershell) antes de habilitar essa política se você estiver usando este módulo do PowerShell.

## <a name="common-issues"></a>Problemas comuns

### <a name="azure-active-directory"></a>Azure Active Directory

#### <a name="aadsts50076"></a>AADSTS50076

Depois de habilitar as políticas de linha de base, você pode descobrir que sua automação ou integração está encontrando uma exceção como a seguinte

    AADSTS50076: Due to a configuration change made by your administrator, or because you moved to a new location, you must use multi-factor authentication to access 'MyApp'.

A razão para essa exceção é que você está Autenticando usando credenciais de usuário e a MFA agora é necessária. Para resolver essa exceção, você precisará utilizar um token de acesso para autenticação. Consulte o [Guia do modelo de aplicativo seguro](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) para obter mais informações.

>[!IMPORTANT]
>As APIs mais modernas e os módulos do PowerShell dão suporte à capacidade de utilizar um token de acesso para autenticação. No entanto, existem alguns que atualmente não dão suporte a essa funcionalidade. Se você precisar de ajuda para determinar se o módulo da API ou do PowerShell que você está tentando aproveitar dá suporte ao uso de um token de acesso para autenticação, poste uma mensagem na Comunidade do [grupo de diretrizes de segurança do Partner Center](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) .

#### <a name="aadsts700082"></a>AADSTS700082

Depois de implementar a estrutura de modelo de aplicativo seguro, há uma chance de que você receba a seguinte exceção 90 dias depois de gerar o token de atualização inicial

    The refresh token has expired due to inactivity. The token was issued on 2019-01-02T09:19:53.5422744Z and was inactive for 90.00:00:00

Com relação a Azure Active Directory o tempo de vida máximo de um token de atualização é de 90 dias. Para resolver esse erro, será necessário gerar e armazenar um novo token de atualização com segurança. Observe que é possível atualizar o token de atualização programaticamente porque, com cada solicitação para Azure Active Directory para um token de acesso, um novo token de atualização é retornado. Você pode implementar a lógica apropriada para atualizar o token de atualização armazenado com segurança antes que ele expire.

Consulte [tempos de vida de token configuráveis no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) para obter mais informações.

### <a name="recovering-compromised-accounts"></a>Recuperando contas comprometidas

Para ajudar a proteger nossos clientes, o serviço de credenciamento vazado da Microsoft encontra pares de nome de usuário/senha disponíveis publicamente. Se eles corresponderem a um de nossos usuários, ajudaremos a proteger essa conta imediatamente. Os usuários identificados como tendo uma credencial vazada são confirmados comprometidos. Esses usuários serão impedidos de entrar até que sua senha seja redefinida.

Os usuários com uma licença de Azure AD Premium podem restaurar o acesso por meio de redefinição de senha por autoatendimento (SSPR) se a funcionalidade estiver habilitada em seu diretório. Os usuários sem uma licença Premium que se tornaram bloqueados devem entrar em contato com um administrador para executar uma redefinição manual de senha e ignorar o evento de risco de usuário sinalizado.

#### <a name="steps-to-unblock-a-user"></a>Etapas para desbloquear um usuário

Confirme se o usuário foi bloqueado pela política examinando os logs de entrada do usuário.

1. Um administrador precisa entrar no **portal do Azure** e navegar até **Azure Active Directory** > **usuários** > clicar no nome do usuário e navegar até as entradas.
2. Para iniciar a redefinição de senha em um usuário bloqueado, um administrador precisa navegar até **Azure Active Directory** > **usuários sinalizados para risco**
3. Clique no usuário cuja conta está bloqueada para exibir informações sobre a atividade de entrada recente do usuário.
4. Clique em Redefinir senha para atribuir uma senha temporária que deve ser alterada no próximo logon.
5. Clique em ignorar todos os eventos para redefinir a pontuação de risco do usuário.

Agora, o usuário pode entrar, redefinir sua senha e acessar o aplicativo.

## <a name="known-issues"></a>Problemas conhecidos

### <a name="exchange-online-powershell"></a>PowerShell do Exchange Online

Quando a MFA estiver habilitada, os parceiros não poderão utilizar seus privilégios administrativos delegados com o PowerShell do Exchange Online para executar ações em seus clientes. Confira [conectar-se ao Exchange Online PowerShell usando a autenticação](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell) multifator para obter mais informações sobre essa limitação.

## <a name="resources-and-support"></a>Recursos e suporte

Por meio da [comunidade do grupo de diretrizes de segurança do Partner Center](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) , você poderá encontrar recursos adicionais e aprender sobre eventos futuros, como horas de escritório técnico. Consulte o documento [perguntas](http://assetsprod.microsoft.com/security-requirements-faq.pdf) frequentes para saber mais sobre os requisitos.
