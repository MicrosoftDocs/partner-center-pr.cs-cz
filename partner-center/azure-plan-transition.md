---
title: Přesun zákazníků z aktuálních nabídek Azure do plánu Azure
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Přečtěte si, jak partneři CSP můžou pomocí partnerského centra přesunout zákazníky ze stávajících nabídek CSP Azure do služeb Azure v rámci plánu Azure.
author: mowree
ms.author: mowrim
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/16/2020
ms.openlocfilehash: 4e22386dc8bddd9662a0d80020a5c90c464e9d39
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534807"
---
# <a name="transition-customers-to-azure-plan-from-existing-csp-azure-offers"></a><span data-ttu-id="d806f-103">Přechod zákazníků do plánu Azure ze stávajících nabídek Azure CSP</span><span class="sxs-lookup"><span data-stu-id="d806f-103">Transition customers to Azure plan from existing CSP Azure offers</span></span>

<span data-ttu-id="d806f-104">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="d806f-104">**Appropriate roles**</span></span>

- <span data-ttu-id="d806f-105">Agent správce</span><span class="sxs-lookup"><span data-stu-id="d806f-105">Admin agent</span></span>
- <span data-ttu-id="d806f-106">Správce fakturace</span><span class="sxs-lookup"><span data-stu-id="d806f-106">Billing admin</span></span>
- <span data-ttu-id="d806f-107">Globální správce</span><span class="sxs-lookup"><span data-stu-id="d806f-107">Global admin</span></span>
- <span data-ttu-id="d806f-108">Agent helpdesku</span><span class="sxs-lookup"><span data-stu-id="d806f-108">Helpdesk agent</span></span>
- <span data-ttu-id="d806f-109">Agent prodeje</span><span class="sxs-lookup"><span data-stu-id="d806f-109">Sales agent</span></span>
- <span data-ttu-id="d806f-110">Správce správy uživatelů</span><span class="sxs-lookup"><span data-stu-id="d806f-110">User management admin</span></span>

<span data-ttu-id="d806f-111">V tomto článku se dozvíte, jak můžou partneři CSP používat Partnerské centrum k přesunu zákazníků ze stávajících nabídek CSP Azure do služeb Azure v rámci plánu Azure.</span><span class="sxs-lookup"><span data-stu-id="d806f-111">This article explains how CSP partners can use Partner Center to move customers from existing CSP Azure offers to Azure services under the Azure plan.</span></span> <span data-ttu-id="d806f-112">Nepřímá poskytovatelé a Přímí partneři s přímým přístupem můžou přejít na nové prostředí pro obchod, které je dostupné v programu poskytovatele Microsoft Cloudch služeb (CSP) pro Azure.</span><span class="sxs-lookup"><span data-stu-id="d806f-112">Indirect providers and direct bill partners can transition to the new commerce experience available in the Microsoft Cloud Service Provider Program (CSP) for Azure.</span></span> <span data-ttu-id="d806f-113">(Nepřímí prodejci budou muset pracovat prostřednictvím jejich nepřímých zprostředkovatelů.) Zákazníci budou mít k dispozici zjednodušený způsob nákupu cloudových služeb, ať už se jedná o nákupy od partnerů, od prodejců Microsoftu nebo přímo na webu.</span><span class="sxs-lookup"><span data-stu-id="d806f-113">(Indirect resellers will need to work through their indirect providers.) Customers will have a streamlined way to buy cloud services, whether purchasing from partners, from Microsoft sellers, or directly on the web.</span></span>

<span data-ttu-id="d806f-114">Možnost přechodu je určena jenom pro zákazníky, kteří přecházejí na nové prostředí pro obchod s Azure a kteří podepsali smlouvu o zákaznících Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="d806f-114">The transition capability is only for customers transitioning to the new commerce experience for Azure and who have signed the Microsoft Customer Agreement.</span></span> <span data-ttu-id="d806f-115">Nejedná se o jiné nabídky ve zprostředkovateli CSP, jako je například Office 365 nebo Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="d806f-115">It is not for other offers in CSP such as Office 365 or Dynamics 365.</span></span>

## <a name="transition-existing-csp-offers-to-an-azure-plan"></a><span data-ttu-id="d806f-116">Převod stávajících nabídek CSP na plán Azure</span><span class="sxs-lookup"><span data-stu-id="d806f-116">Transition existing CSP offers to an Azure plan</span></span>

<span data-ttu-id="d806f-117">Zákazníky ze svých stávajících poskytovatelů CSP Azure můžete převést na služby Azure v rámci plánu Azure v rámci nového prostředí pro obchod v programu CSP z partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="d806f-117">You can transition a customer from their existing CSP Azure offers to Azure services under the Azure plan in the new commerce experience in the CSP program from within Partner Center.</span></span> <span data-ttu-id="d806f-118">Aby to bylo možné, musí mít partner a zákazník zavedeného vztahu prodejce prostřednictvím partnerského centra a zákazník musí mít podepsané smlouvy o zákaznících Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="d806f-118">To do this, the partner and customer must have an established reseller relationship through Partner Center, and the customer must have signed the Microsoft Customer Agreement.</span></span>

### <a name="select-transition-to-azure-plan"></a><span data-ttu-id="d806f-119">Vybrat přechod do plánu Azure</span><span class="sxs-lookup"><span data-stu-id="d806f-119">Select transition to Azure plan</span></span>

1. <span data-ttu-id="d806f-120">Vyberte plán Azure pro zákazníka.</span><span class="sxs-lookup"><span data-stu-id="d806f-120">Select Azure plan for your customer.</span></span>

2. <span data-ttu-id="d806f-121">Vyberte **Převod fakturace do plánu Azure**.</span><span class="sxs-lookup"><span data-stu-id="d806f-121">Select **Transition billing to Azure plan**.</span></span>

   :::image type="content" source="images/azure/transition1.png" alt-text="Snímek obrazovky s informacemi o předplatných založených na využití s možností s možností volby s názvem: přechod předplatného Azure do plánu Azure":::

3. <span data-ttu-id="d806f-123">Vyberte **Pokračovat**.</span><span class="sxs-lookup"><span data-stu-id="d806f-123">Select **Continue**</span></span>

   :::image type="content" source="images/azure/transition2.png" alt-text="Dialogové okno s názvem přechod do plánu Azure s důsledky pro přečtení o přechodu a dvou možnostech pro výběr, pokračování nebo zrušení.":::

   <span data-ttu-id="d806f-125">Váš zákazník se převede na plán Azure.</span><span class="sxs-lookup"><span data-stu-id="d806f-125">Your customer will be transitioned to the Azure plan.</span></span>

   <span data-ttu-id="d806f-126">**Pracovní postup přechodu automatizuje požadavky na tyto kroky**:</span><span class="sxs-lookup"><span data-stu-id="d806f-126">**The transition workflow automates the pre-requisite steps**:</span></span>

   - <span data-ttu-id="d806f-127">Nákup plánů Azure</span><span class="sxs-lookup"><span data-stu-id="d806f-127">Purchase of Azure plan(s)</span></span>
   - <span data-ttu-id="d806f-128">Jeden plán na zákazníka ve scénářích přímého CSP</span><span class="sxs-lookup"><span data-stu-id="d806f-128">One plan per customer in Direct CSP scenarios</span></span>  
   - <span data-ttu-id="d806f-129">Jeden plán na prodejce</span><span class="sxs-lookup"><span data-stu-id="d806f-129">One plan per reseller</span></span>  

   <span data-ttu-id="d806f-130">Například partneři koupili dvě Microsoft Azure nabídky a zahrnuli do nákupu dvě jedinečné POR.</span><span class="sxs-lookup"><span data-stu-id="d806f-130">For an example, a partner has purchased two Microsoft Azure offers and has included two distinct POR in the purchase.</span></span> <span data-ttu-id="d806f-131">V takovém případě bude pracovní postup přechodu nakoupit dva plány Azure (jeden na prodejce) a automaticky namapovat příslušné předplatné Azure v rámci plánů Azure.</span><span class="sxs-lookup"><span data-stu-id="d806f-131">In this case, the transition    workflow will purchase two Azure plans (one per reseller) and map the respective Azure subscriptions under the Azure plans automatically.</span></span>  

   <span data-ttu-id="d806f-132">**Mapování předplatného Azure na plán Azure**</span><span class="sxs-lookup"><span data-stu-id="d806f-132">**Mapping Azure subscription to Azure plan**</span></span>

   <span data-ttu-id="d806f-133">Po zakoupení plánů Azure provede náš systém mapování stávajících předplatných Azure na plány Azure.</span><span class="sxs-lookup"><span data-stu-id="d806f-133">After your purchase of Azure plan(s), our system will map the existing Azure subscriptions to the Azure plans.</span></span> <span data-ttu-id="d806f-134">Průběh můžete zobrazit v Azure Portal i v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="d806f-134">The progress can be viewed in Azure portal as well as in Partner center.</span></span>

4. <span data-ttu-id="d806f-135">Vraťte se na stránku **předplatná** partnerského centra zákazníka a aktualizujte svůj limit rozpočtu pomocí místní měny.</span><span class="sxs-lookup"><span data-stu-id="d806f-135">Return to your customer's Partner Center **Subscriptions** page to update their budget limit using their local currency.</span></span>

   :::image type="content" source="images/azure/transition3.png" alt-text="Částečné zobrazení stránky předplatná partnerského centra s limity rozpočtu nastavenými v místní měně pro fakturační období":::

   >[!NOTE]
   ><span data-ttu-id="d806f-137">Rozpočet, který jste nastavili v partnerském centru, se nepřenese do Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="d806f-137">The budget you set in Partner Center doesn't carry over to the Azure portal.</span></span> <span data-ttu-id="d806f-138">Měli byste také nastavit rozpočet a výstrahu v Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="d806f-138">You should also set the budget and alert in Azure portal.</span></span>

   <span data-ttu-id="d806f-139">Když přejdete na plán Azure, nebudete už moct koupit předplatné Azure pro tohoto zákazníka.</span><span class="sxs-lookup"><span data-stu-id="d806f-139">When you move to the Azure plan, you can no longer purchase Azure subscriptions for this customer.</span></span> <span data-ttu-id="d806f-140">Předplatná můžete vytvořit v rámci plánu Azure v Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="d806f-140">You create the subscriptions under the Azure plan in the Azure portal.</span></span>

   >[!NOTE]
   > <span data-ttu-id="d806f-141">Všechna předplatná Azure zakoupená prostřednictvím služby RBAC v rámci plánu Azure se účtují a účtují v místní měně.</span><span class="sxs-lookup"><span data-stu-id="d806f-141">All Azure subscriptions purchased through RBAC under the Azure plan will be    priced and billed in local currency.</span></span> <span data-ttu-id="d806f-142">Sazby za FX nebudou použity.</span><span class="sxs-lookup"><span data-stu-id="d806f-142">FX rates will not be used.</span></span>

### <a name="track-your-transition-details"></a><span data-ttu-id="d806f-143">Sledovat podrobnosti přechodu</span><span class="sxs-lookup"><span data-stu-id="d806f-143">Track your transition details</span></span>

<span data-ttu-id="d806f-144">Sledujte průběh přechodu v Azure Portal i v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="d806f-144">Follow the transition progress in Azure portal as well as in Partner Center.</span></span>

:::image type="content" source="images/azure/details1.png" alt-text="Snímek obrazovky s tabulkou se seznamem podrobností o přechodu na předplatné – zahrnuje předplatné I D, datum přechodu a stav přechodu.":::

### <a name="billing-impact-to-partners"></a><span data-ttu-id="d806f-146">Dopad fakturace na partnery</span><span class="sxs-lookup"><span data-stu-id="d806f-146">Billing impact to partners</span></span>

<span data-ttu-id="d806f-147">Pokud převedete zákazníka ze stávající nabídky Azure CSP, budete mít následující dopady na fakturaci:</span><span class="sxs-lookup"><span data-stu-id="d806f-147">If you transition a customer from an existing CSP Azure offer, you will have the following billing impacts:</span></span>

- <span data-ttu-id="d806f-148">Bude se vám účtovat stávající faktura CSP pro veškeré využití až do chvíle, kdy se původní předplatné služby CSP Azure ukončí.</span><span class="sxs-lookup"><span data-stu-id="d806f-148">You will be billed on your existing CSP invoice for all usage up to the point of exiting the original CSP Azure subscription.</span></span>

- <span data-ttu-id="d806f-149">Pokud máte přístupová práva správce k existujícímu předplatnému CSP, budete mít k dispozici přístup i v případě, že je předplatné migrováno.</span><span class="sxs-lookup"><span data-stu-id="d806f-149">If you had admin access rights to the existing CSP subscription, you will continue to have access when that subscription is migrated.</span></span>

<span data-ttu-id="d806f-150">Pro přechod přímých smluv Enterprise na cloudové a cloudové registrace do služeb Azure si přečtěte téma [získání vlastnictví fakturace předplatných Azure pro partnery Microsoftu](/azure/billing/mpa-request-ownership) .</span><span class="sxs-lookup"><span data-stu-id="d806f-150">To transition direct Enterprise Agreements to CSP and Server and Cloud enrollments to Azure services, read [Get billing ownership of Azure subscriptions for Microsoft Partner Agreement](/azure/billing/mpa-request-ownership)</span></span>

### <a name="audit-log"></a><span data-ttu-id="d806f-151">Protokol auditu</span><span class="sxs-lookup"><span data-stu-id="d806f-151">Audit log</span></span>

<span data-ttu-id="d806f-152">Pokud chcete sjednotit fakturaci, zobrazte si historii předplatných "Microsoft Azure" (0145P) na stránce **předplatná** .</span><span class="sxs-lookup"><span data-stu-id="d806f-152">To reconcile billing, view your history of "Microsoft Azure" (0145P) subscriptions on the **Subscriptions** page.</span></span>

<span data-ttu-id="d806f-153">Předplatné "Microsoft Azure" (0145P) se skládá ze dvou částí:</span><span class="sxs-lookup"><span data-stu-id="d806f-153">"Microsoft Azure" (0145P) subscription is comprised of two parts:</span></span>

1. <span data-ttu-id="d806f-154">Předplatné Commerce</span><span class="sxs-lookup"><span data-stu-id="d806f-154">Commerce subscription</span></span>
2. <span data-ttu-id="d806f-155">Předplatné Azure (nárok)</span><span class="sxs-lookup"><span data-stu-id="d806f-155">Azure subscription (entitlement)</span></span>

<span data-ttu-id="d806f-156">Po dokončení přechodu se předplatné Azure přesune v části nový plán Azure a předplatné Commerce se pozastaví, aby se neoznámilo žádné další použití.</span><span class="sxs-lookup"><span data-stu-id="d806f-156">When the transition is complete, the Azure subscription is moved under new Azure plan and the commerce subscription is suspended so that no further usage is reported.</span></span>  

>[!NOTE]
><span data-ttu-id="d806f-157">Po zakoupení předplatného Microsoft Azure (0145P) ve zprostředkovateli CSP mají stejné hodnoty jak předplatné obchodu, tak i předplatné Azure (nárok).</span><span class="sxs-lookup"><span data-stu-id="d806f-157">When Microsoft Azure (0145P) subscription is purchased in CSP, both the commerce subscription and the Azure subscription (entitlement) have the same value.</span></span> <span data-ttu-id="d806f-158">Pouze v případě změny vlastnictví fakturace nebo převodů se hodnoty liší.</span><span class="sxs-lookup"><span data-stu-id="d806f-158">It is only in the case of billing ownership changes or transfers do the values differ.</span></span>

### <a name="transition-issues"></a><span data-ttu-id="d806f-159">Problémy s přechodem</span><span class="sxs-lookup"><span data-stu-id="d806f-159">Transition issues</span></span>

<span data-ttu-id="d806f-160">Během přechodů nepředpokládáme žádné problémy.</span><span class="sxs-lookup"><span data-stu-id="d806f-160">We don't anticipate any issues during transitions.</span></span> <span data-ttu-id="d806f-161">Pokud k tomu dojde, budeme v pracovním postupu přechodu aktualizovat sám sebe.</span><span class="sxs-lookup"><span data-stu-id="d806f-161">If one occurs, we will update you in the transition workflow itself.</span></span> <span data-ttu-id="d806f-162">Nehrozí žádné narušení využití Azure.</span><span class="sxs-lookup"><span data-stu-id="d806f-162">There won't be disturbances to Azure usage.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="d806f-163">Další kroky</span><span class="sxs-lookup"><span data-stu-id="d806f-163">Next steps</span></span>

- [<span data-ttu-id="d806f-164">Správa předplatných a prostředků v rámci plánu Azure</span><span class="sxs-lookup"><span data-stu-id="d806f-164">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)

- [<span data-ttu-id="d806f-165">Získaný kredit partnerů – přehled</span><span class="sxs-lookup"><span data-stu-id="d806f-165">Partner earned credit - overview</span></span>](partner-earned-credit.md)