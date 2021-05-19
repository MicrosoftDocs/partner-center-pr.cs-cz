---
title: Výpočet efektivní jednotkové ceny
ms.topic: how-to
ms.date: 04/02/2021
description: Přečtěte si o efektivní jednotkové ceně a o tom, jak se počítá. Tento článek obsahuje také ukázkový výpočet.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 84beac77d41b8c11be9ac3cad87460eec9632ac4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147118"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="06374-104">Výpočet efektivní jednotkové ceny pro spotřebu plánu Azure</span><span class="sxs-lookup"><span data-stu-id="06374-104">Effective unit price calculation for Azure plan consumption</span></span>

<span data-ttu-id="06374-105">**Odpovídající role:** Správce fakturace</span><span class="sxs-lookup"><span data-stu-id="06374-105">**Appropriate roles**: Billing admin</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="06374-106">Efektivní jednotková cena</span><span class="sxs-lookup"><span data-stu-id="06374-106">The effective unit price</span></span>

<span data-ttu-id="06374-107">Efektivní jednotková cena se počítá na úrovni měřiče (na rozdíl od úrovně prostředků) a každý den se upravuje podle využití měřiče.</span><span class="sxs-lookup"><span data-stu-id="06374-107">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="06374-108">Efektivní jednotkovou cenu vypočítáme pomocí následujících tří faktorů:</span><span class="sxs-lookup"><span data-stu-id="06374-108">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="06374-109">Spotřeba, která se monitoruje každý den v průběhu fakturačního cyklu</span><span class="sxs-lookup"><span data-stu-id="06374-109">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="06374-110">Fakturovatelné náklady na měřič</span><span class="sxs-lookup"><span data-stu-id="06374-110">Billable cost for the meter</span></span>
- <span data-ttu-id="06374-111">Vrstvení (pokud je to dostupné)</span><span class="sxs-lookup"><span data-stu-id="06374-111">Tiering (if applicable)</span></span>

<span data-ttu-id="06374-112">Vzhledem k tomu, že spotřebu sledujeme každý den v průběhu fakturačního cyklu, bude efektivní jednotková cena kolísá.</span><span class="sxs-lookup"><span data-stu-id="06374-112">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="06374-113">Konečná cena za dané fakturační období bude k dispozici po zastavení výpočtu spotřeby a uzavření fakturačního období.</span><span class="sxs-lookup"><span data-stu-id="06374-113">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="06374-114">Většinu změn spotřeby uvidíte po čtvrtém nebo pátém desetinném místě.</span><span class="sxs-lookup"><span data-stu-id="06374-114">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="06374-115">Zjistěte, jestli váš měřič používá vrstvené ceny.</span><span class="sxs-lookup"><span data-stu-id="06374-115">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="06374-116">Pokud nevíte, jestli váš měřič používá vrstvené ceny, zjistěte to pomocí následujícího postupu.</span><span class="sxs-lookup"><span data-stu-id="06374-116">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="06374-117">Přihlaste se k [řídicímu panelu pro Partnerské centrum](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="06374-117">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="06374-118">Vyberte **Sell (Prodej),** **vyberte Pricing and offers (Ceny** a nabídky) a pak vyberte **Azure Plan pricing (Ceny plánu Azure).**</span><span class="sxs-lookup"><span data-stu-id="06374-118">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="06374-119">Vyhledejte měřič podle ID a stáhněte si data o cenách.</span><span class="sxs-lookup"><span data-stu-id="06374-119">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="06374-120">Ukázkový výpočet</span><span class="sxs-lookup"><span data-stu-id="06374-120">Sample calculation</span></span>

<span data-ttu-id="06374-121">Následující tabulka uvádí příklad, jak vypočítáme efektivní jednotkovou cenu během otevřeného období.</span><span class="sxs-lookup"><span data-stu-id="06374-121">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="06374-122">V tabulce platí následující hodnoty:</span><span class="sxs-lookup"><span data-stu-id="06374-122">In the table, the following values apply:</span></span> 

- <span data-ttu-id="06374-123">**UP** = jednotková cena prostředku za hodinu = 0,868</span><span class="sxs-lookup"><span data-stu-id="06374-123">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="06374-124">**BCU** = fakturovatelná jednotka spotřeby měřiče</span><span class="sxs-lookup"><span data-stu-id="06374-124">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="06374-125">**BC** = fakturovatelné náklady na měřič = BCU \* UP \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="06374-125">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="06374-126">To odráží úpravu pro 15% slevu PEC.</span><span class="sxs-lookup"><span data-stu-id="06374-126">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="06374-127">Potom použijeme dolní limit funkce k omezení hodnoty na dvě číslice za desetinnou čárkou, aby bylo možné účtovat minimální částku.</span><span class="sxs-lookup"><span data-stu-id="06374-127">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="06374-128">**Efektivní jednotková cena** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="06374-128">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]

><span data-ttu-id="06374-129">Poznámka: Měřič v tomto příkladu nemá úrovně v cenách ani jiných slevách – efektivní jednotková cena bere v úvahu procentuální slevy a další úpravy.</span><span class="sxs-lookup"><span data-stu-id="06374-129">Note: The meter in this example does not have tiers in pricing or other discounts—the Effective Unit Price factors in discount percentages and other adjustments.</span></span>


| <span data-ttu-id="06374-130">Date (Datum)</span><span class="sxs-lookup"><span data-stu-id="06374-130">Date</span></span> | <span data-ttu-id="06374-131">BCU (fakturovatelná jednotka spotřeby)</span><span class="sxs-lookup"><span data-stu-id="06374-131">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="06374-132">BC (fakturovatelné náklady)</span><span class="sxs-lookup"><span data-stu-id="06374-132">BC (Billable cost)</span></span> | <span data-ttu-id="06374-133">Efektivní jednotková cena</span><span class="sxs-lookup"><span data-stu-id="06374-133">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="06374-134">3.8.</span><span class="sxs-lookup"><span data-stu-id="06374-134">3-Aug</span></span> | <span data-ttu-id="06374-135">29</span><span class="sxs-lookup"><span data-stu-id="06374-135">29</span></span> | <span data-ttu-id="06374-136">21.39</span><span class="sxs-lookup"><span data-stu-id="06374-136">21.39</span></span> | <span data-ttu-id="06374-137">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="06374-137">0.737586206896552</span></span> |
| <span data-ttu-id="06374-138">10. srpna</span><span class="sxs-lookup"><span data-stu-id="06374-138">10-Aug</span></span> | <span data-ttu-id="06374-139">210.950039</span><span class="sxs-lookup"><span data-stu-id="06374-139">210.950039</span></span> | <span data-ttu-id="06374-140">155.63</span><span class="sxs-lookup"><span data-stu-id="06374-140">155.63</span></span> | <span data-ttu-id="06374-141">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="06374-141">0.737757626107858</span></span> |
| <span data-ttu-id="06374-142">25. srpna</span><span class="sxs-lookup"><span data-stu-id="06374-142">25-Aug</span></span> | <span data-ttu-id="06374-143">555.950039</span><span class="sxs-lookup"><span data-stu-id="06374-143">555.950039</span></span> | <span data-ttu-id="06374-144">410.17</span><span class="sxs-lookup"><span data-stu-id="06374-144">410.17</span></span> | <span data-ttu-id="06374-145">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="06374-145">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="06374-146">Další kroky</span><span class="sxs-lookup"><span data-stu-id="06374-146">Next steps</span></span>

- [<span data-ttu-id="06374-147">Fakturace a daně</span><span class="sxs-lookup"><span data-stu-id="06374-147">Billing and taxes</span></span>](billing.md)
