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
ms.openlocfilehash: 757383ee264e58e7b4dc8ffefafe213cb49acb79
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149787"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a><span data-ttu-id="eebab-103">Nové obchodní prostředí v CSP – Fakturace Azure</span><span class="sxs-lookup"><span data-stu-id="eebab-103">New commerce experience in CSP - Azure billing</span></span> 

<span data-ttu-id="eebab-104">**Příslušné role**: Agent správce | Správce fakturace | Globální správce</span><span class="sxs-lookup"><span data-stu-id="eebab-104">**Appropriate roles**: Admin agent | Billing admin | Global admin</span></span>

<span data-ttu-id="eebab-105">Tento článek vysvětluje, jak získat přístup ke struktuře souborů fakturace a odsouhlasení souvisejících s fakturací za plán Azure.</span><span class="sxs-lookup"><span data-stu-id="eebab-105">This article explains how to access and understand the invoice and reconciliation file structure related to billing for the Azure plan.</span></span> <span data-ttu-id="eebab-106">Fakturace v rámci plánu Azure je zjednodušené fakturační prostředí s využitím zarovnaných a fakturačních období na základě kalendářního měsíce.</span><span class="sxs-lookup"><span data-stu-id="eebab-106">Billing under the Azure plan is a simplified billing experience using an aligned single billing date and calendar month-based billing period.</span></span>

## <a name="summary-of-billing-essentials"></a><span data-ttu-id="eebab-107">Shrnutí základních informací o fakturaci</span><span class="sxs-lookup"><span data-stu-id="eebab-107">Summary of billing essentials</span></span>

- <span data-ttu-id="eebab-108">**Datum faktury**: soubor fakturace a odsouhlasení bude k dispozici v 8. bodě a řídicím panelu partnerského centra/rozhraní API.</span><span class="sxs-lookup"><span data-stu-id="eebab-108">**Invoice date**: Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).</span></span>

- <span data-ttu-id="eebab-109">**Fakturační období faktury**: fakturační období faktury je zarovnané na kalendářní měsíc, například 10/1-10/31, 11/1-11/30.</span><span class="sxs-lookup"><span data-stu-id="eebab-109">**Invoice billing period**: The invoice billing period is aligned to the calendar month, for example,  10/1-10/31, 11/1-11/30.</span></span>

- <span data-ttu-id="eebab-110">Poplatky **za období služby**: poplatky se budou zarovnávat do kalendářního měsíce.</span><span class="sxs-lookup"><span data-stu-id="eebab-110">**Charge service periods**: Charges will align to the calendar month.</span></span> <span data-ttu-id="eebab-111">Pokud třeba účtováná partner přidá služby Azure prostřednictvím plánu Azure na 10/15 a zákazník začne využívat služby Azure na 10/15, bude vám účtovaný partner dostávat faktury nebo rekognoskaci na 11/8 za spotřebu zákazníka za období služby 10/15-10/31.</span><span class="sxs-lookup"><span data-stu-id="eebab-111">For example, if billed partner adds Azure services through an Azure plan on 10/15 and the customer begins consumption of Azure services on 10/15, then billed partner will receive invoice/recon on 11/8 for customer consumption for the service period 10/15 - 10/31.</span></span> <span data-ttu-id="eebab-112">Faktura za příští měsíc, která se vygeneruje v 12/8, obsahuje všechny poplatky za období služby 11/1-11/31.</span><span class="sxs-lookup"><span data-stu-id="eebab-112">The next month's invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.</span></span>

- <span data-ttu-id="eebab-113">**Platební podmínka faktury**: NET 60 dní.</span><span class="sxs-lookup"><span data-stu-id="eebab-113">**Invoice payment term**: Net 60 days.</span></span>

- <span data-ttu-id="eebab-114">**Měna faktury**: od 1. ledna 28 2021 partneři v oblasti EU/ESVO a UK, kteří noví zákazníci a stávající zákazníci s poskytovatelem CSP nakupují nové nabídky pro Commerce, jejichž klienti byli vytvořeni ještě dřív, než 11. května 2020, budou se fakturovat za tyto nákupy v měně partnera Location.</span><span class="sxs-lookup"><span data-stu-id="eebab-114">**Invoice currency**: Starting January 28th 2021, partners in the EU/EFTA and UK region who have new customers and existing CSP customers purchasing new commerce offers for the first time whose tenants were created prior to 11 May 2020, will be billed for those purchases in partner location currency.</span></span> <span data-ttu-id="eebab-115">Partneři, kteří se nacházejí mimo oblast EU/ESVO a UK, se budou dál účtovat v měně partnera umístění.</span><span class="sxs-lookup"><span data-stu-id="eebab-115">Partners located outside of the EU/EFTA and UK region will continue to be billed in partner location currency.</span></span>

- <span data-ttu-id="eebab-116">**Pobídky pro partnery**: placené 45 dny od konce měsíce faktury.</span><span class="sxs-lookup"><span data-stu-id="eebab-116">**Partner incentives**: Paid 45 days from the end of the invoice month.</span></span>

## <a name="access-your-invoices-and-reconciliation-files"></a><span data-ttu-id="eebab-117">Přístup k vašim fakturám a souborům pro odsouhlasení</span><span class="sxs-lookup"><span data-stu-id="eebab-117">Access your invoices and reconciliation files</span></span>

<span data-ttu-id="eebab-118">Správce globálního správce nebo fakturace vaší společnosti obdrží e-mail, když je faktura připravena k zobrazení.</span><span class="sxs-lookup"><span data-stu-id="eebab-118">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span>

<span data-ttu-id="eebab-119">Přístup k souboru faktury a odsouhlasení:</span><span class="sxs-lookup"><span data-stu-id="eebab-119">To access the invoice and reconciliation file:</span></span>

1. <span data-ttu-id="eebab-120">Přihlaste se k [řídicímu panelu](https://partner.microsoft.com/dashboard/) pro Partnerské centrum.</span><span class="sxs-lookup"><span data-stu-id="eebab-120">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="eebab-121">V nabídce Partnerské centrum vyberte **Fakturace.**</span><span class="sxs-lookup"><span data-stu-id="eebab-121">From the Partner Center menu, select **Billing**.</span></span>

3. <span data-ttu-id="eebab-122">Vyberte kartu Opakující se **a** **Jednou a** měnu, kterou vás zajímá.</span><span class="sxs-lookup"><span data-stu-id="eebab-122">Select the tab for the **Recurring** and **One-time** and the currency you are interested in.</span></span>

   :::image type="content" source="images/azure/billing3.png" alt-text="Fakturační":::

4. <span data-ttu-id="eebab-124">Vyberte **fakturu** nebo **soubor s vyrovnáním.**</span><span class="sxs-lookup"><span data-stu-id="eebab-124">Select **Invoice** or **Reconciliation file**.</span></span>  

   <span data-ttu-id="eebab-125">Pokud chcete zobrazit historické faktury a soubory odsoudíte, rozbalte řádek Historie fakturace níže.</span><span class="sxs-lookup"><span data-stu-id="eebab-125">To view historical invoices and recon files expand the Billing history row below.</span></span>

## <a name="understanding-usage-data"></a><span data-ttu-id="eebab-126">Vysvětlení dat o využití</span><span class="sxs-lookup"><span data-stu-id="eebab-126">Understanding usage data</span></span> 

1. <span data-ttu-id="eebab-127">Plán Azure je kontejner kořenové nebo nejvyšší úrovně pro použití.</span><span class="sxs-lookup"><span data-stu-id="eebab-127">Azure plan is the root or top-level container for usage.</span></span> <span data-ttu-id="eebab-128">Veškeré využití se váže zpět na jeden plán Azure.</span><span class="sxs-lookup"><span data-stu-id="eebab-128">All usage is tied back to a single Azure plan.</span></span>

2. <span data-ttu-id="eebab-129">V rámci plánu bude jedno nebo více předplatných Azure.</span><span class="sxs-lookup"><span data-stu-id="eebab-129">Within a plan, there will be one or more Azure subscriptions.</span></span> <span data-ttu-id="eebab-130">Jedná se o kontejnery používané pro správu a nasazení prostředků.</span><span class="sxs-lookup"><span data-stu-id="eebab-130">These are containers used for resource management and deployment.</span></span> 

3. <span data-ttu-id="eebab-131">Skupiny prostředků se v rámci předplatného přidávají do skupin prostředků.</span><span class="sxs-lookup"><span data-stu-id="eebab-131">Within a subscription, resource groups add to group resources.</span></span> <span data-ttu-id="eebab-132">Každý prostředek je nasazený do jedné skupiny prostředků.</span><span class="sxs-lookup"><span data-stu-id="eebab-132">Every resource is deployed to one resource group.</span></span> 

4. <span data-ttu-id="eebab-133">Mezi příklady prostředků patří virtuální počítače a účty úložiště.</span><span class="sxs-lookup"><span data-stu-id="eebab-133">Examples of resources include virtual machines and storage accounts.</span></span> 

5. <span data-ttu-id="eebab-134">Měřiče pro vysílání prostředků: Měřiče měří spotřebu prostředku a jeden prostředek může generovat využití pro více měřičů.</span><span class="sxs-lookup"><span data-stu-id="eebab-134">Resource emit meters: Meters are measurements of consumption of a resource, and one resource may emit usage for multiple meters.</span></span> <span data-ttu-id="eebab-135">Měřiče se identifikuje podle Id produktu, SKUId a ID dostupnosti.</span><span class="sxs-lookup"><span data-stu-id="eebab-135">Meters are identified by a ProductId, SKUId, and AvailabilityId.</span></span> 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a><span data-ttu-id="eebab-136">Hierarchie skupin prostředků předplatného a měření</span><span class="sxs-lookup"><span data-stu-id="eebab-136">Hierarchy of subscription resource groups and metering</span></span>

<span data-ttu-id="eebab-137">**Účet Azure (tenant)**</span><span class="sxs-lookup"><span data-stu-id="eebab-137">**Azure account (tenant)**</span></span>

- <span data-ttu-id="eebab-138">Předplatné A</span><span class="sxs-lookup"><span data-stu-id="eebab-138">Subscription A</span></span>
    - <span data-ttu-id="eebab-139">ResourceGroup 1</span><span class="sxs-lookup"><span data-stu-id="eebab-139">ResourceGroup 1</span></span>
        - <span data-ttu-id="eebab-140">Virtuální počítač (prostředek)</span><span class="sxs-lookup"><span data-stu-id="eebab-140">Virtual machine (resource)</span></span>
            - <span data-ttu-id="eebab-141">Výpočetní měření</span><span class="sxs-lookup"><span data-stu-id="eebab-141">Compute meter</span></span>
        - <span data-ttu-id="eebab-142">Virtuální síť (prostředek)</span><span class="sxs-lookup"><span data-stu-id="eebab-142">Virtual network (resource)</span></span>
            - <span data-ttu-id="eebab-143">Žádný měřič fakturace</span><span class="sxs-lookup"><span data-stu-id="eebab-143">No billing meter</span></span>

    - <span data-ttu-id="eebab-144">Zdroj dat 2</span><span class="sxs-lookup"><span data-stu-id="eebab-144">ResourceGroup 2</span></span>
        - <span data-ttu-id="eebab-145">Virtuální počítač (prostředek)</span><span class="sxs-lookup"><span data-stu-id="eebab-145">Virtual machine (resource)</span></span>
            - <span data-ttu-id="eebab-146">Měřič počítačů</span><span class="sxs-lookup"><span data-stu-id="eebab-146">Computer meter</span></span>
        - <span data-ttu-id="eebab-147">SSD úrovně Premium spravovaný disk (prostředek)</span><span class="sxs-lookup"><span data-stu-id="eebab-147">Premium SSD-managed disk (resource)</span></span>
            - <span data-ttu-id="eebab-148">Měřič kapacity úložiště</span><span class="sxs-lookup"><span data-stu-id="eebab-148">Storage capacity meter</span></span>
            - <span data-ttu-id="eebab-149">Měřič operací úložiště</span><span class="sxs-lookup"><span data-stu-id="eebab-149">Storage operations meter</span></span>

- <span data-ttu-id="eebab-150">Předplatné B-kategorie prostředků 1 – Azure SQL (prostředek) – měřič DTU – VPN Gateway (prostředek) – měřič brány VPN</span><span class="sxs-lookup"><span data-stu-id="eebab-150">Subscription B   -ResourceGroup 1       - Azure SQL (resource)           - DTU meter       - VPN Gateway (resource)           - VPN gateway meter</span></span>

    - <span data-ttu-id="eebab-151">Zdroj dat 2</span><span class="sxs-lookup"><span data-stu-id="eebab-151">ResourceGroup 2</span></span>
        - <span data-ttu-id="eebab-152">Virtual Network rozhraní (prostředek)</span><span class="sxs-lookup"><span data-stu-id="eebab-152">Virtual Network Interface (resource)</span></span>
            - <span data-ttu-id="eebab-153">Žádný měřič fakturace</span><span class="sxs-lookup"><span data-stu-id="eebab-153">No billing meter</span></span>

## <a name="read-the-invoice"></a><span data-ttu-id="eebab-154">Přečtěte si fakturu</span><span class="sxs-lookup"><span data-stu-id="eebab-154">Read the invoice</span></span>

1. <span data-ttu-id="eebab-155">Faktura bude k dispozici později než osmý měsíc v měsíci.</span><span class="sxs-lookup"><span data-stu-id="eebab-155">Invoice will be available no later than the eighth of each month.</span></span>

2. <span data-ttu-id="eebab-156">Partneři mají 60 dní na platbu.</span><span class="sxs-lookup"><span data-stu-id="eebab-156">Partners have 60 days to remit payment.</span></span>

3. <span data-ttu-id="eebab-157">Fakturační období bude pokrývat určitý kalendářní měsíc, například 10/1-10/31.</span><span class="sxs-lookup"><span data-stu-id="eebab-157">The billing period will cover a given calendar month, for example, 10/1-10/31.</span></span>

4. <span data-ttu-id="eebab-158">Poplatky jsou očištěné od úprav (množství je netto "získaným partnerským kreditem pro spravované služby").</span><span class="sxs-lookup"><span data-stu-id="eebab-158">Charges are net of adjustments (amount is net of “Partner earned credit for services managed").</span></span>

5. <span data-ttu-id="eebab-159">Další informace o fakturaci najdete v souboru rekognoskaci faktury a v souboru denního hodnocení využití.</span><span class="sxs-lookup"><span data-stu-id="eebab-159">Review the invoice recon file and daily rated usage file for additional billing details.</span></span>

   :::image type="content" source="images/azure/invoice1.png" alt-text="faktur":::

## <a name="read-the-invoice-reconciliation-file"></a><span data-ttu-id="eebab-161">Přečtěte si soubor odsouhlasení faktury</span><span class="sxs-lookup"><span data-stu-id="eebab-161">Read the invoice reconciliation file</span></span>

1. <span data-ttu-id="eebab-162">Každá kombinace plánu a měření Azure může mít až dva fakturační řádky v souboru rekognoskaci.</span><span class="sxs-lookup"><span data-stu-id="eebab-162">Each Azure plan and meter combination may have up to two billing lines on the recon file.</span></span>

2. <span data-ttu-id="eebab-163">Pokud je měřič kvalifikován pro jakýkoli typ slevy nebo kreditu (například vrstvené slevy nebo získaný kredit partnerských služeb) v celém kalendářním měsíci, bude soubor rekognoskaci obsahovat jenom jednu fakturační fakturu.</span><span class="sxs-lookup"><span data-stu-id="eebab-163">If the meter qualified for any type of discount or credit (such as tiered discounts or the Partner earned credit for services managed) throughout the entire calendar month, then the recon file will only contain one billing line.</span></span> <span data-ttu-id="eebab-164">Na sloupec **PriceAdjusmentDescription** se odkazuje na slevový nebo získaný kredit.</span><span class="sxs-lookup"><span data-stu-id="eebab-164">The column **PriceAdjusmentDescription** will reference the discount or earned credit.</span></span>

3. <span data-ttu-id="eebab-165">Pokud nejsou k dispozici žádné prostředky pro konkrétní měřič, který je kvalifikován pro zlevněný kredit nebo úvěr získaný pro partnery, bude soubor rekognoskaci obsahovat jenom jednu fakturační fakturu a skutečná Jednotková cena bude maloobchodní cena (což je jednotková cena).</span><span class="sxs-lookup"><span data-stu-id="eebab-165">If there are no resources for a particular meter that qualified for discount or partner earned credit, then the recon file will only contain one billing line and the effective unit price will be the retail price (which is the unit price).</span></span>

4. <span data-ttu-id="eebab-166">Pokud měřič nebo všechny prostředky, které tento měřič vyvolaly, jsou určené pro kredity, které jsou pro **služby spravované** pro část měsíce, a soubor rekognoskaci bude obsahovat dva fakturační řádky.</span><span class="sxs-lookup"><span data-stu-id="eebab-166">If the meter, or any resources emitting that meter, qualified for **Partner earned credit for services managed** for a part of the month, the recon file will contain two billing lines.</span></span> <span data-ttu-id="eebab-167">Jeden řádek bude představovat dny, ve kterých je měřený měřič, a druhý řádek bude představovat dny, které měřič nezpůsobil.</span><span class="sxs-lookup"><span data-stu-id="eebab-167">One line will represent the days the meter qualified and the second line will represent the days the meter did not qualify.</span></span>

## <a name="read-the-daily-usage-file"></a><span data-ttu-id="eebab-168">Přečtěte si soubor denního využití.</span><span class="sxs-lookup"><span data-stu-id="eebab-168">Read the daily usage file</span></span>

- <span data-ttu-id="eebab-169">Měřiče předplatného v rámci plánu Azure jsou ohodnocené a každý den se každoročně kumulovaná.</span><span class="sxs-lookup"><span data-stu-id="eebab-169">Subscription meters under an Azure plan are rated, and are cumulated, on a daily basis.</span></span>

- <span data-ttu-id="eebab-170">**Získaný kredit partnerů pro spravované služby** je stanoven a použit každý den.</span><span class="sxs-lookup"><span data-stu-id="eebab-170">**Partner earned credit for services managed** is determined and applied on a daily basis.</span></span>

- <span data-ttu-id="eebab-171">Každý měřič předplatného bude mít řádek pro každý den v měsíci, kde byla spotřebována spotřeba.</span><span class="sxs-lookup"><span data-stu-id="eebab-171">Every subscription meter will have a row for every day of the month where there was consumption.</span></span>

- <span data-ttu-id="eebab-172">V následujícím příkladu:</span><span class="sxs-lookup"><span data-stu-id="eebab-172">In the example below:</span></span>

  - <span data-ttu-id="eebab-173">Pro měření pro **služby spravované** z 7/1-7/3 se měří pro daný kredit. (Poznámka: efektivní Jednotková cena je maloobchodní cena nižší než partner získaný.</span><span class="sxs-lookup"><span data-stu-id="eebab-173">Meter qualified for **Partner earned credit for services managed** from 7/1 - 7/3 (note the effective unit price is retail price less partner earned credit.</span></span>

  - <span data-ttu-id="eebab-174">U služeb spravovaných z 7/4-7/7 se nezpůsobilo měření pro kredity, které jsou **pro služby spravované** . (Poznámka: efektivní Jednotková cena je maloobchodní cena).</span><span class="sxs-lookup"><span data-stu-id="eebab-174">Meter didn't qualify for **Partner earned credit for services managed** from 7/4 - 7/7 (note the effective unit price is retail price).</span></span>

  - <span data-ttu-id="eebab-175">Pro měřený **kredit pro služby spravované** z 7/8-7/31 se měří na měřič. (Poznámka: efektivní Jednotková cena je cenově dosažená za maloobchodní cenu, která je nižší než partnerský.</span><span class="sxs-lookup"><span data-stu-id="eebab-175">Meter qualified for **Partner earned credit for services managed** from 7/8 - 7/31 (note the effective unit price is retail price less partner earned credit).</span></span>

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2":::

## <a name="invoice-in-customer-currency"></a><span data-ttu-id="eebab-177">Faktura v měně zákazníka</span><span class="sxs-lookup"><span data-stu-id="eebab-177">Invoice in customer currency</span></span>

<span data-ttu-id="eebab-178">Ceny služeb Azure v rámci plánu Azure budou platit v USD a budou se fakturovat v přiřazené měně země zákazníka.</span><span class="sxs-lookup"><span data-stu-id="eebab-178">Azure services through an Azure plan will be priced in USD and billed in the customer country assigned currency.</span></span> <span data-ttu-id="eebab-179">Pokud fakturační měna není USD, zobrazí se na poslední stránce faktury použitá sazba za cizí Exchange (FX).</span><span class="sxs-lookup"><span data-stu-id="eebab-179">If the billing currency is non-USD, then the Foreign exchange (FX) rate used will be shown on the last page of the invoice.</span></span> <span data-ttu-id="eebab-180">Sazby za FX se určují měsíčně a platí pro následující fakturu.</span><span class="sxs-lookup"><span data-stu-id="eebab-180">FX rates are determined monthly and applied to the following invoice.</span></span> <span data-ttu-id="eebab-181">Úplný seznam měn za země najdete v části [Nová obchodní oddělení nabídky dostupnost země a měna zákazníka](https://go.microsoft.com/fwlink/?linkid=2112354).</span><span class="sxs-lookup"><span data-stu-id="eebab-181">For a full list of country currencies, please view the [new commerce offers country availability and customer currency matrix](https://go.microsoft.com/fwlink/?linkid=2112354).</span></span>

<span data-ttu-id="eebab-182">Microsoft dodržuje při konverzi burzovní sklad s Londýn.</span><span class="sxs-lookup"><span data-stu-id="eebab-182">Microsoft follows the London Stock Exchange for conversion.</span></span> <span data-ttu-id="eebab-183">Používáme směnný kurz, který se rovná směnnému kurzu zaznamenanému za poslední sekundu posledního pracovního dne v měsíci na burze cenných papírů v Londýně.</span><span class="sxs-lookup"><span data-stu-id="eebab-183">We use the exchange rate, which is equal to the exchange rate captured on the last second of the last business day of the month on the London Stock Exchange.</span></span> <span data-ttu-id="eebab-184">Sazby za FX budou aktualizovány a k dispozici v den před prvním dnem v měsíci, pro které se vztahují.</span><span class="sxs-lookup"><span data-stu-id="eebab-184">The FX rates will be refreshed and available on the day before the first of the month for which they apply.</span></span>

## <a name="azure-reservations"></a><span data-ttu-id="eebab-185">Rezervace Azure</span><span class="sxs-lookup"><span data-stu-id="eebab-185">Azure reservations</span></span>


<span data-ttu-id="eebab-186">Při nákupu [rezervací Azure](azure-reservations.md) prostřednictvím plánu Azure si můžete vybrat buď jednorázovou, nebo měsíční fakturaci.</span><span class="sxs-lookup"><span data-stu-id="eebab-186">If purchasing [Azure reservations](azure-reservations.md) through an Azure plan, you can choose either one-time or monthly billing.</span></span>


## <a name="azure-spending"></a><span data-ttu-id="eebab-187">Útrata v Azure</span><span class="sxs-lookup"><span data-stu-id="eebab-187">Azure spending</span></span>

<span data-ttu-id="eebab-188">Stávající prostředí Azure útraty se aktualizuje tak, aby podporovalo nové účtování plánu Azure v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="eebab-188">The existing Azure spending experience is updated to support the new Azure plan billing in Partner Center.</span></span> <span data-ttu-id="eebab-189">To umožňuje partnerům:</span><span class="sxs-lookup"><span data-stu-id="eebab-189">This enables partners to:</span></span>

- <span data-ttu-id="eebab-190">Zobrazení, Správa a příjem výstrah pro rozpočtovou sadu na úrovni zákazníka</span><span class="sxs-lookup"><span data-stu-id="eebab-190">View, manage, and receive alerts for budget set at a customer level</span></span> 

- <span data-ttu-id="eebab-191">Zobrazení celkového odhadu útraty v plánu Azure (rozdělené podle prostředků a úrovně měřiče)</span><span class="sxs-lookup"><span data-stu-id="eebab-191">View total estimated spending on an Azure plan (broken down by resource and meter level)</span></span>

<span data-ttu-id="eebab-192">Vzhledem k tomu, že model fakturace pro služby Azure prostřednictvím plánu Azure je spotřeba po platbě, aby se předešlo většímu množství, než je očekávané, můžou partneři použít měsíční rozpočet a sledovat procento využití.</span><span class="sxs-lookup"><span data-stu-id="eebab-192">Because the billing model for Azure services through an Azure plan is post-pay consumption, to avoid a bigger bill than anticipated, partners can apply a monthly budget and track the percentage of usage.</span></span> <span data-ttu-id="eebab-193">Rozpočet lze použít na jednoho zákazníka nebo více zákazníků najednou.</span><span class="sxs-lookup"><span data-stu-id="eebab-193">A budget can be applied to one customer or multiple customers at one time.</span></span> 

:::image type="content" source="images/azure/azurespend.png" alt-text="Útrata v Azure":::

## <a name="next-steps"></a><span data-ttu-id="eebab-195">Další kroky</span><span class="sxs-lookup"><span data-stu-id="eebab-195">Next steps</span></span>

- <span data-ttu-id="eebab-196">Podívejte se, jak se počítá partner získaný kredit (PEC).</span><span class="sxs-lookup"><span data-stu-id="eebab-196">See how the partner earned credit (PEC) is calculated.</span></span> <span data-ttu-id="eebab-197">Přihlaste se na [řídicí panel](https://partner.microsoft.com/dashboard/) partnerského centra a vyhledejte dostupný ceník.</span><span class="sxs-lookup"><span data-stu-id="eebab-197">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/) and locate the price list available.</span></span>

- <span data-ttu-id="eebab-198">Další informace o [nákupu plánu Azure](purchase-azure-plan.md)</span><span class="sxs-lookup"><span data-stu-id="eebab-198">Learn about [purchasing the Azure plan](purchase-azure-plan.md)</span></span>

- <span data-ttu-id="eebab-199">Podívejte se na [ceník pro nové prostředí pro obchod v CSP](azure-plan-price-list.md) .</span><span class="sxs-lookup"><span data-stu-id="eebab-199">See the [price list for the new commerce experience in CSP](azure-plan-price-list.md)</span></span>
