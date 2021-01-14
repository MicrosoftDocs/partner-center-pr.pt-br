---
title: 'Início rápido: gerenciar um Azure Marketplace privado usando o PowerShell'
description: Este guia de início rápido mostra como gerenciar ofertas em um Azure Marketplace privado usando o Azure PowerShell.
author: keferna
ms.author: keferna
ms.topic: quickstart
ms.prod: marketplace-customer
ms.devlang: azurepowershell
ms.date: 11/24/2020
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: d0021be17ab12b6e549b0e5263772a4a1e42f8a3
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182334"
---
# <a name="quickstart-manage-a-private-azure-marketplace-using-powershell"></a><span data-ttu-id="697ab-103">Início rápido: gerenciar um Azure Marketplace privado usando o PowerShell</span><span class="sxs-lookup"><span data-stu-id="697ab-103">Quickstart: Manage a Private Azure Marketplace using PowerShell</span></span>

<span data-ttu-id="697ab-104">Este artigo descreve como você pode gerenciar ofertas em um Azure Marketplace privado usando o módulo do PowerShell [AZ. Marketplace](/powershell/module/az.marketplace) .</span><span class="sxs-lookup"><span data-stu-id="697ab-104">This article describes how you can manage offers in a Private Azure Marketplace using the [Az.Marketplace](/powershell/module/az.marketplace) PowerShell module.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="697ab-105">O Azure Marketplace privado está atualmente em visualização pública.</span><span class="sxs-lookup"><span data-stu-id="697ab-105">Private Azure Marketplace is currently in public preview.</span></span> <span data-ttu-id="697ab-106">A versão prévia é fornecida sem um contrato de nível de serviço.</span><span class="sxs-lookup"><span data-stu-id="697ab-106">This preview version is provided without a service level agreement.</span></span> <span data-ttu-id="697ab-107">Ela não é recomendada para cargas de trabalho de produção.</span><span class="sxs-lookup"><span data-stu-id="697ab-107">It's not recommended for production workloads.</span></span> <span data-ttu-id="697ab-108">Alguns recursos podem não ter suporte ou podem ter recursos restritos.</span><span class="sxs-lookup"><span data-stu-id="697ab-108">Some features might not be supported or might have constrained capabilities.</span></span> <span data-ttu-id="697ab-109">Para obter mais informações, consulte [Termos de Uso Complementares de Versões Prévias do Microsoft Azure](https://azure.microsoft.com/support/legal/preview-supplemental-terms/).</span><span class="sxs-lookup"><span data-stu-id="697ab-109">For more information, see [Supplemental Terms of Use for Microsoft Azure Previews](https://azure.microsoft.com/support/legal/preview-supplemental-terms/).</span></span>

## <a name="requirements"></a><span data-ttu-id="697ab-110">Requisitos</span><span class="sxs-lookup"><span data-stu-id="697ab-110">Requirements</span></span>

* <span data-ttu-id="697ab-111">Se você não tiver uma assinatura do Azure, crie uma conta [gratuita](https://azure.microsoft.com/free/) antes de começar.</span><span class="sxs-lookup"><span data-stu-id="697ab-111">If you don't have an Azure subscription, create a [free](https://azure.microsoft.com/free/) account before you begin.</span></span>

* <span data-ttu-id="697ab-112">Se você optar por usar o Azure PowerShell localmente:</span><span class="sxs-lookup"><span data-stu-id="697ab-112">If you choose to use Azure PowerShell locally:</span></span>
  * <span data-ttu-id="697ab-113">[Instale o módulo Az PowerShell](/powershell/azure/install-az-ps).</span><span class="sxs-lookup"><span data-stu-id="697ab-113">[Install the Az PowerShell module](/powershell/azure/install-az-ps).</span></span>
  * <span data-ttu-id="697ab-114">Conecte-se à sua conta do Azure usando o cmdlet [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount).</span><span class="sxs-lookup"><span data-stu-id="697ab-114">Connect to your Azure account using the [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) cmdlet.</span></span>
* <span data-ttu-id="697ab-115">Se você optar por usar o Azure Cloud Shell:</span><span class="sxs-lookup"><span data-stu-id="697ab-115">If you choose to use Azure Cloud Shell:</span></span>
  * <span data-ttu-id="697ab-116">Confira [Visão geral do Azure Cloud Shell](/azure/cloud-shell/overview) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="697ab-116">See [Overview of Azure Cloud Shell](/azure/cloud-shell/overview) for more information.</span></span>

  > [!IMPORTANT]
  > <span data-ttu-id="697ab-117">Embora o módulo do PowerShell **AZ. Marketplace** esteja em versão prévia, você deve instalá-lo separadamente usando o `Install-Module` cmdlet.</span><span class="sxs-lookup"><span data-stu-id="697ab-117">While the **Az.Marketplace** PowerShell module is in preview, you must install it separately using the `Install-Module` cmdlet.</span></span> <span data-ttu-id="697ab-118">Depois que esse módulo do PowerShell estiver em disponibilidade geral, ele fará parte das versões futuras do módulo Az PowerShell e estará disponível por padrão no Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="697ab-118">After this PowerShell module becomes generally available, it will be part of future Az PowerShell module releases and available by default from within Azure Cloud Shell.</span></span>

  ```azurepowershell-interactive
  Install-Module -Name Az.Marketplace
  ```

* <span data-ttu-id="697ab-119">Se tiver várias assinaturas do Azure, escolha a que for adequada para cobrança do recurso.</span><span class="sxs-lookup"><span data-stu-id="697ab-119">If you have multiple Azure subscriptions, choose the appropriate subscription in which the resources should be billed.</span></span> <span data-ttu-id="697ab-120">Selecione uma assinatura específica usando o cmdlet [Set-AzContext](/powershell/module/az.accounts/set-azcontext).</span><span class="sxs-lookup"><span data-stu-id="697ab-120">Select a specific subscription using the [Set-AzContext](/powershell/module/az.accounts/set-azcontext) cmdlet.</span></span>

  ```azurepowershell-interactive
  Set-AzContext -SubscriptionId 00000000-0000-0000-0000-000000000000
  ```

## <a name="list-private-stores"></a><span data-ttu-id="697ab-121">Listar repositórios privados</span><span class="sxs-lookup"><span data-stu-id="697ab-121">List private stores</span></span>

<span data-ttu-id="697ab-122">Para recuperar uma lista de repositórios privados, use o cmdlet [Get-AzMarketplacePrivateStore](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) .</span><span class="sxs-lookup"><span data-stu-id="697ab-122">To retrieve a list of private stores, you use the [Get-AzMarketplacePrivateStore](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) cmdlet.</span></span> <span data-ttu-id="697ab-123">O exemplo a seguir lista os repositórios privados que foram criados no escopo do locatário.</span><span class="sxs-lookup"><span data-stu-id="697ab-123">The following example lists private stores that were created under the tenant scope.</span></span>

```azurepowershell-interactive
Get-AzMarketplacePrivateStore
```

```Output
Availability   : enabled
PrivateStoreId : 00000000-0000-0000-0000-000000000000
ETag           : "00000000-0000-0000-0000-000000000000"
Id             : /providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000
Name           : 00000000-0000-0000-0000-000000000000
Type           : Microsoft.Marketplace/privateStores
```

## <a name="add-an-offer-to-a-private-marketplace"></a><span data-ttu-id="697ab-124">Adicionar uma oferta a um Marketplace particular</span><span class="sxs-lookup"><span data-stu-id="697ab-124">Add an offer to a private marketplace</span></span>

<span data-ttu-id="697ab-125">Para adicionar uma oferta a um armazenamento privado, use o cmdlet [set-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) .</span><span class="sxs-lookup"><span data-stu-id="697ab-125">To add an offer to a private store, you use the [Set-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="697ab-126">O exemplo a seguir adiciona a oferta especificada a um Marketplace particular para um armazenamento privado que é criado no escopo do locatário.</span><span class="sxs-lookup"><span data-stu-id="697ab-126">The following example adds the specified offer to a private marketplace for a private store that is created under the tenant scope.</span></span>

```azurepowershell-interactive
$Params = @{
  privateStoreId = '00000000-0000-0000-0000-000000000000'
  offerId = 'publisherid.offerid'
  SpecificPlanIdsLimitation =@('PublisherEnterpriseLinux72',
                               'PublisherEnterpriseLinux72-ARM',
                               'PublisherEnterpriseLinux73',
                               'PublisherEnterpriseLinux73-ARM',
                               'PublisherEnterpriseLinux73-ARM-pr'
  )
}
Set-AzMarketplacePrivateStoreOffer @Params
```

```Output
UniqueOfferId             : publisherid.offerid
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {PublisherEnterpriseLinux72, PublisherEnterpriseLinux72-ARM,
PublisherEnterpriseLinux73, PublisherEnterpriseLinux73-ARM, PublisherEnterpriseLinux73-ARM-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid.offerid
Name                      : publisherid.offerid
Type                      : Microsoft.Marketplace/privateStores/offers
```

## <a name="get-private-store-offers"></a><span data-ttu-id="697ab-127">Obter ofertas de repositório privado</span><span class="sxs-lookup"><span data-stu-id="697ab-127">Get private store offers</span></span>

<span data-ttu-id="697ab-128">Para obter uma ou mais ofertas de armazenamento privado, use o cmdlet [Get-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) .</span><span class="sxs-lookup"><span data-stu-id="697ab-128">To get one or more private store offers, you use the [Get-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="697ab-129">O exemplo a seguir obtém ofertas associadas ao repositório particular especificado que foram adicionados sob o escopo do locatário.</span><span class="sxs-lookup"><span data-stu-id="697ab-129">The following example gets offers that are associated with the specified private store that were added under the tenant scope.</span></span>

```azurepowershell-interactive
Get-AzMarketplacePrivateStoreOffer -PrivateStoreId 00000000-0000-0000-0000-000000000000
```

```Output
UniqueOfferId             : publisherid.offerid
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {small, medium-with-upgraded-bandwidth, medium-with-upgraded-apps, large, large-pr,
small-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid.offerid
Name                      : publisherid.offerid
Type                      : Microsoft.Marketplace/privateStores/offers

UniqueOfferId             : publisherid1.offerid1
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {azure_managedservices_professional ,azure_managedservices_professional-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid1.offerid1
Name                      : publisherid1.offerid1
Type                      : Microsoft.Marketplace/privateStores/offers
```

## <a name="remove-an-offer"></a><span data-ttu-id="697ab-130">Remover uma oferta</span><span class="sxs-lookup"><span data-stu-id="697ab-130">Remove an offer</span></span>

<span data-ttu-id="697ab-131">Para remover uma oferta de um armazenamento privado, use o cmdlet [Remove-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) .</span><span class="sxs-lookup"><span data-stu-id="697ab-131">To remove an offer from a private store, you use the [Remove-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="697ab-132">O exemplo a seguir remove uma oferta de um armazenamento privado que foi criado no escopo do locatário.</span><span class="sxs-lookup"><span data-stu-id="697ab-132">The following example removes an offer from a private store that was created in the tenant scope.</span></span>

```azurepowershell-interactive
Remove-AzMarketplacePrivateStoreOffer -privateStoreId 00000000-0000-0000-0000-000000000000 -offerId publisherid.offerid
```

## <a name="next-steps"></a><span data-ttu-id="697ab-133">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="697ab-133">Next steps</span></span>

<span data-ttu-id="697ab-134">[Crie e gerencie o Azure Marketplace privado](create-manage-private-azure-marketplace.md).</span><span class="sxs-lookup"><span data-stu-id="697ab-134">[Create and manage Private Azure Marketplace](create-manage-private-azure-marketplace.md).</span></span>