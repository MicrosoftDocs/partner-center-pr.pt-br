---
title: Requisitos de segurança de parceiros
ms.topic: article
ms.date: 10/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Apresenta os requisitos do parceiro para habilitar a Autenticação Multifator (MFA) e adotar a estrutura do Modelo de Aplicativo Seguro.
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: c92e8c9a9a08582d89ef478a4600f737a548b787
ms.sourcegitcommit: 2847efac28d3bff24ed37cdfaa88ff4be06705c8
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/27/2020
ms.locfileid: "92680393"
---
# <a name="partner-security-requirements-for-partners-using-partner-center-or-partner-center-apis"></a>Requisitos de segurança do parceiro para parceiros usando o Partner Center ou as APIs do Partner Center

**Aplica-se a**

- Todos os parceiros no programa Provedor de Soluções na Nuvem
  - Fatura direta
  - Provedor indireto
  - Revendedor indireto
- Todos os Fornecedores do Painel de Controle
- Todos os consultores

**Usuários apropriados**

- Todos os usuários habilitados, incluindo usuários convidados

As maiores proteções de privacidade e segurança estão entre nossas principais prioridades. Sabemos que a melhor defesa é a prevenção e que somos tão fortes quanto nosso vínculo mais fraco. É por isso que precisamos de todos em nosso ecossistema, para agir e garantir que as proteções de segurança adequadas estejam em vigor. Para ajudar a proteger parceiros e clientes, estamos introduzindo um conjunto de requisitos de segurança obrigatórios para consultores, fornecedores do painel de controle e parceiros que participam do programa de Provedor de Soluções na Nuvem.

## <a name="overview"></a>Visão geral

Os parceiros são obrigados a impor a autenticação multifator para todas as contas de usuário em seu locatário de parceiro. Os termos associados aos requisitos de segurança do parceiro foram adicionados ao Contrato de Parceiro da Microsoft. Como ele é relacionado aos consultores, os mesmos requisitos contratuais estarão em vigor.

Os parceiros que não implementarem os requisitos de segurança obrigatórios não poderão fazer transações no programa de Provedor de Soluções na Nuvem nem gerenciar locatários de clientes que utilizam direitos de administrador delegado, pois esses requisitos são impostos. Além disso, os parceiros que não implementam os requisitos de segurança podem colocar sua participação em programas em risco.  

Para proteger você e seus clientes, estamos exigindo que os parceiros executem as seguintes ações imediatamente:  

1. **Habilite a MFA (Autenticação Multifator) para todas as contas de usuário no locatário de parceiros** . Todas as contas de usuário em locatários de parceiros devem ser desafiadas pela Autenticação Multifator (MFA) ao entrarem nos serviços de nuvem comercial da Microsoft ou ao realizarem transações no programa Provedor de Soluções na Nuvem por meio do Partner Center ou de APIs.

2. **Adote a estrutura do Modelo de Aplicativo Seguro** . Adote a estrutura do Modelo de Aplicativo Seguro. Todos os parceiros que integram a API do Partner Center devem adotar a estrutura do Modelo de Aplicativo Seguro para qualquer aplicativo + aplicativos de modelo de autenticação de usuário.

    > [!IMPORTANT]
    > É altamente recomendável que os parceiros implementem o Modelo de Aplicativo Seguro para integrar com uma API da Microsoft, como Azure Resource Manager, Microsoft Graph ou aproveitar a automação, como o PowerShell, usando as credenciais do usuário, para evitar qualquer interrupção quando a MFA é imposta.

Habilitar a MFA (Autenticação Multifator) e adotar a estrutura do Modelo de Aplicativo Seguro ajudará a proteger a sua infraestrutura e os dados do cliente contra possíveis riscos de segurança, identificando roubos e outros incidentes de fraude.  

## <a name="actions-that-you-need-to-take"></a>Ações que você precisa adotar

Para atender aos requisitos de segurança do parceiro, você precisa impor a autenticação multifator para cada conta de usuário em seu locatário do parceiro. É possível fazer isso das seguintes maneiras:

- Implementar os [padrões de segurança do Azure AD](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

- Comprar o Azure Active Directory Premium para cada conta de usuário. Para obter mais informações, consulte [Planejando uma implantação de Autenticação Multifator do Azure baseada em nuvem](/azure/active-directory/authentication/howto-mfa-getstarted).

- Usar uma solução de terceiros para impor a autenticação multifator para cada conta de usuário em seu locatário do parceiro. Para garantir que a solução forneça as informações esperadas, consulte [Como os requisitos de segurança serão impostos](#how-the-requirements-are-enforced).

> [!NOTE]
> Embora a autenticação multifator não seja exigida de modo contratual para uma nuvem soberana (21Vianet, governo dos EUA e Alemanha), é altamente recomendável que você adote esses requisitos de segurança.

## <a name="security-defaults"></a>Padrões de segurança

A política de padrões de segurança é uma das [opções](#actions-that-you-need-to-take) em que os parceiros podem optar por implementar o MFA para os requisitos de segurança, dependendo de suas necessidades corporativas. Ela oferece um nível básico de segurança habilitado sem nenhum custo adicional. Examine como habilitar a MFA para sua organização com o Azure AD e as principais considerações abaixo antes de habilitar os padrões de segurança.

- As políticas de linha de base permanecerão válidas nos próximos dois meses, mas serão preteridas no final de fevereiro de 2020.

- Os parceiros que já adotaram políticas de linha de base precisam tomar medidas para fazer a transição para os padrões de segurança.

- Os padrões de segurança são a substituição de disponibilidade geral das políticas de linha de base de visualização. Depois que um parceiro habilita os padrões de segurança, eles não poderão mais habilitar as políticas de linha de base.

- Com os padrões de segurança, todas as políticas serão habilitadas ao mesmo tempo.

- Para os parceiros que usam o [acesso condicional](/azure/active-directory/conditional-access/concept-conditional-access-policy-common), [os padrões de segurança não estarão disponíveis](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults#disabling-security-defaults).

- O bloqueio da autenticação herdada não será imposto para parceiros no momento. No entanto, como a maioria dos eventos relacionados a identidades comprometidas são provenientes de tentativas de entrada usando a autenticação herdada, os parceiros são incentivados a se afastar desses protocolos mais antigos.

- A conta de sincronização do Azure AD Connect é excluída dos padrões de segurança.

- Para obter informações detalhadas, leia [Habilitar a autenticação multifator para sua organização](/azure/active-directory/authentication/concept-mfa-get-started) e [Padrões de segurança do Azure Active Directory](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

> [!NOTE]
> Os padrões de segurança do Azure AD são a evolução das políticas de proteção de linha de base simplificadas. Caso você já tenha habilitado as políticas de proteção de linha de base, é altamente recomendável habilitar os padrões de segurança.

Para fazer a transição das políticas de linha de base para os padrões de segurança, leia [O que são os padrões de segurança?](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

### <a name="consideration"></a>Consideração

Como esses requisitos se aplicam a todas as contas de usuário em seu locatário de parceiro, você precisa considerar vários fatores para garantir uma implantação tranquila, incluindo a identificação de contas de usuário no Azure Active Directory que não podem executar a autenticação multifator, bem como aplicativos e dispositivos usados por sua organização que não dão suporte à autenticação moderna.

Antes que você execute qualquer ação, recomendamos concluir as seguintes validações: 

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>Você tem um aplicativo ou dispositivo que não dá suporte ao uso de autenticação moderna?

Quando você impõe a autenticação herdada da autenticação multifator, o uso de protocolos como IMAP, POP3, SMTP etc. é bloqueado porque eles não dão suporte à autenticação multifator. Para resolver essa limitação, um recurso conhecido como [senhas de aplicativo](/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) pode ser usado para garantir que o aplicativo ou dispositivo ainda seja autenticado. Você deve examinar as considerações para usar senhas de aplicativo documentadas [aqui](/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) para determinar se elas podem ser usadas em seu ambiente.

#### <a name="do-you-have-users-using-office-365-provided-by-licenses-associated-with-your-partner-tenant"></a>Você tem usuários usando o Office 365 fornecido por licenças associadas ao seu locatário do parceiro?

Antes de implementar qualquer solução, recomendamos que você determine qual versão do Microsoft Office está sendo usada pelos usuários em seu locatário do parceiro. Há uma chance de que os usuários tenham problemas de conectividade com aplicativos como o Outlook. Antes de impor a autenticação multifator, é importante garantir que o Outlook 2013 SP1 ou posterior esteja sendo usado e que sua empresa tenha a autenticação moderna habilitada. Para obter mais informações, confira [Habilitar a autenticação moderna no Exchange Online](/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online). 

Para habilitar a autenticação moderna nos dispositivos que executam o Windows com o Microsoft Office 2013 instalado, você precisará criar duas chaves do Registro. Consulte [Habilitar a autenticação moderna para o Office 2013 em](/office365/admin/security-and-compliance/enable-modern-authentication)dispositivos Windows.

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>Há uma política que impede que qualquer usuário use seus dispositivos móveis enquanto trabalha?

É importante identificar qualquer política corporativa que impeça que os funcionários usem dispositivos móveis enquanto trabalham, porque isso influenciará a solução de autenticação multifator que você implementará. Há soluções, como a fornecida pela implementação dos [padrões de segurança do Azure AD](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults), que permitem apenas o uso de um aplicativo autenticador para verificação. Caso sua empresa tenha uma política que impeça o uso de dispositivos móveis, considere uma das seguintes opções:

- Implantar um aplicativo com senha TOTP (senha única baseada em tempo) que pode ser executado no sistema seguro

- Implemente uma solução de terceiros que impõe a autenticação multifator para cada conta de usuário no locatário do parceiro com a opção de verificação mais apropriada

- Comprar licenças do [Azure Active Directory Premium](https://azure.microsoft.com/pricing/details/active-directory/) para os usuários afetados

#### <a name="what-automation-or-integration-do-you-have-to-leverage-user-credentials-for-authentication"></a>Qual automação ou integração você tem para aproveitar as credenciais do usuário para autenticação?

Como o requisito é impor a MFA para cada usuário, incluindo contas de serviço, em seu diretório de parceiro, qualquer automação ou integração que aproveita as credenciais do usuário para autenticação será afetada. Portanto, é importante que você identifique quais contas são usadas nessas situações. Consulte a seguinte lista de aplicativos de exemplo ou serviços a serem considerados:

- Painel de controle usado para provisionar recursos em nome de seus clientes

- Integração com qualquer plataforma usada para faturamento (pois está relacionada ao programa CSP) e suporte aos seus clientes

- Scripts do PowerShell que utilizam os módulos AZ, AzureRM, Azure AD, MS online etc.

A lista acima não é abrangente. Portanto, é importante que você realize uma avaliação completa de qualquer aplicativo ou serviço no seu ambiente que utiliza as credenciais do usuário para autenticação. Para lidar com o requisito de autenticação multifator, você deve implementar as orientações na [estrutura de Modelo de Aplicativo Seguro](/partner-center/develop/enable-secure-app-model), sempre que possível.

## <a name="accessing-your-environment"></a>Acessando seu ambiente

Para entender melhor o que ou quem está autenticando sem precisar fornecer a autenticação multifator, recomendamos que você examine a atividade de entrada. Por meio de Azure Active Directory Premium, você pode fazer uso do relatório de entradas. Para obter mais informações, confira os [relatórios de atividades de conexão no portal do Azure Active Directory](/azure/active-directory/reports-monitoring/concept-sign-ins). Caso você não tenha o Azure Active Directory Premium ou esteja procurando uma forma de obter essa atividade de conexão por meio do PowerShell, utilize o cmdlet [Get-PartnerUserSignActivity](/powershell/module/partnercenter/get-partnerusersigninactivity) no módulo [PowerShell do Partner Center](https://www.powershellgallery.com/packages/PartnerCenter/).

## <a name="how-the-requirements-are-enforced"></a>Como os requisitos são impostos

Os requisitos de segurança do parceiro são impostos pelo Azure Active Directory e pelo Partner Center, verificando a presença da declaração da MFA para identificar se a verificação da autenticação multifator ocorreu. Em 18 de novembro de 2019, a Microsoft ativou proteções de segurança adicionais (anteriormente conhecidas como “imposição técnica”) para locatários de parceiros.

Após a ativação, os usuários no locatário do parceiro deverão concluir a verificação da MFA (autenticação multifator) ao executar qualquer operação AOBO (administrador em nome de) acessando o portal do Partner Center ou chamando a API do Partner Center. Para obter informações detalhadas, acesse [Como obrigar o uso da MFA (Autenticação Multifator) para o locatário de parceiro](partner-security-requirements-mandating-mfa.md). 

Os parceiros que não atenderam aos requisitos devem implementar essas medidas assim que possível para evitar qualquer interrupção nos negócios. 

Se você está usando a Autenticação Multifator do Azure ou padrões de segurança do Azure AD, não há nenhuma ação adicional que você precisa executar.

Se você estiver usando uma solução de autenticação multifator de terceiros, haverá a possibilidade de que a declaração da MFA não seja emitida. Se essa declaração estiver ausente, o Azure Active Directory não poderá determinar se a solicitação de autenticação foi desafiada pela autenticação multifator. Para obter informações sobre como verificar se sua solução está emitindo a declaração esperada, leia [Teste dos Requisitos de Segurança do Parceiro](/powershell/partnercenter/test-partner-security-requirements). 

> [!IMPORTANT]
> Se sua solução de terceiros não emitir a declaração esperada, você precisará trabalhar com o fornecedor que desenvolveu a solução para determinar quais ações devem ser executadas.

## <a name="resources-and-support"></a>Recursos e suporte

Consulte os seguintes recursos para obter suporte e o código de exemplo:

- [Comunidade do Grupo de Diretrizes de Segurança do Partner Center](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance): A comunidade do Grupo de Diretrizes de Segurança do Partner Center é uma comunidade online na qual você pode aprender sobre eventos futuros e tirar dúvidas.
- [Amostras .NET do Partner Center](https://github.com/microsoft/partner-center-dotnet-samples): Esse repositório GitHub contém amostras desenvolvidas usando o .NET, que demonstrarão como você pode implementar a estrutura do Modelo de Aplicativo Seguro.
- [Amostras Java do Partner Center](https://github.com/microsoft/partner-center-java-samples): Esse repositório GitHub contém amostras desenvolvidas usando o Java, que demonstrarão como você pode implementar a estrutura do Modelo de Aplicativo Seguro.
- [PowerShell do Partner Center – Autenticação Multifator](/powershell/partnercenter/multi-factor-auth): Este artigo de Autenticação Multifator fornece detalhes sobre como implementar a estrutura de Modelo de Aplicativo Seguro usando o PowerShell.