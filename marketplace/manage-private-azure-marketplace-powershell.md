---
title: 'Rychlý Start: Správa privátních Azure Marketplace pomocí prostředí PowerShell'
description: V tomto rychlém startu se dozvíte, jak spravovat nabídky v privátních Azure Marketplace pomocí Azure PowerShell.
author: keferna
ms.author: keferna
ms.topic: quickstart
ms.service: marketplace-customer
ms.devlang: azurepowershell
ms.date: 11/24/2020
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: d7bd790eab2618822dbc5099ad1ad107794c82d2
ms.sourcegitcommit: 3a2415ab9833d5c574ad76d462f526a131c24f33
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/12/2021
ms.locfileid: "103412450"
---
# <a name="quickstart-manage-a-private-azure-marketplace-using-powershell"></a><span data-ttu-id="c1762-103">Rychlý Start: Správa privátních Azure Marketplace pomocí prostředí PowerShell</span><span class="sxs-lookup"><span data-stu-id="c1762-103">Quickstart: Manage a Private Azure Marketplace using PowerShell</span></span>

<span data-ttu-id="c1762-104">Tento článek popisuje, jak můžete spravovat nabídky v privátních Azure Marketplace pomocí modulu PowerShellu [AZ. Marketplace](/powershell/module/az.marketplace) .</span><span class="sxs-lookup"><span data-stu-id="c1762-104">This article describes how you can manage offers in a Private Azure Marketplace using the [Az.Marketplace](/powershell/module/az.marketplace) PowerShell module.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="c1762-105">Soukromé Azure Marketplace jsou momentálně ve verzi Public Preview.</span><span class="sxs-lookup"><span data-stu-id="c1762-105">Private Azure Marketplace is currently in public preview.</span></span> <span data-ttu-id="c1762-106">Tato verze Preview se poskytuje bez smlouvy o úrovni služeb.</span><span class="sxs-lookup"><span data-stu-id="c1762-106">This preview version is provided without a service level agreement.</span></span> <span data-ttu-id="c1762-107">Nedoporučuje se pro produkční úlohy.</span><span class="sxs-lookup"><span data-stu-id="c1762-107">It's not recommended for production workloads.</span></span> <span data-ttu-id="c1762-108">Některé funkce nemusí být podporované nebo můžou mít omezené možnosti.</span><span class="sxs-lookup"><span data-stu-id="c1762-108">Some features might not be supported or might have constrained capabilities.</span></span> <span data-ttu-id="c1762-109">Další informace najdete v [dodatečných podmínkách použití pro verze Preview v Microsoft Azure](https://azure.microsoft.com/support/legal/preview-supplemental-terms/).</span><span class="sxs-lookup"><span data-stu-id="c1762-109">For more information, see [Supplemental Terms of Use for Microsoft Azure Previews](https://azure.microsoft.com/support/legal/preview-supplemental-terms/).</span></span>

## <a name="requirements"></a><span data-ttu-id="c1762-110">Požadavky</span><span class="sxs-lookup"><span data-stu-id="c1762-110">Requirements</span></span>

* <span data-ttu-id="c1762-111">Pokud ještě nemáte předplatné Azure, vytvořte si [bezplatný účet](https://azure.microsoft.com/free/) před tím, než začnete.</span><span class="sxs-lookup"><span data-stu-id="c1762-111">If you don't have an Azure subscription, create a [free](https://azure.microsoft.com/free/) account before you begin.</span></span>

* <span data-ttu-id="c1762-112">Pokud se rozhodnete použít Azure PowerShell lokálně:</span><span class="sxs-lookup"><span data-stu-id="c1762-112">If you choose to use Azure PowerShell locally:</span></span>
  * <span data-ttu-id="c1762-113">[Nainstalujte modul AZ PowerShell](/powershell/azure/install-az-ps).</span><span class="sxs-lookup"><span data-stu-id="c1762-113">[Install the Az PowerShell module](/powershell/azure/install-az-ps).</span></span>
  * <span data-ttu-id="c1762-114">Připojte se k účtu Azure pomocí rutiny [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) .</span><span class="sxs-lookup"><span data-stu-id="c1762-114">Connect to your Azure account using the [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) cmdlet.</span></span>
* <span data-ttu-id="c1762-115">Pokud se rozhodnete použít Azure Cloud Shell:</span><span class="sxs-lookup"><span data-stu-id="c1762-115">If you choose to use Azure Cloud Shell:</span></span>
  * <span data-ttu-id="c1762-116">Další informace najdete v tématu [přehled Azure Cloud Shell](/azure/cloud-shell/overview) .</span><span class="sxs-lookup"><span data-stu-id="c1762-116">See [Overview of Azure Cloud Shell](/azure/cloud-shell/overview) for more information.</span></span>

  > [!IMPORTANT]
  > <span data-ttu-id="c1762-117">I když je modul PowerShellu **AZ. Marketplace** ve verzi Preview, musíte ho nainstalovat samostatně pomocí `Install-Module` rutiny.</span><span class="sxs-lookup"><span data-stu-id="c1762-117">While the **Az.Marketplace** PowerShell module is in preview, you must install it separately using the `Install-Module` cmdlet.</span></span> <span data-ttu-id="c1762-118">Jakmile bude tento powershellový modul obecně dostupný, stane se součástí budoucích verzí modulu Az PowerShellu a bude ve výchozím nastavení dostupný v rámci Azure Cloud Shellu.</span><span class="sxs-lookup"><span data-stu-id="c1762-118">After this PowerShell module becomes generally available, it will be part of future Az PowerShell module releases and available by default from within Azure Cloud Shell.</span></span>

  ```azurepowershell-interactive
  Install-Module -Name Az.Marketplace
  ```

* <span data-ttu-id="c1762-119">Pokud máte více předplatných Azure, vyberte příslušné předplatné, ve kterém se prostředky mají fakturovat.</span><span class="sxs-lookup"><span data-stu-id="c1762-119">If you have multiple Azure subscriptions, choose the appropriate subscription in which the resources should be billed.</span></span> <span data-ttu-id="c1762-120">Vyberte konkrétní předplatné pomocí rutiny [set-AzContext](/powershell/module/az.accounts/set-azcontext) .</span><span class="sxs-lookup"><span data-stu-id="c1762-120">Select a specific subscription using the [Set-AzContext](/powershell/module/az.accounts/set-azcontext) cmdlet.</span></span>

  ```azurepowershell-interactive
  Set-AzContext -SubscriptionId 00000000-0000-0000-0000-000000000000
  ```

## <a name="list-private-stores"></a><span data-ttu-id="c1762-121">Vypsat privátní úložiště</span><span class="sxs-lookup"><span data-stu-id="c1762-121">List private stores</span></span>

<span data-ttu-id="c1762-122">Pokud chcete načíst seznam privátních úložišť, použijte rutinu [Get-AzMarketplacePrivateStore](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) .</span><span class="sxs-lookup"><span data-stu-id="c1762-122">To retrieve a list of private stores, you use the [Get-AzMarketplacePrivateStore](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) cmdlet.</span></span> <span data-ttu-id="c1762-123">Následující příklad zobrazí seznam privátních úložišť, které byly vytvořeny v oboru tenanta.</span><span class="sxs-lookup"><span data-stu-id="c1762-123">The following example lists private stores that were created under the tenant scope.</span></span>

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

## <a name="add-an-offer-to-a-private-marketplace"></a><span data-ttu-id="c1762-124">Přidání nabídky do privátního tržiště</span><span class="sxs-lookup"><span data-stu-id="c1762-124">Add an offer to a private marketplace</span></span>

<span data-ttu-id="c1762-125">Chcete-li přidat nabídku do soukromého úložiště, použijte rutinu [set-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) .</span><span class="sxs-lookup"><span data-stu-id="c1762-125">To add an offer to a private store, you use the [Set-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="c1762-126">Následující příklad přidá určenou nabídku na soukromý web Marketplace pro soukromé úložiště, které je vytvořeno v rámci oboru tenanta.</span><span class="sxs-lookup"><span data-stu-id="c1762-126">The following example adds the specified offer to a private marketplace for a private store that is created under the tenant scope.</span></span>

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

## <a name="get-private-store-offers"></a><span data-ttu-id="c1762-127">Získat nabídky soukromého úložiště</span><span class="sxs-lookup"><span data-stu-id="c1762-127">Get private store offers</span></span>

<span data-ttu-id="c1762-128">Chcete-li získat jednu nebo více veřejných nabídek úložiště, použijte rutinu [Get-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) .</span><span class="sxs-lookup"><span data-stu-id="c1762-128">To get one or more private store offers, you use the [Get-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="c1762-129">Následující příklad získá nabídky, které jsou přidruženy k zadanému privátnímu úložišti, které byly přidány do oboru tenanta.</span><span class="sxs-lookup"><span data-stu-id="c1762-129">The following example gets offers that are associated with the specified private store that were added under the tenant scope.</span></span>

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

## <a name="remove-an-offer"></a><span data-ttu-id="c1762-130">Odebrání nabídky</span><span class="sxs-lookup"><span data-stu-id="c1762-130">Remove an offer</span></span>

<span data-ttu-id="c1762-131">Pokud chcete odebrat nabídku z privátního úložiště, použijte rutinu [Remove-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) .</span><span class="sxs-lookup"><span data-stu-id="c1762-131">To remove an offer from a private store, you use the [Remove-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="c1762-132">Následující příklad odebere nabídku ze soukromého úložiště, která byla vytvořena v oboru tenanta.</span><span class="sxs-lookup"><span data-stu-id="c1762-132">The following example removes an offer from a private store that was created in the tenant scope.</span></span>

```azurepowershell-interactive
Remove-AzMarketplacePrivateStoreOffer -privateStoreId 00000000-0000-0000-0000-000000000000 -offerId publisherid.offerid
```

## <a name="next-steps"></a><span data-ttu-id="c1762-133">Další kroky</span><span class="sxs-lookup"><span data-stu-id="c1762-133">Next steps</span></span>

<span data-ttu-id="c1762-134">[Vytváření a Správa privátních Azure Marketplace](create-manage-private-azure-marketplace.md).</span><span class="sxs-lookup"><span data-stu-id="c1762-134">[Create and manage Private Azure Marketplace](create-manage-private-azure-marketplace.md).</span></span>