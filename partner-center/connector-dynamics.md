---
title: Konektor pro spoluprodeji pro partnerské Centrum Dynamics 365 CRM
ms.topic: how-to
ms.date: 03/01/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Synchronizujte odkazy v partnerském centru s konektorem pro spoluprodeji pro Dynamics 365 CRM. Prodejci pak můžou v rámci svých systémů CRM prodávat společně s Microsoftem.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 10062fd20e3553856d8b595efd3224ff456c2c49
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756791"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a>Konektor pro společný prodej pro Dynamics 365 CRM – přehled

### <a name="appropriate-roles"></a>Příslušné role

- Správce odkazů
- Správce systému nebo úpravce systému v CRM

Konektor pro spoluprodej v partnerském centru umožňuje prodejcům v rámci svých systémů CRM spolupracovat s Microsoftem. Nebudou se muset vyškolet k používání partnerského centra ke správě obchodů v rámci společného prodeje. Pomocí konektorů pro spoluprodeji můžete vytvořit nový společný odkaz pro prodej prodávajícího, získat referenční údaje od prodejce Microsoftu, přijmout nebo odmítnout odkazy, upravit data o koupi, jako je například hodnota kouposti a datum ukončení. K těmto obchodům v rámci těchto spoluprodejů můžete také dostávat jakékoli aktualizace od prodejců Microsoftu. Všechny vaše odkazy můžete spravovat v CRM dle vašeho výběru, nikoli v partnerském centru. 

Řešení je založené na řešení Microsoft Power automatizuje a používá rozhraní API partnerského centra.

## <a name="before-you-install---pre-requisites"></a>Před instalací – požadavky

|**Témata**   |**Podrobnosti**   |**Odkazy**   |
|--------------|--------------------|------|
|ID Microsoft Partner Network |Potřebujete platné ID MPN.|Připojení k programu [MPN](https://partner.microsoft.com/)|
|Připravený společný prodej|Vaše řešení IP/Services musí být připravené k prodeji.|[Prodej pomocí Microsoftu](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Účet partnerského centra|ID MPN přidružené k tenantovi partnerského centra musí být stejné jako ID MPN přidružené k vašemu řešení společného prodeje. Před nasazením konektorů se můžete podívat na to, jestli máte na portálu partnerského centra zobrazený odkaz na svůj společný prodej.|[Správa vašeho účtu](create-user-accounts-and-set-permissions.md)|
|Role uživatelů partnerského centra|Zaměstnanec, který bude instalovat a používat konektory, musí být správcem odkazů.|[Přiřazování uživatelských rolí a oprávnění](create-user-accounts-and-set-permissions.md)| 
|Dynamics 365 CRM|Role uživatele CRM je správce systému nebo úpravce systému.|[Přiřazení rolí v Dynamics 365](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Zapnout účet toku automatizace|Vytvořte nové provozní prostředí s databází pro testování/přípravu a produkci. Pokud máte existující produkční prostředí s databází, je možné ho znovu použít. Uživatel, který chce instalovat řešení konektoru, musí mít licenci pro automatizaci a přístup k tomuto prostředí. Kliknutím na Zobrazit historii v části řešení můžete monitorovat průběh a získat další podrobnosti, pokud se instalace nezdaří v [Power](https://flow.microsoft.com/) automatu.|[Vytvořit nebo spravovat prostředí](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Nainstalovat synchronizaci odkazů partnerského centra pro Dynamics 365 (řešení Power automat)

1. V pravém horním rohu vyberte **prostředí** k [automatizaci](https://flow.microsoft.com) a vyberte prostředí. Tento krok vám ukáže dostupné instance CRM.

2. V rozevíracím seznamu v pravém horním rohu vyberte příslušnou instanci CRM.

3. Na levém navigačním panelu vyberte **řešení** .

4. V horní nabídce klikněte na odkaz **otevřít AppSource** .

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Otevřít AppSource":::

5. V místní obrazovce vyhledejte **konektory odkazů partnerského centra pro Dynamics365** .  

6. Klikněte na tlačítko **získat nyní** a potom **pokračujte**.

7. Otevře se stránka, kde můžete vybrat prostředí CRM (Dynamics 365) k instalaci aplikace.  Vyjádřit souhlas s podmínkami a ujednáními.

8. Kliknutím na **Zobrazit historii** v části **řešení** můžete monitorovat průběh a získat další podrobnosti, pokud se instalace nezdaří v Power automatu.
 

9. Po dokončení instalace přejděte zpátky na [Power](https://flow.microsoft.com) automat a vyberte **řešení** z navigační oblasti vlevo. Všimněte si, že v seznamu řešení je k dispozici **synchronizace odkazů partnerského centra pro Dynamics 365** .

10. Vyberte **synchronizaci odkazů partnerského centra pro Dynamics 365**. K dispozici jsou tyto toky a entity automatizace pro napájení:

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Dostupné CRMS":::

## <a name="best-practice-test-before-you-go-live"></a>Osvědčené postupy: test před zahájením provozu

Než nainstalujete, nakonfigurujete a přizpůsobíte řešení Power Automate v produkčním prostředí, ujistěte se, že řešení otestujete v pracovní instanci CRM.

- Nainstalujte řešení Microsoft Power automatizuje do přípravného prostředí/instance CRM.
- Nakonfigurujte a přizpůsobte řešení Microsoft Power automatizuje v přípravném prostředí.
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

      2. Vytvořte připojení kliknutím na **vytvořit připojení**.

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Vytvoření připojení":::

      3. Na panelu hledání v pravém horním rohu vyhledejte **odkazy na partnerské Centrum (Preview)** .

      4. Vytvořte připojení pro uživatele partnerského centra s rolí přihlašovacích údajů správce odkazů.

      5. Potom vytvořte připojení událostí partnerského centra pro uživatele partnerského centra s přihlašovacími údaji správce odkazů.

      6. Vytvořte připojení pro Common Data Service (aktuální prostředí) pro uživatele správce CRM.
     
      7. Po přidání všech připojení byste měli ve svém prostředí zobrazit následující připojení:

:::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="Připojení":::
   
## <a name="edit-the-connections"></a>Upravit připojení

1. Vraťte se na stránku **řešení** a vyberte **výchozí řešení**. Kliknutím na tlačítko **vše** vyberte **odkaz připojení (Preview)** .

:::image type="content" source="images/connection-reference-video.gif" alt-text="Úprava připojení":::

2. Každé připojení jednu po jedné upravte výběrem ikony tři tečky. Přidejte příslušná připojení.

:::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="Uvedená připojení"::: 

3.  Vraťte se na stránku řešení, vyberte synchronizace odkazů partnerského centra pro Dynamics 365 a zapněte tok kliknutím na tři tečky vedle každého toku v následujícím pořadí. Pokud narazíte na problémy při zapínání toku, přečtěte si [Postup přizpůsobení](connector-dynamics.md#customize-synchronization-steps) a [Postup řešení potíží](connectors-troubleshoot.md). 

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

Rozhraní API Webhooku partnerského centra vám umožní registrovat se na události změny prostředků. Tyto události změny se odesílají na adresu URL jako příspěvky HTTP.

1. Vyberte **Partnerské centrum pro Dynamics 365 (Insider Preview)**.

2. Vyberte ikonu **Upravit** a vyberte, **kdy se přijme požadavek HTTP**.

3. Kliknutím na ikonu **kopírování** zkopírujte zadanou adresu URL post protokolu HTTP.

 :::image type="content" source="images/webhook-video.gif" alt-text="Použití webhooků k registraci změn prostředků":::

4. Vyberte možnost pro automatizaci automatizace a pak vyberte **Spustit**.

5. Ujistěte se, že se v pravém podokně otevře okno spustit tok a klikněte na **pokračovat**.

6. Zadejte následující podrobnosti:

   - **Koncový bod triggeru http**: adresa URL zkopírována z předchozího kroku

   - **Události k registraci**: výběr všech dostupných událostí ("vytváření odkazů – vytvořeno", "odkaz-aktualizováno", "související-referenční – vytvořeno", "související-referenční-aktualizováno")

   -**Přepsat existující koncové body triggeru, pokud je k dispozici**: Ano je důležité si uvědomit, že pro danou událost Webhooku může být zaregistrována pouze jedna adresa URL. Je důležité si uvědomit, že pro danou událost Webhooku může být zaregistrována pouze jedna adresa URL. 

7. Vyberte **Spustit** a potom vyberte **Hotovo.**

Webhook teď může naslouchat událostem vytvoření a aktualizace.

## <a name="customize-synchronization-steps"></a>Přizpůsobení kroků synchronizace

Systémy CRM jsou vysoce přizpůsobené a můžete upravit řešení Power automat na základě nastavení aplikace CRM.  Pokud se pro spoluprodejní odkazy mezi partnerským centrem a vaším systémem CRM synchronizují, budou pole synchronizovaná v počítači s partnerským centrem uvedená v [Průvodci mapováním vlastních polí](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S).

Postupujte podle pokynů pro mapování polí a v případě potřeby proveďte příslušné změny v **[přizpůsobení] vytvoření nebo získání podrobností z toku**  nebo proměnných prostředí Dynamics 365. V řešení Power Automate doporučujeme neaktualizovat žádné další toky, protože to může mít vliv na budoucí upgrady řešení. 

K dispozici jsou následující možnosti přizpůsobení:

- Zaškrtávací značka zaškrtnutí v názvu příležitosti: ve výchozím nastavení se vedle názvu příležitosti zobrazí značka zaškrtnutí, která indikuje, že synchronizace mezi partnerským centrem a Dynamics 365 CRM proběhne úspěšně. Podobně se zobrazí křížové značky, pokud se synchronizace nezdaří. Chcete-li zabránit přidání zaškrtnutí nebo křížového označení v názvu příležitosti, nastavte aktuální hodnotu zaškrtnutí zaškrtnutí u možnosti prostředí název příležitosti na hodnotu ne.

- Hodnota koupě: ve výchozím nastavení se hodnota koupě z partnerského centra synchronizuje do a z **estimatedvalue** v CRM. Pokud je v aplikaci CRM k dispozici jiné pole pro synchronizaci hodnoty z:

    a.    Aktualizujte název pole hodnoty obchodu v proměnné prostředí Dynamics 365 s názvem pole CRM. Všimněte si, že byste měli zadat název pole, nikoli jeho zobrazované jméno.

    b.    Upravit **[přizpůsobení] vytvořit nebo získat podrobnosti z toku Dynamics 365**  a přejít k možnosti **vytvořit nebo aktualizovat** příležitost v CRM a aktualizovat **vytvořit novou příležitost** a **aktualizovat existující akce příležitostí** , aby bylo možné přiřadit hodnotu **DealValue** k správnému poli v CRM. Odeberte také **přiřazení DealValue** z pole **Odhadované výnosy** .

- Směrové číslo země zákazníka: při vytváření nového odkazu je nutné zadat kód země (ISO 3166) se dvěma písmeny (ISO). Ve výchozím nastavení se kód země synchronizuje do pole address1_country účtu v CRM. Pokud máte jiné pole v CRM pro kód země, ze kterého se má synchronizovat:

   a.    Pro pole kód země nevyhledávání v účtu, který obsahuje kód se dvěma písmeny:

   - Aktualizujte název pole kód země zákazníka v proměnné prostředí Dynamics 365 s názvem pole CRM. Všimněte si, že byste měli zadat název pole, nikoli jeho zobrazované jméno.

   - Upravit **[vlastní] vytvořit nebo získat podrobnosti z toku Dynamics 365**  a přejít k možnosti vytvořit nebo získat účet zákazníka v aplikaci CRM k přiřazení hodnoty země do správného pole v CRM. Odeberte také přiřazení hodnoty země z pole Adresa 1: země/oblast.

   b.    Pro pole kód země na základě vyhledávání v účtu:

   - Přidejte do účtu nové vlastní pole a automaticky ho vyplníte kódem země (ISO 3166) na základě hodnoty vybrané v poli vyhledávání a naopak.

   - Pokud chcete synchronizovat nové vlastní pole z CRM do a z partnerského centra, postupujte podle kroků uvedených výše v poli kód země bez vyhledávání.

- Pole příležitostí: Pokud jsou v příležitosti povinná pole, která je potřeba naplnit úpravou **[přizpůsobení] vytvořit nebo získat podrobnosti z toku Dynamics 365**  , přejděte k části **Vytvoření nebo aktualizace příležitosti** v CRM a v nabídce vytvořit **novou akci** pro přiřazení hodnot k povinným polím na základě vašich obchodních požadavků.

- Pole zájemců: Pokud existují povinná pole v rámci zájemce, která musí být naplněna úpravou **[přizpůsobení] vytvořit nebo získat podrobnosti z toku Dynamics 365**  , přejděte k možnosti **vytvořit nebo aktualizovat vedoucí** v CRM a aktualizovat **vytvořit novou akci zájemce** pro přiřazení hodnot do povinných polí na základě vašich obchodních požadavků.

- Účet zákazníka: když se nový odkaz synchronizuje z partnerského centra s CRM, řešení Power automat se pokusí vyhledat existující účet v CRM pomocí názvu a PSČ společnosti zákazníka. Pokud se nenalezne, vytvoří se v CRM nový účet zákazníka. Pokud chcete aktualizovat kritéria hledání a podrobnosti vytváření nového účtu, upravte **[vlastní] vytvořit nebo získat podrobnosti z toku Dynamics 365** a přejděte k části **Vytvoření nebo získání účtu zákazníka** v CRM a **akci vytvořit účet zákazníka**.

## <a name="update-environment-variable"></a>Aktualizovat proměnnou prostředí

Aktualizace hodnoty proměnné prostředí:

1. Přejít na stránku **řešení** a vybrat **výchozí řešení**. Kliknutím na vše vyberte **proměnnou prostředí** .

2. Vyberte proměnnou prostředí pro hodnotu, kterou je třeba aktualizovat, a klikněte na **Upravit** pomocí ikony tři tečky.

3. Aktualizujte **aktuální hodnotu** (neaktualizujte výchozí hodnotu) pomocí možnosti **Nová hodnota** a zadejte hodnotu. Hodnota se musí shodovat s datovým typem proměnné, např. ano/ne. datový typ bude akceptovat buď Ano, nebo bez hodnoty.

:::image type="content" source="images/environment-variables-video.gif" alt-text="Aktualizovat proměnné prostředí":::

- Komplexní Obousměrná synchronizace odkazů v rámci společného prodeje

Jakmile nainstalujete, nakonfigurujete a přizpůsobíte řešení Power Automate, můžete otestovat synchronizaci odkazů mezi produkty Dynamics 365 a Partnerským centrem společně prodávat.

### <a name="pre-requisites"></a>Požadavky

Aby bylo možné synchronizovat odkazy v rámci partnerského centra a Dynamics 365 CRM, řešení Power automat jasně vymezuje pole odkazů specifická pro společnost Microsoft. Tato identifikace dává prodejcům možnost rozhodnout se, které odkazy chce sdílet se společností Microsoft pro souběžný prodej.

Sada vlastních polí a objektů bude přidána jako součást instalace řešení. Uživatel s oprávněními správce CRM bude muset vytvořit samostatný oddíl CRM s vlastními poli **příležitosti** .

Následující vlastní pole by měla být součástí části CRM:

- **Synchronizovat s partnerským centrem**: jestli se má synchronizovat příležitost s partnerským centrem Microsoftu. Ve výchozím nastavení je hodnota tohoto pole ne a musí být explicitně nastavená na Ano, aby mohl váš prodejce sdílet příležitost s Microsoftem. Nové odkazy sdílené z partnerského centra do CRM budou mít tuto hodnotu pole nastavenou na Ano.

- **Identifikátor odkazu**: pole identifikátoru jen pro čtení pro odkaz na partnerského centra Microsoftu

- **Odkaz** odkazu: odkaz na odkaz určený jen pro čtení v partnerském centru Microsoftu
- **Jak může společnost Microsoft** získat nápovědu? od Microsoftu se dozvíte, jak odkaz požaduje. Pokud chcete vytvořit odkaz pro spoluprodejní, vyberte vhodnou povinnou podporu od Microsoftu. Aby bylo možné vytvořit odkaz pro společný prodej, musí být přidružen k příležitosti kontakt zákazníka. Pokud chcete vytvořit odkaz bez společného prodeje, nechte toto pole nezaškrtnuté. Odkaz na nesouvisející prodej se dá kdykoli převést na odkaz na spoluprodej, a to výběrem vhodné požadované možnosti help.

- **Viditelnost odkazů z partnerského centra Microsoftu**: vyberte viditelnost pro odkaz na partnerské Centrum Microsoftu. Díky tomu, že se dá zviditelnit prodejcům Microsoftu, se odkaz na nesouvisející prodej může převést na společný prodej. Když se vyžaduje pomocník Microsoftu, je odkaz ve výchozím nastavení viditelný pro prodejce Microsoftu. Po označení jako viditelné toto pole nelze vrátit.

- **Identifikátor Microsoft CRM**: když společnost Microsoft vytvoří a přijme odkaz na společný prodej, toto pole se vyplní identifikátorem CRM společnosti Microsoft.

- **Produkty: zastaralé** – nepoužívejte toto pole nebo ho přidejte do oddílu CRM, je k dispozici pouze pro zpětnou kompatibilitu. Místo toho použijte řešení partnerského centra Microsoftu.

- **Audit**: záznam auditu jen pro čtení pro synchronizaci s odkazy partnerského centra

- **Řešení partnerského centra Microsoftu**: vlastní objekt pro přidružení řešení připraveného k prodeji nebo řešení Microsoftu s příležitostí. Jedno nebo více řešení lze z příležitosti přidat nebo odebrat. Před tím, než ho budete moct sdílet se společností Microsoft, je nutné, abyste před tím, než ho nasdíleli do Microsoftu, přidali aspoň jeden předprodejní Pokud chcete tento objekt přidružit k příležitosti, aktualizujte formulář příležitosti v CRM:

  Vyberte příslušnou kartu ve formuláři příležitostí a přidejte podmřížku, jak je znázorněno níže:

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="Formulář příležitosti":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="{alt-text}":::



- Po přidání řešení Microsoftu můžete předem vyplnit podrobnosti řešení připraveného k prodeji, aby je prodejci nemuseli přidávat. Pokud chcete přidat nové podrobnosti řešení, přejděte na objekt Microsoft Solution details v CRM a kliknutím na **Přidat záznam** přidejte jednu položku nebo použijte **nahrávání v Excelu** a přidejte víc položek.

:::image type="content" source="images/dynamic-1a.png" alt-text="Podrobnosti řešení":::

### <a name="scenarios"></a>ŘEŠENÍ

1. Referenční synchronizace při vytvoření nebo aktualizaci odkazu v CRM a synchronizovaných v partnerském centru:

   1. Přihlaste se k prostředí Dynamics 365 CRM s uživatelem, který má v části **příležitost** v aplikaci CRM přehled.

   2. Při vytváření nové příležitosti v prostředí Dynamics 365 se ujistěte, že se nachází oddíl partnerského centra Microsoftu.

   :::image type="content" source="images/dynamic-2a.png" alt-text="Nová příležitost"::: 

   3. Pokud chcete tuto příležitost synchronizovat s partnerským centrem, ujistěte se, že jste v zobrazení karta nastavili následující pole:

      - **Jak může Microsoft pomáhat?**: Pokud chcete vytvořit odkaz pro společný prodej, vyberte příslušnou možnost helpu.

         :::image type="content" source="images/dynamic-3a.png" alt-text="Jak získat příslušná pole v zobrazení karta":::

      - **Kontakt zákazníka**: Chcete-li vytvořit odkaz na společný prodej, přidejte kontakt zákazníka k příležitosti.
      - **Synchronizovat s partnerským centrem**: Ano

      - Řešení Microsoftu: Chcete-li sdílet odkaz s Microsoftem, přidejte k příležitosti platné řešení připraveného k prodeji nebo Microsoftu.
       
      
      :::image type="content" source="images/dynamic-4a.png" alt-text="ID řešení":::

   4. Až se příležitost vytvoří v Dynamics 365 s možností synchronizovat s partnerským centrem nastavenou na Ano, počkejte 10 minut a pak se přihlaste k účtu partnerského centra. Vaše odkazy budou synchronizovány s Dynamics 365 a identifikátorem odkazu. Odkaz na odkaz se vyplní. V případě selhání se pole auditu naplní informacemi o chybě.
     
    5. Podobně platí, že pokud chcete příležitost, která má možnost synchronizovat s partnerským centrem nastavenou na hodnotu Ano, aktualizovat příležitost v Dynamics 365 CRM, změny se synchronizují v účtu partnerského centra.

    6. Příležitosti, které byly úspěšně synchronizovány s partnerským centrem, budou označeny ikonou ✔ v Dynamics 365.

2. Referenční synchronizace při vytvoření nebo aktualizaci odkazu v partnerském centru Microsoftu a synchronizovaných v prostředí Dynamics 365:

   1. Přihlaste se k [řídicímu panelu](https://partner.microsoft.com/dashboard/home)partnerského centra.

   2. V nabídce na levé straně vyberte **odkazy** .

   3. Vytvořte si nový odkaz na společný prodej z partnerského centra tím, že vyberete  **novou možnost koupě** .

   4. Přihlaste se k prostředí Dynamics 365 CRM.

   5. Přejděte na **otevřené příležitosti**. Odkaz vytvořený v partnerském centru Microsoftu je teď synchronizovaný v Dynamics 365 CRM.

   6. Když vyberete synchronizovaný odkaz, vyplní se podrobnosti zobrazení karty.

## <a name="next-steps"></a>Další kroky

- [Správa potenciálních zákazníků](manage-leads.md)

- [Správa příležitostí ke spoluprodeji](manage-co-sell-opportunities.md)

- [Další informace o platformě Microsoft Power automatizuje?](/power-automate/)

- [Webhooky Partnerského centra](/partner-center/develop/partner-center-webhooks)
