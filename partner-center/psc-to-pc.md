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
ms.openlocfilehash: 584f8a7f2794cb64be49fe7f790904eff50c4c26
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855094"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>Průvodce spoluprodejem v partnerském centru (PC) pro partnery, kteří se migrují z partnerského prodejního připojení (PSC)

**Příslušné role**: správce účtu | Správce odkazů | Prodejce partnera Sales Connect (PSC) | Správce PSC (partner Sales Connect) | Manažer koupě partnera Sales Connect (PSC)

Tento článek poskytuje pokyny pro partnery, kteří se migrují z partnerských obchodních připojení k partnerskému centru, aby mohli dál vytvářet a spravovat obchody v partnerském centru.

>[!Note]
> Pokud jste tady, protože jste si v části PSC o migraci viděli banner, jste na správném místě. Tato příručka se nedá použít pro posouzení řešení (SA) a obchodní partneři OEM Licensing, kteří spravují jejich obchody v PBV.

>[!Important]
> Od 1. dubna 2021 nebude vaše společnost moci vytvářet ani upravovat obchody v PBV. **Stále budete moct stáhnout existující data o seprodejech pomocí funkce hromadného exportu v PBV. Po tomto datu můžete také [migrovat otevřené obchody](psc-to-pc.md#psc-deals-migration) z PSC do partnerského centra.** <br><br> Pokud existují obchody, na kterých aktivně pracujete, které obsahují řešení s motivací, která jsou k dispozici pro vlastní prodej, máte dvě možnosti: <br><br> 1. Zaregistrujte se jako získaná a kompletní registrace koupě v řadiči PSC do 31. března 2021. <br> 2. [migrujte obchody](psc-to-pc.md#psc-deals-migration) do partnerského centra, abyste získali více času na práci a mohli začít registraci.

Jak víte, **Společnost ztratí přístup k řadiči PSC po 30. dubnu 2021**. Pořád ale najdete všechno, co chcete dělat v partnerském centru, jako je například vytváření spolupracujících obchodů, Správa vašich obchodů a jednání s obchody, které vám poslali prodejci Microsoftu.

K dispozici jsou však rozdíly. Následující pokyny vám mohou pomoci s přechodem do služby partner Center hladší a pružnější.

## <a name="before-you-move-things-you-need-to-know"></a>Než přesunete, co potřebujete znát

### <a name="if-you-are-a-psc-admin"></a>Pokud jste správce PSC

- K přihlášení do [partnerského centra](https://partner.microsoft.com/)potřebujete pracovní e-mail.
- Nastavte svůj účet pomocí správce Partnerské centrum [účtu.](permissions-overview.md)
- Přečtěte si tento dokument a zjistěte, jak Partnerské centrum spoluprodávat v tomto dokumentu.
- Nastavte uživatelské účty v Partnerské centrum pro všechny uživatele PSC (role správce, správce dohody a prodejce) a přiřaďte jim role [správce referenčních seznamu.](permissions-overview.md)

>[!IMPORTANT]
> Ujistěte se, že ID MPN zobrazené v banneru PSC je k dispozici v seznamu umístění MPN v Partnerské centrum.

:::image type="content" source="images/pscmigration/mpnidcheck.png" alt-text="Obrázek znázorňující banner PSC, kde partneři mohou najít ID MPN":::

 Pokud chcete ověřit, že se ID MPN zobrazuje jako umístění Partnerské centrum MPN, přihlaste se k řídicímu panelu [Partnerské centrum,](https://partner.microsoft.com/dashboard)pak v pravém horním rohu obrazovky vyberte Nastavení **(ikona** ozubeného kola) a pak Nastavení **účtu.** V levé navigační nabídce druhé úrovně  vyberte Umístění. Zobrazí se seznam všech ID a umístění MPN přidružených k účtu mpn Partnerské centrum účtu.

### <a name="if-you-are-a-psc-deal-manager-or-seller"></a>Pokud jste manažerem nebo prodejcem dohody PSC

- K přihlášení k řídicímu panelu služby Partnerské centrum [pracovní e-mail.](https://partner.microsoft.com/dashboard)
- Pokud v PSC používáte nepracujte účet nebo pokud je váš pracovní e-mail pro jinou společnost než partnerská společnost, požádejte o pomoc s nastavením účtu správce PSC.
- Ověřte u správce PSC, jestli Partnerské centrum váš účet je dokončený bez ohledu na účet, který používáte pro přihlášení k PSC.
- Ověřte, jestli máte přístup k Partnerské centrum a části Referenční odkazy.
- Přečtěte si tento dokument, abyste porozuměli pracovním postupům a změnám v Partnerské centrum.

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>Toto jsou vaše další kroky jako správce v PSC.

V Partnerské centrum levé navigační nabídce vyberte možnost **Referenční** odkazy. Ověřte, že máte přístup na stránky Referenční odkazy.

  >[!Note]
  > Možná se budete muset odhlásit z Partnerské centrum a znovu se přihlásit, aby se vaše přihlašovací údaje mohly aktualizovat, abyste měli přístup ke stránkám Referenční odkazy.

Pokud možnost Referenční seznam  v nabídce Partnerské centrum nebo na stránkách souvisejících s referenčními seznamy nevidíte, obraťte se na správce účtu vaší společnosti a požádejte ho, aby vám dal přístup k možnosti **Referenční** seznam a související oblasti. [](permissions-overview.md)

Vyhledání správce účtu vaší společnosti:

1. Z ikony ozubeného kolečka v pravém horním rohu řídicího panelu partnerského centra vyberte **Nastavení účtu** .

1. V navigační nabídce druhé úrovně vyberte **Správa uživatelů** .

1. V horní části seznamu uživatelů vyberte rozevírací nabídku **Filtr** . Změňte možnost na **správce účtu**.

   Na stránce se zobrazí všichni správci účtu se svými příslušnými e-mailovými adresami. Pošlete jednu z nich e-mailem a požádejte je o přiřazení role Správce odkazů pro váš pracovní účet.

  :::image type="content" source="images/pscmigration/account-admin.gif" alt-text="Obrázek znázorňující správce účtu na stránce Správa uživatelů nastavení partnera.":::

>[!Important]
>- Pokud vaše role zahrnuje jenom správu uživatelů v PSC, požádejte správce účtu vaší společnosti, aby vám přidělil roli [správce účtu](permissions-overview.md#manage-mpn-membership-and-your-company) v partnerském centru. 
>- Pokud vaše role zahrnuje i správu příležitostí pro společný prodej, požádejte o přiřazení role [Správce odkazů](permissions-overview.md#manage-referrals) .
> - Je vhodné také pojmenovat jednoho vedoucího řízení změn mezi správci PBV. Tím se zabrání všem správcům PSC v tom, aby se mohli jednotlivě spojit s správci účtů partnerského centra. Místo toho může být vedoucí změny v rámci správy změn primární osobou, která spolupracuje se správcem účtu partnerského centra.

## <a name="user-migration"></a>Migrace uživatelů

Po nastavení účtu v partnerském centru můžete pomocí Průvodce migrací uživatelů na stránce příležitosti společného prodeje automaticky přiřadit role partnerského centra zaměstnancům vaší společnosti.

>[!Note]
> Migraci uživatelů můžou provádět jenom [Správci účtu](permissions-overview.md#manage-mpn-membership-and-your-company) vaší společnosti. Pokud nemáte roli správce účtu, najděte správce účtu, který vám může pomáhat s nastavením uživatelských účtů pomocí Průvodce migrací uživatele.

:::image type="content" source="images/pscmigration/user-migration.gif" alt-text="Obrázek znázorňující Průvodce migrací uživatele":::

Správci účtů uvidí odkaz Průvodce migrací uživatele PSC na stránce příležitosti společného prodeje vedle Průvodce referenčními postupy. Kliknutím na odkaz můžete zahájit migraci uživatelů. Aby bylo možné zahájit migraci uživatelů, mohou správci vybrat odkaz. Tento krok migrace uživatelů může provést vícekrát, dokud nebudou mít všichni uživatelé přiřazené správné role v Partnerské centrum.

Tabulka migrace uživatelů obsahuje následující podrobnosti:

- Uživatelský účet – ID e-mailu zaměstnance
- Partnerský účet PSC – Účet, ke kterému je zaměstnanec přidružený v PSC
- Role uživatele PSC – jedna ze tří rolí přiřazených v PSC.
- Umístění PC MPN – umístění, pro které bude mít uživatel příslušné role počítače. MPN partnerského účtu PSC slouží k vyhledání ekvivalentního umístění MPN v Partnerské centrum přiřazení oprávnění. Celá organizace označuje ID MPN virtuální organizace.
- Role uživatele počítače – Zaměstnanci mají přiřazené role na základě jejich uživatelských rolí PSC. Správce v PSC bude mít v počítači přiřazené role správce referenčních odkazů. Prodejce bude mít v počítači přiřazenou roli uživatele referenčních odkazů. Další informace o rolích počítačů a o tom, co mohou uživatelé s těmito rolemi dělat v Partnerském [centru, najdete tady.](permissions-overview.md#manage-referrals)
- Tenant AAD v PC – tenant, ke kterému jsou uživatelé přiřazení v Partnerské centrum
- Stav – Existují tři možné stavy pro stav migrace.
    - **Nemigrován** – Uživatel nemá přiřazenou žádnou roli referenčních doporučení v počítači.
    - **Migrován** – Uživatel byl úspěšně migrován s přiřazenou odpovídající rolí, jak je znázorněno v tabulce.
    - **Chyba** – Migraci se nepodařilo dokončit kvůli nějaké chybě

Někdy může migrace selhat a vést k chybám. Tady je několik důvodů, proč migrace může způsobit chybu, a některé způsoby, jak tento problém vyřešit:

1. Uživatelé PSC mohou používat nepracují účet.

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

K migraci z PSC do PC mají nárok pouze některé dohody. Tento průvodce migrací je vytvořen tak, aby partnerům pomohl Partnerské centrum tam, kde stále aktivně spolupracuje se svými zákazníky na uzavření dohody. **Na migraci mají nárok jenom dohody, které jsou v otevřeném stavu vytvořené od 1. ledna 2020 s platnými podrobnostmi o partnerském účtu (platné ID MPN) a procházejí registrací dohody.**

**Není možné migrací**

- Dohody o posouzení řešení nemají nárok na migraci dohody
- Obchodní dohody o licencování OEM nemají nárok na migraci dohody
- Žádná dohoda, která byla v PSC označena jako vyhrála, nemá nárok na migraci. Registrace dohody, pokud má nárok na obchody označené jako won, by se měla dokončit v PSC.

## <a name="pre-requisites-for-deal-migration"></a>Předpoklady pro migraci dohody

Před zahájením migrace dohody z PC postupujte podle následujících pokynů a nastavte obchody v PSC pro úspěšnou migraci.

1. O této migraci jsou informováni všichni členové prodejního týmu ve vaší společnosti, kteří pracují na otevřených obchodech.
2. Členové prodejního týmu jsou vytrénované tak, aby Partnerské centrum k řízení dohody.
3. Obchody mají všechny požadované informace, jak je popsáno níže.
    - Podrobnosti o společnosti zákazníka, včetně názvu a adresy
    - Kontaktní údaje zákazníka, pokud se jedná o dohodu o spoluprodát
    - Alespoň jedno řešení
    - Alespoň jeden člen týmu se všemi podrobnostmi – jméno, příjmení, ID e-mailu a telefonní číslo
    - Hodnota dohody
    - Odhadované datum uzavření dohody
    - Poznámky pro partnery

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

Všechny obchody, které byly úspěšně migrovány, nebudou viditelné v PSC. Můžete pokračovat v práci na migrovaných dohod v počítači, včetně dokončení registrace dohody v PC. Interakce s prodejci Microsoftu pro dohody o spoluprodávačích se nemění.

Dohody migrované z PSC budou k dispozici na kartách Příchozí a Odchozí v závislosti na zdroji dohody. Všechny dohody sdílené vaší společností budou dostupné na kartě Odchozí a dohody iniciované Microsoftem budou k dispozici na kartě Příchozí v Partnerské centrum. Po migraci budou vytvořeny dva typy dohod.

1. **Dohody o spoluprodávce** – Dohody, které jsou v PSC označené jako spoluprodávné, se vytvoří jako dohody o spoluprodávce v Partnerské centrum.
2. **Dohody vedené partnery** – Dohody, které nejsou označené jako spoluprodáky, se vytvoří jako dohody vedené partnery v Partnerské centrum. Nabídky vedené partnery jsou viditelné prodejcům Microsoftu a před dosažením stavu terminálů (won, lost) je možné upgradovat na dohody o spoluprodávači. Dohody vedené partnery mají také nárok na registraci dohody, pokud se v rámci dohody nachází řešení s nárokem na pobídky.

>[!Important]
> Pokud dojde k chybám, kvůli kterým se některé dohody nemigrují, můžete migraci dohody znovu zahájit kliknutím na tlačítko **Migrovat dohody.** Tato možnost se povolí jenom v případě, že ještě existuje několik oprávněných dohod, které se mají migrovat. To bude užitečné také v případě, že jste ve fázi přechodu, ve které se v PSC vytvářejí nové dohody po zahájení migrace dohody.

Po úspěšné migraci všech dohod se zobrazí banner No **deals to migrate** (Žádné dohody o migraci) se zakázaným tlačítkem Migrate **deals** (Migrace **dohod).**

Po dokončení migrace uživatelů nebo dohody o migraci použijte následující pokyny k rozhodnutí o strategii migrace:

Pokud má vaše společnost manažera pro vývoj partnerů (PDM) – Když je váš účet Partnerské centrum nastavený a vaši uživatelé se přesunuli a mají role a oprávnění, můžete aktivity spoluprodáva přesunout do Partnerské centrum. Informujte PDM, aby místo čekání na dokončení migrace nečekala na dokončení migrace. Tím umožníte, aby všechny vaše nové obchody pokračovaly do partnerského centra.

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
|Pozvání Microsoftu k účasti na společném prodeji|Od Microsoft prodávajícího neexistují žádné výslovné otázky od partnera.|Partner bude muset vytvořit [explicitní požadavek](manage-co-sell-opportunities.md#add-solutions) , pokud je pro obchod potřeba pomáhat prodejce Microsoftu. Prodejce Microsoftu má možnost žádost odmítnout.|
|Vypršení platnosti|Neexistuje žádný koncept vypršení platnosti dohody.|Platnost příchozích dohod partnerů vyprší za 14 dnů, pokud je partner nepřijme. Totéž platí i pro odchozí dohody partnerů, jejichž platnost vyprší, pokud prodejce Microsoftu za 14 dnů nevyhodí.|
|Podrobnosti o prodejci Microsoftu|Viditelné, jakmile se vytvoří dohoda.|Podrobnosti o prodejci Microsoftu se s partnerem sdílí jenom v případě, že prodejce výslovně přijme pozvánku ke spoluprodávači od partnera.|
|[Privátní kanál](manage-co-sell-opportunities.md#types-of-co-sell-opportunities)|Není k dispozici.|Partneři mohou sdílet svůj kanál, aniž by prodejcům Microsoftu dávají přehled.|
|Řešení|Řešení, která patří pouze do jednoho ceníku, je možné přidat do dohody.|Partner může přidat [řešení,](manage-co-sell-opportunities.md#add-solutions) která patří do následujících seznamů. a) Vlastní řešení b) Řešení z katalogu Microsoftu první strany (podobně jako u role dohody o transakcích v PSC) a c) Řešení spoluproduování od jiných partnerů třetích stran (podobně jako u role dohody ISV v PSC).|
|Přiřazení dohody|Jen přiřazený prodejce může obchody zobrazit a jednat s ohledem na to.|Členy týmu je možné přidat do dohody, aby mohli určit lidi, kteří pracují na dohody, a ostatní správci referenčních seznamu nemají žádné blokování v zobrazení těchto dohod nebo v jejich náplní.|
|Organizace zákazníků|Zadání textu volného formuláře.|Zadáním několika znaků [můžete v](manage-co-sell-opportunities.md#select-your-customer) organizaci zákazníka vyhledat databázi D [&B.](https://www.dnb.com/) Právní název a adresa se vyplní automaticky podle volby.|
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
1. Zobrazení správy uživatelů PSC namapované na Partnerské centrum správy uživatelů
1. Zobrazení přiřazení role uživatele PSC namapované Partnerské centrum zobrazení přiřazení role uživatele
1. Zobrazení oznámení PSC namapované na Partnerské centrum oznámení

### <a name="1---psc-home-page-mapped-to-the-partner-center-co-sell-opportunities-default-view"></a>1 . Domovská stránka PSC namapovaná na výchozí Partnerské centrum příležitosti ke spoluprodávce

Porovnejte odpovídající očíslované kruhy mezi horním snímkem obrazovky PSC a Partnerské centrum snímku obrazovky pod nimi. Odpovídající čísla ukazují, kde můžete najít funkci nebo atribut související s PSC v Partnerské centrum. Červené kruhy označují, že v poli Partnerské centrum žádná shoda.  

:::image type="content" source="images/pscmigration/homepage.png" alt-text="Obrázek znázorňující mapování polí mezi domovskou stránkou aplikace Partner Sales Connect a výchozím zobrazením příležitostí ke spoluprodeji v Partnerské centrum" lightbox="images/pscmigration/home-page-expanded.png":::

### <a name="2---psc-grid-view-mapped-to-the-partner-center-deal-view"></a>2 . Zobrazení mřížky PSC namapované na Partnerské centrum dohody

Porovnejte odpovídající očíslované kruhy mezi horním snímkem obrazovky PSC a Partnerské centrum snímku obrazovky pod nimi. Odpovídající čísla ukazují, kde můžete najít funkci nebo atribut související s PSC v Partnerské centrum. Červené kruhy označují, že v poli Partnerské centrum žádná shoda.  

> [!NOTE]
> Pod snímky obrazovky se zobrazí další důležité informace.

:::image type="content" source="images/pscmigration/gridview.png" alt-text="Obrázek znázorňující mapování polí mezi zobrazením mřížky Partner Sales Connect (PSC) a zobrazením Partnerské centrum dohody" lightbox="images/pscmigration/grid-view-expanded.png":::

**Zvláštní aspekty:**

- Zobrazení seznamu v tomto Partnerské centrum jako v PSC.  Všechny dohody jsou uvedené na základě nejnovějšího přijatého nebo vytvořeného data s informacemi o zákazníkovi a typem dohody. Ve výchozím nastavení je vybrána první dohoda v zobrazení. Většina hodnot zobrazených ve formátu tabulky PSC je k dispozici v podrobném zobrazení dohody v PC.
- Role dohody není povinné pole v počítači. Nezobrazuje se ani se nezachycuje v žádném z pracovních postupů. Je odvozená automaticky na straně prodejce Microsoftu na základě řešení přidaných do obchodu.
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
- V počítači není vyžadován licenční program. Tyto informace se automaticky odvodí na základě řešení vybraných v obchodě.

>[!Note]
>Žádnou dohodu označenou jako won (vyhrála) nebo ztracenou (lost) není možné upravit. Při přesunu dohody do jednoho z těchto terminálových stavů buďte opatrní.

### <a name="4---psc-add-products-view-mapped-to-the-partner-center-add-solutions-view"></a>4. Zobrazení PsC Přidat produkty namapované na Partnerské centrum zobrazení Přidat řešení

Porovnejte odpovídající očíslované kruhy na horním snímku obrazovky (PSC) s Partnerské centrum snímku obrazovky pod ním. Odpovídající čísla ukazují, kde můžete najít funkci nebo atribut související s PSC v Partnerské centrum. Červené kroužky označují, že v seznamu není žádné odpovídající pole nebo Partnerské centrum.
  
:::image type="content" source="images/pscmigration/products.png" alt-text="Obrázek znázorňující mapování polí mezi zobrazením Přidání produktů v nástroji Partner Sales Connect (PSC) a Partnerské centrum zobrazení pro přidání řešení" lightbox="images/pscmigration/products-expanded.png":::

### <a name="5---user-management-in-psc-versus-partner-center"></a>5. Správa uživatelů v PSC versus Partnerské centrum

Porovnejte odpovídající očíslované kruhy na horním snímku obrazovky (PSC) s Partnerské centrum snímku obrazovky pod ním. Odpovídající čísla ukazují, kde můžete najít funkci nebo atribut související s PSC v Partnerské centrum. Červené kroužky označují, že v seznamu není žádné odpovídající pole nebo Partnerské centrum.  

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="Obrázek znázorňující mapování polí mezi domovskou stránkou pro správu uživatelů Partner Sales Connect (PSC) a zobrazením stránky pro správu Partnerské centrum uživatele v oblasti Nastavení účtu."  lightbox="images/pscmigration/user-management-expanded.png":::

### <a name="6---user-role-assignment-in-psc-versus-partner-center"></a>6. Přiřazení role uživatele v PSC v porovnání s Partnerské centrum

Porovnejte odpovídající očíslované kruhy na horním snímku obrazovky (PSC) s Partnerské centrum snímku obrazovky pod ním. Odpovídající čísla ukazují, kde můžete najít funkci nebo atribut související s PSC v Partnerské centrum. Červené kroužky označují, že v seznamu není žádné odpovídající pole nebo Partnerské centrum.  

:::image type="content" source="images/pscmigration/roles.png" alt-text="Obrázek znázorňující mapování polí mezi zobrazením přiřazení role Partner Sales Connect (PSC) a zobrazením přiřazení Partnerské centrum role" lightbox="images/pscmigration/roles-expanded.png":::

**Zvláštní aspekty:**

- Ekvivalentní rolí pro správce PSC je role správce účtu v Partnerské centrum.
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

### <a name="3---the-new-deal-button-is-greyed-out-for-our-account-what-should-i-do-to-start-creating-deals"></a>3 – tlačítko + nové koupě je pro náš účet šedé. Co mám udělat, když mám začít vytvářet dohody?

K tomu dochází pouze v případě, že k organizaci MPN, kterou používáte v rámci programu , nejsou připojená žádná řešení připravená ke spoluprodávce Partnerské centrum. Obraťte se na váš pdm a získejte ID MPN vašich řešení opravené nebo vytvořte lístek podpory s informací o problému "Po migraci PSC je tlačítko Nové dohody zašedé".

### <a name="4---can-i-assign-deals-to-a-specific-person-from-our-organization-like-psc"></a>4 – Můžu přiřadit dohody konkrétní osobě z naší organizace, jako je PSC?

Ke konkrétní dohody můžete přiřadit členy týmu. Nezablokuje ostatním správcům referenčních nabídek jejich zobrazení ani akce s těmito obchody.

### <a name="5---is-there-a-view-of-all-the-deals-assigned-to-me"></a>5 – Je k dispozici zobrazení všech dohod, které mi byly přiřazeny?

Můžete použít funkci oblíbených položek, což je karta na úrovni uživatele. Všechny dohody, které jsou vám přiřazeny, můžete označit jako oblíbené a získat tak rychlý přístup k dohodám.

### <a name="6---is-there-a-read-only-view-for-the-deals"></a>6 – Existuje pro dohody zobrazení jen pro čtení?

Ne, v části referenčních nabídek není k dispozici žádné zobrazení dohod jen pro čtení. Všichni správci referenčních seznamů budou mít ke všem dohodám úplný přístup pro čtení a zápis.

### <a name="7---how-can-i-register-a-deal-after-marking-it-as-won"></a>7 – Jak můžu zaregistrovat dohodu po označení dohody jako won?

Pokud dohoda splňuje následující kritéria, zobrazí se automaticky otevírané okno pro zahájení [registrace dohody.](./register-deals.md)

- K dohody je připojené řešení s nárokem na pobídky.
- Prodejce Microsoftu je pozvaný k účasti v dohody nebo vás k ní pozve.
- Karta Microsoft je ve stavu Přijato nebo Partnerské centrum.

### <a name="8---i-get-an-error-message-when-i-select-the-new-deal-registration-button-in-the-deal-registration-section-how-can-i-register-my-deals"></a>8 – Když v části Registrace dohody vyberu tlačítko +Nová registrace dohody, zobrazí se chybová zpráva. Jak můžu zaregistrovat své dohody?

Tlačítko **+Nová registrace** dohody mají používat jenom partneři zaregistrovaní v programu ISV Connect k registraci dohody bez odpovídající příležitosti ke spoluprodávce v Partnerské centrum. Při registraci dohod s příležitostí ke spoluprodávce se při označení dohody jako won zobrazí automaticky otevírané okno, které splňuje kritéria pro registraci dohody.

### <a name="9---is-adding-a-customer-organization-mandatory"></a>9 – je nutné přidat organizaci zákazníka povinnou?

Ano, v partnerském centru je přidání [organizace zákazníka](./manage-co-sell-opportunities.md#select-your-customer) povinné. Začněte tím, že vyhledáte umístění, kde se zákazník nachází. Na základě podrobností, které máte; můžete být specifické, včetně přesného názvu budovy, nebo jenom poskytnout podrobnosti o městech. Hledání v organizaci načte všechny platné entity, které odpovídají názvu, který zadáte, abyste nemuseli zadávat žádné podrobnosti o adrese. Všechny podrobnosti se vyplní automaticky na základě vybrané organizace.

### <a name="10---are-customer-contact-details-mandatory"></a>10 jsou povinnými kontaktními údaji zákazníka?

Závisí na [typu obchodu](./manage-co-sell-opportunities.md#types-of-co-sell-opportunities) , kterou vytváříte. Pokud sdílíte svůj kanál a nevyžadujete žádnou technickou podporu z prodejní organizace Microsoftu, můžete se rozhodnout nedávat kontaktní údaje od zákazníka. Pokud společně vydáváte, kde aktivně hledáte pomocníka od společnosti Microsoft, budete muset zadat kontaktní údaje zákazníka. Před vytvořením žádosti o společný prodej v partnerském centru byste měli získat výslovný souhlas od zákazníka.

### <a name="11---how-many-solutions-can-i-add-to-a-deal"></a>11 – kolik řešení mohu do obchodu přidat?

Do obchodu můžete přidat až 50 řešení (podobných produktům v PBV). Na rozdíl od PSC můžete kombinovat řešení ze svých vlastních řešení vhodných pro vlastní prodej, SKU Microsoft First stran a dalších oprávněných řešení pro vlastní prodej třetích stran. V partnerském centru neexistuje žádná role koupě, která by se měla vybrat nebo k dispozici. U položek SKU společnosti Microsoft můžete volitelně přidat množství a cenu za každou SKU, která je do obchodu přidána.

### <a name="12---when-will-i-get-to-know-the-microsoft-seller-details-after-creating-a-deal"></a>12. po vytvoření obchodu se dozvíte o podrobnostech o prodejci Microsoftu?

Prodejci Microsoftu se přiřazují až po splnění přesného požadavku na podporu, který jste uvedli při vytváření obchodu s relevantním prodejcem na straně Microsoftu. I po přiřazení budou mít prodejci Microsoftu možnost přijmout nebo odmítnout pozvánku pro spoluprodej. V případě, že prodávající akceptuje pozvání k spoluprodeji, bude aktualizace aktualizována o kontaktní údaje prodejce Microsoftu. Smlouva SLA pro prodejce Microsoftu, kteří se dohodu dohodí, je 14 dnů. Jedná se o stejnou smlouvu SLA, kterou partneři musí na základě dohody jednat, než přejde do stavu vypršení platnosti.

### <a name="13---where-can-i-find-the-opportunity-id"></a>13 – Kde najdu ID příležitosti?

ID příležitosti v PSC je stejné jako ID dohody v PC. ID dohody najdete při otevření dohody vedle názvu dohody.

### <a name="14---how-can-my-pdm-get-access-to-pc"></a>14. Jak může můj pdm získat přístup k počítači?

Partnerské centrum přímo na rozdíl od PSC k primárním řadičům domény, k nimž nelze přistupovat. Tuto funkci můžete povolit několika možnostmi, které jsou uvedené níže.

- Přehledy OCP – Pokud si primární počítače jen prohlíhá obchody a průběh, které s nimi souvisejí, mohou k zobrazení vaší organizace použít portál OCP Insights. Jedná se o interní nástroj, který je k dispozici pouze pro pdmy. Upozorňujeme, že přehledy OCP nejsou k dispozici pro uživatele vaší společnosti.
- Uživatel hosta v Partnerské centrum – V Partnerském centru můžete přidat svůj účet PDM jako uživatele hosta a přiřadit mu roli správce referenčních seznamu, aby si mohli zobrazit referenční odkazy a úlohu @microsoft.com s nimi stoupit.
- Vytvoření nového uživatele ve vašem tenantovi – Můžete vytvořit nového uživatele ve vlastním tenantovi [a](./create-user-accounts-and-set-permissions.md#add-a-new-user) tyto podrobnosti sdílet s PDM, aby mohl zobrazit referenční seznam podobný ostatním uživatelům referenčních seznamu ve vašem účtu a jednat s ním.

## <a name="finding-the-correct-mpn-id-if-your-account-in-psc-is-not-associated-with-a-valid-mpn"></a>Vyhledání správného ID MPN, pokud váš účet v PSC není přidružený k platnému MPN

Pokud jste tady, protože jste v PSC viděli banner se zmínkou o problému s neplatným přidružením ID MPN v PSC, jste na správném místě. Váš účet mohl být propojený s neplatným ID MPN z následujících důvodů:

- Vaše společnost nemá Partnerské centrum účet.
- Váš PDM udělal chybu při zadávání ID MPN vašeho účtu v interních systémech, které propojují váš účet PSC s vaším Partnerské centrum účtem (MPNID).
- Vaše společnost dokončila migraci z Partner Membership Center (PMC) do PC.

Nejprve pomocí následujících kroků vyhledejte správné ID MPN.

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
|Zaregistrujte obchody, které jste vyhráli v partnerském centru |[Registrace nové dohody](./register-deals.md)
|Získejte přehledy referenčních seznamu a zjistěte, jak si vaše referenční reference vede. |[Přehledy referenčních seznamů](./referral-insights.md)
|Vytvoření a správa obchodního profilu|[Správa obchodního profilu](./create-a-marketing-profile.md)
|Správa potenciálních zákazníků pro obchodní profil |[Správa potenciálních zákazníků](./manage-leads.md)|

## <a name="next-steps"></a>Další kroky


- [Partner Sales Connect to Partnerské centrum sešit](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) – sešit pro sladění prodejních procesů a rolí partnerů s novými prodejními procesy prostřednictvím Partnerské centrum vs. Partner Sales Connect.
- [Partnerské centrum provozního průvodce](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) spoluprodálováním – pokyny k identifikaci provozního modelu prostřednictvím Partnerské centrum pro správu potenciálních zákazníků nebo příležitostí ke spoluprodání a registraci dohod.
- [Balíček pro správu referenčních](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) doporučení – vizualizované podrobné pokyny ke správě potenciálních zákazníků a příležitostí ke spoluprodání prostřednictvím Partnerské centrum.
- [Publikování](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) a správa na komerčním marketplace – vizualizované podrobné pokyny k vytváření, správě a publikování nabídek prostřednictvím Partnerské centrum na komerčním marketplace.