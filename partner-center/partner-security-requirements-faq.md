---
title: Perguntas frequentes sobre requisitos de segurança de parceiros
ms.topic: article
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Perguntas frequentes sobre os requisitos de segurança de parceiros – o que são, como os parceiros devem implementá-los e como saber se eles foram atendidos.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 055f7f43e9b5d866c18680de000d6cee01e2e165
ms.sourcegitcommit: e1c8bea4aaf807aebe99c125cb1fb6dc8fdfa210
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2020
ms.locfileid: "87444895"
---
# <a name="frequently-asked-questions-about-the-partner-security-requirements"></a>Perguntas frequentes sobre os requisitos de segurança de parceiros

**Usuários apropriados**

- Todos os usuários habilitados, incluindo usuários convidados

Este artigo contém algumas perguntas frequentes sobre os [requisitos de segurança de parceiros](partner-security-requirements.md).

## <a name="partner-security-requirements"></a>Requisitos de segurança de parceiros

### <a name="what-are-the-partner-security-requirements-and-why-should-partners-implement"></a>Quais são os requisitos de segurança do parceiro e por que os parceiros devem implementá-los?

Garantias de segurança e privacidade maiores e contínuas estão entre as nossas principais prioridades, e continuamos ajudando os parceiros a proteger os clientes e os locatários. Continuamos a ver uma escalada no número e na sofisticação dos ataques de segurança, principalmente aqueles relacionados a incidentes de comprometimento da identidade. Como os controles preventivos desempenham um papel fundamental em uma estratégia de defesa geral para impedir os ataques de segurança, introduzimos [requisitos de segurança obrigatórios](partner-security-requirements.md) em 2019. Todos os parceiros que participam do programa CSP (Provedor de Soluções na Nuvem), fornecedores de painel de controle e consultores devem implementar os requisitos para manter a conformidade.

### <a name="what-are-the-key-timelines-and-milestones"></a>Quais são as principais linhas do tempo e marcos?

Os termos associados a esses requisitos de segurança estão incluídos no Contrato de Parceiro da Microsoft em 2019. Você precisará implementar esses requisitos de segurança o quanto antes para manter a conformidade com a sua participação no programa CSP.

### <a name="what-will-happen-if-i-dont-implement-these-partner-security-requirements"></a>O que acontecerá se eu não implementar esses requisitos de segurança do parceiro?

O Contrato de Parceiro da Microsoft exige que você imponha a autenticação multifator às contas de usuário e adote o Modelo de Aplicativo Seguro para interagir com a API da Central de Parceiros. 

Os parceiros que não seguirem essas práticas de segurança poderão perder a capacidade de realizar transações no programa CSP ou de gerenciar locatários de clientes usando direitos de administrador delegado.

### <a name="do-the-security-requirements-apply-to-all-geographies"></a>Os requisitos de segurança se aplicam a todas as geografias?

Sim, os requisitos de segurança se aplicam a todas as geografias. É altamente recomendável que todos os parceiros que negociam em uma nuvem soberana (21Vianet, governo dos EUA e Alemanha) atuem e adotem esses novos requisitos de segurança imediatamente. No entanto, esses parceiros não precisam atender aos novos requisitos de segurança em vigor a partir de 1º de agosto. Futuramente, a Microsoft fornecerá detalhes adicionais sobre a imposição desses requisitos de segurança para nuvens soberanas.

### <a name="is-it-possible-to-get-an-exclusion-for-an-account"></a>É possível abrir exceção para uma conta?

Não, não é possível isentar nenhuma conta de usuário do requisito de ter a MFA imposta. Considerando a natureza altamente privilegiada de ser um parceiro, o Contrato de Parceiro da Microsoft exige que a autenticação multifator seja imposta para todas as contas de usuário do seu locatário de parceiro.

### <a name="how-do-i-know-if-i-have-met-the-partner-security-requirements"></a>Como faço para saber se atendi aos requisitos de segurança do parceiro?

Você precisa concluir as etapas abaixo

- Será necessário atender a todos os requisitos descritos nos [requisitos de segurança do parceiro](partner-security-requirements.md)
- Você precisa garantir que a autenticação multifator seja imposta em todas as contas de usuário em seu locatário do parceiro.

Para ajudar a identificar as principais áreas em que você pode executar ações, estamos fornecendo o relatório de [status dos requisitos de segurança](https://partner.microsoft.com/commerce/security/compliance), que está disponível por meio do Partner Center.

Confira o [status dos requisitos de segurança do parceiro](partner-security-compliance.md) para obter mais informações sobre o relatório de status.

## <a name="required-actions"></a>Ações necessárias

### <a name="what-are-the-key-actions-i-need-to-take-to-meet-the-requirements"></a>Quais são as principais ações que preciso executar para atender aos requisitos?

Todos os parceiros do programa CSP (cobrança direta, provedor indireto e revendedor indireto), consultores e fornecedores de painel de controle precisam atender aos requisitos.

1. **Impor a MFA para todos os usuários**

    Todos os parceiros do programa CSP, assistentes e fornecedores de painel de controle são obrigados a impor a MFA para todos os usuários do locatário de parceiro.

    Considerações adicionais:

    - os provedores indiretos precisarão trabalhar com os revendedores indiretos para se integrar ao Partner Center, caso ainda não o tenham feito, além de encorajar seus revendedores a atender aos requisitos.
    - A MFA do Azure está sendo disponibilizada para todos os usuários no locatário de parceiro sem nenhum custo por meio dos padrões de segurança do Azure AD com o único método de verificação de um aplicativo autenticador que dá suporte à TOTP (Senhas Avulsas por Tempo Limitado).
    - Há métodos de verificação adicional disponíveis por meio das SKUs do [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium), caso outros métodos – uma chamada telefônica ou mensagem e texto – sejam necessários.
    - Os parceiros também podem aproveitar uma solução de MFA de terceiros para cada conta ao acessar os serviços de nuvem comercial da Microsoft.

2. **Adotar a estrutura do Modelo de Aplicativo Seguro**

    Todos os parceiros que desenvolveram uma integração personalizada usando qualquer API (como as APIs do Azure Resource Manager, do Microsoft Graph, do Partner Center, etc.) ou que implementaram uma automação personalizada usando ferramentas como o PowerShell, precisarão adotar a [estrutura do Modelo de Aplicativo Seguro](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) para se integrar com os serviços em nuvem da Microsoft. Deixar de fazer isso pode resultar em uma interrupção devido à implantação da MFA. Os recursos a seguir fornecem uma visão geral e orientações a respeito de como adotar o modelo.

    - [Visão geral do Modelo de Aplicativo Seguro](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
    - [Partner Center: guia do Modelo de Aplicativo Seguro](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
    - [Parceiros no programa CSP: código de exemplo em .NET para habilitar o Modelo de Aplicativo Seguro](https://docs.microsoft.com/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
    - [Parceiros no programa CSP: código de exemplo em Java para habilitar o Modelo de Aplicativo Seguro](https://docs.microsoft.com/samples/microsoft/partner-center-java-samples/secure-app-model/)
    - [Documento de autenticação do Partner Center](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
    - [Documento de MFA (Autenticação Multifator) do PowerShell do Partner Center](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth)

    Consulte o fornecedor com relação à adoção da estrutura Modelo de Aplicativo Seguro se você estiver usando um painel de controle.

    Os fornecedores de painel de controle são obrigados a se [integrar](enroll-as-cpv.md) com o Partner Center como fornecedores de painel de controle e começar a implementar esses requisitos imediatamente. Confira [Partner Center: estrutura do Modelo de Aplicativo Seguro](https://assetsprod.microsoft.com/secure-application-model-guide.pdf). Os fornecedores de painel de controle devem aceitar e gerenciar o consentimento dos parceiros do CSP em vez de credenciais e limpar todas as credenciais de parceiros do CSP existentes.

## <a name="multi-factor-authentication"></a>Autenticação Multifator

### <a name="what-is-multi-factor-authentication-mfa"></a>O que é a MFA (Autenticação Multifator)?

A MFA é um mecanismo de segurança por meio do qual os indivíduos são autenticados por mais de um procedimento obrigatório de validação e segurança. Ela funciona exigindo dois ou mais dos seguintes métodos de autenticação:

- Algo que você sabe (geralmente uma senha)
- Algo que você tem (um dispositivo confiável que não é duplicado facilmente, como um telefone)
- Algo que você é (biometria)

### <a name="what-is-the-cost-of-enabling-mfa"></a>Qual é o custo para habilitar a MFA?

A Microsoft fornece MFA sem custo por meio da implementação de padrões de segurança do Azure AD. A única opção de verificação disponível por meio desta versão da MFA é um aplicativo autenticador. Se for necessário realizar uma chamada telefônica ou enviar uma mensagem SMS, será preciso comprar uma licença do [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium). Como alternativa, você pode utilizar uma solução de terceiros para fornecer a MFA a cada usuário no seu locatário de parceiro; nesse caso, é sua responsabilidade garantir que a solução de MFA esteja sendo imposta e que você esteja em conformidade.

### <a name="what-actions-do-i-need-to-take-if-i-already-have-an-mfa-solution"></a>Quais ações precisarei executar se eu já tiver uma solução de MFA?

Por meio desses requisitos de segurança, será exigido que os usuários de um locatário de parceiro sejam autenticados usando a MFA ao acessar os serviços de nuvem comercial da Microsoft. Uma solução de terceiros pode ser usada para atender a esses requisitos. A Microsoft não fornece mais testes de validação a provedores de identidade independentes para compatibilidade com o Azure Active Directory. Para testar seu produto quanto à interoperabilidade, veja estas [diretrizes](https://www.microsoft.com/download/details.aspx?id=56843).

> [!IMPORTANT]
> Se você estiver usando uma solução de terceiros, será importante verificar se ela está emitindo a declaração de AMR (referência do método de autenticação) que inclui o valor da MFA. Confira [Teste dos Requisitos de Segurança do Parceiro](https://docs.microsoft.com/powershell/partnercenter/test-partner-security-requirements) para obter detalhes de como validar a solução de terceiros que está emitindo a declaração esperada.

### <a name="i-use-multiple-partner-tenants-to-transact-do-i-need-to-implement-mfa-on-them-all"></a>Eu uso vários locatários de parceiros para realizar transações. É necessário implementar a MFA em todos eles?

Sim, será necessário impor a MFA a cada locatário do Azure Active Directory associado aos programas CSP ou Advisor. Para comprar uma licença do Azure Active Directory Premium, uma licença precisará ser adquirida para o usuário em cada locatário do Azure Active Directory.

### <a name="does-each-user-account-in-my-partner-tenant-need-to-have-mfa-enforced"></a>É necessário impor a MFA a todas as contas de usuário do meu locatário de parceiro?

Sim, cada usuário precisará ter a MFA imposta. No entanto, se você estiver usando os padrões de segurança do Azure AD, não será necessária nenhuma ação adicional, porque o recurso impõe a MFA a todas as contas de usuário. A habilitação de padrões de segurança é uma forma gratuita e fácil de verificar se as contas de usuário estão em conformidade com a MFA e não são afetadas quando a MFA é imposta.

### <a name="i-am-a-direct-bill-partner-with-microsoft-what-do-i-need-to-do"></a>Sou um parceiro de cobrança direta da Microsoft. O que preciso fazer?

Parceiros de cobrança direta do Provedor de Soluções na Nuvem devem impor a MFA para cada usuário do seu locatário de parceiro.

### <a name="i-am-an-indirect-reseller-and-only-transact-though-a-distributor-do-i-still-have-to-do-enable-mfa"></a>Sou um revendedor indireto e realizo transações apenas por meio de um distribuidor. Mesmo assim tenho que habilitar a MFA?

Todos os revendedores indiretos precisam impor a MFA para cada usuário do seu locatário de parceiro. O revendedor indireto deve habilitar a MFA.

### <a name="i-dont-use-the-partner-center-api-do-i-still-need-to-implement-mfa"></a>Eu não uso a API da Central de Parceiros. Mesmo assim preciso implementar a MFA?

Sim, esse requisito de segurança destina-se a todos os usuários, incluindo os usuários administradores de parceiros e os usuários finais do locatário de parceiro.

### <a name="which-third-party-vendors-provide-mfa-solutions-compatible-with-azure-active-directory"></a>Quais fornecedores de terceiros oferecem soluções de MFA compatíveis com o Azure Active Directory?

Ao examinar os fornecedores e as soluções de MFA, os parceiros devem garantir que a solução escolhida seja compatível com o Azure Active Directory.

A Microsoft não fornece mais testes de validação a provedores de identidade independentes para compatibilidade com o Azure Active Directory. Caso deseje testar seu produto quanto à interoperabilidade, veja estas [diretrizes](https://www.microsoft.com/download/details.aspx?id=56843).

Para obter mais informações, confira a [lista de compatibilidade da federação do Azure AD](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-compatibility).

### <a name="how-can-i-test-mfa-in-our-integration-sandbox"></a>Como posso testar a MFA em nossa área restrita de integração?

O recurso de padrões de segurança do Azure AD deve ser habilitado ou, como alternativa, você pode aproveitar a solução de terceiros que utiliza a federação.

### <a name="will-enabling-mfa-affect-how-i-interact-with-my-customers-tenant"></a>A habilitação da MFA afetará o meu modo de interação com o locatário do meu cliente?

Não. O cumprimento desses requisitos de segurança não afetará a maneira como você gerencia seus clientes. Sua capacidade de executar operações administrativas delegadas não será interrompida.

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a>Meus clientes estão sujeitos aos requisitos de segurança de parceiros?

Não, não é necessário impor a MFA para cada usuário nos locatários do Azure AD do seu cliente. No entanto, é recomendável que você trabalhe com cada cliente para determinar a melhor maneira de proteger os usuários de cada um deles.

### <a name="can-any-user-be-excluded-from-the-mfa-requirement"></a>Qualquer usuário pode ser excluído do requisito da MFA?

Não, todos os usuários do seu locatário de parceiro, inclusive as contas de serviço, serão obrigados a se autenticar usando a MFA.

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a>Os requisitos de segurança de parceiros se aplicam à área restrita de integração?

Sim, os requisitos de segurança de parceiros se aplicam à área restrita de integração. Isso significa que você precisará implementar a solução de MFA apropriada para os usuários no locatário da área restrita de integração. É recomendável que você implemente os padrões de segurança do Azure AD para fornecer MFA.

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a>Como faço para configurar uma conta de acesso de emergência?

É considerada uma melhor prática criar uma ou duas contas de acesso de emergência para impedir o bloqueio não intencional do seu locatário do Azure AD. Em relação aos requisitos de segurança de parceiros, é necessário que cada usuário seja autenticado usando a MFA. Esse requisito significa que você precisará modificar a definição da conta de acesso de emergência. Pode ser uma conta que esteja aproveitando uma solução de MFA de terceiros.

### <a name="is-active-directory-federation-service-adfs-required-if-i-am-using-a-third-party-solution"></a>O ADFS (Serviço de Federação do Active Directory) será necessário se eu estiver usando uma solução de terceiros?

Não, não será necessário ter o ADFS (Serviço de Federação do Active Directory) se você estiver usando uma solução de terceiros. É recomendável que você trabalhe com o fornecedor da solução para determinar quais são os requisitos da solução dele.

### <a name="is-it-a-requirement-to-enable-azure-ad-security-defaults"></a>É um requisito habilitar os padrões de segurança do Azure AD?

Não, não é obrigatório habilitar os padrões de segurança do Azure AD.

### <a name="can-conditional-access-be-used-to-meet-the-mfa-requirement"></a>O acesso condicional pode ser usado para atender ao requisito de MFA?

Sim, você pode usar o acesso condicional para impor a MFA para cada usuário do seu locatário de parceiro, inclusive das contas de serviço. Contudo, considerando a natureza altamente privilegiada de um parceiro, precisamos garantir que cada usuário tenha um desafio de MFA a cada autenticação realizada. Isso significa que você não poderá aproveitar o recurso de acesso condicional que contorna o requisito de MFA.

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>A conta de serviço usada pelo Azure AD Connect será afetada pelos requisitos de segurança de parceiros?

Não, a conta de serviço usada pelo Azure AD Connect não será afetada pelos requisitos de segurança de parceiros. Se você tiver um problema com o Azure AD Connect em virtude da imposição da MFA, abra uma solicitação de suporte técnico junto ao suporte da Microsoft.

## <a name="secure-application-model"></a>Modelo de Aplicativo Seguro

### <a name="who-should-adopt-the-secure-application-model-to-meet-the-requirements"></a>Quem deve adotar o modelo de aplicativo seguro para atender aos requisitos?

A Microsoft está introduzindo uma estrutura segura e escalonável para autenticar parceiros do CSP (Provedor de Soluções na Nuvem) e CPVs (Fornecedores de Painel de Controle) que aproveitam a Autenticação Multifator. Consulte o [guia do Modelo de Aplicativo Seguro](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) para obter mais informações. Todos os parceiros que desenvolveram uma integração personalizada usando qualquer API (como as APIs do Azure Resource Manager, do Microsoft Graph, do Partner Center, etc.) ou que implementaram uma automação personalizada usando ferramentas como o PowerShell, precisarão adotar a [estrutura do Modelo de Aplicativo Seguro](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) para se integrar com os serviços em nuvem da Microsoft.

### <a name="what-is-the-secure-application-model"></a>O que é o Modelo de Aplicativo Seguro?

A Microsoft está introduzindo uma estrutura segura e escalonável para autenticar parceiros do CSP (Provedor de Soluções na Nuvem) e CPVs (Fornecedores de Painel de Controle) que aproveitam a Autenticação Multifator. Consulte o [guia do Modelo de Aplicativo Seguro](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) para obter mais informações.  

### <a name="how-do-i-implement-the-secure-application-model"></a>Como faço para implementar o Modelo de Aplicativo Seguro?

Todos os parceiros que desenvolveram uma integração personalizada usando qualquer API (como as APIs do Azure Resource Manager, do Microsoft Graph, do Partner Center, etc.) ou que implementaram uma automação personalizada usando ferramentas como o PowerShell, precisarão adotar a [estrutura do Modelo de Aplicativo Seguro](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) para se integrar com os serviços em nuvem da Microsoft. Deixar de fazer isso pode resultar em uma interrupção devido à implantação da MFA. Os recursos a seguir fornecem uma visão geral e orientações a respeito de como adotar o modelo.

- [Visão geral do Modelo de Aplicativo Seguro](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [Partner Center: guia do Modelo de Aplicativo Seguro](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Parceiros no programa CSP: código de exemplo em .NET para habilitar o Modelo de Aplicativo Seguro](https://docs.microsoft.com/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [Parceiros no programa CSP: código de exemplo em Java para habilitar o Modelo de Aplicativo Seguro](https://docs.microsoft.com/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [Documento de autenticação do Partner Center](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
- [Documento de MFA (Autenticação Multifator) do PowerShell do Partner Center](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth)

Se você estiver usando um painel de controle, precisará consultar o fornecedor com relação à adoção da estrutura Modelo de Aplicativo Seguro.

Os fornecedores de painel de controle são obrigados a se [integrar](enroll-as-cpv.md) com o Partner Center como fornecedores de painel de controle e começar a implementar esses requisitos imediatamente. Confira [Partner Center: estrutura do Modelo de Aplicativo Seguro](https://assetsprod.microsoft.com/secure-application-model-guide.pdf). Os fornecedores de painel de controle devem aceitar e gerenciar o consentimento dos parceiros do CSP em vez de credenciais e limpar todas as credenciais de parceiros do CSP existentes.

### <a name="does-the-secure-application-model-need-to-be-implemented-for-the-partner-center-apisdk-only"></a>O Modelo de Aplicativo Seguro precisa ser implementado somente para a API/o SDK do Partner Center?

Por meio da imposição da autenticação multifator a todas as contas de usuário, qualquer automação ou integração destinada à execução não interativa será afetada. Embora os requisitos de segurança do parceiro exijam que você habilite o modelo de aplicativo seguro para a API do Partner Center, ele pode ser utilizado para atender à necessidade de um segundo fator de autenticação com automação e integração.

>[!Note] 
>Os recursos que estão sendo acessados precisarão ser compatíveis com a autenticação baseada em token de acesso.

### <a name="i-am-using-automation-tools-such-as-powershell-how-do-i-implement-the-secure-application-model"></a>Estou usando ferramentas de automação, como o PowerShell. Como faço para implementar o Modelo de Aplicativo Seguro?

Você precisará implementar o Modelo de Aplicativo Seguro se a automação for destinada à execução não interativa e depender de credenciais do usuário para autenticação. Confira [Modelo de Aplicativo Seguro | PowerShell do Partner Center](https://docs.microsoft.com/powershell/partnercenter/secure-app-model?view=partnercenterps-1.5) para obter orientação sobre como implementar essa estrutura.  

>[!Note] 
>Nem todas as ferramentas de automação fornecem autenticação com tokens de acesso. Poste uma mensagem no grupo [Diretrizes de Segurança da Central de Parceiros](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) caso precise obter ajuda para entender quais alterações são necessárias. 

### <a name="what-user-credentials-should-the-application-administrator-provide-when-performing-the-consent-process"></a>Quais credenciais de usuário o administrador de aplicativos deve fornecer ao executar o processo de consentimento?

É recomendável que você use uma conta de serviço à qual tenha sido atribuído o menor nível de permissões. Em relação à API do Partner Center, você deve usar uma conta que tenha recebido a função Agente de Vendas ou Agente Administrativo.

### <a name="why-should-the-application-administrator-not-provide-global-admin-user-credentials-when-performing-the-consent-process"></a>Por que o administrador de aplicativos não deve fornecer credenciais de usuário administrador global ao executar o processo de consentimento?

É uma melhor prática usar identidades com privilégios mínimos; dessa forma, você reduzirá o risco. Não é recomendável usar uma conta que tenha privilégios de administrador global, pois isso fornece mais permissões do que o necessário.

### <a name="i-am-a-csp-partner-how-do-i-know-if-my-control-panel-vendor-cpv-is-working-on-implementing-the-solution-or-not"></a>Eu sou um parceiro do CSP. Como faço para saber se o meu CPV (Fornecedor de Painel de Controle) está trabalhando para implementar a solução ou não?

Para parceiros que usam a solução de um CPV (Fornecedor de Painel de Controle) para realizar transações no programa do CSP (Provedor de Soluções na Nuvem), é sua responsabilidade consultar seu CPV.

### <a name="who-is-a-control-panel-vendor-cpv"></a>Quem é um CPV (Fornecedor de Painel de Controle)?

Um Fornecedor de Painel de Controle é um fornecedor independente de software que desenvolve aplicativos a serem usados por Parceiros do CSP para integração com as APIs do Partner Center. Um fornecedor de painel de controle não é um Parceiro CSP com acesso direto às APIs ou ao Painel da Central de Parceiros. Uma descrição detalhada está disponível no guia [Partner Center: Modelo de Aplicativos Seguros](https://assetsprod.microsoft.com/secure-application-model-guide.pdf).

### <a name="i-am-a-cpv-how-do-i-enroll"></a>Eu sou um CPV. Como faço para me registrar?

Para se registrar como um CPV (Fornecedor de Painel de Controle), siga as orientações fornecidas [aqui](enroll-as-cpv.md).

Os CPVs precisam entrar em contato pelo email [CPVHelp@microsoft.com](mailto:CPVHelp@microsoft.com) para receber o link de registro e fornecer um patrocinador funcionário da Microsoft que mantenha uma relação comercial com o CPV ou que tenha conhecimento dos negócios realizados por ele. Por exemplo, um PDM (Gerente de Desenvolvimento de Parceiros).

Depois de se registrar e registrar seus aplicativos na Central de Parceiros, você terá acesso às APIs da Central de Parceiros. Você receberá as informações de área restrita por meio de uma notificação da Central de Parceiros se for um novo CPV. Depois de concluir o registro como CPV da Microsoft e aceitar o contrato de CPV, você poderá:

1. Gerenciar aplicativos multilocatários (adicionar aplicativos ao portal do Azure e registrar e cancelar o registro de aplicativos no Partner Center).

   >[!Note]
   >os CPVs deverão registrar seus aplicativos no Partner Center para serem autorizados a usar as APIs do Partner Center. Apenas adicionar aplicativos ao portal do Azure não autoriza os aplicativos de CPV a usarem as APIs do Partner Center.

1. Exiba e gerencie seu perfil de CPV.

1. Exiba e gerencie seus usuários que precisam de acesso aos recursos de CPV. Um CPV só pode ter o administrador global da função.

### <a name="i-am-using-the-partner-center-sdk-will-sdk-automatically-adopt-the-secure-application-model"></a>Estou usando o SDK do Partner Center. O SDK adotará automaticamente o Modelo de Aplicativo Seguro?

Não, você precisará seguir as diretrizes fornecidas no [guia do Modelo de Aplicativo Seguro](https://assetsprod.microsoft.com/secure-application-model-guide.pdf).

### <a name="can-i-generate-a-refresh-token-for-the-secure-application-model-with-accounts-that-dont-have-mfa-enabled"></a>Posso gerar um token de atualização para o Modelo de Aplicativo Seguro com as contas que não têm a MFA habilitada?

Sim, é possível gerar um token de atualização com uma conta que não imponha a MFA. No entanto, deve-se evitar isso. Qualquer token gerado usando uma conta que não tenha a MFA habilitada não poderá acessar os recursos devido ao requisito de MFA.

### <a name="how-should-my-application-obtain-an-access-token-if-we-enable-mfa"></a>Como o meu aplicativo deverá obter um token de acesso se habilitarmos a MFA?

Será necessário seguir o [guia do Modelo de Aplicativo Seguro](https://assetsprod.microsoft.com/secure-application-model-guide.pdf), que fornece detalhes sobre como fazer isso e, ao mesmo tempo, manter-se em conformidade com os novos requisitos de segurança. Você pode encontrar um código de exemplo em .NET [aqui](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model) e um código de exemplo em Java [aqui](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model).

### <a name="as-a-cpv-do-i-create-an-azure-ad-application-in-our-cpv-tenant-or-the-tenant-of-the-csp-partner"></a>Como um CPV, eu devo criar um aplicativo do Azure AD em nosso locatário do CPV ou no locatário do parceiro do CSP?

O CPV precisará criar o aplicativo do Azure Active Directory no locatário associado ao seu registro como CPV.

### <a name="i-am-a-csp-that-is-using-app-only-authentication-do-i-need-to-make-any-changes"></a>Sou um CSP que está usando a autenticação somente por aplicativo. Eu preciso fazer alguma alteração?

A autenticação somente por aplicativo não é afetada, pois as credenciais de usuário não são usadas para solicitar um token de acesso. Se as credenciais do usuário estiverem sendo compartilhadas, os CPVs (Fornecedores de Painel de Controle) deverão adotar a [estrutura do Modelo de Aplicativo Seguro](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) e limpar todas as credenciais de parceiro existentes que eles tiverem.

### <a name="as-a-cpv-can-i-leverage-the-app-only-authentication-style-to-get-access-tokens"></a>Como um CPV, eu posso aproveitar o estilo de autenticação somente por aplicativo para obter tokens de acesso?

Não, os Fornecedores de Painel de Controle não podem utilizar o estilo de autenticação somente por aplicativo para solicitar tokens de acesso em nome do parceiro. Eles devem implementar o Modelo de Aplicativo Seguro, que utiliza o estilo de autenticação por aplicativo + usuário.

## <a name="technical-enforcement"></a>Imposição técnica

### <a name="what-is-the-activation-of-security-safeguards"></a>O que é a ativação de garantias de segurança?

Todos os parceiros que participam do programa CSP (Provedor de Soluções na Nuvem), CPVs (fornecedores de painel de controle) e consultores devem implementar os requisitos obrigatórios de segurança do parceiro para manter a conformidade.

Para fornecer proteção adicional, a Microsoft iniciou a ativação de garantias de segurança que ajuda os parceiros a proteger os locatários e os clientes obrigando o uso da verificação da MFA (autenticação multifator) para impedir o acesso não autorizado.  

Concluímos com êxito a ativação das funcionalidades de AOBO (administrador em nome de) para todos os locatários de parceiros. Para ajudar a proteger ainda mais os parceiros e os clientes, como meta para o segundo trimestre de 2020, iniciaremos a ativação das transações da Central de Parceiros no CSP, ajudando os parceiros a proteger os negócios e os clientes contra incidentes relacionados a roubo de identidade.

Para obter mais informações, acesse a página [Como obrigar o uso da MFA (Autenticação Multifator) ao locatário de parceiro](partner-security-requirements-mandating-mfa.md).

### <a name="i-am-using-a-third-party-mfa-solution-and-i-am-being-blocked-what-should-i-do"></a>Estou usando uma solução de MFA de terceiros e estou sendo bloqueado, o que devo fazer?

Para validar se a conta que está acessando os recursos foi desafiada pela autenticação multifator, verificaremos a declaração de [referência do método de autenticação](https://tools.ietf.org/html/rfc8176) para ver se a MFA está listada. Algumas soluções de terceiros não emitem essa declaração ou não incluem o valor da MFA. Se a declaração estiver ausente ou se o valor da MFA não estiver listado, não haverá como determinar se a conta autenticada foi desafiada pela autenticação multifator. Será necessário trabalhar com o fornecedor da solução de terceiros a fim de determinar quais ações precisam ser adotadas para que a solução emita a declaração da referência do método de autenticação.

Confira [Teste dos Requisitos de Segurança do Parceiro](https://docs.microsoft.com/powershell/partnercenter/test-partner-security-requirements?view=partnercenterps-2.0) caso não tenha certeza se a sua solução de terceiros está emitindo a declaração esperada.

### <a name="mfa-is-blocking-me-from-supporting-my-customer-using-aobo-what-should-i-do"></a>A MFA está me impedindo de oferecer suporte ao meu cliente usando o AOBO, o que devo fazer?

A imposição técnica dos requisitos de segurança do parceiro verificará se a conta autenticada foi desafiada pela autenticação multifator. Em caso negativo, você será redirecionado para a página de logon e receberá uma solicitação para se autenticar novamente. Confira uma experiência e diretrizes mais detalhadas na documentação [Como obrigar o uso da MFA (Autenticação Multifator) ao locatário de parceiro](partner-security-requirements-mandating-mfa.md#partner-delegated-administration). Caso o domínio não seja federado, após a autenticação bem-sucedida, você precisará configurar a autenticação multifator. Ao concluir essa operação, você poderá gerenciar seus clientes usando o AOBO. Caso o domínio seja federado, você precisará verificar se a conta está sendo desafiada pela autenticação multifator.

## <a name="security-defaults-transition"></a>Transição para os padrões de segurança

### <a name="how-can-i-transition-from-baseline-policies-to-security-defaults-or-other-mfa-solutions"></a>Como fazer a transição das políticas de linha de base para os padrões de segurança ou outras soluções de MFA?

As [políticas de "linha de base" do Azure AD (Azure Active Directory) estão sendo removidas e substituídas](https://docs.microsoft.com/azure/active-directory/fundamentals/whats-new#replacement-of-baseline-policies-with-security-defaults) por "padrões de segurança", um conjunto mais abrangente de políticas de proteção para você e seus clientes. Os [padrões de segurança](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) podem ajudar a proteger a sua organização contra ataques de segurança relacionados a roubo de identidade.

A implementação da MFA (autenticação multifator) será removida devido à desativação das políticas de linha de base se você não tiver feito a transição das políticas de linha de base para a política de padrões de segurança ou para [outras opções de implementação de MFA](partner-security-requirements.md#actions-that-you-need-to-take). Todos os usuários nos seus locatários de parceiros que executam operações protegidas por MFA serão solicitados a concluir a verificação de MFA. Examine diretrizes mais detalhadas [aqui](partner-security-requirements-mandating-mfa.md).
Para manter a conformidade e minimizar as interrupções, execute uma das seguintes ações:

- Transição para os padrões de segurança
    - A política de padrões de segurança é uma das opções que os parceiros podem escolher para implementar a MFA. Ela oferece um nível básico de segurança habilitado sem nenhum custo adicional.
    - Saiba como habilitar a MFA para a sua organização com o Azure AD e examine as [principais considerações sobre os padrões de segurança](partner-security-requirements.md#security-defaults).
    - Habilite a política de padrões de segurança de acordo com as suas necessidades comerciais.
- Transição para o acesso condicional
    - Se a política de padrões de segurança não atender às suas necessidades, habilite o acesso condicional. Para obter mais informações, examine a documentação do acesso condicional do Azure AD.

## <a name="key-resources"></a>Principais recursos

### <a name="how-to-get-started"></a>Como começar

- [Requisitos de segurança de parceiros: guia passo a passo](partner-security-requirements.md).
- Encaminhe suas perguntas e seus comentários para este [Grupo de Orientação de Segurança do Partner Center](https://aka.ms/MPCSecurityGuidance).
- Participe dos próximos webinars e horários de escritório do parceiro. Confira [aqui informações detalhadas sobre os recursos e o cronograma](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance).

### <a name="resources-for-adopting-secure-application-model"></a>Recursos para adotar o Modelo de Aplicativo Seguro

- [Visão geral do Modelo de Aplicativo Seguro](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [Partner Center: guia do Modelo de Aplicativo Seguro](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Parceiros no programa CSP: código de exemplo em .NET para habilitar o Modelo de Aplicativo Seguro](https://docs.microsoft.com/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [Parceiros no programa CSP: código de exemplo em Java para habilitar o Modelo de Aplicativo Seguro](https://docs.microsoft.com/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [Documento de autenticação do Partner Center](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
- [Documento de MFA (Autenticação Multifator) do PowerShell do Partner Center](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth)

## <a name="support"></a>Suporte

### <a name="where-can-i-get-support"></a>Onde posso obter suporte?

Para obter recursos de suporte a fim de atender aos requisitos de segurança, se você tiver o ASfP (Suporte Avançado para Parceiros), entre em contato com seu Gerente de Conta de Serviço; se tiver o contrato de PSfP (Suporte Premier para Parceiros), entre em contato com o Gerente de Conta de Serviço e o Gerente de Conta Técnico.

### <a name="how-do-i-get-technical-information-and-support-to-help-me-adopt-secure-application-model-framework"></a>Como faço para obter informações técnicas e suporte para me ajudar a adotar a estrutura do Modelo de Aplicativo Seguro?

Há opções de suporte técnico de produto do Azure Active Directory disponíveis por meio dos seus benefícios do MPN. Parceiros com acesso a assinaturas ativas do ASfP ou do PSfP podem trabalhar com seus Gerentes de Conta associados (SAM/TAM) para entender melhor as opções disponíveis.

### <a name="how-do-i-contact-support-when-ive-lost-access-to-partner-center"></a>Como fazer para entrar em contato com o suporte quando eu tiver perdido o acesso ao Partner Center?

Acesse o [Suporte a Parceiros da Microsoft](https://partner.microsoft.com/support) e escolha **Mostrar todas as opções de suporte**. Você verá as opções disponíveis para entrar em contato com o Suporte do Parceiro da Microsoft, incluindo um número de telefone para ligar para o suporte e uma opção para conversar com o suporte.

### <a name="where-can-i-find-more-information-about-common-technical-issues"></a>Onde posso encontrar mais informações sobre problemas técnicos comuns?

Informações sobre os problemas técnicos comuns podem ser encontradas em [Requisitos de segurança de parceiros para parceiros usando o Partner Center ou as APIs do Partner Center](partner-security-requirements.md)
