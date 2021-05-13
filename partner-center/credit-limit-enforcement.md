---
title: Vynucení limitu kreditu
ms.topic: how-to
ms.date: 05/11/2021
description: Přečtěte si o limitu kreditu a o tom, jak se počítá. Zahrnuje nejčastější dotazy.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: cf0d3c38b301c363a4a990db5258cf2a3f30d487
ms.sourcegitcommit: dc9438475ccc6298bec6a698bf5fc9bd5cf2aa81
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/12/2021
ms.locfileid: "109819377"
---
# <a name="credit-limit-enforcement-cle"></a><span data-ttu-id="77732-104">Vynucení limitu kreditu (CLE)</span><span class="sxs-lookup"><span data-stu-id="77732-104">Credit limit enforcement (CLE)</span></span>

<span data-ttu-id="77732-105">**Odpovídající role**</span><span class="sxs-lookup"><span data-stu-id="77732-105">**Appropriate roles**</span></span>

- <span data-ttu-id="77732-106">Správce fakturace</span><span class="sxs-lookup"><span data-stu-id="77732-106">Billing admin</span></span>

## <a name="your-credit-limit-and-how-it-works"></a><span data-ttu-id="77732-107">Váš limit kreditu a jak funguje</span><span class="sxs-lookup"><span data-stu-id="77732-107">Your credit limit and how it works</span></span>

<span data-ttu-id="77732-108">Váš limit kreditu je maximální částka (v USD), kterou jako partner můžete utratíte za nákup produktů nebo předplatných v Partnerské centrum.</span><span class="sxs-lookup"><span data-stu-id="77732-108">Your credit limit is the maximum amount (in US dollars) that you as a partner can spend to purchase products or subscriptions in Partner Center.</span></span> <span data-ttu-id="77732-109">Pokud překročíte limit kreditu, nebude možné provádět nové nákupy, dokud nebude provedena dostatečná platba.</span><span class="sxs-lookup"><span data-stu-id="77732-109">If you exceed your credit limit, you’ll be unable to make new purchases until sufficient payment has been made.</span></span> <span data-ttu-id="77732-110">Vaše stávající předplatná budou bez přerušení.</span><span class="sxs-lookup"><span data-stu-id="77732-110">Your existing subscriptions will continue uninterrupted.</span></span>

<span data-ttu-id="77732-111">Limity kreditů se vztahují na nabídky v plánech Azure, rezervacích Azure, softwaru, Marketplace, Azure 145 P, Office a produktech Dynamics.</span><span class="sxs-lookup"><span data-stu-id="77732-111">Credit limits apply to offers in Azure plan, Azure reservations, Software, Marketplace, Azure 145 P, Office, and Dynamics products.</span></span> <span data-ttu-id="77732-112">Limity kreditů se nevztahují na prodloužení a průběžné využití.</span><span class="sxs-lookup"><span data-stu-id="77732-112">Credit limits do not apply to renewals and ongoing consumption.</span></span>

<span data-ttu-id="77732-113">Během období onboardingu přiřadíme váš limit kreditu na úrovni tenanta.</span><span class="sxs-lookup"><span data-stu-id="77732-113">We assign your credit limit at the tenant level during your onboarding period.</span></span> <span data-ttu-id="77732-114">Založit ho na vašich předpovídaných výnosech, nákupech a historii plateb.</span><span class="sxs-lookup"><span data-stu-id="77732-114">We base it on your forecasted revenue, purchasing prowess, and payment history.</span></span> <span data-ttu-id="77732-115">K výpočtu dostupného zůstatku pak použijeme následující vzorec:</span><span class="sxs-lookup"><span data-stu-id="77732-115">We then use the following formula to calculate your available balance:</span></span>

<span data-ttu-id="77732-116">**[Credit Limit – (Incoming Purchase + Outstanding Unpaid Invoices + Unbilled Charges – Overpayment)]**</span><span class="sxs-lookup"><span data-stu-id="77732-116">**[Credit Limit – (Incoming Purchase + Outstanding Unpaid Invoices + Unbilled Charges – Overpayment)]**</span></span>

## <a name="frequently-asked-questions"></a><span data-ttu-id="77732-117">Nejčastější dotazy</span><span class="sxs-lookup"><span data-stu-id="77732-117">Frequently Asked Questions</span></span>

### <a name="is-my-credit-limit-set-at-the-tenant-or-global-level"></a><span data-ttu-id="77732-118">Je limit kreditu nastavený na úrovni tenanta nebo na globální úrovni?</span><span class="sxs-lookup"><span data-stu-id="77732-118">Is my credit limit set at the tenant or global level?</span></span>

<span data-ttu-id="77732-119">Úroveň tenanta.</span><span class="sxs-lookup"><span data-stu-id="77732-119">The tenant level.</span></span> <span data-ttu-id="77732-120">Předpokládejme například, že pracujete z USA, Kanady a Japonska.</span><span class="sxs-lookup"><span data-stu-id="77732-120">For example, suppose you operate from the US, Canada, and Japan.</span></span> <span data-ttu-id="77732-121">Pokud kanadský tenant dosáhne svého limitu kreditu, obdrží tento tenant oznámení, když se pokusí provést nákup v Partnerské centrum.</span><span class="sxs-lookup"><span data-stu-id="77732-121">If the Canadian tenant reaches its credit limit, then that tenant will receive a notification when they attempt to make a purchase in Partner Center.</span></span> <span data-ttu-id="77732-122">Ostatní tenanty to nebude mít vliv.</span><span class="sxs-lookup"><span data-stu-id="77732-122">The other tenants will not be affected.</span></span> 

### <a name="if-i-exceed-my-credit-limit-can-i-continue-servicing-existing-customers-and-subscriptions-with-full-access"></a><span data-ttu-id="77732-123">Pokud překročím svůj úvěrový limit, můžu pokračovat ve obsluhování stávajících zákazníků a předplatných s úplným přístupem?</span><span class="sxs-lookup"><span data-stu-id="77732-123">If I exceed my credit limit, can I continue servicing existing customers and subscriptions with full access?</span></span>

<span data-ttu-id="77732-124">Ano.</span><span class="sxs-lookup"><span data-stu-id="77732-124">Yes.</span></span> <span data-ttu-id="77732-125">Stávající předplatná vašich zákazníků budou bez přerušení pokračovat.</span><span class="sxs-lookup"><span data-stu-id="77732-125">Your customers’ existing subscriptions will continue without interruption.</span></span> <span data-ttu-id="77732-126">Nemůžete ale koupit nové předplatné pro vaše zákazníky.</span><span class="sxs-lookup"><span data-stu-id="77732-126">However, you cannot buy new subscriptions for your customers.</span></span>

### <a name="does-cle-apply-to-both-direct-bill-partners-and-indirect-providers"></a><span data-ttu-id="77732-127">Vztahuje se CLE na přímé i nepřímých poskytovatelů faktur?</span><span class="sxs-lookup"><span data-stu-id="77732-127">Does CLE apply to both direct bill partners and indirect providers?</span></span>

<span data-ttu-id="77732-128">Ano, platí pro obojí.</span><span class="sxs-lookup"><span data-stu-id="77732-128">Yes, it applies to both.</span></span>

### <a name="after-i-submit-my-payment-to-reinstate-my-account-when-can-i-purchase-more-subscriptions"></a><span data-ttu-id="77732-129">Kdy se po odeslání platby má účet obnovit, kdy si můžu koupit další předplatné?</span><span class="sxs-lookup"><span data-stu-id="77732-129">After I submit my payment to reinstate my account, when can I purchase more subscriptions?</span></span> 

<span data-ttu-id="77732-130">Během 24 hodin platby byste měli být schopni pokračovat v nákupu, a to za předpokladu, že společnost Microsoft obdržela všechny požadavky, aby bylo možné pokračovat v procesu kontroly kreditu.</span><span class="sxs-lookup"><span data-stu-id="77732-130">You should be able to resume purchasing within 24 hours of your payment, assuming Microsoft has received all the requirements to proceed with the credit check process.</span></span>

### <a name="how-can-i-check-my-credit-limit"></a><span data-ttu-id="77732-131">Jak si můžu ověřit úvěrový limit?</span><span class="sxs-lookup"><span data-stu-id="77732-131">How can I check my credit limit?</span></span>

<span data-ttu-id="77732-132">Kontaktujte, pokud [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) chcete zobrazit úvěrový limit a získat informace o nedávném nákupu.</span><span class="sxs-lookup"><span data-stu-id="77732-132">Contact [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) to see your credit limit and get information about recent purchases.</span></span>

### <a name="do-invoices-that-are-in-dispute-count-against-the-credit-limit"></a><span data-ttu-id="77732-133">Mají se faktury v počtu sporů s limitem úvěru?</span><span class="sxs-lookup"><span data-stu-id="77732-133">Do invoices that are in dispute count against the credit limit?</span></span>

<span data-ttu-id="77732-134">Ano.</span><span class="sxs-lookup"><span data-stu-id="77732-134">Yes.</span></span> <span data-ttu-id="77732-135">Můžete však kontaktovat společnost Microsoft [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) a vyřešit problém.</span><span class="sxs-lookup"><span data-stu-id="77732-135">However, you can contact Microsoft at [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) to resolve the issue.</span></span>

### <a name="how-soon-will-i-hear-back-if-i-write-to-ucmwrcspmicrosoftcom"></a><span data-ttu-id="77732-136">Jak brzy uslyším, když zapisujem ucmwrcsp@microsoft.com ?</span><span class="sxs-lookup"><span data-stu-id="77732-136">How soon will I hear back if I write to ucmwrcsp@microsoft.com?</span></span>

<span data-ttu-id="77732-137">Odpověď by měla být kratší než 24 hodin.</span><span class="sxs-lookup"><span data-stu-id="77732-137">You should have a response in less than 24 hours.</span></span> 

### <a name="what-criteria-does-microsoft-use-for-setting-a-partners-credit-limit"></a><span data-ttu-id="77732-138">Jaká kritéria Microsoft používá k nastavení úvěrového limitu pro partnery?</span><span class="sxs-lookup"><span data-stu-id="77732-138">What criteria does Microsoft use for setting a partner’s credit limit?</span></span>

<span data-ttu-id="77732-139">Váš limit kreditu určíme na základě vašich předpokládaných výnosů, nákupu prowess a historie plateb.</span><span class="sxs-lookup"><span data-stu-id="77732-139">We determine your credit limit based on your forecasted revenue, purchasing prowess, and payment history.</span></span>

### <a name="is-the-credit-limit-currently-enforced-on-the-new-commerce-experience"></a><span data-ttu-id="77732-140">Je limit úvěru aktuálně vyhodnocený na novém prostředí pro obchod?</span><span class="sxs-lookup"><span data-stu-id="77732-140">Is the credit limit currently enforced on the New Commerce Experience?</span></span>

<span data-ttu-id="77732-141">Ano.</span><span class="sxs-lookup"><span data-stu-id="77732-141">Yes.</span></span> <span data-ttu-id="77732-142">Úvěrový limit se vztahuje na všechny programy a produkty CSP v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="77732-142">Credit limits apply to all CSP programs and products in Partner Center.</span></span>

### <a name="who-will-receive-the-notification-when-my-organization-is-nearing-its-credit-limit"></a><span data-ttu-id="77732-143">Kdo obdrží oznámení, když se moje organizace blíží limitu úvěru?</span><span class="sxs-lookup"><span data-stu-id="77732-143">Who will receive the notification when my organization is nearing its credit limit?</span></span>

<span data-ttu-id="77732-144">Oznámení o závazku finančního účtu vaší organizace by mělo obdržet oznámení.</span><span class="sxs-lookup"><span data-stu-id="77732-144">Your organization's Finance Account Payable contact should receive the notification.</span></span>

## <a name="next-steps"></a><span data-ttu-id="77732-145">Další kroky</span><span class="sxs-lookup"><span data-stu-id="77732-145">Next steps</span></span>

[<span data-ttu-id="77732-146">Základní informace o fakturaci</span><span class="sxs-lookup"><span data-stu-id="77732-146">Billing basics</span></span>](./billing-basics.md)
