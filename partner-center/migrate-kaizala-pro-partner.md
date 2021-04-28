---
title: Migrace předplatných Kaizala Pro na Microsoft 365
description: Přečtěte si, jak migrovat odběry Kaizala pro do Microsoft 365 nebo verzí Office 365. Přečtěte si tento článek, kde najdete další podrobnosti o přechodu zákazníků.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 96d18c8f728c56b705d378ac56dcf46e777157f0
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172400"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft-365-or-office-365-versions"></a><span data-ttu-id="b7f4e-104">Migrace samostatného předplatného Kaizala pro na verze Microsoft 365 nebo Office 365</span><span class="sxs-lookup"><span data-stu-id="b7f4e-104">Migrate Kaizala Pro Standalone subscriptions to Microsoft 365 or Office 365 versions</span></span>

<span data-ttu-id="b7f4e-105">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="b7f4e-105">**Appropriate roles**</span></span>

- <span data-ttu-id="b7f4e-106">Agent prodeje</span><span class="sxs-lookup"><span data-stu-id="b7f4e-106">Sales agent</span></span>

<span data-ttu-id="b7f4e-107">Od 1. července 2020 společnost Microsoft ukončuje prodej samostatné služby Kaizala pro.</span><span class="sxs-lookup"><span data-stu-id="b7f4e-107">Effective July 1, 2020, Microsoft is ending sales of the Kaizala Pro standalone service.</span></span> <span data-ttu-id="b7f4e-108">Zákazníci už nebudou moct koupit nové předplatné Kaizala pro po tomto datu a stávající předplatné Kaizala pro se po uplynutí této doby nebudou automaticky obnovovat.</span><span class="sxs-lookup"><span data-stu-id="b7f4e-108">Customers will no longer be able to purchase new Kaizala Pro subscriptions after this date, and existing Kaizala Pro subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="b7f4e-109">Chcete-li zajistit kontinuitu pro zákazníky, doporučujeme, abyste zákazníkům přešli do vypršení platnosti samostatného předplatného Kaizala pro s podporovanou možností SKU, která je uvedená níže.</span><span class="sxs-lookup"><span data-stu-id="b7f4e-109">To ensure continuity for customers, you should transition customers with expiring Kaizala Pro standalone subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="b7f4e-110">Doporučujeme zákazníkům přesunout nové předplatné před uplynutím ročního koncového data předplatného, aby se předešlo výpadkům služby pro zákazníky.</span><span class="sxs-lookup"><span data-stu-id="b7f4e-110">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="b7f4e-111">Pokud používáte rozhraní API (buď CREST nebo Partnerská centra), můžete zjistit platnost předplatných, a to tak, že vyhodnocujete koncové datum předplatného spolu s vlastností automatického obnovení nastavenou na hodnotu NEPRAVDA: `auto renew = False` .</span><span class="sxs-lookup"><span data-stu-id="b7f4e-111">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew property set to false: `auto renew = False`.</span></span>

<span data-ttu-id="b7f4e-112">Odběry E4 budou nastavené na `auto renew=False` 1. července 2020.</span><span class="sxs-lookup"><span data-stu-id="b7f4e-112">The E4 subscriptions will be set to `auto renew=False` on July 1, 2020.</span></span> <span data-ttu-id="b7f4e-113">Zákazníky můžete kdykoli přesunout do nového plánu.</span><span class="sxs-lookup"><span data-stu-id="b7f4e-113">You can move customers to a new plan at any time.</span></span>

## <a name="kaizala-pro-standalone-replacement-plans"></a><span data-ttu-id="b7f4e-114">Samostatné plány nahrazení Kaizala pro</span><span class="sxs-lookup"><span data-stu-id="b7f4e-114">Kaizala Pro Standalone replacement plans</span></span>

<span data-ttu-id="b7f4e-115">S novými plány můžou zákazníci využít výhod novějších funkcí a funkcí v Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="b7f4e-115">With the new plans, your customers can take advantage of newer features and functionality in Microsoft 365.</span></span> <span data-ttu-id="b7f4e-116">Podrobnosti o cenách najdete v seznamu ceníků a v tabulce seznam nabídek v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="b7f4e-116">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span>

- <span data-ttu-id="b7f4e-117">[**Microsoft 365 pro firmy**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), včetně:</span><span class="sxs-lookup"><span data-stu-id="b7f4e-117">[**Microsoft 365 for Business**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), including:</span></span>  
   - <span data-ttu-id="b7f4e-118">Microsoft 365 Business Basic</span><span class="sxs-lookup"><span data-stu-id="b7f4e-118">Microsoft 365 Business Basic</span></span>
   - <span data-ttu-id="b7f4e-119">Microsoft 365 Business Standard</span><span class="sxs-lookup"><span data-stu-id="b7f4e-119">Microsoft 365 Business Standard</span></span>
   - <span data-ttu-id="b7f4e-120">Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="b7f4e-120">Microsoft 365 Business Premium</span></span>
    
- <span data-ttu-id="b7f4e-121">[**Microsoft 365 pro prvotní**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), včetně:</span><span class="sxs-lookup"><span data-stu-id="b7f4e-121">[**Microsoft 365 for Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), including:</span></span>
   - <span data-ttu-id="b7f4e-122">Microsoft 365 F3 (dříve Microsoft 365 F1) a Office 365 F3</span><span class="sxs-lookup"><span data-stu-id="b7f4e-122">Microsoft 365 F3 (formerly Microsoft 365 F1) and Office 365 F3</span></span>
    
- <span data-ttu-id="b7f4e-123">[**Microsoft 365 pro podniky**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), včetně:</span><span class="sxs-lookup"><span data-stu-id="b7f4e-123">[**Microsoft 365 for Enterprise**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), including:</span></span> 
   - <span data-ttu-id="b7f4e-124">Office 365 E1</span><span class="sxs-lookup"><span data-stu-id="b7f4e-124">Office 365 E1</span></span>
   - <span data-ttu-id="b7f4e-125">Microsoft 365 E3 a Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="b7f4e-125">Microsoft 365 E3 and Office 365 E3</span></span>
   - <span data-ttu-id="b7f4e-126">Microsoft 365 E5 a Office 365 E5</span><span class="sxs-lookup"><span data-stu-id="b7f4e-126">Microsoft 365 E5 and Office 365 E5</span></span>

- <span data-ttu-id="b7f4e-127">[**Microsoft 365 pro vzdělávání**](https://www.microsoft.com/education/buy-license/microsoft365), včetně:</span><span class="sxs-lookup"><span data-stu-id="b7f4e-127">[**Microsoft 365 for Education**](https://www.microsoft.com/education/buy-license/microsoft365), including:</span></span> 
    - <span data-ttu-id="b7f4e-128">Microsoft 365 a1 a Office 365 a1</span><span class="sxs-lookup"><span data-stu-id="b7f4e-128">Microsoft 365 A1 and Office 365 A1</span></span>
    - <span data-ttu-id="b7f4e-129">Microsoft 365 a3 a Office 365 a3</span><span class="sxs-lookup"><span data-stu-id="b7f4e-129">Microsoft 365 A3 and Office 365 A3</span></span>
    - <span data-ttu-id="b7f4e-130">Microsoft 365 a5 a Office 365 a5</span><span class="sxs-lookup"><span data-stu-id="b7f4e-130">Microsoft 365 A5 and Office 365 A5</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="b7f4e-131">Přechod zákazníků na nové plány produktů</span><span class="sxs-lookup"><span data-stu-id="b7f4e-131">Transition customers to new product plans</span></span>

<span data-ttu-id="b7f4e-132">Microsoft neustále nabízí našim partnerům nové produkty a služby.</span><span class="sxs-lookup"><span data-stu-id="b7f4e-132">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="b7f4e-133">V těchto případech možná budete muset upgradovat zákazníky na nové služby nebo migrovat své odběry z SKU, které se nakonec vypnou.</span><span class="sxs-lookup"><span data-stu-id="b7f4e-133">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="b7f4e-134">Migrace zákazníků z vyřazených SKU do novějších vyžaduje následující kroky:</span><span class="sxs-lookup"><span data-stu-id="b7f4e-134">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

<span data-ttu-id="b7f4e-135">A.</span><span class="sxs-lookup"><span data-stu-id="b7f4e-135">A.</span></span> <span data-ttu-id="b7f4e-136">Koupit nové předplatné</span><span class="sxs-lookup"><span data-stu-id="b7f4e-136">Purchase the new subscription</span></span>

<span data-ttu-id="b7f4e-137">B.</span><span class="sxs-lookup"><span data-stu-id="b7f4e-137">B.</span></span> <span data-ttu-id="b7f4e-138">Změna přiřazení licencí k aktuálním uživatelům</span><span class="sxs-lookup"><span data-stu-id="b7f4e-138">Reassign current user licenses</span></span>

<span data-ttu-id="b7f4e-139">C.</span><span class="sxs-lookup"><span data-stu-id="b7f4e-139">C.</span></span> <span data-ttu-id="b7f4e-140">Zrušit staré předplatné</span><span class="sxs-lookup"><span data-stu-id="b7f4e-140">Cancel old subscription</span></span>


## <a name="migrate-your-customers-to-new-plans"></a><span data-ttu-id="b7f4e-141">Migrace zákazníků na nové plány</span><span class="sxs-lookup"><span data-stu-id="b7f4e-141">Migrate your customers to new plans</span></span>

### <a name="a-purchase-the-new-subscription"></a><span data-ttu-id="b7f4e-142">A.</span><span class="sxs-lookup"><span data-stu-id="b7f4e-142">A.</span></span> <span data-ttu-id="b7f4e-143">Koupit nové předplatné</span><span class="sxs-lookup"><span data-stu-id="b7f4e-143">Purchase the new subscription</span></span>

1. <span data-ttu-id="b7f4e-144">Pokud chcete nové předplatné koupit, vyberte v nabídce **Partnerské centrum** možnost **zákazníci**, vyberte zákazníka, kterého chcete přesunout, a pak vyberte **Přidat předplatná**.</span><span class="sxs-lookup"><span data-stu-id="b7f4e-144">To purchase the new subscription, from the **Partner Center** menu, select **Customers**, select the customer you want to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="b7f4e-145">Vyberte předplatné, které chcete z katalogu koupit (v tomto případě jednu z výše uvedených možností), zadejte počet licencí a pak vyberte **Odeslat**.</span><span class="sxs-lookup"><span data-stu-id="b7f4e-145">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

<span data-ttu-id="b7f4e-146">Váš zákazník by teď měl mít staré i nové předplatné, staré předplatné Kaizala pro a nové předplatné Target, třeba možnost 1 – Office 365 Enterprise F1.</span><span class="sxs-lookup"><span data-stu-id="b7f4e-146">Your customer should now have both old and new subscriptions, the old Kaizala Pro Standalone subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise F1.</span></span>

### <a name="b-reassign-current-user-licenses"></a><span data-ttu-id="b7f4e-147">B.</span><span class="sxs-lookup"><span data-stu-id="b7f4e-147">B.</span></span> <span data-ttu-id="b7f4e-148">Změna přiřazení licencí k aktuálním uživatelům</span><span class="sxs-lookup"><span data-stu-id="b7f4e-148">Reassign current user licenses</span></span>

1. <span data-ttu-id="b7f4e-149">Pokud chcete znovu přiřadit licence uživatelů zákazníka, vyberte v nabídce **Partnerské centrum** možnost **zákazníci**, vyberte zákazníka, kterého přesouváte, a pak vyberte **Uživatelé a licence**.</span><span class="sxs-lookup"><span data-stu-id="b7f4e-149">To reassign the customer's users' licenses, from the **Partner Center** menu, select **Customers**, select the customer you are moving, and then select **Users and licenses**.</span></span> <span data-ttu-id="b7f4e-150">Otevře se stránka uživatelé a licence zákazníka.</span><span class="sxs-lookup"><span data-stu-id="b7f4e-150">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="b7f4e-151">Pokud chcete znovu přiřadit uživatelskou licenci, vyberte uživatele, kterého chcete znovu přiřadit, a pak vyberte **spravovat licence**.</span><span class="sxs-lookup"><span data-stu-id="b7f4e-151">To reassign user license, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="b7f4e-152">Na stránce **spravovat licence** zrušte zaškrtnutí políčka Kaizala pro samostatnou licenci a vyberte nový plán služby pro předplatné, na které se bude zákazník pohybovat.</span><span class="sxs-lookup"><span data-stu-id="b7f4e-152">On the **Manage licenses** page, clear the Kaizala Pro Standalone license check box, and select a new service plan for the subscription the customer is moving to.</span></span>

4.  <span data-ttu-id="b7f4e-153">Vyberte **Odeslat**.</span><span class="sxs-lookup"><span data-stu-id="b7f4e-153">Select **Submit**.</span></span> <span data-ttu-id="b7f4e-154">Stránka s potvrzením obsahuje seznam nových přiřazení licencí.</span><span class="sxs-lookup"><span data-stu-id="b7f4e-154">A confirmation page lists the new license assignments.</span></span> <span data-ttu-id="b7f4e-155">Pokračujte stejným postupem pro ostatní uživatele, kteří potřebují přiřazení licencí.</span><span class="sxs-lookup"><span data-stu-id="b7f4e-155">Continue this same process for other users who need license assignments.</span></span>

### <a name="c-cancel-old-subscription"></a><span data-ttu-id="b7f4e-156">C.</span><span class="sxs-lookup"><span data-stu-id="b7f4e-156">C.</span></span> <span data-ttu-id="b7f4e-157">Zrušit staré předplatné</span><span class="sxs-lookup"><span data-stu-id="b7f4e-157">Cancel old subscription</span></span>

<span data-ttu-id="b7f4e-158">Po přesunutí uživatelské licence na novou službu můžete zrušit vyřazené předplatné na úrovni zákazníka.</span><span class="sxs-lookup"><span data-stu-id="b7f4e-158">After moving the user license to the new service, you can safely cancel the retired subscription at the customer level.</span></span>

1.  <span data-ttu-id="b7f4e-159">V nabídce **Partnerské centrum** vyberte **zákazníci**.</span><span class="sxs-lookup"><span data-stu-id="b7f4e-159">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="b7f4e-160">Vyberte zákazníka, jehož předplatné rušíte.</span><span class="sxs-lookup"><span data-stu-id="b7f4e-160">Select the customer whose subscription you are canceling.</span></span>

2.  <span data-ttu-id="b7f4e-161">Na stránce s podrobnostmi předplatného nastavte předplatné na **pozastaveno**.</span><span class="sxs-lookup"><span data-stu-id="b7f4e-161">In the subscription detail page, set the subscription to **Suspended**.</span></span>

3.  <span data-ttu-id="b7f4e-162">Vyberte **Odeslat**.</span><span class="sxs-lookup"><span data-stu-id="b7f4e-162">Select **Submit**.</span></span>

<span data-ttu-id="b7f4e-163">Staré předplatné je pozastavené a nové předplatné je aktivní.</span><span class="sxs-lookup"><span data-stu-id="b7f4e-163">The old subscription is suspended, and the new subscription is active.</span></span> <span data-ttu-id="b7f4e-164">Pozastavený odběr bude po 120 dnech automaticky zřízen.</span><span class="sxs-lookup"><span data-stu-id="b7f4e-164">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="b7f4e-165">Zákazník nevzniká žádné další poplatky za původní předplatné.</span><span class="sxs-lookup"><span data-stu-id="b7f4e-165">The customer incurs no additional costs for the old subscription.</span></span>
