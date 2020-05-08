---
title: Gerenciamento de custos do Azure da Cloudyn para CSPs
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como registrar o aplicativo Web Cloudyn e usar uma chave secreta para ele no Partner Center para que você possa usar o aplicativo para acompanhar o uso do cliente e os custos do Azure.
author: LauraBrenner
ms.author: labrenne
Keywords: Aplicativo de gerenciamento de custos do Azure, gerenciar custos, aplicativos Web
robots: ''
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0d88f37e0fe653c679df5729fa283336e4c7e144
ms.sourcegitcommit: e9b627159745bcce53a8c2b1676f63f5249bba76
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "82908372"
---
# <a name="track-customer-azure-usage-and-costs-with-the-azure-cost-management-app-for-csp-partners"></a><span data-ttu-id="9561e-104">Acompanhe o uso e os custos do Azure para clientes com o aplicativo de gerenciamento de custos do Azure para parceiros CSP</span><span class="sxs-lookup"><span data-stu-id="9561e-104">Track customer Azure usage and costs with the Azure cost management app for CSP partners</span></span>  

<span data-ttu-id="9561e-105">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="9561e-105">**Applies to**</span></span>

- <span data-ttu-id="9561e-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="9561e-106">Partner Center</span></span>
- <span data-ttu-id="9561e-107">Parceiros do programa Provedor de Soluções na Nuvem</span><span class="sxs-lookup"><span data-stu-id="9561e-107">Cloud Solution Provider program partners</span></span>

<span data-ttu-id="9561e-108">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="9561e-108">**Appropriate roles**</span></span>

- <span data-ttu-id="9561e-109">Administrador global</span><span class="sxs-lookup"><span data-stu-id="9561e-109">Global admin</span></span>
- <span data-ttu-id="9561e-110">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="9561e-110">Admin agent</span></span>

[<span data-ttu-id="9561e-111">Obtenha mais informações sobre o Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="9561e-111">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="9561e-112">Antes de começar</span><span class="sxs-lookup"><span data-stu-id="9561e-112">Before you begin</span></span>
<span data-ttu-id="9561e-113">Antes de usar o Azure Cost Management, certifique-se de atender aos seguintes requisitos:</span><span class="sxs-lookup"><span data-stu-id="9561e-113">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="9561e-114">Você é um parceiro do programa Provedor de Soluções na Nuvem.</span><span class="sxs-lookup"><span data-stu-id="9561e-114">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="9561e-115">Você pode criar um aplicativo web com a API do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="9561e-115">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="9561e-116">Visão geral</span><span class="sxs-lookup"><span data-stu-id="9561e-116">Overview</span></span>

<span data-ttu-id="9561e-117">O Cloudyn é um aplicativo Web que permite que você acompanhe e gerencie quanto seus clientes estão usando o Azure e os custos desse uso.</span><span class="sxs-lookup"><span data-stu-id="9561e-117">Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="9561e-118">Você pode usá-lo por meio da API do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="9561e-118">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="9561e-119">Registre seu aplicativo Web no Partner Center</span><span class="sxs-lookup"><span data-stu-id="9561e-119">Register your web app in the Partner Center</span></span>
<span data-ttu-id="9561e-120">Ao registrar um aplicativo web do Azure Active Directory no Partner Center, você habilita o acesso à API do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="9561e-120">When you register an Azure Active Directory web app in Partner Center you enable access to the Partner Center API.</span></span> 
1.  <span data-ttu-id="9561e-121">Entre no [Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) usando uma [conta de administrador global ou de agente administrador](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="9561e-121">Sign into [the Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="9561e-122">No **Partner Center**, selecione **configurações** &gt; de conta **[Gerenciamento de aplicativos](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.</span><span class="sxs-lookup"><span data-stu-id="9561e-122">From the **Partner Center**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="9561e-123">Na seção **Aplicativo Web**, clique em **Adicionar novo aplicativo web**.</span><span class="sxs-lookup"><span data-stu-id="9561e-123">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="9561e-124">**Observação**: se você tiver criado anteriormente um aplicativo web, pode pular a etapa 3.</span><span class="sxs-lookup"><span data-stu-id="9561e-124">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="9561e-125">Copie e salve o GUID da **ID do Comércio** e o GUID da **ID do Aplicativo** para seu aplicativo web.</span><span class="sxs-lookup"><span data-stu-id="9561e-125">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="9561e-126">Você precisará das duas IDs para usar o versão de avaliação gratuita de 30 dias do aplicativo Azure Cost Management.</span><span class="sxs-lookup"><span data-stu-id="9561e-126">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="9561e-127">Adicione uma chave secreta ao seu aplicativo</span><span class="sxs-lookup"><span data-stu-id="9561e-127">Add a secret key to your app</span></span>
1. <span data-ttu-id="9561e-128">No menu suspenso ao lado do botão **Adicionar chave**, selecione uma duração de 1 ou 2 anos.</span><span class="sxs-lookup"><span data-stu-id="9561e-128">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="9561e-129">Clique em **Adicionar chave**.</span><span class="sxs-lookup"><span data-stu-id="9561e-129">Click **Add key**.</span></span> 
3. <span data-ttu-id="9561e-130">Copie e salve o valor da chave secreta.</span><span class="sxs-lookup"><span data-stu-id="9561e-130">Copy and save the secret key value.</span></span> <span data-ttu-id="9561e-131">Você precisará disso para a versão de avaliação gratuita de 30 dias.</span><span class="sxs-lookup"><span data-stu-id="9561e-131">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="9561e-132">As chaves secretas do aplicativo são como senhas com datas de expiração mais longas.</span><span class="sxs-lookup"><span data-stu-id="9561e-132">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="9561e-133">Salve o valor da chave em um local seguro para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="9561e-133">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="9561e-134">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="9561e-134">Next steps</span></span>
<span data-ttu-id="9561e-135">Inicie uma [avaliação gratuita de 30 dias](https://go.microsoft.com/fwlink/?linkid=857895).</span><span class="sxs-lookup"><span data-stu-id="9561e-135">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="9561e-136">Você precisa dos seguintes detalhes para iniciar a avaliação:</span><span class="sxs-lookup"><span data-stu-id="9561e-136">You need the following details to start the trial:</span></span>
- <span data-ttu-id="9561e-137">Credenciais para entrar no Partner Center</span><span class="sxs-lookup"><span data-stu-id="9561e-137">Partner Center sign in credentials</span></span>
- <span data-ttu-id="9561e-138">GUID da ID do Comércio</span><span class="sxs-lookup"><span data-stu-id="9561e-138">Commerce ID GUID</span></span>
- <span data-ttu-id="9561e-139">GUID da ID do Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9561e-139">App ID GUID</span></span>
- <span data-ttu-id="9561e-140">Valor da chave secreta do aplicativo</span><span class="sxs-lookup"><span data-stu-id="9561e-140">Application secret key value</span></span>
