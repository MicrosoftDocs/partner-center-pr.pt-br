---
title: Verificar a integridade do serviço para um cliente
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como usar o Partner Center para verificar a integridade do serviço de um cliente quando eles enfrentam um problema com um serviço.
ms.assetid: 05536BE7-A581-45D3-A390-2B9F139B5C6D
author: LauraBrenner
ms.author: labrenne
Keywords: integridade, integridade do serviço, problemas de serviço
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 54817a1288e4a4aebf75527907f0265e384ae839
ms.sourcegitcommit: 775a13540d6576201a900e517a0696a6ff4897d8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/05/2020
ms.locfileid: "84458372"
---
# <a name="check-service-health-for-a-customer-reporting-a-potential-service-problem-or-outage"></a><span data-ttu-id="fd56a-104">Verificar a integridade do serviço para um cliente relatando um potencial problema de serviço ou interrupção</span><span class="sxs-lookup"><span data-stu-id="fd56a-104">Check service health for a customer reporting a potential service problem or outage</span></span>

<span data-ttu-id="fd56a-105">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="fd56a-105">**Applies to**</span></span>

- <span data-ttu-id="fd56a-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="fd56a-106">Partner Center</span></span>

<span data-ttu-id="fd56a-107">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="fd56a-107">**Appropriate roles**</span></span>

- <span data-ttu-id="fd56a-108">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="fd56a-108">Admin agent</span></span>
- <span data-ttu-id="fd56a-109">Administrador global</span><span class="sxs-lookup"><span data-stu-id="fd56a-109">Global admin</span></span>
- <span data-ttu-id="fd56a-110">Agente de suporte técnico</span><span class="sxs-lookup"><span data-stu-id="fd56a-110">Helpdesk agent</span></span>
- <span data-ttu-id="fd56a-111">Agente de vendas</span><span class="sxs-lookup"><span data-stu-id="fd56a-111">Sales agent</span></span>

<span data-ttu-id="fd56a-112">Uma das primeiras coisas que você pode fazer quando um cliente estiver tendo problemas com um serviço é verificar a integridade do serviço.</span><span class="sxs-lookup"><span data-stu-id="fd56a-112">One of the first things you can do when a customer is experiencing problems with a service is to check the service health.</span></span> 

## <a name="check-service-health"></a><span data-ttu-id="fd56a-113">Verifique a integridade do serviço</span><span class="sxs-lookup"><span data-stu-id="fd56a-113">Check service health</span></span>

1. <span data-ttu-id="fd56a-114">Selecione o **cliente** que está tendo o problema na **lista de clientes**.</span><span class="sxs-lookup"><span data-stu-id="fd56a-114">Select the **Customer** that is having the issue from the **Customer list**.</span></span>

2. <span data-ttu-id="fd56a-115">Selecione **Gerenciamento de serviços** no menu à esquerda.</span><span class="sxs-lookup"><span data-stu-id="fd56a-115">Select **Service management** from the left menu.</span></span> <span data-ttu-id="fd56a-116">Isso listará os serviços provisionados para o cliente e a integridade do serviço para cada um.</span><span class="sxs-lookup"><span data-stu-id="fd56a-116">This will list the services provisioned for the customer and the service health for each.</span></span> <span data-ttu-id="fd56a-117">Os parceiros podem clicar no serviço em que estão interessados para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="fd56a-117">Partners can click the service they are interested in to get more information.</span></span> 

>[!NOTE] 
> <span data-ttu-id="fd56a-118">Os links de integridade do serviço nas páginas de **Gerenciamento de serviço** levarão o parceiro ao centro de administração do M365 ou ao portal do Azure como **administrador delegado**. Depois que o parceiro chega ao destino, o parceiro pode navegar até as páginas de integridade do serviço em qualquer portal para obter mais detalhes sobre a interrupção.</span><span class="sxs-lookup"><span data-stu-id="fd56a-118">Service health links on the **Service management** pages will take the partner to either the M365 admin center or the Azure portal as **delegated admin**. Once the partner gets to either destination, the partner can navigate to the service health pages in either portal for more details about the outage.</span></span>
 
<span data-ttu-id="fd56a-119">Durante uma interrupção de serviço, a Microsoft fornece atualizações regulares enquanto trabalhamos para resolver o problema.</span><span class="sxs-lookup"><span data-stu-id="fd56a-119">During a service outage, Microsoft provides regular updates as we work to address the problem.</span></span> <span data-ttu-id="fd56a-120">Essas notificações também são exibidas no portal do Microsoft Azure ou no centro de administração de Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="fd56a-120">These notifications are also displayed on either the Microsoft Azure portal or the Microsoft 365 admin Center.</span></span>

<span data-ttu-id="fd56a-121">Se o problema persistir após o término da interrupção do serviço, envie uma solicitação de serviço.</span><span class="sxs-lookup"><span data-stu-id="fd56a-121">If the problem persists after the end of the service outage, submit a service request.</span></span> <span data-ttu-id="fd56a-122">Consulte [Relatar problemas em nome de um cliente](report-problems-on-behalf-of-a-customer.md).</span><span class="sxs-lookup"><span data-stu-id="fd56a-122">See [Report problems on behalf of a customer](report-problems-on-behalf-of-a-customer.md).</span></span>

<span data-ttu-id="fd56a-123">Microsoft 365 e Microsoft Azure fornecem [APIs que os parceiros podem usar para recuperar a integridade do serviço em tempo real](get-automated-service-notifications-with-our-apis.md), as comunicações do centro de mensagens e os eventos de manutenção planejada.</span><span class="sxs-lookup"><span data-stu-id="fd56a-123">Microsoft 365 and Microsoft Azure each provide [APIs that partners can use to retrieve real-time service health](get-automated-service-notifications-with-our-apis.md), message center communications, and planned maintenance events.</span></span>

 

