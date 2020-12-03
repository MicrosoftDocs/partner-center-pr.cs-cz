---
title: Konektor pro spoluprodeji pro partnerské Centrum Dynamics 365 CRM
ms.topic: how-to
ms.date: 05/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Synchronizujte odkazy v partnerském centru s konektorem pro spoluprodeji pro Dynamics 365 CRM. Prodejci pak můžou v rámci svých systémů CRM prodávat společně s Microsoftem.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 18a54bf777cb987e8f486f85afcf277e04c1055c
ms.sourcegitcommit: 147813ba322653c989df5afe0b3bf0c252523a92
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/03/2020
ms.locfileid: "96556357"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a><span data-ttu-id="39079-104">Konektor pro společný prodej pro Dynamics 365 CRM – přehled</span><span class="sxs-lookup"><span data-stu-id="39079-104">Co-sell connector for Dynamics 365 CRM – Overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="39079-105">Příslušné role</span><span class="sxs-lookup"><span data-stu-id="39079-105">Appropriate roles</span></span>

- <span data-ttu-id="39079-106">Správce odkazů</span><span class="sxs-lookup"><span data-stu-id="39079-106">Referrals admin</span></span>
- <span data-ttu-id="39079-107">Správce systému nebo úpravce systému v CRM</span><span class="sxs-lookup"><span data-stu-id="39079-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="39079-108">Konektor pro spoluprodej v partnerském centru umožňuje prodejcům v rámci svých systémů CRM spolupracovat s Microsoftem.</span><span class="sxs-lookup"><span data-stu-id="39079-108">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="39079-109">Nebudou se muset vyškolet k používání partnerského centra ke správě obchodů v rámci společného prodeje.</span><span class="sxs-lookup"><span data-stu-id="39079-109">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="39079-110">Pomocí konektorů pro spoluprodeji můžete vytvořit nový společný odkaz pro prodej prodávajícího, získat referenční údaje od prodejce Microsoftu, přijmout nebo odmítnout odkazy, upravit data o koupi, jako je například hodnota kouposti a datum ukončení.</span><span class="sxs-lookup"><span data-stu-id="39079-110">Use the Co-sell connectors, to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span> <span data-ttu-id="39079-111">K těmto obchodům v rámci těchto spoluprodejů můžete také dostávat jakékoli aktualizace od prodejců Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="39079-111">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="39079-112">Všechny vaše odkazy můžete v aplikaci CRM použít místo v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="39079-112">You can do all of your referrals work within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="39079-113">Řešení je založené na řešení Microsoft Power automatizuje a používá rozhraní API partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="39079-113">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="39079-114">Před instalací – požadavky</span><span class="sxs-lookup"><span data-stu-id="39079-114">Before you install - pre-requisites</span></span>

|<span data-ttu-id="39079-115">**Témata**</span><span class="sxs-lookup"><span data-stu-id="39079-115">**Topics**</span></span>   |<span data-ttu-id="39079-116">**Podrobnosti**</span><span class="sxs-lookup"><span data-stu-id="39079-116">**Details**</span></span>   |<span data-ttu-id="39079-117">**Odkazy**</span><span class="sxs-lookup"><span data-stu-id="39079-117">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="39079-118">ID Microsoft Partner Network</span><span class="sxs-lookup"><span data-stu-id="39079-118">Microsoft Partner Network ID</span></span> |<span data-ttu-id="39079-119">Potřebujete platné ID MPN.</span><span class="sxs-lookup"><span data-stu-id="39079-119">You need a valid MPN ID</span></span>|<span data-ttu-id="39079-120">Připojení k programu [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="39079-120">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="39079-121">Předprodejní připraveno</span><span class="sxs-lookup"><span data-stu-id="39079-121">Cosell ready</span></span>|<span data-ttu-id="39079-122">Vaše řešení IP/Services musí být připravené k prodeji.</span><span class="sxs-lookup"><span data-stu-id="39079-122">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="39079-123">Prodej pomocí Microsoftu</span><span class="sxs-lookup"><span data-stu-id="39079-123">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="39079-124">Účet partnerského centra</span><span class="sxs-lookup"><span data-stu-id="39079-124">Partner Center account</span></span>|<span data-ttu-id="39079-125">ID MPN přidružené k tenantovi partnerského centra musí být stejné jako ID MPN přidružené k vašemu řešení společného prodeje.</span><span class="sxs-lookup"><span data-stu-id="39079-125">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="39079-126">Před nasazením konektorů se můžete podívat na to, jestli máte na portálu partnerského centra zobrazený odkaz na svůj společný prodej.</span><span class="sxs-lookup"><span data-stu-id="39079-126">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="39079-127">Správa vašeho účtu</span><span class="sxs-lookup"><span data-stu-id="39079-127">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="39079-128">Role uživatelů partnerského centra</span><span class="sxs-lookup"><span data-stu-id="39079-128">Partner Center user roles</span></span>|<span data-ttu-id="39079-129">Zaměstnanec, který bude instalovat a používat konektory, musí být správcem odkazů.</span><span class="sxs-lookup"><span data-stu-id="39079-129">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="39079-130">Přiřazování uživatelských rolí a oprávnění</span><span class="sxs-lookup"><span data-stu-id="39079-130">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)| |<span data-ttu-id="39079-131">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="39079-131">Dynamics 365 CRM</span></span>|<span data-ttu-id="39079-132">Role uživatele CRM je správce systému nebo úpravce systému.</span><span class="sxs-lookup"><span data-stu-id="39079-132">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="39079-133">Přiřazení rolí v Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="39079-133">Assign roles in Dynamics 365</span></span>](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="39079-134">Zapnout účet toku automatizace</span><span class="sxs-lookup"><span data-stu-id="39079-134">Power Automate Flow Account</span></span>|<span data-ttu-id="39079-135">Aktivní účet [Power automatizuje](https://flow.microsoft.com) pro správce systému nebo úpravce systému CRM.</span><span class="sxs-lookup"><span data-stu-id="39079-135">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="39079-136">Tento uživatel se musí před instalací přihlásit k [automatizaci](https://flow.microsoft.com) aspoň jednou.</span><span class="sxs-lookup"><span data-stu-id="39079-136">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a><span data-ttu-id="39079-137">Nainstalovat synchronizaci odkazů partnerského centra pro Dynamics 365 (řešení Power automat)</span><span class="sxs-lookup"><span data-stu-id="39079-137">Install Partner Center Referrals Synchronization for Dynamics 365 (Power Automate Solution)</span></span>

1. <span data-ttu-id="39079-138">V pravém horním rohu vyberte **prostředí** k [automatizaci](https://flow.microsoft.com) a vyberte prostředí.</span><span class="sxs-lookup"><span data-stu-id="39079-138">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="39079-139">Tento krok vám ukáže dostupné instance CRM.</span><span class="sxs-lookup"><span data-stu-id="39079-139">This step will show you the available CRM instances.</span></span>

2. <span data-ttu-id="39079-140">V rozevíracím seznamu v pravém horním rohu vyberte příslušnou instanci CRM.</span><span class="sxs-lookup"><span data-stu-id="39079-140">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="39079-141">Na levém navigačním panelu vyberte **řešení** .</span><span class="sxs-lookup"><span data-stu-id="39079-141">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="39079-142">V horní nabídce klikněte na odkaz **otevřít AppSource** .</span><span class="sxs-lookup"><span data-stu-id="39079-142">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Otevřít AppSource":::

5. <span data-ttu-id="39079-144">V místní obrazovce vyhledejte **konektory odkazů partnerského centra pro Dynamics365** .</span><span class="sxs-lookup"><span data-stu-id="39079-144">Search for **Partner Center Referrals Connectors for Dynamics365** in the pop-up screen.</span></span>  

6. <span data-ttu-id="39079-145">Klikněte na tlačítko **získat nyní** a potom **pokračujte**.</span><span class="sxs-lookup"><span data-stu-id="39079-145">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="39079-146">Otevře se stránka, kde můžete vybrat prostředí CRM (Dynamics 365) k instalaci aplikace.</span><span class="sxs-lookup"><span data-stu-id="39079-146">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="39079-147">Vyjádřit souhlas s podmínkami a ujednáními.</span><span class="sxs-lookup"><span data-stu-id="39079-147">Agree to terms and conditions.</span></span>

8. <span data-ttu-id="39079-148">Pak budete přesměrováni na stránku **spravovat vaše řešení** .</span><span class="sxs-lookup"><span data-stu-id="39079-148">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="39079-149">Přejděte na "odkazy na partnerské Centrum" pomocí tlačítek se šipkami ve spodní části stránky.</span><span class="sxs-lookup"><span data-stu-id="39079-149">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="39079-150">**Naplánovaná instalace** by se měla objevit u řešení s odkazy partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="39079-150">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="39079-151">Instalace bude trvat 10-15 minut.</span><span class="sxs-lookup"><span data-stu-id="39079-151">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="39079-152">Po dokončení instalace přejděte zpátky na [Power](https://flow.microsoft.com) automat a vyberte **řešení** z navigační oblasti vlevo.</span><span class="sxs-lookup"><span data-stu-id="39079-152">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="39079-153">Všimněte si, že v seznamu řešení je k dispozici **synchronizace odkazů partnerského centra pro Dynamics 365** .</span><span class="sxs-lookup"><span data-stu-id="39079-153">Notice that **Partner Center Referrals Synchronization for Dynamics 365** is available in the Solutions list.</span></span>

10. <span data-ttu-id="39079-154">Vyberte **synchronizaci odkazů partnerského centra pro Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="39079-154">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="39079-155">K dispozici jsou tyto toky a entity automatizace pro napájení:</span><span class="sxs-lookup"><span data-stu-id="39079-155">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Dostupné CRMS":::

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="39079-157">Osvědčené postupy: test před zahájením provozu</span><span class="sxs-lookup"><span data-stu-id="39079-157">Best practice: test before you go live</span></span>

<span data-ttu-id="39079-158">Než nainstalujete, nakonfigurujete a přizpůsobíte řešení Power Automate v produkčním prostředí, ujistěte se, že řešení otestujete v pracovní instanci CRM.</span><span class="sxs-lookup"><span data-stu-id="39079-158">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="39079-159">Nainstalujte řešení Microsoft Power automatizuje do přípravného prostředí/instance CRM.</span><span class="sxs-lookup"><span data-stu-id="39079-159">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="39079-160">Vytvořte kopii řešení a spusťte konfiguraci a automatizujte vlastní nastavení toků v přípravném prostředí.</span><span class="sxs-lookup"><span data-stu-id="39079-160">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>
- <span data-ttu-id="39079-161">Otestujte řešení na pracovní instanci/CRM.</span><span class="sxs-lookup"><span data-stu-id="39079-161">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="39079-162">Po úspěšném dokončení naimportujte jako spravované řešení do provozní instance.</span><span class="sxs-lookup"><span data-stu-id="39079-162">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="39079-163">Konfigurace řešení</span><span class="sxs-lookup"><span data-stu-id="39079-163">Configure the solution</span></span>

1. <span data-ttu-id="39079-164">Po instalaci řešení do instance CRM přejděte zpátky na [Power](https://flow.microsoft.com/)automat.</span><span class="sxs-lookup"><span data-stu-id="39079-164">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>


2. <span data-ttu-id="39079-165">V rozevíracím seznamu **prostředí** v pravém horním rohu vyberte instanci CRM, do které jste nainstalovali řešení Power automatizuje.</span><span class="sxs-lookup"><span data-stu-id="39079-165">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="39079-166">Budete muset vytvořit připojení, která přiřadí tři uživatelské účty:</span><span class="sxs-lookup"><span data-stu-id="39079-166">You'll need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="39079-167">Uživatel partnerského centra s přihlašovacími údaji správce odkazů</span><span class="sxs-lookup"><span data-stu-id="39079-167">Partner Center user with referrals admin credentials</span></span>

   - <span data-ttu-id="39079-168">Události Partnerského centra</span><span class="sxs-lookup"><span data-stu-id="39079-168">Partner Center Events</span></span>

   - <span data-ttu-id="39079-169">Správce CRM s Power Automate automatizuje v řešení.</span><span class="sxs-lookup"><span data-stu-id="39079-169">CRM admin with the Power Automate flows in the solution.</span></span>

      1. <span data-ttu-id="39079-170">V levém navigačním panelu vyberte **připojení** a v seznamu vyberte řešení partnerského centra pro partnery.</span><span class="sxs-lookup"><span data-stu-id="39079-170">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>

      2. <span data-ttu-id="39079-171">Vytvořte připojení kliknutím na **vytvořit připojení**.</span><span class="sxs-lookup"><span data-stu-id="39079-171">Create a connection by clicking **Create a connection**.</span></span>

         :::image type="content" source="images/cosellconnectors/dynamics1.png" alt-text="Vytvoření připojení":::

      3. <span data-ttu-id="39079-173">Na panelu hledání v pravém horním rohu vyhledejte **odkazy na partnerské Centrum (Preview)** .</span><span class="sxs-lookup"><span data-stu-id="39079-173">Search for **Partner Center Referrals (preview)** in the search bar on the top-right corner.</span></span>

      4. <span data-ttu-id="39079-174">Vytvořte připojení pro uživatele partnerského centra s rolí přihlašovacích údajů správce odkazů.</span><span class="sxs-lookup"><span data-stu-id="39079-174">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

      5. <span data-ttu-id="39079-175">Potom vytvořte připojení událostí partnerského centra pro uživatele partnerského centra s přihlašovacími údaji správce odkazů.</span><span class="sxs-lookup"><span data-stu-id="39079-175">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

      6. <span data-ttu-id="39079-176">Vytvořte připojení pro Common Data Service (aktuální prostředí) pro uživatele správce CRM.</span><span class="sxs-lookup"><span data-stu-id="39079-176">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>
       
     
      7. <span data-ttu-id="39079-177">Po přidání všech připojení byste měli ve svém prostředí zobrazit následující připojení:</span><span class="sxs-lookup"><span data-stu-id="39079-177">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

:::image type="content" source="images/cosellconnectors/dynamics2.png" alt-text="Připojení":::
   
## <a name="edit-the-connections"></a><span data-ttu-id="39079-179">Upravit připojení</span><span class="sxs-lookup"><span data-stu-id="39079-179">Edit the connections</span></span>

1. <span data-ttu-id="39079-180">Vraťte se na stránku **řešení** a vyberte **výchozí řešení**.</span><span class="sxs-lookup"><span data-stu-id="39079-180">Return to the **Solutions** page and select **Default Solution**.</span></span> <span data-ttu-id="39079-181">Kliknutím na tlačítko **vše** vyberte **odkaz připojení (Preview)** .</span><span class="sxs-lookup"><span data-stu-id="39079-181">Select **Connection Reference (preview)** by clicking **All**.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics3.png" alt-text="Připojit":::

2. <span data-ttu-id="39079-183">Každé připojení jednu po jedné upravte výběrem ikony tři tečky.</span><span class="sxs-lookup"><span data-stu-id="39079-183">Edit each of the Connections one by one by selecting the three dots icon.</span></span> <span data-ttu-id="39079-184">Přidejte příslušná připojení.</span><span class="sxs-lookup"><span data-stu-id="39079-184">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics4.png" alt-text="Uvedená připojení"::: 

3.  <span data-ttu-id="39079-186">Zapněte toky v následujícím pořadí:</span><span class="sxs-lookup"><span data-stu-id="39079-186">Turn on the flows in the following sequence:</span></span>
- <span data-ttu-id="39079-187">Registrace Webhooku partnerského centra (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="39079-187">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="39079-188">Vytvoření odkazu na společný prodej – Dynamics 365 do partnerského centra (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="39079-188">Create Co-sell Referral – Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="39079-189">Partnerské centrum pro spoluprodejní aktualizace pro Microsoft Dynamics 365 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="39079-189">Partner Center Microsoft Co-sell Referral Updates to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="39079-190">Partnerské centrum k Dynamics 365 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="39079-190">Partner Center to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="39079-191">Dynamics 365 do partnerského centra (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="39079-191">Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="39079-192">Příležitost Dynamics 365 do partnerského centra (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="39079-192">Dynamics 365 Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="39079-193">Řešení Microsoft Dynamics 365 od Microsoftu do partnerského centra (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="39079-193">Dynamics 365 Microsoft Solutions to Partner Center (Insider Preview)</span></span>
 

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="39079-194">Použití rozhraní Webhook API k registraci pro události změny prostředku</span><span class="sxs-lookup"><span data-stu-id="39079-194">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="39079-195">Rozhraní API Webhooku partnerského centra vám umožní registrovat se na události změny prostředků.</span><span class="sxs-lookup"><span data-stu-id="39079-195">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="39079-196">Tyto události změny se odesílají na adresu URL jako příspěvky HTTP.</span><span class="sxs-lookup"><span data-stu-id="39079-196">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="39079-197">Pokud chcete zaregistrovat adresu URL, vyberte možnost **registrace Webhooku partnerského centra (Insider Preview)** Power automatizace.</span><span class="sxs-lookup"><span data-stu-id="39079-197">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="39079-198">Přidat připojení pro uživatele partnerského centra (a.) s událostmi partnerského centra s přihlašovacími údaji správce (b.), jak je zvýrazněno níže</span><span class="sxs-lookup"><span data-stu-id="39079-198">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Trigger":::

3. <span data-ttu-id="39079-200">Po provedení těchto aktualizací se zobrazí</span><span class="sxs-lookup"><span data-stu-id="39079-200">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooky":::

4. <span data-ttu-id="39079-202">Uložte změny a vyberte **zapnout**.</span><span class="sxs-lookup"><span data-stu-id="39079-202">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="39079-203">Pokud chcete, aby Webhooky partnerského centra naslouchali změnám událostí, proveďte následující kroky:</span><span class="sxs-lookup"><span data-stu-id="39079-203">To enable Partner Center webhooks to listen to event changes, do the following steps:</span></span>

5. <span data-ttu-id="39079-204">Vyberte **Partnerské centrum pro Dynamics 365 (Insider Preview)**.</span><span class="sxs-lookup"><span data-stu-id="39079-204">Select **Partner Center to Dynamics 365 (Insider Preview)**.</span></span>

6. <span data-ttu-id="39079-205">Vyberte ikonu **Upravit** a vyberte, **kdy se přijme požadavek HTTP**.</span><span class="sxs-lookup"><span data-stu-id="39079-205">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="39079-206">Kliknutím na ikonu **kopírování** zkopírujte zadanou adresu URL post protokolu HTTP.</span><span class="sxs-lookup"><span data-stu-id="39079-206">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="Zkopírování adresy URL":::

8. <span data-ttu-id="39079-208">Nyní vyberte možnost "automatické registrace Webhooku partnerského centra (Insider Preview)" a vyberte **Spustit**.</span><span class="sxs-lookup"><span data-stu-id="39079-208">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="39079-209">Ujistěte se, že se v pravém podokně otevře okno spustit tok a klikněte na **pokračovat**.</span><span class="sxs-lookup"><span data-stu-id="39079-209">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="39079-210">Zadejte následující podrobnosti:</span><span class="sxs-lookup"><span data-stu-id="39079-210">Enter the following details:</span></span>

    1. <span data-ttu-id="39079-211">**Koncový bod triggeru http**: adresa URL zkopírována z předchozího kroku</span><span class="sxs-lookup"><span data-stu-id="39079-211">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="39079-212">**Události k registraci**: odkaz-vytvořeno a odkaz-Aktualizováno</span><span class="sxs-lookup"><span data-stu-id="39079-212">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    3. <span data-ttu-id="39079-213">**Přepsat existující koncové body triggeru, pokud je k dispozici**: Ano (přepsání všech stávajících koncových bodů)</span><span class="sxs-lookup"><span data-stu-id="39079-213">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="39079-214">Vyberte **Spustit** a potom vyberte **Hotovo.**</span><span class="sxs-lookup"><span data-stu-id="39079-214">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="39079-215">Webhook teď může naslouchat událostem vytvoření a aktualizace.</span><span class="sxs-lookup"><span data-stu-id="39079-215">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="39079-216">Přizpůsobení kroků synchronizace</span><span class="sxs-lookup"><span data-stu-id="39079-216">Customize synchronization steps</span></span>

<span data-ttu-id="39079-217">Pokud jsou odkazy na spoluprodejní synchronizace mezi partnerským centrem a vaším systémem CRM, tady jsou uvedená pole synchronizovaná v počítači partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="39079-217">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="39079-218">Systémy CRM jsou často vysoce přizpůsobené.</span><span class="sxs-lookup"><span data-stu-id="39079-218">Often CRM systems are highly customized.</span></span> <span data-ttu-id="39079-219">Můžete přizpůsobit automatické toky Power Automate.</span><span class="sxs-lookup"><span data-stu-id="39079-219">You can customize the Power Automate flows.</span></span> <span data-ttu-id="39079-220">Postupujte podle pokynů pro mapování polí a v případě potřeby proveďte příslušné změny v postupech automatizace toků.</span><span class="sxs-lookup"><span data-stu-id="39079-220">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="39079-221">K dispozici jsou mapování partnerských Center Microsoftu na CRM, ale v závislosti na vašem prostředí CRM, můžete zvolit další přizpůsobení polí.</span><span class="sxs-lookup"><span data-stu-id="39079-221">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="39079-222">V závislosti na vašich potřebách je možné přizpůsobit více kroků každého z těchto toků automatizace napájení.</span><span class="sxs-lookup"><span data-stu-id="39079-222">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="39079-223">Následují příklady dostupných přizpůsobení:</span><span class="sxs-lookup"><span data-stu-id="39079-223">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="39079-224">Přizpůsobení polí pro události vytvoření nebo aktualizace v partnerském centru pro synchronizaci odkazů CRM:</span><span class="sxs-lookup"><span data-stu-id="39079-224">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="39079-225">a.</span><span class="sxs-lookup"><span data-stu-id="39079-225">a.</span></span> <span data-ttu-id="39079-226">Vyberte partnerské Centrum pro Dynamics 365 (Insider Preview) nebo partnerské Centrum do Salesforce (Insider Preview).</span><span class="sxs-lookup"><span data-stu-id="39079-226">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

    <span data-ttu-id="39079-227">b.</span><span class="sxs-lookup"><span data-stu-id="39079-227">b.</span></span> <span data-ttu-id="39079-228">Vyberte **Upravit** a upravte nebo Přizpůsobte tok automatizovaného výkonu.</span><span class="sxs-lookup"><span data-stu-id="39079-228">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="39079-229">c.</span><span class="sxs-lookup"><span data-stu-id="39079-229">c.</span></span> <span data-ttu-id="39079-230">Vyberte **(rozsah) synchronizujte zájemce nebo příležitost**.</span><span class="sxs-lookup"><span data-stu-id="39079-230">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="39079-231">Pokud chcete přizpůsobit mapování polí CRM (na základě Průvodce mapováním polí) pro události vytvořit, vyberte, **jestli je nová sdílená příležitost, a pak**.</span><span class="sxs-lookup"><span data-stu-id="39079-231">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="39079-232">Vyberte dílčí krok, **Pokud ano** , a pak rozbalte **vytvořit novou příležitost v CRM**.</span><span class="sxs-lookup"><span data-stu-id="39079-232">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="39079-233">Mapování v této části můžete upravit pomocí Průvodce mapováním polí.</span><span class="sxs-lookup"><span data-stu-id="39079-233">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="39079-234">d.</span><span class="sxs-lookup"><span data-stu-id="39079-234">d.</span></span> <span data-ttu-id="39079-235">Pro přizpůsobení mapování polí CRM (na základě Průvodce mapováním polí) pro události aktualizace klikněte na krok (obor) synchronizovat zájemce nebo příležitost.</span><span class="sxs-lookup"><span data-stu-id="39079-235">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="39079-236">e.</span><span class="sxs-lookup"><span data-stu-id="39079-236">e.</span></span> <span data-ttu-id="39079-237">Vyberte **, jestli se jedná o aktualizaci příležitosti, a pak**.</span><span class="sxs-lookup"><span data-stu-id="39079-237">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="39079-238">Vyberte dílčí krok, **Pokud ano** , a pak rozbalte **rozdíl mezi objekty příležitostí v partnerském centru a CRM a pak**.</span><span class="sxs-lookup"><span data-stu-id="39079-238">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

    <span data-ttu-id="39079-239">f.</span><span class="sxs-lookup"><span data-stu-id="39079-239">f.</span></span> <span data-ttu-id="39079-240">Vyberte, **jestli ano** , a pak **aktualizovat existující příležitost** .</span><span class="sxs-lookup"><span data-stu-id="39079-240">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="39079-241">Přizpůsobení polí pro synchronizaci odkazů CRM na počítač pro události aktualizace:</span><span class="sxs-lookup"><span data-stu-id="39079-241">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="39079-242">a.</span><span class="sxs-lookup"><span data-stu-id="39079-242">a.</span></span> <span data-ttu-id="39079-243">Vyberte **Upravit**  a upravte nebo Přizpůsobte tok automatizovaného výkonu.</span><span class="sxs-lookup"><span data-stu-id="39079-243">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="39079-244">b.</span><span class="sxs-lookup"><span data-stu-id="39079-244">b.</span></span> <span data-ttu-id="39079-245">Vyberte **(rozsah) synchronizace příležitosti**.</span><span class="sxs-lookup"><span data-stu-id="39079-245">Select **(Scope) Synchronize the opportunity**.</span></span>

    <span data-ttu-id="39079-246">c.</span><span class="sxs-lookup"><span data-stu-id="39079-246">c.</span></span> <span data-ttu-id="39079-247">Pokud chcete přizpůsobit mapování polí CRM pro události aktualizace, vyberte, **jestli jsou mezi objekty zájemce v partnerském centru a CRM rozdílové rozdíly, a pak**.</span><span class="sxs-lookup"><span data-stu-id="39079-247">To customize CRM field mappings for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span> 

    <span data-ttu-id="39079-248">d.</span><span class="sxs-lookup"><span data-stu-id="39079-248">d.</span></span> <span data-ttu-id="39079-249">Vyberte dílčí krok, **Pokud ano** , a pak rozbalte krok **aktualizace odkazu s daty příležitostí**.</span><span class="sxs-lookup"><span data-stu-id="39079-249">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="39079-250">Mapování v této části můžete upravit v závislosti na průvodci mapováním polí.</span><span class="sxs-lookup"><span data-stu-id="39079-250">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="39079-251">Chcete-li přizpůsobit pole pro synchronizaci odkazů CRM na počítač pro vytvoření událostí?</span><span class="sxs-lookup"><span data-stu-id="39079-251">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="39079-252">a.</span><span class="sxs-lookup"><span data-stu-id="39079-252">a.</span></span> <span data-ttu-id="39079-253">Vyberte **Upravit**  a upravte nebo Přizpůsobte tok automatizovaného výkonu.</span><span class="sxs-lookup"><span data-stu-id="39079-253">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="39079-254">b.</span><span class="sxs-lookup"><span data-stu-id="39079-254">b.</span></span> <span data-ttu-id="39079-255">Výběr **(rozsah) synchronizace odkazů.**</span><span class="sxs-lookup"><span data-stu-id="39079-255">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="39079-256">c.</span><span class="sxs-lookup"><span data-stu-id="39079-256">c.</span></span> <span data-ttu-id="39079-257">Pokud chcete přizpůsobit mapování polí CRM (na základě Průvodce mapováním polí) pro události vytvořit, vyberte **vytvořit odkaz Microsoftu**.</span><span class="sxs-lookup"><span data-stu-id="39079-257">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

   <span data-ttu-id="39079-258">Mapování v této části můžete upravit v závislosti na průvodci mapováním polí.</span><span class="sxs-lookup"><span data-stu-id="39079-258">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

<span data-ttu-id="39079-259">Vytvořili jste dvě proměnné prostředí:</span><span class="sxs-lookup"><span data-stu-id="39079-259">There are two environment variables created:</span></span>

- <span data-ttu-id="39079-260">Zaškrtnutí: značí, jestli byste potřebovali ikonu zaškrtnutí, kromě příležitostí, které se synchronizují obousměrně mezi partnerským centrem a Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="39079-260">Checkmark: Signifies whether you would need a checkmark icon besides opportunities that are synchronized bi-directionally between Partner Center and Dynamics 365 CRM.</span></span>

- <span data-ttu-id="39079-261">Synchronizovat pouze příležitosti společného prodeje: označuje, zda chcete synchronizovat pouze příležitosti společného prodeje.</span><span class="sxs-lookup"><span data-stu-id="39079-261">Sync co-sell opportunities only: Signifies whether you want to synchronize only Co-sell opportunities.</span></span>

<span data-ttu-id="39079-262">Můžete zvolit úpravu výchozí hodnoty pro proměnné prostředí.</span><span class="sxs-lookup"><span data-stu-id="39079-262">You can choose to edit the default value for the environment variables.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics5.png" alt-text="Textové pole pro výchozí hodnoty":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="39079-264">Komplexní Obousměrná synchronizace odkazů v rámci společného prodeje</span><span class="sxs-lookup"><span data-stu-id="39079-264">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="39079-265">Jakmile nainstalujete, nakonfigurujete a přizpůsobíte řešení Power Automate, můžete otestovat synchronizaci odkazů mezi produkty Dynamics 365 a Partnerským centrem společně prodávat.</span><span class="sxs-lookup"><span data-stu-id="39079-265">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="39079-266">Požadavky</span><span class="sxs-lookup"><span data-stu-id="39079-266">Pre-requisites</span></span>

<span data-ttu-id="39079-267">Aby bylo možné synchronizovat odkazy v rámci partnerského centra a Dynamics 365 CRM, řešení Power automat jasně vymezuje pole odkazů specifická pro společnost Microsoft.</span><span class="sxs-lookup"><span data-stu-id="39079-267">To synchronize the referrals across Partner Center and Dynamics 365 CRM, the Power Automate solution clearly demarcates Microsoft-specific referral fields.</span></span> <span data-ttu-id="39079-268">Tato identifikace dává prodejcům možnost rozhodnout se, které odkazy chce sdílet se společností Microsoft pro souběžný prodej.</span><span class="sxs-lookup"><span data-stu-id="39079-268">This identification gives your seller teams  the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="39079-269">Sada vlastních polí je k dispozici jako součást entity **příležitosti** .</span><span class="sxs-lookup"><span data-stu-id="39079-269">A set of custom fields is available as part of the **Opportunity** entity.</span></span> <span data-ttu-id="39079-270">Uživatel s oprávněními správce CRM bude muset vytvořit samostatný oddíl CRM s vlastními poli **příležitosti** .</span><span class="sxs-lookup"><span data-stu-id="39079-270">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="39079-271">Následující vlastní pole by měla být součástí části CRM:</span><span class="sxs-lookup"><span data-stu-id="39079-271">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="39079-272">**Synchronizovat s partnerským centrem**: jestli se má synchronizovat příležitost s partnerským centrem Microsoftu</span><span class="sxs-lookup"><span data-stu-id="39079-272">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="39079-273">**Identifikátor odkazu**: pole identifikátoru jen pro čtení pro odkaz na partnerského centra Microsoftu</span><span class="sxs-lookup"><span data-stu-id="39079-273">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="39079-274">**Odkaz** odkazu: odkaz na odkaz určený jen pro čtení v partnerském centru Microsoftu</span><span class="sxs-lookup"><span data-stu-id="39079-274">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="39079-275">**Jak může společnost Microsoft** získat nápovědu? od Microsoftu se dozvíte, jak tento odkaz vyžaduje.</span><span class="sxs-lookup"><span data-stu-id="39079-275">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="39079-276">**Produkty**: seznam produktů přidružených k této příležitosti</span><span class="sxs-lookup"><span data-stu-id="39079-276">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="39079-277">**Audit**: záznam auditu jen pro čtení pro synchronizaci s odkazy partnerského centra</span><span class="sxs-lookup"><span data-stu-id="39079-277">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

<span data-ttu-id="39079-278">Aktualizujte formulář příležitost v Dynamics 365 CRM a uveďte řešení pro pole Products.</span><span class="sxs-lookup"><span data-stu-id="39079-278">Update the opportunity form in Dynamics 365 CRM to include Solutions for Products field.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics6.png" alt-text="Formulář příležitosti":::

:::image type="content" source="images/cosellconnectors/dynamics7.png" alt-text="{alt-text}":::

### <a name="scenarios"></a><span data-ttu-id="39079-281">ŘEŠENÍ</span><span class="sxs-lookup"><span data-stu-id="39079-281">SCENARIOS:</span></span>

1. <span data-ttu-id="39079-282">Referenční synchronizace při vytvoření nebo aktualizaci odkazu v CRM a synchronizovaných v partnerském centru:</span><span class="sxs-lookup"><span data-stu-id="39079-282">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="39079-283">Přihlaste se k prostředí Dynamics 365 CRM s uživatelem, který má v části **příležitost** v aplikaci CRM přehled.</span><span class="sxs-lookup"><span data-stu-id="39079-283">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="39079-284">Při vytváření nové příležitosti v prostředí Dynamics 365 se ujistěte, že je k dispozici následující oddíl.</span><span class="sxs-lookup"><span data-stu-id="39079-284">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="Část s ukázkou příležitostí zobrazující informace o partnerském centru Microsoftu v Dynamics 365.":::

   3. <span data-ttu-id="39079-286">Pokud chcete tuto příležitost synchronizovat s partnerským centrem Microsoftu, ujistěte se, že jste v zobrazení karta nastavili následující pole:</span><span class="sxs-lookup"><span data-stu-id="39079-286">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="39079-287">**Synchronizovat s partnerským centrem**: Ano</span><span class="sxs-lookup"><span data-stu-id="39079-287">**Sync with Partner Center**: Yes</span></span>

      - <span data-ttu-id="39079-288">**Jak může Microsoft pomáhat?**: vyberte z těchto možností:</span><span class="sxs-lookup"><span data-stu-id="39079-288">**How can Microsoft help?**: Select from the following:</span></span>

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="Oddíl ukázkové příležitosti v Dynamics 365, který zobrazuje možnosti pomocníka pro partnerské Centrum Microsoftu vedle pole s názvem Jak může pomáhat Microsoft?":::

      - <span data-ttu-id="39079-290">**Produkty**: ID řešení produktu</span><span class="sxs-lookup"><span data-stu-id="39079-290">**Products**: Solution IDs of the product</span></span>

   4. <span data-ttu-id="39079-291">Až se příležitost vytvoří v Dynamics 365 s možností **synchronizovat s partnerským centrem** nastavenou na **Ano**, počkejte 10 minut a pak se přihlaste k účtu partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="39079-291">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, and then sign into your Partner Center account.</span></span> <span data-ttu-id="39079-292">Vaše odkazy budou synchronizovány s Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="39079-292">Your referrals will be synchronized with Dynamics 365.</span></span>

   5. <span data-ttu-id="39079-293">Podobně platí, že pokud chcete příležitost, která má možnost synchronizovat s partnerským centrem nastavenou na hodnotu Ano, aktualizovat příležitost v Dynamics 365 CRM, změny se synchronizují v účtu partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="39079-293">Likewise, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

   6. <span data-ttu-id="39079-294">Příležitosti, které byly úspěšně synchronizovány s partnerským centrem, budou označeny ikonou ✔ v Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="39079-294">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="39079-295">Referenční synchronizace při vytvoření nebo aktualizaci odkazu v partnerském centru Microsoftu a synchronizovaných v prostředí Dynamics 365:</span><span class="sxs-lookup"><span data-stu-id="39079-295">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="39079-296">Přihlaste se k [řídicímu panelu](https://partner.microsoft.com/dashboard/home)partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="39079-296">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   2. <span data-ttu-id="39079-297">V nabídce na levé straně vyberte **odkazy** .</span><span class="sxs-lookup"><span data-stu-id="39079-297">Select **Referrals** from the left-hand menu.</span></span>

   3. <span data-ttu-id="39079-298">Klikněte na možnost Nová práce a vytvořte si nový odkaz na společný prodej z partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="39079-298">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

   4. <span data-ttu-id="39079-299">Přihlaste se k prostředí Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="39079-299">Sign into your Dynamics 365 CRM environment.</span></span>

   5. <span data-ttu-id="39079-300">Přejděte na **otevřené příležitosti**.</span><span class="sxs-lookup"><span data-stu-id="39079-300">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="39079-301">Odkaz vytvořený v partnerském centru Microsoftu je teď synchronizovaný v Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="39079-301">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   6. <span data-ttu-id="39079-302">Když vyberete synchronizovaný odkaz, vyplní se podrobnosti zobrazení karty.</span><span class="sxs-lookup"><span data-stu-id="39079-302">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="39079-303">Další kroky</span><span class="sxs-lookup"><span data-stu-id="39079-303">Next steps</span></span>

- [<span data-ttu-id="39079-304">Správa potenciálních zákazníků</span><span class="sxs-lookup"><span data-stu-id="39079-304">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="39079-305">Správa příležitostí ke spoluprodeji</span><span class="sxs-lookup"><span data-stu-id="39079-305">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="39079-306">Další informace o platformě Microsoft Power automatizuje?</span><span class="sxs-lookup"><span data-stu-id="39079-306">More about Microsoft Power Automate platform?</span></span>](/power-automate/)

- [<span data-ttu-id="39079-307">Webhooky partnerského centra</span><span class="sxs-lookup"><span data-stu-id="39079-307">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)