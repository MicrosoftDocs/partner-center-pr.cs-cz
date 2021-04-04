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
ms.openlocfilehash: 363c97b8c2b62e8d6b62cbe3b2807fb3c0ef3e38
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132736"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="863c7-103">Migrace Dynamics 365 a plánu Customer Engagement z úrovně Basic na novější verze (u kvalifikovaných nabídek)</span><span class="sxs-lookup"><span data-stu-id="863c7-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="863c7-104">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="863c7-104">**Appropriate roles**</span></span>

- <span data-ttu-id="863c7-105">Globální správce</span><span class="sxs-lookup"><span data-stu-id="863c7-105">Global admin</span></span>
- <span data-ttu-id="863c7-106">Správce správy uživatelů</span><span class="sxs-lookup"><span data-stu-id="863c7-106">User management admin</span></span>
- <span data-ttu-id="863c7-107">Agent správce</span><span class="sxs-lookup"><span data-stu-id="863c7-107">Admin agent</span></span>
- <span data-ttu-id="863c7-108">Agent prodeje</span><span class="sxs-lookup"><span data-stu-id="863c7-108">Sales agent</span></span>

<span data-ttu-id="863c7-109">Od 1. ledna 2019 zákazníci s Dynamics 365 for Sales/Customing Engagement ze základních (kvalifikovaných nabídek) odběry už nemůžou obnovit tyto starší nabídky. existující odběry se po vypršení platnosti automaticky neobnoví.</span><span class="sxs-lookup"><span data-stu-id="863c7-109">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="863c7-110">Na stránce s podrobnostmi o předplatném se stav předplatného změní na "vyprší dne [Date]" z "automatické obnovování v [datum]".</span><span class="sxs-lookup"><span data-stu-id="863c7-110">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="863c7-111">Chcete-li zajistit kontinuitu pro zákazníky, měli byste je přecházet s vypršením platnosti předplatných na podporovanou možnost, která je uvedena níže.</span><span class="sxs-lookup"><span data-stu-id="863c7-111">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="863c7-112">Doporučujeme zákazníkům přesunout nové předplatné před uplynutím ročního koncového data předplatného, aby se předešlo výpadkům služby pro zákazníky.</span><span class="sxs-lookup"><span data-stu-id="863c7-112">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="863c7-113">Pokud používáte rozhraní API (buď CREST nebo Partnerská centra), můžete najít odběry, které vyhodnocuje datum ukončení předplatného spolu s vlastností automaticky obnovit = false.</span><span class="sxs-lookup"><span data-stu-id="863c7-113">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="863c7-114">V případě 1. ledna 2019 budou příslušné odběry nastaveny na automatické obnovení = false.</span><span class="sxs-lookup"><span data-stu-id="863c7-114">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="863c7-115">Zákazníky můžete kdykoli přesunout do nového plánu.</span><span class="sxs-lookup"><span data-stu-id="863c7-115">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="863c7-116">Nabídky Dynamics 365 jsou vyřazeny</span><span class="sxs-lookup"><span data-stu-id="863c7-116">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="863c7-117">Dynamics 365 pro Sales Enterprise Edition CRMOL Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="863c7-117">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="863c7-118">Dynamics 365 pro Sales Enterprise Edition CRMOL Basic (kvalifikovaná nabídka) pro Akademický sbor</span><span class="sxs-lookup"><span data-stu-id="863c7-118">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="863c7-119">Dynamics 365 pro Sales Enterprise Edition CRMOL Basic (kvalifikovaná nabídka) pro studenty</span><span class="sxs-lookup"><span data-stu-id="863c7-119">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="863c7-120">Dynamics 365 pro Sales Enterprise Edition (ceny pro státní správu) CRMOL Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="863c7-120">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="863c7-121">Dynamics 365 pro Sales Enterprise Edition od SA pro CRM Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="863c7-121">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="863c7-122">Dynamics 365 for Sales Enterprise Edition od SA pro CRM Basic (kvalifikovaná nabídka) pro Akademický sbor</span><span class="sxs-lookup"><span data-stu-id="863c7-122">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="863c7-123">Dynamics 365 pro Sales Enterprise Edition od SA pro CRM Basic (kvalifikovaná nabídka) pro studenty</span><span class="sxs-lookup"><span data-stu-id="863c7-123">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="863c7-124">Dynamics 365 pro Sales Enterprise Edition (ceny pro státní správu) od SA pro CRM Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="863c7-124">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="863c7-125">Dynamics 365 pro Sales Enterprise Edition Add-On pro CRM Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="863c7-125">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="863c7-126">Dynamics 365 pro prodej Enterprise Edition Add-On pro CRM Basic (kvalifikovaná nabídka) pro Akademický sbor</span><span class="sxs-lookup"><span data-stu-id="863c7-126">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="863c7-127">Dynamics 365 pro prodej Enterprise Edition Add-On pro CRM Basic (kvalifikovaná nabídka) pro studenty</span><span class="sxs-lookup"><span data-stu-id="863c7-127">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="863c7-128">Dynamics 365 pro Sales Enterprise Edition (ceny pro státní správu) Add-On pro CRM Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="863c7-128">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="863c7-129">Dynamics 365 Customer Engagement plán Enterprise Edition CRMOL úrovně Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="863c7-129">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="863c7-130">Dynamics 365 Customer Engagement Enterprise Edition (ceny pro státní správu) CRMOL Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="863c7-130">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="863c7-131">Dynamics 365 Customer Engagement plán Enterprise Edition CRMOL Basic (kvalifikovaná nabídka) pro studenty</span><span class="sxs-lookup"><span data-stu-id="863c7-131">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="863c7-132">Dynamics 365 Customer Engagement plán Enterprise Edition CRMOL Basic (kvalifikovaná nabídka) pro Akademický sbor</span><span class="sxs-lookup"><span data-stu-id="863c7-132">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="863c7-133">Dynamics 365 Customer Engagement plán Enterprise Edition od SA pro CRM Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="863c7-133">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="863c7-134">Dynamics 365 Customer Engagement plán Enterprise Edition (ceny pro státní správu) od SA pro CRM Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="863c7-134">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="863c7-135">Dynamics 365 Customer Engagement plán Enterprise Edition od SA pro CRM Basic (kvalifikovaná nabídka) pro studenty</span><span class="sxs-lookup"><span data-stu-id="863c7-135">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="863c7-136">Dynamics 365 Customer Engagement plán Enterprise Edition od společnosti SA pro aplikaci CRM Basic (kvalifikovaná nabídka) pro Akademický sbor</span><span class="sxs-lookup"><span data-stu-id="863c7-136">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="863c7-137">Dynamics 365 Customer Engagement – Enterprise Edition Add-On pro CRM Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="863c7-137">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="863c7-138">Dynamics 365 Customer Engagement plán Enterprise Edition (ceny pro státní správu) Add-On pro CRM Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="863c7-138">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="863c7-139">Dynamics 365 Customer Engagement pro zákazníky – edice Enterprise Add-On pro CRM Basic (kvalifikovaná nabídka) pro studenty</span><span class="sxs-lookup"><span data-stu-id="863c7-139">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="863c7-140">Dynamics 365 Customer Engagement – Enterprise Edition Add-On pro CRM Basic (kvalifikovaná nabídka) pro Akademický sbor</span><span class="sxs-lookup"><span data-stu-id="863c7-140">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="863c7-141">Dynamics 365 pro plánování služby Sales/Customer Engagement ze základních (kvalifikovaných nabídek) plánů nahrazení</span><span class="sxs-lookup"><span data-stu-id="863c7-141">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="863c7-142">**Vyřazené nabídky**</span><span class="sxs-lookup"><span data-stu-id="863c7-142">**Retired offers**</span></span>   

- <span data-ttu-id="863c7-143">Dynamics 365 pro prodej z aplikace CRM Basic nebo CRMOL Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="863c7-143">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="863c7-144">Plán Customer Engagement pro Dynamics 365 od CRM Basic nebo CRMOL Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="863c7-144">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="863c7-145">**Možnosti nahrazení**</span><span class="sxs-lookup"><span data-stu-id="863c7-145">**Replacement options**</span></span>
- <span data-ttu-id="863c7-146">Dynamics 365 pro prodejní specialisty (nové)</span><span class="sxs-lookup"><span data-stu-id="863c7-146">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="863c7-147">Dynamics 365 pro prodejní specialisty (nové)</span><span class="sxs-lookup"><span data-stu-id="863c7-147">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="863c7-148">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="863c7-148">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="863c7-149">Plán Customer Engagement pro Dynamics 365 nebo</span><span class="sxs-lookup"><span data-stu-id="863c7-149">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="863c7-150">Členové týmu Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="863c7-150">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="863c7-151">Přechod zákazníků na nové plány produktů</span><span class="sxs-lookup"><span data-stu-id="863c7-151">Transition customers to new product plans</span></span>

<span data-ttu-id="863c7-152">Přesun zákazníků z vyřazených SKU do novějšího vyžaduje následující kroky v tomto pořadí:</span><span class="sxs-lookup"><span data-stu-id="863c7-152">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="863c7-153">Koupit nové předplatné</span><span class="sxs-lookup"><span data-stu-id="863c7-153">Purchase the new subscription</span></span>
- <span data-ttu-id="863c7-154">Změna přiřazení licencí k aktuálním uživatelům</span><span class="sxs-lookup"><span data-stu-id="863c7-154">Reassign current user licenses</span></span>
- <span data-ttu-id="863c7-155">Zrušit staré předplatné</span><span class="sxs-lookup"><span data-stu-id="863c7-155">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="863c7-156">Zakupte si nový plán pro zákazníka.</span><span class="sxs-lookup"><span data-stu-id="863c7-156">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="863c7-157">V levém navigačním panelu vyberte **zákazníky** a pak vyberte zákazníka, kterého chcete přesunout do nového předplatného.</span><span class="sxs-lookup"><span data-stu-id="863c7-157">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="863c7-158">Vyberte **přidat odběr**.</span><span class="sxs-lookup"><span data-stu-id="863c7-158">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="863c7-159">Vyberte předplatné, které chcete z katalogu koupit (v tomto případě jednu z výše uvedených možností), zadejte počet licencí a pak vyberte **Odeslat**.</span><span class="sxs-lookup"><span data-stu-id="863c7-159">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="863c7-160">Zákazník teď bude mít původní předplatné i nový.</span><span class="sxs-lookup"><span data-stu-id="863c7-160">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="863c7-161">Vaším dalším krokem je změna přiřazení licencí uživatelům zákazníka.</span><span class="sxs-lookup"><span data-stu-id="863c7-161">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="863c7-162">V levém navigačním panelu vyberte **zákazníky** a pak vyberte zákazníka, kterého přesouváte.</span><span class="sxs-lookup"><span data-stu-id="863c7-162">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="863c7-163">Vyberte **Uživatelé a licence**.</span><span class="sxs-lookup"><span data-stu-id="863c7-163">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="863c7-164">Pokud chcete uživateli přiřadit licenci, vyberte uživatele a pak vyberte **spravovat licence**.</span><span class="sxs-lookup"><span data-stu-id="863c7-164">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="863c7-165">Na stránce **spravovat licence** zrušte zaškrtnutí políčka Dynamics 365 pro možnost plán služby Sales/zákazník Engagement z licence Basic (kvalifikovaná nabídka) a vyberte nový plán služby pro předplatné, na které se bude zákazník pohybovat.</span><span class="sxs-lookup"><span data-stu-id="863c7-165">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="863c7-166">Vyberte **Odeslat**.</span><span class="sxs-lookup"><span data-stu-id="863c7-166">Select **Submit**.</span></span> <span data-ttu-id="863c7-167">To provedete pro každého uživatele, který bude tuto novou licenci potřebovat.</span><span class="sxs-lookup"><span data-stu-id="863c7-167">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="863c7-168">Po přesunutí licencí do nového předplatného můžete zrušit původní předplatné.</span><span class="sxs-lookup"><span data-stu-id="863c7-168">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="863c7-169">V levém navigačním panelu vyberte **zákazníky** a pak vyberte zákazníka, kterého přesouváte.</span><span class="sxs-lookup"><span data-stu-id="863c7-169">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="863c7-170">Na stránce s podrobnostmi předplatného nastavte původní předplatné na **pozastaveno** a vyberte **Odeslat**.</span><span class="sxs-lookup"><span data-stu-id="863c7-170">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="863c7-171">Staré předplatné je teď pozastavené a nové předplatné je aktivní.</span><span class="sxs-lookup"><span data-stu-id="863c7-171">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="863c7-172">Pozastavený odběr bude po 120 dnech automaticky zřízen.</span><span class="sxs-lookup"><span data-stu-id="863c7-172">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="863c7-173">Pro staré předplatné nepřijde váš zákazník žádné další poplatky.</span><span class="sxs-lookup"><span data-stu-id="863c7-173">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



