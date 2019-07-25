---
title: Perguntas frequentes sobre requisitos de segurança do parceiro | Centro de parceiros
ms.topic: article
ms.date: 07/18/2019
description: Perguntas frequentes sobre os requisitos de segurança do parceiro
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, provedor de soluções na nuvem, programa de provedor de soluções na nuvem, CSP, fornecedor do painel de controle, CPV, autenticação multifator, MFA, modelo de aplicativo seguro, modelo de aplicativo seguro, segurança
ms.localizationpriority: medium
ms.openlocfilehash: 1a178dc71f8042e6b39a316c6c889b619aaed12c
ms.sourcegitcommit: 5c8ac1b6d29d183d85582d6eb32e37b91dd8c6c1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2019
ms.locfileid: "68315545"
---
# <a name="frequently-asked-questions-about-the-partner-security-requirements"></a>Perguntas frequentes sobre os requisitos de segurança do parceiro

Este artigo contém algumas perguntas frequentes para os [requisitos de segurança do parceiro](partner-security-requirements.md). Você pode encontrar uma lista abrangente de perguntas frequentes [aqui](http://assetsprod.microsoft.com/security-requirements-faq.pdf).

## <a name="conditional-access"></a>Acesso condicional

### <a name="can-conditional-access-be-used"></a>O acesso condicional pode ser usado?

Sim, você pode usar o acesso condicional para impor a MFA para cada usuário, incluindo contas de serviço, em seu locatário de parceiro. No entanto, considerando a natureza altamente privilegiada de ser um parceiro, precisamos garantir que cada usuário tenha um desafio de MFA para cada autenticação única. Isso significa que você não poderá aproveitar o recurso de acesso condicional que contorne o requisito para MFA.

## <a name="multi-factor-authentication"></a>Autenticação Multifator

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a>Meus clientes estão sujeitos aos requisitos de segurança do parceiro?

Não, não é necessário impor a MFA para cada usuário nos locatários do Azure AD do seu cliente. No entanto, é recomendável que você trabalhe com cada cliente para determinar a melhor maneira de proteger seus usuários.

### <a name="can-app-passwords-be-used-with-the-baseline-protection-policies"></a>As senhas de aplicativo podem ser usadas com as políticas de proteção de linha de base?

Sim, [as senhas de aplicativo](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) podem ser usadas. Você deve examinar as considerações para usar senhas de aplicativo documentadas [aqui](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) para determinar se há suporte para sua necessidade.

### <a name="can-any-user-be-excluded-from-this-requirement"></a>Qualquer usuário pode ser excluído deste requisito? 

Não, cada usuário, incluindo contas de serviço, no seu locatário do parceiro será solicitado a autenticar usando o MFA.

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a>Os requisitos de segurança do parceiro se aplicam à área restrita da integração?

Sim, os requisitos de segurança do parceiro se aplicam à área restrita da integração. Isso significa que você precisará implementar a solução MFA apropriada para usuários no locatário da área restrita da integração. É recomendável que você implemente as políticas de proteção de linha de base para fornecer MFA.

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a>Como fazer configurar uma conta de acesso de emergência (interrupção)?

Ele considerou a prática recomendada criar uma ou duas contas de acesso de emergência para evitar o bloqueio inadvertidamente do seu locatário do Azure AD. Em relação aos requisitos de segurança do parceiro, é necessário que cada usuário seja autenticado usando o MFA. Portanto, isso significa que você precisará modificar a definição de uma conta de acesso de emergência. Pode ser uma conta que esteja aproveitando uma solução de terceiros para MFA.

### <a name="how-will-guest-users-be-impacted-by-the-partner-security-requirements"></a>Como os usuários convidados serão afetados pelos requisitos de segurança do parceiro?

Os usuários convidados serão solicitados a autenticar-se usando o MFA, ao acessar recursos no seu locatário do parceiro. Os requisitos de segurança do parceiro não terão impacto sobre o usuário convidado que acessará os recursos em seu próprio locatário.

### <a name="if-i-am-using-a-third-party-solution-is-active-directory-federation-service-adfs-required"></a>Se eu estiver usando uma solução de terceiros, o ADFS (Active Directory Serviço de Federação) será necessário? 

Não, não é necessário ter Active Directory Serviço de Federação (ADFS) se você estiver usando uma solução de terceiros. É recomendável que você trabalhe com o fornecedor da solução para determinar quais são os requisitos para sua solução.

### <a name="is-it-a-requirement-to-enable-the-baseline-protection-policies"></a>É um requisito para habilitar as políticas de proteção de linha de base?

Não, não é necessário que você habilite as políticas de proteção de linha de base. O único requisito é que você aplique a MFA para cada usuário, incluindo contas de serviço, em seu locatário de parceiro.

### <a name="what-verification-options-are-provided-through-the-implementation-of-the-baseline-protection-policies"></a>Quais opções de verificação são fornecidas por meio da implementação das políticas de proteção de linha de base? 

Em relação à versão do MFA que está disponível por meio da implementação das políticas de proteção de linha de base, a única opção de verificação disponível é um aplicativo autenticador. O uso de uma chamada telefônica e mensagem de mensagem de texto é considerado menos seguro. Portanto, essas opções não estão disponíveis por meio desta versão do MFA.

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>A conta de serviço usada pelo Azure AD Connect ser afetada pelos requisitos de segurança do parceiro?

Não, a conta de serviço usada pelo Azure AD Connect não será afetada pelos requisitos de segurança do parceiro. Se você tiver um problema com Azure AD Connect como resultado da imposição da MFA, abra uma solicitação de suporte técnico com o suporte da Microsoft.
