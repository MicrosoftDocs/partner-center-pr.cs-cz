---
title: Migrace úplných předplatných Dynamics 365
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Přečtěte si, jak migrovat z kvalifikovaných předplatných, Basic Dynamics 365 na nové předplatné dřív, než vyprší platnost stávajících předplatných.
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5ba6992eff64031aed0dafeb5a5010983396ab63
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151640"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="b2391-103">Migrace Dynamics 365 a plánu Customer Engagement z úrovně Basic na novější verze (u kvalifikovaných nabídek)</span><span class="sxs-lookup"><span data-stu-id="b2391-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="b2391-104">**Příslušné role**: globální správce | Správce správy uživatelů | Agent správce | Agent prodeje</span><span class="sxs-lookup"><span data-stu-id="b2391-104">**Appropriate roles**: Global admin | User management admin | Admin agent | Sales agent</span></span>

<span data-ttu-id="b2391-105">Od 1. ledna 2019 zákazníci s Dynamics 365 for Sales/Customing Engagement ze základních (kvalifikovaných nabídek) odběry už nemůžou obnovit tyto starší nabídky. existující odběry se po vypršení platnosti automaticky neobnoví.</span><span class="sxs-lookup"><span data-stu-id="b2391-105">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="b2391-106">Na stránce s podrobnostmi o předplatném se stav předplatného změní na "vyprší dne [Date]" z "automatické obnovování v [datum]".</span><span class="sxs-lookup"><span data-stu-id="b2391-106">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="b2391-107">Chcete-li zajistit kontinuitu pro zákazníky, měli byste je přecházet s vypršením platnosti předplatných na podporovanou možnost, která je uvedena níže.</span><span class="sxs-lookup"><span data-stu-id="b2391-107">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="b2391-108">Doporučujeme zákazníkům přesunout nové předplatné před uplynutím ročního koncového data předplatného, aby se předešlo výpadkům služby pro zákazníky.</span><span class="sxs-lookup"><span data-stu-id="b2391-108">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="b2391-109">Pokud používáte rozhraní API (buď CREST nebo Partnerská centra), můžete najít odběry, které vyhodnocuje datum ukončení předplatného spolu s vlastností automaticky obnovit = false.</span><span class="sxs-lookup"><span data-stu-id="b2391-109">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="b2391-110">V případě 1. ledna 2019 budou příslušné odběry nastaveny na automatické obnovení = false.</span><span class="sxs-lookup"><span data-stu-id="b2391-110">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="b2391-111">Zákazníky můžete kdykoli přesunout do nového plánu.</span><span class="sxs-lookup"><span data-stu-id="b2391-111">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="b2391-112">Nabídky Dynamics 365 jsou vyřazeny</span><span class="sxs-lookup"><span data-stu-id="b2391-112">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="b2391-113">Dynamics 365 pro Sales Enterprise Edition CRMOL Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="b2391-113">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="b2391-114">Dynamics 365 pro Sales Enterprise Edition CRMOL Basic (kvalifikovaná nabídka) pro Akademický sbor</span><span class="sxs-lookup"><span data-stu-id="b2391-114">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="b2391-115">Dynamics 365 pro Sales Enterprise Edition CRMOL Basic (kvalifikovaná nabídka) pro studenty</span><span class="sxs-lookup"><span data-stu-id="b2391-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="b2391-116">Dynamics 365 pro Sales Enterprise Edition (ceny pro státní správu) CRMOL Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="b2391-116">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="b2391-117">Dynamics 365 pro Sales Enterprise Edition od SA pro CRM Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="b2391-117">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="b2391-118">Dynamics 365 for Sales Enterprise Edition od SA pro CRM Basic (kvalifikovaná nabídka) pro Akademický sbor</span><span class="sxs-lookup"><span data-stu-id="b2391-118">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="b2391-119">Dynamics 365 pro Sales Enterprise Edition od SA pro CRM Basic (kvalifikovaná nabídka) pro studenty</span><span class="sxs-lookup"><span data-stu-id="b2391-119">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="b2391-120">Dynamics 365 pro Sales Enterprise Edition (ceny pro státní správu) od SA pro CRM Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="b2391-120">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="b2391-121">Dynamics 365 for Sales edice Enterprise Add-On for CRM Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="b2391-121">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="b2391-122">Dynamics 365 for Sales edice Enterprise Add-On for CRM Basic (kvalifikovaná nabídka) pro učitelské sbory</span><span class="sxs-lookup"><span data-stu-id="b2391-122">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="b2391-123">Dynamics 365 for Sales edice Enterprise Add-On for CRM Basic (kvalifikovaná nabídka) pro studenty</span><span class="sxs-lookup"><span data-stu-id="b2391-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="b2391-124">Dynamics 365 for Sales edice Enterprise (Ceny pro státní správu) Add-On pro CRM Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="b2391-124">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="b2391-125">Plán Dynamics 365 Customer Engagement edice Enterprise CRMOL Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="b2391-125">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="b2391-126">Plán Dynamics 365 Customer Engagement edice Enterprise (ceny pro státní správu) CRMOL Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="b2391-126">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="b2391-127">Plán Dynamics 365 Customer Engagement edice Enterprise CRMOL Basic (kvalifikovaná nabídka) pro studenty</span><span class="sxs-lookup"><span data-stu-id="b2391-127">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="b2391-128">Plán Dynamics 365 Customer Engagement edice Enterprise CRMOL Basic (kvalifikovaná nabídka) pro učitelské sbory</span><span class="sxs-lookup"><span data-stu-id="b2391-128">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="b2391-129">Plán Dynamics 365 Customer Engagement edice Enterprise od SA pro CRM Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="b2391-129">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="b2391-130">Plán Dynamics 365 Customer Engagement edice Enterprise (ceny pro státní správu) od SA for CRM Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="b2391-130">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="b2391-131">Dynamics 365 Customer Engagement Plan edice Enterprise From SA for CRM Basic (Qualified Offer) for Students</span><span class="sxs-lookup"><span data-stu-id="b2391-131">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="b2391-132">Plán Dynamics 365 Customer Engagement edice Enterprise od SA pro CRM Basic (kvalifikovaná nabídka) pro učitelské sbory</span><span class="sxs-lookup"><span data-stu-id="b2391-132">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="b2391-133">Dynamics 365 Customer Engagement Plan edice Enterprise Add-On for CRM Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="b2391-133">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="b2391-134">Plán Dynamics 365 Customer Engagement edice Enterprise (ceny pro státní správu) Add-On CRM Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="b2391-134">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="b2391-135">Dynamics 365 Customer Engagement Plan edice Enterprise Add-On for CRM Basic (kvalifikovaná nabídka) pro studenty</span><span class="sxs-lookup"><span data-stu-id="b2391-135">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="b2391-136">Dynamics 365 Customer Engagement Plan edice Enterprise Add-On for CRM Basic (kvalifikovaná nabídka) pro učitelské sbory</span><span class="sxs-lookup"><span data-stu-id="b2391-136">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="b2391-137">Plán Dynamics 365 for Sales/ Customer Engagement z náhradních plánů Basic (kvalifikované nabídky)</span><span class="sxs-lookup"><span data-stu-id="b2391-137">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="b2391-138">**Vyřazené nabídky**</span><span class="sxs-lookup"><span data-stu-id="b2391-138">**Retired offers**</span></span>   

- <span data-ttu-id="b2391-139">Dynamics 365 for Sales od CRM Basic nebo CRMOL Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="b2391-139">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="b2391-140">Plán Dynamics 365 Customer Engagement od CRM Basic nebo CRMOL Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="b2391-140">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="b2391-141">**Možnosti nahrazení**</span><span class="sxs-lookup"><span data-stu-id="b2391-141">**Replacement options**</span></span>
- <span data-ttu-id="b2391-142">Dynamics 365 pro prodejní specialisty (nové)</span><span class="sxs-lookup"><span data-stu-id="b2391-142">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="b2391-143">Dynamics 365 pro prodejní specialisty (nové)</span><span class="sxs-lookup"><span data-stu-id="b2391-143">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="b2391-144">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="b2391-144">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="b2391-145">Plán Customer Engagement pro Dynamics 365 nebo</span><span class="sxs-lookup"><span data-stu-id="b2391-145">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="b2391-146">Členové týmu Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="b2391-146">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="b2391-147">Přechod zákazníků na nové plány produktů</span><span class="sxs-lookup"><span data-stu-id="b2391-147">Transition customers to new product plans</span></span>

<span data-ttu-id="b2391-148">Přesun zákazníků z vyřazených SKU do novějšího vyžaduje následující kroky v tomto pořadí:</span><span class="sxs-lookup"><span data-stu-id="b2391-148">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="b2391-149">Koupit nové předplatné</span><span class="sxs-lookup"><span data-stu-id="b2391-149">Purchase the new subscription</span></span>
- <span data-ttu-id="b2391-150">Změna přiřazení licencí k aktuálním uživatelům</span><span class="sxs-lookup"><span data-stu-id="b2391-150">Reassign current user licenses</span></span>
- <span data-ttu-id="b2391-151">Zrušit staré předplatné</span><span class="sxs-lookup"><span data-stu-id="b2391-151">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="b2391-152">Zakupte si nový plán pro zákazníka.</span><span class="sxs-lookup"><span data-stu-id="b2391-152">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="b2391-153">V levém navigačním panelu vyberte **zákazníky** a pak vyberte zákazníka, kterého chcete přesunout do nového předplatného.</span><span class="sxs-lookup"><span data-stu-id="b2391-153">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="b2391-154">Vyberte **přidat odběr**.</span><span class="sxs-lookup"><span data-stu-id="b2391-154">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="b2391-155">Vyberte předplatné, které chcete z katalogu koupit (v tomto případě jednu z výše uvedených možností), zadejte počet licencí a pak vyberte **Odeslat**.</span><span class="sxs-lookup"><span data-stu-id="b2391-155">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="b2391-156">Zákazník teď bude mít původní předplatné i nový.</span><span class="sxs-lookup"><span data-stu-id="b2391-156">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="b2391-157">Vaším dalším krokem je změna přiřazení licencí uživatelům zákazníka.</span><span class="sxs-lookup"><span data-stu-id="b2391-157">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="b2391-158">V levém navigačním panelu vyberte **zákazníky** a pak vyberte zákazníka, kterého přesouváte.</span><span class="sxs-lookup"><span data-stu-id="b2391-158">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="b2391-159">Vyberte **Uživatelé a licence**.</span><span class="sxs-lookup"><span data-stu-id="b2391-159">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="b2391-160">Pokud chcete uživateli přiřadit licenci, vyberte uživatele a pak vyberte **spravovat licence**.</span><span class="sxs-lookup"><span data-stu-id="b2391-160">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="b2391-161">Na stránce **spravovat licence** zrušte zaškrtnutí políčka Dynamics 365 pro možnost plán služby Sales/zákazník Engagement z licence Basic (kvalifikovaná nabídka) a vyberte nový plán služby pro předplatné, na které se bude zákazník pohybovat.</span><span class="sxs-lookup"><span data-stu-id="b2391-161">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="b2391-162">Vyberte **Odeslat**.</span><span class="sxs-lookup"><span data-stu-id="b2391-162">Select **Submit**.</span></span> <span data-ttu-id="b2391-163">To budete dělat pro každého uživatele, který potřebuje novou licenci.</span><span class="sxs-lookup"><span data-stu-id="b2391-163">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="b2391-164">Po přesunu licencí do nového předplatného můžete staré předplatné zrušit.</span><span class="sxs-lookup"><span data-stu-id="b2391-164">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="b2391-165">V **levém** navigačním panelu vyberte Zákazníci a pak vyberte zákazníka, který přesouváte.</span><span class="sxs-lookup"><span data-stu-id="b2391-165">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="b2391-166">Na stránce podrobností o předplatném nastavte staré předplatné na **Pozastaveno** a vyberte **Odeslat.**</span><span class="sxs-lookup"><span data-stu-id="b2391-166">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="b2391-167">Původní předplatné je teď pozastavené a nové předplatné je aktivní.</span><span class="sxs-lookup"><span data-stu-id="b2391-167">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="b2391-168">Pozastavené předplatné bude po 120 dnech automaticky zrušeno.</span><span class="sxs-lookup"><span data-stu-id="b2391-168">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="b2391-169">Za staré předplatné se zákazníkovi ne účtut žádné další poplatky.</span><span class="sxs-lookup"><span data-stu-id="b2391-169">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



