---
title: Použití souborů odsouhlasení
ms.topic: article
ms.date: 03/26/2021
description: Přečtěte si informace o souborech pro odsouhlasení v partnerském centru a o tom, jak interpretovat detailní zobrazení položek poplatků za daný fakturační cyklus.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4a6a1455304f12e364d71e666cbd548821f8be55
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633892"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="7e556-103">Přečtěte si, jak číst položky řádků v souborech odsouhlasení partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="7e556-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="7e556-104">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="7e556-104">**Appropriate roles**</span></span>

- <span data-ttu-id="7e556-105">Správce fakturace</span><span class="sxs-lookup"><span data-stu-id="7e556-105">Billing admin</span></span>
- <span data-ttu-id="7e556-106">Globální správce</span><span class="sxs-lookup"><span data-stu-id="7e556-106">Global admin</span></span>

<span data-ttu-id="7e556-107">Soubory pro odsouhlasení si můžete stáhnout z partnerského centra, kde najdete podrobné zobrazení položek jednotlivých poplatků v rámci fakturačního cyklu.</span><span class="sxs-lookup"><span data-stu-id="7e556-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="7e556-108">Podrobnosti o položkách na řádcích zahrnují poplatky za předplatné každého zákazníka a podrobné události (například přidání licencí do předplatného).</span><span class="sxs-lookup"><span data-stu-id="7e556-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="7e556-109">Informace o tom, jak si **fakturu** přečíst, najdete v tématu [Přečtěte si vyúčtování](read-your-bill.md).</span><span class="sxs-lookup"><span data-stu-id="7e556-109">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="7e556-110">Vysvětlení polí souboru odsouhlasení</span><span class="sxs-lookup"><span data-stu-id="7e556-110">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="7e556-111">Pole v souboru s vyrovnáním na základě licencí</span><span class="sxs-lookup"><span data-stu-id="7e556-111">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="7e556-112">Pole v souboru s vyrovnáním na základě využití</span><span class="sxs-lookup"><span data-stu-id="7e556-112">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="7e556-113">Pole v souboru s vyrovnáním využití podle denní sazby</span><span class="sxs-lookup"><span data-stu-id="7e556-113">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="7e556-114">Pole souborů odsouhlasení zprostředkovatele CSP v jednom čase</span><span class="sxs-lookup"><span data-stu-id="7e556-114">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="7e556-115">Pochopení typů poplatků v souborech pro odsouhlasení</span><span class="sxs-lookup"><span data-stu-id="7e556-115">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="7e556-116">Chcete-li pochopit typy poplatků v souborech pro odsouhlasení (sloupec **ChargeType** ), podívejte se na téma [odsouhlasení typů poplatků za soubor](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="7e556-116">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="7e556-117">Opravit problémy s formátováním</span><span class="sxs-lookup"><span data-stu-id="7e556-117">Fix formatting issues</span></span>

<span data-ttu-id="7e556-118">V některých případech může soubor pro odsouhlasení obsahovat problémy s formátováním.</span><span class="sxs-lookup"><span data-stu-id="7e556-118">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="7e556-119">K tomuto problému může dojít například v případě, že se národní prostředí en-US nepoužívá.</span><span class="sxs-lookup"><span data-stu-id="7e556-119">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="7e556-120">Pomocí těchto kroků opravíte všechny problémy formátování souborů odsouhlasení:</span><span class="sxs-lookup"><span data-stu-id="7e556-120">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="7e556-121">Otevřete soubor pro odsouhlasení (ve formátu CSV) v aplikaci Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="7e556-121">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="7e556-122">Vyberte první sloupec v souboru.</span><span class="sxs-lookup"><span data-stu-id="7e556-122">Select the first column in the file.</span></span>
3. <span data-ttu-id="7e556-123">Otevřete **Průvodce převodem textu na sloupce**.</span><span class="sxs-lookup"><span data-stu-id="7e556-123">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="7e556-124">Na pásu karet vyberte **data** a pak vyberte **text do sloupců**.</span><span class="sxs-lookup"><span data-stu-id="7e556-124">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="7e556-125">V průvodci vyberte **typ souboru s oddělovači**.</span><span class="sxs-lookup"><span data-stu-id="7e556-125">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="7e556-126">Pak vyberte **Další**.</span><span class="sxs-lookup"><span data-stu-id="7e556-126">Then, select **Next**.</span></span>
5. <span data-ttu-id="7e556-127">V poli **oddělovače** vyberte **čárka**.</span><span class="sxs-lookup"><span data-stu-id="7e556-127">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="7e556-128">(Pokud je už vybraná **karta** , můžete tuto možnost nechat vybranou.) Pak vyberte **Další**.</span><span class="sxs-lookup"><span data-stu-id="7e556-128">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="7e556-129">V poli **Formát dat sloupce** vyberte **Datum: MDY**.</span><span class="sxs-lookup"><span data-stu-id="7e556-129">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="7e556-130">Pak vyberte **Další**.</span><span class="sxs-lookup"><span data-stu-id="7e556-130">Then, select **Next**.</span></span>
7. <span data-ttu-id="7e556-131">V poli **Formát dat sloupce** vyberte možnost **text** pro sloupce všech částek.</span><span class="sxs-lookup"><span data-stu-id="7e556-131">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="7e556-132">Pak vyberte **Finish** (Dokončit).</span><span class="sxs-lookup"><span data-stu-id="7e556-132">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="7e556-133">Stažení souborů pro odsouhlasení programově</span><span class="sxs-lookup"><span data-stu-id="7e556-133">Download reconciliation files programmatically</span></span>

<span data-ttu-id="7e556-134">Soubory pro odsouhlasení můžou být velmi velké a někdy je obtížné stáhnout.</span><span class="sxs-lookup"><span data-stu-id="7e556-134">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="7e556-135">Chcete-li stáhnout soubory pro odsouhlasení programově, viz [získat řádky faktury](/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="7e556-135">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a><span data-ttu-id="7e556-136">Pokud soubor překračuje limit řádků v aplikaci Excel</span><span class="sxs-lookup"><span data-stu-id="7e556-136">If your file exceeds the row limit in Excel</span></span>

<span data-ttu-id="7e556-137">Pokud si můžete stáhnout soubor pro odsouhlasení, ale nemůžete ho otevřít v Microsoft Excelu, pravděpodobně to znamená, že soubor obsahuje více řádků, než je Excel bude možné použít.</span><span class="sxs-lookup"><span data-stu-id="7e556-137">If you’re able to download a reconciliation file but not open it in Microsoft Excel, it probably means the file contains more rows than Excel will allow.</span></span> <span data-ttu-id="7e556-138">Pokud k tomu dojde, můžete použít kterýkoli z následujících postupů k otevření souboru.</span><span class="sxs-lookup"><span data-stu-id="7e556-138">If this happens, you can use either of the procedures below to open the file.</span></span>

### <a name="open-a-recon-file-in-power-bi"></a><span data-ttu-id="7e556-139">Otevřete soubor rekognoskaci v Power BI</span><span class="sxs-lookup"><span data-stu-id="7e556-139">Open a recon file in Power BI</span></span>

1. <span data-ttu-id="7e556-140">Stáhněte soubor pro odsouhlasení obvyklým způsobem.</span><span class="sxs-lookup"><span data-stu-id="7e556-140">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="7e556-141">Stáhněte, nainstalujte a otevřete instanci Power BI.</span><span class="sxs-lookup"><span data-stu-id="7e556-141">Download, install, and open an instance of Power BI.</span></span>
3. <span data-ttu-id="7e556-142">Na kartě Power BI **Domů** vyberte **získat data**.</span><span class="sxs-lookup"><span data-stu-id="7e556-142">On the Power BI **Home** tab, select **Get data**.</span></span>
4. <span data-ttu-id="7e556-143">V seznamu **běžných zdrojů dat** vyberte **text/CSV**.</span><span class="sxs-lookup"><span data-stu-id="7e556-143">In the list of **Common data sources**, select **Text/CSV**.</span></span>
5. <span data-ttu-id="7e556-144">Po zobrazení výzvy otevřete soubor rekognoskaci.</span><span class="sxs-lookup"><span data-stu-id="7e556-144">When prompted, open your recon file.</span></span>

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a><span data-ttu-id="7e556-145">Otevření souboru rekognoskaci v kontingenční tabulce aplikace Excel</span><span class="sxs-lookup"><span data-stu-id="7e556-145">Open a recon file in an Excel pivot table</span></span>

1. <span data-ttu-id="7e556-146">Stáhněte soubor pro odsouhlasení obvyklým způsobem.</span><span class="sxs-lookup"><span data-stu-id="7e556-146">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="7e556-147">Otevřete nový soubor v aplikaci Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="7e556-147">Open a new file in Microsoft Excel.</span></span>
3. <span data-ttu-id="7e556-148">Na kartě **data** vyberte **získat data**, vyberte **ze souboru** a pak vyberte **text/CSV**.</span><span class="sxs-lookup"><span data-stu-id="7e556-148">On the **Data** tab, select **Get data**, select **From file**, and then select **Text/CSV**.</span></span>
4. <span data-ttu-id="7e556-149">Po zobrazení výzvy otevřete soubor rekognoskaci.</span><span class="sxs-lookup"><span data-stu-id="7e556-149">When prompted, open your recon file.</span></span> <span data-ttu-id="7e556-150">Vaše data se zobrazí.</span><span class="sxs-lookup"><span data-stu-id="7e556-150">Your data will appear.</span></span>
5. <span data-ttu-id="7e556-151">V rozevírací nabídce **načíst** vyberte **načíst do** a pak **OK**.</span><span class="sxs-lookup"><span data-stu-id="7e556-151">In the **Load** dropdown menu, select **Load to**, and then **OK**.</span></span>
6. <span data-ttu-id="7e556-152">V dialogovém okně **importovat data** vyberte **sestavu kontingenční tabulka** a otevřete soubor.</span><span class="sxs-lookup"><span data-stu-id="7e556-152">In the **Import Data** dialog box, select **PivotTable Report** to open your file.</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="7e556-153">Mapování daní nebo DPH</span><span class="sxs-lookup"><span data-stu-id="7e556-153">Map taxes or VAT</span></span>

<span data-ttu-id="7e556-154">K namapování daně nebo daně z přidané hodnoty (DPH) na fakturu:</span><span class="sxs-lookup"><span data-stu-id="7e556-154">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="7e556-155">Sečtěte sloupec **daně** ze souboru založeného na licencích.</span><span class="sxs-lookup"><span data-stu-id="7e556-155">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="7e556-156">Sečtěte sloupec **TaxAmount** ze souboru založeného na využití.</span><span class="sxs-lookup"><span data-stu-id="7e556-156">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="7e556-157">Soubory pro odsouhlasení itemize podle partnera</span><span class="sxs-lookup"><span data-stu-id="7e556-157">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="7e556-158">Partneři v **nepřímém modelu** můžou použít tato další pole v souborech pro odsouhlasení založené na licencích i na základě využití k itemizeí souborů podle prodejce.</span><span class="sxs-lookup"><span data-stu-id="7e556-158">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="7e556-159">ID MPN</span><span class="sxs-lookup"><span data-stu-id="7e556-159">MPN ID</span></span> | <span data-ttu-id="7e556-160">Description</span><span class="sxs-lookup"><span data-stu-id="7e556-160">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="7e556-161">ID MPN</span><span class="sxs-lookup"><span data-stu-id="7e556-161">MPN ID</span></span> | <span data-ttu-id="7e556-162">Identifikátor Microsoft Partner Network (MPN) pro partnera poskytovatele Cloud Solution Provider (CSP) (přímý nebo nepřímý).</span><span class="sxs-lookup"><span data-stu-id="7e556-162">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="7e556-163">ID MPN prodejce</span><span class="sxs-lookup"><span data-stu-id="7e556-163">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="7e556-164">[Identifikátor MPN prodejce záznamu pro předplatné](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="7e556-164">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="7e556-165">Toto pole odpovídá ID prodejce uvedeného u konkrétního předplatného v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="7e556-165">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="7e556-166">Zobrazí se pouze v souborech pro odsouhlasení pro partnery v nepřímém modelu.</span><span class="sxs-lookup"><span data-stu-id="7e556-166">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="7e556-167">ID MPN prodejce</span><span class="sxs-lookup"><span data-stu-id="7e556-167">Reseller MPN ID</span></span>

<span data-ttu-id="7e556-168">Pokud partner CSP prodal předplatné přímo zákazníkovi, jejich **ID MPN** se uvádí dvakrát, jak **ID MPN** , tak **ID programu MPN prodejce**.</span><span class="sxs-lookup"><span data-stu-id="7e556-168">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="7e556-169">Pokud má partner CSP prodejce bez **ID MPN**, tato hodnota se místo toho nastaví na **ID MPN** partnera.</span><span class="sxs-lookup"><span data-stu-id="7e556-169">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="7e556-170">Pokud partner CSP odebere ID programu **MPN pro prodejce**, tato hodnota se nastaví na hodnotu *-1*.</span><span class="sxs-lookup"><span data-stu-id="7e556-170">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="7e556-171">Zobrazení nebo aktualizace **ID MPN prodejce**:</span><span class="sxs-lookup"><span data-stu-id="7e556-171">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="7e556-172">Přihlaste se do Partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="7e556-172">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="7e556-173">V nabídce partnerské Centrum vyberte **zákazníci**.</span><span class="sxs-lookup"><span data-stu-id="7e556-173">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="7e556-174">Vyberte zákazníka ze seznamu.</span><span class="sxs-lookup"><span data-stu-id="7e556-174">Choose the customer from the list.</span></span>
4. <span data-ttu-id="7e556-175">V nabídce zákazník vyberte **odběry**.</span><span class="sxs-lookup"><span data-stu-id="7e556-175">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="7e556-176">Vyberte předplatné ze seznamu.</span><span class="sxs-lookup"><span data-stu-id="7e556-176">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="7e556-177">Pokud chcete změnit **prodejce (MPN ID)**, vyberte **aktualizovat** .</span><span class="sxs-lookup"><span data-stu-id="7e556-177">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="7e556-178">Další kroky</span><span class="sxs-lookup"><span data-stu-id="7e556-178">Next steps</span></span>

- [<span data-ttu-id="7e556-179">Postup čtení souboru rekognoskaci vy& účtování</span><span class="sxs-lookup"><span data-stu-id="7e556-179">How to read your bill & recon file</span></span>](read-your-bill.md) 