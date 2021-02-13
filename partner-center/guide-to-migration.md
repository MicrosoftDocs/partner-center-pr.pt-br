---
title: Migrar do PMC para o Partner Center
ms.topic: article
ms.date: 10/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como migrar sua empresa do PMC (Partner Membership Center) para o Partner Center, incluindo as etapas que você deverá seguir.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: dd566a6d9ef60747eb7fd515b4d63d87d991da2a
ms.sourcegitcommit: d37a3f353426e52dfbbac577b7576f9c3f6d2ddf
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "99624180"
---
# <a name="guide-to-migrating-from-pmc-to-partner-center"></a>Guia de migração do PMC para o Partner Center

**Funções apropriadas**

- Administrador global

O site do parceiro da Microsoft em partner.microsoft.com é uma experiência digital unificada para parceiros. No site do parceiro, você poderá explorar suas oportunidades e se envolver em experiências guiadas que ajudam a sua empresa a criar e comercializar seus aplicativos e seus serviços com a Microsoft. Usando o link do painel que está disponível no site do parceiro, os membros do Microsoft Partner Network podem entrar no Partner Center, no qual você gerencia seu relacionamento com a Microsoft, registra-se em programas e inscreve-se em ofertas.

O PMC (Partner Membership Center) está sendo desativado. Sua empresa foi convidada a fazer a transição do gerenciamento de sua associação do Microsoft Partner Network para o Partner Center. Este guia preparará você para o que esperar durante a migração do PMC para o Partner Center.

>[!NOTE]
>Mesmo que a sua empresa tenha mais de uma conta ou localização, a migração para o Partner Center começa com a migração de uma (sua primeira) conta para o Partner Center.

## <a name="get-started"></a>Introdução

A migração começa no PMC. Seu administrador global receberá um convite para iniciar a migração.

### <a name="prepare-in-pmc"></a>Preparar-se no PMC

- Verificar os detalhes da empresa
- Verificar o contato principal do programa
- Verificar as localizações da empresa
- Atualizar seus usuários aprovados

### <a name="when-youre-ready"></a>Quando estiver pronto

Selecione **Introdução** no convite. Você será levado para a página de entrada do Partner Center.

:::image type="content" source="images/migration/getstarted.jpg" alt-text="Introdução":::

## <a name="start-with-your-work-email"></a>Começar com seu email de trabalho

Caso a sua empresa não tenha um email de trabalho e um locatário do AAD, poderemos ajudar você a configurar um durante o processo de conexão ao Partner Center. Ao tentar entrar com uma conta de email que não seja um email de trabalho, como a sua conta pessoal, você será direcionado para fornecer informações sobre a sua empresa, de modo que possamos configurar um locatário do AAD e um email de trabalho. Esses detalhes da empresa serão usados para finalizar sua conta no Partner Center, portanto, verifique se eles são precisos.

>[!NOTE]
>Se você for um parceiro na China e estiver registrado no programa Microsoft Partner Network e CSP (Provedor de Soluções na Nuvem), terá um locatário separado para cada conta. Sua conta com o programa Provedor de Soluções na Nuvem é gerenciada na nuvem nacional e sua conta do Microsoft Partner Network é gerenciada na nuvem global. As duas contas não podem ser vinculadas.

:::image type="content" source="images/migration/newtellusabout.png" alt-text="Conte-nos sobre a sua empresa":::

Depois de verificar ou atualizar as informações, selecione **Aceitar e continuar**.
Os Termos e as Condições nesta página são **exatamente os mesmos** indicados no contrato que a sua empresa já assinou no PMC.  
Esta etapa inicia a criação do seu locatário do Azure AD e fornece a você a conta corporativa.

A seleção de **Aceitar e continuar** também faz o seguinte:

- Migra sua conta junto com TODOS os locais para o Partner Center

- Migra as competências ou os MAPs que você possa ter adquirido no PMC

- Migra quaisquer recursos, ofertas e programas de marketing (MAPs, Silver, Gold) que você tinha no PMC

## <a name="invite-employees-to-join-you"></a>Convidar os funcionários para ingressar junto com você

Quando o novo locatário do Azure AD for criado, você poderá convidar seus funcionários para entrar no Partner Center.

:::image type="content" source="images/migration/invite.png" alt-text="Convidar funcionários":::

Se você tiver entrado com um locatário existente do AAD, seus funcionários terão se movido com você. Nesse caso, atribua aos funcionários funções que determinem o que elas podem fazer no Partner Center. 

>[!NOTE] 
>As funções no Partner Center são diferentes das funções no PMC. Para obter mais informações, confira [Como migrar do PMC para o Partner Center](move-pmc-pc-map.md).

## <a name="verify-your-domain-and-become-a-global-admin"></a>Verificar seu domínio e tornar-se um administrador global  

Se o locatário do AAD for novo, ninguém receberá a função de administrador global. Para se tornar o administrador global, você precisará verificar a propriedade do domínio. Talvez você precise do administrador de domínio para ajudar você com isso.

Embora seja possível usar as ofertas compradas, você não poderá comprar novas ofertas até concluir a etapa de atribuição de um administrador global.

:::image type="content" source="images/migration/takecontrol.png" alt-text="Assumir o controle":::

Ao selecionar Introdução, você verá a seguinte tela:

:::image type="content" source="images/migration/verifytxt.png" alt-text="Verificar a propriedade do domínio":::

Seu registrador de domínios já estará preenchido para você. Somente o proprietário do domínio pode atualizar o arquivo DNS; portanto, copiando e adicionando o arquivo de texto ao registro DNS, podemos verificar se você é o proprietário. Levará alguns minutos para que a atualização ocorra. Você precisará sair do Partner Center e entrar novamente. Sua função terá sido alterada para administrador global.

## <a name="get-acquainted-with-your-dashboard-and-partner-center"></a>Familiarizar-se com o painel e o Partner Center

Faça um tour pelo painel. É nele que você pode gerenciar sua associação, adicionar um perfil de negócios para indicações, registrar-se no programa Provedor de Soluções na Nuvem e ver notificações e ofertas relevantes para sua empresa a qualquer momento selecionando **Painel**. Você também pode gerenciar incentivos, fazer compras no Marketplace, inscrever-se em serviços de entrada no mercado, entre outros.  

:::image type="content" source="images/migration/fre.png" alt-text="Fazer o tour":::

## <a name="sign-the-microsoft-partner-agreement"></a>Assinar o Contrato de Parceiro da Microsoft

Se for um revendedor indireto, quando tiver configurado sua conta do Partner Center, você ainda precisará se registrar oficialmente no programa Provedor de Soluções na Nuvem. Para verificar seu status de associação, acesse seu [Perfil legal](https://partner.microsoft.com/pcv/accountsettings/partnerprofile) e confirme o tipo de conta. Em seguida, inscreva-se no CSP como um [revendedor indireto](enrolling-in-the-csp-program.md).

 Após inscrever-se como um revendedor indireto, aceite a [solicitação de relacionamento de CSP com seu provedor indireto](indirect-reseller-tasks-in-partner-center.md).

Em seguida, aceite o Contrato de Parceiro da Microsoft no [painel](https://partner.microsoft.com/pvc/dashboard) do Partner Center usando as credenciais de administrador global. Confirme que você assinou o Contrato de Parceiro da Microsoft na seção Informações do Programa do perfil do parceiro. Além disso, você verá uma barra de notificação de confirmação na página Visão Geral do CSP. 

## <a name="next-steps"></a>Próximas etapas

- [Encontrar seu administrador global](become-global-admin.md)

- [Contrato de Parceiro da Microsoft](microsoft-partner-agreement.md)

- [Criar contas de usuário](create-user-accounts-and-set-permissions.md)

- [Atribuir funções e permissões de usuário](permissions-overview.md)

- [Gerenciar seus programas de associação](renew-mpn-offers.md)

- [Criar perfil de negócios da sua empresa](create-a-marketing-profile.md)

- [Conectar-se com clientes por meio de indicações](manage-leads.md)

- [Guia de migração de várias empresas do PMC para o Partner Center](move-multiple-companies.md)
