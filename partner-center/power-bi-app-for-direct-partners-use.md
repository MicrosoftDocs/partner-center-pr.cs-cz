---
title: Použití analýzy partnerského centra pro Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Naučte se zobrazovat obchodní data pomocí aplikace Datacenter Center Analytics pro Power BI (pro přímé partnery v CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 248527fdbc536c552f7b2d00f208838b4ef19085
ms.sourcegitcommit: 0a6b1e6d845391539f54213efff00af4d23f028c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/14/2020
ms.locfileid: "92527000"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="be197-103">Zobrazení obchodních dat pomocí aplikace Datacenter Center Analytics pro Microsoft Power BI</span><span class="sxs-lookup"><span data-stu-id="be197-103">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>

<span data-ttu-id="be197-104">**Platí pro**</span><span class="sxs-lookup"><span data-stu-id="be197-104">**Applies to**</span></span>

- <span data-ttu-id="be197-105">Partnerské centrum</span><span class="sxs-lookup"><span data-stu-id="be197-105">Partner Center</span></span>

<span data-ttu-id="be197-106">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="be197-106">**Appropriate roles**</span></span>

- <span data-ttu-id="be197-107">Globální správce</span><span class="sxs-lookup"><span data-stu-id="be197-107">Global admin</span></span>
- <span data-ttu-id="be197-108">Správce uživatelů</span><span class="sxs-lookup"><span data-stu-id="be197-108">User admin</span></span>
- <span data-ttu-id="be197-109">Agent prodeje</span><span class="sxs-lookup"><span data-stu-id="be197-109">Sales agent</span></span>
- <span data-ttu-id="be197-110">Agent správce</span><span class="sxs-lookup"><span data-stu-id="be197-110">Admin agent</span></span>

## <a name="view-your-business-data"></a><span data-ttu-id="be197-111">Zobrazení obchodních dat</span><span class="sxs-lookup"><span data-stu-id="be197-111">View your business data</span></span>

<span data-ttu-id="be197-112">Získejte vizuální reprezentaci vašich obchodních dat pomocí aplikace Datacenter Center Analytics pro Power BI, včetně těchto:</span><span class="sxs-lookup"><span data-stu-id="be197-112">Get a visual representation of your business data with the Partner Center Analytics app for Power BI, including:</span></span>

- <span data-ttu-id="be197-113">Růst zákaznické základny, předplatných a licencí</span><span class="sxs-lookup"><span data-stu-id="be197-113">Growth of your customer base, subscriptions, and licenses</span></span>

- <span data-ttu-id="be197-114">Využití produktů Office 365, Microsoft Dynamics a Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="be197-114">Usage of Office 365, Microsoft Dynamics, and Microsoft Azure products</span></span>

- <span data-ttu-id="be197-115">Denní spotřeba jednotek pro každý měřený prostředek v každém předplatném Azure za posledních 60 dní</span><span class="sxs-lookup"><span data-stu-id="be197-115">Daily consumption units for each metered resource in each Azure subscription for the last 60 days</span></span>

- <span data-ttu-id="be197-116">Odhadované náklady (na základě karty s nejnovějšími sazbami)</span><span class="sxs-lookup"><span data-stu-id="be197-116">Estimated cost (based on latest rate card)</span></span>

- <span data-ttu-id="be197-117">Možnost exportovat datové sady a vytvářet vlastní sestavy, včetně jednotlivých zákazníků.</span><span class="sxs-lookup"><span data-stu-id="be197-117">Ability to export datasets and create custom reports, including per customer.</span></span>

### <a name="about-the-partner-center-analytics-app-preview-release"></a><span data-ttu-id="be197-118">Informace o verzi Preview partnerského centra pro aplikaci Analytics</span><span class="sxs-lookup"><span data-stu-id="be197-118">About the Partner Center Analytics app preview release</span></span>

- <span data-ttu-id="be197-119">Tato aplikace je určena pouze pro přímé partnery v programu Cloud Solution Provider.</span><span class="sxs-lookup"><span data-stu-id="be197-119">This app is for direct partners in the Cloud Solution Provider program only.</span></span> <span data-ttu-id="be197-120">Jiní partneři v CSP (například nepřímo prodejci) se nebudou moci přihlásit.</span><span class="sxs-lookup"><span data-stu-id="be197-120">Other partners in CSP (indirect resellers, for example) will not be able to sign in.</span></span>

- <span data-ttu-id="be197-121">Všechny odhadované náklady jsou platby před zdaněním a fakturaci a nejsou právně závazné.</span><span class="sxs-lookup"><span data-stu-id="be197-121">Any estimated costs are pre-tax billing / invoice data, and are not legally binding.</span></span> <span data-ttu-id="be197-122">Odhadované náklady se mají použít jenom pro data Insights.</span><span class="sxs-lookup"><span data-stu-id="be197-122">Estimated costs are meant to be used for data insights only.</span></span>

- <span data-ttu-id="be197-123">Informace o zákaznících jsou založené na předplatných.</span><span class="sxs-lookup"><span data-stu-id="be197-123">Customer information is based on subscriptions.</span></span> <span data-ttu-id="be197-124">Zákazníci, u kterých jste nedávno vytvořili účty pro, ale kteří ještě nemají předplatné, nejsou zahrnuti do počtu.</span><span class="sxs-lookup"><span data-stu-id="be197-124">Any customers that you've recently created accounts for, but who do not yet have subscriptions, are not included in counts.</span></span>

- <span data-ttu-id="be197-125">Odhadované náklady vycházejí z karty nejnovějších sazeb, která vychází z cen CSP.</span><span class="sxs-lookup"><span data-stu-id="be197-125">Estimated cost is based on latest rate card, which is based on CSP pricing.</span></span>

- <span data-ttu-id="be197-126">Dny jsou dny kalendáře.</span><span class="sxs-lookup"><span data-stu-id="be197-126">Days are calendar days.</span></span>

### <a name="business-insights-report"></a><span data-ttu-id="be197-127">Sestava obchodních přehledů</span><span class="sxs-lookup"><span data-stu-id="be197-127">Business Insights report</span></span>

- <span data-ttu-id="be197-128">**Klienti zákazníka** : počet různých TENANTŮ Azure AD pro zákazníky, kteří si zakoupili předplatná</span><span class="sxs-lookup"><span data-stu-id="be197-128">**Customer tenants** : Number of distinct Azure AD tenants of customers that have purchased subscriptions</span></span>

- <span data-ttu-id="be197-129">**Novinka (posledních 30 dnů)** : noví zákazníci, kteří si nakupují aspoň jedno předplatné za posledních 30 dní</span><span class="sxs-lookup"><span data-stu-id="be197-129">**New (last 30 days)** : New customers purchasing at least one subscription in last 30 days</span></span>

- <span data-ttu-id="be197-130">Změny **(posledních 30 dnů)** : zákazníci bez všech předplatných "aktivní", "v odkladu" nebo "zakázáno".</span><span class="sxs-lookup"><span data-stu-id="be197-130">**Churn (last 30 days)** : Customers without any “active", “in grace" or “disabled" subscriptions</span></span>

- <span data-ttu-id="be197-131">**Novinka (posledních 24 hodin)** : noví zákazníci nakupují aspoň jedno předplatné za posledních 24 hodin</span><span class="sxs-lookup"><span data-stu-id="be197-131">**New (last 24 hours)** : New customers purchasing at least one subscription in last 24 hours</span></span>

- <span data-ttu-id="be197-132">**Odhadované měsíční náklady za posledních 12 měsíců** : Měsíční trend odhadované částky za měsíc v měsíci, který je v období posledních 12 měsíců agregovaný měsíčně.</span><span class="sxs-lookup"><span data-stu-id="be197-132">**Estimated monthly cost over last 12 months** : Month over month trend of estimated pre-tax invoice dollar amount aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="be197-133">**Odhadované náklady podle produktu za posledních 12 měsíců** : produkty prodávané podle odhadované částky pro fakturační dolary, které jsou shrnuty v období posledních 12 měsíců.</span><span class="sxs-lookup"><span data-stu-id="be197-133">**Estimated cost by product over last 12 months** : Products sold sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="be197-134">Tento stav označuje nejdůležitější produkty, které přináší většinu výnosů.</span><span class="sxs-lookup"><span data-stu-id="be197-134">This status indicates top products bringing most revenue.</span></span>

- <span data-ttu-id="be197-135">**Zákazníci za posledních 12 měsíců** : trend za měsíc měsíčně nových zákazníků a změny, které se zákazníkům v období posledních 12 měsíců agreguje měsíčně</span><span class="sxs-lookup"><span data-stu-id="be197-135">**Customers over last 12 months** : Month over month trend of new customers and churn customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="be197-136">**Odhadované náklady podle zákazníka za posledních 12 měsíců** : zákazníci setříděni podle odhadované částky předběžného daňového dolaru shrnuté v období posledních 12 měsíců.</span><span class="sxs-lookup"><span data-stu-id="be197-136">**Estimated cost by customer over last 12 months** : Customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="be197-137">Tento stav označuje nejdůležitější zákazníky, kteří přinášejí většinu výnosů.</span><span class="sxs-lookup"><span data-stu-id="be197-137">This status indicates top customers bringing most revenue.</span></span>

- <span data-ttu-id="be197-138">**Počet zákazníků podle produktu** : produktů prodávaných seřazené podle přidružených zákazníků.</span><span class="sxs-lookup"><span data-stu-id="be197-138">**Customer count by product** : Products sold sorted by associated customers.</span></span> <span data-ttu-id="be197-139">Tento stav označuje nejdůležitější produkty prodávané většině zákazníků.</span><span class="sxs-lookup"><span data-stu-id="be197-139">This status indicates top products sold to most customers.</span></span>

### <a name="subscription-insights-report"></a><span data-ttu-id="be197-140">Sestava přehledů předplatných</span><span class="sxs-lookup"><span data-stu-id="be197-140">Subscription Insights report</span></span>

- <span data-ttu-id="be197-141">**Stav předplatného** :</span><span class="sxs-lookup"><span data-stu-id="be197-141">**Subscription status** :</span></span>

- <span data-ttu-id="be197-142">Aktivní: předplatná, která patří do stavu "aktivní" nebo "ve lhůtě".</span><span class="sxs-lookup"><span data-stu-id="be197-142">Active: Subscriptions belonging to either “active" or “in grace" state</span></span>

  - <span data-ttu-id="be197-143">Pozastaveno: odběry patřící do stavu zakázáno</span><span class="sxs-lookup"><span data-stu-id="be197-143">Suspended: Subscriptions belonging to “disabled" state</span></span>

  - <span data-ttu-id="be197-144">Nezřízeno: odběry patřící do stavu "de-provisioned" nebo "vypršela platnost"</span><span class="sxs-lookup"><span data-stu-id="be197-144">De-provisioned: Subscriptions belonging to “de-provisioned" or “expired" status</span></span>

- <span data-ttu-id="be197-145">**Stav vypršení platnosti** :</span><span class="sxs-lookup"><span data-stu-id="be197-145">**Expiry status** :</span></span>

  - <span data-ttu-id="be197-146">Vypršela platnost předplatných, jejichž platnost již vypršela (kde koncové datum předplatného je v minulosti).</span><span class="sxs-lookup"><span data-stu-id="be197-146">Expired: Subscriptions that have already expired (where subscription end date is in past)</span></span>

  - <span data-ttu-id="be197-147">Vypršení platnosti po 30 dnech: předplatná, jejichž platnost vyprší po 30 dnech (kde koncové datum předplatného je po následujících 30 dnech)</span><span class="sxs-lookup"><span data-stu-id="be197-147">Expiring after 30 days: Subscriptions that will expire after 30 days (where subscription end date is after next 30 days)</span></span>

  - <span data-ttu-id="be197-148">Vypršení platnosti během 30 dnů: předplatná, jejichž platnost vyprší během následujících 30 dnů (kde datum ukončení předplatného spadá do rozmezí dnešních a dalších 30 dnů)</span><span class="sxs-lookup"><span data-stu-id="be197-148">Expiring in 30 days: Subscriptions that will expire within next 30 days (where subscription end date is between today and next 30 days)</span></span>

- <span data-ttu-id="be197-149">**Celkový počet předplatných** : předplatná ve stavu "aktivní", "ve lhůtě" nebo "zakázáno"</span><span class="sxs-lookup"><span data-stu-id="be197-149">**Total subscriptions** : Subscriptions in “active," “in grace" or “disabled" status</span></span>

- <span data-ttu-id="be197-150">**Novinka (posledních 30 dnů)** : nové předplatné zakoupené zákazníky během posledních 30 dnů</span><span class="sxs-lookup"><span data-stu-id="be197-150">**New (last 30 days)** : New subscriptions purchased by customers within last 30 days</span></span>

- <span data-ttu-id="be197-151">**Novinka (posledních 24 hodin)** : nové předplatné zakoupené zákazníky během posledních 24 hodin</span><span class="sxs-lookup"><span data-stu-id="be197-151">**New (last 24 hours)** : New subscriptions purchased by customers within last 24 hours</span></span>

- <span data-ttu-id="be197-152">**Platnost vyprší za 30 dní** : předplatná, jejichž platnost vyprší během následujících 30 dnů</span><span class="sxs-lookup"><span data-stu-id="be197-152">**Expiring in 30 days** : Subscriptions that will expire within next 30 days</span></span>

- <span data-ttu-id="be197-153">Změny **(posledních 30 dnů)** : předplatná, která byla během posledních 30 dnů zrušena nebo pozastavena (zakázána)</span><span class="sxs-lookup"><span data-stu-id="be197-153">**Churn (last 30 days)** : Subscriptions that have been de-provisioned or Suspended (disabled) within last 30 days</span></span>

- <span data-ttu-id="be197-154">**Distribuce podle typů předplatného** :% distribuce celkových předplatných podle licencí a typu předplatného založeného na použití</span><span class="sxs-lookup"><span data-stu-id="be197-154">**Distribution by subscription types** : % distribution of total subscriptions by License based and usage-based subscription type</span></span>

- <span data-ttu-id="be197-155">**Počet aktivních předplatných podle produktu** : produkty prodávané seřazené podle aktivního počtu předplatných</span><span class="sxs-lookup"><span data-stu-id="be197-155">**Active subscription count by product** : Products sold sorted by active subscriptions count</span></span>

- <span data-ttu-id="be197-156">**Předplatná za posledních 12 měsíců** : trend za měsíc měsíčně nových předplatných a všech předplatných, které jsou v období posledních 12 měsíců agregované měsíčně.</span><span class="sxs-lookup"><span data-stu-id="be197-156">**Subscriptions over last 12 months** : Month over month trend of new subscriptions and churn subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="be197-157">**Podrobnosti o předplatném zákazníka** : podrobné zobrazení zákazníků, předplatných a nabídek</span><span class="sxs-lookup"><span data-stu-id="be197-157">**Customer subscription details** : Detailed view of the customers, subscriptions, and offers</span></span>

### <a name="license-insights-report"></a><span data-ttu-id="be197-158">Sestava o licenci License Insights:</span><span class="sxs-lookup"><span data-stu-id="be197-158">License Insights report:</span></span>

- <span data-ttu-id="be197-159">**Celkem licencí** : celkový počet licencí agregovaných napříč všemi předplatnými na základě licencí</span><span class="sxs-lookup"><span data-stu-id="be197-159">**Total licenses** : Total number of licenses aggregated across all license-based subscriptions</span></span>

- <span data-ttu-id="be197-160">**Novinka (posledních 30 dnů)** : Přidání licence během posledních 30 dnů</span><span class="sxs-lookup"><span data-stu-id="be197-160">**New (last 30 days)** : License addition within last 30 days</span></span>

- <span data-ttu-id="be197-161">Změny **(posledních 30 dnů)** : snížení počtu licencí během posledních 30 dnů</span><span class="sxs-lookup"><span data-stu-id="be197-161">**Churn (last 30 days)** : License reduction within last 30 days</span></span>

- <span data-ttu-id="be197-162">**Novinka (posledních 24 hodin)** : Přidání licence během posledních 24 hodin</span><span class="sxs-lookup"><span data-stu-id="be197-162">**New (last 24 hours)** : License addition within last 24 hours</span></span>

- <span data-ttu-id="be197-163">**Licence v posledních 90 dnech** : Měsíční trend přidaných licencí a jejich snížení na měsíc za období posledních 90 dnů</span><span class="sxs-lookup"><span data-stu-id="be197-163">**Licenses over last 90 days** : Month over month trend of license additions and reductions aggregated monthly over the period of last 90 days</span></span>

- <span data-ttu-id="be197-164">**Počet aktivních licencí podle produktu** : produkty prodávané seřazené podle počtu aktivních licencí</span><span class="sxs-lookup"><span data-stu-id="be197-164">**Active license count by product** : Products sold sorted by active license count</span></span>

- <span data-ttu-id="be197-165">**Počet aktivních licencí podle zákazníka** : zákazníci seřazené podle počtu aktivních licencí</span><span class="sxs-lookup"><span data-stu-id="be197-165">**Active license count by customer** : Customers sorted by active license count</span></span>

- <span data-ttu-id="be197-166">**Podrobnosti o licenční události zákazníka v posledních 90 dnech** : podrobné zobrazení událostí zákazníků, předplatných a předplatných včetně data události, názvu události, množství a změny v množství.</span><span class="sxs-lookup"><span data-stu-id="be197-166">**Customer license event details over last 90 days** : Detailed view of the customers, subscriptions, and subscription events including event date, event name, quantity, and change in quantity.</span></span>

### <a name="licenses-usage-report"></a><span data-ttu-id="be197-167">Sestava využití licencí:</span><span class="sxs-lookup"><span data-stu-id="be197-167">Licenses Usage report:</span></span>

- <span data-ttu-id="be197-168">**Licence přiřazené produktem** : prodávané produkty seřazené podle počtu přiřazení licencí</span><span class="sxs-lookup"><span data-stu-id="be197-168">**Licenses assigned by product** : Products sold sorted by license assignment count</span></span>

- <span data-ttu-id="be197-169">**Licence používané produktem** : produkty prodávané seřazené podle počtu využití licencí</span><span class="sxs-lookup"><span data-stu-id="be197-169">**Licenses in use by product** : Products sold sorted by license usage count</span></span>

- <span data-ttu-id="be197-170">**Zákaznická distribuce přiřazených licencí** :% rozdělení celkových zákazníků v intervalech, které jsou v intervalech 20% v rozsahu podle přiřazení licencí%</span><span class="sxs-lookup"><span data-stu-id="be197-170">**Customer distribution of licenses assigned** : % distribution of total customers broken in buckets of 20% range by license assignment %</span></span>

- <span data-ttu-id="be197-171">**Zákaznická distribuce licencí, které se používají** :% rozdělení celkových zákazníků v intervalech po 20% rozsahu podle využití licencí%</span><span class="sxs-lookup"><span data-stu-id="be197-171">**Customer distribution of licenses in use** : % distribution of total customers broken in buckets of 20% range by license usage %</span></span>

- <span data-ttu-id="be197-172">**Licence přiřazené zákazníkem** : podrobné zobrazení prodaných licencí a licencí přiřazených zákazníky a produkty</span><span class="sxs-lookup"><span data-stu-id="be197-172">**Licenses assigned by customer** : Detailed view of licenses sold and licenses assigned by customers and products</span></span>

- <span data-ttu-id="be197-173">**Licence používané zákazníkem** : podrobné zobrazení prodaných licencí a licencí používaných zákazníky a produkty</span><span class="sxs-lookup"><span data-stu-id="be197-173">**Licenses in use by customer** : Detailed view of licenses sold and licenses in use by customers and products</span></span>

### <a name="azure-insights-report"></a><span data-ttu-id="be197-174">Sestava Azure Insights:</span><span class="sxs-lookup"><span data-stu-id="be197-174">Azure Insights report:</span></span>

- <span data-ttu-id="be197-175">**Zákazníci na základě využití za posledních 12 měsíců** : Měsíční trend nových zákazníků založených na používání a změny v rámci využívání, které jsou v průběhu posledních 12 měsíců shrnuté měsíčně.</span><span class="sxs-lookup"><span data-stu-id="be197-175">**Usage-based customers over last 12 months** : Month over month trend of new usage-based customers and churned usage-based customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="be197-176">**Předplatná založená na využití za posledních 12 měsíců** : Měsíční trend nových předplatných založených na využití a změny předplatných na základě využití, které jsou v období posledních 12 měsíců shrnuté po měsících.</span><span class="sxs-lookup"><span data-stu-id="be197-176">**Usage-based subscriptions over last 12 months** : Month over month trend of new usage-based subscriptions and churned usage-based subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="be197-177">**Odhadované náklady na využití od zákazníka za posledních 60 dní** : zákazníci na základě využití setříděni podle odhadované částky za použití předběžného daňového dolaru v období posledních 60 dnů.</span><span class="sxs-lookup"><span data-stu-id="be197-177">**Estimated cost of usage by customer over last 60 days** : Usage-based customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span> <span data-ttu-id="be197-178">Tento stav indikuje zákazníky s nejvyšším využitím, který přináší nejvíc výnosů.</span><span class="sxs-lookup"><span data-stu-id="be197-178">This status indicates top usage-based customers bringing most revenue</span></span>

- <span data-ttu-id="be197-179">**Odhadované náklady na využití podle kategorie za posledních 60 dní** : kategorie měřičů předplatných založených na použití seřazené podle odhadované částky předběžného daňového dolaru v období posledních 60 dnů.</span><span class="sxs-lookup"><span data-stu-id="be197-179">**Estimated cost of usage by category over last 60 days** : Meter categories of usage-based subscriptions sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="be197-180">**Odhadované náklady na využití podle předplatného v posledních 60 dnech** : předplatná na základě využití odhadovaná částka za fakturační dolary, která se agreguje za období posledních 60 dnů.</span><span class="sxs-lookup"><span data-stu-id="be197-180">**Estimated cost of usage by subscription over last 60 days** : Usage-based subscriptions by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="be197-181">**Odhadované náklady na využití na zákazníky podle rozpočtu útraty** : zákazníci, kteří se seřadili podle procenta jejich aktuálního využití, překračuje prahovou hodnotu (100%).</span><span class="sxs-lookup"><span data-stu-id="be197-181">**Customer estimated usage cost by spending budget** : Customers sorted by percentage of their current usage spending budget exceeding threshold (100%).</span></span>

### <a name="azure-resource-usage-report"></a><span data-ttu-id="be197-182">Sestava využití prostředků Azure:</span><span class="sxs-lookup"><span data-stu-id="be197-182">Azure Resource Usage report:</span></span>

- <span data-ttu-id="be197-183">**Využití prostředků Azure podle dne pro vybrané období** : denní jednotky spotřeby pro každý měřený prostředek v každém předplatném na základě využití pro vybrané období během posledních 60 dnů.</span><span class="sxs-lookup"><span data-stu-id="be197-183">**Usage of Azure resources by day for selected period** : Daily consumption units for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span>

- <span data-ttu-id="be197-184">**Odhadované náklady na využití prostředků Azure pro vybrané období** : Odhadované náklady na základě karty s nejnovějšími sazbami pro každý měřený prostředek v každém předplatném na základě využití pro vybrané období během posledních 60 dnů.</span><span class="sxs-lookup"><span data-stu-id="be197-184">**Estimated usage cost of Azure resources for selected period** : Estimated cost based on latest rate card for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="be197-185">Další kroky</span><span class="sxs-lookup"><span data-stu-id="be197-185">Next steps</span></span>

- [<span data-ttu-id="be197-186">Přehled služby partner Center Analytics pro aplikaci Power BI</span><span class="sxs-lookup"><span data-stu-id="be197-186">Partner Center Analytics for Power BI app overview</span></span>](power-bi-app-for-direct-partners.md)

- [<span data-ttu-id="be197-187">Instalace a vyzkoušení aplikace Analýzy v Partnerském centru pro Microsoft Power BI</span><span class="sxs-lookup"><span data-stu-id="be197-187">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-install.md)
