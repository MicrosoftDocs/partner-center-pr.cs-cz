---
title: Použití souborů s vyrovnáním
ms.topic: article
ms.date: 03/26/2021
description: Přečtěte si o souborech odsouhlasení v Partnerské centrum a o tom, jak interpretovat podrobná zobrazení řádkové položky poplatků za dané fakturační období.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1a7d5f3169c4b338a07475a7e246e87841b8dcfb
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431562"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="5b549-103">Zjistěte, jak číst řádkové položky v souborech Partnerské centrum odsouhlasení.</span><span class="sxs-lookup"><span data-stu-id="5b549-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="5b549-104">**Odpovídající role:** Správce fakturace | Globální správce</span><span class="sxs-lookup"><span data-stu-id="5b549-104">**Appropriate roles**: Billing admin | Global admin</span></span>

<span data-ttu-id="5b549-105">Soubory s vyrovnáním si můžete stáhnout z Partnerské centrum, kde najdete podrobné zobrazení jednotlivých poplatků ve fakturačním cyklu.</span><span class="sxs-lookup"><span data-stu-id="5b549-105">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="5b549-106">Podrobnosti řádkové položky zahrnují poplatky za předplatná jednotlivých zákazníků a podrobné události (například střednědobé přidání licencí k předplatnému).</span><span class="sxs-lookup"><span data-stu-id="5b549-106">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="5b549-107">Informace o tom, jak číst **fakturu, najdete** v [tématu Čtení faktury.](read-your-bill.md)</span><span class="sxs-lookup"><span data-stu-id="5b549-107">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="5b549-108">Principy polí v souboru s vyrovnáním</span><span class="sxs-lookup"><span data-stu-id="5b549-108">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="5b549-109">Pole v souboru s vyrovnáním na základě licencí</span><span class="sxs-lookup"><span data-stu-id="5b549-109">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="5b549-110">Pole v souboru s vyrovnáním na základě využití</span><span class="sxs-lookup"><span data-stu-id="5b549-110">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="5b549-111">Pole v souboru s vyrovnáním využití podle denní sazby</span><span class="sxs-lookup"><span data-stu-id="5b549-111">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="5b549-112">Pole souboru se souborem odsouhlasení CSP pro jeden nákup</span><span class="sxs-lookup"><span data-stu-id="5b549-112">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="5b549-113">Principy typů poplatků v souborech s vyrovnáním</span><span class="sxs-lookup"><span data-stu-id="5b549-113">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="5b549-114">Informace o typech poplatků v souborech s vyrovnáním (sloupec **ChargeType)** najdete v tématu Typy poplatků [za soubor s vyrovnáním.](recon-file-charge-types.md)</span><span class="sxs-lookup"><span data-stu-id="5b549-114">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="5b549-115">Oprava problémů s formátováním</span><span class="sxs-lookup"><span data-stu-id="5b549-115">Fix formatting issues</span></span>

<span data-ttu-id="5b549-116">V některých případech může soubor s vyrovnáním obsahovat problémy s formátováním.</span><span class="sxs-lookup"><span data-stu-id="5b549-116">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="5b549-117">K tomuto problému může dojít například v případě, že není použito národní prostředí en-US.</span><span class="sxs-lookup"><span data-stu-id="5b549-117">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="5b549-118">Pokud chcete opravit všechny problémy s formátováním v souborech s vyrovnáním, postupujte podle těchto kroků:</span><span class="sxs-lookup"><span data-stu-id="5b549-118">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="5b549-119">Otevřete soubor s vyrovnáním (ve .csv) v Microsoft Excelu.</span><span class="sxs-lookup"><span data-stu-id="5b549-119">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="5b549-120">Vyberte první sloupec v souboru.</span><span class="sxs-lookup"><span data-stu-id="5b549-120">Select the first column in the file.</span></span>
3. <span data-ttu-id="5b549-121">Otevřete Průvodce **převodem textu na sloupce.**</span><span class="sxs-lookup"><span data-stu-id="5b549-121">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="5b549-122">Na pásu karet vyberte **Data** a pak **vyberte Text na Sloupce.**</span><span class="sxs-lookup"><span data-stu-id="5b549-122">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="5b549-123">V průvodci vyberte **Typ souboru s oddělovači.**</span><span class="sxs-lookup"><span data-stu-id="5b549-123">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="5b549-124">Pak vyberte **Další.**</span><span class="sxs-lookup"><span data-stu-id="5b549-124">Then, select **Next**.</span></span>
5. <span data-ttu-id="5b549-125">V **poli Oddělovače** vyberte **Čárka**.</span><span class="sxs-lookup"><span data-stu-id="5b549-125">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="5b549-126">(Pokud **je už** vybraná karta Tabulátor, můžete tuto možnost ponechat vybranou.) Pak vyberte **Další.**</span><span class="sxs-lookup"><span data-stu-id="5b549-126">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="5b549-127">V **poli Formát dat sloupce** vyberte **Date:MDY**.</span><span class="sxs-lookup"><span data-stu-id="5b549-127">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="5b549-128">Pak vyberte **Další.**</span><span class="sxs-lookup"><span data-stu-id="5b549-128">Then, select **Next**.</span></span>
7. <span data-ttu-id="5b549-129">V poli **Formát dat sloupce** vyberte Text **pro** všechny sloupce s množstvím dat.</span><span class="sxs-lookup"><span data-stu-id="5b549-129">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="5b549-130">Pak vyberte **Finish** (Dokončit).</span><span class="sxs-lookup"><span data-stu-id="5b549-130">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="5b549-131">Stažení souborů s vyrovnáním prostřednictvím kódu programu</span><span class="sxs-lookup"><span data-stu-id="5b549-131">Download reconciliation files programmatically</span></span>

<span data-ttu-id="5b549-132">Soubory pro sesouhlasení mohou být velmi velké a někdy se obtížně stahují.</span><span class="sxs-lookup"><span data-stu-id="5b549-132">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="5b549-133">Pokud chcete stáhnout soubory s vyrovnáním prostřednictvím kódu programu, podívejte se [na stránku Získání řádových položek faktury.](/partner-center/develop/get-invoiceline-items)</span><span class="sxs-lookup"><span data-stu-id="5b549-133">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a><span data-ttu-id="5b549-134">Pokud váš soubor překročí limit řádku v Excelu</span><span class="sxs-lookup"><span data-stu-id="5b549-134">If your file exceeds the row limit in Excel</span></span>

<span data-ttu-id="5b549-135">Pokud si můžete stáhnout soubor s vyrovnáním, ale v Microsoft Excelu ho neotevřete, pravděpodobně to znamená, že soubor obsahuje více řádků, než Excel povolí.</span><span class="sxs-lookup"><span data-stu-id="5b549-135">If you’re able to download a reconciliation file but not open it in Microsoft Excel, it probably means the file contains more rows than Excel will allow.</span></span> <span data-ttu-id="5b549-136">Pokud k tomu dojde, můžete soubor otevřít pomocí jednoho z následujících postupů.</span><span class="sxs-lookup"><span data-stu-id="5b549-136">If this happens, you can use either of the procedures below to open the file.</span></span>

### <a name="open-a-recon-file-in-power-bi"></a><span data-ttu-id="5b549-137">Otevřete soubor odsoustavy v Power BI</span><span class="sxs-lookup"><span data-stu-id="5b549-137">Open a recon file in Power BI</span></span>

1. <span data-ttu-id="5b549-138">Stáhněte si soubor s vyrovnáním běžným způsobem.</span><span class="sxs-lookup"><span data-stu-id="5b549-138">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="5b549-139">Stáhněte, nainstalujte a otevřete instanci služby Microsoft Power BI.</span><span class="sxs-lookup"><span data-stu-id="5b549-139">Download, install, and open an instance of Microsoft Power BI.</span></span>
3. <span data-ttu-id="5b549-140">Na kartě Power BI **Domů** vyberte **Získat data**.</span><span class="sxs-lookup"><span data-stu-id="5b549-140">On the Power BI **Home** tab, select **Get data**.</span></span>
4. <span data-ttu-id="5b549-141">V seznamu **Běžných zdrojů dat** vyberte **Text/CSV.**</span><span class="sxs-lookup"><span data-stu-id="5b549-141">In the list of **Common data sources**, select **Text/CSV**.</span></span>
5. <span data-ttu-id="5b549-142">Po zobrazení výzvy otevřete soubor odsoustavy.</span><span class="sxs-lookup"><span data-stu-id="5b549-142">When prompted, open your recon file.</span></span>

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a><span data-ttu-id="5b549-143">Otevření souboru s rekonsekcemi v kontingenční tabulce Excelu</span><span class="sxs-lookup"><span data-stu-id="5b549-143">Open a recon file in an Excel pivot table</span></span>

1. <span data-ttu-id="5b549-144">Stáhněte si soubor s vyrovnáním běžným způsobem.</span><span class="sxs-lookup"><span data-stu-id="5b549-144">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="5b549-145">Otevřete nový soubor v Microsoft Excelu.</span><span class="sxs-lookup"><span data-stu-id="5b549-145">Open a new file in Microsoft Excel.</span></span>
3. <span data-ttu-id="5b549-146">Na kartě **Data** vyberte Získat **data,** vyberte **Ze souboru a** pak vyberte **Text/CSV.**</span><span class="sxs-lookup"><span data-stu-id="5b549-146">On the **Data** tab, select **Get data**, select **From file**, and then select **Text/CSV**.</span></span>
4. <span data-ttu-id="5b549-147">Po zobrazení výzvy otevřete soubor odsoustavy.</span><span class="sxs-lookup"><span data-stu-id="5b549-147">When prompted, open your recon file.</span></span> <span data-ttu-id="5b549-148">Zobrazí se vaše data.</span><span class="sxs-lookup"><span data-stu-id="5b549-148">Your data will appear.</span></span>
5. <span data-ttu-id="5b549-149">V rozevírací **nabídce** Načíst vyberte **Načíst do** a pak vyberte **OK.**</span><span class="sxs-lookup"><span data-stu-id="5b549-149">In the **Load** dropdown menu, select **Load to**, and then select **OK**.</span></span>
6. <span data-ttu-id="5b549-150">V dialogovém **okně Importovat data** otevřete soubor **výběrem možnosti Sestava** kontingenční tabulky.</span><span class="sxs-lookup"><span data-stu-id="5b549-150">In the **Import Data** dialog box, select **PivotTable Report** to open your file.</span></span>

## <a name="negative-amount-displayed"></a><span data-ttu-id="5b549-151">Zobrazené záporné množství</span><span class="sxs-lookup"><span data-stu-id="5b549-151">Negative amount displayed</span></span>

<span data-ttu-id="5b549-152">V souboru s vyrovnáním se může zobrazit záporná částka.</span><span class="sxs-lookup"><span data-stu-id="5b549-152">You may see a negative amount in your reconciliation file.</span></span> <span data-ttu-id="5b549-153">Pravděpodobně to má jednu z následujících příčin:</span><span class="sxs-lookup"><span data-stu-id="5b549-153">This is probably caused by one of the following things:</span></span>

- <span data-ttu-id="5b549-154">Nedávno jste zrušili nebo snížili počet licencí</span><span class="sxs-lookup"><span data-stu-id="5b549-154">You recently canceled or reduced your number of licenses</span></span>
- <span data-ttu-id="5b549-155">Obdrželi jste kredit na licenční smlouvu o službě (SLA) nebo na využití Azure.</span><span class="sxs-lookup"><span data-stu-id="5b549-155">You received credit for either a service license agreement (SLA) or for Azure consumption</span></span>

<span data-ttu-id="5b549-156">Pokud chcete o této transakci získat další informace, zkontrolujte v souboru s vyrovnáním příslušný atribut typu poplatku.</span><span class="sxs-lookup"><span data-stu-id="5b549-156">To get more information about this transaction, review its charge type attribute in your reconciliation file.</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="5b549-157">Mapové daně nebo DPH</span><span class="sxs-lookup"><span data-stu-id="5b549-157">Map taxes or VAT</span></span>

<span data-ttu-id="5b549-158">Mapování daní nebo daně z přidané hodnoty (DIČ) na vaši fakturu:</span><span class="sxs-lookup"><span data-stu-id="5b549-158">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="5b549-159">Sečte **sloupec** Daň ze souboru založeného na licencích.</span><span class="sxs-lookup"><span data-stu-id="5b549-159">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="5b549-160">Sečte **sloupec TaxAmount** ze souboru založeného na využití.</span><span class="sxs-lookup"><span data-stu-id="5b549-160">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="5b549-161">Položky souborů s vyrovnáním podle partnera</span><span class="sxs-lookup"><span data-stu-id="5b549-161">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="5b549-162">Partneři v **nepřímém modelu** mohou tato další pole použít v souborech odsouhlasení na základě licencí i na základě využití k položce souborů podle prodejce.</span><span class="sxs-lookup"><span data-stu-id="5b549-162">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="5b549-163">ID MPN</span><span class="sxs-lookup"><span data-stu-id="5b549-163">MPN ID</span></span> | <span data-ttu-id="5b549-164">Description</span><span class="sxs-lookup"><span data-stu-id="5b549-164">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="5b549-165">ID MPN</span><span class="sxs-lookup"><span data-stu-id="5b549-165">MPN ID</span></span> | <span data-ttu-id="5b549-166">Identifikátor Microsoft Partner Network (MPN) partnera Cloud Solution Provider (CSP) (přímý nebo nepřímý).</span><span class="sxs-lookup"><span data-stu-id="5b549-166">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="5b549-167">ID MPN prodejce</span><span class="sxs-lookup"><span data-stu-id="5b549-167">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="5b549-168">Identifikátor [MPN prodejce záznamu pro předplatné](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="5b549-168">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="5b549-169">Toto pole odpovídá ID prodejce uvedenému pro konkrétní předplatné v Partnerské centrum.</span><span class="sxs-lookup"><span data-stu-id="5b549-169">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="5b549-170">Zobrazuje se jenom v souborech s vyrovnáním pro partnery v nepřímém modelu.</span><span class="sxs-lookup"><span data-stu-id="5b549-170">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="5b549-171">ID MPN prodejce</span><span class="sxs-lookup"><span data-stu-id="5b549-171">Reseller MPN ID</span></span>

<span data-ttu-id="5b549-172">Pokud partner CSP prodá předplatné přímo zákazníkovi, jeho **ID MPN** se vyjádřuje dvakrát, jako **ID MPN** i **ID MPN prodejce.**</span><span class="sxs-lookup"><span data-stu-id="5b549-172">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="5b549-173">Pokud má partner CSP prodejce bez **ID MPN,** nastaví se tato hodnota místo toho na **ID MPN** partnera.</span><span class="sxs-lookup"><span data-stu-id="5b549-173">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="5b549-174">Pokud partner CSP odebere **ID MPN** prodejce, tato hodnota se nastaví *na -1.*</span><span class="sxs-lookup"><span data-stu-id="5b549-174">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="5b549-175">Zobrazení nebo aktualizace **ID MPN prodejce:**</span><span class="sxs-lookup"><span data-stu-id="5b549-175">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="5b549-176">Přihlaste se do Partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="5b549-176">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="5b549-177">V nabídce Partnerské centrum vyberte **Zákazníci.**</span><span class="sxs-lookup"><span data-stu-id="5b549-177">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="5b549-178">V seznamu vyberte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="5b549-178">Choose the customer from the list.</span></span>
4. <span data-ttu-id="5b549-179">V nabídce zákazníka vyberte **Předplatná.**</span><span class="sxs-lookup"><span data-stu-id="5b549-179">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="5b549-180">V seznamu vyberte předplatné.</span><span class="sxs-lookup"><span data-stu-id="5b549-180">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="5b549-181">Výběrem **možnosti** Aktualizovat **změňte reseller (MPN ID).**</span><span class="sxs-lookup"><span data-stu-id="5b549-181">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="5b549-182">Další kroky</span><span class="sxs-lookup"><span data-stu-id="5b549-182">Next steps</span></span>

- [<span data-ttu-id="5b549-183">Čtení souboru s vyúčtováním & odsoustavy</span><span class="sxs-lookup"><span data-stu-id="5b549-183">How to read your bill & recon file</span></span>](read-your-bill.md) 