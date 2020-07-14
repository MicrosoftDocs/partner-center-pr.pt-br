---
title: Inscreva-se como um Fornecedor de Painel de Controle
ms.topic: article
ms.date: 05/20/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Saiba como registrar-se como um fornecedor do painel de controle (CPV) no Partner Center.
author: parthpandyaMSFT
ms.author: parthp
keywords: Fornecedor do painel de controle, registrar aplicativos CPV, gerenciar aplicativos CPV
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 503bbb6d1c083337dc9bad9cc469c43d614eb5a3
ms.sourcegitcommit: 0a6b1e6d845391539f54213efff00af4d23f028c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "86302363"
---
# <a name="enroll-as-a-control-panel-vendor-to-help-integrate-csp-partner-systems-with-partner-center-apis"></a><span data-ttu-id="740a5-104">Registre-se como um fornecedor do painel de controle para ajudar a integrar sistemas de parceiros CSP com APIs do Partner Center</span><span class="sxs-lookup"><span data-stu-id="740a5-104">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>

<span data-ttu-id="740a5-105">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="740a5-105">**Applies to**</span></span>

- <span data-ttu-id="740a5-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="740a5-106">Partner Center</span></span>

<span data-ttu-id="740a5-107">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="740a5-107">**Appropriate roles**</span></span>

- <span data-ttu-id="740a5-108">Administrador global</span><span class="sxs-lookup"><span data-stu-id="740a5-108">Global admin</span></span>

<span data-ttu-id="740a5-109">Um fornecedor do painel de controle (CPV) é um fornecedor de software independente que desenvolve aplicativos para uso por parceiros do CSP (provedor de soluções na nuvem) para permitir que eles integrem seus sistemas com as APIs do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="740a5-109">A Control Panel Vendor (CPV) is an independent software vendor that develops applications for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> <span data-ttu-id="740a5-110">Um fornecedor do painel de controle não é um parceiro CSP com acesso direto ao painel do Partner Center ou às APIs do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="740a5-110">A Control Panel vendor is not a CSP Partner with direct access to the Partner Center dashboard or Partner Center APIs.</span></span>

<span data-ttu-id="740a5-111">Seja você um fornecedor atual do painel de controle (CPV) ou um novo CPV que queira trabalhar com parceiros da Microsoft, a Microsoft agora exige que você se registre no Partner Center para registrar seus aplicativos e dar suporte a parceiros do provedor de soluções na nuvem.</span><span class="sxs-lookup"><span data-stu-id="740a5-111">Whether you are a current Control Panel Vendor (CPV) or a new CPV who wants to work with Microsoft partners, Microsoft now requires you to enroll in Partner Center in order to register your applications and support Cloud Solution Provider partners.</span></span> <span data-ttu-id="740a5-112">Para criar uma conta, um parceiro CPV pode usar um locatário de parceiro CSP existente ou um locatário CPV existente ou pode criar um novo locatário como parte do processo de integração.</span><span class="sxs-lookup"><span data-stu-id="740a5-112">To create an account, a CPV partner can either use an existing CSP partner tenant, or existing CPV tenant or can create a new tenant as part of onboarding process.</span></span> <span data-ttu-id="740a5-113">Se o parceiro CPV optar por usar o locatário CSP existente, ele precisará criar aplicativos separados de vários locatários e registrá-los no Partner Center para atividades do CPV.</span><span class="sxs-lookup"><span data-stu-id="740a5-113">If the CPV partner chooses to use the existing CSP tenant, then they'll need to create separate multi-tenant applications and register them in Partner Center for CPV activities.</span></span> <span data-ttu-id="740a5-114">Um aplicativo não pode ser registrado como um CSP e um aplicativo CPV.</span><span class="sxs-lookup"><span data-stu-id="740a5-114">An application can't be registered as both a CSP and CPV application.</span></span> <span data-ttu-id="740a5-115">Depois de inscrever-se no Partner Center e registrar seus aplicativos, você terá acesso às APIs do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="740a5-115">After you have enrolled in Partner Center and registered your applications, you will have access to the Partner Center APIs.</span></span>  <span data-ttu-id="740a5-116">A Microsoft entrará em contato com você por meio de uma notificação do Partner Center com suas informações de área restrita.</span><span class="sxs-lookup"><span data-stu-id="740a5-116">Microsoft will contact you via a Partner Center notification with your sandbox information.</span></span> <span data-ttu-id="740a5-117">Se você já tiver uma conta de área restrita, continue a usá-la.</span><span class="sxs-lookup"><span data-stu-id="740a5-117">If you already have a sandbox account, continue using it.</span></span> <span data-ttu-id="740a5-118">Você não precisará de uma nova área restrita.</span><span class="sxs-lookup"><span data-stu-id="740a5-118">You won't need a new sandbox.</span></span>

<span data-ttu-id="740a5-119">Examinar o [contrato de fornecedor do painel de controle da Microsoft](https://go.microsoft.com/fwlink/?linkid=2055198)</span><span class="sxs-lookup"><span data-stu-id="740a5-119">Review the [Microsoft Control Panel Vendor agreement](https://go.microsoft.com/fwlink/?linkid=2055198)</span></span>


## <a name="working-in-partner-center"></a><span data-ttu-id="740a5-120">Trabalhando no Partner Center</span><span class="sxs-lookup"><span data-stu-id="740a5-120">Working in Partner Center</span></span>
<span data-ttu-id="740a5-121">Depois que você se inscreveu na experiência de CPV do Partner Center e aceitou o contrato CPV, você pode:</span><span class="sxs-lookup"><span data-stu-id="740a5-121">Once you have enrolled in the Partner Center CPV experience and accepted the CPV agreement, you can:</span></span>

- <span data-ttu-id="740a5-122">Gerencie aplicativos multilocatários (adicione aplicativos para portal do Azure, registrar e cancelar o registro de aplicativos no Partner Center).</span><span class="sxs-lookup"><span data-stu-id="740a5-122">Manage multi-tenant applications (add applications to Azure portal, register, and unregister applications in Partner Center).</span></span>

>[!Note] 
><span data-ttu-id="740a5-123">CPVs deve registrar seus aplicativos no Partner Center para ser autorizado para APIs do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="740a5-123">CPVs must register their applications in Partner Center in order to get authorized for Partner Center APIs.</span></span> <span data-ttu-id="740a5-124">Apenas adicionar aplicativos ao portal do Azure não autoriza os aplicativos de CPV a usarem as APIs do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="740a5-124">Adding applications to the Azure portal alone does not authorize CPV applications for Partner Center APIs.</span></span> 

- <span data-ttu-id="740a5-125">Exibir e gerenciar seu perfil de CPV</span><span class="sxs-lookup"><span data-stu-id="740a5-125">View and manage your CPV profile</span></span> 

- <span data-ttu-id="740a5-126">Exiba e gerencie seus usuários que precisam de acesso aos recursos de CPV.</span><span class="sxs-lookup"><span data-stu-id="740a5-126">View and manage your users who need access to CPV capabilities.</span></span> <span data-ttu-id="740a5-127">O administrador global é a única função que um CPV pode ter.</span><span class="sxs-lookup"><span data-stu-id="740a5-127">Global admin is the only role a CPV can have.</span></span>


