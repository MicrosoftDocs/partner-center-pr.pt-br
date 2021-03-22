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
ms.openlocfilehash: 7d80651c4e5e4afb476dada388f23c118e0bdf25
ms.sourcegitcommit: 35fe0fdc41886f6f5af71ec74e4a4ebd245dfe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2021
ms.locfileid: "104768696"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="50d22-104">Solucionar problemas de configuração de conta ou de renovação de MPN</span><span class="sxs-lookup"><span data-stu-id="50d22-104">Troubleshoot account setup or MPN renewal issues</span></span>


<span data-ttu-id="50d22-105">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="50d22-105">**Appropriate roles**</span></span>

- <span data-ttu-id="50d22-106">Administrador global</span><span class="sxs-lookup"><span data-stu-id="50d22-106">Global admin</span></span>
- <span data-ttu-id="50d22-107">Administrador de parceiros do MPN</span><span class="sxs-lookup"><span data-stu-id="50d22-107">MPN partner admin</span></span> 
 
<span data-ttu-id="50d22-108">Aqui estão algumas sugestões para solucionar problemas comuns que surgem ao configurar sua conta do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="50d22-108">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="50d22-109">O que acontece se você estiver migrando do centro de associação de parceiro e não for possível editar os campos de informações da empresa</span><span class="sxs-lookup"><span data-stu-id="50d22-109">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="50d22-110">Nos casos em que sua empresa já tem uma presença no Partner Center (por exemplo, uma conta CSP), você verá uma tela somente leitura.</span><span class="sxs-lookup"><span data-stu-id="50d22-110">In cases where your company already has a presence in Partner Center (for example, a CSP account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="50d22-111">Esta tela exibirá todas as informações sobre sua empresa, pois elas existem no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="50d22-111">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="50d22-112">Você não pode alterar os detalhes nesta tela.</span><span class="sxs-lookup"><span data-stu-id="50d22-112">You can't change the details on this screen.</span></span> <span data-ttu-id="50d22-113">Isso é por design e não é um erro.</span><span class="sxs-lookup"><span data-stu-id="50d22-113">This is by design and not an error.</span></span>

<span data-ttu-id="50d22-114">Selecione **aceitar** e **continuar** para continuar.</span><span class="sxs-lookup"><span data-stu-id="50d22-114">Select **Accept** and **Continue** to proceed.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="50d22-115">Se o departamento de TI tiver desativado a **inscrição no Partner Center**</span><span class="sxs-lookup"><span data-stu-id="50d22-115">If the IT department has turned off **Sign up for Partner Center**</span></span>

<span data-ttu-id="50d22-116">Você vê essa mensagem porque os usuários viral estão desabilitados ou porque a inscrição viral está desabilitada no locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="50d22-116">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="50d22-117">O administrador global da sua conta do Azure AD pode habilitar os recursos necessários executando o seguinte comando do PowerShell:</span><span class="sxs-lookup"><span data-stu-id="50d22-117">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="50d22-118">**Set-MsolCompanySettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="50d22-118">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="50d22-119">Para obter mais informações, leia [inscrição de autoatendimento](/azure/active-directory/users-groups-roles/directory-self-service-signup).</span><span class="sxs-lookup"><span data-stu-id="50d22-119">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup).</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="50d22-120">Você esqueceu sua senha</span><span class="sxs-lookup"><span data-stu-id="50d22-120">You forgot your password</span></span>

<span data-ttu-id="50d22-121">Se você esqueceu sua senha, selecione o link **não consegue acessar sua conta?** na página de entrada.</span><span class="sxs-lookup"><span data-stu-id="50d22-121">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page.</span></span> <span data-ttu-id="50d22-122">Essa opção permite que você Redefina sua senha ou peça ao administrador global para atribuir novas credenciais.</span><span class="sxs-lookup"><span data-stu-id="50d22-122">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="50d22-123">Na tela "Conte-nos sobre sua empresa", você recebe um erro "algo deu errado"</span><span class="sxs-lookup"><span data-stu-id="50d22-123">On the “Tell us about your company” screen, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="50d22-124">Essa mensagem de erro geralmente aparece se você usar inadvertidamente caracteres especiais, espaços ou código de país no número de telefone da empresa.</span><span class="sxs-lookup"><span data-stu-id="50d22-124">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="50d22-125">O valor inserido no campo número de telefone pode conter apenas um máximo de 10 caracteres.</span><span class="sxs-lookup"><span data-stu-id="50d22-125">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="50d22-126">Sua compra de cartão de crédito está recebendo uma mensagem de erro informando que "seu pedido foi recusado.</span><span class="sxs-lookup"><span data-stu-id="50d22-126">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="50d22-127">Verifique suas informações "</span><span class="sxs-lookup"><span data-stu-id="50d22-127">Please verify your information”</span></span>


<span data-ttu-id="50d22-128">Sempre use o endereço correspondente ao seu cartão de crédito em vez de sua entidade legal.</span><span class="sxs-lookup"><span data-stu-id="50d22-128">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="50d22-129">Além disso, verifique se o CEP está correto e corresponde ao endereço que você usa.</span><span class="sxs-lookup"><span data-stu-id="50d22-129">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="50d22-130">Você deseja alternar de pagamento offline para método de pagamento online</span><span class="sxs-lookup"><span data-stu-id="50d22-130">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="50d22-131">Você precisará cancelar o pedido original e adquirir novamente-lo usando o método de pagamento preferencial.</span><span class="sxs-lookup"><span data-stu-id="50d22-131">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="50d22-132">Para cancelar um pedido:</span><span class="sxs-lookup"><span data-stu-id="50d22-132">To cancel an order:</span></span>

1. <span data-ttu-id="50d22-133">Selecione a guia **ofertas de associação** no painel.</span><span class="sxs-lookup"><span data-stu-id="50d22-133">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="50d22-134">Selecione **Cancelar pedido**</span><span class="sxs-lookup"><span data-stu-id="50d22-134">Select **Cancel order**</span></span>

3. <span data-ttu-id="50d22-135">Uma janela de confirmação será exibida e você deverá confirmar para cancelar a ordem inicial.</span><span class="sxs-lookup"><span data-stu-id="50d22-135">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="50d22-136">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="50d22-136">Next steps</span></span>

- [<span data-ttu-id="50d22-137">Gerenciar sua conta do Partner Center</span><span class="sxs-lookup"><span data-stu-id="50d22-137">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="50d22-138">Como ler seu arquivo de fatura e reconhecimento</span><span class="sxs-lookup"><span data-stu-id="50d22-138">How to read your bill and recon file</span></span>](read-your-bill.md)
