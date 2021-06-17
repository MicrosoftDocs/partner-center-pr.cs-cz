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
ms.openlocfilehash: 74894671966ac0409f6366f33c91ddadfae1ba4c
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276973"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="0daca-104">Konektor pro společný prodej pro Salesforce CRM – přehled</span><span class="sxs-lookup"><span data-stu-id="0daca-104">Co-sell connector for Salesforce CRM - overview</span></span>

<span data-ttu-id="0daca-105">**Příslušné role**: Správce odkazů | Správce systému nebo úpravce systému v CRM</span><span class="sxs-lookup"><span data-stu-id="0daca-105">**Appropriate roles**: Referrals admin | System admin or system customizer on the CRM</span></span>

<span data-ttu-id="0daca-106">Konektor pro spoluprodej v partnerském centru umožňuje prodejcům v rámci svých systémů CRM spolupracovat s Microsoftem.</span><span class="sxs-lookup"><span data-stu-id="0daca-106">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="0daca-107">Nebudou se muset vyškolet k používání partnerského centra ke správě obchodů v rámci společného prodeje.</span><span class="sxs-lookup"><span data-stu-id="0daca-107">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="0daca-108">Pomocí konektorů pro spoluprodeji můžete vytvořit nový společný prodejní odkaz, který bude kontaktovat prodejce Microsoftu, získat referenční údaje od prodejce Microsoftu, přijmout nebo odmítnout reference, upravit data o koupi, jako je třeba hodnota koupě a datum ukončení.</span><span class="sxs-lookup"><span data-stu-id="0daca-108">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="0daca-109">K těmto obchodům v rámci těchto spoluprodejů můžete také dostávat jakékoli aktualizace od prodejců Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="0daca-109">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="0daca-110">Všechny vaše odkazy fungují při práci v aplikaci CRM dle vašeho výběru a nikoli v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="0daca-110">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="0daca-111">Řešení je založené na řešení Microsoft Power automatizuje a používá rozhraní API partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="0daca-111">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="0daca-112">Před instalací – požadavky</span><span class="sxs-lookup"><span data-stu-id="0daca-112">Before you install - pre-requisites</span></span>

|<span data-ttu-id="0daca-113">**Témata**</span><span class="sxs-lookup"><span data-stu-id="0daca-113">**Topics**</span></span>   |<span data-ttu-id="0daca-114">**Podrobnosti**</span><span class="sxs-lookup"><span data-stu-id="0daca-114">**Details**</span></span>   |<span data-ttu-id="0daca-115">**Odkazy**</span><span class="sxs-lookup"><span data-stu-id="0daca-115">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="0daca-116">ID Microsoft Partner Network</span><span class="sxs-lookup"><span data-stu-id="0daca-116">Microsoft Partner Network ID</span></span> |<span data-ttu-id="0daca-117">Potřebujete platné ID MPN.</span><span class="sxs-lookup"><span data-stu-id="0daca-117">You need a valid MPN ID</span></span>|<span data-ttu-id="0daca-118">Připojení k programu [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="0daca-118">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="0daca-119">Připravený společný prodej</span><span class="sxs-lookup"><span data-stu-id="0daca-119">Co-sell ready</span></span>|<span data-ttu-id="0daca-120">Vaše řešení IP/Services musí být připravené k prodeji.</span><span class="sxs-lookup"><span data-stu-id="0daca-120">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="0daca-121">Prodej pomocí Microsoftu</span><span class="sxs-lookup"><span data-stu-id="0daca-121">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="0daca-122">Účet partnerského centra</span><span class="sxs-lookup"><span data-stu-id="0daca-122">Partner Center account</span></span>|<span data-ttu-id="0daca-123">ID MPN přidružené k tenantovi partnerského centra musí být stejné jako ID MPN přidružené k vašemu řešení společného prodeje.</span><span class="sxs-lookup"><span data-stu-id="0daca-123">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="0daca-124">Před nasazením konektorů se můžete podívat na to, jestli máte na portálu partnerského centra zobrazený odkaz na svůj společný prodej.</span><span class="sxs-lookup"><span data-stu-id="0daca-124">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="0daca-125">Správa vašeho účtu</span><span class="sxs-lookup"><span data-stu-id="0daca-125">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="0daca-126">Role uživatelů partnerského centra</span><span class="sxs-lookup"><span data-stu-id="0daca-126">Partner Center user roles</span></span>|<span data-ttu-id="0daca-127">Zaměstnanec, který bude instalovat a používat konektory, musí být správcem odkazů.</span><span class="sxs-lookup"><span data-stu-id="0daca-127">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="0daca-128">Přiřazování uživatelských rolí a oprávnění</span><span class="sxs-lookup"><span data-stu-id="0daca-128">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="0daca-129">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="0daca-129">Salesforce CRM</span></span>|<span data-ttu-id="0daca-130">Role uživatele CRM je správce systému nebo úpravce systému.</span><span class="sxs-lookup"><span data-stu-id="0daca-130">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="0daca-131">Přiřazení rolí v Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="0daca-131">Assign roles in Salesforce CRM</span></span>](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|<span data-ttu-id="0daca-132">Zapnout účet toku automatizace</span><span class="sxs-lookup"><span data-stu-id="0daca-132">Power Automate Flow Account</span></span>|<span data-ttu-id="0daca-133">Aktivní účet [Power automatizuje](https://flow.microsoft.com) pro správce systému nebo úpravce systému CRM.</span><span class="sxs-lookup"><span data-stu-id="0daca-133">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="0daca-134">Tento uživatel se musí před instalací přihlásit k [automatizaci](https://flow.microsoft.com) aspoň jednou.</span><span class="sxs-lookup"><span data-stu-id="0daca-134">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="0daca-135">Instalace balíčku Salesforce pro vlastní pole Microsoftu</span><span class="sxs-lookup"><span data-stu-id="0daca-135">Installation of Salesforce Package for Microsoft Custom Fields</span></span> 

<span data-ttu-id="0daca-136">Aby bylo možné synchronizovat odkazy v rámci partnerského centra a Salesforce CRM, musí řešení Power automat jasně identifikovat pole odkazů specifická pro společnost Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0daca-136">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft-specific referral fields.</span></span> <span data-ttu-id="0daca-137">Tato vymezená část poskytuje partnerům partnerských prodejců možnost rozhodnout se, které referenční seznamy chtějí sdílet se společností Microsoft pro souběžný prodej.</span><span class="sxs-lookup"><span data-stu-id="0daca-137">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="0daca-138">V Salesforce aktivujte **poznámky** a přidejte je do seznamu souvisejících příležitostí.</span><span class="sxs-lookup"><span data-stu-id="0daca-138">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> 
[<span data-ttu-id="0daca-139">Odkaz</span><span class="sxs-lookup"><span data-stu-id="0daca-139">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. <span data-ttu-id="0daca-140">**Týmy příležitostí** aktivujte pomocí následujících kroků:</span><span class="sxs-lookup"><span data-stu-id="0daca-140">Activate **Opportunity teams** by following the steps:</span></span> 
    - <span data-ttu-id="0daca-141">V instalačním programu použijte pole **Rychlé hledání** k vyhledání nastavení týmu příležitostí.</span><span class="sxs-lookup"><span data-stu-id="0daca-141">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="0daca-142">Podle potřeby definujte nastavení.</span><span class="sxs-lookup"><span data-stu-id="0daca-142">Define the settings as needed.</span></span>
[<span data-ttu-id="0daca-143">Odkaz</span><span class="sxs-lookup"><span data-stu-id="0daca-143">Reference</span></span>](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. <span data-ttu-id="0daca-144">V Salesforce nainstalujte vlastní pole a objekty pomocí [instalačního programu balíčku](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV).</span><span class="sxs-lookup"><span data-stu-id="0daca-144">In Salesforce, install custom fields and objects using the [package installer](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV).</span></span> <span data-ttu-id="0daca-145">Tento balíček použijte k instalaci balíčku do libovolné společnosti.</span><span class="sxs-lookup"><span data-stu-id="0daca-145">Use this to install the package into any company.</span></span>

>[!NOTE]
><span data-ttu-id="0daca-146">Pokud instalujete do izolovaného prostoru (sandbox), je nutné nahradit počáteční část adresy URL http://test.salesforce.com</span><span class="sxs-lookup"><span data-stu-id="0daca-146">If you are installing into a sandbox, you must replace the initial portion of the URL with http://test.salesforce.com</span></span>

4. <span data-ttu-id="0daca-147">V Salesforce přidejte řešení Microsoftu do seznamu souvisejících **příležitostí** .</span><span class="sxs-lookup"><span data-stu-id="0daca-147">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="0daca-148">Po přidání vyberte ikonu **klíče** a aktualizujte vlastnosti.</span><span class="sxs-lookup"><span data-stu-id="0daca-148">Once added, select the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="0daca-149">Osvědčené postupy: test před zahájením provozu</span><span class="sxs-lookup"><span data-stu-id="0daca-149">Best Practice: Test before you go live</span></span>

<span data-ttu-id="0daca-150">Než nainstalujete, nakonfigurujete a přizpůsobíte řešení Power Automate v produkčním prostředí, ujistěte se, že řešení otestujete v pracovní instanci CRM.</span><span class="sxs-lookup"><span data-stu-id="0daca-150">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="0daca-151">Nainstalujte řešení Microsoft Power automatizuje do přípravného prostředí/instance CRM.</span><span class="sxs-lookup"><span data-stu-id="0daca-151">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="0daca-152">Vytvořte kopii řešení a spusťte konfiguraci a automatizujte vlastní nastavení toků v přípravném prostředí.</span><span class="sxs-lookup"><span data-stu-id="0daca-152">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="0daca-153">Otestujte řešení na pracovní instanci/CRM.</span><span class="sxs-lookup"><span data-stu-id="0daca-153">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="0daca-154">Po úspěšném dokončení naimportujte jako spravované řešení do produkční instance.</span><span class="sxs-lookup"><span data-stu-id="0daca-154">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="0daca-155">Nainstalovat synchronizaci odkazů partnerského centra pro Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="0daca-155">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="0daca-156">V pravém horním rohu vyberte **prostředí** k [automatizaci](https://flow.microsoft.com) a vyberte prostředí.</span><span class="sxs-lookup"><span data-stu-id="0daca-156">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="0daca-157">Zobrazí se vám dostupné instance CRM.</span><span class="sxs-lookup"><span data-stu-id="0daca-157">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="0daca-158">V rozevíracím seznamu v pravém horním rohu vyberte příslušnou instanci CRM.</span><span class="sxs-lookup"><span data-stu-id="0daca-158">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="0daca-159">Na levém navigačním panelu vyberte **řešení** .</span><span class="sxs-lookup"><span data-stu-id="0daca-159">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="0daca-160">V horní nabídce vyberte odkaz **otevřít AppSource** .</span><span class="sxs-lookup"><span data-stu-id="0daca-160">Select the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Otevřete AppSource.":::

5. <span data-ttu-id="0daca-162">V místní obrazovce vyhledejte **konektory odkazů partnerského centra pro Salesforce** .</span><span class="sxs-lookup"><span data-stu-id="0daca-162">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Produktu.":::

6. <span data-ttu-id="0daca-164">Vyberte tlačítko **získat nyní** a potom **pokračujte**.</span><span class="sxs-lookup"><span data-stu-id="0daca-164">Select the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="0daca-165">Otevře se stránka, kde můžete vybrat prostředí Salesforce CRM k instalaci aplikace.</span><span class="sxs-lookup"><span data-stu-id="0daca-165">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="0daca-166">Vyjádřit souhlas s podmínkami a ujednáními.</span><span class="sxs-lookup"><span data-stu-id="0daca-166">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="Dostupné CRMS.":::

8. <span data-ttu-id="0daca-168">Pak budete přesměrováni na stránku **spravovat vaše řešení** .</span><span class="sxs-lookup"><span data-stu-id="0daca-168">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="0daca-169">Přejděte na "odkazy na partnerské Centrum" pomocí tlačítek se šipkami ve spodní části stránky.</span><span class="sxs-lookup"><span data-stu-id="0daca-169">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="0daca-170">**Naplánovaná instalace** by se měla objevit u řešení s odkazy partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="0daca-170">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="0daca-171">Instalace bude trvat 10-15 minut.</span><span class="sxs-lookup"><span data-stu-id="0daca-171">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="0daca-172">Po dokončení instalace přejděte zpátky na [Power](https://flow.microsoft.com) automat a vyberte **řešení** z navigační oblasti vlevo.</span><span class="sxs-lookup"><span data-stu-id="0daca-172">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="0daca-173">Všimněte si, že v seznamu řešení je k dispozici **synchronizace odkazů partnerského centra pro Salesforce** .</span><span class="sxs-lookup"><span data-stu-id="0daca-173">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="0daca-174">Vyberte **synchronizaci odkazů z partnerského centra pro Salesforce**.</span><span class="sxs-lookup"><span data-stu-id="0daca-174">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="0daca-175">K dispozici jsou tyto toky a entity automatizace pro napájení:</span><span class="sxs-lookup"><span data-stu-id="0daca-175">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Toky Salesforce.":::



## <a name="configure-the-solution"></a><span data-ttu-id="0daca-177">Konfigurace řešení</span><span class="sxs-lookup"><span data-stu-id="0daca-177">Configure the solution</span></span>

1. <span data-ttu-id="0daca-178">Po instalaci řešení do instance CRM přejděte zpátky na [Power](https://flow.microsoft.com/)automat.</span><span class="sxs-lookup"><span data-stu-id="0daca-178">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="0daca-179">V rozevíracím seznamu **prostředí** v pravém horním rohu vyberte instanci CRM, do které jste nainstalovali řešení Power automatizuje.</span><span class="sxs-lookup"><span data-stu-id="0daca-179">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>
3. <span data-ttu-id="0daca-180">Budete muset vytvořit připojení, která přiřadí tři uživatelské účty:</span><span class="sxs-lookup"><span data-stu-id="0daca-180">You will need to create connections that associate the three user accounts:</span></span>
    - <span data-ttu-id="0daca-181">Uživatel partnerského centra s přihlašovacími údaji správce odkazů</span><span class="sxs-lookup"><span data-stu-id="0daca-181">Partner Center user with referrals admin credentials</span></span>
    - <span data-ttu-id="0daca-182">Události Partnerského centra</span><span class="sxs-lookup"><span data-stu-id="0daca-182">Partner Center Events</span></span>
    - <span data-ttu-id="0daca-183">Správce CRM s Power Automate automatizuje v řešení.</span><span class="sxs-lookup"><span data-stu-id="0daca-183">CRM admin with the Power Automate flows in the solution.</span></span>
4. <span data-ttu-id="0daca-184">V levém navigačním panelu vyberte **připojení** a v seznamu vyberte řešení partnerského centra pro partnery.</span><span class="sxs-lookup"><span data-stu-id="0daca-184">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

5. <span data-ttu-id="0daca-185">Vytvořte připojení kliknutím na **vytvořit připojení**.</span><span class="sxs-lookup"><span data-stu-id="0daca-185">Create a connection by clicking **Create a connection**.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Vytvořte připojení.":::

- <span data-ttu-id="0daca-187">Na panelu hledání v pravém horním rohu vyhledejte odkazy na partnerské Centrum (Preview).</span><span class="sxs-lookup"><span data-stu-id="0daca-187">Search for Partner Center Referrals (preview) in the search bar on the top-right corner.</span></span>

- <span data-ttu-id="0daca-188">Vytvořte připojení pro uživatele partnerského centra s rolí přihlašovacích údajů správce odkazů.</span><span class="sxs-lookup"><span data-stu-id="0daca-188">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

-  <span data-ttu-id="0daca-189">Potom vytvořte připojení událostí partnerského centra pro uživatele partnerského centra s přihlašovacími údaji správce odkazů.</span><span class="sxs-lookup"><span data-stu-id="0daca-189">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

- <span data-ttu-id="0daca-190">Vytvořte připojení pro Salesforce pro uživatele správce CRM.</span><span class="sxs-lookup"><span data-stu-id="0daca-190">Create a connection for Salesforce for the CRM administrator user.</span></span>

-  <span data-ttu-id="0daca-191">Po přidání všech připojení byste měli ve svém prostředí zobrazit následující připojení:</span><span class="sxs-lookup"><span data-stu-id="0daca-191">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Sledujte připojení.":::

### <a name="edit-the-connections"></a><span data-ttu-id="0daca-193">Upravit připojení</span><span class="sxs-lookup"><span data-stu-id="0daca-193">Edit the connections</span></span>

1. <span data-ttu-id="0daca-194">Vraťte se na stránku řešení a vyberte **výchozí řešení**.</span><span class="sxs-lookup"><span data-stu-id="0daca-194">Return to the Solutions page and select **Default Solution**.</span></span>  <span data-ttu-id="0daca-195">Kliknutím na tlačítko **vše** vyberte **odkaz připojení (Preview)** .</span><span class="sxs-lookup"><span data-stu-id="0daca-195">Select **Connection Reference (preview)** by clicking **All**.</span></span>
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Zahájit úpravu konektoru":::

2. <span data-ttu-id="0daca-197">Jednotlivá připojení upravte jednotlivě výběrem ikony tři tečky.</span><span class="sxs-lookup"><span data-stu-id="0daca-197">Edit each of the Connections individually by selecting the three dots icon.</span></span> <span data-ttu-id="0daca-198">Přidejte příslušná připojení.</span><span class="sxs-lookup"><span data-stu-id="0daca-198">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Upravit konektory.":::

3. <span data-ttu-id="0daca-200">Zapněte toky v následujícím pořadí:</span><span class="sxs-lookup"><span data-stu-id="0daca-200">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="0daca-201">Partnerské centrum registrace webhooku (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="0daca-201">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="0daca-202">Vytvoření referenčního odkazu pro spoluprodej – Salesforce pro Partnerské centrum (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="0daca-202">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="0daca-203">Partnerské centrum referenčních doporučení spoluprodeje Microsoftu pro Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="0daca-203">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="0daca-204">Partnerské centrum salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="0daca-204">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="0daca-205">Salesforce na Partnerské centrum (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="0daca-205">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="0daca-206">Salesforce Opportunity to Partnerské centrum (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="0daca-206">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="0daca-207">Salesforce – řešení Microsoftu pro Partnerské centrum (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="0daca-207">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="0daca-208">Použití rozhraní WEBHOOK API k registraci událostí změny prostředků</span><span class="sxs-lookup"><span data-stu-id="0daca-208">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="0daca-209">Rozhraní PARTNERSKÉ CENTRUM API webhooku umožňují registrovat události změny prostředků.</span><span class="sxs-lookup"><span data-stu-id="0daca-209">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="0daca-210">Tyto události změny se posílají na vaši adresu URL jako příspěvky HTTP.</span><span class="sxs-lookup"><span data-stu-id="0daca-210">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="0daca-211">Pokud chcete zaregistrovat adresu URL, **Partnerské centrum toku vyberte Registrace webhooku (Insider** Power Automate Preview).</span><span class="sxs-lookup"><span data-stu-id="0daca-211">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="0daca-212">Přidejte připojení pro uživatele (a.) s přihlašovacími údaji správce referenčních Partnerské centrum (b.) a Partnerské centrum událostmi, jak je zvýrazněno níže.</span><span class="sxs-lookup"><span data-stu-id="0daca-212">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Aktivační událost.":::

3. <span data-ttu-id="0daca-214">Při těchto aktualizacích se zobrazí</span><span class="sxs-lookup"><span data-stu-id="0daca-214">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooky.":::

4. <span data-ttu-id="0daca-216">Uložte změny a vyberte **Zapnout**.</span><span class="sxs-lookup"><span data-stu-id="0daca-216">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="0daca-217">Pokud chcete Partnerské centrum, aby webhooky naslouchaly změnám událostí, proveďte následující kroky:</span><span class="sxs-lookup"><span data-stu-id="0daca-217">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="0daca-218">Vyberte **Partnerské centrum Salesforce CRM (Insider Preview).**</span><span class="sxs-lookup"><span data-stu-id="0daca-218">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="0daca-219">Vyberte **ikonu** Upravit a vyberte **Při přijetí požadavku HTTP.**</span><span class="sxs-lookup"><span data-stu-id="0daca-219">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="0daca-220">Vyberte **ikonu Kopírovat** a zkopírujte zadanou adresu URL HTTP POST.</span><span class="sxs-lookup"><span data-stu-id="0daca-220">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Zkopírujte adresu URL.":::

8. <span data-ttu-id="0daca-222">Teď vyberte tok Partnerské centrum webhooku (Insider Preview) a Power Automate **Spustit.**</span><span class="sxs-lookup"><span data-stu-id="0daca-222">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="0daca-223">Ujistěte se, že se v pravém podokně otevře okno Spustit tok, a vyberte **Pokračovat.**</span><span class="sxs-lookup"><span data-stu-id="0daca-223">Ensure that the "Run Flow" window opens on the right-hand pane and select **Continue**.</span></span>

10. <span data-ttu-id="0daca-224">Zadejte následující podrobnosti:</span><span class="sxs-lookup"><span data-stu-id="0daca-224">Enter the following details:</span></span>

    1. <span data-ttu-id="0daca-225">**Koncový bod triggeru HTTP:** Adresa URL zkopírovaná z předchozího kroku</span><span class="sxs-lookup"><span data-stu-id="0daca-225">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="0daca-226">**Události k registraci:**"referenční seznam byl vytvořen" a "aktualizován referenční seznam".</span><span class="sxs-lookup"><span data-stu-id="0daca-226">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="0daca-227">**Přepsat existující koncové body triggeru, pokud jsou k dispozici:** Ano (Tím se přepíšou všechny existující koncové body.)</span><span class="sxs-lookup"><span data-stu-id="0daca-227">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="0daca-228">Vyberte **Spustit a** pak vyberte **Hotovo.**</span><span class="sxs-lookup"><span data-stu-id="0daca-228">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="0daca-229">Webhook teď může naslouchat událostem vytváření a aktualizace.</span><span class="sxs-lookup"><span data-stu-id="0daca-229">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="0daca-230">Přizpůsobení kroků synchronizace</span><span class="sxs-lookup"><span data-stu-id="0daca-230">Customize synchronization steps</span></span>

<span data-ttu-id="0daca-231">Když se referenční seznam pro spoluprodácí synchronizuje mezi systémem Partnerské centrum a systémem CRM, zobrazí se tady pole synchronizovaná v Partnerské centrum počítači.</span><span class="sxs-lookup"><span data-stu-id="0daca-231">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="0daca-232">Systémy CRM jsou často vysoce přizpůsobené.</span><span class="sxs-lookup"><span data-stu-id="0daca-232">Often CRM systems are highly customized.</span></span> <span data-ttu-id="0daca-233">Můžete přizpůsobit Power Automate toky.</span><span class="sxs-lookup"><span data-stu-id="0daca-233">You can customize the Power Automate flows.</span></span> <span data-ttu-id="0daca-234">Postupujte podle průvodce mapováním polí a v případě potřeby proveďte odpovídající změny v krocích Power Automate toků.</span><span class="sxs-lookup"><span data-stu-id="0daca-234">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="0daca-235">K dispozici jsou partnerská centra Microsoftu pro mapování CRM, ale na základě prostředí CRM se můžete rozhodnout pole dále přizpůsobit.</span><span class="sxs-lookup"><span data-stu-id="0daca-235">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="0daca-236">Několik kroků každého z těchto toků Power Automate přizpůsobit podle vašich potřeb.</span><span class="sxs-lookup"><span data-stu-id="0daca-236">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="0daca-237">Tady jsou příklady dostupných přizpůsobení:</span><span class="sxs-lookup"><span data-stu-id="0daca-237">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="0daca-238">Pokud chcete přizpůsobit pole pro události vytvoření nebo aktualizace v Partnerské centrum se synchronizací referenčních seznamu CRM:</span><span class="sxs-lookup"><span data-stu-id="0daca-238">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="0daca-239">Vyberte Partnerské centrum Salesforce CRM (Insider Preview).</span><span class="sxs-lookup"><span data-stu-id="0daca-239">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="0daca-240">Pokud **chcete upravit** nebo přizpůsobit tok Power Automate upravit.</span><span class="sxs-lookup"><span data-stu-id="0daca-240">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="0daca-241">Vyberte **(Rozsah) Synchronizovat zájemce nebo příležitost.**</span><span class="sxs-lookup"><span data-stu-id="0daca-241">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="0daca-242">Pokud chcete přizpůsobit mapování polí CRM pro události vytváření, vyberte Pokud se jedná **o novou sdílenou příležitost, pak**.</span><span class="sxs-lookup"><span data-stu-id="0daca-242">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="0daca-243">Pokud ano, vyberte dílčí **krok** a potom rozbalte položku Creating a new opportunity in the CRM (Vytvoření **nové příležitosti v CRM).**</span><span class="sxs-lookup"><span data-stu-id="0daca-243">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="0daca-244">Mapování v této části můžete upravit pomocí Průvodce mapováním polí.</span><span class="sxs-lookup"><span data-stu-id="0daca-244">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="0daca-245">Pokud chcete přizpůsobit mapování polí CRM pro události aktualizací, vyberte krok "(Rozsah) Synchronizovat zájemce nebo příležitost".</span><span class="sxs-lookup"><span data-stu-id="0daca-245">To customize CRM field mappings for update events, select the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="0daca-246">Vyberte **Pokud se jedná o aktualizaci příležitosti, pak**.</span><span class="sxs-lookup"><span data-stu-id="0daca-246">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="0daca-247">Pokud ano, vyberte dílčí **krok** a pak rozbalte If difference between the opportunity objects in Partnerské centrum and CRM (Pokud je rozdíl mezi objekty příležitostí v Partnerské centrum **a CRM).**</span><span class="sxs-lookup"><span data-stu-id="0daca-247">Select the sub-step **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="0daca-248">Vyberte **Pokud ano a** pak Aktualizovat existující **příležitost.**</span><span class="sxs-lookup"><span data-stu-id="0daca-248">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="0daca-249">Přizpůsobení polí synchronizace referenčních seznamů CRM do pc pro události aktualizace:</span><span class="sxs-lookup"><span data-stu-id="0daca-249">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="0daca-250">Pokud **chcete upravit**  nebo přizpůsobit tok Power Automate upravit.</span><span class="sxs-lookup"><span data-stu-id="0daca-250">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="0daca-251">Vyberte **(Rozsah) Synchronizovat příležitost.**</span><span class="sxs-lookup"><span data-stu-id="0daca-251">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="0daca-252">Pokud chcete přizpůsobit mapování polí CRM (na základě průvodce mapováním polí) pro aktualizační události, vyberte Pokud je mezi objekty zájemců v aplikaci Partnerské centrum a **CRM rozdíl, pak vyberte**.</span><span class="sxs-lookup"><span data-stu-id="0daca-252">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="0daca-253">Pokud ano, vyberte dílčí **krok** a potom rozbalte krok Aktualizovat referenční **seznam daty příležitostí**.</span><span class="sxs-lookup"><span data-stu-id="0daca-253">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="0daca-254">Mapování v této části můžete upravit na základě Průvodce mapováním polí.</span><span class="sxs-lookup"><span data-stu-id="0daca-254">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="0daca-255">Chcete přizpůsobit pole synchronizace referenčních seznamů CRM do pc pro vytváření událostí?</span><span class="sxs-lookup"><span data-stu-id="0daca-255">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="0daca-256">Pokud **chcete upravit**  nebo přizpůsobit tok Power Automate upravit.</span><span class="sxs-lookup"><span data-stu-id="0daca-256">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="0daca-257">Vyberte **(Rozsah) Synchronizace referenčních seznamu.**</span><span class="sxs-lookup"><span data-stu-id="0daca-257">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="0daca-258">Pokud chcete přizpůsobit mapování polí CRM (na základě průvodce mapováním polí) pro vytváření událostí, vyberte Create Microsoft Referral (Vytvořit **referenční seznam Microsoftu).**</span><span class="sxs-lookup"><span data-stu-id="0daca-258">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="0daca-259">Mapování v této části můžete upravit na základě Průvodce mapováním polí.</span><span class="sxs-lookup"><span data-stu-id="0daca-259">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="0daca-260">Synchronizace referenčních odkazů end-to-end bi-directional co-sell</span><span class="sxs-lookup"><span data-stu-id="0daca-260">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="0daca-261">Po instalaci, konfiguraci a přizpůsobení řešení Power Automate můžete otestovat synchronizaci referenčních odkazů spoluprodeje mezi salesforce CRM a Partnerské centrum.</span><span class="sxs-lookup"><span data-stu-id="0daca-261">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="0daca-262">Požadavky</span><span class="sxs-lookup"><span data-stu-id="0daca-262">Pre-requisites</span></span>

<span data-ttu-id="0daca-263">Pokud chcete synchronizovat referenční Partnerské centrum napříč aplikacemi a salesforce CRM, Power Automate řešení musí jasně vytyčovat pole referenčních seznamů specifická pro Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0daca-263">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="0daca-264">Tato identifikace poskytuje týmům prodejců možnost rozhodnout se, které referenční odkazy chce sdílet s Microsoftem pro spoluprodávač.</span><span class="sxs-lookup"><span data-stu-id="0daca-264">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="0daca-265">Sada vlastních polí je k dispozici jako součást synchronizace referenčních  Partnerské centrum referenčních seznamů pro entitu Opportunity řešení Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="0daca-265">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="0daca-266">Uživatel s rolí správce CRM bude muset vytvořit samostatný oddíl CRM s vlastními **poli Opportunity.**</span><span class="sxs-lookup"><span data-stu-id="0daca-266">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="0daca-267">Následující vlastní pole by měla být součástí oddílu CRM:</span><span class="sxs-lookup"><span data-stu-id="0daca-267">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="0daca-268">**Synchronizace s Partnerské centrum:** Jestli se má synchronizovat příležitost s Microsoft Partnerské centrum</span><span class="sxs-lookup"><span data-stu-id="0daca-268">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="0daca-269">**Identifikátor referenčního** seznamu: Pole identifikátoru jen pro čtení pro referenční Partnerské centrum referenčního seznamu</span><span class="sxs-lookup"><span data-stu-id="0daca-269">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="0daca-270">**Odkaz na referenční** seznam: Odkaz jen pro čtení referenčního seznamu v Microsoft Partnerské centrum</span><span class="sxs-lookup"><span data-stu-id="0daca-270">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="0daca-271">**Jak může Microsoft pomoci:** Pomoc od Microsoftu požadovaná pro referenční informace</span><span class="sxs-lookup"><span data-stu-id="0daca-271">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="0daca-272">**Produkty:** Seznam produktů přidružených k této příležitosti</span><span class="sxs-lookup"><span data-stu-id="0daca-272">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="0daca-273">**Audit:** Záznam pro audit jen pro čtení pro synchronizaci s referenčními Partnerské centrum referenčními odkazy</span><span class="sxs-lookup"><span data-stu-id="0daca-273">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="0daca-274">Scénáře:</span><span class="sxs-lookup"><span data-stu-id="0daca-274">SCENARIOS:</span></span>

1. <span data-ttu-id="0daca-275">Synchronizace referenčních odkazů při vytvoření nebo aktualizaci referenčních seznamů v CRM a synchronizaci v Partnerské centrum:</span><span class="sxs-lookup"><span data-stu-id="0daca-275">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="0daca-276">Přihlaste se k prostředí Salesforce CRM s uživatelem, který má přehled v **části Opportunity** v CRM.</span><span class="sxs-lookup"><span data-stu-id="0daca-276">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="0daca-277">Při vytváření nové příležitosti v prostředí Salesforce CRM se ujistěte, že se nachází následující část.</span><span class="sxs-lookup"><span data-stu-id="0daca-277">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Prostředí Salesforce.":::

   3. <span data-ttu-id="0daca-279">Pokud chcete tuto příležitost synchronizovat s microsoft Partnerské centrum, ujistěte se, že jste v zobrazení karty nastavili následující pole:</span><span class="sxs-lookup"><span data-stu-id="0daca-279">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="0daca-280">"Synchronizace s Partnerské centrum": Ano</span><span class="sxs-lookup"><span data-stu-id="0daca-280">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="0daca-281">"Jak může Microsoft pomoct?": Vyberte jednu z následujících možností:</span><span class="sxs-lookup"><span data-stu-id="0daca-281">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="0daca-282">Produkty: ID řešení produktu</span><span class="sxs-lookup"><span data-stu-id="0daca-282">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="0daca-283">Po nastavení možnosti Synchronizovat s  **Partnerské centrum** na **Ano,** počkejte 10 minut, přihlaste se ke svému Partnerské centrum účtu.</span><span class="sxs-lookup"><span data-stu-id="0daca-283">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="0daca-284">Vaše referenční seznamy se synchronizují s aplikací Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="0daca-284">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="0daca-285">Když je možnost Synchronizovat s Partnerské centrum nastavená na Ano, při aktualizaci příležitosti v Salesforce CRM se změny synchronizují s vaším Partnerské centrum účtem.</span><span class="sxs-lookup"><span data-stu-id="0daca-285">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="0daca-286">Příležitosti, které se úspěšně synchronizují s Partnerské centrum, se identifikují pomocí ✔icon v Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="0daca-286">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="0daca-287">Synchronizace referenčních seznamů při vytvoření nebo aktualizaci referenčního Partnerské centrum v prostředí Salesforce CRM:</span><span class="sxs-lookup"><span data-stu-id="0daca-287">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="0daca-288">Přihlaste se k řídicímu [Partnerské centrum.](https://partner.microsoft.com/dashboard/home)</span><span class="sxs-lookup"><span data-stu-id="0daca-288">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="0daca-289">V **nabídce vlevo** vyberte Referenční odkazy.</span><span class="sxs-lookup"><span data-stu-id="0daca-289">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="0daca-290">Kliknutím na možnost New deal (Nová dohoda) Partnerské centrum nový referenční seznam pro spoludácí se na Partnerské centrum.</span><span class="sxs-lookup"><span data-stu-id="0daca-290">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="0daca-291">Přihlaste se k prostředí Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="0daca-291">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="0daca-292">Přejděte na **Otevřít příležitosti.**</span><span class="sxs-lookup"><span data-stu-id="0daca-292">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="0daca-293">Referenční seznam vytvořený v Microsoft Partnerské centrum se teď synchronizuje v Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="0daca-293">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Obrazovka prodejních příležitostí Salesforce":::

    6. <span data-ttu-id="0daca-295">Když vyberete synchronizovaný referenční seznam, vyplní se podrobnosti o zobrazení karty.</span><span class="sxs-lookup"><span data-stu-id="0daca-295">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="0daca-296">Další kroky</span><span class="sxs-lookup"><span data-stu-id="0daca-296">Next steps</span></span>

- [<span data-ttu-id="0daca-297">Správa potenciálních zákazníků</span><span class="sxs-lookup"><span data-stu-id="0daca-297">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="0daca-298">Správa příležitostí ke spoluprodeji</span><span class="sxs-lookup"><span data-stu-id="0daca-298">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="0daca-299">Webhooky Partnerského centra</span><span class="sxs-lookup"><span data-stu-id="0daca-299">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)
