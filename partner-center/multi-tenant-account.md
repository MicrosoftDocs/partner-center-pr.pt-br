---
title: Adicionar locatários adicionais à sua conta do Partner Center
ms.topic: article
ms.date: 07/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Gerenciar vários locatários por meio de sua conta do Partner Center
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ecdfcbd4801bee34be298030016d7366b12d7db3
ms.sourcegitcommit: 9bbad472a86086eec684f3b7f4568fdf152f625e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2020
ms.locfileid: "88846946"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="e5c77-103">Adicionar e gerenciar vários locatários em sua conta do Partner Center</span><span class="sxs-lookup"><span data-stu-id="e5c77-103">Add and manage multiple tenants in your Partner Center account</span></span>

<span data-ttu-id="e5c77-104">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="e5c77-104">**Applies to**</span></span>

- <span data-ttu-id="e5c77-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="e5c77-105">Partner Center</span></span>

<span data-ttu-id="e5c77-106">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="e5c77-106">**Appropriate roles**</span></span>

- <span data-ttu-id="e5c77-107">Administrador global</span><span class="sxs-lookup"><span data-stu-id="e5c77-107">Global admin</span></span>

<span data-ttu-id="e5c77-108">Esse recurso permite que você gerencie vários locatários para sua empresa e consolide-os em sua conta do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e5c77-108">This feature allows you to manage multiple tenants for your company and to consolidate them into your Partner Center account.</span></span> <span data-ttu-id="e5c77-109">Há muitas razões pelas quais você pode precisar gerenciar vários locatários do Azure AD em sua conta do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e5c77-109">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="e5c77-110">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="e5c77-110">For example:</span></span>

- <span data-ttu-id="e5c77-111">Sua empresa pode comprar outra empresa e você deseja que os funcionários da nova empresa possam usar o Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e5c77-111">Your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="e5c77-112">No entanto, você deseja que as duas empresas permaneçam separadas.</span><span class="sxs-lookup"><span data-stu-id="e5c77-112">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="e5c77-113">Nesse caso, você associaria o locatário do Azure AD da nova empresa à sua conta global do parceiro (PGA).</span><span class="sxs-lookup"><span data-stu-id="e5c77-113">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="e5c77-114">Essa associação permitiria que os usuários em ambas as empresas trabalhassem no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e5c77-114">This association would enable users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="e5c77-115">Se você tiver mais de um locatário para executar seu negócio (por exemplo, contoso.com, contoso.uk, contoso.in), poderá usar multilocação para associá-los à mesma conta do PC.</span><span class="sxs-lookup"><span data-stu-id="e5c77-115">If you have more than one tenant to run your business (e.g. contoso.com, contoso.uk, contoso.in) you can use multi-tenancy to tie them under the same PC account.</span></span>

- <span data-ttu-id="e5c77-116">Fusões e aquisições exigem que você trabalhe com mais de um locatário (por exemplo, se a contoso adquire a Fabrikam, você precisaria ser capaz de usar os respectivos locatários Constoso.com e Fabrikam.com).</span><span class="sxs-lookup"><span data-stu-id="e5c77-116">Mergers and acquisitions requires you to work with more than one tenant (e.g. If Contoso acquires Fabrikam, you would need to be able to use both Constoso.com and Fabrikam.com respective tenants).</span></span>

- <span data-ttu-id="e5c77-117">Os usuários de qualquer um dos locatários precisariam ser capazes de:</span><span class="sxs-lookup"><span data-stu-id="e5c77-117">Users from any of the tenants would need to be able to:</span></span>
    1.  <span data-ttu-id="e5c77-118">Central de parceiros de acesso para treinamento, downloads digitais, associação MCP</span><span class="sxs-lookup"><span data-stu-id="e5c77-118">Access Partner Center for training, digital downloads, MCP association</span></span>
    2.  <span data-ttu-id="e5c77-119">Receber funções do Partner Center como administrador do MPN, incentivos para o administrador, etc.</span><span class="sxs-lookup"><span data-stu-id="e5c77-119">Be assigned Partner Center roles like MPN Admin, Incentives Admin etc.</span></span>


## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="e5c77-120">Adicionar outro locatário do Azure AD à sua conta</span><span class="sxs-lookup"><span data-stu-id="e5c77-120">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="e5c77-121">Como administrador global, entre no [painel](https://partner.microsoft.com/dashboard)do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e5c77-121">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="e5c77-122">No ícone de **configurações** , selecione **configurações de conta** e, em seguida, selecione **locatários**.</span><span class="sxs-lookup"><span data-stu-id="e5c77-122">From the **Settings** icon, select **Account settings** and then select **Tenants**.</span></span>
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="associar locatários"::: 

3. <span data-ttu-id="e5c77-124">Selecione **associar outro locatário do AD** e indique o locatário que você deseja associar.</span><span class="sxs-lookup"><span data-stu-id="e5c77-124">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="e5c77-125">Como administrador global, entre no locatário que você deseja associar e confirme a associação.</span><span class="sxs-lookup"><span data-stu-id="e5c77-125">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="confirmar os locatários associados"::: 

5. <span data-ttu-id="e5c77-127">Depois de confirmar, você verá um aviso de **tudo definido** .</span><span class="sxs-lookup"><span data-stu-id="e5c77-127">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="e5c77-128">Selecione **retornar ao gerenciamento de locatário** e você verá o locatário recém-adicionado listado.</span><span class="sxs-lookup"><span data-stu-id="e5c77-128">Select **Return to tenant management** and you will see the newly added tenant listed.</span></span> 
 

>[!NOTE]
><span data-ttu-id="e5c77-129">Você não poderá associar um locatário a uma conta se ela já estiver associada a outra conta do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e5c77-129">You can't associate a tenant to an account if it is already associated to another Partner Center account.</span></span>

 
## <a name="next-steps"></a><span data-ttu-id="e5c77-130">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="e5c77-130">Next steps</span></span>

- [<span data-ttu-id="e5c77-131">Adicionar usuários</span><span class="sxs-lookup"><span data-stu-id="e5c77-131">Add users</span></span>](create-user-accounts-and-set-permissions.md)
