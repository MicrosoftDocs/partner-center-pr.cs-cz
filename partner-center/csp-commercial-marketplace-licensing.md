---
title: Správa licencování v nabídek marketplace
ms.topic: how-to
ms.date: 04/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zjistěte, jak nastavit a spravovat licencování nabídek komerčního marketplace isv.
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c128b99b034564bcaa100ca975253f8b1bad7a42
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147951"
---
# <a name="manage-licensing-in-marketplace-offers"></a><span data-ttu-id="dc77d-103">Správa licencování v nabídek marketplace</span><span class="sxs-lookup"><span data-stu-id="dc77d-103">Manage licensing in marketplace offers</span></span>

<span data-ttu-id="dc77d-104">**Odpovídající role:** Globální správce | Správce účtu</span><span class="sxs-lookup"><span data-stu-id="dc77d-104">**Appropriate roles**: Global admin | Account admin</span></span>

<span data-ttu-id="dc77d-105">Tento článek vás provede procesem nastavení nabídky v Partnerské centrum, zpřístupnění v Microsoft AppSource a následně správy licencí pro tuto nabídku.</span><span class="sxs-lookup"><span data-stu-id="dc77d-105">This article walks you through the process of setting up an offer in Partner Center, making it available in Microsoft AppSource, and then managing licenses for that offer.</span></span>  

>[!IMPORTANT]
><span data-ttu-id="dc77d-106">Možnosti v tomto článku jsou aktuálně v Public Preview.</span><span class="sxs-lookup"><span data-stu-id="dc77d-106">The capabilities in this article are currently in Public Preview.</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="dc77d-107">Než začnete</span><span class="sxs-lookup"><span data-stu-id="dc77d-107">Before you begin</span></span>

### <a name="commercial-marketplace-basics"></a><span data-ttu-id="dc77d-108">Základy komerčního marketplace</span><span class="sxs-lookup"><span data-stu-id="dc77d-108">Commercial marketplace basics</span></span>

<span data-ttu-id="dc77d-109">Než s tímto procesem začnete, měli byste se seznámit se základy komerčního marketplace.</span><span class="sxs-lookup"><span data-stu-id="dc77d-109">Before you begin this process, you should familiarize yourself with the basics of the commercial marketplace.</span></span> <span data-ttu-id="dc77d-110">Články v následující tabulce vám pomůžou začít.</span><span class="sxs-lookup"><span data-stu-id="dc77d-110">The articles in the table below will help get you started.</span></span> 

| <span data-ttu-id="dc77d-111">Téma</span><span class="sxs-lookup"><span data-stu-id="dc77d-111">Topic</span></span>  | <span data-ttu-id="dc77d-112">Článek</span><span class="sxs-lookup"><span data-stu-id="dc77d-112">Article</span></span>  |
|-------|--------|
|<span data-ttu-id="dc77d-113">Plány komerčního marketplace</span><span class="sxs-lookup"><span data-stu-id="dc77d-113">Commercial marketplace plans</span></span> | [<span data-ttu-id="dc77d-114">Plány a ceny nabídek komerčního marketplace</span><span class="sxs-lookup"><span data-stu-id="dc77d-114">Plans and pricing for commercial marketplace offers</span></span>](/azure/marketplace/plans-pricing)    |
|<span data-ttu-id="dc77d-115">Nabídky komerčního marketplace</span><span class="sxs-lookup"><span data-stu-id="dc77d-115">Commercial marketplace offers</span></span>  | [<span data-ttu-id="dc77d-116">Výpis typů</span><span class="sxs-lookup"><span data-stu-id="dc77d-116">Listing types</span></span>](/azure/marketplace/determine-your-listing-type)    |
|<span data-ttu-id="dc77d-117">Účty komerčního marketplace</span><span class="sxs-lookup"><span data-stu-id="dc77d-117">Commercial marketplace accounts</span></span> |  [<span data-ttu-id="dc77d-118">Vytvoření účtu komerčního marketplace v Partnerské centrum</span><span class="sxs-lookup"><span data-stu-id="dc77d-118">Create a commercial marketplace account in Partner Center</span></span>](/azure/marketplace/create-account) |

### <a name="determine-your-offer-id"></a><span data-ttu-id="dc77d-119">Určení ID vaší nabídky</span><span class="sxs-lookup"><span data-stu-id="dc77d-119">Determine your Offer ID</span></span>

<span data-ttu-id="dc77d-120">V následujících postupech budete vyzváni k zadání ID nabídky.</span><span class="sxs-lookup"><span data-stu-id="dc77d-120">In the procedures below, you’ll be prompted to enter an Offer ID.</span></span> <span data-ttu-id="dc77d-121">Chvíli si vymyslete vhodné ID nabídky s vezměte v paměti následující body:</span><span class="sxs-lookup"><span data-stu-id="dc77d-121">Take some time now to come up with a suitable Offer ID, keeping in mind the following points:</span></span>

- <span data-ttu-id="dc77d-122">Toto ID se zákazníkům zobrazí na webové adrese nabídky marketplace a v Azure Resource Manager šablony, pokud jsou k dispozici.</span><span class="sxs-lookup"><span data-stu-id="dc77d-122">This ID is visible to customers in the web address for the marketplace offer and Azure Resource Manager templates, if applicable.</span></span>
- <span data-ttu-id="dc77d-123">ID nabídky v kombinaci s ID vydavatele musí být dlouhé pod 40 znaky.</span><span class="sxs-lookup"><span data-stu-id="dc77d-123">The Offer ID combined with the Publisher ID must be under 40 characters in length.</span></span>
- <span data-ttu-id="dc77d-124">Použijte při tom jenom malá písmena a číslice.</span><span class="sxs-lookup"><span data-stu-id="dc77d-124">Use only lowercase letters and numbers.</span></span> <span data-ttu-id="dc77d-125">ID nabídky může zahrnovat pomlčky a podtržítka, ale ne mezery.</span><span class="sxs-lookup"><span data-stu-id="dc77d-125">The Offer ID can include hyphens and underscores, but no spaces.</span></span> <span data-ttu-id="dc77d-126">Pokud je například vaším vydavatelem ID `testpublisherid` a zadáte `test-offer-1` , bude webová adresa nabídky `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1` .</span><span class="sxs-lookup"><span data-stu-id="dc77d-126">For example, if your Publisher ID is `testpublisherid` and you enter `test-offer-1`, the offer web address will be `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1`.</span></span>
- <span data-ttu-id="dc77d-127">Toto ID se po výběru **vytvořit** nedá změnit.</span><span class="sxs-lookup"><span data-stu-id="dc77d-127">This ID can't be changed after you select **Create**.</span></span>

### <a name="determine-your-offer-alias"></a><span data-ttu-id="dc77d-128">Určení aliasu nabídky</span><span class="sxs-lookup"><span data-stu-id="dc77d-128">Determine your Offer alias</span></span>

<span data-ttu-id="dc77d-129">Alias nabídky je název, který se používá pro nabídku v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="dc77d-129">The Offer alias is the name used for the offer in Partner Center.</span></span> <span data-ttu-id="dc77d-130">Budete také potřebovat příslušný alias nabídky, který bude postupovat podle níže uvedených pokynů:</span><span class="sxs-lookup"><span data-stu-id="dc77d-130">You’ll also need an appropriate Offer alias that follows the guidelines below:</span></span>

- <span data-ttu-id="dc77d-131">Tento název se na webu Marketplace nepoužívá a liší se od názvu nabídky a dalších hodnot, které se zákazníkům zobrazují.</span><span class="sxs-lookup"><span data-stu-id="dc77d-131">This name isn't used in the marketplace and is different from the offer name and other values shown to customers.</span></span>
- <span data-ttu-id="dc77d-132">Po výběru vytvořit se tento název nedá změnit.</span><span class="sxs-lookup"><span data-stu-id="dc77d-132">This name can't be changed after you select Create.</span></span>

## <a name="create-your-offer"></a><span data-ttu-id="dc77d-133">Vytvoření nabídky</span><span class="sxs-lookup"><span data-stu-id="dc77d-133">Create your offer</span></span>

<span data-ttu-id="dc77d-134">Prvním krokem v licenčním procesu je vytvoření komerční nabídky na webu Marketplace.</span><span class="sxs-lookup"><span data-stu-id="dc77d-134">The first step in the licensing process is to create your commercial marketplace offer.</span></span> 

1. <span data-ttu-id="dc77d-135">Přihlaste se k [řídicímu panelu pro Partnerské centrum](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="dc77d-135">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="dc77d-136">V levé navigační nabídce vyberte **komerční Marketplace/přehled**.</span><span class="sxs-lookup"><span data-stu-id="dc77d-136">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="dc77d-137">V horní části stránky přehled vyberte možnost **Nová nabídka** a potom vyberte **Dynamics 365 pro customer Engagement & PowerApps**.</span><span class="sxs-lookup"><span data-stu-id="dc77d-137">At the top of the Overview page, select **New offer**, and then select **Dynamics 365 for Customer Engagement & PowerApps**.</span></span>
4. <span data-ttu-id="dc77d-138">Zadejte **ID nabídky** a **alias nabídky** , který jste vytvořili dříve.</span><span class="sxs-lookup"><span data-stu-id="dc77d-138">Enter the **Offer ID** and **Offer alias** you created earlier.</span></span>
5. <span data-ttu-id="dc77d-139">Vyberte **vytvořit** pro vygenerování nabídky a pokračování.</span><span class="sxs-lookup"><span data-stu-id="dc77d-139">Select **Create** to generate the offer and continue.</span></span>
6. <span data-ttu-id="dc77d-140">Vyberte možnosti licencování.</span><span class="sxs-lookup"><span data-stu-id="dc77d-140">Choose your licensing options.</span></span>

    - <span data-ttu-id="dc77d-141">Pokud chcete pro vaši nabídku povolit správu licencí, vyberte **Povolit správu licencí aplikací prostřednictvím Microsoftu**.</span><span class="sxs-lookup"><span data-stu-id="dc77d-141">To enable license management for your offer, select **Enable app license management through Microsoft**.</span></span> <span data-ttu-id="dc77d-142">Jedná se o jednorázové nastavení a po publikování vaší nabídky ho nemůžete změnit.</span><span class="sxs-lookup"><span data-stu-id="dc77d-142">This is a one-time setting, and you can’t change it once your offer is published.</span></span>

    - <span data-ttu-id="dc77d-143">Zákazníkům taky můžete povolit, aby se základní funkce vaší aplikace spouštěli bez licence, a po zakoupení licence mohli používat prémiové funkce.</span><span class="sxs-lookup"><span data-stu-id="dc77d-143">You can also enable customers to run your app’s base functionality without a license, and run premium features once they’ve purchased a license.</span></span> <span data-ttu-id="dc77d-144">Pokud to chcete provést, vyberte možnost **Povolit zákazníkům instalaci aplikace i v případě, že licence nejsou přiřazeny**.</span><span class="sxs-lookup"><span data-stu-id="dc77d-144">To do this, select **Allow customers to install my app even if licenses are not assigned**.</span></span>

    - <span data-ttu-id="dc77d-145">Pokud nechcete, aby vaše nabídka měla povolenou správu licencí, vyberte **získat hned (zdarma)**, **bezplatnou zkušební verzi** nebo **kontaktujte mě**.</span><span class="sxs-lookup"><span data-stu-id="dc77d-145">If you don’t want your offer to have license management enabled, select **Get it now (Free)**, **Free trial**, or **Contact me**.</span></span>

## <a name="create-your-plan"></a><span data-ttu-id="dc77d-146">Vytvoření plánu</span><span class="sxs-lookup"><span data-stu-id="dc77d-146">Create your plan</span></span>

<span data-ttu-id="dc77d-147">V tomto postupu definujete plán nebo plány, které chcete pro svou nabídku povolit.</span><span class="sxs-lookup"><span data-stu-id="dc77d-147">In these steps you’ll define the plan or plans you want to enable for your offer.</span></span>

1. <span data-ttu-id="dc77d-148">V levé navigační nabídce vyberte **Přehled plánu** a pak vyberte Vytvořit **nový plán.**</span><span class="sxs-lookup"><span data-stu-id="dc77d-148">On the left navigation menu, select **Plan overview**, and then select **Create new plan**.</span></span>
2. <span data-ttu-id="dc77d-149">Zadejte **ID plánu a** **název plánu** a pak vyberte **Vytvořit.**</span><span class="sxs-lookup"><span data-stu-id="dc77d-149">Enter a **Plan ID** and **Plan name**, and then select **Create**.</span></span>
3. <span data-ttu-id="dc77d-150">Na stránce **Výpis** plánu zadejte popis **plánu**.</span><span class="sxs-lookup"><span data-stu-id="dc77d-150">On the **Plan listing** page, enter your **Plan description**.</span></span>
4. <span data-ttu-id="dc77d-151">Pokud chcete popis uložit a dokončit ho později, vyberte **Save draft (Uložit koncept).**</span><span class="sxs-lookup"><span data-stu-id="dc77d-151">To save the description and finish later, select **Save draft**.</span></span>

5. <span data-ttu-id="dc77d-152">Až budete hotovi, vyberte Zkontrolovat a **publikovat**.</span><span class="sxs-lookup"><span data-stu-id="dc77d-152">When you’re finished, select **Review and publish**.</span></span> <span data-ttu-id="dc77d-153">Informace o plánu se teď zobrazí v části appsource.microsoft.com výpisu nabídek (oddíl plány).</span><span class="sxs-lookup"><span data-stu-id="dc77d-153">The plan information will now be displayed on appsource.microsoft.com under offer listing (plans section).</span></span>

6. <span data-ttu-id="dc77d-154">Po vytvoření všech plánů pro tuto nabídku budete muset zkopírovat ID služby každého plánu.</span><span class="sxs-lookup"><span data-stu-id="dc77d-154">After you’ve created all of the plans for this offer, you’ll need to copy each plan’s Service ID.</span></span> <span data-ttu-id="dc77d-155">V **horní části** stránky Výpis plánu vyberte Přehled plánu.</span><span class="sxs-lookup"><span data-stu-id="dc77d-155">Select **Plan overview** at the top of the Plan listing page.</span></span> <span data-ttu-id="dc77d-156">Zkopírujte ID služby pro každý plán do bezpečného umístění.</span><span class="sxs-lookup"><span data-stu-id="dc77d-156">Copy the Service ID for each plan to a safe location.</span></span>

## <a name="add-service-ids-to-your-solution"></a><span data-ttu-id="dc77d-157">Přidání ID služeb do řešení</span><span class="sxs-lookup"><span data-stu-id="dc77d-157">Add Service IDs to your solution</span></span>

<span data-ttu-id="dc77d-158">Dalším krokem je aktualizace řešení přidáním ID služeb pro každý plán, který jste právě zkopíroval.</span><span class="sxs-lookup"><span data-stu-id="dc77d-158">The next step is to update your solution by adding the Service IDs for each plan that you just copied.</span></span> <span data-ttu-id="dc77d-159">Pokyny najdete v tématu [Vytvoření balíčku AppSource pro vaše řešení.](/powerapps/developer/data-platform/create-package-app-appsource)</span><span class="sxs-lookup"><span data-stu-id="dc77d-159">For guidance on this, see [Create an AppSource Package for your solution](/powerapps/developer/data-platform/create-package-app-appsource).</span></span>

## <a name="upload-your-package-and-publish-your-offer"></a><span data-ttu-id="dc77d-160">Nahrání balíčku a publikování nabídky</span><span class="sxs-lookup"><span data-stu-id="dc77d-160">Upload your package and publish your offer</span></span>

1. <span data-ttu-id="dc77d-161">V levém navigačním podokně vyberte **Komerční marketplace** a pak vyberte **Technická konfigurace**.</span><span class="sxs-lookup"><span data-stu-id="dc77d-161">On the left navigation pane, select **Commercial Marketplace**, and then select **Technical configuration**.</span></span>
2. <span data-ttu-id="dc77d-162">V **části Základní licenční model** vyberte **Uživatel.**</span><span class="sxs-lookup"><span data-stu-id="dc77d-162">Under **Base License Model**, select **User**.</span></span>
3. <span data-ttu-id="dc77d-163">V **části Crm Package**(Balíček CRM) zadejte adresu URL umístění vašeho balíčku.</span><span class="sxs-lookup"><span data-stu-id="dc77d-163">Under **CRM Package**, enter the URL of your package location.</span></span>
4. <span data-ttu-id="dc77d-164">Pomocí ostatních karet v levém navigačním podokně zadejte další požadované informace.</span><span class="sxs-lookup"><span data-stu-id="dc77d-164">Use the other tabs on the left navigation pane to enter any other required information.</span></span> <span data-ttu-id="dc77d-165">Až budete hotovi, vyberte Zkontrolovat a **publikovat.**</span><span class="sxs-lookup"><span data-stu-id="dc77d-165">When you’re done, select **Review and publish**.</span></span>

<span data-ttu-id="dc77d-166">Po publikování nabídky si vaše informace ověříme a ověříme.</span><span class="sxs-lookup"><span data-stu-id="dc77d-166">After you publish the offer, we’ll review and verify your information.</span></span> <span data-ttu-id="dc77d-167">Pokud s tímto procesem dojde k nějakým potížím, budeme vás informovat.</span><span class="sxs-lookup"><span data-stu-id="dc77d-167">If there are any issues with this process, we’ll notify you.</span></span> <span data-ttu-id="dc77d-168">Po vyřešení všech problémů se zobrazí oznámení, že vaše nabídka bude k dispozici v AppSource.</span><span class="sxs-lookup"><span data-stu-id="dc77d-168">When all issues have been resolved, you’ll get a notification that your offer is available in AppSource.</span></span> <span data-ttu-id="dc77d-169">V tomto okamžiku ji můžete nastavit jako živou.</span><span class="sxs-lookup"><span data-stu-id="dc77d-169">At that point you can make it live.</span></span>

## <a name="make-your-offer-live-in-partner-center"></a><span data-ttu-id="dc77d-170">Zajištění živé nabídky v partnerském centru</span><span class="sxs-lookup"><span data-stu-id="dc77d-170">Make your offer live in Partner Center</span></span>

<span data-ttu-id="dc77d-171">Následující postup vás provede procesem zajištění živé nabídky v AppSource.</span><span class="sxs-lookup"><span data-stu-id="dc77d-171">The procedure below walks you through the process of making your offer live in AppSource.</span></span> <span data-ttu-id="dc77d-172">Další informace o tomto procesu najdete v tématu [Úvod do možností výpisu](/azure/marketplace/determine-your-listing-type).</span><span class="sxs-lookup"><span data-stu-id="dc77d-172">To learn more about this process, see [Introduction to listing options](/azure/marketplace/determine-your-listing-type).</span></span>

>[!NOTE]
><span data-ttu-id="dc77d-173">Po publikování vaší nabídky bude trvat 4-6 hodin, než budete moct zasílat.</span><span class="sxs-lookup"><span data-stu-id="dc77d-173">Once you publish your offer, it will take 4-6 hours to go live.</span></span>

1. <span data-ttu-id="dc77d-174">Přihlaste se k [řídicímu panelu pro Partnerské centrum](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="dc77d-174">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="dc77d-175">V levé navigační nabídce vyberte **komerční Marketplace/přehled**.</span><span class="sxs-lookup"><span data-stu-id="dc77d-175">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="dc77d-176">Na stránce **Přehled** Najděte nabídku, kterou hledáte.</span><span class="sxs-lookup"><span data-stu-id="dc77d-176">On the **Overview** page, find the offer you’re looking for.</span></span> <span data-ttu-id="dc77d-177">Nabídky připravené k publikování budou mít stav **Preview**.</span><span class="sxs-lookup"><span data-stu-id="dc77d-177">Offers ready to be published will have a status of **Preview**.</span></span> <span data-ttu-id="dc77d-178">Vyberte nabídku.</span><span class="sxs-lookup"><span data-stu-id="dc77d-178">Select the offer.</span></span>
4. <span data-ttu-id="dc77d-179">Na stránce **Přehled nabídky** vyberte možnost **Přejít na aktivní**.</span><span class="sxs-lookup"><span data-stu-id="dc77d-179">On the **Offer overview** page, select **Go live**.</span></span>
<span data-ttu-id="dc77d-180">Nabídka bude živá během 4-6 hodin.</span><span class="sxs-lookup"><span data-stu-id="dc77d-180">The offer will be live in 4-6 hours.</span></span>
5. <span data-ttu-id="dc77d-181">Pokud chcete zobrazit seznam nabídek na AppSource, vyberte odkaz **AppSource** v dolní části stránky s **přehledem nabídky** .</span><span class="sxs-lookup"><span data-stu-id="dc77d-181">To see your offer listing on AppSource, select the **AppSource** link at the bottom of the **Offer overview** page.</span></span>

    - <span data-ttu-id="dc77d-182">**Pro nabídky s povolenými licencemi**: Pokud vaše nabídka vyžaduje kontrolu licencí, uživatelé budou moct zadat zájemce jenom tak, že kliknou na **kontaktovat**, abyste s nimi mohli komunikovat.</span><span class="sxs-lookup"><span data-stu-id="dc77d-182">**For license-enabled offers**: If your offer requires a license check, users will only be able to enter a lead by clicking **Contact Me**, so that you can communicate with them.</span></span>

    - <span data-ttu-id="dc77d-183">**U nabídek s povolenými licencemi s možností bezplatné instalace**: Pokud vaše nabídka nevyžaduje kontrolu licencí, uživatelům s oprávněními správce se zobrazí tlačítko **získat nyní** , aby se **mi kontaktovalo**.</span><span class="sxs-lookup"><span data-stu-id="dc77d-183">**For license-enabled offers with free installation option**: If your offer does not require a license check, admin users will see a **Get It Now** button in addition to **Contact Me**.</span></span> <span data-ttu-id="dc77d-184">Uživatelé, kteří chtějí vyzkoušet možnost bezplatné instalace, by měli kliknout na **získat hned**, což jim umožní nainstalovat nabídku do centra pro správu Power Platform.</span><span class="sxs-lookup"><span data-stu-id="dc77d-184">Users who want to try your free installation option should click **Get It Now**, which will bring them to install the offer on Power Platform Admin Center.</span></span> <span data-ttu-id="dc77d-185">Pokud mají uživatelé nějaké dotazy nebo pokud chtějí upgradovat na placený plán, můžou pořád použít **kontakt** .</span><span class="sxs-lookup"><span data-stu-id="dc77d-185">Users can still use **Contact Me** if they have any questions, or if they want to upgrade to a paid plan.</span></span>

## <a name="register-isv-connect-deal-in-deal-registration"></a><span data-ttu-id="dc77d-186">Registrace ISV Connect v registraci koupí</span><span class="sxs-lookup"><span data-stu-id="dc77d-186">Register ISV Connect deal in Deal Registration</span></span>

<span data-ttu-id="dc77d-187">Než budete moct přiřadit licence k zákazníkovi, musíte každý prodej zaregistrovat v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="dc77d-187">Before you can assign licenses to a customer, each sale needs to be registered in Partner Center.</span></span> <span data-ttu-id="dc77d-188">Pokud to chcete udělat, podívejte [se na stránku Registrace dohod.](register-deals.md)</span><span class="sxs-lookup"><span data-stu-id="dc77d-188">To do this, see [Register your deals](register-deals.md).</span></span>

## <a name="invite-the-customer"></a><span data-ttu-id="dc77d-189">Pozvání zákazníka</span><span class="sxs-lookup"><span data-stu-id="dc77d-189">Invite the customer</span></span>

<span data-ttu-id="dc77d-190">Pomocí následujícího postupu pozvěte zákazníka, aby se této dohody účastnil.</span><span class="sxs-lookup"><span data-stu-id="dc77d-190">Use the following procedure to invite the customer to participate in this deal.</span></span>  

1. <span data-ttu-id="dc77d-191">Přihlaste se k [řídicímu panelu pro Partnerské centrum](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="dc77d-191">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="dc77d-192">V levé navigační nabídce vyberte **Komerční marketplace/ Přehled.**</span><span class="sxs-lookup"><span data-stu-id="dc77d-192">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="dc77d-193">V levé navigační nabídce vyberte **Referenční odkazy** a pak vyberte **Registrace dohody.**</span><span class="sxs-lookup"><span data-stu-id="dc77d-193">On the left navigation menu, select **Referrals**, and then select **Deal Registration**.</span></span>
4. <span data-ttu-id="dc77d-194">**Vyfiltrujte Odeslané** dohody, vyberte **kartu Probíhá** a pak vyberte požadovanou dohodu.</span><span class="sxs-lookup"><span data-stu-id="dc77d-194">Filter for **Submitted** deals, select the **In Progress** tab, and then select the deal you want.</span></span>
5. <span data-ttu-id="dc77d-195">Na stránce přehledu pro tuto dohodu vyberte **Spravovat licence.**</span><span class="sxs-lookup"><span data-stu-id="dc77d-195">On the overview page for this deal, select **Manage licenses**.</span></span>
6. <span data-ttu-id="dc77d-196">V **okně Spravovat licence** vyberte zákazníka z rozevíracího seznamu **Podrobnosti** o zákazníkovi.</span><span class="sxs-lookup"><span data-stu-id="dc77d-196">In the **Manage licenses** window, select the customer from the **Customer details** dropdown list.</span></span> <span data-ttu-id="dc77d-197">Pokud vztah se zákazníkem ještě neexistuje, vyberte + Pozvat nového zákazníka k **udělení souhlasu**.</span><span class="sxs-lookup"><span data-stu-id="dc77d-197">If the customer relationship does not exist yet, select **+Invite a new customer to consent**.</span></span>
7. <span data-ttu-id="dc77d-198">Zkopírujte odkaz, který se zobrazí.</span><span class="sxs-lookup"><span data-stu-id="dc77d-198">Copy the link that is displayed.</span></span>
8. <span data-ttu-id="dc77d-199">Pošlete tento odkaz e-mailem správci fakturace nebo globálnímu správci zákazníka a nechat je použít tento odkaz pro přístup k admin.microsoft.com a přijetí a autorizaci navazování vztahu.</span><span class="sxs-lookup"><span data-stu-id="dc77d-199">Email this link to your customer’s billing admin or global admin, and have them use this link to access admin.microsoft.com and accept and authorize the relationship you’re establishing.</span></span>

    >[!NOTE]
    ><span data-ttu-id="dc77d-200">Vztah nebude navázán, dokud zákazník tento krok neprovádí.</span><span class="sxs-lookup"><span data-stu-id="dc77d-200">The relationship will not be established until the customer performs this step.</span></span>

## <a name="activate-manage-and-remove-your-licenses"></a><span data-ttu-id="dc77d-201">Aktivace, správa a odebrání licencí</span><span class="sxs-lookup"><span data-stu-id="dc77d-201">Activate, manage, and remove your licenses</span></span>

<span data-ttu-id="dc77d-202">Jakmile s vám zákazník autorizovaným vztahem začne přidávat plány z nabídky a přiřazovat licence k jednotlivým plánům.</span><span class="sxs-lookup"><span data-stu-id="dc77d-202">Once your customer has authorized the relationship with you, you can start adding plans from your offer and assigning licenses to each plan.</span></span>

1. <span data-ttu-id="dc77d-203">V okně Spravovat licence pro tuto dohodu vyberte **+ Přidat plán**.</span><span class="sxs-lookup"><span data-stu-id="dc77d-203">In the Manage licenses window for this deal, select **+Add a plan**.</span></span>
2. <span data-ttu-id="dc77d-204">Vyplňte **pole Plány pro toto** řešení **a** Počet licencí a pak vyberte **Aktualizovat licence.**</span><span class="sxs-lookup"><span data-stu-id="dc77d-204">Complete the **Plans for this solution** and **Number of licenses** fields, and then select **Update licenses**.</span></span> <span data-ttu-id="dc77d-205">Licence budou k dispozici na admin.microsoft.com, aby je zákazníci spravují a přiřazují zaměstnancům.</span><span class="sxs-lookup"><span data-stu-id="dc77d-205">The licenses will be available at admin.microsoft.com for customers to manage and assign to employees.</span></span>

    - <span data-ttu-id="dc77d-206">Pokud chcete změnit počet licencí pro existující plán, zadejte nové číslo do pole **Počet** licencí a pak vyberte **Aktualizovat licence.**</span><span class="sxs-lookup"><span data-stu-id="dc77d-206">To change the number of licenses for an existing plan, enter the new number in the **Number of licenses** field and then select **Update licenses**.</span></span>

    - <span data-ttu-id="dc77d-207">Pokud chcete deaktivovat nebo odebrat licence pro dohodu,  vyberte ikonu odpadkového koše v poli Akce a pak vyberte **Aktualizovat licence.**</span><span class="sxs-lookup"><span data-stu-id="dc77d-207">To deactivate or remove licenses for a deal, select the trash can icon in the **Actions** field and then select **Update licenses**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="dc77d-208">Další kroky</span><span class="sxs-lookup"><span data-stu-id="dc77d-208">Next steps</span></span>

[<span data-ttu-id="dc77d-209">Zdroje informací o licencování</span><span class="sxs-lookup"><span data-stu-id="dc77d-209">Licensing resources</span></span>](support-resources-licensing.md)