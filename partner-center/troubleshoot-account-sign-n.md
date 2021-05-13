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
ms.openlocfilehash: a5e8a292ad8593dc0b94179d5f0ee418344ef9af
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854682"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="6f9fc-104">Solucionar problemas de configuração de conta ou de renovação de MPN</span><span class="sxs-lookup"><span data-stu-id="6f9fc-104">Troubleshoot account setup or MPN renewal issues</span></span>

<span data-ttu-id="6f9fc-105">**Funções apropriadas**: Administração Global | Administrador do parceiro do MPN</span><span class="sxs-lookup"><span data-stu-id="6f9fc-105">**Appropriate roles**: Global admin | MPN partner admin</span></span>
 
<span data-ttu-id="6f9fc-106">Aqui estão algumas sugestões para solucionar problemas comuns que surgem ao configurar sua conta do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="6f9fc-106">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="6f9fc-107">O que acontece se você estiver migrando do centro de associação de parceiro e não for possível editar os campos de informações da empresa</span><span class="sxs-lookup"><span data-stu-id="6f9fc-107">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="6f9fc-108">Nos casos em que sua empresa já tem uma presença no Partner Center (por exemplo, uma conta CSP), você verá uma tela somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6f9fc-108">In cases where your company already has a presence in Partner Center (for example, a CSP account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="6f9fc-109">Esta tela exibirá todas as informações sobre sua empresa, pois elas existem no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="6f9fc-109">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="6f9fc-110">Você não pode alterar os detalhes nesta tela.</span><span class="sxs-lookup"><span data-stu-id="6f9fc-110">You can't change the details on this screen.</span></span> <span data-ttu-id="6f9fc-111">Isso é por design e não é um erro.</span><span class="sxs-lookup"><span data-stu-id="6f9fc-111">This is by design and not an error.</span></span>

<span data-ttu-id="6f9fc-112">Selecione **aceitar** e **continuar** para continuar.</span><span class="sxs-lookup"><span data-stu-id="6f9fc-112">Select **Accept** and **Continue** to proceed.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="6f9fc-113">Se o departamento de TI tiver desativado a **inscrição no Partner Center**</span><span class="sxs-lookup"><span data-stu-id="6f9fc-113">If the IT department has turned off **Sign up for Partner Center**</span></span>

<span data-ttu-id="6f9fc-114">Você vê essa mensagem porque os usuários viral estão desabilitados ou porque a inscrição viral está desabilitada no locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6f9fc-114">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="6f9fc-115">O administrador global da sua conta do Azure AD pode habilitar os recursos necessários executando o seguinte comando do PowerShell:</span><span class="sxs-lookup"><span data-stu-id="6f9fc-115">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="6f9fc-116">**Set-MsolCompanySettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="6f9fc-116">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="6f9fc-117">Para obter mais informações, leia [inscrição de autoatendimento](/azure/active-directory/users-groups-roles/directory-self-service-signup).</span><span class="sxs-lookup"><span data-stu-id="6f9fc-117">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup).</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="6f9fc-118">Você esqueceu sua senha</span><span class="sxs-lookup"><span data-stu-id="6f9fc-118">You forgot your password</span></span>

<span data-ttu-id="6f9fc-119">Se você esqueceu sua senha, selecione o link **não consegue acessar sua conta?** na página de entrada.</span><span class="sxs-lookup"><span data-stu-id="6f9fc-119">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page.</span></span> <span data-ttu-id="6f9fc-120">Essa opção permite que você Redefina sua senha ou peça ao administrador global para atribuir novas credenciais.</span><span class="sxs-lookup"><span data-stu-id="6f9fc-120">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="6f9fc-121">Na tela "Conte-nos sobre sua empresa", você receberá um erro "Algo deu errado"</span><span class="sxs-lookup"><span data-stu-id="6f9fc-121">On the “Tell us about your company” screen, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="6f9fc-122">Essa mensagem de erro geralmente aparece se você usa inadvertidamente caracteres especiais, espaços ou código de país em seu número de telefone da empresa.</span><span class="sxs-lookup"><span data-stu-id="6f9fc-122">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="6f9fc-123">O valor inserido no campo Número de Telefone só pode conter um máximo de 10 caracteres.</span><span class="sxs-lookup"><span data-stu-id="6f9fc-123">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="6f9fc-124">Sua compra de cartão de crédito está recebendo uma mensagem de erro informando que "Seu pedido foi recusado.</span><span class="sxs-lookup"><span data-stu-id="6f9fc-124">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="6f9fc-125">Verifique suas informações"</span><span class="sxs-lookup"><span data-stu-id="6f9fc-125">Please verify your information”</span></span>


<span data-ttu-id="6f9fc-126">Sempre use o endereço correspondente ao seu cartão de crédito em vez de sua entidade jurídica.</span><span class="sxs-lookup"><span data-stu-id="6f9fc-126">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="6f9fc-127">Além disso, certifique-se de que o cep está correto e corresponda ao endereço usado.</span><span class="sxs-lookup"><span data-stu-id="6f9fc-127">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="6f9fc-128">Você deseja alternar do pagamento offline para a forma de pagamento online</span><span class="sxs-lookup"><span data-stu-id="6f9fc-128">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="6f9fc-129">Você precisará cancelar o pedido original e recomprar usando a forma de pagamento preferencial.</span><span class="sxs-lookup"><span data-stu-id="6f9fc-129">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="6f9fc-130">Para cancelar um pedido:</span><span class="sxs-lookup"><span data-stu-id="6f9fc-130">To cancel an order:</span></span>

1. <span data-ttu-id="6f9fc-131">Selecione **a guia Ofertas** de Associação no Painel.</span><span class="sxs-lookup"><span data-stu-id="6f9fc-131">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="6f9fc-132">Selecione **Cancelar pedido**</span><span class="sxs-lookup"><span data-stu-id="6f9fc-132">Select **Cancel order**</span></span>

3. <span data-ttu-id="6f9fc-133">Uma janela de confirmação será exibida e você deverá confirmar para cancelar a ordem inicial.</span><span class="sxs-lookup"><span data-stu-id="6f9fc-133">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="6f9fc-134">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="6f9fc-134">Next steps</span></span>

- [<span data-ttu-id="6f9fc-135">Gerenciar sua conta do Partner Center</span><span class="sxs-lookup"><span data-stu-id="6f9fc-135">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="6f9fc-136">Como ler seu arquivo de cobrança e reconhecimento</span><span class="sxs-lookup"><span data-stu-id="6f9fc-136">How to read your bill and recon file</span></span>](read-your-bill.md)
