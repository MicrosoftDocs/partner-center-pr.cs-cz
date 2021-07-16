---
title: Seznam ukázkových dotazů
description: Pomocí ukázkových dotazů můžete prostřednictvím kódu programu přistupovat k analytickým datům partnerských přehledů.
ms.topic: reference
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: e25784585a1ac505db99e58265939a8851edcbad
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376381"
---
# <a name="sample-queries-for-partner-center-insights-report"></a>Ukázkové dotazy pro Partnerské centrum přehledů

Tento článek obsahuje ukázkové dotazy pro sestavy Přehledy partnerů. Tyto dotazy můžete použít voláním koncového bodu rozhraní API pro vytvoření dotazu na sestavu. V případě potřeby je možné upravit volání rozhraní [API](insights-programmatic-access-paradigm.md#create-report-query-api) pro vytvoření dotazu na sestavu a přidat další sloupce, upravit dobu výpočtu a přidat podmínky filtru.

Podrobnosti o názvech sloupců, atributech a popisech najdete v tématu [Definice dat.](insights-data-definitions.md)

## <a name="customer-details"></a>Podrobnosti o zákazníkovi

Tyto ukázkové dotazy se vztahují na sestavu podrobností o zákaznících:

### <a name="by-geography"></a>Podle zeměpisné oblasti

Seznam zákazníků z konkrétní geografické oblasti za poslední měsíc

```sql
SELECT CustomerName, CustomerTpid, Product 
FROM CustomersAndTenants 
WHERE CustomerMarket='United States' TIMESPAN LAST_MONTH
```

### <a name="by-sku-and-billed-revenue"></a>Podle SKU a fakturovaných výnosů

Seznam zákazníků, kteří za posledních 6 měsíců používají konkrétní SKU a fakturované výnosy, je více než 20 000.

```sql
SELECT CustomerName, CustomerTpid, SKU, Month, BilledRevenueUSD 
FROM CustomersAndTenants 
WHERE SKU='MICROSOFT 365 BUSINESS STANDARD' AND BilledRevenueUSD>20000 TIMESPAN LAST_6_MONTHS
```

### <a name="by-available-seats"></a>Podle dostupných licencí

Top 10 customers based on Available seats in last month

```sql
SELECT CustomerName, CustomerTpid, Product, AvailableSeats 
FROM CustomersAndTenants ORDER BY AvailableSeats DESC LIMIT 10 TIMESPAN LAST_MONTH
```

## <a name="partner-profile"></a>Profil partnera

Tyto ukázkové dotazy se vztahují na sestavu profilu partnera:

### <a name="by-geography"></a>Podle zeměpisné oblasti

Seznam partnerů z konkrétní geografické oblasti

```sql
SELECT MPNId, PartnerName 
FROM Profile 
WHERE Country='United States'
```

### <a name="by-mpn-partner"></a>Podle partnera MPN

Seznam partnerů v rámci stejného partnera PGA MPN

```sql
SELECT MPNId, PartnerName, PGAMpnId 
FROM Profile 
WHERE PGAMpnId='1001xx'
```

## <a name="reseller-performance"></a>Reseller Performance

Tyto ukázkové dotazy se vztahují na sestavu výkonu prodejce:

### <a name="by-geography"></a>Podle zeměpisné oblasti

Seznam prodejců z konkrétní geografické oblasti za poslední měsíc

```sql
SELECT ResellerMpnId, ResellerName 
FROM ResellerPerformance 
WHERE ResellerMarket='US' TIMESPAN LAST_MONTH
```

### <a name="by-reseller"></a>Podle prodejce

Customer count, subscription count, total available seats, total assigned seats, total revenue for a specific reseller.

```sql
SELECT ResellerMpnId, ResellerName, CustomerCount, SubscriptionCount, TotalAvailableSeats, TotalAssignedSeats, TotalRevenue 
FROM ResellerPerformance 
WHERE ResellerMpnId='1051xxx'
```

### <a name="top-10-by-revenue"></a>Top 10 by revenue

Top 10 resellers based on total revenue in last month.

```sql
SELECT ResellerMpnId, ResellerName, TotalRevenue 
FROM ResellerPerformance 
ORDER BY TotalRevenue 
LIMIT 10 
TIMESPAN LAST_MONTH
```

## <a name="subscription-details"></a>Podrobnosti o předplatném

Tyto ukázkové dotazy se vztahují na sestavu podrobností o předplatném:

### <a name="by-renewal-eligibility"></a>Podle způsobilosti pro prodloužení

Seznam předplatných, která za poslední měsíc nemají nárok na automatické prodlužování platnosti

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE IsAutoRenew='N' TIMESPAN LAST_MONTH
```

### <a name="by-subscription-state"></a>Podle stavu předplatného

Seznam předplatných, která jsou za poslední měsíc ve stavu Zakázat

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE SubscriptionState='Disabled' TIMESPAN LAST_MONTH
```

### <a name="counts-for-six-months"></a>Počty za šest měsíců

Počet předplatných, celkový počet prodaných licencí, počet zákazníků pro konkrétního partnera za posledních šest měsíců.

```sql
SELECT MPNId, SubscriptionCount, TotalSoldSeats, BilledRevenueUSD, CustomerCount 
FROM SeatsSubscriptionsAndRevenue 
WHERE MPNId=6096xxx TIMESPAN LAST_6_MONTHS
```

## <a name="azure-usage"></a>Využití Azure

Tyto ukázkové dotazy se vztahují na sestavu využití Azure:

### <a name="by-meter-category"></a>Podle kategorie měřiče

Seznam předplatných využití Azure s jednotkami využití a ACR pro konkrétní kategorii měřičů za posledních šest měsíců

```sql
SELECT SubscriptionId, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE MeterCategory='Azure DNS' 
TIMESPAN LAST_6_MONTHS
```

### <a name="by-total-acr"></a>Podle celkového počtu ACR

Seznam předplatných využití Azure, ve kterých je celkový počet ACR za posledních šest měsíců vyšší než 20 000

```sql
SELECT SubscriptionId, ServiceName, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE TotalACR>20000 TIMESPAN LAST_6_MONTHS
```

## <a name="next-steps"></a>Další kroky

- [Rozhraní API pro přístup k analytickým datům partnerských přehledů](insights-programmatic-analytics-available-api.md)