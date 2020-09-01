---
title: Solucionar problemas de configuração da conta do Partner Center ou dos problemas de renovação do MPN
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Solucionar problemas com o registro no Partner Center
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c1d850663224469f24d5d4442e33cc17c1bb6704
ms.sourcegitcommit: 5f31146f50e01dc4c1922e0a5bc369f0a3cd8162
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/01/2020
ms.locfileid: "89220234"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>Solucionar problemas de configuração de conta ou de renovação de MPN

**Aplica-se a**

- Partner Center
 
**Funções apropriadas**

- Administrador global
- Administrador de parceiros do MPN 
 
Aqui estão algumas sugestões para solucionar problemas comuns que surgem ao configurar sua conta do Partner Center.

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>O que acontece se você estiver migrando do centro de associação de parceiro e não for possível editar os campos de informações da empresa

Isso ocorre nos casos em que sua empresa já tem uma presença no Partner Center (digamos, conta CSP) – você verá uma tela somente leitura que exibirá todas as informações sobre a sua empresa, como existe no Partner Center.

Você não pode alterar os detalhes nesta tela. Isso é por design e não é um erro.

Selecione **aceitar** e **continuar** para continuar.

## <a name="you-are-trying-to-enroll-or-to-migrate-from-partner-membership-center-and-you-receive-an-error-message-saying-that-the-it-department-has-turned-off-sign-up-for-partner-center"></a>Você está tentando registrar ou migrar do centro de associação de parceiro e recebe uma mensagem de erro informando que o departamento de ti desativou a **inscrição no Partner Center**.

Você vê essa mensagem porque os usuários viral estão desabilitados ou a inscrição viral está desabilitada no locatário do Azure AD. O administrador global da sua conta do Azure AD pode habilitar os recursos necessários executando o seguinte comando do PowerShell:

**Set-MsolCompanySettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**

Para obter mais informações, leia [inscrição de autoatendimento](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-self-service-signup)

## <a name="you-forgot-your-password"></a>Você esqueceu sua senha

Se você esqueceu sua senha, selecione o link **não consegue acessar sua conta?** na página de entrada para redefinir sua senha ou peça ao administrador global para atribuir novas credenciais.

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>Na tela "Conte-nos sobre sua empresa", você recebe um erro "algo deu errado"

Isso geralmente acontece se você usar inadvertidamente caracteres especiais, espaços ou códigos de país no número de telefone da empresa. O valor inserido no campo número de telefone pode conter apenas um máximo de 10 caracteres.

## <a name="you-are-trying-to-complete-the-purchase-via-credit-card-but-you-are-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>Você está tentando concluir a compra por meio de cartão de crédito, mas está recebendo uma mensagem de erro informando que "seu pedido foi recusado. Verifique suas informações "

Você sempre deve inserir o endereço correspondente ao seu cartão de crédito e não correspondente à sua entidade legal. Além disso, verifique se o CEP está correto e corresponde ao endereço que você usa.

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>Você deseja alternar de pagamento offline para método de pagamento online 

Você precisará cancelar o pedido original e adquirir novamente-lo usando o método de pagamento preferencial.

Para cancelar um pedido:

1. Selecione a guia **ofertas de associação** no painel.

2. Selecione **Cancelar pedido**

3. Uma janela de confirmação será exibida e você deverá confirmar para cancelar a ordem inicial.
