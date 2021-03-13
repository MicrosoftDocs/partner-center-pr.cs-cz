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
# <a name="quickstart-manage-a-private-azure-marketplace-using-powershell"></a>Rychlý Start: Správa privátních Azure Marketplace pomocí prostředí PowerShell

Tento článek popisuje, jak můžete spravovat nabídky v privátních Azure Marketplace pomocí modulu PowerShellu [AZ. Marketplace](/powershell/module/az.marketplace) .

> [!IMPORTANT]
> Soukromé Azure Marketplace jsou momentálně ve verzi Public Preview. Tato verze Preview se poskytuje bez smlouvy o úrovni služeb. Nedoporučuje se pro produkční úlohy. Některé funkce nemusí být podporované nebo můžou mít omezené možnosti. Další informace najdete v [dodatečných podmínkách použití pro verze Preview v Microsoft Azure](https://azure.microsoft.com/support/legal/preview-supplemental-terms/).

## <a name="requirements"></a>Požadavky

* Pokud ještě nemáte předplatné Azure, vytvořte si [bezplatný účet](https://azure.microsoft.com/free/) před tím, než začnete.

* Pokud se rozhodnete použít Azure PowerShell lokálně:
  * [Nainstalujte modul AZ PowerShell](/powershell/azure/install-az-ps).
  * Připojte se k účtu Azure pomocí rutiny [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) .
* Pokud se rozhodnete použít Azure Cloud Shell:
  * Další informace najdete v tématu [přehled Azure Cloud Shell](/azure/cloud-shell/overview) .

  > [!IMPORTANT]
  > I když je modul PowerShellu **AZ. Marketplace** ve verzi Preview, musíte ho nainstalovat samostatně pomocí `Install-Module` rutiny. Jakmile bude tento powershellový modul obecně dostupný, stane se součástí budoucích verzí modulu Az PowerShellu a bude ve výchozím nastavení dostupný v rámci Azure Cloud Shellu.

  ```azurepowershell-interactive
  Install-Module -Name Az.Marketplace
  ```

* Pokud máte více předplatných Azure, vyberte příslušné předplatné, ve kterém se prostředky mají fakturovat. Vyberte konkrétní předplatné pomocí rutiny [set-AzContext](/powershell/module/az.accounts/set-azcontext) .

  ```azurepowershell-interactive
  Set-AzContext -SubscriptionId 00000000-0000-0000-0000-000000000000
  ```

## <a name="list-private-stores"></a>Vypsat privátní úložiště

Pokud chcete načíst seznam privátních úložišť, použijte rutinu [Get-AzMarketplacePrivateStore](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) . Následující příklad zobrazí seznam privátních úložišť, které byly vytvořeny v oboru tenanta.

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

## <a name="add-an-offer-to-a-private-marketplace"></a>Přidání nabídky do privátního tržiště

Chcete-li přidat nabídku do soukromého úložiště, použijte rutinu [set-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) . Následující příklad přidá určenou nabídku na soukromý web Marketplace pro soukromé úložiště, které je vytvořeno v rámci oboru tenanta.

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

## <a name="get-private-store-offers"></a>Získat nabídky soukromého úložiště

Chcete-li získat jednu nebo více veřejných nabídek úložiště, použijte rutinu [Get-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) . Následující příklad získá nabídky, které jsou přidruženy k zadanému privátnímu úložišti, které byly přidány do oboru tenanta.

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

## <a name="remove-an-offer"></a>Odebrání nabídky

Pokud chcete odebrat nabídku z privátního úložiště, použijte rutinu [Remove-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) . Následující příklad odebere nabídku ze soukromého úložiště, která byla vytvořena v oboru tenanta.

```azurepowershell-interactive
Remove-AzMarketplacePrivateStoreOffer -privateStoreId 00000000-0000-0000-0000-000000000000 -offerId publisherid.offerid
```

## <a name="next-steps"></a>Další kroky

[Vytváření a Správa privátních Azure Marketplace](create-manage-private-azure-marketplace.md).