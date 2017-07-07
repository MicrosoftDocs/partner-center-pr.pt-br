---
title: "Locatários do Azure Active Directory e o Partner Center | Partner Center"
description: "Para criar uma conta do Partner Center, sua empresa deve ter um locatário do Azure Active Directory (Azure AD). O Azure AD é o diretório baseado em nuvem e o serviço de gerenciamento de identidades da Microsoft."
author: labrenne
robots: 
ms.openlocfilehash: 9a9a3c3aa239017fe8ecf655f79acbfab6ff8a0b
ms.sourcegitcommit: d7c4ca62acd1ef1026c7d322e40f55a83a80e72a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/28/2017
---
# <a name="azure-active-directory-tenants-and-partner-center"></a>Locatários do Azure Active Directory e o Partner Center  

**Aplicável a**

-  Partner Center

## <a name="why-you-need-an-azure-ad-tenant"></a>Por que você precisa de um locatário do Azure AD

Precisamos vincular o locatário do Azure AD de sua organização à sua nova conta do Partner Center para que os usuários do locatário possam se conectar ao Partner Center com seus nomes de usuário e senhas do Azure AD (conta da Microsoft).

Se a sua empresa já tem um locatário do Azure AD, você pode vinculá-lo à sua conta do Partner Center. 

>**Observação**<br> Antes de decidir usar um locatário do Azure AD existente, pense sobre quantos usuários do locatário precisarão trabalhar no Partner Center. Se você tiver usuários no locatário que não precisam trabalhar no Partner Center, considere criar um novo locatário somente para os usuários que precisem trabalhar no Partner Center.

Se a sua empresa não tiver um locatário do Azure AD, você poderá criar um gratuitamente durante o processo de inscrição. Selecione **Criar um novo locatário** na página **Entrar no Azure Active Directory**. 

### <a name="not-sure-if-your-company-already-has-an-azure-ad-tenant"></a>Não tem certeza se a sua empresa já tem um locatário do Azure AD?

Se você não tiver certeza se a empresa tem um locatário do Azure AD, siga estas etapas para verificar. Observe que se você tiver uma assinatura ativa do Microsoft Azure ou Office 365, você já tem um locatário do Azure AD.
1.  Entre no portal do administrador do Azure em https://ms.portal.azure.com
2.  Selecione Azure Active Directory no menu e, em seguida, selecione Nomes de Domínio.
3.  Se você já tiver um locatário, seu nome de domínio estará listado.

### <a name="using-an-existing-tenant"></a>Usando um locatário existente?

Se quiser usar um locatário do Azure AD existente, mas estiver tendo problemas para se conectar, encontre o cenário no diagrama a seguir que melhor corresponda à sua situação e siga as etapas recomendadas. 

![Você tem um locatário do Azure AD ou precisa criar um?](images/onboardingAADFlow.png)

Para saber mais sobre como adicionar domínios no Azure AD, consulte [Adicionar ou associar um domínio no Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-add-domain)

## <a name="about-microsoft-azure"></a>Sobre o Microsoft Azure

O Microsoft Azure é uma plataforma de nuvem pública que as empresas podem usar para compilar, implantar e gerenciar aplicativos em uma rede global de datacenters gerenciados pela Microsoft. As empresas usam o Azure para criar uma infraestrutura de TI virtual com funções virtuais ou serviços, em vez de computadores físicos. 

Ao comprar uma assinatura do Azure, você está essencialmente alugando um espaço dedicado e seguro na nuvem pública do Azure, não muito diferente de alugar um andar de um prédio para abrigar sua empresa física. Para o proprietário do prédio, sua empresa é um locatário. 

Um locatário do Azure AD é uma representação virtual dedicada e isolada de sua empresa na nuvem pública do Azure, criada para você quando assina um serviço em nuvem da Microsoft, como o Azure, o Microsoft Intune ou o Office 365. 

Seu locatário hospeda os usuários do Azure AD e as informações sobre eles: suas senhas, dados de perfil, permissões e assim por diante. O locatário também contém grupos, aplicativos e outras informações relacionadas a uma empresa e sua segurança. 

Para saber mais sobre o Azure AD, consulte a [Documentação do Azure Active Directory](https://docs.microsoft.com/ azure/active-directory/). 