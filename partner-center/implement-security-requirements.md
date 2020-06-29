---
title: Implementar os requisitos de segurança de parceiros
ms.topic: article
ms.date: 06/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como implementar os requisitos de segurança necessários para os seus usuários
author: LauraBrenner
ms.author: labrenne
keywords: segurança
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: d162e8c5fd3cfd335920e4cc5fc826c3622f633c
ms.sourcegitcommit: 562535a4b16a8217c1e1945b7663ca3735e1ee27
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2020
ms.locfileid: "85133258"
---
# <a name="implement-the-partner-security-requirements"></a>Implementar os requisitos de segurança de parceiros

**Funções apropriadas**

- Administrador global

A segurança e a privacidade de clientes e parceiros são as prioridades da Microsoft. Continuamos vendo um crescente número de ataques de segurança mais sofisticados, principalmente relacionados a identidades comprometidas. Como os controles de prevenção desempenham uma função fundamental na estratégia global de defesa para frustrar os ataques de segurança, passaremos a impor um conjunto de requisitos de segurança obrigatórios para ajudar a proteger os parceiros e seus clientes.

Usando este tutorial, você aprenderá mais sobre os requisitos de segurança do parceiro, como atendê-los e o impacto nos usuários em seu diretório de parceiros.

Todos os parceiros que estão participando do programa Provedor de Soluções na Nuvem, os Fornecedores do Painel de Controle e os parceiros do Advisor devem impor a MFA (Autenticação Multifator) para cada usuário em seu locatário de parceiro. Essa imposição pode ser feita habilitando duas [políticas de linha de base do Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection). As políticas de linha de base são um conjunto de políticas predefinidas que ajudam a proteger as empresas contra muitos ataques comuns. Esses ataques comuns podem incluir pulverização, reprodução e phishing de senha. As políticas de linha de base estão disponíveis em todas as edições do Azure Active Directory. A Microsoft está disponibilizando essas políticas de proteção de linha de base para todos, pois o volume de ataques baseados em identidade vem aumentando nos últimos anos.

Os procedimentos a seguir descrevem o processo de habilitar as duas políticas de linha de base necessárias:

- **Exigir MFA para administradores** Habilitar a política "Exigir MFA para administradores" fará com que os usuários nas funções de administrador se registrem na MFA usando o aplicativo autenticador. Depois que o registro de MFA for concluído, os administradores precisarão executar a MFA sempre que entrarem.

- **Proteção do usuário final** A proteção do usuário final é uma política de linha de base da MFA baseada em risco que protege todos os usuários em um diretório. A habilitação dessa política exige que todos os usuários se registrem na MFA usando o aplicativo autenticador. Os usuários podem ignorar o prompt de registro de MFA por 14 dias, após o qual eles serão impedidos de entrar até que se registrem na MFA. Depois de registrado para MFA, os usuários serão solicitados a receber MFA somente durante tentativas de inserção de credenciais arriscadas. As contas de usuário comprometidas são bloqueadas até que a senha seja redefinida e os eventos de risco tenham sido ignorados.

Quando essas políticas estiverem habilitadas, cada usuário poderá utilizar o MFA do Azure sem custo adicional. Se você estiver usando uma solução de terceiros, você deverá impor a MFA para cada usuário ao acessar os serviços de nuvem comercial da Microsoft.

>[!NOTE]
>Como a MFA será imposta para cada usuário no diretório de parceiros, haverá um impacto em qualquer automação ou integração que utiliza credenciais do usuário. Para resolver esse impacto, será necessário modificar a maneira como a automação ou a integração se conecta aos serviços de nuvem comercial da Microsoft. Se o serviço ao qual você estiver se conectando for compatível à autenticação baseada em token, será recomendável implementar a [estrutura do Modelo de Aplicativo Seguro](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model).

## <a name="step-one-block-any-existing-legacy-authentication-protocols"></a>Etapa 1: Bloquear quaisquer protocolos de autenticação herdados existentes

Antes de habilitar as políticas "Exigir MFA para administradores" e "Proteção do usuário final", verifique se os usuários não estão usando protocolos de autenticação herdados. Confira o artigo [Como bloquear a autenticação herdada no Azure AD com Acesso Condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection#identify-legacy-authentication-use) para obter mais informações.

## <a name="step-two-enable-the-require-mfa-for-admins-baseline-policy"></a>Etapa 2: Habilitar a política de linha de base "Exigir MFA para administradores"

A política de linha de base Exigir MFA para administrador requer a MFA para as funções de diretório a seguir, que são consideradas as funções mais privilegiadas do Azure AD:

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

5. Selecione  **Salvar**.

Após habilitar essa política, os usuários nas funções de administrador acima serão solicitados a entrar para fornecer mais informações de segurança e configurar o aplicativo móvel. Depois disso, será possível entrar no serviço de nuvem apropriado.

## <a name="step-three-enable-the-end-user-protection-baseline-policy"></a>Etapa 3: Habilitar a política de linha de base "Proteção do usuário final"

A política de linha de base de proteção do usuário final protege todos os usuários em um diretório. A habilitação dessa política exige que todos os usuários se registrem na MFA do Azure em até 14 dias. Depois de registrados, os usuários serão solicitados a receber MFA somente durante tentativas de entradas arriscadas; esse comportamento mudará para locatários de parceiros no futuro. Contas de usuário comprometidas são bloqueadas até a redefinição de senha e risco de demissão.

A política de linha de base: "Proteção do usuário final" vem pré-configurada e aparecerá na parte superior quando você navegar para a folha Acesso Condicional no portal do Azure.

Para habilitar essa política e proteger seus usuários:

1. Entre no **portal do Azure** como administrador global, administrador de segurança ou administrador de acesso condicional.

2. Navegue até o **Azure Active Directory** > **Acesso Condicional**.

3. Na lista de políticas, selecione a **política de linha de base: Proteção do usuário final (visualização)** .

4. Defina **Habilitar política** para **Usar política imediatamente**.

5. Selecione  **Salvar**.

Após habilitar essa política, todos os usuários serão solicitados a entrar para fornecer mais informações de segurança e configurar o aplicativo móvel. Depois disso, será possível entrar no serviço de nuvem apropriado.

>[!NOTE]
>Até que os requisitos de segurança do parceiro sejam impostos, os usuários que não forem cobertos pela política de linha de base "Exigir MFA para administradores" só serão consultados para a MFA com base no risco.