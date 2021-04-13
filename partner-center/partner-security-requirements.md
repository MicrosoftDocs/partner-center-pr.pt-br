---
title: Requisitos de segurança de parceiros
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Apresenta os requisitos de segurança do parceiro para habilitar a MFA (Autenticação Multifator) e adotar a estrutura do Modelo de Aplicativo Seguro.
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: b7fa76999d2e071f80c0175a8dfcbc1afe527bfc
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "106087052"
---
# <a name="security-requirements-for-using-partner-center-or-partner-center-apis"></a>Requisitos de segurança para usar o Partner Center ou as APIs do Partner Center

**Funções apropriadas**

- Todos os usuários do Partner Center

Este artigo explica os requisitos de segurança obrigatórios para Assistentes, Fornecedores do Painel de Controle e parceiros que participam do programa do Provedor de Soluções na Nuvem, bem como opções de autenticação e outras considerações de segurança. As proteções de privacidade e de segurança estão entre nossas principais prioridades. Sabemos que a melhor defesa é a prevenção e que somos tão fortes quanto nosso vínculo mais fraco. É por isso que precisamos de todos em nosso ecossistema, para agir e garantir que as proteções de segurança adequadas estejam em vigor.

## <a name="mandatory-security-requirements"></a>Requisitos de segurança obrigatórios

Os parceiros que não implementarem os requisitos de segurança obrigatórios não poderão fazer transações no programa de Provedor de Soluções na Nuvem nem gerenciar locatários de clientes que utilizam direitos de administrador delegado. Além disso, os parceiros que não implementam os requisitos de segurança podem colocar sua participação em programas em risco. Os termos associados aos requisitos de segurança do parceiro foram adicionados ao Contrato de Parceiro da Microsoft. Como ele é relacionado aos consultores, os mesmos requisitos contratuais estarão em vigor.

Para proteger você e seus clientes, estamos exigindo que os parceiros executem as seguintes ações imediatamente:  

1. **Habilite a MFA (autenticação multifator) para todas as contas de usuário no locatário do parceiro**. Você precisa impor a MFA em todas as contas de usuário nos locatários do parceiro. Os usuários precisam passar pela MFA ao entrarem nos serviços de nuvem comercial da Microsoft ou ao realizarem transações no programa Provedor de Soluções na Nuvem por meio do Partner Center ou de APIs.

2. **Adote a estrutura do Modelo de Aplicativo Seguro**. Todos os parceiros que integram as APIs do Partner Center precisam adotar a [estrutura do Modelo de Aplicativo Seguro](/partner-center/develop/enable-secure-app-model) em qualquer aplicativo e aplicativos de modelo de autenticação de usuário.

    > [!IMPORTANT]
    > É altamente recomendável que os parceiros implementem o Modelo de Aplicativo Seguro para integrar com uma API da Microsoft, como Azure Resource Manager, Microsoft Graph ou aproveitem a automação, como o PowerShell, usando as credenciais do usuário, para evitar qualquer interrupção quando a MFA é imposta.

Esses requisitos de segurança ajudarão a proteger a sua infraestrutura e a proteger os dados dos seus clientes contra possíveis riscos de segurança, como identificar roubos ou outros incidentes de fraude.  

## <a name="implementing-multi-factor-authentication"></a>Como implementar a autenticação multifator

Para atender aos requisitos de segurança do parceiro, você precisa implementar e impor a MFA para cada conta de usuário no seu locatário do parceiro. É possível fazer isso das seguintes maneiras:

- Implemente os [padrões de segurança do Azure AD (Azure Active Directory)](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults). Veja mais sobre isso na [próxima seção](#security-defaults).

- Compre o Azure Active Directory Premium para cada conta de usuário. Para obter mais informações, confira [Planejar uma implantação de Autenticação Multifator do Azure AD](/azure/active-directory/authentication/howto-mfa-getstarted).

- Use uma solução de terceiros para impor a MFA em cada conta de usuário no seu locatário do parceiro. Para garantir que a solução forneça as informações esperadas, consulte [Como os requisitos de segurança serão impostos](#how-the-requirements-are-enforced).

> [!NOTE]
> Embora a autenticação multifator não seja exigida de modo contratual para uma nuvem soberana (governo dos EUA e Alemanha), é altamente recomendável que você adote esses requisitos de segurança.

### <a name="security-defaults"></a>Padrões de segurança

Uma das opções que os parceiros podem escolher para implementar os requisitos de MFA é habilitar os padrões de segurança no Azure AD. Os padrões de segurança oferecem um nível básico de segurança sem nenhum custo adicional. Examine como habilitar a MFA para a sua organização com o Azure AD e as principais considerações abaixo antes de habilitar os padrões de segurança.

- Os parceiros que já adotaram políticas de linha de base precisam tomar medidas para fazer a transição para os padrões de segurança.

- Os padrões de segurança são a substituição de disponibilidade geral das políticas de linha de base de visualização. Depois que um parceiro habilita os padrões de segurança, eles não poderão mais habilitar as políticas de linha de base.

- Com os padrões de segurança, todas as políticas serão habilitadas ao mesmo tempo.

- Para os parceiros que usam o [acesso condicional](/azure/active-directory/conditional-access/concept-conditional-access-policy-common), [os padrões de segurança não estarão disponíveis](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults#disabling-security-defaults).

- Não bloqueamos a autenticação herdada neste momento. No entanto, como a maioria dos eventos relacionados a identidades comprometidas são provenientes de tentativas de entrada usando a autenticação herdada, recomendamos aos parceiros não usar esses protocolos mais antigos.

- A conta de sincronização do Azure AD Connect é excluída dos padrões de segurança.

Para obter informações detalhadas, leia [Visão geral da Autenticação Multifator do Azure AD para a sua organização](/azure/active-directory/authentication/concept-mfa-get-started) e [Quais são os padrões de segurança?](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

> [!NOTE]
> Os padrões de segurança do Azure AD são a evolução das políticas de proteção de linha de base simplificadas. Caso você já tenha habilitado as políticas de proteção de linha de base, é altamente recomendável habilitar os [padrões de segurança](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

## <a name="implementation-considerations"></a>Considerações sobre a implementação

Como esses requisitos se aplicam a todas as contas de usuário no seu locatário do parceiro, há várias considerações que precisam ser feitas para garantir uma implantação tranquila. Por exemplo, identifique as contas de usuários no Azure AD que não podem executar a MFA, bem como aplicativos e dispositivos na sua empresa que não dão suporte para a autenticação moderna.

Antes que você execute qualquer ação, recomendamos concluir as validações a seguir. 

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>Você tem um aplicativo ou dispositivo que não dá suporte ao uso de autenticação moderna?

Quando você impõe a MFA, o uso de autenticação herdada em protocolos como IMAP, POP3, SMTP, entre outros, será bloqueado porque eles não são compatíveis com a MFA. Para resolver essa limitação, use um recurso de [senhas de aplicativo](/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) para garantir que o aplicativo ou dispositivo ainda seja autenticado. Examine as [considerações para usar senhas de aplicativo](/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) a fim de determinar se elas podem ser usadas no seu ambiente.

#### <a name="do-you-have-office-365-users-with-licenses-associated-with-your-partner-tenant"></a>Você tem usuários do Office 365 com licenças associadas ao seu locatário do parceiro?

Antes de implementar qualquer solução, recomendamos que você determine qual versão do Microsoft Office está sendo usada pelos usuários no seu locatário do parceiro. Há uma chance de que os usuários tenham problemas de conectividade com aplicativos como o Outlook. Antes de impor a MFA, é importante confirmar que você está usando o Outlook 2013 SP1 ou posterior e que a sua empresa tem a autenticação moderna habilitada. Para obter mais informações, confira [Habilitar a autenticação moderna no Exchange Online](/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online). 

Para habilitar a autenticação moderna para os dispositivos que executam o Windows e têm o Microsoft Office 2013 instalado, será necessário criar duas chaves de Registro. Consulte [Habilitar a autenticação moderna para o Office 2013 em](/office365/admin/security-and-compliance/enable-modern-authentication)dispositivos Windows.

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>Há uma política que impede que qualquer usuário use seus dispositivos móveis enquanto trabalha?

É importante identificar qualquer política corporativa que impeça que os funcionários usem dispositivos móveis enquanto trabalham, porque isso influenciará a solução de MFA que você implementará. Há soluções, como a fornecida pela implementação dos [padrões de segurança do Azure AD](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults), que permitem apenas o uso de um aplicativo autenticador para verificação. Caso sua empresa tenha uma política que impeça o uso de dispositivos móveis, considere uma das seguintes opções:

- Implantar um aplicativo com senha TOTP (senha única baseada em tempo) que pode ser executado no sistema seguro.

- Implemente uma solução de terceiros que impõe a MFA para cada conta de usuário no locatário do parceiro com a opção de verificação mais apropriada.

- Compre as licenças do [Azure Active Directory Premium](https://azure.microsoft.com/pricing/details/active-directory/) para os usuários impactados.

#### <a name="what-automation-or-integration-do-you-have-to-leverage-user-credentials-for-authentication"></a>Qual automação ou integração você tem para aproveitar as credenciais do usuário para autenticação?

Como a MFA é imposta para cada usuário, incluindo contas de serviço, no seu diretório de parceiro, qualquer automação ou integração que use as credenciais do usuário para autenticação será afetada. Portanto, é importante que você identifique quais contas são usadas nessas situações. Consulte a seguinte lista de aplicativos de exemplo ou serviços a serem considerados:

- Painel de controle usado para provisionar recursos em nome de seus clientes

- Integração com qualquer plataforma usada para faturamento (pois está relacionada ao programa CSP) e suporte aos seus clientes

- Scripts do PowerShell que usam os módulos AZ, AzureRM, Azure AD, MS Online e outros

A lista acima não é abrangente. Portanto, é importante que você realize uma avaliação completa de qualquer aplicativo ou serviço no seu ambiente que use as credenciais do usuário para autenticação. Para lidar com o requisito de MFA, você deve implementar a orientação na [ estrutura de Modelo de Aplicativo Seguro ](/partner-center/develop/enable-secure-app-model), sempre que possível.

## <a name="accessing-your-environment"></a>Acessando seu ambiente

Para entender melhor o que ou quem está autenticando sem precisar fornecer a MFA, recomendamos que você examine a atividade de conexão. Por meio de Azure Active Directory Premium, você pode usar o relatório de entradas. Para obter mais informações sobre este assunto, confira [Relatórios de atividades de entrada no portal do Azure Active Directory](/azure/active-directory/reports-monitoring/concept-sign-ins). Caso você não tenha o Azure Active Directory Premium ou esteja procurando uma forma de obter essa atividade de conexão por meio do PowerShell, use o cmdlet [Get-PartnerUserSignActivity](/powershell/module/partnercenter/get-partnerusersigninactivity) no módulo [PowerShell do Partner Center](https://www.powershellgallery.com/packages/PartnerCenter/).

## <a name="how-the-requirements-are-enforced"></a>Como os requisitos são impostos

Os requisitos de segurança do parceiro são impostos pelo Azure AD e pelo Partner Center, verificando a presença da declaração da MFA para identificar se a verificação da MFA ocorreu. Em 18 de novembro de 2019, a Microsoft ativou proteções de segurança adicionais (anteriormente conhecidas como “imposição técnica”) para locatários do parceiro.

Após a ativação, os usuários no locatário do parceiro deverão concluir a verificação da MFA ao executar qualquer operação AOBO (administrador em nome de) acessando o portal do Partner Center ou chamando a APIs do Partner Center. Para obter mais informações, confira [Como obrigar o uso da MFA (Autenticação Multifator) para o locatário do parceiro](partner-security-requirements-mandating-mfa.md). 

Os parceiros que não atenderam aos requisitos devem implementar essas medidas assim que possível para evitar qualquer interrupção nos negócios. Se você está usando a Autenticação Multifator do Azure Active Directory ou padrões de segurança do Azure AD, não há nenhuma ação adicional que você precisa executar.

Se você estiver usando uma solução de MFA de terceiros, haverá a possibilidade de que a declaração da MFA não seja emitida. Se essa declaração estiver ausente, o Azure AD não poderá determinar se a solicitação de autenticação passou pela MFA. Para obter informações sobre como verificar se sua solução está emitindo a declaração esperada, leia [Teste dos Requisitos de Segurança do Parceiro](/powershell/partnercenter/test-partner-security-requirements). 

> [!IMPORTANT]
> Se sua solução de terceiros não emitir a declaração esperada, você precisará trabalhar com o fornecedor que desenvolveu a solução para determinar quais ações devem ser executadas.

## <a name="resources-and-samples"></a>Recursos e exemplos

Consulte os seguintes recursos para obter suporte e o código de exemplo:

- [Comunidade do Grupo de Diretrizes de Segurança do Partner Center](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance): A comunidade do Grupo de Diretrizes de Segurança do Partner Center é uma comunidade online na qual você pode aprender sobre eventos futuros e tirar dúvidas.
- [Amostras .NET do Partner Center](https://github.com/microsoft/partner-center-dotnet-samples): Esse repositório GitHub contém amostras desenvolvidas usando o .NET, que demonstrarão como você pode implementar a estrutura do Modelo de Aplicativo Seguro.
- [Amostras Java do Partner Center](https://github.com/microsoft/partner-center-java-samples): Esse repositório GitHub contém amostras desenvolvidas usando o Java, que demonstrarão como você pode implementar a estrutura do Modelo de Aplicativo Seguro.
- [PowerShell do Partner Center – Autenticação Multifator](/powershell/partnercenter/multi-factor-auth): Este artigo de Autenticação Multifator fornece detalhes sobre como implementar a estrutura de Modelo de Aplicativo Seguro usando o PowerShell.

## <a name="next-steps"></a>Próximas etapas

- [Obrigar a MFA (Autenticação Multifator) para seu locatário parceiro](partner-security-requirements-mandating-mfa.md)