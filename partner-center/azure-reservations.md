---
title: Venda Microsoft Azure reservas de clientes
description: Como um provedor de soluções de nuvem, você pode comprar, vender ou gerenciar reservas do Azure para clientes. Use o Partner Center, o portal do Azure ou a API do Partner Center.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: 317d1f0295b79b79bf06f1091ae365bc7012b749
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000230"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="1c71e-104">Venda Microsoft Azure reservas para clientes usando o Partner Center, o portal do Azure ou as APIs</span><span class="sxs-lookup"><span data-stu-id="1c71e-104">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="1c71e-105">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="1c71e-105">**Applies to**</span></span>

- <span data-ttu-id="1c71e-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="1c71e-106">Partner Center</span></span>
- <span data-ttu-id="1c71e-107">Portal do Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="1c71e-107">Microsoft Azure portal</span></span>
- <span data-ttu-id="1c71e-108">Parceiros no programa CSP</span><span class="sxs-lookup"><span data-stu-id="1c71e-108">Partners in the CSP program</span></span>

<span data-ttu-id="1c71e-109">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="1c71e-109">**Appropriate roles**</span></span>

- <span data-ttu-id="1c71e-110">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="1c71e-110">Admin agent</span></span>
- <span data-ttu-id="1c71e-111">Administrador global</span><span class="sxs-lookup"><span data-stu-id="1c71e-111">Global admin</span></span>
- <span data-ttu-id="1c71e-112">Agente de suporte técnico</span><span class="sxs-lookup"><span data-stu-id="1c71e-112">Helpdesk agent</span></span>
- <span data-ttu-id="1c71e-113">Agente de vendas</span><span class="sxs-lookup"><span data-stu-id="1c71e-113">Sales agent</span></span>
- <span data-ttu-id="1c71e-114">Administrador de gerenciamento de usuário</span><span class="sxs-lookup"><span data-stu-id="1c71e-114">User management admin</span></span>

> [!NOTE]
> <span data-ttu-id="1c71e-115">Este artigo se aplica somente a parceiros no programa CSP (provedor de soluções na nuvem).</span><span class="sxs-lookup"><span data-stu-id="1c71e-115">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="1c71e-116">Os clientes que usam outros tipos de assinaturas (como pagamento conforme o uso, individuais, contrato de cliente da Microsoft ou assinaturas de Enterprise Agreement) devem ler [essa documentação de reservas do Azure](/azure/cost-management-billing/reservations).</span><span class="sxs-lookup"><span data-stu-id="1c71e-116">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

<span data-ttu-id="1c71e-117">Os parceiros no programa CSP podem oferecer aos seus clientes Microsoft Azure reservas.</span><span class="sxs-lookup"><span data-stu-id="1c71e-117">Partners in the CSP program can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="1c71e-118">Os clientes podem obter uma economia significativa quando reservam com antecedência.</span><span class="sxs-lookup"><span data-stu-id="1c71e-118">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="1c71e-119">As reservas do Azure oferecem aos clientes simplicidade e flexibilidade das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="1c71e-119">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="1c71e-120">Um ou três termos de reserva</span><span class="sxs-lookup"><span data-stu-id="1c71e-120">One or three-year reservation terms</span></span>
- <span data-ttu-id="1c71e-121">Introdução fácil; instalação concluída em segundos</span><span class="sxs-lookup"><span data-stu-id="1c71e-121">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="1c71e-122">Cancelar ou trocar instâncias reservadas a qualquer momento para reembolso ajustado</span><span class="sxs-lookup"><span data-stu-id="1c71e-122">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="1c71e-123">Gerenciar o uso de instâncias reservadas no nível do departamento organizacional ou individual</span><span class="sxs-lookup"><span data-stu-id="1c71e-123">Manage reserved instances usage at the organizational or individual department level</span></span>

<span data-ttu-id="1c71e-124">As reservas do Azure podem atrair clientes das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="1c71e-124">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="1c71e-125">As reservas podem oferecer economias significativas em relação ao preço pago conforme o uso (PAYG)</span><span class="sxs-lookup"><span data-stu-id="1c71e-125">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="1c71e-126">Orçamento e previsão melhores com pagamento antecipado por termos de um ou três anos</span><span class="sxs-lookup"><span data-stu-id="1c71e-126">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="1c71e-127">Capacidade de computação priorizada na região do Azure mais próxima aos escritórios</span><span class="sxs-lookup"><span data-stu-id="1c71e-127">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="1c71e-128">As reservas do Azure fornecem a base para soluções de infraestrutura de ponta a ponta quando combinadas com software como o Microsoft Windows Server e o banco de dados SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="1c71e-128">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="1c71e-129">Você pode comprar, vender e gerenciar reservas do Azure no Partner Center e no portal do Azure e usando a API do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="1c71e-129">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="1c71e-130">Você também pode conceder a seus clientes permissão para comprar suas próprias reservas do Azure de uma assinatura do Azure que você comprou para elas.</span><span class="sxs-lookup"><span data-stu-id="1c71e-130">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="1c71e-131">Siga os links abaixo para saber como.</span><span class="sxs-lookup"><span data-stu-id="1c71e-131">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="1c71e-132">Recursos de reservas do Azure</span><span class="sxs-lookup"><span data-stu-id="1c71e-132">Azure reservations resources</span></span>

|<span data-ttu-id="1c71e-133">**Para obter informações sobre**</span><span class="sxs-lookup"><span data-stu-id="1c71e-133">**For information about**</span></span>   |<span data-ttu-id="1c71e-134">**Leia isto**</span><span class="sxs-lookup"><span data-stu-id="1c71e-134">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="1c71e-135">Documentação de reservas do Azure para seus clientes</span><span class="sxs-lookup"><span data-stu-id="1c71e-135">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="1c71e-136">O que são reservas do Azure?</span><span class="sxs-lookup"><span data-stu-id="1c71e-136">What are Azure reservations?</span></span>](/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="1c71e-137">Comprando reservas do Azure para seus clientes no Partner Center</span><span class="sxs-lookup"><span data-stu-id="1c71e-137">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="1c71e-138">Comprar reservas do Azure</span><span class="sxs-lookup"><span data-stu-id="1c71e-138">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="1c71e-139">Gerenciando reservas do Azure no Partner Center</span><span class="sxs-lookup"><span data-stu-id="1c71e-139">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="1c71e-140">Gerenciando reservas do Azure no Partner Center</span><span class="sxs-lookup"><span data-stu-id="1c71e-140">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="1c71e-141">Determinando o tamanho correto da VM e verificando o uso da VM do cliente</span><span class="sxs-lookup"><span data-stu-id="1c71e-141">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="1c71e-142">Dimensionamento de VM para uso máximo de reserva do Azure</span><span class="sxs-lookup"><span data-stu-id="1c71e-142">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="1c71e-143">Como comprar reservas do Azure usando a API do Partner Center</span><span class="sxs-lookup"><span data-stu-id="1c71e-143">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="1c71e-144">[Comprar Instâncias de VM Reservadas do Azure](/partner-center/develop/purchase-azure-reservations) na documentação do desenvolvedor do Partner Center</span><span class="sxs-lookup"><span data-stu-id="1c71e-144">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="1c71e-145">Conceder aos clientes permissão para comprar suas próprias reservas do Azure de sua assinatura do CSP.</span><span class="sxs-lookup"><span data-stu-id="1c71e-145">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="1c71e-146">Dê permissão aos clientes para comprar suas próprias reservas do Azure</span><span class="sxs-lookup"><span data-stu-id="1c71e-146">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |