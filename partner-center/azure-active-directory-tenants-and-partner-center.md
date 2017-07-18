---
title: "Locatários do Azure Active Directory e o Partner Center | Partner Center"
description: "Para criar uma conta do Partner Center, sua empresa deve ter um locatário do Azure Active Directory (Azure AD). O Azure AD é o diretório baseado em nuvem e o serviço de gerenciamento de identidades da Microsoft."
author: labrenne
robots: 
ms.openlocfilehash: 9a9a3c3aa239017fe8ecf655f79acbfab6ff8a0b
ms.sourcegitcommit: d7c4ca62acd1ef1026c7d322e40f55a83a80e72a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/28/2017
---
# <a name="azure-active-directory-tenants-and-partner-center"></a><span data-ttu-id="e452a-104">Locatários do Azure Active Directory e o Partner Center</span><span class="sxs-lookup"><span data-stu-id="e452a-104">Azure Active Directory tenants and Partner Center</span></span>  

**<span data-ttu-id="e452a-105">Aplicável a</span><span class="sxs-lookup"><span data-stu-id="e452a-105">Applies to</span></span>**

-  <span data-ttu-id="e452a-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="e452a-106">Partner Center</span></span>

## <a name="why-you-need-an-azure-ad-tenant"></a><span data-ttu-id="e452a-107">Por que você precisa de um locatário do Azure AD</span><span class="sxs-lookup"><span data-stu-id="e452a-107">Why you need an Azure AD tenant</span></span>

<span data-ttu-id="e452a-108">Precisamos vincular o locatário do Azure AD de sua organização à sua nova conta do Partner Center para que os usuários do locatário possam se conectar ao Partner Center com seus nomes de usuário e senhas do Azure AD (conta da Microsoft).</span><span class="sxs-lookup"><span data-stu-id="e452a-108">We need to link your organization’s Azure AD tenant to your new Partner Center account, so your tenant users can sign in to Partner Center with their Azure AD (Microsoft account) user names and passwords.</span></span>

<span data-ttu-id="e452a-109">Se a sua empresa já tem um locatário do Azure AD, você pode vinculá-lo à sua conta do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e452a-109">If your company already has an Azure AD tenant, you can link it to your Partner Center account.</span></span> 

>**<span data-ttu-id="e452a-110">Observação</span><span class="sxs-lookup"><span data-stu-id="e452a-110">Note</span></span>**<br> <span data-ttu-id="e452a-111">Antes de decidir usar um locatário do Azure AD existente, pense sobre quantos usuários do locatário precisarão trabalhar no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e452a-111">Before you decide to use an existing Azure AD tenant, think about how many users in the tenant will need to work in Partner Center.</span></span> <span data-ttu-id="e452a-112">Se você tiver usuários no locatário que não precisam trabalhar no Partner Center, considere criar um novo locatário somente para os usuários que precisem trabalhar no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e452a-112">If you have users in the tenant who won’t need to work in Partner Center, consider creating a new tenant for only those users who will need to work in Partner Center.</span></span>

<span data-ttu-id="e452a-113">Se a sua empresa não tiver um locatário do Azure AD, você poderá criar um gratuitamente durante o processo de inscrição.</span><span class="sxs-lookup"><span data-stu-id="e452a-113">If your company doesn’t already have an Azure AD tenant, you can create one for free during the enrollment process.</span></span> <span data-ttu-id="e452a-114">Selecione **Criar um novo locatário** na página **Entrar no Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="e452a-114">Select **Create new tenant** on the **Sign in to Azure Active Directory** page.</span></span> 

### <a name="not-sure-if-your-company-already-has-an-azure-ad-tenant"></a><span data-ttu-id="e452a-115">Não tem certeza se a sua empresa já tem um locatário do Azure AD?</span><span class="sxs-lookup"><span data-stu-id="e452a-115">Not sure if your company already has an Azure AD tenant?</span></span>

<span data-ttu-id="e452a-116">Se você não tiver certeza se a empresa tem um locatário do Azure AD, siga estas etapas para verificar.</span><span class="sxs-lookup"><span data-stu-id="e452a-116">If you’re not sure whether your company has an Azure AD tenant, follow these steps to check.</span></span> <span data-ttu-id="e452a-117">Observe que se você tiver uma assinatura ativa do Microsoft Azure ou Office 365, você já tem um locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e452a-117">Note that If you have an active subscription to Microsoft Azure or Office 365, you already have an Azure AD tenant.</span></span>
1.  <span data-ttu-id="e452a-118">Entre no portal do administrador do Azure em https://ms.portal.azure.com</span><span class="sxs-lookup"><span data-stu-id="e452a-118">Sign in to the Azure admin portal at https://ms.portal.azure.com</span></span>
2.  <span data-ttu-id="e452a-119">Selecione Azure Active Directory no menu e, em seguida, selecione Nomes de Domínio.</span><span class="sxs-lookup"><span data-stu-id="e452a-119">Select Azure Active Directory from the menu and then select Domain Names.</span></span>
3.  <span data-ttu-id="e452a-120">Se você já tiver um locatário, seu nome de domínio estará listado.</span><span class="sxs-lookup"><span data-stu-id="e452a-120">If you already have a tenant, your domain name will be listed.</span></span>

### <a name="using-an-existing-tenant"></a><span data-ttu-id="e452a-121">Usando um locatário existente?</span><span class="sxs-lookup"><span data-stu-id="e452a-121">Using an existing tenant?</span></span>

<span data-ttu-id="e452a-122">Se quiser usar um locatário do Azure AD existente, mas estiver tendo problemas para se conectar, encontre o cenário no diagrama a seguir que melhor corresponda à sua situação e siga as etapas recomendadas.</span><span class="sxs-lookup"><span data-stu-id="e452a-122">If you want to use an existing Azure AD tenant but you’re having trouble signing in, find the scenario on the diagram below that best matches your situation and follow the recommended steps.</span></span> 

![Você tem um locatário do Azure AD ou precisa criar um?](images/onboardingAADFlow.png)

<span data-ttu-id="e452a-124">Para saber mais sobre como adicionar domínios no Azure AD, consulte [Adicionar ou associar um domínio no Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-add-domain)</span><span class="sxs-lookup"><span data-stu-id="e452a-124">For more information about adding domains in Azure AD, see [Add or associate a domain in Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-add-domain)</span></span>

## <a name="about-microsoft-azure"></a><span data-ttu-id="e452a-125">Sobre o Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="e452a-125">About Microsoft Azure</span></span>

<span data-ttu-id="e452a-126">O Microsoft Azure é uma plataforma de nuvem pública que as empresas podem usar para compilar, implantar e gerenciar aplicativos em uma rede global de datacenters gerenciados pela Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e452a-126">Microsoft Azure is a public cloud platform that companies can use to build, deploy, and manage applications across a global network of Microsoft-managed datacenters.</span></span> <span data-ttu-id="e452a-127">As empresas usam o Azure para criar uma infraestrutura de TI virtual com funções virtuais ou serviços, em vez de computadores físicos.</span><span class="sxs-lookup"><span data-stu-id="e452a-127">Companies use Azure to build a virtual IT infrastructure with virtual functions, or services, instead of physical machines.</span></span> 

<span data-ttu-id="e452a-128">Ao comprar uma assinatura do Azure, você está essencialmente alugando um espaço dedicado e seguro na nuvem pública do Azure, não muito diferente de alugar um andar de um prédio para abrigar sua empresa física.</span><span class="sxs-lookup"><span data-stu-id="e452a-128">When you purchase an Azure subscription, you’re essentially renting a dedicated, secure space in the Azure public cloud, not too different from renting a floor in an office building to house your company’s physical business.</span></span> <span data-ttu-id="e452a-129">Para o proprietário do prédio, sua empresa é um locatário.</span><span class="sxs-lookup"><span data-stu-id="e452a-129">To the office building’s owner, your company is a tenant.</span></span> 

<span data-ttu-id="e452a-130">Um locatário do Azure AD é uma representação virtual dedicada e isolada de sua empresa na nuvem pública do Azure, criada para você quando assina um serviço em nuvem da Microsoft, como o Azure, o Microsoft Intune ou o Office 365.</span><span class="sxs-lookup"><span data-stu-id="e452a-130">An Azure AD tenant is a dedicated and isolated virtual representation of your company in the Azure public cloud, created for you when you subscribe to a Microsoft cloud service such as Azure, Microsoft Intune, or Office 365.</span></span> 

<span data-ttu-id="e452a-131">Seu locatário hospeda os usuários do Azure AD e as informações sobre eles: suas senhas, dados de perfil, permissões e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="e452a-131">Your tenant hosts your Azure AD users and the information about them - their passwords, profile data, permissions, and so on.</span></span> <span data-ttu-id="e452a-132">O locatário também contém grupos, aplicativos e outras informações relacionadas a uma empresa e sua segurança.</span><span class="sxs-lookup"><span data-stu-id="e452a-132">The tenant also contains groups,applications, and other information pertaining to a company and its security.</span></span> 

<span data-ttu-id="e452a-133">Para saber mais sobre o Azure AD, consulte a [Documentação do Azure Active Directory](https://docs.microsoft.com/ azure/active-directory/).</span><span class="sxs-lookup"><span data-stu-id="e452a-133">To learn more about Azure AD, see the [Azure Active Directory Documentation](https://docs.microsoft.com/ azure/active-directory/).</span></span> 