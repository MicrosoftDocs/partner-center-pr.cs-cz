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
ms.openlocfilehash: 87083c8124762f0952b0c98cbc209164151dcb0c
ms.sourcegitcommit: 6a6e8f9af0a58b32770c7fce9f567dd4795b9797
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/29/2021
ms.locfileid: "113029188"
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

   :::image type="content" source="images/cosellconnectors/open-appsource.png" alt-text="Snímek obrazovky, který zobrazuje otevřený AppSource.":::

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

1. Vraťte se na stránku **řešení** , vyberte **synchronizace odkazů partnerského centra pro Dynamics 365** a potom tok zapněte výběrem ikony se třemi tečkami vedle každého toku v následujícím pořadí. Pokud narazíte na problémy při zapnutí toku, Projděte si téma [Postup přizpůsobení](connector-dynamics.md#customize-synchronization-steps) a [Postup řešení potíží](connectors-troubleshoot.md).

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

K registraci událostí změn prostředků můžete použít rozhraní API Webhooku partnerského centra. Tyto události změny se na vaši adresu URL odesílat jako příspěvky HTTP.

1. Vyberte **Partnerské centrum Dynamics 365 (Insider Preview).**

1. Vyberte **ikonu** Upravit a vyberte **Při přijetí požadavku HTTP.**

1. Vyberte **ikonu Kopírovat** a zkopírujte zadanou adresu URL HTTP POST.

   :::image type="content" source="images/webhook-video.gif" alt-text="Snímek obrazovky znázorňuje použití webhooků k registraci změn prostředků":::

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

Postupujte podle průvodce mapováním polí a v případě potřeby proveďte příslušné změny v tématu [Přizpůsobit] Vytvoření nebo získání podrobností z toku **Dynamics 365** nebo proměnných prostředí. Ne aktualizujte žádné jiné toky v Power Automate, protože to může mít vliv na budoucí upgrady řešení.

K dispozici jsou následující přizpůsobení:

- **Zobrazit značku zaškrtnutí v** názvu příležitosti: Ve výchozím nastavení se vedle názvu příležitosti zobrazí značka zaškrtnutí, která označuje, že synchronizace mezi Partnerské centrum a Dynamics 365 CRM probíhá úspěšně. Podobně se křížové označení zobrazí, pokud synchronizace selže. Pokud se chcete vyhnout přidání zaškrtnutí nebo křížové značky  v názvu příležitosti, nastavte aktuální hodnotu značky zaškrtnutí Zobrazit v proměnné prostředí název příležitosti na Ne.
- **Hodnota dohody:** Ve výchozím nastavení se hodnota dohody z Partnerské centrum bude synchronizovat do a **z** odhadované hodnoty v CRM. Pokud máte v CRM jiné pole pro hodnotu dohody, ze které se má synchronizovat:

  - Aktualizujte **název pole Hodnoty** dohody v proměnné prostředí Dynamics 365 názvem pole CRM. Ujistěte se, že zadáte název pole, nikoli jeho zobrazovaný název.
  - Upravte [Přizpůsobit] Vytvořte nebo získejte podrobnosti z **toku Dynamics 365,** přejděte do  části Vytvoření nebo aktualizace příležitosti v CRM a aktualizujte možnosti Vytvořit novou příležitost **a** Aktualizovat existující příležitosti a přiřaďte hodnotu **DealValue** ke správnému poli v CRM.  Odeberte také **přiřazení DealValue** z pole **Odhadované výnosy.**

- **Kód země účtu zákazníka:** Při vytváření nového referenčního seznamu je nutné zadat dvoupísmenný kód země (ISO 3166). Ve výchozím nastavení se kód země synchronizuje do pole účtu a z pole address1_country **v** CRM. Pokud máte v CRM jiné pole pro kód země, ze které se má synchronizovat:

  - Pro pole s kódem země, které nenílookup, v účtu, které obsahuje dvou písmeno kódu:
    - Aktualizujte **název pole Kód země** účtu zákazníka v proměnné prostředí Dynamics 365 názvem pole CRM. Ujistěte se, že zadáte název pole, nikoli jeho zobrazovaný název.
    - Upravte [Přizpůsobit] Vytvořte nebo získejte podrobnosti z  **toku Dynamics 365** a v  akci CRM přejděte na Vytvoření nebo získání zákaznického účtu a přiřaďte hodnotu Země ke správnému poli v CRM. Také odeberte přiřazení **hodnoty Země** z pole **Adresa 1: Země/oblast.**

  - Pole s kódem země založené na vyhledávání v účtu:
    - Přidejte do účtu nové vlastní pole a automaticky ho naplňte dvoupísmenný kód země (ISO 3166) na základě hodnoty vybrané v poli založeném na vyhledávání a naopak.
    - Pokud chcete synchronizovat nové vlastní pole z CRM do a z aplikace, postupujte podle předchozích kroků pro pole s kódem země, která není v seznamu Partnerské centrum.

- Pole příležitosti: Pokud v  příležitosti existují povinná pole, která je potřeba naplnit, upravte [Přizpůsobit]  Vytvoření nebo získání podrobností z toku **Dynamics 365,** přejděte do části Vytvoření nebo aktualizace příležitosti v CRM **a** aktualizujte akci Vytvořit novou příležitost a přiřaďte hodnoty povinným polím na základě vašich obchodních požadavků. 
- Pole potenciálních **zákazníků:** Pokud  je potřeba vyplnit povinná pole zájemce, upravte [Přizpůsobit] Vytvoření nebo  získání podrobností z toku **Dynamics 365,** přejděte do části Vytvoření nebo aktualizace potenciálního zákazníka v CRM **a** aktualizujte akci Vytvořit nového potenciálního zákazníka a přiřaďte hodnoty povinným polím na základě vašich obchodních požadavků.
- **Zákaznický účet:** Když se nový referenční seznam synchronizuje z Partnerské centrum do CRM, řešení Power Automate se pokusí vyhledat existující účet v CRM pomocí názvu společnosti zákazníka a PSČ. Pokud ho nenajde, vytvoří se v CRM nový zákaznický účet. Pokud chcete aktualizovat kritéria vyhledávání a podrobnosti o vytvoření nového účtu, upravte **tok [Customize] Create or Get Details from Dynamics 365** (Vytvořit nebo získat podrobnosti o účtu zákazníka) a v akci CRM (Crm) přejděte na Create or get **customer account**(Vytvořit nebo získat zákaznický účet). 

## <a name="update-environment-variable"></a>Aktualizace proměnné prostředí

Aktualizace hodnoty proměnné prostředí:

1. Přejděte na **stránku Řešení a** vyberte Výchozí **řešení.** Výběrem možnosti **All (Vše) vyberte Environment** **Variable** (Proměnná prostředí).

1. Vyberte proměnnou prostředí pro hodnotu, kterou je potřeba aktualizovat, a vyberte **Upravit** pomocí ikony se třemi tečkami.

1. Aktualizovat **aktuální hodnotu** (ne aktualizovat výchozí **hodnotu)** pomocí možnosti **Nová hodnota** a poskytnutím hodnoty. Hodnota musí odpovídat datovému typu proměnné. Datový typ Ano nebo Ne například přijme hodnotu Ano nebo Ne.

   :::image type="content" source="images/cosellconnectors/environment-variables-video.gif" alt-text="Snímek obrazovky znázorňuje aktualizaci proměnných prostředí":::

## <a name="end-to-end-bidirectional-co-sell-referral-synchronization"></a>Synchronizace referenčních odkazů s úplným obousměrným spoluprodážením

Po instalaci, konfiguraci a přizpůsobení řešení Power Automate můžete otestovat synchronizaci referenčních odkazů spoluprodáků mezi Dynamics 365 a Partnerské centrum.

### <a name="prerequisites"></a>Požadavky

Pokud chcete synchronizovat referenční Partnerské centrum a Dynamics 365 CRM, řešení Power Automate přehledně vymešká pole referenčních seznamů specifická pro Microsoft. Tato identifikace dává týmům prodejců možnost rozhodnout, které referenční reference chce sdílet s Microsoftem pro spoluprodávač.

Jako součást instalace řešení se přidá sada vlastních polí a objektů. Uživatel s rolí správce CRM bude muset vytvořit samostatný oddíl CRM s vlastními **poli Opportunity.**

Následující vlastní pole by měla být součástí oddílu CRM:

- **Synchronizace s Partnerské centrum:** Jestli se má synchronizovat příležitost s Partnerské centrum. Ve výchozím nastavení má toto pole hodnotu Ne a prodejce musí explicitně nastavit možnost Ano, aby bylo možné sdílet příležitost s Microsoftem. Nové referenční odkazy sdílené z Partnerské centrum do CRM budou mít tuto hodnotu pole nastavenou na Ano.
- **Identifikátor referenčního** seznamu: Pole identifikátoru jen pro čtení pro Partnerské centrum referenčního seznamu.
- **Odkaz na referenční** seznam: Odkaz jen pro čtení referenčního seznamu v Partnerské centrum.
- **Jak může Microsoft pomoct?**: Pomoc od Microsoftu požadovaná pro referenční informace. Pokud chcete vytvořit referenční seznam pro spoluprodácí, vyberte vhodnou nápovědu od Microsoftu. Ke příležitosti k vytvoření referenčního seznamu pro spoluprodát musí být přidružený kontakt zákazníka. Pokud chcete vytvořit referenční seznam bez spoluproduování, toto pole nevytvářejte. Referenční seznam bez spoluproduování můžete kdykoli převést na referenční seznam pro spoluprodát výběrem příslušné možnosti požadované nápovědy.
- **Viditelnost referenčních Partnerské centrum** microsoftu: Vyberte viditelnost referenčního Partnerské centrum referenčního seznamu. Když ho prodejci Microsoftu zviditelní, může se referenční seznam bez spoluprodávače převést na spoluprodávač. Pokud je požadována nápověda Microsoftu, je referenční odkaz standardně viditelný prodejcům Microsoftu. Jakmile je toto pole označené jako viditelné, není možné ho vrátit zpět.
- **Identifikátor Microsoft CRM:** Když Microsoft vytvoří referenční seznam pro spoluprodávaného prodeje a přijme ho, naplní se toto pole identifikátorem CRM od Microsoftu.
- **Produkty: Zastaralé:** Toto pole nepoužívejte nebo ho přidejte do části CRM. Je k dispozici pouze pro zpětnou kompatibilitu. Použijte Partnerské centrum řešení.
- **Audit:** Záznam pro audit jen pro čtení pro synchronizaci s referenčními Partnerské centrum referenčními odkazy.
- **Microsoft Partnerské centrum Solutions:** Vlastní objekt pro přidružení řešení připravených ke spoluproduování nebo řešení Microsoftu s příležitostí. Z příležitosti je možné přidat nebo odebrat jedno nebo více řešení. Před sdílením s Microsoftem je nutné přidat k příležitosti alespoň jedno připravené řešení pro spoluprodání nebo řešení Microsoftu. Pokud chcete tento objekt přidružit k příležitosti, aktualizujte **formulář Opportunity** v aplikaci CRM.

  Ve formuláři Opportunity vyberte **příslušnou** kartu a přidejte podmřížku, jak je znázorněno tady.

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="Snímek obrazovky znázorňuje formulář příležitosti":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="Snímek obrazovky znázorňuje řešení Microsoftu":::

- Po přidání řešení Microsoftu můžete předem doplnit podrobnosti o řešení připraveném ke spoluprodávce, aby je prodejci nemusí přidávat. Pokud chcete přidat podrobnosti o novém řešení, přejděte v  CRM na objekt Microsoft Solution Details a vyberte Přidat záznam, abyste přidali jednu položku, nebo pomocí možnosti Nahrát do **Excelu** přidejte více položek.

  :::image type="content" source="images/cosellconnectors/dynamics-solution-1.png" alt-text="Snímek obrazovky s podrobnostmi o novém řešení Microsoftu":::

### <a name="scenarios"></a>Scénáře

1. Synchronizace referenčních odkazů při vytvoření nebo aktualizaci referenčních seznamů v CRM a synchronizaci v Partnerské centrum:

   1. Přihlaste se k prostředí Dynamics 365 CRM pomocí uživatele, který má přehled v části **Opportunity** (Příležitost) aplikace CRM.

   1. Při vytváření **nové příležitosti v prostředí** Dynamics 365 se ujistěte, že je k dispozici oddíl Microsoft Partnerské centrum.

      :::image type="content" source="images/cosellconnectors/dynamics-solution-2.png" alt-text="Snímek obrazovky znázorňuje novou příležitost":::

   1. Pokud chcete tuto příležitost synchronizovat Partnerské centrum, ujistěte se, že jste v zobrazení karty nastavili následující pole:

      - **Jak může Microsoft pomoct?**: Pokud chcete vytvořit referenční seznam pro spoluprodácí, vyberte vhodnou možnost nápovědy.

         :::image type="content" source="images/cosellconnectors/dynamics-solution-3.png" alt-text="Snímek obrazovky, který znázorňuje, jak získat příslušná pole v zobrazení karty":::

      - **Kontakt zákazníka:** Pokud chcete vytvořit referenční seznam pro spoluprodácí, přidejte k této příležitosti kontakt zákazníka.
      - **Synchronizovat s Partnerské centrum:** Ano.
      - **Řešení Microsoftu:** Pokud chcete sdílet referenční seznam s Microsoftem, přidejte k této příležitosti platné řešení pro spoluprodání nebo řešení Microsoftu.

        :::image type="content" source="images/cosellconnectors/dynamics-solution-4.png" alt-text="Snímek obrazovky zobrazující ID řešení":::

   1. Po vytvoření příležitosti v Dynamics 365 s možností Synchronizovat s Partnerské centrum nastavenou na Ano, počkejte 10 minut.  Pak se přihlaste ke svému Partnerské centrum účtu. Vaše referenční seznamy se budou synchronizovat s Dynamics 365 a **identifikátorem referenčního seznamu.** **Odkaz na** referenční seznam se vyplní. Pokud dojde k selhání, pole **Audit** se naplní informacemi o chybě.

      1. Podobně pro příležitost, která měla možnost Synchronizovat s **Partnerské centrum** nastavenou na Ano, pokud příležitost aktualizujete v Dynamics 365 CRM, změny se synchronizují ve vašem Partnerské centrum účtu.

      1. Příležitosti, které se úspěšně synchronizují s Partnerské centrum, se identifikují pomocí ✔icon v Dynamics 365.

1. Synchronizace referenčních odkazů při vytvoření nebo aktualizaci referenčního Partnerské centrum a synchronizována v prostředí Dynamics 365:

   1. Přihlaste se k řídicímu [Partnerské centrum.](https://partner.microsoft.com/dashboard/home)

   1. V **nabídce vlevo** vyberte Referenční odkazy.

   1. Výběrem možnosti New deal (Nová dohoda) Partnerské centrum nový referenční seznam pro **spoludácí** se na Partnerské centrum seznamu.

   1. Přihlaste se k prostředí Dynamics 365 CRM.

   1. Přejděte na **stránku Open Opportunities**. Referenční seznam vytvořený v Partnerské centrum se teď synchronizuje v Dynamics 365 CRM.

   1. Když vyberete synchronizovaný referenční seznam, vyplní se podrobnosti o zobrazení karty.

## <a name="next-steps"></a>Další kroky

- [Správa potenciálních zákazníků](manage-leads.md)
- [Správa příležitostí ke spoluprodeji](manage-co-sell-opportunities.md)
- [Další informace o platformě Microsoft Power Automate Platform](/power-automate/)
- [Webhooky Partnerského centra](/partner-center/develop/partner-center-webhooks)
