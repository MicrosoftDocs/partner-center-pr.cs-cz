---
title: Konektor pro spoluprodejní účast v partnerském centru pro Salesforce CRM
ms.topic: how-to
ms.date: 01/06/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Synchronizujte své odkazy v partnerském centru se službou Salesforce CRM. Prodejci pak můžou v rámci svých systémů CRM prodávat společně s Microsoftem.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: fa9b35343e1251cfce5caff107de8dff344f4e68
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148410"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="e6bcf-104">Konektor pro společný prodej pro Salesforce CRM – přehled</span><span class="sxs-lookup"><span data-stu-id="e6bcf-104">Co-sell connector for Salesforce CRM - overview</span></span>

<span data-ttu-id="e6bcf-105">**Příslušné role**: Správce odkazů | Správce systému nebo úpravce systému v CRM</span><span class="sxs-lookup"><span data-stu-id="e6bcf-105">**Appropriate roles**: Referrals admin | System admin or system customizer on the CRM</span></span>

<span data-ttu-id="e6bcf-106">Konektor pro spoluprodej v partnerském centru umožňuje prodejcům v rámci svých systémů CRM spolupracovat s Microsoftem.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-106">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="e6bcf-107">Nebudou se muset vyškolet k používání partnerského centra ke správě obchodů v rámci společného prodeje.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-107">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="e6bcf-108">Pomocí konektorů pro spoluprodeji můžete vytvořit nový společný prodejní odkaz, který bude kontaktovat prodejce Microsoftu, získat referenční údaje od prodejce Microsoftu, přijmout nebo odmítnout reference, upravit data o koupi, jako je třeba hodnota koupě a datum ukončení.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-108">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="e6bcf-109">K těmto obchodům v rámci těchto spoluprodejů můžete také dostávat jakékoli aktualizace od prodejců Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-109">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="e6bcf-110">Všechny vaše odkazy fungují při práci v aplikaci CRM dle vašeho výběru a nikoli v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-110">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="e6bcf-111">Řešení je založené na řešení Microsoft Power automatizuje a používá rozhraní API partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-111">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="e6bcf-112">Před instalací – požadavky</span><span class="sxs-lookup"><span data-stu-id="e6bcf-112">Before you install - pre-requisites</span></span>

|<span data-ttu-id="e6bcf-113">**Témata**</span><span class="sxs-lookup"><span data-stu-id="e6bcf-113">**Topics**</span></span>   |<span data-ttu-id="e6bcf-114">**Podrobnosti**</span><span class="sxs-lookup"><span data-stu-id="e6bcf-114">**Details**</span></span>   |<span data-ttu-id="e6bcf-115">**Odkazy**</span><span class="sxs-lookup"><span data-stu-id="e6bcf-115">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="e6bcf-116">ID Microsoft Partner Network</span><span class="sxs-lookup"><span data-stu-id="e6bcf-116">Microsoft Partner Network ID</span></span> |<span data-ttu-id="e6bcf-117">Potřebujete platné ID MPN.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-117">You need a valid MPN ID</span></span>|<span data-ttu-id="e6bcf-118">Připojení k programu [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="e6bcf-118">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="e6bcf-119">Připravený společný prodej</span><span class="sxs-lookup"><span data-stu-id="e6bcf-119">Co-sell ready</span></span>|<span data-ttu-id="e6bcf-120">Vaše řešení IP/Services musí být připravené k prodeji.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-120">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="e6bcf-121">Prodej pomocí Microsoftu</span><span class="sxs-lookup"><span data-stu-id="e6bcf-121">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="e6bcf-122">Účet partnerského centra</span><span class="sxs-lookup"><span data-stu-id="e6bcf-122">Partner Center account</span></span>|<span data-ttu-id="e6bcf-123">ID MPN přidružené k tenantovi partnerského centra musí být stejné jako ID MPN přidružené k vašemu řešení společného prodeje.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-123">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="e6bcf-124">Před nasazením konektorů se můžete podívat na to, jestli máte na portálu partnerského centra zobrazený odkaz na svůj společný prodej.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-124">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="e6bcf-125">Správa vašeho účtu</span><span class="sxs-lookup"><span data-stu-id="e6bcf-125">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="e6bcf-126">Partnerské centrum rolí uživatelů</span><span class="sxs-lookup"><span data-stu-id="e6bcf-126">Partner Center user roles</span></span>|<span data-ttu-id="e6bcf-127">Zaměstnanec, který bude tyto konektory instalovat a používat, musí být správcem referenčních seznamu.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-127">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="e6bcf-128">Přiřazování uživatelských rolí a oprávnění</span><span class="sxs-lookup"><span data-stu-id="e6bcf-128">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="e6bcf-129">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="e6bcf-129">Salesforce CRM</span></span>|<span data-ttu-id="e6bcf-130">Role uživatele CRM je Správce systému nebo Úpravce systému.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-130">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="e6bcf-131">Přiřazení rolí v Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="e6bcf-131">Assign roles in Salesforce CRM</span></span>](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|<span data-ttu-id="e6bcf-132">Power Automate toku</span><span class="sxs-lookup"><span data-stu-id="e6bcf-132">Power Automate Flow Account</span></span>|<span data-ttu-id="e6bcf-133">Aktivní účet [Power Automate](https://flow.microsoft.com) správce systému CRM nebo úpravce systému.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-133">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="e6bcf-134">Tento uživatel by se měl [Power Automate](https://flow.microsoft.com) před instalací alespoň jednou přihlásit.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-134">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="e6bcf-135">Instalace balíčku Salesforce pro vlastní pole Microsoftu</span><span class="sxs-lookup"><span data-stu-id="e6bcf-135">Installation of Salesforce Package for Microsoft Custom Fields</span></span> 

<span data-ttu-id="e6bcf-136">Aby bylo možné synchronizovat referenční Partnerské centrum napříč aplikacemi a salesforce CRM, Power Automate řešení musí jasně identifikovat pole referenčních seznamů specifická pro Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-136">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft-specific referral fields.</span></span> <span data-ttu-id="e6bcf-137">Toto vyněcování poskytuje týmům prodejců partnerů možnost rozhodnout se, které referenční reference chce sdílet s Microsoftem pro spoluprodávku.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-137">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="e6bcf-138">V Salesforce aktivujte **Poznámky** a přidejte je do seznamu příležitostí.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-138">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> 
[<span data-ttu-id="e6bcf-139">Odkaz</span><span class="sxs-lookup"><span data-stu-id="e6bcf-139">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. <span data-ttu-id="e6bcf-140">Aktivujte **týmy příležitostí** pomocí následujících kroků:</span><span class="sxs-lookup"><span data-stu-id="e6bcf-140">Activate **Opportunity teams** by following the steps:</span></span> 
    - <span data-ttu-id="e6bcf-141">V instalačním programu vyhledejte **pomocí pole Rychlé** hledání nastavení týmu příležitostí.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-141">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="e6bcf-142">Definujte nastavení podle potřeby.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-142">Define the settings as needed.</span></span>
[<span data-ttu-id="e6bcf-143">Odkaz</span><span class="sxs-lookup"><span data-stu-id="e6bcf-143">Reference</span></span>](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. <span data-ttu-id="e6bcf-144">V Salesforce nainstalujte vlastní pole a objekty pomocí [instalačního programu balíčků](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV).</span><span class="sxs-lookup"><span data-stu-id="e6bcf-144">In Salesforce, install custom fields and objects using the [package installer](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV).</span></span> <span data-ttu-id="e6bcf-145">Tento nástroj použijte k instalaci balíčku do jakékoli společnosti.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-145">Use this to install the package into any company.</span></span>

>[!NOTE]
><span data-ttu-id="e6bcf-146">Pokud instalujete do sandboxu, musíte počáteční část adresy URL nahradit za . http://test.salesforce.com</span><span class="sxs-lookup"><span data-stu-id="e6bcf-146">If you are installing into a sandbox, you must replace the initial portion of the URL with http://test.salesforce.com</span></span>

4. <span data-ttu-id="e6bcf-147">V Salesforce přidejte řešení Microsoftu do **seznamu souvisejícího** s příležitostí.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-147">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="e6bcf-148">Po přidání vyberte ikonu **klíče** a aktualizujte vlastnosti.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-148">Once added, select the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="e6bcf-149">Osvědčené postupy: test před zahájením provozu</span><span class="sxs-lookup"><span data-stu-id="e6bcf-149">Best Practice: Test before you go live</span></span>

<span data-ttu-id="e6bcf-150">Než nainstalujete, nakonfigurujete a přizpůsobíte řešení Power Automate v produkčním prostředí, ujistěte se, že řešení otestujete v pracovní instanci CRM.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-150">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="e6bcf-151">Nainstalujte řešení Microsoft Power automatizuje do přípravného prostředí/instance CRM.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-151">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="e6bcf-152">Vytvořte kopii řešení a spusťte konfiguraci a automatizujte vlastní nastavení toků v přípravném prostředí.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-152">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="e6bcf-153">Otestujte řešení na pracovní instanci/CRM.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-153">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="e6bcf-154">Po úspěšném dokončení naimportujte jako spravované řešení do produkční instance.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-154">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="e6bcf-155">Nainstalovat synchronizaci odkazů partnerského centra pro Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="e6bcf-155">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="e6bcf-156">V pravém horním rohu vyberte **prostředí** k [automatizaci](https://flow.microsoft.com) a vyberte prostředí.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-156">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="e6bcf-157">Zobrazí se vám dostupné instance CRM.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-157">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="e6bcf-158">V rozevíracím seznamu v pravém horním rohu vyberte příslušnou instanci CRM.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-158">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="e6bcf-159">Na levém navigačním panelu vyberte **řešení** .</span><span class="sxs-lookup"><span data-stu-id="e6bcf-159">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="e6bcf-160">V horní nabídce vyberte odkaz **otevřít AppSource** .</span><span class="sxs-lookup"><span data-stu-id="e6bcf-160">Select the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Otevřít AppSource":::

5. <span data-ttu-id="e6bcf-162">V místní obrazovce vyhledejte **konektory odkazů partnerského centra pro Salesforce** .</span><span class="sxs-lookup"><span data-stu-id="e6bcf-162">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. <span data-ttu-id="e6bcf-164">Vyberte tlačítko **získat nyní** a potom **pokračujte**.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-164">Select the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="e6bcf-165">Otevře se stránka, kde můžete vybrat prostředí Salesforce CRM k instalaci aplikace.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-165">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="e6bcf-166">Vyjádřit souhlas s podmínkami a ujednáními.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-166">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="Dostupné CRMS":::

8. <span data-ttu-id="e6bcf-168">Pak budete přesměrováni na stránku **spravovat vaše řešení** .</span><span class="sxs-lookup"><span data-stu-id="e6bcf-168">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="e6bcf-169">Přejděte na "odkazy na partnerské Centrum" pomocí tlačítek se šipkami ve spodní části stránky.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-169">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="e6bcf-170">**Vedle řešení** referenčních Partnerské centrum by se měla zobrazit naplánovaná instalace.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-170">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="e6bcf-171">Instalace bude trvat 10 až 15 minut.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-171">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="e6bcf-172">Po dokončení instalace přejděte zpět na stránku [Power Automate](https://flow.microsoft.com) **v** levé navigační oblasti vyberte Řešení.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-172">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="e6bcf-173">Všimněte **si Partnerské centrum synchronizace referenčních** seznamu pro Salesforce dostupná v seznamu Řešení.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-173">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="e6bcf-174">Vyberte **Partnerské centrum referenčních seznamu pro Salesforce.**</span><span class="sxs-lookup"><span data-stu-id="e6bcf-174">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="e6bcf-175">K dispozici Power Automate toky a entity:</span><span class="sxs-lookup"><span data-stu-id="e6bcf-175">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Toky Salesforce":::



## <a name="configure-the-solution"></a><span data-ttu-id="e6bcf-177">Konfigurace řešení</span><span class="sxs-lookup"><span data-stu-id="e6bcf-177">Configure the solution</span></span>

1. <span data-ttu-id="e6bcf-178">Po instalaci řešení v instanci CRM přejděte zpět na Power Automate [.](https://flow.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="e6bcf-178">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="e6bcf-179">V **rozevíracím** seznamu Prostředí v pravém horním rohu vyberte instanci CRM, do které jste nainstalovali Power Automate řešení.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-179">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>
3. <span data-ttu-id="e6bcf-180">Budete muset vytvořit připojení, která přidruží tyto tři uživatelské účty:</span><span class="sxs-lookup"><span data-stu-id="e6bcf-180">You will need to create connections that associate the three user accounts:</span></span>
    - <span data-ttu-id="e6bcf-181">Partnerské centrum uživatele s přihlašovacími údaji správce referenčních odkazů</span><span class="sxs-lookup"><span data-stu-id="e6bcf-181">Partner Center user with referrals admin credentials</span></span>
    - <span data-ttu-id="e6bcf-182">Události Partnerského centra</span><span class="sxs-lookup"><span data-stu-id="e6bcf-182">Partner Center Events</span></span>
    - <span data-ttu-id="e6bcf-183">Správce CRM s Power Automate toky v řešení.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-183">CRM admin with the Power Automate flows in the solution.</span></span>
4. <span data-ttu-id="e6bcf-184">V **levém** navigačním panelu vyberte Připojení a ze seznamu vyberte Partnerské centrum referenčních seznamech.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-184">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

5. <span data-ttu-id="e6bcf-185">Vytvořte připojení kliknutím na **Vytvořit připojení.**</span><span class="sxs-lookup"><span data-stu-id="e6bcf-185">Create a connection by clicking **Create a connection**.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Vytvoření připojení":::

- <span data-ttu-id="e6bcf-187">Na panelu Partnerské centrum v pravém horním rohu vyhledejte referenční Partnerské centrum (Preview).</span><span class="sxs-lookup"><span data-stu-id="e6bcf-187">Search for Partner Center Referrals (preview) in the search bar on the top-right corner.</span></span>

- <span data-ttu-id="e6bcf-188">Vytvořte pro svého uživatele Partnerské centrum s rolí přihlašovacích údajů správce referenčních seznamů.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-188">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

-  <span data-ttu-id="e6bcf-189">Dále vytvořte připojení Partnerské centrum události pro vašeho Partnerské centrum uživatele s přihlašovacími údaji správce referenčních seznamů.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-189">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

- <span data-ttu-id="e6bcf-190">Vytvořte připojení pro Salesforce pro uživatele správce CRM.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-190">Create a connection for Salesforce for the CRM administrator user.</span></span>

-  <span data-ttu-id="e6bcf-191">Po přidání všech připojení by se ve vašem prostředí měla zobrazit následující připojení:</span><span class="sxs-lookup"><span data-stu-id="e6bcf-191">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Sledovat připojení":::

### <a name="edit-the-connections"></a><span data-ttu-id="e6bcf-193">Upravit připojení</span><span class="sxs-lookup"><span data-stu-id="e6bcf-193">Edit the connections</span></span>

1. <span data-ttu-id="e6bcf-194">Vraťte se na stránku řešení a vyberte **výchozí řešení**.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-194">Return to the Solutions page and select **Default Solution**.</span></span>  <span data-ttu-id="e6bcf-195">Kliknutím na tlačítko **vše** vyberte **odkaz připojení (Preview)** .</span><span class="sxs-lookup"><span data-stu-id="e6bcf-195">Select **Connection Reference (preview)** by clicking **All**.</span></span>
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Zahájit úpravu konektoru":::

2. <span data-ttu-id="e6bcf-197">Jednotlivá připojení upravte jednotlivě výběrem ikony tři tečky.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-197">Edit each of the Connections individually by selecting the three dots icon.</span></span> <span data-ttu-id="e6bcf-198">Přidejte příslušná připojení.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-198">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Upravit konektory":::

3. <span data-ttu-id="e6bcf-200">Zapněte toky v následujícím pořadí:</span><span class="sxs-lookup"><span data-stu-id="e6bcf-200">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="e6bcf-201">Registrace Webhooku partnerského centra (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="e6bcf-201">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="e6bcf-202">Vytvoření společného prodejního odkazu – Salesforce do partnerského centra (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="e6bcf-202">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="e6bcf-203">Aktualizace referenčních seznamů Microsoftu v partnerském centru pro spoluprodej na Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="e6bcf-203">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="e6bcf-204">Partnerské centrum do Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="e6bcf-204">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="e6bcf-205">Salesforce do partnerského centra (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="e6bcf-205">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="e6bcf-206">Možnost Salesforce v partnerském centru (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="e6bcf-206">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="e6bcf-207">Řešení Salesforce Microsoftu do partnerského centra (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="e6bcf-207">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="e6bcf-208">Použití rozhraní Webhook API k registraci pro události změny prostředku</span><span class="sxs-lookup"><span data-stu-id="e6bcf-208">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="e6bcf-209">Rozhraní API Webhooku partnerského centra vám umožní registrovat se na události změny prostředků.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-209">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="e6bcf-210">Tyto události změny se odesílají na adresu URL jako příspěvky HTTP.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-210">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="e6bcf-211">Pokud chcete zaregistrovat adresu URL, vyberte možnost **registrace Webhooku partnerského centra (Insider Preview)** Power automatizace.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-211">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="e6bcf-212">Přidat připojení pro uživatele partnerského centra (a.) s událostmi partnerského centra s přihlašovacími údaji správce (b.), jak je zvýrazněno níže</span><span class="sxs-lookup"><span data-stu-id="e6bcf-212">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Trigger":::

3. <span data-ttu-id="e6bcf-214">Po provedení těchto aktualizací se zobrazí</span><span class="sxs-lookup"><span data-stu-id="e6bcf-214">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooky":::

4. <span data-ttu-id="e6bcf-216">Uložte změny a vyberte **zapnout**.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-216">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="e6bcf-217">Pokud chcete, aby Webhooky partnerského centra naslouchali změnám událostí, proveďte následující kroky:</span><span class="sxs-lookup"><span data-stu-id="e6bcf-217">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="e6bcf-218">Vyberte **Partnerské centrum pro SALESFORCE CRM (Insider Preview)**.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-218">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="e6bcf-219">Vyberte ikonu **Upravit** a vyberte, **kdy se přijme požadavek HTTP**.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-219">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="e6bcf-220">Kliknutím na ikonu **kopírování** zkopírujte zadanou adresu URL post protokolu HTTP.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-220">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Zkopírování adresy URL":::

8. <span data-ttu-id="e6bcf-222">Nyní vyberte možnost "automatické registrace Webhooku partnerského centra (Insider Preview)" a vyberte **Spustit**.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-222">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="e6bcf-223">Ujistěte se, že se v pravém podokně otevře okno spustit tok a vyberte **pokračovat**.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-223">Ensure that the "Run Flow" window opens on the right-hand pane and select **Continue**.</span></span>

10. <span data-ttu-id="e6bcf-224">Zadejte následující podrobnosti:</span><span class="sxs-lookup"><span data-stu-id="e6bcf-224">Enter the following details:</span></span>

    1. <span data-ttu-id="e6bcf-225">**Koncový bod triggeru http**: adresa URL zkopírována z předchozího kroku</span><span class="sxs-lookup"><span data-stu-id="e6bcf-225">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="e6bcf-226">**Události k registraci**: odkaz-vytvořeno a odkaz-Aktualizováno</span><span class="sxs-lookup"><span data-stu-id="e6bcf-226">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="e6bcf-227">**Přepsat existující koncové body triggeru, pokud je k dispozici**: Ano (přepsání všech stávajících koncových bodů)</span><span class="sxs-lookup"><span data-stu-id="e6bcf-227">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="e6bcf-228">Vyberte **Spustit** a potom vyberte **Hotovo.**</span><span class="sxs-lookup"><span data-stu-id="e6bcf-228">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="e6bcf-229">Webhook teď může naslouchat událostem vytvoření a aktualizace.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-229">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="e6bcf-230">Přizpůsobení kroků synchronizace</span><span class="sxs-lookup"><span data-stu-id="e6bcf-230">Customize synchronization steps</span></span>

<span data-ttu-id="e6bcf-231">Pokud jsou odkazy na spoluprodejní synchronizace mezi partnerským centrem a vaším systémem CRM, tady jsou uvedená pole synchronizovaná v počítači partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-231">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="e6bcf-232">Systémy CRM jsou často vysoce přizpůsobené.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-232">Often CRM systems are highly customized.</span></span> <span data-ttu-id="e6bcf-233">Můžete přizpůsobit automatické toky Power Automate.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-233">You can customize the Power Automate flows.</span></span> <span data-ttu-id="e6bcf-234">Postupujte podle pokynů pro mapování polí a v případě potřeby proveďte příslušné změny v postupech automatizace toků.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-234">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="e6bcf-235">K dispozici jsou mapování partnerských Center Microsoftu na CRM, ale v závislosti na vašem prostředí CRM, můžete zvolit další přizpůsobení polí.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-235">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="e6bcf-236">Několik kroků každého z těchto toků Power Automate přizpůsobit podle vašich potřeb.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-236">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="e6bcf-237">Tady jsou příklady dostupných přizpůsobení:</span><span class="sxs-lookup"><span data-stu-id="e6bcf-237">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="e6bcf-238">Pokud chcete přizpůsobit pole pro události vytvoření nebo aktualizace v Partnerské centrum se synchronizací referenčních seznamů CRM:</span><span class="sxs-lookup"><span data-stu-id="e6bcf-238">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="e6bcf-239">Vyberte Partnerské centrum Salesforce CRM (Insider Preview).</span><span class="sxs-lookup"><span data-stu-id="e6bcf-239">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="e6bcf-240">Pokud **chcete upravit** nebo přizpůsobit tok Power Automate upravit.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-240">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="e6bcf-241">Vyberte **(Rozsah) Synchronizovat zájemce nebo příležitost.**</span><span class="sxs-lookup"><span data-stu-id="e6bcf-241">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="e6bcf-242">Pokud chcete přizpůsobit mapování polí CRM pro události vytváření, vyberte Pokud se jedná **o novou sdílenou příležitost, pak**.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-242">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="e6bcf-243">Pokud ano, vyberte dílčí **krok** a potom rozbalte položku Creating a new opportunity in the CRM (Vytvoření **nové příležitosti v CRM).**</span><span class="sxs-lookup"><span data-stu-id="e6bcf-243">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="e6bcf-244">Mapování v této části můžete upravit pomocí Průvodce mapováním polí.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-244">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="e6bcf-245">Pokud chcete přizpůsobit mapování polí CRM pro události aktualizací, vyberte krok "(Rozsah) Synchronizovat zájemce nebo příležitost".</span><span class="sxs-lookup"><span data-stu-id="e6bcf-245">To customize CRM field mappings for update events, select the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="e6bcf-246">Vyberte **Pokud se jedná o aktualizaci příležitosti, pak**.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-246">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="e6bcf-247">Pokud ano, vyberte dílčí **krok** a potom rozbalte If difference between the opportunity objects in Partnerské centrum and CRM (Pokud je rozdíl mezi objekty příležitostí v Partnerské centrum **a CRM).**</span><span class="sxs-lookup"><span data-stu-id="e6bcf-247">Select the sub-step **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="e6bcf-248">Vyberte **Pokud ano a** pak Aktualizovat existující **příležitost.**</span><span class="sxs-lookup"><span data-stu-id="e6bcf-248">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="e6bcf-249">Přizpůsobení polí synchronizace referenčních seznamů CRM do pc pro události aktualizace:</span><span class="sxs-lookup"><span data-stu-id="e6bcf-249">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="e6bcf-250">Pokud **chcete upravit**  nebo přizpůsobit tok Power Automate upravit.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-250">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="e6bcf-251">Vyberte **(Rozsah) Synchronizovat příležitost.**</span><span class="sxs-lookup"><span data-stu-id="e6bcf-251">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="e6bcf-252">Pokud chcete přizpůsobit mapování polí CRM (na základě průvodce mapováním polí) pro aktualizační události, vyberte Pokud je mezi objekty zájemců v **aplikaci Partnerské centrum a CRM rozdíl, pak .**</span><span class="sxs-lookup"><span data-stu-id="e6bcf-252">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="e6bcf-253">Pokud ano, vyberte dílčí **krok** a potom rozbalte krok Aktualizovat referenční **seznam daty příležitostí**.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-253">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="e6bcf-254">Mapování v této části můžete upravit na základě Průvodce mapováním polí.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-254">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="e6bcf-255">Chcete přizpůsobit pole synchronizace referenčních seznamů CRM do pc pro vytváření událostí?</span><span class="sxs-lookup"><span data-stu-id="e6bcf-255">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="e6bcf-256">Vyberte **Upravit**  a upravte nebo Přizpůsobte tok automatizovaného výkonu.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-256">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="e6bcf-257">Výběr **(rozsah) synchronizace odkazů.**</span><span class="sxs-lookup"><span data-stu-id="e6bcf-257">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="e6bcf-258">Pokud chcete přizpůsobit mapování polí CRM (na základě Průvodce mapováním polí) pro události vytvořit, vyberte **vytvořit odkaz Microsoftu**.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-258">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="e6bcf-259">Mapování v této části můžete upravit v závislosti na průvodci mapováním polí.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-259">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="e6bcf-260">Komplexní Obousměrná synchronizace odkazů v rámci společného prodeje</span><span class="sxs-lookup"><span data-stu-id="e6bcf-260">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="e6bcf-261">Jakmile nainstalujete, nakonfigurujete a přizpůsobili řešení Power Automate, můžete otestovat synchronizaci odkazů pro spoluprodej mezi Salesforce CRM a Partnerským centrem.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-261">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="e6bcf-262">Požadavky</span><span class="sxs-lookup"><span data-stu-id="e6bcf-262">Pre-requisites</span></span>

<span data-ttu-id="e6bcf-263">K synchronizaci odkazů v rámci partnerského centra a Salesforce CRM musí řešení Power automat jasně vymezit pole odkazů specifická pro společnost Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-263">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="e6bcf-264">Tato identifikace poskytuje prodejcům v prodejci možnost rozhodnout se, které odkazy chtějí sdílet se společností Microsoft pro souběžný prodej.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-264">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="e6bcf-265">Sada vlastních polí je k dispozici jako součást synchronizace odkazů partnerského centra pro entitu **příležitosti** řešení Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-265">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="e6bcf-266">Uživatel s oprávněními správce CRM bude muset vytvořit samostatný oddíl CRM s vlastními poli **příležitosti** .</span><span class="sxs-lookup"><span data-stu-id="e6bcf-266">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="e6bcf-267">Následující vlastní pole by měla být součástí části CRM:</span><span class="sxs-lookup"><span data-stu-id="e6bcf-267">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="e6bcf-268">**Synchronizovat s partnerským centrem**: jestli se má synchronizovat příležitost s partnerským centrem Microsoftu</span><span class="sxs-lookup"><span data-stu-id="e6bcf-268">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="e6bcf-269">**Identifikátor odkazu**: pole identifikátoru jen pro čtení pro odkaz na partnerského centra Microsoftu</span><span class="sxs-lookup"><span data-stu-id="e6bcf-269">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="e6bcf-270">**Odkaz** odkazu: odkaz na odkaz určený jen pro čtení v partnerském centru Microsoftu</span><span class="sxs-lookup"><span data-stu-id="e6bcf-270">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="e6bcf-271">**Jak může Microsoft pomáhat**: Podrobnější informace od Microsoftu</span><span class="sxs-lookup"><span data-stu-id="e6bcf-271">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="e6bcf-272">**Produkty**: seznam produktů přidružených k této příležitosti</span><span class="sxs-lookup"><span data-stu-id="e6bcf-272">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="e6bcf-273">**Audit**: záznam auditu jen pro čtení pro synchronizaci s odkazy partnerského centra</span><span class="sxs-lookup"><span data-stu-id="e6bcf-273">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="e6bcf-274">ŘEŠENÍ</span><span class="sxs-lookup"><span data-stu-id="e6bcf-274">SCENARIOS:</span></span>

1. <span data-ttu-id="e6bcf-275">Referenční synchronizace při vytvoření nebo aktualizaci odkazu v CRM a synchronizovaných v partnerském centru:</span><span class="sxs-lookup"><span data-stu-id="e6bcf-275">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="e6bcf-276">Přihlaste se k prostředí Salesforce CRM s uživatelem, který má v části **příležitost** v CRM přehled.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-276">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="e6bcf-277">Při vytváření nové příležitosti v prostředí Salesforce CRM se ujistěte, že se nachází následující část.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-277">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Prostředí Salesforce":::

   3. <span data-ttu-id="e6bcf-279">Pokud chcete tuto příležitost synchronizovat s microsoft Partnerské centrum, ujistěte se, že jste v zobrazení karty nastavili následující pole:</span><span class="sxs-lookup"><span data-stu-id="e6bcf-279">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="e6bcf-280">"Synchronizace s Partnerské centrum": Ano</span><span class="sxs-lookup"><span data-stu-id="e6bcf-280">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="e6bcf-281">"Jak může Microsoft pomoct?": Vyberte jednu z následujících možností:</span><span class="sxs-lookup"><span data-stu-id="e6bcf-281">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="e6bcf-282">Produkty: ID řešení produktu</span><span class="sxs-lookup"><span data-stu-id="e6bcf-282">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="e6bcf-283">Jakmile nastavíte možnost Synchronizovat s  **Partnerské centrum** na **Ano,** počkejte 10 minut, přihlaste se ke svému Partnerské centrum účtu.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-283">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="e6bcf-284">Vaše referenční seznamy se synchronizují s aplikací Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-284">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="e6bcf-285">Pokud je možnost Synchronizovat s Partnerské centrum nastavená na Ano, při aktualizaci příležitosti v Salesforce CRM se změny synchronizují s vaším Partnerské centrum účtem.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-285">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="e6bcf-286">Příležitosti, které se úspěšně synchronizují s Partnerské centrum, se identifikují pomocí ✔icon v Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-286">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="e6bcf-287">Synchronizace referenčních seznamů při vytvoření nebo aktualizaci referenčního Partnerské centrum v prostředí Salesforce CRM:</span><span class="sxs-lookup"><span data-stu-id="e6bcf-287">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="e6bcf-288">Přihlaste se k řídicímu [Partnerské centrum.](https://partner.microsoft.com/dashboard/home)</span><span class="sxs-lookup"><span data-stu-id="e6bcf-288">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="e6bcf-289">V **nabídce vlevo** vyberte Referenční odkazy.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-289">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="e6bcf-290">Kliknutím na možnost New deal (Nová dohoda) Partnerské centrum nový referenční seznam pro spoludácí se ze seznamu.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-290">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="e6bcf-291">Přihlaste se k prostředí Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-291">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="e6bcf-292">Přejděte na **Otevřít příležitosti.**</span><span class="sxs-lookup"><span data-stu-id="e6bcf-292">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="e6bcf-293">Referenční seznam vytvořený v Microsoft Partnerské centrum se teď synchronizuje v Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-293">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Obrazovka prodejních příležitostí Salesforce":::

    6. <span data-ttu-id="e6bcf-295">Když vyberete synchronizovaný referenční seznam, vyplní se podrobnosti o zobrazení karty.</span><span class="sxs-lookup"><span data-stu-id="e6bcf-295">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="e6bcf-296">Další kroky</span><span class="sxs-lookup"><span data-stu-id="e6bcf-296">Next steps</span></span>

- [<span data-ttu-id="e6bcf-297">Správa potenciálních zákazníků</span><span class="sxs-lookup"><span data-stu-id="e6bcf-297">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="e6bcf-298">Správa příležitostí ke spoluprodeji</span><span class="sxs-lookup"><span data-stu-id="e6bcf-298">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="e6bcf-299">Webhooky Partnerského centra</span><span class="sxs-lookup"><span data-stu-id="e6bcf-299">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)
