---
title: Migrace Dynamics 365 Business Edition
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zjistěte, jak migrovat kvalifikované nabídky Dynamics 365 Business Edition na novější verze před vypršením jejich platnosti.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8232ab165ea68ebefdfbb30f3ac52c907e1b7278
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151521"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="93471-103">Migrace nabídek Dynamics 365 Business Edition na novější verze</span><span class="sxs-lookup"><span data-stu-id="93471-103">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span>

<span data-ttu-id="93471-104">**Odpovídající role:** Globální správce | Správce správy uživatelů | Agent správy | Agent prodeje</span><span class="sxs-lookup"><span data-stu-id="93471-104">**Appropriate roles**: Global admin | User management admin | Admin agent | Sales agent</span></span>

<span data-ttu-id="93471-105">Od 1. ledna 2019 se zákazníci s předplatným Dynamics 365 Business Edition už nebudou moci v těchto starších verzích nabídek prodlužovat. stávající předplatná se po vypršení jejich platnosti automaticky neobnoví.</span><span class="sxs-lookup"><span data-stu-id="93471-105">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="93471-106">Na stránce s podrobnostmi o předplatném se stav předplatného změní na Platnost vyprší [datum]" z "Automatické prodloužení platnosti k [datum]".</span><span class="sxs-lookup"><span data-stu-id="93471-106">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="93471-107">Pokud chcete zajistit kontinuitu pro zákazníky, měli byste uživatele s předplatným s vypršenou platnosti přejít na podporovanou možnost uvedenou níže.</span><span class="sxs-lookup"><span data-stu-id="93471-107">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="93471-108">Doporučujeme přestěhovat zákazníky na nová předplatná před ročním datem ukončení předplatného, abyste se vyhnuli výpadkům služeb pro zákazníky.</span><span class="sxs-lookup"><span data-stu-id="93471-108">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="93471-109">Pokud používáte rozhraní API (CREST nebo Partnerské centrum), můžete zjistit vypršení platnosti odběrů vyhodnocením koncového data odběru spolu s vlastností auto renew = False.</span><span class="sxs-lookup"><span data-stu-id="93471-109">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="93471-110">1. ledna 2019 budou 1. ledna 2019 sporná předplatná nastavená na auto renew=False.</span><span class="sxs-lookup"><span data-stu-id="93471-110">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="93471-111">Zákazníky můžete kdykoli přesunout do nového plánu.</span><span class="sxs-lookup"><span data-stu-id="93471-111">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="93471-112">Vyřazení edicí Dynamics 365 Business Edition</span><span class="sxs-lookup"><span data-stu-id="93471-112">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="93471-113">Dynamics 365 for Finance and Operations, edice Business</span><span class="sxs-lookup"><span data-stu-id="93471-113">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="93471-114">Dynamics 365 for Team Members, edice Business</span><span class="sxs-lookup"><span data-stu-id="93471-114">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="93471-115">Dynamics Business Central – nové nabídky Dynamics 365 Business Edition</span><span class="sxs-lookup"><span data-stu-id="93471-115">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="93471-116">S novými nabídkami Dynamics Business Central mohou vaši zákazníci propojit své finanční prostředky, prodej, službu a provoz a zjednodušit tak obchodní procesy, zlepšit interakce se zákazníky a lépe se rozhodovat.</span><span class="sxs-lookup"><span data-stu-id="93471-116">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="93471-117">Dynamics 365 Business Central je cloudová a dostupná pouze prostřednictvím partnerů Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="93471-117">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="93471-118">Zákazníci Dynamics 365 Business Edition mají nárok na zvýhodněné převodní ceny pro nové nabídky Business Central do 30. června 2020.</span><span class="sxs-lookup"><span data-stu-id="93471-118">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="93471-119">Převod zákazníků na nové produktové plány</span><span class="sxs-lookup"><span data-stu-id="93471-119">Transition customers to new product plans</span></span>

 <span data-ttu-id="93471-120">Přesun zákazníků z vyřazených SKU na novější vyžaduje následující kroky v tomto pořadí:</span><span class="sxs-lookup"><span data-stu-id="93471-120">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="93471-121">Zakoupení nového předplatného</span><span class="sxs-lookup"><span data-stu-id="93471-121">Purchase the new subscription</span></span>
- <span data-ttu-id="93471-122">Opětovné přiřazení aktuálních uživatelských licencí</span><span class="sxs-lookup"><span data-stu-id="93471-122">Reassign current user licenses</span></span>
- <span data-ttu-id="93471-123">Zrušení starého předplatného</span><span class="sxs-lookup"><span data-stu-id="93471-123">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="93471-124">Nákup nového plánu pro zákazníka</span><span class="sxs-lookup"><span data-stu-id="93471-124">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="93471-125">V **levém** navigačním panelu vyberte Zákazníci a pak vyberte zákazníka, kterého chcete přesunout do nového předplatného.</span><span class="sxs-lookup"><span data-stu-id="93471-125">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="93471-126">Vyberte **Přidat předplatné.**</span><span class="sxs-lookup"><span data-stu-id="93471-126">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="93471-127">Vyberte předplatné, které chcete zakoupit z katalogu (v tomto případě jednu z výše uvedených možností), zadejte počet licencí a pak vyberte **Odeslat.**</span><span class="sxs-lookup"><span data-stu-id="93471-127">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="93471-128">Váš zákazník teď bude mít staré i nové předplatné.</span><span class="sxs-lookup"><span data-stu-id="93471-128">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="93471-129">Dalším krokem je opětovné přiřazení licencí uživatelům zákazníka.</span><span class="sxs-lookup"><span data-stu-id="93471-129">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="93471-130">V **levém** navigačním panelu vyberte Zákazníci a pak vyberte zákazníka, který přesouváte.</span><span class="sxs-lookup"><span data-stu-id="93471-130">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="93471-131">Vyberte **Uživatelé a licence.**</span><span class="sxs-lookup"><span data-stu-id="93471-131">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="93471-132">Pokud chcete přiřadit licenci uživateli znovu, vyberte uživatele a pak vyberte **Spravovat licence.**</span><span class="sxs-lookup"><span data-stu-id="93471-132">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="93471-133">Na  stránce Spravovat licence zrušte zaškrtnutí políčka Dynamics 365 for Sales/ Customer Engagement Plan (Plán Dynamics 365 for Customer Engagement z licence basic (kvalifikovaná nabídka) a vyberte nový plán služby pro předplatné, do které zákazník přechází.</span><span class="sxs-lookup"><span data-stu-id="93471-133">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="93471-134">Vyberte **Odeslat**.</span><span class="sxs-lookup"><span data-stu-id="93471-134">Select **Submit**.</span></span> <span data-ttu-id="93471-135">To budete dělat pro každého uživatele, který potřebuje novou licenci.</span><span class="sxs-lookup"><span data-stu-id="93471-135">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="93471-136">Po přesunu licencí do nového předplatného můžete staré předplatné zrušit.</span><span class="sxs-lookup"><span data-stu-id="93471-136">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="93471-137">V **levém** navigačním panelu vyberte Zákazníci a pak vyberte zákazníka, který přesouváte.</span><span class="sxs-lookup"><span data-stu-id="93471-137">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="93471-138">Na stránce podrobností o předplatném nastavte staré předplatné na **Pozastaveno** a vyberte **Odeslat.**</span><span class="sxs-lookup"><span data-stu-id="93471-138">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="93471-139">Původní předplatné je teď pozastavené a nové předplatné je aktivní.</span><span class="sxs-lookup"><span data-stu-id="93471-139">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="93471-140">Pozastavené předplatné bude po 120 dnech automaticky zrušeno.</span><span class="sxs-lookup"><span data-stu-id="93471-140">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="93471-141">Za staré předplatné se zákazníkovi ne účtut žádné další poplatky.</span><span class="sxs-lookup"><span data-stu-id="93471-141">Your customer will incur no additional costs for the old subscription.</span></span>
