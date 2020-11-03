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
ms.openlocfilehash: bbd2aceac62a7e726ed81a78305ea23213c94156
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/03/2020
ms.locfileid: "92526990"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="f3255-104">Migrace předplatných Office 365 E4 na novější verze Office 365</span><span class="sxs-lookup"><span data-stu-id="f3255-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="f3255-105">**Platí pro**</span><span class="sxs-lookup"><span data-stu-id="f3255-105">**Applies to**</span></span>

-  <span data-ttu-id="f3255-106">Partnerské centrum</span><span class="sxs-lookup"><span data-stu-id="f3255-106">Partner Center</span></span>

<span data-ttu-id="f3255-107">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="f3255-107">**Appropriate roles**</span></span>
-   <span data-ttu-id="f3255-108">Globální správce</span><span class="sxs-lookup"><span data-stu-id="f3255-108">Global admin</span></span>
-   <span data-ttu-id="f3255-109">Správce uživatelů</span><span class="sxs-lookup"><span data-stu-id="f3255-109">User admin</span></span>
-   <span data-ttu-id="f3255-110">Agent správce</span><span class="sxs-lookup"><span data-stu-id="f3255-110">Admin agent</span></span>
-   <span data-ttu-id="f3255-111">Agent prodeje</span><span class="sxs-lookup"><span data-stu-id="f3255-111">Sales agent</span></span>

<span data-ttu-id="f3255-112">Plán Office 365 Enterprise E4 je vyřazený, platný 7. dubna 2017.</span><span class="sxs-lookup"><span data-stu-id="f3255-112">The Office 365 Enterprise E4 plan is retired, effective April 7, 2017.</span></span> <span data-ttu-id="f3255-113">Po tomto datu už nebudete moct koupit nová předplatná Office 365 E4 a existující odběry E4 se po uplynutí této doby nebudou automaticky obnovovat.</span><span class="sxs-lookup"><span data-stu-id="f3255-113">You can no longer purchase new Office 365 E4 subscriptions after this date, and existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="f3255-114">Po ukončení předplatných E4 se zruší.</span><span class="sxs-lookup"><span data-stu-id="f3255-114">When E4 subscriptions end, they will be canceled.</span></span> <span data-ttu-id="f3255-115">Chcete-li zajistit kontinuitu pro zákazníky, měli byste převést zákazníky s vypršením platnosti předplatných E4 na podporovanou možnost SKU, která je uvedena níže.</span><span class="sxs-lookup"><span data-stu-id="f3255-115">To ensure continuity for customers, you should transition customers with expiring E4 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="f3255-116">Doporučujeme zákazníkům přesunout nové předplatné před uplynutím ročního koncového data předplatného, aby se předešlo výpadkům služby pro zákazníky.</span><span class="sxs-lookup"><span data-stu-id="f3255-116">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

> [!NOTE]  
> <span data-ttu-id="f3255-117">Vyřadí se SKU komerčních a vládních skladů Office 365 Enterprise E4.</span><span class="sxs-lookup"><span data-stu-id="f3255-117">Both Office 365 Enterprise E4 commercial and government SKUs are retired.</span></span>
 
<span data-ttu-id="f3255-118">Na stránce s podrobnostmi o předplatném se stav předplatného E4 změnil na "vyprší dne [Date]" z "automatické obnovy" v [datum] ".</span><span class="sxs-lookup"><span data-stu-id="f3255-118">On the subscription's detail page, the E4 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="f3255-119">Pokud používáte rozhraní API (buď CREST nebo Partnerská centra), můžete zjistit vypršení platnosti předplatného, a to společně s vlastností auto Renew = false.</span><span class="sxs-lookup"><span data-stu-id="f3255-119">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> 

<span data-ttu-id="f3255-120">Odběry E4 budou nastavené na automatické obnovení = false, 7. dubna 2017.</span><span class="sxs-lookup"><span data-stu-id="f3255-120">The E4 subscriptions will be set to auto renew=False in April 7, 2017.</span></span> <span data-ttu-id="f3255-121">Zákazníky můžete kdykoli přesunout do nového plánu.</span><span class="sxs-lookup"><span data-stu-id="f3255-121">You can move customers to a new plan at any time.</span></span> 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a><span data-ttu-id="f3255-122">Plány nahrazení edice Office 365 Enterprise E4</span><span class="sxs-lookup"><span data-stu-id="f3255-122">Office 365 Enterprise E4 edition replacement plans</span></span>

<span data-ttu-id="f3255-123">Můžete se rozhodnout, že budete stejné funkce udržovat s E4, nebo pokud chcete, aby vaši zákazníci využili výhod novějších funkcí a funkcí v Office 365 a Online Skypu pro firmy.</span><span class="sxs-lookup"><span data-stu-id="f3255-123">You can choose to maintain the same functionality with E4 or have your customers take advantage of newer features and functionality in Office 365 and Skype for Business Online.</span></span> <span data-ttu-id="f3255-124">Podrobnosti o cenách najdete v seznamu ceníků a v tabulce seznam nabídek v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="f3255-124">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> <span data-ttu-id="f3255-125">Zabezpečení produktu Enterprise E3 nebo zabezpečená produktivita Enterprise E5 může být nahrazena následujícími možnostmi pro Office 365 Enterprise E3 nebo Office 365 Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="f3255-125">Secure Product Enterprise E3 or Secure Productive Enterprise E5 may be substituted in the following options for Office 365 Enterprise E3 or Office 365 Enterprise E5 respectively.</span></span>

- <span data-ttu-id="f3255-126">Možnost 1: Office 365 Enterprise E5</span><span class="sxs-lookup"><span data-stu-id="f3255-126">Option 1: Office 365 Enterprise E5</span></span>

- <span data-ttu-id="f3255-127">Možnost 2: Office 365 Enterprise E3 + Skype pro firmy Cloud PBX</span><span class="sxs-lookup"><span data-stu-id="f3255-127">Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span></span>

- <span data-ttu-id="f3255-128">Možnost 3: Office 365 Enterprise E3 + Skype pro firmy plus CAL (cenová a parita funkčnosti s E4)</span><span class="sxs-lookup"><span data-stu-id="f3255-128">Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (price and functionality parity with E4)</span></span>

- <span data-ttu-id="f3255-129">Možnost 4: Office 365 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="f3255-129">Option 4: Office 365 Enterprise E3</span></span>


| <span data-ttu-id="f3255-130">Doporučené</span><span class="sxs-lookup"><span data-stu-id="f3255-130">Feature</span></span> | <span data-ttu-id="f3255-131">Možnost 1</span><span class="sxs-lookup"><span data-stu-id="f3255-131">Option 1</span></span> | <span data-ttu-id="f3255-132">Možnost 2</span><span class="sxs-lookup"><span data-stu-id="f3255-132">Option 2</span></span> | <span data-ttu-id="f3255-133">Možnost 3</span><span class="sxs-lookup"><span data-stu-id="f3255-133">Option 3</span></span> | <span data-ttu-id="f3255-134">Možnost 4</span><span class="sxs-lookup"><span data-stu-id="f3255-134">Option 4</span></span> |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| <span data-ttu-id="f3255-135">Chcete získat všechny funkce zahrnuté v Office 365 Enterprise E4?</span><span class="sxs-lookup"><span data-stu-id="f3255-135">Get all the features included in Office 365 Enterprise E4?</span></span> | <span data-ttu-id="f3255-136">Ano</span><span class="sxs-lookup"><span data-stu-id="f3255-136">Yes</span></span> | <span data-ttu-id="f3255-137">Ano</span><span class="sxs-lookup"><span data-stu-id="f3255-137">Yes</span></span> | <span data-ttu-id="f3255-138">Ano</span><span class="sxs-lookup"><span data-stu-id="f3255-138">Yes</span></span> | <span data-ttu-id="f3255-139">Ne</span><span class="sxs-lookup"><span data-stu-id="f3255-139">No</span></span> |
| <span data-ttu-id="f3255-140">Telefonní čísla spravovaná v sadě Office 365?</span><span class="sxs-lookup"><span data-stu-id="f3255-140">Phone numbers managed in Office 365?</span></span> | <span data-ttu-id="f3255-141">Ano</span><span class="sxs-lookup"><span data-stu-id="f3255-141">Yes</span></span> | <span data-ttu-id="f3255-142">Ano</span><span class="sxs-lookup"><span data-stu-id="f3255-142">Yes</span></span> | <span data-ttu-id="f3255-143">Ne</span><span class="sxs-lookup"><span data-stu-id="f3255-143">No</span></span> | <span data-ttu-id="f3255-144">Ne</span><span class="sxs-lookup"><span data-stu-id="f3255-144">No</span></span> |
| <span data-ttu-id="f3255-145">Telefonní čísla spravovaná místně i v Office 365 (hybridní nasazení)?</span><span class="sxs-lookup"><span data-stu-id="f3255-145">Phone numbers managed both on-premises and in Office 365 (hybrid deployment)?</span></span> | <span data-ttu-id="f3255-146">Ano</span><span class="sxs-lookup"><span data-stu-id="f3255-146">Yes</span></span> | <span data-ttu-id="f3255-147">Ano</span><span class="sxs-lookup"><span data-stu-id="f3255-147">Yes</span></span> | <span data-ttu-id="f3255-148">Ne</span><span class="sxs-lookup"><span data-stu-id="f3255-148">No</span></span> | <span data-ttu-id="f3255-149">Ne</span><span class="sxs-lookup"><span data-stu-id="f3255-149">No</span></span> |
| <span data-ttu-id="f3255-150">Možnost přidání plánu hlasového volání veřejné telefonní sítě?</span><span class="sxs-lookup"><span data-stu-id="f3255-150">Option to add a PSTN voice calling plan?</span></span> | <span data-ttu-id="f3255-151">Ano</span><span class="sxs-lookup"><span data-stu-id="f3255-151">Yes</span></span> | <span data-ttu-id="f3255-152">Ano</span><span class="sxs-lookup"><span data-stu-id="f3255-152">Yes</span></span> | <span data-ttu-id="f3255-153">Ne</span><span class="sxs-lookup"><span data-stu-id="f3255-153">No</span></span> | <span data-ttu-id="f3255-154">Ne</span><span class="sxs-lookup"><span data-stu-id="f3255-154">No</span></span> |
| <span data-ttu-id="f3255-155">Konference v PSTN?</span><span class="sxs-lookup"><span data-stu-id="f3255-155">PSTN Conferencing?</span></span> | <span data-ttu-id="f3255-156">Ano</span><span class="sxs-lookup"><span data-stu-id="f3255-156">Yes</span></span> | <span data-ttu-id="f3255-157">Ne</span><span class="sxs-lookup"><span data-stu-id="f3255-157">No</span></span> | <span data-ttu-id="f3255-158">Ne</span><span class="sxs-lookup"><span data-stu-id="f3255-158">No</span></span> | <span data-ttu-id="f3255-159">Ne</span><span class="sxs-lookup"><span data-stu-id="f3255-159">No</span></span> |
| <span data-ttu-id="f3255-160">Rozšířené nástroje pro spolupráci, analýzu a zabezpečení?</span><span class="sxs-lookup"><span data-stu-id="f3255-160">Advanced tools for collaboration, analytics, and security?</span></span> | <span data-ttu-id="f3255-161">Ano</span><span class="sxs-lookup"><span data-stu-id="f3255-161">Yes</span></span> | <span data-ttu-id="f3255-162">Ne</span><span class="sxs-lookup"><span data-stu-id="f3255-162">No</span></span> | <span data-ttu-id="f3255-163">Ne</span><span class="sxs-lookup"><span data-stu-id="f3255-163">No</span></span> | <span data-ttu-id="f3255-164">Ne</span><span class="sxs-lookup"><span data-stu-id="f3255-164">No</span></span> |
| <span data-ttu-id="f3255-165">Interaktivní sestavy, řídicí panely a vizualizace dat?</span><span class="sxs-lookup"><span data-stu-id="f3255-165">Interactive reports, dashboards, and data visualizations?</span></span> | <span data-ttu-id="f3255-166">Ano</span><span class="sxs-lookup"><span data-stu-id="f3255-166">Yes</span></span> | <span data-ttu-id="f3255-167">Ne</span><span class="sxs-lookup"><span data-stu-id="f3255-167">No</span></span> | <span data-ttu-id="f3255-168">Ne</span><span class="sxs-lookup"><span data-stu-id="f3255-168">No</span></span> | <span data-ttu-id="f3255-169">Ne</span><span class="sxs-lookup"><span data-stu-id="f3255-169">No</span></span> | 
| <span data-ttu-id="f3255-170">Lepší kontrola zabezpečení dat a dodržování předpisů pomocí integrovaných uživatelských ovládacích prvků ochrany osobních údajů, transparentnosti a kontrastu?</span><span class="sxs-lookup"><span data-stu-id="f3255-170">More control over data security and compliance with built-in privacy, transparency, and refined user controls?</span></span> | <span data-ttu-id="f3255-171">Ano</span><span class="sxs-lookup"><span data-stu-id="f3255-171">Yes</span></span> | <span data-ttu-id="f3255-172">Ne</span><span class="sxs-lookup"><span data-stu-id="f3255-172">No</span></span> | <span data-ttu-id="f3255-173">Ne</span><span class="sxs-lookup"><span data-stu-id="f3255-173">No</span></span> | <span data-ttu-id="f3255-174">Ne</span><span class="sxs-lookup"><span data-stu-id="f3255-174">No</span></span> | 

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="f3255-175">Přechod zákazníků na nové plány produktů</span><span class="sxs-lookup"><span data-stu-id="f3255-175">Transition customers to new product plans</span></span>

<span data-ttu-id="f3255-176">Microsoft neustále nabízí našim partnerům nové produkty a služby.</span><span class="sxs-lookup"><span data-stu-id="f3255-176">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="f3255-177">V těchto případech možná budete muset upgradovat zákazníky na nové služby nebo migrovat své odběry z SKU, které se nakonec vypnou.</span><span class="sxs-lookup"><span data-stu-id="f3255-177">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="f3255-178">Migrace zákazníků z vyřazených SKU do novějších vyžaduje následující kroky:</span><span class="sxs-lookup"><span data-stu-id="f3255-178">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

-   <span data-ttu-id="f3255-179">Koupit nové předplatné</span><span class="sxs-lookup"><span data-stu-id="f3255-179">Purchase the new subscription</span></span>
-   <span data-ttu-id="f3255-180">Změna přiřazení licencí k aktuálním uživatelům</span><span class="sxs-lookup"><span data-stu-id="f3255-180">Reassign current user licenses</span></span>
-   <span data-ttu-id="f3255-181">Zrušit staré předplatné</span><span class="sxs-lookup"><span data-stu-id="f3255-181">Cancel the old subscription</span></span>

<span data-ttu-id="f3255-182">Pomocí těchto kroků migrujete předplatné Office 365 Enterprise E4 zákazníka na jednu z možností v tabulce výše.</span><span class="sxs-lookup"><span data-stu-id="f3255-182">Follow these steps to migrate a customer's Office 365 Enterprise E4 subscription to one of the options in the table above.</span></span>

### <a name="step-1---purchase-the-new-subscription"></a><span data-ttu-id="f3255-183">Krok 1 – zakoupení nového předplatného</span><span class="sxs-lookup"><span data-stu-id="f3255-183">Step 1 - Purchase the new subscription</span></span>

1. <span data-ttu-id="f3255-184">V nabídce **Partnerské centrum** vyberte **zákazníky** , vyberte zákazníka, kterého chcete přesunout, a pak vyberte **Přidat předplatná** .</span><span class="sxs-lookup"><span data-stu-id="f3255-184">From the **Partner Center** menu, select **Customers** , select the customer you wish to move, and then select **Add subscriptions** .</span></span>

2. <span data-ttu-id="f3255-185">Vyberte předplatné, které chcete z katalogu koupit (v tomto případě jednu z výše uvedených možností), zadejte počet licencí a pak vyberte **Odeslat** .</span><span class="sxs-lookup"><span data-stu-id="f3255-185">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit** .</span></span>

   <span data-ttu-id="f3255-186">Váš zákazník by teď měl mít staré i nové předplatné, staré předplatné Office 365 Enterprise E4 a nové předplatné Target, například možnost 1 – Office 365 Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="f3255-186">Your customer should now have both old and new subscriptions, the old Office 365 Enterprise E4 subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise E5.</span></span>

### <a name="step-2---reassign-the-customers-users-licenses"></a><span data-ttu-id="f3255-187">Krok 2 – Změna přiřazení licencí uživatelům zákazníka</span><span class="sxs-lookup"><span data-stu-id="f3255-187">Step 2 - Reassign the customer's users' licenses</span></span>

1. <span data-ttu-id="f3255-188">V nabídce **Partnerské centrum** vyberte **zákazníky** , vyberte zákazníka, kterého chcete přesunout, a pak vyberte **Uživatelé a licence** .</span><span class="sxs-lookup"><span data-stu-id="f3255-188">From the **Partner Center** menu, select **Customers** , select the customer you wish to move, and then select **Users and licenses** .</span></span> <span data-ttu-id="f3255-189">Otevře se stránka uživatelé a licence zákazníka.</span><span class="sxs-lookup"><span data-stu-id="f3255-189">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="f3255-190">Pokud chcete znovu přiřadit uživatelské licence, vyberte uživatele, kterého chcete znovu přiřadit, a pak vyberte **spravovat licence** .</span><span class="sxs-lookup"><span data-stu-id="f3255-190">To re-assign user licenses, select the user to reassign and then select **Manage licenses** .</span></span>

3. <span data-ttu-id="f3255-191">Na stránce **spravovat licence** zrušte zaškrtnutí políčka licence **Office 365 Enterprise E4** a vyberte nový plán služby pro předplatné, na které se bude zákazník pohybovat.</span><span class="sxs-lookup"><span data-stu-id="f3255-191">On the **Manage licenses** page, clear the **Office 365 Enterprise E4** license check box and select a new service plan for the subscription the customer is moving to.</span></span>

4. <span data-ttu-id="f3255-192">Vyberte **Odeslat** .</span><span class="sxs-lookup"><span data-stu-id="f3255-192">Select **Submit** .</span></span> <span data-ttu-id="f3255-193">Stránka s potvrzením obsahuje seznam nových přiřazení licencí.</span><span class="sxs-lookup"><span data-stu-id="f3255-193">A confirmation page lists the new license assignments.</span></span>

5. <span data-ttu-id="f3255-194">Pokračujte stejnými kroky u všech ostatních zákaznických uživatelů, kteří potřebují opětovné přiřazení licence.</span><span class="sxs-lookup"><span data-stu-id="f3255-194">Continue the same steps with any other customer users that need license reassignment.</span></span>

<span data-ttu-id="f3255-195">Po přesunutí uživatelských licencí do nové služby můžete toto vyřazené předplatné bezpečně zrušit na nejvyšší úrovni zákazníka.</span><span class="sxs-lookup"><span data-stu-id="f3255-195">After moving the user licenses to the new service, you can safely cancel the retired subscription at the top Customer level.</span></span>

### <a name="step-3---cancel-the-old-subscription"></a><span data-ttu-id="f3255-196">Krok 3 – zrušení původního předplatného</span><span class="sxs-lookup"><span data-stu-id="f3255-196">Step 3 - Cancel the old subscription</span></span>

1. <span data-ttu-id="f3255-197">V nabídce **Partnerské centrum** vyberte **zákazníci** .</span><span class="sxs-lookup"><span data-stu-id="f3255-197">From the **Partner Center** menu, select **Customers** .</span></span> <span data-ttu-id="f3255-198">Vyberte zákazníka, kterého chcete přesunout, a vyberte předplatné, které chcete zrušit.</span><span class="sxs-lookup"><span data-stu-id="f3255-198">Select the customer you want to move, and select the subscription you want to cancel.</span></span>

2. <span data-ttu-id="f3255-199">Na stránce Podrobnosti předplatného nastavte stav předplatného na **pozastaveno** .</span><span class="sxs-lookup"><span data-stu-id="f3255-199">In the subscription details page, set the subscription status to **Suspended** .</span></span>

3. <span data-ttu-id="f3255-200">Vyberte **Odeslat** .</span><span class="sxs-lookup"><span data-stu-id="f3255-200">Select **Submit** .</span></span>

<span data-ttu-id="f3255-201">Staré předplatné je pozastavené a nové předplatné je aktivní.</span><span class="sxs-lookup"><span data-stu-id="f3255-201">The old subscription is suspended and the new subscription is active.</span></span> <span data-ttu-id="f3255-202">Pozastavený odběr bude po 120 dnech automaticky zřízen.</span><span class="sxs-lookup"><span data-stu-id="f3255-202">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="f3255-203">Zákazník nevzniká žádné další poplatky za původní předplatné.</span><span class="sxs-lookup"><span data-stu-id="f3255-203">The customer incurs no additional costs for the old subscription.</span></span>



 



