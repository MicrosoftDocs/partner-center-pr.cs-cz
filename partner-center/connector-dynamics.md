---
title: Konektor pro spoluprodeji pro partnerské Centrum Dynamics 365 CRM
description: Synchronizujte odkazy v partnerském centru s konektorem pro spoluprodeji pro Dynamics 365 CRM. V rámci vašeho systému CRM pak můžete společně prodávat pomocí Microsoftu.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 03/01/2021
ms.openlocfilehash: c399e00394208ec29dd59a41afe7cce1b1d07253
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284328"
---
# <a name="co-sell-connector-for-dynamics-365-crm-overview"></a>Přehled konektoru pro Dynamics 365 CRM pro předprodej

**Příslušné role**

- Správce odkazů
- Správce systému nebo úpravce systému v CRM

Konektory pro spoluprodej v partnerském centru umožňují prodejcům v rámci svých systémů CRM společný prodej s Microsoftem. Nebudou se muset vyškolet k používání partnerského centra ke správě obchodů v rámci společného prodeje. Pomocí konektorů pro spoluprodeji můžete vytvořit nový společný odkaz k účasti na prodejci Microsoftu, přijímat odkazy od prodejce Microsoftu, přijímat nebo odmítat odkazy a upravovat data týkající se obchodu, jako je hodnota kouposti a datum uzavření. K těmto obchodům v rámci těchto spoluprodejů můžete také dostávat jakékoli aktualizace od prodejců Microsoftu. Všechny vaše odkazy můžete spravovat v CRM dle vašeho výběru, nikoli v partnerském centru.

Řešení je založené na automatizaci Power and používá rozhraní API partnerského centra.

## <a name="prerequisites"></a>Požadavky

Před instalací řešení se ujistěte, že splňujete následující požadavky.

|**Témata**   |**Podrobnosti**   |**Odkazy**   |
|--------------|--------------------|------|
|ID Microsoft Partner Network (MPN) |Potřebujete platné ID MPN.|[Připojte se k partnerské síti](https://partner.microsoft.com/)|
|Připravený společný prodej|Vaše řešení IP/Services musí být připravené k prodeji.|[Prodej pomocí Microsoftu](https://partner.microsoft.com/membership/sell-with-microsoft)|
|Účet partnerského centra|ID MPN přidružené k tenantovi partnerského centra musí být stejné jako ID MPN přidružené k vašemu řešení společného prodeje. Než konektory nasadíte, ověřte, že se vám na portálu partnerského centra zobrazuje odkaz na společný prodej.|[Správa vašeho účtu](create-user-accounts-and-set-permissions.md)|
|Role uživatelů partnerského centra|Zaměstnanec, který bude instalovat a používat konektory, musí být správce odkazů.|[Přiřazování uživatelských rolí a oprávnění](create-user-accounts-and-set-permissions.md)|
|Dynamics 365 CRM|Uživatelská role CRM je správce systému nebo úpravce systému.|[Přiřazení rolí v Dynamics 365](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Zapnout účet toku automatizace|Vytvořte nové provozní prostředí s databází pro testování, přípravu a produkci. Máte-li existující provozní prostředí s databází, je možné jej znovu použít. Uživatel, který chce nainstalovat řešení konektoru, musí mít licenci Power automatizující a přístup k tomuto prostředí. V případě neúspěchu instalace můžete monitorovat průběh a získat další informace v [Power](https://flow.microsoft.com/) automatu. V části **řešení** vyberte **Zobrazit historii** .|[Vytvořit nebo spravovat prostředí](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Nainstalovat synchronizaci odkazů partnerského centra pro Dynamics 365 (řešení Power automat)

1. V pravém horním rohu přejdete na [Power](https://flow.microsoft.com)Automata a vyberte **prostředí** . Tento krok vám ukáže dostupné instance CRM.

1. V rozevíracím seznamu v pravém horním rohu vyberte příslušnou instanci CRM.

1. Vyberte **řešení** na levé straně.

1. V horní nabídce vyberte odkaz **otevřít AppSource** .

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Snímek obrazovky, který zobrazuje otevřený AppSource.":::

1. V místní obrazovce vyhledejte **konektory odkazů partnerského centra pro Dynamics 365** .  

1. Vyberte tlačítko **získat nyní** a pak vyberte **pokračovat**.

1. Zobrazí se stránka, kde můžete vybrat prostředí CRM (Dynamics 365) a nainstalovat aplikaci. Vyjádřit souhlas s podmínkami a ujednáními.

1. Můžete monitorovat průběh a pokud se instalace nepovede, můžete získat další podrobnosti v tématu automatizace, a to výběrem možnosti **Zobrazit historii** v části **řešení**.

1. Po dokončení instalace se vraťte k [Power](https://flow.microsoft.com) automatu a vyberte **řešení** na levé straně. V seznamu **řešení** je teď dostupná **synchronizace odkazů partnerského centra pro Dynamics 365** .

1. Vyberte **synchronizaci odkazů partnerského centra pro Dynamics 365**. K dispozici jsou následující toky a možnosti automatizace napájení.

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Snímek obrazovky, který zobrazuje dostupné CRMs.":::

## <a name="test-before-you-go-live"></a>Před přechodem do provozu proveďte test.

Než nainstalujete, nakonfigurujete a přizpůsobíte řešení Power Automate v produkčním prostředí, ujistěte se, že řešení otestujete v pracovní instanci CRM. Budete potřebovat:

- Nainstalujte řešení Power Automate do přípravného prostředí CRM instance.
- Nakonfigurujte a upravte řešení Power Automate v přípravném prostředí.
- Otestujte řešení na pracovní instanci CRM.
- Po úspěšném testu ho importujte jako spravované řešení do produkční instance.

## <a name="configure-the-solution"></a>Konfigurace řešení

1. Po instalaci řešení do instance CRM se vraťte k [Power](https://flow.microsoft.com/)automatu.

1. V rozevíracím seznamu **prostředí** v pravém horním rohu vyberte instanci CRM, do které jste nainstalovali řešení Power automatizuje.

1. Budete muset vytvořit připojení, která přiřadí tři uživatelské účty:

   - Uživatel partnerského centra s přihlašovacími údaji správce odkazů
   - Události Partnerského centra
   - Správce CRM s automatickým automatizací toků v řešení

   1. Na levé straně vyberte **připojení** a v seznamu vyberte řešení **partnerského centra s odkazy** .

   1. Vytvořte připojení výběrem možnosti **vytvořit připojení**.

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Snímek obrazovky, který ukazuje vytvoření připojení.":::

   1. Na panelu hledání v pravém horním rohu vyhledejte **odkazy na partnerské Centrum (Preview)** .

   1. Vytvořte připojení pro uživatele partnerského centra s rolí přihlašovacích údajů správce odkazů.

   1. Potom vytvořte připojení událostí partnerského centra pro uživatele partnerského centra s přihlašovacími údaji správce odkazů.

   1. Vytvořte připojení pro Common Data Service (aktuální prostředí) pro uživatele správce CRM.
     
   1. Po přidání všech připojení byste měli ve svém prostředí zobrazit následující připojení.

      :::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="Snímek obrazovky, který zobrazuje připojení":::

## <a name="edit-the-connections"></a>Upravit připojení

1. Vraťte se na stránku **řešení** a vyberte **výchozí řešení**. Vyberte možnost **odkaz na připojení (Preview)** tím, že vyberete **vše**.

   :::image type="content" source="images/connection-reference-video.gif" alt-text="Snímek obrazovky, který zobrazuje úpravu připojení.":::

1. Jednotlivá připojení upravte jednotlivě výběrem ikony se třemi tečkami. Přidejte příslušná připojení.

   :::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="Snímek obrazovky zobrazující uvedená připojení":::

1.  Vraťte se na stránku **řešení** , vyberte **synchronizace odkazů partnerského centra pro Dynamics 365** a potom tok zapněte výběrem ikony se třemi tečkami vedle každého toku v následujícím pořadí. Pokud narazíte na problémy při zapnutí toku, Projděte si téma [Postup přizpůsobení](connector-dynamics.md#customize-synchronization-steps) a [Postup řešení potíží](connectors-troubleshoot.md).

Zapněte toky v následujícím pořadí:

- Registrace Webhooku partnerského centra (Insider Preview)
- Vytvoření odkazu na společný prodej – Dynamics 365 do partnerského centra (Insider Preview)
- Přizpůsobit Vytvoření nebo získání podrobností z toku Dynamics 365
- Partnerské centrum pro Dynamics 365 – pomocníka (Insider Preview)
- Partnerské centrum pro spoluprodejní aktualizace pro Microsoft Dynamics 365 (Insider Preview)
- Partnerské centrum k Dynamics 365 (Insider Preview)
- Dynamics 365 do partnerského centra (Insider Preview)
- Příležitost Dynamics 365 do partnerského centra (Insider Preview)
- Řešení Microsoft Dynamics 365 od Microsoftu do partnerského centra (Insider Preview)
 
## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Použití rozhraní Webhook API k registraci pro události změny prostředku

K registraci událostí změn prostředků můžete použít rozhraní API Webhooku partnerského centra. Tyto události změny se odesílají na adresu URL jako příspěvky HTTP.

1. Vyberte **Partnerské centrum pro Dynamics 365 (Insider Preview)**.

1. Vyberte ikonu **Upravit** a vyberte, **kdy se přijme požadavek HTTP**.

1. Kliknutím na ikonu **kopírování** zkopírujte zadanou adresu URL post protokolu HTTP.

   :::image type="content" source="images/webhook-video.gif" alt-text="Snímek obrazovky, který ukazuje použití webhooků k registraci změn prostředků.":::

1. Vyberte možnost **registrace Webhooku partnerského centra (Insider Preview)** automatizace a pak vyberte **Spustit**.

1. Ujistěte se, že se v pravém podokně otevře okno **tok spuštění** , a vyberte **pokračovat**.

1. Zadejte následující podrobnosti:

   - **Koncový bod triggeru http**: Tato adresa URL byla zkopírována z předchozího kroku.
   - **Události, které se mají zaregistrovat**: vyberte všechny dostupné události (**odkaz – vytvořeno**, **odkazový – Aktualizováno**, **související-referenční – vytvořeno** a **související-referenční – Aktualizováno**).
   - **Přepsat existující koncové body triggeru, pokud je k dispozici?**: Ano. Pro danou událost Webhooku se dá zaregistrovat jenom jedna adresa URL.

1. Vyberte **Spustit tok** a potom vyberte **Hotovo.**

Webhook teď může naslouchat, vytvářet a aktualizovat události.

## <a name="customize-synchronization-steps"></a>Přizpůsobení kroků synchronizace

Systémy CRM jsou vysoce přizpůsobené a můžete upravit řešení Power automat na základě nastavení aplikace CRM. V případě, že se pro spoluprodejní odkazy mezi partnerským centrem a vaším systémem CRM synchronizují, jsou pole, která jsou synchronizovaná v počítači partnerského centra, uvedená v [Průvodci mapováním vlastních polí](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S).

Postupujte podle pokynů pro mapování polí a v případě potřeby proveďte příslušné změny v **[přizpůsobení] vytvoření nebo získání podrobností z toku** nebo proměnných prostředí Dynamics 365. Neaktualizujte žádné další toky v řešení Power automat, protože může ovlivnit budoucí upgrady řešení.

K dispozici jsou následující vlastní nastavení:

- **Zobrazit zaškrtnutí v názvu příležitosti**: ve výchozím nastavení se vedle názvu příležitosti zobrazí značka zaškrtnutí, která značí, že synchronizace mezi partnerským centrem a Dynamics 365 CRM proběhne úspěšně. Podobně se zobrazí křížové značky, pokud se synchronizace nezdaří. Chcete-li se vyhnout přidání zaškrtnutí nebo křížového označení v názvu příležitosti, nastavte aktuální hodnotu **značky zaškrtnutí v proměnné prostředí název příležitosti** na hodnotu ne.
- **Hodnota koupě**: ve výchozím nastavení se hodnota koupě z partnerského centra synchronizuje do a z **estimatedvalue** v CRM. Pokud v aplikaci CRM máte jiné pole pro hodnotu obchodu, ze které se má synchronizovat:

  - Aktualizujte název pole **hodnoty obchodu** v proměnné prostředí Dynamics 365 s názvem pole CRM. Ujistěte se, že zadáváte název pole, nikoli jeho zobrazované jméno.
  - Upravit **[přizpůsobení] vytvořit nebo získat podrobnosti z toku Dynamics 365** a přejít na **vytvořit nebo aktualizovat příležitost** v CRM a aktualizovat **vytvořit novou příležitost** a **aktualizovat existující akce příležitostí** a přiřadit hodnotu **DealValue** ke správnému poli v CRM. Odeberte také přiřazení **DealValue** z pole **Odhadované výnosy** .

- **Kód země zákazníka**: je nutné při vytváření nového odkazu zadat dvoumístné číslo země (ISO 3166). Ve výchozím nastavení se kód země synchronizuje s polem **address1_country** účtu v CRM. Pokud v CRM máte jiné pole pro kód země, ze kterého se má provést synchronizace:

   - Pole kód země v nevyhledávání v účtu, který obsahuje kód se dvěma písmeny:
     - Aktualizujte název pole **kód země země zákazníka** v proměnné prostředí Dynamics 365 s názvem pole CRM. Ujistěte se, že zadáváte název pole, nikoli jeho zobrazované jméno.
     - Upravte **[vlastní] Vytvořte nebo Získejte podrobnosti z toku Dynamics 365** a v akci CRM **vytvořte nebo Získejte účet zákazníka** , abyste přiřadili hodnotu **země** ke správnému poli v CRM. Také odeberte přiřazení hodnoty **země** z pole **Adresa 1: země/oblast** .

   - Pro pole kód země na základě vyhledávání v účtu:
     - Přidejte do účtu nové vlastní pole a automaticky ho vyplníte kódem země (ISO 3166) na základě hodnoty vybrané v poli vyhledávání a naopak.
     - Pomocí předchozích kroků v poli kód země nevyhledávání proveďte synchronizaci nového vlastního pole z CRM do a z partnerského centra.

- **Pole příležitostí**: Pokud jsou v **příležitosti** povinná pole, která je potřeba naplnit, upravte **[přizpůsobení] vytvořit nebo získat podrobnosti z toku Dynamics 365** a v části **Vytvoření nebo aktualizace příležitosti** přiřaďte hodnoty do povinných **polí na základě** vašich obchodních požadavků.
- **Pole zájemců**: Pokud existují povinná pole v rámci **zájemce** , která musí být naplněna, upravte **[přizpůsobení] vytvořit nebo získat podrobnosti z toku Dynamics 365** a v části **Vytvoření nebo aktualizace zájemce** přiřaďte hodnoty do povinných **polí na základě** vašich obchodních požadavků.
- **Účet zákazníka**: když je nový odkaz synchronizovaný z partnerského centra do CRM, pokusí se řešení Power Automate vyhledat existující účet v CRM pomocí názvu společnosti zákazníka a poštovního směrovacího čísla. Pokud se jeden z nich nenajde, vytvoří se v CRM nový účet zákazníka. Pokud chcete aktualizovat kritéria hledání a podrobnosti vytváření nového účtu, upravte **[přizpůsobení] vytvořit nebo získat podrobnosti z toku Dynamics 365** a v části **Vytvoření nebo získání účtu zákazníka** v akci CRM a **vytvořit účet zákazníka** klikněte na vytvořit nebo získat účet zákazníka.

## <a name="update-environment-variable"></a>Aktualizovat proměnnou prostředí

Aktualizace hodnoty proměnné prostředí:

1. Přejít na stránku **řešení** a vyberte **výchozí řešení**. Výběrem možnosti **vše** vyberte **proměnnou prostředí** .

1. Vyberte proměnnou prostředí pro hodnotu, kterou je třeba aktualizovat, a vyberte **Upravit** pomocí ikony tří teček.

1. Aktualizuje **aktuální hodnotu** (neaktualizuje **výchozí hodnotu**) pomocí možnosti **Nová hodnota** a zadáním hodnoty. Hodnota se musí shodovat s datovým typem proměnné. Například datový typ Ano nebo ne bude akceptovat hodnotu Ano nebo ne.

   :::image type="content" source="images/environment-variables-video.gif" alt-text="Snímek obrazovky, který zobrazuje aktualizace proměnných prostředí.":::

## <a name="end-to-end-bidirectional-co-sell-referral-synchronization"></a>Ucelená referenční synchronizace pro souběžný obchod s obousměrným prodejem

Po instalaci, konfiguraci a přizpůsobení řešení Power Automate můžete testovat synchronizaci odkazů mezi produkty Dynamics 365 a Partnerským centrem společně prodávat.

### <a name="prerequisites"></a>Požadavky

Aby bylo možné synchronizovat odkazy v rámci partnerského centra a Dynamics 365 CRM, řešení Power automat jasně vymezuje pole odkazů specifická pro společnost Microsoft. Tato identifikace dává prodejcům možnost rozhodnout se, které odkazy chce sdílet se společností Microsoft pro souběžný prodej.

Sada vlastních polí a objektů bude přidána jako součást instalace řešení. Uživatel s oprávněními správce CRM bude muset vytvořit samostatný oddíl CRM s vlastními poli **příležitosti** .

Následující vlastní pole by měla být součástí části CRM:

- **Synchronizovat s partnerským centrem**: Určuje, jestli se má tato příležitost synchronizovat s partnerským centrem. Ve výchozím nastavení je hodnota tohoto pole ne a musí být explicitně nastavená na Ano, aby mohl váš prodejce sdílet příležitost s Microsoftem. Nové odkazy sdílené z partnerského centra do CRM budou mít tuto hodnotu pole nastavenou na Ano.
- **Identifikátor odkazu**: pole identifikátoru jen pro čtení pro odkaz na partnerského centra.
- **Odkaz** odkazu: odkaz na odkaz v partnerském centru určený jen pro čtení.
- **Jak může společnost Microsoft** získat nápovědu? od Microsoftu se dozvíte, jak odkaz požaduje. Pokud chcete vytvořit odkaz pro spoluprodejní, vyberte požadovanou povinnou podporu od Microsoftu. Aby bylo možné vytvořit odkaz pro společný prodej, musí být přidružen k příležitosti kontakt zákazníka. Pokud chcete vytvořit odkaz bez účasti na prodeji, toto pole nevybírejte. Odkaz na nesouvisející prodej se dá kdykoli převést na odkaz na společný prodej tím, že vyberete příslušnou možnost povinnou pro podporu.
- **Viditelnost odkazů z partnerského centra Microsoftu**: vyberte viditelnost pro odkaz na partnerského centra. Když je zpřístupníte prodejcům Microsoftu, odkaz na nesouvisející prodej se může převést na společný prodej. Když se vyžaduje Microsoft Help, odkaz je ve výchozím nastavení viditelný pro prodejce Microsoftu. Po označení tohoto pole jako viditelné ho nelze vrátit zpět.
- **Identifikátor Microsoft CRM**: když společnost Microsoft vytvoří a přijme odkaz na společný prodej, toto pole se vyplní identifikátorem CRM společnosti Microsoft.
- **Produkty: zastaralé**: Nepoužívejte toto pole ani ho přidejte do oddílu CRM. Je k dispozici pouze pro zpětnou kompatibilitu. Místo toho použijte řešení partnerského centra.
- **Audit**: záznam auditu jen pro čtení pro synchronizaci s odkazy partnerského centra.
- **Řešení partnerského centra Microsoftu**: vlastní objekt pro přidružení řešení připraveného k prodeji nebo řešení Microsoftu s příležitostí. Z příležitosti můžete přidat nebo odebrat jedno nebo více řešení. Před tím, než ho budete moct sdílet s Microsoftem, je nutné přidat alespoň jeden vlastní prodej nebo řešení společnosti Microsoft. Pokud chcete tento objekt přidružit k příležitosti, aktualizujte formulář **příležitosti** v CRM.

  Vyberte příslušnou kartu na formuláři **příležitosti** a přidejte dílčí mřížku, jak je znázorněno zde.

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="Snímek obrazovky, který zobrazuje formulář s příležitostí":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="Snímek obrazovky, který zobrazuje řešení Microsoftu.":::

- Po přidání řešení Microsoftu můžete předem naplnit podrobnosti o řešení připraveného pro prodej, aby je prodejci nemuseli přidávat. Chcete-li přidat nové podrobnosti o řešení, v aplikaci CRM otevřete objekt podrobnosti řešení společnosti Microsoft a vyberte možnost **Přidat záznam** a přidejte jednu položku, nebo použijte možnost **Odeslat do aplikace Excel** k přidání více položek.

  :::image type="content" source="images/dynamic-1a.png" alt-text="Snímek obrazovky, který ukazuje nové podrobnosti o řešení Microsoftu.":::

### <a name="scenarios"></a>Scénáře

1. Referenční synchronizace při vytvoření nebo aktualizaci odkazu v CRM a synchronizovaných v partnerském centru:

   1. Přihlaste se do prostředí Dynamics 365 CRM s uživatelem, který má v části **příležitost** v aplikaci CRM přehled.

   1. Při vytváření nové příležitosti v prostředí Dynamics 365 se ujistěte, že se nachází oddíl **partnerského centra Microsoftu** .

      :::image type="content" source="images/dynamic-2a.png" alt-text="Snímek obrazovky, který zobrazuje novou příležitost":::

   1. Pokud chcete tuto příležitost synchronizovat s partnerským centrem, ujistěte se, že jste v zobrazení karta nastavili následující pole:

      - **Jak může pomáhat Microsoft?**: Chcete-li vytvořit doplňující odkaz, vyberte příslušnou možnost Help.

         :::image type="content" source="images/dynamic-3a.png" alt-text="Snímek obrazovky, který ukazuje, jak získat příslušná pole v zobrazení karta.":::

      - **Kontakt zákazníka**: Chcete-li vytvořit odkaz pro spoluprodej, přidejte k příležitosti kontakt zákazníka.
      - **Synchronizovat s partnerským centrem**: Ano.
      - **Řešení Microsoftu**: Chcete-li sdílet odkaz s Microsoftem, přidejte k příležitosti platné řešení připravené k spoluprodeji nebo Microsoftu.
      
        :::image type="content" source="images/dynamic-4a.png" alt-text="Snímek obrazovky zobrazující ID řešení":::

   1. Po vytvoření příležitosti v Dynamics 365 s možností **synchronizovat s partnerským centrem** nastavenou na Ano počkejte 10 minut. Pak se přihlaste k účtu partnerského centra. Vaše odkazy budou synchronizovány s Dynamics 365 a **identifikátorem odkazu**. **Odkaz na odkaz** se vyplní. Pokud dojde k selhání, pole **auditu** se naplní informacemi o chybě.
     
    1. Podobně platí, že u příležitosti s možností **synchronizovat s partnerským centrem** nastavenou na Ano platí, že pokud aktualizujete příležitost v Dynamics 365 CRM, změny se synchronizují v účtu partnerského centra.

    1. Příležitosti, které byly úspěšně synchronizovány s partnerským centrem, budou označeny ikonou ✔ v Dynamics 365.

1. Referenční synchronizace při vytvoření nebo aktualizaci odkazu v partnerském centru a synchronizovaná v prostředí Dynamics 365:

   1. Přihlaste se k [řídicímu panelu](https://partner.microsoft.com/dashboard/home)partnerského centra.

   1. V nabídce vlevo vyberte **odkaz** .

   1. Vytvořte si nový odkaz na společný prodej z partnerského centra tím, že vyberete **novou možnost koupě** .

   1. Přihlaste se k prostředí Dynamics 365 CRM.

   1. Přejít na **otevřené příležitosti**. Odkaz vytvořený v partnerském centru se teď synchronizuje v Dynamics 365 CRM.

   1. Když vyberete synchronizovaný odkaz, vyplní se podrobnosti zobrazení karty.

## <a name="next-steps"></a>Další kroky

- [Správa potenciálních zákazníků](manage-leads.md)
- [Správa příležitostí ke spoluprodeji](manage-co-sell-opportunities.md)
- [Další informace o platformě Microsoft Power automatizaci](/power-automate/)
- [Webhooky Partnerského centra](/partner-center/develop/partner-center-webhooks)
