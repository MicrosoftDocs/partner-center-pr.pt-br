---
title: Solucionar problemas de configuração da conta do Partner Center ou dos problemas de renovação do MPN
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Solucionar problemas ao tentar se registrar no Partner Center. Responde a desafios de endereços com métodos de pagamento, esquecer senhas e muito mais.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6bf3e3af8e0d1d87a63f86e892d8bddcd74b6460
ms.sourcegitcommit: 0e142b4fbb044fe8dd2dbc7d13ab70a1a91b9f60
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2020
ms.locfileid: "94381402"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>Solucionar problemas de configuração de conta ou de renovação de MPN

**Aplica-se a**

- Partner Center
 
**Funções apropriadas**

- Administrador global
- Administrador de parceiros do MPN 
 
Aqui estão algumas sugestões para solucionar problemas comuns que surgem ao configurar sua conta do Partner Center.

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>O que acontece se você estiver migrando do centro de associação de parceiro e não for possível editar os campos de informações da empresa

Nos casos em que sua empresa já tem uma presença no Partner Center (digamos, conta CSP) – você verá uma tela somente leitura. Esta tela exibirá todas as informações sobre sua empresa, pois elas existem no Partner Center.

Você não pode alterar os detalhes nesta tela. Isso é por design e não é um erro.

Selecione **aceitar** e **continuar** para continuar.


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a>Se o departamento de TI tiver desativado a **inscrição no Partner Center**.

Você vê essa mensagem porque os usuários viral estão desabilitados ou porque a inscrição viral está desabilitada no locatário do Azure AD. O administrador global da sua conta do Azure AD pode habilitar os recursos necessários executando o seguinte comando do PowerShell:

**Set-MsolCompanySettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**

Para obter mais informações, leia [inscrição de autoatendimento](/azure/active-directory/users-groups-roles/directory-self-service-signup)

## <a name="you-forgot-your-password"></a>Você esqueceu sua senha

Se você esqueceu sua senha, selecione o link **não consegue acessar sua conta?** na página de entrada. Essa opção permite que você Redefina sua senha ou peça ao administrador global para atribuir novas credenciais.

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>Na tela "Conte-nos sobre sua empresa", você recebe um erro "algo deu errado"

Essa mensagem de erro geralmente aparece se você usar inadvertidamente caracteres especiais, espaços ou código de país no número de telefone da empresa. O valor inserido no campo número de telefone pode conter apenas um máximo de 10 caracteres.


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>Sua compra de cartão de crédito está recebendo uma mensagem de erro informando que "seu pedido foi recusado. Verifique suas informações "


Sempre use o endereço correspondente ao seu cartão de crédito em vez de sua entidade legal. Além disso, verifique se o CEP está correto e corresponde ao endereço que você usa.

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>Você deseja alternar de pagamento offline para método de pagamento online 

Você precisará cancelar o pedido original e adquirir novamente-lo usando o método de pagamento preferencial.

Para cancelar um pedido:

1. Selecione a guia **ofertas de associação** no painel.

2. Selecione **Cancelar pedido**

3. Uma janela de confirmação será exibida e você deverá confirmar para cancelar a ordem inicial.

## <a name="next-steps"></a>Próximas etapas

- [Gerenciar sua conta do Partner Center](partner-center-account-setup.md)
- [Como ler seu arquivo de fatura e reconhecimento](read-your-bill.md)
