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
# <a name="sample-queries-for-partner-center-insights-report"></a><span data-ttu-id="d35fe-103">Ukázkové dotazy pro Partnerské centrum přehledů</span><span class="sxs-lookup"><span data-stu-id="d35fe-103">Sample queries for Partner Center insights report</span></span>

<span data-ttu-id="d35fe-104">Tento článek obsahuje ukázkové dotazy pro sestavy Přehledy partnerů.</span><span class="sxs-lookup"><span data-stu-id="d35fe-104">This article provides sample queries for the Partner Insights reports.</span></span> <span data-ttu-id="d35fe-105">Tyto dotazy můžete použít voláním koncového bodu rozhraní API pro vytvoření dotazu na sestavu.</span><span class="sxs-lookup"><span data-stu-id="d35fe-105">You can use these queries by calling the Create Report Query API endpoint.</span></span> <span data-ttu-id="d35fe-106">V případě potřeby je možné upravit volání rozhraní [API](insights-programmatic-access-paradigm.md#create-report-query-api) pro vytvoření dotazu na sestavu a přidat další sloupce, upravit dobu výpočtu a přidat podmínky filtru.</span><span class="sxs-lookup"><span data-stu-id="d35fe-106">If necessary, the [Create Report Query API](insights-programmatic-access-paradigm.md#create-report-query-api) call can be modified to add more columns, adjust the computation period, and add filter conditions.</span></span>

<span data-ttu-id="d35fe-107">Podrobnosti o názvech sloupců, atributech a popisech najdete v tématu [Definice dat.](insights-data-definitions.md)</span><span class="sxs-lookup"><span data-stu-id="d35fe-107">For details about the column names, attributes, and descriptions, refer to the [Data Definitions](insights-data-definitions.md).</span></span>

## <a name="customer-details"></a><span data-ttu-id="d35fe-108">Podrobnosti o zákazníkovi</span><span class="sxs-lookup"><span data-stu-id="d35fe-108">Customer details</span></span>

<span data-ttu-id="d35fe-109">Tyto ukázkové dotazy se vztahují na sestavu podrobností o zákaznících:</span><span class="sxs-lookup"><span data-stu-id="d35fe-109">These sample queries apply to the customers details report:</span></span>

### <a name="by-geography"></a><span data-ttu-id="d35fe-110">Podle zeměpisné oblasti</span><span class="sxs-lookup"><span data-stu-id="d35fe-110">By geography</span></span>

<span data-ttu-id="d35fe-111">Seznam zákazníků z konkrétní geografické oblasti za poslední měsíc</span><span class="sxs-lookup"><span data-stu-id="d35fe-111">List of customers from a specific geography in last month.</span></span>

```sql
SELECT CustomerName, CustomerTpid, Product 
FROM CustomersAndTenants 
WHERE CustomerMarket='United States' TIMESPAN LAST_MONTH
```

### <a name="by-sku-and-billed-revenue"></a><span data-ttu-id="d35fe-112">Podle SKU a fakturovaných výnosů</span><span class="sxs-lookup"><span data-stu-id="d35fe-112">By SKU and billed revenue</span></span>

<span data-ttu-id="d35fe-113">Seznam zákazníků, kteří za posledních 6 měsíců používají konkrétní SKU a fakturované výnosy, je více než 20 000.</span><span class="sxs-lookup"><span data-stu-id="d35fe-113">List of customers using specific SKU and Billed Revenue is more than 20,000 in the last 6 months</span></span>

```sql
SELECT CustomerName, CustomerTpid, SKU, Month, BilledRevenueUSD 
FROM CustomersAndTenants 
WHERE SKU='MICROSOFT 365 BUSINESS STANDARD' AND BilledRevenueUSD>20000 TIMESPAN LAST_6_MONTHS
```

### <a name="by-available-seats"></a><span data-ttu-id="d35fe-114">Podle dostupných licencí</span><span class="sxs-lookup"><span data-stu-id="d35fe-114">By available seats</span></span>

<span data-ttu-id="d35fe-115">Top 10 customers based on Available seats in last month</span><span class="sxs-lookup"><span data-stu-id="d35fe-115">Top 10 customers based on Available seats in last month</span></span>

```sql
SELECT CustomerName, CustomerTpid, Product, AvailableSeats 
FROM CustomersAndTenants ORDER BY AvailableSeats DESC LIMIT 10 TIMESPAN LAST_MONTH
```

## <a name="partner-profile"></a><span data-ttu-id="d35fe-116">Profil partnera</span><span class="sxs-lookup"><span data-stu-id="d35fe-116">Partner Profile</span></span>

<span data-ttu-id="d35fe-117">Tyto ukázkové dotazy se vztahují na sestavu profilu partnera:</span><span class="sxs-lookup"><span data-stu-id="d35fe-117">These sample queries apply to the partner profile report:</span></span>

### <a name="by-geography"></a><span data-ttu-id="d35fe-118">Podle zeměpisné oblasti</span><span class="sxs-lookup"><span data-stu-id="d35fe-118">By geography</span></span>

<span data-ttu-id="d35fe-119">Seznam partnerů z konkrétní geografické oblasti</span><span class="sxs-lookup"><span data-stu-id="d35fe-119">List of partners from a specific geography.</span></span>

```sql
SELECT MPNId, PartnerName 
FROM Profile 
WHERE Country='United States'
```

### <a name="by-mpn-partner"></a><span data-ttu-id="d35fe-120">Podle partnera MPN</span><span class="sxs-lookup"><span data-stu-id="d35fe-120">By MPN partner</span></span>

<span data-ttu-id="d35fe-121">Seznam partnerů v rámci stejného partnera PGA MPN</span><span class="sxs-lookup"><span data-stu-id="d35fe-121">List of partners under same PGA MPN Partner</span></span>

```sql
SELECT MPNId, PartnerName, PGAMpnId 
FROM Profile 
WHERE PGAMpnId='1001xx'
```

## <a name="reseller-performance"></a><span data-ttu-id="d35fe-122">Reseller Performance</span><span class="sxs-lookup"><span data-stu-id="d35fe-122">Reseller Performance</span></span>

<span data-ttu-id="d35fe-123">Tyto ukázkové dotazy se vztahují na sestavu výkonu prodejce:</span><span class="sxs-lookup"><span data-stu-id="d35fe-123">These sample queries apply to the reseller performance report:</span></span>

### <a name="by-geography"></a><span data-ttu-id="d35fe-124">Podle zeměpisné oblasti</span><span class="sxs-lookup"><span data-stu-id="d35fe-124">By geography</span></span>

<span data-ttu-id="d35fe-125">Seznam prodejců z konkrétní geografické oblasti za poslední měsíc</span><span class="sxs-lookup"><span data-stu-id="d35fe-125">List of resellers from a specific geography in last month.</span></span>

```sql
SELECT ResellerMpnId, ResellerName 
FROM ResellerPerformance 
WHERE ResellerMarket='US' TIMESPAN LAST_MONTH
```

### <a name="by-reseller"></a><span data-ttu-id="d35fe-126">Podle prodejce</span><span class="sxs-lookup"><span data-stu-id="d35fe-126">By reseller</span></span>

<span data-ttu-id="d35fe-127">Customer count, subscription count, total available seats, total assigned seats, total revenue for a specific reseller.</span><span class="sxs-lookup"><span data-stu-id="d35fe-127">Customer count, subscription count, total available seats, total assigned seats, total revenue for a specific reseller.</span></span>

```sql
SELECT ResellerMpnId, ResellerName, CustomerCount, SubscriptionCount, TotalAvailableSeats, TotalAssignedSeats, TotalRevenue 
FROM ResellerPerformance 
WHERE ResellerMpnId='1051xxx'
```

### <a name="top-10-by-revenue"></a><span data-ttu-id="d35fe-128">Top 10 by revenue</span><span class="sxs-lookup"><span data-stu-id="d35fe-128">Top 10 by revenue</span></span>

<span data-ttu-id="d35fe-129">Top 10 resellers based on total revenue in last month.</span><span class="sxs-lookup"><span data-stu-id="d35fe-129">Top 10 resellers based on total revenue in last month.</span></span>

```sql
SELECT ResellerMpnId, ResellerName, TotalRevenue 
FROM ResellerPerformance 
ORDER BY TotalRevenue 
LIMIT 10 
TIMESPAN LAST_MONTH
```

## <a name="subscription-details"></a><span data-ttu-id="d35fe-130">Podrobnosti o předplatném</span><span class="sxs-lookup"><span data-stu-id="d35fe-130">Subscription Details</span></span>

<span data-ttu-id="d35fe-131">Tyto ukázkové dotazy se vztahují na sestavu podrobností o předplatném:</span><span class="sxs-lookup"><span data-stu-id="d35fe-131">These sample queries apply to the subscription details report:</span></span>

### <a name="by-renewal-eligibility"></a><span data-ttu-id="d35fe-132">Podle způsobilosti pro prodloužení</span><span class="sxs-lookup"><span data-stu-id="d35fe-132">By renewal eligibility</span></span>

<span data-ttu-id="d35fe-133">Seznam předplatných, která za poslední měsíc nemají nárok na automatické prodlužování platnosti</span><span class="sxs-lookup"><span data-stu-id="d35fe-133">List of subscriptions who are not eligible for auto renewal in last month.</span></span>

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE IsAutoRenew='N' TIMESPAN LAST_MONTH
```

### <a name="by-subscription-state"></a><span data-ttu-id="d35fe-134">Podle stavu předplatného</span><span class="sxs-lookup"><span data-stu-id="d35fe-134">By subscription state</span></span>

<span data-ttu-id="d35fe-135">Seznam předplatných, která jsou za poslední měsíc ve stavu Zakázat</span><span class="sxs-lookup"><span data-stu-id="d35fe-135">List of subscriptions who are in Disable state in last month.</span></span>

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE SubscriptionState='Disabled' TIMESPAN LAST_MONTH
```

### <a name="counts-for-six-months"></a><span data-ttu-id="d35fe-136">Počty za šest měsíců</span><span class="sxs-lookup"><span data-stu-id="d35fe-136">Counts for six months</span></span>

<span data-ttu-id="d35fe-137">Počet předplatných, celkový počet prodaných licencí, počet zákazníků pro konkrétního partnera za posledních šest měsíců.</span><span class="sxs-lookup"><span data-stu-id="d35fe-137">Subscription count, total sold seats, customer count for a specific partner in last six months.</span></span>

```sql
SELECT MPNId, SubscriptionCount, TotalSoldSeats, BilledRevenueUSD, CustomerCount 
FROM SeatsSubscriptionsAndRevenue 
WHERE MPNId=6096xxx TIMESPAN LAST_6_MONTHS
```

## <a name="azure-usage"></a><span data-ttu-id="d35fe-138">Využití Azure</span><span class="sxs-lookup"><span data-stu-id="d35fe-138">Azure Usage</span></span>

<span data-ttu-id="d35fe-139">Tyto ukázkové dotazy se vztahují na sestavu využití Azure:</span><span class="sxs-lookup"><span data-stu-id="d35fe-139">These sample queries apply to the Azure usage report:</span></span>

### <a name="by-meter-category"></a><span data-ttu-id="d35fe-140">Podle kategorie měřiče</span><span class="sxs-lookup"><span data-stu-id="d35fe-140">By meter category</span></span>

<span data-ttu-id="d35fe-141">Seznam předplatných využití Azure s jednotkami využití a ACR pro konkrétní kategorii měřičů za posledních šest měsíců</span><span class="sxs-lookup"><span data-stu-id="d35fe-141">List of Azure usage subscriptions with usage units and ACR for specific meter category in last six months.</span></span>

```sql
SELECT SubscriptionId, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE MeterCategory='Azure DNS' 
TIMESPAN LAST_6_MONTHS
```

### <a name="by-total-acr"></a><span data-ttu-id="d35fe-142">Podle celkového počtu ACR</span><span class="sxs-lookup"><span data-stu-id="d35fe-142">By total ACR</span></span>

<span data-ttu-id="d35fe-143">Seznam předplatných využití Azure, ve kterých je celkový počet ACR za posledních šest měsíců vyšší než 20 000</span><span class="sxs-lookup"><span data-stu-id="d35fe-143">List of Azure usage subscriptions where total ACR is greater than 20,000 in last six months</span></span>

```sql
SELECT SubscriptionId, ServiceName, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE TotalACR>20000 TIMESPAN LAST_6_MONTHS
```

## <a name="next-steps"></a><span data-ttu-id="d35fe-144">Další kroky</span><span class="sxs-lookup"><span data-stu-id="d35fe-144">Next steps</span></span>

- [<span data-ttu-id="d35fe-145">Rozhraní API pro přístup k analytickým datům partnerských přehledů</span><span class="sxs-lookup"><span data-stu-id="d35fe-145">APIs for accessing partner insights analytics data</span></span>](insights-programmatic-analytics-available-api.md)