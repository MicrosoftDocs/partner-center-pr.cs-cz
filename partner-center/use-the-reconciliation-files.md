---
title: Použití souborů odsouhlasení
ms.topic: article
ms.date: 06/08/2020
description: Přečtěte si informace o souborech pro odsouhlasení v partnerském centru a o tom, jak interpretovat detailní zobrazení položek poplatků za daný fakturační cyklus.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d09c1e57d16937c5656579f3932e9c8feb3ecf24
ms.sourcegitcommit: 95a5afdf68d88b6be848729830dcd114e3fb0c0f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/11/2020
ms.locfileid: "94488075"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="af7ee-103">Přečtěte si, jak číst položky řádků v souborech odsouhlasení partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="af7ee-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="af7ee-104">Platí pro:</span><span class="sxs-lookup"><span data-stu-id="af7ee-104">Applies to:</span></span>

- <span data-ttu-id="af7ee-105">Partnerské centrum</span><span class="sxs-lookup"><span data-stu-id="af7ee-105">Partner Center</span></span>
- <span data-ttu-id="af7ee-106">Partnerské centrum pro Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="af7ee-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="af7ee-107">Soubory pro odsouhlasení si můžete stáhnout z partnerského centra, kde najdete podrobné zobrazení položek jednotlivých poplatků v rámci fakturačního cyklu.</span><span class="sxs-lookup"><span data-stu-id="af7ee-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="af7ee-108">Podrobnosti o položkách na řádcích zahrnují poplatky za předplatné každého zákazníka a podrobné události (například přidání licencí do předplatného).</span><span class="sxs-lookup"><span data-stu-id="af7ee-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="af7ee-109">Příslušné role:</span><span class="sxs-lookup"><span data-stu-id="af7ee-109">Appropriate roles:</span></span>

- <span data-ttu-id="af7ee-110">Správce fakturace</span><span class="sxs-lookup"><span data-stu-id="af7ee-110">Billing admin</span></span>
- <span data-ttu-id="af7ee-111">Globální správce</span><span class="sxs-lookup"><span data-stu-id="af7ee-111">Global admin</span></span>

<span data-ttu-id="af7ee-112">Informace o tom, jak si **fakturu** přečíst, najdete v tématu [Přečtěte si vyúčtování](read-your-bill.md).</span><span class="sxs-lookup"><span data-stu-id="af7ee-112">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="af7ee-113">Vysvětlení polí souboru odsouhlasení</span><span class="sxs-lookup"><span data-stu-id="af7ee-113">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="af7ee-114">Pole souboru odsouhlasení založeného na licencích</span><span class="sxs-lookup"><span data-stu-id="af7ee-114">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="af7ee-115">Pole souboru odsouhlasení založeného na využití</span><span class="sxs-lookup"><span data-stu-id="af7ee-115">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="af7ee-116">Pole souborů odsouhlasení podle denního hodnocení využití</span><span class="sxs-lookup"><span data-stu-id="af7ee-116">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="af7ee-117">Pole souborů odsouhlasení zprostředkovatele CSP v jednom čase</span><span class="sxs-lookup"><span data-stu-id="af7ee-117">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="af7ee-118">Pochopení typů poplatků v souborech pro odsouhlasení</span><span class="sxs-lookup"><span data-stu-id="af7ee-118">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="af7ee-119">Chcete-li pochopit typy poplatků v souborech pro odsouhlasení (sloupec **ChargeType** ), podívejte se na téma [odsouhlasení typů poplatků za soubor](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="af7ee-119">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="af7ee-120">Opravit problémy s formátováním</span><span class="sxs-lookup"><span data-stu-id="af7ee-120">Fix formatting issues</span></span>

<span data-ttu-id="af7ee-121">V některých případech může soubor pro odsouhlasení obsahovat problémy s formátováním.</span><span class="sxs-lookup"><span data-stu-id="af7ee-121">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="af7ee-122">K tomuto problému může dojít například v případě, že se národní prostředí en-US nepoužívá.</span><span class="sxs-lookup"><span data-stu-id="af7ee-122">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="af7ee-123">Pomocí těchto kroků opravíte všechny problémy formátování souborů odsouhlasení:</span><span class="sxs-lookup"><span data-stu-id="af7ee-123">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="af7ee-124">Otevřete soubor pro odsouhlasení (ve formátu CSV) v aplikaci Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="af7ee-124">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="af7ee-125">Vyberte první sloupec v souboru.</span><span class="sxs-lookup"><span data-stu-id="af7ee-125">Select the first column in the file.</span></span>
3. <span data-ttu-id="af7ee-126">Otevřete **Průvodce převodem textu na sloupce**.</span><span class="sxs-lookup"><span data-stu-id="af7ee-126">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="af7ee-127">Na pásu karet vyberte **data** a pak vyberte **text do sloupců**.</span><span class="sxs-lookup"><span data-stu-id="af7ee-127">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="af7ee-128">V průvodci vyberte **typ souboru s oddělovači**.</span><span class="sxs-lookup"><span data-stu-id="af7ee-128">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="af7ee-129">Pak vyberte **Další**.</span><span class="sxs-lookup"><span data-stu-id="af7ee-129">Then, select **Next**.</span></span>
5. <span data-ttu-id="af7ee-130">V poli **oddělovače** vyberte **čárka**.</span><span class="sxs-lookup"><span data-stu-id="af7ee-130">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="af7ee-131">(Pokud je už vybraná **karta** , můžete tuto možnost nechat vybranou.) Pak vyberte **Další**.</span><span class="sxs-lookup"><span data-stu-id="af7ee-131">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="af7ee-132">V poli **Formát dat sloupce** vyberte **Datum: MDY**.</span><span class="sxs-lookup"><span data-stu-id="af7ee-132">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="af7ee-133">Pak vyberte **Další**.</span><span class="sxs-lookup"><span data-stu-id="af7ee-133">Then, select **Next**.</span></span>
7. <span data-ttu-id="af7ee-134">V poli **Formát dat sloupce** vyberte možnost **text** pro sloupce všech částek.</span><span class="sxs-lookup"><span data-stu-id="af7ee-134">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="af7ee-135">Pak vyberte **Finish** (Dokončit).</span><span class="sxs-lookup"><span data-stu-id="af7ee-135">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="af7ee-136">Stažení souborů pro odsouhlasení programově</span><span class="sxs-lookup"><span data-stu-id="af7ee-136">Download reconciliation files programmatically</span></span>

<span data-ttu-id="af7ee-137">Soubory pro odsouhlasení můžou být velmi velké a někdy je obtížné stáhnout.</span><span class="sxs-lookup"><span data-stu-id="af7ee-137">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="af7ee-138">Chcete-li stáhnout soubory pro odsouhlasení programově, viz [získat řádky faktury](/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="af7ee-138">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="af7ee-139">Mapování daní nebo DPH</span><span class="sxs-lookup"><span data-stu-id="af7ee-139">Map taxes or VAT</span></span>

<span data-ttu-id="af7ee-140">K namapování daně nebo daně z přidané hodnoty (DPH) na fakturu:</span><span class="sxs-lookup"><span data-stu-id="af7ee-140">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="af7ee-141">Sečtěte sloupec **daně** ze souboru založeného na licencích.</span><span class="sxs-lookup"><span data-stu-id="af7ee-141">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="af7ee-142">Sečtěte sloupec **TaxAmount** ze souboru založeného na využití.</span><span class="sxs-lookup"><span data-stu-id="af7ee-142">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="af7ee-143">Soubory pro odsouhlasení itemize podle partnera</span><span class="sxs-lookup"><span data-stu-id="af7ee-143">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="af7ee-144">Partneři v **nepřímém modelu** můžou použít tato další pole v souborech pro odsouhlasení založené na licencích i na základě využití k itemizeí souborů podle prodejce.</span><span class="sxs-lookup"><span data-stu-id="af7ee-144">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="af7ee-145">ID MPN</span><span class="sxs-lookup"><span data-stu-id="af7ee-145">MPN ID</span></span> | <span data-ttu-id="af7ee-146">Popis</span><span class="sxs-lookup"><span data-stu-id="af7ee-146">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="af7ee-147">ID MPN</span><span class="sxs-lookup"><span data-stu-id="af7ee-147">MPN ID</span></span> | <span data-ttu-id="af7ee-148">Identifikátor Microsoft Partner Network (MPN) pro partnera poskytovatele Cloud Solution Provider (CSP) (přímý nebo nepřímý).</span><span class="sxs-lookup"><span data-stu-id="af7ee-148">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="af7ee-149">ID MPN prodejce</span><span class="sxs-lookup"><span data-stu-id="af7ee-149">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="af7ee-150">[Identifikátor MPN prodejce záznamu pro předplatné](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="af7ee-150">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="af7ee-151">Toto pole odpovídá ID prodejce uvedeného u konkrétního předplatného v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="af7ee-151">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="af7ee-152">Zobrazí se pouze v souborech pro odsouhlasení pro partnery v nepřímém modelu.</span><span class="sxs-lookup"><span data-stu-id="af7ee-152">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="af7ee-153">ID MPN prodejce</span><span class="sxs-lookup"><span data-stu-id="af7ee-153">Reseller MPN ID</span></span>

<span data-ttu-id="af7ee-154">Pokud partner CSP prodal předplatné přímo zákazníkovi, jejich **ID MPN** se uvádí dvakrát, jak **ID MPN** , tak **ID programu MPN prodejce**.</span><span class="sxs-lookup"><span data-stu-id="af7ee-154">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="af7ee-155">Pokud má partner CSP prodejce bez **ID MPN**, tato hodnota se místo toho nastaví na **ID MPN** partnera.</span><span class="sxs-lookup"><span data-stu-id="af7ee-155">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="af7ee-156">Pokud partner CSP odebere ID programu **MPN pro prodejce**, tato hodnota se nastaví na hodnotu *-1*.</span><span class="sxs-lookup"><span data-stu-id="af7ee-156">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="af7ee-157">Zobrazení nebo aktualizace **ID MPN prodejce**:</span><span class="sxs-lookup"><span data-stu-id="af7ee-157">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="af7ee-158">Přihlaste se do Partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="af7ee-158">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="af7ee-159">V nabídce partnerské Centrum vyberte **zákazníci**.</span><span class="sxs-lookup"><span data-stu-id="af7ee-159">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="af7ee-160">Vyberte zákazníka ze seznamu.</span><span class="sxs-lookup"><span data-stu-id="af7ee-160">Choose the customer from the list.</span></span>
4. <span data-ttu-id="af7ee-161">V nabídce zákazník vyberte **odběry**.</span><span class="sxs-lookup"><span data-stu-id="af7ee-161">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="af7ee-162">Vyberte předplatné ze seznamu.</span><span class="sxs-lookup"><span data-stu-id="af7ee-162">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="af7ee-163">Pokud chcete změnit **prodejce (MPN ID)**, vyberte **aktualizovat** .</span><span class="sxs-lookup"><span data-stu-id="af7ee-163">Select **update** to change the **Reseller (MPN ID)**.</span></span>