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
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Konektor pro společný prodej pro Salesforce CRM – přehled

**Příslušné role**: Správce odkazů | Správce systému nebo úpravce systému v CRM

Konektor pro spoluprodej v partnerském centru umožňuje prodejcům v rámci svých systémů CRM spolupracovat s Microsoftem. Nebudou se muset vyškolet k používání partnerského centra ke správě obchodů v rámci společného prodeje. Pomocí konektorů pro spoluprodeji můžete vytvořit nový společný prodejní odkaz, který bude kontaktovat prodejce Microsoftu, získat referenční údaje od prodejce Microsoftu, přijmout nebo odmítnout reference, upravit data o koupi, jako je třeba hodnota koupě a datum ukončení.  K těmto obchodům v rámci těchto spoluprodejů můžete také dostávat jakékoli aktualizace od prodejců Microsoftu. Všechny vaše odkazy fungují při práci v aplikaci CRM dle vašeho výběru a nikoli v partnerském centru. 

Řešení je založené na řešení Microsoft Power automatizuje a používá rozhraní API partnerského centra.

## <a name="before-you-install---pre-requisites"></a>Před instalací – požadavky

|**Témata**   |**Podrobnosti**   |**Odkazy**   |
|--------------|--------------------|------|
|ID Microsoft Partner Network |Potřebujete platné ID MPN.|Připojení k programu [MPN](https://partner.microsoft.com/)|
|Připravený společný prodej|Vaše řešení IP/Services musí být připravené k prodeji.|[Prodej pomocí Microsoftu](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Účet partnerského centra|ID MPN přidružené k tenantovi partnerského centra musí být stejné jako ID MPN přidružené k vašemu řešení společného prodeje. Před nasazením konektorů se můžete podívat na to, jestli máte na portálu partnerského centra zobrazený odkaz na svůj společný prodej.|[Správa vašeho účtu](create-user-accounts-and-set-permissions.md)|
|Role uživatelů partnerského centra|Zaměstnanec, který bude instalovat a používat konektory, musí být správcem odkazů.|[Přiřazování uživatelských rolí a oprávnění](create-user-accounts-and-set-permissions.md)|
|Salesforce CRM|Role uživatele CRM je správce systému nebo úpravce systému.|[Přiřazení rolí v Salesforce CRM](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|Zapnout účet toku automatizace|Aktivní účet [Power automatizuje](https://flow.microsoft.com) pro správce systému nebo úpravce systému CRM. Tento uživatel se musí před instalací přihlásit k [automatizaci](https://flow.microsoft.com) aspoň jednou.|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a>Instalace balíčku Salesforce pro vlastní pole Microsoftu 

Aby bylo možné synchronizovat odkazy v rámci partnerského centra a Salesforce CRM, musí řešení Power automat jasně identifikovat pole odkazů specifická pro společnost Microsoft. Tato vymezená část poskytuje partnerům partnerských prodejců možnost rozhodnout se, které referenční seznamy chtějí sdílet se společností Microsoft pro souběžný prodej.

1. V Salesforce aktivujte **poznámky** a přidejte je do seznamu souvisejících příležitostí. 
[Odkaz](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. **Týmy příležitostí** aktivujte pomocí následujících kroků: 
    - V instalačním programu použijte pole **Rychlé hledání** k vyhledání nastavení týmu příležitostí.
    - Podle potřeby definujte nastavení.
[Odkaz](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. V Salesforce nainstalujte vlastní pole a objekty pomocí [instalačního programu balíčku](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV). Tento balíček použijte k instalaci balíčku do libovolné společnosti.

>[!NOTE]
>Pokud instalujete do izolovaného prostoru (sandbox), je nutné nahradit počáteční část adresy URL http://test.salesforce.com

4. V Salesforce přidejte řešení Microsoftu do seznamu souvisejících **příležitostí** . Po přidání vyberte ikonu **klíče** a aktualizujte vlastnosti.

## <a name="best-practice-test-before-you-go-live"></a>Osvědčené postupy: test před zahájením provozu

Než nainstalujete, nakonfigurujete a přizpůsobíte řešení Power Automate v produkčním prostředí, ujistěte se, že řešení otestujete v pracovní instanci CRM.

- Nainstalujte řešení Microsoft Power automatizuje do přípravného prostředí/instance CRM.

- Vytvořte kopii řešení a spusťte konfiguraci a automatizujte vlastní nastavení toků v přípravném prostředí.

- Otestujte řešení na pracovní instanci/CRM.

- Po úspěšném dokončení naimportujte jako spravované řešení do produkční instance.

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>Nainstalovat synchronizaci odkazů partnerského centra pro Salesforce CRM

1. V pravém horním rohu vyberte **prostředí** k [automatizaci](https://flow.microsoft.com) a vyberte prostředí. Zobrazí se vám dostupné instance CRM.

2. V rozevíracím seznamu v pravém horním rohu vyberte příslušnou instanci CRM.

3. Na levém navigačním panelu vyberte **řešení** .

4. V horní nabídce vyberte odkaz **otevřít AppSource** .

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Otevřete AppSource.":::

5. V místní obrazovce vyhledejte **konektory odkazů partnerského centra pro Salesforce** .  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Produktu.":::

6. Vyberte tlačítko **získat nyní** a potom **pokračujte**.

7. Otevře se stránka, kde můžete vybrat prostředí Salesforce CRM k instalaci aplikace.  Vyjádřit souhlas s podmínkami a ujednáními.

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="Dostupné CRMS.":::

8. Pak budete přesměrováni na stránku **spravovat vaše řešení** .  Přejděte na "odkazy na partnerské Centrum" pomocí tlačítek se šipkami ve spodní části stránky. **Naplánovaná instalace** by se měla objevit u řešení s odkazy partnerského centra. Instalace bude trvat 10-15 minut.

9. Po dokončení instalace přejděte zpátky na [Power](https://flow.microsoft.com) automat a vyberte **řešení** z navigační oblasti vlevo. Všimněte si, že v seznamu řešení je k dispozici **synchronizace odkazů partnerského centra pro Salesforce** .

10. Vyberte **synchronizaci odkazů z partnerského centra pro Salesforce**. K dispozici jsou tyto toky a entity automatizace pro napájení:

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Toky Salesforce.":::



## <a name="configure-the-solution"></a>Konfigurace řešení

1. Po instalaci řešení do instance CRM přejděte zpátky na [Power](https://flow.microsoft.com/)automat.

2. V rozevíracím seznamu **prostředí** v pravém horním rohu vyberte instanci CRM, do které jste nainstalovali řešení Power automatizuje.
3. Budete muset vytvořit připojení, která přiřadí tři uživatelské účty:
    - Uživatel partnerského centra s přihlašovacími údaji správce odkazů
    - Události Partnerského centra
    - Správce CRM s Power Automate automatizuje v řešení.
4. V levém navigačním panelu vyberte **připojení** a v seznamu vyberte řešení partnerského centra pro partnery.

5. Vytvořte připojení kliknutím na **vytvořit připojení**.

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Vytvořte připojení.":::

- Na panelu hledání v pravém horním rohu vyhledejte odkazy na partnerské Centrum (Preview).

- Vytvořte připojení pro uživatele partnerského centra s rolí přihlašovacích údajů správce odkazů.

-  Potom vytvořte připojení událostí partnerského centra pro uživatele partnerského centra s přihlašovacími údaji správce odkazů.

- Vytvořte připojení pro Salesforce pro uživatele správce CRM.

-  Po přidání všech připojení byste měli ve svém prostředí zobrazit následující připojení:

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Sledujte připojení.":::

### <a name="edit-the-connections"></a>Upravit připojení

1. Vraťte se na stránku řešení a vyberte **výchozí řešení**.  Kliknutím na tlačítko **vše** vyberte **odkaz připojení (Preview)** .
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Zahájit úpravu konektoru":::

2. Jednotlivá připojení upravte jednotlivě výběrem ikony tři tečky. Přidejte příslušná připojení.

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Upravit konektory.":::

3. Zapněte toky v následujícím pořadí:

- Partnerské centrum registrace webhooku (Insider Preview)
- Vytvoření referenčního odkazu pro spoluprodej – Salesforce pro Partnerské centrum (Insider Preview)
- Partnerské centrum referenčních doporučení spoluprodeje Microsoftu pro Salesforce (Insider Preview)
- Partnerské centrum salesforce (Insider Preview)
- Salesforce na Partnerské centrum (Insider Preview)
- Salesforce Opportunity to Partnerské centrum (Insider Preview)
- Salesforce – řešení Microsoftu pro Partnerské centrum (Insider Preview)

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Použití rozhraní WEBHOOK API k registraci událostí změny prostředků

Rozhraní PARTNERSKÉ CENTRUM API webhooku umožňují registrovat události změny prostředků. Tyto události změny se posílají na vaši adresu URL jako příspěvky HTTP.

1. Pokud chcete zaregistrovat adresu URL, **Partnerské centrum toku vyberte Registrace webhooku (Insider** Power Automate Preview).

2. Přidejte připojení pro uživatele (a.) s přihlašovacími údaji správce referenčních Partnerské centrum (b.) a Partnerské centrum událostmi, jak je zvýrazněno níže.

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Aktivační událost.":::

3. Při těchto aktualizacích se zobrazí

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooky.":::

4. Uložte změny a vyberte **Zapnout**.

   Pokud chcete Partnerské centrum, aby webhooky naslouchaly změnám událostí, proveďte následující kroky:

5. Vyberte **Partnerské centrum Salesforce CRM (Insider Preview).**

6. Vyberte **ikonu** Upravit a vyberte **Při přijetí požadavku HTTP.**

7. Vyberte **ikonu Kopírovat** a zkopírujte zadanou adresu URL HTTP POST.

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Zkopírujte adresu URL.":::

8. Teď vyberte tok Partnerské centrum webhooku (Insider Preview) a Power Automate **Spustit.**

9. Ujistěte se, že se v pravém podokně otevře okno Spustit tok, a vyberte **Pokračovat.**

10. Zadejte následující podrobnosti:

    1. **Koncový bod triggeru HTTP:** Adresa URL zkopírovaná z předchozího kroku

    2. **Události k registraci:**"referenční seznam byl vytvořen" a "aktualizován referenční seznam".

    3. **Přepsat existující koncové body triggeru, pokud jsou k dispozici:** Ano (Tím se přepíšou všechny existující koncové body.)

11. Vyberte **Spustit a** pak vyberte **Hotovo.**

Webhook teď může naslouchat událostem vytváření a aktualizace.

## <a name="customize-synchronization-steps"></a>Přizpůsobení kroků synchronizace

Když se referenční seznam pro spoluprodácí synchronizuje mezi systémem Partnerské centrum a systémem CRM, zobrazí se tady pole synchronizovaná v Partnerské centrum počítači.

Systémy CRM jsou často vysoce přizpůsobené. Můžete přizpůsobit Power Automate toky. Postupujte podle průvodce mapováním polí a v případě potřeby proveďte odpovídající změny v krocích Power Automate toků.  K dispozici jsou partnerská centra Microsoftu pro mapování CRM, ale na základě prostředí CRM se můžete rozhodnout pole dále přizpůsobit.

Několik kroků každého z těchto toků Power Automate přizpůsobit podle vašich potřeb. Tady jsou příklady dostupných přizpůsobení:

1. Pokud chcete přizpůsobit pole pro události vytvoření nebo aktualizace v Partnerské centrum se synchronizací referenčních seznamu CRM:

   1. Vyberte Partnerské centrum Salesforce CRM (Insider Preview).

   2. Pokud **chcete upravit** nebo přizpůsobit tok Power Automate upravit.

   3. Vyberte **(Rozsah) Synchronizovat zájemce nebo příležitost.**

2. Pokud chcete přizpůsobit mapování polí CRM pro události vytváření, vyberte Pokud se jedná **o novou sdílenou příležitost, pak**. Pokud ano, vyberte dílčí **krok** a potom rozbalte položku Creating a new opportunity in the CRM (Vytvoření **nové příležitosti v CRM).** Mapování v této části můžete upravit pomocí Průvodce mapováním polí.

   1. Pokud chcete přizpůsobit mapování polí CRM pro události aktualizací, vyberte krok "(Rozsah) Synchronizovat zájemce nebo příležitost".

   2. Vyberte **Pokud se jedná o aktualizaci příležitosti, pak**. Pokud ano, vyberte dílčí **krok** a pak rozbalte If difference between the opportunity objects in Partnerské centrum and CRM (Pokud je rozdíl mezi objekty příležitostí v Partnerské centrum **a CRM).**  

   3. Vyberte **Pokud ano a** pak Aktualizovat existující **příležitost.**

3. Přizpůsobení polí synchronizace referenčních seznamů CRM do pc pro události aktualizace:

   1. Pokud **chcete upravit**  nebo přizpůsobit tok Power Automate upravit.

   2. Vyberte **(Rozsah) Synchronizovat příležitost.**

   3. Pokud chcete přizpůsobit mapování polí CRM (na základě průvodce mapováním polí) pro aktualizační události, vyberte Pokud je mezi objekty zájemců v aplikaci Partnerské centrum a **CRM rozdíl, pak vyberte**.

   4. Pokud ano, vyberte dílčí **krok** a potom rozbalte krok Aktualizovat referenční **seznam daty příležitostí**.

   Mapování v této části můžete upravit na základě Průvodce mapováním polí.

4. Chcete přizpůsobit pole synchronizace referenčních seznamů CRM do pc pro vytváření událostí?

   1. Pokud **chcete upravit**  nebo přizpůsobit tok Power Automate upravit.

   2. Vyberte **(Rozsah) Synchronizace referenčních seznamu.**

   3. Pokud chcete přizpůsobit mapování polí CRM (na základě průvodce mapováním polí) pro vytváření událostí, vyberte Create Microsoft Referral (Vytvořit **referenční seznam Microsoftu).**

Mapování v této části můžete upravit na základě Průvodce mapováním polí.


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>Synchronizace referenčních odkazů end-to-end bi-directional co-sell

Po instalaci, konfiguraci a přizpůsobení řešení Power Automate můžete otestovat synchronizaci referenčních odkazů spoluprodeje mezi salesforce CRM a Partnerské centrum.

### <a name="pre-requisites"></a>Požadavky

Pokud chcete synchronizovat referenční Partnerské centrum napříč aplikacemi a salesforce CRM, Power Automate řešení musí jasně vytyčovat pole referenčních seznamů specifická pro Microsoft. Tato identifikace poskytuje týmům prodejců možnost rozhodnout se, které referenční odkazy chce sdílet s Microsoftem pro spoluprodávač.

Sada vlastních polí je k dispozici jako součást synchronizace referenčních  Partnerské centrum referenčních seznamů pro entitu Opportunity řešení Salesforce CRM. Uživatel s rolí správce CRM bude muset vytvořit samostatný oddíl CRM s vlastními **poli Opportunity.**

Následující vlastní pole by měla být součástí oddílu CRM:

- **Synchronizace s Partnerské centrum:** Jestli se má synchronizovat příležitost s Microsoft Partnerské centrum

- **Identifikátor referenčního** seznamu: Pole identifikátoru jen pro čtení pro referenční Partnerské centrum referenčního seznamu

- **Odkaz na referenční** seznam: Odkaz jen pro čtení referenčního seznamu v Microsoft Partnerské centrum

- **Jak může Microsoft pomoci:** Pomoc od Microsoftu požadovaná pro referenční informace

- **Produkty:** Seznam produktů přidružených k této příležitosti

- **Audit:** Záznam pro audit jen pro čtení pro synchronizaci s referenčními Partnerské centrum referenčními odkazy

### <a name="scenarios"></a>Scénáře:

1. Synchronizace referenčních odkazů při vytvoření nebo aktualizaci referenčních seznamů v CRM a synchronizaci v Partnerské centrum:

   1. Přihlaste se k prostředí Salesforce CRM s uživatelem, který má přehled v **části Opportunity** v CRM.

   2. Při vytváření nové příležitosti v prostředí Salesforce CRM se ujistěte, že se nachází následující část.

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Prostředí Salesforce.":::

   3. Pokud chcete tuto příležitost synchronizovat s microsoft Partnerské centrum, ujistěte se, že jste v zobrazení karty nastavili následující pole:

       - "Synchronizace s Partnerské centrum": Ano
       - "Jak může Microsoft pomoct?": Vyberte jednu z následujících možností:
       - Produkty: ID řešení produktu

   4. Po nastavení možnosti Synchronizovat s  **Partnerské centrum** na **Ano,** počkejte 10 minut, přihlaste se ke svému Partnerské centrum účtu. Vaše referenční seznamy se synchronizují s aplikací Salesforce CRM.

   5. Když je možnost Synchronizovat s Partnerské centrum nastavená na Ano, při aktualizaci příležitosti v Salesforce CRM se změny synchronizují s vaším Partnerské centrum účtem.

   6. Příležitosti, které se úspěšně synchronizují s Partnerské centrum, se identifikují pomocí ✔icon v Salesforce CRM.

2. Synchronizace referenčních seznamů při vytvoření nebo aktualizaci referenčního Partnerské centrum v prostředí Salesforce CRM:

    1. Přihlaste se k řídicímu [Partnerské centrum.](https://partner.microsoft.com/dashboard/home)

    2. V **nabídce vlevo** vyberte Referenční odkazy.

    3. Kliknutím na možnost New deal (Nová dohoda) Partnerské centrum nový referenční seznam pro spoludácí se na Partnerské centrum.

    4. Přihlaste se k prostředí Salesforce CRM.

    5. Přejděte na **Otevřít příležitosti.** Referenční seznam vytvořený v Microsoft Partnerské centrum se teď synchronizuje v Salesforce CRM.

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Obrazovka prodejních příležitostí Salesforce":::

    6. Když vyberete synchronizovaný referenční seznam, vyplní se podrobnosti o zobrazení karty.

## <a name="next-steps"></a>Další kroky

- [Správa potenciálních zákazníků](manage-leads.md)

- [Správa příležitostí ke spoluprodeji](manage-co-sell-opportunities.md)

- [Webhooky Partnerského centra](/partner-center/develop/partner-center-webhooks)
