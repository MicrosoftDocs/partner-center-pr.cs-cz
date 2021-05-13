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
ms.openlocfilehash: 14e901f51841e58b28a3cbbb1b7a19ce89d7c324
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855348"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="1d448-103">Nastavení, kontrolu nebo odebrání měsíčních rozpočtů Azure útraty pro zákazníky v partnerském centru</span><span class="sxs-lookup"><span data-stu-id="1d448-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="1d448-104">**Příslušné role**: Agent správce</span><span class="sxs-lookup"><span data-stu-id="1d448-104">**Appropriate roles**: Admin agent</span></span>

<span data-ttu-id="1d448-105">Můžete [nastavit měsíční rozpočet Azure útraty pro vaše zákazníky](#set-azure-spending-budget) v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="1d448-105">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="1d448-106">To pomáhá vašim zákazníkům spravovat útraty Azure.</span><span class="sxs-lookup"><span data-stu-id="1d448-106">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="1d448-107">Tato možnost umožňuje porovnat náklady na Azure, které jsou v daném měsíci v rozpočtu.</span><span class="sxs-lookup"><span data-stu-id="1d448-107">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="1d448-108">Pomáhá zákazníkům také rozpočtovat své výdaje na Azure, takže jejich měsíční vyúčtování není vyšší než jejich předvídání.</span><span class="sxs-lookup"><span data-stu-id="1d448-108">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="1d448-109">Tato funkce není k dispozici v izolovaném prostoru nebo v produkčním účtu (TIP).</span><span class="sxs-lookup"><span data-stu-id="1d448-109">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="1d448-110">Po [nastavení rozpočtu útraty Azure pro zákazníky](#set-azure-spending-budget)můžete také zkontrolovat používání zákazníka následujícími způsoby.</span><span class="sxs-lookup"><span data-stu-id="1d448-110">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="1d448-111">Tyto možnosti vám mohou nabídnout možnost vyznačovat nesprávně nakonfigurované služby nebo neobvyklé trendy, které mohou navrhovat podvod.</span><span class="sxs-lookup"><span data-stu-id="1d448-111">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="1d448-112">Potom můžete s vašimi zákazníky spolupracovat a identifikovat hlavní příčinu a spravovat náklady.</span><span class="sxs-lookup"><span data-stu-id="1d448-112">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="1d448-113">V případě potřeby můžete také [změnit rozpočet zákazníka](#set-azure-spending-budget) na vyšší částku.</span><span class="sxs-lookup"><span data-stu-id="1d448-113">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="1d448-114">Kontrolovat aktuální útratu Azure</span><span class="sxs-lookup"><span data-stu-id="1d448-114">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="1d448-115">Zapnout e-mailová oznámení v případě, že se útrata zákazníka blíží ke svému limitu rozpočtu</span><span class="sxs-lookup"><span data-stu-id="1d448-115">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="1d448-116">Zobrazit nákladové náklady podle služby pro odběry založené na využití</span><span class="sxs-lookup"><span data-stu-id="1d448-116">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="1d448-117">[Rozpočet Azure útraty](#remove-azure-spending-budget) můžete také kdykoli odebrat pro zákazníky.</span><span class="sxs-lookup"><span data-stu-id="1d448-117">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="1d448-118">Data o výdajích Azure</span><span class="sxs-lookup"><span data-stu-id="1d448-118">Azure spending data</span></span>

<span data-ttu-id="1d448-119">Data o výdajích Azure jsou *odhadem* a *skutečné fakturační částky se můžou lišit*.</span><span class="sxs-lookup"><span data-stu-id="1d448-119">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="1d448-120">Hodnota dat *nezohledňuje* daně, kredity, úpravy nebo jiné poplatky, které mohou platit.</span><span class="sxs-lookup"><span data-stu-id="1d448-120">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="1d448-121">Data o výdajích se *aktualizují jednou denně*.</span><span class="sxs-lookup"><span data-stu-id="1d448-121">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="1d448-122">Vaši zákazníci mohou dál používat (a budou se jim účtovat) služby a prostředky Azure, pokud nezměníte jejich nastavení účtu v Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="1d448-122">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="1d448-123">Nastavení rozpočtu na útratu v Azure</span><span class="sxs-lookup"><span data-stu-id="1d448-123">Set Azure spending budget</span></span>

<span data-ttu-id="1d448-124">Můžete nastavit *měsíční rozpočet útraty za Azure* pro více zákazníků v Partnerské centrum:</span><span class="sxs-lookup"><span data-stu-id="1d448-124">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="1d448-125">Přihlaste se k [řídicímu panelu pro Partnerské centrum](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="1d448-125">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="1d448-126">V nabídce vlevo v části **CSP** zvolte **Útratu v Azure.**</span><span class="sxs-lookup"><span data-stu-id="1d448-126">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="1d448-127">Na stránce **Útraty** Azure v části Zákazníci **Microsoft Azure předplatných** vyberte zákazníka, pro kterého chcete nastavit rozpočet.</span><span class="sxs-lookup"><span data-stu-id="1d448-127">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="1d448-128">Zadejte hodnotu **měsíčního rozpočtu**.</span><span class="sxs-lookup"><span data-stu-id="1d448-128">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="1d448-129">Zvolte **Použít a** uložte změny.</span><span class="sxs-lookup"><span data-stu-id="1d448-129">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="1d448-130">Rozpočet pro *jednotlivé zákazníky můžete také* nastavit v nastavení předplatného:</span><span class="sxs-lookup"><span data-stu-id="1d448-130">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="1d448-131">Přihlaste se k řídicímu panelu pro Partnerské centrum.</span><span class="sxs-lookup"><span data-stu-id="1d448-131">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="1d448-132">V nabídce vlevo v části **CSP** zvolte **Zákazníci.**</span><span class="sxs-lookup"><span data-stu-id="1d448-132">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="1d448-133">Na **stránce** Zákazníci vyberte název společnosti **zákazníka.**</span><span class="sxs-lookup"><span data-stu-id="1d448-133">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="1d448-134">Na stránce **Předplatná** zákazníka v části **Předplatné na** základě využití zvolte **Změnit rozpočet.**</span><span class="sxs-lookup"><span data-stu-id="1d448-134">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="1d448-135">Zadejte hodnotu rozpočtu.</span><span class="sxs-lookup"><span data-stu-id="1d448-135">Enter a value for the budget.</span></span>

6. <span data-ttu-id="1d448-136">Zvolte **Použít a** uložte změny.</span><span class="sxs-lookup"><span data-stu-id="1d448-136">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="1d448-137">Odebrání rozpočtu na útratu v Azure</span><span class="sxs-lookup"><span data-stu-id="1d448-137">Remove Azure spending budget</span></span>

<span data-ttu-id="1d448-138">Měsíční *rozpočet útraty zákazníků v Azure* můžete odebrat v Partnerské centrum:</span><span class="sxs-lookup"><span data-stu-id="1d448-138">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="1d448-139">Přihlaste se k [řídicímu panelu pro Partnerské centrum](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="1d448-139">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="1d448-140">V nabídce vlevo v části **CSP** zvolte **Útratu v Azure.**</span><span class="sxs-lookup"><span data-stu-id="1d448-140">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="1d448-141">Na stránce **Útraty Azure** v části Zákazníci **Microsoft Azure předplatných** vyberte zákazníka, jehož rozpočet chcete odebrat.</span><span class="sxs-lookup"><span data-stu-id="1d448-141">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="1d448-142">Zvolte **Odebrat rozpočet.**</span><span class="sxs-lookup"><span data-stu-id="1d448-142">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="1d448-143">Kontrola aktuální útraty za Azure</span><span class="sxs-lookup"><span data-stu-id="1d448-143">Check current Azure spending</span></span>

<span data-ttu-id="1d448-144">Aktuální *útraty zákazníků v Azure* a měsíční rozpočty můžete kdykoli sledovat:</span><span class="sxs-lookup"><span data-stu-id="1d448-144">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="1d448-145">Přihlaste se k [řídicímu panelu pro Partnerské centrum](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="1d448-145">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="1d448-146">V nabídce vlevo v části **CSP** vyberte **útraty Azure**.</span><span class="sxs-lookup"><span data-stu-id="1d448-146">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="1d448-147">Na stránce **útraty Azure** můžete v části **zákazníci s předplatnými Microsoft Azure** zobrazit přehled měsíčních rozpočtů zákazníků, aktuální odhady útraty a procento využití rozpočtu.</span><span class="sxs-lookup"><span data-stu-id="1d448-147">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="1d448-148">Oznámení pro limity rozpočtu</span><span class="sxs-lookup"><span data-stu-id="1d448-148">Notifications for budget limits</span></span>

<span data-ttu-id="1d448-149">*E-mailová oznámení můžete zapnout* , když se Měsíční útrata vašeho zákazníka blíží jejich limitu.</span><span class="sxs-lookup"><span data-stu-id="1d448-149">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="1d448-150">Když zapnete tuto možnost, budete upozorněni, když zákazníci použijí 80% nebo více jejich měsíčních rozpočtů.</span><span class="sxs-lookup"><span data-stu-id="1d448-150">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="1d448-151">Tato možnost vám pomůže udržet si přehled o fakturaci Azure.</span><span class="sxs-lookup"><span data-stu-id="1d448-151">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="1d448-152">Konfigurace e-mailových oznámení:</span><span class="sxs-lookup"><span data-stu-id="1d448-152">To configure email notifications:</span></span>

1. <span data-ttu-id="1d448-153">Přihlaste se do Partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="1d448-153">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="1d448-154">Přejít na **Nastavení**.</span><span class="sxs-lookup"><span data-stu-id="1d448-154">Go to **Settings**.</span></span>

3. <span data-ttu-id="1d448-155">Vyberte **moje předvolby**.</span><span class="sxs-lookup"><span data-stu-id="1d448-155">Select **My preferences**.</span></span>

4. <span data-ttu-id="1d448-156">Pokud jste neučinili, nakonfigurujte upřednostňovanou e-mailovou adresu.</span><span class="sxs-lookup"><span data-stu-id="1d448-156">Configure a preferred email address if you haven't.</span></span>

5. <span data-ttu-id="1d448-157">Nakonfigurujte preferovaný jazyk pro oznámení.</span><span class="sxs-lookup"><span data-stu-id="1d448-157">Configure the preferred language for the notification.</span></span>

6. <span data-ttu-id="1d448-158">V části **předvolby oznámení** vyberte kartu **CSP** .</span><span class="sxs-lookup"><span data-stu-id="1d448-158">Select **CSP** tab under **Notification preferences** section.</span></span>

7. <span data-ttu-id="1d448-159">Podívejte se na E-mail s oznámením o **útratách Azure** a **uložte** ho.</span><span class="sxs-lookup"><span data-stu-id="1d448-159">Check the Email option for **Azure Spending** notification, and **Save**.</span></span>


## <a name="itemized-costs-by-service"></a><span data-ttu-id="1d448-160">Vynásobené náklady podle služby</span><span class="sxs-lookup"><span data-stu-id="1d448-160">Itemized costs by service</span></span>

<span data-ttu-id="1d448-161">*Podle služby můžete u předplatných založených na využití zobrazit náklady na zboží (a Odhadované využití)*:</span><span class="sxs-lookup"><span data-stu-id="1d448-161">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="1d448-162">Přihlaste se do Partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="1d448-162">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="1d448-163">V nabídce vlevo v části **CSP** vyberte **zákazníci**.</span><span class="sxs-lookup"><span data-stu-id="1d448-163">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="1d448-164">Na stránce **Customers (zákazníci** ) vyberte **název společnosti** zákazníka.</span><span class="sxs-lookup"><span data-stu-id="1d448-164">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="1d448-165">Na stránce **předplatná** zákazníka v části **předplatná na základě využití** vyberte název **předplatného**.</span><span class="sxs-lookup"><span data-stu-id="1d448-165">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="1d448-166">Na stránce předplatného můžete zkontrolovat **náklady na zboží** podle služby a **Odhadované využití** aktuálního měsíce.</span><span class="sxs-lookup"><span data-stu-id="1d448-166">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>


## <a name="next-steps"></a><span data-ttu-id="1d448-167">Další kroky</span><span class="sxs-lookup"><span data-stu-id="1d448-167">Next steps</span></span>

- [<span data-ttu-id="1d448-168">Nové obchodní prostředí v CSP – Fakturace Azure</span><span class="sxs-lookup"><span data-stu-id="1d448-168">New commerce experience in CSP - Azure billing</span></span>](azure-plan-billing.md)
