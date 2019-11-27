---
title: Azure Cost Management by Cloudyn para parceiros CSP | Partner Center
ms.topic: article
ms.date: 11/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como registrar o aplicativo Web Cloudyn e usar uma chave secreta para ele no Partner Center para que você possa usar o aplicativo para acompanhar o uso do cliente e os custos do Azure.
author: Janet
ms.author: janet
Keywords: Aplicativo de gerenciamento de custos do Azure, gerenciar custos, aplicativos Web
robots: ''
ms.localizationpriority: medium
ms.openlocfilehash: b05f2085aad63f8a0e23fa44de97550d13053f86
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253302"
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a><span data-ttu-id="cc3d5-104">Aplicativo de gerenciamento de custos do Azure para parceiros CSP do Azure</span><span class="sxs-lookup"><span data-stu-id="cc3d5-104">Azure cost management app for Azure CSP partners</span></span>  

<span data-ttu-id="cc3d5-105">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="cc3d5-105">**Applies to**</span></span>

- <span data-ttu-id="cc3d5-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="cc3d5-106">Partner Center</span></span>
- <span data-ttu-id="cc3d5-107">Parceiros do programa Provedor de Soluções na Nuvem</span><span class="sxs-lookup"><span data-stu-id="cc3d5-107">Cloud Solution Provider program partners</span></span>

<span data-ttu-id="cc3d5-108">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="cc3d5-108">**Appropriate roles**</span></span>

- <span data-ttu-id="cc3d5-109">Administração global</span><span class="sxs-lookup"><span data-stu-id="cc3d5-109">Global admin</span></span>
- <span data-ttu-id="cc3d5-110">Agente administrador</span><span class="sxs-lookup"><span data-stu-id="cc3d5-110">Admin agent</span></span>

[<span data-ttu-id="cc3d5-111">Obter mais informações sobre o gerenciamento de custos do Azure</span><span class="sxs-lookup"><span data-stu-id="cc3d5-111">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="cc3d5-112">Antes de começar</span><span class="sxs-lookup"><span data-stu-id="cc3d5-112">Before you begin</span></span>
<span data-ttu-id="cc3d5-113">Antes de usar o Azure Cost Management, certifique-se de atender aos seguintes requisitos:</span><span class="sxs-lookup"><span data-stu-id="cc3d5-113">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="cc3d5-114">Você é um parceiro do programa Provedor de Soluções na Nuvem.</span><span class="sxs-lookup"><span data-stu-id="cc3d5-114">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="cc3d5-115">Você pode criar um aplicativo web com a API do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="cc3d5-115">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="cc3d5-116">Visão geral</span><span class="sxs-lookup"><span data-stu-id="cc3d5-116">Overview</span></span>

<span data-ttu-id="cc3d5-117">O Cloudyn é um aplicativo Web que permite que você acompanhe e gerencie quanto seus clientes estão usando o Azure e os custos desse uso.</span><span class="sxs-lookup"><span data-stu-id="cc3d5-117">Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="cc3d5-118">Você pode usá-lo por meio da API do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="cc3d5-118">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="cc3d5-119">Registre seu aplicativo Web no Partner Center</span><span class="sxs-lookup"><span data-stu-id="cc3d5-119">Register your web app in the Partner Center</span></span>
<span data-ttu-id="cc3d5-120">Ao registrar um aplicativo web do Azure Active Directory no Partner Center, você habilita o acesso à API do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="cc3d5-120">When you register an Azure Active Directory web app in Partner Center you enable access to the Partner Center API.</span></span> 
1.  <span data-ttu-id="cc3d5-121">Entre no [Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) usando uma [conta de administrador global ou de agente administrador](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="cc3d5-121">Sign into [the Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="cc3d5-122">No **Partner Center**, selecione **configurações de conta** &gt; **[Gerenciamento de aplicativos](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)** .</span><span class="sxs-lookup"><span data-stu-id="cc3d5-122">From the **Partner Center**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="cc3d5-123">Na seção **Aplicativo Web**, clique em **Adicionar novo aplicativo web**.</span><span class="sxs-lookup"><span data-stu-id="cc3d5-123">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="cc3d5-124">**Observação**: se você tiver criado anteriormente um aplicativo web, pode pular a etapa 3.</span><span class="sxs-lookup"><span data-stu-id="cc3d5-124">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="cc3d5-125">Copie e salve o GUID da **ID do Comércio** e o GUID da **ID do Aplicativo** para seu aplicativo web.</span><span class="sxs-lookup"><span data-stu-id="cc3d5-125">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="cc3d5-126">Você precisará das duas IDs para usar o versão de avaliação gratuita de 30 dias do aplicativo Azure Cost Management.</span><span class="sxs-lookup"><span data-stu-id="cc3d5-126">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="cc3d5-127">Adicione uma chave secreta ao seu aplicativo</span><span class="sxs-lookup"><span data-stu-id="cc3d5-127">Add a secret key to your app</span></span>
1. <span data-ttu-id="cc3d5-128">No menu suspenso ao lado do botão **Adicionar chave**, selecione uma duração de 1 ou 2 anos.</span><span class="sxs-lookup"><span data-stu-id="cc3d5-128">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="cc3d5-129">Clique em **Adicionar chave**.</span><span class="sxs-lookup"><span data-stu-id="cc3d5-129">Click **Add key**.</span></span> 
3. <span data-ttu-id="cc3d5-130">Copie e salve o valor da chave secreta.</span><span class="sxs-lookup"><span data-stu-id="cc3d5-130">Copy and save the secret key value.</span></span> <span data-ttu-id="cc3d5-131">Você precisará disso para a versão de avaliação gratuita de 30 dias.</span><span class="sxs-lookup"><span data-stu-id="cc3d5-131">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="cc3d5-132">As chaves secretas do aplicativo são como senhas com datas de expiração mais longas.</span><span class="sxs-lookup"><span data-stu-id="cc3d5-132">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="cc3d5-133">Salve o valor da chave em um local seguro para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="cc3d5-133">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="cc3d5-134">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="cc3d5-134">Next steps</span></span>
<span data-ttu-id="cc3d5-135">Inicie uma [avaliação gratuita de 30 dias](https://go.microsoft.com/fwlink/?linkid=857895).</span><span class="sxs-lookup"><span data-stu-id="cc3d5-135">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="cc3d5-136">Você precisa dos seguintes detalhes para iniciar a avaliação:</span><span class="sxs-lookup"><span data-stu-id="cc3d5-136">You need the following details to start the trial:</span></span>
- <span data-ttu-id="cc3d5-137">Credenciais para entrar no Partner Center</span><span class="sxs-lookup"><span data-stu-id="cc3d5-137">Partner Center sign in credentials</span></span>
- <span data-ttu-id="cc3d5-138">GUID da ID do Comércio</span><span class="sxs-lookup"><span data-stu-id="cc3d5-138">Commerce ID GUID</span></span>
- <span data-ttu-id="cc3d5-139">GUID da ID do Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cc3d5-139">App ID GUID</span></span>
- <span data-ttu-id="cc3d5-140">Valor da chave secreta do aplicativo</span><span class="sxs-lookup"><span data-stu-id="cc3d5-140">Application secret key value</span></span>
