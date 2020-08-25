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
ms.openlocfilehash: a516d569791356c4ba967b8835268562d1597a16
ms.sourcegitcommit: 9bbad472a86086eec684f3b7f4568fdf152f625e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2020
ms.locfileid: "88848919"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="6edbd-103">Solucionar problemas de configuração de conta ou de renovação de MPN</span><span class="sxs-lookup"><span data-stu-id="6edbd-103">Troubleshoot account setup or MPN renewal issues</span></span>

### <a name="applies-to"></a><span data-ttu-id="6edbd-104">Aplica-se a</span><span class="sxs-lookup"><span data-stu-id="6edbd-104">Applies to</span></span>

- <span data-ttu-id="6edbd-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="6edbd-105">Partner Center</span></span>
 
### <a name="appropriate-roles"></a><span data-ttu-id="6edbd-106">Funções apropriadas</span><span class="sxs-lookup"><span data-stu-id="6edbd-106">Appropriate roles</span></span>

- <span data-ttu-id="6edbd-107">Administrador global</span><span class="sxs-lookup"><span data-stu-id="6edbd-107">Global admin</span></span>
- <span data-ttu-id="6edbd-108">Administrador de parceiros do MPN</span><span class="sxs-lookup"><span data-stu-id="6edbd-108">MPN partner admin</span></span> 
 

<span data-ttu-id="6edbd-109">Aqui estão algumas sugestões para solucionar problemas comuns que surgem ao configurar sua conta do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="6edbd-109">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

### <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="6edbd-110">O que acontece se você estiver migrando do centro de associação de parceiro e não for possível editar os campos de informações da empresa</span><span class="sxs-lookup"><span data-stu-id="6edbd-110">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="6edbd-111">Isso ocorre nos casos em que sua empresa já tem uma presença no Partner Center (digamos, conta CSP) – você verá uma tela somente leitura que exibirá todas as informações sobre a sua empresa, como existe no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="6edbd-111">This occurs in cases where your company already has a presence in Partner Center (say CSP account) – you will be shown a read-only screen which will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="6edbd-112">Você não pode alterar os detalhes nesta tela.</span><span class="sxs-lookup"><span data-stu-id="6edbd-112">You cannot change the details on this screen.</span></span> <span data-ttu-id="6edbd-113">Isso é por design e não é um erro.</span><span class="sxs-lookup"><span data-stu-id="6edbd-113">This is by design and not an error.</span></span>

<span data-ttu-id="6edbd-114">Selecione **aceitar** e **continuar** para continuar.</span><span class="sxs-lookup"><span data-stu-id="6edbd-114">Select **Accept** and **Continue** to proceed.</span></span>

### <a name="you-are-trying-to-enroll-or-to-migrate-from-partner-membership-center-and-you-receive-an-error-message-saying-that-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="6edbd-115">Você está tentando registrar ou migrar do centro de associação de parceiro e recebe uma mensagem de erro informando que o departamento de ti desativou a **inscrição no Partner Center**.</span><span class="sxs-lookup"><span data-stu-id="6edbd-115">You are trying to enroll or to migrate from Partner Membership Center and you receive an error message saying that the IT department has turned off **sign up for Partner Center**.</span></span> 

<span data-ttu-id="6edbd-116">Você vê essa mensagem porque os usuários viral estão desabilitados ou a inscrição viral está desabilitada no locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6edbd-116">You see this message because viral users are disabled, or Viral Sign up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="6edbd-117">O administrador global da sua conta do Azure AD pode habilitar os recursos necessários executando o seguinte comando do PowerShell:</span><span class="sxs-lookup"><span data-stu-id="6edbd-117">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="6edbd-118">**Set-MsolCompanySettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="6edbd-118">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="6edbd-119">Para obter mais informações, leia [inscrição de autoatendimento](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-self-service-signup)</span><span class="sxs-lookup"><span data-stu-id="6edbd-119">For more information, read [Self-service sign up](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-self-service-signup)</span></span>

### <a name="you-forgot-your-password"></a><span data-ttu-id="6edbd-120">Você esqueceu sua senha</span><span class="sxs-lookup"><span data-stu-id="6edbd-120">You forgot your password</span></span>

<span data-ttu-id="6edbd-121">Se você esqueceu sua senha, selecione o link **não consegue acessar sua conta?** na página de entrada para redefinir sua senha ou peça ao administrador global para atribuir novas credenciais.</span><span class="sxs-lookup"><span data-stu-id="6edbd-121">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page to reset your password, or ask your Global admin to assign you new credentials.</span></span>

### <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="6edbd-122">Na tela "Conte-nos sobre sua empresa", você recebe um erro "algo deu errado"</span><span class="sxs-lookup"><span data-stu-id="6edbd-122">On the “Tell us about your company” screen you receive a “Something went wrong” error</span></span>

<span data-ttu-id="6edbd-123">Isso geralmente acontece se você usar inadvertidamente caracteres especiais, espaços ou códigos de país no número de telefone da empresa.</span><span class="sxs-lookup"><span data-stu-id="6edbd-123">This usually happens if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="6edbd-124">O valor inserido no campo número de telefone pode conter apenas um máximo de 10 caracteres.</span><span class="sxs-lookup"><span data-stu-id="6edbd-124">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>

### <a name="you-are-trying-to-complete-the-purchase-via-credit-card-but-you-are-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="6edbd-125">Você está tentando concluir a compra por meio de cartão de crédito, mas está recebendo uma mensagem de erro informando que "seu pedido foi recusado.</span><span class="sxs-lookup"><span data-stu-id="6edbd-125">You are trying to complete the purchase via credit card, but you are receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="6edbd-126">Verifique suas informações "</span><span class="sxs-lookup"><span data-stu-id="6edbd-126">Please verify your information”</span></span>

<span data-ttu-id="6edbd-127">Você sempre deve inserir o endereço correspondente ao seu cartão de crédito e não correspondente à sua entidade legal.</span><span class="sxs-lookup"><span data-stu-id="6edbd-127">You should always insert the address corresponding to your credit card and not corresponding to your legal entity.</span></span> <span data-ttu-id="6edbd-128">Além disso, verifique se o CEP está correto e corresponde ao endereço que você usa.</span><span class="sxs-lookup"><span data-stu-id="6edbd-128">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

### <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="6edbd-129">Você deseja alternar de pagamento offline para método de pagamento online</span><span class="sxs-lookup"><span data-stu-id="6edbd-129">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="6edbd-130">Você precisará cancelar o pedido original e adquirir novamente-lo usando o método de pagamento preferencial.</span><span class="sxs-lookup"><span data-stu-id="6edbd-130">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="6edbd-131">Para cancelar um pedido:</span><span class="sxs-lookup"><span data-stu-id="6edbd-131">To cancel an order:</span></span>

1. <span data-ttu-id="6edbd-132">Selecione a guia **ofertas de associação** no painel.</span><span class="sxs-lookup"><span data-stu-id="6edbd-132">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="6edbd-133">Selecione **Cancelar pedido**</span><span class="sxs-lookup"><span data-stu-id="6edbd-133">Select **Cancel order**</span></span>

3. <span data-ttu-id="6edbd-134">Uma janela de confirmação será exibida e você deverá confirmar para cancelar a ordem inicial.</span><span class="sxs-lookup"><span data-stu-id="6edbd-134">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>
