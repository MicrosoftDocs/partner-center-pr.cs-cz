---
title: Typy poplatků za soubor odsouhlasení
ms.topic: article
ms.date: 06/05/2020
description: Seznamte se s typy poplatků (jako jsou založené na licencích a na základě využití a jednorázové), kredity a slevy v souborech pro odsouhlasení partnerského centra.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f65c4a6496082934e8c38fbd924b96ef969be95b
ms.sourcegitcommit: e7931fbe7ce16a62124e00b2802520a17d7285b8
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/31/2020
ms.locfileid: "92527085"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="d356a-103">Pochopení různých typů poplatků v souborech pro odsouhlasení partnerského centra</span><span class="sxs-lookup"><span data-stu-id="d356a-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="d356a-104">**Platí pro**</span><span class="sxs-lookup"><span data-stu-id="d356a-104">**Applies to**</span></span>

- <span data-ttu-id="d356a-105">Partnerské centrum</span><span class="sxs-lookup"><span data-stu-id="d356a-105">Partner Center</span></span>
- <span data-ttu-id="d356a-106">Partnerské centrum pro Microsoft Cloud pro státní správu USA</span><span class="sxs-lookup"><span data-stu-id="d356a-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="d356a-107">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="d356a-107">**Appropriate roles**</span></span>

- <span data-ttu-id="d356a-108">Agent správce</span><span class="sxs-lookup"><span data-stu-id="d356a-108">Admin agent</span></span>
- <span data-ttu-id="d356a-109">Správce fakturace</span><span class="sxs-lookup"><span data-stu-id="d356a-109">Billing admin</span></span>
- <span data-ttu-id="d356a-110">Globální správce</span><span class="sxs-lookup"><span data-stu-id="d356a-110">Global admin</span></span>

<span data-ttu-id="d356a-111">Toto téma popisuje mapování mezi oddílem faktury a typy přidružených poplatků, které mohou být na vašem souboru pro odsouhlasení.</span><span class="sxs-lookup"><span data-stu-id="d356a-111">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="d356a-112">Vaše faktura poskytuje souhrn poplatků.</span><span class="sxs-lookup"><span data-stu-id="d356a-112">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="d356a-113">Váš soubor pro odsouhlasení poskytuje podrobný rozpis transakcí položek řádků, včetně typů poplatků.</span><span class="sxs-lookup"><span data-stu-id="d356a-113">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="d356a-114">Další informace o souborech pro odsouhlasení najdete v tématu [Jak používat soubory pro odsouhlasení](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="d356a-114">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="d356a-115">[Soubory odsouhlasení založené na použití](usage-based-recon-files.md) a [soubory odsouhlasení založené na licencích](license-based-recon-files.md) zobrazují jenom transakce a poplatky související s využitím (spotřebované jednotky a související poplatky).</span><span class="sxs-lookup"><span data-stu-id="d356a-115">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="d356a-116">Jednorázové kredity, slevy nebo refundace, které se zobrazí na faktuře jako **Úpravy** , se v souboru pro odsouhlasení nezobrazují.</span><span class="sxs-lookup"><span data-stu-id="d356a-116">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="d356a-117">Mapování typů nákladů na faktury</span><span class="sxs-lookup"><span data-stu-id="d356a-117">Map charge types to invoice charges</span></span>

<span data-ttu-id="d356a-118">Chcete-li náklady na křížové odkazy mezi vaším souborem faktury a odsouhlasení, použijte možnosti filtru v aplikaci Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="d356a-118">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="d356a-119">Filtrovat poplatky za fakturu na sadu rozdělení poplatků v souboru odsouhlasení podle typu poplatků za poplatek.</span><span class="sxs-lookup"><span data-stu-id="d356a-119">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="d356a-120">Poplatky na základě licencí</span><span class="sxs-lookup"><span data-stu-id="d356a-120">License-based charges</span></span>

<span data-ttu-id="d356a-121">Chcete-li namapovat tyto poplatky na základě licencí na fakturu, sečtěte sloupec **částky** ze souboru založeného na licencích.</span><span class="sxs-lookup"><span data-stu-id="d356a-121">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="d356a-122">Popis poplatku (sloupec ChargeType v souboru pro odsouhlasení)</span><span class="sxs-lookup"><span data-stu-id="d356a-122">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="d356a-123">Vysvětlení poplatků</span><span class="sxs-lookup"><span data-stu-id="d356a-123">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="d356a-124">Aktivační poplatek</span><span class="sxs-lookup"><span data-stu-id="d356a-124">Activation fee</span></span> | <span data-ttu-id="d356a-125">Částka, která se účtuje zákazníkovi při použití předplatného po nákupu</span><span class="sxs-lookup"><span data-stu-id="d356a-125">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="d356a-126">Zrušit poplatek</span><span class="sxs-lookup"><span data-stu-id="d356a-126">Cancel fee</span></span> | <span data-ttu-id="d356a-127">Poměrné náklady se účtují zákazníkovi při změně přidružených licencí.</span><span class="sxs-lookup"><span data-stu-id="d356a-127">Prorated charges refunded to the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="d356a-128">Zrušit poměr instancí</span><span class="sxs-lookup"><span data-stu-id="d356a-128">Cancel instance prorate</span></span> | <span data-ttu-id="d356a-129">Poměrné poplatky se zrušily, když zákazník s měsíčním předplatným má předplatné pozastaveno a přidružené licence se v rámci stejného měsíce změnily.</span><span class="sxs-lookup"><span data-stu-id="d356a-129">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated licenses changed within the same month.</span></span> |
| <span data-ttu-id="d356a-130">Poplatek za cyklus</span><span class="sxs-lookup"><span data-stu-id="d356a-130">Cycle fee</span></span> | <span data-ttu-id="d356a-131">Pravidelné poplatky za předplatné</span><span class="sxs-lookup"><span data-stu-id="d356a-131">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="d356a-132">Poměr instance cyklu</span><span class="sxs-lookup"><span data-stu-id="d356a-132">Cycle instance prorate</span></span> | <span data-ttu-id="d356a-133">Poměrné poplatky se od zákazníka vyhodnotily při změně přidružených licencí.</span><span class="sxs-lookup"><span data-stu-id="d356a-133">Prorated charges assessed from the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="d356a-134">Poměr poplatků při zrušení</span><span class="sxs-lookup"><span data-stu-id="d356a-134">Prorate fees when cancel</span></span> | <span data-ttu-id="d356a-135">Poměrná refundace nevyužité části služby při zrušení.</span><span class="sxs-lookup"><span data-stu-id="d356a-135">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="d356a-136">Poměrné poplatky při převodu z aktuální nabídky</span><span class="sxs-lookup"><span data-stu-id="d356a-136">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="d356a-137">Poměrné náklady po převodu od aktuálního měsíčního předplatného na roční předplatné</span><span class="sxs-lookup"><span data-stu-id="d356a-137">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="d356a-138">Poměrné poplatky při převodu na novou nabídku</span><span class="sxs-lookup"><span data-stu-id="d356a-138">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="d356a-139">Poměrné náklady po převodu měsíčního předplatného na nové roční předplatné.</span><span class="sxs-lookup"><span data-stu-id="d356a-139">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="d356a-140">Poměrné poplatky při nákupu</span><span class="sxs-lookup"><span data-stu-id="d356a-140">Prorate fees when purchase</span></span> | <span data-ttu-id="d356a-141">Typ poplatků pro předplatné při použití měsíčního nebo ročního účtování.</span><span class="sxs-lookup"><span data-stu-id="d356a-141">The charge type for a subscription when using both monthly or annual billing.</span></span> |
| <span data-ttu-id="d356a-142">Poplatek za prodlužování</span><span class="sxs-lookup"><span data-stu-id="d356a-142">Prorate fee when renew</span></span> | <span data-ttu-id="d356a-143">Poměrné poplatky při obnovení předplatného.</span><span class="sxs-lookup"><span data-stu-id="d356a-143">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="d356a-144">Prodloužit poplatek</span><span class="sxs-lookup"><span data-stu-id="d356a-144">Renew fee</span></span> | <span data-ttu-id="d356a-145">Poplatek za obnovení předplatného</span><span class="sxs-lookup"><span data-stu-id="d356a-145">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="d356a-146">Poplatky za rychlost při aktivaci</span><span class="sxs-lookup"><span data-stu-id="d356a-146">Prorate fees when activate</span></span> | <span data-ttu-id="d356a-147">Poměrné poplatky od aktivace až do konce fakturačního období.</span><span class="sxs-lookup"><span data-stu-id="d356a-147">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="d356a-148">Jednorázové poplatky</span><span class="sxs-lookup"><span data-stu-id="d356a-148">One-time charges</span></span>

<span data-ttu-id="d356a-149">Chcete-li namapovat tyto jednorázové poplatky na fakturu, sečtěte sloupec **částky** ze souboru založeného na licencích.</span><span class="sxs-lookup"><span data-stu-id="d356a-149">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="d356a-150">Popis poplatku (sloupec ChargeType v souboru pro odsouhlasení)</span><span class="sxs-lookup"><span data-stu-id="d356a-150">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="d356a-151">Vysvětlení poplatků</span><span class="sxs-lookup"><span data-stu-id="d356a-151">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="d356a-152">Nová</span><span class="sxs-lookup"><span data-stu-id="d356a-152">New</span></span> | <span data-ttu-id="d356a-153">Používá se při vytvoření nového nákupu.</span><span class="sxs-lookup"><span data-stu-id="d356a-153">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="d356a-154">addQuantity</span><span class="sxs-lookup"><span data-stu-id="d356a-154">addQuantity</span></span> | <span data-ttu-id="d356a-155">Používá se v refundaci původního nákupu i v novém množství po zvýšení.</span><span class="sxs-lookup"><span data-stu-id="d356a-155">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="d356a-156">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="d356a-156">removeQuantity</span></span> | <span data-ttu-id="d356a-157">Používá se v refundaci původního nákupu i v novém množství po zmenšení.</span><span class="sxs-lookup"><span data-stu-id="d356a-157">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="d356a-158">Zrušit</span><span class="sxs-lookup"><span data-stu-id="d356a-158">Cancel</span></span> | <span data-ttu-id="d356a-159">Používá se při zrušení odběru.</span><span class="sxs-lookup"><span data-stu-id="d356a-159">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="d356a-160">Převést</span><span class="sxs-lookup"><span data-stu-id="d356a-160">Convert</span></span> | <span data-ttu-id="d356a-161">Používá se při upgradu licence, ale počet licencí zůstane beze změny.</span><span class="sxs-lookup"><span data-stu-id="d356a-161">Used when a license is upgraded but the number of licenses remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="d356a-162">Poplatky za používání</span><span class="sxs-lookup"><span data-stu-id="d356a-162">Usage charges</span></span>

<span data-ttu-id="d356a-163">Pokud chcete namapovat tyto poplatky za použití na fakturu, sečtěte sloupec **PretaxCharges** ze souboru založeného na využití.</span><span class="sxs-lookup"><span data-stu-id="d356a-163">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="d356a-164">Popis poplatku (sloupec ChargeType v souboru pro odsouhlasení)</span><span class="sxs-lookup"><span data-stu-id="d356a-164">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="d356a-165">Vysvětlení poplatků</span><span class="sxs-lookup"><span data-stu-id="d356a-165">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="d356a-166">Vyhodnotit poplatek za použití při zrušení</span><span class="sxs-lookup"><span data-stu-id="d356a-166">Assess usage fee when cancel</span></span> | <span data-ttu-id="d356a-167">Použít poplatek za použití při zrušení neplaceného využití během aktuálního fakturačního období.</span><span class="sxs-lookup"><span data-stu-id="d356a-167">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="d356a-168">Vyhodnotit poplatek za použití pro aktuální cyklus</span><span class="sxs-lookup"><span data-stu-id="d356a-168">Assess usage fee for current cycle</span></span> | <span data-ttu-id="d356a-169">Přístup k poplatku za použití pro aktuální fakturační období</span><span class="sxs-lookup"><span data-stu-id="d356a-169">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="d356a-170">Kredity</span><span class="sxs-lookup"><span data-stu-id="d356a-170">Credits</span></span>

<span data-ttu-id="d356a-171">Chcete-li namapovat tyto kredity na vaši fakturu:</span><span class="sxs-lookup"><span data-stu-id="d356a-171">To map these credits to your invoice:</span></span>

- <span data-ttu-id="d356a-172">Sečtěte **TotalForCustomer** ze souboru založeného na licencích.</span><span class="sxs-lookup"><span data-stu-id="d356a-172">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="d356a-173">Sečtěte sloupec **PostTaxTotal** ze souboru založeného na využití.</span><span class="sxs-lookup"><span data-stu-id="d356a-173">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="d356a-174">Popis poplatku (sloupec ChargeType v souboru pro odsouhlasení)</span><span class="sxs-lookup"><span data-stu-id="d356a-174">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="d356a-175">Vysvětlení poplatků</span><span class="sxs-lookup"><span data-stu-id="d356a-175">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="d356a-176">Posunutí položky řádku</span><span class="sxs-lookup"><span data-stu-id="d356a-176">Offset a line item</span></span> | <span data-ttu-id="d356a-177">Částečná nebo celá náhrada za položku na řádku, včetně daní.</span><span class="sxs-lookup"><span data-stu-id="d356a-177">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="d356a-178">Slevy na základě využití</span><span class="sxs-lookup"><span data-stu-id="d356a-178">Usage-based discounts</span></span>

<span data-ttu-id="d356a-179">Pokud chcete tyto slevy na základě využití namapovat na fakturu, sečtěte sloupec **PretaxCharges** ze souboru založeného na využití.</span><span class="sxs-lookup"><span data-stu-id="d356a-179">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="d356a-180">Popis poplatku (sloupec ChargeType v souboru pro odsouhlasení)</span><span class="sxs-lookup"><span data-stu-id="d356a-180">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="d356a-181">Vysvětlení poplatků</span><span class="sxs-lookup"><span data-stu-id="d356a-181">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="d356a-182">Aktivační sleva</span><span class="sxs-lookup"><span data-stu-id="d356a-182">Activation discount</span></span> | <span data-ttu-id="d356a-183">Sleva použitá při aktivaci předplatného</span><span class="sxs-lookup"><span data-stu-id="d356a-183">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="d356a-184">Sleva na cyklus</span><span class="sxs-lookup"><span data-stu-id="d356a-184">Cycle discount</span></span> | <span data-ttu-id="d356a-185">Zvýhodněná sleva se účtuje na základě pravidelných poplatků.</span><span class="sxs-lookup"><span data-stu-id="d356a-185">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="d356a-186">Prodloužit slevu</span><span class="sxs-lookup"><span data-stu-id="d356a-186">Renew discount</span></span> | <span data-ttu-id="d356a-187">Sleva použitá při obnovení předplatného</span><span class="sxs-lookup"><span data-stu-id="d356a-187">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="d356a-188">Zrušit slevu</span><span class="sxs-lookup"><span data-stu-id="d356a-188">Cancel discount</span></span> | <span data-ttu-id="d356a-189">Poplatky se účtují při zrušení slev.</span><span class="sxs-lookup"><span data-stu-id="d356a-189">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="d356a-190">Slevy na základě licencí</span><span class="sxs-lookup"><span data-stu-id="d356a-190">License-based discounts</span></span>

<span data-ttu-id="d356a-191">Chcete-li namapovat slevy na základě licencí na fakturu, sečtěte sloupec **TotalOtherDiscount** ze souboru založeného na licencích.</span><span class="sxs-lookup"><span data-stu-id="d356a-191">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="d356a-192">*Slevy založené na licencích mohou být uplatněny na více typů poplatků.*</span><span class="sxs-lookup"><span data-stu-id="d356a-192">*License-based discounts may be applied to multiple charge types.*</span></span>
