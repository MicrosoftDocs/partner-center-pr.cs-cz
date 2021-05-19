---
title: Sloučení partnerského účtu s jiným partnerským účtem
description: Zjistěte, jak sloučit partnerský účet s jiným partnerským účtem v Partnerské centrum – pro společnosti, které jsou aktivními partnery Microsoftu v Partnerské centrum.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: parthpandyaMSFT
ms.author: parthp
ms.custom: seodec18
ms.date: 06/12/2020
ms.openlocfilehash: 8c47204d54cf05113eae73cede4afedf106ac121
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146506"
---
# <a name="merge-your-partner-account-with-another-partner-account"></a><span data-ttu-id="3339a-103">Sloučení partnerského účtu s jiným partnerským účtem</span><span class="sxs-lookup"><span data-stu-id="3339a-103">Merge your partner account with another partner account</span></span>

<span data-ttu-id="3339a-104">**Odpovídající role:** Správce účtu</span><span class="sxs-lookup"><span data-stu-id="3339a-104">**Appropriate roles**: Account admin</span></span>

<span data-ttu-id="3339a-105">Dvě nebo více společností, které jsou aktivními partnery Microsoftu a mají účty v Partnerské centrum si mohou zvolit sloučení svých účtů.</span><span class="sxs-lookup"><span data-stu-id="3339a-105">Two or more companies who are active Microsoft partners and have accounts in Partner Center can choose to merge their accounts.</span></span>

## <a name="what-happens-when-two-partners-elect-to-merge-their-partner-center-accounts"></a><span data-ttu-id="3339a-106">Co se stane, když se dva partneři rozhodne sloučit své Partnerské centrum účty</span><span class="sxs-lookup"><span data-stu-id="3339a-106">What happens when two partners elect to merge their Partner Center accounts</span></span>

- <span data-ttu-id="3339a-107">Partnerská organizace, která zahájí sloučení, bude globální účet partnera (PGA).</span><span class="sxs-lookup"><span data-stu-id="3339a-107">The partner organization who initiates the merge will be the Partner global account (PGA).</span></span>

- <span data-ttu-id="3339a-108">Zzvaný PGA organizace se stane umístěním iniciující společnosti.</span><span class="sxs-lookup"><span data-stu-id="3339a-108">The invited organization’s PGA becomes a location of the initiating company.</span></span>

- <span data-ttu-id="3339a-109">Všechna umístění slučování účtu se stanou umístěními v rámci PGA.</span><span class="sxs-lookup"><span data-stu-id="3339a-109">All the locations of the merging account become locations under the PGA.</span></span>

- <span data-ttu-id="3339a-110">Po sloučení účtu se zobrazí podrobnosti o účtu, jako jsou umístění i uživatelé v rámci profilu PGA.</span><span class="sxs-lookup"><span data-stu-id="3339a-110">Once the account merger is complete, you will see both account’s details such as locations and users within the PGA profile.</span></span> <span data-ttu-id="3339a-111">Tento proces nelze vrátit zpět.</span><span class="sxs-lookup"><span data-stu-id="3339a-111">You can't reverse this process.</span></span>

- <span data-ttu-id="3339a-112">Během této konsolidace se zachovají všechna ID MPN pro umístění.</span><span class="sxs-lookup"><span data-stu-id="3339a-112">All MPN IDs for locations are preserved during this consolidation.</span></span>

- <span data-ttu-id="3339a-113">Role uživatelů se přenesly.</span><span class="sxs-lookup"><span data-stu-id="3339a-113">User's roles are brought over.</span></span> <span data-ttu-id="3339a-114">Pokud by například uživatel byl správcem pobídek pro konkrétní lokalitu, měl by i po fúzi roli a mohl by vidět pobídky, které viděl před fúzí.</span><span class="sxs-lookup"><span data-stu-id="3339a-114">For example, if a user had been the incentives admin for a specific location, they would still have that role after the merger and be able to see the incentives they saw prior to the merger.</span></span>

- <span data-ttu-id="3339a-115">Tenanti Azure AD a účty CSP se nesloučí a nemají žádný vliv.</span><span class="sxs-lookup"><span data-stu-id="3339a-115">Azure AD tenants and CSP accounts are not merged and have no effect.</span></span>

- <span data-ttu-id="3339a-116">Publikované nabídky a data kanálu spoluproduování přidružená k oběma společnostem se zachovají.</span><span class="sxs-lookup"><span data-stu-id="3339a-116">Published offers and Co-sell pipeline data associated to both companies are preserved</span></span>

### <a name="view-of-merged-accounts"></a><span data-ttu-id="3339a-117">Zobrazení sloučených účtů</span><span class="sxs-lookup"><span data-stu-id="3339a-117">View of merged accounts</span></span>

:::image type="content" source="images/merge-accounts/account-merge.png" alt-text="Fúze účtů":::

## <a name="what-to-expect-if-you-have-been-invited-to-merge-your-partner-center-account-with-another-partner-center-account"></a><span data-ttu-id="3339a-119">Co očekávat, pokud jste byli pozváni ke sloučení účtu Partnerské centrum s jiným Partnerské centrum účtem</span><span class="sxs-lookup"><span data-stu-id="3339a-119">What to expect if you have been invited to merge your Partner Center account with another Partner Center account</span></span>

<span data-ttu-id="3339a-120">Pokud se rozhodnete přijmout pozvánku ke sloučení účtů: · Vaše ID MPN a umístění se sloučí s PGA partnerského účtu, který vás pozval.</span><span class="sxs-lookup"><span data-stu-id="3339a-120">If you decide to accept the invitation to merge accounts: · Your MPN ID(s) and locations will be merged into the PGA of the partner account that invited you.</span></span>

- <span data-ttu-id="3339a-121">Vaši uživatelé se převedou do sloučeného účtu s jejich rolemi beze změny.</span><span class="sxs-lookup"><span data-stu-id="3339a-121">Your users will be brought into the merged account with their roles intact.</span></span>

- <span data-ttu-id="3339a-122">Stávající výhody a kompetence budou pro obě společnosti zachovány po fúzi až do prodloužení.</span><span class="sxs-lookup"><span data-stu-id="3339a-122">Existing benefits and competencies will be preserved for both companies after the merger until renewal.</span></span> <span data-ttu-id="3339a-123">Při obnovení se budou účty považovat za jednu společnost a standardní pravidla obnovy.</span><span class="sxs-lookup"><span data-stu-id="3339a-123">At renewal, the accounts will be treated as one company and standard renewal rules will apply.</span></span>

## <a name="understand-the-impacts-to-programs-and-benefits-when-partners-elect-to-merge-accounts"></a><span data-ttu-id="3339a-124">Pochopení dopadů na programy a výhody, když se partneři rozhodnou sloučit účty</span><span class="sxs-lookup"><span data-stu-id="3339a-124">Understand the impacts to programs and benefits when partners elect to merge accounts</span></span>

- <span data-ttu-id="3339a-125">Všechny stávající kompetence (Gold/stříbrné), nákupy (například Microsoft Action Pack) a související výhody se během konsolidace uchovávají.</span><span class="sxs-lookup"><span data-stu-id="3339a-125">All existing competencies (Gold/Silver), purchases (such as Microsoft Action Pack), and associated benefits are preserved during consolidation.</span></span> <span data-ttu-id="3339a-126">Pokud mají obě společnosti stejnou kompetenci, ale jedna je zlatá a druhá stříbrná, bude udělována kompetence s nejvyšší úrovní znalostí a partneři budou mít pro tuto kompetenci jednu sadu výhod stříbra a jednu sadu zlatých výhod, dokud jejich další obnovení neproběhne.</span><span class="sxs-lookup"><span data-stu-id="3339a-126">If both companies have the same competency but one's is gold and the other silver, the competency with highest proficiency level will be awarded, and partners will have one set of silver benefits and one set of gold benefits for that competency until their next renewal.</span></span> 

- <span data-ttu-id="3339a-127">Po spojení bude zachováno nejvyšší datum výročí pro sadu Microsoft Action Pack.</span><span class="sxs-lookup"><span data-stu-id="3339a-127">Highest anniversary date for Microsoft Action Pack will be retained after the merger.</span></span> <span data-ttu-id="3339a-128">Například pokud datum výročí pro společnost 1 je června 2020 pro obnovení sady Action Pack a datum výročí pro obnovení sady Action Pack pro společnost 2 je v 2020, bude společnost Microsoft 2020 používat datum. října, jako nové datum výročí pro sloučenou společnost.</span><span class="sxs-lookup"><span data-stu-id="3339a-128">For example, if the anniversary date for company 1 is June 2020 for Action Pack renewal and the anniversary date for Action Pack renewal for company 2 is October 2020, Microsoft will use the October 2020 date as the new anniversary date for the merged company.</span></span>

- <span data-ttu-id="3339a-129">Během slučování účtů a až do dalšího obnovení se u každého účtu zachová jejich Akční balíček a výhody kompetence.</span><span class="sxs-lookup"><span data-stu-id="3339a-129">During the account merger and until your next renewal, each account will retain their Action Pack and/or competency benefits.</span></span> <span data-ttu-id="3339a-130">Při obnovení se použijí standardní pravidla pro obnovení sady Action Pack a kompetence.</span><span class="sxs-lookup"><span data-stu-id="3339a-130">At renewal, standard Action Pack and competency renewal rules apply.</span></span>

- <span data-ttu-id="3339a-131">Po obnovení jsou pro globální účet partnera partnerské společnosti implementovány výhody, které jsou součástí dosahování kompetence a sady Action Pack:</span><span class="sxs-lookup"><span data-stu-id="3339a-131">Upon renewal, benefits that are included with competency attainment and Action Pack are implemented for the partner company’s partner global account:</span></span>

  - <span data-ttu-id="3339a-132">Microsoft Action Pack: Partnerská společnost bude moct zakoupit jeden globální účet pro každý partner.</span><span class="sxs-lookup"><span data-stu-id="3339a-132">Microsoft Action Pack: The partner company will be able to purchase one Action Pack per partner global account.</span></span>

  - <span data-ttu-id="3339a-133">Kompetence: Partnerská společnost dostane jeden balíček základních výhod, které jsou přidružené k jejich nejvyššímu dosahu, a výhody pro konkrétní kompetenci, na které má partner nárok na globální účet partnera.</span><span class="sxs-lookup"><span data-stu-id="3339a-133">Competency: The partner company will receive one package of core benefits, associated to their highest attainment, plus competency-specific benefits the partner is eligible for per partner global account.</span></span>

- <span data-ttu-id="3339a-134">Na všechny výhody se vztahují [Průvodce využitím Microsoft Partner Network výhody](https://aka.ms/partner-benefits-use-guide).</span><span class="sxs-lookup"><span data-stu-id="3339a-134">All benefits are subject to the [Microsoft Partner Network benefits usage guide](https://aka.ms/partner-benefits-use-guide).</span></span> <span data-ttu-id="3339a-135">Příklad: aktivovaný token O365 E3 je funkční po dobu 12 měsíců od aktivace.</span><span class="sxs-lookup"><span data-stu-id="3339a-135">For example: an activated O365 E3 token is functional for 12 months after activation.</span></span> <span data-ttu-id="3339a-136">Po aktivaci tokenu pro licence na tenanta se tyto licence nemusí přesunout do jiného tenanta.</span><span class="sxs-lookup"><span data-stu-id="3339a-136">Once a token has been activated for licenses on a tenant, those licenses may not be moved to another tenant.</span></span>

- <span data-ttu-id="3339a-137">Asociace ID MCP pro obě společnosti budou zachovaná a přidružená k PGA MPN ID.</span><span class="sxs-lookup"><span data-stu-id="3339a-137">The MCP ID associations for both companies will be retained and associated with the PGA MPN ID.</span></span>

- <span data-ttu-id="3339a-138">Možnosti uvedení na trh a technické výhody se nabízejí jako zvýhodnění Core.</span><span class="sxs-lookup"><span data-stu-id="3339a-138">Go-to-market and technical benefits are offered as competency core benefit.</span></span> <span data-ttu-id="3339a-139">Po sloučení se doporučuje zkontrolovat bankovní a daňové údaje, aby se zajistila přesnost.</span><span class="sxs-lookup"><span data-stu-id="3339a-139">Post-merge, it’s recommended that you check your bank and tax information to ensure accuracy.</span></span>

- <span data-ttu-id="3339a-140">Pokud je vaše společnost v programu pro odborníky na Azure, zachová se do obnovení výhody.</span><span class="sxs-lookup"><span data-stu-id="3339a-140">If your company is in the Azure Expert MSP program, benefits are retained until renewal.</span></span>

- <span data-ttu-id="3339a-141">Pokud vaše společnost získala pokročilé specializace, uchovávají se v obou účtech.</span><span class="sxs-lookup"><span data-stu-id="3339a-141">If your company has earned advanced specializations, they are retained across both accounts are retained.</span></span>

- <span data-ttu-id="3339a-142">Všechny doklady Software Assurance se uchovávají v obou účtech.</span><span class="sxs-lookup"><span data-stu-id="3339a-142">Any software assurance vouchers are retained across both accounts.</span></span> 

- <span data-ttu-id="3339a-143">Neexistuje žádný vliv na přidružení partnera DPOR nebo PAL.</span><span class="sxs-lookup"><span data-stu-id="3339a-143">There is no effect to DPOR or PAL association.</span></span> <span data-ttu-id="3339a-144">Všechny přidružené příjmové příspěvky začnou přesměrovat do nového globálního účtu partnera.</span><span class="sxs-lookup"><span data-stu-id="3339a-144">Any associated revenue contributions will begin to flow into the new Partner Global Account</span></span>

## <a name="invite-a-company-to-merge-their-partner-center-account-with-your-partner-center-account"></a><span data-ttu-id="3339a-145">Pozvání společnosti pro sloučení účtu partnerského centra s účtem partnerského centra</span><span class="sxs-lookup"><span data-stu-id="3339a-145">Invite a company to merge their Partner Center account with your Partner Center account</span></span>

>[!Note]
><span data-ttu-id="3339a-146">K provedení fúze účtu musíte být **správcem účtu** vaší společnosti.</span><span class="sxs-lookup"><span data-stu-id="3339a-146">To perform the account merger, you must be the **Account admin** for your company.</span></span>

1. <span data-ttu-id="3339a-147">Na řídicím panelu partnerského centra vyberte **Nastavení** .</span><span class="sxs-lookup"><span data-stu-id="3339a-147">Select **Settings** from your Partner Center dashboard.</span></span> 

2. <span data-ttu-id="3339a-148">Vyberte **Sloučení účtů**.</span><span class="sxs-lookup"><span data-stu-id="3339a-148">Select **Account merge**.</span></span>

3. <span data-ttu-id="3339a-149">Přidejte ID MPN nacházející se v **partnerském profilu** účtu, který chcete s vámi vyzvat ke sloučení.</span><span class="sxs-lookup"><span data-stu-id="3339a-149">Add the MPN ID located in the **Partner profile** of the account that you want to invite to merge with you.</span></span> <span data-ttu-id="3339a-150">Musíte použít jeho globální ID MPN partnera.</span><span class="sxs-lookup"><span data-stu-id="3339a-150">You must use their Partner global MPN ID.</span></span> <span data-ttu-id="3339a-151">Nemůžete použít umístění MPN ID.</span><span class="sxs-lookup"><span data-stu-id="3339a-151">You can't use a location MPN ID.</span></span>

4. <span data-ttu-id="3339a-152">Když vyberete **Sloučit**, pošle se Partnerská společnost Pozvánka.</span><span class="sxs-lookup"><span data-stu-id="3339a-152">When you select **Merge**, an invitation is sent to the partner company.</span></span> <span data-ttu-id="3339a-153">Po přijetí žádosti můžete sloučení účtů zahájit v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="3339a-153">When they accept your request, you can initiate the account merge within Partner Center.</span></span> <span data-ttu-id="3339a-154">Pokud společnost vaši žádost o sloučení účtů odmítne, může vysvětlit, proč žádost zamítla.</span><span class="sxs-lookup"><span data-stu-id="3339a-154">If the company rejects your request to merge accounts, they can explain why they rejected the request.</span></span> <span data-ttu-id="3339a-155">Seznam všech sloučení vašich účtů najdete v části **Historie sloučení**.</span><span class="sxs-lookup"><span data-stu-id="3339a-155">A list of all your account merges is available to you under **Merge history**.</span></span>
 
### <a name="example-of-two-companies-merging-accounts"></a><span data-ttu-id="3339a-156">Příklad dvou společností, které slučují účty</span><span class="sxs-lookup"><span data-stu-id="3339a-156">Example of two companies merging accounts</span></span>

1. <span data-ttu-id="3339a-157">Contoso, Ltd. má</span><span class="sxs-lookup"><span data-stu-id="3339a-157">Contoso, Ltd. has</span></span> 

    <span data-ttu-id="3339a-158">a.</span><span class="sxs-lookup"><span data-stu-id="3339a-158">a.</span></span> <span data-ttu-id="3339a-159">globální [ID MPN 1111111](https://partner.microsoft.com/pcv/accountsettings/connectedpartnerprofile) a JEDNO ID MPN podřízeného [umístění 2222222.](https://partner.microsoft.com/pcv/accountsettings/locationsprofile)</span><span class="sxs-lookup"><span data-stu-id="3339a-159">a [global MPN ID of 1111111](https://partner.microsoft.com/pcv/accountsettings/connectedpartnerprofile) and one subordinate [location MPN IDs of 2222222](https://partner.microsoft.com/pcv/accountsettings/locationsprofile).</span></span>
  
    <span data-ttu-id="3339a-160">b.</span><span class="sxs-lookup"><span data-stu-id="3339a-160">b.</span></span> <span data-ttu-id="3339a-161">tenant Azure AD = @contoso.com</span><span class="sxs-lookup"><span data-stu-id="3339a-161">an Azure AD tenant = @contoso.com</span></span>
 
    <span data-ttu-id="3339a-162">c.</span><span class="sxs-lookup"><span data-stu-id="3339a-162">c.</span></span> <span data-ttu-id="3339a-163">gold competency that expires October 1, 2020</span><span class="sxs-lookup"><span data-stu-id="3339a-163">a gold competency that expires October 1, 2020</span></span>
2. <span data-ttu-id="3339a-164">Společnost Fabrikam, Inc. má</span><span class="sxs-lookup"><span data-stu-id="3339a-164">Fabrikam, Inc. has</span></span>
 
    <span data-ttu-id="3339a-165">a.</span><span class="sxs-lookup"><span data-stu-id="3339a-165">a.</span></span>  <span data-ttu-id="3339a-166">globální ID MPN 333333 a ID MPN dvou podřízených umístění 4444444 a 5555555</span><span class="sxs-lookup"><span data-stu-id="3339a-166">a global MPN ID of 3333333 and two subordinate location MPN IDs of 4444444 and 5555555</span></span>

    <span data-ttu-id="3339a-167">b.</span><span class="sxs-lookup"><span data-stu-id="3339a-167">b.</span></span>  <span data-ttu-id="3339a-168">tenant Azure AD = @fabrikam.com</span><span class="sxs-lookup"><span data-stu-id="3339a-168">an Azure AD tenant = @fabrikam.com</span></span>

    <span data-ttu-id="3339a-169">c.</span><span class="sxs-lookup"><span data-stu-id="3339a-169">c.</span></span>  <span data-ttu-id="3339a-170">dvě zlaté kompetence, které vyprší 1. prosince 2020</span><span class="sxs-lookup"><span data-stu-id="3339a-170">two gold competencies that expire December 1, 2020</span></span>
3.  <span data-ttu-id="3339a-171">Společnost Contoso koupí společnost Fabrikam a přejde [sem,](https://partner.microsoft.com/dashboard/account/merger) aby zahájila žádost o sloučení.</span><span class="sxs-lookup"><span data-stu-id="3339a-171">Contoso buys Fabrikam and goes [here](https://partner.microsoft.com/dashboard/account/merger) to initiate a merge request.</span></span>
4.  <span data-ttu-id="3339a-172">Společnost Fabrikam se Partnerské centrum přihlásí a přejde na stejnou stránku, na které se #3 contoso, aby schválila žádost společnosti Contoso.</span><span class="sxs-lookup"><span data-stu-id="3339a-172">Fabrikam signs into Partner Center and goes to the same page as Contoso did in step #3, to approve Contoso’s request.</span></span>
5.  <span data-ttu-id="3339a-173">Společnost Contoso na stejné stránce proše informace o sloučení a poskytne potvrzení, že může pokračovat v fúzi účtů.</span><span class="sxs-lookup"><span data-stu-id="3339a-173">Contoso reviews the details of the merge on that same page and provides confirmation to proceed with the account merger.</span></span>
6.  <span data-ttu-id="3339a-174">Po fúzi se firemní účet zobrazí takto:</span><span class="sxs-lookup"><span data-stu-id="3339a-174">After the merger, the company account will display as:</span></span>

    <span data-ttu-id="3339a-175">a.</span><span class="sxs-lookup"><span data-stu-id="3339a-175">a.</span></span>  <span data-ttu-id="3339a-176">Společnost Contoso s globálním ID MPN 1111111 a 4 ID MPN podřízeného umístění 2222222, 3333333, 4444444 a 5555555</span><span class="sxs-lookup"><span data-stu-id="3339a-176">A company named Contoso with a global MPN ID of 1111111 and 4 subordinate location MPN IDs of 2222222, 3333333, 4444444, and 5555555</span></span>
    
    <span data-ttu-id="3339a-177">b.</span><span class="sxs-lookup"><span data-stu-id="3339a-177">b.</span></span>  <span data-ttu-id="3339a-178">Bude mít dva tenanty Azure AD ( + ), kteří mají přístup ke @contoso.com @fabrikam.com stejnému Partnerské centrum účtu.</span><span class="sxs-lookup"><span data-stu-id="3339a-178">It will have two Azure AD tenants (@contoso.com + @fabrikam.com) that have access to the same Partner Center account</span></span>
    
    <span data-ttu-id="3339a-179">c.</span><span class="sxs-lookup"><span data-stu-id="3339a-179">c.</span></span>  <span data-ttu-id="3339a-180">Bude mít balíčky se dvěma výhodami kompetencí– jednu, která vyprší 1. října 2020 a druhá vyprší 1. prosince 2020.</span><span class="sxs-lookup"><span data-stu-id="3339a-180">It will have two competency benefits packages, one that expires October 1, 2020 and another that expires December 1, 2020.</span></span> <span data-ttu-id="3339a-181">1. prosince 2020 budou moct prodloužit platnost jako balíček výhod s jednou kompetencí.</span><span class="sxs-lookup"><span data-stu-id="3339a-181">They'll be able to renew as a single competency benefits package on December 1, 2020.</span></span> <span data-ttu-id="3339a-182">Po prodloužení si společnost Contoso zachová všechny tři kompetence, i když si může zachovat pouze jeden balíček výhod.</span><span class="sxs-lookup"><span data-stu-id="3339a-182">When they renew, Contoso will retain all three competencies even though they can only maintain a single benefits package.</span></span>
    
7.  <span data-ttu-id="3339a-183">Správci společnosti Contoso budou nadále spravovat Partnerské centrum role @contoso.com uživatelů společnosti Contoso.</span><span class="sxs-lookup"><span data-stu-id="3339a-183">Contoso’s admins will continue to manage Partner Center roles for @contoso.com’s users.</span></span> <span data-ttu-id="3339a-184">Správci společnosti Fabrikam budou nadále spravovat Partnerské centrum role @fabrikam.com uživatelů společnosti Fabrikam.</span><span class="sxs-lookup"><span data-stu-id="3339a-184">Fabrikam’s admins will continue to manage Partner Center roles for @fabrikam.com’s users.</span></span> <span data-ttu-id="3339a-185">Správci společnosti Contoso mohou spravovat uživatele společnosti Fabrikam pouze v případě, že jsou pozvaní jako host do tenanta společnosti Fabrikam.</span><span class="sxs-lookup"><span data-stu-id="3339a-185">Contoso’s admins can only administer Fabrikam’s users if they are invited as a guest into Fabrikam’s tenant.</span></span>
8.  <span data-ttu-id="3339a-186">Společnost Contoso se může rozhodnout tenanta ignorovat a znovu pro zaměstnance Fabrikam zadat nové přihlašovací údaje s novými rolemi a @fabrikam.com @contoso.com oprávněními.</span><span class="sxs-lookup"><span data-stu-id="3339a-186">Contoso could decide to ignore the @fabrikam.com tenant, and reissue the Fabrikam employees new @contoso.com credentials with new roles and permissions.</span></span>

## <a name="next-steps"></a><span data-ttu-id="3339a-187">Další kroky</span><span class="sxs-lookup"><span data-stu-id="3339a-187">Next steps</span></span>

- [<span data-ttu-id="3339a-188">Přiřazování uživatelských rolí a oprávnění</span><span class="sxs-lookup"><span data-stu-id="3339a-188">Assign users roles and permissions</span></span>](permissions-overview.md)

- [<span data-ttu-id="3339a-189">Ověření informací o profilu partnera</span><span class="sxs-lookup"><span data-stu-id="3339a-189">Verify your partner profile information</span></span>](update-your-partner-profile.md)

- [<span data-ttu-id="3339a-190">Přidání Azure Partner Shared Services, aby si partneři mohli koupit předplatná Azure pro vlastní použití</span><span class="sxs-lookup"><span data-stu-id="3339a-190">Add Azure Partner Shared Services so partners can buy Azure subscriptions for their own use</span></span>](shared-services.md)
