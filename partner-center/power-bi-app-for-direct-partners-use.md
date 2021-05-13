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
ms.openlocfilehash: 96fe57f6e89928a69051c2e201c444882500b844
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855025"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="7990c-103">Zobrazení obchodních dat pomocí aplikace Datacenter Center Analytics pro Microsoft Power BI</span><span class="sxs-lookup"><span data-stu-id="7990c-103">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>



<span data-ttu-id="7990c-104">**Příslušné role**: globální správce | Správce správy uživatelů | Prodejní agent | Agent správce</span><span class="sxs-lookup"><span data-stu-id="7990c-104">**Appropriate roles**: Global admin | User management admin | Sales agent | Admin agent</span></span>

## <a name="view-your-business-data"></a><span data-ttu-id="7990c-105">Zobrazení obchodních dat</span><span class="sxs-lookup"><span data-stu-id="7990c-105">View your business data</span></span>

<span data-ttu-id="7990c-106">Získejte vizuální reprezentaci vašich obchodních dat pomocí aplikace Datacenter Center Analytics pro Power BI, včetně těchto:</span><span class="sxs-lookup"><span data-stu-id="7990c-106">Get a visual representation of your business data with the Partner Center Analytics app for Power BI, including:</span></span>

- <span data-ttu-id="7990c-107">Růst zákaznické základny, předplatných a licencí</span><span class="sxs-lookup"><span data-stu-id="7990c-107">Growth of your customer base, subscriptions, and licenses</span></span>

- <span data-ttu-id="7990c-108">Využití produktů Office 365, Microsoft Dynamics a Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="7990c-108">Usage of Office 365, Microsoft Dynamics, and Microsoft Azure products</span></span>

- <span data-ttu-id="7990c-109">Denní spotřeba jednotek pro každý měřený prostředek v každém předplatném Azure za posledních 60 dní</span><span class="sxs-lookup"><span data-stu-id="7990c-109">Daily consumption units for each metered resource in each Azure subscription for the last 60 days</span></span>

- <span data-ttu-id="7990c-110">Odhadované náklady (na základě karty s nejnovějšími sazbami)</span><span class="sxs-lookup"><span data-stu-id="7990c-110">Estimated cost (based on latest rate card)</span></span>

- <span data-ttu-id="7990c-111">Možnost exportovat datové sady a vytvářet vlastní sestavy, včetně jednotlivých zákazníků.</span><span class="sxs-lookup"><span data-stu-id="7990c-111">Ability to export datasets and create custom reports, including per customer.</span></span>

### <a name="about-the-partner-center-analytics-app-preview-release"></a><span data-ttu-id="7990c-112">Informace o verzi Preview partnerského centra pro aplikaci Analytics</span><span class="sxs-lookup"><span data-stu-id="7990c-112">About the Partner Center Analytics app preview release</span></span>

- <span data-ttu-id="7990c-113">Tato aplikace je určena pouze pro přímé partnery v programu Cloud Solution Provider.</span><span class="sxs-lookup"><span data-stu-id="7990c-113">This app is for direct partners in the Cloud Solution Provider program only.</span></span> <span data-ttu-id="7990c-114">Jiní partneři v CSP (například nepřímo prodejci) se nebudou moci přihlásit.</span><span class="sxs-lookup"><span data-stu-id="7990c-114">Other partners in CSP (indirect resellers, for example) will not be able to sign in.</span></span>

- <span data-ttu-id="7990c-115">Všechny odhadované náklady jsou platby před zdaněním a fakturaci a nejsou právně závazné.</span><span class="sxs-lookup"><span data-stu-id="7990c-115">Any estimated costs are pre-tax billing / invoice data, and are not legally binding.</span></span> <span data-ttu-id="7990c-116">Odhadované náklady se mají použít jenom pro data Insights.</span><span class="sxs-lookup"><span data-stu-id="7990c-116">Estimated costs are meant to be used for data insights only.</span></span>

- <span data-ttu-id="7990c-117">Informace o zákaznících jsou založené na předplatných.</span><span class="sxs-lookup"><span data-stu-id="7990c-117">Customer information is based on subscriptions.</span></span> <span data-ttu-id="7990c-118">Zákazníci, u kterých jste nedávno vytvořili účty pro, ale kteří ještě nemají předplatné, nejsou zahrnuti do počtu.</span><span class="sxs-lookup"><span data-stu-id="7990c-118">Any customers that you've recently created accounts for, but who don't yet have subscriptions, aren't included in counts.</span></span>

- <span data-ttu-id="7990c-119">Odhadované náklady vycházejí z karty nejnovějších sazeb, která vychází z cen CSP.</span><span class="sxs-lookup"><span data-stu-id="7990c-119">Estimated cost is based on latest rate card, which is based on CSP pricing.</span></span>

- <span data-ttu-id="7990c-120">Dny jsou dny kalendáře.</span><span class="sxs-lookup"><span data-stu-id="7990c-120">Days are calendar days.</span></span>

### <a name="business-insights-report"></a><span data-ttu-id="7990c-121">Sestava Business Insights</span><span class="sxs-lookup"><span data-stu-id="7990c-121">Business Insights report</span></span>

- <span data-ttu-id="7990c-122">**Tenanti zákazníků:** Počet různých tenantů Azure AD zákazníků, kteří si zakoupili předplatná</span><span class="sxs-lookup"><span data-stu-id="7990c-122">**Customer tenants**: Number of distinct Azure AD tenants of customers that have purchased subscriptions</span></span>

- <span data-ttu-id="7990c-123">**Nové (posledních 30 dnů):** Noví zákazníci kupující alespoň jedno předplatné za posledních 30 dnů</span><span class="sxs-lookup"><span data-stu-id="7990c-123">**New (last 30 days)**: New customers purchasing at least one subscription in last 30 days</span></span>

- <span data-ttu-id="7990c-124">**Četnost změn (posledních 30 dnů):** Zákazníci bez jakýchkoli aktivních předplatných, předplatných s odkladem nebo zakázaných předplatných</span><span class="sxs-lookup"><span data-stu-id="7990c-124">**Churn (last 30 days)**: Customers without any “active", “in grace" or “disabled" subscriptions</span></span>

- <span data-ttu-id="7990c-125">**Nové (posledních 24 hodin):** Noví zákazníci kupující alespoň jedno předplatné za posledních 24 hodin</span><span class="sxs-lookup"><span data-stu-id="7990c-125">**New (last 24 hours)**: New customers purchasing at least one subscription in last 24 hours</span></span>

- <span data-ttu-id="7990c-126">**Odhadované měsíční náklady za posledních 12** měsíců: Trend odhadované částky faktury před zdaněním agregované měsíčně za období posledních 12 měsíců</span><span class="sxs-lookup"><span data-stu-id="7990c-126">**Estimated monthly cost over last 12 months**: Month over month trend of estimated pre-tax invoice dollar amount aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="7990c-127">**Odhadované náklady podle produktu za posledních 12** měsíců: Prodané produkty seřazené podle odhadované částky faktury před zdaněním agregované za období posledních 12 měsíců.</span><span class="sxs-lookup"><span data-stu-id="7990c-127">**Estimated cost by product over last 12 months**: Products sold sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="7990c-128">Tento stav označuje hlavní produkty, které mají největší výnosy.</span><span class="sxs-lookup"><span data-stu-id="7990c-128">This status indicates top products bringing most revenue.</span></span>

- <span data-ttu-id="7990c-129">**Zákazníci za posledních 12 měsíců:** Trend nových zákazníků po měsících a zákazníků se četností změn agregovaný měsíčně za období posledních 12 měsíců</span><span class="sxs-lookup"><span data-stu-id="7990c-129">**Customers over last 12 months**: Month over month trend of new customers and churn customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="7990c-130">**Odhadované náklady podle zákazníků za posledních 12** měsíců: Zákazníci seřazení podle odhadované částky faktury před zdaněním agregované za období posledních 12 měsíců.</span><span class="sxs-lookup"><span data-stu-id="7990c-130">**Estimated cost by customer over last 12 months**: Customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="7990c-131">Tento stav indikuje, že nejvíce výnosů mají zákazníci s nejvyššími tržby.</span><span class="sxs-lookup"><span data-stu-id="7990c-131">This status indicates top customers bringing most revenue.</span></span>

- <span data-ttu-id="7990c-132">**Počet zákazníků podle produktu:** Prodané produkty seřazené podle přidružených zákazníků.</span><span class="sxs-lookup"><span data-stu-id="7990c-132">**Customer count by product**: Products sold sorted by associated customers.</span></span> <span data-ttu-id="7990c-133">Tento stav označuje nejprodávané produkty většině zákazníků.</span><span class="sxs-lookup"><span data-stu-id="7990c-133">This status indicates top products sold to most customers.</span></span>

### <a name="subscription-insights-report"></a><span data-ttu-id="7990c-134">Sestava Přehledy předplatného</span><span class="sxs-lookup"><span data-stu-id="7990c-134">Subscription Insights report</span></span>

- <span data-ttu-id="7990c-135">**Stav předplatného:**</span><span class="sxs-lookup"><span data-stu-id="7990c-135">**Subscription status**:</span></span>

- <span data-ttu-id="7990c-136">Aktivní: Předplatná patřící do "aktivní" nebo "v odkladu"</span><span class="sxs-lookup"><span data-stu-id="7990c-136">Active: Subscriptions belonging to either “active" or “in grace" state</span></span>

  - <span data-ttu-id="7990c-137">Pozastaveno: Předplatná patřící do stavu Zakázáno</span><span class="sxs-lookup"><span data-stu-id="7990c-137">Suspended: Subscriptions belonging to “disabled" state</span></span>

  - <span data-ttu-id="7990c-138">Zrušit zřízení: Předplatná patřící do stavu "není zřízeno" nebo "vypršela jeho platnost".</span><span class="sxs-lookup"><span data-stu-id="7990c-138">De-provisioned: Subscriptions belonging to “de-provisioned" or “expired" status</span></span>

- <span data-ttu-id="7990c-139">**Stav vypršení platnosti:**</span><span class="sxs-lookup"><span data-stu-id="7990c-139">**Expiry status**:</span></span>

  - <span data-ttu-id="7990c-140">Platnost vypršela: Předplatná, jejichž platnost už vypršela (u kterých vypršelo koncové datum předplatného)</span><span class="sxs-lookup"><span data-stu-id="7990c-140">Expired: Subscriptions that have already expired (where subscription end date is in past)</span></span>

  - <span data-ttu-id="7990c-141">Vypršení platnosti po 30 dnech: předplatná, jejichž platnost vyprší po 30 dnech (kde koncové datum předplatného je po následujících 30 dnech)</span><span class="sxs-lookup"><span data-stu-id="7990c-141">Expiring after 30 days: Subscriptions that will expire after 30 days (where subscription end date is after next 30 days)</span></span>

  - <span data-ttu-id="7990c-142">Vypršení platnosti během 30 dnů: předplatná, jejichž platnost vyprší během následujících 30 dnů (kde datum ukončení předplatného spadá do rozmezí dnešních a dalších 30 dnů)</span><span class="sxs-lookup"><span data-stu-id="7990c-142">Expiring in 30 days: Subscriptions that will expire within next 30 days (where subscription end date is between today and next 30 days)</span></span>

- <span data-ttu-id="7990c-143">**Celkový počet předplatných**: předplatná ve stavu "aktivní", "ve lhůtě" nebo "zakázáno"</span><span class="sxs-lookup"><span data-stu-id="7990c-143">**Total subscriptions**: Subscriptions in “active," “in grace" or “disabled" status</span></span>

- <span data-ttu-id="7990c-144">**Novinka (posledních 30 dnů)**: nové předplatné zakoupené zákazníky během posledních 30 dnů</span><span class="sxs-lookup"><span data-stu-id="7990c-144">**New (last 30 days)**: New subscriptions purchased by customers within last 30 days</span></span>

- <span data-ttu-id="7990c-145">**Novinka (posledních 24 hodin)**: nové předplatné zakoupené zákazníky během posledních 24 hodin</span><span class="sxs-lookup"><span data-stu-id="7990c-145">**New (last 24 hours)**: New subscriptions purchased by customers within last 24 hours</span></span>

- <span data-ttu-id="7990c-146">**Platnost vyprší za 30 dní**: předplatná, jejichž platnost vyprší během následujících 30 dnů</span><span class="sxs-lookup"><span data-stu-id="7990c-146">**Expiring in 30 days**: Subscriptions that will expire within next 30 days</span></span>

- <span data-ttu-id="7990c-147">Změny **(posledních 30 dnů)**: předplatná, která byla během posledních 30 dnů zrušena nebo pozastavena (zakázána)</span><span class="sxs-lookup"><span data-stu-id="7990c-147">**Churn (last 30 days)**: Subscriptions that have been de-provisioned or Suspended (disabled) within last 30 days</span></span>

- <span data-ttu-id="7990c-148">**Distribuce podle typů předplatného**:% distribuce celkových předplatných podle licencí a typu předplatného založeného na použití</span><span class="sxs-lookup"><span data-stu-id="7990c-148">**Distribution by subscription types**: % distribution of total subscriptions by License based and usage-based subscription type</span></span>

- <span data-ttu-id="7990c-149">**Počet aktivních předplatných podle produktu**: produkty prodávané seřazené podle aktivního počtu předplatných</span><span class="sxs-lookup"><span data-stu-id="7990c-149">**Active subscription count by product**: Products sold sorted by active subscriptions count</span></span>

- <span data-ttu-id="7990c-150">**Předplatná za posledních 12 měsíců**: trend za měsíc měsíčně nových předplatných a všech předplatných, které jsou v období posledních 12 měsíců agregované měsíčně.</span><span class="sxs-lookup"><span data-stu-id="7990c-150">**Subscriptions over last 12 months**: Month over month trend of new subscriptions and churn subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="7990c-151">**Podrobnosti o předplatném zákazníka**: podrobné zobrazení zákazníků, předplatných a nabídek</span><span class="sxs-lookup"><span data-stu-id="7990c-151">**Customer subscription details**: Detailed view of the customers, subscriptions, and offers</span></span>

### <a name="license-insights-report"></a><span data-ttu-id="7990c-152">Sestava o licenci License Insights:</span><span class="sxs-lookup"><span data-stu-id="7990c-152">License Insights report:</span></span>

- <span data-ttu-id="7990c-153">**Celkem licencí**: celkový počet licencí agregovaných napříč všemi předplatnými na základě licencí</span><span class="sxs-lookup"><span data-stu-id="7990c-153">**Total licenses**: Total number of licenses aggregated across all license-based subscriptions</span></span>

- <span data-ttu-id="7990c-154">**Novinka (posledních 30 dnů)**: Přidání licence během posledních 30 dnů</span><span class="sxs-lookup"><span data-stu-id="7990c-154">**New (last 30 days)**: License addition within last 30 days</span></span>

- <span data-ttu-id="7990c-155">Změny **(posledních 30 dnů)**: snížení počtu licencí během posledních 30 dnů</span><span class="sxs-lookup"><span data-stu-id="7990c-155">**Churn (last 30 days)**: License reduction within last 30 days</span></span>

- <span data-ttu-id="7990c-156">**Novinka (posledních 24 hodin)**: Přidání licence během posledních 24 hodin</span><span class="sxs-lookup"><span data-stu-id="7990c-156">**New (last 24 hours)**: License addition within last 24 hours</span></span>

- <span data-ttu-id="7990c-157">**Licence v posledních 90 dnech**: Měsíční trend přidaných licencí a jejich snížení na měsíc za období posledních 90 dnů</span><span class="sxs-lookup"><span data-stu-id="7990c-157">**Licenses over last 90 days**: Month over month trend of license additions and reductions aggregated monthly over the period of last 90 days</span></span>

- <span data-ttu-id="7990c-158">**Počet aktivních licencí podle produktu**: produkty prodávané seřazené podle počtu aktivních licencí</span><span class="sxs-lookup"><span data-stu-id="7990c-158">**Active license count by product**: Products sold sorted by active license count</span></span>

- <span data-ttu-id="7990c-159">**Počet aktivních licencí podle zákazníka**: zákazníci seřazené podle počtu aktivních licencí</span><span class="sxs-lookup"><span data-stu-id="7990c-159">**Active license count by customer**: Customers sorted by active license count</span></span>

- <span data-ttu-id="7990c-160">Podrobnosti o události zákaznické licence za **posledních 90** dnů: Podrobné zobrazení událostí zákazníků, předplatných a odběrů, včetně data události, názvu události, množství a změny množství.</span><span class="sxs-lookup"><span data-stu-id="7990c-160">**Customer license event details over last 90 days**: Detailed view of the customers, subscriptions, and subscription events including event date, event name, quantity, and change in quantity.</span></span>

### <a name="licenses-usage-report"></a><span data-ttu-id="7990c-161">Sestava využití licencí:</span><span class="sxs-lookup"><span data-stu-id="7990c-161">Licenses Usage report:</span></span>

- <span data-ttu-id="7990c-162">**Licence přiřazené podle produktu:** Prodané produkty seřazené podle počtu přiřazení licencí</span><span class="sxs-lookup"><span data-stu-id="7990c-162">**Licenses assigned by product**: Products sold sorted by license assignment count</span></span>

- <span data-ttu-id="7990c-163">**Licence, které se používají podle produktu:** Prodané produkty seřazené podle počtu využití licencí</span><span class="sxs-lookup"><span data-stu-id="7990c-163">**Licenses in use by product**: Products sold sorted by license usage count</span></span>

- <span data-ttu-id="7990c-164">**Distribuce přiřazených licencí ze strany** zákazníků: % rozdělení celkového počtu zákazníků v kbelíkůch po 20 % rozsahu podle % přiřazení licence</span><span class="sxs-lookup"><span data-stu-id="7990c-164">**Customer distribution of licenses assigned**: % distribution of total customers broken in buckets of 20% range by license assignment %</span></span>

- <span data-ttu-id="7990c-165">**Distribuce licencí, které se používají** pro zákazníky: % distribuce celkového počtu zákazníků rozdělených do kbelíků o 20% rozsahu podle % využití licencí</span><span class="sxs-lookup"><span data-stu-id="7990c-165">**Customer distribution of licenses in use**: % distribution of total customers broken in buckets of 20% range by license usage %</span></span>

- <span data-ttu-id="7990c-166">**Licence přiřazené zákazníkem:** Podrobné zobrazení prodaných licencí a licencí přiřazených zákazníky a produkty</span><span class="sxs-lookup"><span data-stu-id="7990c-166">**Licenses assigned by customer**: Detailed view of licenses sold and licenses assigned by customers and products</span></span>

- <span data-ttu-id="7990c-167">**Licence, které používá zákazník:** Podrobné zobrazení prodaných licencí a licencí, které používají zákazníci a produkty</span><span class="sxs-lookup"><span data-stu-id="7990c-167">**Licenses in use by customer**: Detailed view of licenses sold and licenses in use by customers and products</span></span>

### <a name="azure-insights-report"></a><span data-ttu-id="7990c-168">Sestava Azure Insights:</span><span class="sxs-lookup"><span data-stu-id="7990c-168">Azure Insights report:</span></span>

- <span data-ttu-id="7990c-169">Zákazníci se založenými na využití za **posledních 12** měsíců: Trend měsíčních trendů nových zákazníků založených na využití a zákazníků založených na churnedu využití agregovaných měsíčně za období posledních 12 měsíců</span><span class="sxs-lookup"><span data-stu-id="7990c-169">**Usage-based customers over last 12 months**: Month over month trend of new usage-based customers and churned usage-based customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="7990c-170">Předplatná založená na využití za **posledních 12** měsíců: Trend nových předplatných založených na využití a předplatných založených na četnosti změn agregovaných měsíčně za období posledních 12 měsíců</span><span class="sxs-lookup"><span data-stu-id="7990c-170">**Usage-based subscriptions over last 12 months**: Month over month trend of new usage-based subscriptions and churned usage-based subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="7990c-171">**Odhadované náklady** na využití podle zákazníka za posledních 60 dnů: Zákazníci na základě využití seřazení podle odhadované částky faktury před zdaněním agregované za období posledních 60 dnů.</span><span class="sxs-lookup"><span data-stu-id="7990c-171">**Estimated cost of usage by customer over last 60 days**: Usage-based customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span> <span data-ttu-id="7990c-172">Tento stav znamená, že zákazníci s nejvyšším využitím mají největší výnosy.</span><span class="sxs-lookup"><span data-stu-id="7990c-172">This status indicates top usage-based customers bringing most revenue</span></span>

- <span data-ttu-id="7990c-173">Odhadované náklady na využití podle kategorií za posledních **60** dnů: Kategorie měřičů předplatných založených na využití seřazené podle odhadované částky faktury před zdaněním agregované za období posledních 60 dnů.</span><span class="sxs-lookup"><span data-stu-id="7990c-173">**Estimated cost of usage by category over last 60 days**: Meter categories of usage-based subscriptions sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="7990c-174">**Odhadované náklady** na využití podle předplatného za posledních 60 dnů: Předplatná založená na využití podle odhadované částky faktury před zdaněním agregované za období posledních 60 dnů.</span><span class="sxs-lookup"><span data-stu-id="7990c-174">**Estimated cost of usage by subscription over last 60 days**: Usage-based subscriptions by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="7990c-175">**Odhadované náklady na využití na zákazníky podle rozpočtu útraty**: zákazníci, kteří se seřadili podle procenta jejich aktuálního využití, překračuje prahovou hodnotu (100%).</span><span class="sxs-lookup"><span data-stu-id="7990c-175">**Customer estimated usage cost by spending budget**: Customers sorted by percentage of their current usage spending budget exceeding threshold (100%).</span></span>

### <a name="azure-resource-usage-report"></a><span data-ttu-id="7990c-176">Sestava využití prostředků Azure:</span><span class="sxs-lookup"><span data-stu-id="7990c-176">Azure Resource Usage report:</span></span>

- <span data-ttu-id="7990c-177">**Využití prostředků Azure podle dne pro vybrané období**: denní jednotky spotřeby pro každý měřený prostředek v každém předplatném na základě využití pro vybrané období během posledních 60 dnů.</span><span class="sxs-lookup"><span data-stu-id="7990c-177">**Usage of Azure resources by day for selected period**: Daily consumption units for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span>

- <span data-ttu-id="7990c-178">**Odhadované náklady na využití prostředků Azure pro vybrané období**: Odhadované náklady na základě karty s nejnovějšími sazbami pro každý měřený prostředek v každém předplatném na základě využití pro vybrané období během posledních 60 dnů.</span><span class="sxs-lookup"><span data-stu-id="7990c-178">**Estimated usage cost of Azure resources for selected period**: Estimated cost based on latest rate card for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="7990c-179">Další kroky</span><span class="sxs-lookup"><span data-stu-id="7990c-179">Next steps</span></span>

- [<span data-ttu-id="7990c-180">Přehled služby partner Center Analytics pro aplikaci Power BI</span><span class="sxs-lookup"><span data-stu-id="7990c-180">Partner Center Analytics for Power BI app overview</span></span>](power-bi-app-for-direct-partners.md)

- [<span data-ttu-id="7990c-181">Instalace a vyzkoušení aplikace Analýzy v Partnerském centru pro Microsoft Power BI</span><span class="sxs-lookup"><span data-stu-id="7990c-181">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-install.md)
