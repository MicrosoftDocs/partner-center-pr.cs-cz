---
title: Fakturace plánu Azure – & soubory rekognoskaci na faktuře
ms.topic: article
ms.date: 01/20/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Naučte se, jak získat přístup ke strukturám souborů faktur a odsouhlasení souvisejících s fakturací za plán Azure.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: e230cc0d8ff3afea4bf2cc7b55d3847814696af6
ms.sourcegitcommit: f99424919f0d77bbe4f44293d84f9ea1e3317f13
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/21/2021
ms.locfileid: "98658429"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a><span data-ttu-id="809a2-103">Nové obchodní prostředí v CSP – Fakturace Azure</span><span class="sxs-lookup"><span data-stu-id="809a2-103">New commerce experience in CSP - Azure billing</span></span> 

<span data-ttu-id="809a2-104">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="809a2-104">**Appropriate roles**</span></span>

- <span data-ttu-id="809a2-105">Agent správce</span><span class="sxs-lookup"><span data-stu-id="809a2-105">Admin agent</span></span>
- <span data-ttu-id="809a2-106">Správce fakturace</span><span class="sxs-lookup"><span data-stu-id="809a2-106">Billing admin</span></span>
- <span data-ttu-id="809a2-107">Globální správce</span><span class="sxs-lookup"><span data-stu-id="809a2-107">Global admin</span></span>

<span data-ttu-id="809a2-108">Tento článek vysvětluje, jak získat přístup ke struktuře souborů fakturace a odsouhlasení souvisejících s fakturací za plán Azure.</span><span class="sxs-lookup"><span data-stu-id="809a2-108">This article explains how to access and understand the invoice and reconciliation file structure related to billing for the Azure plan.</span></span> <span data-ttu-id="809a2-109">Fakturace v rámci plánu Azure je zjednodušené fakturační prostředí s využitím zarovnaných a fakturačních období na základě kalendářního měsíce.</span><span class="sxs-lookup"><span data-stu-id="809a2-109">Billing under the Azure plan is a simplified billing experience using an aligned single billing date and calendar month-based billing period.</span></span>

## <a name="summary-of-billing-essentials"></a><span data-ttu-id="809a2-110">Shrnutí základních informací o fakturaci</span><span class="sxs-lookup"><span data-stu-id="809a2-110">Summary of billing essentials</span></span>

- <span data-ttu-id="809a2-111">**Datum faktury**: soubor fakturace a odsouhlasení bude k dispozici v 8. bodě a řídicím panelu partnerského centra/rozhraní API.</span><span class="sxs-lookup"><span data-stu-id="809a2-111">**Invoice date**: Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).</span></span>

- <span data-ttu-id="809a2-112">**Fakturační období faktury**: fakturační období faktury je zarovnané na kalendářní měsíc, například 10/1-10/31, 11/1-11/30.</span><span class="sxs-lookup"><span data-stu-id="809a2-112">**Invoice billing period**: The invoice billing period is aligned to the calendar month, for example,  10/1-10/31, 11/1-11/30.</span></span>

- <span data-ttu-id="809a2-113">Poplatky **za období služby**: poplatky se budou zarovnávat do kalendářního měsíce.</span><span class="sxs-lookup"><span data-stu-id="809a2-113">**Charge service periods**: Charges will align to the calendar month.</span></span> <span data-ttu-id="809a2-114">Pokud třeba účtováná partner přidá služby Azure prostřednictvím plánu Azure na 10/15 a zákazník začne využívat služby Azure na 10/15, bude vám účtovaný partner dostávat faktury nebo rekognoskaci na 11/8 za spotřebu zákazníka za období služby 10/15-10/31.</span><span class="sxs-lookup"><span data-stu-id="809a2-114">For example, if billed partner adds Azure services through an Azure plan on 10/15 and the customer begins consumption of Azure services on 10/15, then billed partner will receive invoice/recon on 11/8 for customer consumption for the service period 10/15 - 10/31.</span></span> <span data-ttu-id="809a2-115">Faktura za příští měsíc, která se vygeneruje v 12/8, obsahuje všechny poplatky za období služby 11/1-11/31.</span><span class="sxs-lookup"><span data-stu-id="809a2-115">The next month's invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.</span></span>

- <span data-ttu-id="809a2-116">**Platební podmínka faktury**: NET 60 dní.</span><span class="sxs-lookup"><span data-stu-id="809a2-116">**Invoice payment term**: Net 60 days.</span></span>

- <span data-ttu-id="809a2-117">**Měna faktury**: partneři se budou dál účtovat v přiřazené měně zákazníka v country's.</span><span class="sxs-lookup"><span data-stu-id="809a2-117">**Invoice currency**: Partners will continue to be billed in the customer's country's assigned currency.</span></span> <span data-ttu-id="809a2-118">Pokud je například účtovaný partner v Irsku se zákazníky ve Spojeném království, Norsku a Německu, bude se fakturovaná Partnerská adresa GBP, NOK a EUR a rekognoskaci.</span><span class="sxs-lookup"><span data-stu-id="809a2-118">For example, if the billed partner is in Ireland with customers in the UK, Norway, and Germany, then the billed partner will receive a GBP, NOK, and EUR invoice/recon.</span></span>

- <span data-ttu-id="809a2-119">**Pobídky pro partnery**: placené 45 dny od konce měsíce faktury.</span><span class="sxs-lookup"><span data-stu-id="809a2-119">**Partner incentives**: Paid 45 days from the end of the invoice month.</span></span>

## <a name="access-your-invoices-and-reconciliation-files"></a><span data-ttu-id="809a2-120">Přístup k vašim fakturám a souborům pro odsouhlasení</span><span class="sxs-lookup"><span data-stu-id="809a2-120">Access your invoices and reconciliation files</span></span>

<span data-ttu-id="809a2-121">Správce globálního správce nebo fakturace vaší společnosti obdrží e-mail, když je faktura připravena k zobrazení.</span><span class="sxs-lookup"><span data-stu-id="809a2-121">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span>

<span data-ttu-id="809a2-122">Přístup k souboru faktury a odsouhlasení:</span><span class="sxs-lookup"><span data-stu-id="809a2-122">To access the invoice and reconciliation file:</span></span>

1. <span data-ttu-id="809a2-123">Přihlaste se k [řídicímu panelu](https://partner.microsoft.com/dashboard/) pro Partnerské centrum.</span><span class="sxs-lookup"><span data-stu-id="809a2-123">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="809a2-124">V nabídce partnerského centra vyberte **fakturace**.</span><span class="sxs-lookup"><span data-stu-id="809a2-124">From the Partner Center menu, select **Billing**.</span></span>

3. <span data-ttu-id="809a2-125">Vyberte kartu pro **opakovanou** a **jednorázovou** a měnu, které vás zajímají.</span><span class="sxs-lookup"><span data-stu-id="809a2-125">Select the tab for the **Recurring** and **One-time** and the currency you are interested in.</span></span>

   :::image type="content" source="images/azure/billing3.png" alt-text="fakturované":::

4. <span data-ttu-id="809a2-127">Vyberte soubor **faktury** nebo **souboru k odsouhlasení**.</span><span class="sxs-lookup"><span data-stu-id="809a2-127">Select **Invoice** or **Reconciliation file**.</span></span>  

   <span data-ttu-id="809a2-128">Chcete-li zobrazit historické faktury a soubory rekognoskaci, rozbalte řádek historie fakturace níže.</span><span class="sxs-lookup"><span data-stu-id="809a2-128">To view historical invoices and recon files expand the Billing history row below.</span></span>

## <a name="understanding-usage-data"></a><span data-ttu-id="809a2-129">Seznámení s daty o využití</span><span class="sxs-lookup"><span data-stu-id="809a2-129">Understanding usage data</span></span> 

1. <span data-ttu-id="809a2-130">Plán Azure je kořenový adresář nebo kontejner nejvyšší úrovně pro použití.</span><span class="sxs-lookup"><span data-stu-id="809a2-130">Azure plan is the root or top-level container for usage.</span></span> <span data-ttu-id="809a2-131">Veškeré využití je vázané zpátky na jeden plán Azure.</span><span class="sxs-lookup"><span data-stu-id="809a2-131">All usage is tied back to a single Azure plan.</span></span>

2. <span data-ttu-id="809a2-132">V rámci plánu bude k dispozici jedno nebo několik předplatných Azure.</span><span class="sxs-lookup"><span data-stu-id="809a2-132">Within a plan, there will be one or more Azure subscriptions.</span></span> <span data-ttu-id="809a2-133">Jedná se o kontejnery používané pro správu a nasazení prostředků.</span><span class="sxs-lookup"><span data-stu-id="809a2-133">These are containers used for resource management and deployment.</span></span> 

3. <span data-ttu-id="809a2-134">V rámci předplatného se skupiny prostředků přidávají do skupin prostředků.</span><span class="sxs-lookup"><span data-stu-id="809a2-134">Within a subscription, resource groups add to group resources.</span></span> <span data-ttu-id="809a2-135">Všechny prostředky se nasazují do jedné skupiny prostředků.</span><span class="sxs-lookup"><span data-stu-id="809a2-135">Every resource is deployed to one resource group.</span></span> 

4. <span data-ttu-id="809a2-136">Mezi příklady prostředků patří virtuální počítače a účty úložiště.</span><span class="sxs-lookup"><span data-stu-id="809a2-136">Examples of resources include virtual machines and storage accounts.</span></span> 

5. <span data-ttu-id="809a2-137">Měřiče emitování prostředků: měřiče měří spotřebu prostředku a jeden prostředek může vysílat využití pro více měřičů.</span><span class="sxs-lookup"><span data-stu-id="809a2-137">Resource emit meters: Meters are measurements of consumption of a resource, and one resource may emit usage for multiple meters.</span></span> <span data-ttu-id="809a2-138">Měřiče jsou označeny ProductId, SKUId a AvailabilityId.</span><span class="sxs-lookup"><span data-stu-id="809a2-138">Meters are identified by a ProductId, SKUId, and AvailabilityId.</span></span> 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a><span data-ttu-id="809a2-139">Hierarchie skupin prostředků předplatného a měření</span><span class="sxs-lookup"><span data-stu-id="809a2-139">Hierarchy of subscription resource groups and metering</span></span>

<span data-ttu-id="809a2-140">**Účet Azure (tenant)**</span><span class="sxs-lookup"><span data-stu-id="809a2-140">**Azure account (tenant)**</span></span>

- <span data-ttu-id="809a2-141">Předplatné A</span><span class="sxs-lookup"><span data-stu-id="809a2-141">Subscription A</span></span>
    - <span data-ttu-id="809a2-142">Zdroj dat 1</span><span class="sxs-lookup"><span data-stu-id="809a2-142">ResourceGroup 1</span></span>
        - <span data-ttu-id="809a2-143">Virtuální počítač (prostředek)</span><span class="sxs-lookup"><span data-stu-id="809a2-143">Virtual machine (resource)</span></span>
            - <span data-ttu-id="809a2-144">Výpočetní měření</span><span class="sxs-lookup"><span data-stu-id="809a2-144">Compute meter</span></span>
        - <span data-ttu-id="809a2-145">Virtuální síť (prostředek)</span><span class="sxs-lookup"><span data-stu-id="809a2-145">Virtual network (resource)</span></span>
            - <span data-ttu-id="809a2-146">Žádný měřič fakturace</span><span class="sxs-lookup"><span data-stu-id="809a2-146">No billing meter</span></span>

    - <span data-ttu-id="809a2-147">Zdroj dat 2</span><span class="sxs-lookup"><span data-stu-id="809a2-147">ResourceGroup 2</span></span>
        - <span data-ttu-id="809a2-148">Virtuální počítač (prostředek)</span><span class="sxs-lookup"><span data-stu-id="809a2-148">Virtual machine (resource)</span></span>
            - <span data-ttu-id="809a2-149">Měřič počítačů</span><span class="sxs-lookup"><span data-stu-id="809a2-149">Computer meter</span></span>
        - <span data-ttu-id="809a2-150">SSD úrovně Premium spravovaný disk (prostředek)</span><span class="sxs-lookup"><span data-stu-id="809a2-150">Premium SSD-managed disk (resource)</span></span>
            - <span data-ttu-id="809a2-151">Měřič kapacity úložiště</span><span class="sxs-lookup"><span data-stu-id="809a2-151">Storage capacity meter</span></span>
            - <span data-ttu-id="809a2-152">Měřič operací úložiště</span><span class="sxs-lookup"><span data-stu-id="809a2-152">Storage operations meter</span></span>

- <span data-ttu-id="809a2-153">Předplatné B-kategorie prostředků 1 – Azure SQL (prostředek) – měřič DTU – VPN Gateway (prostředek) – měřič brány VPN</span><span class="sxs-lookup"><span data-stu-id="809a2-153">Subscription B   -ResourceGroup 1       - Azure SQL (resource)           - DTU meter       - VPN Gateway (resource)           - VPN gateway meter</span></span>

    - <span data-ttu-id="809a2-154">Zdroj dat 2</span><span class="sxs-lookup"><span data-stu-id="809a2-154">ResourceGroup 2</span></span>
        - <span data-ttu-id="809a2-155">Virtual Network rozhraní (prostředek)</span><span class="sxs-lookup"><span data-stu-id="809a2-155">Virtual Network Interface (resource)</span></span>
            - <span data-ttu-id="809a2-156">Žádný měřič fakturace</span><span class="sxs-lookup"><span data-stu-id="809a2-156">No billing meter</span></span>

## <a name="read-the-invoice"></a><span data-ttu-id="809a2-157">Přečtěte si fakturu</span><span class="sxs-lookup"><span data-stu-id="809a2-157">Read the invoice</span></span>

1. <span data-ttu-id="809a2-158">Faktura bude k dispozici později než osmý měsíc v měsíci.</span><span class="sxs-lookup"><span data-stu-id="809a2-158">Invoice will be available no later than the eighth of each month.</span></span>

2. <span data-ttu-id="809a2-159">Partneři mají 60 dní na platbu.</span><span class="sxs-lookup"><span data-stu-id="809a2-159">Partners have 60 days to remit payment.</span></span>

3. <span data-ttu-id="809a2-160">Fakturační období bude pokrývat určitý kalendářní měsíc, například 10/1-10/31.</span><span class="sxs-lookup"><span data-stu-id="809a2-160">The billing period will cover a given calendar month, for example, 10/1-10/31.</span></span>

4. <span data-ttu-id="809a2-161">Poplatky jsou očištěné od úprav (množství je netto "získaným partnerským kreditem pro spravované služby").</span><span class="sxs-lookup"><span data-stu-id="809a2-161">Charges are net of adjustments (amount is net of “Partner earned credit for services managed").</span></span>

5. <span data-ttu-id="809a2-162">Další informace o fakturaci najdete v souboru rekognoskaci faktury a v souboru denního hodnocení využití.</span><span class="sxs-lookup"><span data-stu-id="809a2-162">Review the invoice recon file and daily rated usage file for additional billing details.</span></span>

   :::image type="content" source="images/azure/invoice1.png" alt-text="faktur":::

## <a name="read-the-invoice-reconciliation-file"></a><span data-ttu-id="809a2-164">Přečtěte si soubor odsouhlasení faktury</span><span class="sxs-lookup"><span data-stu-id="809a2-164">Read the invoice reconciliation file</span></span>

1. <span data-ttu-id="809a2-165">Každá kombinace plánu a měření Azure může mít až dva fakturační řádky v souboru rekognoskaci.</span><span class="sxs-lookup"><span data-stu-id="809a2-165">Each Azure plan and meter combination may have up to two billing lines on the recon file.</span></span>

2. <span data-ttu-id="809a2-166">Pokud je měřič kvalifikován pro jakýkoli typ slevy nebo kreditu (například vrstvené slevy nebo získaný kredit partnerských služeb) v celém kalendářním měsíci, bude soubor rekognoskaci obsahovat jenom jednu fakturační fakturu.</span><span class="sxs-lookup"><span data-stu-id="809a2-166">If the meter qualified for any type of discount or credit (such as tiered discounts or the Partner earned credit for services managed) throughout the entire calendar month, then the recon file will only contain one billing line.</span></span> <span data-ttu-id="809a2-167">Na sloupec **PriceAdjusmentDescription** se odkazuje na slevový nebo získaný kredit.</span><span class="sxs-lookup"><span data-stu-id="809a2-167">The column **PriceAdjusmentDescription** will reference the discount or earned credit.</span></span>

3. <span data-ttu-id="809a2-168">Pokud nejsou k dispozici žádné prostředky pro konkrétní měřič, který je kvalifikován pro zlevněný kredit nebo úvěr získaný pro partnery, bude soubor rekognoskaci obsahovat jenom jednu fakturační fakturu a skutečná Jednotková cena bude maloobchodní cena (což je jednotková cena).</span><span class="sxs-lookup"><span data-stu-id="809a2-168">If there are no resources for a particular meter that qualified for discount or partner earned credit, then the recon file will only contain one billing line and the effective unit price will be the retail price (which is the unit price).</span></span>

4. <span data-ttu-id="809a2-169">Pokud měřič nebo všechny prostředky, které tento měřič vyvolaly, jsou určené pro kredity, které jsou pro **služby spravované** pro část měsíce, a soubor rekognoskaci bude obsahovat dva fakturační řádky.</span><span class="sxs-lookup"><span data-stu-id="809a2-169">If the meter, or any resources emitting that meter, qualified for **Partner earned credit for services managed** for a part of the month, the recon file will contain two billing lines.</span></span> <span data-ttu-id="809a2-170">Jeden řádek bude představovat dny, ve kterých je měřený měřič, a druhý řádek bude představovat dny, které měřič nezpůsobil.</span><span class="sxs-lookup"><span data-stu-id="809a2-170">One line will represent the days the meter qualified and the second line will represent the days the meter did not qualify.</span></span>

## <a name="read-the-daily-usage-file"></a><span data-ttu-id="809a2-171">Přečtěte si soubor denního využití.</span><span class="sxs-lookup"><span data-stu-id="809a2-171">Read the daily usage file</span></span>

- <span data-ttu-id="809a2-172">Měřiče předplatného v rámci plánu Azure jsou ohodnocené a každý den se každoročně kumulovaná.</span><span class="sxs-lookup"><span data-stu-id="809a2-172">Subscription meters under an Azure plan are rated, and are cumulated, on a daily basis.</span></span>

- <span data-ttu-id="809a2-173">**Získaný kredit partnerů pro spravované služby** je stanoven a použit každý den.</span><span class="sxs-lookup"><span data-stu-id="809a2-173">**Partner earned credit for services managed** is determined and applied on a daily basis.</span></span>

- <span data-ttu-id="809a2-174">Každý měřič předplatného bude mít řádek pro každý den v měsíci, kde byla spotřebována spotřeba.</span><span class="sxs-lookup"><span data-stu-id="809a2-174">Every subscription meter will have a row for every day of the month where there was consumption.</span></span>

- <span data-ttu-id="809a2-175">V následujícím příkladu:</span><span class="sxs-lookup"><span data-stu-id="809a2-175">In the example below:</span></span>

  - <span data-ttu-id="809a2-176">Pro měření pro **služby spravované** z 7/1-7/3 se měří pro daný kredit. (Poznámka: efektivní Jednotková cena je maloobchodní cena nižší než partner získaný.</span><span class="sxs-lookup"><span data-stu-id="809a2-176">Meter qualified for **Partner earned credit for services managed** from 7/1 - 7/3 (note the effective unit price is retail price less partner earned credit.</span></span>

  - <span data-ttu-id="809a2-177">U služeb spravovaných z 7/4-7/7 se nezpůsobilo měření pro kredity, které jsou **pro služby spravované** . (Poznámka: efektivní Jednotková cena je maloobchodní cena).</span><span class="sxs-lookup"><span data-stu-id="809a2-177">Meter didn't qualify for **Partner earned credit for services managed** from 7/4 - 7/7 (note the effective unit price is retail price).</span></span>

  - <span data-ttu-id="809a2-178">Pro měřený **kredit pro služby spravované** z 7/8-7/31 se měří na měřič. (Poznámka: efektivní Jednotková cena je cenově dosažená za maloobchodní cenu, která je nižší než partnerský.</span><span class="sxs-lookup"><span data-stu-id="809a2-178">Meter qualified for **Partner earned credit for services managed** from 7/8 - 7/31 (note the effective unit price is retail price less partner earned credit).</span></span>

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2":::

## <a name="invoice-in-customer-currency"></a><span data-ttu-id="809a2-180">Faktura v měně zákazníka</span><span class="sxs-lookup"><span data-stu-id="809a2-180">Invoice in customer currency</span></span>

<span data-ttu-id="809a2-181">Ceny služeb Azure v rámci plánu Azure budou platit v USD a budou se fakturovat v přiřazené měně země zákazníka.</span><span class="sxs-lookup"><span data-stu-id="809a2-181">Azure services through an Azure plan will be priced in USD and billed in the customer country assigned currency.</span></span> <span data-ttu-id="809a2-182">Pokud fakturační měna není USD, zobrazí se na poslední stránce faktury použitá sazba za cizí Exchange (FX).</span><span class="sxs-lookup"><span data-stu-id="809a2-182">If the billing currency is non-USD, then the Foreign exchange (FX) rate used will be shown on the last page of the invoice.</span></span> <span data-ttu-id="809a2-183">Sazby za FX se určují měsíčně a platí pro následující fakturu.</span><span class="sxs-lookup"><span data-stu-id="809a2-183">FX rates are determined monthly and applied to the following invoice.</span></span> <span data-ttu-id="809a2-184">Úplný seznam měn za země najdete v části [Nová obchodní oddělení nabídky dostupnost země a měna zákazníka](https://go.microsoft.com/fwlink/?linkid=2112354).</span><span class="sxs-lookup"><span data-stu-id="809a2-184">For a full list of country currencies, please view the [new commerce offers country availability and customer currency matrix](https://go.microsoft.com/fwlink/?linkid=2112354).</span></span>

<span data-ttu-id="809a2-185">Microsoft dodržuje při konverzi burzovní sklad s Londýn.</span><span class="sxs-lookup"><span data-stu-id="809a2-185">Microsoft follows the London Stock Exchange for conversion.</span></span> <span data-ttu-id="809a2-186">Používáme směnný kurz, který se rovná směnnému kurzu zaznamenanému za poslední sekundu posledního pracovního dne v měsíci na burze cenných papírů v Londýně.</span><span class="sxs-lookup"><span data-stu-id="809a2-186">We use the exchange rate, which is equal to the exchange rate captured on the last second of the last business day of the month on the London Stock Exchange.</span></span> <span data-ttu-id="809a2-187">Sazby za FX budou aktualizovány a k dispozici v den před prvním dnem v měsíci, pro které se vztahují.</span><span class="sxs-lookup"><span data-stu-id="809a2-187">The FX rates will be refreshed and available on the day before the first of the month for which they apply.</span></span>

## <a name="azure-reservations"></a><span data-ttu-id="809a2-188">Rezervace Azure</span><span class="sxs-lookup"><span data-stu-id="809a2-188">Azure reservations</span></span>


<span data-ttu-id="809a2-189">Při nákupu [rezervací Azure](azure-reservations.md) prostřednictvím plánu Azure si můžete vybrat buď jednorázovou, nebo měsíční fakturaci.</span><span class="sxs-lookup"><span data-stu-id="809a2-189">If purchasing [Azure reservations](azure-reservations.md) through an Azure plan, you can choose either one-time or monthly billing.</span></span>


## <a name="azure-spending"></a><span data-ttu-id="809a2-190">Útrata v Azure</span><span class="sxs-lookup"><span data-stu-id="809a2-190">Azure spending</span></span>

<span data-ttu-id="809a2-191">Stávající prostředí Azure útraty se aktualizuje tak, aby podporovalo nové účtování plánu Azure v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="809a2-191">The existing Azure spending experience is updated to support the new Azure plan billing in Partner Center.</span></span> <span data-ttu-id="809a2-192">To umožňuje partnerům:</span><span class="sxs-lookup"><span data-stu-id="809a2-192">This enables partners to:</span></span>

- <span data-ttu-id="809a2-193">Zobrazení, Správa a příjem výstrah pro rozpočtovou sadu na úrovni zákazníka</span><span class="sxs-lookup"><span data-stu-id="809a2-193">View, manage, and receive alerts for budget set at a customer level</span></span> 

- <span data-ttu-id="809a2-194">Zobrazení celkového odhadu útraty v plánu Azure (rozdělené podle prostředků a úrovně měřiče)</span><span class="sxs-lookup"><span data-stu-id="809a2-194">View total estimated spending on an Azure plan (broken down by resource and meter level)</span></span>

<span data-ttu-id="809a2-195">Vzhledem k tomu, že model fakturace pro služby Azure prostřednictvím plánu Azure je spotřeba po platbě, aby se předešlo většímu množství, než je očekávané, můžou partneři použít měsíční rozpočet a sledovat procento využití.</span><span class="sxs-lookup"><span data-stu-id="809a2-195">Because the billing model for Azure services through an Azure plan is post-pay consumption, to avoid a bigger bill than anticipated, partners can apply a monthly budget and track the percentage of usage.</span></span> <span data-ttu-id="809a2-196">Rozpočet lze použít na jednoho zákazníka nebo více zákazníků najednou.</span><span class="sxs-lookup"><span data-stu-id="809a2-196">A budget can be applied to one customer or multiple customers at one time.</span></span> 

:::image type="content" source="images/azure/azurespend.png" alt-text="Útrata v Azure":::

## <a name="next-steps"></a><span data-ttu-id="809a2-198">Další kroky</span><span class="sxs-lookup"><span data-stu-id="809a2-198">Next steps</span></span>

- <span data-ttu-id="809a2-199">Podívejte se, jak se počítá partner získaný kredit (PEC).</span><span class="sxs-lookup"><span data-stu-id="809a2-199">See how the partner earned credit (PEC) is calculated.</span></span> <span data-ttu-id="809a2-200">Přihlaste se na [řídicí panel](https://partner.microsoft.com/dashboard/) partnerského centra a vyhledejte dostupný ceník.</span><span class="sxs-lookup"><span data-stu-id="809a2-200">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/) and locate the price list available.</span></span>

- <span data-ttu-id="809a2-201">Další informace o [nákupu plánu Azure](purchase-azure-plan.md)</span><span class="sxs-lookup"><span data-stu-id="809a2-201">Learn about [purchasing the Azure plan](purchase-azure-plan.md)</span></span>

- <span data-ttu-id="809a2-202">Podívejte se na [ceník pro nové prostředí pro obchod v CSP](azure-plan-price-list.md) .</span><span class="sxs-lookup"><span data-stu-id="809a2-202">See the [price list for the new commerce experience in CSP](azure-plan-price-list.md)</span></span>
