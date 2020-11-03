---
title: Konektor pro spoluprodeji pro partnerské Centrum Dynamics 365 CRM
ms.topic: how-to
ms.date: 05/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Synchronizujte své odkazy v partnerském centru s konektorem pro spoluprodeji pro Dynamics 365 CRM. Prodejci pak můžou v rámci svých systémů CRM prodávat společně s Microsoftem.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 8ea803e675ce7c2d21d680491bbdaedf792e631f
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/14/2020
ms.locfileid: "92527685"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a><span data-ttu-id="c75e3-104">Konektor pro společný prodej pro Dynamics 365 CRM – přehled</span><span class="sxs-lookup"><span data-stu-id="c75e3-104">Co-sell connector for Dynamics 365 CRM – Overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="c75e3-105">Příslušné role</span><span class="sxs-lookup"><span data-stu-id="c75e3-105">Appropriate roles</span></span>

- <span data-ttu-id="c75e3-106">Správce odkazů</span><span class="sxs-lookup"><span data-stu-id="c75e3-106">Referrals admin</span></span>
- <span data-ttu-id="c75e3-107">Správce systému nebo úpravce systému v CRM</span><span class="sxs-lookup"><span data-stu-id="c75e3-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="c75e3-108">Konektor pro spoluprodej v partnerském centru umožňuje prodejcům v rámci svých systémů CRM spolupracovat s Microsoftem.</span><span class="sxs-lookup"><span data-stu-id="c75e3-108">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="c75e3-109">Nebudou se muset vyškolet k používání partnerského centra ke správě obchodů v rámci společného prodeje.</span><span class="sxs-lookup"><span data-stu-id="c75e3-109">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="c75e3-110">Pomocí konektorů pro spoluprodeji můžete vytvořit nový společný odkaz pro prodej prodávajícího, získat referenční údaje od prodejce Microsoftu, přijmout nebo odmítnout odkazy, upravit data o koupi, jako je například hodnota kouposti a datum ukončení.</span><span class="sxs-lookup"><span data-stu-id="c75e3-110">Use the Co-sell connectors, to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span> <span data-ttu-id="c75e3-111">K těmto obchodům v rámci těchto spoluprodejů můžete také dostávat jakékoli aktualizace od prodejců Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="c75e3-111">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="c75e3-112">Všechny vaše odkazy můžete v aplikaci CRM použít místo v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="c75e3-112">You can do all of your referrals work within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="c75e3-113">Řešení je založené na řešení Microsoft Power automatizuje a používá rozhraní API partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="c75e3-113">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="c75e3-114">Před instalací – požadavky</span><span class="sxs-lookup"><span data-stu-id="c75e3-114">Before you install - pre-requisites</span></span>

|<span data-ttu-id="c75e3-115">**Témata**</span><span class="sxs-lookup"><span data-stu-id="c75e3-115">**Topics**</span></span>   |<span data-ttu-id="c75e3-116">**Podrobnosti**</span><span class="sxs-lookup"><span data-stu-id="c75e3-116">**Details**</span></span>   |<span data-ttu-id="c75e3-117">**Odkazy**</span><span class="sxs-lookup"><span data-stu-id="c75e3-117">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="c75e3-118">ID Microsoft Partner Network</span><span class="sxs-lookup"><span data-stu-id="c75e3-118">Microsoft Partner Network ID</span></span> |<span data-ttu-id="c75e3-119">Potřebujete platné ID MPN.</span><span class="sxs-lookup"><span data-stu-id="c75e3-119">You need a valid MPN ID</span></span>|<span data-ttu-id="c75e3-120">Připojení k programu [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="c75e3-120">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="c75e3-121">Předprodejní připraveno</span><span class="sxs-lookup"><span data-stu-id="c75e3-121">Cosell ready</span></span>|<span data-ttu-id="c75e3-122">Vaše řešení IP/Services musí být připravené k prodeji.</span><span class="sxs-lookup"><span data-stu-id="c75e3-122">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="c75e3-123">Prodej pomocí Microsoftu</span><span class="sxs-lookup"><span data-stu-id="c75e3-123">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="c75e3-124">Účet partnerského centra</span><span class="sxs-lookup"><span data-stu-id="c75e3-124">Partner Center account</span></span>|<span data-ttu-id="c75e3-125">ID MPN přidružené k tenantovi partnerského centra musí být stejné jako ID MPN přidružené k vašemu řešení společného prodeje.</span><span class="sxs-lookup"><span data-stu-id="c75e3-125">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="c75e3-126">Před nasazením konektorů se můžete podívat na to, jestli máte na portálu partnerského centra zobrazený odkaz na svůj společný prodej.</span><span class="sxs-lookup"><span data-stu-id="c75e3-126">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="c75e3-127">Správa vašeho účtu</span><span class="sxs-lookup"><span data-stu-id="c75e3-127">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="c75e3-128">Role uživatelů partnerského centra</span><span class="sxs-lookup"><span data-stu-id="c75e3-128">Partner Center user roles</span></span>|<span data-ttu-id="c75e3-129">Zaměstnanec, který bude instalovat a používat konektory, musí být správcem odkazů.</span><span class="sxs-lookup"><span data-stu-id="c75e3-129">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="c75e3-130">Přiřazování uživatelských rolí a oprávnění</span><span class="sxs-lookup"><span data-stu-id="c75e3-130">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)| |<span data-ttu-id="c75e3-131">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="c75e3-131">Dynamics 365 CRM</span></span>|<span data-ttu-id="c75e3-132">Role uživatele CRM je správce systému nebo úpravce systému.</span><span class="sxs-lookup"><span data-stu-id="c75e3-132">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="c75e3-133">Přiřazení rolí v Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="c75e3-133">Assign roles in Dynamics 365</span></span>](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="c75e3-134">Zapnout účet toku automatizace</span><span class="sxs-lookup"><span data-stu-id="c75e3-134">Power Automate Flow Account</span></span>|<span data-ttu-id="c75e3-135">Aktivní účet [Power automatizuje](https://flow.microsoft.com) pro správce systému nebo úpravce systému CRM.</span><span class="sxs-lookup"><span data-stu-id="c75e3-135">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="c75e3-136">Tento uživatel se musí před instalací přihlásit k [automatizaci](https://flow.microsoft.com) aspoň jednou.</span><span class="sxs-lookup"><span data-stu-id="c75e3-136">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a><span data-ttu-id="c75e3-137">Nainstalovat synchronizaci odkazů partnerského centra pro Dynamics 365 (řešení Power automat)</span><span class="sxs-lookup"><span data-stu-id="c75e3-137">Install Partner Center Referrals Synchronization for Dynamics 365 (Power Automate Solution)</span></span>

1. <span data-ttu-id="c75e3-138">V pravém horním rohu vyberte **prostředí** k [automatizaci](https://flow.microsoft.com) a vyberte prostředí.</span><span class="sxs-lookup"><span data-stu-id="c75e3-138">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="c75e3-139">Tento krok vám ukáže dostupné instance CRM.</span><span class="sxs-lookup"><span data-stu-id="c75e3-139">This step will show you the available CRM instances.</span></span>

2. <span data-ttu-id="c75e3-140">V rozevíracím seznamu v pravém horním rohu vyberte příslušnou instanci CRM.</span><span class="sxs-lookup"><span data-stu-id="c75e3-140">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="c75e3-141">Na levém navigačním panelu vyberte **řešení** .</span><span class="sxs-lookup"><span data-stu-id="c75e3-141">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="c75e3-142">V horní nabídce klikněte na odkaz **otevřít AppSource** .</span><span class="sxs-lookup"><span data-stu-id="c75e3-142">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Otevřít AppSource":::

5. <span data-ttu-id="c75e3-144">V místní obrazovce vyhledejte **konektory odkazů partnerského centra pro Dynamics365** .</span><span class="sxs-lookup"><span data-stu-id="c75e3-144">Search for **Partner Center Referrals Connectors for Dynamics365** in the pop-up screen.</span></span>  

6. <span data-ttu-id="c75e3-145">Klikněte na tlačítko **získat nyní** a potom **pokračujte** .</span><span class="sxs-lookup"><span data-stu-id="c75e3-145">Click the **Get it now** button and then **Continue** .</span></span>

7. <span data-ttu-id="c75e3-146">Otevře se stránka, kde můžete vybrat prostředí CRM (Dynamics 365) k instalaci aplikace.</span><span class="sxs-lookup"><span data-stu-id="c75e3-146">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="c75e3-147">Vyjádřit souhlas s podmínkami a ujednáními.</span><span class="sxs-lookup"><span data-stu-id="c75e3-147">Agree to terms and conditions.</span></span>

8. <span data-ttu-id="c75e3-148">Pak budete přesměrováni na stránku **spravovat vaše řešení** .</span><span class="sxs-lookup"><span data-stu-id="c75e3-148">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="c75e3-149">Přejděte na "odkazy na partnerské Centrum" pomocí tlačítek se šipkami ve spodní části stránky.</span><span class="sxs-lookup"><span data-stu-id="c75e3-149">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="c75e3-150">**Naplánovaná instalace** by se měla objevit u řešení s odkazy partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="c75e3-150">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="c75e3-151">Instalace bude trvat 10-15 minut.</span><span class="sxs-lookup"><span data-stu-id="c75e3-151">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="c75e3-152">Po dokončení instalace přejděte zpátky na [Power](https://flow.microsoft.com) automat a vyberte **řešení** z navigační oblasti vlevo.</span><span class="sxs-lookup"><span data-stu-id="c75e3-152">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="c75e3-153">Všimněte si, že v seznamu řešení je k dispozici **synchronizace odkazů partnerského centra pro Dynamics 365** .</span><span class="sxs-lookup"><span data-stu-id="c75e3-153">Notice that **Partner Center Referrals Synchronization for Dynamics 365** is available in the Solutions list.</span></span>

10. <span data-ttu-id="c75e3-154">Vyberte **synchronizaci odkazů partnerského centra pro Dynamics 365** .</span><span class="sxs-lookup"><span data-stu-id="c75e3-154">Select **Partner Center Referrals Synchronization for Dynamics 365** .</span></span> <span data-ttu-id="c75e3-155">K dispozici jsou tyto toky a entity automatizace pro napájení:</span><span class="sxs-lookup"><span data-stu-id="c75e3-155">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Dostupné CRMS":::

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="c75e3-157">Osvědčené postupy: test před zahájením provozu</span><span class="sxs-lookup"><span data-stu-id="c75e3-157">Best practice: test before you go live</span></span>

<span data-ttu-id="c75e3-158">Než nainstalujete, nakonfigurujete a přizpůsobíte řešení Power Automate v produkčním prostředí, ujistěte se, že řešení otestujete v pracovní instanci CRM.</span><span class="sxs-lookup"><span data-stu-id="c75e3-158">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="c75e3-159">Nainstalujte řešení Microsoft Power automatizuje do přípravného prostředí/instance CRM.</span><span class="sxs-lookup"><span data-stu-id="c75e3-159">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="c75e3-160">Vytvořte kopii řešení a spusťte konfiguraci a automatizujte vlastní nastavení toků v přípravném prostředí.</span><span class="sxs-lookup"><span data-stu-id="c75e3-160">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>
- <span data-ttu-id="c75e3-161">Otestujte řešení na pracovní instanci/CRM.</span><span class="sxs-lookup"><span data-stu-id="c75e3-161">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="c75e3-162">Po úspěšném dokončení naimportujte jako spravované řešení do provozní instance.</span><span class="sxs-lookup"><span data-stu-id="c75e3-162">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="c75e3-163">Konfigurace řešení</span><span class="sxs-lookup"><span data-stu-id="c75e3-163">Configure the solution</span></span>

1. <span data-ttu-id="c75e3-164">Po instalaci řešení do instance CRM přejděte zpátky na [Power](https://flow.microsoft.com/)automat.</span><span class="sxs-lookup"><span data-stu-id="c75e3-164">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="c75e3-165">V rozevíracím seznamu **prostředí** v pravém horním rohu vyberte instanci CRM, do které jste nainstalovali řešení Power automatizuje.</span><span class="sxs-lookup"><span data-stu-id="c75e3-165">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="c75e3-166">Budete muset vytvořit připojení, která přiřadí tři uživatelské účty:</span><span class="sxs-lookup"><span data-stu-id="c75e3-166">You'll need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="c75e3-167">Uživatel partnerského centra s přihlašovacími údaji správce odkazů</span><span class="sxs-lookup"><span data-stu-id="c75e3-167">Partner Center user with referrals admin credentials</span></span>

   - <span data-ttu-id="c75e3-168">Události Partnerského centra</span><span class="sxs-lookup"><span data-stu-id="c75e3-168">Partner Center Events</span></span>

   - <span data-ttu-id="c75e3-169">Správce CRM s Power Automate automatizuje v řešení.</span><span class="sxs-lookup"><span data-stu-id="c75e3-169">CRM admin with the Power Automate flows in the solution.</span></span>

      1. <span data-ttu-id="c75e3-170">V levém navigačním panelu vyberte **připojení** a v seznamu vyberte řešení partnerského centra pro partnery.</span><span class="sxs-lookup"><span data-stu-id="c75e3-170">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>

      2. <span data-ttu-id="c75e3-171">Vytvořte připojení kliknutím na **vytvořit připojení** .</span><span class="sxs-lookup"><span data-stu-id="c75e3-171">Create a connection by clicking **Create a connection** .</span></span>

         :::image type="content" source="images/cosellconnectors/createconnection.png" alt-text="Vytvoření připojení":::

      3. <span data-ttu-id="c75e3-173">Na panelu hledání v pravém horním rohu vyhledejte **odkazy na partnerské Centrum (Preview)** .</span><span class="sxs-lookup"><span data-stu-id="c75e3-173">Search for **Partner Center Referrals (preview)** in the search bar on the top-right corner.</span></span>

      4. <span data-ttu-id="c75e3-174">Vytvořte připojení pro uživatele partnerského centra s rolí přihlašovacích údajů správce odkazů.</span><span class="sxs-lookup"><span data-stu-id="c75e3-174">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

      5. <span data-ttu-id="c75e3-175">Potom vytvořte připojení událostí partnerského centra pro uživatele partnerského centra s přihlašovacími údaji správce odkazů.</span><span class="sxs-lookup"><span data-stu-id="c75e3-175">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

      6. <span data-ttu-id="c75e3-176">Vytvořte připojení pro Common Data Service (aktuální prostředí) pro uživatele správce CRM.</span><span class="sxs-lookup"><span data-stu-id="c75e3-176">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

4. <span data-ttu-id="c75e3-177">Pokud chcete přidružit Power Automate k připojením, upravte jednotlivé toky Power automatu pro připojení k Common Data Service a odkazům partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="c75e3-177">To associate the Power Automate flows with the connections, edit each of the Power Automate flows to connect to Common Data Service and Partner Center Referrals.</span></span> <span data-ttu-id="c75e3-178">Uložte změny.</span><span class="sxs-lookup"><span data-stu-id="c75e3-178">Save the changes.</span></span>

5. <span data-ttu-id="c75e3-179">**Zapněte** automatické toky napájení.</span><span class="sxs-lookup"><span data-stu-id="c75e3-179">**Turn on** the Power Automate flows.</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="c75e3-180">Použití rozhraní Webhook API k registraci pro události změny prostředku</span><span class="sxs-lookup"><span data-stu-id="c75e3-180">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="c75e3-181">Rozhraní API Webhooku partnerského centra vám umožní registrovat se na události změny prostředků.</span><span class="sxs-lookup"><span data-stu-id="c75e3-181">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="c75e3-182">Tyto události změny se odesílají na adresu URL jako příspěvky HTTP.</span><span class="sxs-lookup"><span data-stu-id="c75e3-182">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="c75e3-183">Pokud chcete zaregistrovat adresu URL, vyberte možnost **registrace Webhooku partnerského centra (Insider Preview)** Power automatizace.</span><span class="sxs-lookup"><span data-stu-id="c75e3-183">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="c75e3-184">Přidat připojení pro uživatele partnerského centra (a.) s událostmi partnerského centra s přihlašovacími údaji správce (b.), jak je zvýrazněno níže</span><span class="sxs-lookup"><span data-stu-id="c75e3-184">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Trigger":::

3. <span data-ttu-id="c75e3-186">Po provedení těchto aktualizací se zobrazí</span><span class="sxs-lookup"><span data-stu-id="c75e3-186">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooky":::

4. <span data-ttu-id="c75e3-188">Uložte změny a vyberte **zapnout** .</span><span class="sxs-lookup"><span data-stu-id="c75e3-188">Save your changes and select **Turn on** .</span></span>

   <span data-ttu-id="c75e3-189">Pokud chcete, aby Webhooky partnerského centra naslouchali změnám událostí, proveďte následující kroky:</span><span class="sxs-lookup"><span data-stu-id="c75e3-189">To enable Partner Center webhooks to listen to event changes, do the following steps:</span></span>

5. <span data-ttu-id="c75e3-190">Vyberte **Partnerské centrum pro Dynamics 365 (Insider Preview)** .</span><span class="sxs-lookup"><span data-stu-id="c75e3-190">Select **Partner Center to Dynamics 365 (Insider Preview)** .</span></span>

6. <span data-ttu-id="c75e3-191">Vyberte ikonu **Upravit** a vyberte, **kdy se přijme požadavek HTTP** .</span><span class="sxs-lookup"><span data-stu-id="c75e3-191">Select the **Edit** icon and select **When a HTTP request is received** .</span></span>

7. <span data-ttu-id="c75e3-192">Kliknutím na ikonu **kopírování** zkopírujte zadanou adresu URL post protokolu HTTP.</span><span class="sxs-lookup"><span data-stu-id="c75e3-192">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="Zkopírování adresy URL":::

8. <span data-ttu-id="c75e3-194">Nyní vyberte možnost "automatické registrace Webhooku partnerského centra (Insider Preview)" a vyberte **Spustit** .</span><span class="sxs-lookup"><span data-stu-id="c75e3-194">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run** .</span></span>

9. <span data-ttu-id="c75e3-195">Ujistěte se, že se v pravém podokně otevře okno spustit tok a klikněte na **pokračovat** .</span><span class="sxs-lookup"><span data-stu-id="c75e3-195">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue** .</span></span>

10. <span data-ttu-id="c75e3-196">Zadejte následující podrobnosti:</span><span class="sxs-lookup"><span data-stu-id="c75e3-196">Enter the following details:</span></span>

    1. <span data-ttu-id="c75e3-197">**Koncový bod triggeru http** : adresa URL zkopírována z předchozího kroku</span><span class="sxs-lookup"><span data-stu-id="c75e3-197">**Http Trigger Endpoint** : URL copied from earlier step</span></span>

    2. <span data-ttu-id="c75e3-198">**Události k registraci** : odkaz-vytvořeno a odkaz-Aktualizováno</span><span class="sxs-lookup"><span data-stu-id="c75e3-198">**Events to Register** : “referral-created” and “referral-updated”</span></span>

    3. <span data-ttu-id="c75e3-199">**Přepsat existující koncové body triggeru, pokud je k dispozici** : Ano (přepsání všech stávajících koncových bodů)</span><span class="sxs-lookup"><span data-stu-id="c75e3-199">**Overwrite existing trigger endpoints if present** : Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="c75e3-200">Vyberte **Spustit** a potom vyberte **Hotovo.**</span><span class="sxs-lookup"><span data-stu-id="c75e3-200">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="c75e3-201">Webhook teď může naslouchat událostem vytvoření a aktualizace.</span><span class="sxs-lookup"><span data-stu-id="c75e3-201">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="c75e3-202">Přizpůsobení kroků synchronizace</span><span class="sxs-lookup"><span data-stu-id="c75e3-202">Customize synchronization steps</span></span>

<span data-ttu-id="c75e3-203">Pokud jsou odkazy na spoluprodejní synchronizace mezi partnerským centrem a vaším systémem CRM, tady jsou uvedená pole synchronizovaná v počítači partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="c75e3-203">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="c75e3-204">Systémy CRM jsou často vysoce přizpůsobené.</span><span class="sxs-lookup"><span data-stu-id="c75e3-204">Often CRM systems are highly customized.</span></span> <span data-ttu-id="c75e3-205">Můžete přizpůsobit automatické toky Power Automate.</span><span class="sxs-lookup"><span data-stu-id="c75e3-205">You can customize the Power Automate flows.</span></span> <span data-ttu-id="c75e3-206">Postupujte podle pokynů pro mapování polí a v případě potřeby proveďte příslušné změny v postupech automatizace toků.</span><span class="sxs-lookup"><span data-stu-id="c75e3-206">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="c75e3-207">K dispozici jsou mapování partnerských Center Microsoftu na CRM, ale v závislosti na vašem prostředí CRM, můžete zvolit další přizpůsobení polí.</span><span class="sxs-lookup"><span data-stu-id="c75e3-207">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="c75e3-208">V závislosti na vašich potřebách je možné přizpůsobit více kroků každého z těchto toků automatizace napájení.</span><span class="sxs-lookup"><span data-stu-id="c75e3-208">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="c75e3-209">Následují příklady dostupných přizpůsobení:</span><span class="sxs-lookup"><span data-stu-id="c75e3-209">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="c75e3-210">Přizpůsobení polí pro události vytvoření nebo aktualizace v partnerském centru pro synchronizaci odkazů CRM:</span><span class="sxs-lookup"><span data-stu-id="c75e3-210">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="c75e3-211">a.</span><span class="sxs-lookup"><span data-stu-id="c75e3-211">a.</span></span> <span data-ttu-id="c75e3-212">Vyberte partnerské Centrum pro Dynamics 365 (Insider Preview) nebo partnerské Centrum do Salesforce (Insider Preview).</span><span class="sxs-lookup"><span data-stu-id="c75e3-212">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

    <span data-ttu-id="c75e3-213">b.</span><span class="sxs-lookup"><span data-stu-id="c75e3-213">b.</span></span> <span data-ttu-id="c75e3-214">Vyberte **Upravit** a upravte nebo Přizpůsobte tok automatizovaného výkonu.</span><span class="sxs-lookup"><span data-stu-id="c75e3-214">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="c75e3-215">c.</span><span class="sxs-lookup"><span data-stu-id="c75e3-215">c.</span></span> <span data-ttu-id="c75e3-216">Vyberte **(rozsah) synchronizujte zájemce nebo příležitost** .</span><span class="sxs-lookup"><span data-stu-id="c75e3-216">Select **(Scope) Synchronize the lead or opportunity** .</span></span>

2. <span data-ttu-id="c75e3-217">Pokud chcete přizpůsobit mapování polí CRM (na základě Průvodce mapováním polí) pro události vytvořit, vyberte, **jestli je nová sdílená příležitost, a pak** .</span><span class="sxs-lookup"><span data-stu-id="c75e3-217">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then** .</span></span> <span data-ttu-id="c75e3-218">Vyberte dílčí krok, **Pokud ano** , a pak rozbalte **vytvořit novou příležitost v CRM** .</span><span class="sxs-lookup"><span data-stu-id="c75e3-218">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM** .</span></span> <span data-ttu-id="c75e3-219">Mapování v této části můžete upravit pomocí Průvodce mapováním polí.</span><span class="sxs-lookup"><span data-stu-id="c75e3-219">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="c75e3-220">d.</span><span class="sxs-lookup"><span data-stu-id="c75e3-220">d.</span></span> <span data-ttu-id="c75e3-221">Pro přizpůsobení mapování polí CRM (na základě Průvodce mapováním polí) pro události aktualizace klikněte na krok (obor) synchronizovat zájemce nebo příležitost.</span><span class="sxs-lookup"><span data-stu-id="c75e3-221">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="c75e3-222">e.</span><span class="sxs-lookup"><span data-stu-id="c75e3-222">e.</span></span> <span data-ttu-id="c75e3-223">Vyberte **, jestli se jedná o aktualizaci příležitosti, a pak** .</span><span class="sxs-lookup"><span data-stu-id="c75e3-223">Select **If it’s an update to an opportunity, then** .</span></span> <span data-ttu-id="c75e3-224">Vyberte dílčí krok, **Pokud ano** , a pak rozbalte **rozdíl mezi objekty příležitostí v partnerském centru a CRM a pak** .</span><span class="sxs-lookup"><span data-stu-id="c75e3-224">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then** .</span></span>  

    <span data-ttu-id="c75e3-225">f.</span><span class="sxs-lookup"><span data-stu-id="c75e3-225">f.</span></span> <span data-ttu-id="c75e3-226">Vyberte, **jestli ano** , a pak **aktualizovat existující příležitost** .</span><span class="sxs-lookup"><span data-stu-id="c75e3-226">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="c75e3-227">Přizpůsobení polí pro synchronizaci odkazů CRM na počítač pro události aktualizace:</span><span class="sxs-lookup"><span data-stu-id="c75e3-227">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="c75e3-228">a.</span><span class="sxs-lookup"><span data-stu-id="c75e3-228">a.</span></span> <span data-ttu-id="c75e3-229">Vyberte **Upravit**  a upravte nebo Přizpůsobte tok automatizovaného výkonu.</span><span class="sxs-lookup"><span data-stu-id="c75e3-229">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="c75e3-230">b.</span><span class="sxs-lookup"><span data-stu-id="c75e3-230">b.</span></span> <span data-ttu-id="c75e3-231">Vyberte **(rozsah) synchronizace příležitosti** .</span><span class="sxs-lookup"><span data-stu-id="c75e3-231">Select **(Scope) Synchronize the opportunity** .</span></span>

    <span data-ttu-id="c75e3-232">c.</span><span class="sxs-lookup"><span data-stu-id="c75e3-232">c.</span></span> <span data-ttu-id="c75e3-233">Pokud chcete přizpůsobit mapování polí CRM pro události aktualizace, vyberte, **jestli jsou mezi objekty zájemce v partnerském centru a CRM rozdílové rozdíly, a pak** .</span><span class="sxs-lookup"><span data-stu-id="c75e3-233">To customize CRM field mappings for update events, select **If there is difference between the lead objects in Partner Center and CRM, then** .</span></span> 

    <span data-ttu-id="c75e3-234">d.</span><span class="sxs-lookup"><span data-stu-id="c75e3-234">d.</span></span> <span data-ttu-id="c75e3-235">Vyberte dílčí krok, **Pokud ano** , a pak rozbalte krok **aktualizace odkazu s daty příležitostí** .</span><span class="sxs-lookup"><span data-stu-id="c75e3-235">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data** .</span></span>

   <span data-ttu-id="c75e3-236">Mapování v této části můžete upravit v závislosti na průvodci mapováním polí.</span><span class="sxs-lookup"><span data-stu-id="c75e3-236">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="c75e3-237">Chcete-li přizpůsobit pole pro synchronizaci odkazů CRM na počítač pro vytvoření událostí?</span><span class="sxs-lookup"><span data-stu-id="c75e3-237">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="c75e3-238">a.</span><span class="sxs-lookup"><span data-stu-id="c75e3-238">a.</span></span> <span data-ttu-id="c75e3-239">Vyberte **Upravit**  a upravte nebo Přizpůsobte tok automatizovaného výkonu.</span><span class="sxs-lookup"><span data-stu-id="c75e3-239">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="c75e3-240">b.</span><span class="sxs-lookup"><span data-stu-id="c75e3-240">b.</span></span> <span data-ttu-id="c75e3-241">Výběr **(rozsah) synchronizace odkazů.**</span><span class="sxs-lookup"><span data-stu-id="c75e3-241">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="c75e3-242">c.</span><span class="sxs-lookup"><span data-stu-id="c75e3-242">c.</span></span> <span data-ttu-id="c75e3-243">Pokud chcete přizpůsobit mapování polí CRM (na základě Průvodce mapováním polí) pro události vytvořit, vyberte **vytvořit odkaz Microsoftu** .</span><span class="sxs-lookup"><span data-stu-id="c75e3-243">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral** .</span></span>

   <span data-ttu-id="c75e3-244">Mapování v této části můžete upravit v závislosti na průvodci mapováním polí.</span><span class="sxs-lookup"><span data-stu-id="c75e3-244">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="c75e3-245">Komplexní Obousměrná synchronizace odkazů v rámci společného prodeje</span><span class="sxs-lookup"><span data-stu-id="c75e3-245">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="c75e3-246">Jakmile nainstalujete, nakonfigurujete a přizpůsobíte řešení Power Automate, můžete otestovat synchronizaci odkazů mezi produkty Dynamics 365 a Partnerským centrem společně prodávat.</span><span class="sxs-lookup"><span data-stu-id="c75e3-246">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="c75e3-247">Požadavky</span><span class="sxs-lookup"><span data-stu-id="c75e3-247">Pre-requisites</span></span>

<span data-ttu-id="c75e3-248">Aby bylo možné synchronizovat odkazy v rámci partnerského centra a Dynamics 365 CRM, řešení Power automat jasně vymezuje pole odkazů specifická pro společnost Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c75e3-248">To synchronize the referrals across Partner Center and Dynamics 365 CRM, the Power Automate solution clearly demarcates Microsoft-specific referral fields.</span></span> <span data-ttu-id="c75e3-249">Tato identifikace dává prodejcům možnost rozhodnout se, které odkazy chce sdílet se společností Microsoft pro souběžný prodej.</span><span class="sxs-lookup"><span data-stu-id="c75e3-249">This identification gives your seller teams  the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="c75e3-250">Sada vlastních polí je k dispozici jako součást entity **příležitosti** .</span><span class="sxs-lookup"><span data-stu-id="c75e3-250">A set of custom fields is available as part of the **Opportunity** entity.</span></span> <span data-ttu-id="c75e3-251">Uživatel s oprávněními správce CRM bude muset vytvořit samostatný oddíl CRM s vlastními poli **příležitosti** .</span><span class="sxs-lookup"><span data-stu-id="c75e3-251">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="c75e3-252">Následující vlastní pole by měla být součástí části CRM:</span><span class="sxs-lookup"><span data-stu-id="c75e3-252">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="c75e3-253">**Synchronizovat s partnerským centrem** : jestli se má synchronizovat příležitost s partnerským centrem Microsoftu</span><span class="sxs-lookup"><span data-stu-id="c75e3-253">**Sync with Partner Center** : Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="c75e3-254">**Identifikátor odkazu** : pole identifikátoru jen pro čtení pro odkaz na partnerského centra Microsoftu</span><span class="sxs-lookup"><span data-stu-id="c75e3-254">**Referral Identifier** : A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="c75e3-255">**Odkaz** odkazu: odkaz na odkaz určený jen pro čtení v partnerském centru Microsoftu</span><span class="sxs-lookup"><span data-stu-id="c75e3-255">**Referral Link** : A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="c75e3-256">**Jak může společnost Microsoft** získat nápovědu? od Microsoftu se dozvíte, jak tento odkaz vyžaduje.</span><span class="sxs-lookup"><span data-stu-id="c75e3-256">**How can Microsoft help?** : Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="c75e3-257">**Produkty** : seznam produktů přidružených k této příležitosti</span><span class="sxs-lookup"><span data-stu-id="c75e3-257">**Products** : List of products associated with this opportunity</span></span>

- <span data-ttu-id="c75e3-258">**Audit** : záznam auditu jen pro čtení pro synchronizaci s odkazy partnerského centra</span><span class="sxs-lookup"><span data-stu-id="c75e3-258">**Audit** : A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="c75e3-259">ŘEŠENÍ</span><span class="sxs-lookup"><span data-stu-id="c75e3-259">SCENARIOS:</span></span>

1. <span data-ttu-id="c75e3-260">Referenční synchronizace při vytvoření nebo aktualizaci odkazu v CRM a synchronizovaných v partnerském centru:</span><span class="sxs-lookup"><span data-stu-id="c75e3-260">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="c75e3-261">Přihlaste se k prostředí Dynamics 365 CRM s uživatelem, který má v části **příležitost** v aplikaci CRM přehled.</span><span class="sxs-lookup"><span data-stu-id="c75e3-261">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="c75e3-262">Při vytváření nové příležitosti v prostředí Dynamics 365 se ujistěte, že je k dispozici následující oddíl.</span><span class="sxs-lookup"><span data-stu-id="c75e3-262">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="Část s ukázkou příležitostí zobrazující informace o partnerském centru Microsoftu v Dynamics 365.":::

   3. <span data-ttu-id="c75e3-264">Pokud chcete tuto příležitost synchronizovat s partnerským centrem Microsoftu, ujistěte se, že jste v zobrazení karta nastavili následující pole:</span><span class="sxs-lookup"><span data-stu-id="c75e3-264">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="c75e3-265">**Synchronizovat s partnerským centrem** : Ano</span><span class="sxs-lookup"><span data-stu-id="c75e3-265">**Sync with Partner Center** : Yes</span></span>

      - <span data-ttu-id="c75e3-266">**Jak může Microsoft pomáhat?** : vyberte z těchto možností:</span><span class="sxs-lookup"><span data-stu-id="c75e3-266">**How can Microsoft help?** : Select from the following:</span></span>

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="Oddíl ukázkové příležitosti v Dynamics 365, který zobrazuje možnosti pomocníka pro partnerské Centrum Microsoftu vedle pole s názvem Jak může pomáhat Microsoft?":::

      - <span data-ttu-id="c75e3-268">**Produkty** : ID řešení produktu</span><span class="sxs-lookup"><span data-stu-id="c75e3-268">**Products** : Solution IDs of the product</span></span>

   4. <span data-ttu-id="c75e3-269">Až se příležitost vytvoří v Dynamics 365 s možností **synchronizovat s partnerským centrem** nastavenou na **Ano** , počkejte 10 minut a pak se přihlaste k účtu partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="c75e3-269">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes** , wait 10 minutes, and then sign into your Partner Center account.</span></span> <span data-ttu-id="c75e3-270">Vaše odkazy budou synchronizovány s Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="c75e3-270">Your referrals will be synchronized with Dynamics 365.</span></span>

   5. <span data-ttu-id="c75e3-271">Podobně platí, že pokud chcete příležitost, která má možnost synchronizovat s partnerským centrem nastavenou na hodnotu Ano, aktualizovat příležitost v Dynamics 365 CRM, změny se synchronizují v účtu partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="c75e3-271">Likewise, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

   6. <span data-ttu-id="c75e3-272">Příležitosti, které byly úspěšně synchronizovány s partnerským centrem, budou označeny ikonou ✔ v Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="c75e3-272">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="c75e3-273">Referenční synchronizace při vytvoření nebo aktualizaci odkazu v partnerském centru Microsoftu a synchronizovaných v prostředí Dynamics 365:</span><span class="sxs-lookup"><span data-stu-id="c75e3-273">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="c75e3-274">Přihlaste se k [řídicímu panelu](https://partner.microsoft.com/dashboard/home)partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="c75e3-274">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   2. <span data-ttu-id="c75e3-275">V nabídce na levé straně vyberte **odkazy** .</span><span class="sxs-lookup"><span data-stu-id="c75e3-275">Select **Referrals** from the left-hand menu.</span></span>

   3. <span data-ttu-id="c75e3-276">Klikněte na možnost Nová práce a vytvořte si nový odkaz na společný prodej z partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="c75e3-276">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

   4. <span data-ttu-id="c75e3-277">Přihlaste se k prostředí Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="c75e3-277">Sign into your Dynamics 365 CRM environment.</span></span>

   5. <span data-ttu-id="c75e3-278">Přejděte na **otevřené příležitosti** .</span><span class="sxs-lookup"><span data-stu-id="c75e3-278">Navigate to **Open Opportunities** .</span></span> <span data-ttu-id="c75e3-279">Odkaz vytvořený v partnerském centru Microsoftu je teď synchronizovaný v Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="c75e3-279">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   6. <span data-ttu-id="c75e3-280">Když vyberete synchronizovaný odkaz, vyplní se podrobnosti zobrazení karty.</span><span class="sxs-lookup"><span data-stu-id="c75e3-280">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c75e3-281">Další kroky</span><span class="sxs-lookup"><span data-stu-id="c75e3-281">Next steps</span></span>

- [<span data-ttu-id="c75e3-282">Správa potenciálních zákazníků</span><span class="sxs-lookup"><span data-stu-id="c75e3-282">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="c75e3-283">Správa příležitostí ke spoluprodeji</span><span class="sxs-lookup"><span data-stu-id="c75e3-283">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="c75e3-284">Další informace o platformě Microsoft Power automatizuje?</span><span class="sxs-lookup"><span data-stu-id="c75e3-284">More about Microsoft Power Automate platform?</span></span>](/power-automate/)

- [<span data-ttu-id="c75e3-285">Webhooky partnerského centra</span><span class="sxs-lookup"><span data-stu-id="c75e3-285">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)