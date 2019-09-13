---
title: Azure Cost Management by Cloudyn para parceiros CSP | Partner Center
ms.topic: article
ms.date: 03/15/2019
description: Azure Cost Management by Cloudyn requer acesso provisionado à API do Partner Center.
author: Janet
ms.author: janet
Keywords: Aplicativo de gerenciamento de custos do Azure, gerenciar custos, aplicativos Web
robots: ''
ms.localizationpriority: medium
ms.openlocfilehash: 27ff91d9d42f08e44f812663f3d4409e1080d580
ms.sourcegitcommit: bae29ab191c72e15259d99c40c69a9e7c3f2b502
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/06/2019
ms.locfileid: "68820305"
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a><span data-ttu-id="12df9-104">Aplicativo de gerenciamento de custos do Azure para parceiros CSP do Azure</span><span class="sxs-lookup"><span data-stu-id="12df9-104">Azure cost management app for Azure CSP partners</span></span>  

<span data-ttu-id="12df9-105">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="12df9-105">**Applies to**</span></span>

-  <span data-ttu-id="12df9-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="12df9-106">Partner Center</span></span>

[<span data-ttu-id="12df9-107">Obter mais informações sobre o gerenciamento de custos do Azure</span><span class="sxs-lookup"><span data-stu-id="12df9-107">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="12df9-108">Antes de começar</span><span class="sxs-lookup"><span data-stu-id="12df9-108">Before you begin</span></span>
<span data-ttu-id="12df9-109">Antes de usar o Azure Cost Management, certifique-se de atender aos seguintes requisitos:</span><span class="sxs-lookup"><span data-stu-id="12df9-109">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="12df9-110">Você é um parceiro do programa Provedor de Soluções na Nuvem.</span><span class="sxs-lookup"><span data-stu-id="12df9-110">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="12df9-111">Você pode criar um aplicativo web com a API do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="12df9-111">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="12df9-112">Visão geral</span><span class="sxs-lookup"><span data-stu-id="12df9-112">Overview</span></span>

<span data-ttu-id="12df9-113">O Cloudyn é um aplicativo Web que permite que você acompanhe e gerencie quanto seus clientes estão usando o Azure e os custos desse uso.</span><span class="sxs-lookup"><span data-stu-id="12df9-113">Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="12df9-114">Você pode usá-lo por meio da API do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="12df9-114">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="12df9-115">Registre seu aplicativo Web no Partner Center</span><span class="sxs-lookup"><span data-stu-id="12df9-115">Register your web app in the Partner Center</span></span>
<span data-ttu-id="12df9-116">Ao registrar um aplicativo Web do Azure Active Directory no Partner Center, você habilita o acesso à API do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="12df9-116">When you register an Azure Active Directory web app in Partner Center you enable access to the the Partner Center API.</span></span> 
1.  <span data-ttu-id="12df9-117">Entre no [Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) usando uma [conta de administrador global ou de agente administrador](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="12df9-117">Sign into [the Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="12df9-118">No **Partner Center**, selecione **configurações** &gt; de conta **[Gerenciamento de aplicativos](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)** .</span><span class="sxs-lookup"><span data-stu-id="12df9-118">From the **Partner Center**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="12df9-119">Na seção **Aplicativo Web**, clique em **Adicionar novo aplicativo web**.</span><span class="sxs-lookup"><span data-stu-id="12df9-119">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="12df9-120">**Observação**: Se você já tiver criado um aplicativo Web, poderá ignorar a etapa 3.</span><span class="sxs-lookup"><span data-stu-id="12df9-120">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="12df9-121">Copie e salve o GUID da **ID do Comércio** e o GUID da **ID do Aplicativo** para seu aplicativo web.</span><span class="sxs-lookup"><span data-stu-id="12df9-121">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="12df9-122">Você precisará das duas IDs para usar o versão de avaliação gratuita de 30 dias do aplicativo Azure Cost Management.</span><span class="sxs-lookup"><span data-stu-id="12df9-122">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="12df9-123">Adicione uma chave secreta ao seu aplicativo</span><span class="sxs-lookup"><span data-stu-id="12df9-123">Add a secret key to your app</span></span>
1. <span data-ttu-id="12df9-124">No menu suspenso ao lado do botão **Adicionar chave**, selecione uma duração de 1 ou 2 anos.</span><span class="sxs-lookup"><span data-stu-id="12df9-124">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="12df9-125">Clique em **Adicionar chave**.</span><span class="sxs-lookup"><span data-stu-id="12df9-125">Click **Add key**.</span></span> 
3. <span data-ttu-id="12df9-126">Copie e salve o valor da chave secreta.</span><span class="sxs-lookup"><span data-stu-id="12df9-126">Copy and save the secret key value.</span></span> <span data-ttu-id="12df9-127">Você precisará disso para a versão de avaliação gratuita de 30 dias.</span><span class="sxs-lookup"><span data-stu-id="12df9-127">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="12df9-128">As chaves secretas do aplicativo são como senhas com datas de expiração mais longas.</span><span class="sxs-lookup"><span data-stu-id="12df9-128">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="12df9-129">Salve o valor da chave em um local seguro para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="12df9-129">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="12df9-130">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="12df9-130">Next steps</span></span>
<span data-ttu-id="12df9-131">Inicie uma [avaliação gratuita de 30 dias](https://go.microsoft.com/fwlink/?linkid=857895).</span><span class="sxs-lookup"><span data-stu-id="12df9-131">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="12df9-132">Você precisa dos seguintes detalhes para iniciar a avaliação:</span><span class="sxs-lookup"><span data-stu-id="12df9-132">You need the following details to start the trial:</span></span>
- <span data-ttu-id="12df9-133">Credenciais para entrar no Partner Center</span><span class="sxs-lookup"><span data-stu-id="12df9-133">Partner Center sign in credentials</span></span>
- <span data-ttu-id="12df9-134">GUID da ID do Comércio</span><span class="sxs-lookup"><span data-stu-id="12df9-134">Commerce ID GUID</span></span>
- <span data-ttu-id="12df9-135">GUID da ID do Aplicativo</span><span class="sxs-lookup"><span data-stu-id="12df9-135">App ID GUID</span></span>
- <span data-ttu-id="12df9-136">Valor da chave secreta do aplicativo</span><span class="sxs-lookup"><span data-stu-id="12df9-136">Application secret key value</span></span>
