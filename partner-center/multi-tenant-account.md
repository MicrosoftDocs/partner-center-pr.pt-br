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
ms.openlocfilehash: 6bf9399f23153f25f319e399c9c327515cd9ed51
ms.sourcegitcommit: 583c792d904cc1b15eda9217a1f21f434564c8e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2020
ms.locfileid: "87389501"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="c2e52-103">Adicionar e gerenciar vários locatários em sua conta do Partner Center</span><span class="sxs-lookup"><span data-stu-id="c2e52-103">Add and manage multiple tenants in your Partner Center account</span></span>

<span data-ttu-id="c2e52-104">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="c2e52-104">**Applies to**</span></span>

- <span data-ttu-id="c2e52-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="c2e52-105">Partner Center</span></span>

<span data-ttu-id="c2e52-106">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="c2e52-106">**Appropriate roles**</span></span>

- <span data-ttu-id="c2e52-107">Administrador global</span><span class="sxs-lookup"><span data-stu-id="c2e52-107">Global admin</span></span>

<span data-ttu-id="c2e52-108">Há muitas razões pelas quais você pode precisar gerenciar vários locatários do Azure AD em sua conta do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="c2e52-108">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="c2e52-109">Por exemplo, sua empresa pode comprar outra empresa e você deseja que os funcionários da nova empresa possam usar o Partner Center.</span><span class="sxs-lookup"><span data-stu-id="c2e52-109">For example, your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="c2e52-110">No entanto, você deseja que as duas empresas permaneçam separadas.</span><span class="sxs-lookup"><span data-stu-id="c2e52-110">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="c2e52-111">Nesse caso, você associaria o locatário do Azure AD da nova empresa à sua conta global do parceiro (PNG).</span><span class="sxs-lookup"><span data-stu-id="c2e52-111">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PNG).</span></span> <span data-ttu-id="c2e52-112">Essa associação permitiria que os usuários em ambas as empresas trabalhassem no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="c2e52-112">This association would enable users in both companies to work in Partner Center.</span></span>

## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="c2e52-113">Adicionar outro locatário do Azure AD à sua conta</span><span class="sxs-lookup"><span data-stu-id="c2e52-113">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="c2e52-114">Como administrador global, entre no [painel](https://partner.microsoft.com/dashboard)do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="c2e52-114">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="c2e52-115">No ícone de **configurações** , selecione **configurações de conta** e, em seguida, selecione **locatários**.</span><span class="sxs-lookup"><span data-stu-id="c2e52-115">From the **Settings** icon, select **Account settings** and then select **Tenants**.</span></span>
 
:::image type="content" source="images/merge-accounts/multitenant.png" alt-text="associar locatários"::: 

3. <span data-ttu-id="c2e52-117">Selecione **associar outro locatário do AD** e indique o locatário que você deseja associar.</span><span class="sxs-lookup"><span data-stu-id="c2e52-117">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="c2e52-118">Como administrador global, entre no locatário que você deseja associar e confirme a associação.</span><span class="sxs-lookup"><span data-stu-id="c2e52-118">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenant2.png" alt-text="confirmar os locatários associados"::: 

5. <span data-ttu-id="c2e52-120">Depois de confirmar, você verá um aviso de **tudo definido** .</span><span class="sxs-lookup"><span data-stu-id="c2e52-120">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="c2e52-121">Selecione **retornar ao gerenciamento de locatário** e você verá o locatário recém-adicionado listado.</span><span class="sxs-lookup"><span data-stu-id="c2e52-121">Select **Return to tenant management** and you will see the newly added tenant listed.</span></span>
 
## <a name="next-steps"></a><span data-ttu-id="c2e52-122">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="c2e52-122">Next steps</span></span>

- [<span data-ttu-id="c2e52-123">Adicionar usuários</span><span class="sxs-lookup"><span data-stu-id="c2e52-123">Add users</span></span>](create-user-accounts-and-set-permissions.md)
