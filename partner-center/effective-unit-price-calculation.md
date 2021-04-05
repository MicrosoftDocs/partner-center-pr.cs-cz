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
ms.openlocfilehash: a662e0b815c979b3454762c5b35eb510887c96ad
ms.sourcegitcommit: c6c741475604b8daf386fb54bb2795a6445ac887
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/05/2021
ms.locfileid: "106374383"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="5e10e-104">Efektivní výpočet jednotkové ceny pro spotřebu plánu Azure</span><span class="sxs-lookup"><span data-stu-id="5e10e-104">Effective unit price calculation for Azure plan consumption</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="5e10e-105">Efektivní Jednotková cena</span><span class="sxs-lookup"><span data-stu-id="5e10e-105">The effective unit price</span></span>

<span data-ttu-id="5e10e-106">Platná Jednotková cena se vypočítá na úrovni měřiče (na rozdíl od úrovně prostředku) a v závislosti na využití měřiče se upraví každý den.</span><span class="sxs-lookup"><span data-stu-id="5e10e-106">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="5e10e-107">Platnou jednotkovou cenu vypočítáme pomocí následujících tří faktorů:</span><span class="sxs-lookup"><span data-stu-id="5e10e-107">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="5e10e-108">Spotřeba, která se denně monitoruje v průběhu fakturačního cyklu</span><span class="sxs-lookup"><span data-stu-id="5e10e-108">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="5e10e-109">Fakturovatelné náklady za měřič</span><span class="sxs-lookup"><span data-stu-id="5e10e-109">Billable cost for the meter</span></span>
- <span data-ttu-id="5e10e-110">Vrstvení (Pokud je k dispozici)</span><span class="sxs-lookup"><span data-stu-id="5e10e-110">Tiering (if applicable)</span></span>

<span data-ttu-id="5e10e-111">Vzhledem k tomu, že monitoruje denní spotřebu v průběhu fakturačního cyklu, efektivní Jednotková cena bude kolísat.</span><span class="sxs-lookup"><span data-stu-id="5e10e-111">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="5e10e-112">Konečná cena za daný fakturační cyklus bude k dispozici po zastavení výpočtu spotřeby a uzavření fakturačního období.</span><span class="sxs-lookup"><span data-stu-id="5e10e-112">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="5e10e-113">Po čtvrtém nebo pátém desetinném místě uvidíte většinu změn v spotřebě.</span><span class="sxs-lookup"><span data-stu-id="5e10e-113">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="5e10e-114">Zjistěte, jestli měřič používá vrstvené ceny.</span><span class="sxs-lookup"><span data-stu-id="5e10e-114">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="5e10e-115">Pokud si nejste jistí, jestli měřič používá vrstvené ceny, najděte pomocí níže uvedeného postupu.</span><span class="sxs-lookup"><span data-stu-id="5e10e-115">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="5e10e-116">Přihlaste se k [řídicímu panelu pro Partnerské centrum](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="5e10e-116">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="5e10e-117">Vyberte **prodávat**, vyberte **ceny a nabídky** a pak vyberte **ceny plánu Azure**.</span><span class="sxs-lookup"><span data-stu-id="5e10e-117">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="5e10e-118">Vyhledejte měřič podle ID a Stáhněte si data o cenách.</span><span class="sxs-lookup"><span data-stu-id="5e10e-118">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="5e10e-119">Ukázkový výpočet</span><span class="sxs-lookup"><span data-stu-id="5e10e-119">Sample calculation</span></span>

<span data-ttu-id="5e10e-120">V následující tabulce najdete příklad toho, jak vypočítat efektivní jednotkovou cenu během otevřeného období.</span><span class="sxs-lookup"><span data-stu-id="5e10e-120">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="5e10e-121">V tabulce platí následující hodnoty:</span><span class="sxs-lookup"><span data-stu-id="5e10e-121">In the table, the following values apply:</span></span> 

- <span data-ttu-id="5e10e-122">**Nahoru** = Jednotková cena prostředku/hodiny = 0,868</span><span class="sxs-lookup"><span data-stu-id="5e10e-122">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="5e10e-123">**BCU** = fakturovatelná jednotka spotřeby pro měřič</span><span class="sxs-lookup"><span data-stu-id="5e10e-123">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="5e10e-124">**BC** = Fakturovatelné náklady za měřič = BCU \* nahoru × 0,85.</span><span class="sxs-lookup"><span data-stu-id="5e10e-124">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="5e10e-125">To odráží úpravu pro 15% slevu PEC.</span><span class="sxs-lookup"><span data-stu-id="5e10e-125">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="5e10e-126">Pak použijeme spodní limit funkce k omezení hodnoty na dvě číslice za desetinnou čárkou, aby se využívala minimální částka.</span><span class="sxs-lookup"><span data-stu-id="5e10e-126">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="5e10e-127">**Efektivní Jednotková cena** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="5e10e-127">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]
><span data-ttu-id="5e10e-128">Měřidlo v tomto příkladu nemá v ceně žádné úrovně.</span><span class="sxs-lookup"><span data-stu-id="5e10e-128">The meter in this example does not have tiers in pricing.</span></span> <span data-ttu-id="5e10e-129">Efektivní faktory jednotkové ceny v procentech slevy a dalších úpravách.</span><span class="sxs-lookup"><span data-stu-id="5e10e-129">The Effective Unit Price factors in discount percentages and other adjustments.</span></span>

| <span data-ttu-id="5e10e-130">Date (Datum)</span><span class="sxs-lookup"><span data-stu-id="5e10e-130">Date</span></span> | <span data-ttu-id="5e10e-131">BCU (jednotka fakturovatelných spotřeby)</span><span class="sxs-lookup"><span data-stu-id="5e10e-131">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="5e10e-132">BC (Fakturovatelné náklady)</span><span class="sxs-lookup"><span data-stu-id="5e10e-132">BC (Billable cost)</span></span> | <span data-ttu-id="5e10e-133">Efektivní Jednotková cena</span><span class="sxs-lookup"><span data-stu-id="5e10e-133">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="5e10e-134">3. srpna</span><span class="sxs-lookup"><span data-stu-id="5e10e-134">3-Aug</span></span> | <span data-ttu-id="5e10e-135">29</span><span class="sxs-lookup"><span data-stu-id="5e10e-135">29</span></span> | <span data-ttu-id="5e10e-136">21,39</span><span class="sxs-lookup"><span data-stu-id="5e10e-136">21.39</span></span> | <span data-ttu-id="5e10e-137">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="5e10e-137">0.737586206896552</span></span> |
| <span data-ttu-id="5e10e-138">10. srpna</span><span class="sxs-lookup"><span data-stu-id="5e10e-138">10-Aug</span></span> | <span data-ttu-id="5e10e-139">210,950039</span><span class="sxs-lookup"><span data-stu-id="5e10e-139">210.950039</span></span> | <span data-ttu-id="5e10e-140">155,63</span><span class="sxs-lookup"><span data-stu-id="5e10e-140">155.63</span></span> | <span data-ttu-id="5e10e-141">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="5e10e-141">0.737757626107858</span></span> |
| <span data-ttu-id="5e10e-142">25. srpna</span><span class="sxs-lookup"><span data-stu-id="5e10e-142">25-Aug</span></span> | <span data-ttu-id="5e10e-143">555,950039</span><span class="sxs-lookup"><span data-stu-id="5e10e-143">555.950039</span></span> | <span data-ttu-id="5e10e-144">410,17</span><span class="sxs-lookup"><span data-stu-id="5e10e-144">410.17</span></span> | <span data-ttu-id="5e10e-145">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="5e10e-145">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="5e10e-146">Další kroky</span><span class="sxs-lookup"><span data-stu-id="5e10e-146">Next steps</span></span>

- [<span data-ttu-id="5e10e-147">Fakturace a daně</span><span class="sxs-lookup"><span data-stu-id="5e10e-147">Billing and taxes</span></span>](billing.md)
