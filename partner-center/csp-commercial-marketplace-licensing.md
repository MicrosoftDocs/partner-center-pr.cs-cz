---
title: Správa licencování v nabídkách Marketplace
ms.topic: how-to
ms.date: 04/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Naučte se, jak nastavit a spravovat licencování pro vaše nabídky ISV komerčního tržiště.
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3b2281696a2fe69253cd033eb2a7eef7fb3046f3
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284885"
---
# <a name="manage-licensing-in-marketplace-offers"></a><span data-ttu-id="bae13-103">Správa licencování v nabídkách Marketplace</span><span class="sxs-lookup"><span data-stu-id="bae13-103">Manage licensing in marketplace offers</span></span>

<span data-ttu-id="bae13-104">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="bae13-104">**Appropriate roles**</span></span>

- <span data-ttu-id="bae13-105">Globální správce</span><span class="sxs-lookup"><span data-stu-id="bae13-105">Global admin</span></span>
- <span data-ttu-id="bae13-106">Správce účtu</span><span class="sxs-lookup"><span data-stu-id="bae13-106">Account admin</span></span>

<span data-ttu-id="bae13-107">Tento článek vás provede procesem nastavení nabídky v partnerském centru, jejím zpřístupněním v Microsoft AppSource a následnou správou licencí pro tuto nabídku.</span><span class="sxs-lookup"><span data-stu-id="bae13-107">This article walks you through the process of setting up an offer in Partner Center, making it available in Microsoft AppSource, and then managing licenses for that offer.</span></span>  

>[!IMPORTANT]
><span data-ttu-id="bae13-108">Možnosti v tomto článku jsou momentálně v Public Preview.</span><span class="sxs-lookup"><span data-stu-id="bae13-108">The capabilities in this article are currently in Public Preview.</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="bae13-109">Než začnete</span><span class="sxs-lookup"><span data-stu-id="bae13-109">Before you begin</span></span>

<span data-ttu-id="bae13-110">Před zahájením tohoto procesu byste se měli seznámit s informacemi uvedenými níže.</span><span class="sxs-lookup"><span data-stu-id="bae13-110">Before beginning this process, you should familiarize yourself with the information below.</span></span>

### <a name="review-the-azure-marketplace-documentation"></a><span data-ttu-id="bae13-111">Přečtěte si dokumentaci k Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="bae13-111">Review the Azure Marketplace documentation</span></span>

<span data-ttu-id="bae13-112">Níže uvedené články obsahují informace, které byste měli znát, než budete pokračovat.</span><span class="sxs-lookup"><span data-stu-id="bae13-112">The articles below contain information you should know before continuing.</span></span> 

- [<span data-ttu-id="bae13-113">Vytvoření nabídky Dynamics 365 for Customer Engagement a PowerApps</span><span class="sxs-lookup"><span data-stu-id="bae13-113">Create a Dynamics 365 for Customer Engagement & PowerApps offer</span></span>](https://docs.microsoft.com/azure/marketplace/dynamics-365-customer-engage-offer-setup)
- [<span data-ttu-id="bae13-114">Vytvoření účtu obchodního tržiště v partnerském centru</span><span class="sxs-lookup"><span data-stu-id="bae13-114">Create a commercial marketplace account in Partner Center</span></span>](https://docs.microsoft.com/azure/marketplace/create-account)

### <a name="create-your-offer-id"></a><span data-ttu-id="bae13-115">Vytvoření ID nabídky</span><span class="sxs-lookup"><span data-stu-id="bae13-115">Create your Offer ID</span></span>

<span data-ttu-id="bae13-116">V níže uvedených postupech budete vyzváni k zadání ID nabídky.</span><span class="sxs-lookup"><span data-stu-id="bae13-116">In the procedures below, you’ll be prompted to enter an Offer ID.</span></span> <span data-ttu-id="bae13-117">Pořiďte si čas, který vám umožní začít s vhodným ID nabídky. Pamatujte na tyto body:</span><span class="sxs-lookup"><span data-stu-id="bae13-117">Take some time now to come up with a suitable Offer ID, keeping in mind the following points:</span></span>

- <span data-ttu-id="bae13-118">Toto ID je viditelné pro zákazníky na webové adrese pro nabídku webu Marketplace a šablony Azure Resource Manager, pokud jsou k dispozici.</span><span class="sxs-lookup"><span data-stu-id="bae13-118">This ID is visible to customers in the web address for the marketplace offer and Azure Resource Manager templates, if applicable.</span></span>
- <span data-ttu-id="bae13-119">ID nabídky v kombinaci s ID vydavatele musí být kratší než 40 znaků.</span><span class="sxs-lookup"><span data-stu-id="bae13-119">The Offer ID combined with the Publisher ID must be under 40 characters in length.</span></span>
- <span data-ttu-id="bae13-120">Použijte při tom jenom malá písmena a číslice.</span><span class="sxs-lookup"><span data-stu-id="bae13-120">Use only lowercase letters and numbers.</span></span> <span data-ttu-id="bae13-121">ID nabídky může zahrnovat pomlčky a podtržítka, ale ne mezery.</span><span class="sxs-lookup"><span data-stu-id="bae13-121">The Offer ID can include hyphens and underscores, but no spaces.</span></span> <span data-ttu-id="bae13-122">Pokud je například ID vydavatele testpublisherid a zadáte test-nabídka-1, bude webová adresa nabídky https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1 .</span><span class="sxs-lookup"><span data-stu-id="bae13-122">For example, if your Publisher ID is testpublisherid and you enter test-offer-1, the offer web address will be https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1.</span></span>
- <span data-ttu-id="bae13-123">Toto ID se po výběru **vytvořit** nedá změnit.</span><span class="sxs-lookup"><span data-stu-id="bae13-123">This ID can't be changed after you select **Create**.</span></span>

### <a name="create-your-offer-alias"></a><span data-ttu-id="bae13-124">Vytvoření aliasu nabídky</span><span class="sxs-lookup"><span data-stu-id="bae13-124">Create your Offer alias</span></span>

<span data-ttu-id="bae13-125">Alias nabídky je název, který se používá pro nabídku v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="bae13-125">The Offer alias is the name used for the offer in Partner Center.</span></span> <span data-ttu-id="bae13-126">Budete také potřebovat příslušný alias nabídky, který bude postupovat podle níže uvedených pokynů:</span><span class="sxs-lookup"><span data-stu-id="bae13-126">You’ll also need an appropriate Offer alias that follows the guidelines below:</span></span>

- <span data-ttu-id="bae13-127">Tento název se na webu Marketplace nepoužívá a liší se od názvu nabídky a dalších hodnot, které se zákazníkům zobrazují.</span><span class="sxs-lookup"><span data-stu-id="bae13-127">This name isn't used in the marketplace and is different from the offer name and other values shown to customers.</span></span>
- <span data-ttu-id="bae13-128">Po výběru vytvořit se tento název nedá změnit.</span><span class="sxs-lookup"><span data-stu-id="bae13-128">This name can't be changed after you select Create.</span></span>

## <a name="create-your-offer"></a><span data-ttu-id="bae13-129">Vytvoření nabídky</span><span class="sxs-lookup"><span data-stu-id="bae13-129">Create your offer</span></span>

<span data-ttu-id="bae13-130">Prvním krokem v licenčním procesu je vytvoření komerční nabídky na webu Marketplace.</span><span class="sxs-lookup"><span data-stu-id="bae13-130">The first step in the licensing process is to create your commercial marketplace offer.</span></span> 

1. <span data-ttu-id="bae13-131">Přihlaste se k [řídicímu panelu pro Partnerské centrum](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="bae13-131">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="bae13-132">V levé navigační nabídce vyberte **komerční Marketplace/přehled**.</span><span class="sxs-lookup"><span data-stu-id="bae13-132">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="bae13-133">V horní části stránky přehled vyberte možnost **Nová nabídka** a potom vyberte **Dynamics 365 pro customer Engagement & PowerApps**.</span><span class="sxs-lookup"><span data-stu-id="bae13-133">At the top of the Overview page, select **New offer**, and then select **Dynamics 365 for Customer Engagement & PowerApps**.</span></span>
4. <span data-ttu-id="bae13-134">Zadejte **ID nabídky** a **alias nabídky** , který jste vytvořili dříve.</span><span class="sxs-lookup"><span data-stu-id="bae13-134">Enter the **Offer ID** and **Offer alias** you created earlier.</span></span>
5. <span data-ttu-id="bae13-135">Vyberte **vytvořit** pro vygenerování nabídky a pokračování.</span><span class="sxs-lookup"><span data-stu-id="bae13-135">Select **Create** to generate the offer and continue.</span></span>
6. <span data-ttu-id="bae13-136">Vyberte možnosti licencování.</span><span class="sxs-lookup"><span data-stu-id="bae13-136">Choose your licensing options.</span></span>

    - <span data-ttu-id="bae13-137">Pokud chcete pro vaši nabídku povolit správu licencí, vyberte **Povolit správu licencí aplikací prostřednictvím Microsoftu**.</span><span class="sxs-lookup"><span data-stu-id="bae13-137">To enable license management for your offer, select **Enable app license management through Microsoft**.</span></span> <span data-ttu-id="bae13-138">Jedná se o jednorázové nastavení a po publikování vaší nabídky ho nemůžete změnit.</span><span class="sxs-lookup"><span data-stu-id="bae13-138">This is a one-time setting, and you can’t change it once your offer is published.</span></span>

    - <span data-ttu-id="bae13-139">Zákazníkům taky můžete povolit, aby se základní funkce vaší aplikace spouštěli bez licence, a po zakoupení licence mohli používat prémiové funkce.</span><span class="sxs-lookup"><span data-stu-id="bae13-139">You can also enable customers to run your app’s base functionality without a license, and run premium features once they’ve purchased a license.</span></span> <span data-ttu-id="bae13-140">Pokud to chcete provést, vyberte možnost **Povolit zákazníkům instalaci aplikace i v případě, že licence nejsou přiřazeny**.</span><span class="sxs-lookup"><span data-stu-id="bae13-140">To do this, select **Allow customers to install my app even if licenses are not assigned**.</span></span>

    - <span data-ttu-id="bae13-141">Pokud nechcete, aby vaše nabídka měla povolenou správu licencí, vyberte **získat hned (zdarma)**, **bezplatnou zkušební verzi** nebo **kontaktujte mě**.</span><span class="sxs-lookup"><span data-stu-id="bae13-141">If you don’t want your offer to have license management enabled, select **Get it now (Free)**, **Free trial**, or **Contact me**.</span></span>

## <a name="create-your-plan"></a><span data-ttu-id="bae13-142">Vytvoření plánu</span><span class="sxs-lookup"><span data-stu-id="bae13-142">Create your plan</span></span>

<span data-ttu-id="bae13-143">V těchto krocích budete definovat plán nebo plány, které chcete pro vaši nabídku povolit.</span><span class="sxs-lookup"><span data-stu-id="bae13-143">In these steps you’ll define the plan or plans you want to enable for your offer.</span></span>

1. <span data-ttu-id="bae13-144">V levém navigačním panelu vyberte **plán přehled** a pak vyberte **vytvořit nový plán**.</span><span class="sxs-lookup"><span data-stu-id="bae13-144">On the left navigation menu, select **Plan overview**, and then select **Create new plan**.</span></span>
2. <span data-ttu-id="bae13-145">Zadejte **ID plánu** a **název plánu** a pak vyberte **vytvořit**.</span><span class="sxs-lookup"><span data-stu-id="bae13-145">Enter a **Plan ID** and **Plan name**, and then select **Create**.</span></span>
3. <span data-ttu-id="bae13-146">Na stránce **seznam plánů** zadejte svůj **Popis plánu**.</span><span class="sxs-lookup"><span data-stu-id="bae13-146">On the **Plan listing** page, enter your **Plan description**.</span></span>
4. <span data-ttu-id="bae13-147">Pokud chcete popis Uložit a dokončit později, vyberte **Uložit koncept**.</span><span class="sxs-lookup"><span data-stu-id="bae13-147">To save the description and finish later, select **Save draft**.</span></span>

5. <span data-ttu-id="bae13-148">Až budete hotovi, vyberte **zkontrolovat a publikovat**.</span><span class="sxs-lookup"><span data-stu-id="bae13-148">When you’re finished, select **Review and publish**.</span></span> <span data-ttu-id="bae13-149">Informace o plánu se teď budou zobrazovat na appsource.microsoft.com v části Seznam nabídek (oddíl plány).</span><span class="sxs-lookup"><span data-stu-id="bae13-149">The plan information will now be displayed on appsource.microsoft.com under offer listing (plans section).</span></span>

6. <span data-ttu-id="bae13-150">Po vytvoření všech plánů této nabídky budete muset zkopírovat ID služby každého plánu.</span><span class="sxs-lookup"><span data-stu-id="bae13-150">After you’ve created all of the plans for this offer, you’ll need to copy each plan’s Service ID.</span></span> <span data-ttu-id="bae13-151">V horní části stránky se seznamem plánů vyberte **plán – přehled** .</span><span class="sxs-lookup"><span data-stu-id="bae13-151">Select **Plan overview** at the top of the Plan listing page.</span></span> <span data-ttu-id="bae13-152">Zkopírujte ID služby pro každý plán do bezpečného umístění.</span><span class="sxs-lookup"><span data-stu-id="bae13-152">Copy the Service ID for each plan to a safe location.</span></span>

## <a name="add-service-ids-to-your-solution"></a><span data-ttu-id="bae13-153">Přidání ID služeb do řešení</span><span class="sxs-lookup"><span data-stu-id="bae13-153">Add Service IDs to your solution</span></span>

<span data-ttu-id="bae13-154">Dalším krokem je aktualizace řešení přidáním ID služby pro každý plán, který jste právě zkopírovali.</span><span class="sxs-lookup"><span data-stu-id="bae13-154">The next step is to update your solution by adding the Service IDs for each plan that you just copied.</span></span> <span data-ttu-id="bae13-155">Pokyny k tomuto problému najdete v tématu [Vytvoření balíčku AppSource pro vaše řešení](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource).</span><span class="sxs-lookup"><span data-stu-id="bae13-155">For guidance on this, see [Create an AppSource Package for your solution](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource).</span></span>

## <a name="upload-your-package-and-publish-your-offer"></a><span data-ttu-id="bae13-156">Nahrání balíčku a publikování vaší nabídky</span><span class="sxs-lookup"><span data-stu-id="bae13-156">Upload your package and publish your offer</span></span>

1. <span data-ttu-id="bae13-157">V levém navigačním podokně vyberte **komerční web Marketplace** a pak vyberte **Technická konfigurace**.</span><span class="sxs-lookup"><span data-stu-id="bae13-157">On the left navigation pane, select **Commercial Marketplace**, and then select **Technical configuration**.</span></span>
2. <span data-ttu-id="bae13-158">V části **základní licenční model** vyberte **uživatel**.</span><span class="sxs-lookup"><span data-stu-id="bae13-158">Under **Base License Model**, select **User**.</span></span>
3. <span data-ttu-id="bae13-159">V části **balíček CRM** zadejte adresu URL umístění balíčku.</span><span class="sxs-lookup"><span data-stu-id="bae13-159">Under **CRM Package**, enter the URL of your package location.</span></span>
4. <span data-ttu-id="bae13-160">Další karty v levém navigačním podokně použijte k zadání jakýchkoli dalších požadovaných informací.</span><span class="sxs-lookup"><span data-stu-id="bae13-160">Use the other tabs on the left navigation pane to enter any other required information.</span></span> <span data-ttu-id="bae13-161">Až budete hotovi, vyberte **zkontrolovat a publikovat**.</span><span class="sxs-lookup"><span data-stu-id="bae13-161">When you’re done, select **Review and publish**.</span></span>

<span data-ttu-id="bae13-162">Po publikování této nabídky si probereme a ověříte vaše informace.</span><span class="sxs-lookup"><span data-stu-id="bae13-162">After you publish the offer, we’ll review and verify your information.</span></span> <span data-ttu-id="bae13-163">Pokud s tímto procesem dojde k nějakým potížím, budeme vás informovat.</span><span class="sxs-lookup"><span data-stu-id="bae13-163">If there are any issues with this process, we’ll notify you.</span></span> <span data-ttu-id="bae13-164">Po vyřešení všech problémů se zobrazí oznámení, že vaše nabídka bude k dispozici v AppSource.</span><span class="sxs-lookup"><span data-stu-id="bae13-164">When all issues have been resolved, you’ll get a notification that your offer is available in AppSource.</span></span> <span data-ttu-id="bae13-165">V tomto okamžiku ji můžete nastavit jako živou.</span><span class="sxs-lookup"><span data-stu-id="bae13-165">At that point you can make it live.</span></span>

## <a name="make-your-offer-live-in-partner-center"></a><span data-ttu-id="bae13-166">Zajištění živé nabídky v partnerském centru</span><span class="sxs-lookup"><span data-stu-id="bae13-166">Make your offer live in Partner Center</span></span>

<span data-ttu-id="bae13-167">Následující postup vás provede procesem zajištění živé nabídky v AppSource.</span><span class="sxs-lookup"><span data-stu-id="bae13-167">The procedure below walks you through the process of making your offer live in AppSource.</span></span> <span data-ttu-id="bae13-168">Další informace o tomto procesu najdete v tématu [Úvod do možností výpisu](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type).</span><span class="sxs-lookup"><span data-stu-id="bae13-168">To learn more about this process, see [Introduction to listing options](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type).</span></span>

>[!NOTE]
><span data-ttu-id="bae13-169">Po publikování vaší nabídky bude trvat 4-6 hodin, než budete moct zasílat.</span><span class="sxs-lookup"><span data-stu-id="bae13-169">Once you publish your offer, it will take 4-6 hours to go live.</span></span>

1. <span data-ttu-id="bae13-170">Přihlaste se k [řídicímu panelu pro Partnerské centrum](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="bae13-170">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="bae13-171">V levé navigační nabídce vyberte **komerční Marketplace/přehled**.</span><span class="sxs-lookup"><span data-stu-id="bae13-171">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="bae13-172">Na stránce **Přehled** Najděte nabídku, kterou hledáte.</span><span class="sxs-lookup"><span data-stu-id="bae13-172">On the **Overview** page, find the offer you’re looking for.</span></span> <span data-ttu-id="bae13-173">Nabídky připravené k publikování budou mít stav **Preview**.</span><span class="sxs-lookup"><span data-stu-id="bae13-173">Offers ready to be published will have a status of **Preview**.</span></span> <span data-ttu-id="bae13-174">Vyberte nabídku.</span><span class="sxs-lookup"><span data-stu-id="bae13-174">Select the offer.</span></span>
4. <span data-ttu-id="bae13-175">Na stránce **Přehled nabídky** vyberte možnost **Přejít na aktivní**.</span><span class="sxs-lookup"><span data-stu-id="bae13-175">On the **Offer overview** page, select **Go live**.</span></span>
<span data-ttu-id="bae13-176">Nabídka bude živá během 4-6 hodin.</span><span class="sxs-lookup"><span data-stu-id="bae13-176">The offer will be live in 4-6 hours.</span></span>
5. <span data-ttu-id="bae13-177">Pokud chcete zobrazit seznam nabídek na AppSource, vyberte odkaz **AppSource** v dolní části stránky s **přehledem nabídky** .</span><span class="sxs-lookup"><span data-stu-id="bae13-177">To see your offer listing on AppSource, select the **AppSource** link at the bottom of the **Offer overview** page.</span></span>

    - <span data-ttu-id="bae13-178">**Pro nabídky s povolenými licencemi**: Pokud vaše nabídka vyžaduje kontrolu licencí, uživatelé budou moct zadat zájemce jenom tak, že kliknou na **kontaktovat**, abyste s nimi mohli komunikovat.</span><span class="sxs-lookup"><span data-stu-id="bae13-178">**For license-enabled offers**: If your offer requires a license check, users will only be able to enter a lead by clicking **Contact Me**, so that you can communicate with them.</span></span>

    - <span data-ttu-id="bae13-179">**U nabídek s povolenými licencemi s možností bezplatné instalace**: Pokud vaše nabídka nevyžaduje kontrolu licencí, uživatelům s oprávněními správce se zobrazí tlačítko **získat nyní** , aby se **mi kontaktovalo**.</span><span class="sxs-lookup"><span data-stu-id="bae13-179">**For license-enabled offers with free installation option**: If your offer does not require a license check, admin users will see a **Get It Now** button in addition to **Contact Me**.</span></span> <span data-ttu-id="bae13-180">Uživatelé, kteří chtějí vyzkoušet možnost bezplatné instalace, by měli kliknout na **získat hned**, což jim umožní nainstalovat nabídku do centra pro správu Power Platform.</span><span class="sxs-lookup"><span data-stu-id="bae13-180">Users who want to try your free installation option should click **Get It Now**, which will bring them to install the offer on Power Platform Admin Center.</span></span> <span data-ttu-id="bae13-181">Pokud mají uživatelé nějaké dotazy nebo pokud chtějí upgradovat na placený plán, můžou pořád použít **kontakt** .</span><span class="sxs-lookup"><span data-stu-id="bae13-181">Users can still use **Contact Me** if they have any questions, or if they want to upgrade to a paid plan.</span></span>

## <a name="register-isv-connect-deal-in-dealreg"></a><span data-ttu-id="bae13-182">Registrace ISV Connect v DealReg</span><span class="sxs-lookup"><span data-stu-id="bae13-182">Register ISV Connect deal in DealReg</span></span>

<span data-ttu-id="bae13-183">Dalším krokem je registrace vaší koupě.</span><span class="sxs-lookup"><span data-stu-id="bae13-183">The next step is to register your deal.</span></span> <span data-ttu-id="bae13-184">Postup najdete v tématu [registrace vašich obchodů](https://docs.microsoft.com/partner-center/register-deals).</span><span class="sxs-lookup"><span data-stu-id="bae13-184">To do this, see [Register your deals](https://docs.microsoft.com/partner-center/register-deals).</span></span>

## <a name="invite-the-customer"></a><span data-ttu-id="bae13-185">Pozvat zákazníka</span><span class="sxs-lookup"><span data-stu-id="bae13-185">Invite the customer</span></span>

<span data-ttu-id="bae13-186">Následující postup slouží k pozvání zákazníka k účasti v této koupi.</span><span class="sxs-lookup"><span data-stu-id="bae13-186">Use the following procedure to invite the customer to participate in this deal.</span></span>  

1. <span data-ttu-id="bae13-187">Přihlaste se k [řídicímu panelu pro Partnerské centrum](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="bae13-187">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="bae13-188">V levé navigační nabídce vyberte **komerční Marketplace/přehled**.</span><span class="sxs-lookup"><span data-stu-id="bae13-188">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="bae13-189">Filtr pro **odeslané** obchody vyberte kartu **probíhá** a pak vyberte obchod, kterou chcete.</span><span class="sxs-lookup"><span data-stu-id="bae13-189">Filter for **Submitted** deals, select the **In Progress** tab, and then select the deal you want.</span></span>
4. <span data-ttu-id="bae13-190">Na stránce Přehled této práce vyberte **spravovat licence**.</span><span class="sxs-lookup"><span data-stu-id="bae13-190">On the overview page for this deal, select **Manage licenses**.</span></span>
5. <span data-ttu-id="bae13-191">V okně **spravovat licence** vyberte zákazníka v rozevíracím seznamu **Podrobnosti o zákazníkovi** .</span><span class="sxs-lookup"><span data-stu-id="bae13-191">In the **Manage licenses** window, select the customer from the **Customer details** dropdown list.</span></span> <span data-ttu-id="bae13-192">Pokud ještě neexistuje vztah zákazníka, vyberte **+ pozvat nového zákazníka k souhlasu**.</span><span class="sxs-lookup"><span data-stu-id="bae13-192">If the customer relationship does not exist yet, select **+Invite a new customer to consent**.</span></span>
6. <span data-ttu-id="bae13-193">Zkopírujte zobrazený odkaz.</span><span class="sxs-lookup"><span data-stu-id="bae13-193">Copy the link that is displayed.</span></span>
7. <span data-ttu-id="bae13-194">Tento odkaz odešlete e-mailem zákazníkovi nebo globálnímu správci fakturace zákazníka a požádejte ho, aby používali tento odkaz k přístupu k admin.microsoft.com a přijetí a autorizaci vztahu, který vytváříte.</span><span class="sxs-lookup"><span data-stu-id="bae13-194">Email this link to your customer’s billing admin or global admin, and have them use this link to access admin.microsoft.com and accept and authorize the relationship you’re establishing.</span></span>

    >[!NOTE]
    ><span data-ttu-id="bae13-195">Relace nebude navázána, dokud zákazník neprovede tento krok.</span><span class="sxs-lookup"><span data-stu-id="bae13-195">The relationship will not be established until the customer performs this step.</span></span>

## <a name="activate-manage-and-remove-your-licenses"></a><span data-ttu-id="bae13-196">Aktivace, Správa a odebírání licencí</span><span class="sxs-lookup"><span data-stu-id="bae13-196">Activate, manage, and remove your licenses</span></span>

<span data-ttu-id="bae13-197">Po navázání zákazníka můžete začít přidávat plány z nabídky a přiřazovat licence k jednotlivým plánům.</span><span class="sxs-lookup"><span data-stu-id="bae13-197">Once your customer has been established, you can start adding plans from your offer and assigning licenses to each plan.</span></span>

1. <span data-ttu-id="bae13-198">V okně Spravovat licence pro tento obchod vyberte **+ Přidat plán**.</span><span class="sxs-lookup"><span data-stu-id="bae13-198">In the Manage licenses window for this deal, select **+Add a plan**.</span></span>
2. <span data-ttu-id="bae13-199">Dokončete **plány pro toto řešení** a **počet licencí** a pak vyberte **aktualizovat licence**.</span><span class="sxs-lookup"><span data-stu-id="bae13-199">Complete the **Plans for this solution** and **Number of licenses** fields, and then select **Update licenses**.</span></span> <span data-ttu-id="bae13-200">Licence budou k dispozici na adrese admin.microsoft.com, aby si zákazníci mohli spravovat a přiřazovat k zaměstnancům.</span><span class="sxs-lookup"><span data-stu-id="bae13-200">The licenses will be available at admin.microsoft.com for customers to manage and assign to employees.</span></span>

    - <span data-ttu-id="bae13-201">Pokud chcete změnit počet licencí pro existující plán, zadejte nové číslo do pole **počet licencí** a pak vyberte **aktualizovat licence**.</span><span class="sxs-lookup"><span data-stu-id="bae13-201">To change the number of licenses for an existing plan, enter the new number in the **Number of licenses** field and then select **Update licenses**.</span></span>

    - <span data-ttu-id="bae13-202">Pokud chcete deaktivovat nebo odebrat licence pro určitý obchod, vyberte v poli **Akce** ikonu odpadkového koše a pak vyberte **aktualizovat licence**.</span><span class="sxs-lookup"><span data-stu-id="bae13-202">To deactivate or remove licenses for a deal, select the trash can icon in the **Actions** field and then select **Update licenses**.</span></span>