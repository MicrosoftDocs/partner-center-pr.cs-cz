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
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a>Konektor pro společný prodej pro Dynamics 365 CRM – přehled

### <a name="appropriate-roles"></a>Příslušné role

- Správce odkazů
- Správce systému nebo úpravce systému v CRM

Konektor pro spoluprodej v partnerském centru umožňuje prodejcům v rámci svých systémů CRM spolupracovat s Microsoftem. Nebudou se muset vyškolet k používání partnerského centra ke správě obchodů v rámci společného prodeje. Pomocí konektorů pro spoluprodeji můžete vytvořit nový společný odkaz pro prodej prodávajícího, získat referenční údaje od prodejce Microsoftu, přijmout nebo odmítnout odkazy, upravit data o koupi, jako je například hodnota kouposti a datum ukončení. K těmto obchodům v rámci těchto spoluprodejů můžete také dostávat jakékoli aktualizace od prodejců Microsoftu. Všechny vaše odkazy můžete v aplikaci CRM použít místo v partnerském centru. 

Řešení je založené na řešení Microsoft Power automatizuje a používá rozhraní API partnerského centra.

## <a name="before-you-install---pre-requisites"></a>Před instalací – požadavky

|**Témata**   |**Podrobnosti**   |**Odkazy**   |
|--------------|--------------------|------|
|ID Microsoft Partner Network |Potřebujete platné ID MPN.|Připojení k programu [MPN](https://partner.microsoft.com/)|
|Předprodejní připraveno|Vaše řešení IP/Services musí být připravené k prodeji.|[Prodej pomocí Microsoftu](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Účet partnerského centra|ID MPN přidružené k tenantovi partnerského centra musí být stejné jako ID MPN přidružené k vašemu řešení společného prodeje. Před nasazením konektorů se můžete podívat na to, jestli máte na portálu partnerského centra zobrazený odkaz na svůj společný prodej.|[Správa vašeho účtu](create-user-accounts-and-set-permissions.md)|
|Role uživatelů partnerského centra|Zaměstnanec, který bude instalovat a používat konektory, musí být správcem odkazů.|[Přiřazování uživatelských rolí a oprávnění](create-user-accounts-and-set-permissions.md)| |Dynamics 365 CRM|Role uživatele CRM je správce systému nebo úpravce systému.|[Přiřazení rolí v Dynamics 365](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Zapnout účet toku automatizace|Aktivní účet [Power automatizuje](https://flow.microsoft.com) pro správce systému nebo úpravce systému CRM. Tento uživatel se musí před instalací přihlásit k [automatizaci](https://flow.microsoft.com) aspoň jednou.|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Nainstalovat synchronizaci odkazů partnerského centra pro Dynamics 365 (řešení Power automat)

1. V pravém horním rohu vyberte **prostředí** k [automatizaci](https://flow.microsoft.com) a vyberte prostředí. Tento krok vám ukáže dostupné instance CRM.

2. V rozevíracím seznamu v pravém horním rohu vyberte příslušnou instanci CRM.

3. Na levém navigačním panelu vyberte **řešení** .

4. V horní nabídce klikněte na odkaz **otevřít AppSource** .

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Otevřít AppSource&quot;:::

5. V místní obrazovce vyhledejte **konektory odkazů partnerského centra pro Dynamics365** .  

6. Klikněte na tlačítko **získat nyní** a potom **pokračujte** .

7. Otevře se stránka, kde můžete vybrat prostředí CRM (Dynamics 365) k instalaci aplikace.  Vyjádřit souhlas s podmínkami a ujednáními.

8. Pak budete přesměrováni na stránku **spravovat vaše řešení** .  Přejděte na &quot;odkazy na partnerské Centrum" pomocí tlačítek se šipkami ve spodní části stránky. **Naplánovaná instalace** by se měla objevit u řešení s odkazy partnerského centra. Instalace bude trvat 10-15 minut. 

9. Po dokončení instalace přejděte zpátky na [Power](https://flow.microsoft.com) automat a vyberte **řešení** z navigační oblasti vlevo. Všimněte si, že v seznamu řešení je k dispozici **synchronizace odkazů partnerského centra pro Dynamics 365** .

10. Vyberte **synchronizaci odkazů partnerského centra pro Dynamics 365** . K dispozici jsou tyto toky a entity automatizace pro napájení:

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Otevřít AppSource&quot;:::

5. V místní obrazovce vyhledejte **konektory odkazů partnerského centra pro Dynamics365** .  

6. Klikněte na tlačítko **získat nyní** a potom **pokračujte** .

7. Otevře se stránka, kde můžete vybrat prostředí CRM (Dynamics 365) k instalaci aplikace.  Vyjádřit souhlas s podmínkami a ujednáními.

8. Pak budete přesměrováni na stránku **spravovat vaše řešení** .  Přejděte na &quot;odkazy na partnerské Centrum":::

## <a name="best-practice-test-before-you-go-live"></a>Osvědčené postupy: test před zahájením provozu

Než nainstalujete, nakonfigurujete a přizpůsobíte řešení Power Automate v produkčním prostředí, ujistěte se, že řešení otestujete v pracovní instanci CRM.

- Nainstalujte řešení Microsoft Power automatizuje do přípravného prostředí/instance CRM.
- Vytvořte kopii řešení a spusťte konfiguraci a automatizujte vlastní nastavení toků v přípravném prostředí.
- Otestujte řešení na pracovní instanci/CRM. 
- Po úspěšném dokončení naimportujte jako spravované řešení do provozní instance. 

## <a name="configure-the-solution"></a>Konfigurace řešení

1. Po instalaci řešení do instance CRM přejděte zpátky na [Power](https://flow.microsoft.com/)automat.

2. V rozevíracím seznamu **prostředí** v pravém horním rohu vyberte instanci CRM, do které jste nainstalovali řešení Power automatizuje.

3. Budete muset vytvořit připojení, která přiřadí tři uživatelské účty:

   - Uživatel partnerského centra s přihlašovacími údaji správce odkazů

   - Události Partnerského centra

   - Správce CRM s Power Automate automatizuje v řešení.

      1. V levém navigačním panelu vyberte **připojení** a v seznamu vyberte řešení partnerského centra pro partnery.

      2. Vytvořte připojení kliknutím na **vytvořit připojení** .

         :::image type="content" source="images/cosellconnectors/createconnection.png" alt-text="Otevřít AppSource&quot;:::

5. V místní obrazovce vyhledejte **konektory odkazů partnerského centra pro Dynamics365** .  

6. Klikněte na tlačítko **získat nyní** a potom **pokračujte** .

7. Otevře se stránka, kde můžete vybrat prostředí CRM (Dynamics 365) k instalaci aplikace.  Vyjádřit souhlas s podmínkami a ujednáními.

8. Pak budete přesměrováni na stránku **spravovat vaše řešení** .  Přejděte na &quot;odkazy na partnerské Centrum":::

      3. Na panelu hledání v pravém horním rohu vyhledejte **odkazy na partnerské Centrum (Preview)** .

      4. Vytvořte připojení pro uživatele partnerského centra s rolí přihlašovacích údajů správce odkazů.

      5. Potom vytvořte připojení událostí partnerského centra pro uživatele partnerského centra s přihlašovacími údaji správce odkazů.

      6. Vytvořte připojení pro Common Data Service (aktuální prostředí) pro uživatele správce CRM.

4. Pokud chcete přidružit Power Automate k připojením, upravte jednotlivé toky Power automatu pro připojení k Common Data Service a odkazům partnerského centra. Uložte změny.

5. **Zapněte** automatické toky napájení.

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Použití rozhraní Webhook API k registraci pro události změny prostředku

Rozhraní API Webhooku partnerského centra vám umožní registrovat se na události změny prostředků. Tyto události změny se odesílají na adresu URL jako příspěvky HTTP.

1. Pokud chcete zaregistrovat adresu URL, vyberte možnost **registrace Webhooku partnerského centra (Insider Preview)** Power automatizace.

2. Přidat připojení pro uživatele partnerského centra (a.) s událostmi partnerského centra s přihlašovacími údaji správce (b.), jak je zvýrazněno níže

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Otevřít AppSource&quot;:::

5. V místní obrazovce vyhledejte **konektory odkazů partnerského centra pro Dynamics365** .  

6. Klikněte na tlačítko **získat nyní** a potom **pokračujte** .

7. Otevře se stránka, kde můžete vybrat prostředí CRM (Dynamics 365) k instalaci aplikace.  Vyjádřit souhlas s podmínkami a ujednáními.

8. Pak budete přesměrováni na stránku **spravovat vaše řešení** .  Přejděte na &quot;odkazy na partnerské Centrum":::

3. Po provedení těchto aktualizací se zobrazí

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Otevřít AppSource&quot;:::

5. V místní obrazovce vyhledejte **konektory odkazů partnerského centra pro Dynamics365** .  

6. Klikněte na tlačítko **získat nyní** a potom **pokračujte** .

7. Otevře se stránka, kde můžete vybrat prostředí CRM (Dynamics 365) k instalaci aplikace.  Vyjádřit souhlas s podmínkami a ujednáními.

8. Pak budete přesměrováni na stránku **spravovat vaše řešení** .  Přejděte na &quot;odkazy na partnerské Centrum":::

4. Uložte změny a vyberte **zapnout** .

   Pokud chcete, aby Webhooky partnerského centra naslouchali změnám událostí, proveďte následující kroky:

5. Vyberte **Partnerské centrum pro Dynamics 365 (Insider Preview)** .

6. Vyberte ikonu **Upravit** a vyberte, **kdy se přijme požadavek HTTP** .

7. Kliknutím na ikonu **kopírování** zkopírujte zadanou adresu URL post protokolu HTTP.

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="Otevřít AppSource&quot;:::

5. V místní obrazovce vyhledejte **konektory odkazů partnerského centra pro Dynamics365** .  

6. Klikněte na tlačítko **získat nyní** a potom **pokračujte** .

7. Otevře se stránka, kde můžete vybrat prostředí CRM (Dynamics 365) k instalaci aplikace.  Vyjádřit souhlas s podmínkami a ujednáními.

8. Pak budete přesměrováni na stránku **spravovat vaše řešení** .  Přejděte na &quot;odkazy na partnerské Centrum" a vyberte **Spustit** .

9. Ujistěte se, že se v pravém podokně otevře okno spustit tok a klikněte na **pokračovat** .

10. Zadejte následující podrobnosti:

    1. **Koncový bod triggeru http** : adresa URL zkopírována z předchozího kroku

    2. **Události k registraci** : odkaz-vytvořeno a odkaz-Aktualizováno

    3. **Přepsat existující koncové body triggeru, pokud je k dispozici** : Ano (přepsání všech stávajících koncových bodů)

11. Vyberte **Spustit** a potom vyberte **Hotovo.**

Webhook teď může naslouchat událostem vytvoření a aktualizace.

## <a name="customize-synchronization-steps"></a>Přizpůsobení kroků synchronizace

Pokud jsou odkazy na spoluprodejní synchronizace mezi partnerským centrem a vaším systémem CRM, tady jsou uvedená pole synchronizovaná v počítači partnerského centra.

Systémy CRM jsou často vysoce přizpůsobené. Můžete přizpůsobit automatické toky Power Automate. Postupujte podle pokynů pro mapování polí a v případě potřeby proveďte příslušné změny v postupech automatizace toků.  K dispozici jsou mapování partnerských Center Microsoftu na CRM, ale v závislosti na vašem prostředí CRM, můžete zvolit další přizpůsobení polí.

V závislosti na vašich potřebách je možné přizpůsobit více kroků každého z těchto toků automatizace napájení. Následují příklady dostupných přizpůsobení:

1. Přizpůsobení polí pro události vytvoření nebo aktualizace v partnerském centru pro synchronizaci odkazů CRM: 

    a. Vyberte partnerské Centrum pro Dynamics 365 (Insider Preview) nebo partnerské Centrum do Salesforce (Insider Preview).

    b. Vyberte **Upravit** a upravte nebo Přizpůsobte tok automatizovaného výkonu.

    c. Vyberte **(rozsah) synchronizujte zájemce nebo příležitost** .

2. Pokud chcete přizpůsobit mapování polí CRM (na základě Průvodce mapováním polí) pro události vytvořit, vyberte, **jestli je nová sdílená příležitost, a pak** . Vyberte dílčí krok, **Pokud ano** , a pak rozbalte **vytvořit novou příležitost v CRM** . Mapování v této části můžete upravit pomocí Průvodce mapováním polí.

    d. Pro přizpůsobení mapování polí CRM (na základě Průvodce mapováním polí) pro události aktualizace klikněte na krok (obor) synchronizovat zájemce nebo příležitost.

    e. Vyberte **, jestli se jedná o aktualizaci příležitosti, a pak** . Vyberte dílčí krok, **Pokud ano** , a pak rozbalte **rozdíl mezi objekty příležitostí v partnerském centru a CRM a pak** .  

    f. Vyberte, **jestli ano** , a pak **aktualizovat existující příležitost** .

3. Přizpůsobení polí pro synchronizaci odkazů CRM na počítač pro události aktualizace:

    a. Vyberte **Upravit**  a upravte nebo Přizpůsobte tok automatizovaného výkonu.

    b. Vyberte **(rozsah) synchronizace příležitosti** .

    c. Pokud chcete přizpůsobit mapování polí CRM pro události aktualizace, vyberte, **jestli jsou mezi objekty zájemce v partnerském centru a CRM rozdílové rozdíly, a pak** . 

    d. Vyberte dílčí krok, **Pokud ano** , a pak rozbalte krok **aktualizace odkazu s daty příležitostí** .

   Mapování v této části můžete upravit v závislosti na průvodci mapováním polí.

4. Chcete-li přizpůsobit pole pro synchronizaci odkazů CRM na počítač pro vytvoření událostí?

   a. Vyberte **Upravit**  a upravte nebo Přizpůsobte tok automatizovaného výkonu.

   b. Výběr **(rozsah) synchronizace odkazů.**

   c. Pokud chcete přizpůsobit mapování polí CRM (na základě Průvodce mapováním polí) pro události vytvořit, vyberte **vytvořit odkaz Microsoftu** .

   Mapování v této části můžete upravit v závislosti na průvodci mapováním polí.

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>Komplexní Obousměrná synchronizace odkazů v rámci společného prodeje

Jakmile nainstalujete, nakonfigurujete a přizpůsobíte řešení Power Automate, můžete otestovat synchronizaci odkazů mezi produkty Dynamics 365 a Partnerským centrem společně prodávat.

### <a name="pre-requisites"></a>Požadavky

Aby bylo možné synchronizovat odkazy v rámci partnerského centra a Dynamics 365 CRM, řešení Power automat jasně vymezuje pole odkazů specifická pro společnost Microsoft. Tato identifikace dává prodejcům možnost rozhodnout se, které odkazy chce sdílet se společností Microsoft pro souběžný prodej.

Sada vlastních polí je k dispozici jako součást entity **příležitosti** . Uživatel s oprávněními správce CRM bude muset vytvořit samostatný oddíl CRM s vlastními poli **příležitosti** .

Následující vlastní pole by měla být součástí části CRM:

- **Synchronizovat s partnerským centrem** : jestli se má synchronizovat příležitost s partnerským centrem Microsoftu

- **Identifikátor odkazu** : pole identifikátoru jen pro čtení pro odkaz na partnerského centra Microsoftu

- **Odkaz** odkazu: odkaz na odkaz určený jen pro čtení v partnerském centru Microsoftu

- **Jak může společnost Microsoft** získat nápovědu? od Microsoftu se dozvíte, jak tento odkaz vyžaduje.

- **Produkty** : seznam produktů přidružených k této příležitosti

- **Audit** : záznam auditu jen pro čtení pro synchronizaci s odkazy partnerského centra

### <a name="scenarios"></a>ŘEŠENÍ

1. Referenční synchronizace při vytvoření nebo aktualizaci odkazu v CRM a synchronizovaných v partnerském centru:

   1. Přihlaste se k prostředí Dynamics 365 CRM s uživatelem, který má v části **příležitost** v aplikaci CRM přehled.

   2. Při vytváření nové příležitosti v prostředí Dynamics 365 se ujistěte, že je k dispozici následující oddíl.

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="Otevřít AppSource&quot;:::

5. V místní obrazovce vyhledejte **konektory odkazů partnerského centra pro Dynamics365** .  

6. Klikněte na tlačítko **získat nyní** a potom **pokračujte** .

7. Otevře se stránka, kde můžete vybrat prostředí CRM (Dynamics 365) k instalaci aplikace.  Vyjádřit souhlas s podmínkami a ujednáními.

8. Pak budete přesměrováni na stránku **spravovat vaše řešení** .  Přejděte na &quot;odkazy na partnerské Centrum":::

   3. Pokud chcete tuto příležitost synchronizovat s partnerským centrem Microsoftu, ujistěte se, že jste v zobrazení karta nastavili následující pole:

      - **Synchronizovat s partnerským centrem** : Ano

      - **Jak může Microsoft pomáhat?** : vyberte z těchto možností:

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="Otevřít AppSource&quot;:::

5. V místní obrazovce vyhledejte **konektory odkazů partnerského centra pro Dynamics365** .  

6. Klikněte na tlačítko **získat nyní** a potom **pokračujte** .

7. Otevře se stránka, kde můžete vybrat prostředí CRM (Dynamics 365) k instalaci aplikace.  Vyjádřit souhlas s podmínkami a ujednáními.

8. Pak budete přesměrováni na stránku **spravovat vaše řešení** .  Přejděte na &quot;odkazy na partnerské Centrum":::

      - **Produkty** : ID řešení produktu

   4. Až se příležitost vytvoří v Dynamics 365 s možností **synchronizovat s partnerským centrem** nastavenou na **Ano** , počkejte 10 minut a pak se přihlaste k účtu partnerského centra. Vaše odkazy budou synchronizovány s Dynamics 365.

   5. Podobně platí, že pokud chcete příležitost, která má možnost synchronizovat s partnerským centrem nastavenou na hodnotu Ano, aktualizovat příležitost v Dynamics 365 CRM, změny se synchronizují v účtu partnerského centra.

   6. Příležitosti, které byly úspěšně synchronizovány s partnerským centrem, budou označeny ikonou ✔ v Dynamics 365.

2. Referenční synchronizace při vytvoření nebo aktualizaci odkazu v partnerském centru Microsoftu a synchronizovaných v prostředí Dynamics 365:

   1. Přihlaste se k [řídicímu panelu](https://partner.microsoft.com/dashboard/home)partnerského centra.

   2. V nabídce na levé straně vyberte **odkazy** .

   3. Klikněte na možnost Nová práce a vytvořte si nový odkaz na společný prodej z partnerského centra.

   4. Přihlaste se k prostředí Dynamics 365 CRM.

   5. Přejděte na **otevřené příležitosti** . Odkaz vytvořený v partnerském centru Microsoftu je teď synchronizovaný v Dynamics 365 CRM.

   6. Když vyberete synchronizovaný odkaz, vyplní se podrobnosti zobrazení karty.

## <a name="next-steps"></a>Další kroky

- [Správa potenciálních zákazníků](manage-leads.md)

- [Správa příležitostí ke spoluprodeji](manage-co-sell-opportunities.md)

- [Další informace o platformě Microsoft Power automatizuje?](/power-automate/)

- [Webhooky partnerského centra](/partner-center/develop/partner-center-webhooks)