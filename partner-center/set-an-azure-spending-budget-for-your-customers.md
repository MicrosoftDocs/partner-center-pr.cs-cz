---
title: Nastavení rozpočtu na útratu zákazníků v Azure
ms.topic: how-to
ms.date: 03/17/2021
description: Naučte se, jak nastavit nebo odebrat měsíční rozpočty Azure útraty pro vaše zákazníky, a také zobrazit data o výdajích Azure a nastavit oznámení týkající se rozpočtu.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: eaf54898d7a130ca38e5a2aaeba279fb722c9e66
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712745"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="85f0a-103">Nastavení, kontrolu nebo odebrání měsíčních rozpočtů Azure útraty pro zákazníky v partnerském centru</span><span class="sxs-lookup"><span data-stu-id="85f0a-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="85f0a-104">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="85f0a-104">**Appropriate roles**</span></span>

- <span data-ttu-id="85f0a-105">Agent správce</span><span class="sxs-lookup"><span data-stu-id="85f0a-105">Admin agent</span></span>

<span data-ttu-id="85f0a-106">Můžete [nastavit měsíční rozpočet Azure útraty pro vaše zákazníky](#set-azure-spending-budget) v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="85f0a-106">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="85f0a-107">To pomáhá vašim zákazníkům spravovat útraty Azure.</span><span class="sxs-lookup"><span data-stu-id="85f0a-107">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="85f0a-108">Tato možnost umožňuje porovnat náklady na Azure, které jsou v daném měsíci v rozpočtu.</span><span class="sxs-lookup"><span data-stu-id="85f0a-108">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="85f0a-109">Pomáhá zákazníkům také rozpočtovat své výdaje na Azure, takže jejich měsíční vyúčtování není vyšší než jejich předvídání.</span><span class="sxs-lookup"><span data-stu-id="85f0a-109">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="85f0a-110">Tato funkce není k dispozici v izolovaném prostoru nebo v produkčním účtu (TIP).</span><span class="sxs-lookup"><span data-stu-id="85f0a-110">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="85f0a-111">Po [nastavení rozpočtu útraty Azure pro zákazníky](#set-azure-spending-budget)můžete také zkontrolovat používání zákazníka následujícími způsoby.</span><span class="sxs-lookup"><span data-stu-id="85f0a-111">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="85f0a-112">Tyto možnosti vám mohou nabídnout možnost vyznačovat nesprávně nakonfigurované služby nebo neobvyklé trendy, které mohou navrhovat podvod.</span><span class="sxs-lookup"><span data-stu-id="85f0a-112">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="85f0a-113">Potom můžete s vašimi zákazníky spolupracovat a identifikovat hlavní příčinu a spravovat náklady.</span><span class="sxs-lookup"><span data-stu-id="85f0a-113">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="85f0a-114">V případě potřeby můžete také [změnit rozpočet zákazníka](#set-azure-spending-budget) na vyšší částku.</span><span class="sxs-lookup"><span data-stu-id="85f0a-114">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="85f0a-115">Kontrolovat aktuální útratu Azure</span><span class="sxs-lookup"><span data-stu-id="85f0a-115">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="85f0a-116">Zapnout e-mailová oznámení v případě, že se útrata zákazníka blíží ke svému limitu rozpočtu</span><span class="sxs-lookup"><span data-stu-id="85f0a-116">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="85f0a-117">Zobrazit nákladové náklady podle služby pro odběry založené na využití</span><span class="sxs-lookup"><span data-stu-id="85f0a-117">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="85f0a-118">[Rozpočet Azure útraty](#remove-azure-spending-budget) můžete také kdykoli odebrat pro zákazníky.</span><span class="sxs-lookup"><span data-stu-id="85f0a-118">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="85f0a-119">Data o výdajích Azure</span><span class="sxs-lookup"><span data-stu-id="85f0a-119">Azure spending data</span></span>

<span data-ttu-id="85f0a-120">Data o výdajích Azure jsou *odhadem* a *skutečné fakturační částky se můžou lišit*.</span><span class="sxs-lookup"><span data-stu-id="85f0a-120">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="85f0a-121">Hodnota dat *nezohledňuje* daně, kredity, úpravy nebo jiné poplatky, které mohou platit.</span><span class="sxs-lookup"><span data-stu-id="85f0a-121">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="85f0a-122">Data o výdajích se *aktualizují jednou denně*.</span><span class="sxs-lookup"><span data-stu-id="85f0a-122">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="85f0a-123">Vaši zákazníci můžou dál používat (a budou se vám účtovat) služby a prostředky Azure, pokud nezměníte nastavení svého účtu v Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="85f0a-123">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="85f0a-124">Nastavení rozpočtu útraty Azure</span><span class="sxs-lookup"><span data-stu-id="85f0a-124">Set Azure spending budget</span></span>

<span data-ttu-id="85f0a-125">Můžete *nastavit měsíční rozpočet Azure útraty* pro více zákazníků v partnerském centru:</span><span class="sxs-lookup"><span data-stu-id="85f0a-125">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="85f0a-126">Přihlaste se k [řídicímu panelu pro Partnerské centrum](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="85f0a-126">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="85f0a-127">V nabídce vlevo v části **CSP** vyberte **útraty Azure**.</span><span class="sxs-lookup"><span data-stu-id="85f0a-127">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="85f0a-128">Na stránce **útraty Azure** v části **zákazníci s předplatnými Microsoft Azure** vyberte zákazníky, pro které chcete nastavit rozpočet.</span><span class="sxs-lookup"><span data-stu-id="85f0a-128">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="85f0a-129">Zadejte hodnotu pro **měsíční rozpočet**.</span><span class="sxs-lookup"><span data-stu-id="85f0a-129">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="85f0a-130">Chcete-li uložit změny, klikněte na tlačítko **použít** .</span><span class="sxs-lookup"><span data-stu-id="85f0a-130">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="85f0a-131">Můžete také *nastavit rozpočet pro jednotlivé zákazníky* v nastavení jejich předplatného:</span><span class="sxs-lookup"><span data-stu-id="85f0a-131">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="85f0a-132">Přihlaste se k řídicímu panelu pro Partnerské centrum.</span><span class="sxs-lookup"><span data-stu-id="85f0a-132">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="85f0a-133">V nabídce vlevo v části **CSP** vyberte **zákazníci**.</span><span class="sxs-lookup"><span data-stu-id="85f0a-133">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="85f0a-134">Na stránce **Customers (zákazníci** ) vyberte **název společnosti** zákazníka.</span><span class="sxs-lookup"><span data-stu-id="85f0a-134">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="85f0a-135">Na stránce **předplatná** zákazníka v části **předplatné na základě využití** vyberte **změnit rozpočet**.</span><span class="sxs-lookup"><span data-stu-id="85f0a-135">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="85f0a-136">Zadejte hodnotu pro rozpočet.</span><span class="sxs-lookup"><span data-stu-id="85f0a-136">Enter a value for the budget.</span></span>

6. <span data-ttu-id="85f0a-137">Chcete-li uložit změny, klikněte na tlačítko **použít** .</span><span class="sxs-lookup"><span data-stu-id="85f0a-137">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="85f0a-138">Odebrat rozpočet útraty Azure</span><span class="sxs-lookup"><span data-stu-id="85f0a-138">Remove Azure spending budget</span></span>

<span data-ttu-id="85f0a-139">*Měsíční rozpočet Azure útraty* můžete pro zákazníky v partnerském centru odebrat:</span><span class="sxs-lookup"><span data-stu-id="85f0a-139">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="85f0a-140">Přihlaste se k [řídicímu panelu pro Partnerské centrum](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="85f0a-140">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="85f0a-141">V nabídce vlevo v části **CSP** vyberte **útraty Azure**.</span><span class="sxs-lookup"><span data-stu-id="85f0a-141">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="85f0a-142">Na stránce **útraty Azure** v části **zákazníci s předplatnými Microsoft Azure** vyberte zákazníky, jejichž rozpočet chcete odebrat.</span><span class="sxs-lookup"><span data-stu-id="85f0a-142">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="85f0a-143">Vyberte možnost **Odebrat rozpočet**.</span><span class="sxs-lookup"><span data-stu-id="85f0a-143">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="85f0a-144">Kontrolovat aktuální útratu Azure</span><span class="sxs-lookup"><span data-stu-id="85f0a-144">Check current Azure spending</span></span>

<span data-ttu-id="85f0a-145">*Aktuální výdaje na Azure a měsíční rozpočty můžete sledovat* kdykoli:</span><span class="sxs-lookup"><span data-stu-id="85f0a-145">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="85f0a-146">Přihlaste se k [řídicímu panelu pro Partnerské centrum](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="85f0a-146">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="85f0a-147">V nabídce vlevo v části **CSP** vyberte **útraty Azure**.</span><span class="sxs-lookup"><span data-stu-id="85f0a-147">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="85f0a-148">Na stránce **útraty Azure** můžete v části **zákazníci s předplatnými Microsoft Azure** zobrazit přehled měsíčních rozpočtů zákazníků, aktuální odhady útraty a procento využití rozpočtu.</span><span class="sxs-lookup"><span data-stu-id="85f0a-148">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="85f0a-149">Oznámení pro limity rozpočtu</span><span class="sxs-lookup"><span data-stu-id="85f0a-149">Notifications for budget limits</span></span>

<span data-ttu-id="85f0a-150">*E-mailová oznámení můžete zapnout* , když se Měsíční útrata vašeho zákazníka blíží jejich limitu.</span><span class="sxs-lookup"><span data-stu-id="85f0a-150">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="85f0a-151">Když zapnete tuto možnost, budete upozorněni, když zákazníci použijí 80% nebo více jejich měsíčních rozpočtů.</span><span class="sxs-lookup"><span data-stu-id="85f0a-151">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="85f0a-152">Tato možnost vám pomůže udržet si přehled o fakturaci Azure.</span><span class="sxs-lookup"><span data-stu-id="85f0a-152">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="85f0a-153">Konfigurace e-mailových oznámení:</span><span class="sxs-lookup"><span data-stu-id="85f0a-153">To configure email notifications:</span></span>

1. <span data-ttu-id="85f0a-154">Přihlaste se do Partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="85f0a-154">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="85f0a-155">Přejít na **Nastavení**.</span><span class="sxs-lookup"><span data-stu-id="85f0a-155">Go to **Settings**.</span></span>

3. <span data-ttu-id="85f0a-156">Vyberte **moje předvolby**.</span><span class="sxs-lookup"><span data-stu-id="85f0a-156">Select **My preferences**.</span></span>

4. <span data-ttu-id="85f0a-157">Pokud jste neučinili, nakonfigurujte upřednostňovanou e-mailovou adresu.</span><span class="sxs-lookup"><span data-stu-id="85f0a-157">Configure a preferred email address if you haven't.</span></span>

5. <span data-ttu-id="85f0a-158">Nakonfigurujte preferovaný jazyk pro oznámení.</span><span class="sxs-lookup"><span data-stu-id="85f0a-158">Configure the preferred language for the notification.</span></span>

6. <span data-ttu-id="85f0a-159">V části **předvolby oznámení** vyberte kartu **CSP** .</span><span class="sxs-lookup"><span data-stu-id="85f0a-159">Select **CSP** tab under **Notification preferences** section.</span></span>

7. <span data-ttu-id="85f0a-160">Podívejte se na E-mail s oznámením o **útratách Azure** a **uložte** ho.</span><span class="sxs-lookup"><span data-stu-id="85f0a-160">Check the Email option for **Azure Spending** notification, and **Save**.</span></span>


## <a name="itemized-costs-by-service"></a><span data-ttu-id="85f0a-161">Vynásobené náklady podle služby</span><span class="sxs-lookup"><span data-stu-id="85f0a-161">Itemized costs by service</span></span>

<span data-ttu-id="85f0a-162">*Podle služby můžete u předplatných založených na využití zobrazit náklady na zboží (a Odhadované využití)*:</span><span class="sxs-lookup"><span data-stu-id="85f0a-162">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="85f0a-163">Přihlaste se do Partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="85f0a-163">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="85f0a-164">V nabídce vlevo v části **CSP** vyberte **zákazníci**.</span><span class="sxs-lookup"><span data-stu-id="85f0a-164">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="85f0a-165">Na stránce **Customers (zákazníci** ) vyberte **název společnosti** zákazníka.</span><span class="sxs-lookup"><span data-stu-id="85f0a-165">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="85f0a-166">Na stránce **předplatná** zákazníka v části **předplatná na základě využití** vyberte název **předplatného**.</span><span class="sxs-lookup"><span data-stu-id="85f0a-166">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="85f0a-167">Na stránce předplatného můžete zkontrolovat **náklady na zboží** podle služby a **Odhadované využití** aktuálního měsíce.</span><span class="sxs-lookup"><span data-stu-id="85f0a-167">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>


## <a name="next-steps"></a><span data-ttu-id="85f0a-168">Další kroky</span><span class="sxs-lookup"><span data-stu-id="85f0a-168">Next steps</span></span>

- [<span data-ttu-id="85f0a-169">Nové obchodní prostředí v CSP – Fakturace Azure</span><span class="sxs-lookup"><span data-stu-id="85f0a-169">New commerce experience in CSP - Azure billing</span></span>](azure-plan-billing.md)
