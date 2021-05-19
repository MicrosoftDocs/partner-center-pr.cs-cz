---
title: Migrace předplatných Office 365 E4
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: systém Microsoft Office 365 Enterprise E4 se k 7. dubnu 2017 vyřazena. Zjistěte, jak migrovat předplatná zákazníků na novější verze Office 365.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f738ddace805838cdf202c23cca8535c11cbdf54
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151555"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="1c893-104">Migrace předplatných Office 365 E4 na novější verze Office 365</span><span class="sxs-lookup"><span data-stu-id="1c893-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="1c893-105">**Odpovídající role:** Globální správce | Správce správy uživatelů | Agent správy | Agent prodeje</span><span class="sxs-lookup"><span data-stu-id="1c893-105">**Appropriate roles**: Global admin | User management admin | Admin agent | Sales agent</span></span>

<span data-ttu-id="1c893-106">Plán Office 365 Enterprise E4 je od 7. dubna 2017 vyřazený.</span><span class="sxs-lookup"><span data-stu-id="1c893-106">The Office 365 Enterprise E4 plan is retired, effective April 7, 2017.</span></span> <span data-ttu-id="1c893-107">Po tomto datu už není možné kupovat nová předplatná Office 365 E4 a stávající předplatná E4 se po vypršení jejich platnosti automaticky neobnoví.</span><span class="sxs-lookup"><span data-stu-id="1c893-107">You can no longer purchase new Office 365 E4 subscriptions after this date, and existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="1c893-108">Po skončení předplatných E4 se zruší.</span><span class="sxs-lookup"><span data-stu-id="1c893-108">When E4 subscriptions end, they will be canceled.</span></span> <span data-ttu-id="1c893-109">Pokud chcete zajistit kontinuitu pro zákazníky, měli byste zákazníky s předplatným E4 s vypršenou platnosti pře převodem na podporovanou možnost SKU uvedenou níže.</span><span class="sxs-lookup"><span data-stu-id="1c893-109">To ensure continuity for customers, you should transition customers with expiring E4 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="1c893-110">Doporučujeme přestěhovat zákazníky na nová předplatná před ročním datem ukončení předplatného, abyste se vyhnuli výpadkům služeb pro zákazníky.</span><span class="sxs-lookup"><span data-stu-id="1c893-110">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

> [!NOTE]  
> <span data-ttu-id="1c893-111">Komerční i státní SKU Office 365 Enterprise E4 jsou vyřazené z provozu.</span><span class="sxs-lookup"><span data-stu-id="1c893-111">Both Office 365 Enterprise E4 commercial and government SKUs are retired.</span></span>
 
<span data-ttu-id="1c893-112">Na stránce s podrobnostmi o předplatném se stav předplatného E4 změnil na Platnost vyprší [datum]" z "Automatické prodloužení platnosti k [datum]".</span><span class="sxs-lookup"><span data-stu-id="1c893-112">On the subscription's detail page, the E4 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="1c893-113">Pokud používáte rozhraní API (CREST nebo Partnerské centrum), můžete zjistit předplatná, kterým vyprší platnost, vyhodnocením koncového data odběru spolu s vlastností auto renew = False.</span><span class="sxs-lookup"><span data-stu-id="1c893-113">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> 

<span data-ttu-id="1c893-114">V 7. dubnu 2017 se předplatná E4 nastaví na auto renew=False.</span><span class="sxs-lookup"><span data-stu-id="1c893-114">The E4 subscriptions will be set to auto renew=False in April 7, 2017.</span></span> <span data-ttu-id="1c893-115">Zákazníky můžete kdykoli přesunout do nového plánu.</span><span class="sxs-lookup"><span data-stu-id="1c893-115">You can move customers to a new plan at any time.</span></span> 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a><span data-ttu-id="1c893-116">Plány nahrazení edice Office 365 Enterprise E4</span><span class="sxs-lookup"><span data-stu-id="1c893-116">Office 365 Enterprise E4 edition replacement plans</span></span>

<span data-ttu-id="1c893-117">Můžete se rozhodnout pro zachování stejných funkcí s E4 nebo můžete svým zákazníkům využít novější funkce v Office 365 a Online Skypu pro firmy.</span><span class="sxs-lookup"><span data-stu-id="1c893-117">You can choose to maintain the same functionality with E4 or have your customers take advantage of newer features and functionality in Office 365 and Skype for Business Online.</span></span> <span data-ttu-id="1c893-118">Podrobnosti o cenách najdete v matici ceníku a seznamu nabídek v Partnerské centrum.</span><span class="sxs-lookup"><span data-stu-id="1c893-118">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> <span data-ttu-id="1c893-119">Možnost Secure Product Enterprise E3 nebo Secure Productive Enterprise E5 může být nahrazena následujícími možnostmi pro Office 365 Enterprise E3 nebo Office 365 Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="1c893-119">Secure Product Enterprise E3 or Secure Productive Enterprise E5 may be substituted in the following options for Office 365 Enterprise E3 or Office 365 Enterprise E5 respectively.</span></span>

- <span data-ttu-id="1c893-120">Možnost 1: Office 365 Enterprise E5</span><span class="sxs-lookup"><span data-stu-id="1c893-120">Option 1: Office 365 Enterprise E5</span></span>

- <span data-ttu-id="1c893-121">Možnost 2: Soubor PBX Office 365 Enterprise E3 + Skype pro firmy</span><span class="sxs-lookup"><span data-stu-id="1c893-121">Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span></span>

- <span data-ttu-id="1c893-122">Možnost 3: Office 365 Enterprise E3 + Skype pro firmy plus CAL (cenová a parita funkčnosti s E4)</span><span class="sxs-lookup"><span data-stu-id="1c893-122">Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (price and functionality parity with E4)</span></span>

- <span data-ttu-id="1c893-123">Možnost 4: Office 365 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="1c893-123">Option 4: Office 365 Enterprise E3</span></span>


| <span data-ttu-id="1c893-124">Funkce</span><span class="sxs-lookup"><span data-stu-id="1c893-124">Feature</span></span> | <span data-ttu-id="1c893-125">Možnost 1</span><span class="sxs-lookup"><span data-stu-id="1c893-125">Option 1</span></span> | <span data-ttu-id="1c893-126">Možnost 2</span><span class="sxs-lookup"><span data-stu-id="1c893-126">Option 2</span></span> | <span data-ttu-id="1c893-127">Možnost 3</span><span class="sxs-lookup"><span data-stu-id="1c893-127">Option 3</span></span> | <span data-ttu-id="1c893-128">Možnost 4</span><span class="sxs-lookup"><span data-stu-id="1c893-128">Option 4</span></span> |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| <span data-ttu-id="1c893-129">Chcete získat všechny funkce zahrnuté v Office 365 Enterprise E4?</span><span class="sxs-lookup"><span data-stu-id="1c893-129">Get all the features included in Office 365 Enterprise E4?</span></span> | <span data-ttu-id="1c893-130">Yes</span><span class="sxs-lookup"><span data-stu-id="1c893-130">Yes</span></span> | <span data-ttu-id="1c893-131">Yes</span><span class="sxs-lookup"><span data-stu-id="1c893-131">Yes</span></span> | <span data-ttu-id="1c893-132">Yes</span><span class="sxs-lookup"><span data-stu-id="1c893-132">Yes</span></span> | <span data-ttu-id="1c893-133">No</span><span class="sxs-lookup"><span data-stu-id="1c893-133">No</span></span> |
| <span data-ttu-id="1c893-134">Telefonní čísla spravovaná v sadě Office 365?</span><span class="sxs-lookup"><span data-stu-id="1c893-134">Phone numbers managed in Office 365?</span></span> | <span data-ttu-id="1c893-135">Yes</span><span class="sxs-lookup"><span data-stu-id="1c893-135">Yes</span></span> | <span data-ttu-id="1c893-136">Yes</span><span class="sxs-lookup"><span data-stu-id="1c893-136">Yes</span></span> | <span data-ttu-id="1c893-137">No</span><span class="sxs-lookup"><span data-stu-id="1c893-137">No</span></span> | <span data-ttu-id="1c893-138">No</span><span class="sxs-lookup"><span data-stu-id="1c893-138">No</span></span> |
| <span data-ttu-id="1c893-139">Telefonní čísla spravovaná místně i v Office 365 (hybridní nasazení)?</span><span class="sxs-lookup"><span data-stu-id="1c893-139">Phone numbers managed both on-premises and in Office 365 (hybrid deployment)?</span></span> | <span data-ttu-id="1c893-140">Yes</span><span class="sxs-lookup"><span data-stu-id="1c893-140">Yes</span></span> | <span data-ttu-id="1c893-141">Yes</span><span class="sxs-lookup"><span data-stu-id="1c893-141">Yes</span></span> | <span data-ttu-id="1c893-142">No</span><span class="sxs-lookup"><span data-stu-id="1c893-142">No</span></span> | <span data-ttu-id="1c893-143">No</span><span class="sxs-lookup"><span data-stu-id="1c893-143">No</span></span> |
| <span data-ttu-id="1c893-144">Možnost přidání plánu hlasového volání veřejné telefonní sítě?</span><span class="sxs-lookup"><span data-stu-id="1c893-144">Option to add a PSTN voice calling plan?</span></span> | <span data-ttu-id="1c893-145">Yes</span><span class="sxs-lookup"><span data-stu-id="1c893-145">Yes</span></span> | <span data-ttu-id="1c893-146">Yes</span><span class="sxs-lookup"><span data-stu-id="1c893-146">Yes</span></span> | <span data-ttu-id="1c893-147">No</span><span class="sxs-lookup"><span data-stu-id="1c893-147">No</span></span> | <span data-ttu-id="1c893-148">No</span><span class="sxs-lookup"><span data-stu-id="1c893-148">No</span></span> |
| <span data-ttu-id="1c893-149">Konference v PSTN?</span><span class="sxs-lookup"><span data-stu-id="1c893-149">PSTN Conferencing?</span></span> | <span data-ttu-id="1c893-150">Yes</span><span class="sxs-lookup"><span data-stu-id="1c893-150">Yes</span></span> | <span data-ttu-id="1c893-151">No</span><span class="sxs-lookup"><span data-stu-id="1c893-151">No</span></span> | <span data-ttu-id="1c893-152">No</span><span class="sxs-lookup"><span data-stu-id="1c893-152">No</span></span> | <span data-ttu-id="1c893-153">No</span><span class="sxs-lookup"><span data-stu-id="1c893-153">No</span></span> |
| <span data-ttu-id="1c893-154">Rozšířené nástroje pro spolupráci, analýzu a zabezpečení?</span><span class="sxs-lookup"><span data-stu-id="1c893-154">Advanced tools for collaboration, analytics, and security?</span></span> | <span data-ttu-id="1c893-155">Yes</span><span class="sxs-lookup"><span data-stu-id="1c893-155">Yes</span></span> | <span data-ttu-id="1c893-156">No</span><span class="sxs-lookup"><span data-stu-id="1c893-156">No</span></span> | <span data-ttu-id="1c893-157">No</span><span class="sxs-lookup"><span data-stu-id="1c893-157">No</span></span> | <span data-ttu-id="1c893-158">No</span><span class="sxs-lookup"><span data-stu-id="1c893-158">No</span></span> |
| <span data-ttu-id="1c893-159">Interaktivní sestavy, řídicí panely a vizualizace dat?</span><span class="sxs-lookup"><span data-stu-id="1c893-159">Interactive reports, dashboards, and data visualizations?</span></span> | <span data-ttu-id="1c893-160">Yes</span><span class="sxs-lookup"><span data-stu-id="1c893-160">Yes</span></span> | <span data-ttu-id="1c893-161">No</span><span class="sxs-lookup"><span data-stu-id="1c893-161">No</span></span> | <span data-ttu-id="1c893-162">No</span><span class="sxs-lookup"><span data-stu-id="1c893-162">No</span></span> | <span data-ttu-id="1c893-163">No</span><span class="sxs-lookup"><span data-stu-id="1c893-163">No</span></span> | 
| <span data-ttu-id="1c893-164">Lepší kontrola zabezpečení dat a dodržování předpisů pomocí integrovaných uživatelských ovládacích prvků ochrany osobních údajů, transparentnosti a kontrastu?</span><span class="sxs-lookup"><span data-stu-id="1c893-164">More control over data security and compliance with built-in privacy, transparency, and refined user controls?</span></span> | <span data-ttu-id="1c893-165">Yes</span><span class="sxs-lookup"><span data-stu-id="1c893-165">Yes</span></span> | <span data-ttu-id="1c893-166">No</span><span class="sxs-lookup"><span data-stu-id="1c893-166">No</span></span> | <span data-ttu-id="1c893-167">No</span><span class="sxs-lookup"><span data-stu-id="1c893-167">No</span></span> | <span data-ttu-id="1c893-168">No</span><span class="sxs-lookup"><span data-stu-id="1c893-168">No</span></span> | 

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="1c893-169">Přechod zákazníků na nové plány produktů</span><span class="sxs-lookup"><span data-stu-id="1c893-169">Transition customers to new product plans</span></span>

<span data-ttu-id="1c893-170">Microsoft neustále nabízí našim partnerům nové produkty a služby.</span><span class="sxs-lookup"><span data-stu-id="1c893-170">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="1c893-171">V těchto případech možná budete muset upgradovat zákazníky na nové služby nebo migrovat své odběry z SKU, které se nakonec vypnou.</span><span class="sxs-lookup"><span data-stu-id="1c893-171">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="1c893-172">Migrace zákazníků z vyřazených SKU do novějších vyžaduje následující kroky:</span><span class="sxs-lookup"><span data-stu-id="1c893-172">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

-   <span data-ttu-id="1c893-173">Koupit nové předplatné</span><span class="sxs-lookup"><span data-stu-id="1c893-173">Purchase the new subscription</span></span>
-   <span data-ttu-id="1c893-174">Změna přiřazení licencí k aktuálním uživatelům</span><span class="sxs-lookup"><span data-stu-id="1c893-174">Reassign current user licenses</span></span>
-   <span data-ttu-id="1c893-175">Zrušit staré předplatné</span><span class="sxs-lookup"><span data-stu-id="1c893-175">Cancel the old subscription</span></span>

<span data-ttu-id="1c893-176">Pomocí těchto kroků migrujete předplatné Office 365 Enterprise E4 zákazníka na jednu z možností v tabulce výše.</span><span class="sxs-lookup"><span data-stu-id="1c893-176">Follow these steps to migrate a customer's Office 365 Enterprise E4 subscription to one of the options in the table above.</span></span>

### <a name="step-1---purchase-the-new-subscription"></a><span data-ttu-id="1c893-177">Krok 1 – Zakoupení nového předplatného</span><span class="sxs-lookup"><span data-stu-id="1c893-177">Step 1 - Purchase the new subscription</span></span>

1. <span data-ttu-id="1c893-178">V **Partnerské centrum** vyberte **Zákazníci,** vyberte zákazníka, který chcete přesunout, a pak vyberte **Přidat předplatná**.</span><span class="sxs-lookup"><span data-stu-id="1c893-178">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="1c893-179">Vyberte předplatné, které chcete zakoupit z katalogu (v tomto případě jednu z výše uvedených možností), zadejte počet licencí a pak vyberte **Odeslat.**</span><span class="sxs-lookup"><span data-stu-id="1c893-179">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

   <span data-ttu-id="1c893-180">Váš zákazník by teď měl mít stará i nová předplatná, staré předplatné Office 365 Enterprise E4 a nové cílové předplatné, například možnost 1 – Office 365 Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="1c893-180">Your customer should now have both old and new subscriptions, the old Office 365 Enterprise E4 subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise E5.</span></span>

### <a name="step-2---reassign-the-customers-users-licenses"></a><span data-ttu-id="1c893-181">Krok 2 – Opětovné přiřazení licencí uživatelů zákazníka</span><span class="sxs-lookup"><span data-stu-id="1c893-181">Step 2 - Reassign the customer's users' licenses</span></span>

1. <span data-ttu-id="1c893-182">V **Partnerské centrum** vyberte **Zákazníci,** vyberte zákazníka, který chcete přesunout, a pak vyberte **Uživatelé a licence.**</span><span class="sxs-lookup"><span data-stu-id="1c893-182">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Users and licenses**.</span></span> <span data-ttu-id="1c893-183">Otevře se stránka Uživatelé a licence zákazníka.</span><span class="sxs-lookup"><span data-stu-id="1c893-183">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="1c893-184">Pokud chcete znovu přiřadit uživatelské licence, vyberte uživatele, který chcete znovu přiřadit, a pak vyberte **Spravovat licence.**</span><span class="sxs-lookup"><span data-stu-id="1c893-184">To reassign user licenses, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="1c893-185">Na stránce **Spravovat licence** zrušte zaškrtnutí políčka Licence **Office 365 Enterprise E4** a vyberte nový plán služby pro předplatné, do které zákazník přesouvá.</span><span class="sxs-lookup"><span data-stu-id="1c893-185">On the **Manage licenses** page, clear the **Office 365 Enterprise E4** license check box and select a new service plan for the subscription the customer is moving to.</span></span>

4. <span data-ttu-id="1c893-186">Vyberte **Odeslat**.</span><span class="sxs-lookup"><span data-stu-id="1c893-186">Select **Submit**.</span></span> <span data-ttu-id="1c893-187">Na potvrzovací stránce se zobrazí nová přiřazení licencí.</span><span class="sxs-lookup"><span data-stu-id="1c893-187">A confirmation page lists the new license assignments.</span></span>

5. <span data-ttu-id="1c893-188">Pokračujte ve stejných krocích u všech ostatních zákaznických uživatelů, kteří potřebují znovu přiřadit licenci.</span><span class="sxs-lookup"><span data-stu-id="1c893-188">Continue the same steps with any other customer users that need license reassignment.</span></span>

<span data-ttu-id="1c893-189">Po přesunutí uživatelských licencí do nové služby můžete vyřazené předplatné bezpečně zrušit na nejvyšší úrovni zákazníka.</span><span class="sxs-lookup"><span data-stu-id="1c893-189">After moving the user licenses to the new service, you can safely cancel the retired subscription at the top Customer level.</span></span>

### <a name="step-3---cancel-the-old-subscription"></a><span data-ttu-id="1c893-190">Krok 3 – Zrušení starého předplatného</span><span class="sxs-lookup"><span data-stu-id="1c893-190">Step 3 - Cancel the old subscription</span></span>

1. <span data-ttu-id="1c893-191">V **nabídce Partnerské centrum** vyberte **Zákazníci.**</span><span class="sxs-lookup"><span data-stu-id="1c893-191">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="1c893-192">Vyberte zákazníka, kterého chcete přesunout, a vyberte předplatné, které chcete zrušit.</span><span class="sxs-lookup"><span data-stu-id="1c893-192">Select the customer you want to move, and select the subscription you want to cancel.</span></span>

2. <span data-ttu-id="1c893-193">Na stránce s podrobnostmi o předplatném nastavte stav předplatného na **Pozastaveno.**</span><span class="sxs-lookup"><span data-stu-id="1c893-193">In the subscription details page, set the subscription status to **Suspended**.</span></span>

3. <span data-ttu-id="1c893-194">Vyberte **Odeslat**.</span><span class="sxs-lookup"><span data-stu-id="1c893-194">Select **Submit**.</span></span>

<span data-ttu-id="1c893-195">Původní předplatné je pozastavené a nové předplatné je aktivní.</span><span class="sxs-lookup"><span data-stu-id="1c893-195">The old subscription is suspended and the new subscription is active.</span></span> <span data-ttu-id="1c893-196">Pozastavené předplatné bude po 120 dnech automaticky zrušeno.</span><span class="sxs-lookup"><span data-stu-id="1c893-196">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="1c893-197">Za staré předplatné se zákazníkovi ne účtuly žádné další poplatky.</span><span class="sxs-lookup"><span data-stu-id="1c893-197">The customer incurs no additional costs for the old subscription.</span></span>



 



