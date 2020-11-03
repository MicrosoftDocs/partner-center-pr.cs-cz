---
title: Sestavy o prostředcích služby partner Center Insights – CloudAscent
description: Přečtěte si o sestavách PROPER CloudAscent v partnerském centru. Obsahuje informace o prodaných properech zákazníka při nákupu produktů společnosti Microsoft.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 09/18/2020
ms.openlocfilehash: fd017884c29df3874a06e8c4213c6fe5f05a8995
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/19/2020
ms.locfileid: "92527773"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a><span data-ttu-id="c08d1-104">CloudAscent sestavy o prostředcích, které jsou dostupné na řídicím panelu partnerského centra</span><span class="sxs-lookup"><span data-stu-id="c08d1-104">CloudAscent Propensity reports available from Partner Center dashboard</span></span>

<span data-ttu-id="c08d1-105">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="c08d1-105">**Appropriate roles**</span></span>
- <span data-ttu-id="c08d1-106">Prohlížeč sestav Executive</span><span class="sxs-lookup"><span data-stu-id="c08d1-106">Executive report viewer</span></span>
- <span data-ttu-id="c08d1-107">Prohlížeč sestav</span><span class="sxs-lookup"><span data-stu-id="c08d1-107">Report viewer</span></span>

<span data-ttu-id="c08d1-108">Řídicí panel partnerského centra poskytuje data o prostředcích ke stažení z programu CloudAscent.</span><span class="sxs-lookup"><span data-stu-id="c08d1-108">The Partner Center Dashboard provides downloadable propensity data from the CloudAscent Program.</span></span> <span data-ttu-id="c08d1-109">Tato data zobrazují PROPER zákazníků při nákupu produktů Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="c08d1-109">The data shows the customers' propensity to purchase Microsoft products.</span></span>  <span data-ttu-id="c08d1-110">Tento článek popisuje rozpis těchto dat, způsob využití bodování a to, co znamená.</span><span class="sxs-lookup"><span data-stu-id="c08d1-110">This articles describes the breakdown of this data, how to utilize the scoring, and what it means.</span></span>

## <a name="summary-definitions"></a><span data-ttu-id="c08d1-111">Souhrnné definice</span><span class="sxs-lookup"><span data-stu-id="c08d1-111">Summary definitions</span></span>

- <span data-ttu-id="c08d1-112">**Zákazníci** se systémem SMC – Toto je celkový počet zákazníků při stahování proper.</span><span class="sxs-lookup"><span data-stu-id="c08d1-112">**SMC Customers** – This is the total number of customers in the propensity downloads.</span></span>  <span data-ttu-id="c08d1-113">Zákazníci jsou identifikováni partnerem záznamu.</span><span class="sxs-lookup"><span data-stu-id="c08d1-113">Customers are identified by partner of record.</span></span>
- <span data-ttu-id="c08d1-114">**Smlouvy s vypršenou platností** – v rámci aktuálního fiskálního roku poskytujeme počet smluv o vypršení platnosti.</span><span class="sxs-lookup"><span data-stu-id="c08d1-114">**Expire Agreements** – within the current fiscal year, we're providing the number of expiring agreements.</span></span>
- <span data-ttu-id="c08d1-115">**Vypršení výnosů** – tržby spojené s smlouvami o vypršení platnosti.</span><span class="sxs-lookup"><span data-stu-id="c08d1-115">**Expiring Revenue** – the revenue associated to the expiring agreements.</span></span>
- <span data-ttu-id="c08d1-116">**Otevřené výnosy po vypršení platnosti** – tržby spojené s otevřenými smlouvami o vypršení platnosti.</span><span class="sxs-lookup"><span data-stu-id="c08d1-116">**Open Expiring Revenue** – The revenue associated to the open expiring agreements.</span></span>

:::image type="content" source="images/pci/cust-oppor-1.png" alt-text="Snímek obrazovky se souhrnným řídicím panelem příležitostí pro zákazníky":::

## <a name="cloudascent-smb-segmentation"></a><span data-ttu-id="c08d1-118">Segmentace SMB CloudAscent</span><span class="sxs-lookup"><span data-stu-id="c08d1-118">CloudAscent SMB segmentation</span></span>

<span data-ttu-id="c08d1-119">Segment malý až střední firmy (SMB) je dále rozdělen do tří samostatných dílčích segmentů.</span><span class="sxs-lookup"><span data-stu-id="c08d1-119">The small to medium business (SMB) segment is further divided into three distinct sub segments.</span></span>

1. <span data-ttu-id="c08d1-120">**Hlavní nespravované** zahrnuje největší zákazníky s protokolem SMB s největší příležitostí pro Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c08d1-120">**Top Unmanaged** includes the largest SMB customers with the most opportunity for Microsoft.</span></span> <span data-ttu-id="c08d1-121">Typický hlavní nespravovaný zákazník sdílí podobné charakteristiky jako spravované účty, velký počet zaměstnanců, velké rozpočty IT a výdaje a velké objemy potenciálních výnosů pro Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c08d1-121">Typical Top Unmanaged customers share similar characteristics as Managed accounts, with large number of employees, large IT budgets and spend, and large amounts of potential revenue for Microsoft.</span></span>

   <span data-ttu-id="c08d1-122">Definujeme hlavní nespravované dva způsoby:</span><span class="sxs-lookup"><span data-stu-id="c08d1-122">We define Top Unmanaged two ways:</span></span>

   - <span data-ttu-id="c08d1-123">**Hlavní nespravovaný uživatel** – obsahuje účty s 300 nebo více zaměstnanci.</span><span class="sxs-lookup"><span data-stu-id="c08d1-123">**Top Unmanaged User Based** – includes accounts with 300 or more employees.</span></span> <span data-ttu-id="c08d1-124">Účty User-Based jsou skvělé cíle pro první nákup nebo rozšíření produktů pro odběr uživatelů, jako je M365, D365 nebo Surface.</span><span class="sxs-lookup"><span data-stu-id="c08d1-124">User-Based accounts are great targets for first-time purchase, or expansion of user-based subscription products such as M365, D365, or Surface.</span></span>
   - <span data-ttu-id="c08d1-125">**Založené na hlavních nespravovaných výpočetních** operacích – obsahuje účty s potenciálem Azure větším než $10 000.</span><span class="sxs-lookup"><span data-stu-id="c08d1-125">**Top Unmanaged Compute Based** – includes accounts with Azure potential greater than $10k.</span></span> <span data-ttu-id="c08d1-126">Účty založené na COMPUTE zahrnují existující Azure.</span><span class="sxs-lookup"><span data-stu-id="c08d1-126">Compute based accounts include existing Azure.</span></span> <span data-ttu-id="c08d1-127">účty s významným potenciálem budoucích let a účty, které ještě ještě kupují Azure, ale mají možnost Azure větší než $10 000.</span><span class="sxs-lookup"><span data-stu-id="c08d1-127">accounts with significant future year potential and accounts who have yet to purchase Azure yet but have potential for Azure greater than $10k.</span></span>

2. <span data-ttu-id="c08d1-128">**Středně velké firmy** zahrnují stávající zákazníky a účty nadějných zákazníků s 25 až 300 zaměstnanci.</span><span class="sxs-lookup"><span data-stu-id="c08d1-128">**Medium Business** includes existing customers and prospect accounts with 25 to 300 employees.</span></span>

3. <span data-ttu-id="c08d1-129">**Malé firmy** zahrnují všechny zbývající firmy s méně než 25 zaměstnanci.</span><span class="sxs-lookup"><span data-stu-id="c08d1-129">**Small Business** includes all remaining businesses with fewer than 25 employees.</span></span>

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="Zákazník podle typu SMC.":::

<span data-ttu-id="c08d1-131">**Hlavní nespravované** a **střední části podniku** reprezentují vysoké LTV zákazníky pro Microsoft a partnery Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="c08d1-131">**Top Unmanaged** and **Medium Business** subsegments represent high life-time value (LTV) customers for Microsoft, and Microsoft Partners.</span></span> <span data-ttu-id="c08d1-132">Proto jsou v tomto segmentu oblasti olova zaměřeny na zvýšení růstu.</span><span class="sxs-lookup"><span data-stu-id="c08d1-132">Hence they are the lead areas of focus for driving growth in this segment.</span></span> <span data-ttu-id="c08d1-133">V těchto dvou segmentech jsme lépe umístili k získání soketu pomocí M365, monetizovat s D365/Azure obchodními aplikacemi (LOB) a zajistili jsme vysoké LTV pro společnost Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c08d1-133">In these two subsegments, we are better positioned to acquire the socket with M365, monetize further with D365/Azure line of business (LOB) apps, and realize a high LTV for Microsoft.</span></span>

<span data-ttu-id="c08d1-134">Dnes máme dvě klíčové oblasti příležitosti – 1.</span><span class="sxs-lookup"><span data-stu-id="c08d1-134">Today we have two key areas of opportunity – 1.</span></span> <span data-ttu-id="c08d1-135">Náš zákazník přináší růst; odst.</span><span class="sxs-lookup"><span data-stu-id="c08d1-135">our customer adds growth; 2.</span></span> <span data-ttu-id="c08d1-136">i když máme kvalitní cloudové sokety, které začínají na M365, máme v D365 a Azure velkou příležitost.</span><span class="sxs-lookup"><span data-stu-id="c08d1-136">while we do well acquiring cloud sockets leading with M365, we have a large opportunity in D365 and Azure.</span></span>

<span data-ttu-id="c08d1-137">Následující snímek obrazovky představuje tři segmenty SMB a optimalizované trasy k uvedení na trh.</span><span class="sxs-lookup"><span data-stu-id="c08d1-137">The following screenshot represents the three SMB Subsegments and optimized routes to market.</span></span> <span data-ttu-id="c08d1-138">CloudAscent stanovit prioritu profilace, bodování a modelování všech hlavních nespravovaných a středně velkých obchodních účtů.</span><span class="sxs-lookup"><span data-stu-id="c08d1-138">CloudAscent prioritize the profiling, scoring, and modeling of all Top Unmanaged and Medium Business accounts.</span></span>

:::image type="content" source="images/pci/cust-oppor-3.png" alt-text="Snímek obrazovky s podsegmenty SMB.":::

## <a name="cloudascent-machine-learning"></a><span data-ttu-id="c08d1-140">CloudAscent Machine Learning</span><span class="sxs-lookup"><span data-stu-id="c08d1-140">CloudAscent Machine Learning</span></span>

<span data-ttu-id="c08d1-141">Protokol SMB používá technologii strojového učení k řízení prodeje a marketingu zákaznických předpovědi v hlavních nespravovaných a středních obchodních segmentech.</span><span class="sxs-lookup"><span data-stu-id="c08d1-141">SMB uses machine learning technology to drive sales and marketing customer predictions within the Top Unmanaged and Medium Business segments.</span></span> <span data-ttu-id="c08d1-142">Jak jsou signály shromažďovány a přeměněny na doporučení týkající se Proper?</span><span class="sxs-lookup"><span data-stu-id="c08d1-142">How are signals collected and turned into propensity recommendations?</span></span>

- <span data-ttu-id="c08d1-143">**Shromažďování dat** : webové prohledávací moduly hledají a shromažďují miliardy zákaznických signálů pomocí příkazů k otestování domén společnosti a monitorují: blogové příspěvky, tiskové příspěvky, sociální toky a technická fóra.</span><span class="sxs-lookup"><span data-stu-id="c08d1-143">**Data Collection** : Web crawlers scan and collect billions of customer signals by pinging the company domains, and monitoring: blog posts, press releases, social streams, and technical forums.</span></span>  <span data-ttu-id="c08d1-144">Kromě shromážděných signálů se informace o firmographics shromažďují z interních i externích zdrojů, jako je například D&B, interní předplatné Microsoftu a transakční data.</span><span class="sxs-lookup"><span data-stu-id="c08d1-144">In addition to the collected signals, firmographics information is collected from both internal and external sources such as D&B, Microsoft Internal subscription and transactional data.</span></span>

- <span data-ttu-id="c08d1-145">**Machine Learning** : signály se dopravují do modelu machine learningu, který pro každého zákazníka cloudového produktu a clusteru vytvoří strukturu strukturované datové sady předpovědi pro prodej a marketing.</span><span class="sxs-lookup"><span data-stu-id="c08d1-145">**Machine Learning** : The signals are fed into the machine learning model that outputs a structured data set of Sales and Marketing predictions for each customer by cloud product and cluster.</span></span>  <span data-ttu-id="c08d1-146">Každý zákazník se vyhodnotí pomocí podobného modelu jako v horním protokolu SMB od Microsoftu, který určuje přizpůsobení a algoritmy strojového učení, které integrují online chování zákazníka, se definuje jako záměr.</span><span class="sxs-lookup"><span data-stu-id="c08d1-146">Each customer is scored using a look alike model to Microsoft's top SMB that determines the customer's Fit, and machine learning algorithms that integrate the customer's online behavior define as Intent.</span></span> <span data-ttu-id="c08d1-147">Bodování se sloučí do clusterů, které znázorňují prohlédnutí zákazníka k nákupu Microsoft Cloudch produktů.</span><span class="sxs-lookup"><span data-stu-id="c08d1-147">The scoring is merged into clusters that show a customer's propensity to purchase Microsoft Cloud Products.</span></span>

- <span data-ttu-id="c08d1-148">**Optimalizace** : systém Machine Learning optimalizuje modely tím, že spotřebovává data transakcí měsíčně a čtvrtletní data předplatného.</span><span class="sxs-lookup"><span data-stu-id="c08d1-148">**Optimization** : The Machine Learning system optimizes the models by consuming the transaction data monthly and the subscription data quarterly.</span></span>  <span data-ttu-id="c08d1-149">Pomocí dat o výher a ztrátách Machine Learning upravuje algoritmy a ověřuje, že modely pracují podle očekávání, tím, že porovnává doporučení clusteru s možnostmi, které se v hlavní části vycházejí.</span><span class="sxs-lookup"><span data-stu-id="c08d1-149">Using the win/loss data, the Machine Learning adjusts the algorithms and validates that the models are working as expected by comparing cluster recommendations to opportunities acted upon in MSX.</span></span>

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="Snímek obrazovky s protokolem SMB Machine Learning.":::

## <a name="cloudascent-propensity"></a><span data-ttu-id="c08d1-151">CloudAscent Proper</span><span class="sxs-lookup"><span data-stu-id="c08d1-151">CloudAscent Propensity</span></span>

<span data-ttu-id="c08d1-152">Jak se vytvářejí doporučení k properům?</span><span class="sxs-lookup"><span data-stu-id="c08d1-152">How are propensity recommendations created?</span></span>

<span data-ttu-id="c08d1-153">Pomocí signálů shromážděných prostřednictvím webových procházecích a dat z různých zdrojů konsolidujeme firmographics data a sociální signály sociálních médií zákazníka.</span><span class="sxs-lookup"><span data-stu-id="c08d1-153">Using signals collected via web crawlers and data provided from various sources, we consolidate the firmographics data and customer's social media signals.</span></span>  <span data-ttu-id="c08d1-154">Bodování používá tyto signály a data v porovnání modelů pro potřeby a modely bodování pro záměr.</span><span class="sxs-lookup"><span data-stu-id="c08d1-154">The scoring uses these signals and data in comparison models for fit and scoring models for Intent.</span></span>

1. <span data-ttu-id="c08d1-155">Přizpůsobení účtu zákazníka</span><span class="sxs-lookup"><span data-stu-id="c08d1-155">Customer Account Fit</span></span>

   - <span data-ttu-id="c08d1-156">Interní a externí datové body, které definují firmographics.</span><span class="sxs-lookup"><span data-stu-id="c08d1-156">Internal and External data points that define firmographics.</span></span>

   - <span data-ttu-id="c08d1-157">Pro účely bodování se používá model podobného typu, který umožňuje porovnat zákazníky a zjistit, jestli jsou potenciálně vyhovující Microsoft Cloud produktů.</span><span class="sxs-lookup"><span data-stu-id="c08d1-157">Fit scoring uses a look alike model to our best SMB to compare customers and see if they're a potential  fit for Microsoft Cloud Products.</span></span>

   - <span data-ttu-id="c08d1-158">Podle skóre se aktualizuje čtvrtletní</span><span class="sxs-lookup"><span data-stu-id="c08d1-158">Fit scoring is updated quarterly</span></span>

2. <span data-ttu-id="c08d1-159">Záměr účtu zákazníka</span><span class="sxs-lookup"><span data-stu-id="c08d1-159">Customer Account Intent</span></span>

   - <span data-ttu-id="c08d1-160">Signály týkající se sociálních médií a definování záměrů online zákazníka.</span><span class="sxs-lookup"><span data-stu-id="c08d1-160">Signals related to Social media and a customer's online behavior define Intent.</span></span>

   - <span data-ttu-id="c08d1-161">Bodování záměru je překrytí na základě přizpůsobení, aby bylo možné definovat clustery.</span><span class="sxs-lookup"><span data-stu-id="c08d1-161">Intent scoring is overlaid on top of fit to define the clusters.</span></span>

   - <span data-ttu-id="c08d1-162">Bodování záměru se aktualizuje měsíčně.</span><span class="sxs-lookup"><span data-stu-id="c08d1-162">Intent scoring is updated monthly.</span></span>

   :::image type="content" source="images/pci/cust-oppor-5.png" alt-text="CloudAscenté prediktivní modely protokolu SMB.":::

3. <span data-ttu-id="c08d1-164">Clustering</span><span class="sxs-lookup"><span data-stu-id="c08d1-164">Clustering</span></span>

   <span data-ttu-id="c08d1-165">Signály pro přizpůsobení a záměr jsou konsolidovány do skóre clusteringu.</span><span class="sxs-lookup"><span data-stu-id="c08d1-165">The Signals for fit and intent are consolidated into a clustering score.</span></span> <span data-ttu-id="c08d1-166">CloudAscent má čtyři clustery:</span><span class="sxs-lookup"><span data-stu-id="c08d1-166">CloudAscent has four clusters:</span></span>

      - <span data-ttu-id="c08d1-167">Zákazníci, kteří jsou nyní připravení k prodeji</span><span class="sxs-lookup"><span data-stu-id="c08d1-167">Act Now - sales ready customers</span></span>
      - <span data-ttu-id="c08d1-168">Vyhodnocení – zákazníci připravení pro marketing</span><span class="sxs-lookup"><span data-stu-id="c08d1-168">Evaluate - marketing ready customers</span></span>
      - <span data-ttu-id="c08d1-169">Nurture – kampaně pro osvětu</span><span class="sxs-lookup"><span data-stu-id="c08d1-169">Nurture - drive awareness campaigns</span></span>
      - <span data-ttu-id="c08d1-170">Vzdělávání – vzdělávání a monitorování pro záměr</span><span class="sxs-lookup"><span data-stu-id="c08d1-170">Educate - educate and monitor for intent</span></span>

   <span data-ttu-id="c08d1-171">Clustering umožňuje uživatelům zaměřit se na konkrétní zákazníky na prodejní a marketingové iniciativy na základě faktorů segmentů, například: produkt, geografické prostředí, odvětví a vertikální.</span><span class="sxs-lookup"><span data-stu-id="c08d1-171">The clustering allows users to target specific customers for sales and marketing initiatives based on segment factors, for example: product, geo, industry and vertical.</span></span>

   <span data-ttu-id="c08d1-172">Karta **model PROPER** v sešitech CloudAscent sdílí PROPER a odhadované tržby za prázdných znaků.</span><span class="sxs-lookup"><span data-stu-id="c08d1-172">The **Propensity model** tab in the CloudAscent Workbooks shares the propensity and the estimated whitespace revenue.</span></span> <span data-ttu-id="c08d1-173">Pokud chcete definovat clustery, které je vhodné a záměr, Projděte si následující kroky:</span><span class="sxs-lookup"><span data-stu-id="c08d1-173">To define the clustering of Fit and Intent, we go through the following steps:</span></span>

      1. <span data-ttu-id="c08d1-174">Pomocí modelů ML si předem vypočítáme skóre a skóre záměru zákazníka na škále 100.</span><span class="sxs-lookup"><span data-stu-id="c08d1-174">Using ML Models, we first calculate Customer Fit Score and intent Score on a scale of 100.</span></span>  <span data-ttu-id="c08d1-175">Přesné výsledky se budou lišit v závislosti na modelů ML.</span><span class="sxs-lookup"><span data-stu-id="c08d1-175">Exact Scores will vary based on ML Models.</span></span>  <span data-ttu-id="c08d1-176">Příklad skóre níže:</span><span class="sxs-lookup"><span data-stu-id="c08d1-176">Example Scores Below:</span></span>

         |<span data-ttu-id="c08d1-177">**Klasifikace**</span><span class="sxs-lookup"><span data-stu-id="c08d1-177">**Classification**</span></span>|<span data-ttu-id="c08d1-178">**Skóre**</span><span class="sxs-lookup"><span data-stu-id="c08d1-178">**Score**</span></span>|
         |---------|:---------|
         |<span data-ttu-id="c08d1-179">Vysoké</span><span class="sxs-lookup"><span data-stu-id="c08d1-179">High</span></span>|<span data-ttu-id="c08d1-180">75 – 100</span><span class="sxs-lookup"><span data-stu-id="c08d1-180">75 - 100</span></span>|
         |<span data-ttu-id="c08d1-181">Střední</span><span class="sxs-lookup"><span data-stu-id="c08d1-181">Medium</span></span>|<span data-ttu-id="c08d1-182">55 – 74</span><span class="sxs-lookup"><span data-stu-id="c08d1-182">55 - 74</span></span>|
         |<span data-ttu-id="c08d1-183">Nízká</span><span class="sxs-lookup"><span data-stu-id="c08d1-183">Low</span></span>|<span data-ttu-id="c08d1-184">30 - 54</span><span class="sxs-lookup"><span data-stu-id="c08d1-184">30 - 54</span></span>|
         |<span data-ttu-id="c08d1-185">Velmi nízké</span><span class="sxs-lookup"><span data-stu-id="c08d1-185">Very Low</span></span>|<span data-ttu-id="c08d1-186">0 - 29</span><span class="sxs-lookup"><span data-stu-id="c08d1-186">0 - 29</span></span>|

      2. <span data-ttu-id="c08d1-187">Pomocí výše uvedeného pravidla klasifikujeme společnosti tak, aby byly vysoké, střední, nízké a velmi nízké v rámci přizpůsobení a signálů pro zákazníky.</span><span class="sxs-lookup"><span data-stu-id="c08d1-187">Using the rule above, we classify companies to be High, Medium, Low, and Very Low across both Customer Fit    and Intent Signals.</span></span>

      3. <span data-ttu-id="c08d1-188">Na 2D matrici vykreslíme vydaných a vystupujících signálů zákazníků s každým průnikem, který představuje proper.</span><span class="sxs-lookup"><span data-stu-id="c08d1-188">We plot customer fit and intent signals on a 2D matrix with each intersection representing the propensity.</span></span>     <span data-ttu-id="c08d1-189">Například vysoká velikost + vysoká záměr = a1, který představuje nejvyšší proper.</span><span class="sxs-lookup"><span data-stu-id="c08d1-189">For Example, High Fit + High Intent = A1, representing the highest propensity.</span></span>

      4. <span data-ttu-id="c08d1-190">Nakonec tyto segmenty seskupují clustery.</span><span class="sxs-lookup"><span data-stu-id="c08d1-190">Finally, these segments group to form clusters.</span></span>  <span data-ttu-id="c08d1-191">Například, a1, a2, a3, A4 tvoří cluster Act Now.</span><span class="sxs-lookup"><span data-stu-id="c08d1-191">For Example, A1, A2, A3, A4 form the Act Now cluster.</span></span>

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="CloudAscent modely.":::

   <span data-ttu-id="c08d1-193">Pro tyto zákazníky doporučujeme cílit na Act nyní a vyhodnocovat zákazníky.</span><span class="sxs-lookup"><span data-stu-id="c08d1-193">For these customers, we recommend targeting Act Now and Evaluate customers.</span></span>

## <a name="cloudascent-products--models"></a><span data-ttu-id="c08d1-194">CloudAscent produkty & modely</span><span class="sxs-lookup"><span data-stu-id="c08d1-194">CloudAscent Products & Models</span></span>

<span data-ttu-id="c08d1-195">Následující obrázek poskytuje zobrazení jednotlivých modelů PROPER v rámci CloudAscent:</span><span class="sxs-lookup"><span data-stu-id="c08d1-195">The following graphic provides a view of each propensity model within CloudAscent:</span></span>

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="CloudAscent model proper.":::

<span data-ttu-id="c08d1-197">Prázdné modely se skládají z předpovědi pro stávající zákazníky Microsoftu, kde nemají produkt a/nebo jsou noví zákazníci, kteří používají zákazníky v rámci zákazníků.</span><span class="sxs-lookup"><span data-stu-id="c08d1-197">Whitespace models are composed of predictions for existing Microsoft customers where they don't have a product and/or are net new prospect customers.</span></span>

<span data-ttu-id="c08d1-198">Modely přeprodat používají data transakcí k předpovídání potenciálu přeprodat v SKU Azure a M365.</span><span class="sxs-lookup"><span data-stu-id="c08d1-198">Upsell models use transaction data to predict the potential for upsell in Azure and M365 SKUs.</span></span>

<span data-ttu-id="c08d1-199">EOS sdílí koncové zákazníky služby pro Win 7, Office 2010, SQL Server a Windows Server.</span><span class="sxs-lookup"><span data-stu-id="c08d1-199">EOS shares the end of service customers for Win 7, Office 2010, SQL Server, and Windows Server.</span></span> <span data-ttu-id="c08d1-200">Data EOS se předají z prodeje MS a překrývají se pomocí modelování PROPER CloudAscent, kde jsou k dispozici.</span><span class="sxs-lookup"><span data-stu-id="c08d1-200">The EOS data is pulled from MS Sales and overlaid with the CloudAscent propensity modeling where available.</span></span> <span data-ttu-id="c08d1-201">EOS data v moderní práci a prodej v Azure.</span><span class="sxs-lookup"><span data-stu-id="c08d1-201">EOS data lives in the Modern Work and Azure Sales plays.</span></span>
