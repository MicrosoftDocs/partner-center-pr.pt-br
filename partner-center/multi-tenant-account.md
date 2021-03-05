---
title: Adicionar locatários à sua conta do Partner Center
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como adicionar, consolidar ou gerenciar vários locatários do Azure AD em sua conta do Partner Center e saber por que você talvez queira fazer isso.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2f3094489f65b7164b4a55804047f9a4ab5f11cb
ms.sourcegitcommit: 79d2f00c352db61252e523f45abf93fe2a2742a5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "102124798"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="98caf-103">Adicionar e gerenciar vários locatários em sua conta do Partner Center</span><span class="sxs-lookup"><span data-stu-id="98caf-103">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="98caf-104">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="98caf-104">**Appropriate roles**</span></span>

- <span data-ttu-id="98caf-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="98caf-105">Global admin</span></span>
- <span data-ttu-id="98caf-106">Administrador de conta</span><span class="sxs-lookup"><span data-stu-id="98caf-106">Account admin</span></span>

<span data-ttu-id="98caf-107">Este artigo discute como consolidar vários locatários do Azure Active Directory (Azure AD) para sua empresa e, em seguida, adicioná-los e gerenciá-los em sua conta do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="98caf-107">This article discusses how to consolidate multiple Azure Active Directory (Azure AD) tenants for your company and then add and manage them in your Partner Center account.</span></span> <span data-ttu-id="98caf-108">Há muitas razões para fazer isso.</span><span class="sxs-lookup"><span data-stu-id="98caf-108">There are many reasons to do so.</span></span> <span data-ttu-id="98caf-109">Por exemplo: </span><span class="sxs-lookup"><span data-stu-id="98caf-109">For example:</span></span>

- <span data-ttu-id="98caf-110">Digamos que sua empresa, contoso, tenha adquirido outra empresa, fabrikam.</span><span class="sxs-lookup"><span data-stu-id="98caf-110">Let's say your company, Contoso, has acquired another company, Fabrikam.</span></span> <span data-ttu-id="98caf-111">Você quer que as duas empresas permaneçam separadas, mas você deseja que os novos funcionários possam usar o Partner Center.</span><span class="sxs-lookup"><span data-stu-id="98caf-111">You want the two companies to remain separate, but you want the new employees to be able to use Partner Center.</span></span> <span data-ttu-id="98caf-112">Nesse caso, você associa o locatário do Azure AD da nova empresa à sua conta global do parceiro (PGA).</span><span class="sxs-lookup"><span data-stu-id="98caf-112">In this case, you associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="98caf-113">Essa associação permite que os usuários em ambas as empresas trabalhem no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="98caf-113">This association enables users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="98caf-114">Se você executar sua empresa com mais de um locatário (por exemplo, *contoso.com*, *contoso.uk* e *contoso.in*), poderá usar o multilocação para agrupá-los na mesma conta de PC.</span><span class="sxs-lookup"><span data-stu-id="98caf-114">If you run your business with more than one tenant (for example, *contoso.com*, *contoso.uk*, and *contoso.in*), you can use multitenancy to group them in the same PC account.</span></span>

- <span data-ttu-id="98caf-115">Se as diretrizes de fusões e aquisições exigirem que você trabalhe com locatários de ambas as empresas, você usaria os locatários *constoso.com* e *fabrikam.com* .</span><span class="sxs-lookup"><span data-stu-id="98caf-115">If mergers and acquisitions guidelines require you to work with tenants of both companies, you would use both the *constoso.com* and *fabrikam.com* tenants.</span></span>

- <span data-ttu-id="98caf-116">Os usuários de qualquer um dos locatários precisam ser capazes de:</span><span class="sxs-lookup"><span data-stu-id="98caf-116">Users of any of the tenants need to be able to:</span></span>
    * <span data-ttu-id="98caf-117">Acesse o Partner Center para treinamento, downloads digitais ou a Associação Microsoft Certified Professional (MCP).</span><span class="sxs-lookup"><span data-stu-id="98caf-117">Access Partner Center for training, digital downloads, or Microsoft Certified Professional (MCP) association.</span></span>
    * <span data-ttu-id="98caf-118">Ser atribuídas funções do Partner Center como administrador de Microsoft Partner Network (MPN) ou de incentivos.</span><span class="sxs-lookup"><span data-stu-id="98caf-118">Be assigned Partner Center roles such as Microsoft Partner Network (MPN) admin or incentives admin.</span></span>

## <a name="add-an-azure-ad-tenant-to-your-account"></a><span data-ttu-id="98caf-119">Adicionar um locatário do Azure AD à sua conta</span><span class="sxs-lookup"><span data-stu-id="98caf-119">Add an Azure AD tenant to your account</span></span>

1. <span data-ttu-id="98caf-120">Entre como administrador global no [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="98caf-120">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="98caf-121">No canto superior direito, selecione **configurações**, selecione **configurações de conta** e, em seguida, selecione **locatários**.</span><span class="sxs-lookup"><span data-stu-id="98caf-121">At the upper right, select **Settings**, select **Account settings**, and then select **Tenants**.</span></span>
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Captura de tela do botão associar no painel de perfil do Azure AD."::: 

1. <span data-ttu-id="98caf-123">Selecione **associar** e, em seguida, indique o locatário que você deseja associar.</span><span class="sxs-lookup"><span data-stu-id="98caf-123">Select **Associate**, and then indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="98caf-124">No prompt, entre como administrador global para o locatário que você deseja associar e, em seguida, selecione **confirmar**.</span><span class="sxs-lookup"><span data-stu-id="98caf-124">At the prompt, sign in as global admin to the tenant you want to associate, and then select **Confirm**.</span></span> 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Captura de tela do botão confirmar no painel confirmar nova associação do Azure AD."::: 

   <span data-ttu-id="98caf-126">Depois de confirmar a associação, será exibida uma mensagem de **todos os conjuntos** .</span><span class="sxs-lookup"><span data-stu-id="98caf-126">After you've confirmed the association, an **All set** message is displayed.</span></span> <span data-ttu-id="98caf-127">Para exibir o locatário recém-adicionado, selecione **retornar ao gerenciamento de locatário**.</span><span class="sxs-lookup"><span data-stu-id="98caf-127">To view the newly added tenant, select **Return to tenant management**.</span></span> 
 
>[!NOTE]
><span data-ttu-id="98caf-128">Você não poderá associar um locatário a uma conta se ela já estiver associada a outra conta do centro do parceiro.</span><span class="sxs-lookup"><span data-stu-id="98caf-128">You can't associate a tenant with an account if it's already associated with another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="98caf-129">Remover um locatário de sua conta</span><span class="sxs-lookup"><span data-stu-id="98caf-129">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="98caf-130">Entre como administrador global no [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="98caf-130">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="98caf-131">No canto superior direito, selecione o ícone **configurações** e, em seguida, selecione **configurações de conta**.</span><span class="sxs-lookup"><span data-stu-id="98caf-131">At the upper right, select the **Settings** icon, and then select **Account settings**.</span></span>

1. <span data-ttu-id="98caf-132">No painel esquerdo, selecione **locatários**.</span><span class="sxs-lookup"><span data-stu-id="98caf-132">On the left pane, select **Tenants**.</span></span> <span data-ttu-id="98caf-133">Em **gerenciar locatários do Azure ad**, selecione a guia **parceiro** .</span><span class="sxs-lookup"><span data-stu-id="98caf-133">Under **Manage Azure AD tenants**, select the **Partner** tab.</span></span>
 
1. <span data-ttu-id="98caf-134">Selecione **remover** ao lado do locatário cuja associação você deseja remover.</span><span class="sxs-lookup"><span data-stu-id="98caf-134">Select **Remove** next to the tenant whose association you want to remove.</span></span>

   :::image type="content" source="images/disassociate.png" alt-text="Captura de tela das associações de locatário atuais e seus links de remoção.":::

   <span data-ttu-id="98caf-136">Conforme mostrado na captura de tela anterior, os links de **remoção** são habilitados para todos os locatários associados, exceto para o locatário primário e o locatário ao qual você está conectado no momento.</span><span class="sxs-lookup"><span data-stu-id="98caf-136">As shown in the preceding screenshot, the **Remove** links are enabled for all associated tenants, except for the primary tenant and the tenant that you're currently signed in to.</span></span> 

   > [!NOTE]   
   > <span data-ttu-id="98caf-137">Quando você remove um locatário, os usuários nesse locatário não têm mais acesso à conta do Partner Center e a remoção pode ter um impacto sobre suas competências.</span><span class="sxs-lookup"><span data-stu-id="98caf-137">When you remove a tenant, the users on that tenant no longer have access to the Partner Center account, and the removal might have an impact on your competencies.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="98caf-138">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="98caf-138">Next steps</span></span>

- [<span data-ttu-id="98caf-139">Criar contas de usuário</span><span class="sxs-lookup"><span data-stu-id="98caf-139">Create user accounts</span></span>](create-user-accounts-and-set-permissions.md)






