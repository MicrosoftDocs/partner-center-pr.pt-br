---
title: Requisitos de segurança do parceiro | Partner Center
ms.topic: article
ms.date: 10/11/2019
description: Saiba mais sobre os requisitos de segurança para consultores e parceiros que participam do programa de Provedor de Soluções na Nuvem.
author: isaiahwilliams
ms.author: iswillia
keywords: O Azure Active Directory, provedor de soluções na nuvem, programa de provedor de soluções na nuvem, CSP, fornecedor do painel de controle, CPV, autenticação multifator, MFA, modelo de aplicativo seguro, modelo de aplicativo seguro, segurança
ms.localizationpriority: high
ms.openlocfilehash: 4c7f4e61cc249fb51f58e4a94892a2d937cae4e1
ms.sourcegitcommit: 1fe366f787d97c96510cfd409304e7d48af7c286
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/30/2019
ms.locfileid: "73141974"
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

## <a name="overview"></a>Visão geral

A partir de 1º de agosto de 2019, todos os parceiros são obrigados a impor a autenticação multifator para todas as contas de usuário em seu locatário de parceiro. Os termos associados aos requisitos de segurança do parceiro foram adicionados ao guia [do programa do Provedor de Soluções na Nuvem](https://go.microsoft.com/fwlink/p/?LinkId=617100). Como ele é relacionado aos consultores, os mesmos requisitos contratuais estarão em vigor.

> [!NOTE]
> É altamente recomendável que todos os parceiros que negociam em uma nuvem soberana (21Vianet, US Government e Alemanha) atuem e adotem esses requisitos de segurança imediatamente. No entanto, esses parceiros não precisam atender aos requisitos de segurança em vigor em 1º de agosto de 2019. Futuramente, a Microsoft fornecerá detalhes adicionais sobre a imposição desses requisitos de segurança para nuvens soberanas.

Os parceiros que não implementarem os requisitos de segurança obrigatórios não poderão fazer transações no programa de Provedor de Soluções na Nuvem nem gerenciar locatários de clientes que utilizam direitos de administrador delegado, pois esses requisitos são impostos.

## <a name="actions-that-you-need-to-take"></a>Ações que você precisa adotar

Para atender aos requisitos de segurança do parceiro, você precisa impor a autenticação multifator para cada conta de usuário em seu locatário do parceiro. Para fazer isso, devemos adotar uma das seguintes opções

- Implementar o recurso das políticas de proteção de linha de base [Exigir MFA para administradores](/azure/active-directory/conditional-access/howto-baseline-protect-administrators) e [Proteção do usuário final](/azure/active-directory/conditional-access/howto-baseline-protect-end-users) do Azure Active Directory sem custo adicional
- Comprar o Azure Active Directory Premium para cada conta de usuário. Consulte [Planejando uma implantação de Autenticação Multifator do Azure baseada em nuvem](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted) para obter mais informações.
- Usar uma solução de terceiros para impor a autenticação multifator para cada conta de usuário em seu locatário do parceiro. Consulte [Como os requisitos de segurança serão impostos](#how-the-requirements-will-be-enforced) para obter mais detalhes, a fim de garantir que a solução forneça as informações esperadas.

### <a name="consideration"></a>Consideração

Como esses requisitos se aplicam a todas as contas de usuário em seu locatário do parceiro há várias considerações que precisam ser feitas para garantir uma implantação tranquila. Essas considerações incluem a identificação de contas de usuário no Azure Active Directory que não podem executar a autenticação multifator, bem como dos aplicativos e dispositivos usados pela sua empresa que não dão suporte à autenticação moderna.

Antes de executar qualquer ação, é recomendável que você identifique o seguinte

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>Você tem um aplicativo ou dispositivo que não dá suporte ao uso de autenticação moderna?

Quando você impõe a autenticação herdada da autenticação multifator, o uso de protocolos como IMAP, POP3, SMTP etc. é bloqueado porque esses protocolos não dão suporte à autenticação multifator. Para resolver essa limitação, um recurso conhecido como [senhas de aplicativo](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) pode ser usado para garantir que o aplicativo ou dispositivo ainda possa ser autenticado. Você deve examinar as considerações para usar senhas de aplicativo documentadas [aqui](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) para determinar se elas podem ser usadas em seu ambiente.

#### <a name="do-you-have-users-using-office-365-provided-by-licenses-associated-with-your-partner-tenant"></a>Você tem usuários usando o Office 365 fornecido por licenças associadas ao seu locatário do parceiro?

Antes de implementar qualquer solução, é recomendável que você determine qual versão do Microsoft Office está sendo usada pelos usuários em seu locatário do parceiro. Analise [o plano de autenticação multifator para implantações do Office 365](https://docs.microsoft.com/office365/admin/security-and-compliance/multi-factor-authentication-plan#enable-mfa) antes de realizar qualquer ação. Há uma chance de que os usuários tenham problemas de conectividade com aplicativos como o Outlook. Antes de impor a autenticação multifator, é importante garantir que o Outlook 2013 SP1 ou posterior esteja sendo usado e que sua empresa tenha a autenticação moderna habilitada. Consulte [Habilitar a autenticação moderna no Exchange Online](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online) para obter mais informações.

Para habilitar a autenticação moderna para todos os dispositivos que executam o Windows, com o Microsoft Office 2013 instalado, será necessário criar duas chaves do registro. Consulte [Habilitar a autenticação moderna para o Office 2013 em](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)dispositivos Windows.

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>Há uma política que impede que qualquer usuário use seus dispositivos móveis enquanto trabalha?

É importante identificar qualquer política corporativa que impeça que os funcionários usem dispositivos móveis enquanto trabalham, porque isso influenciará a solução de autenticação multifator que você implementará. Há soluções, como a fornecida pela implementação das políticas de [proteção de linha de base](/azure/active-directory/conditional-access/concept-baseline-protection), que permitem apenas o uso de um aplicativo autenticador para verificação. Caso sua empresa tenha uma política que impeça o uso de dispositivos móveis, você deve considerar uma das seguintes opções

- Implantar um aplicativo com senha TOTP (senha única baseada em tempo) que pode ser executado no sistema seguro
- Implemente uma solução de terceiros que impõe a autenticação multifator para cada conta de usuário no locatário do parceiro com a opção de verificação mais apropriada
- Comprar licenças do [Azure Active Directory Premium](https://azure.microsoft.com/pricing/details/active-directory/) para os usuários afetados

#### <a name="what-automation-or-integration-do-you-have-that-leverages-user-credentials-for-authentication"></a>Qual automação ou integração você tem para aproveitar as credenciais do usuário para autenticação?

Como o requisito é impor a MFA para cada usuário, incluindo contas de serviço, em seu diretório de parceiro, qualquer automação ou integração que aproveita as credenciais do usuário para autenticação será afetada. Portanto, é importante que você identifique quais contas são usadas nessas situações. Veja a seguir uma lista de exemplos de aplicativos ou serviços que devem ser considerados

- Painel de controle usado para provisionar recursos em nome de seus clientes
- Integração com qualquer plataforma usada para faturamento (pois está relacionada ao programa CSP) e suporte aos seus clientes
- Scripts do PowerShell que utilizam os módulos AZ, AzureRM, Azure AD, MS online etc.

A lista acima não é abrangente. Portanto, é importante que você execute uma avaliação completa de qualquer aplicativo ou serviço em seu ambiente, que aproveite as credenciais do usuário para autenticação. Para lidar com o requisito de autenticação multifator, você deve implementar as orientações na [estrutura de Modelo de Aplicativo Seguro](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model), sempre que possível.

## <a name="accessing-your-environment"></a>Acessando seu ambiente

Para entender melhor o que ou quem está autenticando sem precisar fornecer a autenticação multifator, é recomendável examinar a atividade de entrada. Por meio de Azure Active Directory Premium, você pode fazer uso do relatório de entradas. Confira [Relatórios de atividade de entrada no portal do Azure Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins) para obter mais informações. Se não tiver o Azure Active Directory Premium ou se estiver procurando uma maneira de obtê-lo por meio do PowerShell, você precisará fazer uso do cmdlet [Get-PartnerUserSignActivity](https://docs.microsoft.com/powershell/module/partnercenter/get-partnerusersigninactivity) do módulo [Partner Center do PowerShell](https://www.powershellgallery.com/packages/PartnerCenter/).

## <a name="how-the-requirements-will-be-enforced"></a>Como os requisitos serão impostos

Os requisitos de segurança do parceiro serão impostos pelo Azure Active Directory e, em seguida, pelo Partner Center, verificando a presença da declaração de MFA para identificar que a verificação da autenticação multifator ocorreu. Se você está usando a autenticação multifator do Azure ou políticas de proteção de linha de base, não há nenhuma ação adicional que você precisa executar.

Ao usar uma solução de autenticação multifator de terceiros, há uma chance de a declaração de MFA não ser emitida. Se essa declaração estiver ausente, o Azure Active Directory não poderá determinar se a solicitação de autenticação foi desafiada pela autenticação multifator. Confira [Teste dos Requisitos de Segurança do Parceiro](https://docs.microsoft.com/powershell/partnercenter/test-partner-security-requirements) para obter informações sobre como verificar se sua solução está emitindo a declaração esperada.

> [!IMPORTANT]
> Se sua solução de terceiros não emitir a declaração esperada, você precisará trabalhar com o fornecedor que desenvolveu a solução para determinar quais ações devem ser executadas.

## <a name="resources-and-support"></a>Recursos e suporte

Veja a seguir os recursos em que você pode encontrar suporte e código de exemplo

- [Comunidade do grupo de orientação de segurança do Partner Center](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)  – Esta é uma comunidade online na qual você pode aprender sobre eventos futuros e tirar dúvidas.
- [Amostras .NET do Partner Center](https://github.com/microsoft/partner-center-dotnet-samples) - Esse repositório GitHub contém amostras desenvolvidas usando o .NET, que demonstrarão como você pode implementar a estrutura do Modelo de Aplicativo Seguro.
- [Amostras Java do Partner Center](https://github.com/microsoft/partner-center-java-samples) - Esse repositório GitHub contém amostras desenvolvidas usando o Java, que demonstrarão como você pode implementar a estrutura do Modelo de Aplicativo Seguro.
- [PowerShell do Partner Center – Autenticação Multifator](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth) – Este é um artigo que fornece detalhes sobre como implementar a estrutura de Modelo de Aplicativo Seguro usando o PowerShell.
