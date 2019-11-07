---
title: Registrar-se no Partner Center como um fornecedor do painel de controle | Centro de parceiros
ms.topic: article
ms.date: 12/11/2018
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Como registrar-se no Partner Center como um fornecedor do painel de controle
author: LauraBrenner
ms.author: labrenne
keywords: Fornecedor do painel de controle, registrar aplicativos CPV, gerenciar aplicativos CPV
ms.localizationpriority: medium
ms.openlocfilehash: 7764764804fda5d0c7d83f4d0cc426ea3e27805c
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "73653223"
---
# <a name="enroll-in-partner-center-as-a-control-panel-vendor"></a><span data-ttu-id="83557-104">Registrar-se no Partner Center como um fornecedor do painel de controle</span><span class="sxs-lookup"><span data-stu-id="83557-104">Enroll in Partner Center as a Control Panel Vendor</span></span>

<span data-ttu-id="83557-105">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="83557-105">**Applies to**</span></span>

- <span data-ttu-id="83557-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="83557-106">Partner Center</span></span>

<span data-ttu-id="83557-107">Um fornecedor do painel de controle (CPV) é um fornecedor de software independente que desenvolve aplicativos para uso por parceiros do CSP (provedor de soluções na nuvem) para permitir que eles integrem seus sistemas com as APIs do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="83557-107">A Control Panel Vendor (CPV) is an independent software vendor that develops applications for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> <span data-ttu-id="83557-108">Um fornecedor do painel de controle não é um parceiro CSP com acesso direto ao painel do Partner Center ou às APIs do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="83557-108">A Control Panel vendor is not a CSP Partner with direct access to the Partner Center dashboard or Partner Center APIs.</span></span>

<span data-ttu-id="83557-109">Seja você um fornecedor atual do painel de controle (CPV) ou um novo CPV que queira trabalhar com parceiros da Microsoft, a Microsoft agora exige que você se registre no Partner Center para registrar seus aplicativos e dar suporte a parceiros do provedor de soluções na nuvem.</span><span class="sxs-lookup"><span data-stu-id="83557-109">Whether you are a current Control Panel Vendor (CPV) or a new CPV who wants to work with Microsoft partners, Microsoft now requires you to enroll in Partner Center in order to register your applications and support Cloud Solution Provider partners.</span></span> <span data-ttu-id="83557-110">Para criar uma conta, um parceiro CPV pode usar um locatário de parceiro CSP existente ou um locatário CPV existente ou pode criar um novo locatário como parte do processo de integração.</span><span class="sxs-lookup"><span data-stu-id="83557-110">To create an account, a CPV partner can either use an existing CSP partner tenant, or existing CPV tenant or can create a new tenant as part of onboarding process.</span></span> <span data-ttu-id="83557-111">Se o parceiro CPV optar por usar o locatário CSP existente, ele precisará criar aplicativos separados de vários locatários e registrá-los no Partner Center para atividades do CPV.</span><span class="sxs-lookup"><span data-stu-id="83557-111">If the CPV partner chooses to use the existing CSP tenant, then they'll need to create separate multi-tenant applications and register them in Partner Center for CPV activities.</span></span> <span data-ttu-id="83557-112">Um aplicativo não pode ser registrado como um CSP e um aplicativo CPV.</span><span class="sxs-lookup"><span data-stu-id="83557-112">An application can't be registered as both a CSP and CPV application.</span></span> <span data-ttu-id="83557-113">Depois de inscrever-se no Partner Center e registrar seus aplicativos, você terá acesso às APIs do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="83557-113">After you have enrolled in Partner Center and registered your applications, you will have access to the Partner Center APIs.</span></span>  <span data-ttu-id="83557-114">A Microsoft entrará em contato com você por meio de uma notificação do Partner Center com suas informações de área restrita.</span><span class="sxs-lookup"><span data-stu-id="83557-114">Microsoft will contact you via a Partner Center notification with your sandbox information.</span></span> <span data-ttu-id="83557-115">Se, no entanto, você já tiver uma conta de área restrita, continue a usá-la.</span><span class="sxs-lookup"><span data-stu-id="83557-115">If, however, you already have a sandbox account, continue using it.</span></span> <span data-ttu-id="83557-116">Você não precisará de uma nova área restrita.</span><span class="sxs-lookup"><span data-stu-id="83557-116">You won't need a new sandbox.</span></span>   

<span data-ttu-id="83557-117">Examinar o [contrato de fornecedor do painel de controle da Microsoft](https://go.microsoft.com/fwlink/?linkid=2055198)</span><span class="sxs-lookup"><span data-stu-id="83557-117">Review the [Microsoft Control Panel Vendor agreement](https://go.microsoft.com/fwlink/?linkid=2055198)</span></span>


## <a name="working-in-partner-center"></a><span data-ttu-id="83557-118">Trabalhando no Partner Center</span><span class="sxs-lookup"><span data-stu-id="83557-118">Working in Partner Center</span></span>
<span data-ttu-id="83557-119">Depois que você se inscreveu na experiência de CPV do Partner Center e aceitou o contrato CPV, você pode:</span><span class="sxs-lookup"><span data-stu-id="83557-119">Once you have enrolled in the Partner Center CPV experience and accepted the CPV agreement you can:</span></span>

- <span data-ttu-id="83557-120">Gerenciar aplicativos multilocatários (adicionar aplicativos para portal do Azure, registrar e cancelar o registro de aplicativos no Partner Center).</span><span class="sxs-lookup"><span data-stu-id="83557-120">Manage multi-tenant applications (add applications to Azure portal, register and unregister applications in Partner Center).</span></span>

>[!Note] 
><span data-ttu-id="83557-121">CPVs deve registrar seus aplicativos no Partner Center para ser autorizado para APIs do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="83557-121">CPVs must register their applications in Partner Center in order to get authorized for Partner Center APIs.</span></span> <span data-ttu-id="83557-122">Apenas adicionar aplicativos ao portal do Azure não autoriza os aplicativos de CPV a usarem as APIs do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="83557-122">Adding applications to the Azure portal alone does not authorize CPV applications for Partner Center APIs.</span></span> 

- <span data-ttu-id="83557-123">Exibir e gerenciar seu perfil de CPV</span><span class="sxs-lookup"><span data-stu-id="83557-123">View and manage your CPV profile</span></span> 

- <span data-ttu-id="83557-124">Exiba e gerencie seus usuários que precisam de acesso aos recursos de CPV.</span><span class="sxs-lookup"><span data-stu-id="83557-124">View and manage your users who need access to CPV capabilities.</span></span> <span data-ttu-id="83557-125">A única função que um CPV pode ter é administrador global.</span><span class="sxs-lookup"><span data-stu-id="83557-125">The only role a CPV can have is global admin.</span></span>


