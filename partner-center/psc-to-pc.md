---
title: Migrace z partnerského prodejního připojení (PSC)
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Přečtěte si, jak můžou partneři Microsoftu migrovat z partnerského prodejního připojení (PSC) do partnerského centra a vytvářet nebo spravovat obchody odesílané prodejci Microsoftu.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 12/07/2020
ms.openlocfilehash: 84863e96278ba17ecc9922ff9589abc504ff1fe0
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756185"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>Průvodce spoluprodejem v partnerském centru (PC) pro partnery, kteří se migrují z partnerského prodejního připojení (PSC)

**Příslušné role**

- Správce účtu
- Správce odkazů
- Prodejce partnera Sales Connect (PSC)
- Správce PSC (partner Sales Connect)
- Manažer koupě partnera Sales Connect (PSC)

Tento článek poskytuje pokyny pro partnery, kteří se migrují z partnerských obchodních připojení k partnerskému centru, aby mohli dál vytvářet a spravovat obchody v partnerském centru.

>[!Note]
> Pokud jste tady, protože jste si v části PSC o migraci viděli banner, jste na správném místě. Tato příručka se nedá použít pro posouzení řešení (SA) a obchodní partneři OEM Licensing, kteří spravují jejich obchody v PBV.

>[!Important]
> Od 1. května 2021 nebude vaše společnost moci vytvářet ani upravovat obchody v PBV. **Stále budete moct stáhnout existující data o seprodejech pomocí funkce hromadného exportu v PBV. Po tomto datu můžete také [migrovat otevřené obchody](psc-to-pc.md#psc-deals-migration) z PSC do partnerského centra.** <br><br> Pokud existují obchody, na kterých aktivně pracujete, které obsahují řešení s motivací, která jsou k dispozici pro vlastní prodej, máte dvě možnosti: <br><br> 1. Zaregistrujte se jako získaná a kompletní registrace koupě v řadiči PSC do 30. dubna 2021. <br> 2. [migrujte obchody](psc-to-pc.md#psc-deals-migration) do partnerského centra, abyste získali více času na práci a mohli začít registraci.

Jak víte, **Společnost ztratí přístup k PBV až do 31. května 2021**. Pořád ale najdete všechno, co chcete dělat v partnerském centru, jako je například vytváření spolupracujících obchodů, Správa vašich obchodů a jednání s obchody, které vám poslali prodejci Microsoftu.

K dispozici jsou však rozdíly. Následující pokyny vám mohou pomoci s přechodem do služby partner Center hladší a pružnější.

## <a name="before-you-move-things-you-need-to-know"></a>Než přesunete, co potřebujete znát

### <a name="if-you-are-a-psc-admin"></a>Pokud jste správce PSC

- K přihlášení do [partnerského centra](https://partner.microsoft.com/)potřebujete pracovní e-mail.
- Nastavte si účet pomocí [správce účtu](permissions-overview.md)partnerského centra.
- Přečtěte si tento dokument a Naučte se, jak v partnerském centru využít společný prodej.
- Nastavte uživatelské účty v partnerském centru pro všechny vaše uživatele PSC (role správce, správce řízení a prodejce) a přiřaďte jim [role Správce odkazů](permissions-overview.md).

>[!IMPORTANT]
> Ujistěte se, že ID MPN zobrazené v proužku PSC je dostupné v seznamu umístění MPN v partnerském centru.

:::image type="content" source="images/pscmigration/mpnidcheck.png" alt-text="Obrázek znázorňující hlavičku PSC, kde mohou partneři najít ID MPN.":::

 Pokud chcete ověřit, že ID MPN se zobrazuje jako umístění MPN partnerského centra, přihlaste se k [řídicímu panelu](https://partner.microsoft.com/dashboard)partnerského centra a pak vyberte **Nastavení** (ikona ozubeného kolečka) v pravém horním rohu obrazovky a pak **Nastavení účtu**. V nabídce vlevo na druhé úrovni vyberte **umístění** a zobrazí se seznam všech ID MPN a umístění přidružená k účtu partnerského centra.

### <a name="if-you-are-a-psc-deal-manager-or-seller"></a>Pokud jste správce koupě PSC nebo prodejce

- Pro přihlášení k [řídicímu panelu](https://partner.microsoft.com/dashboard)partnerského centra potřebujete pracovní e-mail.
- Pokud používáte nepracovní účet v PSC nebo máte pracovní e-mail pro jinou společnost než Partnerská společnost, požádejte správce PSC, aby vám pomohli nastavit účet.
- Pokud je váš účet partnerského centra nastavený na úplný, obraťte se na správce PSC bez ohledu na účet, který používáte k přihlášení k účtu PSC.
- Ověřte, zda máte přístup do partnerského centra a části s odkazy.
- Přečtěte si tento dokument, abyste pochopili pracovní postupy a změny v partnerském centru.

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>Jako správce v PSC se jedná o vaše další kroky.

V nabídce centrální navigace v partnerském centru vyberte možnost **odkazy** . Potvrďte, že máte přístup ke stránkám odkazů.

  >[!Note]
  > Možná se budete muset odhlásit z partnerského centra a znovu se přihlásit a aktualizovat přihlašovací údaje pro přístup ke stránkám s odkazy.

Pokud nevidíte možnost **odkazy** v nabídce partnerského centra nebo na stránkách souvisejících s odkazy, obraťte se na [správce účtu](permissions-overview.md) společnosti a požádejte ho, aby vám poskytl přístup k možnosti **odkazy** a související oblasti.

Jak najít správce účtu vaší společnosti:

1. Z ikony ozubeného kolečka v pravém horním rohu řídicího panelu partnerského centra vyberte **Nastavení účtu** .

1. V navigační nabídce druhé úrovně vyberte **Správa uživatelů** .

1. V horní části seznamu uživatelů vyberte rozevírací nabídku **Filtr** . Změňte možnost na **správce účtu**.

   Na stránce se zobrazí všichni správci účtu se svými příslušnými e-mailovými adresami. Pošlete jednu z nich e-mailem a požádejte je o přiřazení role Správce odkazů pro váš pracovní účet.

  :::image type="content" source="images/pscmigration/account-admin.png" alt-text="Obrázek znázorňující správce účtu na stránce Správa uživatelů nastavení partnera.":::

>[!Important]
>- Pokud vaše role zahrnuje jenom správu uživatelů v PSC, požádejte správce účtu vaší společnosti, aby vám přidělil roli [správce účtu](permissions-overview.md#manage-mpn-membership-and-your-company) v partnerském centru. 
>- Pokud vaše role zahrnuje i správu příležitostí pro společný prodej, požádejte o přiřazení role [Správce odkazů](permissions-overview.md#manage-referrals) .
> - Je vhodné také pojmenovat jednoho vedoucího řízení změn mezi správci PBV. Tím se zabrání všem správcům PSC v tom, aby se mohli jednotlivě spojit s správci účtů partnerského centra. Místo toho může být vedoucí změny v rámci správy změn primární osobou, která spolupracuje se správcem účtu partnerského centra.

## <a name="user-migration"></a>Migrace uživatelů

Po nastavení účtu v partnerském centru můžete pomocí Průvodce migrací uživatelů na stránce příležitosti společného prodeje automaticky přiřadit role partnerského centra zaměstnancům vaší společnosti.

>[!Note]
> Migraci uživatelů můžou provádět jenom [Správci účtu](permissions-overview.md#manage-mpn-membership-and-your-company) vaší společnosti. Pokud nemáte roli správce účtu, najděte správce účtu, který vám může pomáhat s nastavením uživatelských účtů pomocí Průvodce migrací uživatele.

:::image type="content" source="images/pscmigration/psc-user-migration.png" alt-text="Obrázek znázorňující Průvodce migrací uživatele":::

Správci účtů uvidí odkaz Průvodce migrací uživatele PSC na stránce příležitosti společného prodeje vedle Průvodce referenčními postupy. Kliknutím na odkaz můžete zahájit migraci uživatelů. Aby bylo možné zahájit migraci uživatelů, mohou správci vybrat odkaz. Tento krok migrace uživatelů můžou provádět víckrát, dokud se všem uživatelům nepřiřazují správné role v partnerském centru.

Tabulka migrace uživatelů má následující podrobnosti:

- Uživatelský účet – ID e-mailu zaměstnance
- Partnerský účet PSC – účet, ke kterému je zaměstnanec přidružen v účtu PSC
- PBV role uživatele – jedna ze tří rolí přiřazených do PSC.
- Umístění programu MPN počítače – umístění, pro které se uživateli přidají příslušné role počítačů. Partnerský účet PSČ MPN slouží k vyhledání ekvivalentního umístění programu MPN v partnerském centru za účelem přiřazení oprávnění. Celá organizace označuje ID MPN vOrg.
- POČÍTAČová role uživatele – zaměstnanci jsou přiřazeni role na základě jejich rolí uživatele PBV. Správci v řadiči PSC budou v počítači přiřazeni role správců odkazů. Prodávající bude mít přiřazenou roli uživatele odkazy v počítači. Přečtěte si další informace o rolích počítačů a o tom, co můžou uživatelé s těmito rolemi dělat v partnerském [centru.](permissions-overview.md#manage-referrals)
- POČÍTAČ AAD – tenant, ke kterému se uživatelé přiřazují v partnerském centru
- Stav: stav migrace je tři možné stavy.
    - **Nemigrováno** – uživatel nemá přiřazenou žádnou roli odkazů na počítače.
    - **Migrace** – uživatel byl úspěšně migrován s přiřazenou relevantní rolí, jak je znázorněno v tabulce.
    - **Chyba** : nepovedlo se dokončit migraci kvůli nějaké chybě.

V některých případech může migrace selhat a způsobit chyby. Tady je několik důvodů, proč může migrace způsobit chybu a některé způsoby, jak problém vyřešit:

1. Uživatelé PSC můžou používat nepracovní účet.

2. Uživatel PSC může používat účet z jiné domény než tu, kterou používáte v partnerském centru.

   Pokud chcete vyřešit chyby související s scénáři 1 a 2, požádejte uživatele, aby se přihlásil do partnerského centra pomocí svého pracovního účtu připojeného k vašemu tenantovi služby Azure AD. Váš [globální správce](permissions-overview.md#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles) může pomáhat.
   
   Pokud chcete najít globálního správce: 
   - Přihlaste se na [řídicí panel](https://partner.microsoft.com/dashboard) partnerského centra a v pravém horním rohu vyberte **Nastavení účtu** .
   - V levém navigačním panelu na druhé úrovni vyberte **Správa uživatelů** .
   - V horní části seznamu uživatelů vyberte rozevírací nabídku **Filtr** a změňte možnost **globální správce**. Na stránce se pak zobrazí všichni globální správci s příslušnými e-mailovými adresami. Položte jednu z nich, abyste přiřadili roli správce odkazů pro váš pracovní účet.
   
      Globální správce může buď vytvořit nový uživatelský účet v tenantovi Azure AD, nebo přiřadit přístup uživatelů typu Host k ostatním uživatelům účtu domény. Jakmile jsou účty nastavené pro všechny správce a uživatele pro řízení účtu PSC, musí se přihlásit k partnerskému centru, vybrat **odkazy** z nabídky vlevo a potvrdit, že uvidí stránku odkazy.

3. Uživatel už má přiřazenou roli reference v partnerském centru.
    - Můžete ověřit stávající roli uživatele. V pravém horním rohu partnerského centra vyberte **Nastavení** (ikona ozubeného kola) a pak **Nastavení účtu**. Když se zobrazí druhá levá navigační nabídka, vyberte **Správa uživatelů** a vyhledejte uživatele.

## <a name="psc-deals-migration"></a>Při migraci do PSC se zakoupí

Po dokončení migrace uživatelů můžete použít Průvodce migrací do provozu na stránce s příležitostmi k prodeji a přenést všechny opravňující otevřené obchody z PSC do počítače. **Odkaz na migraci se bude zobrazovat jenom správcům odkazů s celým oborem organizace v partnerském centru.** V pravém horním rohu stránky s příležitostmi k prodeji bude odkaz s názvem **"PBV rozdat Migration"** . tím se otevře Průvodce migrací obchodu.

Před zahájením migrace obchodu si přečtěte tento oddíl.

**Vhodné pro migraci**

Pouze některé obchody mají nárok na migraci z PSC do počítače. Tento průvodce migrací je navržený tak, aby pomáhal partnerům přenést své obchody do partnerského centra, kde stále aktivně pracují se svými zákazníky, aby mohli obchod uzavřít. **Pouze ty, které jsou v otevřeném stavu vytvořené z 1. ledna 2020 s platnými podrobnostmi o partnerském účtu (platným ID MPN) a neprovádí registraci služby, jsou vhodné pro migraci.**

**Není vhodné pro migraci**

- V rámci posouzení řešení se nedají migrovat na obchody.
- Obchodní obchody pro licencování OEM nejsou způsobilé k migraci koupí.
- Jakákoli taková práce, která byla označena jako získaná v PBV, není vhodná pro migraci. Registrace obchodu, pokud má nárok na obchody označené jako výhra, by měla být dokončena v PBV.

## <a name="pre-requisites-for-deal-migration"></a>Předpoklady pro migraci služby rozdat

Před zahájením migrace ze služby rozdat z počítače použijte následující pokyny a nastavte obchody v PBV pro úspěšnou migraci.

1. Všichni členové prodejního týmu ve vaší společnosti, kteří pracují s otevřenými obchody, jsou informováni o této migraci.
2. Členové prodejního týmu jsou vyškoleni k používání partnerského centra pro správu koupek.
3. Všechny obchody mají požadované informace, jak je popsáno níže.
    - Podrobnosti společnosti zákazníka včetně jména a adresy
    - Kontaktní údaje zákazníka, pokud jde o společný obchod
    - Aspoň jedno řešení
    - Aspoň jeden člen týmu se všemi podrobnostmi – křestní jméno, příjmení, ID e-mailu a telefonní číslo
    - Hodnota koupě
    - Odhadované datum uzavření koupě
    - Poznámky k partnerovi

Možnosti hromadného stažení a nahrání v PSC můžete použít k přidání všech chybějících detailů do obchodu pro všechny oprávněné obchody.

>[!Note]
> Migrace do provozu bude úspěšná i v případě, že nejsou splněné výše uvedené požadavky. Ale nemůžete změnit stav obchodu, pokud některá z výše uvedených povinných polí v partnerském centru nejsou k dispozici. Potom budete muset zadat všechny požadované informace v části obchody v partnerském centru, abyste na ně mohli začít pracovat. **Důrazně doporučujeme vyčistit opravňující obchody v PSC před jejich migrací do partnerského centra.**

Migrace obchodu na partnerském centru je postavená na jednom kliknutí. Stačí kliknout na tlačítko **migrovat obchody** , jakmile je vaše společnost připravená na migraci oprávněných obchodů. **Nemůžete zvolit obchody, které chcete migrovat z PSC. Pokud nechcete migrovat žádné obchody do partnerského centra, před zahájením migrace je přesuňte do zavřeného stavu v poli PSC.**

>[!Note]
> Po zahájení migrace **může trvat až 24 hodin**, než se budou tyto obchody migrovat.

Po dokončení migrace se stav zprávy změní na dokončeno s odkazem na sestavu migrace. Stáhněte si sestavu a zobrazte si podrobnosti o tom, které byly migrovány z protokolu PSC do počítače PC.

Sestava obsahuje níže uvedené podrobnosti.

1. **ID zapojení partnerského centra** – jedinečný identifikátor v partnerském centru pro všechny obchody ve službě Engagement. Existují dva obchody – jeden pro každého partnera a jeden pro Microsoft v rámci účasti v partnerském centru pro spoluprodejní zapojení.
2. **ID odkazu partnerského centra** – jedinečný identifikátor v partnerském centru pro obchod patřící partnerovi.
3. **Název obchodu** – identifikátor uvedený pro obchod v PBV.
4. **ID transakce PSC** – jedinečný identifikátor v poli PSC pro obchod.
5. **Chyby** – k označení, zda při migraci konkrétního obchodování dojde k chybě.

Všechny obchody, které byly úspěšně migrovány, nebudou viditelné v PSC. Můžete pokračovat v práci na migrovaných obchodech v počítači, včetně dokončení registrace koupě v počítači. V interakcích s prodejci Microsoftu pro spoluprodejní obchody se žádné změny nemění.

Služby migrované z PSC budou k dispozici na kartách příchozí a odchozí na základě zdroje obchodu. Všechny obchody, které vaše společnost sdílí, budou k dispozici na kartě odchozí a iniciované obchody společnosti Microsoft budou k dispozici na kartě příchozí v partnerském centru. Budou se vytvářet migrace po dvou typech obchodů.

1. **Společné obchody** – obchody, které jsou označené jako spoluprodej v rámci PSC, se vytvoří jako společné obchody v partnerském centru.
2. Probíhající **obchody** – obchody, které nejsou označené jako společný prodej, se budou vytvářet jako obchody řízené partnerským centrem v partnerském centru. Obchody na základě partnerských partnerů jsou viditelné prodejcům Microsoftu a je možné je upgradovat na společné obchody ještě před dosažením stavu terminálu (výhra, ztraceno). V případě, že jsou v rámci obchodu k dispozici vhodné řešení, mají také nárok na registraci v rámci partnerů.

>[!Important]
> Pokud dojde k chybám, protože některé obchody nemohly být migrovány, **můžete migraci obchodu znovu iniciovat kliknutím na tlačítko migrovat obchody**. Bude povoleno pouze v případě, že budou migrovány některé opravňující obchody. Tato akce bude užitečná také v případě, že jste ve fázi přechodu, kde se po zahájení migrace ze koupě vytvoří nějaké nové obchody v PBV.

Až budou všechny obchody úspěšně migrovány, zobrazí se zpráva s informacemi o tom, že se neúčtují **žádné obchody, aby** se **aktivovalo** tlačítko **migrovat obchody** .

Po dokončení migrace uživatelů a/nebo migraci za provozu použijte při rozhodování o strategii migrace následující pokyny:

Pokud má vaše společnost manažer vývoje pro vývoj (PDM) – když je nastavený účet partnerského centra a vaši uživatelé přesunuli a mají role a oprávnění, můžete své spolupracovní aktivity přesunout do partnerského centra. Informujte PDM, aby místo čekání na dokončení migrace nečekala na dokončení migrace. Tím umožníte, aby všechny vaše nové obchody pokračovaly do partnerského centra.

>[!Note]
>Po provedení tohoto přepínače budete moct pracovat jenom s existujícími aktivními obchody v PBV. Nemůžete ani vytvořit nové obchody ani dostávat žádné obchody od prodejců Microsoftu v PBV.

Pokud vaše společnost nemá PDM, ujistěte se, že jsou všechny uživatelské účty nastavené a ověřené všemi uživateli. Budete upozorněni e-mailem a bannerem v části PSC ohledně přesného data, kdy můžete začít prodávat v partnerském centru. Mějte na paměti, že stále budete muset spravovat existující aktivní obchody v PSC.

>[!Important]
> Až do 30. dubna 2021 zaregistrujete obchody, které jsou označené jako získané.

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>Další kroky pro správce PSC, správci koupích a PBV

Přečtěte si, jak v partnerském centru využít společný prodej.
Toto je důležitý krok, který vám pomůže připravit se na společný prodej v partnerském centru. Seznamte se s pracovními postupy a změnami v partnerském centru, abyste mohli efektivně prodávat hned. Začněte tím, že dokument přečtete úplně. V [galerii možností společného prodeje](https://aka.ms/cosellexperience)je dostupná i dobrá sada prostředků.

## <a name="major-differences-between-psc-and-pc-workflows"></a>Hlavní rozdíly mezi pracovními postupy PSC a počítačů

|**Scénář**|**Partner – prodejní připojení**|**Partnerské centrum**|
|-----|:-----|:-----|
|Role uživatelů|PBV má role správce, správce rozdat a prodejce.|POČÍTAČ má pouze roli [Správce odkazů](permissions-overview.md#manage-referrals) , která poskytuje oprávnění ke čtení i zápisu pro všechny obchody.|
|Pozvání Microsoftu k účasti na společném prodeji|Od Microsoft prodávajícího neexistují žádné výslovné otázky od partnera.|Partner bude muset vytvořit [explicitní požadavek](manage-co-sell-opportunities.md#add-solutions) , pokud je pro obchod potřeba pomáhat prodejce Microsoftu. Prodávající Microsoftu má možnost tuto žádost odmítnout.|
|Vypršení platnosti|Neexistují žádné pojmy na vypršení platnosti obchodu.|Pokud partner příchozí obchody neakceptují, vyprší za 14 dní. Totéž platí i u partnerských odchozích obchodů, kde můžou přejít do stavu vypršení platnosti, pokud na ně prodejce Microsoftu za 14 dnů nejedná.|
|Podrobnosti o prodejci Microsoftu|Zobrazuje se hned po vytvoření obchodu.|Podrobnosti o prodejci Microsoftu se sdílí s partnerem jenom v případě, že prodávající explicitně přijme pozvání k spoluprodeji od partnera.|
|[Privátní kanál](manage-co-sell-opportunities.md#types-of-co-sell-opportunities)|Není k dispozici.|Partneři můžou sdílet svůj kanál, aniž by jim poskytli přehled prodejců Microsoftu.|
|Řešení|Do obchodu lze přidat řešení patřící pouze k jednomu ceníku.|Partner může přidat [řešení](manage-co-sell-opportunities.md#add-solutions) , která patří do následujících seznamů. a) z katalogu Microsoft First stran (podobně jako role transakcí pro transakce v PBV) a c) řešení pro spoluprodej od jiných partnerů třetích stran (podobně jako role koupě ISV v PSC).|
|Přiřazení koupě|Pouze přiřazený prodejce může tyto obchody zobrazit a zpracovat.|Členové týmu mohou být přidáni do obchodu, aby mohli určit lidi, kteří pracují na práci, neexistují žádné blokování jiných správců odkazů v tom, aby si tyto obchody mohli zobrazit ani na nich nepracovali.|
|Organizace zákazníka|Bezplatná položka textu formuláře|Můžete hledat v [organizaci zákazníka](manage-co-sell-opportunities.md#select-your-customer) v rámci [databáze D&B](https://www.dnb.com/) pouhým zadáním několika znaků. Právní jméno a adresa se vyplní automaticky na základě volby.|
|Kontakt zákazníka|Není povinná.|Není povinné pro sdílení privátních kanálů. Požadováno v případě, že se prodejce Microsoftu pozve k účasti na žádosti o společný prodej.|
|Veřejné rozhraní API|Není k dispozici.|[Veřejné rozhraní API](/partner/develop/referrals) pro programové řízení odkazů partnerského centra|

## <a name="map-the-fields-in-psc-to-the-corresponding-fields-in-partner-center"></a>Mapování polí v PBV na odpovídající pole v partnerském centru

V této části se porovnávají (nebo "Maps") vybrané snímky obrazovky zobrazované pro PBV proti odpovídajícímu zobrazení v části související příležitosti partnerského centra.

Na každé dvojici snímků obrazovky se zobrazí číslované, žluté nebo červené kroužky:

- **Co znamenají žluté kroužky?** Očíslované – žluté kroužky se zobrazí jako první na každém snímku zobrazení PSC. Potom najdete doprovodného průvodce pro partnerských partnerů pod ním a mnoha stejnými čísly.

   Pokud chcete zjistit, jak se každé pole nebo atribut v PBV mapuje na jeho protějšek v partnerském centru, porovnejte očíslované kružnice s nimi ve dvou souvisejících snímcích obrazovky. Například odpovídá číslu, žlutému číslu "1" v prvním a PSC snímek obrazovky očíslované, žlutá "1" v druhém, na druhém snímku v partnerském centru pod ním.

- **Co znamená červené kolečko?** Pokud se zobrazí červený kroužek na jednom snímku obrazovky, který indikuje, že pole PSČ není v partnerském centru k dispozici.

Mapování polí pro PSČ do partnerského centra se zobrazí v následujících oblastech:

1. Domovská stránka PSC namapovaná na výchozí zobrazení příležitostí partnerského centra pro společné prodeje
1. Zobrazení mřížky PSC mapované na zobrazení obchodu partnerského centra
1. Zobrazení podrobností o koupi PSC mapované na zobrazení Podrobnosti o koupi partnerského centra
1. PBV přidat zobrazení produktů mapované do partnerského centra přidat zobrazení řešení
1. Zobrazení správy uživatelů PBV mapované na zobrazení správy uživatelů v partnerském centru
1. Zobrazení přiřazení role uživatele PBV mapované na zobrazení přiřazení role partnerského centra
1. Zobrazení oznámení PSC mapované na zobrazení oznámení v partnerském centru

### <a name="1---psc-home-page-mapped-to-the-partner-center-co-sell-opportunities-default-view"></a>1 – Domovská stránka PSC mapovaná na výchozí zobrazení příležitostí partnerského centra pro souběžné prodejy

Porovnejte párové a očíslované kružnice mezi horním snímkem PSC a snímkem partnerského centra pod ním. Odpovídající čísla ukazují, kde můžete najít funkci nebo atribut související s PSC v partnerském centru. Červené kroužky označují, že neexistuje žádné odpovídajícího pole partnerského centra.  

:::image type="content" source="images/pscmigration/homepage.png" alt-text="Obrázek znázorňující mapování polí mezi domovskou stránkou partnera Sales Connect a výchozím zobrazením příležitostí v partnerském centru pro společné prodeje." lightbox="images/pscmigration/home-page-expanded.png":::

### <a name="2---psc-grid-view-mapped-to-the-partner-center-deal-view"></a>2 – zobrazení tabulky PSC mapované na zobrazení obchodu v partnerském centru

Porovnejte párové a očíslované kružnice mezi horním snímkem PSC a snímkem partnerského centra pod ním. Čísla odpovídajících čísel ukazují, kde můžete najít funkci nebo atribut související s PSC v partnerském centru. Červené kroužky označují, že neexistuje žádné odpovídajícího pole partnerského centra.  

> [!NOTE]
> Pod snímky obrazovky se zobrazí další požadavky.

:::image type="content" source="images/pscmigration/gridview.png" alt-text="Obrázek znázorňující mapování polí mezi zobrazením mřížky partnera Sales Connect (PSC) a zobrazením obchodu v partnerském centru." lightbox="images/pscmigration/grid-view-expanded.png":::

**Zvláštní požadavky:**

- V partnerském centru neexistuje žádné zobrazení seznamu, jako je třeba PBV.  Všechny obchody jsou uvedené na základě nejnovějšího data přijetí nebo vytvoření s informacemi o zákaznících a typu obchodu. Ve výchozím nastavení je vybrán první obchod v zobrazení. Většina hodnot zobrazených ve formátu tabulky PSC je k dispozici v podrobném zobrazení obchodu v počítači.
- Role koupě není požadované pole v počítači. Nezobrazuje se ani se nezachycuje v žádném z pracovních postupů. Je odvozená automaticky na straně prodejce Microsoftu na základě řešení přidaných do obchodu.
- Datum poslední změny se nezobrazí na stránce podrobností odkazu v počítači PC. Partneři mohou pomocí funkce řazení seřadit obchody na základě data poslední aktualizace.

### <a name="3---psc-deal-details-view-mapped-to-partner-center"></a>3 – zobrazení podrobností o koupi PSC mapované na partnerské Centrum

Porovnejte párové kroužky na horním (PBV) snímku obrazovky, na které se nachází snímek obrazovky partnerského centra. Čísla odpovídajících čísel ukazují, kde můžete najít funkci nebo atribut související s PSC v partnerském centru. Červené kroužky označují, že v partnerském centru neexistuje žádné vyhovující pole ani oblast.

> [!NOTE]
> Pod snímky obrazovky se zobrazí další požadavky.

:::image type="content" source="images/pscmigration/dealdetails.png" alt-text="Obrázek znázorňující mapování polí mezi zobrazením podrobností o prodeji partnera Sales Connect (PSC) a zobrazení podrobností pro partnerské Centrum" lightbox="images/pscmigration/deal-details-expanded.png":::

**Zvláštní požadavky:**

- Partneři můžou upravit práci výběrem tlačítka upravit v zobrazení podrobností o partnerském obchodu (6). Po výběru tlačítka pro úpravy se všechna pole stanou upravitelná. Pak máte možnost buď uložit, nebo zrušit úpravy provedené v obchodu.
- Neexistuje možnost uzavřít obchod jako duplicitní v partnerském centru.
- Výsledek zákazníka není v partnerském centru k dispozici. Všechny podrobnosti související s interakcí zákazníků lze aktualizovat v části poznámky v počítači PC.
- Odhadované datum ukončení řešení je k dispozici pouze pro obchody OEM IOT v partnerském centru. Tyto informace se nezobrazují pro žádné jiné typy obchodování.
- V počítači není vyžadován licenční program. Tyto informace jsou automaticky odvozené v závislosti na řešeních vybraných v obchodu.

>[!Note]
>Jakoukoli práci označenou jako získanou nebo ztracenou nelze následně upravit. Při přesunu obchodu do jednoho z těchto stavů terminálu Vyzkoušejte opatrnost.

### <a name="4---psc-add-products-view-mapped-to-the-partner-center-add-solutions-view"></a>4-PBV zobrazení přidat produkty mapované na zobrazení partnerského centra přidat řešení

Porovnejte párové kroužky na horním (PBV) snímku obrazovky, na které se nachází snímek obrazovky partnerského centra. Čísla odpovídajících čísel ukazují, kde můžete najít funkci nebo atribut související s PSC v partnerském centru. Červené kroužky označují, že v partnerském centru neexistuje žádné vyhovující pole ani oblast.
  
:::image type="content" source="images/pscmigration/products.png" alt-text="Obrázek znázorňující mapování polí mezi zobrazením pro přidání produktů z partnerského prodeje (PSC) a v partnerském centru pro přidání řešení." lightbox="images/pscmigration/products-expanded.png":::

### <a name="5---user-management-in-psc-versus-partner-center"></a>5. Správa uživatelů v PSC a partnerské Centrum

Porovnejte párové kroužky na horním (PBV) snímku obrazovky, na které se nachází snímek obrazovky partnerského centra. Čísla odpovídajících čísel ukazují, kde můžete najít funkci nebo atribut související s PSC v partnerském centru. Červené kroužky označují, že v partnerském centru neexistuje žádné vyhovující pole ani oblast.  

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="Obrázek znázorňující mapování polí pro domovskou stránku správy uživatelů (PSC) pro partnery a zobrazení stránky pro správu uživatelů v partnerském centru v oblasti nastavení účtu."  lightbox="images/pscmigration/user-management-expanded.png":::

### <a name="6---user-role-assignment-in-psc-versus-partner-center"></a>6. přiřazení role uživatele v PSC a partnerském centru

Porovnejte párové kroužky na horním (PBV) snímku obrazovky, na které se nachází snímek obrazovky partnerského centra. Čísla odpovídajících čísel ukazují, kde můžete najít funkci nebo atribut související s PSC v partnerském centru. Červené kroužky označují, že v partnerském centru neexistuje žádné vyhovující pole ani oblast.  

:::image type="content" source="images/pscmigration/roles.png" alt-text="Obrázek znázorňující mapování polí mezi zobrazením přiřazení role partnerský prodej Connect (PSC) a zobrazení přiřazení role partnerského centra." lightbox="images/pscmigration/roles-expanded.png":::

**Zvláštní požadavky:**

- Ekvivalentní role pro správce PSC je role správce účtu v partnerském centru.
- V partnerském centru existuje jenom jedna role pro spoluprodejní správu koupek. Tato role je role Správce odkazů.

### <a name="7---notifications-in-psc-versus-partner-center"></a>7 – oznámení v PBV versus partnerské Centrum

Porovnejte párové kroužky na horním (PBV) snímku obrazovky, na které se nachází snímek obrazovky partnerského centra. Čísla odpovídajících čísel ukazují, kde můžete najít funkci nebo atribut související s PSC v partnerském centru. Červené kroužky označují, že v partnerském centru neexistuje žádné vyhovující pole ani oblast.  

:::image type="content" source="images/pscmigration/notifications.png" alt-text="Obrázek znázorňující mapování mezi oznámeními partnera Sales Connect (PSC) a zobrazením oznámení partnerského centra"  lightbox="images/pscmigration/notifications-expanded.png":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>Přesun z PSC do partnerského centra – Nejčastější dotazy

V následujících částech najdete odpovědi na časté otázky týkající se migrace.

### <a name="1---what-should-i-do-if-i-dont-have-access-to-partner-center"></a>1 – co mám dělat, když nemám přístup k partnerskému centru?

Můžete se obrátit na správce, kteří jsou uvedeni na stránce "bez přístupu", a získat tak přiřazené role. V části referenčních seznamů budete potřebovat roli [Správce odkazů](permissions-overview.md#manage-referrals) pro oprávnění ke čtení a zápisu. Pokud spravujete jenom obchodní profily, budete potřebovat roli správce obchodního profilu v partnerském centru.

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="Obrázek znázorňující, že v partnerském centru není prostředí pro přístup.":::

### <a name="2---who-can-grant-me-access-to-the-referrals-section-in-partner-center"></a>2 – kdo mi může udělit přístup k části odkazy v partnerském centru?

[Správce účtu](permissions-overview.md#manage-mpn-membership-and-your-company) vám může udělit přístup k kartě odkazy. Pokud chcete najít správce účtu, vyberte **Nastavení účtu** z ikony ozubeného kolečka v pravém horním rohu [řídicího panelu](https://partner.microsoft.com/dashboard)partnerského centra. Pak vyberte **Správa uživatelů** z druhé úrovně vlevo v navigačním panelu. V horní části seznamu uživatelů vyberte rozevírací nabídku **Filtr** a změňte možnost na **správce účtu**. Na stránce se zobrazí všichni správci účtu se svými příslušnými e-mailovými adresami. Položte jednu z nich, abyste přiřadili roli správce odkazů pro váš pracovní účet.

### <a name="3---the-new-deal-button-is-greyed-out-for-our-account-what-should-i-do-to-start-creating-deals"></a>3 – tlačítko + nové koupě je pro náš účet šedé. Co mám udělat, pokud chcete začít vytvářet obchody?

K tomu dochází pouze v případě, že v partnerském centru nejsou k dispozici žádná řešení připravená k prodeji do organizace programu MPN. Kontaktujte PDM a Získejte ID MPN vašich řešení, nebo vytvořte lístek podpory, který zmiňuje tento problém, "nové možnosti koupě šedé po migraci PSC".

### <a name="4---can-i-assign-deals-to-a-specific-person-from-our-organization-like-psc"></a>4 – mohu na konkrétní osobu přiřadit nějaké obchody, jako je například PSC?

Členům týmu můžete přiřadit konkrétní obchod. Neblokuje zobrazení ani nefunguje na těchto vzdaných správcích odkazů.

### <a name="5---is-there-a-view-of-all-the-deals-assigned-to-me"></a>5 – existuje pohled na všechny obchody přiřazené mně?

Můžete použít funkci oblíbené, což je karta na úrovni uživatele. Všechny obchody, které jsou vám přiřazeny jako oblíbené, můžete označit jako oblíbené a získat tak rychlý přístup k těmto seznámení.

### <a name="6---is-there-a-read-only-view-for-the-deals"></a>6 – pro tyto obchody existuje zobrazení jen pro čtení?

Ne, v části referenčních seznamů neexistují žádné zobrazení obchodů jen pro čtení. Všichni správci odkazů budou mít úplný přístup pro čtení a zápis pro všechny obchody.

### <a name="7---how-can-i-register-a-deal-after-marking-it-as-won"></a>7 – Jak můžu zaregistrovat práci, když ji označíte jako získanou?

Pokud obchod splňuje níže uvedená kritéria, zobrazí se automaticky otevírané okno pro zahájení [registrace](./register-deals.md).

- Je k dispozici vhodné řešení, které by mělo být spojeno s motivací.
- Prodejce Microsoftu se zve k účasti na obchodování nebo vás pozval k obchodování.
- Karta Microsoft je ve stavu přijato nebo získáno v partnerském centru.

### <a name="8---i-get-an-error-message-when-i-select-the-new-deal-registration-button-in-the-deal-registration-section-how-can-i-register-my-deals"></a>8 – zobrazí se chybová zpráva, když v části registrace Koupek vyberem tlačítko + Nová registrace koupek. Jak můžu zaregistrovat svoje obchody?

Tlačítko **+ Nová registrace koupě** se používá jenom pro partnery, kteří jsou zaregistrovaní v programu ISV Connect pro registraci obchodu bez odpovídající možnosti společného prodeje v partnerském centru. Pro registraci obchodů s příležitostí pro spoluprodeji se zobrazí automaticky otevírané okno, když je práce označena jako získaná a pokud splňuje kritéria pro registraci koupek.

### <a name="9---is-adding-a-customer-organization-mandatory"></a>9 – je nutné přidat organizaci zákazníka povinnou?

Ano, v partnerském centru je přidání [organizace zákazníka](./manage-co-sell-opportunities.md#select-your-customer) povinné. Začněte tím, že vyhledáte umístění, kde se zákazník nachází. Na základě podrobností, které máte; můžete být specifické, včetně přesného názvu budovy, nebo jenom poskytnout podrobnosti o městech. Hledání v organizaci načte všechny platné entity, které odpovídají názvu, který zadáte, abyste nemuseli zadávat žádné podrobnosti o adrese. Všechny podrobnosti se vyplní automaticky na základě vybrané organizace.

### <a name="10---are-customer-contact-details-mandatory"></a>10 jsou povinnými kontaktními údaji zákazníka?

Závisí na [typu obchodu](./manage-co-sell-opportunities.md#types-of-co-sell-opportunities) , kterou vytváříte. Pokud sdílíte svůj kanál a nevyžadujete žádnou technickou podporu z prodejní organizace Microsoftu, můžete se rozhodnout nedávat kontaktní údaje od zákazníka. Pokud společně vydáváte, kde aktivně hledáte pomocníka od společnosti Microsoft, budete muset zadat kontaktní údaje zákazníka. Před vytvořením žádosti o společný prodej v partnerském centru byste měli získat výslovný souhlas od zákazníka.

### <a name="11---how-many-solutions-can-i-add-to-a-deal"></a>11 – kolik řešení mohu do obchodu přidat?

Do obchodu můžete přidat až 50 řešení (podobných produktům v PBV). Na rozdíl od PSC můžete kombinovat řešení ze svých vlastních řešení vhodných pro vlastní prodej, SKU Microsoft First stran a dalších oprávněných řešení pro vlastní prodej třetích stran. V partnerském centru neexistuje žádná role koupě, která by se měla vybrat nebo k dispozici. U položek SKU společnosti Microsoft můžete volitelně přidat množství a cenu za každou SKU, která je do obchodu přidána.

### <a name="12---when-will-i-get-to-know-the-microsoft-seller-details-after-creating-a-deal"></a>12. po vytvoření obchodu se dozvíte o podrobnostech o prodejci Microsoftu?

Prodejci Microsoftu se přiřazují až po splnění přesného požadavku na podporu, který jste uvedli při vytváření obchodu s relevantním prodejcem na straně Microsoftu. I po přiřazení budou mít prodejci Microsoftu možnost přijmout nebo odmítnout pozvánku pro spoluprodej. V případě, že prodávající akceptuje pozvání k spoluprodeji, bude aktualizace aktualizována o kontaktní údaje prodejce Microsoftu. Smlouva SLA, kterou prodejci Microsoftu budou působit na obchod, je 14 dní. Jedná se o stejnou smlouvu SLA, kterou partneři musí v obchodu řešit předtím, než se do stavu vypršení platnosti.

### <a name="13---where-can-i-find-the-opportunity-id"></a>13 – kde můžu najít ID příležitosti?

ID příležitosti v PSC je stejné jako ID koupě v počítači. ID koupě můžete najít vedle názvu obchodu při otevření jakékoli koupě.

### <a name="14---how-can-my-pdm-get-access-to-pc"></a>14. jak má PDM získat přístup k počítači?

Partnerskému centru nemůže mít váš PDM přímý pøístup na rozdíl od PSC. Existuje několik možností, jak tuto funkci povolit, které jsou uvedeny níže.

- OCP Insights – Pokud PDM jenom zobrazují obchody a průběh, které s nimi souvisejí, můžou pomocí portálu OCP Insights získat zobrazení vaší organizace. Toto je interní nástroj, který je dostupný jenom pro PDM. Upozorňujeme, že pro uživatele vaší společnosti nejsou k dispozici informace OCP Insights.
- Uživatel typu Host v partnerském centru – účet PDM můžete přidat @microsoft.com jako uživatele typu Host v partnerském centru a přiřadit jim roli správce odkazů, aby mohli zobrazit a pracovat s referenčními seznamy.
- Vytváří se [Nový uživatel](./create-user-accounts-and-set-permissions.md#add-a-new-user) ve vašem tenantovi – můžete vytvořit nového uživatele ve vlastním tenantovi a sdílet tyto podrobnosti s PDM, aby mohli zobrazit a pracovat s odkazy podobnými ostatním uživatelům s odkazem ve vašem účtu.

## <a name="finding-the-correct-mpn-id-if-your-account-in-psc-is-not-associated-with-a-valid-mpn"></a>Hledání správného ID MPN, pokud váš účet v PBV není přidružený k platnému programu MPN

Pokud jste tady, vzhledem k tomu, že jste si všimli banneru s názvem PSC neplatný problém přidružení ID MPN, jste na správném místě. Váš účet může být propojený s neplatným ID MPN z následujících důvodů.

- Vaše společnost nemá účet partnerského centra.
- V PDM došlo k chybě při zadávání ID MPN účtu do interních systémů, které propojí váš účet PSC s účtem partnerského centra (MPNID).
- Vaše společnost nedokončila migraci z centra pro členství v partnerech (PMC) do počítače.

Nejdřív vyhledejte správné ID MPN pomocí následujících kroků.

- Přihlaste se k účtu partnerského centra.
- Pomocí pokynů uvedených v [dokumentaci nastavení účtu](./partner-center-account-setup.md#locate-your-mpn-id) vyhledejte ID MPN.

Níže je zobrazený snímek obrazovky s přesným umístěním, kde můžete najít ID MPN partnerského centra.

:::image type="content" source="images/pscmigration/findingMPNID.png" alt-text="Obrázek znázorňující nastavení účtu, kde partner může najít své ID MPN."  lightbox="images/pscmigration/findingMPNID.png":::

Další, 

- Pokud máte PDM, požádejte je, aby se opravilo ID programu MPN se správným ID MPN z účtu partnerského centra.
- Pokud nemáte PDM, pošlete e-mail na adresu uvedenou v proužku PSC s použitím informací účtu PSC zobrazených v hlavičce PSC a správného ID MPN z účtu partnerského centra.

## <a name="resources-to-help-you-create-and-manage-your-deals-in-partner-center"></a>Materiály, které vám pomůžou vytvářet a spravovat vaše obchody v partnerském centru

Pokud jste si ještě neučinili témata nápovědy pro spoluprodeji, pomůžou vám následující zdroje informací, které vám pomůžou se správou obchodů v partnerském centru.

|**K tomu**   |**Přečtěte si:**   |
|-----------------------|:-----------------------|
|Přehled karet a navigace na stránce s příležitostmi k vzájemnému prodeji|[Navigace v části společný prodej](./manage-co-sell-opportunities.md#navigating-the-co-sell-section)|
|Výběr organizace zákazníka ze seznamu D&B |[Vybrat zákazníka](./manage-co-sell-opportunities.md#select-your-customer)|
|Úprava polí v části Podrobnosti o koupi|[Podrobnosti o obchodu](./manage-co-sell-opportunities.md#deal-details)|
|Přidání členů týmu do týmu pro koupce|[Přidání zaměstnanců](./manage-co-sell-opportunities.md#add-team-members)|
|Reakce na společný obchod|[Správa obchodů společného prodeje](./manage-co-sell-opportunities.md#responding-to-a-co-sell-opportunity)
|Zaregistrujte obchody, které jste vyhráli v partnerském centru |[Registrace nové koupě](./register-deals.md)
|Získejte přehledy odkazů a zjistěte, jak dělají vaše odkazy. |[Přehledy referenčních seznamů](./referral-insights.md)
|Vytváření a Správa obchodního profilu|[Správa obchodního profilu](./create-a-marketing-profile.md)
|Správa zájemců pro obchodní profil |[Správa potenciálních zákazníků](./manage-leads.md)|

## <a name="next-steps"></a>Další kroky


- [Partner Sales Connect to](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) Workbook – sešit – sešit pro zarovnávání prodejních procesů a rolí partnerů pomocí nových prodejních procesů prostřednictvím partnerského centra vs. partner Sales Connect.
- [Provozní příručka pro partnery v partnerském centru](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) – pokyny k identifikaci operačního modelu prostřednictvím partnerského centra za účelem správy zájemců nebo příležitostí společného prodeje a evidence obchodů.
- [Balíček pro správu referenčních](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) informací – vizuální podrobné pokyny pro správu zájemců a příležitostí k prodeji prostřednictvím partnerského centra.
- [Publikování a správa na komerčním webu Marketplace](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) – vizuální podrobné pokyny k vytváření, správě a publikování nabídek prostřednictvím partnerského centra na komerčním tržišti.