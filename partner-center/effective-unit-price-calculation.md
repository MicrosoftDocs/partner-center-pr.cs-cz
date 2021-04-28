---
title: Výpočet efektivní jednotkové ceny
ms.topic: how-to
ms.date: 04/02/2021
description: Přečtěte si o efektivní jednotkové ceně a způsobu jejich výpočtu. Tento článek obsahuje také ukázkový výpočet.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1473b3c0b90cca1152b4dab0b8efec86dbc3d22d
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172213"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="7341c-104">Efektivní výpočet jednotkové ceny pro spotřebu plánu Azure</span><span class="sxs-lookup"><span data-stu-id="7341c-104">Effective unit price calculation for Azure plan consumption</span></span>

<span data-ttu-id="7341c-105">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="7341c-105">**Appropriate roles**</span></span>

- <span data-ttu-id="7341c-106">Správce fakturace</span><span class="sxs-lookup"><span data-stu-id="7341c-106">Billing admin</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="7341c-107">Efektivní Jednotková cena</span><span class="sxs-lookup"><span data-stu-id="7341c-107">The effective unit price</span></span>

<span data-ttu-id="7341c-108">Platná Jednotková cena se vypočítá na úrovni měřiče (na rozdíl od úrovně prostředku) a v závislosti na využití měřiče se upraví každý den.</span><span class="sxs-lookup"><span data-stu-id="7341c-108">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="7341c-109">Platnou jednotkovou cenu vypočítáme pomocí následujících tří faktorů:</span><span class="sxs-lookup"><span data-stu-id="7341c-109">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="7341c-110">Spotřeba, která se denně monitoruje v průběhu fakturačního cyklu</span><span class="sxs-lookup"><span data-stu-id="7341c-110">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="7341c-111">Fakturovatelné náklady za měřič</span><span class="sxs-lookup"><span data-stu-id="7341c-111">Billable cost for the meter</span></span>
- <span data-ttu-id="7341c-112">Vrstvení (Pokud je k dispozici)</span><span class="sxs-lookup"><span data-stu-id="7341c-112">Tiering (if applicable)</span></span>

<span data-ttu-id="7341c-113">Vzhledem k tomu, že monitoruje denní spotřebu v průběhu fakturačního cyklu, efektivní Jednotková cena bude kolísat.</span><span class="sxs-lookup"><span data-stu-id="7341c-113">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="7341c-114">Konečná cena za daný fakturační cyklus bude k dispozici po zastavení výpočtu spotřeby a uzavření fakturačního období.</span><span class="sxs-lookup"><span data-stu-id="7341c-114">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="7341c-115">Po čtvrtém nebo pátém desetinném místě uvidíte většinu změn v spotřebě.</span><span class="sxs-lookup"><span data-stu-id="7341c-115">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="7341c-116">Zjistěte, jestli měřič používá vrstvené ceny.</span><span class="sxs-lookup"><span data-stu-id="7341c-116">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="7341c-117">Pokud si nejste jistí, jestli měřič používá vrstvené ceny, najděte pomocí níže uvedeného postupu.</span><span class="sxs-lookup"><span data-stu-id="7341c-117">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="7341c-118">Přihlaste se k [řídicímu panelu pro Partnerské centrum](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="7341c-118">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="7341c-119">Vyberte **prodávat**, vyberte **ceny a nabídky** a pak vyberte **ceny plánu Azure**.</span><span class="sxs-lookup"><span data-stu-id="7341c-119">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="7341c-120">Vyhledejte měřič podle ID a Stáhněte si data o cenách.</span><span class="sxs-lookup"><span data-stu-id="7341c-120">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="7341c-121">Ukázkový výpočet</span><span class="sxs-lookup"><span data-stu-id="7341c-121">Sample calculation</span></span>

<span data-ttu-id="7341c-122">V následující tabulce najdete příklad toho, jak vypočítat efektivní jednotkovou cenu během otevřeného období.</span><span class="sxs-lookup"><span data-stu-id="7341c-122">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="7341c-123">V tabulce platí následující hodnoty:</span><span class="sxs-lookup"><span data-stu-id="7341c-123">In the table, the following values apply:</span></span> 

- <span data-ttu-id="7341c-124">**Nahoru** = Jednotková cena prostředku/hodiny = 0,868</span><span class="sxs-lookup"><span data-stu-id="7341c-124">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="7341c-125">**BCU** = fakturovatelná jednotka spotřeby pro měřič</span><span class="sxs-lookup"><span data-stu-id="7341c-125">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="7341c-126">**BC** = Fakturovatelné náklady za měřič = BCU \* nahoru × 0,85.</span><span class="sxs-lookup"><span data-stu-id="7341c-126">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="7341c-127">To odráží úpravu pro 15% slevu PEC.</span><span class="sxs-lookup"><span data-stu-id="7341c-127">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="7341c-128">Pak použijeme spodní limit funkce k omezení hodnoty na dvě číslice za desetinnou čárkou, aby se využívala minimální částka.</span><span class="sxs-lookup"><span data-stu-id="7341c-128">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="7341c-129">**Efektivní Jednotková cena** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="7341c-129">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]

><span data-ttu-id="7341c-130">Poznámka: měřič v tomto příkladu nemá úrovně v cenách nebo jiných slevách – efektivní faktory pro ceny za jednotku v procentech slevy a další úpravy.</span><span class="sxs-lookup"><span data-stu-id="7341c-130">Note: The meter in this example does not have tiers in pricing or other discounts—the Effective Unit Price factors in discount percentages and other adjustments.</span></span>


| <span data-ttu-id="7341c-131">Date (Datum)</span><span class="sxs-lookup"><span data-stu-id="7341c-131">Date</span></span> | <span data-ttu-id="7341c-132">BCU (jednotka fakturovatelných spotřeby)</span><span class="sxs-lookup"><span data-stu-id="7341c-132">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="7341c-133">BC (Fakturovatelné náklady)</span><span class="sxs-lookup"><span data-stu-id="7341c-133">BC (Billable cost)</span></span> | <span data-ttu-id="7341c-134">Efektivní Jednotková cena</span><span class="sxs-lookup"><span data-stu-id="7341c-134">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="7341c-135">3. srpna</span><span class="sxs-lookup"><span data-stu-id="7341c-135">3-Aug</span></span> | <span data-ttu-id="7341c-136">29</span><span class="sxs-lookup"><span data-stu-id="7341c-136">29</span></span> | <span data-ttu-id="7341c-137">21,39</span><span class="sxs-lookup"><span data-stu-id="7341c-137">21.39</span></span> | <span data-ttu-id="7341c-138">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="7341c-138">0.737586206896552</span></span> |
| <span data-ttu-id="7341c-139">10. srpna</span><span class="sxs-lookup"><span data-stu-id="7341c-139">10-Aug</span></span> | <span data-ttu-id="7341c-140">210,950039</span><span class="sxs-lookup"><span data-stu-id="7341c-140">210.950039</span></span> | <span data-ttu-id="7341c-141">155,63</span><span class="sxs-lookup"><span data-stu-id="7341c-141">155.63</span></span> | <span data-ttu-id="7341c-142">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="7341c-142">0.737757626107858</span></span> |
| <span data-ttu-id="7341c-143">25. srpna</span><span class="sxs-lookup"><span data-stu-id="7341c-143">25-Aug</span></span> | <span data-ttu-id="7341c-144">555,950039</span><span class="sxs-lookup"><span data-stu-id="7341c-144">555.950039</span></span> | <span data-ttu-id="7341c-145">410,17</span><span class="sxs-lookup"><span data-stu-id="7341c-145">410.17</span></span> | <span data-ttu-id="7341c-146">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="7341c-146">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="7341c-147">Další kroky</span><span class="sxs-lookup"><span data-stu-id="7341c-147">Next steps</span></span>

- [<span data-ttu-id="7341c-148">Fakturace a daně</span><span class="sxs-lookup"><span data-stu-id="7341c-148">Billing and taxes</span></span>](billing.md)
