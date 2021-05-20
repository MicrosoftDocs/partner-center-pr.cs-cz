---
title: Fakturace plánu Azure – soubory & faktury
ms.topic: article
ms.date: 05/19/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zjistěte, jak získat přístup k faktuře a struktuře souborů s vyrovnáním a porozumět jim související s fakturací plánu Azure.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 5ab086a4d15d16f094e33d19b81f1c93711916dc
ms.sourcegitcommit: e0444145d7720df948b9d02ae2469206db48dba5
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110201421"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a><span data-ttu-id="484b7-103">Nové obchodní prostředí v CSP – Fakturace Azure</span><span class="sxs-lookup"><span data-stu-id="484b7-103">New commerce experience in CSP - Azure billing</span></span> 

<span data-ttu-id="484b7-104">**Odpovídající role:** Agent pro správu | Správce fakturace | Globální správce</span><span class="sxs-lookup"><span data-stu-id="484b7-104">**Appropriate roles**: Admin agent | Billing admin | Global admin</span></span>

<span data-ttu-id="484b7-105">Tento článek vysvětluje, jak získat přístup k faktuře a struktuře souborů s vyrovnáním související s fakturací plánu Azure a porozumět jim.</span><span class="sxs-lookup"><span data-stu-id="484b7-105">This article explains how to access and understand the invoice and reconciliation file structure related to billing for the Azure plan.</span></span> <span data-ttu-id="484b7-106">Fakturace v rámci plánu Azure je zjednodušené prostředí pro fakturaci s využitím jednotného fakturačního data a kalendářního fakturačního období podle měsíců.</span><span class="sxs-lookup"><span data-stu-id="484b7-106">Billing under the Azure plan is a simplified billing experience using an aligned single billing date and calendar month-based billing period.</span></span>

## <a name="summary-of-billing-essentials"></a><span data-ttu-id="484b7-107">Souhrn základních informací o fakturaci</span><span class="sxs-lookup"><span data-stu-id="484b7-107">Summary of billing essentials</span></span>

- <span data-ttu-id="484b7-108">**Datum faktury:** Soubor faktury a odsouhlasení budou k dispozici Partnerské centrum řídicím panelu nebo rozhraní API do 8. dne (půlnoc v UTC).</span><span class="sxs-lookup"><span data-stu-id="484b7-108">**Invoice date**: Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).</span></span>

- <span data-ttu-id="484b7-109">**Fakturační období faktury:** Fakturační období faktury je v souladu s kalendářním měsícem, například 31. 10. 10. 11. 11. 2011.</span><span class="sxs-lookup"><span data-stu-id="484b7-109">**Invoice billing period**: The invoice billing period is aligned to the calendar month, for example,  10/1-10/31, 11/1-11/30.</span></span>

- <span data-ttu-id="484b7-110">**Období služeb s poplatky:** Poplatky se budou v souladu s kalendářním měsícem.</span><span class="sxs-lookup"><span data-stu-id="484b7-110">**Charge service periods**: Charges will align to the calendar month.</span></span> <span data-ttu-id="484b7-111">Pokud například fakturovaný partner přidá služby Azure prostřednictvím plánu Azure 15. 10. 2015 a zákazník začne 15. 10. 2015 spotřebovat služby Azure, pak fakturovaný partner obdrží fakturu a odsoustavu 8. 11. 10. 2011 pro spotřebu zákazníkům v 10./ 15. 10. 2011.</span><span class="sxs-lookup"><span data-stu-id="484b7-111">For example, if billed partner adds Azure services through an Azure plan on 10/15 and the customer begins consumption of Azure services on 10/15, then billed partner will receive invoice/recon on 11/8 for customer consumption for the service period 10/15 - 10/31.</span></span> <span data-ttu-id="484b7-112">Faktura za následující měsíc, která se vygeneruje 12. 8. 2018, obsahuje všechny poplatky za období služeb od 11. 1. do 31. 11. 2011.</span><span class="sxs-lookup"><span data-stu-id="484b7-112">The next month's invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.</span></span>

- <span data-ttu-id="484b7-113">**Platební období faktury:** Net 60 dnů.</span><span class="sxs-lookup"><span data-stu-id="484b7-113">**Invoice payment term**: Net 60 days.</span></span>

- <span data-ttu-id="484b7-114">Měna **faktury:** Od 28. ledna 2021 budou partneři v oblasti EU/EFTA a Spojeného království, kteří mají nové zákazníky a stávající zákazníky CSP, kteří poprvé kupují nové obchodní nabídky, jejichž tenanti byli vytvořeni před 11. květnem 2020, fakturovat za tyto nákupy v měně umístění partnera.</span><span class="sxs-lookup"><span data-stu-id="484b7-114">**Invoice currency**: Starting January 28th 2021, partners in the EU/EFTA and UK region who have new customers and existing CSP customers purchasing new commerce offers for the first time whose tenants were created prior to 11 May 2020, will be billed for those purchases in partner location currency.</span></span> <span data-ttu-id="484b7-115">Partneři, kteří se nacházejí mimo oblast EU/EFTA a Spojené království, se budou dál fakturovat v měně umístění partnera.</span><span class="sxs-lookup"><span data-stu-id="484b7-115">Partners located outside of the EU/EFTA and UK region will continue to be billed in partner location currency.</span></span>

- <span data-ttu-id="484b7-116">**Pobídky pro partnery:** Placené 45 dnů od konce fakturačního měsíce.</span><span class="sxs-lookup"><span data-stu-id="484b7-116">**Partner incentives**: Paid 45 days from the end of the invoice month.</span></span>

## <a name="access-your-invoices-and-reconciliation-files"></a><span data-ttu-id="484b7-117">Přístup k fakturám a souborům odsouhlasení</span><span class="sxs-lookup"><span data-stu-id="484b7-117">Access your invoices and reconciliation files</span></span>

<span data-ttu-id="484b7-118">Globální správce nebo správce fakturace vaší společnosti obdrží e-mail, jakmile bude faktura připravená k zobrazení.</span><span class="sxs-lookup"><span data-stu-id="484b7-118">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span>

<span data-ttu-id="484b7-119">Přístup k faktuře a souboru s vyrovnáním:</span><span class="sxs-lookup"><span data-stu-id="484b7-119">To access the invoice and reconciliation file:</span></span>

1. <span data-ttu-id="484b7-120">Přihlaste se k [řídicímu panelu](https://partner.microsoft.com/dashboard/) pro Partnerské centrum.</span><span class="sxs-lookup"><span data-stu-id="484b7-120">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="484b7-121">V nabídce partnerského centra vyberte **fakturace**.</span><span class="sxs-lookup"><span data-stu-id="484b7-121">From the Partner Center menu, select **Billing**.</span></span>

3. <span data-ttu-id="484b7-122">Vyberte kartu pro **opakovanou** a **jednorázovou** a měnu, které vás zajímají.</span><span class="sxs-lookup"><span data-stu-id="484b7-122">Select the tab for the **Recurring** and **One-time** and the currency you are interested in.</span></span>

   :::image type="content" source="images/azure/billing3.png" alt-text="fakturované":::

4. <span data-ttu-id="484b7-124">Vyberte soubor **faktury** nebo **souboru k odsouhlasení**.</span><span class="sxs-lookup"><span data-stu-id="484b7-124">Select **Invoice** or **Reconciliation file**.</span></span>  

   <span data-ttu-id="484b7-125">Chcete-li zobrazit historické faktury a soubory rekognoskaci, rozbalte řádek historie fakturace níže.</span><span class="sxs-lookup"><span data-stu-id="484b7-125">To view historical invoices and recon files expand the Billing history row below.</span></span>

## <a name="understanding-usage-data"></a><span data-ttu-id="484b7-126">Seznámení s daty o využití</span><span class="sxs-lookup"><span data-stu-id="484b7-126">Understanding usage data</span></span> 

1. <span data-ttu-id="484b7-127">Plán Azure je kořenový adresář nebo kontejner nejvyšší úrovně pro použití.</span><span class="sxs-lookup"><span data-stu-id="484b7-127">Azure plan is the root or top-level container for usage.</span></span> <span data-ttu-id="484b7-128">Veškeré využití je vázané zpátky na jeden plán Azure.</span><span class="sxs-lookup"><span data-stu-id="484b7-128">All usage is tied back to a single Azure plan.</span></span>

2. <span data-ttu-id="484b7-129">V rámci plánu bude k dispozici jedno nebo několik předplatných Azure.</span><span class="sxs-lookup"><span data-stu-id="484b7-129">Within a plan, there will be one or more Azure subscriptions.</span></span> <span data-ttu-id="484b7-130">Jedná se o kontejnery používané pro správu a nasazení prostředků.</span><span class="sxs-lookup"><span data-stu-id="484b7-130">These are containers used for resource management and deployment.</span></span> 

3. <span data-ttu-id="484b7-131">V rámci předplatného se skupiny prostředků přidávají do skupin prostředků.</span><span class="sxs-lookup"><span data-stu-id="484b7-131">Within a subscription, resource groups add to group resources.</span></span> <span data-ttu-id="484b7-132">Všechny prostředky se nasazují do jedné skupiny prostředků.</span><span class="sxs-lookup"><span data-stu-id="484b7-132">Every resource is deployed to one resource group.</span></span> 

4. <span data-ttu-id="484b7-133">Mezi příklady prostředků patří virtuální počítače a účty úložiště.</span><span class="sxs-lookup"><span data-stu-id="484b7-133">Examples of resources include virtual machines and storage accounts.</span></span> 

5. <span data-ttu-id="484b7-134">Měřiče emitování prostředků: měřiče měří spotřebu prostředku a jeden prostředek může vysílat využití pro více měřičů.</span><span class="sxs-lookup"><span data-stu-id="484b7-134">Resource emit meters: Meters are measurements of consumption of a resource, and one resource may emit usage for multiple meters.</span></span> <span data-ttu-id="484b7-135">Měřiče jsou označeny ProductId, SKUId a AvailabilityId.</span><span class="sxs-lookup"><span data-stu-id="484b7-135">Meters are identified by a ProductId, SKUId, and AvailabilityId.</span></span> 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a><span data-ttu-id="484b7-136">Hierarchie skupin prostředků předplatného a měření</span><span class="sxs-lookup"><span data-stu-id="484b7-136">Hierarchy of subscription resource groups and metering</span></span>

<span data-ttu-id="484b7-137">**Účet Azure (tenant)**</span><span class="sxs-lookup"><span data-stu-id="484b7-137">**Azure account (tenant)**</span></span>

- <span data-ttu-id="484b7-138">Předplatné A</span><span class="sxs-lookup"><span data-stu-id="484b7-138">Subscription A</span></span>
    - <span data-ttu-id="484b7-139">Zdroj dat 1</span><span class="sxs-lookup"><span data-stu-id="484b7-139">ResourceGroup 1</span></span>
        - <span data-ttu-id="484b7-140">Virtuální počítač (prostředek)</span><span class="sxs-lookup"><span data-stu-id="484b7-140">Virtual machine (resource)</span></span>
            - <span data-ttu-id="484b7-141">Měřič výpočetních prostředků</span><span class="sxs-lookup"><span data-stu-id="484b7-141">Compute meter</span></span>
        - <span data-ttu-id="484b7-142">Virtuální síť (prostředek)</span><span class="sxs-lookup"><span data-stu-id="484b7-142">Virtual network (resource)</span></span>
            - <span data-ttu-id="484b7-143">Bez fakturačního měřiče</span><span class="sxs-lookup"><span data-stu-id="484b7-143">No billing meter</span></span>

    - <span data-ttu-id="484b7-144">ResourceGroup 2</span><span class="sxs-lookup"><span data-stu-id="484b7-144">ResourceGroup 2</span></span>
        - <span data-ttu-id="484b7-145">Virtuální počítač (prostředek)</span><span class="sxs-lookup"><span data-stu-id="484b7-145">Virtual machine (resource)</span></span>
            - <span data-ttu-id="484b7-146">Měřič počítače</span><span class="sxs-lookup"><span data-stu-id="484b7-146">Computer meter</span></span>
        - <span data-ttu-id="484b7-147">SSD úrovně Premium spravovaný disk (prostředek)</span><span class="sxs-lookup"><span data-stu-id="484b7-147">Premium SSD-managed disk (resource)</span></span>
            - <span data-ttu-id="484b7-148">Měřič kapacity úložiště</span><span class="sxs-lookup"><span data-stu-id="484b7-148">Storage capacity meter</span></span>
            - <span data-ttu-id="484b7-149">Měřič operací úložiště</span><span class="sxs-lookup"><span data-stu-id="484b7-149">Storage operations meter</span></span>

- <span data-ttu-id="484b7-150">Předplatné B -ResourceGroup 1 – Azure SQL (prostředek) – měřič DTU – VPN Gateway (prostředek) – měřič brány VPN</span><span class="sxs-lookup"><span data-stu-id="484b7-150">Subscription B   -ResourceGroup 1       - Azure SQL (resource)           - DTU meter       - VPN Gateway (resource)           - VPN gateway meter</span></span>

    - <span data-ttu-id="484b7-151">ResourceGroup 2</span><span class="sxs-lookup"><span data-stu-id="484b7-151">ResourceGroup 2</span></span>
        - <span data-ttu-id="484b7-152">Virtual Network rozhraní (prostředek)</span><span class="sxs-lookup"><span data-stu-id="484b7-152">Virtual Network Interface (resource)</span></span>
            - <span data-ttu-id="484b7-153">Bez fakturačního měřiče</span><span class="sxs-lookup"><span data-stu-id="484b7-153">No billing meter</span></span>

## <a name="read-the-invoice"></a><span data-ttu-id="484b7-154">Čtení faktury</span><span class="sxs-lookup"><span data-stu-id="484b7-154">Read the invoice</span></span>

1. <span data-ttu-id="484b7-155">Faktura bude k dispozici nejpozději do 8. dne každého měsíce.</span><span class="sxs-lookup"><span data-stu-id="484b7-155">Invoice will be available no later than the eighth of each month.</span></span>

2. <span data-ttu-id="484b7-156">Partneři mají na úhradu 60 dnů.</span><span class="sxs-lookup"><span data-stu-id="484b7-156">Partners have 60 days to remit payment.</span></span>

3. <span data-ttu-id="484b7-157">Fakturační období bude pokrývat daný kalendářní měsíc, například 31. 10. 10. 10.</span><span class="sxs-lookup"><span data-stu-id="484b7-157">The billing period will cover a given calendar month, for example, 10/1-10/31.</span></span>

4. <span data-ttu-id="484b7-158">Poplatky se netýkají úprav (částka je bez "kreditu získaného partnerem za spravované služby").</span><span class="sxs-lookup"><span data-stu-id="484b7-158">Charges are net of adjustments (amount is net of “Partner earned credit for services managed").</span></span>

5. <span data-ttu-id="484b7-159">Další podrobnosti o fakturaci najdete v souboru s vyúčtováním faktur a souboru s denním hodnocením využití.</span><span class="sxs-lookup"><span data-stu-id="484b7-159">Review the invoice recon file and daily rated usage file for additional billing details.</span></span>

   :::image type="content" source="images/azure/invoice1.png" alt-text="Faktury":::

## <a name="read-the-invoice-reconciliation-file"></a><span data-ttu-id="484b7-161">Přečtěte si soubor odsouhlasení faktury</span><span class="sxs-lookup"><span data-stu-id="484b7-161">Read the invoice reconciliation file</span></span>

1. <span data-ttu-id="484b7-162">Každá kombinace plánu a měření Azure může mít až dva fakturační řádky v souboru rekognoskaci.</span><span class="sxs-lookup"><span data-stu-id="484b7-162">Each Azure plan and meter combination may have up to two billing lines on the recon file.</span></span>

2. <span data-ttu-id="484b7-163">Pokud je měřič kvalifikován pro jakýkoli typ slevy nebo kreditu (například vrstvené slevy nebo získaný kredit partnerských služeb) v celém kalendářním měsíci, bude soubor rekognoskaci obsahovat jenom jednu fakturační fakturu.</span><span class="sxs-lookup"><span data-stu-id="484b7-163">If the meter qualified for any type of discount or credit (such as tiered discounts or the Partner earned credit for services managed) throughout the entire calendar month, then the recon file will only contain one billing line.</span></span> <span data-ttu-id="484b7-164">Na sloupec **PriceAdjusmentDescription** se odkazuje na slevový nebo získaný kredit.</span><span class="sxs-lookup"><span data-stu-id="484b7-164">The column **PriceAdjusmentDescription** will reference the discount or earned credit.</span></span>

3. <span data-ttu-id="484b7-165">Pokud nejsou k dispozici žádné prostředky pro konkrétní měřič, který je kvalifikován pro zlevněný kredit nebo úvěr získaný pro partnery, bude soubor rekognoskaci obsahovat jenom jednu fakturační fakturu a skutečná Jednotková cena bude maloobchodní cena (což je jednotková cena).</span><span class="sxs-lookup"><span data-stu-id="484b7-165">If there are no resources for a particular meter that qualified for discount or partner earned credit, then the recon file will only contain one billing line and the effective unit price will be the retail price (which is the unit price).</span></span>

4. <span data-ttu-id="484b7-166">Pokud měřič nebo všechny prostředky, které tento měřič vyvolaly, jsou určené pro kredity, které jsou pro **služby spravované** pro část měsíce, a soubor rekognoskaci bude obsahovat dva fakturační řádky.</span><span class="sxs-lookup"><span data-stu-id="484b7-166">If the meter, or any resources emitting that meter, qualified for **Partner earned credit for services managed** for a part of the month, the recon file will contain two billing lines.</span></span> <span data-ttu-id="484b7-167">Jeden řádek bude představovat dny, ve kterých je měřený měřič, a druhý řádek bude představovat dny, které měřič nezpůsobil.</span><span class="sxs-lookup"><span data-stu-id="484b7-167">One line will represent the days the meter qualified and the second line will represent the days the meter did not qualify.</span></span>

>[!NOTE]
><span data-ttu-id="484b7-168">Můžete sjednotit využití Azure v jednorázovém souboru rekognoskaci nákupu.</span><span class="sxs-lookup"><span data-stu-id="484b7-168">You can reconcile your Azure consumption in your one-time purchase recon file.</span></span> <span data-ttu-id="484b7-169">Provedete to tak, že přejdete na denní hodnocený soubor rekognoskaci využití a vyhledáte ID předplatného.</span><span class="sxs-lookup"><span data-stu-id="484b7-169">To do this, go to your daily-rated usage recon file and search for your SubscriptionID.</span></span> <span data-ttu-id="484b7-170">Zobrazí se všechny náklady spojené s vaším ID plánu Azure.</span><span class="sxs-lookup"><span data-stu-id="484b7-170">This will display all costs associated with your Azure Plan ID.</span></span> <span data-ttu-id="484b7-171">Vaše ID předplatného Azure se zobrazuje jako EntitlementID.</span><span class="sxs-lookup"><span data-stu-id="484b7-171">Your Azure SubscriptionID is shown as the EntitlementID.</span></span>

## <a name="read-the-daily-usage-file"></a><span data-ttu-id="484b7-172">Přečtěte si soubor denního využití.</span><span class="sxs-lookup"><span data-stu-id="484b7-172">Read the daily usage file</span></span>

- <span data-ttu-id="484b7-173">Měřiče předplatného v rámci plánu Azure jsou ohodnocené a každý den se každoročně kumulovaná.</span><span class="sxs-lookup"><span data-stu-id="484b7-173">Subscription meters under an Azure plan are rated, and are cumulated, on a daily basis.</span></span>

- <span data-ttu-id="484b7-174">**Získaný kredit partnerů pro spravované služby** je stanoven a použit každý den.</span><span class="sxs-lookup"><span data-stu-id="484b7-174">**Partner earned credit for services managed** is determined and applied on a daily basis.</span></span>

- <span data-ttu-id="484b7-175">Každý měřič předplatného bude mít řádek pro každý den v měsíci, kde byla spotřebována spotřeba.</span><span class="sxs-lookup"><span data-stu-id="484b7-175">Every subscription meter will have a row for every day of the month where there was consumption.</span></span>

- <span data-ttu-id="484b7-176">V následujícím příkladu:</span><span class="sxs-lookup"><span data-stu-id="484b7-176">In the example below:</span></span>

  - <span data-ttu-id="484b7-177">Pro měření pro **služby spravované** z 7/1-7/3 se měří pro daný kredit. (Poznámka: efektivní Jednotková cena je maloobchodní cena nižší než partner získaný.</span><span class="sxs-lookup"><span data-stu-id="484b7-177">Meter qualified for **Partner earned credit for services managed** from 7/1 - 7/3 (note the effective unit price is retail price less partner earned credit.</span></span>

  - <span data-ttu-id="484b7-178">U služeb spravovaných z 7/4-7/7 se nezpůsobilo měření pro kredity, které jsou **pro služby spravované** . (Poznámka: efektivní Jednotková cena je maloobchodní cena).</span><span class="sxs-lookup"><span data-stu-id="484b7-178">Meter didn't qualify for **Partner earned credit for services managed** from 7/4 - 7/7 (note the effective unit price is retail price).</span></span>

  - <span data-ttu-id="484b7-179">Měřič kvalifikovaný pro **kredit získaný** partnerem pro služby spravované od 7/8 do 7/31 (všimněte si, že efektivní jednotková cena je maloobchodní cena menší než kredit získaný partnerem).</span><span class="sxs-lookup"><span data-stu-id="484b7-179">Meter qualified for **Partner earned credit for services managed** from 7/8 - 7/31 (note the effective unit price is retail price less partner earned credit).</span></span>

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2":::

## <a name="invoice-in-customer-currency"></a><span data-ttu-id="484b7-181">Faktura v měně zákazníka</span><span class="sxs-lookup"><span data-stu-id="484b7-181">Invoice in customer currency</span></span>

<span data-ttu-id="484b7-182">Služby Azure prostřednictvím plánu Azure se budou účtovat v USD a fakturují se v měně přiřazené zemi zákazníka.</span><span class="sxs-lookup"><span data-stu-id="484b7-182">Azure services through an Azure plan will be priced in USD and billed in the customer country assigned currency.</span></span> <span data-ttu-id="484b7-183">Pokud je fakturační měna mimo USD, použitá sazba devizové výměny (FX) se zobrazí na poslední stránce faktury.</span><span class="sxs-lookup"><span data-stu-id="484b7-183">If the billing currency is non-USD, then the Foreign exchange (FX) rate used will be shown on the last page of the invoice.</span></span> <span data-ttu-id="484b7-184">Směnné kurzy se určují měsíčně a použijí se na následující faktuře.</span><span class="sxs-lookup"><span data-stu-id="484b7-184">FX rates are determined monthly and applied to the following invoice.</span></span> <span data-ttu-id="484b7-185">Úplný seznam měn zemí najdete v nových obchodních nabídek pro země dostupnosti a [v matici měn zákazníků.](https://go.microsoft.com/fwlink/?linkid=2112354)</span><span class="sxs-lookup"><span data-stu-id="484b7-185">For a full list of country currencies, please view the [new commerce offers country availability and customer currency matrix](https://go.microsoft.com/fwlink/?linkid=2112354).</span></span>

<span data-ttu-id="484b7-186">Microsoft se za převod řídí londýnské burzovní burzy.</span><span class="sxs-lookup"><span data-stu-id="484b7-186">Microsoft follows the London Stock Exchange for conversion.</span></span> <span data-ttu-id="484b7-187">Používáme směnný kurz, který se rovná směnné sazbě zaznamenané k poslední sekundě posledního obchodního dne v měsíci na londýnské burze.</span><span class="sxs-lookup"><span data-stu-id="484b7-187">We use the exchange rate, which is equal to the exchange rate captured on the last second of the last business day of the month on the London Stock Exchange.</span></span> <span data-ttu-id="484b7-188">Sazby FX se aktualizují a budou k dispozici den před prvním měsícem, pro který platí.</span><span class="sxs-lookup"><span data-stu-id="484b7-188">The FX rates will be refreshed and available on the day before the first of the month for which they apply.</span></span>

## <a name="azure-reservations"></a><span data-ttu-id="484b7-189">Rezervace Azure</span><span class="sxs-lookup"><span data-stu-id="484b7-189">Azure reservations</span></span>


<span data-ttu-id="484b7-190">Pokud [nakupujete rezervace Azure](azure-reservations.md) prostřednictvím plánu Azure, můžete zvolit buď jednou, nebo měsíční fakturaci.</span><span class="sxs-lookup"><span data-stu-id="484b7-190">If purchasing [Azure reservations](azure-reservations.md) through an Azure plan, you can choose either one-time or monthly billing.</span></span>


## <a name="azure-spending"></a><span data-ttu-id="484b7-191">Útrata v Azure</span><span class="sxs-lookup"><span data-stu-id="484b7-191">Azure spending</span></span>

<span data-ttu-id="484b7-192">Stávající prostředí útraty v Azure se aktualizuje tak, aby podporovalo fakturaci nového plánu Azure v Partnerské centrum.</span><span class="sxs-lookup"><span data-stu-id="484b7-192">The existing Azure spending experience is updated to support the new Azure plan billing in Partner Center.</span></span> <span data-ttu-id="484b7-193">To umožňuje partnerům:</span><span class="sxs-lookup"><span data-stu-id="484b7-193">This enables partners to:</span></span>

- <span data-ttu-id="484b7-194">Zobrazení, správa a příjem upozornění pro rozpočet nastavený na úrovni zákazníka</span><span class="sxs-lookup"><span data-stu-id="484b7-194">View, manage, and receive alerts for budget set at a customer level</span></span> 

- <span data-ttu-id="484b7-195">Zobrazení celkových odhadovaných výdajů v plánu Azure (rozdělené podle prostředků a úrovně měřiče)</span><span class="sxs-lookup"><span data-stu-id="484b7-195">View total estimated spending on an Azure plan (broken down by resource and meter level)</span></span>

<span data-ttu-id="484b7-196">Vzhledem k tomu, že fakturační model pro služby Azure prostřednictvím plánu Azure je spotřeba po platbě, aby se zabránilo vyšším fakturám, než se čekalo, mohou partneři použít měsíční rozpočet a sledovat procento využití.</span><span class="sxs-lookup"><span data-stu-id="484b7-196">Because the billing model for Azure services through an Azure plan is post-pay consumption, to avoid a bigger bill than anticipated, partners can apply a monthly budget and track the percentage of usage.</span></span> <span data-ttu-id="484b7-197">Rozpočet se může použít pro jednoho zákazníka nebo více zákazníků najednou.</span><span class="sxs-lookup"><span data-stu-id="484b7-197">A budget can be applied to one customer or multiple customers at one time.</span></span> 

:::image type="content" source="images/azure/azurespend.png" alt-text="Útrata v Azure":::

## <a name="next-steps"></a><span data-ttu-id="484b7-199">Další kroky</span><span class="sxs-lookup"><span data-stu-id="484b7-199">Next steps</span></span>

- <span data-ttu-id="484b7-200">Podívejte se, jak se počítá kredit získaný partnerem (PEC).</span><span class="sxs-lookup"><span data-stu-id="484b7-200">See how the partner earned credit (PEC) is calculated.</span></span> <span data-ttu-id="484b7-201">Přihlaste se k Partnerské centrum [řídicího panelu a](https://partner.microsoft.com/dashboard/) vyhledejte ceník, který je k dispozici.</span><span class="sxs-lookup"><span data-stu-id="484b7-201">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/) and locate the price list available.</span></span>

- <span data-ttu-id="484b7-202">Informace o [nákupu plánu Azure](purchase-azure-plan.md)</span><span class="sxs-lookup"><span data-stu-id="484b7-202">Learn about [purchasing the Azure plan](purchase-azure-plan.md)</span></span>

- <span data-ttu-id="484b7-203">Podívejte se na [ceník pro nové prostředí pro obchod v CSP](azure-plan-price-list.md) .</span><span class="sxs-lookup"><span data-stu-id="484b7-203">See the [price list for the new commerce experience in CSP](azure-plan-price-list.md)</span></span>
