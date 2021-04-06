---
title: Typy poplatků v souborech s vyrovnáním
ms.topic: article
ms.date: 06/05/2020
description: Seznamte se s typy poplatků (jako jsou založené na licencích a na základě využití a jednorázové), kredity a slevy v souborech pro odsouhlasení partnerského centra.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f1fb7fdcc4ec56f0d5cf0eb26b62294235a5b908
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441589"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="7fb46-103">Pochopení různých typů poplatků v souborech pro odsouhlasení partnerského centra</span><span class="sxs-lookup"><span data-stu-id="7fb46-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="7fb46-104">**Platí pro**</span><span class="sxs-lookup"><span data-stu-id="7fb46-104">**Applies to**</span></span>

- <span data-ttu-id="7fb46-105">Partnerské centrum pro Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="7fb46-105">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="7fb46-106">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="7fb46-106">**Appropriate roles**</span></span>

- <span data-ttu-id="7fb46-107">Agent správce</span><span class="sxs-lookup"><span data-stu-id="7fb46-107">Admin agent</span></span>
- <span data-ttu-id="7fb46-108">Správce fakturace</span><span class="sxs-lookup"><span data-stu-id="7fb46-108">Billing admin</span></span>
- <span data-ttu-id="7fb46-109">Globální správce</span><span class="sxs-lookup"><span data-stu-id="7fb46-109">Global admin</span></span>

<span data-ttu-id="7fb46-110">Tento článek popisuje mapování mezi oddílem faktury a typy přidružených poplatků, které mohou být na vašem souboru pro odsouhlasení.</span><span class="sxs-lookup"><span data-stu-id="7fb46-110">This article describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="7fb46-111">Vaše faktura poskytuje souhrn poplatků.</span><span class="sxs-lookup"><span data-stu-id="7fb46-111">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="7fb46-112">Váš soubor pro odsouhlasení poskytuje podrobný rozpis transakcí položek řádků, včetně typů poplatků.</span><span class="sxs-lookup"><span data-stu-id="7fb46-112">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="7fb46-113">Další informace o souborech pro odsouhlasení najdete v tématu [Jak používat soubory pro odsouhlasení](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="7fb46-113">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="7fb46-114">[Soubory odsouhlasení založené na použití](usage-based-recon-files.md) a [soubory odsouhlasení založené na licencích](license-based-recon-files.md) zobrazují jenom transakce a poplatky související s využitím (spotřebované jednotky a související poplatky).</span><span class="sxs-lookup"><span data-stu-id="7fb46-114">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="7fb46-115">Jednorázové kredity, slevy nebo refundace, které se zobrazí na faktuře jako **Úpravy** , se v souboru pro odsouhlasení nezobrazují.</span><span class="sxs-lookup"><span data-stu-id="7fb46-115">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="7fb46-116">Mapování typů nákladů na faktury</span><span class="sxs-lookup"><span data-stu-id="7fb46-116">Map charge types to invoice charges</span></span>

<span data-ttu-id="7fb46-117">Chcete-li náklady na křížové odkazy mezi vaším souborem faktury a odsouhlasení, použijte možnosti filtru v aplikaci Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="7fb46-117">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="7fb46-118">Filtrovat poplatky za fakturu na sadu rozdělení poplatků v souboru odsouhlasení podle typu poplatků za poplatek.</span><span class="sxs-lookup"><span data-stu-id="7fb46-118">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="7fb46-119">Poplatky na základě licencí</span><span class="sxs-lookup"><span data-stu-id="7fb46-119">License-based charges</span></span>

<span data-ttu-id="7fb46-120">Chcete-li namapovat tyto poplatky na základě licencí na fakturu, sečtěte sloupec **částky** ze souboru založeného na licencích.</span><span class="sxs-lookup"><span data-stu-id="7fb46-120">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="7fb46-121">Popis poplatku (sloupec ChargeType v souboru pro odsouhlasení)</span><span class="sxs-lookup"><span data-stu-id="7fb46-121">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="7fb46-122">Vysvětlení poplatků</span><span class="sxs-lookup"><span data-stu-id="7fb46-122">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="7fb46-123">Aktivační poplatek</span><span class="sxs-lookup"><span data-stu-id="7fb46-123">Activation fee</span></span> | <span data-ttu-id="7fb46-124">Částka, která se účtuje zákazníkovi při použití předplatného po nákupu</span><span class="sxs-lookup"><span data-stu-id="7fb46-124">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="7fb46-125">Zrušit poplatek</span><span class="sxs-lookup"><span data-stu-id="7fb46-125">Cancel fee</span></span> | <span data-ttu-id="7fb46-126">Poměrné náklady se účtují zákazníkovi při změně přidružených licencí.</span><span class="sxs-lookup"><span data-stu-id="7fb46-126">Prorated charges refunded to the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="7fb46-127">Zrušit poměr instancí</span><span class="sxs-lookup"><span data-stu-id="7fb46-127">Cancel instance prorate</span></span> | <span data-ttu-id="7fb46-128">Poměrné poplatky se zrušily, když zákazník s měsíčním předplatným má předplatné pozastaveno a přidružené licence se v rámci stejného měsíce změnily.</span><span class="sxs-lookup"><span data-stu-id="7fb46-128">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated licenses changed within the same month.</span></span> |
| <span data-ttu-id="7fb46-129">Poplatek za cyklus</span><span class="sxs-lookup"><span data-stu-id="7fb46-129">Cycle fee</span></span> | <span data-ttu-id="7fb46-130">Pravidelné poplatky za předplatné</span><span class="sxs-lookup"><span data-stu-id="7fb46-130">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="7fb46-131">Poměr instance cyklu</span><span class="sxs-lookup"><span data-stu-id="7fb46-131">Cycle instance prorate</span></span> | <span data-ttu-id="7fb46-132">Poměrné poplatky se od zákazníka vyhodnotily při změně přidružených licencí.</span><span class="sxs-lookup"><span data-stu-id="7fb46-132">Prorated charges assessed from the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="7fb46-133">Poměr poplatků při zrušení</span><span class="sxs-lookup"><span data-stu-id="7fb46-133">Prorate fees when cancel</span></span> | <span data-ttu-id="7fb46-134">Poměrná refundace nevyužité části služby při zrušení.</span><span class="sxs-lookup"><span data-stu-id="7fb46-134">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="7fb46-135">Poměrné poplatky při převodu z aktuální nabídky</span><span class="sxs-lookup"><span data-stu-id="7fb46-135">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="7fb46-136">Poměrné náklady po převodu od aktuálního měsíčního předplatného na roční předplatné</span><span class="sxs-lookup"><span data-stu-id="7fb46-136">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="7fb46-137">Poměrné poplatky při převodu na novou nabídku</span><span class="sxs-lookup"><span data-stu-id="7fb46-137">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="7fb46-138">Poměrné náklady po převodu měsíčního předplatného na nové roční předplatné.</span><span class="sxs-lookup"><span data-stu-id="7fb46-138">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="7fb46-139">Poměrné poplatky při nákupu</span><span class="sxs-lookup"><span data-stu-id="7fb46-139">Prorate fees when purchase</span></span> | <span data-ttu-id="7fb46-140">Typ poplatků pro předplatné při použití měsíčního nebo ročního účtování.</span><span class="sxs-lookup"><span data-stu-id="7fb46-140">The charge type for a subscription when using both monthly or annual billing.</span></span> |
| <span data-ttu-id="7fb46-141">Poplatek za prodlužování</span><span class="sxs-lookup"><span data-stu-id="7fb46-141">Prorate fee when renew</span></span> | <span data-ttu-id="7fb46-142">Poměrné poplatky při obnovení předplatného.</span><span class="sxs-lookup"><span data-stu-id="7fb46-142">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="7fb46-143">Prodloužit poplatek</span><span class="sxs-lookup"><span data-stu-id="7fb46-143">Renew fee</span></span> | <span data-ttu-id="7fb46-144">Poplatek za obnovení předplatného</span><span class="sxs-lookup"><span data-stu-id="7fb46-144">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="7fb46-145">Poplatky za rychlost při aktivaci</span><span class="sxs-lookup"><span data-stu-id="7fb46-145">Prorate fees when activate</span></span> | <span data-ttu-id="7fb46-146">Poměrné poplatky od aktivace až do konce fakturačního období.</span><span class="sxs-lookup"><span data-stu-id="7fb46-146">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="7fb46-147">Jednorázové poplatky</span><span class="sxs-lookup"><span data-stu-id="7fb46-147">One-time charges</span></span>

<span data-ttu-id="7fb46-148">Chcete-li namapovat tyto jednorázové poplatky na fakturu, sečtěte sloupec **částky** ze souboru založeného na licencích.</span><span class="sxs-lookup"><span data-stu-id="7fb46-148">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="7fb46-149">Popis poplatku (sloupec ChargeType v souboru pro odsouhlasení)</span><span class="sxs-lookup"><span data-stu-id="7fb46-149">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="7fb46-150">Vysvětlení poplatků</span><span class="sxs-lookup"><span data-stu-id="7fb46-150">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="7fb46-151">Nová</span><span class="sxs-lookup"><span data-stu-id="7fb46-151">New</span></span> | <span data-ttu-id="7fb46-152">Používá se při vytvoření nového nákupu.</span><span class="sxs-lookup"><span data-stu-id="7fb46-152">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="7fb46-153">addQuantity</span><span class="sxs-lookup"><span data-stu-id="7fb46-153">addQuantity</span></span> | <span data-ttu-id="7fb46-154">Používá se v refundaci původního nákupu i v novém množství po zvýšení.</span><span class="sxs-lookup"><span data-stu-id="7fb46-154">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="7fb46-155">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="7fb46-155">removeQuantity</span></span> | <span data-ttu-id="7fb46-156">Používá se v refundaci původního nákupu i v novém množství po zmenšení.</span><span class="sxs-lookup"><span data-stu-id="7fb46-156">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="7fb46-157">Zrušit</span><span class="sxs-lookup"><span data-stu-id="7fb46-157">Cancel</span></span> | <span data-ttu-id="7fb46-158">Používá se při zrušení odběru.</span><span class="sxs-lookup"><span data-stu-id="7fb46-158">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="7fb46-159">Převést</span><span class="sxs-lookup"><span data-stu-id="7fb46-159">Convert</span></span> | <span data-ttu-id="7fb46-160">Používá se při upgradu licence, ale počet licencí zůstane beze změny.</span><span class="sxs-lookup"><span data-stu-id="7fb46-160">Used when a license is upgraded but the number of licenses remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="7fb46-161">Poplatky za používání</span><span class="sxs-lookup"><span data-stu-id="7fb46-161">Usage charges</span></span>

<span data-ttu-id="7fb46-162">Pokud chcete namapovat tyto poplatky za použití na fakturu, sečtěte sloupec **PretaxCharges** ze souboru založeného na využití.</span><span class="sxs-lookup"><span data-stu-id="7fb46-162">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="7fb46-163">Popis poplatku (sloupec ChargeType v souboru pro odsouhlasení)</span><span class="sxs-lookup"><span data-stu-id="7fb46-163">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="7fb46-164">Vysvětlení poplatků</span><span class="sxs-lookup"><span data-stu-id="7fb46-164">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="7fb46-165">Vyhodnotit poplatek za použití při zrušení</span><span class="sxs-lookup"><span data-stu-id="7fb46-165">Assess usage fee when cancel</span></span> | <span data-ttu-id="7fb46-166">Použít poplatek za použití při zrušení neplaceného využití během aktuálního fakturačního období.</span><span class="sxs-lookup"><span data-stu-id="7fb46-166">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="7fb46-167">Vyhodnotit poplatek za použití pro aktuální cyklus</span><span class="sxs-lookup"><span data-stu-id="7fb46-167">Assess usage fee for current cycle</span></span> | <span data-ttu-id="7fb46-168">Přístup k poplatku za použití pro aktuální fakturační období</span><span class="sxs-lookup"><span data-stu-id="7fb46-168">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="7fb46-169">Kredity</span><span class="sxs-lookup"><span data-stu-id="7fb46-169">Credits</span></span>

<span data-ttu-id="7fb46-170">Chcete-li namapovat tyto kredity na vaši fakturu:</span><span class="sxs-lookup"><span data-stu-id="7fb46-170">To map these credits to your invoice:</span></span>

- <span data-ttu-id="7fb46-171">Sečtěte **TotalForCustomer** ze souboru založeného na licencích.</span><span class="sxs-lookup"><span data-stu-id="7fb46-171">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="7fb46-172">Sečtěte sloupec **PostTaxTotal** ze souboru založeného na využití.</span><span class="sxs-lookup"><span data-stu-id="7fb46-172">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="7fb46-173">Popis poplatku (sloupec ChargeType v souboru pro odsouhlasení)</span><span class="sxs-lookup"><span data-stu-id="7fb46-173">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="7fb46-174">Vysvětlení poplatků</span><span class="sxs-lookup"><span data-stu-id="7fb46-174">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="7fb46-175">Posunutí položky řádku</span><span class="sxs-lookup"><span data-stu-id="7fb46-175">Offset a line item</span></span> | <span data-ttu-id="7fb46-176">Částečná nebo celá náhrada za položku na řádku, včetně daní.</span><span class="sxs-lookup"><span data-stu-id="7fb46-176">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="7fb46-177">Slevy na základě využití</span><span class="sxs-lookup"><span data-stu-id="7fb46-177">Usage-based discounts</span></span>

<span data-ttu-id="7fb46-178">Pokud chcete tyto slevy na základě využití namapovat na fakturu, sečtěte sloupec **PretaxCharges** ze souboru založeného na využití.</span><span class="sxs-lookup"><span data-stu-id="7fb46-178">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="7fb46-179">Popis poplatku (sloupec ChargeType v souboru pro odsouhlasení)</span><span class="sxs-lookup"><span data-stu-id="7fb46-179">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="7fb46-180">Vysvětlení poplatků</span><span class="sxs-lookup"><span data-stu-id="7fb46-180">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="7fb46-181">Aktivační sleva</span><span class="sxs-lookup"><span data-stu-id="7fb46-181">Activation discount</span></span> | <span data-ttu-id="7fb46-182">Sleva použitá při aktivaci předplatného</span><span class="sxs-lookup"><span data-stu-id="7fb46-182">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="7fb46-183">Sleva na cyklus</span><span class="sxs-lookup"><span data-stu-id="7fb46-183">Cycle discount</span></span> | <span data-ttu-id="7fb46-184">Zvýhodněná sleva se účtuje na základě pravidelných poplatků.</span><span class="sxs-lookup"><span data-stu-id="7fb46-184">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="7fb46-185">Prodloužit slevu</span><span class="sxs-lookup"><span data-stu-id="7fb46-185">Renew discount</span></span> | <span data-ttu-id="7fb46-186">Sleva použitá při obnovení předplatného</span><span class="sxs-lookup"><span data-stu-id="7fb46-186">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="7fb46-187">Zrušit slevu</span><span class="sxs-lookup"><span data-stu-id="7fb46-187">Cancel discount</span></span> | <span data-ttu-id="7fb46-188">Poplatky se účtují při zrušení slev.</span><span class="sxs-lookup"><span data-stu-id="7fb46-188">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="7fb46-189">Slevy na základě licencí</span><span class="sxs-lookup"><span data-stu-id="7fb46-189">License-based discounts</span></span>

<span data-ttu-id="7fb46-190">Chcete-li namapovat slevy na základě licencí na fakturu, sečtěte sloupec **TotalOtherDiscount** ze souboru založeného na licencích.</span><span class="sxs-lookup"><span data-stu-id="7fb46-190">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="7fb46-191">*Slevy založené na licencích mohou být uplatněny na více typů poplatků.*</span><span class="sxs-lookup"><span data-stu-id="7fb46-191">*License-based discounts may be applied to multiple charge types.*</span></span>
