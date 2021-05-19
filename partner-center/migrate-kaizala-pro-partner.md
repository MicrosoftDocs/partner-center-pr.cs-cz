---
title: Migrace předplatných Kaizala Pro na Microsoft 365
description: Zjistěte, jak migrovat předplatná Kaizala Pro na Microsoft 365 nebo verze Office 365. Další podrobnosti o přechodu zákazníků najdete v tomto článku.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 583e9c40bb8d161c30440f12331dc8dcbf3db417
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146421"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft-365-or-office-365-versions"></a><span data-ttu-id="0ae56-104">Migrace samostatných předplatných Kaizala Pro na Microsoft 365 nebo verze Office 365</span><span class="sxs-lookup"><span data-stu-id="0ae56-104">Migrate Kaizala Pro Standalone subscriptions to Microsoft 365 or Office 365 versions</span></span>

<span data-ttu-id="0ae56-105">**Odpovídající role:** Agent prodeje</span><span class="sxs-lookup"><span data-stu-id="0ae56-105">**Appropriate roles**: Sales agent</span></span>

<span data-ttu-id="0ae56-106">Od 1. července 2020 Microsoft ukončí prodej samostatné služby Kaizala Pro.</span><span class="sxs-lookup"><span data-stu-id="0ae56-106">Effective July 1, 2020, Microsoft is ending sales of the Kaizala Pro standalone service.</span></span> <span data-ttu-id="0ae56-107">Zákazníci už nebudou moct po tomto datu kupovat nová předplatná Kaizala Pro a stávající předplatná Kaizala Pro se po vypršení jejich platnosti automaticky neobnoví.</span><span class="sxs-lookup"><span data-stu-id="0ae56-107">Customers will no longer be able to purchase new Kaizala Pro subscriptions after this date, and existing Kaizala Pro subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="0ae56-108">Pokud chcete zajistit kontinuitu pro zákazníky, měli byste zákazníky, kteří mají vypršenou platnost samostatných předplatných Kaizala Pro, pře převodovat na podporovanou možnost SKU uvedenou níže.</span><span class="sxs-lookup"><span data-stu-id="0ae56-108">To ensure continuity for customers, you should transition customers with expiring Kaizala Pro standalone subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="0ae56-109">Doporučujeme přestěhovat zákazníky na nová předplatná před ročním datem ukončení předplatného, abyste se vyhnuli výpadkům služeb pro zákazníky.</span><span class="sxs-lookup"><span data-stu-id="0ae56-109">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="0ae56-110">Pokud používáte rozhraní API (CREST nebo Partnerské centrum), můžete zjistit předplatná, kterým vyprší platnost, vyhodnocením koncového data odběru spolu s vlastností automatického obnovení nastavenou na false: `auto renew = False` .</span><span class="sxs-lookup"><span data-stu-id="0ae56-110">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew property set to false: `auto renew = False`.</span></span>

<span data-ttu-id="0ae56-111">Předplatná E4 se nastaví na `auto renew=False` 1. července 2020.</span><span class="sxs-lookup"><span data-stu-id="0ae56-111">The E4 subscriptions will be set to `auto renew=False` on July 1, 2020.</span></span> <span data-ttu-id="0ae56-112">Zákazníky můžete kdykoli přesunout do nového plánu.</span><span class="sxs-lookup"><span data-stu-id="0ae56-112">You can move customers to a new plan at any time.</span></span>

## <a name="kaizala-pro-standalone-replacement-plans"></a><span data-ttu-id="0ae56-113">Náhradní plány Kaizala Pro Standalone</span><span class="sxs-lookup"><span data-stu-id="0ae56-113">Kaizala Pro Standalone replacement plans</span></span>

<span data-ttu-id="0ae56-114">S těmito novými plány mohou vaši zákazníci využívat novější funkce v Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0ae56-114">With the new plans, your customers can take advantage of newer features and functionality in Microsoft 365.</span></span> <span data-ttu-id="0ae56-115">Podrobnosti o cenách najdete v matici ceníku a seznamu nabídek v Partnerské centrum.</span><span class="sxs-lookup"><span data-stu-id="0ae56-115">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span>

- <span data-ttu-id="0ae56-116">[**Microsoft 365 for Business,**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2)včetně:</span><span class="sxs-lookup"><span data-stu-id="0ae56-116">[**Microsoft 365 for Business**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), including:</span></span>  
   - <span data-ttu-id="0ae56-117">Microsoft 365 Business Basic</span><span class="sxs-lookup"><span data-stu-id="0ae56-117">Microsoft 365 Business Basic</span></span>
   - <span data-ttu-id="0ae56-118">Microsoft 365 Business Standard</span><span class="sxs-lookup"><span data-stu-id="0ae56-118">Microsoft 365 Business Standard</span></span>
   - <span data-ttu-id="0ae56-119">Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="0ae56-119">Microsoft 365 Business Premium</span></span>
    
- <span data-ttu-id="0ae56-120">[**Microsoft 365 pro frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), včetně:</span><span class="sxs-lookup"><span data-stu-id="0ae56-120">[**Microsoft 365 for Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), including:</span></span>
   - <span data-ttu-id="0ae56-121">Microsoft 365 F3 (dříve Microsoft 365 F1) a Office 365 F3</span><span class="sxs-lookup"><span data-stu-id="0ae56-121">Microsoft 365 F3 (formerly Microsoft 365 F1) and Office 365 F3</span></span>
    
- <span data-ttu-id="0ae56-122">[**Microsoft 365 pro podniky**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), včetně:</span><span class="sxs-lookup"><span data-stu-id="0ae56-122">[**Microsoft 365 for Enterprise**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), including:</span></span> 
   - <span data-ttu-id="0ae56-123">Office 365 E1</span><span class="sxs-lookup"><span data-stu-id="0ae56-123">Office 365 E1</span></span>
   - <span data-ttu-id="0ae56-124">Microsoft 365 E3 a Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="0ae56-124">Microsoft 365 E3 and Office 365 E3</span></span>
   - <span data-ttu-id="0ae56-125">Microsoft 365 E5 a Office 365 E5</span><span class="sxs-lookup"><span data-stu-id="0ae56-125">Microsoft 365 E5 and Office 365 E5</span></span>

- <span data-ttu-id="0ae56-126">[**Microsoft 365 pro vzdělávání**](https://www.microsoft.com/education/buy-license/microsoft365), včetně:</span><span class="sxs-lookup"><span data-stu-id="0ae56-126">[**Microsoft 365 for Education**](https://www.microsoft.com/education/buy-license/microsoft365), including:</span></span> 
    - <span data-ttu-id="0ae56-127">Microsoft 365 a1 a Office 365 a1</span><span class="sxs-lookup"><span data-stu-id="0ae56-127">Microsoft 365 A1 and Office 365 A1</span></span>
    - <span data-ttu-id="0ae56-128">Microsoft 365 a3 a Office 365 a3</span><span class="sxs-lookup"><span data-stu-id="0ae56-128">Microsoft 365 A3 and Office 365 A3</span></span>
    - <span data-ttu-id="0ae56-129">Microsoft 365 a5 a Office 365 a5</span><span class="sxs-lookup"><span data-stu-id="0ae56-129">Microsoft 365 A5 and Office 365 A5</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="0ae56-130">Přechod zákazníků na nové plány produktů</span><span class="sxs-lookup"><span data-stu-id="0ae56-130">Transition customers to new product plans</span></span>

<span data-ttu-id="0ae56-131">Microsoft neustále nabízí našim partnerům nové produkty a služby.</span><span class="sxs-lookup"><span data-stu-id="0ae56-131">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="0ae56-132">V těchto případech možná budete muset upgradovat zákazníky na nové služby nebo migrovat své odběry z SKU, které se nakonec vypnou.</span><span class="sxs-lookup"><span data-stu-id="0ae56-132">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="0ae56-133">Migrace zákazníků z vyřazených SKU do novějších vyžaduje následující kroky:</span><span class="sxs-lookup"><span data-stu-id="0ae56-133">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

<span data-ttu-id="0ae56-134">A.</span><span class="sxs-lookup"><span data-stu-id="0ae56-134">A.</span></span> <span data-ttu-id="0ae56-135">Koupit nové předplatné</span><span class="sxs-lookup"><span data-stu-id="0ae56-135">Purchase the new subscription</span></span>

<span data-ttu-id="0ae56-136">B.</span><span class="sxs-lookup"><span data-stu-id="0ae56-136">B.</span></span> <span data-ttu-id="0ae56-137">Změna přiřazení licencí k aktuálním uživatelům</span><span class="sxs-lookup"><span data-stu-id="0ae56-137">Reassign current user licenses</span></span>

<span data-ttu-id="0ae56-138">C.</span><span class="sxs-lookup"><span data-stu-id="0ae56-138">C.</span></span> <span data-ttu-id="0ae56-139">Zrušit staré předplatné</span><span class="sxs-lookup"><span data-stu-id="0ae56-139">Cancel old subscription</span></span>


## <a name="migrate-your-customers-to-new-plans"></a><span data-ttu-id="0ae56-140">Migrace zákazníků na nové plány</span><span class="sxs-lookup"><span data-stu-id="0ae56-140">Migrate your customers to new plans</span></span>

### <a name="a-purchase-the-new-subscription"></a><span data-ttu-id="0ae56-141">A.</span><span class="sxs-lookup"><span data-stu-id="0ae56-141">A.</span></span> <span data-ttu-id="0ae56-142">Koupit nové předplatné</span><span class="sxs-lookup"><span data-stu-id="0ae56-142">Purchase the new subscription</span></span>

1. <span data-ttu-id="0ae56-143">Pokud chcete nové předplatné koupit, vyberte v nabídce **Partnerské centrum** možnost **zákazníci**, vyberte zákazníka, kterého chcete přesunout, a pak vyberte **Přidat předplatná**.</span><span class="sxs-lookup"><span data-stu-id="0ae56-143">To purchase the new subscription, from the **Partner Center** menu, select **Customers**, select the customer you want to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="0ae56-144">Vyberte předplatné, které chcete z katalogu koupit (v tomto případě jednu z výše uvedených možností), zadejte počet licencí a pak vyberte **Odeslat**.</span><span class="sxs-lookup"><span data-stu-id="0ae56-144">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

<span data-ttu-id="0ae56-145">Váš zákazník by teď měl mít staré i nové předplatné, staré předplatné Kaizala pro a nové předplatné Target, třeba možnost 1 – Office 365 Enterprise F1.</span><span class="sxs-lookup"><span data-stu-id="0ae56-145">Your customer should now have both old and new subscriptions, the old Kaizala Pro Standalone subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise F1.</span></span>

### <a name="b-reassign-current-user-licenses"></a><span data-ttu-id="0ae56-146">B.</span><span class="sxs-lookup"><span data-stu-id="0ae56-146">B.</span></span> <span data-ttu-id="0ae56-147">Opětovné přiřazení aktuálních uživatelských licencí</span><span class="sxs-lookup"><span data-stu-id="0ae56-147">Reassign current user licenses</span></span>

1. <span data-ttu-id="0ae56-148">Pokud chcete znovu přiřadit licence uživatelů zákazníka, v nabídce **Partnerské centrum** vyberte **Zákazníci,** vyberte zákazníka, který přesouváte, a pak vyberte Uživatelé a **licence.**</span><span class="sxs-lookup"><span data-stu-id="0ae56-148">To reassign the customer's users' licenses, from the **Partner Center** menu, select **Customers**, select the customer you are moving, and then select **Users and licenses**.</span></span> <span data-ttu-id="0ae56-149">Otevře se stránka Uživatelé a licence zákazníka.</span><span class="sxs-lookup"><span data-stu-id="0ae56-149">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="0ae56-150">Pokud chcete znovu přiřadit uživatelskou licenci, vyberte uživatele, který chcete znovu přiřadit, a pak vyberte **Spravovat licence.**</span><span class="sxs-lookup"><span data-stu-id="0ae56-150">To reassign user license, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="0ae56-151">Na stránce **Spravovat licence** zrušte zaškrtnutí políčka Kaizala Pro Standalone license (Samostatná licence Kaizala Pro) a vyberte nový plán služby pro předplatné, do které zákazník přemísťuje.</span><span class="sxs-lookup"><span data-stu-id="0ae56-151">On the **Manage licenses** page, clear the Kaizala Pro Standalone license check box, and select a new service plan for the subscription the customer is moving to.</span></span>

4.  <span data-ttu-id="0ae56-152">Vyberte **Odeslat**.</span><span class="sxs-lookup"><span data-stu-id="0ae56-152">Select **Submit**.</span></span> <span data-ttu-id="0ae56-153">Na potvrzovací stránce se zobrazí nová přiřazení licencí.</span><span class="sxs-lookup"><span data-stu-id="0ae56-153">A confirmation page lists the new license assignments.</span></span> <span data-ttu-id="0ae56-154">Pokračujte stejným způsobem i pro ostatní uživatele, kteří potřebují přiřazení licencí.</span><span class="sxs-lookup"><span data-stu-id="0ae56-154">Continue this same process for other users who need license assignments.</span></span>

### <a name="c-cancel-old-subscription"></a><span data-ttu-id="0ae56-155">C.</span><span class="sxs-lookup"><span data-stu-id="0ae56-155">C.</span></span> <span data-ttu-id="0ae56-156">Zrušení starého předplatného</span><span class="sxs-lookup"><span data-stu-id="0ae56-156">Cancel old subscription</span></span>

<span data-ttu-id="0ae56-157">Po přesunutí uživatelské licence na novou službu můžete vyřazené předplatné bezpečně zrušit na úrovni zákazníka.</span><span class="sxs-lookup"><span data-stu-id="0ae56-157">After moving the user license to the new service, you can safely cancel the retired subscription at the customer level.</span></span>

1.  <span data-ttu-id="0ae56-158">V **nabídce Partnerské centrum** vyberte **Zákazníci.**</span><span class="sxs-lookup"><span data-stu-id="0ae56-158">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="0ae56-159">Vyberte zákazníka, jehož předplatné zrušíte.</span><span class="sxs-lookup"><span data-stu-id="0ae56-159">Select the customer whose subscription you are canceling.</span></span>

2.  <span data-ttu-id="0ae56-160">Na stránce s podrobnostmi o předplatném nastavte předplatné na **Pozastaveno.**</span><span class="sxs-lookup"><span data-stu-id="0ae56-160">In the subscription detail page, set the subscription to **Suspended**.</span></span>

3.  <span data-ttu-id="0ae56-161">Vyberte **Odeslat**.</span><span class="sxs-lookup"><span data-stu-id="0ae56-161">Select **Submit**.</span></span>

<span data-ttu-id="0ae56-162">Původní předplatné je pozastavené a nové předplatné je aktivní.</span><span class="sxs-lookup"><span data-stu-id="0ae56-162">The old subscription is suspended, and the new subscription is active.</span></span> <span data-ttu-id="0ae56-163">Pozastavené předplatné bude po 120 dnech automaticky zrušeno.</span><span class="sxs-lookup"><span data-stu-id="0ae56-163">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="0ae56-164">Za staré předplatné se zákazníkovi ne účtuly žádné další poplatky.</span><span class="sxs-lookup"><span data-stu-id="0ae56-164">The customer incurs no additional costs for the old subscription.</span></span>
