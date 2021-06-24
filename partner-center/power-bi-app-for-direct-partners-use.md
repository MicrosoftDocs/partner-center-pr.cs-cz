---
title: Použití analýzy partnerského centra pro Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Naučte se, jak zobrazit obchodní data pomocí aplikace Datacenter Center Analytics pro Power BI (pro přímé partnery v programu Cloud Solution Provider (CSP)).
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 95eb018a3284d2de98c0ce6a9cd0ce6299d5571a
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/24/2021
ms.locfileid: "112564977"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="ecc98-103">Zobrazení obchodních dat pomocí aplikace Datacenter Center Analytics pro Microsoft Power BI</span><span class="sxs-lookup"><span data-stu-id="ecc98-103">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>



<span data-ttu-id="ecc98-104">**Příslušné role**: globální správce | Správce správy uživatelů | Prodejní agent | Agent správce</span><span class="sxs-lookup"><span data-stu-id="ecc98-104">**Appropriate roles**: Global admin | User management admin | Sales agent | Admin agent</span></span>

## <a name="view-your-business-data"></a><span data-ttu-id="ecc98-105">Zobrazení obchodních dat</span><span class="sxs-lookup"><span data-stu-id="ecc98-105">View your business data</span></span>

<span data-ttu-id="ecc98-106">Získejte vizuální reprezentaci vašich obchodních dat pomocí aplikace partnera Center Analytics pro Microsoft Power BI, včetně těchto:</span><span class="sxs-lookup"><span data-stu-id="ecc98-106">Get a visual representation of your business data with the Partner Center Analytics app for Microsoft Power BI, including:</span></span>

- <span data-ttu-id="ecc98-107">Růst zákaznické základny, předplatných a licencí</span><span class="sxs-lookup"><span data-stu-id="ecc98-107">Growth of your customer base, subscriptions, and licenses</span></span>

- <span data-ttu-id="ecc98-108">Využití produktů Office 365, Microsoft Dynamics a Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="ecc98-108">Usage of Office 365, Microsoft Dynamics, and Microsoft Azure products</span></span>

- <span data-ttu-id="ecc98-109">Denní spotřeba jednotek pro každý měřený prostředek v každém předplatném Azure za posledních 60 dní</span><span class="sxs-lookup"><span data-stu-id="ecc98-109">Daily consumption units for each metered resource in each Azure subscription for the last 60 days</span></span>

- <span data-ttu-id="ecc98-110">Odhadované náklady (na základě karty s nejnovějšími sazbami)</span><span class="sxs-lookup"><span data-stu-id="ecc98-110">Estimated cost (based on latest rate card)</span></span>

- <span data-ttu-id="ecc98-111">Možnost exportovat datové sady a vytvářet vlastní sestavy, včetně jednotlivých zákazníků.</span><span class="sxs-lookup"><span data-stu-id="ecc98-111">Ability to export datasets and create custom reports, including per customer.</span></span>

### <a name="about-the-partner-center-analytics-app-preview-release"></a><span data-ttu-id="ecc98-112">Informace o verzi Preview partnerského centra pro aplikaci Analytics</span><span class="sxs-lookup"><span data-stu-id="ecc98-112">About the Partner Center Analytics app preview release</span></span>

- <span data-ttu-id="ecc98-113">Tato aplikace je určena pouze pro přímé partnery v programu Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="ecc98-113">This app is for direct partners in the Cloud Solution Provider (CSP) program only.</span></span> <span data-ttu-id="ecc98-114">Jiní partneři v CSP (například nepřímo prodejci) se nebudou moci přihlásit.</span><span class="sxs-lookup"><span data-stu-id="ecc98-114">Other partners in CSP (indirect resellers, for example) will not be able to sign in.</span></span>

- <span data-ttu-id="ecc98-115">Všechny odhadované náklady jsou platby před zdaněním a fakturaci a nejsou právně závazné.</span><span class="sxs-lookup"><span data-stu-id="ecc98-115">Any estimated costs are pre-tax billing / invoice data, and are not legally binding.</span></span> <span data-ttu-id="ecc98-116">Odhadované náklady se mají použít jenom pro data Insights.</span><span class="sxs-lookup"><span data-stu-id="ecc98-116">Estimated costs are meant to be used for data insights only.</span></span>

- <span data-ttu-id="ecc98-117">Informace o zákaznících jsou založené na předplatných.</span><span class="sxs-lookup"><span data-stu-id="ecc98-117">Customer information is based on subscriptions.</span></span> <span data-ttu-id="ecc98-118">Zákazníci, u kterých jste nedávno vytvořili účty pro, ale kteří ještě nemají předplatné, nejsou zahrnuti do počtu.</span><span class="sxs-lookup"><span data-stu-id="ecc98-118">Any customers that you've recently created accounts for, but who don't yet have subscriptions, aren't included in counts.</span></span>

- <span data-ttu-id="ecc98-119">Odhadované náklady vycházejí z karty nejnovějších sazeb, která vychází z cen CSP.</span><span class="sxs-lookup"><span data-stu-id="ecc98-119">Estimated cost is based on latest rate card, which is based on CSP pricing.</span></span>

- <span data-ttu-id="ecc98-120">Dny jsou dny kalendáře.</span><span class="sxs-lookup"><span data-stu-id="ecc98-120">Days are calendar days.</span></span>

### <a name="business-insights-report"></a><span data-ttu-id="ecc98-121">Sestava obchodních přehledů</span><span class="sxs-lookup"><span data-stu-id="ecc98-121">Business Insights report</span></span>

- <span data-ttu-id="ecc98-122">**Klienti zákazníka**: počet různých tenantů Azure Active Directory (Azure AD) pro zákazníky, kteří si zakoupili předplatná</span><span class="sxs-lookup"><span data-stu-id="ecc98-122">**Customer tenants**: Number of distinct Azure Active Directory (Azure AD) tenants of customers that have purchased subscriptions</span></span>

- <span data-ttu-id="ecc98-123">**Novinka (posledních 30 dnů)**: noví zákazníci, kteří si nakupují aspoň jedno předplatné za posledních 30 dní</span><span class="sxs-lookup"><span data-stu-id="ecc98-123">**New (last 30 days)**: New customers purchasing at least one subscription in last 30 days</span></span>

- <span data-ttu-id="ecc98-124">Změny **(posledních 30 dnů)**: zákazníci bez všech předplatných "aktivní", "v odkladu" nebo "zakázáno".</span><span class="sxs-lookup"><span data-stu-id="ecc98-124">**Churn (last 30 days)**: Customers without any “active", “in grace" or “disabled" subscriptions</span></span>

- <span data-ttu-id="ecc98-125">**Novinka (posledních 24 hodin)**: noví zákazníci nakupují aspoň jedno předplatné za posledních 24 hodin</span><span class="sxs-lookup"><span data-stu-id="ecc98-125">**New (last 24 hours)**: New customers purchasing at least one subscription in last 24 hours</span></span>

- <span data-ttu-id="ecc98-126">**Odhadované měsíční náklady za posledních 12 měsíců**: Měsíční trend odhadované částky za měsíc v měsíci, který je v období posledních 12 měsíců agregovaný měsíčně.</span><span class="sxs-lookup"><span data-stu-id="ecc98-126">**Estimated monthly cost over last 12 months**: Month over month trend of estimated pre-tax invoice dollar amount aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="ecc98-127">**Odhadované náklady podle produktu za posledních 12 měsíců**: produkty prodávané podle odhadované částky pro fakturační dolary, které jsou shrnuty v období posledních 12 měsíců.</span><span class="sxs-lookup"><span data-stu-id="ecc98-127">**Estimated cost by product over last 12 months**: Products sold sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="ecc98-128">Tento stav označuje nejdůležitější produkty, které přináší většinu výnosů.</span><span class="sxs-lookup"><span data-stu-id="ecc98-128">This status indicates top products bringing most revenue.</span></span>

- <span data-ttu-id="ecc98-129">**Zákazníci za posledních 12 měsíců**: trend za měsíc měsíčně nových zákazníků a změny, které se zákazníkům v období posledních 12 měsíců agreguje měsíčně</span><span class="sxs-lookup"><span data-stu-id="ecc98-129">**Customers over last 12 months**: Month over month trend of new customers and churn customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="ecc98-130">**Odhadované náklady podle zákazníka za posledních 12 měsíců**: zákazníci setříděni podle odhadované částky předběžného daňového dolaru shrnuté v období posledních 12 měsíců.</span><span class="sxs-lookup"><span data-stu-id="ecc98-130">**Estimated cost by customer over last 12 months**: Customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="ecc98-131">Tento stav označuje nejdůležitější zákazníky, kteří přinášejí většinu výnosů.</span><span class="sxs-lookup"><span data-stu-id="ecc98-131">This status indicates top customers bringing most revenue.</span></span>

- <span data-ttu-id="ecc98-132">**Počet zákazníků podle produktu**: produktů prodávaných seřazené podle přidružených zákazníků.</span><span class="sxs-lookup"><span data-stu-id="ecc98-132">**Customer count by product**: Products sold sorted by associated customers.</span></span> <span data-ttu-id="ecc98-133">Tento stav označuje nejdůležitější produkty prodávané většině zákazníků.</span><span class="sxs-lookup"><span data-stu-id="ecc98-133">This status indicates top products sold to most customers.</span></span>

### <a name="subscription-insights-report"></a><span data-ttu-id="ecc98-134">Sestava přehledů předplatných</span><span class="sxs-lookup"><span data-stu-id="ecc98-134">Subscription Insights report</span></span>

- <span data-ttu-id="ecc98-135">**Stav předplatného**:</span><span class="sxs-lookup"><span data-stu-id="ecc98-135">**Subscription status**:</span></span>

- <span data-ttu-id="ecc98-136">Aktivní: předplatná, která patří do stavu "aktivní" nebo "ve lhůtě".</span><span class="sxs-lookup"><span data-stu-id="ecc98-136">Active: Subscriptions belonging to either “active" or “in grace" state</span></span>

  - <span data-ttu-id="ecc98-137">Pozastaveno: odběry patřící do stavu zakázáno</span><span class="sxs-lookup"><span data-stu-id="ecc98-137">Suspended: Subscriptions belonging to “disabled" state</span></span>

  - <span data-ttu-id="ecc98-138">Nezřízeno: odběry patřící do stavu "de-provisioned" nebo "vypršela platnost"</span><span class="sxs-lookup"><span data-stu-id="ecc98-138">De-provisioned: Subscriptions belonging to “de-provisioned" or “expired" status</span></span>

- <span data-ttu-id="ecc98-139">**Stav vypršení platnosti**:</span><span class="sxs-lookup"><span data-stu-id="ecc98-139">**Expiry status**:</span></span>

  - <span data-ttu-id="ecc98-140">Vypršela platnost předplatných, jejichž platnost již vypršela (kde koncové datum předplatného je v minulosti).</span><span class="sxs-lookup"><span data-stu-id="ecc98-140">Expired: Subscriptions that have already expired (where subscription end date is in past)</span></span>

  - <span data-ttu-id="ecc98-141">Vypršení platnosti po 30 dnech: předplatná, jejichž platnost vyprší po 30 dnech (kde koncové datum předplatného je po následujících 30 dnech)</span><span class="sxs-lookup"><span data-stu-id="ecc98-141">Expiring after 30 days: Subscriptions that will expire after 30 days (where subscription end date is after next 30 days)</span></span>

  - <span data-ttu-id="ecc98-142">Vypršení platnosti během 30 dnů: předplatná, jejichž platnost vyprší během následujících 30 dnů (kde datum ukončení předplatného spadá do rozmezí dnešních a dalších 30 dnů)</span><span class="sxs-lookup"><span data-stu-id="ecc98-142">Expiring in 30 days: Subscriptions that will expire within next 30 days (where subscription end date is between today and next 30 days)</span></span>

- <span data-ttu-id="ecc98-143">**Celkový počet předplatných**: předplatná ve stavu "aktivní", "ve lhůtě" nebo "zakázáno"</span><span class="sxs-lookup"><span data-stu-id="ecc98-143">**Total subscriptions**: Subscriptions in “active," “in grace" or “disabled" status</span></span>

- <span data-ttu-id="ecc98-144">**Novinka (posledních 30 dnů)**: nové předplatné zakoupené zákazníky během posledních 30 dnů</span><span class="sxs-lookup"><span data-stu-id="ecc98-144">**New (last 30 days)**: New subscriptions purchased by customers within last 30 days</span></span>

- <span data-ttu-id="ecc98-145">**Novinka (posledních 24 hodin)**: nové předplatné zakoupené zákazníky během posledních 24 hodin</span><span class="sxs-lookup"><span data-stu-id="ecc98-145">**New (last 24 hours)**: New subscriptions purchased by customers within last 24 hours</span></span>

- <span data-ttu-id="ecc98-146">**Platnost vyprší za 30 dní**: předplatná, jejichž platnost vyprší během následujících 30 dnů</span><span class="sxs-lookup"><span data-stu-id="ecc98-146">**Expiring in 30 days**: Subscriptions that will expire within next 30 days</span></span>

- <span data-ttu-id="ecc98-147">Změny **(posledních 30 dnů)**: předplatná, která byla během posledních 30 dnů zrušena nebo pozastavena (zakázána)</span><span class="sxs-lookup"><span data-stu-id="ecc98-147">**Churn (last 30 days)**: Subscriptions that have been de-provisioned or suspended (disabled) within last 30 days</span></span>

- <span data-ttu-id="ecc98-148">**Distribuce podle typů předplatného**:% distribuce celkových předplatných podle licencí a typu předplatného založeného na použití</span><span class="sxs-lookup"><span data-stu-id="ecc98-148">**Distribution by subscription types**: % distribution of total subscriptions by License based and usage-based subscription type</span></span>

- <span data-ttu-id="ecc98-149">**Počet aktivních předplatných podle produktu**: produkty prodávané seřazené podle aktivního počtu předplatných</span><span class="sxs-lookup"><span data-stu-id="ecc98-149">**Active subscription count by product**: Products sold sorted by active subscriptions count</span></span>

- <span data-ttu-id="ecc98-150">**Předplatná za posledních 12 měsíců**: trend za měsíc měsíčně nových předplatných a všech předplatných, které jsou v období posledních 12 měsíců agregované měsíčně.</span><span class="sxs-lookup"><span data-stu-id="ecc98-150">**Subscriptions over last 12 months**: Month over month trend of new subscriptions and churn subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="ecc98-151">**Podrobnosti o předplatném zákazníka**: podrobné zobrazení zákazníků, předplatných a nabídek</span><span class="sxs-lookup"><span data-stu-id="ecc98-151">**Customer subscription details**: Detailed view of the customers, subscriptions, and offers</span></span>

### <a name="license-insights-report"></a><span data-ttu-id="ecc98-152">Sestava o licenci License Insights:</span><span class="sxs-lookup"><span data-stu-id="ecc98-152">License Insights report:</span></span>

- <span data-ttu-id="ecc98-153">**Celkem licencí**: celkový počet licencí agregovaných napříč všemi předplatnými na základě licencí</span><span class="sxs-lookup"><span data-stu-id="ecc98-153">**Total licenses**: Total number of licenses aggregated across all license-based subscriptions</span></span>

- <span data-ttu-id="ecc98-154">**Novinka (posledních 30 dnů)**: Přidání licence během posledních 30 dnů</span><span class="sxs-lookup"><span data-stu-id="ecc98-154">**New (last 30 days)**: License addition within last 30 days</span></span>

- <span data-ttu-id="ecc98-155">Změny **(posledních 30 dnů)**: snížení počtu licencí během posledních 30 dnů</span><span class="sxs-lookup"><span data-stu-id="ecc98-155">**Churn (last 30 days)**: License reduction within last 30 days</span></span>

- <span data-ttu-id="ecc98-156">**Novinka (posledních 24 hodin)**: Přidání licence během posledních 24 hodin</span><span class="sxs-lookup"><span data-stu-id="ecc98-156">**New (last 24 hours)**: License addition within last 24 hours</span></span>

- <span data-ttu-id="ecc98-157">**Licence v posledních 90 dnech**: Měsíční trend přidaných licencí a jejich snížení na měsíc za období posledních 90 dnů</span><span class="sxs-lookup"><span data-stu-id="ecc98-157">**Licenses over last 90 days**: Month over month trend of license additions and reductions aggregated monthly over the period of last 90 days</span></span>

- <span data-ttu-id="ecc98-158">**Počet aktivních licencí podle produktu**: produkty prodávané seřazené podle počtu aktivních licencí</span><span class="sxs-lookup"><span data-stu-id="ecc98-158">**Active license count by product**: Products sold sorted by active license count</span></span>

- <span data-ttu-id="ecc98-159">**Počet aktivních licencí podle zákazníka**: zákazníci seřazené podle počtu aktivních licencí</span><span class="sxs-lookup"><span data-stu-id="ecc98-159">**Active license count by customer**: Customers sorted by active license count</span></span>

- <span data-ttu-id="ecc98-160">**Podrobnosti o licenční události zákazníka v posledních 90 dnech**: podrobné zobrazení událostí zákazníků, předplatných a předplatných včetně data události, názvu události, množství a změny v množství.</span><span class="sxs-lookup"><span data-stu-id="ecc98-160">**Customer license event details over last 90 days**: Detailed view of the customers, subscriptions, and subscription events including event date, event name, quantity, and change in quantity.</span></span>

### <a name="licenses-usage-report"></a><span data-ttu-id="ecc98-161">Sestava využití licencí:</span><span class="sxs-lookup"><span data-stu-id="ecc98-161">Licenses Usage report:</span></span>

- <span data-ttu-id="ecc98-162">**Licence přiřazené produktem**: prodávané produkty seřazené podle počtu přiřazení licencí</span><span class="sxs-lookup"><span data-stu-id="ecc98-162">**Licenses assigned by product**: Products sold sorted by license assignment count</span></span>

- <span data-ttu-id="ecc98-163">**Licence používané produktem**: produkty prodávané seřazené podle počtu využití licencí</span><span class="sxs-lookup"><span data-stu-id="ecc98-163">**Licenses in use by product**: Products sold sorted by license usage count</span></span>

- <span data-ttu-id="ecc98-164">**Zákaznická distribuce přiřazených licencí**:% rozdělení celkových zákazníků v intervalech, které jsou v intervalech 20% v rozsahu podle přiřazení licencí%</span><span class="sxs-lookup"><span data-stu-id="ecc98-164">**Customer distribution of licenses assigned**: % distribution of total customers broken in buckets of 20% range by license assignment %</span></span>

- <span data-ttu-id="ecc98-165">**Zákaznická distribuce licencí, které se používají**:% rozdělení celkových zákazníků v intervalech po 20% rozsahu podle využití licencí%</span><span class="sxs-lookup"><span data-stu-id="ecc98-165">**Customer distribution of licenses in use**: % distribution of total customers broken in buckets of 20% range by license usage %</span></span>

- <span data-ttu-id="ecc98-166">**Licence přiřazené zákazníkem**: podrobné zobrazení prodaných licencí a licencí přiřazených zákazníky a produkty</span><span class="sxs-lookup"><span data-stu-id="ecc98-166">**Licenses assigned by customer**: Detailed view of licenses sold and licenses assigned by customers and products</span></span>

- <span data-ttu-id="ecc98-167">**Licence používané zákazníkem**: podrobné zobrazení prodaných licencí a licencí používaných zákazníky a produkty</span><span class="sxs-lookup"><span data-stu-id="ecc98-167">**Licenses in use by customer**: Detailed view of licenses sold and licenses in use by customers and products</span></span>

### <a name="azure-insights-report"></a><span data-ttu-id="ecc98-168">Sestava Azure Insights:</span><span class="sxs-lookup"><span data-stu-id="ecc98-168">Azure Insights report:</span></span>

- <span data-ttu-id="ecc98-169">**Zákazníci na základě využití za posledních 12 měsíců**: Měsíční trend nových zákazníků založených na používání a změny v rámci využívání, které jsou v průběhu posledních 12 měsíců shrnuté měsíčně.</span><span class="sxs-lookup"><span data-stu-id="ecc98-169">**Usage-based customers over last 12 months**: Month over month trend of new usage-based customers and churned usage-based customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="ecc98-170">**Předplatná založená na využití za posledních 12 měsíců**: Měsíční trend nových předplatných založených na využití a změny předplatných na základě využití, které jsou v období posledních 12 měsíců shrnuté po měsících.</span><span class="sxs-lookup"><span data-stu-id="ecc98-170">**Usage-based subscriptions over last 12 months**: Month over month trend of new usage-based subscriptions and churned usage-based subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="ecc98-171">**Odhadované náklady na využití od zákazníka za posledních 60 dní**: zákazníci na základě využití setříděni podle odhadované částky za použití předběžného daňového dolaru v období posledních 60 dnů.</span><span class="sxs-lookup"><span data-stu-id="ecc98-171">**Estimated cost of usage by customer over last 60 days**: Usage-based customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span> <span data-ttu-id="ecc98-172">Tento stav indikuje zákazníky s nejvyšším využitím, který přináší nejvíc výnosů.</span><span class="sxs-lookup"><span data-stu-id="ecc98-172">This status indicates top usage-based customers bringing most revenue</span></span>

- <span data-ttu-id="ecc98-173">**Odhadované náklady na využití podle kategorie za posledních 60 dní**: kategorie měřičů předplatných založených na použití seřazené podle odhadované částky předběžného daňového dolaru v období posledních 60 dnů.</span><span class="sxs-lookup"><span data-stu-id="ecc98-173">**Estimated cost of usage by category over last 60 days**: Meter categories of usage-based subscriptions sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="ecc98-174">**Odhadované náklady na využití podle předplatného v posledních 60 dnech**: předplatná na základě využití odhadovaná částka za fakturační dolary, která se agreguje za období posledních 60 dnů.</span><span class="sxs-lookup"><span data-stu-id="ecc98-174">**Estimated cost of usage by subscription over last 60 days**: Usage-based subscriptions by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="ecc98-175">**Odhadované náklady na využití na zákazníky podle rozpočtu útraty**: zákazníci, kteří se seřadili podle procenta jejich aktuálního využití, překračuje prahovou hodnotu (100%).</span><span class="sxs-lookup"><span data-stu-id="ecc98-175">**Customer estimated usage cost by spending budget**: Customers sorted by percentage of their current usage spending budget exceeding threshold (100%).</span></span>

### <a name="azure-resource-usage-report"></a><span data-ttu-id="ecc98-176">Sestava využití prostředků Azure:</span><span class="sxs-lookup"><span data-stu-id="ecc98-176">Azure Resource Usage report:</span></span>

- <span data-ttu-id="ecc98-177">**Využití prostředků Azure podle dne pro vybrané období**: denní jednotky spotřeby pro každý měřený prostředek v každém předplatném na základě využití pro vybrané období během posledních 60 dnů.</span><span class="sxs-lookup"><span data-stu-id="ecc98-177">**Usage of Azure resources by day for selected period**: Daily consumption units for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span>

- <span data-ttu-id="ecc98-178">**Odhadované náklady na využití prostředků Azure pro vybrané období**: Odhadované náklady na základě karty s nejnovějšími sazbami pro každý měřený prostředek v každém předplatném na základě využití pro vybrané období během posledních 60 dnů.</span><span class="sxs-lookup"><span data-stu-id="ecc98-178">**Estimated usage cost of Azure resources for selected period**: Estimated cost based on latest rate card for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="ecc98-179">Další kroky</span><span class="sxs-lookup"><span data-stu-id="ecc98-179">Next steps</span></span>

- [<span data-ttu-id="ecc98-180">Přehled služby partner Center Analytics pro aplikaci Power BI</span><span class="sxs-lookup"><span data-stu-id="ecc98-180">Partner Center Analytics for Power BI app overview</span></span>](power-bi-app-for-direct-partners.md)

- [<span data-ttu-id="ecc98-181">Instalace a vyzkoušení aplikace Analýzy v Partnerském centru pro Microsoft Power BI</span><span class="sxs-lookup"><span data-stu-id="ecc98-181">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-install.md)
