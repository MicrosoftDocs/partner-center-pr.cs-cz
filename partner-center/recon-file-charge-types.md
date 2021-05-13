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
ms.openlocfilehash: 5a1f45de59fc9dac6a443bb8a14c3a80b36ba3f7
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855875"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="ee01b-103">Pochopení různých typů poplatků v souborech pro odsouhlasení partnerského centra</span><span class="sxs-lookup"><span data-stu-id="ee01b-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="ee01b-104">**Platí pro**: partnerské Centrum | Partnerské centrum pro Microsoft Cloud pro státní správu USA</span><span class="sxs-lookup"><span data-stu-id="ee01b-104">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="ee01b-105">**Příslušné role**: Agent správce | Správce fakturace | Globální správce</span><span class="sxs-lookup"><span data-stu-id="ee01b-105">**Appropriate roles**: Admin agent | Billing admin | Global admin</span></span>

<span data-ttu-id="ee01b-106">Tento článek popisuje mapování mezi oddílem faktury a typy přidružených poplatků, které mohou být na vašem souboru pro odsouhlasení.</span><span class="sxs-lookup"><span data-stu-id="ee01b-106">This article describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="ee01b-107">Vaše faktura poskytuje souhrn poplatků.</span><span class="sxs-lookup"><span data-stu-id="ee01b-107">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="ee01b-108">Váš soubor pro odsouhlasení poskytuje podrobný rozpis transakcí položek řádků, včetně typů poplatků.</span><span class="sxs-lookup"><span data-stu-id="ee01b-108">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="ee01b-109">Další informace o souborech pro odsouhlasení najdete v tématu [Jak používat soubory pro odsouhlasení](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="ee01b-109">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="ee01b-110">[Soubory odsouhlasení založené na použití](usage-based-recon-files.md) a [soubory odsouhlasení založené na licencích](license-based-recon-files.md) zobrazují jenom transakce a poplatky související s využitím (spotřebované jednotky a související poplatky).</span><span class="sxs-lookup"><span data-stu-id="ee01b-110">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="ee01b-111">Jednorázové kredity, slevy nebo refundace, které se zobrazí na faktuře jako **Úpravy** , se v souboru pro odsouhlasení nezobrazují.</span><span class="sxs-lookup"><span data-stu-id="ee01b-111">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="ee01b-112">Mapování typů nákladů na faktury</span><span class="sxs-lookup"><span data-stu-id="ee01b-112">Map charge types to invoice charges</span></span>

<span data-ttu-id="ee01b-113">Chcete-li náklady na křížové odkazy mezi vaším souborem faktury a odsouhlasení, použijte možnosti filtru v aplikaci Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="ee01b-113">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="ee01b-114">Filtrovat poplatky za fakturu na sadu rozdělení poplatků v souboru odsouhlasení podle typu poplatků za poplatek.</span><span class="sxs-lookup"><span data-stu-id="ee01b-114">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="ee01b-115">Poplatky na základě licencí</span><span class="sxs-lookup"><span data-stu-id="ee01b-115">License-based charges</span></span>

<span data-ttu-id="ee01b-116">Chcete-li namapovat tyto poplatky na základě licencí na fakturu, sečtěte sloupec **částky** ze souboru založeného na licencích.</span><span class="sxs-lookup"><span data-stu-id="ee01b-116">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="ee01b-117">Popis poplatku (sloupec ChargeType v souboru pro odsouhlasení)</span><span class="sxs-lookup"><span data-stu-id="ee01b-117">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="ee01b-118">Vysvětlení poplatků</span><span class="sxs-lookup"><span data-stu-id="ee01b-118">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="ee01b-119">Aktivační poplatek</span><span class="sxs-lookup"><span data-stu-id="ee01b-119">Activation fee</span></span> | <span data-ttu-id="ee01b-120">Částka, která se účtuje zákazníkovi při použití předplatného po nákupu</span><span class="sxs-lookup"><span data-stu-id="ee01b-120">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="ee01b-121">Zrušit poplatek</span><span class="sxs-lookup"><span data-stu-id="ee01b-121">Cancel fee</span></span> | <span data-ttu-id="ee01b-122">Po změně přidružených licencí se zákazníkovi vrátí zaceněné poplatky.</span><span class="sxs-lookup"><span data-stu-id="ee01b-122">Prorated charges refunded to the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="ee01b-123">Zrušení přenosové rychlosti instancí</span><span class="sxs-lookup"><span data-stu-id="ee01b-123">Cancel instance prorate</span></span> | <span data-ttu-id="ee01b-124">Poplatky za předplatná se zruší v případě, že u zákazníka s měsíčním předplatným je předplatné pozastavené a přidružené licence se během stejného měsíce změnily.</span><span class="sxs-lookup"><span data-stu-id="ee01b-124">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated licenses changed within the same month.</span></span> |
| <span data-ttu-id="ee01b-125">Poplatek za cyklus</span><span class="sxs-lookup"><span data-stu-id="ee01b-125">Cycle fee</span></span> | <span data-ttu-id="ee01b-126">Pravidelné poplatky za předplatné.</span><span class="sxs-lookup"><span data-stu-id="ee01b-126">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="ee01b-127">Cyklické přenosy instancí</span><span class="sxs-lookup"><span data-stu-id="ee01b-127">Cycle instance prorate</span></span> | <span data-ttu-id="ee01b-128">Poplatky rozceněné zákazníkem posuzované při změně přidružených licencí.</span><span class="sxs-lookup"><span data-stu-id="ee01b-128">Prorated charges assessed from the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="ee01b-129">Poplatky za přenos při zrušení</span><span class="sxs-lookup"><span data-stu-id="ee01b-129">Prorate fees when cancel</span></span> | <span data-ttu-id="ee01b-130">Naceněná refundace za nevyužitou část služby po zrušení.</span><span class="sxs-lookup"><span data-stu-id="ee01b-130">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="ee01b-131">Poplatky za přenos při převodu z aktuální nabídky</span><span class="sxs-lookup"><span data-stu-id="ee01b-131">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="ee01b-132">Přeceněné poplatky po převodu z aktuálního měsíčního předplatného na roční předplatné.</span><span class="sxs-lookup"><span data-stu-id="ee01b-132">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="ee01b-133">Poplatky za přenos při převodu na novou nabídku</span><span class="sxs-lookup"><span data-stu-id="ee01b-133">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="ee01b-134">Přehodnocené poplatky po převodu měsíčního předplatného na nové roční předplatné.</span><span class="sxs-lookup"><span data-stu-id="ee01b-134">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="ee01b-135">Poplatky za přenos při nákupu</span><span class="sxs-lookup"><span data-stu-id="ee01b-135">Prorate fees when purchase</span></span> | <span data-ttu-id="ee01b-136">Typ poplatku za předplatné při použití měsíční i roční fakturace.</span><span class="sxs-lookup"><span data-stu-id="ee01b-136">The charge type for a subscription when using both monthly or annual billing.</span></span> |
| <span data-ttu-id="ee01b-137">Poplatek za přenos při prodloužení platnosti</span><span class="sxs-lookup"><span data-stu-id="ee01b-137">Prorate fee when renew</span></span> | <span data-ttu-id="ee01b-138">Poplatky na základě předplatných při prodloužení platnosti předplatného.</span><span class="sxs-lookup"><span data-stu-id="ee01b-138">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="ee01b-139">Poplatek za prodloužení platnosti</span><span class="sxs-lookup"><span data-stu-id="ee01b-139">Renew fee</span></span> | <span data-ttu-id="ee01b-140">Poplatek za prodloužení platnosti předplatného</span><span class="sxs-lookup"><span data-stu-id="ee01b-140">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="ee01b-141">Poplatky za přenos při aktivaci</span><span class="sxs-lookup"><span data-stu-id="ee01b-141">Prorate fees when activate</span></span> | <span data-ttu-id="ee01b-142">Poměrné poplatky od aktivace až do konce fakturačního období.</span><span class="sxs-lookup"><span data-stu-id="ee01b-142">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="ee01b-143">Jednorázové poplatky</span><span class="sxs-lookup"><span data-stu-id="ee01b-143">One-time charges</span></span>

<span data-ttu-id="ee01b-144">Chcete-li namapovat tyto jednorázové poplatky na fakturu, sečtěte sloupec **částky** ze souboru založeného na licencích.</span><span class="sxs-lookup"><span data-stu-id="ee01b-144">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="ee01b-145">Popis poplatku (sloupec ChargeType v souboru pro odsouhlasení)</span><span class="sxs-lookup"><span data-stu-id="ee01b-145">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="ee01b-146">Vysvětlení poplatků</span><span class="sxs-lookup"><span data-stu-id="ee01b-146">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="ee01b-147">Nová</span><span class="sxs-lookup"><span data-stu-id="ee01b-147">New</span></span> | <span data-ttu-id="ee01b-148">Používá se při vytvoření nového nákupu.</span><span class="sxs-lookup"><span data-stu-id="ee01b-148">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="ee01b-149">addQuantity</span><span class="sxs-lookup"><span data-stu-id="ee01b-149">addQuantity</span></span> | <span data-ttu-id="ee01b-150">Používá se v refundaci původního nákupu i v novém množství po zvýšení.</span><span class="sxs-lookup"><span data-stu-id="ee01b-150">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="ee01b-151">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="ee01b-151">removeQuantity</span></span> | <span data-ttu-id="ee01b-152">Používá se v refundaci původního nákupu i v novém množství po zmenšení.</span><span class="sxs-lookup"><span data-stu-id="ee01b-152">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="ee01b-153">Zrušit</span><span class="sxs-lookup"><span data-stu-id="ee01b-153">Cancel</span></span> | <span data-ttu-id="ee01b-154">Používá se při zrušení odběru.</span><span class="sxs-lookup"><span data-stu-id="ee01b-154">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="ee01b-155">Převést</span><span class="sxs-lookup"><span data-stu-id="ee01b-155">Convert</span></span> | <span data-ttu-id="ee01b-156">Používá se při upgradu licence, ale počet licencí zůstane beze změny.</span><span class="sxs-lookup"><span data-stu-id="ee01b-156">Used when a license is upgraded but the number of licenses remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="ee01b-157">Poplatky za používání</span><span class="sxs-lookup"><span data-stu-id="ee01b-157">Usage charges</span></span>

<span data-ttu-id="ee01b-158">Pokud chcete namapovat tyto poplatky za použití na fakturu, sečtěte sloupec **PretaxCharges** ze souboru založeného na využití.</span><span class="sxs-lookup"><span data-stu-id="ee01b-158">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="ee01b-159">Popis poplatku (sloupec ChargeType v souboru pro odsouhlasení)</span><span class="sxs-lookup"><span data-stu-id="ee01b-159">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="ee01b-160">Vysvětlení poplatků</span><span class="sxs-lookup"><span data-stu-id="ee01b-160">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="ee01b-161">Vyhodnotit poplatek za použití při zrušení</span><span class="sxs-lookup"><span data-stu-id="ee01b-161">Assess usage fee when cancel</span></span> | <span data-ttu-id="ee01b-162">Použít poplatek za použití při zrušení neplaceného využití během aktuálního fakturačního období.</span><span class="sxs-lookup"><span data-stu-id="ee01b-162">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="ee01b-163">Vyhodnotit poplatek za použití pro aktuální cyklus</span><span class="sxs-lookup"><span data-stu-id="ee01b-163">Assess usage fee for current cycle</span></span> | <span data-ttu-id="ee01b-164">Přístup k poplatku za použití pro aktuální fakturační období</span><span class="sxs-lookup"><span data-stu-id="ee01b-164">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="ee01b-165">Kredity</span><span class="sxs-lookup"><span data-stu-id="ee01b-165">Credits</span></span>

<span data-ttu-id="ee01b-166">Chcete-li namapovat tyto kredity na vaši fakturu:</span><span class="sxs-lookup"><span data-stu-id="ee01b-166">To map these credits to your invoice:</span></span>

- <span data-ttu-id="ee01b-167">Sečte **totalForCustomer** ze souboru založeného na licencích.</span><span class="sxs-lookup"><span data-stu-id="ee01b-167">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="ee01b-168">Sečte **sloupec PostTaxTotal** ze souboru založeného na využití.</span><span class="sxs-lookup"><span data-stu-id="ee01b-168">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="ee01b-169">Popis poplatku (sloupec ChargeType v souboru s vyrovnáním)</span><span class="sxs-lookup"><span data-stu-id="ee01b-169">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="ee01b-170">Vysvětlení poplatků</span><span class="sxs-lookup"><span data-stu-id="ee01b-170">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="ee01b-171">Posun řádkové položky</span><span class="sxs-lookup"><span data-stu-id="ee01b-171">Offset a line item</span></span> | <span data-ttu-id="ee01b-172">Částečná nebo celá refundace řádkové položky, včetně daní.</span><span class="sxs-lookup"><span data-stu-id="ee01b-172">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="ee01b-173">Slevy založené na využití</span><span class="sxs-lookup"><span data-stu-id="ee01b-173">Usage-based discounts</span></span>

<span data-ttu-id="ee01b-174">Pokud chcete tyto slevy založené na využití namapovat na fakturu, sečtete sloupec **PretaxCharges** ze souboru založeného na využití.</span><span class="sxs-lookup"><span data-stu-id="ee01b-174">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="ee01b-175">Popis poplatku (sloupec ChargeType v souboru s vyrovnáním)</span><span class="sxs-lookup"><span data-stu-id="ee01b-175">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="ee01b-176">Vysvětlení poplatků</span><span class="sxs-lookup"><span data-stu-id="ee01b-176">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="ee01b-177">Sleva za aktivaci</span><span class="sxs-lookup"><span data-stu-id="ee01b-177">Activation discount</span></span> | <span data-ttu-id="ee01b-178">Sleva uplatněná při aktivaci předplatného</span><span class="sxs-lookup"><span data-stu-id="ee01b-178">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="ee01b-179">Sleva za cyklus</span><span class="sxs-lookup"><span data-stu-id="ee01b-179">Cycle discount</span></span> | <span data-ttu-id="ee01b-180">Sleva uplatněná na pravidelné poplatky.</span><span class="sxs-lookup"><span data-stu-id="ee01b-180">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="ee01b-181">Sleva za prodloužení platnosti</span><span class="sxs-lookup"><span data-stu-id="ee01b-181">Renew discount</span></span> | <span data-ttu-id="ee01b-182">Sleva uplatněná při prodloužení platnosti předplatného</span><span class="sxs-lookup"><span data-stu-id="ee01b-182">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="ee01b-183">Zrušení slevy</span><span class="sxs-lookup"><span data-stu-id="ee01b-183">Cancel discount</span></span> | <span data-ttu-id="ee01b-184">Poplatky uplatněné při zrušení slev</span><span class="sxs-lookup"><span data-stu-id="ee01b-184">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="ee01b-185">Slevy založené na licencích</span><span class="sxs-lookup"><span data-stu-id="ee01b-185">License-based discounts</span></span>

<span data-ttu-id="ee01b-186">Pokud chcete na svou fakturu mapovat slevy založené na licencích, sečtete sloupec **TotalOtherDiscount** ze souboru založeného na licencích.</span><span class="sxs-lookup"><span data-stu-id="ee01b-186">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="ee01b-187">*Slevy založené na licencích mohou být uplatněny na více typů poplatků.*</span><span class="sxs-lookup"><span data-stu-id="ee01b-187">*License-based discounts may be applied to multiple charge types.*</span></span>
