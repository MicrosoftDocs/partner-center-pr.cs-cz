---
title: Nastavení rozpočtu Azure útraty pro zákazníky
ms.topic: how-to
ms.date: 06/03/2020
description: Naučte se, jak nastavit nebo odebrat měsíční rozpočty Azure útraty pro vaše zákazníky, a také zobrazit data o výdajích Azure a nastavit oznámení týkající se rozpočtu.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e311af31bbce65ed38c20df12243d325c7a63d04
ms.sourcegitcommit: 7beb7327472dc1b0c07c101d121196fb2830bbf8
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/01/2020
ms.locfileid: "96438988"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="26938-103">Nastavení, kontrolu nebo odebrání měsíčních rozpočtů Azure útraty pro zákazníky v partnerském centru</span><span class="sxs-lookup"><span data-stu-id="26938-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="26938-104">Platí pro:</span><span class="sxs-lookup"><span data-stu-id="26938-104">Applies to:</span></span>

- <span data-ttu-id="26938-105">Partnerské centrum</span><span class="sxs-lookup"><span data-stu-id="26938-105">Partner Center</span></span>
- <span data-ttu-id="26938-106">Partnerské centrum pro Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="26938-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="26938-107">Můžete [nastavit měsíční rozpočet Azure útraty pro vaše zákazníky](#set-azure-spending-budget) v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="26938-107">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="26938-108">To pomáhá vašim zákazníkům spravovat útraty Azure.</span><span class="sxs-lookup"><span data-stu-id="26938-108">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="26938-109">Tato možnost umožňuje porovnat náklady na Azure, které jsou v daném měsíci v rozpočtu.</span><span class="sxs-lookup"><span data-stu-id="26938-109">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="26938-110">Pomáhá zákazníkům také rozpočtovat své výdaje na Azure, takže jejich měsíční vyúčtování není vyšší než jejich předvídání.</span><span class="sxs-lookup"><span data-stu-id="26938-110">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="26938-111">Tato funkce není k dispozici v izolovaném prostoru nebo v produkčním účtu (TIP).</span><span class="sxs-lookup"><span data-stu-id="26938-111">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="26938-112">Po [nastavení rozpočtu útraty Azure pro zákazníky](#set-azure-spending-budget)můžete také zkontrolovat používání zákazníka následujícími způsoby.</span><span class="sxs-lookup"><span data-stu-id="26938-112">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="26938-113">Tyto možnosti vám mohou nabídnout možnost vyznačovat nesprávně nakonfigurované služby nebo neobvyklé trendy, které mohou navrhovat podvod.</span><span class="sxs-lookup"><span data-stu-id="26938-113">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="26938-114">Potom můžete s vašimi zákazníky spolupracovat a identifikovat hlavní příčinu a spravovat náklady.</span><span class="sxs-lookup"><span data-stu-id="26938-114">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="26938-115">V případě potřeby můžete také [změnit rozpočet zákazníka](#set-azure-spending-budget) na vyšší částku.</span><span class="sxs-lookup"><span data-stu-id="26938-115">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="26938-116">Kontrolovat aktuální útratu Azure</span><span class="sxs-lookup"><span data-stu-id="26938-116">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="26938-117">Zapnout e-mailová oznámení v případě, že se útrata zákazníka blíží ke svému limitu rozpočtu</span><span class="sxs-lookup"><span data-stu-id="26938-117">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="26938-118">Zobrazit nákladové náklady podle služby pro odběry založené na využití</span><span class="sxs-lookup"><span data-stu-id="26938-118">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="26938-119">[Rozpočet Azure útraty](#remove-azure-spending-budget) můžete také kdykoli odebrat pro zákazníky.</span><span class="sxs-lookup"><span data-stu-id="26938-119">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="26938-120">Data o výdajích Azure</span><span class="sxs-lookup"><span data-stu-id="26938-120">Azure spending data</span></span>

<span data-ttu-id="26938-121">Data o výdajích Azure jsou *odhadem* a *skutečné fakturační částky se můžou lišit*.</span><span class="sxs-lookup"><span data-stu-id="26938-121">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="26938-122">Hodnota dat *nezohledňuje* daně, kredity, úpravy nebo jiné poplatky, které mohou platit.</span><span class="sxs-lookup"><span data-stu-id="26938-122">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="26938-123">Data o výdajích se *aktualizují jednou denně*.</span><span class="sxs-lookup"><span data-stu-id="26938-123">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="26938-124">Vaši zákazníci můžou dál používat (a budou se vám účtovat) služby a prostředky Azure, pokud nezměníte nastavení svého účtu v Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="26938-124">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="26938-125">Nastavení rozpočtu útraty Azure</span><span class="sxs-lookup"><span data-stu-id="26938-125">Set Azure spending budget</span></span>

<span data-ttu-id="26938-126">Můžete *nastavit měsíční rozpočet Azure útraty* pro více zákazníků v partnerském centru:</span><span class="sxs-lookup"><span data-stu-id="26938-126">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="26938-127">Přihlaste se k [řídicímu panelu partnerského centra](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="26938-127">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="26938-128">V nabídce vlevo v části **CSP** vyberte **útraty Azure**.</span><span class="sxs-lookup"><span data-stu-id="26938-128">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="26938-129">Na stránce **útraty Azure** v části **zákazníci s předplatnými Microsoft Azure** vyberte zákazníky, pro které chcete nastavit rozpočet.</span><span class="sxs-lookup"><span data-stu-id="26938-129">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="26938-130">Zadejte hodnotu pro **měsíční rozpočet**.</span><span class="sxs-lookup"><span data-stu-id="26938-130">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="26938-131">Chcete-li uložit změny, klikněte na tlačítko **použít** .</span><span class="sxs-lookup"><span data-stu-id="26938-131">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="26938-132">Můžete také *nastavit rozpočet pro jednotlivé zákazníky* v nastavení jejich předplatného:</span><span class="sxs-lookup"><span data-stu-id="26938-132">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="26938-133">Přihlaste se k řídicímu panelu partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="26938-133">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="26938-134">V nabídce vlevo v části **CSP** vyberte **zákazníci**.</span><span class="sxs-lookup"><span data-stu-id="26938-134">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="26938-135">Na stránce **Customers (zákazníci** ) vyberte **název společnosti** zákazníka.</span><span class="sxs-lookup"><span data-stu-id="26938-135">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="26938-136">Na stránce **předplatná** zákazníka v části **předplatné na základě využití** vyberte **změnit rozpočet**.</span><span class="sxs-lookup"><span data-stu-id="26938-136">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="26938-137">Zadejte hodnotu pro rozpočet.</span><span class="sxs-lookup"><span data-stu-id="26938-137">Enter a value for the budget.</span></span>

6. <span data-ttu-id="26938-138">Chcete-li uložit změny, klikněte na tlačítko **použít** .</span><span class="sxs-lookup"><span data-stu-id="26938-138">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="26938-139">Odebrat rozpočet útraty Azure</span><span class="sxs-lookup"><span data-stu-id="26938-139">Remove Azure spending budget</span></span>

<span data-ttu-id="26938-140">*Měsíční rozpočet Azure útraty* můžete pro zákazníky v partnerském centru odebrat:</span><span class="sxs-lookup"><span data-stu-id="26938-140">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="26938-141">Přihlaste se k [řídicímu panelu partnerského centra](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="26938-141">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="26938-142">V nabídce vlevo v části **CSP** vyberte **útraty Azure**.</span><span class="sxs-lookup"><span data-stu-id="26938-142">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="26938-143">Na stránce **útraty Azure** v části **zákazníci s předplatnými Microsoft Azure** vyberte zákazníky, jejichž rozpočet chcete odebrat.</span><span class="sxs-lookup"><span data-stu-id="26938-143">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="26938-144">Vyberte možnost **Odebrat rozpočet**.</span><span class="sxs-lookup"><span data-stu-id="26938-144">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="26938-145">Kontrolovat aktuální útratu Azure</span><span class="sxs-lookup"><span data-stu-id="26938-145">Check current Azure spending</span></span>

<span data-ttu-id="26938-146">*Aktuální výdaje na Azure a měsíční rozpočty můžete sledovat* kdykoli:</span><span class="sxs-lookup"><span data-stu-id="26938-146">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="26938-147">Přihlaste se k [řídicímu panelu partnerského centra](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="26938-147">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="26938-148">V nabídce vlevo v části **CSP** vyberte **útraty Azure**.</span><span class="sxs-lookup"><span data-stu-id="26938-148">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="26938-149">Na stránce **útraty Azure** můžete v části **zákazníci s předplatnými Microsoft Azure** zobrazit přehled měsíčních rozpočtů zákazníků, aktuální odhady útraty a procento využití rozpočtu.</span><span class="sxs-lookup"><span data-stu-id="26938-149">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="26938-150">Oznámení pro limity rozpočtu</span><span class="sxs-lookup"><span data-stu-id="26938-150">Notifications for budget limits</span></span>

<span data-ttu-id="26938-151">*E-mailová oznámení můžete zapnout* , když se Měsíční útrata vašeho zákazníka blíží jejich limitu.</span><span class="sxs-lookup"><span data-stu-id="26938-151">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="26938-152">Když zapnete tuto možnost, budete upozorněni, když zákazníci použijí 80% nebo více jejich měsíčních rozpočtů.</span><span class="sxs-lookup"><span data-stu-id="26938-152">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="26938-153">Tato možnost vám pomůže udržet si přehled o fakturaci Azure.</span><span class="sxs-lookup"><span data-stu-id="26938-153">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="26938-154">Konfigurace e-mailových oznámení:</span><span class="sxs-lookup"><span data-stu-id="26938-154">To configure email notifications:</span></span>

1. <span data-ttu-id="26938-155">Přihlaste se do Partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="26938-155">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="26938-156">Přejít na **Nastavení**.</span><span class="sxs-lookup"><span data-stu-id="26938-156">Go to **Settings**.</span></span>

3. <span data-ttu-id="26938-157">Vyberte **moje předvolby**.</span><span class="sxs-lookup"><span data-stu-id="26938-157">Select **My preferences**.</span></span>

4. <span data-ttu-id="26938-158">Pokud jste neučinili, nakonfigurujte upřednostňovanou e-mailovou adresu.</span><span class="sxs-lookup"><span data-stu-id="26938-158">Configure a preferred email address if you haven't.</span></span>

5. <span data-ttu-id="26938-159">Nakonfigurujte preferovaný jazyk pro oznámení.</span><span class="sxs-lookup"><span data-stu-id="26938-159">Configure the preferred language for the notification.</span></span>

6. <span data-ttu-id="26938-160">V části **předvolby oznámení** vyberte kartu **CSP** .</span><span class="sxs-lookup"><span data-stu-id="26938-160">Select **CSP** tab under **Notification preferences** section.</span></span>

7. <span data-ttu-id="26938-161">Podívejte se na E-mail s oznámením o **útratách Azure** a **uložte** ho.</span><span class="sxs-lookup"><span data-stu-id="26938-161">Check the Email option for **Azure Spending** notification, and **Save**.</span></span>


## <a name="itemized-costs-by-service"></a><span data-ttu-id="26938-162">Vynásobené náklady podle služby</span><span class="sxs-lookup"><span data-stu-id="26938-162">Itemized costs by service</span></span>

<span data-ttu-id="26938-163">*Podle služby můžete u předplatných založených na využití zobrazit náklady na zboží (a Odhadované využití)*:</span><span class="sxs-lookup"><span data-stu-id="26938-163">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="26938-164">Přihlaste se do Partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="26938-164">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="26938-165">V nabídce vlevo v části **CSP** vyberte **zákazníci**.</span><span class="sxs-lookup"><span data-stu-id="26938-165">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="26938-166">Na stránce **Customers (zákazníci** ) vyberte **název společnosti** zákazníka.</span><span class="sxs-lookup"><span data-stu-id="26938-166">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="26938-167">Na stránce **předplatná** zákazníka v části **předplatná na základě využití** vyberte název **předplatného**.</span><span class="sxs-lookup"><span data-stu-id="26938-167">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="26938-168">Na stránce předplatného můžete zkontrolovat **náklady na zboží** podle služby a **Odhadované využití** aktuálního měsíce.</span><span class="sxs-lookup"><span data-stu-id="26938-168">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>
