---
title: Adicionar locatários adicionais à sua conta do Partner Center
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como adicionar, consolidar ou gerenciar vários locatários do Azure AD em sua conta do Partner Center. Saiba também sobre alguns dos motivos pelos quais você pode querer fazer isso.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 22f85bda0a651559da1717ae1e5365da40d62aff
ms.sourcegitcommit: 8cb98de420f6ab5bb4cb3efc9007262c4d7d3327
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2021
ms.locfileid: "98105538"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="51257-104">Adicionar e gerenciar vários locatários em sua conta do Partner Center</span><span class="sxs-lookup"><span data-stu-id="51257-104">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="51257-105">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="51257-105">**Appropriate roles**</span></span>

- <span data-ttu-id="51257-106">Administrador global</span><span class="sxs-lookup"><span data-stu-id="51257-106">Global admin</span></span>

<span data-ttu-id="51257-107">Esse recurso permite que você gerencie vários locatários para sua empresa e consolide-os em sua conta do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="51257-107">This feature allows you to manage multiple tenants for your company and to consolidate them into your Partner Center account.</span></span> <span data-ttu-id="51257-108">Há muitas razões pelas quais você pode precisar gerenciar vários locatários do Azure AD em sua conta do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="51257-108">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="51257-109">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="51257-109">For example:</span></span>

- <span data-ttu-id="51257-110">Sua empresa pode comprar outra empresa e você deseja que os funcionários da nova empresa possam usar o Partner Center.</span><span class="sxs-lookup"><span data-stu-id="51257-110">Your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="51257-111">No entanto, você deseja que as duas empresas permaneçam separadas.</span><span class="sxs-lookup"><span data-stu-id="51257-111">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="51257-112">Nesse caso, você associaria o locatário do Azure AD da nova empresa à sua conta global do parceiro (PGA).</span><span class="sxs-lookup"><span data-stu-id="51257-112">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="51257-113">Essa associação permitiria que os usuários em ambas as empresas trabalhassem no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="51257-113">This association would enable users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="51257-114">Se você tiver mais de um locatário para executar seu negócio (por exemplo, contoso.com, contoso.uk, contoso.in), poderá usar multilocação para associá-los à mesma conta do PC.</span><span class="sxs-lookup"><span data-stu-id="51257-114">If you have more than one tenant to run your business (e.g. contoso.com, contoso.uk, contoso.in) you can use multi-tenancy to tie them under the same PC account.</span></span>

- <span data-ttu-id="51257-115">Fusões e aquisições exigem que você trabalhe com mais de um locatário (por exemplo, se a contoso adquire a Fabrikam, você precisaria ser capaz de usar os respectivos locatários Constoso.com e Fabrikam.com).</span><span class="sxs-lookup"><span data-stu-id="51257-115">Mergers and acquisitions requires you to work with more than one tenant (e.g. If Contoso acquires Fabrikam, you would need to be able to use both Constoso.com and Fabrikam.com respective tenants).</span></span>

- <span data-ttu-id="51257-116">Os usuários de qualquer um dos locatários precisariam ser capazes de:</span><span class="sxs-lookup"><span data-stu-id="51257-116">Users from any of the tenants would need to be able to:</span></span>
    1.  <span data-ttu-id="51257-117">Central de parceiros de acesso para treinamento, downloads digitais, associação MCP</span><span class="sxs-lookup"><span data-stu-id="51257-117">Access Partner Center for training, digital downloads, MCP association</span></span>
    2.  <span data-ttu-id="51257-118">Receber funções do Partner Center como administrador do MPN, incentivos para o administrador, etc.</span><span class="sxs-lookup"><span data-stu-id="51257-118">Be assigned Partner Center roles like MPN Admin, Incentives Admin etc.</span></span>


## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="51257-119">Adicionar outro locatário do Azure AD à sua conta</span><span class="sxs-lookup"><span data-stu-id="51257-119">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="51257-120">Como administrador global, entre no [painel](https://partner.microsoft.com/dashboard)do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="51257-120">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="51257-121">No ícone de **configurações** , selecione **configurações de conta** e, em seguida, selecione **locatários**.</span><span class="sxs-lookup"><span data-stu-id="51257-121">From the **Settings** icon, select **Account settings** and then select **Tenants**.</span></span>
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="associar locatários"::: 

3. <span data-ttu-id="51257-123">Selecione **associar outro locatário do AD** e indique o locatário que você deseja associar.</span><span class="sxs-lookup"><span data-stu-id="51257-123">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="51257-124">Como administrador global, entre no locatário que você deseja associar e confirme a associação.</span><span class="sxs-lookup"><span data-stu-id="51257-124">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="confirmar os locatários associados"::: 

5. <span data-ttu-id="51257-126">Depois de confirmar, você verá um aviso de **tudo definido** .</span><span class="sxs-lookup"><span data-stu-id="51257-126">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="51257-127">Selecione **retornar ao gerenciamento de locatário** e você verá o locatário recém-adicionado listado.</span><span class="sxs-lookup"><span data-stu-id="51257-127">Select **Return to tenant management** and you'll see the newly added tenant listed.</span></span> 
 

>[!NOTE]
><span data-ttu-id="51257-128">Você não poderá associar um locatário a uma conta se ela já estiver associada a outra conta do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="51257-128">You can't associate a tenant to an account if it is already associated to another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="51257-129">Remover um locatário de sua conta</span><span class="sxs-lookup"><span data-stu-id="51257-129">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="51257-130">Como administrador global, entre no [painel](https://partner.microsoft.com/dashboard)do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="51257-130">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="51257-131">No ícone **configurações** , selecione **configurações da conta** -> locatários e clique na guia **parceiro** .</span><span class="sxs-lookup"><span data-stu-id="51257-131">From the **Settings** icon, select **Account settings** -> Tenants and click on the **Partner** tab.</span></span>
 
3. <span data-ttu-id="51257-132">Clique em **remover** para o locatário que você deseja dissociar.</span><span class="sxs-lookup"><span data-stu-id="51257-132">Click **Remove** for the tenant you want to dissociate.</span></span>

4. <span data-ttu-id="51257-133">Dissociar um locatário significa que os usuários nesse locatário não terão mais acesso à conta do Partner Center e isso poderá afetar suas competências.</span><span class="sxs-lookup"><span data-stu-id="51257-133">Dissociating a tenant means that the users on that tenant will no longer have access to the Partner Center account, and this could have an impact on your competencies.</span></span> 

<span data-ttu-id="51257-134">O botão **remover** está habilitado para todos os locatários associados, exceto o locatário primário e o locatário ao qual você está conectado no momento.</span><span class="sxs-lookup"><span data-stu-id="51257-134">The **Remove** button is enabled for all associated tenants, except the primary tenant and the tenant which you are currently signed into.</span></span>

:::image type="content" source="images/disassociate.png" alt-text="locatários com o botão remover":::
 

## <a name="next-steps"></a><span data-ttu-id="51257-136">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="51257-136">Next steps</span></span>

- [<span data-ttu-id="51257-137">Adicionar usuários</span><span class="sxs-lookup"><span data-stu-id="51257-137">Add users</span></span>](create-user-accounts-and-set-permissions.md)






