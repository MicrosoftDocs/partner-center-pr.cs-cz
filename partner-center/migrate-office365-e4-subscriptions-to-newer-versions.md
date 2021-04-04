---
title: Migrace předplatných Office 365 E4
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Edice systém Microsoft Office 365 Enterprise E4 je vyřazení od 7. dubna 2017. Přečtěte si, jak migrovat zákaznická předplatná do novějších verzí Office 365.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8a9662e0ce99fc054149dfbd4149532ce336eff6
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132617"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="3ea86-104">Migrace předplatných Office 365 E4 na novější verze Office 365</span><span class="sxs-lookup"><span data-stu-id="3ea86-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="3ea86-105">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="3ea86-105">**Appropriate roles**</span></span>

- <span data-ttu-id="3ea86-106">Globální správce</span><span class="sxs-lookup"><span data-stu-id="3ea86-106">Global admin</span></span>
- <span data-ttu-id="3ea86-107">Správce správy uživatelů</span><span class="sxs-lookup"><span data-stu-id="3ea86-107">User management admin</span></span>
- <span data-ttu-id="3ea86-108">Agent správce</span><span class="sxs-lookup"><span data-stu-id="3ea86-108">Admin agent</span></span>
- <span data-ttu-id="3ea86-109">Agent prodeje</span><span class="sxs-lookup"><span data-stu-id="3ea86-109">Sales agent</span></span>

<span data-ttu-id="3ea86-110">Plán Office 365 Enterprise E4 je vyřazený, platný 7. dubna 2017.</span><span class="sxs-lookup"><span data-stu-id="3ea86-110">The Office 365 Enterprise E4 plan is retired, effective April 7, 2017.</span></span> <span data-ttu-id="3ea86-111">Po tomto datu už nebudete moct koupit nová předplatná Office 365 E4 a existující odběry E4 se po uplynutí této doby nebudou automaticky obnovovat.</span><span class="sxs-lookup"><span data-stu-id="3ea86-111">You can no longer purchase new Office 365 E4 subscriptions after this date, and existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="3ea86-112">Po ukončení předplatných E4 se zruší.</span><span class="sxs-lookup"><span data-stu-id="3ea86-112">When E4 subscriptions end, they will be canceled.</span></span> <span data-ttu-id="3ea86-113">Chcete-li zajistit kontinuitu pro zákazníky, měli byste převést zákazníky s vypršením platnosti předplatných E4 na podporovanou možnost SKU, která je uvedena níže.</span><span class="sxs-lookup"><span data-stu-id="3ea86-113">To ensure continuity for customers, you should transition customers with expiring E4 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="3ea86-114">Doporučujeme zákazníkům přesunout nové předplatné před uplynutím ročního koncového data předplatného, aby se předešlo výpadkům služby pro zákazníky.</span><span class="sxs-lookup"><span data-stu-id="3ea86-114">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

> [!NOTE]  
> <span data-ttu-id="3ea86-115">Vyřadí se SKU komerčních a vládních skladů Office 365 Enterprise E4.</span><span class="sxs-lookup"><span data-stu-id="3ea86-115">Both Office 365 Enterprise E4 commercial and government SKUs are retired.</span></span>
 
<span data-ttu-id="3ea86-116">Na stránce s podrobnostmi o předplatném se stav předplatného E4 změnil na "vyprší dne [Date]" z "automatické obnovy" v [datum] ".</span><span class="sxs-lookup"><span data-stu-id="3ea86-116">On the subscription's detail page, the E4 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="3ea86-117">Pokud používáte rozhraní API (buď CREST nebo Partnerská centra), můžete zjistit vypršení platnosti předplatného, a to společně s vlastností auto Renew = false.</span><span class="sxs-lookup"><span data-stu-id="3ea86-117">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> 

<span data-ttu-id="3ea86-118">Odběry E4 budou nastavené na automatické obnovení = false, 7. dubna 2017.</span><span class="sxs-lookup"><span data-stu-id="3ea86-118">The E4 subscriptions will be set to auto renew=False in April 7, 2017.</span></span> <span data-ttu-id="3ea86-119">Zákazníky můžete kdykoli přesunout do nového plánu.</span><span class="sxs-lookup"><span data-stu-id="3ea86-119">You can move customers to a new plan at any time.</span></span> 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a><span data-ttu-id="3ea86-120">Plány nahrazení edice Office 365 Enterprise E4</span><span class="sxs-lookup"><span data-stu-id="3ea86-120">Office 365 Enterprise E4 edition replacement plans</span></span>

<span data-ttu-id="3ea86-121">Můžete se rozhodnout, že budete stejné funkce udržovat s E4, nebo pokud chcete, aby vaši zákazníci využili výhod novějších funkcí a funkcí v Office 365 a Online Skypu pro firmy.</span><span class="sxs-lookup"><span data-stu-id="3ea86-121">You can choose to maintain the same functionality with E4 or have your customers take advantage of newer features and functionality in Office 365 and Skype for Business Online.</span></span> <span data-ttu-id="3ea86-122">Podrobnosti o cenách najdete v seznamu ceníků a v tabulce seznam nabídek v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="3ea86-122">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> <span data-ttu-id="3ea86-123">Zabezpečení produktu Enterprise E3 nebo zabezpečená produktivita Enterprise E5 může být nahrazena následujícími možnostmi pro Office 365 Enterprise E3 nebo Office 365 Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="3ea86-123">Secure Product Enterprise E3 or Secure Productive Enterprise E5 may be substituted in the following options for Office 365 Enterprise E3 or Office 365 Enterprise E5 respectively.</span></span>

- <span data-ttu-id="3ea86-124">Možnost 1: Office 365 Enterprise E5</span><span class="sxs-lookup"><span data-stu-id="3ea86-124">Option 1: Office 365 Enterprise E5</span></span>

- <span data-ttu-id="3ea86-125">Možnost 2: Office 365 Enterprise E3 + Skype pro firmy Cloud PBX</span><span class="sxs-lookup"><span data-stu-id="3ea86-125">Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span></span>

- <span data-ttu-id="3ea86-126">Možnost 3: Office 365 Enterprise E3 + Skype pro firmy plus CAL (cenová a parita funkčnosti s E4)</span><span class="sxs-lookup"><span data-stu-id="3ea86-126">Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (price and functionality parity with E4)</span></span>

- <span data-ttu-id="3ea86-127">Možnost 4: Office 365 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="3ea86-127">Option 4: Office 365 Enterprise E3</span></span>


| <span data-ttu-id="3ea86-128">Funkce</span><span class="sxs-lookup"><span data-stu-id="3ea86-128">Feature</span></span> | <span data-ttu-id="3ea86-129">Možnost 1</span><span class="sxs-lookup"><span data-stu-id="3ea86-129">Option 1</span></span> | <span data-ttu-id="3ea86-130">Možnost 2</span><span class="sxs-lookup"><span data-stu-id="3ea86-130">Option 2</span></span> | <span data-ttu-id="3ea86-131">Možnost 3</span><span class="sxs-lookup"><span data-stu-id="3ea86-131">Option 3</span></span> | <span data-ttu-id="3ea86-132">Možnost 4</span><span class="sxs-lookup"><span data-stu-id="3ea86-132">Option 4</span></span> |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| <span data-ttu-id="3ea86-133">Chcete získat všechny funkce zahrnuté v Office 365 Enterprise E4?</span><span class="sxs-lookup"><span data-stu-id="3ea86-133">Get all the features included in Office 365 Enterprise E4?</span></span> | <span data-ttu-id="3ea86-134">Yes</span><span class="sxs-lookup"><span data-stu-id="3ea86-134">Yes</span></span> | <span data-ttu-id="3ea86-135">Yes</span><span class="sxs-lookup"><span data-stu-id="3ea86-135">Yes</span></span> | <span data-ttu-id="3ea86-136">Yes</span><span class="sxs-lookup"><span data-stu-id="3ea86-136">Yes</span></span> | <span data-ttu-id="3ea86-137">No</span><span class="sxs-lookup"><span data-stu-id="3ea86-137">No</span></span> |
| <span data-ttu-id="3ea86-138">Telefonní čísla spravovaná v sadě Office 365?</span><span class="sxs-lookup"><span data-stu-id="3ea86-138">Phone numbers managed in Office 365?</span></span> | <span data-ttu-id="3ea86-139">Yes</span><span class="sxs-lookup"><span data-stu-id="3ea86-139">Yes</span></span> | <span data-ttu-id="3ea86-140">Yes</span><span class="sxs-lookup"><span data-stu-id="3ea86-140">Yes</span></span> | <span data-ttu-id="3ea86-141">No</span><span class="sxs-lookup"><span data-stu-id="3ea86-141">No</span></span> | <span data-ttu-id="3ea86-142">No</span><span class="sxs-lookup"><span data-stu-id="3ea86-142">No</span></span> |
| <span data-ttu-id="3ea86-143">Telefonní čísla spravovaná místně i v Office 365 (hybridní nasazení)?</span><span class="sxs-lookup"><span data-stu-id="3ea86-143">Phone numbers managed both on-premises and in Office 365 (hybrid deployment)?</span></span> | <span data-ttu-id="3ea86-144">Yes</span><span class="sxs-lookup"><span data-stu-id="3ea86-144">Yes</span></span> | <span data-ttu-id="3ea86-145">Yes</span><span class="sxs-lookup"><span data-stu-id="3ea86-145">Yes</span></span> | <span data-ttu-id="3ea86-146">No</span><span class="sxs-lookup"><span data-stu-id="3ea86-146">No</span></span> | <span data-ttu-id="3ea86-147">No</span><span class="sxs-lookup"><span data-stu-id="3ea86-147">No</span></span> |
| <span data-ttu-id="3ea86-148">Možnost přidání plánu hlasového volání veřejné telefonní sítě?</span><span class="sxs-lookup"><span data-stu-id="3ea86-148">Option to add a PSTN voice calling plan?</span></span> | <span data-ttu-id="3ea86-149">Yes</span><span class="sxs-lookup"><span data-stu-id="3ea86-149">Yes</span></span> | <span data-ttu-id="3ea86-150">Yes</span><span class="sxs-lookup"><span data-stu-id="3ea86-150">Yes</span></span> | <span data-ttu-id="3ea86-151">No</span><span class="sxs-lookup"><span data-stu-id="3ea86-151">No</span></span> | <span data-ttu-id="3ea86-152">No</span><span class="sxs-lookup"><span data-stu-id="3ea86-152">No</span></span> |
| <span data-ttu-id="3ea86-153">Konference v PSTN?</span><span class="sxs-lookup"><span data-stu-id="3ea86-153">PSTN Conferencing?</span></span> | <span data-ttu-id="3ea86-154">Yes</span><span class="sxs-lookup"><span data-stu-id="3ea86-154">Yes</span></span> | <span data-ttu-id="3ea86-155">No</span><span class="sxs-lookup"><span data-stu-id="3ea86-155">No</span></span> | <span data-ttu-id="3ea86-156">No</span><span class="sxs-lookup"><span data-stu-id="3ea86-156">No</span></span> | <span data-ttu-id="3ea86-157">No</span><span class="sxs-lookup"><span data-stu-id="3ea86-157">No</span></span> |
| <span data-ttu-id="3ea86-158">Rozšířené nástroje pro spolupráci, analýzu a zabezpečení?</span><span class="sxs-lookup"><span data-stu-id="3ea86-158">Advanced tools for collaboration, analytics, and security?</span></span> | <span data-ttu-id="3ea86-159">Yes</span><span class="sxs-lookup"><span data-stu-id="3ea86-159">Yes</span></span> | <span data-ttu-id="3ea86-160">No</span><span class="sxs-lookup"><span data-stu-id="3ea86-160">No</span></span> | <span data-ttu-id="3ea86-161">No</span><span class="sxs-lookup"><span data-stu-id="3ea86-161">No</span></span> | <span data-ttu-id="3ea86-162">No</span><span class="sxs-lookup"><span data-stu-id="3ea86-162">No</span></span> |
| <span data-ttu-id="3ea86-163">Interaktivní sestavy, řídicí panely a vizualizace dat?</span><span class="sxs-lookup"><span data-stu-id="3ea86-163">Interactive reports, dashboards, and data visualizations?</span></span> | <span data-ttu-id="3ea86-164">Yes</span><span class="sxs-lookup"><span data-stu-id="3ea86-164">Yes</span></span> | <span data-ttu-id="3ea86-165">No</span><span class="sxs-lookup"><span data-stu-id="3ea86-165">No</span></span> | <span data-ttu-id="3ea86-166">No</span><span class="sxs-lookup"><span data-stu-id="3ea86-166">No</span></span> | <span data-ttu-id="3ea86-167">No</span><span class="sxs-lookup"><span data-stu-id="3ea86-167">No</span></span> | 
| <span data-ttu-id="3ea86-168">Lepší kontrola zabezpečení dat a dodržování předpisů pomocí integrovaných uživatelských ovládacích prvků ochrany osobních údajů, transparentnosti a kontrastu?</span><span class="sxs-lookup"><span data-stu-id="3ea86-168">More control over data security and compliance with built-in privacy, transparency, and refined user controls?</span></span> | <span data-ttu-id="3ea86-169">Yes</span><span class="sxs-lookup"><span data-stu-id="3ea86-169">Yes</span></span> | <span data-ttu-id="3ea86-170">No</span><span class="sxs-lookup"><span data-stu-id="3ea86-170">No</span></span> | <span data-ttu-id="3ea86-171">No</span><span class="sxs-lookup"><span data-stu-id="3ea86-171">No</span></span> | <span data-ttu-id="3ea86-172">No</span><span class="sxs-lookup"><span data-stu-id="3ea86-172">No</span></span> | 

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="3ea86-173">Přechod zákazníků na nové plány produktů</span><span class="sxs-lookup"><span data-stu-id="3ea86-173">Transition customers to new product plans</span></span>

<span data-ttu-id="3ea86-174">Microsoft neustále nabízí našim partnerům nové produkty a služby.</span><span class="sxs-lookup"><span data-stu-id="3ea86-174">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="3ea86-175">V těchto případech možná budete muset upgradovat zákazníky na nové služby nebo migrovat své odběry z SKU, které se nakonec vypnou.</span><span class="sxs-lookup"><span data-stu-id="3ea86-175">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="3ea86-176">Migrace zákazníků z vyřazených SKU do novějších vyžaduje následující kroky:</span><span class="sxs-lookup"><span data-stu-id="3ea86-176">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

-   <span data-ttu-id="3ea86-177">Koupit nové předplatné</span><span class="sxs-lookup"><span data-stu-id="3ea86-177">Purchase the new subscription</span></span>
-   <span data-ttu-id="3ea86-178">Změna přiřazení licencí k aktuálním uživatelům</span><span class="sxs-lookup"><span data-stu-id="3ea86-178">Reassign current user licenses</span></span>
-   <span data-ttu-id="3ea86-179">Zrušit staré předplatné</span><span class="sxs-lookup"><span data-stu-id="3ea86-179">Cancel the old subscription</span></span>

<span data-ttu-id="3ea86-180">Pomocí těchto kroků migrujete předplatné Office 365 Enterprise E4 zákazníka na jednu z možností v tabulce výše.</span><span class="sxs-lookup"><span data-stu-id="3ea86-180">Follow these steps to migrate a customer's Office 365 Enterprise E4 subscription to one of the options in the table above.</span></span>

### <a name="step-1---purchase-the-new-subscription"></a><span data-ttu-id="3ea86-181">Krok 1 – zakoupení nového předplatného</span><span class="sxs-lookup"><span data-stu-id="3ea86-181">Step 1 - Purchase the new subscription</span></span>

1. <span data-ttu-id="3ea86-182">V nabídce **Partnerské centrum** vyberte **zákazníky**, vyberte zákazníka, kterého chcete přesunout, a pak vyberte **Přidat předplatná**.</span><span class="sxs-lookup"><span data-stu-id="3ea86-182">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="3ea86-183">Vyberte předplatné, které chcete z katalogu koupit (v tomto případě jednu z výše uvedených možností), zadejte počet licencí a pak vyberte **Odeslat**.</span><span class="sxs-lookup"><span data-stu-id="3ea86-183">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

   <span data-ttu-id="3ea86-184">Váš zákazník by teď měl mít staré i nové předplatné, staré předplatné Office 365 Enterprise E4 a nové předplatné Target, například možnost 1 – Office 365 Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="3ea86-184">Your customer should now have both old and new subscriptions, the old Office 365 Enterprise E4 subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise E5.</span></span>

### <a name="step-2---reassign-the-customers-users-licenses"></a><span data-ttu-id="3ea86-185">Krok 2 – Změna přiřazení licencí uživatelům zákazníka</span><span class="sxs-lookup"><span data-stu-id="3ea86-185">Step 2 - Reassign the customer's users' licenses</span></span>

1. <span data-ttu-id="3ea86-186">V nabídce **Partnerské centrum** vyberte **zákazníky**, vyberte zákazníka, kterého chcete přesunout, a pak vyberte **Uživatelé a licence**.</span><span class="sxs-lookup"><span data-stu-id="3ea86-186">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Users and licenses**.</span></span> <span data-ttu-id="3ea86-187">Otevře se stránka uživatelé a licence zákazníka.</span><span class="sxs-lookup"><span data-stu-id="3ea86-187">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="3ea86-188">Pokud chcete změnit přiřazení uživatelských licencí, vyberte uživatele, kterého chcete znovu přiřadit, a pak vyberte **spravovat licence**.</span><span class="sxs-lookup"><span data-stu-id="3ea86-188">To reassign user licenses, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="3ea86-189">Na stránce **spravovat licence** zrušte zaškrtnutí políčka licence **Office 365 Enterprise E4** a vyberte nový plán služby pro předplatné, na které se bude zákazník pohybovat.</span><span class="sxs-lookup"><span data-stu-id="3ea86-189">On the **Manage licenses** page, clear the **Office 365 Enterprise E4** license check box and select a new service plan for the subscription the customer is moving to.</span></span>

4. <span data-ttu-id="3ea86-190">Vyberte **Odeslat**.</span><span class="sxs-lookup"><span data-stu-id="3ea86-190">Select **Submit**.</span></span> <span data-ttu-id="3ea86-191">Stránka s potvrzením obsahuje seznam nových přiřazení licencí.</span><span class="sxs-lookup"><span data-stu-id="3ea86-191">A confirmation page lists the new license assignments.</span></span>

5. <span data-ttu-id="3ea86-192">Pokračujte stejnými kroky u všech ostatních zákaznických uživatelů, kteří potřebují opětovné přiřazení licence.</span><span class="sxs-lookup"><span data-stu-id="3ea86-192">Continue the same steps with any other customer users that need license reassignment.</span></span>

<span data-ttu-id="3ea86-193">Po přesunutí uživatelských licencí do nové služby můžete toto vyřazené předplatné bezpečně zrušit na nejvyšší úrovni zákazníka.</span><span class="sxs-lookup"><span data-stu-id="3ea86-193">After moving the user licenses to the new service, you can safely cancel the retired subscription at the top Customer level.</span></span>

### <a name="step-3---cancel-the-old-subscription"></a><span data-ttu-id="3ea86-194">Krok 3 – zrušení původního předplatného</span><span class="sxs-lookup"><span data-stu-id="3ea86-194">Step 3 - Cancel the old subscription</span></span>

1. <span data-ttu-id="3ea86-195">V nabídce **Partnerské centrum** vyberte **zákazníci**.</span><span class="sxs-lookup"><span data-stu-id="3ea86-195">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="3ea86-196">Vyberte zákazníka, kterého chcete přesunout, a vyberte předplatné, které chcete zrušit.</span><span class="sxs-lookup"><span data-stu-id="3ea86-196">Select the customer you want to move, and select the subscription you want to cancel.</span></span>

2. <span data-ttu-id="3ea86-197">Na stránce Podrobnosti předplatného nastavte stav předplatného na **pozastaveno**.</span><span class="sxs-lookup"><span data-stu-id="3ea86-197">In the subscription details page, set the subscription status to **Suspended**.</span></span>

3. <span data-ttu-id="3ea86-198">Vyberte **Odeslat**.</span><span class="sxs-lookup"><span data-stu-id="3ea86-198">Select **Submit**.</span></span>

<span data-ttu-id="3ea86-199">Staré předplatné je pozastavené a nové předplatné je aktivní.</span><span class="sxs-lookup"><span data-stu-id="3ea86-199">The old subscription is suspended and the new subscription is active.</span></span> <span data-ttu-id="3ea86-200">Pozastavený odběr bude po 120 dnech automaticky zřízen.</span><span class="sxs-lookup"><span data-stu-id="3ea86-200">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="3ea86-201">Zákazník nevzniká žádné další poplatky za původní předplatné.</span><span class="sxs-lookup"><span data-stu-id="3ea86-201">The customer incurs no additional costs for the old subscription.</span></span>



 



