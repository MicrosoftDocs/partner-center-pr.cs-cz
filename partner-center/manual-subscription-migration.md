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
ms.openlocfilehash: 8575d87ab3c4c7970135a87b7ef7564c4fe06232
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/17/2020
ms.locfileid: "92527031"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="f50a7-103">Migrace Dynamics 365 a plánu Customer Engagement z úrovně Basic na novější verze (u kvalifikovaných nabídek)</span><span class="sxs-lookup"><span data-stu-id="f50a7-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="f50a7-104">**Platí pro**</span><span class="sxs-lookup"><span data-stu-id="f50a7-104">**Applies to**</span></span>

-  <span data-ttu-id="f50a7-105">Partnerské centrum</span><span class="sxs-lookup"><span data-stu-id="f50a7-105">Partner Center</span></span>

<span data-ttu-id="f50a7-106">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="f50a7-106">**Appropriate roles**</span></span>
-   <span data-ttu-id="f50a7-107">Globální správce</span><span class="sxs-lookup"><span data-stu-id="f50a7-107">Global admin</span></span>
-   <span data-ttu-id="f50a7-108">Správce uživatelů</span><span class="sxs-lookup"><span data-stu-id="f50a7-108">User admin</span></span>
-   <span data-ttu-id="f50a7-109">Agent správce</span><span class="sxs-lookup"><span data-stu-id="f50a7-109">Admin agent</span></span>
-   <span data-ttu-id="f50a7-110">Agent prodeje</span><span class="sxs-lookup"><span data-stu-id="f50a7-110">Sales agent</span></span>

<span data-ttu-id="f50a7-111">Od 1. ledna 2019 zákazníci s Dynamics 365 for Sales/Customing Engagement ze základních (kvalifikovaných nabídek) odběry už nemůžou obnovit tyto starší nabídky. existující odběry se po vypršení platnosti automaticky neobnoví.</span><span class="sxs-lookup"><span data-stu-id="f50a7-111">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="f50a7-112">Na stránce s podrobnostmi o předplatném se stav předplatného změní na "vyprší dne [Date]" z "automatické obnovování v [datum]".</span><span class="sxs-lookup"><span data-stu-id="f50a7-112">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="f50a7-113">Chcete-li zajistit kontinuitu pro zákazníky, měli byste je přecházet s vypršením platnosti předplatných na podporovanou možnost, která je uvedena níže.</span><span class="sxs-lookup"><span data-stu-id="f50a7-113">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="f50a7-114">Doporučujeme zákazníkům přesunout nové předplatné před uplynutím ročního koncového data předplatného, aby se předešlo výpadkům služby pro zákazníky.</span><span class="sxs-lookup"><span data-stu-id="f50a7-114">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="f50a7-115">Pokud používáte rozhraní API (buď CREST nebo Partnerská centra), můžete najít odběry, které vyhodnocuje datum ukončení předplatného spolu s vlastností automaticky obnovit = false.</span><span class="sxs-lookup"><span data-stu-id="f50a7-115">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="f50a7-116">V případě 1. ledna 2019 budou předplatná nastavena na hodnotu automaticky obnovit = false.</span><span class="sxs-lookup"><span data-stu-id="f50a7-116">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="f50a7-117">Zákazníky můžete kdykoli přesunout do nového plánu.</span><span class="sxs-lookup"><span data-stu-id="f50a7-117">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="f50a7-118">Nabídky Dynamics 365 jsou vyřazeny</span><span class="sxs-lookup"><span data-stu-id="f50a7-118">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="f50a7-119">Dynamics 365 pro Sales Enterprise Edition CRMOL Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="f50a7-119">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f50a7-120">Dynamics 365 pro Sales Enterprise Edition CRMOL Basic (kvalifikovaná nabídka) pro Akademický sbor</span><span class="sxs-lookup"><span data-stu-id="f50a7-120">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="f50a7-121">Dynamics 365 pro Sales Enterprise Edition CRMOL Basic (kvalifikovaná nabídka) pro studenty</span><span class="sxs-lookup"><span data-stu-id="f50a7-121">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="f50a7-122">Dynamics 365 pro Sales Enterprise Edition (ceny pro státní správu) CRMOL Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="f50a7-122">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f50a7-123">Dynamics 365 pro Sales Enterprise Edition od SA pro CRM Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="f50a7-123">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f50a7-124">Dynamics 365 for Sales Enterprise Edition od SA pro CRM Basic (kvalifikovaná nabídka) pro Akademický sbor</span><span class="sxs-lookup"><span data-stu-id="f50a7-124">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="f50a7-125">Dynamics 365 pro Sales Enterprise Edition od SA pro CRM Basic (kvalifikovaná nabídka) pro studenty</span><span class="sxs-lookup"><span data-stu-id="f50a7-125">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="f50a7-126">Dynamics 365 pro Sales Enterprise Edition (ceny pro státní správu) od SA pro CRM Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="f50a7-126">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f50a7-127">Dynamics 365 pro Sales Enterprise Edition Add-On pro CRM Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="f50a7-127">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f50a7-128">Dynamics 365 pro prodej Enterprise Edition Add-On pro CRM Basic (kvalifikovaná nabídka) pro Akademický sbor</span><span class="sxs-lookup"><span data-stu-id="f50a7-128">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="f50a7-129">Dynamics 365 pro prodej Enterprise Edition Add-On pro CRM Basic (kvalifikovaná nabídka) pro studenty</span><span class="sxs-lookup"><span data-stu-id="f50a7-129">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="f50a7-130">Dynamics 365 pro Sales Enterprise Edition (ceny pro státní správu) Add-On pro CRM Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="f50a7-130">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f50a7-131">Dynamics 365 Customer Engagement plán Enterprise Edition CRMOL úrovně Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="f50a7-131">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f50a7-132">Dynamics 365 Customer Engagement Enterprise Edition (ceny pro státní správu) CRMOL Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="f50a7-132">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f50a7-133">Dynamics 365 Customer Engagement plán Enterprise Edition CRMOL Basic (kvalifikovaná nabídka) pro studenty</span><span class="sxs-lookup"><span data-stu-id="f50a7-133">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="f50a7-134">Dynamics 365 Customer Engagement plán Enterprise Edition CRMOL Basic (kvalifikovaná nabídka) pro Akademický sbor</span><span class="sxs-lookup"><span data-stu-id="f50a7-134">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="f50a7-135">Dynamics 365 Customer Engagement plán Enterprise Edition od SA pro CRM Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="f50a7-135">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f50a7-136">Dynamics 365 Customer Engagement plán Enterprise Edition (ceny pro státní správu) od SA pro CRM Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="f50a7-136">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f50a7-137">Dynamics 365 Customer Engagement plán Enterprise Edition od SA pro CRM Basic (kvalifikovaná nabídka) pro studenty</span><span class="sxs-lookup"><span data-stu-id="f50a7-137">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="f50a7-138">Dynamics 365 Customer Engagement plán Enterprise Edition od společnosti SA pro aplikaci CRM Basic (kvalifikovaná nabídka) pro Akademický sbor</span><span class="sxs-lookup"><span data-stu-id="f50a7-138">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="f50a7-139">Dynamics 365 Customer Engagement – Enterprise Edition Add-On pro CRM Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="f50a7-139">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f50a7-140">Dynamics 365 Customer Engagement plán Enterprise Edition (ceny pro státní správu) Add-On pro CRM Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="f50a7-140">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f50a7-141">Dynamics 365 Customer Engagement pro zákazníky – edice Enterprise Add-On pro CRM Basic (kvalifikovaná nabídka) pro studenty</span><span class="sxs-lookup"><span data-stu-id="f50a7-141">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="f50a7-142">Dynamics 365 Customer Engagement – Enterprise Edition Add-On pro CRM Basic (kvalifikovaná nabídka) pro Akademický sbor</span><span class="sxs-lookup"><span data-stu-id="f50a7-142">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="f50a7-143">Dynamics 365 pro plánování služby Sales/Customer Engagement ze základních (kvalifikovaných nabídek) plánů nahrazení</span><span class="sxs-lookup"><span data-stu-id="f50a7-143">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="f50a7-144">**Vyřazené nabídky**</span><span class="sxs-lookup"><span data-stu-id="f50a7-144">**Retired offers**</span></span>   

- <span data-ttu-id="f50a7-145">Dynamics 365 pro prodej z aplikace CRM Basic nebo CRMOL Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="f50a7-145">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f50a7-146">Plán Customer Engagement pro Dynamics 365 od CRM Basic nebo CRMOL Basic (kvalifikovaná nabídka)</span><span class="sxs-lookup"><span data-stu-id="f50a7-146">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="f50a7-147">**Možnosti nahrazení**</span><span class="sxs-lookup"><span data-stu-id="f50a7-147">**Replacement options**</span></span>
- <span data-ttu-id="f50a7-148">Dynamics 365 pro prodejní specialisty (nové)</span><span class="sxs-lookup"><span data-stu-id="f50a7-148">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="f50a7-149">Dynamics 365 pro prodejní specialisty (nové)</span><span class="sxs-lookup"><span data-stu-id="f50a7-149">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="f50a7-150">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="f50a7-150">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="f50a7-151">Plán Customer Engagement pro Dynamics 365 nebo</span><span class="sxs-lookup"><span data-stu-id="f50a7-151">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="f50a7-152">Členové týmu Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="f50a7-152">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="f50a7-153">Přechod zákazníků na nové plány produktů</span><span class="sxs-lookup"><span data-stu-id="f50a7-153">Transition customers to new product plans</span></span>

<span data-ttu-id="f50a7-154">Přesun zákazníků z vyřazených SKU do novějšího vyžaduje následující kroky v tomto pořadí:</span><span class="sxs-lookup"><span data-stu-id="f50a7-154">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="f50a7-155">Koupit nové předplatné</span><span class="sxs-lookup"><span data-stu-id="f50a7-155">Purchase the new subscription</span></span>
- <span data-ttu-id="f50a7-156">Změna přiřazení licencí k aktuálním uživatelům</span><span class="sxs-lookup"><span data-stu-id="f50a7-156">Reassign current user licenses</span></span>
- <span data-ttu-id="f50a7-157">Zrušit staré předplatné</span><span class="sxs-lookup"><span data-stu-id="f50a7-157">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="f50a7-158">Zakupte si nový plán pro zákazníka.</span><span class="sxs-lookup"><span data-stu-id="f50a7-158">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="f50a7-159">V levém navigačním panelu vyberte **zákazníky** a pak vyberte zákazníka, kterého chcete přesunout do nového předplatného.</span><span class="sxs-lookup"><span data-stu-id="f50a7-159">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="f50a7-160">Vyberte **přidat odběr** .</span><span class="sxs-lookup"><span data-stu-id="f50a7-160">Select **Add Subscription** .</span></span>
3. <span data-ttu-id="f50a7-161">Vyberte předplatné, které chcete z katalogu koupit (v tomto případě jednu z výše uvedených možností), zadejte počet licencí a pak vyberte **Odeslat** .</span><span class="sxs-lookup"><span data-stu-id="f50a7-161">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit** .</span></span> 

<span data-ttu-id="f50a7-162">Zákazník teď bude mít původní předplatné i nový.</span><span class="sxs-lookup"><span data-stu-id="f50a7-162">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="f50a7-163">Vaším dalším krokem je změna přiřazení licencí uživatelům zákazníka.</span><span class="sxs-lookup"><span data-stu-id="f50a7-163">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="f50a7-164">V levém navigačním panelu vyberte **zákazníky** a pak vyberte zákazníka, kterého přesouváte.</span><span class="sxs-lookup"><span data-stu-id="f50a7-164">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="f50a7-165">Vyberte **Uživatelé a licence** .</span><span class="sxs-lookup"><span data-stu-id="f50a7-165">Select **Users and licenses** .</span></span>
3. <span data-ttu-id="f50a7-166">Pokud chcete uživateli přiřadit licenci, vyberte uživatele a pak vyberte **spravovat licence** .</span><span class="sxs-lookup"><span data-stu-id="f50a7-166">To reassign a license to a user, select the user and then select **Manage licenses** .</span></span> 
4. <span data-ttu-id="f50a7-167">Na stránce **spravovat licence** zrušte zaškrtnutí políčka Dynamics 365 pro možnost plán služby Sales/zákazník Engagement z licence Basic (kvalifikovaná nabídka) a vyberte nový plán služby pro předplatné, na které se bude zákazník pohybovat.</span><span class="sxs-lookup"><span data-stu-id="f50a7-167">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="f50a7-168">Vyberte **Odeslat** .</span><span class="sxs-lookup"><span data-stu-id="f50a7-168">Select **Submit** .</span></span> <span data-ttu-id="f50a7-169">To provedete pro každého uživatele, který bude tuto novou licenci potřebovat.</span><span class="sxs-lookup"><span data-stu-id="f50a7-169">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="f50a7-170">Po přesunutí licencí do nového předplatného můžete zrušit původní předplatné.</span><span class="sxs-lookup"><span data-stu-id="f50a7-170">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="f50a7-171">V levém navigačním panelu vyberte **zákazníky** a pak vyberte zákazníka, kterého přesouváte.</span><span class="sxs-lookup"><span data-stu-id="f50a7-171">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="f50a7-172">Na stránce s podrobnostmi předplatného nastavte původní předplatné na **pozastaveno** a vyberte **Odeslat** .</span><span class="sxs-lookup"><span data-stu-id="f50a7-172">On the subscription detail page, set the old subscription to **Suspended** and select **Submit** .</span></span>

<span data-ttu-id="f50a7-173">Staré předplatné je teď pozastavené a nové předplatné je aktivní.</span><span class="sxs-lookup"><span data-stu-id="f50a7-173">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="f50a7-174">Pozastavený odběr bude po 120 dnech automaticky zřízen.</span><span class="sxs-lookup"><span data-stu-id="f50a7-174">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="f50a7-175">Pro staré předplatné nepřijde váš zákazník žádné další poplatky.</span><span class="sxs-lookup"><span data-stu-id="f50a7-175">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



