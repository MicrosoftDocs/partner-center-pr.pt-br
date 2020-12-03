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
ms.openlocfilehash: 9dc92685503fd4b9b05e40337f72e810c1693779
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534889"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="07ed9-104">Venda Microsoft Azure reservas para clientes usando o Partner Center, o portal do Azure ou as APIs</span><span class="sxs-lookup"><span data-stu-id="07ed9-104">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="07ed9-105">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="07ed9-105">**Appropriate roles**</span></span>

- <span data-ttu-id="07ed9-106">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="07ed9-106">Admin agent</span></span>
- <span data-ttu-id="07ed9-107">Administrador global</span><span class="sxs-lookup"><span data-stu-id="07ed9-107">Global admin</span></span>
- <span data-ttu-id="07ed9-108">Agente de suporte técnico</span><span class="sxs-lookup"><span data-stu-id="07ed9-108">Helpdesk agent</span></span>
- <span data-ttu-id="07ed9-109">Agente de vendas</span><span class="sxs-lookup"><span data-stu-id="07ed9-109">Sales agent</span></span>
- <span data-ttu-id="07ed9-110">Administrador de gerenciamento de usuário</span><span class="sxs-lookup"><span data-stu-id="07ed9-110">User management admin</span></span>

<span data-ttu-id="07ed9-111">Como um parceiro no CSP (programa de provedor de soluções na nuvem), você pode comprar, vender ou gerenciar reservas do Azure para clientes.</span><span class="sxs-lookup"><span data-stu-id="07ed9-111">As a partner in the Cloud Solution Provider program (CSP), you can buy, sell, or manage Azure reservations for customers.</span></span> <span data-ttu-id="07ed9-112">Use o Partner Center, o portal do Azure ou a API do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="07ed9-112">Use Partner Center, the Azure portal, or the Partner Center API.</span></span>

> [!NOTE]
> <span data-ttu-id="07ed9-113">Este artigo se aplica somente aos parceiros no CSP.</span><span class="sxs-lookup"><span data-stu-id="07ed9-113">This article applies only to partners in CSP.</span></span> <span data-ttu-id="07ed9-114">Os clientes que usam outros tipos de assinaturas (como pagamento conforme o uso, individuais, contrato de cliente da Microsoft ou assinaturas de Enterprise Agreement) devem ler [essa documentação de reservas do Azure](/azure/cost-management-billing/reservations).</span><span class="sxs-lookup"><span data-stu-id="07ed9-114">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

<span data-ttu-id="07ed9-115">Os parceiros no programa CSP podem oferecer aos seus clientes Microsoft Azure reservas.</span><span class="sxs-lookup"><span data-stu-id="07ed9-115">Partners in the CSP program can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="07ed9-116">Os clientes podem obter uma economia significativa quando reservam com antecedência.</span><span class="sxs-lookup"><span data-stu-id="07ed9-116">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="07ed9-117">As reservas do Azure oferecem aos clientes simplicidade e flexibilidade das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="07ed9-117">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="07ed9-118">Um ou três termos de reserva</span><span class="sxs-lookup"><span data-stu-id="07ed9-118">One or three-year reservation terms</span></span>
- <span data-ttu-id="07ed9-119">Introdução fácil; instalação concluída em segundos</span><span class="sxs-lookup"><span data-stu-id="07ed9-119">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="07ed9-120">Cancelar ou trocar instâncias reservadas a qualquer momento para reembolso ajustado</span><span class="sxs-lookup"><span data-stu-id="07ed9-120">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="07ed9-121">Gerenciar o uso de instâncias reservadas no nível do departamento organizacional ou individual</span><span class="sxs-lookup"><span data-stu-id="07ed9-121">Manage reserved instances usage at the organizational or individual department level</span></span>

<span data-ttu-id="07ed9-122">As reservas do Azure podem atrair clientes das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="07ed9-122">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="07ed9-123">As reservas podem oferecer economias significativas em relação ao preço pago conforme o uso (PAYG)</span><span class="sxs-lookup"><span data-stu-id="07ed9-123">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="07ed9-124">Orçamento e previsão melhores com pagamento antecipado por termos de um ou três anos</span><span class="sxs-lookup"><span data-stu-id="07ed9-124">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="07ed9-125">Capacidade de computação priorizada na região do Azure mais próxima aos escritórios</span><span class="sxs-lookup"><span data-stu-id="07ed9-125">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="07ed9-126">As reservas do Azure fornecem a base para soluções de infraestrutura de ponta a ponta quando combinadas com software como o Microsoft Windows Server e o banco de dados SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="07ed9-126">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="07ed9-127">Você pode comprar, vender e gerenciar reservas do Azure no Partner Center e no portal do Azure e usando a API do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="07ed9-127">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="07ed9-128">Você também pode conceder a seus clientes permissão para comprar suas próprias reservas do Azure de uma assinatura do Azure que você comprou para elas.</span><span class="sxs-lookup"><span data-stu-id="07ed9-128">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="07ed9-129">Siga os links abaixo para saber como.</span><span class="sxs-lookup"><span data-stu-id="07ed9-129">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="07ed9-130">Recursos de reservas do Azure</span><span class="sxs-lookup"><span data-stu-id="07ed9-130">Azure reservations resources</span></span>

|<span data-ttu-id="07ed9-131">**Para obter informações sobre**</span><span class="sxs-lookup"><span data-stu-id="07ed9-131">**For information about**</span></span>   |<span data-ttu-id="07ed9-132">**Leia isto**</span><span class="sxs-lookup"><span data-stu-id="07ed9-132">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="07ed9-133">Documentação de reservas do Azure para seus clientes</span><span class="sxs-lookup"><span data-stu-id="07ed9-133">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="07ed9-134">O que são reservas do Azure?</span><span class="sxs-lookup"><span data-stu-id="07ed9-134">What are Azure reservations?</span></span>](/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="07ed9-135">Comprando reservas do Azure para seus clientes no Partner Center</span><span class="sxs-lookup"><span data-stu-id="07ed9-135">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="07ed9-136">Comprar reservas do Azure</span><span class="sxs-lookup"><span data-stu-id="07ed9-136">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="07ed9-137">Gerenciando reservas do Azure no Partner Center</span><span class="sxs-lookup"><span data-stu-id="07ed9-137">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="07ed9-138">Gerenciando reservas do Azure no Partner Center</span><span class="sxs-lookup"><span data-stu-id="07ed9-138">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="07ed9-139">Determinando o tamanho correto da VM e verificando o uso da VM do cliente</span><span class="sxs-lookup"><span data-stu-id="07ed9-139">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="07ed9-140">Dimensionamento de VM para uso máximo de reserva do Azure</span><span class="sxs-lookup"><span data-stu-id="07ed9-140">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="07ed9-141">Como comprar reservas do Azure usando a API do Partner Center</span><span class="sxs-lookup"><span data-stu-id="07ed9-141">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="07ed9-142">[Comprar Instâncias de VM Reservadas do Azure](/partner-center/develop/purchase-azure-reservations) na documentação do desenvolvedor do Partner Center</span><span class="sxs-lookup"><span data-stu-id="07ed9-142">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="07ed9-143">Conceder aos clientes permissão para comprar suas próprias reservas do Azure de sua assinatura do CSP.</span><span class="sxs-lookup"><span data-stu-id="07ed9-143">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="07ed9-144">Dê permissão aos clientes para comprar suas próprias reservas do Azure</span><span class="sxs-lookup"><span data-stu-id="07ed9-144">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |