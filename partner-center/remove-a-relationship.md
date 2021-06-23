---
title: Remover a relação de revendedor com um cliente
ms.topic: how-to
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Descubra como os parceiros diretos da Microsoft podem remover clientes de sua lista, remover privilégios de administrador delegados e parar de dar suporte ou comprar para um cliente.
author: dineshvu
ms.author: dineshvu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 83259f2f895be9ef34c55db5613ccfe6891a4424
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551462"
---
# <a name="how-to-remove-a-reseller-relationship-with-a-customer-in-partner-center"></a><span data-ttu-id="17bf8-103">Como remover uma relação de revendedor com um cliente no Partner Center</span><span class="sxs-lookup"><span data-stu-id="17bf8-103">How to remove a reseller relationship with a customer in Partner Center</span></span>

<span data-ttu-id="17bf8-104">**Funções apropriadas**: administrador global</span><span class="sxs-lookup"><span data-stu-id="17bf8-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="17bf8-105">Este artigo descreve como remover uma relação de revendedor com um cliente no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="17bf8-105">This article describes how to remove a reseller relationship with a customer in Partner Center.</span></span>

<span data-ttu-id="17bf8-106">Parceiros diretos ou provedores indiretos: se você não estiver mais fazendo transações com um cliente, poderá remover a relação em Partner Center.</span><span class="sxs-lookup"><span data-stu-id="17bf8-106">Direct partners or Indirect providers: if you're no longer transacting with a customer, you can remove the relationship in Partner Center.</span></span>

<span data-ttu-id="17bf8-107">A remoção de uma relação tem as seguintes consequências:</span><span class="sxs-lookup"><span data-stu-id="17bf8-107">Removing a relationship has the following consequences:</span></span>

- <span data-ttu-id="17bf8-108">Remove o cliente da sua lista de clientes no Partner Center</span><span class="sxs-lookup"><span data-stu-id="17bf8-108">Removes the customer from your list of customers in Partner Center</span></span>
- <span data-ttu-id="17bf8-109">Remove você da lista [de contatos de suporte disponíveis](assign-support-contacts.md) para seu cliente</span><span class="sxs-lookup"><span data-stu-id="17bf8-109">Removes you from the [list of available support contacts](assign-support-contacts.md) for your customer</span></span>
- <span data-ttu-id="17bf8-110">Remove seus privilégios de administrador de delegação para o cliente</span><span class="sxs-lookup"><span data-stu-id="17bf8-110">Removes your delegation admin privileges for the customer</span></span>
- <span data-ttu-id="17bf8-111">Impede que você faça compras futuras para o cliente</span><span class="sxs-lookup"><span data-stu-id="17bf8-111">Prevents you from making future purchases for the customer</span></span>

## <a name="how-to-remove-a-relationship"></a><span data-ttu-id="17bf8-112">Como remover uma relação</span><span class="sxs-lookup"><span data-stu-id="17bf8-112">How to remove a relationship</span></span>

<span data-ttu-id="17bf8-113">Para remover a relação, você precisará cancelar reservas de RI (instância reservada) do Azure, cancelar compras de software e suspender todas as assinaturas ativas restantes primeiro.</span><span class="sxs-lookup"><span data-stu-id="17bf8-113">To remove the relationship, you'll need to cancel Azure reserved instance (RI) reservations, cancel software purchases, and suspend any remaining active subscriptions first.</span></span>

1. <span data-ttu-id="17bf8-114">**Suspenda todas as assinaturas ativas.**</span><span class="sxs-lookup"><span data-stu-id="17bf8-114">**Suspend any active subscriptions.**</span></span>

   1. <span data-ttu-id="17bf8-115">No Partner Center, acesse **Clientes** e selecione um cliente</span><span class="sxs-lookup"><span data-stu-id="17bf8-115">From the Partner Center, go to **Customers** and select a customer</span></span>

   2. <span data-ttu-id="17bf8-116">Em **Assinaturas,** selecione uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="17bf8-116">Under **Subscriptions**, select a subscription.</span></span>

   3. <span data-ttu-id="17bf8-117">Selecione **Suspenso**</span><span class="sxs-lookup"><span data-stu-id="17bf8-117">Select **Suspended**</span></span>

   4. <span data-ttu-id="17bf8-118">Repita essas etapas para cada assinatura ativa.</span><span class="sxs-lookup"><span data-stu-id="17bf8-118">Repeat these steps for each active subscription.</span></span>

2. <span data-ttu-id="17bf8-119">**Remova a relação em Partner Center:**</span><span class="sxs-lookup"><span data-stu-id="17bf8-119">**Remove the relationship in Partner Center:**</span></span>

   <span data-ttu-id="17bf8-120">a.</span><span class="sxs-lookup"><span data-stu-id="17bf8-120">a.</span></span> <span data-ttu-id="17bf8-121">No Partner Center, acesse **Clientes** e selecione um cliente.</span><span class="sxs-lookup"><span data-stu-id="17bf8-121">From the Partner Center, go to **Customers** and select a customer.</span></span>

   <span data-ttu-id="17bf8-122">b.</span><span class="sxs-lookup"><span data-stu-id="17bf8-122">b.</span></span> <span data-ttu-id="17bf8-123">Selecione a **Conta**.</span><span class="sxs-lookup"><span data-stu-id="17bf8-123">Select the **Account**.</span></span>

   <span data-ttu-id="17bf8-124">c.</span><span class="sxs-lookup"><span data-stu-id="17bf8-124">c.</span></span> <span data-ttu-id="17bf8-125">Selecione **Remover relação de revendedor**.</span><span class="sxs-lookup"><span data-stu-id="17bf8-125">Select **Remove reseller relationship**.</span></span>

   > [!NOTE]
   > <span data-ttu-id="17bf8-126">Se alguma assinatura ainda estiver ativa, o link Remover **relação de** revendedor estará inativo.</span><span class="sxs-lookup"><span data-stu-id="17bf8-126">If any subscriptions are still active, the **Remove reseller relationship** link will be inactive.</span></span>

## <a name="next-steps"></a><span data-ttu-id="17bf8-127">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="17bf8-127">Next steps</span></span>

- [<span data-ttu-id="17bf8-128">Solicitar ou restabelecer uma relação com um cliente</span><span class="sxs-lookup"><span data-stu-id="17bf8-128">Request or re-establish a relationship with a customer</span></span>](request-a-relationship-with-a-customer.md)
