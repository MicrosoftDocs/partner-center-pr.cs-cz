---
title: Konektor pro spoluprodej pro Salesforce CRM Partnerské centrum
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Synchronizujte referenční seznam v Partnerské centrum se salesforce CRM. Prodejci pak mohou v rámci systémů CRM spoluprodávat s Microsoftem.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 06/28/2021
ms.openlocfilehash: f8cb4cd2488e55ab64cf7b7cdce4a3e950b266de
ms.sourcegitcommit: 6a6e8f9af0a58b32770c7fce9f567dd4795b9797
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/29/2021
ms.locfileid: "113029060"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Konektor pro spoluprodej pro Salesforce CRM – přehled

**Odpovídající role:** Správce referenčních | Správce systému nebo úpravce systému v CRM

Partnerské centrum spoluprodávače umožňuje prodejcům spoluprodávat s Microsoftem z vašich systémů CRM. Nebudou muset být vytrénovány tak, aby Partnerské centrum spravovat dohody o spoluprodátech. Pomocí konektorů pro spoluprodávku můžete vytvořit nový referenční seznam pro spoluprodávku, abyste se mohli zapojit jako prodejce Microsoftu, získat referenční seznam od prodejce Microsoftu, přijmout nebo odmítnout referenční seznam, upravit data o dohodu, jako je hodnota dohody, a datum ukončení.  Můžete také dostávat jakékoli aktualizace těchto dohod o spoluprodávce od prodejců Microsoftu. Při práci v rámci CRM podle vašeho výběru můžete všechny referenční seznamy dělat, a ne v Partnerské centrum.

Řešení je založené na řešení Microsoft Power Automate a používá Partnerské centrum API.

## <a name="before-you-install---pre-requisites"></a>Před instalací – předpoklady

|**Témata**|**Podrobnosti**|**Odkazy**|
|--------------|--------------------|------|
|Microsoft Partner Network ID |Potřebujete platné ID MPN.|Připojení k [MPN](https://partner.microsoft.com/)|
|Připraveno ke spoluprodání|Řešení IP adres nebo služeb musí být připravené ke spoluprodání.|[Prodej s Microsoftem](https://partner.microsoft.com/membership/sell-with-microsoft)|
|Účet partnerského centra|ID MPN přidružené k tenantovi Partnerské centrum musí být stejné jako ID MPN přidružené k vašemu řešení spoluprodávku. Před nasazením konektorů ověřte, že se referenční Partnerské centrum spoluprodáte na portálu.|[Správa vašeho účtu](create-user-accounts-and-set-permissions.md)|
|Partnerské centrum rolí uživatelů|Zaměstnanec, který bude tyto konektory instalovat a používat, musí být správcem referenčních seznamu.|[Přiřazování uživatelských rolí a oprávnění](create-user-accounts-and-set-permissions.md)|
|Salesforce CRM|Role uživatele CRM je Správce systému nebo Úpravce systému.|[Přiřazení rolí v Salesforce CRM](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|Power Automate toku|Vytvořte nové produkční prostředí s databází pro testování, fázování a produkci. Pokud máte stávající produkční prostředí s databází, můžete ho znovu použít. Uživatel, který bude řešení konektoru instalovat, musí mít Power Automate a přístup k tomuto prostředí. Průběh můžete sledovat a získat další informace v [Power Automate](https://flow.microsoft.com/) případě, že instalace selže. V části **Řešení vyberte** Zobrazit **historii.**|[Vytvoření nebo správa prostředí](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a>Instalace balíčku Salesforce pro vlastní pole Microsoftu

Aby bylo možné synchronizovat referenční Partnerské centrum napříč aplikacemi a salesforce CRM, Power Automate řešení musí jasně identifikovat pole referenčních seznamů specifická pro Microsoft. Toto vyněcování poskytuje týmům prodejců partnerů možnost rozhodnout se, které referenční reference chce sdílet s Microsoftem pro spoluprodávku.

1. V Salesforce aktivujte **Poznámky** a přidejte je do seznamu příležitostí. [Odkaz](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

1. Aktivujte **týmy příležitostí** pomocí následujících kroků:
    - V instalačním programu vyhledejte **pomocí pole Rychlé** hledání nastavení týmu příležitostí.
    - Definujte nastavení podle potřeby. [Odkaz](https://help.salesforce.com/articleView?id=sf.opp_team_manage.htm&type=5)

1. V Salesforce nainstalujte vlastní pole a objekty pomocí [instalačního programu balíčků](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV). Pomocí tohoto instalačního programu nainstalujte balíček do libovolné společnosti.

    >[!NOTE]
    >Pokud instalujete do sandboxu, musíte počáteční část adresy URL nahradit `http://test.salesforce.com` .

1. V Salesforce přidejte řešení Microsoftu do **seznamu souvisejícího** s příležitostí. Po přidání vyberte ikonu **klíče** a aktualizujte vlastnosti.

## <a name="best-practice-test-before-you-go-live"></a>Osvědčený postup: Testování před živým vysíláním

Než nainstalujete, nakonfigurujete a přizpůsobíte Power Automate v produkčním prostředí, nezapomeňte řešení otestovat na pracovní instanci CRM.

- Nainstalujte řešení Microsoft Power Automate do pracovního prostředí nebo instance CRM.

- Vytvořte kopii řešení a spusťte konfiguraci a Power Automate toku v pracovním prostředí.

- Otestujte řešení na pracovní instanci nebo instanci CRM.

- V případě úspěchu importujte jako spravované řešení do produkční instance.

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>Instalace Partnerské centrum referenčních seznamů pro Salesforce CRM

1. Přejděte na [Power Automate](https://flow.microsoft.com) a **v pravém** horním rohu vyberte Prostředí. Zobrazí se dostupné instance CRM.

1. V rozevíracím seznamu v pravém horním rohu vyberte příslušnou instanci CRM.

1. V **levém navigačním** panelu vyberte Řešení.

1. V horní nabídce vyberte odkaz Open AppSource (Otevřít **AppSource).**

   :::image type="content" source="images/cosellconnectors/open-appsource.png" alt-text="Otevření AppSource":::

1. Na **místní Partnerské centrum vyhledejte konektory referenčních** odkazů pro Salesforce.  

   :::image type="content" source="images/salesforce/salesforce-get-it-now.png" alt-text="Snímek obrazovky s ukázkou Získat":::

1. Vyberte tlačítko **Get it now (Získat)** a pak vyberte **Continue (Pokračovat).**

1. Na další stránce vyberte prostředí Salesforce CRM pro instalaci aplikace. Odsouhlaste podmínky a podmínky.

1. Pak budete přesměrováni na stránku **Spravovat řešení.**  Pomocí tlačítek Partnerské centrum v dolní části stránky přejděte k části Referenční odkazy. **Vedle řešení** referenčních Partnerské centrum by se měla zobrazit naplánovaná instalace. Instalace bude trvat 10 až 15 minut.

1. Po dokončení instalace přejděte zpět na stránku [Power Automate](https://flow.microsoft.com) **v** levé navigační oblasti vyberte Řešení. Všimněte **si, Partnerské centrum referenčních seznamů** pro Salesforce je teď dostupná v seznamu Řešení.

1. Vyberte **Partnerské centrum referenčních seznamu pro Salesforce**. K dispozici Power Automate toky a entity:

   :::image type="content" source="images/cosellconnectors/partner-center-referrals-synchronization.png" alt-text="Toky Salesforce":::

## <a name="configure-the-solution"></a>Konfigurace řešení

1. Po instalaci řešení v instanci CRM přejděte zpět na Power Automate [.](https://flow.microsoft.com/)

1. V **rozevíracím** seznamu Prostředí v pravém horním rohu vyberte instanci CRM, do které jste nainstalovali Power Automate řešení.

1. Budete muset vytvořit připojení, která přidruží tyto tři uživatelské účty:

   - Partnerské centrum uživatele s přihlašovacími údaji správce referenčních odkazů
   - Události Partnerského centra
   - Správce CRM s Power Automate toky v řešení

   1. V **levém** navigačním panelu vyberte Připojení a v **seznamu Partnerské centrum referenčních** seznamech.

   1. Vytvořte připojení výběrem **možnosti Vytvořit připojení.**

        :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Snímek obrazovky znázorňuje vytvoření připojení":::

   1. Na **panelu Partnerské centrum v pravém** horním rohu vyhledejte Referenční Partnerské centrum (Preview).

   1. Vytvořte pro svého uživatele Partnerské centrum s rolí přihlašovacích údajů správce referenčních seznamů.

   1. Dále vytvořte připojení Partnerské centrum události pro vašeho Partnerské centrum uživatele s přihlašovacími údaji správce referenčních seznamů.

   1. Vytvořte připojení pro Salesforce pro uživatele správce CRM.
  
   1. Vytvořte připojení pro Microsoft Dataverse pro uživatele s oprávněními správce CRM.

   1. Po přidání všech připojení by se ve vašem prostředí měla zobrazit následující připojení:

        :::image type="content" source="images/cosellconnectors/salesforce-connections.png" alt-text="Snímek obrazovky, který znázorňuje, jak sledovat připojení":::

### <a name="edit-the-connections"></a>Úprava připojení

1. Vraťte se **na stránku** Řešení a vyberte **Výchozí řešení.** Kliknutím **na Všechny** vyberte Odkaz na připojení **(Preview).**

   :::image type="content" source="images/connection-reference-video.gif" alt-text="Snímek obrazovky znázorňuje úpravy připojení":::

1. Jednotlivě upravte jednotlivá připojení výběrem ikony se třemi tečkami. Přidejte příslušná připojení.

   :::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Snímek obrazovky ukazuje, jak upravit konektory.":::

1. Zapněte toky v následujícím pořadí:
   - Partnerské centrum registrace webhooku (Insider Preview)
   - [Přizpůsobit] Vytvoření nebo získání podrobností z Salesforce
   - Vytvoření nabídky spoluprodá Referral-Salesforce k Partnerské centrum (Insider Preview)
   - Partnerské centrum referenčních doporučení spoluprodeje Microsoftu pro Salesforce (Insider Preview)  
   - Partnerské centrum salesforce (Insider Preview)
   - Salesforce do Partnerské centrum (Insider Preview)
   - Salesforce Opportunity to Partnerské centrum (Insider Preview)
   - Salesforce – řešení Microsoftu pro Partnerské centrum (Insider Preview)

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Použití rozhraní WEBHOOK API k registraci událostí změny prostředků

Pomocí rozhraní API Partnerské centrum webhooku můžete registrovat události změny prostředků. Tyto události změny se posílají na vaši adresu URL jako příspěvky HTTP.

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

Systémy CRM jsou vysoce přizpůsobené a můžete přizpůsobit Power Automate na základě nastavení CRM. Když se referenční seznam pro spoluprodácí synchronizuje mezi systémem Partnerské centrum a vaším systémem CRM, pole synchronizovaná v počítači Partnerské centrum PC jsou uvedená v průvodci mapováním vlastních [polí.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)

Postupujte podle průvodce mapováním polí a v případě potřeby proveďte příslušné změny v **tématu [Přizpůsobit]** Vytvoření nebo získání podrobností z Salesforce nebo proměnných prostředí. Ne aktualizujte žádné jiné toky v Power Automate, protože to může mít vliv na budoucí upgrady řešení.

K dispozici jsou následující přizpůsobení:

- **Zobrazit značku zaškrtnutí v** názvu příležitosti: Ve výchozím nastavení se vedle názvu příležitosti zobrazí značka zaškrtnutí, která označuje, že synchronizace mezi Partnerské centrum a Salesforce CRM probíhá úspěšně. Podobně se křížové označení zobrazí, pokud synchronizace selže. Pokud se chcete vyhnout přidání zaškrtnutí nebo křížové značky  v názvu příležitosti, nastavte aktuální hodnotu značky zaškrtnutí Zobrazit v proměnné prostředí název příležitosti na Ne.

- **Název fáze:**

  - **Název aktivní fáze:** Toto je fáze v prodejním kanálu příležitosti v Salesforce.  Představuje aktivní fázi a je ekvivalentní referenčnímu seznamu v přijatém stavu v Partnerské centrum. To může být další fáze v prodejním kanálu po fázi on-hold. Přesunutí prodejní fáze příležitosti z fáze on-hold do aktivní fáze přijme referenční Partnerské centrum a změny se začnou synchronizovat.

  - **Název fáze v zdržení:** Název fáze v prodejním kanálu příležitosti v Salesforce. Představuje fázi blokování. Nová referenční doporučení ke spoluprodeji sdílená od Microsoftu, která ještě nejsou přijata, se v Salesforce nastaví na tuto fázi. Změny provedené v příležitosti v době, kdy je ve fázi blokování, se nebudou synchronizovat do Partnerské centrum. Fáze prodeje přesunutí příležitosti z této fáze blokování přijme referenční Partnerské centrum a změny se začnou synchronizovat.

- **Kód země účtu zákazníka:** Při vytváření nového referenčního seznamu je povinné zadat dvoupísmenný kód země (ISO 3166). Ve výchozím nastavení se kód země synchronizuje do a z pole **BillingCountry** účtu v Salesforce. Pokud máte v Salesforce jiné pole pro kód země, ze které se má synchronizovat:

  - Pro pole s kódem země, které nenílookup, v účtu, které obsahuje dvou písmeno kódu:

    - Aktualizujte **název pole Kód země** účtu zákazníka v proměnné prostředí Salesforce názvem pole CRM. Ujistěte se, že zadáte název pole, nikoli jeho zobrazovaný název.

    - Upravte **[Customize] Create or Get Details from Salesforce**(Vytvořit nebo získat podrobnosti z Salesforce) a v akci CRM přejděte na Create **or get customer account** (Vytvořit nebo získat zákaznický účet) a přiřaďte hodnotu **Země** ke správnému poli v CRM. Odeberte také přiřazení **hodnoty Země** z **billingcountry**.

  - Pole s kódem země založené na vyhledávání v účtu:

    - Přidejte do účtu nové vlastní pole a automaticky ho vyplňte dvoupísmenný kód země (ISO 3166) na základě hodnoty vybrané v poli založeném na vyhledávání a naopak.

    - Pokud chcete synchronizovat nové vlastní pole z CRM do a z aplikace, postupujte podle předchozích kroků pro pole s kódem země, která není v seznamu Partnerské centrum.

- **Hodnota dohody:** Ve výchozím nastavení se hodnota dohody z Partnerské centrum synchronizuje do a z **částky** v CRM. Pokud máte v CRM jiné pole pro hodnotu dohody, která se má synchronizovat z:

  - Aktualizujte **název pole hodnota** dohody v proměnné prostředí Salesforce názvem pole CRM. Ujistěte se, že zadáte název pole, nikoli jeho zobrazovaný název.

  - Upravte **[Customize] Create or Get Details** from Salesforce (Vytvořit nebo získat podrobnosti z Salesforce), přejděte do části Create or update **opportunity** in CRM (Vytvořit nebo aktualizovat příležitost v CRM) a aktualizujte akce Create a new opportunity (Vytvořit novou příležitost) **a** Update **existing opportunity** (Aktualizovat existující příležitost) a přiřaďte **hodnotu DealValue** ke správnému poli v Salesforce.

- **Kód měny hodnoty dohody:** Název pole kódu měny hodnoty dohody v Salesforce. Toto pole Název rozhraní API se použije k získání kódu měny hodnoty dohody příležitosti při vytváření nebo aktualizaci referenčního seznamu v Microsoft Partnerské centrum. Pokud se pole kódu měny hodnoty dohody liší od výchozího pole **CurrencyIsoCode,** aktualizujte aktuální hodnotu této proměnné prostředí.

  - Aktualizujte **název pole měny hodnoty** dohody v proměnné prostředí Salesforce názvem pole CRM. Ujistěte se, že zadáte název pole, nikoli jeho zobrazovaný název.

  - Upravte **[Customize] Create or Get Details** from Salesforce (Vytvořit nebo získat podrobnosti z Salesforce), přejděte do části Create or update **opportunity** in CRM (Vytvořit nebo aktualizovat příležitost v CRM) a aktualizujte akce Create a new opportunity (Vytvořit novou příležitost) **a** Update existing **opportunity** (Aktualizovat existující příležitost) a přiřaďte **hodnotu DealValueCurrency** ke správnému poli v Salesforce.

- **Synchronizace příležitosti ke** spoluprodeji: Pokud je nastavená na **ano,** budou se mezi a Salesforce synchronizovat pouze příležitosti ke spoluprodeji a sdílení Partnerské centrum kanálu. Pokud je **nastavená na hodnotu žádná,** potenciální zákazníky, spoluprodej a příležitosti ke sdílení kanálu se budou synchronizovat z Partnerské centrum do Salesforce. Tato proměnná nemá žádný vliv na příležitosti synchronizované ze Salesforce do Partnerské centrum.

## <a name="update-environment-variable"></a>Aktualizace proměnné prostředí

Aktualizace hodnoty proměnné prostředí:

1. Přejděte na **stránku Řešení** a vyberte Výchozí **řešení.** Výběrem možnosti **All (Vše) vyberte Environment** **Variable** (Proměnná prostředí).

1. Vyberte proměnnou prostředí pro hodnotu, kterou je potřeba aktualizovat, a vyberte **Upravit** pomocí ikony se třemi tečkami.

1. Aktualizovat **aktuální hodnotu** (ne aktualizovat výchozí **hodnotu)** pomocí možnosti **Nová hodnota** a poskytnutím hodnoty. Hodnota musí odpovídat datovému typu proměnné. Datový typ Ano nebo Ne například přijme hodnotu Ano nebo Ne.

   :::image type="content" source="images/cosellconnectors/environment-variables-video.gif" alt-text="Snímek obrazovky znázorňuje aktualizaci proměnných prostředí":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>Synchronizace referenčních odkazů end-to-end bi-directional co-sell

Po instalaci, konfiguraci a přizpůsobení řešení Power Automate můžete otestovat synchronizaci referenčních odkazů spoluprodeje mezi salesforce CRM a Partnerské centrum.

### <a name="pre-requisites"></a>Požadavky

Pokud chcete synchronizovat referenční Partnerské centrum napříč aplikacemi a salesforce CRM, Power Automate řešení musí jasně vytyčovat pole referenčních seznamů specifická pro Microsoft. Tato identifikace poskytuje týmům prodejců možnost rozhodnout se, které referenční odkazy chce sdílet s Microsoftem pro spoluprodávač.

Sada vlastních polí je k dispozici jako součást synchronizace referenčních  Partnerské centrum referenčních seznamů pro entitu Opportunity řešení Salesforce CRM. Uživatel s rolí správce CRM bude muset vytvořit samostatný oddíl CRM s vlastními **poli Opportunity.**

Následující vlastní pole by měla být součástí oddílu CRM:

- **Synchronizace s Partnerské centrum:** Jestli se má synchronizovat příležitost s Partnerské centrum. Ve výchozím nastavení má toto pole hodnotu Ne a váš prodejce musí explicitně nastavit možnost Ano, aby bylo možné sdílet příležitost s Microsoftem. Nové referenční odkazy sdílené z Partnerské centrum do CRM budou mít tuto hodnotu pole nastavenou na Ano.

- **Identifikátor referenčního** seznamu: Pole identifikátoru jen pro čtení pro referenční Partnerské centrum referenční seznam.

- **Odkaz na referenční** seznam: Odkaz jen pro čtení referenčního seznamu v Microsoft Partnerské centrum.

- **Jak může Microsoft pomoci:** Pomoc od Microsoftu požadovaná pro referenční informace. Pokud chcete vytvořit referenční seznam pro spoluprodácí, vyberte vhodnou nápovědu od Microsoftu. Ke příležitosti k vytvoření referenčního seznamu pro spoluprodát musí být přidružený kontakt zákazníka. Pokud chcete vytvořit referenční seznam bez spoluproduování, toto pole nevytvářejte. Referenční seznam bez spoluproduování můžete kdykoli převést na referenční seznam pro spoluprodát výběrem příslušné možnosti požadované nápovědy.

- **Viditelnost referenčních Partnerské centrum** microsoftu: Vyberte viditelnost referenčního Partnerské centrum referenčního seznamu. Když ho prodejci Microsoftu zviditelní, může se referenční seznam bez spoluprodávače převést na spoluprodávač. Pokud je požadována nápověda Microsoftu, je referenční odkaz standardně viditelný prodejcům Microsoftu. Jakmile je toto pole označené jako viditelné, není možné ho vrátit zpět.

- **Identifikátor Microsoft CRM:** Když Microsoft vytvoří referenční seznam pro spoluprodávaného prodeje a přijme ho, naplní se toto pole identifikátorem CRM od Microsoftu.

- **Microsoft Partnerské centrum Solutions:** Vlastní objekt pro přidružení řešení připravených ke spoluproduování nebo řešení Microsoftu s příležitostí. Z příležitosti je možné přidat nebo odebrat jedno nebo více řešení. Před sdílením s Microsoftem je nutné přidat k příležitosti alespoň jedno řešení připravené pro spoluprodání nebo řešení Microsoftu. Pokud chcete tento objekt přidružit k příležitosti, aktualizujte **formulář Opportunity** v aplikaci CRM.

- **Audit:** Záznam pro audit jen pro čtení pro synchronizaci s referenčními Partnerské centrum referenčními odkazy

### <a name="scenarios"></a>Scénáře

1. Synchronizace referenčních odkazů při vytvoření nebo aktualizaci referenčních seznamů v CRM a synchronizaci v Partnerské centrum:

   1. Přihlaste se k prostředí Salesforce CRM s uživatelem, který má přehled v **oddílu Opportunity** v CRM.

   1. Ujistěte se, že se při vytváření nové  příležitosti v prostředí Salesforce CRM nachází oddíl **Microsoft Partnerské centrum.**

   1. Příležitosti, které jsou úspěšně synchronizovány s Partnerské centrum, se identifikují ikonou ✔ salesforce CRM.
      :::image type="content" source="images/salesforce/salesforce-environment.png" alt-text="Snímek obrazovky s prostředím Salesforce":::

   1. Pokud chcete tuto příležitost synchronizovat s microsoft Partnerské centrum, ujistěte se, že jste v zobrazení karty nastavili následující pole:

      - **Jak může Microsoft pomoct?**: Pokud chcete vytvořit referenční seznam pro spoluprodácí, vyberte vhodnou možnost nápovědy.

        :::image type="content" source="images/salesforce/salesforce-help-option.png" alt-text="Snímek obrazovky, který znázorňuje, jak získat příslušná pole v zobrazení karty":::

      - **Synchronizace s Partnerské centrum:** Ano
      - **Kontakt zákazníka:** Pokud chcete vytvořit referenční seznam pro spoluprodácí, přidejte k této příležitosti kontakt zákazníka.
      - **Řešení Microsoftu:** Pokud chcete sdílet referenční seznam s Microsoftem, přidejte k této příležitosti platné řešení pro spoluprodání nebo řešení Microsoftu.

   1. Po nastavení možnosti Synchronizovat s Partnerské centrum **na** Ano **počkejte** 10 minut, přihlaste se ke svému Partnerské centrum účtu. Vaše referenční seznamy se synchronizují s aplikací Salesforce CRM a odkaz na referenční seznam se vyplní. Pokud dojde k selhání, do pole Audit se vyplní informace o chybě.

   1. Podobně když je možnost Synchronizovat **s Partnerské centrum** nastavená na **Ano,** pokud aktualizujete příležitost v Salesforce CRM, změny se synchronizují s vaším Partnerské centrum účtem.

2. Synchronizace referenčních seznamů při vytvoření nebo aktualizaci referenčního Partnerské centrum v prostředí Salesforce CRM:

    1. Přihlaste se k řídicímu [Partnerské centrum.](https://partner.microsoft.com/dashboard/home)

    1. V **nabídce vlevo** vyberte Referenční odkazy.

    1. Kliknutím na možnost New deal (Nová dohoda) Partnerské centrum nový referenční seznam pro spoludácí se ze seznamu.

    1. Přihlaste se k prostředí Salesforce CRM.

    1. Přejděte na **Otevřít příležitosti.** Referenční seznam vytvořený v Microsoft Partnerské centrum se teď synchronizuje v Salesforce CRM.

    1. Když vyberete synchronizovaný referenční seznam, vyplní se podrobnosti o zobrazení karty.

       :::image type="content" source="images/salesforce/salesforce-casino.png" alt-text="Snímek obrazovky se stránkou prodejní příležitosti Salesforce":::

>[!NOTE]
>**Potřebujete pomoc s nasazením?**
>Pokud potřebujete pomoc s nasazením konektoru referenčních doporučení ke spoluprodávu, můžete se zapojit do partnerského technického konzultanta. Mohou poskytovat pomoc při nasazení a osvědčené postupy pro úspěšnou implementaci.
>
>Další informace najdete v tématu Odeslání technické žádosti o [služby předprodeje a nasazení.](technical-benefits.md)

## <a name="next-steps"></a>Další kroky

- [Správa potenciálních zákazníků](manage-leads.md)

- [Správa příležitostí ke spoluprodeji](manage-co-sell-opportunities.md)

- [Webhooky Partnerského centra](/partner-center/develop/partner-center-webhooks)
