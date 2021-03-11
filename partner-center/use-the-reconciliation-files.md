---
title: Použití souborů odsouhlasení
ms.topic: article
ms.date: 03/10/2021
description: Přečtěte si informace o souborech pro odsouhlasení v partnerském centru a o tom, jak interpretovat detailní zobrazení položek poplatků za daný fakturační cyklus.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e6b9e466402d71c988729052bd72ba2346a9d977
ms.sourcegitcommit: 868f90c54f26a037eee29749c207a7316bb4b475
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/11/2021
ms.locfileid: "103022770"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="137e1-103">Přečtěte si, jak číst položky řádků v souborech odsouhlasení partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="137e1-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="137e1-104">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="137e1-104">**Appropriate roles**</span></span>

- <span data-ttu-id="137e1-105">Správce fakturace</span><span class="sxs-lookup"><span data-stu-id="137e1-105">Billing admin</span></span>
- <span data-ttu-id="137e1-106">Globální správce</span><span class="sxs-lookup"><span data-stu-id="137e1-106">Global admin</span></span>

<span data-ttu-id="137e1-107">Soubory pro odsouhlasení si můžete stáhnout z partnerského centra, kde najdete podrobné zobrazení položek jednotlivých poplatků v rámci fakturačního cyklu.</span><span class="sxs-lookup"><span data-stu-id="137e1-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="137e1-108">Podrobnosti o položkách na řádcích zahrnují poplatky za předplatné každého zákazníka a podrobné události (například přidání licencí do předplatného).</span><span class="sxs-lookup"><span data-stu-id="137e1-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="137e1-109">Informace o tom, jak si **fakturu** přečíst, najdete v tématu [Přečtěte si vyúčtování](read-your-bill.md).</span><span class="sxs-lookup"><span data-stu-id="137e1-109">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="137e1-110">Vysvětlení polí souboru odsouhlasení</span><span class="sxs-lookup"><span data-stu-id="137e1-110">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="137e1-111">Pole v souboru s vyrovnáním na základě licencí</span><span class="sxs-lookup"><span data-stu-id="137e1-111">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="137e1-112">Pole v souboru s vyrovnáním na základě využití</span><span class="sxs-lookup"><span data-stu-id="137e1-112">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="137e1-113">Pole v souboru s vyrovnáním využití podle denní sazby</span><span class="sxs-lookup"><span data-stu-id="137e1-113">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="137e1-114">Pole souborů odsouhlasení zprostředkovatele CSP v jednom čase</span><span class="sxs-lookup"><span data-stu-id="137e1-114">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="137e1-115">Pochopení typů poplatků v souborech pro odsouhlasení</span><span class="sxs-lookup"><span data-stu-id="137e1-115">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="137e1-116">Chcete-li pochopit typy poplatků v souborech pro odsouhlasení (sloupec **ChargeType** ), podívejte se na téma [odsouhlasení typů poplatků za soubor](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="137e1-116">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="137e1-117">Opravit problémy s formátováním</span><span class="sxs-lookup"><span data-stu-id="137e1-117">Fix formatting issues</span></span>

<span data-ttu-id="137e1-118">V některých případech může soubor pro odsouhlasení obsahovat problémy s formátováním.</span><span class="sxs-lookup"><span data-stu-id="137e1-118">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="137e1-119">K tomuto problému může dojít například v případě, že se národní prostředí en-US nepoužívá.</span><span class="sxs-lookup"><span data-stu-id="137e1-119">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="137e1-120">Pomocí těchto kroků opravíte všechny problémy formátování souborů odsouhlasení:</span><span class="sxs-lookup"><span data-stu-id="137e1-120">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="137e1-121">Otevřete soubor pro odsouhlasení (ve formátu CSV) v aplikaci Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="137e1-121">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="137e1-122">Vyberte první sloupec v souboru.</span><span class="sxs-lookup"><span data-stu-id="137e1-122">Select the first column in the file.</span></span>
3. <span data-ttu-id="137e1-123">Otevřete **Průvodce převodem textu na sloupce**.</span><span class="sxs-lookup"><span data-stu-id="137e1-123">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="137e1-124">Na pásu karet vyberte **data** a pak vyberte **text do sloupců**.</span><span class="sxs-lookup"><span data-stu-id="137e1-124">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="137e1-125">V průvodci vyberte **typ souboru s oddělovači**.</span><span class="sxs-lookup"><span data-stu-id="137e1-125">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="137e1-126">Pak vyberte **Další**.</span><span class="sxs-lookup"><span data-stu-id="137e1-126">Then, select **Next**.</span></span>
5. <span data-ttu-id="137e1-127">V poli **oddělovače** vyberte **čárka**.</span><span class="sxs-lookup"><span data-stu-id="137e1-127">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="137e1-128">(Pokud je už vybraná **karta** , můžete tuto možnost nechat vybranou.) Pak vyberte **Další**.</span><span class="sxs-lookup"><span data-stu-id="137e1-128">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="137e1-129">V poli **Formát dat sloupce** vyberte **Datum: MDY**.</span><span class="sxs-lookup"><span data-stu-id="137e1-129">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="137e1-130">Pak vyberte **Další**.</span><span class="sxs-lookup"><span data-stu-id="137e1-130">Then, select **Next**.</span></span>
7. <span data-ttu-id="137e1-131">V poli **Formát dat sloupce** vyberte možnost **text** pro sloupce všech částek.</span><span class="sxs-lookup"><span data-stu-id="137e1-131">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="137e1-132">Pak vyberte **Finish** (Dokončit).</span><span class="sxs-lookup"><span data-stu-id="137e1-132">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="137e1-133">Stažení souborů pro odsouhlasení programově</span><span class="sxs-lookup"><span data-stu-id="137e1-133">Download reconciliation files programmatically</span></span>

<span data-ttu-id="137e1-134">Soubory pro odsouhlasení můžou být velmi velké a někdy je obtížné stáhnout.</span><span class="sxs-lookup"><span data-stu-id="137e1-134">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="137e1-135">Chcete-li stáhnout soubory pro odsouhlasení programově, viz [získat řádky faktury](/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="137e1-135">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="137e1-136">Mapování daní nebo DPH</span><span class="sxs-lookup"><span data-stu-id="137e1-136">Map taxes or VAT</span></span>

<span data-ttu-id="137e1-137">K namapování daně nebo daně z přidané hodnoty (DPH) na fakturu:</span><span class="sxs-lookup"><span data-stu-id="137e1-137">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="137e1-138">Sečtěte sloupec **daně** ze souboru založeného na licencích.</span><span class="sxs-lookup"><span data-stu-id="137e1-138">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="137e1-139">Sečtěte sloupec **TaxAmount** ze souboru založeného na využití.</span><span class="sxs-lookup"><span data-stu-id="137e1-139">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="137e1-140">Soubory pro odsouhlasení itemize podle partnera</span><span class="sxs-lookup"><span data-stu-id="137e1-140">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="137e1-141">Partneři v **nepřímém modelu** můžou použít tato další pole v souborech pro odsouhlasení založené na licencích i na základě využití k itemizeí souborů podle prodejce.</span><span class="sxs-lookup"><span data-stu-id="137e1-141">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="137e1-142">ID MPN</span><span class="sxs-lookup"><span data-stu-id="137e1-142">MPN ID</span></span> | <span data-ttu-id="137e1-143">Description</span><span class="sxs-lookup"><span data-stu-id="137e1-143">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="137e1-144">ID MPN</span><span class="sxs-lookup"><span data-stu-id="137e1-144">MPN ID</span></span> | <span data-ttu-id="137e1-145">Identifikátor Microsoft Partner Network (MPN) pro partnera poskytovatele Cloud Solution Provider (CSP) (přímý nebo nepřímý).</span><span class="sxs-lookup"><span data-stu-id="137e1-145">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="137e1-146">ID MPN prodejce</span><span class="sxs-lookup"><span data-stu-id="137e1-146">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="137e1-147">[Identifikátor MPN prodejce záznamu pro předplatné](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="137e1-147">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="137e1-148">Toto pole odpovídá ID prodejce uvedeného u konkrétního předplatného v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="137e1-148">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="137e1-149">Zobrazí se pouze v souborech pro odsouhlasení pro partnery v nepřímém modelu.</span><span class="sxs-lookup"><span data-stu-id="137e1-149">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="137e1-150">ID MPN prodejce</span><span class="sxs-lookup"><span data-stu-id="137e1-150">Reseller MPN ID</span></span>

<span data-ttu-id="137e1-151">Pokud partner CSP prodal předplatné přímo zákazníkovi, jejich **ID MPN** se uvádí dvakrát, jak **ID MPN** , tak **ID programu MPN prodejce**.</span><span class="sxs-lookup"><span data-stu-id="137e1-151">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="137e1-152">Pokud má partner CSP prodejce bez **ID MPN**, tato hodnota se místo toho nastaví na **ID MPN** partnera.</span><span class="sxs-lookup"><span data-stu-id="137e1-152">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="137e1-153">Pokud partner CSP odebere ID programu **MPN pro prodejce**, tato hodnota se nastaví na hodnotu *-1*.</span><span class="sxs-lookup"><span data-stu-id="137e1-153">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="137e1-154">Zobrazení nebo aktualizace **ID MPN prodejce**:</span><span class="sxs-lookup"><span data-stu-id="137e1-154">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="137e1-155">Přihlaste se do Partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="137e1-155">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="137e1-156">V nabídce partnerské Centrum vyberte **zákazníci**.</span><span class="sxs-lookup"><span data-stu-id="137e1-156">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="137e1-157">Vyberte zákazníka ze seznamu.</span><span class="sxs-lookup"><span data-stu-id="137e1-157">Choose the customer from the list.</span></span>
4. <span data-ttu-id="137e1-158">V nabídce zákazník vyberte **odběry**.</span><span class="sxs-lookup"><span data-stu-id="137e1-158">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="137e1-159">Vyberte předplatné ze seznamu.</span><span class="sxs-lookup"><span data-stu-id="137e1-159">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="137e1-160">Pokud chcete změnit **prodejce (MPN ID)**, vyberte **aktualizovat** .</span><span class="sxs-lookup"><span data-stu-id="137e1-160">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="137e1-161">Další kroky</span><span class="sxs-lookup"><span data-stu-id="137e1-161">Next steps</span></span>

- [<span data-ttu-id="137e1-162">Postup čtení souboru rekognoskaci vy& účtování</span><span class="sxs-lookup"><span data-stu-id="137e1-162">How to read your bill & recon file</span></span>](read-your-bill.md) 