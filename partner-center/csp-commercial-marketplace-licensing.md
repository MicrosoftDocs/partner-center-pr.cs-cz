---
title: Správa licencování v nabídkách Marketplace
ms.topic: how-to
ms.date: 04/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Naučte se, jak nastavit a spravovat licencování pro vaše nabídky ISV komerčního tržiště.
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f049ffda4c3d9476c09257fc814e5acac393cb54
ms.sourcegitcommit: 6c20c3cc4a226cada70c56df295966696affcec8
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/30/2021
ms.locfileid: "108328011"
---
# <a name="manage-licensing-in-marketplace-offers"></a><span data-ttu-id="5063e-103">Správa licencování v nabídkách Marketplace</span><span class="sxs-lookup"><span data-stu-id="5063e-103">Manage licensing in marketplace offers</span></span>

<span data-ttu-id="5063e-104">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="5063e-104">**Appropriate roles**</span></span>

- <span data-ttu-id="5063e-105">Globální správce</span><span class="sxs-lookup"><span data-stu-id="5063e-105">Global admin</span></span>
- <span data-ttu-id="5063e-106">Správce účtu</span><span class="sxs-lookup"><span data-stu-id="5063e-106">Account admin</span></span>

<span data-ttu-id="5063e-107">Tento článek vás provede procesem nastavení nabídky v partnerském centru, jejím zpřístupněním v Microsoft AppSource a následnou správou licencí pro tuto nabídku.</span><span class="sxs-lookup"><span data-stu-id="5063e-107">This article walks you through the process of setting up an offer in Partner Center, making it available in Microsoft AppSource, and then managing licenses for that offer.</span></span>  

>[!IMPORTANT]
><span data-ttu-id="5063e-108">Možnosti v tomto článku jsou momentálně v Public Preview.</span><span class="sxs-lookup"><span data-stu-id="5063e-108">The capabilities in this article are currently in Public Preview.</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="5063e-109">Než začnete</span><span class="sxs-lookup"><span data-stu-id="5063e-109">Before you begin</span></span>

### <a name="commercial-marketplace-basics"></a><span data-ttu-id="5063e-110">Základy komerčního tržiště</span><span class="sxs-lookup"><span data-stu-id="5063e-110">Commercial marketplace basics</span></span>

<span data-ttu-id="5063e-111">Než zahájíte tento proces, měli byste se seznámit se základy komerčního tržiště.</span><span class="sxs-lookup"><span data-stu-id="5063e-111">Before you begin this process, you should familiarize yourself with the basics of the commercial marketplace.</span></span> <span data-ttu-id="5063e-112">Články v následující tabulce vám pomůžou začít.</span><span class="sxs-lookup"><span data-stu-id="5063e-112">The articles in the table below will help get you started.</span></span> 

| <span data-ttu-id="5063e-113">Téma</span><span class="sxs-lookup"><span data-stu-id="5063e-113">Topic</span></span>  | <span data-ttu-id="5063e-114">Článek</span><span class="sxs-lookup"><span data-stu-id="5063e-114">Article</span></span>  |
|-------|--------|
|<span data-ttu-id="5063e-115">Plány komerčního tržiště</span><span class="sxs-lookup"><span data-stu-id="5063e-115">Commercial marketplace plans</span></span> | [<span data-ttu-id="5063e-116">Plány a ceny pro komerční nabídky na webu Marketplace</span><span class="sxs-lookup"><span data-stu-id="5063e-116">Plans and pricing for commercial marketplace offers</span></span>](/azure/marketplace/plans-pricing)    |
|<span data-ttu-id="5063e-117">Nabídky komerčních Marketplace</span><span class="sxs-lookup"><span data-stu-id="5063e-117">Commercial marketplace offers</span></span>  | [<span data-ttu-id="5063e-118">Typy seznamů</span><span class="sxs-lookup"><span data-stu-id="5063e-118">Listing types</span></span>](/azure/marketplace/determine-your-listing-type)    |
|<span data-ttu-id="5063e-119">Účty komerčního tržiště</span><span class="sxs-lookup"><span data-stu-id="5063e-119">Commercial marketplace accounts</span></span> |  [<span data-ttu-id="5063e-120">Vytvoření účtu obchodního tržiště v partnerském centru</span><span class="sxs-lookup"><span data-stu-id="5063e-120">Create a commercial marketplace account in Partner Center</span></span>](/azure/marketplace/create-account) |

### <a name="determine-your-offer-id"></a><span data-ttu-id="5063e-121">Určení ID vaší nabídky</span><span class="sxs-lookup"><span data-stu-id="5063e-121">Determine your Offer ID</span></span>

<span data-ttu-id="5063e-122">V níže uvedených postupech budete vyzváni k zadání ID nabídky.</span><span class="sxs-lookup"><span data-stu-id="5063e-122">In the procedures below, you’ll be prompted to enter an Offer ID.</span></span> <span data-ttu-id="5063e-123">Pořiďte si čas, který vám umožní začít s vhodným ID nabídky. Pamatujte na tyto body:</span><span class="sxs-lookup"><span data-stu-id="5063e-123">Take some time now to come up with a suitable Offer ID, keeping in mind the following points:</span></span>

- <span data-ttu-id="5063e-124">Toto ID je viditelné pro zákazníky na webové adrese pro nabídku webu Marketplace a šablony Azure Resource Manager, pokud jsou k dispozici.</span><span class="sxs-lookup"><span data-stu-id="5063e-124">This ID is visible to customers in the web address for the marketplace offer and Azure Resource Manager templates, if applicable.</span></span>
- <span data-ttu-id="5063e-125">ID nabídky v kombinaci s ID vydavatele musí být kratší než 40 znaků.</span><span class="sxs-lookup"><span data-stu-id="5063e-125">The Offer ID combined with the Publisher ID must be under 40 characters in length.</span></span>
- <span data-ttu-id="5063e-126">Použijte při tom jenom malá písmena a číslice.</span><span class="sxs-lookup"><span data-stu-id="5063e-126">Use only lowercase letters and numbers.</span></span> <span data-ttu-id="5063e-127">ID nabídky může zahrnovat pomlčky a podtržítka, ale ne mezery.</span><span class="sxs-lookup"><span data-stu-id="5063e-127">The Offer ID can include hyphens and underscores, but no spaces.</span></span> <span data-ttu-id="5063e-128">Pokud je například vaším vydavatelem ID `testpublisherid` a zadáte `test-offer-1` , bude webová adresa nabídky `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1` .</span><span class="sxs-lookup"><span data-stu-id="5063e-128">For example, if your Publisher ID is `testpublisherid` and you enter `test-offer-1`, the offer web address will be `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1`.</span></span>
- <span data-ttu-id="5063e-129">Toto ID se po výběru **vytvořit** nedá změnit.</span><span class="sxs-lookup"><span data-stu-id="5063e-129">This ID can't be changed after you select **Create**.</span></span>

### <a name="determine-your-offer-alias"></a><span data-ttu-id="5063e-130">Určení aliasu nabídky</span><span class="sxs-lookup"><span data-stu-id="5063e-130">Determine your Offer alias</span></span>

<span data-ttu-id="5063e-131">Alias nabídky je název, který se používá pro nabídku v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="5063e-131">The Offer alias is the name used for the offer in Partner Center.</span></span> <span data-ttu-id="5063e-132">Budete také potřebovat příslušný alias nabídky, který bude postupovat podle níže uvedených pokynů:</span><span class="sxs-lookup"><span data-stu-id="5063e-132">You’ll also need an appropriate Offer alias that follows the guidelines below:</span></span>

- <span data-ttu-id="5063e-133">Tento název se na webu Marketplace nepoužívá a liší se od názvu nabídky a dalších hodnot, které se zákazníkům zobrazují.</span><span class="sxs-lookup"><span data-stu-id="5063e-133">This name isn't used in the marketplace and is different from the offer name and other values shown to customers.</span></span>
- <span data-ttu-id="5063e-134">Po výběru vytvořit se tento název nedá změnit.</span><span class="sxs-lookup"><span data-stu-id="5063e-134">This name can't be changed after you select Create.</span></span>

## <a name="create-your-offer"></a><span data-ttu-id="5063e-135">Vytvoření nabídky</span><span class="sxs-lookup"><span data-stu-id="5063e-135">Create your offer</span></span>

<span data-ttu-id="5063e-136">Prvním krokem v licenčním procesu je vytvoření komerční nabídky na webu Marketplace.</span><span class="sxs-lookup"><span data-stu-id="5063e-136">The first step in the licensing process is to create your commercial marketplace offer.</span></span> 

1. <span data-ttu-id="5063e-137">Přihlaste se k [řídicímu panelu pro Partnerské centrum](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="5063e-137">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="5063e-138">V levé navigační nabídce vyberte **komerční Marketplace/přehled**.</span><span class="sxs-lookup"><span data-stu-id="5063e-138">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="5063e-139">V horní části stránky přehled vyberte možnost **Nová nabídka** a potom vyberte **Dynamics 365 pro customer Engagement & PowerApps**.</span><span class="sxs-lookup"><span data-stu-id="5063e-139">At the top of the Overview page, select **New offer**, and then select **Dynamics 365 for Customer Engagement & PowerApps**.</span></span>
4. <span data-ttu-id="5063e-140">Zadejte **ID nabídky** a **alias nabídky** , který jste vytvořili dříve.</span><span class="sxs-lookup"><span data-stu-id="5063e-140">Enter the **Offer ID** and **Offer alias** you created earlier.</span></span>
5. <span data-ttu-id="5063e-141">Vyberte **vytvořit** pro vygenerování nabídky a pokračování.</span><span class="sxs-lookup"><span data-stu-id="5063e-141">Select **Create** to generate the offer and continue.</span></span>
6. <span data-ttu-id="5063e-142">Vyberte možnosti licencování.</span><span class="sxs-lookup"><span data-stu-id="5063e-142">Choose your licensing options.</span></span>

    - <span data-ttu-id="5063e-143">Pokud chcete pro vaši nabídku povolit správu licencí, vyberte **Povolit správu licencí aplikací prostřednictvím Microsoftu**.</span><span class="sxs-lookup"><span data-stu-id="5063e-143">To enable license management for your offer, select **Enable app license management through Microsoft**.</span></span> <span data-ttu-id="5063e-144">Jedná se o jednorázové nastavení a po publikování vaší nabídky ho nemůžete změnit.</span><span class="sxs-lookup"><span data-stu-id="5063e-144">This is a one-time setting, and you can’t change it once your offer is published.</span></span>

    - <span data-ttu-id="5063e-145">Zákazníkům taky můžete povolit, aby se základní funkce vaší aplikace spouštěli bez licence, a po zakoupení licence mohli používat prémiové funkce.</span><span class="sxs-lookup"><span data-stu-id="5063e-145">You can also enable customers to run your app’s base functionality without a license, and run premium features once they’ve purchased a license.</span></span> <span data-ttu-id="5063e-146">Pokud to chcete provést, vyberte možnost **Povolit zákazníkům instalaci aplikace i v případě, že licence nejsou přiřazeny**.</span><span class="sxs-lookup"><span data-stu-id="5063e-146">To do this, select **Allow customers to install my app even if licenses are not assigned**.</span></span>

    - <span data-ttu-id="5063e-147">Pokud nechcete, aby vaše nabídka měla povolenou správu licencí, vyberte **získat hned (zdarma)**, **bezplatnou zkušební verzi** nebo **kontaktujte mě**.</span><span class="sxs-lookup"><span data-stu-id="5063e-147">If you don’t want your offer to have license management enabled, select **Get it now (Free)**, **Free trial**, or **Contact me**.</span></span>

## <a name="create-your-plan"></a><span data-ttu-id="5063e-148">Vytvoření plánu</span><span class="sxs-lookup"><span data-stu-id="5063e-148">Create your plan</span></span>

<span data-ttu-id="5063e-149">V těchto krocích budete definovat plán nebo plány, které chcete pro vaši nabídku povolit.</span><span class="sxs-lookup"><span data-stu-id="5063e-149">In these steps you’ll define the plan or plans you want to enable for your offer.</span></span>

1. <span data-ttu-id="5063e-150">V levém navigačním panelu vyberte **plán přehled** a pak vyberte **vytvořit nový plán**.</span><span class="sxs-lookup"><span data-stu-id="5063e-150">On the left navigation menu, select **Plan overview**, and then select **Create new plan**.</span></span>
2. <span data-ttu-id="5063e-151">Zadejte **ID plánu** a **název plánu** a pak vyberte **vytvořit**.</span><span class="sxs-lookup"><span data-stu-id="5063e-151">Enter a **Plan ID** and **Plan name**, and then select **Create**.</span></span>
3. <span data-ttu-id="5063e-152">Na stránce **seznam plánů** zadejte svůj **Popis plánu**.</span><span class="sxs-lookup"><span data-stu-id="5063e-152">On the **Plan listing** page, enter your **Plan description**.</span></span>
4. <span data-ttu-id="5063e-153">Pokud chcete popis Uložit a dokončit později, vyberte **Uložit koncept**.</span><span class="sxs-lookup"><span data-stu-id="5063e-153">To save the description and finish later, select **Save draft**.</span></span>

5. <span data-ttu-id="5063e-154">Až budete hotovi, vyberte **zkontrolovat a publikovat**.</span><span class="sxs-lookup"><span data-stu-id="5063e-154">When you’re finished, select **Review and publish**.</span></span> <span data-ttu-id="5063e-155">Informace o plánu se teď budou zobrazovat na appsource.microsoft.com v části Seznam nabídek (oddíl plány).</span><span class="sxs-lookup"><span data-stu-id="5063e-155">The plan information will now be displayed on appsource.microsoft.com under offer listing (plans section).</span></span>

6. <span data-ttu-id="5063e-156">Po vytvoření všech plánů této nabídky budete muset zkopírovat ID služby každého plánu.</span><span class="sxs-lookup"><span data-stu-id="5063e-156">After you’ve created all of the plans for this offer, you’ll need to copy each plan’s Service ID.</span></span> <span data-ttu-id="5063e-157">V horní části stránky se seznamem plánů vyberte **plán – přehled** .</span><span class="sxs-lookup"><span data-stu-id="5063e-157">Select **Plan overview** at the top of the Plan listing page.</span></span> <span data-ttu-id="5063e-158">Zkopírujte ID služby pro každý plán do bezpečného umístění.</span><span class="sxs-lookup"><span data-stu-id="5063e-158">Copy the Service ID for each plan to a safe location.</span></span>

## <a name="add-service-ids-to-your-solution"></a><span data-ttu-id="5063e-159">Přidání ID služeb do řešení</span><span class="sxs-lookup"><span data-stu-id="5063e-159">Add Service IDs to your solution</span></span>

<span data-ttu-id="5063e-160">Dalším krokem je aktualizace řešení přidáním ID služby pro každý plán, který jste právě zkopírovali.</span><span class="sxs-lookup"><span data-stu-id="5063e-160">The next step is to update your solution by adding the Service IDs for each plan that you just copied.</span></span> <span data-ttu-id="5063e-161">Pokyny k tomuto problému najdete v tématu [Vytvoření balíčku AppSource pro vaše řešení](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource).</span><span class="sxs-lookup"><span data-stu-id="5063e-161">For guidance on this, see [Create an AppSource Package for your solution](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource).</span></span>

## <a name="upload-your-package-and-publish-your-offer"></a><span data-ttu-id="5063e-162">Nahrání balíčku a publikování vaší nabídky</span><span class="sxs-lookup"><span data-stu-id="5063e-162">Upload your package and publish your offer</span></span>

1. <span data-ttu-id="5063e-163">V levém navigačním podokně vyberte **komerční web Marketplace** a pak vyberte **Technická konfigurace**.</span><span class="sxs-lookup"><span data-stu-id="5063e-163">On the left navigation pane, select **Commercial Marketplace**, and then select **Technical configuration**.</span></span>
2. <span data-ttu-id="5063e-164">V části **základní licenční model** vyberte **uživatel**.</span><span class="sxs-lookup"><span data-stu-id="5063e-164">Under **Base License Model**, select **User**.</span></span>
3. <span data-ttu-id="5063e-165">V části **balíček CRM** zadejte adresu URL umístění balíčku.</span><span class="sxs-lookup"><span data-stu-id="5063e-165">Under **CRM Package**, enter the URL of your package location.</span></span>
4. <span data-ttu-id="5063e-166">Další karty v levém navigačním podokně použijte k zadání jakýchkoli dalších požadovaných informací.</span><span class="sxs-lookup"><span data-stu-id="5063e-166">Use the other tabs on the left navigation pane to enter any other required information.</span></span> <span data-ttu-id="5063e-167">Až budete hotovi, vyberte **zkontrolovat a publikovat**.</span><span class="sxs-lookup"><span data-stu-id="5063e-167">When you’re done, select **Review and publish**.</span></span>

<span data-ttu-id="5063e-168">Po publikování této nabídky si probereme a ověříte vaše informace.</span><span class="sxs-lookup"><span data-stu-id="5063e-168">After you publish the offer, we’ll review and verify your information.</span></span> <span data-ttu-id="5063e-169">Pokud s tímto procesem dojde k nějakým potížím, budeme vás informovat.</span><span class="sxs-lookup"><span data-stu-id="5063e-169">If there are any issues with this process, we’ll notify you.</span></span> <span data-ttu-id="5063e-170">Po vyřešení všech problémů se zobrazí oznámení, že vaše nabídka bude k dispozici v AppSource.</span><span class="sxs-lookup"><span data-stu-id="5063e-170">When all issues have been resolved, you’ll get a notification that your offer is available in AppSource.</span></span> <span data-ttu-id="5063e-171">V tomto okamžiku ji můžete nastavit jako živou.</span><span class="sxs-lookup"><span data-stu-id="5063e-171">At that point you can make it live.</span></span>

## <a name="make-your-offer-live-in-partner-center"></a><span data-ttu-id="5063e-172">Zajištění živé nabídky v partnerském centru</span><span class="sxs-lookup"><span data-stu-id="5063e-172">Make your offer live in Partner Center</span></span>

<span data-ttu-id="5063e-173">Následující postup vás provede procesem zajištění živé nabídky v AppSource.</span><span class="sxs-lookup"><span data-stu-id="5063e-173">The procedure below walks you through the process of making your offer live in AppSource.</span></span> <span data-ttu-id="5063e-174">Další informace o tomto procesu najdete v tématu [Úvod do možností výpisu](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type).</span><span class="sxs-lookup"><span data-stu-id="5063e-174">To learn more about this process, see [Introduction to listing options](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type).</span></span>

>[!NOTE]
><span data-ttu-id="5063e-175">Po publikování vaší nabídky bude trvat 4-6 hodin, než budete moct zasílat.</span><span class="sxs-lookup"><span data-stu-id="5063e-175">Once you publish your offer, it will take 4-6 hours to go live.</span></span>

1. <span data-ttu-id="5063e-176">Přihlaste se k [řídicímu panelu pro Partnerské centrum](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="5063e-176">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="5063e-177">V levé navigační nabídce vyberte **komerční Marketplace/přehled**.</span><span class="sxs-lookup"><span data-stu-id="5063e-177">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="5063e-178">Na stránce **Přehled** Najděte nabídku, kterou hledáte.</span><span class="sxs-lookup"><span data-stu-id="5063e-178">On the **Overview** page, find the offer you’re looking for.</span></span> <span data-ttu-id="5063e-179">Nabídky připravené k publikování budou mít stav **Preview**.</span><span class="sxs-lookup"><span data-stu-id="5063e-179">Offers ready to be published will have a status of **Preview**.</span></span> <span data-ttu-id="5063e-180">Vyberte nabídku.</span><span class="sxs-lookup"><span data-stu-id="5063e-180">Select the offer.</span></span>
4. <span data-ttu-id="5063e-181">Na stránce **Přehled nabídky** vyberte možnost **Přejít na aktivní**.</span><span class="sxs-lookup"><span data-stu-id="5063e-181">On the **Offer overview** page, select **Go live**.</span></span>
<span data-ttu-id="5063e-182">Nabídka bude živá během 4-6 hodin.</span><span class="sxs-lookup"><span data-stu-id="5063e-182">The offer will be live in 4-6 hours.</span></span>
5. <span data-ttu-id="5063e-183">Pokud chcete zobrazit seznam nabídek na AppSource, vyberte odkaz **AppSource** v dolní části stránky s **přehledem nabídky** .</span><span class="sxs-lookup"><span data-stu-id="5063e-183">To see your offer listing on AppSource, select the **AppSource** link at the bottom of the **Offer overview** page.</span></span>

    - <span data-ttu-id="5063e-184">**Pro nabídky s povolenými licencemi**: Pokud vaše nabídka vyžaduje kontrolu licencí, uživatelé budou moct zadat zájemce jenom tak, že kliknou na **kontaktovat**, abyste s nimi mohli komunikovat.</span><span class="sxs-lookup"><span data-stu-id="5063e-184">**For license-enabled offers**: If your offer requires a license check, users will only be able to enter a lead by clicking **Contact Me**, so that you can communicate with them.</span></span>

    - <span data-ttu-id="5063e-185">**U nabídek s povolenými licencemi s možností bezplatné instalace**: Pokud vaše nabídka nevyžaduje kontrolu licencí, uživatelům s oprávněními správce se zobrazí tlačítko **získat nyní** , aby se **mi kontaktovalo**.</span><span class="sxs-lookup"><span data-stu-id="5063e-185">**For license-enabled offers with free installation option**: If your offer does not require a license check, admin users will see a **Get It Now** button in addition to **Contact Me**.</span></span> <span data-ttu-id="5063e-186">Uživatelé, kteří chtějí vyzkoušet možnost bezplatné instalace, by měli kliknout na **získat hned**, což jim umožní nainstalovat nabídku do centra pro správu Power Platform.</span><span class="sxs-lookup"><span data-stu-id="5063e-186">Users who want to try your free installation option should click **Get It Now**, which will bring them to install the offer on Power Platform Admin Center.</span></span> <span data-ttu-id="5063e-187">Pokud mají uživatelé nějaké dotazy nebo pokud chtějí upgradovat na placený plán, můžou pořád použít **kontakt** .</span><span class="sxs-lookup"><span data-stu-id="5063e-187">Users can still use **Contact Me** if they have any questions, or if they want to upgrade to a paid plan.</span></span>

## <a name="register-isv-connect-deal-in-deal-registration"></a><span data-ttu-id="5063e-188">Registrace ISV Connect v registraci koupí</span><span class="sxs-lookup"><span data-stu-id="5063e-188">Register ISV Connect deal in Deal Registration</span></span>

<span data-ttu-id="5063e-189">Než budete moct přiřadit licence k zákazníkovi, musíte každý prodej zaregistrovat v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="5063e-189">Before you can assign licenses to a customer, each sale needs to be registered in Partner Center.</span></span> <span data-ttu-id="5063e-190">Postup najdete v tématu [registrace vašich obchodů](register-deals.md).</span><span class="sxs-lookup"><span data-stu-id="5063e-190">To do this, see [Register your deals](register-deals.md).</span></span>

## <a name="invite-the-customer"></a><span data-ttu-id="5063e-191">Pozvat zákazníka</span><span class="sxs-lookup"><span data-stu-id="5063e-191">Invite the customer</span></span>

<span data-ttu-id="5063e-192">Následující postup slouží k pozvání zákazníka k účasti v této koupi.</span><span class="sxs-lookup"><span data-stu-id="5063e-192">Use the following procedure to invite the customer to participate in this deal.</span></span>  

1. <span data-ttu-id="5063e-193">Přihlaste se k [řídicímu panelu pro Partnerské centrum](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="5063e-193">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="5063e-194">V levé navigační nabídce vyberte **komerční Marketplace/přehled**.</span><span class="sxs-lookup"><span data-stu-id="5063e-194">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="5063e-195">V navigační nabídce vlevo vyberte **odkazy** a pak vyberte **registrace koupek**.</span><span class="sxs-lookup"><span data-stu-id="5063e-195">On the left navigation menu, select **Referrals**, and then select **Deal Registration**.</span></span>
4. <span data-ttu-id="5063e-196">Filtr pro **odeslané** obchody vyberte kartu **probíhá** a pak vyberte obchod, kterou chcete.</span><span class="sxs-lookup"><span data-stu-id="5063e-196">Filter for **Submitted** deals, select the **In Progress** tab, and then select the deal you want.</span></span>
5. <span data-ttu-id="5063e-197">Na stránce Přehled této práce vyberte **spravovat licence**.</span><span class="sxs-lookup"><span data-stu-id="5063e-197">On the overview page for this deal, select **Manage licenses**.</span></span>
6. <span data-ttu-id="5063e-198">V okně **spravovat licence** vyberte zákazníka v rozevíracím seznamu **Podrobnosti o zákazníkovi** .</span><span class="sxs-lookup"><span data-stu-id="5063e-198">In the **Manage licenses** window, select the customer from the **Customer details** dropdown list.</span></span> <span data-ttu-id="5063e-199">Pokud ještě neexistuje vztah zákazníka, vyberte **+ pozvat nového zákazníka k souhlasu**.</span><span class="sxs-lookup"><span data-stu-id="5063e-199">If the customer relationship does not exist yet, select **+Invite a new customer to consent**.</span></span>
7. <span data-ttu-id="5063e-200">Zkopírujte zobrazený odkaz.</span><span class="sxs-lookup"><span data-stu-id="5063e-200">Copy the link that is displayed.</span></span>
8. <span data-ttu-id="5063e-201">Tento odkaz odešlete e-mailem zákazníkovi nebo globálnímu správci fakturace zákazníka a požádejte ho, aby používali tento odkaz k přístupu k admin.microsoft.com a přijetí a autorizaci vztahu, který vytváříte.</span><span class="sxs-lookup"><span data-stu-id="5063e-201">Email this link to your customer’s billing admin or global admin, and have them use this link to access admin.microsoft.com and accept and authorize the relationship you’re establishing.</span></span>

    >[!NOTE]
    ><span data-ttu-id="5063e-202">Relace nebude navázána, dokud zákazník neprovede tento krok.</span><span class="sxs-lookup"><span data-stu-id="5063e-202">The relationship will not be established until the customer performs this step.</span></span>

## <a name="activate-manage-and-remove-your-licenses"></a><span data-ttu-id="5063e-203">Aktivace, Správa a odebírání licencí</span><span class="sxs-lookup"><span data-stu-id="5063e-203">Activate, manage, and remove your licenses</span></span>

<span data-ttu-id="5063e-204">Jakmile se vám s vámi zákazník autorizuje, můžete začít přidávat plány z nabídky a přiřazovat licence k jednotlivým plánům.</span><span class="sxs-lookup"><span data-stu-id="5063e-204">Once your customer has authorized the relationship with you, you can start adding plans from your offer and assigning licenses to each plan.</span></span>

1. <span data-ttu-id="5063e-205">V okně Spravovat licence pro tento obchod vyberte **+ Přidat plán**.</span><span class="sxs-lookup"><span data-stu-id="5063e-205">In the Manage licenses window for this deal, select **+Add a plan**.</span></span>
2. <span data-ttu-id="5063e-206">Dokončete **plány pro toto řešení** a **počet licencí** a pak vyberte **aktualizovat licence**.</span><span class="sxs-lookup"><span data-stu-id="5063e-206">Complete the **Plans for this solution** and **Number of licenses** fields, and then select **Update licenses**.</span></span> <span data-ttu-id="5063e-207">Licence budou k dispozici na adrese admin.microsoft.com, aby si zákazníci mohli spravovat a přiřazovat k zaměstnancům.</span><span class="sxs-lookup"><span data-stu-id="5063e-207">The licenses will be available at admin.microsoft.com for customers to manage and assign to employees.</span></span>

    - <span data-ttu-id="5063e-208">Pokud chcete změnit počet licencí pro existující plán, zadejte nové číslo do pole **počet licencí** a pak vyberte **aktualizovat licence**.</span><span class="sxs-lookup"><span data-stu-id="5063e-208">To change the number of licenses for an existing plan, enter the new number in the **Number of licenses** field and then select **Update licenses**.</span></span>

    - <span data-ttu-id="5063e-209">Pokud chcete deaktivovat nebo odebrat licence pro určitý obchod, vyberte v poli **Akce** ikonu odpadkového koše a pak vyberte **aktualizovat licence**.</span><span class="sxs-lookup"><span data-stu-id="5063e-209">To deactivate or remove licenses for a deal, select the trash can icon in the **Actions** field and then select **Update licenses**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="5063e-210">Další kroky</span><span class="sxs-lookup"><span data-stu-id="5063e-210">Next steps</span></span>

[<span data-ttu-id="5063e-211">Zdroje informací o licencování</span><span class="sxs-lookup"><span data-stu-id="5063e-211">Licensing resources</span></span>](support-resources-licensing.md)
