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
ms.openlocfilehash: fa9b35343e1251cfce5caff107de8dff344f4e68
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148410"
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
|Partnerské centrum rolí uživatelů|Zaměstnanec, který bude tyto konektory instalovat a používat, musí být správcem referenčních seznamu.|[Přiřazování uživatelských rolí a oprávnění](create-user-accounts-and-set-permissions.md)|
|Salesforce CRM|Role uživatele CRM je Správce systému nebo Úpravce systému.|[Přiřazení rolí v Salesforce CRM](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|Power Automate toku|Aktivní účet [Power Automate](https://flow.microsoft.com) správce systému CRM nebo úpravce systému. Tento uživatel by se měl [Power Automate](https://flow.microsoft.com) před instalací alespoň jednou přihlásit.|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a>Instalace balíčku Salesforce pro vlastní pole Microsoftu 

Aby bylo možné synchronizovat referenční Partnerské centrum napříč aplikacemi a salesforce CRM, Power Automate řešení musí jasně identifikovat pole referenčních seznamů specifická pro Microsoft. Toto vyněcování poskytuje týmům prodejců partnerů možnost rozhodnout se, které referenční reference chce sdílet s Microsoftem pro spoluprodávku.

1. V Salesforce aktivujte **Poznámky** a přidejte je do seznamu příležitostí. 
[Odkaz](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. Aktivujte **týmy příležitostí** pomocí následujících kroků: 
    - V instalačním programu vyhledejte **pomocí pole Rychlé** hledání nastavení týmu příležitostí.
    - Definujte nastavení podle potřeby.
[Odkaz](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. V Salesforce nainstalujte vlastní pole a objekty pomocí [instalačního programu balíčků](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV). Tento nástroj použijte k instalaci balíčku do jakékoli společnosti.

>[!NOTE]
>Pokud instalujete do sandboxu, musíte počáteční část adresy URL nahradit za . http://test.salesforce.com

4. V Salesforce přidejte řešení Microsoftu do **seznamu souvisejícího** s příležitostí. Po přidání vyberte ikonu **klíče** a aktualizujte vlastnosti.

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

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Otevřít AppSource":::

5. V místní obrazovce vyhledejte **konektory odkazů partnerského centra pro Salesforce** .  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. Vyberte tlačítko **získat nyní** a potom **pokračujte**.

7. Otevře se stránka, kde můžete vybrat prostředí Salesforce CRM k instalaci aplikace.  Vyjádřit souhlas s podmínkami a ujednáními.

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="Dostupné CRMS":::

8. Pak budete přesměrováni na stránku **spravovat vaše řešení** .  Přejděte na "odkazy na partnerské Centrum" pomocí tlačítek se šipkami ve spodní části stránky. **Vedle řešení** referenčních Partnerské centrum by se měla zobrazit naplánovaná instalace. Instalace bude trvat 10 až 15 minut.

9. Po dokončení instalace přejděte zpět na stránku [Power Automate](https://flow.microsoft.com) **v** levé navigační oblasti vyberte Řešení. Všimněte **si Partnerské centrum synchronizace referenčních** seznamu pro Salesforce dostupná v seznamu Řešení.

10. Vyberte **Partnerské centrum referenčních seznamu pro Salesforce.** K dispozici Power Automate toky a entity:

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Toky Salesforce":::



## <a name="configure-the-solution"></a>Konfigurace řešení

1. Po instalaci řešení v instanci CRM přejděte zpět na Power Automate [.](https://flow.microsoft.com/)

2. V **rozevíracím** seznamu Prostředí v pravém horním rohu vyberte instanci CRM, do které jste nainstalovali Power Automate řešení.
3. Budete muset vytvořit připojení, která přidruží tyto tři uživatelské účty:
    - Partnerské centrum uživatele s přihlašovacími údaji správce referenčních odkazů
    - Události Partnerského centra
    - Správce CRM s Power Automate toky v řešení.
4. V **levém** navigačním panelu vyberte Připojení a ze seznamu vyberte Partnerské centrum referenčních seznamech.

5. Vytvořte připojení kliknutím na **Vytvořit připojení.**

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Vytvoření připojení":::

- Na panelu Partnerské centrum v pravém horním rohu vyhledejte referenční Partnerské centrum (Preview).

- Vytvořte pro svého uživatele Partnerské centrum s rolí přihlašovacích údajů správce referenčních seznamů.

-  Dále vytvořte připojení Partnerské centrum události pro vašeho Partnerské centrum uživatele s přihlašovacími údaji správce referenčních seznamů.

- Vytvořte připojení pro Salesforce pro uživatele správce CRM.

-  Po přidání všech připojení by se ve vašem prostředí měla zobrazit následující připojení:

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Sledovat připojení":::

### <a name="edit-the-connections"></a>Upravit připojení

1. Vraťte se na stránku řešení a vyberte **výchozí řešení**.  Kliknutím na tlačítko **vše** vyberte **odkaz připojení (Preview)** .
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Zahájit úpravu konektoru":::

2. Jednotlivá připojení upravte jednotlivě výběrem ikony tři tečky. Přidejte příslušná připojení.

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Upravit konektory":::

3. Zapněte toky v následujícím pořadí:

- Registrace Webhooku partnerského centra (Insider Preview)
- Vytvoření společného prodejního odkazu – Salesforce do partnerského centra (Insider Preview)
- Aktualizace referenčních seznamů Microsoftu v partnerském centru pro spoluprodej na Salesforce (Insider Preview)
- Partnerské centrum do Salesforce (Insider Preview)
- Salesforce do partnerského centra (Insider Preview)
- Možnost Salesforce v partnerském centru (Insider Preview)
- Řešení Salesforce Microsoftu do partnerského centra (Insider Preview)

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Použití rozhraní Webhook API k registraci pro události změny prostředku

Rozhraní API Webhooku partnerského centra vám umožní registrovat se na události změny prostředků. Tyto události změny se odesílají na adresu URL jako příspěvky HTTP.

1. Pokud chcete zaregistrovat adresu URL, vyberte možnost **registrace Webhooku partnerského centra (Insider Preview)** Power automatizace.

2. Přidat připojení pro uživatele partnerského centra (a.) s událostmi partnerského centra s přihlašovacími údaji správce (b.), jak je zvýrazněno níže

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Trigger":::

3. Po provedení těchto aktualizací se zobrazí

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooky":::

4. Uložte změny a vyberte **zapnout**.

   Pokud chcete, aby Webhooky partnerského centra naslouchali změnám událostí, proveďte následující kroky:

5. Vyberte **Partnerské centrum pro SALESFORCE CRM (Insider Preview)**.

6. Vyberte ikonu **Upravit** a vyberte, **kdy se přijme požadavek HTTP**.

7. Kliknutím na ikonu **kopírování** zkopírujte zadanou adresu URL post protokolu HTTP.

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Zkopírování adresy URL":::

8. Nyní vyberte možnost "automatické registrace Webhooku partnerského centra (Insider Preview)" a vyberte **Spustit**.

9. Ujistěte se, že se v pravém podokně otevře okno spustit tok a vyberte **pokračovat**.

10. Zadejte následující podrobnosti:

    1. **Koncový bod triggeru http**: adresa URL zkopírována z předchozího kroku

    2. **Události k registraci**: odkaz-vytvořeno a odkaz-Aktualizováno

    3. **Přepsat existující koncové body triggeru, pokud je k dispozici**: Ano (přepsání všech stávajících koncových bodů)

11. Vyberte **Spustit** a potom vyberte **Hotovo.**

Webhook teď může naslouchat událostem vytvoření a aktualizace.

## <a name="customize-synchronization-steps"></a>Přizpůsobení kroků synchronizace

Pokud jsou odkazy na spoluprodejní synchronizace mezi partnerským centrem a vaším systémem CRM, tady jsou uvedená pole synchronizovaná v počítači partnerského centra.

Systémy CRM jsou často vysoce přizpůsobené. Můžete přizpůsobit automatické toky Power Automate. Postupujte podle pokynů pro mapování polí a v případě potřeby proveďte příslušné změny v postupech automatizace toků.  K dispozici jsou mapování partnerských Center Microsoftu na CRM, ale v závislosti na vašem prostředí CRM, můžete zvolit další přizpůsobení polí.

Několik kroků každého z těchto toků Power Automate přizpůsobit podle vašich potřeb. Tady jsou příklady dostupných přizpůsobení:

1. Pokud chcete přizpůsobit pole pro události vytvoření nebo aktualizace v Partnerské centrum se synchronizací referenčních seznamů CRM:

   1. Vyberte Partnerské centrum Salesforce CRM (Insider Preview).

   2. Pokud **chcete upravit** nebo přizpůsobit tok Power Automate upravit.

   3. Vyberte **(Rozsah) Synchronizovat zájemce nebo příležitost.**

2. Pokud chcete přizpůsobit mapování polí CRM pro události vytváření, vyberte Pokud se jedná **o novou sdílenou příležitost, pak**. Pokud ano, vyberte dílčí **krok** a potom rozbalte položku Creating a new opportunity in the CRM (Vytvoření **nové příležitosti v CRM).** Mapování v této části můžete upravit pomocí Průvodce mapováním polí.

   1. Pokud chcete přizpůsobit mapování polí CRM pro události aktualizací, vyberte krok "(Rozsah) Synchronizovat zájemce nebo příležitost".

   2. Vyberte **Pokud se jedná o aktualizaci příležitosti, pak**. Pokud ano, vyberte dílčí **krok** a potom rozbalte If difference between the opportunity objects in Partnerské centrum and CRM (Pokud je rozdíl mezi objekty příležitostí v Partnerské centrum **a CRM).**  

   3. Vyberte **Pokud ano a** pak Aktualizovat existující **příležitost.**

3. Přizpůsobení polí synchronizace referenčních seznamů CRM do pc pro události aktualizace:

   1. Pokud **chcete upravit**  nebo přizpůsobit tok Power Automate upravit.

   2. Vyberte **(Rozsah) Synchronizovat příležitost.**

   3. Pokud chcete přizpůsobit mapování polí CRM (na základě průvodce mapováním polí) pro aktualizační události, vyberte Pokud je mezi objekty zájemců v **aplikaci Partnerské centrum a CRM rozdíl, pak .**

   4. Pokud ano, vyberte dílčí **krok** a potom rozbalte krok Aktualizovat referenční **seznam daty příležitostí**.

   Mapování v této části můžete upravit na základě Průvodce mapováním polí.

4. Chcete přizpůsobit pole synchronizace referenčních seznamů CRM do pc pro vytváření událostí?

   1. Vyberte **Upravit**  a upravte nebo Přizpůsobte tok automatizovaného výkonu.

   2. Výběr **(rozsah) synchronizace odkazů.**

   3. Pokud chcete přizpůsobit mapování polí CRM (na základě Průvodce mapováním polí) pro události vytvořit, vyberte **vytvořit odkaz Microsoftu**.

Mapování v této části můžete upravit v závislosti na průvodci mapováním polí.


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>Komplexní Obousměrná synchronizace odkazů v rámci společného prodeje

Jakmile nainstalujete, nakonfigurujete a přizpůsobili řešení Power Automate, můžete otestovat synchronizaci odkazů pro spoluprodej mezi Salesforce CRM a Partnerským centrem.

### <a name="pre-requisites"></a>Požadavky

K synchronizaci odkazů v rámci partnerského centra a Salesforce CRM musí řešení Power automat jasně vymezit pole odkazů specifická pro společnost Microsoft. Tato identifikace poskytuje prodejcům v prodejci možnost rozhodnout se, které odkazy chtějí sdílet se společností Microsoft pro souběžný prodej.

Sada vlastních polí je k dispozici jako součást synchronizace odkazů partnerského centra pro entitu **příležitosti** řešení Salesforce CRM. Uživatel s oprávněními správce CRM bude muset vytvořit samostatný oddíl CRM s vlastními poli **příležitosti** .

Následující vlastní pole by měla být součástí části CRM:

- **Synchronizovat s partnerským centrem**: jestli se má synchronizovat příležitost s partnerským centrem Microsoftu

- **Identifikátor odkazu**: pole identifikátoru jen pro čtení pro odkaz na partnerského centra Microsoftu

- **Odkaz** odkazu: odkaz na odkaz určený jen pro čtení v partnerském centru Microsoftu

- **Jak může Microsoft pomáhat**: Podrobnější informace od Microsoftu

- **Produkty**: seznam produktů přidružených k této příležitosti

- **Audit**: záznam auditu jen pro čtení pro synchronizaci s odkazy partnerského centra

### <a name="scenarios"></a>ŘEŠENÍ

1. Referenční synchronizace při vytvoření nebo aktualizaci odkazu v CRM a synchronizovaných v partnerském centru:

   1. Přihlaste se k prostředí Salesforce CRM s uživatelem, který má v části **příležitost** v CRM přehled.

   2. Při vytváření nové příležitosti v prostředí Salesforce CRM se ujistěte, že se nachází následující část.

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Prostředí Salesforce":::

   3. Pokud chcete tuto příležitost synchronizovat s microsoft Partnerské centrum, ujistěte se, že jste v zobrazení karty nastavili následující pole:

       - "Synchronizace s Partnerské centrum": Ano
       - "Jak může Microsoft pomoct?": Vyberte jednu z následujících možností:
       - Produkty: ID řešení produktu

   4. Jakmile nastavíte možnost Synchronizovat s  **Partnerské centrum** na **Ano,** počkejte 10 minut, přihlaste se ke svému Partnerské centrum účtu. Vaše referenční seznamy se synchronizují s aplikací Salesforce CRM.

   5. Pokud je možnost Synchronizovat s Partnerské centrum nastavená na Ano, při aktualizaci příležitosti v Salesforce CRM se změny synchronizují s vaším Partnerské centrum účtem.

   6. Příležitosti, které se úspěšně synchronizují s Partnerské centrum, se identifikují pomocí ✔icon v Salesforce CRM.

2. Synchronizace referenčních seznamů při vytvoření nebo aktualizaci referenčního Partnerské centrum v prostředí Salesforce CRM:

    1. Přihlaste se k řídicímu [Partnerské centrum.](https://partner.microsoft.com/dashboard/home)

    2. V **nabídce vlevo** vyberte Referenční odkazy.

    3. Kliknutím na možnost New deal (Nová dohoda) Partnerské centrum nový referenční seznam pro spoludácí se ze seznamu.

    4. Přihlaste se k prostředí Salesforce CRM.

    5. Přejděte na **Otevřít příležitosti.** Referenční seznam vytvořený v Microsoft Partnerské centrum se teď synchronizuje v Salesforce CRM.

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Obrazovka prodejních příležitostí Salesforce":::

    6. Když vyberete synchronizovaný referenční seznam, vyplní se podrobnosti o zobrazení karty.

## <a name="next-steps"></a>Další kroky

- [Správa potenciálních zákazníků](manage-leads.md)

- [Správa příležitostí ke spoluprodeji](manage-co-sell-opportunities.md)

- [Webhooky Partnerského centra](/partner-center/develop/partner-center-webhooks)
