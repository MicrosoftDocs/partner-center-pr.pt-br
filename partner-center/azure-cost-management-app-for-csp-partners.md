---
title: Azure Cost Management by Cloudyn para parceiros CSP | Partner Center
description: Azure Cost Management by Cloudyn requer acesso provisionado à API do Partner Center.
author: Janet
Keywords: Azure cost management app, manage costs, web apps
robots: ''
ms.openlocfilehash: 1b778dee20e449f778b9a67ea681a9ee9a430c8c
ms.sourcegitcommit: 034336ae3a697a97a62ad549b8645c836624efaa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2018
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a><span data-ttu-id="c5681-103">Aplicativo de gerenciamento de custos do Azure para parceiros CSP do Azure</span><span class="sxs-lookup"><span data-stu-id="c5681-103">Azure cost management app for Azure CSP partners</span></span>  

**<span data-ttu-id="c5681-104">Aplicável a</span><span class="sxs-lookup"><span data-stu-id="c5681-104">Applies to</span></span>**

-  <span data-ttu-id="c5681-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="c5681-105">Partner Center</span></span>

[<span data-ttu-id="c5681-106">Obtenha mais informações sobre o Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="c5681-106">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="c5681-107">Antes de começar</span><span class="sxs-lookup"><span data-stu-id="c5681-107">Before you begin</span></span>
<span data-ttu-id="c5681-108">Antes de usar o Azure Cost Management, certifique-se de atender aos seguintes requisitos:</span><span class="sxs-lookup"><span data-stu-id="c5681-108">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="c5681-109">Você é um parceiro do programa Provedor de Soluções na Nuvem.</span><span class="sxs-lookup"><span data-stu-id="c5681-109">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="c5681-110">Você pode criar um aplicativo web com a API do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="c5681-110">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="c5681-111">Visão geral</span><span class="sxs-lookup"><span data-stu-id="c5681-111">Overview</span></span>

<span data-ttu-id="c5681-112">Azure Cost Management by Cloudyn é um aplicativo web que permite controlar e gerenciar o quanto os clientes estão usando o Azure e os custos desse uso.</span><span class="sxs-lookup"><span data-stu-id="c5681-112">Azure cost management by Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="c5681-113">Você pode usá-lo por meio da API do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="c5681-113">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="c5681-114">Registre seu aplicativo Web no Partner Center</span><span class="sxs-lookup"><span data-stu-id="c5681-114">Register your web app in the Partner Center</span></span>
<span data-ttu-id="c5681-115">Ao registrar um aplicativo Web do Azure Active Directory no Partner Center, você habilita o acesso à API do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="c5681-115">When you register an Azure Active Directory web app in Partner Center you enable access to the the Partner Center API.</span></span> 
1.  <span data-ttu-id="c5681-116">Entre no [Partner Center](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview) usando uma [conta de administrador global ou de agente administrador](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="c5681-116">Sign into [the Partner Center](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="c5681-117">No menu **Painel**, selecione **Configurações da conta** &gt; **[Gerenciamento de aplicativos](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)**.</span><span class="sxs-lookup"><span data-stu-id="c5681-117">From the **Dashboard**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="c5681-118">Na seção **Aplicativo Web**, clique em **Adicionar novo aplicativo web**.</span><span class="sxs-lookup"><span data-stu-id="c5681-118">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="c5681-119">**Observação**: se você tiver criado anteriormente um aplicativo web, pode pular a etapa 3.</span><span class="sxs-lookup"><span data-stu-id="c5681-119">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="c5681-120">Copie e salve o GUID da **ID do Comércio** e o GUID da **ID do Aplicativo** para seu aplicativo web.</span><span class="sxs-lookup"><span data-stu-id="c5681-120">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="c5681-121">Você precisará das duas IDs para usar o versão de avaliação gratuita de 30 dias do aplicativo Azure Cost Management.</span><span class="sxs-lookup"><span data-stu-id="c5681-121">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="c5681-122">Adicione uma chave secreta ao seu aplicativo</span><span class="sxs-lookup"><span data-stu-id="c5681-122">Add a secret key to your app</span></span>
1.  <span data-ttu-id="c5681-123">No menu suspenso ao lado do botão **Adicionar chave**, selecione uma duração de 1 ou 2 anos.</span><span class="sxs-lookup"><span data-stu-id="c5681-123">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2.  <span data-ttu-id="c5681-124">Clique em **Adicionar chave**.</span><span class="sxs-lookup"><span data-stu-id="c5681-124">Click **Add key**.</span></span> 
3.  <span data-ttu-id="c5681-125">Copie e salve o valor da chave secreta.</span><span class="sxs-lookup"><span data-stu-id="c5681-125">Copy and save the secret key value.</span></span> <span data-ttu-id="c5681-126">Você precisará disso para a versão de avaliação gratuita de 30 dias.</span><span class="sxs-lookup"><span data-stu-id="c5681-126">You will need this for the 30-day free trial.</span></span>
<br><span data-ttu-id="c5681-127">**Observação**: as chaves secretas do aplicativo são como senhas com datas de vencimento mais longas.</span><span class="sxs-lookup"><span data-stu-id="c5681-127">**Note**: The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="c5681-128">Salve o valor da chave em um local seguro para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="c5681-128">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c5681-129">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="c5681-129">Next steps</span></span>
<span data-ttu-id="c5681-130">Inicie uma [avaliação gratuita de 30 dias](https://go.microsoft.com/fwlink/?linkid=857895).</span><span class="sxs-lookup"><span data-stu-id="c5681-130">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="c5681-131">Você precisa dos seguintes detalhes para iniciar a avaliação:</span><span class="sxs-lookup"><span data-stu-id="c5681-131">You need the following details to start the trial:</span></span>
- <span data-ttu-id="c5681-132">Credenciais para entrar no Partner Center</span><span class="sxs-lookup"><span data-stu-id="c5681-132">Partner Center sign in credentials</span></span>
- <span data-ttu-id="c5681-133">GUID da ID do Comércio</span><span class="sxs-lookup"><span data-stu-id="c5681-133">Commerce ID GUID</span></span>
- <span data-ttu-id="c5681-134">GUID da ID do Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c5681-134">App ID GUID</span></span>
- <span data-ttu-id="c5681-135">Valor da chave secreta do aplicativo</span><span class="sxs-lookup"><span data-stu-id="c5681-135">Application secret key value</span></span>
