---
title: Solucionar problemas de configuração de sua Partner Center ou problemas de renovação do MPN
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Solucionar problemas ao tentar se registrar no Partner Center. As respostas abordam desafios com formas de pagamento, esquecer senhas e muito mais.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f34adc57e668caecb69af37afc72b5153f667335
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686255"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>Solucionar problemas de configuração de conta ou renovação do MPN


**Funções apropriadas**

- Administrador global
- Administrador de parceiros do MPN
 
Aqui estão algumas sugestões para solucionar problemas comuns que surgem ao configurar sua Partner Center conta.

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>O que acontece se você estiver migrando do Partner Membership Center e não puder editar nenhum campo de informações da empresa

Nos casos em que sua empresa já tem uma presença Partner Center (por exemplo, uma conta CSP) – você receberá uma tela somente leitura. Esta tela exibirá todas as informações sobre sua empresa como ela existe Partner Center.

Você não pode alterar os detalhes nesta tela. Isso ocorre por design e não por um erro.

Selecione **Aceitar** e **Continuar** para continuar.


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a>Se o departamento de IT tiver desligado **Inscrever-se para Partner Center**

Você verá essa mensagem porque os usuários vírus estão desabilitados ou porque a Assinatura Viral está desabilitada no locatário do Azure AD. O administrador global da sua conta do Azure AD pode habilitar os recursos necessários executando o seguinte comando do PowerShell:

**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**

Para obter mais informações, leia [Inscrever-se por autoatend site.](/azure/active-directory/users-groups-roles/directory-self-service-signup)

## <a name="you-forgot-your-password"></a>Você esqueceu sua senha

Se você esqueceu sua senha, selecione o link **Não é possível acessar sua conta?** na página de entrada. Essa opção permite que você redefina sua senha ou peça ao administrador global para atribuir novas credenciais.

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>Na tela "Conte-nos sobre sua empresa", você receberá um erro "Algo deu errado"

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
