---
title: Migrace některých předplatných Skypu pro firmy
description: Zjistěte, jak a kdy migrovat určité zákazníky s vypršeným platnostim předplatných Online Skypu pro firmy Plan 1 na nové verze Office 365.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 06/03/2020
ms.openlocfilehash: 0e8289ad06dbc8a95f5cff22ca386176d6ba65ab
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854821"
---
# <a name="migrate-skype-for-business-online-plan-1-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="3b526-103">Migrace předplatných Online Skypu pro firmy (plán 1) na novější verze Office 365</span><span class="sxs-lookup"><span data-stu-id="3b526-103">Migrate Skype for Business Online Plan 1 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="3b526-104">**Odpovídající role:** Agent prodeje</span><span class="sxs-lookup"><span data-stu-id="3b526-104">**Appropriate roles**: Sales agent</span></span>

<span data-ttu-id="3b526-105">Online Skype for Business Plan 1 bude od 1. srpna 2018 vyřazen z provozu.</span><span class="sxs-lookup"><span data-stu-id="3b526-105">The Skype for Business Online Plan 1 will be retired, effective August 1, 2018.</span></span> <span data-ttu-id="3b526-106">Po tomto datu už zákazníci nebudou moci kupovat nová předplatná Skypu pro firmy s plánem 1 a stávající předplatná se po vypršení jejich platnosti automaticky neobnoví a neposkytnou možnost prodloužení.</span><span class="sxs-lookup"><span data-stu-id="3b526-106">After that date customers can no longer purchase new Skype for Business Plan 1 subscriptions, and existing subscriptions will not renew automatically when they expire and will not provide a renewal option.</span></span> <span data-ttu-id="3b526-107">Na stránce s podrobnostmi o předplatném se stav předplatného Online Skypu pro firmy (Plán 1) změnil na Platnost vyprší [datum]" z "Automatické prodlužování platnosti k [datum]".</span><span class="sxs-lookup"><span data-stu-id="3b526-107">On the subscription's detail page, the Skype for Business Online Plan 1 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span>  

<span data-ttu-id="3b526-108">Pokud chcete zajistit kontinuitu pro zákazníky, měli byste zákazníky s vypršením platnosti předplatných Online Skypu pro firmy ( Plán 1) přeplánovat na podporovanou možnost SKU uvedenou níže.</span><span class="sxs-lookup"><span data-stu-id="3b526-108">To ensure continuity for customers, you should transition customers with expiring Skype for Business Online Plan 1 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="3b526-109">Doporučujeme přestěhovat zákazníky na nová předplatná před ročním datem ukončení předplatného, abyste se vyhnuli výpadkům služeb pro zákazníky.</span><span class="sxs-lookup"><span data-stu-id="3b526-109">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

>[!NOTE]
><span data-ttu-id="3b526-110">Komerční i státní SKU Skypu pro firmy Online Plán 1 jsou vyřazené z provozu.</span><span class="sxs-lookup"><span data-stu-id="3b526-110">Both Skype for Business Online Plan 1 commercial and government SKUs are retired.</span></span>

<span data-ttu-id="3b526-111">Pokud používáte rozhraní API (CREST nebo Partnerské centrum), vyhledejte předplatná, kterým vyprší platnost, vyhodnocením koncového data odběru spolu s vlastností auto renew = False.</span><span class="sxs-lookup"><span data-stu-id="3b526-111">If you use the API (either CREST or Partner Center), find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="3b526-112">Předplatná Online Skypu pro firmy Plan 1 se 1. září 2018 nastaví na auto renew=False.</span><span class="sxs-lookup"><span data-stu-id="3b526-112">The Skype for Business Online Plan 1 subscriptions will be set to auto renew=False on September 1, 2018.</span></span> <span data-ttu-id="3b526-113">Zákazníky můžete kdykoli přesunout do nového plánu.</span><span class="sxs-lookup"><span data-stu-id="3b526-113">You can move customers to a new plan at any time.</span></span> 

## <a name="skype-for-business-online-plan-1-replacement-plans"></a><span data-ttu-id="3b526-114">Náhradní plány online Skypu pro firmy – Plán 1</span><span class="sxs-lookup"><span data-stu-id="3b526-114">Skype for Business Online Plan 1 replacement plans</span></span>

<span data-ttu-id="3b526-115">S novými plány mohou vaši zákazníci využívat novější funkce v Office 365.</span><span class="sxs-lookup"><span data-stu-id="3b526-115">With the new plans, your customers take can advantage of newer features and functionality in Office 365.</span></span> <span data-ttu-id="3b526-116">Podrobnosti o cenách najdete v matici ceníku a seznamu nabídek v Partnerské centrum.</span><span class="sxs-lookup"><span data-stu-id="3b526-116">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> 

- <span data-ttu-id="3b526-117">Možnost 1: Office 365 Enterprise F1</span><span class="sxs-lookup"><span data-stu-id="3b526-117">Option 1: Office 365 Enterprise F1</span></span>
- <span data-ttu-id="3b526-118">Možnost 2: Microsoft 365 Enterprise F1</span><span class="sxs-lookup"><span data-stu-id="3b526-118">Option 2: Microsoft 365 Enterprise F1</span></span>
- <span data-ttu-id="3b526-119">Možnost 3: Další plány Office 365</span><span class="sxs-lookup"><span data-stu-id="3b526-119">Option 3: Other Office 365 plans</span></span>

|<span data-ttu-id="3b526-120">**Funkce**</span><span class="sxs-lookup"><span data-stu-id="3b526-120">**Feature**</span></span>    |<span data-ttu-id="3b526-121">**Možnost 1**</span><span class="sxs-lookup"><span data-stu-id="3b526-121">**Option 1**</span></span>   |<span data-ttu-id="3b526-122">**Možnost 2**</span><span class="sxs-lookup"><span data-stu-id="3b526-122">**Option 2**</span></span>   |<span data-ttu-id="3b526-123">**Možnost 3**</span><span class="sxs-lookup"><span data-stu-id="3b526-123">**Option 3**</span></span>   |
|:-----------------|:-----------------|:-------------|:------------|
|<span data-ttu-id="3b526-124">Získejte všechny funkce, které jsou součástí Online Skypu pro firmy – Plán 1.</span><span class="sxs-lookup"><span data-stu-id="3b526-124">Get all the features included in Skype for Business Online Plan 1</span></span>|<span data-ttu-id="3b526-125">Yes</span><span class="sxs-lookup"><span data-stu-id="3b526-125">Yes</span></span>   |<span data-ttu-id="3b526-126">Yes</span><span class="sxs-lookup"><span data-stu-id="3b526-126">Yes</span></span>   |<span data-ttu-id="3b526-127">Yes</span><span class="sxs-lookup"><span data-stu-id="3b526-127">Yes</span></span>   |
|<span data-ttu-id="3b526-128">IM a přítomnost</span><span class="sxs-lookup"><span data-stu-id="3b526-128">IM and presence</span></span> |<span data-ttu-id="3b526-129">Yes</span><span class="sxs-lookup"><span data-stu-id="3b526-129">Yes</span></span>   |<span data-ttu-id="3b526-130">Yes</span><span class="sxs-lookup"><span data-stu-id="3b526-130">Yes</span></span>   |<span data-ttu-id="3b526-131">Yes</span><span class="sxs-lookup"><span data-stu-id="3b526-131">Yes</span></span>   |
|<span data-ttu-id="3b526-132">Zvuk a video peer-to-peer přes IP adresu</span><span class="sxs-lookup"><span data-stu-id="3b526-132">Peer-to-peer Audio and Video over IP</span></span>|<span data-ttu-id="3b526-133">Yes</span><span class="sxs-lookup"><span data-stu-id="3b526-133">Yes</span></span>   |<span data-ttu-id="3b526-134">Yes</span><span class="sxs-lookup"><span data-stu-id="3b526-134">Yes</span></span>   |<span data-ttu-id="3b526-135">Yes</span><span class="sxs-lookup"><span data-stu-id="3b526-135">Yes</span></span>   
|<span data-ttu-id="3b526-136">Připojit schůzky jako ověřeného uživatele</span><span class="sxs-lookup"><span data-stu-id="3b526-136">Join meetings as an authenticated user</span></span>| <span data-ttu-id="3b526-137">Yes</span><span class="sxs-lookup"><span data-stu-id="3b526-137">Yes</span></span>   |<span data-ttu-id="3b526-138">Yes</span><span class="sxs-lookup"><span data-stu-id="3b526-138">Yes</span></span>   |<span data-ttu-id="3b526-139">Yes</span><span class="sxs-lookup"><span data-stu-id="3b526-139">Yes</span></span>   |

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="3b526-140">Přechod zákazníků na nové plány produktů</span><span class="sxs-lookup"><span data-stu-id="3b526-140">Transition customers to new product plans</span></span>

<span data-ttu-id="3b526-141">Microsoft neustále nabízí našim partnerům nové produkty a služby.</span><span class="sxs-lookup"><span data-stu-id="3b526-141">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="3b526-142">V těchto případech možná budete muset upgradovat zákazníky na nové služby nebo migrovat své odběry z SKU, které se nakonec vypnou.</span><span class="sxs-lookup"><span data-stu-id="3b526-142">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="3b526-143">Migrace zákazníků z vyřazených SKU do novějších vyžaduje následující kroky:</span><span class="sxs-lookup"><span data-stu-id="3b526-143">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

- <span data-ttu-id="3b526-144">Koupit nové předplatné</span><span class="sxs-lookup"><span data-stu-id="3b526-144">Purchase the new subscription</span></span>
- <span data-ttu-id="3b526-145">Změna přiřazení licencí k aktuálním uživatelům</span><span class="sxs-lookup"><span data-stu-id="3b526-145">Reassign current user licenses</span></span>
- <span data-ttu-id="3b526-146">Zrušit staré předplatné</span><span class="sxs-lookup"><span data-stu-id="3b526-146">Cancel old subscription</span></span>

### <a name="migrate-your-customers-to-new-plans"></a><span data-ttu-id="3b526-147">Migrace zákazníků na nové plány</span><span class="sxs-lookup"><span data-stu-id="3b526-147">Migrate your customers to new plans</span></span>

1. <span data-ttu-id="3b526-148">Pokud chcete nové předplatné koupit, vyberte v **nabídce partnerské Centrum** možnost **zákazníci**, vyberte zákazníka, kterého chcete přesunout, a pak vyberte **Přidat předplatná**.</span><span class="sxs-lookup"><span data-stu-id="3b526-148">To purchase the new subscription, from the **Partner Center menu**, select **Customers**, select the customer you want to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="3b526-149">Vyberte předplatné, které chcete z katalogu koupit (v tomto případě jednu z výše uvedených možností), zadejte počet licencí a pak vyberte **Odeslat**.</span><span class="sxs-lookup"><span data-stu-id="3b526-149">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="3b526-150">Váš zákazník by teď měl mít staré i nové předplatné, staré předplatné online pro Skype pro firmy a nové předplatné Target, třeba možnost 1 – Office 365 Enterprise F1.</span><span class="sxs-lookup"><span data-stu-id="3b526-150">Your customer should now have both old and new subscriptions, the old Skype for Business Online Plan 1  subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise F1.</span></span>

3. <span data-ttu-id="3b526-151">Pokud chcete znovu přiřadit licence uživatelů zákazníka, vyberte v nabídce **Partnerské centrum** možnost **zákazníci**, vyberte zákazníka, kterého přesouváte, a pak vyberte **Uživatelé a licence**.</span><span class="sxs-lookup"><span data-stu-id="3b526-151">To reassign the customer's users' licenses, from the **Partner Center** menu, select **Customers**, select the customer you are moving, and then select **Users and licenses**.</span></span> <span data-ttu-id="3b526-152">Otevře se stránka uživatelé a licence zákazníka.</span><span class="sxs-lookup"><span data-stu-id="3b526-152">The customer's Users and Licenses page opens.</span></span>

4. <span data-ttu-id="3b526-153">Pokud chcete znovu přiřadit uživatelskou licenci, vyberte uživatele, kterého chcete znovu přiřadit, a pak vyberte **spravovat licence.**</span><span class="sxs-lookup"><span data-stu-id="3b526-153">To reassign user license, select the user to reassign and then select **Manage licenses.**</span></span>

5. <span data-ttu-id="3b526-154">Na stránce **spravovat licence** zrušte zaškrtnutí políčka licence pro Skype for Business Online Plan 1 a vyberte nový plán služby pro předplatné, na které se bude zákazník pohybovat.</span><span class="sxs-lookup"><span data-stu-id="3b526-154">On the **Manage licenses** page, clear the Skype for Business Online Plan 1 license check box and select a new service plan for the subscription the customer is moving to.</span></span>

6. <span data-ttu-id="3b526-155">Vyberte **Odeslat**.</span><span class="sxs-lookup"><span data-stu-id="3b526-155">Select **Submit**.</span></span> <span data-ttu-id="3b526-156">Stránka s potvrzením obsahuje seznam nových přiřazení licencí.</span><span class="sxs-lookup"><span data-stu-id="3b526-156">A confirmation page lists the new license assignments.</span></span> <span data-ttu-id="3b526-157">Pokračujte stejným postupem pro ostatní uživatele, kteří potřebují přiřazení licencí.</span><span class="sxs-lookup"><span data-stu-id="3b526-157">Continue this same process for other users who need license assignments.</span></span>

<span data-ttu-id="3b526-158">Po přesunutí uživatelské licence na novou službu můžete vyřazené předplatné bezpečně zrušit na úrovni zákazníka.</span><span class="sxs-lookup"><span data-stu-id="3b526-158">After moving the user license to the new service, you can safely cancel the retired subscription at the customer level.</span></span>

7. <span data-ttu-id="3b526-159">V **nabídce Partnerské centrum** vyberte **Zákazníci.**</span><span class="sxs-lookup"><span data-stu-id="3b526-159">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="3b526-160">Vyberte zákazníka, jehož předplatné zrušíte.</span><span class="sxs-lookup"><span data-stu-id="3b526-160">Select the customer whose subscription you are canceling.</span></span>

8. <span data-ttu-id="3b526-161">Na stránce s podrobnostmi o předplatném nastavte předplatné na **Pozastaveno.**</span><span class="sxs-lookup"><span data-stu-id="3b526-161">In the subscription detail page, set the subscription to **Suspended**.</span></span>

9. <span data-ttu-id="3b526-162">Vyberte **Odeslat.**</span><span class="sxs-lookup"><span data-stu-id="3b526-162">Select **Submit.**</span></span>

<span data-ttu-id="3b526-163">Původní předplatné je pozastavené a nové předplatné je aktivní.</span><span class="sxs-lookup"><span data-stu-id="3b526-163">The old subscription is suspended, and the new subscription is active.</span></span> <span data-ttu-id="3b526-164">Pozastavené předplatné bude po 120 dnech automaticky zrušeno.</span><span class="sxs-lookup"><span data-stu-id="3b526-164">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="3b526-165">Za staré předplatné se zákazníkovi ne účtuly žádné další poplatky.</span><span class="sxs-lookup"><span data-stu-id="3b526-165">The customer incurs no additional costs for the old subscription.</span></span>

## <a name="next-steps"></a><span data-ttu-id="3b526-166">Další kroky</span><span class="sxs-lookup"><span data-stu-id="3b526-166">Next steps</span></span>

- [<span data-ttu-id="3b526-167">Poradci: Vytvoření a odeslání pozvánky ke zkušební verzi pro klienty, kteří si mohou vyzkoušet Office 365</span><span class="sxs-lookup"><span data-stu-id="3b526-167">Advisors: Create and send a trial invitation for clients to try Office 365</span></span>](advisors-create-a-trial-invitation.md)
- [<span data-ttu-id="3b526-168">Poradci: Vytvoření klientské základny pomocí pozvánek ke zkušební verzi Office 365 a nabídek k nákupu</span><span class="sxs-lookup"><span data-stu-id="3b526-168">Advisors: Build your client base with Office 365 trial invitations and purchase offers</span></span>](advisors-build-your-business.md)
- [<span data-ttu-id="3b526-169">Poradci: Vytvoření nabídky nákupu</span><span class="sxs-lookup"><span data-stu-id="3b526-169">Advisors: Create a purchase offer</span></span>](advisor-create-a-purchase-offer.md)
