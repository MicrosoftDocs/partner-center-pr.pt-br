---
title: Adicionar locatários à sua Partner Center de dados
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como adicionar, consolidar ou gerenciar vários locatários do Azure AD em sua conta do Partner Center e saiba por que você pode querer fazer isso.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: caea2002b5edc2958c0af316762408e309bcf14a
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151195"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="9494f-103">Adicionar e gerenciar vários locatários em sua Partner Center de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="9494f-103">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="9494f-104">**Funções apropriadas:** administrador global | Administrador da conta</span><span class="sxs-lookup"><span data-stu-id="9494f-104">**Appropriate roles**: Global admin | Account admin</span></span>

<span data-ttu-id="9494f-105">Este artigo discute como consolidar vários locatários Azure Active Directory (Azure AD) para sua empresa e, em seguida, adicioná-los e gerenciá-los em sua Partner Center conta.</span><span class="sxs-lookup"><span data-stu-id="9494f-105">This article discusses how to consolidate multiple Azure Active Directory (Azure AD) tenants for your company and then add and manage them in your Partner Center account.</span></span> <span data-ttu-id="9494f-106">Há muitos motivos para fazer isso.</span><span class="sxs-lookup"><span data-stu-id="9494f-106">There are many reasons to do so.</span></span> <span data-ttu-id="9494f-107">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="9494f-107">For example:</span></span>

- <span data-ttu-id="9494f-108">Digamos que sua empresa, Contoso, adquiriu outra empresa, Fabrikam.</span><span class="sxs-lookup"><span data-stu-id="9494f-108">Let's say your company, Contoso, has acquired another company, Fabrikam.</span></span> <span data-ttu-id="9494f-109">Você deseja que as duas empresas permaneçam separadas, mas deseja que os novos funcionários sejam capazes de usar Partner Center.</span><span class="sxs-lookup"><span data-stu-id="9494f-109">You want the two companies to remain separate, but you want the new employees to be able to use Partner Center.</span></span> <span data-ttu-id="9494f-110">Nesse caso, você associa o locatário do Azure AD da nova empresa à sua PGA (conta global de parceiro).</span><span class="sxs-lookup"><span data-stu-id="9494f-110">In this case, you associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="9494f-111">Essa associação permite que os usuários em ambas as empresas trabalhem em Partner Center.</span><span class="sxs-lookup"><span data-stu-id="9494f-111">This association enables users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="9494f-112">Se você executar sua empresa com mais de um locatário (por exemplo, *contoso.com*, *contoso.uk* e contoso.in ), poderá usar *a* multitenuidade para a groupá-los na mesma conta de PC.</span><span class="sxs-lookup"><span data-stu-id="9494f-112">If you run your business with more than one tenant (for example, *contoso.com*, *contoso.uk*, and *contoso.in*), you can use multitenancy to group them in the same PC account.</span></span>

- <span data-ttu-id="9494f-113">Se as diretrizes de fusões e aquisições exigirem que você trabalhe  com locatários de ambas as empresas, você usaria os locatários constoso.com e *fabrikam.com* locatários.</span><span class="sxs-lookup"><span data-stu-id="9494f-113">If mergers and acquisitions guidelines require you to work with tenants of both companies, you would use both the *constoso.com* and *fabrikam.com* tenants.</span></span>

- <span data-ttu-id="9494f-114">Os usuários de qualquer um dos locatários precisam ser capazes de:</span><span class="sxs-lookup"><span data-stu-id="9494f-114">Users of any of the tenants need to be able to:</span></span>
    * <span data-ttu-id="9494f-115">Acesso Partner Center para treinamento, downloads digitais ou associação MCP (Microsoft Certified Professional).</span><span class="sxs-lookup"><span data-stu-id="9494f-115">Access Partner Center for training, digital downloads, or Microsoft Certified Professional (MCP) association.</span></span>
    * <span data-ttu-id="9494f-116">Sejam atribuídas Partner Center funções como administrador Microsoft Partner Network (MPN) ou administrador de incentivos.</span><span class="sxs-lookup"><span data-stu-id="9494f-116">Be assigned Partner Center roles such as Microsoft Partner Network (MPN) admin or incentives admin.</span></span>

## <a name="add-an-azure-ad-tenant-to-your-account"></a><span data-ttu-id="9494f-117">Adicionar um locatário do Azure AD à sua conta</span><span class="sxs-lookup"><span data-stu-id="9494f-117">Add an Azure AD tenant to your account</span></span>

1. <span data-ttu-id="9494f-118">Entre como administrador global no [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="9494f-118">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="9494f-119">No canto superior direito, selecione **Configurações,** selecione **Configurações da conta** e, em seguida, **locatários.**</span><span class="sxs-lookup"><span data-stu-id="9494f-119">At the upper right, select **Settings**, select **Account settings**, and then select **Tenants**.</span></span>
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Captura de tela do botão Associar no painel Perfil do Azure AD."::: 

1. <span data-ttu-id="9494f-121">Selecione **Associar** e, em seguida, indique o locatário que você deseja associar.</span><span class="sxs-lookup"><span data-stu-id="9494f-121">Select **Associate**, and then indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="9494f-122">No prompt, entre como administrador global para o locatário que você deseja associar e, em seguida, selecione **confirmar**.</span><span class="sxs-lookup"><span data-stu-id="9494f-122">At the prompt, sign in as global admin to the tenant you want to associate, and then select **Confirm**.</span></span> 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Captura de tela do botão confirmar no painel confirmar nova associação do Azure AD."::: 

   <span data-ttu-id="9494f-124">Depois de confirmar a associação, será exibida uma mensagem de **todos os conjuntos** .</span><span class="sxs-lookup"><span data-stu-id="9494f-124">After you've confirmed the association, an **All set** message is displayed.</span></span> <span data-ttu-id="9494f-125">Para exibir o locatário recém-adicionado, selecione **retornar ao gerenciamento de locatário**.</span><span class="sxs-lookup"><span data-stu-id="9494f-125">To view the newly added tenant, select **Return to tenant management**.</span></span> 
 
>[!NOTE]
><span data-ttu-id="9494f-126">Você não poderá associar um locatário a uma conta se ela já estiver associada a outra conta do centro do parceiro.</span><span class="sxs-lookup"><span data-stu-id="9494f-126">You can't associate a tenant with an account if it's already associated with another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="9494f-127">Remover um locatário de sua conta</span><span class="sxs-lookup"><span data-stu-id="9494f-127">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="9494f-128">Entre como administrador global no [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="9494f-128">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="9494f-129">No canto superior direito, selecione o ícone **configurações** e, em seguida, selecione **configurações de conta**.</span><span class="sxs-lookup"><span data-stu-id="9494f-129">At the upper right, select the **Settings** icon, and then select **Account settings**.</span></span>

1. <span data-ttu-id="9494f-130">No painel esquerdo, selecione **locatários**.</span><span class="sxs-lookup"><span data-stu-id="9494f-130">On the left pane, select **Tenants**.</span></span> <span data-ttu-id="9494f-131">Em **gerenciar locatários do Azure ad**, selecione a guia **parceiro** .</span><span class="sxs-lookup"><span data-stu-id="9494f-131">Under **Manage Azure AD tenants**, select the **Partner** tab.</span></span>
 
1. <span data-ttu-id="9494f-132">Selecione **remover** ao lado do locatário cuja associação você deseja remover.</span><span class="sxs-lookup"><span data-stu-id="9494f-132">Select **Remove** next to the tenant whose association you want to remove.</span></span>

   :::image type="content" source="images/disassociate.png" alt-text="Captura de tela das associações de locatário atuais e seus links de remoção.":::

   <span data-ttu-id="9494f-134">Conforme mostrado na captura de tela anterior, os links de **remoção** são habilitados para todos os locatários associados, exceto para o locatário primário e o locatário ao qual você está conectado no momento.</span><span class="sxs-lookup"><span data-stu-id="9494f-134">As shown in the preceding screenshot, the **Remove** links are enabled for all associated tenants, except for the primary tenant and the tenant that you're currently signed in to.</span></span> 

   > [!NOTE]   
   > <span data-ttu-id="9494f-135">Quando você remove um locatário, os usuários nesse locatário não têm mais acesso à conta do Partner Center e a remoção pode ter um impacto sobre suas competências.</span><span class="sxs-lookup"><span data-stu-id="9494f-135">When you remove a tenant, the users on that tenant no longer have access to the Partner Center account, and the removal might have an impact on your competencies.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="9494f-136">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="9494f-136">Next steps</span></span>

- [<span data-ttu-id="9494f-137">Criar contas de usuário</span><span class="sxs-lookup"><span data-stu-id="9494f-137">Create user accounts</span></span>](create-user-accounts-and-set-permissions.md)






