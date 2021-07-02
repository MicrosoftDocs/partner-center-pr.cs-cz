---
title: Konektor pro spoluprodejní účast v partnerském centru pro Salesforce CRM
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Synchronizujte své odkazy v partnerském centru se službou Salesforce CRM. Prodejci pak můžou v rámci svých systémů CRM prodávat společně s Microsoftem.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 06/28/2021
ms.openlocfilehash: 726e9071347e1590885b4bf82676f7767311f945
ms.sourcegitcommit: c4601069340445135b551fa96bee6d9923d8aa97
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/01/2021
ms.locfileid: "113173677"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Konektor pro společný prodej pro Salesforce CRM – přehled

**Příslušné role**: Správce odkazů | Správce systému nebo úpravce systému v CRM

Konektor pro spoluprodej v partnerském centru umožňuje prodejcům v rámci svých systémů CRM spolupracovat s Microsoftem. Nebudou se muset vyškolet k používání partnerského centra ke správě obchodů v rámci společného prodeje. Pomocí konektorů pro spoluprodeji můžete vytvořit nový společný prodejní odkaz, který bude kontaktovat prodejce Microsoftu, získat referenční údaje od prodejce Microsoftu, přijmout nebo odmítnout reference, upravit data o koupi, jako je třeba hodnota koupě a datum ukončení.  K těmto obchodům v rámci těchto spoluprodejů můžete také dostávat jakékoli aktualizace od prodejců Microsoftu. Všechny vaše odkazy fungují při práci v aplikaci CRM dle vašeho výběru a nikoli v partnerském centru.

řešení je založené na řešení Microsoft Power Automate a používá rozhraní api partnerského centra.

## <a name="before-you-install---pre-requisites"></a>Před instalací – požadavky

|**Témata**|**Podrobnosti**|**Odkazy**|
|--------------|--------------------|------|
|ID Microsoft Partner Network |Potřebujete platné ID MPN.|Připojení k programu [MPN](https://partner.microsoft.com/)|
|Připravený společný prodej|Vaše řešení IP/Services musí být připravené k prodeji.|[Prodej pomocí Microsoftu](https://partner.microsoft.com/membership/sell-with-microsoft)|
|Účet partnerského centra|ID MPN přidružené k tenantovi partnerského centra musí být stejné jako ID MPN přidružené k vašemu řešení společného prodeje. Před nasazením konektorů se můžete podívat na to, jestli máte na portálu partnerského centra zobrazený odkaz na svůj společný prodej.|[Správa vašeho účtu](create-user-accounts-and-set-permissions.md)|
|Role uživatelů partnerského centra|Zaměstnanec, který bude instalovat a používat konektory, musí být správcem odkazů.|[Přiřazování uživatelských rolí a oprávnění](create-user-accounts-and-set-permissions.md)|
|Salesforce CRM|Role uživatele CRM je správce systému nebo úpravce systému.|[Přiřazení rolí v Salesforce CRM](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|účet Power Automate Flow|Vytvořte nové provozní prostředí s databází pro testování, přípravu a produkci. Máte-li existující provozní prostředí s databází, je možné jej znovu použít. uživatel, který chce nainstalovat řešení konektoru, musí mít licenci Power Automate a přístup k tomuto prostředí. pokud se instalace nepovede, můžete monitorovat průběh a získat další informace v [Power Automate](https://flow.microsoft.com/) . V části **řešení** vyberte **Zobrazit historii** .|[Vytvořit nebo spravovat prostředí](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a>Instalace balíčku Salesforce pro vlastní pole Microsoftu

aby bylo možné synchronizovat odkazy v rámci partnerského centra a Salesforce CRM, je nutné, aby řešení Power Automate jasně identifikovala pole odkazů specifická pro společnost Microsoft. Tato vymezená část poskytuje partnerům partnerských prodejců možnost rozhodnout se, které referenční seznamy chtějí sdílet se společností Microsoft pro souběžný prodej.

1. V Salesforce aktivujte **poznámky** a přidejte je do seznamu souvisejících příležitostí. [Odkaz](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

1. **Týmy příležitostí** aktivujte pomocí následujících kroků:
    - v instalačním programu pomocí pole **rychlé hledání** vyhledejte Nastavení týmu příležitostí.
    - Podle potřeby definujte nastavení. [Odkaz](https://help.salesforce.com/articleView?id=sf.opp_team_manage.htm&type=5)

1. V Salesforce nainstalujte vlastní pole a objekty pomocí [instalačního programu balíčku](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV). Tento instalační program použijte k instalaci balíčku do libovolné společnosti.

    >[!NOTE]
    >Pokud instalujete do izolovaného prostoru (sandbox), je nutné nahradit počáteční část adresy URL `http://test.salesforce.com` .

1. V Salesforce přidejte řešení Microsoftu do seznamu souvisejících **příležitostí** . Po přidání vyberte ikonu **klíče** a aktualizujte vlastnosti.

## <a name="best-practice-test-before-you-go-live"></a>Osvědčené postupy: test před zahájením provozu

než nainstalujete, nakonfigurujete a přizpůsobíte Power Automate řešení v produkčním prostředí, nezapomeňte řešení otestovat na pracovní instanci CRM.

- nainstalujte řešení Microsoft Power Automate do přípravného prostředí/instance CRM.

- vytvořte kopii řešení a spusťte přizpůsobení konfigurace a Power Automate flow v přípravném prostředí.

- Otestujte řešení na pracovní instanci/CRM.

- Po úspěšném dokončení naimportujte jako spravované řešení do produkční instance.

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>Nainstalovat synchronizaci odkazů partnerského centra pro Salesforce CRM

1. přejít na [Power Automate](https://flow.microsoft.com) a v pravém horním rohu vyberte **prostředí** . Zobrazí se vám dostupné instance CRM.

1. V rozevíracím seznamu v pravém horním rohu vyberte příslušnou instanci CRM.

1. Na levém navigačním panelu vyberte **řešení** .

1. V horní nabídce vyberte odkaz **otevřít AppSource** .

   :::image type="content" source="images/cosellconnectors/open-appsource.png" alt-text="Otevřete AppSource.":::

1. V místní obrazovce vyhledejte **konektory odkazů partnerského centra pro Salesforce** .  

   :::image type="content" source="images/salesforce/salesforce-get-it-now.png" alt-text="Snímek obrazovky, který teď získá.":::

1. Vyberte tlačítko **získat nyní** a pak vyberte **pokračovat**.

1. Na další stránce vyberte prostředí Salesforce CRM pro instalaci aplikace. Vyjádřit souhlas s podmínkami a ujednáními.

1. Pak budete přesměrováni na stránku **spravovat vaše řešení** .  Přejděte na "odkazy na partnerské Centrum" pomocí tlačítek se šipkami ve spodní části stránky. **Naplánovaná instalace** by se měla objevit u řešení s odkazy partnerského centra. Instalace bude trvat 10-15 minut.

1. po dokončení instalace přejděte zpět na [Power Automate](https://flow.microsoft.com) a vyberte **řešení** z levé navigační oblasti. Všimněte si, že **synchronizace odkazů partnerského centra pro Salesforce** je teď k dispozici v seznamu řešení.

1. Vyberte **synchronizaci odkazů z partnerského centra pro Salesforce**. k dispozici jsou následující Power Automate toky a entity:

   :::image type="content" source="images/cosellconnectors/partner-center-referrals-synchronization.png" alt-text="Toky Salesforce.":::

## <a name="configure-the-solution"></a>Konfigurace řešení

1. Po instalaci řešení do instance CRM přejděte zpět na [Power Automate](https://flow.microsoft.com/).

1. v rozevíracím seznamu **prostředí** v pravém horním rohu vyberte instanci CRM, do které jste nainstalovali řešení Power Automate.

1. Budete muset vytvořit připojení, která přiřadí tři uživatelské účty:

   - Uživatel partnerského centra s přihlašovacími údaji správce odkazů
   - Události Partnerského centra
   - správce CRM s toky Power Automate v řešení

   1. V levém navigačním panelu vyberte **připojení** a v seznamu vyberte řešení **Partnerské centrum odkazů** .

   1. Vytvořte připojení výběrem možnosti **vytvořit připojení**.

        :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Snímek obrazovky, který ukazuje vytvoření připojení.":::

   1. Na panelu hledání v pravém horním rohu vyhledejte **odkazy na partnerské Centrum (Preview)** .

   1. Vytvořte připojení pro uživatele partnerského centra s rolí přihlašovacích údajů správce odkazů.

   1. Potom vytvořte připojení událostí partnerského centra pro uživatele partnerského centra s přihlašovacími údaji správce odkazů.

   1. Vytvořte připojení pro Salesforce pro uživatele správce CRM.
  
   1. Vytvořte připojení k aplikaci Microsoft DataConnection pro uživatele s oprávněním správce aplikace CRM.

   1. Po přidání všech připojení byste měli ve svém prostředí zobrazit následující připojení:

        :::image type="content" source="images/cosellconnectors/salesforce-connections.png" alt-text="Snímek obrazovky, který ukazuje, jak sledovat připojení.":::

### <a name="edit-the-connections"></a>Upravit připojení

1. Vraťte se na stránku **řešení** a vyberte **výchozí řešení**. Kliknutím na tlačítko **vše** vyberte **odkaz připojení (Preview)** .

   :::image type="content" source="images/connection-reference-video.gif" alt-text="Snímek obrazovky, který zobrazuje úpravu připojení.":::

1. Jednotlivě upravte jednotlivá připojení výběrem ikony se třemi tečkami. Přidejte příslušná připojení.

   :::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Snímek obrazovky ukazuje, jak upravit konektory.":::

1. Zapněte toky v následujícím pořadí:
   - Partnerské centrum registrace webhooku (Insider Preview)
   - [Přizpůsobit] Vytvoření nebo získání podrobností z Salesforce
   - Vytvoření nabídky spoluprodá Referral-Salesforce k Partnerské centrum (Insider Preview)
   - Partnerské centrum referenčních doporučení spoluprodeje Microsoftu pro Salesforce (Insider Preview)  
   - Partnerské centrum salesforce (Insider Preview)
   - Salesforce na Partnerské centrum (Insider Preview)
   - Salesforce Opportunity to Partnerské centrum (Insider Preview)
   - Salesforce – řešení Microsoftu pro Partnerské centrum (Insider Preview)

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Použití rozhraní WEBHOOK API k registraci událostí změny prostředků

Pomocí rozhraní API Partnerské centrum webhooku můžete registrovat události změny prostředků. Tyto události změny se na vaši adresu URL odesílat jako příspěvky HTTP.

1. Vyberte **Partnerské centrum Salesforce CRM (Insider Preview).**

1. Vyberte **ikonu Upravit** a vyberte **Při přijetí požadavku HTTP.**

1. Vyberte **ikonu Kopírovat** a zkopírujte zadanou adresu **URL HTTP POST**.

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Snímek obrazovky, který ukazuje, jak zkopírovat adresu URL":::

1. Vyberte **tok Partnerské centrum webhooku (Insider Preview)** Power Automate a pak vyberte **Spustit.**

1. Ujistěte **se, že** se v pravém podokně otevře okno Spustit tok, a vyberte **Pokračovat.**

1. Zadejte následující podrobnosti:

   - **Koncový bod triggeru HTTP:** Tato adresa URL se zkopíroval z předchozího kroku.
   - **Události k registraci:** Vyberte všechny dostupné události **(vytvořené** referenčními seznamem, aktualizované referenční **seznamy,** vytvořené související referenční odkazy a aktualizace souvisejících **referenčních seznamu).**
   - **Přepsat existující koncové body triggeru, pokud jsou k dispozici?**: Ano. Pro danou událost webhooku je možné zaregistrovat pouze jednu adresu URL.

1. Vyberte **Spustit tok** a pak vyberte **Hotovo.**

Webhook teď může naslouchat událostem, vytvářet a aktualizovat je.

## <a name="customize-synchronization-steps"></a>Přizpůsobení kroků synchronizace

Systémy CRM jsou vysoce přizpůsobené a můžete přizpůsobit Power Automate na základě nastavení CRM. Když se referenční seznam spoluprodáte mezi systémem Partnerské centrum a systémem CRM, pole synchronizovaná v počítači Partnerské centrum PC jsou uvedená v průvodci mapováním vlastních [polí.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)

Postupujte podle průvodce mapováním polí a v případě potřeby proveďte příslušné změny v **[Přizpůsobení] Vytvoření** nebo získání podrobností z Salesforce nebo proměnných prostředí. Ne aktualizujte žádné jiné toky v Power Automate, protože to může mít vliv na budoucí upgrady řešení.

K dispozici jsou následující přizpůsobení:

- **Zobrazit značku zaškrtnutí v** názvu příležitosti: Ve výchozím nastavení se vedle názvu příležitosti zobrazí značka zaškrtnutí, která označuje, že synchronizace mezi Partnerské centrum a Salesforce CRM probíhá úspěšně. Podobně se křížové označení zobrazí, pokud synchronizace selže. Pokud se chcete vyhnout přidání zaškrtnutí nebo křížové značky  v názvu příležitosti, nastavte aktuální hodnotu značky zaškrtnutí Zobrazit v proměnné prostředí název příležitosti na Ne.

- **Název fáze:**

  - **Název aktivní fáze:** Toto je fáze v prodejním kanálu příležitosti v Salesforce.  Představuje aktivní fázi a je ekvivalentní referenčnímu seznamu v přijatém stavu v Partnerské centrum. Může to být další fáze v prodejním kanálu po fázi on-hold. Přesunutí prodejní fáze příležitosti z fáze on-hold do aktivní fáze přijme referenční Partnerské centrum a změny se začnou synchronizovat.

  - **Název fáze přidržení:** Název fáze v prodejním kanálu příležitosti v Salesforce. Představuje fázi blokování. Nová referenční doporučení ke spoluprodeji sdílená od Microsoftu, která ještě nejsou přijata, se v Salesforce nastaví na tuto fázi. Změny provedené v příležitosti v době, kdy je ve fázi blokování, se nebudou synchronizovat do Partnerské centrum. Fáze prodeje přesunutí příležitosti z této fáze blokování přijme referenční Partnerské centrum a změny se začnou synchronizovat.

- **Kód země účtu zákazníka:** Při vytváření nového referenčního seznamu je povinné zadat dvoupísmenný kód země (ISO 3166). Ve výchozím nastavení se kód země synchronizuje do a z pole **BillingCountry** účtu v Salesforce. Pokud máte v Salesforce jiné pole, ze které se má kód země synchronizovat:

  - Pro pole s kódem země, které nenílookup, v účtu, které obsahuje dvou písmeno kódu:

    - Aktualizujte **název pole Customer Account Country Code** v proměnné prostředí Salesforce názvem pole CRM. Ujistěte se, že zadáte název pole, nikoli jeho zobrazovaný název.

    - Upravte **[Customize] Create or Get Details from Salesforce**(Vytvořit nebo získat podrobnosti z Salesforce) a v akci CRM přejděte na Create **or get customer account** (Vytvořit nebo získat zákaznický účet) a přiřaďte hodnotu **Země** ke správnému poli v CRM. Odeberte také přiřazení **hodnoty Země** z **billingcountry**.

  - Pole s kódem země založené na vyhledávání v účtu:

    - Přidejte do účtu nové vlastní pole a automaticky ho naplňte dvoupísmenný kód země (ISO 3166) na základě hodnoty vybrané v poli založeném na vyhledávání a naopak.

    - Pokud chcete synchronizovat nové vlastní pole z CRM do a z aplikace, postupujte podle předchozích kroků pro pole s kódem země, která není v seznamu Partnerské centrum.

- **Hodnota dohody:** Ve výchozím nastavení se hodnota dohody z Partnerské centrum synchronizuje do a z **částky** v CRM. Pokud máte v CRM jiné pole pro hodnotu dohody, ze které se má synchronizovat:

  - Aktualizujte **název pole Hodnota** dohody v proměnné prostředí Salesforce názvem pole CRM. Ujistěte se, že zadáte název pole, nikoli jeho zobrazovaný název.

  - Upravte **[Customize] Create or Get Details** from Salesforce (Vytvořit nebo získat podrobnosti z Salesforce), přejděte do části Create or update **opportunity** in CRM (Vytvořit nebo aktualizovat příležitost v CRM) a aktualizujte akce Create a new opportunity (Vytvořit novou příležitost) **a** Update **existing opportunity** (Aktualizovat existující příležitost) a přiřaďte **hodnotu DealValue** ke správnému poli v Salesforce.

- **Kód měny hodnoty dohody:** Název pole kódu měny hodnoty dohody v Salesforce. Toto pole Název rozhraní API se použije k získání kódu měny hodnoty dohody příležitosti při vytváření nebo aktualizaci referenčního seznamu v Microsoft Partnerské centrum. Pokud se pole kódu měny hodnoty dohody liší od výchozího pole **CurrencyIsoCode,** aktualizujte aktuální hodnotu této proměnné prostředí.

  - Aktualizujte **název pole měny** hodnoty dohody v proměnné prostředí Salesforce názvem pole CRM. Ujistěte se, že zadáte název pole, nikoli jeho zobrazovaný název.

  - Upravte **[Customize] Create or Get Details** from Salesforce (Vytvořit nebo získat podrobnosti z Salesforce), přejděte do části Create or update **opportunity** in CRM (Vytvořit nebo aktualizovat příležitost v CRM) a aktualizujte akce Create a new opportunity (Vytvořit novou příležitost) **a** Update existing **opportunity** (Aktualizovat existující příležitost) a přiřaďte **hodnotu DealValueCurrency** ke správnému poli v Salesforce.

- **Synchronizace příležitosti ke** spoluprodeji: Pokud je nastavená na **ano,** budou se mezi a Salesforce synchronizovat pouze příležitosti ke spoluprodeji a sdílení Partnerské centrum kanálu. Pokud je **nastavená na hodnotu žádná,** potenciální zákazníky, spoluprodej a příležitosti ke sdílení kanálu se budou synchronizovat z Partnerské centrum do Salesforce. Tato proměnná nemá žádný vliv na příležitosti synchronizované ze Salesforce do Partnerské centrum.

## <a name="update-environment-variable"></a>Aktualizace proměnné prostředí

Aktualizace hodnoty proměnné prostředí:

1. Přejděte na **stránku Řešení a** vyberte Výchozí **řešení.** Výběrem možnosti **All (Vše) vyberte Environment** **Variable** (Proměnná prostředí).

1. Vyberte proměnnou prostředí pro hodnotu, kterou je potřeba aktualizovat, a vyberte **Upravit** pomocí ikony se třemi tečkami.

1. Aktualizovat **aktuální hodnotu** (ne aktualizovat výchozí **hodnotu)** pomocí možnosti **Nová hodnota** a poskytnutím hodnoty. Hodnota musí odpovídat datovému typu proměnné. Datový typ Ano nebo Ne například přijme hodnotu Ano nebo Ne.

   :::image type="content" source="images/cosellconnectors/environment-variables-video.gif" alt-text="Snímek obrazovky znázorňuje aktualizaci proměnných prostředí":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>Synchronizace referenčních odkazů end-to-end bi-directional co-sell

Po instalaci, konfiguraci a přizpůsobení řešení Power Automate můžete otestovat synchronizaci referenčních odkazů spoluprodeje mezi salesforce CRM a Partnerské centrum.

### <a name="pre-requisites"></a>Požadavky

Pokud chcete synchronizovat referenční Partnerské centrum a Salesforce CRM, musí Power Automate jasně vymehat pole referenčních seznamů specifická pro Microsoft. Tato identifikace poskytuje týmům prodejců možnost rozhodnout se, které referenční odkazy chce sdílet s Microsoftem pro spoluprodávač.

Sada vlastních polí je k dispozici jako součást synchronizace referenčních  Partnerské centrum referenčních seznamů pro entitu Opportunity řešení Salesforce CRM. Uživatel s rolí správce CRM bude muset vytvořit samostatný oddíl CRM s vlastními **poli Opportunity.**

Následující vlastní pole by měla být součástí oddílu CRM:

- **Synchronizace s Partnerské centrum:** Jestli se má synchronizovat příležitost s Partnerské centrum. Ve výchozím nastavení má toto pole hodnotu Ne a prodejce musí explicitně nastavit možnost Ano, aby bylo možné sdílet příležitost s Microsoftem. Nové referenční odkazy sdílené z Partnerské centrum do CRM budou mít tuto hodnotu pole nastavenou na Ano.

- **Identifikátor referenčního** seznamu: Pole identifikátoru jen pro čtení pro referenční Partnerské centrum referenční seznam.

- **Odkaz na referenční** seznam: Odkaz jen pro čtení referenčního seznamu v Microsoft Partnerské centrum.

- **Jak může Microsoft pomoci:** Pomoc od Microsoftu požadovaná pro referenční informace. Pokud chcete vytvořit referenční seznam pro spoluprodácí, vyberte vhodnou nápovědu od Microsoftu. Ke příležitosti k vytvoření referenčního seznamu pro spoluprodát musí být přidružený kontakt zákazníka. Pokud chcete vytvořit referenční seznam bez spoluproduování, toto pole nevytvářejte. Referenční seznam bez spoluproduování můžete kdykoli převést na referenční seznam pro spoluprodát výběrem příslušné možnosti požadované nápovědy.

- **Viditelnost referenčních Partnerské centrum** microsoftu: Vyberte viditelnost referenčního Partnerské centrum referenčního seznamu. Když ho prodejci Microsoftu zviditelní, může se referenční seznam bez spoluprodávače převést na spoluprodávač. Pokud je požadována nápověda Microsoftu, je referenční odkaz standardně viditelný prodejcům Microsoftu. Jakmile je toto pole označené jako viditelné, není možné ho vrátit zpět.

- **aplikace Microsoft CRM:** Když Microsoft vytvoří referenční seznam pro spoluprodávaného prodeje a přijme ho, naplní se toto pole identifikátorem CRM od Microsoftu.

- **Microsoft Partnerské centrum Solutions:** Vlastní objekt pro přidružení řešení připravených ke spoluproduování nebo řešení Microsoftu s příležitostí. Z příležitosti je možné přidat nebo odebrat jedno nebo více řešení. Před sdílením s Microsoftem je nutné přidat k příležitosti alespoň jedno připravené řešení pro spoluprodání nebo řešení Microsoftu. Pokud chcete tento objekt přidružit k příležitosti, aktualizujte **formulář Opportunity** v aplikaci CRM.

- **Audit:** Záznam pro audit jen pro čtení pro synchronizaci s referenčními Partnerské centrum referenčními odkazy

### <a name="scenarios"></a>Scénáře

1. Synchronizace referenčních odkazů při vytvoření nebo aktualizaci referenčních seznamů v CRM a synchronizaci v Partnerské centrum:

   1. Přihlaste se k prostředí Salesforce CRM s uživatelem, který má přehled v **části Opportunity** v CRM.

   1. Při vytváření nové příležitosti v prostředí Salesforce  **CRM Partnerské centrum** oddíl Microsoft Partnerské centrum.

   1. Příležitosti, které jsou úspěšně synchronizovány s Partnerské centrum, se identifikují ikonou ✔ salesforce CRM.
      :::image type="content" source="images/salesforce/salesforce-environment.png" alt-text="Snímek obrazovky s prostředím Salesforce":::

   1. Pokud chcete tuto příležitost synchronizovat s microsoft Partnerské centrum, ujistěte se, že jste v zobrazení karty nastavili následující pole:

      - **Jak může Microsoft pomoct?**: Pokud chcete vytvořit referenční seznam pro spoluprodácí, vyberte vhodnou možnost nápovědy.

        :::image type="content" source="images/salesforce/salesforce-help-option.png" alt-text="Snímek obrazovky, který znázorňuje, jak získat příslušná pole v zobrazení karty":::

      - **Synchronizace s Partnerské centrum:** Ano
      - **Kontakt zákazníka:** Pokud chcete vytvořit referenční seznam pro spoluprodácí, přidejte k příležitosti kontakt zákazníka.
      - **Řešení Microsoftu:** Pokud chcete sdílet referenční seznam s Microsoftem, přidejte k této příležitosti platné řešení pro spoluprodání nebo řešení Microsoftu.

   1. Po nastavení možnosti Synchronizovat s Partnerské centrum **na** Ano **počkejte** 10 minut, přihlaste se ke svému Partnerské centrum účtu. Vaše referenční seznamy se synchronizují s aplikací Salesforce CRM a odkaz na referenční seznam se vyplní. Pokud dojde k selhání, pole Audit se naplní informacemi o chybě.

   1. Podobně když je možnost Synchronizovat **s Partnerské centrum** nastavená na **Ano,** pokud aktualizujete příležitost v Salesforce CRM, změny se synchronizují s vaším Partnerské centrum účtem.

2. Synchronizace referenčních seznamů při vytvoření nebo aktualizaci referenčního Partnerské centrum v prostředí Salesforce CRM:

    1. Přihlaste se k řídicímu [Partnerské centrum.](https://partner.microsoft.com/dashboard/home)

    1. V **nabídce vlevo** vyberte Referenční odkazy.

    1. Kliknutím na možnost New deal (Nová dohoda) Partnerské centrum nový referenční seznam pro spoludácí se na Partnerské centrum.

    1. Přihlaste se k prostředí Salesforce CRM.

    1. Přejděte na **Otevřít příležitosti.** Referenční seznam vytvořený v Microsoft Partnerské centrum se teď synchronizuje v Salesforce CRM.

    1. Když vyberete synchronizovaný referenční seznam, vyplní se podrobnosti o zobrazení karty.

       :::image type="content" source="images/salesforce/salesforce-casino.png" alt-text="Snímek obrazovky se stránkou salesforce opportunity":::

>[!NOTE]
>**Potřebujete pomoc s nasazením?**
>Pokud potřebujete pomoc s nasazením konektoru referenčních doporučení ke spoluprodávu, můžete se zapojit do partnerského technického konzultanta. Mohou poskytovat pomoc při nasazení a osvědčené postupy pro úspěšnou implementaci.
>
>Další informace najdete v tématu Odeslání technické žádosti o [služby předprodeje a nasazení.](technical-benefits.md)

## <a name="next-steps"></a>Další kroky

- [Správa potenciálních zákazníků](manage-leads.md)

- [Správa příležitostí ke spoluprodeji](manage-co-sell-opportunities.md)

- [Webhooky Partnerského centra](/partner-center/develop/partner-center-webhooks)
