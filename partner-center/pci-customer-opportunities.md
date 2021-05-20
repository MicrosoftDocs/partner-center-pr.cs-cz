---
title: Partnerské centrum Insights – sestavy sklonu CloudAscent
description: Seznamte se se zprávami CloudAscent Propensity v Partnerské centrum. Obsahuje informace o náchylnosti zákazníka k nákupu produktů Microsoftu.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 04/27/2021
ms.openlocfilehash: 430aea81964d1b75514b6e1377bd2ba1af41b538
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110153034"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a><span data-ttu-id="d0276-104">Sestavy CloudAscent Propensity dostupné na Partnerské centrum řídicím panelu</span><span class="sxs-lookup"><span data-stu-id="d0276-104">CloudAscent Propensity reports available from Partner Center dashboard</span></span>

<span data-ttu-id="d0276-105">**Odpovídající role:** Prohlížeč sestav executive | Prohlížeč sestav</span><span class="sxs-lookup"><span data-stu-id="d0276-105">**Appropriate roles**: Executive report viewer | Report viewer</span></span>

<span data-ttu-id="d0276-106">Řídicí Partnerské centrum poskytuje data o sklonu ke stažení z programu CloudAscent.</span><span class="sxs-lookup"><span data-stu-id="d0276-106">The Partner Center dashboard provides downloadable propensity data from the CloudAscent program.</span></span> <span data-ttu-id="d0276-107">Data ukazují pravděpodobnost, že zákazníci budou kupovat produkty Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="d0276-107">The data shows the customers' likelihood to purchase Microsoft products.</span></span>  <span data-ttu-id="d0276-108">Tento článek popisuje rozpis těchto dat, způsob použití vyhodnocování a co to znamená.</span><span class="sxs-lookup"><span data-stu-id="d0276-108">This article describes the breakdown of this data, how to use the scoring, and what it means.</span></span>

## <a name="summary-definitions"></a><span data-ttu-id="d0276-109">Souhrnné definice</span><span class="sxs-lookup"><span data-stu-id="d0276-109">Summary definitions</span></span>

- <span data-ttu-id="d0276-110">**Zákazníci SMC**– Celkový počet zákazníků, kteří se ke stažení s náchylností stahují.</span><span class="sxs-lookup"><span data-stu-id="d0276-110">**SMC Customers**– This is the total number of customers in the propensity downloads.</span></span>  <span data-ttu-id="d0276-111">Zákazníci jsou identifikováni partnerem záznamu.</span><span class="sxs-lookup"><span data-stu-id="d0276-111">Customers are identified by partner of record.</span></span>
- <span data-ttu-id="d0276-112">**Vypršení platnosti** smluv – v rámci aktuálního fiskálního roku zadáte počet smluv, u které vyprší platnost.</span><span class="sxs-lookup"><span data-stu-id="d0276-112">**Expire Agreements**– Within the current fiscal year, we're providing the number of expiring agreements.</span></span>
- <span data-ttu-id="d0276-113">**Open Expiring Revenue**–Výnosy spojené se smlouvami o otevření, u které vyprší platnost.</span><span class="sxs-lookup"><span data-stu-id="d0276-113">**Open Expiring Revenue**– The revenue associated to the open expiring agreements.</span></span>

:::image type="content" source="images/pci/cust-oppor-11.png" alt-text="Snímek obrazovky s řídicím panelem Souhrn příležitostí zákazníků":::

## <a name="cloudascent-smb-segmentation"></a><span data-ttu-id="d0276-115">Segmentace SMB v CloudAscent</span><span class="sxs-lookup"><span data-stu-id="d0276-115">CloudAscent SMB segmentation</span></span>

<span data-ttu-id="d0276-116">Segment SMB (Small to Medium Business) je rozdělen do tří různých dílčích segmentů.</span><span class="sxs-lookup"><span data-stu-id="d0276-116">The small to medium business (SMB) segment is divided into three distinct sub segments.</span></span>

1. <span data-ttu-id="d0276-117">**Top Unmanaged zahrnuje** největší zákazníky SMB s největší příležitostí pro Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d0276-117">**Top Unmanaged** includes the largest SMB customers with the most opportunity for Microsoft.</span></span> <span data-ttu-id="d0276-118">Typickí nespravované zákazníky mají podobné vlastnosti jako spravované účty s velkým počtem zaměstnanců, velkými rozpočty a výdaje na IT a velkými objemy potenciálních výnosů pro Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d0276-118">Typical Top Unmanaged customers share similar characteristics to Managed accounts, with large number of employees, large IT budgets and spend, and large amounts of potential revenue for Microsoft.</span></span>

   <span data-ttu-id="d0276-119">Nespravované prostředky definujeme dvěma způsoby:</span><span class="sxs-lookup"><span data-stu-id="d0276-119">We define Top Unmanaged in two ways:</span></span>

   - <span data-ttu-id="d0276-120">**Top Unmanaged User Based –zahrnuje** účty se 300 nebo více zaměstnanci.</span><span class="sxs-lookup"><span data-stu-id="d0276-120">**Top Unmanaged User Based**– includes accounts with 300 or more employees.</span></span> <span data-ttu-id="d0276-121">Účty User-Based jsou skvělé cíle pro první nákup nebo rozšíření produktů pro odběr uživatelů, jako je Microsoft 365, Dynamics 365 nebo Surface.</span><span class="sxs-lookup"><span data-stu-id="d0276-121">User-Based accounts are great targets for first-time purchase, or expansion of user-based subscription products such as Microsoft 365, Dynamics 365, or Surface.</span></span>
   - <span data-ttu-id="d0276-122">**Založené na hlavních nespravovaných výpočetních** operacích – obsahuje účty s potenciálem Azure větším než $10 000.</span><span class="sxs-lookup"><span data-stu-id="d0276-122">**Top Unmanaged Compute Based** – includes accounts with Azure potential greater than $10k.</span></span> <span data-ttu-id="d0276-123">Účty založené na COMPUTE zahrnují existující Azure.</span><span class="sxs-lookup"><span data-stu-id="d0276-123">Compute based accounts include existing Azure.</span></span> <span data-ttu-id="d0276-124">účty s významným potenciálem budoucích let a účty, které ještě ještě kupují Azure, ale mají možnost Azure větší než $10 000.</span><span class="sxs-lookup"><span data-stu-id="d0276-124">accounts with significant future year potential and accounts who have yet to purchase Azure yet but have potential for Azure greater than $10k.</span></span>

2. <span data-ttu-id="d0276-125">**Středně velké firmy** zahrnují stávající zákazníky a účty nadějných zákazníků s 25 až 300 zaměstnanci.</span><span class="sxs-lookup"><span data-stu-id="d0276-125">**Medium Business** includes existing customers and prospect accounts with 25 to 300 employees.</span></span>

3. <span data-ttu-id="d0276-126">**Malá společnost** zahrnuje firmy s 10-25 zaměstnanci.</span><span class="sxs-lookup"><span data-stu-id="d0276-126">**Small Business** includes businesses with 10-25 employees.</span></span>

4. <span data-ttu-id="d0276-127">**Velmi malá společnost** zahrnuje firmy s 1-9 zaměstnanci.</span><span class="sxs-lookup"><span data-stu-id="d0276-127">**Very Small Business** includes businesses with 1-9 employees.</span></span>

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="Zákazník podle typu SMC.":::

<span data-ttu-id="d0276-129">**Hlavní nespravované** a **střední části podniku** reprezentují vysoké LTV zákazníky pro Microsoft a partnery Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="d0276-129">**Top Unmanaged** and **Medium Business** subsegments represent high life-time value (LTV) customers for Microsoft, and Microsoft Partners.</span></span> <span data-ttu-id="d0276-130">Z tohoto důvodu se jedná o oblasti potenciálních zákazníků, které se zaměřují na růst v tomto segmentu.</span><span class="sxs-lookup"><span data-stu-id="d0276-130">Because of this, they're the lead areas of focus for driving growth in this segment.</span></span> <span data-ttu-id="d0276-131">V těchto dvou segmentech jsme lépe umístili k získání soketu s Microsoft 365 monetizovat a D365/Azure obchodními aplikacemi (LOB) a zajistili jsme vysoké LTV pro společnost Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d0276-131">In these two subsegments, we're better positioned to acquire the socket with Microsoft 365, monetize further with D365/Azure line of business (LOB) apps, and realize a high LTV for Microsoft.</span></span>

<span data-ttu-id="d0276-132">Dnes máme dvě klíčové oblasti příležitosti – 1.</span><span class="sxs-lookup"><span data-stu-id="d0276-132">Today we have two key areas of opportunity – 1.</span></span> <span data-ttu-id="d0276-133">Náš zákazník přináší růst; odst.</span><span class="sxs-lookup"><span data-stu-id="d0276-133">our customer adds growth; 2.</span></span> <span data-ttu-id="d0276-134">i když nám načítáme cloudové sokety s Microsoft 365, máme v Dynamics 365 a Azure velkou příležitost.</span><span class="sxs-lookup"><span data-stu-id="d0276-134">while we do well acquiring cloud sockets leading with Microsoft 365, we have a large opportunity in Dynamics 365 and Azure.</span></span>

<span data-ttu-id="d0276-135">Následující snímek obrazovky představuje čtyři segmenty SMB.</span><span class="sxs-lookup"><span data-stu-id="d0276-135">The following screenshot represents the four SMB Subsegments.</span></span> <span data-ttu-id="d0276-136">CloudAscent stanovit prioritu profilace, bodování a modelování všech hlavních nespravovaných a středně velkých obchodních účtů.</span><span class="sxs-lookup"><span data-stu-id="d0276-136">CloudAscent prioritize the profiling, scoring, and modeling of all Top Unmanaged and Medium Business accounts.</span></span>

:::image type="content" source="images/pci/cust-oppor-32.png" alt-text="Snímek obrazovky s podsegmenty SMB.":::

## <a name="cloudascent-machine-learning"></a><span data-ttu-id="d0276-138">CloudAscent Machine Learning</span><span class="sxs-lookup"><span data-stu-id="d0276-138">CloudAscent Machine Learning</span></span>

<span data-ttu-id="d0276-139">Protokol SMB používá technologii strojového učení k řízení prodeje a marketingu zákaznických předpovědi v hlavních nespravovaných a středních obchodních segmentech.</span><span class="sxs-lookup"><span data-stu-id="d0276-139">SMB uses machine learning technology to drive sales and marketing customer predictions within the Top Unmanaged and Medium Business segments.</span></span> <span data-ttu-id="d0276-140">Jak jsou signály shromažďovány a přeměněny na doporučení týkající se Proper?</span><span class="sxs-lookup"><span data-stu-id="d0276-140">How are signals collected and turned into propensity recommendations?</span></span>

- <span data-ttu-id="d0276-141">**Shromažďování dat:** Webové prohledávací systémy prohledávače skenují a shromažďují miliardy signálů zákazníků příkazem ping na domény společnosti a monitorují blogové příspěvky, tiskové zprávy, sociální streamy a technická fóra.</span><span class="sxs-lookup"><span data-stu-id="d0276-141">**Data Collection**: Web crawlers scan and collect billions of customer signals by pinging the company domains, and monitoring blog posts, press releases, social streams, and technical forums.</span></span>  <span data-ttu-id="d0276-142">Kromě shromážděných signálů se firemní údaje shromažďují z interních i externích zdrojů, jako jsou D&B, interní předplatné Microsoftu a transakční data.</span><span class="sxs-lookup"><span data-stu-id="d0276-142">In addition to the collected signals, firmographics information is collected from both internal and external sources such as D&B, Microsoft Internal subscription and transactional data.</span></span>

- <span data-ttu-id="d0276-143">**Machine Learning:** Signály se předá do modelu strojového učení, který každému zákazníkovi předpovídá strukturovaná datová sada předpovědí prodeje a marketingu podle cloudových produktů a shluků.</span><span class="sxs-lookup"><span data-stu-id="d0276-143">**Machine Learning**: The signals are fed into the machine learning model that outputs a structured data set of Sales and Marketing predictions for each customer by cloud product and cluster.</span></span>  <span data-ttu-id="d0276-144">Každý zákazník má skóre s použitím podobného modelu pro nejlepší SMB Microsoftu, který určuje algoritmy Fit zákazníka a strojové učení, které integrují online chování zákazníka, které definují záměr.</span><span class="sxs-lookup"><span data-stu-id="d0276-144">Each customer is scored using a look alike model to Microsoft's top SMB that determines the customer's Fit, and machine learning algorithms that integrate the customer's online behavior define as Intent.</span></span> <span data-ttu-id="d0276-145">Bodování se sloučí do clusterů, které ukazují náchylnost zákazníka k nákupu cloudových produktů Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="d0276-145">The scoring is merged into clusters that show a customer's propensity to purchase Microsoft Cloud Products.</span></span>

- <span data-ttu-id="d0276-146">**Optimalizace:** systém Machine Learning optimalizuje modely tím, že každý měsíc spotřebovává data transakcí a čtvrtletně data předplatného.</span><span class="sxs-lookup"><span data-stu-id="d0276-146">**Optimization**: The Machine Learning system optimizes the models by consuming the transaction data monthly and the subscription data quarterly.</span></span>  <span data-ttu-id="d0276-147">Pomocí dat o výhře/ztrátě Machine Learning upraví algoritmy a ověří, že modely fungují podle očekávání, porovnáním doporučení clusteru s příležitostmi v MSX.</span><span class="sxs-lookup"><span data-stu-id="d0276-147">Using the win/loss data, the Machine Learning adjusts the algorithms and validates that the models are working as expected by comparing cluster recommendations to opportunities acted upon in MSX.</span></span>

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="Snímek obrazovky se strojového učením SMB":::

## <a name="cloudascent-propensity"></a><span data-ttu-id="d0276-149">CloudAscent Propensity</span><span class="sxs-lookup"><span data-stu-id="d0276-149">CloudAscent Propensity</span></span>

<span data-ttu-id="d0276-150">Jak se vytvářejí doporučení pro sklony?</span><span class="sxs-lookup"><span data-stu-id="d0276-150">How are propensity recommendations created?</span></span>

<span data-ttu-id="d0276-151">Pomocí signálů shromážděných prostřednictvím webových prohledávacích systémů a dat poskytovaných z různých zdrojů konsolidujeme firemní data a signály zákazníků ze sociálních sítí.</span><span class="sxs-lookup"><span data-stu-id="d0276-151">Using signals collected via web crawlers and data provided from various sources, we consolidate the firmographics data and customer's social media signals.</span></span>  <span data-ttu-id="d0276-152">Bodování používá tyto signály a data v modelech porovnání pro fitovací a bodovací modely záměru.</span><span class="sxs-lookup"><span data-stu-id="d0276-152">The scoring uses these signals and data in comparison models for fit and scoring models for Intent.</span></span>

1. <span data-ttu-id="d0276-153">Přizpůsobení zákaznického účtu</span><span class="sxs-lookup"><span data-stu-id="d0276-153">Customer Account Fit</span></span>

   - <span data-ttu-id="d0276-154">Interní a externí datové body, které definují pevné údaje.</span><span class="sxs-lookup"><span data-stu-id="d0276-154">Internal and External data points that define firmographics.</span></span>

   - <span data-ttu-id="d0276-155">Bodování fitů používá pro náš nejlepší protokol SMB podobný model, který porovnává zákazníky a zkoumá, jestli se hodí pro cloudové produkty Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="d0276-155">Fit scoring uses a look alike model to our best SMB to compare customers and see if they're a potential  fit for Microsoft Cloud Products.</span></span>

   - <span data-ttu-id="d0276-156">Vyhodnocování fitů se aktualizuje čtvrtletně.</span><span class="sxs-lookup"><span data-stu-id="d0276-156">Fit scoring is updated quarterly</span></span>

2. <span data-ttu-id="d0276-157">Záměr účtu zákazníka</span><span class="sxs-lookup"><span data-stu-id="d0276-157">Customer Account Intent</span></span>

   - <span data-ttu-id="d0276-158">Signály související se sociálních sítěmi a online chováním zákazníka definují záměr.</span><span class="sxs-lookup"><span data-stu-id="d0276-158">Signals related to Social media and a customer's online behavior define Intent.</span></span>

   - <span data-ttu-id="d0276-159">Bodování záměru je překrytí na základě přizpůsobení, aby bylo možné definovat clustery.</span><span class="sxs-lookup"><span data-stu-id="d0276-159">Intent scoring is overlaid on top of fit to define the clusters.</span></span>

   - <span data-ttu-id="d0276-160">Bodování záměru se aktualizuje měsíčně.</span><span class="sxs-lookup"><span data-stu-id="d0276-160">Intent scoring is updated monthly.</span></span>

   :::image type="content" source="images/pci/cust-oppor-5.png" alt-text="CloudAscenté prediktivní modely protokolu SMB.":::

3. <span data-ttu-id="d0276-162">Clustering</span><span class="sxs-lookup"><span data-stu-id="d0276-162">Clustering</span></span>

   <span data-ttu-id="d0276-163">Signály pro přizpůsobení a záměr jsou konsolidovány do skóre clusteringu.</span><span class="sxs-lookup"><span data-stu-id="d0276-163">The Signals for fit and intent are consolidated into a clustering score.</span></span> <span data-ttu-id="d0276-164">CloudAscent má čtyři clustery:</span><span class="sxs-lookup"><span data-stu-id="d0276-164">CloudAscent has four clusters:</span></span>

      - <span data-ttu-id="d0276-165">Zákazníci, kteří jsou nyní připravení k prodeji</span><span class="sxs-lookup"><span data-stu-id="d0276-165">Act Now - sales ready customers</span></span>
      - <span data-ttu-id="d0276-166">Vyhodnocení – zákazníci připravení pro marketing</span><span class="sxs-lookup"><span data-stu-id="d0276-166">Evaluate - marketing ready customers</span></span>
      - <span data-ttu-id="d0276-167">Nurture – kampaně pro osvětu</span><span class="sxs-lookup"><span data-stu-id="d0276-167">Nurture - drive awareness campaigns</span></span>
      - <span data-ttu-id="d0276-168">Vzdělávání – vzdělávání a monitorování pro záměr</span><span class="sxs-lookup"><span data-stu-id="d0276-168">Educate - educate and monitor for intent</span></span>

   <span data-ttu-id="d0276-169">Clustering umožňuje uživatelům zaměřit se na konkrétní zákazníky na prodejní a marketingové iniciativy na základě faktorů segmentů, například: produkt, geografické prostředí, odvětví a vertikální.</span><span class="sxs-lookup"><span data-stu-id="d0276-169">The clustering allows users to target specific customers for sales and marketing initiatives based on segment factors, for example: product, geo, industry and vertical.</span></span>

   <span data-ttu-id="d0276-170">Karta **model PROPER** v sešitech CloudAscent sdílí PROPER a odhadované tržby za prázdných znaků.</span><span class="sxs-lookup"><span data-stu-id="d0276-170">The **Propensity model** tab in the CloudAscent Workbooks shares the propensity and the estimated whitespace revenue.</span></span> <span data-ttu-id="d0276-171">Pokud chcete definovat clustery, které je vhodné a záměr, Projděte si následující kroky:</span><span class="sxs-lookup"><span data-stu-id="d0276-171">To define the clustering of Fit and Intent, we go through the following steps:</span></span>

      1. <span data-ttu-id="d0276-172">Pomocí modelů ML si předem vypočítáme skóre a skóre záměru zákazníka na škále 100.</span><span class="sxs-lookup"><span data-stu-id="d0276-172">Using ML Models, we first calculate Customer Fit Score and intent Score on a scale of 100.</span></span>  <span data-ttu-id="d0276-173">Přesné výsledky se budou lišit v závislosti na modelů ML.</span><span class="sxs-lookup"><span data-stu-id="d0276-173">Exact Scores will vary based on ML Models.</span></span>  <span data-ttu-id="d0276-174">Příklad skóre níže:</span><span class="sxs-lookup"><span data-stu-id="d0276-174">Example Scores Below:</span></span>

         |<span data-ttu-id="d0276-175">**Classification**</span><span class="sxs-lookup"><span data-stu-id="d0276-175">**Classification**</span></span>|<span data-ttu-id="d0276-176">**Podtržítk**</span><span class="sxs-lookup"><span data-stu-id="d0276-176">**Score**</span></span>|
         |---------|:---------|
         |<span data-ttu-id="d0276-177">Vysoká</span><span class="sxs-lookup"><span data-stu-id="d0276-177">High</span></span>|<span data-ttu-id="d0276-178">75 – 100</span><span class="sxs-lookup"><span data-stu-id="d0276-178">75 - 100</span></span>|
         |<span data-ttu-id="d0276-179">Střední</span><span class="sxs-lookup"><span data-stu-id="d0276-179">Medium</span></span>|<span data-ttu-id="d0276-180">55 – 74</span><span class="sxs-lookup"><span data-stu-id="d0276-180">55 - 74</span></span>|
         |<span data-ttu-id="d0276-181">Nízká</span><span class="sxs-lookup"><span data-stu-id="d0276-181">Low</span></span>|<span data-ttu-id="d0276-182">30 - 54</span><span class="sxs-lookup"><span data-stu-id="d0276-182">30 - 54</span></span>|
         |<span data-ttu-id="d0276-183">Velmi nízké</span><span class="sxs-lookup"><span data-stu-id="d0276-183">Very Low</span></span>|<span data-ttu-id="d0276-184">0 - 29</span><span class="sxs-lookup"><span data-stu-id="d0276-184">0 - 29</span></span>|

      2. <span data-ttu-id="d0276-185">Pomocí výše uvedeného pravidla klasifikujeme společnosti tak, aby byly vysoké, střední, nízké a velmi nízké napříč signály Customer Fit i Intent Signals.</span><span class="sxs-lookup"><span data-stu-id="d0276-185">Using the rule above, we classify companies to be High, Medium, Low, and Very Low across both Customer Fit and Intent Signals.</span></span>

      3. <span data-ttu-id="d0276-186">Vykreslujeme signály zákazníka fit a záměr na 2D matici, kde každý průnik představuje sklon.</span><span class="sxs-lookup"><span data-stu-id="d0276-186">We plot customer fit and intent signals on a 2D matrix with each intersection representing the propensity.</span></span> <span data-ttu-id="d0276-187">Příklad: High Fit + High Intent = A1 představující nejvyšší sklon.</span><span class="sxs-lookup"><span data-stu-id="d0276-187">For Example, High Fit + High Intent = A1, representing the highest propensity.</span></span>

      4. <span data-ttu-id="d0276-188">Nakonec se tyto segmenty seskupí do shluků.</span><span class="sxs-lookup"><span data-stu-id="d0276-188">Finally, these segments group to form clusters.</span></span>  <span data-ttu-id="d0276-189">Například cluster Act Now tvoří A1, A2, A3 a A4.</span><span class="sxs-lookup"><span data-stu-id="d0276-189">For Example, A1, A2, A3, A4 form the Act Now cluster.</span></span>

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="Modely CloudAscent.":::

   <span data-ttu-id="d0276-191">Pro tyto zákazníky doporučujeme zacílení na Jednat hned a Vyhodnotit zákazníky.</span><span class="sxs-lookup"><span data-stu-id="d0276-191">For these customers, we recommend targeting Act Now and Evaluate customers.</span></span>

## <a name="cloudascent-products--models"></a><span data-ttu-id="d0276-192">CloudAscent Products & Models</span><span class="sxs-lookup"><span data-stu-id="d0276-192">CloudAscent Products & Models</span></span>

<span data-ttu-id="d0276-193">Následující obrázek poskytuje zobrazení jednotlivých modelů sklonů v CloudAscent:</span><span class="sxs-lookup"><span data-stu-id="d0276-193">The following graphic provides a view of each propensity model within CloudAscent:</span></span>

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="CloudAscent propensity model.":::

<span data-ttu-id="d0276-195">Prázdné modely se skládají z předpovědí pro stávající zákazníky Microsoftu, kteří nemají produkt nebo jsou novými potenciálními zákazníky.</span><span class="sxs-lookup"><span data-stu-id="d0276-195">Whitespace models are composed of predictions for existing Microsoft customers where they don't have a product and/or are net new prospect customers.</span></span>

<span data-ttu-id="d0276-196">Modely upsell používají transakční data k předpovídání potenciálního prodávat v Azure a Microsoft 365 skladových náklady.</span><span class="sxs-lookup"><span data-stu-id="d0276-196">Upsell models use transaction data to predict the potential for upsell in Azure and Microsoft 365 SKUs.</span></span>

<span data-ttu-id="d0276-197">Tito zákazníci už budou mít Azure nebo Microsoft 365 a model pro prodej ukazuje, že si pravděpodobně koupí větší část své stávající SKU.</span><span class="sxs-lookup"><span data-stu-id="d0276-197">These customers will already have both Azure or Microsoft 365 and the upsell model shows that they’re likely to purchase more of their existing SKU.</span></span>

<span data-ttu-id="d0276-198">EOS sdílí zákazníky s EOS (End of Service) pro Win 7, Office 2010, SQL Server a Windows Server.</span><span class="sxs-lookup"><span data-stu-id="d0276-198">EOS shares the end of service (EOS) customers for Win 7, Office 2010, SQL Server, and Windows Server.</span></span> <span data-ttu-id="d0276-199">Data EOS se načtou z MS Sales a přelásní se modelováním sklonu CloudAscent, pokud je k dispozici.</span><span class="sxs-lookup"><span data-stu-id="d0276-199">The EOS data is pulled from MS Sales and overlaid with the CloudAscent propensity modeling where available.</span></span> <span data-ttu-id="d0276-200">Data eOS se nachází v roli Moderní práce a Azure Sales.</span><span class="sxs-lookup"><span data-stu-id="d0276-200">EOS data lives in the Modern Work and Azure Sales plays.</span></span>
