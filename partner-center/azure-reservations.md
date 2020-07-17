---
title: Venda Microsoft Azure reservas de clientes
ms.topic: article
ms.date: 06/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Como um provedor de soluções de nuvem, você pode comprar, vender ou gerenciar reservas do Azure para clientes. Use o Partner Center, o portal do Azure ou a API do Partner Center.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4524d810a036953e45fb94a72241734e02a2798f
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2020
ms.locfileid: "86435725"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="62184-104">Venda Microsoft Azure reservas para clientes usando o Partner Center, o portal do Azure ou as APIs</span><span class="sxs-lookup"><span data-stu-id="62184-104">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="62184-105">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="62184-105">**Applies to**</span></span>

- <span data-ttu-id="62184-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="62184-106">Partner Center</span></span>
- <span data-ttu-id="62184-107">Portal do Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="62184-107">Microsoft Azure portal</span></span>
- <span data-ttu-id="62184-108">Parceiros no CSP</span><span class="sxs-lookup"><span data-stu-id="62184-108">Partners in CSP</span></span>

<span data-ttu-id="62184-109">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="62184-109">**Appropriate roles**</span></span>

- <span data-ttu-id="62184-110">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="62184-110">Admin agent</span></span>
- <span data-ttu-id="62184-111">Administrador global</span><span class="sxs-lookup"><span data-stu-id="62184-111">Global admin</span></span>
- <span data-ttu-id="62184-112">Agente de suporte técnico</span><span class="sxs-lookup"><span data-stu-id="62184-112">Helpdesk agent</span></span>
- <span data-ttu-id="62184-113">Agente de vendas</span><span class="sxs-lookup"><span data-stu-id="62184-113">Sales agent</span></span>
- <span data-ttu-id="62184-114">Administrador de gerenciamento de usuário</span><span class="sxs-lookup"><span data-stu-id="62184-114">User management admin</span></span>

<span data-ttu-id="62184-115">Os parceiros no CSP (programa de provedor de soluções na nuvem) podem oferecer aos seus clientes Microsoft Azure reservas.</span><span class="sxs-lookup"><span data-stu-id="62184-115">Partners in the Cloud Solution Provider program (CSP) can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="62184-116">Os clientes podem obter uma economia significativa quando reservam com antecedência.</span><span class="sxs-lookup"><span data-stu-id="62184-116">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="62184-117">As reservas do Azure oferecem aos clientes simplicidade e flexibilidade das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="62184-117">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="62184-118">Um ou três termos de reserva</span><span class="sxs-lookup"><span data-stu-id="62184-118">One or three-year reservation terms</span></span>
- <span data-ttu-id="62184-119">Introdução fácil; instalação concluída em segundos</span><span class="sxs-lookup"><span data-stu-id="62184-119">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="62184-120">Cancelar ou trocar instâncias reservadas a qualquer momento para reembolso ajustado</span><span class="sxs-lookup"><span data-stu-id="62184-120">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="62184-121">Gerenciar o uso de instâncias reservadas no nível do departamento organizacional ou individual</span><span class="sxs-lookup"><span data-stu-id="62184-121">Manage reserved instances usage at the organizational or individual department level</span></span> 

<span data-ttu-id="62184-122">As reservas do Azure podem atrair clientes das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="62184-122">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="62184-123">As reservas podem oferecer economias significativas em relação ao preço pago conforme o uso (PAYG)</span><span class="sxs-lookup"><span data-stu-id="62184-123">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="62184-124">Orçamento e previsão melhores com pagamento antecipado por termos de um ou três anos</span><span class="sxs-lookup"><span data-stu-id="62184-124">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="62184-125">Capacidade de computação priorizada na região do Azure mais próxima aos escritórios</span><span class="sxs-lookup"><span data-stu-id="62184-125">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="62184-126">As reservas do Azure fornecem a base para soluções de infraestrutura de ponta a ponta quando combinadas com software como o Microsoft Windows Server e o banco de dados SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="62184-126">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="62184-127">Você pode comprar, vender e gerenciar reservas do Azure no Partner Center e no portal do Azure e usando a API do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="62184-127">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="62184-128">Você também pode conceder a seus clientes permissão para comprar suas próprias reservas do Azure de uma assinatura do Azure que você comprou para elas.</span><span class="sxs-lookup"><span data-stu-id="62184-128">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="62184-129">Siga os links abaixo para saber como.</span><span class="sxs-lookup"><span data-stu-id="62184-129">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="62184-130">Recursos de reservas do Azure</span><span class="sxs-lookup"><span data-stu-id="62184-130">Azure reservations resources</span></span>

|<span data-ttu-id="62184-131">**Para obter informações sobre**</span><span class="sxs-lookup"><span data-stu-id="62184-131">**For information about**</span></span>   |<span data-ttu-id="62184-132">**Leia isto**</span><span class="sxs-lookup"><span data-stu-id="62184-132">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="62184-133">Documentação de reservas do Azure para seus clientes</span><span class="sxs-lookup"><span data-stu-id="62184-133">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="62184-134">O que são reservas do Azure?</span><span class="sxs-lookup"><span data-stu-id="62184-134">What are Azure reservations?</span></span>](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="62184-135">Comprando reservas do Azure para seus clientes no Partner Center</span><span class="sxs-lookup"><span data-stu-id="62184-135">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="62184-136">Comprar reservas do Azure</span><span class="sxs-lookup"><span data-stu-id="62184-136">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="62184-137">Gerenciando reservas do Azure no Partner Center</span><span class="sxs-lookup"><span data-stu-id="62184-137">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="62184-138">Gerenciando reservas do Azure no Partner Center</span><span class="sxs-lookup"><span data-stu-id="62184-138">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="62184-139">Determinando o tamanho correto da VM e verificando o uso da VM do cliente</span><span class="sxs-lookup"><span data-stu-id="62184-139">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="62184-140">Dimensionamento de VM para uso máximo de reserva do Azure</span><span class="sxs-lookup"><span data-stu-id="62184-140">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="62184-141">Como comprar reservas do Azure usando a API do Partner Center</span><span class="sxs-lookup"><span data-stu-id="62184-141">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="62184-142">[Comprar Instâncias de VM Reservadas do Azure](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) na documentação do desenvolvedor do Partner Center</span><span class="sxs-lookup"><span data-stu-id="62184-142">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="62184-143">Conceder aos clientes permissão para comprar suas próprias reservas do Azure de sua assinatura do CSP.</span><span class="sxs-lookup"><span data-stu-id="62184-143">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="62184-144">Dê permissão aos clientes para comprar suas próprias reservas do Azure</span><span class="sxs-lookup"><span data-stu-id="62184-144">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |
