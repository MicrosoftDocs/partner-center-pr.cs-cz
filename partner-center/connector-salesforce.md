---
title: Konektor pro spoluprodejní účast v partnerském centru pro Salesforce CRM
ms.topic: how-to
ms.date: 09/29/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Synchronizujte své odkazy v partnerském centru se službou Salesforce CRM. Prodejci pak můžou v rámci svých systémů CRM prodávat společně s Microsoftem.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: b73f0b24538daa18b93fa206fce5eda1ab9bc9b9
ms.sourcegitcommit: 7e32544cf91f932cbeb053c9de506ba9ee773fe2
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/20/2020
ms.locfileid: "94947847"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Konektor pro společný prodej pro Salesforce CRM – přehled

### <a name="appropriate-roles"></a>Příslušné role

- Správce odkazů
- Správce systému nebo úpravce systému v CRM

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

Aby bylo možné synchronizovat odkazy v rámci partnerského centra a Salesforce CRM, musí řešení Power automat jasně identifikovat konkrétní pole odkazů specifická pro společnost Microsoft. Tato vymezená část poskytuje partnerům partnerských prodejců možnost rozhodnout se, které referenční seznamy chtějí sdílet se společností Microsoft pro souběžný prodej.

1. V Salesforce aktivujte **poznámky** a přidejte je do seznamu souvisejících příležitostí. 
[Odkaz](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. **Týmy příležitostí** aktivujte pomocí následujících kroků: 
    - V instalačním programu použijte pole **Rychlé hledání** k vyhledání nastavení týmu příležitostí.
    - Podle potřeby definujte nastavení.
[Odkaz](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. V Salesforce nainstalujte vlastní pole a objekty pomocí instalačního programu balíčků níže.
  
Pokud chcete balíček nainstalovat do libovolné společnosti, navštivte [Toto](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006Vs9a) :


Poznámka: Pokud instalujete do izolovaného prostoru (sandbox), musíte nahradit počáteční část adresy URL. http://test.salesforce.com

4. V Salesforce přidejte řešení Microsoftu do seznamu souvisejících **příležitostí** . Po přidání klikněte na ikonu **klíče** a aktualizujte vlastnosti.

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

4. V horní nabídce klikněte na odkaz **otevřít AppSource** .

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Otevřít AppSource":::

5. V místní obrazovce vyhledejte **konektory odkazů partnerského centra pro Salesforce** .  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. Klikněte na tlačítko **získat nyní** a potom **pokračujte**.

7. Otevře se stránka, kde můžete vybrat prostředí Salesforce CRM k instalaci aplikace.  Vyjádřit souhlas s podmínkami a ujednáními.

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="Dostupné CRMS":::

8. Pak budete přesměrováni na stránku **spravovat vaše řešení** .  Přejděte na "odkazy na partnerské Centrum" pomocí tlačítek se šipkami ve spodní části stránky. **Naplánovaná instalace** by se měla objevit u řešení s odkazy partnerského centra. Instalace bude trvat 10-15 minut.

9. Po dokončení instalace přejděte zpátky na [Power](https://flow.microsoft.com) automat a vyberte **řešení** z navigační oblasti vlevo. Všimněte si, že v seznamu řešení je k dispozici **synchronizace odkazů partnerského centra pro Salesforce** .

10. Vyberte **synchronizaci odkazů z partnerského centra pro Salesforce**. K dispozici jsou tyto toky a entity automatizace pro napájení:

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Toky Salesforce":::



## <a name="configure-the-solution"></a>Konfigurace řešení

1. Po instalaci řešení do instance CRM přejděte zpátky na [Power](https://flow.microsoft.com/)automat.

2. V rozevíracím seznamu **prostředí** v pravém horním rohu vyberte instanci CRM, do které jste nainstalovali řešení Power automatizuje.
3. Budete muset vytvořit připojení, která přiřadí tři uživatelské účty:
    - Uživatel partnerského centra s přihlašovacími údaji správce odkazů
    - Události Partnerského centra
    - Správce CRM s Power Automate automatizuje v řešení.
4. V levém navigačním panelu vyberte **připojení** a v seznamu vyberte řešení partnerského centra pro partnery.

5. Vytvořte připojení kliknutím na **vytvořit připojení**.

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Vytvoření připojení":::

- Na panelu hledání v pravém horním rohu vyhledejte odkazy na partnerské Centrum (Preview).

- Vytvořte připojení pro uživatele partnerského centra s rolí přihlašovacích údajů správce odkazů.

-  Potom vytvořte připojení událostí partnerského centra pro uživatele partnerského centra s přihlašovacími údaji správce odkazů.

- Vytvořte připojení pro Salesforce pro uživatele správce CRM.

-  Po přidání všech připojení byste měli ve svém prostředí zobrazit následující připojení:

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Sledovat připojení":::

### <a name="edit-the-connections"></a>Upravit připojení

1. Vraťte se na stránku řešení a vyberte **výchozí řešení**.  Kliknutím na tlačítko **vše** vyberte **odkaz připojení (Preview)** .
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Zahájit úpravu konektoru":::

2. Každé připojení jednu po jedné upravte výběrem ikony tři tečky. Přidejte příslušná připojení.

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

9. Ujistěte se, že se v pravém podokně otevře okno spustit tok a klikněte na **pokračovat**.

10. Zadejte následující podrobnosti:

    1. **Koncový bod triggeru http**: adresa URL zkopírována z předchozího kroku

    2. **Události k registraci**: odkaz-vytvořeno a odkaz-Aktualizováno

    3. **Přepsat existující koncové body triggeru, pokud je k dispozici**: Ano (přepsání všech stávajících koncových bodů)

11. Vyberte **Spustit** a potom vyberte **Hotovo.**

Webhook teď může naslouchat událostem vytvoření a aktualizace.

## <a name="customize-synchronization-steps"></a>Přizpůsobení kroků synchronizace

Pokud jsou odkazy na spoluprodejní synchronizace mezi partnerským centrem a vaším systémem CRM, tady jsou uvedená pole synchronizovaná v počítači partnerského centra.

Systémy CRM jsou často vysoce přizpůsobené. Můžete přizpůsobit automatické toky Power Automate. Postupujte podle pokynů pro mapování polí a v případě potřeby proveďte příslušné změny v postupech automatizace toků.  K dispozici jsou mapování partnerských Center Microsoftu na CRM, ale v závislosti na vašem prostředí CRM, můžete zvolit další přizpůsobení polí.

V závislosti na vašich potřebách je možné přizpůsobit více kroků každého z těchto toků automatizace napájení. Následují příklady dostupných přizpůsobení:

1. Přizpůsobení polí pro události vytvoření nebo aktualizace v partnerském centru pro synchronizaci odkazů CRM:

   1. Vyberte partnerské Centrum pro Salesforce CRM (Insider Preview).

   2. Vyberte **Upravit** a upravte nebo Přizpůsobte tok automatizovaného výkonu.

   3. Vyberte **(rozsah) synchronizujte zájemce nebo příležitost**.

2. Pokud chcete přizpůsobit mapování polí CRM pro události vytvoření, vyberte, **jestli je nová sdílená příležitost, a pak**. Vyberte dílčí krok, **Pokud ano** , a pak rozbalte **vytvořit novou příležitost v CRM**. Mapování v této části můžete upravit pomocí Průvodce mapováním polí.

   1. Pokud chcete přizpůsobit mapování polí CRM pro události aktualizace, klikněte na krok (obor) synchronizovat zájemce nebo příležitost.

   2. Vyberte **, jestli se jedná o aktualizaci příležitosti, a pak**. Vyberte dílčí krok, **Pokud ano** , a pak rozbalte **rozdíl mezi objekty příležitostí v partnerském centru a CRM a pak**.  

   3. Vyberte, **jestli ano** , a pak **aktualizovat existující příležitost** .

3. Přizpůsobení polí pro synchronizaci odkazů CRM na počítač pro události aktualizace:

   1. Vyberte **Upravit**  a upravte nebo Přizpůsobte tok automatizovaného výkonu.

   2. Vyberte **(rozsah) synchronizace příležitosti**.

   3. Chcete-li upravit mapování polí CRM (na základě Průvodce mapováním polí) pro události aktualizace, vyberte, **zda existuje rozdíl mezi objekty potenciálních zákazníků v partnerském centru a CRM, a pak**.

   4. Vyberte dílčí krok, **Pokud ano** , a pak rozbalte krok **aktualizace odkazu s daty příležitostí**.

   Mapování v této části můžete upravit v závislosti na průvodci mapováním polí.

4. Chcete-li přizpůsobit pole pro synchronizaci odkazů CRM na počítač pro vytvoření událostí?

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

   2. Při vytváření nové příležitosti v prostředí Salesforce CRM se ujistěte, že je k dispozici následující oddíl.

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Prostředí Salesforce":::

   3. Pokud chcete tuto příležitost synchronizovat s partnerským centrem Microsoftu, ujistěte se, že jste v zobrazení karta nastavili následující pole:

       - Synchronizovat s partnerským centrem: Ano
       - "Jak může Microsoft pomáhat?": Vyberte si z následujících možností:
       - Produkty: ID řešení produktu

   4. Jakmile nastavíte možnost Synchronizovat příležitost  **s partnerským centrem** na **Ano**, počkejte 10 minut, přihlaste se k účtu partnerského centra. Vaše odkazy budou synchronizovány s CRM Salesforce.

   5. Pokud je možnost synchronizovat s partnerským centrem nastavená na hodnotu Ano, změny se synchronizují s vaším účtem partnerského centra.

   6. Příležitosti, které byly úspěšně synchronizovány s partnerským centrem, budou označeny ikonou ✔ v Salesforce CRM.

2. Referenční synchronizace při vytvoření nebo aktualizaci odkazu v partnerském centru Microsoftu a synchronizovaných v prostředí Salesforce CRM:

    1. Přihlaste se k [řídicímu panelu](https://partner.microsoft.com/dashboard/home)partnerského centra.

    2. V nabídce na levé straně vyberte **odkazy** .

    3. Klikněte na možnost Nová práce a vytvořte si nový odkaz na společný prodej z partnerského centra.

    4. Přihlaste se do prostředí Salesforce CRM.

    5. Přejděte na **otevřené příležitosti**. Odkaz vytvořený v partnerském centru Microsoftu je teď synchronizovaný v Salesforce CRM.

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Obrazovka příležitostí pro Salesforce":::

    6. Když vyberete synchronizovaný odkaz, vyplní se podrobnosti zobrazení karty.

## <a name="next-steps"></a>Další kroky

- [Správa potenciálních zákazníků](manage-leads.md)

- [Správa příležitostí ke spoluprodeji](manage-co-sell-opportunities.md)

- [Webhooky partnerského centra](/partner-center/develop/partner-center-webhooks)
