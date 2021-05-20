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
ms.openlocfilehash: 035a819020097ddee2230b5541e1b477d4b34c14
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148461"
---
# <a name="co-sell-connector-for-dynamics-365-crm-overview"></a>Přehled konektoru pro Dynamics 365 CRM pro předprodej

**Příslušné role**: Správce odkazů | Správce systému nebo úpravce systému v CRM

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

1. Vyberte tlačítko **Get it now (Získat)** a pak vyberte **Continue (Pokračovat).**

1. Zobrazí se stránka, kde můžete vybrat prostředí CRM (Dynamics 365) pro instalaci aplikace. Odsouhlaste podmínky a podmínky.

1. Průběh můžete monitorovat, a pokud se instalace nezdaří, můžete získat další podrobnosti v Power Automate výběrem možnosti **Zobrazit** historii v části **Řešení.**

1. Po dokončení instalace se vraťte na [stránku Power Automate](https://flow.microsoft.com) na **levé** straně vyberte Řešení. **Partnerské centrum referenčních seznamů pro Dynamics 365** je teď dostupná v **seznamu** Řešení.

1. Vyberte **Partnerské centrum referenčních seznamů pro Dynamics 365.** K dispozici Power Automate toky a entity.

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Snímek obrazovky znázorňuje dostupné CRM":::

## <a name="test-before-you-go-live"></a>Testování před živým vysíláním

Než nainstalujete, nakonfigurujete a přizpůsobíte Power Automate v produkčním prostředí, nezapomeňte řešení otestovat na pracovní instanci CRM. Budete muset:

- Nainstalujte Power Automate do pracovní instance prostředí CRM.
- Nakonfigurujte a přizpůsobte Power Automate v pracovním prostředí.
- Otestujte řešení na pracovní instanci CRM.
- Po úspěšném testu importujte jako spravované řešení do produkční instance.

## <a name="configure-the-solution"></a>Konfigurace řešení

1. Po instalaci řešení v instanci CRM se vraťte do Power Automate [.](https://flow.microsoft.com/)

1. V **rozevíracím** seznamu Prostředí v pravém horním rohu vyberte instanci CRM, do které jste nainstalovali Power Automate řešení.

1. Budete muset vytvořit připojení, která přidruží tyto tři uživatelské účty:

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

- Partnerské centrum registrace webhooku (Insider Preview)
- Vytvoření referenčního přehledu spoluproduování – Dynamics 365 na Partnerské centrum (Insider Preview)
- [Přizpůsobit] Vytvoření nebo získání podrobností z toku Dynamics 365
- Partnerské centrum dynamics 365 – pomocná funkce (Insider Preview)
- Partnerské centrum referenčních seznamů spoluproduování Microsoftu pro Dynamics 365 (Insider Preview)
- Partnerské centrum dynamics 365 (Insider Preview)
- Dynamics 365 na Partnerské centrum (Insider Preview)
- Dynamics 365 Opportunity to Partnerské centrum (Insider Preview)
- Dynamics 365 Microsoft Solutions to Partnerské centrum (Insider Preview)
 
## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Použití rozhraní API webhooku k registraci událostí změny prostředků

Pomocí rozhraní API Partnerské centrum webhooku můžete registrovat události změny prostředků. Tyto události změny se posílají na vaši adresu URL jako příspěvky HTTP.

1. Vyberte **Partnerské centrum Dynamics 365 (Insider Preview).**

1. Vyberte **ikonu** Upravit a vyberte **Při přijetí požadavku HTTP.**

1. Vyberte **ikonu Kopírovat** a zkopírujte zadanou adresu URL HTTP POST.

   :::image type="content" source="images/webhook-video.gif" alt-text="Snímek obrazovky znázorňuje použití webhooků k registraci změn prostředků":::

1. Vyberte **tok Partnerské centrum webhooku (Insider Preview)** Power Automate a pak vyberte **Spustit.**

1. Ujistěte **se, že** se v pravém podokně otevře okno Spustit tok, a vyberte **Pokračovat.**

1. Zadejte následující podrobnosti:

   - **Koncový bod triggeru HTTP:** Tato adresa URL byla zkopírována z předchozího kroku.
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
  - Upravte [Přizpůsobit] Vytvořte nebo získejte podrobnosti z **toku Dynamics 365,** přejděte do  části Vytvoření nebo aktualizace příležitosti v CRM a aktualizujte možnosti Vytvořit novou příležitost **a** Aktualizovat existující příležitosti a přiřaďte hodnotu **DealValue** ke správnému poli v CRM.  Odeberte také **přiřazení DealValue** z pole **Odhadované výnosy.**

- **Kód země účtu zákazníka:** Při vytváření nového referenčního seznamu je nutné zadat dvoupísmenný kód země (ISO 3166). Ve výchozím nastavení se kód země synchronizuje do pole účtu a z pole address1_country **v** CRM. Pokud máte v CRM jiné pole pro kód země, ze které se má synchronizovat:

   - Pro pole s kódem země, které nenílookup, v účtu, které obsahuje dvou písmeno kódu:
     - Aktualizujte **název pole Kód země** účtu zákazníka v proměnné prostředí Dynamics 365 názvem pole CRM. Ujistěte se, že zadáte název pole, nikoli jeho zobrazovaný název.
     - Upravte [Přizpůsobit] Vytvořte nebo získejte podrobnosti z  **toku Dynamics 365** a v  akci CRM přejděte na Vytvoření nebo získání zákaznického účtu a přiřaďte hodnotu Země ke správnému poli v CRM. Také odeberte přiřazení **hodnoty Země** z pole **Adresa 1: Země/oblast.**

   - Pole s kódem země založené na vyhledávání v účtu:
     - Přidejte do účtu nové vlastní pole a automaticky ho vyplňte dvoupísmenný kód země (ISO 3166) na základě hodnoty vybrané v poli založeném na vyhledávání a naopak.
     - Pokud chcete synchronizovat nové vlastní pole z CRM do a z aplikace, postupujte podle předchozích kroků pro pole s kódem země, která není v seznamu Partnerské centrum.

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

Po instalaci, konfiguraci a přizpůsobení řešení Power Automate můžete otestovat synchronizaci referenčních odkazů spoluprodáků mezi Dynamics 365 a Partnerské centrum.

### <a name="prerequisites"></a>Požadavky

Pokud chcete synchronizovat referenční Partnerské centrum napříč aplikacemi a Dynamics 365 CRM, Power Automate řešení jasně vymešká pole referenčních seznamů specifická pro Microsoft. Tato identifikace dává týmům prodejců možnost rozhodnout se, které referenční odkazy chce sdílet s Microsoftem pro spoluprodávač.

Sada vlastních polí a objektů se přidá jako součást instalace řešení. Uživatel s rolí správce CRM bude muset vytvořit samostatný oddíl CRM s vlastními **poli Opportunity.**

Následující vlastní pole by měla být součástí oddílu CRM:

- **Synchronizace s Partnerské centrum:** Jestli se má synchronizovat příležitost s Partnerské centrum. Ve výchozím nastavení má toto pole hodnotu Ne a váš prodejce musí explicitně nastavit možnost Ano, aby bylo možné sdílet příležitost s Microsoftem. Nové referenční odkazy sdílené z Partnerské centrum do CRM budou mít tuto hodnotu pole nastavenou na Ano.
- **Identifikátor referenčního** seznamu: Pole identifikátoru jen pro čtení pro Partnerské centrum referenčního seznamu.
- **Odkaz na referenční** seznam: Odkaz jen pro čtení referenčního seznamu v Partnerské centrum.
- **Jak může Microsoft pomoct?**: Pomoc od Microsoftu požadovaná pro referenční informace. Pokud chcete vytvořit referenční seznam pro spoluprodácí, vyberte vhodnou nápovědu od Microsoftu. Ke příležitosti k vytvoření referenčního seznamu pro spoluprodát musí být přidružený kontakt zákazníka. Pokud chcete vytvořit referenční seznam bez spoluproduování, toto pole nevytvářejte. Referenční seznam bez spoluproduování můžete kdykoli převést na referenční seznam pro spoluprodát výběrem příslušné možnosti požadované nápovědy.
- **Viditelnost referenčních Partnerské centrum** microsoftu: Vyberte viditelnost referenčního Partnerské centrum referenčního seznamu. Když ho prodejci Microsoftu zviditelní, může se referenční seznam bez spoluprodávače převést na spoluprodávač. Pokud je požadována nápověda Microsoftu, je referenční odkaz standardně viditelný prodejcům Microsoftu. Jakmile je toto pole označené jako viditelné, není možné ho vrátit zpět.
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

      - **Jak může Microsoft pomoct?**: Pokud chcete vytvořit referenční seznam pro spoluprodácí, vyberte vhodnou možnost nápovědy.

         :::image type="content" source="images/dynamic-3a.png" alt-text="Snímek obrazovky, který znázorňuje, jak získat příslušná pole v zobrazení karty":::

      - **Kontakt zákazníka:** Pokud chcete vytvořit referenční seznam pro spoluprodácí, přidejte k této příležitosti kontakt zákazníka.
      - **Synchronizovat s Partnerské centrum:** Ano.
      - **Řešení Microsoftu:** Pokud chcete sdílet referenční seznam s Microsoftem, přidejte k této příležitosti platné řešení pro spoluprodání nebo řešení Microsoftu.
      
        :::image type="content" source="images/dynamic-4a.png" alt-text="Snímek obrazovky zobrazující ID řešení":::

   1. Po vytvoření příležitosti v Dynamics 365 s možností Synchronizovat s Partnerské centrum nastavenou na Ano, počkejte 10 minut.  Pak se přihlaste ke svému Partnerské centrum účtu. Vaše referenční seznamy se budou synchronizovat s Dynamics 365 a **identifikátorem referenčního seznamu.** **Odkaz na** referenční seznam se vyplní. Pokud dojde k selhání, do **pole Audit** se vyplní informace o chybě.
     
    1. Podobně pro příležitost, která měla možnost Synchronizovat s **Partnerské centrum** nastavenou na Ano, pokud příležitost aktualizujete v Dynamics 365 CRM, změny se synchronizují ve vašem Partnerské centrum účtu.

    1. Příležitosti, které se úspěšně synchronizují s Partnerské centrum, se identifikují pomocí ✔icon v Dynamics 365.

1. Synchronizace referenčních odkazů při vytvoření nebo aktualizaci referenčního Partnerské centrum a synchronizována v prostředí Dynamics 365:

   1. Přihlaste se k řídicímu [Partnerské centrum.](https://partner.microsoft.com/dashboard/home)

   1. V **nabídce vlevo** vyberte Referenční odkazy.

   1. Výběrem možnosti New deal (Nová dohoda) Partnerské centrum nový referenční seznam pro **spoludácí** se na Partnerské centrum seznamu.

   1. Přihlaste se k prostředí Dynamics 365 CRM.

   1. Přejděte na **stránku Open Opportunities**. Referenční seznam vytvořený v Partnerské centrum se teď synchronizuje v Dynamics 365 CRM.

   1. Když vyberete synchronizovaný odkaz, vyplní se podrobnosti zobrazení karty.

## <a name="next-steps"></a>Další kroky

- [Správa potenciálních zákazníků](manage-leads.md)
- [Správa příležitostí ke spoluprodeji](manage-co-sell-opportunities.md)
- [Další informace o platformě Microsoft Power automatizaci](/power-automate/)
- [Webhooky Partnerského centra](/partner-center/develop/partner-center-webhooks)
