---
title: Vynucení limitu kreditu
ms.topic: how-to
ms.date: 05/11/2021
description: Přečtěte si o kreditním limitu a o tom, jak se počítá. Obsahuje nejčastější dotazy.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: da3fc23a51cc70eec91a304f14189eb191c71339
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148104"
---
# <a name="credit-limit-enforcement-cle"></a><span data-ttu-id="a266b-104">Vynucení limitu kreditu (CLE)</span><span class="sxs-lookup"><span data-stu-id="a266b-104">Credit limit enforcement (CLE)</span></span>

<span data-ttu-id="a266b-105">**Příslušné role**: správce fakturace</span><span class="sxs-lookup"><span data-stu-id="a266b-105">**Appropriate roles**: Billing admin</span></span>

## <a name="your-credit-limit-and-how-it-works"></a><span data-ttu-id="a266b-106">Limit kreditu a jak to funguje</span><span class="sxs-lookup"><span data-stu-id="a266b-106">Your credit limit and how it works</span></span>

<span data-ttu-id="a266b-107">Vaše kreditní omezení je maximální částka (v amerických dolarech), kterou můžete jako partner zaplatit za nákup produktů nebo předplatných v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="a266b-107">Your credit limit is the maximum amount (in US dollars) that you as a partner can spend to purchase products or subscriptions in Partner Center.</span></span> <span data-ttu-id="a266b-108">Pokud překročíte úvěrový limit, nebudete moct vytvářet nové nákupy, dokud neproběhne dostatečná platba.</span><span class="sxs-lookup"><span data-stu-id="a266b-108">If you exceed your credit limit, you’ll be unable to make new purchases until sufficient payment has been made.</span></span> <span data-ttu-id="a266b-109">Stávající předplatná budou bez přerušení pokračovat.</span><span class="sxs-lookup"><span data-stu-id="a266b-109">Your existing subscriptions will continue uninterrupted.</span></span>

<span data-ttu-id="a266b-110">Úvěrový limit se vztahuje na nabídky v plánu Azure, rezervacích Azure, softwaru, Marketplace, Azure 145 P, Office a Dynamics Products.</span><span class="sxs-lookup"><span data-stu-id="a266b-110">Credit limits apply to offers in Azure plan, Azure reservations, Software, Marketplace, Azure 145 P, Office, and Dynamics products.</span></span> <span data-ttu-id="a266b-111">Limity úvěru se nevztahují na obnovení a průběžnou spotřebu.</span><span class="sxs-lookup"><span data-stu-id="a266b-111">Credit limits do not apply to renewals and ongoing consumption.</span></span>

<span data-ttu-id="a266b-112">Vaše kreditní limit přiřadíme na úrovni tenanta během období připojování.</span><span class="sxs-lookup"><span data-stu-id="a266b-112">We assign your credit limit at the tenant level during your onboarding period.</span></span> <span data-ttu-id="a266b-113">Založíme ji na vaše předpovědi pro tržby, nákup prowess a historii plateb.</span><span class="sxs-lookup"><span data-stu-id="a266b-113">We base it on your forecasted revenue, purchasing prowess, and payment history.</span></span> <span data-ttu-id="a266b-114">K výpočtu dostupného zůstatku použijeme následující vzorec:</span><span class="sxs-lookup"><span data-stu-id="a266b-114">We then use the following formula to calculate your available balance:</span></span>

<span data-ttu-id="a266b-115">**[Limit úvěru – (příchozí nákup + nedokončené faktury + neúčtované poplatky – přeplatek)]**</span><span class="sxs-lookup"><span data-stu-id="a266b-115">**[Credit Limit – (Incoming Purchase + Outstanding Unpaid Invoices + Unbilled Charges – Overpayment)]**</span></span>

## <a name="frequently-asked-questions"></a><span data-ttu-id="a266b-116">Nejčastější dotazy</span><span class="sxs-lookup"><span data-stu-id="a266b-116">Frequently Asked Questions</span></span>

### <a name="is-my-credit-limit-set-at-the-tenant-or-global-level"></a><span data-ttu-id="a266b-117">Je můj limit kreditu nastavený na tenantovi nebo na globální úrovni?</span><span class="sxs-lookup"><span data-stu-id="a266b-117">Is my credit limit set at the tenant or global level?</span></span>

<span data-ttu-id="a266b-118">Úroveň tenanta.</span><span class="sxs-lookup"><span data-stu-id="a266b-118">The tenant level.</span></span> <span data-ttu-id="a266b-119">Předpokládejme například, že pracujete v USA, Kanadě a Japonsku.</span><span class="sxs-lookup"><span data-stu-id="a266b-119">For example, suppose you operate from the US, Canada, and Japan.</span></span> <span data-ttu-id="a266b-120">Pokud má kanadský tenant limit úvěru, pak tento tenant obdrží oznámení o tom, že se pokusí koupit v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="a266b-120">If the Canadian tenant reaches its credit limit, then that tenant will receive a notification when they attempt to make a purchase in Partner Center.</span></span> <span data-ttu-id="a266b-121">Ostatní klienti nebudou ovlivněni.</span><span class="sxs-lookup"><span data-stu-id="a266b-121">The other tenants will not be affected.</span></span> 

### <a name="if-i-exceed-my-credit-limit-can-i-continue-servicing-existing-customers-and-subscriptions-with-full-access"></a><span data-ttu-id="a266b-122">Pokud překročím svůj úvěrový limit, můžu pokračovat ve obsluhování stávajících zákazníků a předplatných s úplným přístupem?</span><span class="sxs-lookup"><span data-stu-id="a266b-122">If I exceed my credit limit, can I continue servicing existing customers and subscriptions with full access?</span></span>

<span data-ttu-id="a266b-123">Ano.</span><span class="sxs-lookup"><span data-stu-id="a266b-123">Yes.</span></span> <span data-ttu-id="a266b-124">Stávající předplatná vašich zákazníků budou bez přerušení pokračovat.</span><span class="sxs-lookup"><span data-stu-id="a266b-124">Your customers’ existing subscriptions will continue without interruption.</span></span> <span data-ttu-id="a266b-125">Nemůžete ale koupit nové předplatné pro vaše zákazníky.</span><span class="sxs-lookup"><span data-stu-id="a266b-125">However, you cannot buy new subscriptions for your customers.</span></span>

### <a name="does-cle-apply-to-both-direct-bill-partners-and-indirect-providers"></a><span data-ttu-id="a266b-126">Vztahuje se CLE na přímé i nepřímých poskytovatelů faktur?</span><span class="sxs-lookup"><span data-stu-id="a266b-126">Does CLE apply to both direct bill partners and indirect providers?</span></span>

<span data-ttu-id="a266b-127">Ano, platí pro obojí.</span><span class="sxs-lookup"><span data-stu-id="a266b-127">Yes, it applies to both.</span></span>

### <a name="after-i-submit-my-payment-to-reinstate-my-account-when-can-i-purchase-more-subscriptions"></a><span data-ttu-id="a266b-128">Kdy se po odeslání platby má účet obnovit, kdy si můžu koupit další předplatné?</span><span class="sxs-lookup"><span data-stu-id="a266b-128">After I submit my payment to reinstate my account, when can I purchase more subscriptions?</span></span> 

<span data-ttu-id="a266b-129">Během 24 hodin platby byste měli být schopni pokračovat v nákupu, a to za předpokladu, že společnost Microsoft obdržela všechny požadavky, aby bylo možné pokračovat v procesu kontroly kreditu.</span><span class="sxs-lookup"><span data-stu-id="a266b-129">You should be able to resume purchasing within 24 hours of your payment, assuming Microsoft has received all the requirements to proceed with the credit check process.</span></span>

### <a name="how-can-i-check-my-credit-limit"></a><span data-ttu-id="a266b-130">Jak si můžu ověřit úvěrový limit?</span><span class="sxs-lookup"><span data-stu-id="a266b-130">How can I check my credit limit?</span></span>

<span data-ttu-id="a266b-131">Kontaktujte, pokud [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) chcete zobrazit úvěrový limit a získat informace o nedávném nákupu.</span><span class="sxs-lookup"><span data-stu-id="a266b-131">Contact [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) to see your credit limit and get information about recent purchases.</span></span>

### <a name="do-invoices-that-are-in-dispute-count-against-the-credit-limit"></a><span data-ttu-id="a266b-132">Mají se faktury v počtu sporů s limitem úvěru?</span><span class="sxs-lookup"><span data-stu-id="a266b-132">Do invoices that are in dispute count against the credit limit?</span></span>

<span data-ttu-id="a266b-133">Ano.</span><span class="sxs-lookup"><span data-stu-id="a266b-133">Yes.</span></span> <span data-ttu-id="a266b-134">Můžete však kontaktovat společnost Microsoft [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) a vyřešit problém.</span><span class="sxs-lookup"><span data-stu-id="a266b-134">However, you can contact Microsoft at [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) to resolve the issue.</span></span>

### <a name="how-soon-will-i-hear-back-if-i-write-to-ucmwrcspmicrosoftcom"></a><span data-ttu-id="a266b-135">Jak brzy uslyším, když zapisujem ucmwrcsp@microsoft.com ?</span><span class="sxs-lookup"><span data-stu-id="a266b-135">How soon will I hear back if I write to ucmwrcsp@microsoft.com?</span></span>

<span data-ttu-id="a266b-136">Odpověď by měla být kratší než 24 hodin.</span><span class="sxs-lookup"><span data-stu-id="a266b-136">You should have a response in less than 24 hours.</span></span> 

### <a name="what-criteria-does-microsoft-use-for-setting-a-partners-credit-limit"></a><span data-ttu-id="a266b-137">Jaká kritéria Microsoft používá k nastavení úvěrového limitu pro partnery?</span><span class="sxs-lookup"><span data-stu-id="a266b-137">What criteria does Microsoft use for setting a partner’s credit limit?</span></span>

<span data-ttu-id="a266b-138">Váš limit kreditu určíme na základě vašich předpokládaných výnosů, nákupu prowess a historie plateb.</span><span class="sxs-lookup"><span data-stu-id="a266b-138">We determine your credit limit based on your forecasted revenue, purchasing prowess, and payment history.</span></span>

### <a name="is-the-credit-limit-currently-enforced-on-the-new-commerce-experience"></a><span data-ttu-id="a266b-139">Je limit úvěru aktuálně vyhodnocený na novém prostředí pro obchod?</span><span class="sxs-lookup"><span data-stu-id="a266b-139">Is the credit limit currently enforced on the New Commerce Experience?</span></span>

<span data-ttu-id="a266b-140">Ano.</span><span class="sxs-lookup"><span data-stu-id="a266b-140">Yes.</span></span> <span data-ttu-id="a266b-141">Úvěrový limit se vztahuje na všechny programy a produkty CSP v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="a266b-141">Credit limits apply to all CSP programs and products in Partner Center.</span></span>

### <a name="who-will-receive-the-notification-when-my-organization-is-nearing-its-credit-limit"></a><span data-ttu-id="a266b-142">Kdo obdrží oznámení, když se moje organizace blíží limitu úvěru?</span><span class="sxs-lookup"><span data-stu-id="a266b-142">Who will receive the notification when my organization is nearing its credit limit?</span></span>

<span data-ttu-id="a266b-143">Oznámení o závazku finančního účtu vaší organizace by mělo obdržet oznámení.</span><span class="sxs-lookup"><span data-stu-id="a266b-143">Your organization's Finance Account Payable contact should receive the notification.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a266b-144">Další kroky</span><span class="sxs-lookup"><span data-stu-id="a266b-144">Next steps</span></span>

[<span data-ttu-id="a266b-145">Základní informace o fakturaci</span><span class="sxs-lookup"><span data-stu-id="a266b-145">Billing basics</span></span>](./billing-basics.md)
