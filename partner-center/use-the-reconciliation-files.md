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
ms.openlocfilehash: 755881d0bd96b9d601346ebb6271bd524c31d0a3
ms.sourcegitcommit: 837d3c5b52ab056b2b761cd85eb2426f56b62614
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/12/2021
ms.locfileid: "109794951"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="08efd-103">Přečtěte si, jak číst položky řádků v souborech odsouhlasení partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="08efd-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="08efd-104">**Příslušné role**: správce fakturace | Globální správce</span><span class="sxs-lookup"><span data-stu-id="08efd-104">**Appropriate roles**: Billing admin | Global admin</span></span>

<span data-ttu-id="08efd-105">Soubory pro odsouhlasení si můžete stáhnout z partnerského centra, kde najdete podrobné zobrazení položek jednotlivých poplatků v rámci fakturačního cyklu.</span><span class="sxs-lookup"><span data-stu-id="08efd-105">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="08efd-106">Podrobnosti o položkách na řádcích zahrnují poplatky za předplatné každého zákazníka a podrobné události (například přidání licencí do předplatného).</span><span class="sxs-lookup"><span data-stu-id="08efd-106">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="08efd-107">Informace o tom, jak si **fakturu** přečíst, najdete v tématu [Přečtěte si vyúčtování](read-your-bill.md).</span><span class="sxs-lookup"><span data-stu-id="08efd-107">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="08efd-108">Vysvětlení polí souboru odsouhlasení</span><span class="sxs-lookup"><span data-stu-id="08efd-108">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="08efd-109">Pole v souboru s vyrovnáním na základě licencí</span><span class="sxs-lookup"><span data-stu-id="08efd-109">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="08efd-110">Pole v souboru s vyrovnáním na základě využití</span><span class="sxs-lookup"><span data-stu-id="08efd-110">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="08efd-111">Pole v souboru s vyrovnáním využití podle denní sazby</span><span class="sxs-lookup"><span data-stu-id="08efd-111">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="08efd-112">Pole souborů odsouhlasení zprostředkovatele CSP v jednom čase</span><span class="sxs-lookup"><span data-stu-id="08efd-112">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="08efd-113">Pochopení typů poplatků v souborech pro odsouhlasení</span><span class="sxs-lookup"><span data-stu-id="08efd-113">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="08efd-114">Chcete-li pochopit typy poplatků v souborech pro odsouhlasení (sloupec **ChargeType** ), podívejte se na téma [odsouhlasení typů poplatků za soubor](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="08efd-114">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="08efd-115">Opravit problémy s formátováním</span><span class="sxs-lookup"><span data-stu-id="08efd-115">Fix formatting issues</span></span>

<span data-ttu-id="08efd-116">V některých případech může soubor pro odsouhlasení obsahovat problémy s formátováním.</span><span class="sxs-lookup"><span data-stu-id="08efd-116">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="08efd-117">K tomuto problému může dojít například v případě, že se národní prostředí en-US nepoužívá.</span><span class="sxs-lookup"><span data-stu-id="08efd-117">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="08efd-118">Pomocí těchto kroků opravíte všechny problémy formátování souborů odsouhlasení:</span><span class="sxs-lookup"><span data-stu-id="08efd-118">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="08efd-119">Otevřete soubor pro odsouhlasení (ve formátu CSV) v aplikaci Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="08efd-119">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="08efd-120">Vyberte první sloupec v souboru.</span><span class="sxs-lookup"><span data-stu-id="08efd-120">Select the first column in the file.</span></span>
3. <span data-ttu-id="08efd-121">Otevřete **Průvodce převodem textu na sloupce**.</span><span class="sxs-lookup"><span data-stu-id="08efd-121">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="08efd-122">Na pásu karet vyberte **data** a pak vyberte **text do sloupců**.</span><span class="sxs-lookup"><span data-stu-id="08efd-122">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="08efd-123">V průvodci vyberte **typ souboru s oddělovači**.</span><span class="sxs-lookup"><span data-stu-id="08efd-123">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="08efd-124">Pak vyberte **Další.**</span><span class="sxs-lookup"><span data-stu-id="08efd-124">Then, select **Next**.</span></span>
5. <span data-ttu-id="08efd-125">V **poli Oddělovače** vyberte **Čárka**.</span><span class="sxs-lookup"><span data-stu-id="08efd-125">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="08efd-126">(Pokud **je už** vybraná karta Tabulátor, můžete tuto možnost ponechat vybranou.) Pak vyberte **Další.**</span><span class="sxs-lookup"><span data-stu-id="08efd-126">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="08efd-127">V **poli Formát dat sloupce** vyberte **Date:MDY**.</span><span class="sxs-lookup"><span data-stu-id="08efd-127">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="08efd-128">Pak vyberte **Další.**</span><span class="sxs-lookup"><span data-stu-id="08efd-128">Then, select **Next**.</span></span>
7. <span data-ttu-id="08efd-129">V poli **Formát dat sloupce** vyberte Text **pro** všechny sloupce s množstvím dat.</span><span class="sxs-lookup"><span data-stu-id="08efd-129">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="08efd-130">Pak vyberte **Finish** (Dokončit).</span><span class="sxs-lookup"><span data-stu-id="08efd-130">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="08efd-131">Stažení souborů s vyrovnáním prostřednictvím kódu programu</span><span class="sxs-lookup"><span data-stu-id="08efd-131">Download reconciliation files programmatically</span></span>

<span data-ttu-id="08efd-132">Soubory pro sesouhlasení mohou být velmi velké a někdy se obtížně stahují.</span><span class="sxs-lookup"><span data-stu-id="08efd-132">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="08efd-133">Pokud chcete stáhnout soubory s vyrovnáním prostřednictvím kódu programu, podívejte se [na stránku Získání řádových položek faktury.](/partner-center/develop/get-invoiceline-items)</span><span class="sxs-lookup"><span data-stu-id="08efd-133">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a><span data-ttu-id="08efd-134">Pokud váš soubor překročí limit řádku v Excelu</span><span class="sxs-lookup"><span data-stu-id="08efd-134">If your file exceeds the row limit in Excel</span></span>

<span data-ttu-id="08efd-135">Pokud si můžete stáhnout soubor s vyrovnáním, ale v Microsoft Excelu ho neotevřete, pravděpodobně to znamená, že soubor obsahuje více řádků, než Excel povolí.</span><span class="sxs-lookup"><span data-stu-id="08efd-135">If you’re able to download a reconciliation file but not open it in Microsoft Excel, it probably means the file contains more rows than Excel will allow.</span></span> <span data-ttu-id="08efd-136">Pokud k tomu dojde, můžete soubor otevřít pomocí jednoho z následujících postupů.</span><span class="sxs-lookup"><span data-stu-id="08efd-136">If this happens, you can use either of the procedures below to open the file.</span></span>

### <a name="open-a-recon-file-in-power-bi"></a><span data-ttu-id="08efd-137">Otevřete soubor odsoustavy v Power BI</span><span class="sxs-lookup"><span data-stu-id="08efd-137">Open a recon file in Power BI</span></span>

1. <span data-ttu-id="08efd-138">Stáhněte si soubor s vyrovnáním běžným způsobem.</span><span class="sxs-lookup"><span data-stu-id="08efd-138">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="08efd-139">Stáhněte, nainstalujte a otevřete instanci Power BI.</span><span class="sxs-lookup"><span data-stu-id="08efd-139">Download, install, and open an instance of Power BI.</span></span>
3. <span data-ttu-id="08efd-140">Na Power BI **Domů** vyberte Získat **data**.</span><span class="sxs-lookup"><span data-stu-id="08efd-140">On the Power BI **Home** tab, select **Get data**.</span></span>
4. <span data-ttu-id="08efd-141">V seznamu **Běžných zdrojů dat** vyberte **Text/CSV.**</span><span class="sxs-lookup"><span data-stu-id="08efd-141">In the list of **Common data sources**, select **Text/CSV**.</span></span>
5. <span data-ttu-id="08efd-142">Po zobrazení výzvy otevřete soubor odsoustavy.</span><span class="sxs-lookup"><span data-stu-id="08efd-142">When prompted, open your recon file.</span></span>

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a><span data-ttu-id="08efd-143">Otevření souboru s rekonsekcemi v excelové kontingenční tabulce</span><span class="sxs-lookup"><span data-stu-id="08efd-143">Open a recon file in an Excel pivot table</span></span>

1. <span data-ttu-id="08efd-144">Stáhněte si soubor s vyrovnáním běžným způsobem.</span><span class="sxs-lookup"><span data-stu-id="08efd-144">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="08efd-145">Otevřete nový soubor v aplikaci Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="08efd-145">Open a new file in Microsoft Excel.</span></span>
3. <span data-ttu-id="08efd-146">Na kartě **data** vyberte **získat data**, vyberte **ze souboru** a pak vyberte **text/CSV**.</span><span class="sxs-lookup"><span data-stu-id="08efd-146">On the **Data** tab, select **Get data**, select **From file**, and then select **Text/CSV**.</span></span>
4. <span data-ttu-id="08efd-147">Po zobrazení výzvy otevřete soubor rekognoskaci.</span><span class="sxs-lookup"><span data-stu-id="08efd-147">When prompted, open your recon file.</span></span> <span data-ttu-id="08efd-148">Vaše data se zobrazí.</span><span class="sxs-lookup"><span data-stu-id="08efd-148">Your data will appear.</span></span>
5. <span data-ttu-id="08efd-149">V rozevírací nabídce **načíst** vyberte **načíst do** a pak **OK**.</span><span class="sxs-lookup"><span data-stu-id="08efd-149">In the **Load** dropdown menu, select **Load to**, and then **OK**.</span></span>
6. <span data-ttu-id="08efd-150">V dialogovém okně **importovat data** vyberte **sestavu kontingenční tabulka** a otevřete soubor.</span><span class="sxs-lookup"><span data-stu-id="08efd-150">In the **Import Data** dialog box, select **PivotTable Report** to open your file.</span></span>

## <a name="negative-amount-displayed"></a><span data-ttu-id="08efd-151">Zobrazená záporná částka</span><span class="sxs-lookup"><span data-stu-id="08efd-151">Negative amount displayed</span></span>

<span data-ttu-id="08efd-152">V souboru pro odsouhlasení se může zobrazit záporná částka.</span><span class="sxs-lookup"><span data-stu-id="08efd-152">You may see a negative amount in your reconciliation file.</span></span> <span data-ttu-id="08efd-153">Pravděpodobně to má jednu z následujících příčin:</span><span class="sxs-lookup"><span data-stu-id="08efd-153">This is probably caused by one of the following things:</span></span>

- <span data-ttu-id="08efd-154">Nedávno jste zrušili nebo snížili počet licencí.</span><span class="sxs-lookup"><span data-stu-id="08efd-154">You recently canceled or reduced your number of licenses</span></span>
- <span data-ttu-id="08efd-155">Dostali jste kredit pro licenční smlouvu o úrovni služeb (SLA) nebo pro využití Azure.</span><span class="sxs-lookup"><span data-stu-id="08efd-155">You received credit for either a service license agreement (SLA) or for Azure consumption</span></span>

<span data-ttu-id="08efd-156">Pokud chcete o této transakci získat další informace, zkontrolujte v souboru s vyrovnáním příslušný atribut typu poplatku.</span><span class="sxs-lookup"><span data-stu-id="08efd-156">To get more information about this transaction, review its charge type attribute in your reconciliation file.</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="08efd-157">Mapování daní nebo DPH</span><span class="sxs-lookup"><span data-stu-id="08efd-157">Map taxes or VAT</span></span>

<span data-ttu-id="08efd-158">K namapování daně nebo daně z přidané hodnoty (DPH) na fakturu:</span><span class="sxs-lookup"><span data-stu-id="08efd-158">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="08efd-159">Sečtěte sloupec **daně** ze souboru založeného na licencích.</span><span class="sxs-lookup"><span data-stu-id="08efd-159">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="08efd-160">Sečtěte sloupec **TaxAmount** ze souboru založeného na využití.</span><span class="sxs-lookup"><span data-stu-id="08efd-160">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="08efd-161">Soubory pro odsouhlasení itemize podle partnera</span><span class="sxs-lookup"><span data-stu-id="08efd-161">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="08efd-162">Partneři v **nepřímém modelu** můžou použít tato další pole v souborech pro odsouhlasení založené na licencích i na základě využití k itemizeí souborů podle prodejce.</span><span class="sxs-lookup"><span data-stu-id="08efd-162">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="08efd-163">ID MPN</span><span class="sxs-lookup"><span data-stu-id="08efd-163">MPN ID</span></span> | <span data-ttu-id="08efd-164">Description</span><span class="sxs-lookup"><span data-stu-id="08efd-164">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="08efd-165">ID MPN</span><span class="sxs-lookup"><span data-stu-id="08efd-165">MPN ID</span></span> | <span data-ttu-id="08efd-166">Identifikátor Microsoft Partner Network (MPN) pro partnera poskytovatele Cloud Solution Provider (CSP) (přímý nebo nepřímý).</span><span class="sxs-lookup"><span data-stu-id="08efd-166">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="08efd-167">ID MPN prodejce</span><span class="sxs-lookup"><span data-stu-id="08efd-167">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="08efd-168">[Identifikátor MPN prodejce záznamu pro předplatné](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="08efd-168">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="08efd-169">Toto pole odpovídá ID prodejce uvedeného u konkrétního předplatného v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="08efd-169">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="08efd-170">Zobrazuje se jenom v souborech s vyrovnáním pro partnery v nepřímém modelu.</span><span class="sxs-lookup"><span data-stu-id="08efd-170">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="08efd-171">ID MPN prodejce</span><span class="sxs-lookup"><span data-stu-id="08efd-171">Reseller MPN ID</span></span>

<span data-ttu-id="08efd-172">Pokud partner CSP prodá předplatné přímo zákazníkovi, jeho **ID MPN** se vyjádřuje dvakrát jako **ID MPN** i **ID MPN prodejce**.</span><span class="sxs-lookup"><span data-stu-id="08efd-172">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="08efd-173">Pokud má partner CSP prodejce bez **ID MPN,** nastaví se tato hodnota místo toho na **ID MPN** partnera.</span><span class="sxs-lookup"><span data-stu-id="08efd-173">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="08efd-174">Pokud partner CSP odebere **ID MPN** prodejce, tato hodnota se nastaví *na -1.*</span><span class="sxs-lookup"><span data-stu-id="08efd-174">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="08efd-175">Zobrazení nebo aktualizace **ID MPN prodejce:**</span><span class="sxs-lookup"><span data-stu-id="08efd-175">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="08efd-176">Přihlaste se do Partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="08efd-176">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="08efd-177">V nabídce Partnerské centrum vyberte **Zákazníci.**</span><span class="sxs-lookup"><span data-stu-id="08efd-177">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="08efd-178">V seznamu vyberte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="08efd-178">Choose the customer from the list.</span></span>
4. <span data-ttu-id="08efd-179">V nabídce zákazníka vyberte **Předplatná.**</span><span class="sxs-lookup"><span data-stu-id="08efd-179">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="08efd-180">V seznamu vyberte předplatné.</span><span class="sxs-lookup"><span data-stu-id="08efd-180">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="08efd-181">Výběrem **možnosti** Aktualizovat **změňte reseller (MPN ID).**</span><span class="sxs-lookup"><span data-stu-id="08efd-181">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="08efd-182">Další kroky</span><span class="sxs-lookup"><span data-stu-id="08efd-182">Next steps</span></span>

- [<span data-ttu-id="08efd-183">Čtení souboru s vyúčtováním & odsoustavy</span><span class="sxs-lookup"><span data-stu-id="08efd-183">How to read your bill & recon file</span></span>](read-your-bill.md) 