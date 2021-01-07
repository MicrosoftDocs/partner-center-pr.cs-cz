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
ms.openlocfilehash: 68b8bdf7a88c1ca8d063cf3198fc49bf87552edb
ms.sourcegitcommit: de2ac2eea26426ae8f962d29ab50b68850318ce6
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/07/2021
ms.locfileid: "97960947"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="9c854-104">Konektor pro společný prodej pro Salesforce CRM – přehled</span><span class="sxs-lookup"><span data-stu-id="9c854-104">Co-sell connector for Salesforce CRM - overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="9c854-105">Příslušné role</span><span class="sxs-lookup"><span data-stu-id="9c854-105">Appropriate roles</span></span>

- <span data-ttu-id="9c854-106">Správce odkazů</span><span class="sxs-lookup"><span data-stu-id="9c854-106">Referrals admin</span></span>
- <span data-ttu-id="9c854-107">Správce systému nebo úpravce systému v CRM</span><span class="sxs-lookup"><span data-stu-id="9c854-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="9c854-108">Konektor pro spoluprodej v partnerském centru umožňuje prodejcům v rámci svých systémů CRM spolupracovat s Microsoftem.</span><span class="sxs-lookup"><span data-stu-id="9c854-108">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="9c854-109">Nebudou se muset vyškolet k používání partnerského centra ke správě obchodů v rámci společného prodeje.</span><span class="sxs-lookup"><span data-stu-id="9c854-109">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="9c854-110">Pomocí konektorů pro spoluprodeji můžete vytvořit nový společný prodejní odkaz, který bude kontaktovat prodejce Microsoftu, získat referenční údaje od prodejce Microsoftu, přijmout nebo odmítnout reference, upravit data o koupi, jako je třeba hodnota koupě a datum ukončení.</span><span class="sxs-lookup"><span data-stu-id="9c854-110">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="9c854-111">K těmto obchodům v rámci těchto spoluprodejů můžete také dostávat jakékoli aktualizace od prodejců Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="9c854-111">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="9c854-112">Všechny vaše odkazy fungují při práci v aplikaci CRM dle vašeho výběru a nikoli v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="9c854-112">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="9c854-113">Řešení je založené na řešení Microsoft Power automatizuje a používá rozhraní API partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="9c854-113">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="9c854-114">Před instalací – požadavky</span><span class="sxs-lookup"><span data-stu-id="9c854-114">Before you install - pre-requisites</span></span>

|<span data-ttu-id="9c854-115">**Témata**</span><span class="sxs-lookup"><span data-stu-id="9c854-115">**Topics**</span></span>   |<span data-ttu-id="9c854-116">**Podrobnosti**</span><span class="sxs-lookup"><span data-stu-id="9c854-116">**Details**</span></span>   |<span data-ttu-id="9c854-117">**Odkazy**</span><span class="sxs-lookup"><span data-stu-id="9c854-117">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="9c854-118">ID Microsoft Partner Network</span><span class="sxs-lookup"><span data-stu-id="9c854-118">Microsoft Partner Network ID</span></span> |<span data-ttu-id="9c854-119">Potřebujete platné ID MPN.</span><span class="sxs-lookup"><span data-stu-id="9c854-119">You need a valid MPN ID</span></span>|<span data-ttu-id="9c854-120">Připojení k programu [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="9c854-120">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="9c854-121">Připravený společný prodej</span><span class="sxs-lookup"><span data-stu-id="9c854-121">Co-sell ready</span></span>|<span data-ttu-id="9c854-122">Vaše řešení IP/Services musí být připravené k prodeji.</span><span class="sxs-lookup"><span data-stu-id="9c854-122">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="9c854-123">Prodej pomocí Microsoftu</span><span class="sxs-lookup"><span data-stu-id="9c854-123">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="9c854-124">Účet partnerského centra</span><span class="sxs-lookup"><span data-stu-id="9c854-124">Partner Center account</span></span>|<span data-ttu-id="9c854-125">ID MPN přidružené k tenantovi partnerského centra musí být stejné jako ID MPN přidružené k vašemu řešení společného prodeje.</span><span class="sxs-lookup"><span data-stu-id="9c854-125">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="9c854-126">Před nasazením konektorů se můžete podívat na to, jestli máte na portálu partnerského centra zobrazený odkaz na svůj společný prodej.</span><span class="sxs-lookup"><span data-stu-id="9c854-126">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="9c854-127">Správa vašeho účtu</span><span class="sxs-lookup"><span data-stu-id="9c854-127">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="9c854-128">Role uživatelů partnerského centra</span><span class="sxs-lookup"><span data-stu-id="9c854-128">Partner Center user roles</span></span>|<span data-ttu-id="9c854-129">Zaměstnanec, který bude instalovat a používat konektory, musí být správcem odkazů.</span><span class="sxs-lookup"><span data-stu-id="9c854-129">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="9c854-130">Přiřazování uživatelských rolí a oprávnění</span><span class="sxs-lookup"><span data-stu-id="9c854-130">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="9c854-131">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="9c854-131">Salesforce CRM</span></span>|<span data-ttu-id="9c854-132">Role uživatele CRM je správce systému nebo úpravce systému.</span><span class="sxs-lookup"><span data-stu-id="9c854-132">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="9c854-133">Přiřazení rolí v Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="9c854-133">Assign roles in Salesforce CRM</span></span>](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|<span data-ttu-id="9c854-134">Zapnout účet toku automatizace</span><span class="sxs-lookup"><span data-stu-id="9c854-134">Power Automate Flow Account</span></span>|<span data-ttu-id="9c854-135">Aktivní účet [Power automatizuje](https://flow.microsoft.com) pro správce systému nebo úpravce systému CRM.</span><span class="sxs-lookup"><span data-stu-id="9c854-135">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="9c854-136">Tento uživatel se musí před instalací přihlásit k [automatizaci](https://flow.microsoft.com) aspoň jednou.</span><span class="sxs-lookup"><span data-stu-id="9c854-136">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="9c854-137">Instalace balíčku Salesforce pro vlastní pole Microsoftu</span><span class="sxs-lookup"><span data-stu-id="9c854-137">Installation of Salesforce Package for Microsoft Custom Fields</span></span> 

<span data-ttu-id="9c854-138">Aby bylo možné synchronizovat odkazy v rámci partnerského centra a Salesforce CRM, musí řešení Power automat jasně identifikovat konkrétní pole odkazů specifická pro společnost Microsoft.</span><span class="sxs-lookup"><span data-stu-id="9c854-138">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft specific referral fields.</span></span> <span data-ttu-id="9c854-139">Tato vymezená část poskytuje partnerům partnerských prodejců možnost rozhodnout se, které referenční seznamy chtějí sdílet se společností Microsoft pro souběžný prodej.</span><span class="sxs-lookup"><span data-stu-id="9c854-139">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="9c854-140">V Salesforce aktivujte **poznámky** a přidejte je do seznamu souvisejících příležitostí.</span><span class="sxs-lookup"><span data-stu-id="9c854-140">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> 
[<span data-ttu-id="9c854-141">Odkaz</span><span class="sxs-lookup"><span data-stu-id="9c854-141">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. <span data-ttu-id="9c854-142">**Týmy příležitostí** aktivujte pomocí následujících kroků:</span><span class="sxs-lookup"><span data-stu-id="9c854-142">Activate **Opportunity teams** by following the steps:</span></span> 
    - <span data-ttu-id="9c854-143">V instalačním programu použijte pole **Rychlé hledání** k vyhledání nastavení týmu příležitostí.</span><span class="sxs-lookup"><span data-stu-id="9c854-143">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="9c854-144">Podle potřeby definujte nastavení.</span><span class="sxs-lookup"><span data-stu-id="9c854-144">Define the settings as needed.</span></span>
[<span data-ttu-id="9c854-145">Odkaz</span><span class="sxs-lookup"><span data-stu-id="9c854-145">Reference</span></span>](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. <span data-ttu-id="9c854-146">V Salesforce nainstalujte vlastní pole a objekty pomocí instalačního programu balíčků níže.</span><span class="sxs-lookup"><span data-stu-id="9c854-146">In Salesforce, install custom fields and objects using package installer below.</span></span>
  
<span data-ttu-id="9c854-147">Chcete-li nainstalovat balíček do libovolné společnosti, pokračujte [zde](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV) .</span><span class="sxs-lookup"><span data-stu-id="9c854-147">Go [here](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV) to install the package into any company.</span></span>


<span data-ttu-id="9c854-148">Poznámka: Pokud instalujete do izolovaného prostoru (sandbox), musíte nahradit počáteční část adresy URL. http://test.salesforce.com</span><span class="sxs-lookup"><span data-stu-id="9c854-148">Note: If you are installing into a sandbox you must replace the initial portion of the URL with http://test.salesforce.com</span></span>

4. <span data-ttu-id="9c854-149">V Salesforce přidejte řešení Microsoftu do seznamu souvisejících **příležitostí** .</span><span class="sxs-lookup"><span data-stu-id="9c854-149">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="9c854-150">Po přidání klikněte na ikonu **klíče** a aktualizujte vlastnosti.</span><span class="sxs-lookup"><span data-stu-id="9c854-150">Once added, click on the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="9c854-151">Osvědčené postupy: test před zahájením provozu</span><span class="sxs-lookup"><span data-stu-id="9c854-151">Best Practice: Test before you go live</span></span>

<span data-ttu-id="9c854-152">Než nainstalujete, nakonfigurujete a přizpůsobíte řešení Power Automate v produkčním prostředí, ujistěte se, že řešení otestujete v pracovní instanci CRM.</span><span class="sxs-lookup"><span data-stu-id="9c854-152">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="9c854-153">Nainstalujte řešení Microsoft Power automatizuje do přípravného prostředí/instance CRM.</span><span class="sxs-lookup"><span data-stu-id="9c854-153">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="9c854-154">Vytvořte kopii řešení a spusťte konfiguraci a automatizujte vlastní nastavení toků v přípravném prostředí.</span><span class="sxs-lookup"><span data-stu-id="9c854-154">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="9c854-155">Otestujte řešení na pracovní instanci/CRM.</span><span class="sxs-lookup"><span data-stu-id="9c854-155">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="9c854-156">Po úspěšném dokončení naimportujte jako spravované řešení do produkční instance.</span><span class="sxs-lookup"><span data-stu-id="9c854-156">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="9c854-157">Nainstalovat synchronizaci odkazů partnerského centra pro Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="9c854-157">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="9c854-158">V pravém horním rohu vyberte **prostředí** k [automatizaci](https://flow.microsoft.com) a vyberte prostředí.</span><span class="sxs-lookup"><span data-stu-id="9c854-158">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="9c854-159">Zobrazí se vám dostupné instance CRM.</span><span class="sxs-lookup"><span data-stu-id="9c854-159">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="9c854-160">V rozevíracím seznamu v pravém horním rohu vyberte příslušnou instanci CRM.</span><span class="sxs-lookup"><span data-stu-id="9c854-160">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="9c854-161">Na levém navigačním panelu vyberte **řešení** .</span><span class="sxs-lookup"><span data-stu-id="9c854-161">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="9c854-162">V horní nabídce klikněte na odkaz **otevřít AppSource** .</span><span class="sxs-lookup"><span data-stu-id="9c854-162">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Otevřít AppSource":::

5. <span data-ttu-id="9c854-164">V místní obrazovce vyhledejte **konektory odkazů partnerského centra pro Salesforce** .</span><span class="sxs-lookup"><span data-stu-id="9c854-164">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. <span data-ttu-id="9c854-166">Klikněte na tlačítko **získat nyní** a potom **pokračujte**.</span><span class="sxs-lookup"><span data-stu-id="9c854-166">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="9c854-167">Otevře se stránka, kde můžete vybrat prostředí Salesforce CRM k instalaci aplikace.</span><span class="sxs-lookup"><span data-stu-id="9c854-167">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="9c854-168">Vyjádřit souhlas s podmínkami a ujednáními.</span><span class="sxs-lookup"><span data-stu-id="9c854-168">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="Dostupné CRMS":::

8. <span data-ttu-id="9c854-170">Pak budete přesměrováni na stránku **spravovat vaše řešení** .</span><span class="sxs-lookup"><span data-stu-id="9c854-170">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="9c854-171">Přejděte na "odkazy na partnerské Centrum" pomocí tlačítek se šipkami ve spodní části stránky.</span><span class="sxs-lookup"><span data-stu-id="9c854-171">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="9c854-172">**Naplánovaná instalace** by se měla objevit u řešení s odkazy partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="9c854-172">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="9c854-173">Instalace bude trvat 10-15 minut.</span><span class="sxs-lookup"><span data-stu-id="9c854-173">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="9c854-174">Po dokončení instalace přejděte zpátky na [Power](https://flow.microsoft.com) automat a vyberte **řešení** z navigační oblasti vlevo.</span><span class="sxs-lookup"><span data-stu-id="9c854-174">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="9c854-175">Všimněte si, že v seznamu řešení je k dispozici **synchronizace odkazů partnerského centra pro Salesforce** .</span><span class="sxs-lookup"><span data-stu-id="9c854-175">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="9c854-176">Vyberte **synchronizaci odkazů z partnerského centra pro Salesforce**.</span><span class="sxs-lookup"><span data-stu-id="9c854-176">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="9c854-177">K dispozici jsou tyto toky a entity automatizace pro napájení:</span><span class="sxs-lookup"><span data-stu-id="9c854-177">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Toky Salesforce":::



## <a name="configure-the-solution"></a><span data-ttu-id="9c854-179">Konfigurace řešení</span><span class="sxs-lookup"><span data-stu-id="9c854-179">Configure the solution</span></span>

1. <span data-ttu-id="9c854-180">Po instalaci řešení do instance CRM přejděte zpátky na [Power](https://flow.microsoft.com/)automat.</span><span class="sxs-lookup"><span data-stu-id="9c854-180">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="9c854-181">V rozevíracím seznamu **prostředí** v pravém horním rohu vyberte instanci CRM, do které jste nainstalovali řešení Power automatizuje.</span><span class="sxs-lookup"><span data-stu-id="9c854-181">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>
3. <span data-ttu-id="9c854-182">Budete muset vytvořit připojení, která přiřadí tři uživatelské účty:</span><span class="sxs-lookup"><span data-stu-id="9c854-182">You will need to create connections that associate the three user accounts:</span></span>
    - <span data-ttu-id="9c854-183">Uživatel partnerského centra s přihlašovacími údaji správce odkazů</span><span class="sxs-lookup"><span data-stu-id="9c854-183">Partner Center user with referrals admin credentials</span></span>
    - <span data-ttu-id="9c854-184">Události Partnerského centra</span><span class="sxs-lookup"><span data-stu-id="9c854-184">Partner Center Events</span></span>
    - <span data-ttu-id="9c854-185">Správce CRM s Power Automate automatizuje v řešení.</span><span class="sxs-lookup"><span data-stu-id="9c854-185">CRM admin with the Power Automate flows in the solution.</span></span>
4. <span data-ttu-id="9c854-186">V levém navigačním panelu vyberte **připojení** a v seznamu vyberte řešení partnerského centra pro partnery.</span><span class="sxs-lookup"><span data-stu-id="9c854-186">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

5. <span data-ttu-id="9c854-187">Vytvořte připojení kliknutím na **vytvořit připojení**.</span><span class="sxs-lookup"><span data-stu-id="9c854-187">Create a connection by clicking **Create a connection**.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Vytvoření připojení":::

- <span data-ttu-id="9c854-189">Na panelu hledání v pravém horním rohu vyhledejte odkazy na partnerské Centrum (Preview).</span><span class="sxs-lookup"><span data-stu-id="9c854-189">Search for Partner Center Referrals (preview) in the search bar on the top right corner.</span></span>

- <span data-ttu-id="9c854-190">Vytvořte připojení pro uživatele partnerského centra s rolí přihlašovacích údajů správce odkazů.</span><span class="sxs-lookup"><span data-stu-id="9c854-190">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

-  <span data-ttu-id="9c854-191">Potom vytvořte připojení událostí partnerského centra pro uživatele partnerského centra s přihlašovacími údaji správce odkazů.</span><span class="sxs-lookup"><span data-stu-id="9c854-191">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

- <span data-ttu-id="9c854-192">Vytvořte připojení pro Salesforce pro uživatele správce CRM.</span><span class="sxs-lookup"><span data-stu-id="9c854-192">Create a connection for Salesforce for the CRM administrator user.</span></span>

-  <span data-ttu-id="9c854-193">Po přidání všech připojení byste měli ve svém prostředí zobrazit následující připojení:</span><span class="sxs-lookup"><span data-stu-id="9c854-193">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Sledovat připojení":::

### <a name="edit-the-connections"></a><span data-ttu-id="9c854-195">Upravit připojení</span><span class="sxs-lookup"><span data-stu-id="9c854-195">Edit the connections</span></span>

1. <span data-ttu-id="9c854-196">Vraťte se na stránku řešení a vyberte **výchozí řešení**.</span><span class="sxs-lookup"><span data-stu-id="9c854-196">Return to the Solutions page and select **Default Solution**.</span></span>  <span data-ttu-id="9c854-197">Kliknutím na tlačítko **vše** vyberte **odkaz připojení (Preview)** .</span><span class="sxs-lookup"><span data-stu-id="9c854-197">Select **Connection Reference (preview)** by clicking **All**.</span></span>
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Zahájit úpravu konektoru":::

2. <span data-ttu-id="9c854-199">Každé připojení jednu po jedné upravte výběrem ikony tři tečky.</span><span class="sxs-lookup"><span data-stu-id="9c854-199">Edit each of the Connections one by one by selecting the three dots icon.</span></span> <span data-ttu-id="9c854-200">Přidejte příslušná připojení.</span><span class="sxs-lookup"><span data-stu-id="9c854-200">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Upravit konektory":::

3. <span data-ttu-id="9c854-202">Zapněte toky v následujícím pořadí:</span><span class="sxs-lookup"><span data-stu-id="9c854-202">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="9c854-203">Registrace Webhooku partnerského centra (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="9c854-203">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="9c854-204">Vytvoření společného prodejního odkazu – Salesforce do partnerského centra (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="9c854-204">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="9c854-205">Aktualizace referenčních seznamů Microsoftu v partnerském centru pro spoluprodej na Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="9c854-205">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="9c854-206">Partnerské centrum do Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="9c854-206">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="9c854-207">Salesforce do partnerského centra (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="9c854-207">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="9c854-208">Možnost Salesforce v partnerském centru (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="9c854-208">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="9c854-209">Řešení Salesforce Microsoftu do partnerského centra (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="9c854-209">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="9c854-210">Použití rozhraní Webhook API k registraci pro události změny prostředku</span><span class="sxs-lookup"><span data-stu-id="9c854-210">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="9c854-211">Rozhraní API Webhooku partnerského centra vám umožní registrovat se na události změny prostředků.</span><span class="sxs-lookup"><span data-stu-id="9c854-211">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="9c854-212">Tyto události změny se odesílají na adresu URL jako příspěvky HTTP.</span><span class="sxs-lookup"><span data-stu-id="9c854-212">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="9c854-213">Pokud chcete zaregistrovat adresu URL, vyberte možnost **registrace Webhooku partnerského centra (Insider Preview)** Power automatizace.</span><span class="sxs-lookup"><span data-stu-id="9c854-213">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="9c854-214">Přidat připojení pro uživatele partnerského centra (a.) s událostmi partnerského centra s přihlašovacími údaji správce (b.), jak je zvýrazněno níže</span><span class="sxs-lookup"><span data-stu-id="9c854-214">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Trigger":::

3. <span data-ttu-id="9c854-216">Po provedení těchto aktualizací se zobrazí</span><span class="sxs-lookup"><span data-stu-id="9c854-216">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooky":::

4. <span data-ttu-id="9c854-218">Uložte změny a vyberte **zapnout**.</span><span class="sxs-lookup"><span data-stu-id="9c854-218">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="9c854-219">Pokud chcete, aby Webhooky partnerského centra naslouchali změnám událostí, proveďte následující kroky:</span><span class="sxs-lookup"><span data-stu-id="9c854-219">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="9c854-220">Vyberte **Partnerské centrum pro SALESFORCE CRM (Insider Preview)**.</span><span class="sxs-lookup"><span data-stu-id="9c854-220">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="9c854-221">Vyberte ikonu **Upravit** a vyberte, **kdy se přijme požadavek HTTP**.</span><span class="sxs-lookup"><span data-stu-id="9c854-221">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="9c854-222">Kliknutím na ikonu **kopírování** zkopírujte zadanou adresu URL post protokolu HTTP.</span><span class="sxs-lookup"><span data-stu-id="9c854-222">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Zkopírování adresy URL":::

8. <span data-ttu-id="9c854-224">Nyní vyberte možnost "automatické registrace Webhooku partnerského centra (Insider Preview)" a vyberte **Spustit**.</span><span class="sxs-lookup"><span data-stu-id="9c854-224">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="9c854-225">Ujistěte se, že se v pravém podokně otevře okno spustit tok a klikněte na **pokračovat**.</span><span class="sxs-lookup"><span data-stu-id="9c854-225">Ensure that the "Run Flow" window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="9c854-226">Zadejte následující podrobnosti:</span><span class="sxs-lookup"><span data-stu-id="9c854-226">Enter the following details:</span></span>

    1. <span data-ttu-id="9c854-227">**Koncový bod triggeru http**: adresa URL zkopírována z předchozího kroku</span><span class="sxs-lookup"><span data-stu-id="9c854-227">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="9c854-228">**Události k registraci**: odkaz-vytvořeno a odkaz-Aktualizováno</span><span class="sxs-lookup"><span data-stu-id="9c854-228">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="9c854-229">**Přepsat existující koncové body triggeru, pokud je k dispozici**: Ano (přepsání všech stávajících koncových bodů)</span><span class="sxs-lookup"><span data-stu-id="9c854-229">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="9c854-230">Vyberte **Spustit** a potom vyberte **Hotovo.**</span><span class="sxs-lookup"><span data-stu-id="9c854-230">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="9c854-231">Webhook teď může naslouchat událostem vytvoření a aktualizace.</span><span class="sxs-lookup"><span data-stu-id="9c854-231">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="9c854-232">Přizpůsobení kroků synchronizace</span><span class="sxs-lookup"><span data-stu-id="9c854-232">Customize synchronization steps</span></span>

<span data-ttu-id="9c854-233">Pokud jsou odkazy na spoluprodejní synchronizace mezi partnerským centrem a vaším systémem CRM, tady jsou uvedená pole synchronizovaná v počítači partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="9c854-233">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="9c854-234">Systémy CRM jsou často vysoce přizpůsobené.</span><span class="sxs-lookup"><span data-stu-id="9c854-234">Often CRM systems are highly customized.</span></span> <span data-ttu-id="9c854-235">Můžete přizpůsobit automatické toky Power Automate.</span><span class="sxs-lookup"><span data-stu-id="9c854-235">You can customize the Power Automate flows.</span></span> <span data-ttu-id="9c854-236">Postupujte podle pokynů pro mapování polí a v případě potřeby proveďte příslušné změny v postupech automatizace toků.</span><span class="sxs-lookup"><span data-stu-id="9c854-236">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="9c854-237">K dispozici jsou mapování partnerských Center Microsoftu na CRM, ale v závislosti na vašem prostředí CRM, můžete zvolit další přizpůsobení polí.</span><span class="sxs-lookup"><span data-stu-id="9c854-237">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="9c854-238">V závislosti na vašich potřebách je možné přizpůsobit více kroků každého z těchto toků automatizace napájení.</span><span class="sxs-lookup"><span data-stu-id="9c854-238">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="9c854-239">Následují příklady dostupných přizpůsobení:</span><span class="sxs-lookup"><span data-stu-id="9c854-239">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="9c854-240">Přizpůsobení polí pro události vytvoření nebo aktualizace v partnerském centru pro synchronizaci odkazů CRM:</span><span class="sxs-lookup"><span data-stu-id="9c854-240">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="9c854-241">Vyberte partnerské Centrum pro Salesforce CRM (Insider Preview).</span><span class="sxs-lookup"><span data-stu-id="9c854-241">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="9c854-242">Vyberte **Upravit** a upravte nebo Přizpůsobte tok automatizovaného výkonu.</span><span class="sxs-lookup"><span data-stu-id="9c854-242">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="9c854-243">Vyberte **(rozsah) synchronizujte zájemce nebo příležitost**.</span><span class="sxs-lookup"><span data-stu-id="9c854-243">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="9c854-244">Pokud chcete přizpůsobit mapování polí CRM pro události vytvoření, vyberte, **jestli je nová sdílená příležitost, a pak**.</span><span class="sxs-lookup"><span data-stu-id="9c854-244">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="9c854-245">Vyberte dílčí krok, **Pokud ano** , a pak rozbalte **vytvořit novou příležitost v CRM**.</span><span class="sxs-lookup"><span data-stu-id="9c854-245">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="9c854-246">Mapování v této části můžete upravit pomocí Průvodce mapováním polí.</span><span class="sxs-lookup"><span data-stu-id="9c854-246">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="9c854-247">Pokud chcete přizpůsobit mapování polí CRM pro události aktualizace, klikněte na krok (obor) synchronizovat zájemce nebo příležitost.</span><span class="sxs-lookup"><span data-stu-id="9c854-247">To customize CRM field mappings for update events, click on the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="9c854-248">Vyberte **, jestli se jedná o aktualizaci příležitosti, a pak**.</span><span class="sxs-lookup"><span data-stu-id="9c854-248">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="9c854-249">Vyberte dílčí krok, **Pokud ano** , a pak rozbalte **rozdíl mezi objekty příležitostí v partnerském centru a CRM a pak**.</span><span class="sxs-lookup"><span data-stu-id="9c854-249">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="9c854-250">Vyberte, **jestli ano** , a pak **aktualizovat existující příležitost** .</span><span class="sxs-lookup"><span data-stu-id="9c854-250">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="9c854-251">Přizpůsobení polí pro synchronizaci odkazů CRM na počítač pro události aktualizace:</span><span class="sxs-lookup"><span data-stu-id="9c854-251">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="9c854-252">Vyberte **Upravit**  a upravte nebo Přizpůsobte tok automatizovaného výkonu.</span><span class="sxs-lookup"><span data-stu-id="9c854-252">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="9c854-253">Vyberte **(rozsah) synchronizace příležitosti**.</span><span class="sxs-lookup"><span data-stu-id="9c854-253">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="9c854-254">Chcete-li upravit mapování polí CRM (na základě Průvodce mapováním polí) pro události aktualizace, vyberte, **zda existuje rozdíl mezi objekty potenciálních zákazníků v partnerském centru a CRM, a pak**.</span><span class="sxs-lookup"><span data-stu-id="9c854-254">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="9c854-255">Vyberte dílčí krok, **Pokud ano** , a pak rozbalte krok **aktualizace odkazu s daty příležitostí**.</span><span class="sxs-lookup"><span data-stu-id="9c854-255">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="9c854-256">Mapování v této části můžete upravit v závislosti na průvodci mapováním polí.</span><span class="sxs-lookup"><span data-stu-id="9c854-256">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="9c854-257">Chcete-li přizpůsobit pole pro synchronizaci odkazů CRM na počítač pro vytvoření událostí?</span><span class="sxs-lookup"><span data-stu-id="9c854-257">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="9c854-258">Vyberte **Upravit**  a upravte nebo Přizpůsobte tok automatizovaného výkonu.</span><span class="sxs-lookup"><span data-stu-id="9c854-258">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="9c854-259">Výběr **(rozsah) synchronizace odkazů.**</span><span class="sxs-lookup"><span data-stu-id="9c854-259">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="9c854-260">Pokud chcete přizpůsobit mapování polí CRM (na základě Průvodce mapováním polí) pro události vytvořit, vyberte **vytvořit odkaz Microsoftu**.</span><span class="sxs-lookup"><span data-stu-id="9c854-260">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="9c854-261">Mapování v této části můžete upravit v závislosti na průvodci mapováním polí.</span><span class="sxs-lookup"><span data-stu-id="9c854-261">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="9c854-262">Komplexní Obousměrná synchronizace odkazů v rámci společného prodeje</span><span class="sxs-lookup"><span data-stu-id="9c854-262">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="9c854-263">Jakmile nainstalujete, nakonfigurujete a přizpůsobili řešení Power Automate, můžete otestovat synchronizaci odkazů pro spoluprodej mezi Salesforce CRM a Partnerským centrem.</span><span class="sxs-lookup"><span data-stu-id="9c854-263">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="9c854-264">Požadavky</span><span class="sxs-lookup"><span data-stu-id="9c854-264">Pre-requisites</span></span>

<span data-ttu-id="9c854-265">K synchronizaci odkazů v rámci partnerského centra a Salesforce CRM musí řešení Power automat jasně vymezit pole odkazů specifická pro společnost Microsoft.</span><span class="sxs-lookup"><span data-stu-id="9c854-265">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="9c854-266">Tato identifikace poskytuje prodejcům v prodejci možnost rozhodnout se, které odkazy chtějí sdílet se společností Microsoft pro souběžný prodej.</span><span class="sxs-lookup"><span data-stu-id="9c854-266">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="9c854-267">Sada vlastních polí je k dispozici jako součást synchronizace odkazů partnerského centra pro entitu **příležitosti** řešení Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="9c854-267">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="9c854-268">Uživatel s oprávněními správce CRM bude muset vytvořit samostatný oddíl CRM s vlastními poli **příležitosti** .</span><span class="sxs-lookup"><span data-stu-id="9c854-268">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="9c854-269">Následující vlastní pole by měla být součástí části CRM:</span><span class="sxs-lookup"><span data-stu-id="9c854-269">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="9c854-270">**Synchronizovat s partnerským centrem**: jestli se má synchronizovat příležitost s partnerským centrem Microsoftu</span><span class="sxs-lookup"><span data-stu-id="9c854-270">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="9c854-271">**Identifikátor odkazu**: pole identifikátoru jen pro čtení pro odkaz na partnerského centra Microsoftu</span><span class="sxs-lookup"><span data-stu-id="9c854-271">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="9c854-272">**Odkaz** odkazu: odkaz na odkaz určený jen pro čtení v partnerském centru Microsoftu</span><span class="sxs-lookup"><span data-stu-id="9c854-272">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="9c854-273">**Jak může Microsoft pomáhat**: Podrobnější informace od Microsoftu</span><span class="sxs-lookup"><span data-stu-id="9c854-273">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="9c854-274">**Produkty**: seznam produktů přidružených k této příležitosti</span><span class="sxs-lookup"><span data-stu-id="9c854-274">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="9c854-275">**Audit**: záznam auditu jen pro čtení pro synchronizaci s odkazy partnerského centra</span><span class="sxs-lookup"><span data-stu-id="9c854-275">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="9c854-276">ŘEŠENÍ</span><span class="sxs-lookup"><span data-stu-id="9c854-276">SCENARIOS:</span></span>

1. <span data-ttu-id="9c854-277">Referenční synchronizace při vytvoření nebo aktualizaci odkazu v CRM a synchronizovaných v partnerském centru:</span><span class="sxs-lookup"><span data-stu-id="9c854-277">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="9c854-278">Přihlaste se k prostředí Salesforce CRM s uživatelem, který má v části **příležitost** v CRM přehled.</span><span class="sxs-lookup"><span data-stu-id="9c854-278">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="9c854-279">Při vytváření nové příležitosti v prostředí Salesforce CRM se ujistěte, že je k dispozici následující oddíl.</span><span class="sxs-lookup"><span data-stu-id="9c854-279">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Prostředí Salesforce":::

   3. <span data-ttu-id="9c854-281">Pokud chcete tuto příležitost synchronizovat s partnerským centrem Microsoftu, ujistěte se, že jste v zobrazení karta nastavili následující pole:</span><span class="sxs-lookup"><span data-stu-id="9c854-281">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="9c854-282">Synchronizovat s partnerským centrem: Ano</span><span class="sxs-lookup"><span data-stu-id="9c854-282">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="9c854-283">"Jak může Microsoft pomáhat?": Vyberte si z následujících možností:</span><span class="sxs-lookup"><span data-stu-id="9c854-283">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="9c854-284">Produkty: ID řešení produktu</span><span class="sxs-lookup"><span data-stu-id="9c854-284">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="9c854-285">Jakmile nastavíte možnost Synchronizovat příležitost  **s partnerským centrem** na **Ano**, počkejte 10 minut, přihlaste se k účtu partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="9c854-285">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="9c854-286">Vaše odkazy budou synchronizovány s CRM Salesforce.</span><span class="sxs-lookup"><span data-stu-id="9c854-286">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="9c854-287">Pokud je možnost synchronizovat s partnerským centrem nastavená na hodnotu Ano, změny se synchronizují s vaším účtem partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="9c854-287">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="9c854-288">Příležitosti, které byly úspěšně synchronizovány s partnerským centrem, budou označeny ikonou ✔ v Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="9c854-288">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="9c854-289">Referenční synchronizace při vytvoření nebo aktualizaci odkazu v partnerském centru Microsoftu a synchronizovaných v prostředí Salesforce CRM:</span><span class="sxs-lookup"><span data-stu-id="9c854-289">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="9c854-290">Přihlaste se k [řídicímu panelu](https://partner.microsoft.com/dashboard/home)partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="9c854-290">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="9c854-291">V nabídce na levé straně vyberte **odkazy** .</span><span class="sxs-lookup"><span data-stu-id="9c854-291">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="9c854-292">Klikněte na možnost Nová práce a vytvořte si nový odkaz na společný prodej z partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="9c854-292">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="9c854-293">Přihlaste se do prostředí Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="9c854-293">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="9c854-294">Přejděte na **otevřené příležitosti**.</span><span class="sxs-lookup"><span data-stu-id="9c854-294">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="9c854-295">Odkaz vytvořený v partnerském centru Microsoftu je teď synchronizovaný v Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="9c854-295">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Obrazovka příležitostí pro Salesforce":::

    6. <span data-ttu-id="9c854-297">Když vyberete synchronizovaný odkaz, vyplní se podrobnosti zobrazení karty.</span><span class="sxs-lookup"><span data-stu-id="9c854-297">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="9c854-298">Další kroky</span><span class="sxs-lookup"><span data-stu-id="9c854-298">Next steps</span></span>

- [<span data-ttu-id="9c854-299">Správa potenciálních zákazníků</span><span class="sxs-lookup"><span data-stu-id="9c854-299">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="9c854-300">Správa příležitostí ke spoluprodeji</span><span class="sxs-lookup"><span data-stu-id="9c854-300">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="9c854-301">Webhooky partnerského centra</span><span class="sxs-lookup"><span data-stu-id="9c854-301">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)
