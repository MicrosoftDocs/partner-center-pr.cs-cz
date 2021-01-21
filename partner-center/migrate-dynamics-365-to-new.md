---
title: Migrace verze Dynamics 365 Business Edition
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Přečtěte si, jak migrovat kvalifikované nabídky Dynamics 365 Business Edition do novějších verzí, než vyprší jejich platnost.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d441d121c28c2762d1f1c71d6f6a1e81d089f99c
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/17/2020
ms.locfileid: "92527030"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="efd78-103">Migrace nabídek Dynamics 365 Business Edition na novější verze</span><span class="sxs-lookup"><span data-stu-id="efd78-103">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span>

<span data-ttu-id="efd78-104">**Platí pro**</span><span class="sxs-lookup"><span data-stu-id="efd78-104">**Applies to**</span></span>

- <span data-ttu-id="efd78-105">Partnerské centrum</span><span class="sxs-lookup"><span data-stu-id="efd78-105">Partner Center</span></span>

<span data-ttu-id="efd78-106">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="efd78-106">**Appropriate roles**</span></span>
- <span data-ttu-id="efd78-107">Globální správce</span><span class="sxs-lookup"><span data-stu-id="efd78-107">Global admin</span></span>
- <span data-ttu-id="efd78-108">Správce uživatelů</span><span class="sxs-lookup"><span data-stu-id="efd78-108">User admin</span></span>
- <span data-ttu-id="efd78-109">Agent správce</span><span class="sxs-lookup"><span data-stu-id="efd78-109">Admin agent</span></span>
- <span data-ttu-id="efd78-110">Agent prodeje</span><span class="sxs-lookup"><span data-stu-id="efd78-110">Sales agent</span></span>

<span data-ttu-id="efd78-111">Od 1. ledna 2019 se zákazníci s předplatným Dynamics 365 Business Edition už nemůžou prodloužit na tyto starší nabídky. existující odběry se po vypršení platnosti automaticky neobnoví.</span><span class="sxs-lookup"><span data-stu-id="efd78-111">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="efd78-112">Na stránce s podrobnostmi o předplatném se stav předplatného změní na "vyprší dne [Date]" z "automatické obnovování v [datum]".</span><span class="sxs-lookup"><span data-stu-id="efd78-112">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="efd78-113">Chcete-li zajistit kontinuitu pro zákazníky, měli byste je přecházet s vypršením platnosti předplatných na podporovanou možnost, která je uvedena níže.</span><span class="sxs-lookup"><span data-stu-id="efd78-113">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="efd78-114">Doporučujeme zákazníkům přesunout nové předplatné před uplynutím ročního koncového data předplatného, aby se předešlo výpadkům služby pro zákazníky.</span><span class="sxs-lookup"><span data-stu-id="efd78-114">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="efd78-115">Pokud používáte rozhraní API (buď CREST nebo Partnerská centra), můžete najít odběry, které vyhodnocuje datum ukončení předplatného spolu s vlastností automaticky obnovit = false.</span><span class="sxs-lookup"><span data-stu-id="efd78-115">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="efd78-116">V případě 1. ledna 2019 budou předplatná nastavena na hodnotu automaticky obnovit = false.</span><span class="sxs-lookup"><span data-stu-id="efd78-116">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="efd78-117">Zákazníky můžete kdykoli přesunout do nového plánu.</span><span class="sxs-lookup"><span data-stu-id="efd78-117">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="efd78-118">Vyřazení obchodních edicí Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="efd78-118">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="efd78-119">Dynamics 365 pro finance a provoz, Business Edition</span><span class="sxs-lookup"><span data-stu-id="efd78-119">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="efd78-120">Dynamics 365 pro členy týmu, verze Business Edition</span><span class="sxs-lookup"><span data-stu-id="efd78-120">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="efd78-121">Dynamics Business Central – nové nabídky pro Dynamics 365 Business Edition</span><span class="sxs-lookup"><span data-stu-id="efd78-121">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="efd78-122">Díky novým nabídkám Dynamics Business Central můžou vaši zákazníci připojit své finanční služby, prodej, služby a operace, aby zjednodušily obchodní procesy, zlepšili interakce zákazníků a lépe rozhodovat.</span><span class="sxs-lookup"><span data-stu-id="efd78-122">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="efd78-123">Dynamics 365 Business Central je cloudová a dostupná jenom prostřednictvím partnerů programu Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="efd78-123">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="efd78-124">Zákazníci Dynamics 365 Business Edition mají nárok na zlevněné přechody na nové nabídky Business Central do 30. června 2020.</span><span class="sxs-lookup"><span data-stu-id="efd78-124">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="efd78-125">Přechod zákazníků na nové plány produktů</span><span class="sxs-lookup"><span data-stu-id="efd78-125">Transition customers to new product plans</span></span>

 <span data-ttu-id="efd78-126">Přesun zákazníků z vyřazených SKU do novějšího vyžaduje následující kroky v tomto pořadí:</span><span class="sxs-lookup"><span data-stu-id="efd78-126">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="efd78-127">Koupit nové předplatné</span><span class="sxs-lookup"><span data-stu-id="efd78-127">Purchase the new subscription</span></span>
- <span data-ttu-id="efd78-128">Změna přiřazení licencí k aktuálním uživatelům</span><span class="sxs-lookup"><span data-stu-id="efd78-128">Reassign current user licenses</span></span>
- <span data-ttu-id="efd78-129">Zrušit staré předplatné</span><span class="sxs-lookup"><span data-stu-id="efd78-129">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="efd78-130">Zakupte si nový plán pro zákazníka.</span><span class="sxs-lookup"><span data-stu-id="efd78-130">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="efd78-131">V levém navigačním panelu vyberte **zákazníky** a pak vyberte zákazníka, kterého chcete přesunout do nového předplatného.</span><span class="sxs-lookup"><span data-stu-id="efd78-131">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="efd78-132">Vyberte **přidat odběr**.</span><span class="sxs-lookup"><span data-stu-id="efd78-132">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="efd78-133">Vyberte předplatné, které chcete z katalogu koupit (v tomto případě jednu z výše uvedených možností), zadejte počet licencí a pak vyberte **Odeslat**.</span><span class="sxs-lookup"><span data-stu-id="efd78-133">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="efd78-134">Zákazník teď bude mít původní předplatné i nový.</span><span class="sxs-lookup"><span data-stu-id="efd78-134">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="efd78-135">Vaším dalším krokem je změna přiřazení licencí uživatelům zákazníka.</span><span class="sxs-lookup"><span data-stu-id="efd78-135">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="efd78-136">V levém navigačním panelu vyberte **zákazníky** a pak vyberte zákazníka, kterého přesouváte.</span><span class="sxs-lookup"><span data-stu-id="efd78-136">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="efd78-137">Vyberte **Uživatelé a licence**.</span><span class="sxs-lookup"><span data-stu-id="efd78-137">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="efd78-138">Pokud chcete uživateli přiřadit licenci, vyberte uživatele a pak vyberte **spravovat licence**.</span><span class="sxs-lookup"><span data-stu-id="efd78-138">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="efd78-139">Na stránce **spravovat licence** zrušte zaškrtnutí políčka Dynamics 365 pro možnost plán služby Sales/zákazník Engagement z licence Basic (kvalifikovaná nabídka) a vyberte nový plán služby pro předplatné, na které se bude zákazník pohybovat.</span><span class="sxs-lookup"><span data-stu-id="efd78-139">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="efd78-140">Vyberte **Odeslat**.</span><span class="sxs-lookup"><span data-stu-id="efd78-140">Select **Submit**.</span></span> <span data-ttu-id="efd78-141">To provedete pro každého uživatele, který bude tuto novou licenci potřebovat.</span><span class="sxs-lookup"><span data-stu-id="efd78-141">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="efd78-142">Po přesunutí licencí do nového předplatného můžete zrušit původní předplatné.</span><span class="sxs-lookup"><span data-stu-id="efd78-142">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="efd78-143">V levém navigačním panelu vyberte **zákazníky** a pak vyberte zákazníka, kterého přesouváte.</span><span class="sxs-lookup"><span data-stu-id="efd78-143">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="efd78-144">Na stránce s podrobnostmi předplatného nastavte původní předplatné na **pozastaveno** a vyberte **Odeslat**.</span><span class="sxs-lookup"><span data-stu-id="efd78-144">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="efd78-145">Staré předplatné je teď pozastavené a nové předplatné je aktivní.</span><span class="sxs-lookup"><span data-stu-id="efd78-145">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="efd78-146">Pozastavený odběr bude po 120 dnech automaticky zřízen.</span><span class="sxs-lookup"><span data-stu-id="efd78-146">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="efd78-147">Pro staré předplatné nepřijde váš zákazník žádné další poplatky.</span><span class="sxs-lookup"><span data-stu-id="efd78-147">Your customer will incur no additional costs for the old subscription.</span></span>
